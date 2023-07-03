# Comparing `tmp/altcos-common-0.0.2.tar.gz` & `tmp/altcos-common-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altcos-common-0.0.2.tar", last modified: Tue Jun 20 09:11:30 2023, max compression
+gzip compressed data, was "altcos-common-1.0.0.tar", last modified: Mon Jul  3 09:46:21 2023, max compression
```

## Comparing `altcos-common-0.0.2.tar` & `altcos-common-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,16 @@
-drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-20 09:11:30.129539 altcos-common-0.0.2/
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)     1070 2023-06-09 09:40:20.000000 altcos-common-0.0.2/LICENSE
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      774 2023-06-20 09:11:30.129539 altcos-common-0.0.2/PKG-INFO
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      326 2023-06-20 08:49:16.000000 altcos-common-0.0.2/README.md
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      630 2023-06-20 09:05:21.000000 altcos-common-0.0.2/pyproject.toml
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)       38 2023-06-20 09:11:30.129539 altcos-common-0.0.2/setup.cfg
-drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-20 09:11:30.128538 altcos-common-0.0.2/src/
-drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-20 09:11:30.128538 altcos-common-0.0.2/src/altcos/
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-09 07:19:00.000000 altcos-common-0.0.2/src/altcos/__init__.py
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      174 2023-06-20 08:49:16.000000 altcos-common-0.0.2/src/altcos/_common.py
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      679 2023-06-20 08:49:16.000000 altcos-common-0.0.2/src/altcos/build.py
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)     7921 2023-06-20 09:01:19.000000 altcos-common-0.0.2/src/altcos/ostree.py
-drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-20 09:11:30.128538 altcos-common-0.0.2/src/altcos_common.egg-info/
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      774 2023-06-20 09:11:30.000000 altcos-common-0.0.2/src/altcos_common.egg-info/PKG-INFO
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      343 2023-06-20 09:11:30.000000 altcos-common-0.0.2/src/altcos_common.egg-info/SOURCES.txt
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)        1 2023-06-20 09:11:30.000000 altcos-common-0.0.2/src/altcos_common.egg-info/dependency_links.txt
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)       10 2023-06-20 09:11:30.000000 altcos-common-0.0.2/src/altcos_common.egg-info/requires.txt
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)        7 2023-06-20 09:11:30.000000 altcos-common-0.0.2/src/altcos_common.egg-info/top_level.txt
-drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-20 09:11:30.128538 altcos-common-0.0.2/tests/
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)     4873 2023-06-09 08:46:37.000000 altcos-common-0.0.2/tests/test_ostree.py
+drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-07-03 09:46:21.425700 altcos-common-1.0.0/
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)     1070 2023-06-09 09:40:20.000000 altcos-common-1.0.0/LICENSE
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      774 2023-07-03 09:46:21.425700 altcos-common-1.0.0/PKG-INFO
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      326 2023-06-20 08:49:16.000000 altcos-common-1.0.0/README.md
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      627 2023-07-03 09:15:53.000000 altcos-common-1.0.0/pyproject.toml
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)       38 2023-07-03 09:46:21.425700 altcos-common-1.0.0/setup.cfg
+drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-07-03 09:46:21.425700 altcos-common-1.0.0/src/
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)     8259 2023-07-03 09:38:24.000000 altcos-common-1.0.0/src/altcos.py
+drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-07-03 09:46:21.425700 altcos-common-1.0.0/src/altcos_common.egg-info/
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      774 2023-07-03 09:46:21.000000 altcos-common-1.0.0/src/altcos_common.egg-info/PKG-INFO
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      271 2023-07-03 09:46:21.000000 altcos-common-1.0.0/src/altcos_common.egg-info/SOURCES.txt
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)        1 2023-07-03 09:46:21.000000 altcos-common-1.0.0/src/altcos_common.egg-info/dependency_links.txt
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)       10 2023-07-03 09:46:21.000000 altcos-common-1.0.0/src/altcos_common.egg-info/requires.txt
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)        7 2023-07-03 09:46:21.000000 altcos-common-1.0.0/src/altcos_common.egg-info/top_level.txt
+drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-07-03 09:46:21.425700 altcos-common-1.0.0/tests/
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)     4861 2023-07-03 09:18:54.000000 altcos-common-1.0.0/tests/test_altcos.py
```

### Comparing `altcos-common-0.0.2/LICENSE` & `altcos-common-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `altcos-common-0.0.2/PKG-INFO` & `altcos-common-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altcos-common
-Version: 0.0.2
+Version: 1.0.0
 Summary: Components for working with altcos
 Author-email: Ivan Pepelyaev <fl0pp5@altlinux.org>
 Project-URL: Homepage, https://github.com/fl0pp5/altcos-common
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `altcos-common-0.0.2/pyproject.toml` & `altcos-common-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "altcos-common"
-version = "0.0.2"
+version = "1.0.0"
 authors = [
     { name = "Ivan Pepelyaev", email = "fl0pp5@altlinux.org" },
 ]
 description = "Components for working with altcos"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -21,8 +21,8 @@
 "Homepage" = "https://github.com/fl0pp5/altcos-common"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
-package-data = { "altcos" = ["*.py"] }
+package-data = { "src" = ["*.py"] }
```

### Comparing `altcos-common-0.0.2/src/altcos/ostree.py` & `altcos-common-1.0.0/src/altcos.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,59 @@
 from __future__ import annotations
 
+import dataclasses
 import datetime
-import os
+import enum
 import pathlib
 
 import gi
 
 gi.require_version("OSTree", "1.0")
 
 from gi.repository import Gio, OSTree
 
-from altcos import _common
 
-
-class OSName(_common.StrEnum):
+class OSName(enum.StrEnum):
     ALTCOS = "altcos"
 
 
-class Arch(_common.StrEnum):
+class Arch(enum.StrEnum):
     X86_64 = "x86_64"
 
 
-class Branch(_common.StrEnum):
+class Branch(enum.StrEnum):
     SISYPHUS = "sisyphus"
     P10 = "p10"
 
 
+@dataclasses.dataclass
 class Stream:
-    def __init__(self,
-                 streams_root: str | os.PathLike,
-                 osname: OSName,
-                 arch: Arch,
-                 branch: Branch,
-                 substream: str | None = None) -> None:
-        self.streams_root = streams_root
-        self.osname = osname
-        self.arch = arch
-        self.branch = branch
-        self.substream = substream
+    streams_root: str
+    osname: OSName
+    arch: Arch
+    branch: Branch
+    name: str | None = None
 
     def base_stream(self) -> Stream:
         """
-        :return: экземпляр "Stream" без поля substream
+        :return: экземпляр "Stream" без поля name
         """
         return Stream(self.streams_root,
                       self.osname,
                       self.arch,
                       self.branch)
 
     def like_ostree_ref(self) -> str:
         """
         :return: строка вида: "altcos/x86_64/p10", "altcos/x86_64/P10/k8s"
         """
-        return str(pathlib.Path(self.osname.value,
-                                self.arch.value,
-                                self.branch.value.title() if self.substream else self.branch.value,
-                                self.substream or ""))
+        return str(pathlib.Path(self.osname,
+                                self.arch,
+                                self.branch.value.title() if self.name else self.branch.value,
+                                self.name or ""))
 
     @classmethod
     def from_ostree_ref(cls, streams_root: str, ref: str) -> Stream:
         """
         :param streams_root: путь до хранилища потоков
         :param ref: ветка вида: "altcos/x86_64/Sisyphus/k8s"
         :return: экземпляр "Stream"
@@ -75,17 +69,17 @@
 
     @property
     def stream_dir(self) -> pathlib.Path:
         """
         :return: корень потока
         """
         return pathlib.Path(self.streams_root,
-                            self.branch.value,
-                            self.arch.value,
-                            self.substream or "")
+                            self.branch,
+                            self.arch,
+                            self.name or "")
 
     @property
     def rootfs_dir(self) -> pathlib.Path:
         """
         :return: путь до хранилища rootfs-образов, полученых при помощи mkimage-profiles
         """
         return self.base_stream().stream_dir.joinpath("rootfs")
@@ -124,15 +118,15 @@
         """
         :return: путь до директории, примонтированной в overlay-режиме
         """
         return self.work_dir.joinpath("merged")
 
 
 class Repository:
-    class Mode(_common.StrEnum):
+    class Mode(enum.StrEnum):
         BARE = "bare"
         ARCHIVE = "archive"
 
     def __init__(self, stream: Stream, mode: Repository.Mode = Mode.BARE) -> None:
         self.stream = stream
         match mode:
             case Repository.Mode.BARE:
@@ -170,34 +164,34 @@
 
 
 class Version:
     def __init__(self,
                  major: int,
                  minor: int,
                  branch: Branch,
-                 substream: str | None = None,
+                 name: str | None = None,
                  date: str | None = None):
         self.major = major
         self.minor = minor
         self.branch = branch
-        self.substream = substream
+        self.name = name
         self.date = date or datetime.datetime.now().strftime("%Y%m%d")
 
     def __str__(self) -> str:
         """
         :return: строка версии вида: "20220101.1.0"
         """
         return f"{self.date}.{self.major}.{self.minor}"
 
     @property
     def full_version(self) -> str:
         """
         :return: строка версии вида: "p10_k8s.20220101.1.0"
         """
-        return f"{self.branch}_{self.substream or 'base'}.{self}"
+        return f"{self.branch}_{self.name or 'base'}.{self}"
 
     @property
     def like_path(self) -> pathlib.Path:
         return pathlib.Path(self.date, str(self.major), str(self.minor))
 
     @classmethod
     def from_str(cls, version: str) -> Version:
@@ -207,21 +201,21 @@
         """
         if len(parts := version.split(".")) != 4:
             raise ValueError(f"Invalid version format \"{version}\".")
 
         if len(prefix := parts[0].split("_")) != 2:
             raise ValueError(f"Invalid version prefix format \"{version}\".")
 
-        [branch, substream] = Branch(prefix[0]), prefix[1]
+        [branch, name] = Branch(prefix[0]), prefix[1]
         [date, major, minor] = parts[1], *map(int, parts[2:])
 
-        if substream == "base":
-            substream = None
+        if name == "base":
+            name = None
 
-        return Version(major, minor, branch, substream, date)
+        return Version(major, minor, branch, name, date)
 
 
 class Commit:
     def __init__(self, repo: Repository, hashsum: str) -> None:
         self.repo = repo
         self.hashsum = hashsum
 
@@ -242,7 +236,49 @@
     def parent(self) -> Commit | None:
         content = self.repo.storage.load_commit(self.hashsum)
         parent_hashsum = OSTree.commit_get_parent(content[1])
 
         return Commit(self.repo, parent_hashsum) \
             if parent_hashsum \
             else None
+
+
+class Platform(enum.StrEnum):
+    QEMU = "qemu"
+    METAL = "metal"
+
+
+class Format(enum.StrEnum):
+    QCOW2 = "qcow2"
+    ISO = "iso"
+    RAW = "raw"
+
+
+@dataclasses.dataclass
+class Artifact:
+    location: str | None = None
+    signature: str | None = None
+    uncompressed: str | None = None
+    uncompressed_signature: str | None = None
+
+
+@dataclasses.dataclass
+class Build:
+    platform: Platform
+    fmt: Format
+    disk: Artifact | None = None
+    kernel: Artifact | None = None
+    initrd: Artifact | None = None
+    rootfs: Artifact | None = None
+
+
+ALLOWED_BUILDS = {
+    Platform.QEMU: {
+        Format.QCOW2,
+    },
+    Platform.METAL: {
+        Format.ISO,
+        Format.RAW,
+    }
+}
+
+
```

### Comparing `altcos-common-0.0.2/src/altcos_common.egg-info/PKG-INFO` & `altcos-common-1.0.0/src/altcos_common.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altcos-common
-Version: 0.0.2
+Version: 1.0.0
 Summary: Components for working with altcos
 Author-email: Ivan Pepelyaev <fl0pp5@altlinux.org>
 Project-URL: Homepage, https://github.com/fl0pp5/altcos-common
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `altcos-common-0.0.2/tests/test_ostree.py` & `altcos-common-1.0.0/tests/test_altcos.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 import pathlib
 import unittest
 
-from altcos import ostree
+import altcos
 
 
 class TestStream(unittest.TestCase):
     SR = "<some-path>" # STREAMS_ROOT
-    VALID_STREAM = ostree.Stream.from_ostree_ref(SR, "altcos/x86_64/sisyphus")
-    VALID_SUBSTREAM = ostree.Stream.from_ostree_ref(SR, "altcos/x86_64/Sisyphus/k8s")
+    VALID_STREAM = altcos.Stream.from_ostree_ref(SR, "altcos/x86_64/sisyphus")
+    VALID_SUBSTREAM = altcos.Stream.from_ostree_ref(SR, "altcos/x86_64/Sisyphus/k8s")
 
     def test_like_ostree_ref(self):
         good = "altcos/x86_64/sisyphus"
         self.assertEqual(good, self.VALID_STREAM.like_ostree_ref())
 
     def test_like_ostree_ref_for_subref(self):
         good = "altcos/x86_64/Sisyphus/k8s"
         self.assertEqual(good, self.VALID_SUBSTREAM.like_ostree_ref())
 
     def test_valid_stream_init_from_ref(self):
         ref = "altcos/x86_64/sisyphus"
         try:
-            ostree.Stream.from_ostree_ref(self.SR, ref)
+            altcos.Stream.from_ostree_ref(self.SR, ref)
         except ValueError as e:
             self.fail(e)
 
     def test_valid_stream_init_from_subref(self):
         ref = "altcos/x86_64/Sisyphus/k8s"
         try:
-            ostree.Stream.from_ostree_ref(self.SR, ref)
+            altcos.Stream.from_ostree_ref(self.SR, ref)
         except ValueError as e:
             self.fail(e)
 
     def test_invalid_stream_init_from_ref(self):
         ref = "altcos/x86_4/branch"
         try:
-            ostree.Stream.from_ostree_ref(self.SR, ref)
+            altcos.Stream.from_ostree_ref(self.SR, ref)
         except ValueError:
             pass
 
     def test_invalid_stream_init_from_subref(self):
         ref = "altcos/x86_65/Lol/k8s"
         try:
-            ostree.Stream.from_ostree_ref(self.SR, ref)
+            altcos.Stream.from_ostree_ref(self.SR, ref)
         except ValueError:
             pass
 
     def test_stream_dir(self):
         good = pathlib.Path(f"{self.SR}/sisyphus/x86_64")
         self.assertEqual(good, self.VALID_STREAM.stream_dir)
 
@@ -101,34 +101,34 @@
         good = pathlib.Path(f"{self.SR}/sisyphus/x86_64/k8s/work/merged")
         self.assertEqual(good, self.VALID_SUBSTREAM.merged_dir)
 
 
 class TestVersion(unittest.TestCase):
     def test_valid_version_init_from_str(self):
         try:
-            ostree.Version.from_str("sisyphus_base.20230101.1.0")
+            altcos.Version.from_str("sisyphus_base.20230101.1.0")
         except ValueError as e:
             self.fail(e)
 
     def test_str(self):
         good = "20230101.1.0"
-        version = ostree.Version.from_str("sisyphus_base.20230101.1.0")
+        version = altcos.Version.from_str("sisyphus_base.20230101.1.0")
         self.assertEqual(good, str(version))
 
     def test_full_version(self):
         good = "sisyphus_base.20230101.1.0"
-        version = ostree.Version.from_str("sisyphus_base.20230101.1.0")
+        version = altcos.Version.from_str("sisyphus_base.20230101.1.0")
         self.assertEqual(good, version.full_version)
 
     def test_full_version_for_subref(self):
         good = "sisyphus_k8s.20230101.1.0"
-        version = ostree.Version.from_str("sisyphus_k8s.20230101.1.0")
+        version = altcos.Version.from_str("sisyphus_k8s.20230101.1.0")
         self.assertEqual(good, version.full_version)
 
     def test_like_path(self):
         good = pathlib.Path("20230101/1/0")
-        version = ostree.Version.from_str("sisyphus_base.20230101.1.0")
+        version = altcos.Version.from_str("sisyphus_base.20230101.1.0")
         self.assertEqual(good, version.like_path)
 
 
 if __name__ == "__main__":
     unittest.main()
```

