# Comparing `tmp/ms2rescore-3.0.0.dev2.tar.gz` & `tmp/ms2rescore-3.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms2rescore-3.0.0.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ms2rescore-3.0.0.dev3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ms2rescore-3.0.0.dev2.tar` & `ms2rescore-3.0.0.dev3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-06-29 16:23:22.112024 ms2rescore-3.0.0.dev2/LICENSE
--rw-r--r--   0        0        0    11395 2023-06-29 16:23:22.112024 ms2rescore-3.0.0.dev2/README.md
--rw-r--r--   0        0        0      376 2023-06-29 16:23:22.852054 ms2rescore-3.0.0.dev2/ms2rescore/__init__.py
--rw-r--r--   0        0        0     1346 2023-06-29 16:23:22.852054 ms2rescore-3.0.0.dev2/ms2rescore/__main__.py
--rw-r--r--   0        0        0     6817 2023-06-29 16:23:22.852054 ms2rescore-3.0.0.dev2/ms2rescore/config_parser.py
--rw-r--r--   0        0        0      428 2023-06-29 16:23:22.852054 ms2rescore-3.0.0.dev2/ms2rescore/exceptions.py
--rw-r--r--   0        0        0      415 2023-06-29 16:23:22.852054 ms2rescore-3.0.0.dev2/ms2rescore/feature_generators/__init__.py
--rw-r--r--   0        0        0     9563 2023-06-29 16:23:22.852054 ms2rescore-3.0.0.dev2/ms2rescore/feature_generators/deeplc.py
--rw-r--r--   0        0        0    14146 2023-06-29 16:23:22.852054 ms2rescore-3.0.0.dev2/ms2rescore/feature_generators/intensity.py
--rw-r--r--   0        0        0     5472 2023-06-29 16:23:22.852054 ms2rescore-3.0.0.dev2/ms2rescore/feature_generators/maxquant.py
--rw-r--r--   0        0        0    33210 2023-06-29 16:23:22.852054 ms2rescore-3.0.0.dev2/ms2rescore/gui.py
--rw-r--r--   0        0        0     6103 2023-06-29 16:23:22.852054 ms2rescore-3.0.0.dev2/ms2rescore/ms2rescore_main.py
--rw-r--r--   0        0        0        0 2023-06-29 16:23:22.852054 ms2rescore-3.0.0.dev2/ms2rescore/package_data/__init__.py
--rw-r--r--   0        0        0      778 2023-06-29 16:23:22.852054 ms2rescore-3.0.0.dev2/ms2rescore/package_data/config_default.json
--rw-r--r--   0        0        0     6239 2023-06-29 16:23:22.852054 ms2rescore-3.0.0.dev2/ms2rescore/package_data/config_schema.json
--rw-r--r--   0        0        0        0 2023-06-29 16:23:22.852054 ms2rescore-3.0.0.dev2/ms2rescore/package_data/img/__init__.py
--rw-r--r--   0        0        0 44669194 2023-06-29 16:23:22.932057 ms2rescore-3.0.0.dev2/ms2rescore/package_data/img/config_icon.png
--rw-r--r--   0        0        0     4837 2023-06-29 16:23:22.932057 ms2rescore-3.0.0.dev2/ms2rescore/package_data/img/github-mark-white.png
--rw-r--r--   0        0        0     5557 2023-06-29 16:23:22.932057 ms2rescore-3.0.0.dev2/ms2rescore/package_data/img/github-mark.png
--rw-r--r--   0        0        0    52066 2023-06-29 16:23:22.932057 ms2rescore-3.0.0.dev2/ms2rescore/package_data/img/ms2rescore_logo.png
--rw-r--r--   0        0        0    43034 2023-06-29 16:23:22.932057 ms2rescore-3.0.0.dev2/ms2rescore/package_data/img/program_icon.ico
--rw-r--r--   0        0        0     4514 2023-06-29 16:23:22.932057 ms2rescore-3.0.0.dev2/ms2rescore/package_data/ms2rescore-gui-theme.json
--rw-r--r--   0        0        0     1420 2023-06-29 16:23:22.932057 ms2rescore-3.0.0.dev2/ms2rescore/parse_mgf.py
--rw-r--r--   0        0        0    33752 2023-06-29 16:23:22.932057 ms2rescore-3.0.0.dev2/ms2rescore/plotting.py
--rw-r--r--   0        0        0      407 2023-06-29 16:23:22.932057 ms2rescore-3.0.0.dev2/ms2rescore/rescoring_engines/__init__.py
--rw-r--r--   0        0        0     3671 2023-06-29 16:23:22.932057 ms2rescore-3.0.0.dev2/ms2rescore/rescoring_engines/percolator.py
--rw-r--r--   0        0        0     1082 2023-06-29 16:23:22.932057 ms2rescore-3.0.0.dev2/ms2rescore/setup_logging.py
--rw-r--r--   0        0        0     2667 2023-06-29 16:23:22.932057 ms2rescore-3.0.0.dev2/ms2rescore/utils.py
--rw-r--r--   0        0        0     2248 2023-06-29 16:23:22.932057 ms2rescore-3.0.0.dev2/pyproject.toml
--rw-r--r--   0        0        0    13553 1970-01-01 00:00:00.000000 ms2rescore-3.0.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-03 13:55:14.930067 ms2rescore-3.0.0.dev3/LICENSE
+-rw-r--r--   0        0        0    11395 2023-07-03 13:55:14.930067 ms2rescore-3.0.0.dev3/README.md
+-rw-r--r--   0        0        0      376 2023-07-03 13:55:15.810142 ms2rescore-3.0.0.dev3/ms2rescore/__init__.py
+-rw-r--r--   0        0        0     1346 2023-07-03 13:55:15.810142 ms2rescore-3.0.0.dev3/ms2rescore/__main__.py
+-rw-r--r--   0        0        0     6817 2023-07-03 13:55:15.810142 ms2rescore-3.0.0.dev3/ms2rescore/config_parser.py
+-rw-r--r--   0        0        0      428 2023-07-03 13:55:15.810142 ms2rescore-3.0.0.dev3/ms2rescore/exceptions.py
+-rw-r--r--   0        0        0      415 2023-07-03 13:55:15.810142 ms2rescore-3.0.0.dev3/ms2rescore/feature_generators/__init__.py
+-rw-r--r--   0        0        0     9563 2023-07-03 13:55:15.810142 ms2rescore-3.0.0.dev3/ms2rescore/feature_generators/deeplc.py
+-rw-r--r--   0        0        0    14146 2023-07-03 13:55:15.810142 ms2rescore-3.0.0.dev3/ms2rescore/feature_generators/intensity.py
+-rw-r--r--   0        0        0     5472 2023-07-03 13:55:15.810142 ms2rescore-3.0.0.dev3/ms2rescore/feature_generators/maxquant.py
+-rw-r--r--   0        0        0    33210 2023-07-03 13:55:15.810142 ms2rescore-3.0.0.dev3/ms2rescore/gui.py
+-rw-r--r--   0        0        0     6103 2023-07-03 13:55:15.810142 ms2rescore-3.0.0.dev3/ms2rescore/ms2rescore_main.py
+-rw-r--r--   0        0        0        0 2023-07-03 13:55:15.810142 ms2rescore-3.0.0.dev3/ms2rescore/package_data/__init__.py
+-rw-r--r--   0        0        0      778 2023-07-03 13:55:15.810142 ms2rescore-3.0.0.dev3/ms2rescore/package_data/config_default.json
+-rw-r--r--   0        0        0     6239 2023-07-03 13:55:15.810142 ms2rescore-3.0.0.dev3/ms2rescore/package_data/config_schema.json
+-rw-r--r--   0        0        0        0 2023-07-03 13:55:15.810142 ms2rescore-3.0.0.dev3/ms2rescore/package_data/img/__init__.py
+-rw-r--r--   0        0        0 44669194 2023-07-03 13:55:15.902150 ms2rescore-3.0.0.dev3/ms2rescore/package_data/img/config_icon.png
+-rw-r--r--   0        0        0     4837 2023-07-03 13:55:15.902150 ms2rescore-3.0.0.dev3/ms2rescore/package_data/img/github-mark-white.png
+-rw-r--r--   0        0        0     5557 2023-07-03 13:55:15.902150 ms2rescore-3.0.0.dev3/ms2rescore/package_data/img/github-mark.png
+-rw-r--r--   0        0        0    52066 2023-07-03 13:55:15.902150 ms2rescore-3.0.0.dev3/ms2rescore/package_data/img/ms2rescore_logo.png
+-rw-r--r--   0        0        0    43034 2023-07-03 13:55:15.902150 ms2rescore-3.0.0.dev3/ms2rescore/package_data/img/program_icon.ico
+-rw-r--r--   0        0        0     4514 2023-07-03 13:55:15.902150 ms2rescore-3.0.0.dev3/ms2rescore/package_data/ms2rescore-gui-theme.json
+-rw-r--r--   0        0        0     1420 2023-07-03 13:55:15.902150 ms2rescore-3.0.0.dev3/ms2rescore/parse_mgf.py
+-rw-r--r--   0        0        0    33752 2023-07-03 13:55:15.902150 ms2rescore-3.0.0.dev3/ms2rescore/plotting.py
+-rw-r--r--   0        0        0      407 2023-07-03 13:55:15.902150 ms2rescore-3.0.0.dev3/ms2rescore/rescoring_engines/__init__.py
+-rw-r--r--   0        0        0     3671 2023-07-03 13:55:15.902150 ms2rescore-3.0.0.dev3/ms2rescore/rescoring_engines/percolator.py
+-rw-r--r--   0        0        0     1082 2023-07-03 13:55:15.902150 ms2rescore-3.0.0.dev3/ms2rescore/setup_logging.py
+-rw-r--r--   0        0        0     2667 2023-07-03 13:55:15.902150 ms2rescore-3.0.0.dev3/ms2rescore/utils.py
+-rw-r--r--   0        0        0     2248 2023-07-03 13:55:15.902150 ms2rescore-3.0.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0    13553 1970-01-01 00:00:00.000000 ms2rescore-3.0.0.dev3/PKG-INFO
```

### Comparing `ms2rescore-3.0.0.dev2/LICENSE` & `ms2rescore-3.0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/README.md` & `ms2rescore-3.0.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/__main__.py` & `ms2rescore-3.0.0.dev3/ms2rescore/__main__.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/config_parser.py` & `ms2rescore-3.0.0.dev3/ms2rescore/config_parser.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/feature_generators/deeplc.py` & `ms2rescore-3.0.0.dev3/ms2rescore/feature_generators/deeplc.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/feature_generators/intensity.py` & `ms2rescore-3.0.0.dev3/ms2rescore/feature_generators/intensity.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/feature_generators/maxquant.py` & `ms2rescore-3.0.0.dev3/ms2rescore/feature_generators/maxquant.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/gui.py` & `ms2rescore-3.0.0.dev3/ms2rescore/gui.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/ms2rescore_main.py` & `ms2rescore-3.0.0.dev3/ms2rescore/ms2rescore_main.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/package_data/config_default.json` & `ms2rescore-3.0.0.dev3/ms2rescore/package_data/config_default.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/package_data/config_schema.json` & `ms2rescore-3.0.0.dev3/ms2rescore/package_data/config_schema.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/package_data/img/config_icon.png` & `ms2rescore-3.0.0.dev3/ms2rescore/package_data/img/config_icon.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/package_data/img/github-mark-white.png` & `ms2rescore-3.0.0.dev3/ms2rescore/package_data/img/github-mark-white.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/package_data/img/github-mark.png` & `ms2rescore-3.0.0.dev3/ms2rescore/package_data/img/github-mark.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/package_data/img/ms2rescore_logo.png` & `ms2rescore-3.0.0.dev3/ms2rescore/package_data/img/ms2rescore_logo.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/package_data/img/program_icon.ico` & `ms2rescore-3.0.0.dev3/ms2rescore/package_data/img/program_icon.ico`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/package_data/ms2rescore-gui-theme.json` & `ms2rescore-3.0.0.dev3/ms2rescore/package_data/ms2rescore-gui-theme.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994736842105263%*

 * *Differences: {"'CTkSwitch'": "{'fg_color': ['#939BA2', '#4A4D50'], delete: ['fg_Color']}"}*

```diff
@@ -291,15 +291,15 @@
         ],
         "button_hover_color": [
             "gray20",
             "gray100"
         ],
         "button_length": 0,
         "corner_radius": 1000,
-        "fg_Color": [
+        "fg_color": [
             "#939BA2",
             "#4A4D50"
         ],
         "progress_color": [
             "#3a7ebf",
             "#1f538d"
         ],
```

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/parse_mgf.py` & `ms2rescore-3.0.0.dev3/ms2rescore/parse_mgf.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/plotting.py` & `ms2rescore-3.0.0.dev3/ms2rescore/plotting.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/rescoring_engines/percolator.py` & `ms2rescore-3.0.0.dev3/ms2rescore/rescoring_engines/percolator.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/setup_logging.py` & `ms2rescore-3.0.0.dev3/ms2rescore/setup_logging.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/ms2rescore/utils.py` & `ms2rescore-3.0.0.dev3/ms2rescore/utils.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/pyproject.toml` & `ms2rescore-3.0.0.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.0.dev2/PKG-INFO` & `ms2rescore-3.0.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2rescore
-Version: 3.0.0.dev2
+Version: 3.0.0.dev3
 Summary: MS²Rescore: Sensitive PSM rescoring with predicted MS² peak intensities and retention times.
 Keywords: MS2Rescore,MS2PIP,DeepLC,Percolator,proteomics,mass spectrometry,peptide identification,rescoring,machine learning
 Author: Ana Sílvia C. Silva, Robbin Bouwmeester, Louise Buur
 Author-email: Ralf Gabriels <ralf@gabriels.dev>, Arthur Declercq <arthur.declercq@ugent.be>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
```

