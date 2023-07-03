# Comparing `tmp/talkytrend-1.5.6.tar.gz` & `tmp/talkytrend-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.5.6.tar", max compression
+gzip compressed data, was "talkytrend-1.5.7.tar", max compression
```

## Comparing `talkytrend-1.5.6.tar` & `talkytrend-1.5.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-03 14:27:12.152038 talkytrend-1.5.6/LICENSE
--rw-r--r--   0        0        0     2190 2023-07-03 14:27:12.152038 talkytrend-1.5.6/README.md
--rw-r--r--   0        0        0     2178 2023-07-03 14:27:12.936051 talkytrend-1.5.6/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-03 14:27:12.936051 talkytrend-1.5.6/talkytrend/__init__.py
--rw-r--r--   0        0        0      708 2023-07-03 14:27:12.152038 talkytrend-1.5.6/talkytrend/config.py
--rw-r--r--   0        0        0     2087 2023-07-03 14:27:12.152038 talkytrend-1.5.6/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6467 2023-07-03 14:27:12.152038 talkytrend-1.5.6/talkytrend/main.py
--rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 talkytrend-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-03 17:07:49.464969 talkytrend-1.5.7/LICENSE
+-rw-r--r--   0        0        0     2190 2023-07-03 17:07:49.464969 talkytrend-1.5.7/README.md
+-rw-r--r--   0        0        0     2178 2023-07-03 17:07:50.184982 talkytrend-1.5.7/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-03 17:07:50.184982 talkytrend-1.5.7/talkytrend/__init__.py
+-rw-r--r--   0        0        0      708 2023-07-03 17:07:49.464969 talkytrend-1.5.7/talkytrend/config.py
+-rw-r--r--   0        0        0     2087 2023-07-03 17:07:49.464969 talkytrend-1.5.7/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6467 2023-07-03 17:07:49.464969 talkytrend-1.5.7/talkytrend/main.py
+-rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 talkytrend-1.5.7/PKG-INFO
```

### Comparing `talkytrend-1.5.6/LICENSE` & `talkytrend-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.6/README.md` & `talkytrend-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.6/pyproject.toml` & `talkytrend-1.5.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.5.6"
+version = "1.5.7"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.5.6/talkytrend/config.py` & `talkytrend-1.5.7/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.6/talkytrend/default_settings.toml` & `talkytrend-1.5.7/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.6/talkytrend/main.py` & `talkytrend-1.5.7/talkytrend/main.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.6/PKG-INFO` & `talkytrend-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.5.6
+Version: 1.5.7
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

