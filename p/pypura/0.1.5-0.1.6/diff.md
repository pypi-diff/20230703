# Comparing `tmp/pypura-0.1.5.tar.gz` & `tmp/pypura-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypura-0.1.5.tar", max compression
+gzip compressed data, was "pypura-0.1.6.tar", max compression
```

## Comparing `pypura-0.1.5.tar` & `pypura-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-06-01 02:10:40.536047 pypura-0.1.5/LICENSE
--rw-r--r--   0        0        0       76 2023-06-01 02:10:40.536047 pypura-0.1.5/README.md
--rw-r--r--   0        0        0      747 2023-06-01 02:10:57.236236 pypura-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      251 2023-06-01 02:10:57.236236 pypura-0.1.5/pypura/__init__.py
--rw-r--r--   0        0        0      414 2023-06-01 02:10:40.536047 pypura-0.1.5/pypura/const.py
--rw-r--r--   0        0        0      200 2023-06-01 02:10:40.536047 pypura-0.1.5/pypura/exceptions.py
--rw-r--r--   0        0        0    30567 2023-06-01 02:10:40.536047 pypura-0.1.5/pypura/fragrances.json
--rw-r--r--   0        0        0     6705 2023-06-01 02:10:40.536047 pypura-0.1.5/pypura/pura.py
--rw-r--r--   0        0        0        0 2023-06-01 02:10:40.536047 pypura-0.1.5/pypura/py.typed
--rw-r--r--   0        0        0      803 2023-06-01 02:10:40.536047 pypura-0.1.5/pypura/utils.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 pypura-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-03 16:25:32.832779 pypura-0.1.6/LICENSE
+-rw-r--r--   0        0        0       76 2023-07-03 16:25:32.832779 pypura-0.1.6/README.md
+-rw-r--r--   0        0        0      754 2023-07-03 16:25:56.572957 pypura-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      251 2023-07-03 16:25:56.576957 pypura-0.1.6/pypura/__init__.py
+-rw-r--r--   0        0        0      414 2023-07-03 16:25:32.836779 pypura-0.1.6/pypura/const.py
+-rw-r--r--   0        0        0      200 2023-07-03 16:25:32.836779 pypura-0.1.6/pypura/exceptions.py
+-rw-r--r--   0        0        0    32132 2023-07-03 16:25:32.836779 pypura-0.1.6/pypura/fragrances.json
+-rw-r--r--   0        0        0     6705 2023-07-03 16:25:32.836779 pypura-0.1.6/pypura/pura.py
+-rw-r--r--   0        0        0        0 2023-07-03 16:25:32.836779 pypura-0.1.6/pypura/py.typed
+-rw-r--r--   0        0        0      803 2023-07-03 16:25:32.836779 pypura-0.1.6/pypura/utils.py
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 pypura-0.1.6/PKG-INFO
```

### Comparing `pypura-0.1.5/LICENSE` & `pypura-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypura-0.1.5/pyproject.toml` & `pypura-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pypura"
-version = "0.1.5"
+version = "0.1.6"
 description = "Python package for interacting with Pura smart fragrance diffuser"
 authors = ["Nathan Spencer <natekspencer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 include = ["pypura/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 boto3 = "^1.26.135"
-pycognito = "^2022.12.0"
+pycognito = ">=2022.12,<2024.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
 pydocstyle = "^6.3.0"
```

### Comparing `pypura-0.1.5/pypura/fragrances.json` & `pypura-0.1.6/pypura/fragrances.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9501661129568106%*

 * *Differences: {'insert': "[(2, OrderedDict([('name', 'Dew'), ('type', 'Car Fragrance'), ('sku', 'DEWC'), "*

 * *           "('brand', 'Unify Co.')])), (8, OrderedDict([('name', 'Salt'), ('type', 'Car "*

 * *           "Fragrance'), ('sku', 'SLTC'), ('brand', 'Unify Co.')])), (23, OrderedDict([('name', "*

 * *           "'Apple'), ('type', 'Fragrance'), ('sku', 'ACP'), ('brand', 'Simplicity')])), (24, "*

 * *           "OrderedDict([('name', 'Apple'), ('type', 'Fragrance'), ('sku', 'ACP'), ('brand', "*

 * *           "'Simplicity by Pura')])), (6 […]*

```diff
@@ -8,14 +8,20 @@
     {
         "brand": "Pura",
         "name": "Cucumber & Mint",
         "sku": "CBMC",
         "type": "Car Fragrance"
     },
     {
+        "brand": "Unify Co.",
+        "name": "Dew",
+        "sku": "DEWC",
+        "type": "Car Fragrance"
+    },
+    {
         "brand": "Pura",
         "name": "Fairway Morning",
         "sku": "FQMC",
         "type": "Car Fragrance"
     },
     {
         "brand": "Pura",
@@ -38,14 +44,20 @@
     {
         "brand": "Pura",
         "name": "Red Rock & Amber",
         "sku": "RRAC",
         "type": "Car Fragrance"
     },
     {
+        "brand": "Unify Co.",
+        "name": "Salt",
+        "sku": "SLTC",
+        "type": "Car Fragrance"
+    },
+    {
         "brand": "Bridgewater Candle Company",
         "name": "Sweet Grace",
         "sku": "LWZC",
         "type": "Car Fragrance"
     },
     {
         "brand": "Pura",
@@ -122,14 +134,26 @@
     {
         "brand": "Disney",
         "name": "Anna & Olaf in the Enchanted Forest",
         "sku": "LHT",
         "type": "Fragrance"
     },
     {
+        "brand": "Simplicity",
+        "name": "Apple",
+        "sku": "ACP",
+        "type": "Fragrance"
+    },
+    {
+        "brand": "Simplicity by Pura",
+        "name": "Apple",
+        "sku": "ACP",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Pura",
         "name": "Apple Orchard",
         "sku": "VKN",
         "type": "Fragrance"
     },
     {
         "brand": "Soap & Paper Factory",
@@ -356,26 +380,44 @@
     {
         "brand": "ILLUME",
         "name": "Citrus Crush",
         "sku": "ICC",
         "type": "Fragrance"
     },
     {
+        "brand": "Floral Street",
+        "name": "Citrus Rose",
+        "sku": "CNR",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Unify Co.",
         "name": "Cliff",
         "sku": "CLF",
         "type": "Fragrance"
     },
     {
         "brand": "K. Hall Designs",
         "name": "Cocoa Almond",
         "sku": "CCA",
         "type": "Fragrance"
     },
     {
+        "brand": "Simplicity",
+        "name": "Coconut",
+        "sku": "CNP",
+        "type": "Fragrance"
+    },
+    {
+        "brand": "Simplicity by Pura",
+        "name": "Coconut",
+        "sku": "CNP",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Becki Owens",
         "name": "Coconut Calm",
         "sku": "MZX",
         "type": "Fragrance"
     },
     {
         "brand": "ILLUME",
@@ -392,14 +434,26 @@
     {
         "brand": "Capri Blue",
         "name": "Coconut Santal",
         "sku": "CST",
         "type": "Fragrance"
     },
     {
+        "brand": "Simplicity",
+        "name": "Coffee",
+        "sku": "CFP",
+        "type": "Fragrance"
+    },
+    {
+        "brand": "Simplicity by Pura",
+        "name": "Coffee",
+        "sku": "CFP",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Joya Studio",
         "name": "Copaline",
         "sku": "CPL",
         "type": "Fragrance"
     },
     {
         "brand": "Soap & Paper Factory",
@@ -710,14 +764,26 @@
     {
         "brand": "Caswell-Massey",
         "name": "Honeysuckle",
         "sku": "HYS",
         "type": "Fragrance"
     },
     {
+        "brand": "Simplicity",
+        "name": "Honeysuckle",
+        "sku": "FPP",
+        "type": "Fragrance"
+    },
+    {
+        "brand": "Simplicity by Pura",
+        "name": "Honeysuckle",
+        "sku": "FPP",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Votivo",
         "name": "ICY BLUE PINE",
         "sku": "JYT",
         "type": "Fragrance"
     },
     {
         "brand": "Antica Farmacista",
@@ -842,14 +908,20 @@
     {
         "brand": "Pura",
         "name": "Linens & Surf",
         "sku": "LMU",
         "type": "Fragrance"
     },
     {
+        "brand": "Pura",
+        "name": "Linens & Surf",
+        "sku": "LSP",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Brooklyn Candle Studio",
         "name": "Love Potion",
         "sku": "LPO",
         "type": "Fragrance"
     },
     {
         "brand": "K. Hall Designs",
@@ -1430,14 +1502,20 @@
     {
         "brand": "Becki Owens",
         "name": "Sugar Blossom",
         "sku": "SBM",
         "type": "Fragrance"
     },
     {
+        "brand": "Pura",
+        "name": "Sugared Lemon",
+        "sku": "LEP",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Pure Placid",
         "name": "Summer by the Lake",
         "sku": "SBL",
         "type": "Fragrance"
     },
     {
         "brand": "Unify Co.",
@@ -1550,14 +1628,26 @@
     {
         "brand": "Caswell-Massey",
         "name": "VIC",
         "sku": "CVC",
         "type": "Fragrance"
     },
     {
+        "brand": "Simplicity",
+        "name": "Vanilla",
+        "sku": "VNP",
+        "type": "Fragrance"
+    },
+    {
+        "brand": "Simplicity by Pura",
+        "name": "Vanilla",
+        "sku": "VNP",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Becki Owens",
         "name": "Vanilla Berry",
         "sku": "IFB",
         "type": "Fragrance"
     },
     {
         "brand": "Floral Street",
```

### Comparing `pypura-0.1.5/pypura/pura.py` & `pypura-0.1.6/pypura/pura.py`

 * *Files identical despite different names*

### Comparing `pypura-0.1.5/pypura/utils.py` & `pypura-0.1.6/pypura/utils.py`

 * *Files identical despite different names*

### Comparing `pypura-0.1.5/PKG-INFO` & `pypura-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pypura
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package for interacting with Pura smart fragrance diffuser
 License: MIT
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.135,<2.0.0)
-Requires-Dist: pycognito (>=2022.12.0,<2023.0.0)
+Requires-Dist: pycognito (>=2022.12,<2024.0)
 Description-Content-Type: text/markdown
 
 # pypura
 Python package for interacting with Pura smart fragrance diffusers
```

