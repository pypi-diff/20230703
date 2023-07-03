# Comparing `tmp/deciphon_snap-0.1.2.tar.gz` & `tmp/deciphon_snap-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon_snap-0.1.2.tar", max compression
+gzip compressed data, was "deciphon_snap-0.2.0.tar", max compression
```

## Comparing `deciphon_snap-0.1.2.tar` & `deciphon_snap-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-06-21 09:49:04.100190 deciphon_snap-0.1.2/LICENSE
--rw-r--r--   0        0        0     2453 2023-06-21 09:49:04.100190 deciphon_snap-0.1.2/README.md
--rw-r--r--   0        0        0      275 2023-06-21 09:49:04.100190 deciphon_snap-0.1.2/deciphon_snap/hit.py
--rw-r--r--   0        0        0      607 2023-06-21 09:49:04.100190 deciphon_snap-0.1.2/deciphon_snap/match.py
--rw-r--r--   0        0        0     1008 2023-06-21 09:49:04.100190 deciphon_snap-0.1.2/deciphon_snap/match_list.py
--rw-r--r--   0        0        0       72 2023-06-21 09:49:04.100190 deciphon_snap-0.1.2/deciphon_snap/path_like.py
--rw-r--r--   0        0        0      265 2023-06-21 09:49:04.100190 deciphon_snap-0.1.2/deciphon_snap/prod.py
--rw-r--r--   0        0        0      360 2023-06-21 09:49:04.100190 deciphon_snap-0.1.2/deciphon_snap/prod_list.py
--rw-r--r--   0        0        0      251 2023-06-21 09:49:04.100190 deciphon_snap-0.1.2/deciphon_snap/read_snap.py
--rw-r--r--   0        0        0      436 2023-06-21 09:49:04.100190 deciphon_snap-0.1.2/deciphon_snap/shorten.py
--rw-r--r--   0        0        0     2010 2023-06-21 09:49:04.100190 deciphon_snap-0.1.2/deciphon_snap/snap_file.py
--rw-r--r--   0        0        0      157 2023-06-21 09:49:04.100190 deciphon_snap-0.1.2/deciphon_snap/stringify.py
--rw-r--r--   0        0        0      521 2023-06-21 09:49:04.100190 deciphon_snap-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3055 1970-01-01 00:00:00.000000 deciphon_snap-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2453 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/README.md
+-rw-r--r--   0        0        0      355 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/amino.py
+-rw-r--r--   0        0        0     1564 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/hit.py
+-rw-r--r--   0        0        0     2178 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/hmmer.py
+-rw-r--r--   0        0        0     2680 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/interval.py
+-rw-r--r--   0        0        0     2773 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/match.py
+-rw-r--r--   0        0        0       72 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/path_like.py
+-rw-r--r--   0        0        0      913 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/prod.py
+-rw-r--r--   0        0        0      724 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/query_interval.py
+-rw-r--r--   0        0        0      347 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/read_snap.py
+-rw-r--r--   0        0        0      570 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/shorten.py
+-rw-r--r--   0        0        0     2495 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/snap_file.py
+-rw-r--r--   0        0        0      157 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/deciphon_snap/stringify.py
+-rw-r--r--   0        0        0      541 2023-07-03 09:47:58.832892 deciphon_snap-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 deciphon_snap-0.2.0/PKG-INFO
```

### Comparing `deciphon_snap-0.1.2/LICENSE` & `deciphon_snap-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.1.2/README.md` & `deciphon_snap-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `deciphon_snap-0.1.2/deciphon_snap/snap_file.py` & `deciphon_snap-0.2.0/deciphon_snap/snap_file.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,70 @@
 from __future__ import annotations
 
-from csv import DictReader
+import csv
 from typing import List
 
 import prettytable as pt
+from h3result.read_h3result import read_h3result
 
-from deciphon_snap.match_list import LazyMatchList
+from deciphon_snap.hmmer import H3Result
+from deciphon_snap.match import LazyMatchList
 from deciphon_snap.prod import Prod
-from deciphon_snap.prod_list import ProdList
+from deciphon_snap.prod import ProdList
 from deciphon_snap.shorten import shorten
 from deciphon_snap.stringify import stringify
 
 __all__ = ["SnapFile"]
 
+csv.field_size_limit(8388608)
+
 
 class SnapFile:
     def __init__(self, filesystem):
-        self._fs = filesystem
+        fs = filesystem
 
-        files = self._fs.ls("/")
+        files = fs.ls("/", detail=False)
         assert len(files) == 1
 
-        root_dir = files[0]["filename"][:-1]
-        assert self._fs.isdir(root_dir)
+        root_dir = files[0].rstrip("/")
+        assert fs.isdir(root_dir)
         prod_file = f"{root_dir}/products.tsv"
 
-        with self._fs.open(prod_file, "rb") as file:
-            self._prods = read_products(file)
+        hmmer_dir = f"{root_dir}/hmmer"
+        assert fs.isdir(hmmer_dir)
+
+        with fs.open(prod_file, "rb") as file:
+            prods: List[Prod] = []
+            reader = csv.DictReader((stringify(x) for x in file), delimiter="\t")
+            for idx, row in enumerate(reader):
+                seq_id = int(row["seq_id"])
+                profile = str(row["profile"])
+                with fs.open(f"{hmmer_dir}/{seq_id}/{profile}.h3r", "rb") as f2:
+                    h3r = H3Result(raw=read_h3result(fileno=f2.fileno()))
+                prods.append(
+                    Prod(
+                        id=idx,
+                        seq_id=seq_id,
+                        profile=profile,
+                        abc=str(row["abc"]),
+                        alt=float(row["alt"]),
+                        null=float(row["null"]),
+                        evalue=float(row["evalue"]),
+                        match_list=LazyMatchList(raw=str(row["match"])),
+                        h3result=h3r,
+                    )
+                )
+            self._prods = ProdList.model_validate(prods)
 
     @property
     def products(self):
         return self._prods
 
     def __str__(self):
-        fields = list(Prod.schema()["properties"].keys())
+        fields = Prod.__fields__
 
         num_fields = len(fields)
         prods = [[getattr(x, i) for i in fields] for x in self.products]
         num_products = len(prods)
         if num_products >= 10:
             prods = prods[:4] + [["…"] * num_fields] + prods[-4:]
 
@@ -46,25 +73,7 @@
         x.field_names = fields
         x.align = "l"
         for prod in prods:
             x.add_row([shorten(i) for i in prod])
 
         header = f"shape: ({num_products}, {num_fields})"
         return header + "\n" + x.get_string()
-
-
-def read_products(file):
-    prods: List[Prod] = []
-    for i, row in enumerate(DictReader((stringify(i) for i in file), delimiter="\t")):
-        prods.append(
-            Prod(
-                id=i,
-                seq_id=int(row["seq_id"]),
-                profile=str(row["profile"]),
-                abc=str(row["abc"]),
-                alt=float(row["alt"]),
-                null=float(row["null"]),
-                evalue=float(row["evalue"]),
-                match_list=LazyMatchList(raw=str(row["match"])),
-            )
-        )
-    return ProdList.parse_obj(prods)
```

### Comparing `deciphon_snap-0.1.2/PKG-INFO` & `deciphon_snap-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: deciphon-snap
-Version: 0.1.2
+Version: 0.2.0
 Summary: Reader for Deciphon snap files.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fsspec[libarchive] (>=2023.6.0)
+Requires-Dist: fsspec (>=2023.6.0)
+Requires-Dist: h3result (>=0.3.0)
+Requires-Dist: hmmer-tables (>=0.4.0)
 Requires-Dist: prettytable (>=3.8.0)
-Requires-Dist: pydantic (>=1.10.9)
+Requires-Dist: pydantic (>=2.0b3)
 Description-Content-Type: text/markdown
 
 # deciphon-snap
 
 ## Example
 
 ```python
```

