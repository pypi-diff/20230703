# Comparing `tmp/hayloft-0.4.0.tar.gz` & `tmp/hayloft-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.4.0.tar", max compression
+gzip compressed data, was "hayloft-0.4.0a0.tar", max compression
```

## Comparing `hayloft-0.4.0.tar` & `hayloft-0.4.0a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.4.0/LICENSE
--rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.4.0/hayloft/__init__.py
--rw-r--r--   0        0        0     5048 2023-07-03 08:43:15.676287 hayloft-0.4.0/hayloft/app.py
--rw-r--r--   0        0        0     1660 2023-07-03 08:42:36.775929 hayloft-0.4.0/hayloft/llama_index.py
--rw-r--r--   0        0        0      922 2023-07-02 09:44:38.522358 hayloft-0.4.0/hayloft/logger.py
--rw-r--r--   0        0        0    28209 2023-07-03 08:44:28.656963 hayloft-0.4.0/hayloft/public/assets/index-883c7b1f.css
--rw-r--r--   0        0        0   184324 2023-07-03 08:44:28.656963 hayloft-0.4.0/hayloft/public/assets/index-889253f9.js
--rw-r--r--   0        0        0      384 2023-07-03 08:44:28.656963 hayloft-0.4.0/hayloft/public/index.html
--rw-r--r--   0        0        0      575 2023-06-26 15:43:07.772960 hayloft-0.4.0/hayloft/schema.py
--rw-r--r--   0        0        0      569 2023-06-22 15:54:28.929777 hayloft-0.4.0/hayloft/sse.py
--rw-r--r--   0        0        0      571 2023-07-03 08:57:11.480785 hayloft-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 hayloft-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.4.0a0/LICENSE
+-rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.4.0a0/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.4.0a0/hayloft/__init__.py
+-rw-r--r--   0        0        0     5048 2023-07-03 08:43:15.676287 hayloft-0.4.0a0/hayloft/app.py
+-rw-r--r--   0        0        0     1660 2023-07-03 08:42:36.775929 hayloft-0.4.0a0/hayloft/llama_index.py
+-rw-r--r--   0        0        0      922 2023-07-02 09:44:38.522358 hayloft-0.4.0a0/hayloft/logger.py
+-rw-r--r--   0        0        0    28209 2023-07-03 08:44:28.656963 hayloft-0.4.0a0/hayloft/public/assets/index-883c7b1f.css
+-rw-r--r--   0        0        0   184324 2023-07-03 08:44:28.656963 hayloft-0.4.0a0/hayloft/public/assets/index-889253f9.js
+-rw-r--r--   0        0        0      384 2023-07-03 08:44:28.656963 hayloft-0.4.0a0/hayloft/public/index.html
+-rw-r--r--   0        0        0      575 2023-06-26 15:43:07.772960 hayloft-0.4.0a0/hayloft/schema.py
+-rw-r--r--   0        0        0      569 2023-06-22 15:54:28.929777 hayloft-0.4.0a0/hayloft/sse.py
+-rw-r--r--   0        0        0      573 2023-07-03 08:45:50.574393 hayloft-0.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 hayloft-0.4.0a0/PKG-INFO
```

### Comparing `hayloft-0.4.0/LICENSE` & `hayloft-0.4.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0/README.md` & `hayloft-0.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0/hayloft/app.py` & `hayloft-0.4.0a0/hayloft/app.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0/hayloft/llama_index.py` & `hayloft-0.4.0a0/hayloft/llama_index.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0/hayloft/logger.py` & `hayloft-0.4.0a0/hayloft/logger.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0/hayloft/public/assets/index-883c7b1f.css` & `hayloft-0.4.0a0/hayloft/public/assets/index-883c7b1f.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0/hayloft/public/assets/index-889253f9.js` & `hayloft-0.4.0a0/hayloft/public/assets/index-889253f9.js`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0/hayloft/schema.py` & `hayloft-0.4.0a0/hayloft/schema.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0/hayloft/sse.py` & `hayloft-0.4.0a0/hayloft/sse.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.4.0/pyproject.toml` & `hayloft-0.4.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hayloft"
-version = "0.4.0"
+version = "0.4.0a0"
 description = "UI tool for LLM frameworks"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eturchenkov/hayloft"
 keywords = ["llm framework", "llm app tracking", "ui for llm app"]
```

### Comparing `hayloft-0.4.0/PKG-INFO` & `hayloft-0.4.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hayloft
-Version: 0.4.0
+Version: 0.4.0a0
 Summary: UI tool for LLM frameworks
 Home-page: https://github.com/eturchenkov/hayloft
 License: MIT
 Keywords: llm framework,llm app tracking,ui for llm app
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

