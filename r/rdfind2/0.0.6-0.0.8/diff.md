# Comparing `tmp/rdfind2-0.0.6.tar.gz` & `tmp/rdfind2-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfind2-0.0.6.tar", last modified: Sun May 28 01:35:36 2023, max compression
+gzip compressed data, was "rdfind2-0.0.8.tar", max compression
```

## Comparing `rdfind2-0.0.6.tar` & `rdfind2-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,4 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 01:35:36.635533 rdfind2-0.0.6/
--rw-rw-rw-   0        0        0     1065 2023-05-28 01:35:36.634532 rdfind2-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      684 2023-05-28 01:34:56.000000 rdfind2-0.0.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-28 01:35:36.633531 rdfind2-0.0.6/rdfind2.egg-info/
--rw-rw-rw-   0        0        0     1065 2023-05-28 01:35:36.000000 rdfind2-0.0.6/rdfind2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-28 01:35:36.000000 rdfind2-0.0.6/rdfind2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 01:35:36.000000 rdfind2-0.0.6/rdfind2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-28 01:35:36.000000 rdfind2-0.0.6/rdfind2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-05-28 01:35:36.000000 rdfind2-0.0.6/rdfind2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 01:35:36.000000 rdfind2-0.0.6/rdfind2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7788 2023-05-28 01:33:55.000000 rdfind2-0.0.6/rdfind2.py
--rw-rw-rw-   0        0        0      698 2023-05-28 01:34:39.000000 rdfind2-0.0.6/readme.md
--rw-rw-rw-   0        0        0       42 2023-05-28 01:35:36.635533 rdfind2-0.0.6/setup.cfg
+-rw-r--r--   0        0        0      411 2023-07-03 17:38:35.677176 rdfind2-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    10716 2023-07-03 17:30:37.776172 rdfind2-0.0.8/rdfind2.py
+-rw-r--r--   0        0        0      698 2023-07-03 17:30:37.776172 rdfind2-0.0.8/readme.md
+-rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 rdfind2-0.0.8/PKG-INFO
```

### Comparing `rdfind2-0.0.6/rdfind2.py` & `rdfind2-0.0.8/rdfind2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,37 @@
+from __future__ import annotations
+
 import contextlib
 import dataclasses
 import hashlib
 import io
 import os
-import pathlib
+import sys
 from collections import defaultdict
-from typing import Dict, Iterable, List, Optional, Tuple
+from collections.abc import Iterable
+from pathlib import Path
 
 import click
 from tqdm import tqdm
 
 
 PROGRESS_SIZE = 128 * 1024 * 1024  # 512M
 CHUNK_SIZE = 16 * 1024  # 16k
-PARTIAL_SIZE = 16
+PARTIAL_SIZE = 16  # head/tail size
 SMALL_FILE_THRESHOLD = 256 * 1024 * 1024  # 256 mb
 
 
 @dataclasses.dataclass
 class Entry:
-    path: pathlib.Path
+    path: Path
     size: int
+    idev: int
     inode: int
 
-    head_middle_and_tail: Tuple[bytes, bytes, bytes] = None
-
-    b2sum: Optional[str] = None
+    head_middle_and_tail: tuple[bytes, bytes, bytes] = None
 
     @property
     def head(self):
         if self.head_middle_and_tail:
             return self.head_middle_and_tail[0]
         self.head_middle_and_tail = self.read_partial(self.path, self.size)
         return self.head_middle_and_tail[0]
@@ -44,48 +46,75 @@
     @property
     def tail(self):
         if self.head_middle_and_tail:
             return self.head_middle_and_tail[2]
         self.head_middle_and_tail = self.read_partial(self.path, self.size)
         return self.head_middle_and_tail[2]
 
-    def calculate_b2sum(self):
+    def unsafe_b2sum(self, factory: int) -> str:
+        h = hashlib.blake2b()
+        step = 16 * 1024 * 1024
+
+        with (
+            self.path.open("rb") as f,
+            tqdm(
+                total=self.size,
+                ascii=True,
+                unit_scale=True,
+                unit="iB",
+                unit_divisor=1024,
+                mininterval=1,
+                position=1,
+                leave=False,
+            ) as bar,
+        ):
+            for i in range(0, self.size, step * factory):
+                f.seek(i, io.SEEK_SET)
+                h.update(f.read(step))
+                bar.update(step * factory)
+
+        return h.hexdigest()
+
+    def safe_b2sum(self):
         h = hashlib.blake2b()
 
         with self.open() as f:
+            if sys.platform == "linux":
+                os.posix_fadvise(f.fileno(), 0, self.size, os.POSIX_FADV_SEQUENTIAL)
             while data := f.read(CHUNK_SIZE):
                 h.update(data)
 
-        self.b2sum = h.hexdigest()
-
-        return self.b2sum
+        return h.hexdigest()
 
     @contextlib.contextmanager
     def open(self) -> io.BytesIO:
         if self.size > PROGRESS_SIZE:
-            with self.path.open("rb") as f:
-                with tqdm.wrapattr(
-                        f,
-                        "read",
-                        total=self.size,
-                        ascii=True,
-                        leave=False,
-                        position=1,
-                ) as reader:
-                    yield reader
+            with self.path.open("rb") as f, tqdm.wrapattr(
+                f,
+                "read",
+                total=self.size,
+                ascii=True,
+                leave=False,
+                mininterval=1,
+                position=1,
+                unit="B",
+                unit_scale=True,
+                unit_divisor=1024,
+            ) as reader:
+                yield reader
             return
         with self.path.open("rb") as f:
             yield f
 
     @property
     def check_key(self) -> tuple:
         return self.size, self.head, self.middle, self.tail
 
     @staticmethod
-    def read_partial(p: pathlib.Path, size: int) -> Tuple[bytes, bytes, bytes]:
+    def read_partial(p: Path, size: int) -> tuple[bytes, bytes, bytes]:
         with p.open("rb", buffering=0) as f:
             head = f.read(PARTIAL_SIZE)
             f.seek(size // 2, io.SEEK_SET)
             middle = f.read(PARTIAL_SIZE)
             f.seek(-min(PARTIAL_SIZE, size), io.SEEK_END)
             tail = f.read(PARTIAL_SIZE)
         return head, middle, tail
@@ -94,140 +123,212 @@
 @click.command()
 @click.argument(
     "location",
     required=True,
     nargs=-1,
     type=click.Path(exists=True, file_okay=False, readable=True, resolve_path=True),
 )
-@click.option("--make-hardlink", "hardlink", is_flag=True, default=False,
-              help='used when you search duplicate files in same device')
+@click.option(
+    "--hardlink",
+    is_flag=True,
+    default=False,
+    help="used when you search duplicate files in same device",
+)
 @click.option("--delete", "delete", is_flag=True, default=False)
-@click.option('--file-size-threshold', 'threshold', default=SMALL_FILE_THRESHOLD, type=int)
-def rdfind2(location: Tuple[str], threshold: int, hardlink=False, delete=False):
+@click.option(
+    "--delete-from",
+    "delete_from",
+    type=click.Path(resolve_path=True, path_type=Path),
+    required=False,
+)
+@click.option("--min-file-size", "threshold", default=SMALL_FILE_THRESHOLD, type=int)
+@click.option(
+    "--unsafe",
+    "unsafe",
+    is_flag=False,
+    flag_value=4,
+    type=click.IntRange(min=1),
+    help="unsafe partial fast checksum, check only 1/N content of this file. If pass --unsafe=1, it will works like safe hash",
+)
+@click.option(
+    "-v",
+    "--verbose",
+    count=True,
+    help="increase output level",
+)
+@click.option(
+    "--dry-run",
+    is_flag=True,
+    default=False,
+)
+def rdfind2(
+    location: tuple[str],
+    threshold: int,
+    unsafe: int,
+    verbose: int = 0,
+    hardlink=False,
+    delete=False,
+    dry_run: bool = False,
+    delete_from: Path | None = None,
+):
+    if unsafe is None:
+        unsafe = 0
     if hardlink and delete:
         click.secho("can't use '--make-hardlink' with '--delete'", fg="green", err=True)
+        sys.exit(1)
+    if delete_from is not None:
+        if not delete:
+            click.secho("can't use '--delete-from' without '--delete'", fg="red", err=True)
+            sys.exit(1)
+
+    click.secho("dry run enabled")
+
     group_by_size = dedupe_by_size(location)
 
     if threshold:
         group_by_size = {key: value for key, value in group_by_size.items() if key >= threshold}
 
-    groups: Dict[tuple, List[Entry]] = dedupe_by_head_tail(group_by_size)
+    groups: dict[tuple, list[Entry]] = dedupe_by_head_tail(group_by_size)
 
-    entry_groups: List[List[Entry]] = []
+    entry_groups: list[list[Entry]] = []
 
     for _, headGroups in sorted(groups.items(), reverse=True):
         if len(headGroups) == 1:
             continue
 
         entry_groups.append(headGroups)
 
-    click.secho("check file hashed", fg='cyan')
+    click.secho("check file hashed", fg="cyan")
     for entry_group in tqdm(entry_groups, ascii=True, position=0):
-        entry_grouped = compare_groups(entry_group)
+        entry_grouped = compare_groups(entry_group, unsafe=unsafe, verbose=verbose)
         for g in entry_grouped:
             if len(g) == 1:
                 continue
 
+            g.sort(key=lambda x: [len(p := x.path.as_posix()), p])
+
             if hardlink:
+                if len({x.idev for x in g}) != 1:
+                    click.secho("can't use --hardlink flag with multiple filesystem")
+                    sys.exit(1)
                 tqdm.write("link files:")
+                link_src = g.pop(0)
+                tqdm.write(click.style(f"{link_src.path!s}", fg="green"))
 
-                link_src = g.pop()
-                tqdm.write(click.style(f"hard link target file {link_src.path!s}", fg="green"))
                 for file in g:
                     tqdm.write(click.style(f"{file.path!s}", fg="red"))
 
                 for file in g:
                     if link_src.inode == file.inode:
                         continue
                     if file.path.name.endswith(".rdfind2.old"):
                         tqdm.write(click.style(f"find internal temp file {file.path!s}", fg="red"))
                         continue
-                    temp_file_path = pathlib.Path(
-                        file.path.with_name(file.path.name + ".rdfind2.old")
-                    )
+                    if dry_run:
+                        continue
+                    temp_file_path = Path(file.path.with_name(file.path.name + ".rdfind2.old"))
                     file.path.rename(temp_file_path)
                     os.link(src=link_src.path, dst=file.path)
                     temp_file_path.unlink()
 
             elif delete:
-                link_src = g.pop()
-                tqdm.write(click.style(f"keep file {link_src.path}", fg="green"))
-                for file in g:
+                if delete_from:
+                    keep = [x for x in g if not x.path.is_relative_to(delete_from)]
+                    if keep:
+                        remove = [x for x in g if x.path.is_relative_to(delete_from)]
+                    else:
+                        remove = g[1:]
+                    for f in keep:
+                        tqdm.write(click.style(f"keep file {f.path}", fg="green"))
+                else:
+                    keep = g.pop(0)
+                    remove = g
+                    tqdm.write(click.style(f"keep file {keep.path}", fg="green"))
+                for file in remove:
                     Stat.deleted += file.size
                     tqdm.write(click.style(f"remove file {file.path}", fg="red"))
-                    os.unlink(file.path)
+                    if not dry_run:
+                        os.unlink(file.path)
             else:
                 tqdm.write(tqdm.format_sizeof(g[0].size, suffix="B", divisor=1024))
-                for entry in sorted(g, key=lambda x: x.path):
+                for entry in g:
                     tqdm.write(str(entry.path))
 
     print("hashed file size:", format_size(Stat.hashed))
     if delete:
         print("deleted file size:", format_size(Stat.deleted))
 
 
-def dedupe_by_size(locations: Iterable[str]) -> Dict[int, List[Entry]]:
-    group_by_size: Dict[int, List[Entry]] = defaultdict(list)
+def dedupe_by_size(locations: Iterable[str]) -> dict[int, list[Entry]]:
+    group_by_size: dict[int, list[Entry]] = defaultdict(list)
 
     with tqdm(desc="get all files", ascii=True) as bar:
         for locate in locations:
             for top, _, files in os.walk(locate):
-                t = pathlib.Path(top).absolute()
+                t = Path(top).absolute()
                 for file in files:
                     bar.update()
                     p = t.joinpath(file)
+                    if p.is_symlink():
+                        continue
                     stat = p.stat()
                     size = stat.st_size
                     group_by_size[size].append(
-                        Entry(path=p, size=size, inode=stat.st_ino)
+                        Entry(path=p, size=size, idev=stat.st_dev, inode=stat.st_ino)
                     )
 
     return {key: value for key, value in group_by_size.items() if len(value) > 1}
 
 
 def dedupe_by_head_tail(
-        group_by_size: Dict[Tuple[int], List[Entry]]
-) -> Dict[Tuple[int, bytes, bytes], List[Entry]]:
-    groups: Dict[Tuple[int, bytes, bytes], List[Entry]] = defaultdict(list)
+    group_by_size: dict[tuple[int], list[Entry]]
+) -> dict[tuple[int, bytes, bytes], list[Entry]]:
+    groups: dict[tuple[int, bytes, bytes], list[Entry]] = defaultdict(list)
     total = sum(len(x) for x in group_by_size.values())
 
     with tqdm(
-            total=total,
-            desc="dedupe by file head/tail",
-            ascii=True,
+        total=total,
+        desc="dedupe by file head/tail",
+        ascii=True,
     ) as bar:
         for _, sizeGroups in sorted(group_by_size.items()):
             for e in sizeGroups:
                 bar.update()
                 groups[e.check_key].append(e)
 
     return groups
 
 
 class Stat:
     hashed = 0
     deleted = 0
 
 
-def compare_groups(group: List[Entry]) -> List[List[Entry]]:
-    inode_group: Dict[int, List[Entry]] = defaultdict(list)
+def compare_groups(group: list[Entry], unsafe: int, verbose: int) -> list[list[Entry]]:
+    inode_group: dict[tuple[int, int], list[Entry]] = defaultdict(list)
     for e in group:
-        inode_group[e.inode].append(e)
+        inode_group[(e.idev, e.inode)].append(e)
 
     if len(inode_group) == 1:
         return []
 
-    hash_map: Dict[int, str] = {}
-    for inode, files in inode_group.items():
-        Stat.hashed += files[0].size
-        hash_map[inode] = files[0].calculate_b2sum()
+    hash_map: dict[tuple[int, int], str] = {}
+    for key, files in inode_group.items():
+        file = files[0]
+        Stat.hashed += file.size
+        if verbose:
+            tqdm.write(f"hashing file {file.path!r}")
+        if unsafe > 1 and file.size >= 512 * 1024**2:
+            hash_map[key] = file.unsafe_b2sum(unsafe)
+        else:
+            hash_map[key] = file.safe_b2sum()
 
     result = defaultdict(list)
     for e in group:
-        hash = hash_map[e.inode]
+        hash = hash_map[(e.idev, e.inode)]
         result[hash].append(e)
 
     return list(result.values())
 
 
 def format_size(n: int):
     return tqdm.format_sizeof(n, "B", divisor=1024)
```

### Comparing `rdfind2-0.0.6/readme.md` & `rdfind2-0.0.8/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 
 ## Usage:
 
 ```shell
 rdfind2 [--file-size-threshold=268435456] [--make-hardlink --delete] ./dir1 ./dir2 ...directory
 ```
 
-(268435456 is 256mb)
+(268435456 is 256MB)
```

