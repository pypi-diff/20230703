# Comparing `tmp/yt_dlp_types-0.0.2.tar.gz` & `tmp/yt_dlp_types-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_dlp_types-0.0.2.tar", max compression
+gzip compressed data, was "yt_dlp_types-0.0.3.tar", max compression
```

## Comparing `yt_dlp_types-0.0.2.tar` & `yt_dlp_types-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1087 2023-07-03 15:46:20.349120 yt_dlp_types-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      139 2023-07-03 15:46:20.358120 yt_dlp_types-0.0.2/README.md
--rw-r--r--   0        0        0      699 2023-07-03 19:39:07.170338 yt_dlp_types-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      438 2023-07-03 19:24:39.941985 yt_dlp_types-0.0.2/yt_dlp-stubs/YoutubeDL.pyi
--rw-r--r--   0        0        0    27804 2023-07-03 19:37:36.027414 yt_dlp_types-0.0.2/yt_dlp-stubs/__init__.pyi
--rw-r--r--   0        0        0      286 2023-07-03 19:24:37.015987 yt_dlp_types-0.0.2/yt_dlp-stubs/_misc.pyi
--rw-r--r--   0        0        0      588 2023-07-03 19:24:38.504986 yt_dlp_types-0.0.2/yt_dlp-stubs/cookies.pyi
--rw-r--r--   0        0        0        0 2023-07-03 19:24:30.422991 yt_dlp_types-0.0.2/yt_dlp-stubs/extractor/__init__.pyi
--rw-r--r--   0        0        0     1917 2023-07-03 19:24:31.719990 yt_dlp_types-0.0.2/yt_dlp-stubs/extractor/common.pyi
--rw-r--r--   0        0        0        0 2023-07-03 19:04:47.210090 yt_dlp_types-0.0.2/yt_dlp-stubs/py.typed
--rw-r--r--   0        0        0       22 2023-07-03 19:24:33.389989 yt_dlp_types-0.0.2/yt_dlp-stubs/utils/__init__.pyi
--rw-r--r--   0        0        0     1178 2023-07-03 19:24:34.339989 yt_dlp_types-0.0.2/yt_dlp-stubs/utils/_utils.pyi
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 yt_dlp_types-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-07-03 15:46:20.349120 yt_dlp_types-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      128 2023-07-03 19:42:09.982181 yt_dlp_types-0.0.3/README.md
+-rw-r--r--   0        0        0      699 2023-07-03 20:12:36.690228 yt_dlp_types-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      501 2023-07-03 19:58:11.117874 yt_dlp_types-0.0.3/yt_dlp-stubs/YoutubeDL.pyi
+-rw-r--r--   0        0        0    27804 2023-07-03 19:37:36.027414 yt_dlp_types-0.0.3/yt_dlp-stubs/__init__.pyi
+-rw-r--r--   0        0        0      286 2023-07-03 19:24:37.015987 yt_dlp_types-0.0.3/yt_dlp-stubs/_misc.pyi
+-rw-r--r--   0        0        0      588 2023-07-03 19:24:38.504986 yt_dlp_types-0.0.3/yt_dlp-stubs/cookies.pyi
+-rw-r--r--   0        0        0        0 2023-07-03 19:24:30.422991 yt_dlp_types-0.0.3/yt_dlp-stubs/extractor/__init__.pyi
+-rw-r--r--   0        0        0     1917 2023-07-03 19:24:31.719990 yt_dlp_types-0.0.3/yt_dlp-stubs/extractor/common.pyi
+-rw-r--r--   0        0        0        0 2023-07-03 19:04:47.210090 yt_dlp_types-0.0.3/yt_dlp-stubs/py.typed
+-rw-r--r--   0        0        0       22 2023-07-03 19:24:33.389989 yt_dlp_types-0.0.3/yt_dlp-stubs/utils/__init__.pyi
+-rw-r--r--   0        0        0     1178 2023-07-03 19:24:34.339989 yt_dlp_types-0.0.3/yt_dlp-stubs/utils/_utils.pyi
+-rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 yt_dlp_types-0.0.3/PKG-INFO
```

### Comparing `yt_dlp_types-0.0.2/LICENSE.txt` & `yt_dlp_types-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yt_dlp_types-0.0.2/pyproject.toml` & `yt_dlp_types-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 authors = ["Andrew Udvare <audvare@gmail.com>"]
 classifiers = ['Typing :: Typed']
 description = "Typing stubs for yt-dlp"
 license = "MIT"
 name = "yt-dlp-types"
 packages = [{ include = "yt_dlp-stubs" }]
 readme = "README.md"
-version = "0.0.2"
+version = "0.0.3"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `yt_dlp_types-0.0.2/yt_dlp-stubs/__init__.pyi` & `yt_dlp_types-0.0.3/yt_dlp-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `yt_dlp_types-0.0.2/yt_dlp-stubs/cookies.pyi` & `yt_dlp_types-0.0.3/yt_dlp-stubs/cookies.pyi`

 * *Files identical despite different names*

### Comparing `yt_dlp_types-0.0.2/yt_dlp-stubs/extractor/common.pyi` & `yt_dlp_types-0.0.3/yt_dlp-stubs/extractor/common.pyi`

 * *Files identical despite different names*

### Comparing `yt_dlp_types-0.0.2/yt_dlp-stubs/utils/_utils.pyi` & `yt_dlp_types-0.0.3/yt_dlp-stubs/utils/_utils.pyi`

 * *Files identical despite different names*

### Comparing `yt_dlp_types-0.0.2/PKG-INFO` & `yt_dlp_types-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: yt-dlp-types
-Version: 0.0.2
+Version: 0.0.3
 Summary: Typing stubs for yt-dlp
 License: MIT
 Author: Andrew Udvare
 Author-email: audvare@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 
 # yt-dlp types
 
-Types for yt-dlp
+Types for yt-dlp.
 
 ## Installation
 
 ```shell
 pip install types-yt-dlp
 ```
 
-## Command line usage
-
 ```shell
-types-yt-dlp
+poetry add types-yt-dlp
 ```
```

