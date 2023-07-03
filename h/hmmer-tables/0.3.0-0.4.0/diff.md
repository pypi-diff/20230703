# Comparing `tmp/hmmer_tables-0.3.0.tar.gz` & `tmp/hmmer_tables-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmmer_tables-0.3.0.tar", max compression
+gzip compressed data, was "hmmer_tables-0.4.0.tar", max compression
```

## Comparing `hmmer_tables-0.3.0.tar` & `hmmer_tables-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/LICENSE
--rw-r--r--   0        0        0       15 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/hmmer_tables/__init__.py
--rw-r--r--   0        0        0      367 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/hmmer_tables/csv_iter.py
--rw-r--r--   0        0        0     3419 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/hmmer_tables/domtbl.py
--rw-r--r--   0        0        0     1885 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/hmmer_tables/interval.py
--rw-r--r--   0        0        0       72 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/hmmer_tables/path_like.py
--rw-r--r--   0        0        0     2131 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/hmmer_tables/tbl.py
--rw-r--r--   0        0        0      441 2023-06-22 00:06:49.605539 hmmer_tables-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 hmmer_tables-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/LICENSE
+-rw-r--r--   0        0        0       15 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/hmmer_tables/__init__.py
+-rw-r--r--   0        0        0      692 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/hmmer_tables/cleanup.py
+-rw-r--r--   0        0        0      367 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/hmmer_tables/csv_iter.py
+-rw-r--r--   0        0        0     3432 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/hmmer_tables/domtbl.py
+-rw-r--r--   0        0        0     1966 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/hmmer_tables/interval.py
+-rw-r--r--   0        0        0     1456 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/hmmer_tables/output.py
+-rw-r--r--   0        0        0       72 2023-07-03 09:28:23.802459 hmmer_tables-0.4.0/hmmer_tables/path_like.py
+-rw-r--r--   0        0        0     7334 2023-07-03 09:28:23.806459 hmmer_tables-0.4.0/hmmer_tables/query.py
+-rw-r--r--   0        0        0     2141 2023-07-03 09:28:23.806459 hmmer_tables-0.4.0/hmmer_tables/tbl.py
+-rw-r--r--   0        0        0      468 2023-07-03 09:28:23.806459 hmmer_tables-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 hmmer_tables-0.4.0/PKG-INFO
```

### Comparing `hmmer_tables-0.3.0/LICENSE` & `hmmer_tables-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.3.0/hmmer_tables/domtbl.py` & `hmmer_tables-0.4.0/hmmer_tables/domtbl.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 class DomTBL(RootModel):
     root: List[DomTBLRow]
 
     def __iter__(self):
         return iter(self.root)
 
-    def __getitem__(self, item):
+    def __getitem__(self, item) -> DomTBLRow:
         return self.root[item]
 
     def __len__(self):
         return len(self.root)
 
 
 def _read_domtbl_stream(stream: Iterable[str]):
```

### Comparing `hmmer_tables-0.3.0/hmmer_tables/interval.py` & `hmmer_tables-0.4.0/hmmer_tables/interval.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,18 +51,22 @@
       `start, start+1, ..., stop-1, stop`.
     """
 
     start: int
     stop: int
 
     def __post_init__(self):
-        if self.start > self.stop:
+        if self.start > self.stop + 1:
             raise ValueError(f"Invalid RInterval({self.start}, {self.stop}).")
 
     def to_pyinterval(self) -> PyInterval:
         return PyInterval(self.start - 1, self.stop)
 
     def to_slice(self) -> slice:
         return self.to_pyinterval().to_slice()
 
     def offset(self, offset: int) -> RInterval:
         return RInterval(self.start + offset, self.stop + offset)
+
+    @property
+    def size(self):
+        return self.stop - self.start + 1
```

### Comparing `hmmer_tables-0.3.0/hmmer_tables/tbl.py` & `hmmer_tables-0.4.0/hmmer_tables/tbl.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 class TBL(RootModel):
     root: List[TBLRow]
 
     def __iter__(self):
         return iter(self.root)
 
-    def __getitem__(self, item):
+    def __getitem__(self, item) -> TBLRow:
         return self.root[item]
 
     def __len__(self):
         return len(self.root)
 
 
 def _read_tbl_stream(stream: Iterable[str]) -> List[TBLRow]:
```

### Comparing `hmmer_tables-0.3.0/PKG-INFO` & `hmmer_tables-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: hmmer-tables
-Version: 0.3.0
+Version: 0.4.0
 Summary: Read tables produced by HMMER software.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: more-itertools (>=9.1.0)
 Requires-Dist: pydantic (>=2.0b3)
 Description-Content-Type: text/markdown
 
 # hmmer-tables
```

