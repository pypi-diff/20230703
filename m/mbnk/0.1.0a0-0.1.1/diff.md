# Comparing `tmp/mbnk-0.1.0a0.tar.gz` & `tmp/mbnk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbnk-0.1.0a0.tar", max compression
+gzip compressed data, was "mbnk-0.1.1.tar", max compression
```

## Comparing `mbnk-0.1.0a0.tar` & `mbnk-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,14 @@
--rw-r--r--   0        0        0     1420 2023-07-02 05:05:53.695059 mbnk-0.1.0a0/README.md
--rw-r--r--   0        0        0      359 2023-07-02 05:26:34.519609 mbnk-0.1.0a0/mbnk/__init__.py
--rw-r--r--   0        0        0    14803 2023-07-02 18:44:15.060560 mbnk-0.1.0a0/mbnk/api.py
--rw-r--r--   0        0        0      101 2023-07-02 05:26:15.783700 mbnk-0.1.0a0/mbnk/asyncio/__init__.py
--rw-r--r--   0        0        0      323 2023-07-02 17:30:10.132706 mbnk-0.1.0a0/mbnk/asyncio/mbnk.py
--rw-r--r--   0        0        0     2710 2023-07-02 17:32:57.818194 mbnk-0.1.0a0/mbnk/decorators.py
--rw-r--r--   0        0        0     1697 2023-07-02 05:20:44.513374 mbnk-0.1.0a0/mbnk/enums.py
--rw-r--r--   0        0        0      300 2023-07-02 01:07:19.623331 mbnk-0.1.0a0/mbnk/exceptions.py
--rw-r--r--   0        0        0     2164 2023-07-02 18:13:15.452507 mbnk-0.1.0a0/mbnk/instances.py
--rw-r--r--   0        0        0      315 2023-07-02 18:14:01.695715 mbnk-0.1.0a0/mbnk/mbnk.py
--rw-r--r--   0        0        0     2217 2023-07-01 23:15:46.030057 mbnk-0.1.0a0/mbnk/responses.py
--rw-r--r--   0        0        0       97 2023-07-01 23:23:24.859301 mbnk-0.1.0a0/mbnk/utils/__init__.py
--rw-r--r--   0        0        0      269 2023-07-01 23:23:25.011300 mbnk-0.1.0a0/mbnk/utils/builders.py
--rw-r--r--   0        0        0      839 2023-07-02 18:14:30.643213 mbnk-0.1.0a0/mbnk/utils/format.py
--rw-r--r--   0        0        0      389 2023-07-02 01:04:35.544706 mbnk-0.1.0a0/mbnk/utils/is_exception.py
--rw-r--r--   0        0        0      466 2023-07-01 22:05:58.624489 mbnk-0.1.0a0/mbnk/utils/webhook.py
--rw-r--r--   0        0        0      315 2023-07-02 18:55:37.617760 mbnk-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0     1953 1970-01-01 00:00:00.000000 mbnk-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1799 2023-07-02 23:48:44.152523 mbnk-0.1.1/README.md
+-rw-r--r--   0        0        0      308 2023-07-02 23:36:59.720764 mbnk-0.1.1/mbnk/__init__.py
+-rw-r--r--   0        0        0    17634 2023-07-02 23:18:41.104797 mbnk-0.1.1/mbnk/api.py
+-rw-r--r--   0        0        0      127 2023-07-02 23:03:02.426763 mbnk-0.1.1/mbnk/asyncio/__init__.py
+-rw-r--r--   0        0        0      423 2023-07-02 23:04:25.131158 mbnk-0.1.1/mbnk/asyncio/mbnk.py
+-rw-r--r--   0        0        0     1347 2023-07-02 22:17:52.460089 mbnk-0.1.1/mbnk/enums.py
+-rw-r--r--   0        0        0      300 2023-07-02 23:06:33.479647 mbnk-0.1.1/mbnk/exceptions.py
+-rw-r--r--   0        0        0     2164 2023-07-02 18:13:15.452507 mbnk-0.1.1/mbnk/instances.py
+-rw-r--r--   0        0        0      315 2023-07-02 18:14:01.695715 mbnk-0.1.1/mbnk/mbnk.py
+-rw-r--r--   0        0        0     2217 2023-07-01 23:15:46.030057 mbnk-0.1.1/mbnk/responses.py
+-rw-r--r--   0        0        0       23 2023-07-02 22:21:13.141308 mbnk-0.1.1/mbnk/utils/__init__.py
+-rw-r--r--   0        0        0      510 2023-07-02 22:21:26.081132 mbnk-0.1.1/mbnk/utils/webhook.py
+-rw-r--r--   0        0        0      313 2023-07-02 22:33:00.127952 mbnk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 mbnk-0.1.1/PKG-INFO
```

### Comparing `mbnk-0.1.0a0/README.md` & `mbnk-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,32 @@
+# Mbnk
+<hr>
+
+![PyPI](https://img.shields.io/pypi/v/mbnk)
+
 ## Sync/Async Python3 Monobank API
 
 ### Introduction
 
 <b>mbnk</b> - python lib for: 
 <br>
-<br>
-&bull; Monobank Open API <br> official docs: https://api.monobank.ua/docs/
-<br>
-&bull; Monobank Open API for providers <br> official docs: https://api.monobank.ua/docs/corporate.html
-<br>
-&bull; MonoPay - Monobank Acquiring <br> official docs: https://api.monobank.ua/docs/acquiring.html
+<br>&bull; Monobank Open API 
+<br>official docs: https://api.monobank.ua/docs/ 
+<br>lib docs: https://github.com/yeghorkikhai/mbnk/blob/master/docs/monobank_open_api.md
+<br>&bull; Monobank Open API for providers 
+<br> official docs: https://api.monobank.ua/docs/corporate.html
+<br>lib docs: https://github.com/yeghorkikhai/mbnk/blob/master/docs/monobank_corp_open_api.md
+<br>&bull; MonoPay - Monobank Acquiring
+<br>official docs: https://api.monobank.ua/docs/acquiring.html
+<br>lib docs: https://github.com/yeghorkikhai/mbnk/blob/master/docs/monopay_api.md
+
+### Github
+```
+https://github.com/yeghorkikhai/mbnk
+```
 
 ### Installation
 ```python
 pip install mbnk
 ```
 
 ### Getting Started Monobank Open API
```

### Comparing `mbnk-0.1.0a0/mbnk/instances.py` & `mbnk-0.1.1/mbnk/instances.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.0a0/mbnk/responses.py` & `mbnk-0.1.1/mbnk/responses.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.0a0/PKG-INFO` & `mbnk-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 Metadata-Version: 2.1
 Name: mbnk
-Version: 0.1.0a0
+Version: 0.1.1
 Summary: Sync/Async version monobank api
 License: MIT
 Author: yeghorkikhai
 Author-email: yeghorkikhai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
+# Mbnk
+<hr>
+
+![PyPI](https://img.shields.io/pypi/v/mbnk)
+
 ## Sync/Async Python3 Monobank API
 
 ### Introduction
 
 <b>mbnk</b> - python lib for: 
 <br>
-<br>
-&bull; Monobank Open API <br> official docs: https://api.monobank.ua/docs/
-<br>
-&bull; Monobank Open API for providers <br> official docs: https://api.monobank.ua/docs/corporate.html
-<br>
-&bull; MonoPay - Monobank Acquiring <br> official docs: https://api.monobank.ua/docs/acquiring.html
+<br>&bull; Monobank Open API 
+<br>official docs: https://api.monobank.ua/docs/ 
+<br>lib docs: https://github.com/yeghorkikhai/mbnk/blob/master/docs/monobank_open_api.md
+<br>&bull; Monobank Open API for providers 
+<br> official docs: https://api.monobank.ua/docs/corporate.html
+<br>lib docs: https://github.com/yeghorkikhai/mbnk/blob/master/docs/monobank_corp_open_api.md
+<br>&bull; MonoPay - Monobank Acquiring
+<br>official docs: https://api.monobank.ua/docs/acquiring.html
+<br>lib docs: https://github.com/yeghorkikhai/mbnk/blob/master/docs/monopay_api.md
+
+### Github
+```
+https://github.com/yeghorkikhai/mbnk
+```
 
 ### Installation
 ```python
 pip install mbnk
 ```
 
 ### Getting Started Monobank Open API
```

