# Comparing `tmp/talkytrend-1.5.7.tar.gz` & `tmp/talkytrend-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.5.7.tar", max compression
+gzip compressed data, was "talkytrend-1.5.8.tar", max compression
```

## Comparing `talkytrend-1.5.7.tar` & `talkytrend-1.5.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-03 17:07:49.464969 talkytrend-1.5.7/LICENSE
--rw-r--r--   0        0        0     2190 2023-07-03 17:07:49.464969 talkytrend-1.5.7/README.md
--rw-r--r--   0        0        0     2178 2023-07-03 17:07:50.184982 talkytrend-1.5.7/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-03 17:07:50.184982 talkytrend-1.5.7/talkytrend/__init__.py
--rw-r--r--   0        0        0      708 2023-07-03 17:07:49.464969 talkytrend-1.5.7/talkytrend/config.py
--rw-r--r--   0        0        0     2087 2023-07-03 17:07:49.464969 talkytrend-1.5.7/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6467 2023-07-03 17:07:49.464969 talkytrend-1.5.7/talkytrend/main.py
--rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 talkytrend-1.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-03 20:45:45.007926 talkytrend-1.5.8/LICENSE
+-rw-r--r--   0        0        0     2247 2023-07-03 20:45:45.007926 talkytrend-1.5.8/README.md
+-rw-r--r--   0        0        0     2178 2023-07-03 20:45:45.727937 talkytrend-1.5.8/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-03 20:45:45.727937 talkytrend-1.5.8/talkytrend/__init__.py
+-rw-r--r--   0        0        0      708 2023-07-03 20:45:45.007926 talkytrend-1.5.8/talkytrend/config.py
+-rw-r--r--   0        0        0     2087 2023-07-03 20:45:45.007926 talkytrend-1.5.8/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6551 2023-07-03 20:45:45.007926 talkytrend-1.5.8/talkytrend/main.py
+-rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 talkytrend-1.5.8/PKG-INFO
```

### Comparing `talkytrend-1.5.7/LICENSE` & `talkytrend-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.7/README.md` & `talkytrend-1.5.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/226854338-e900f69e-d884-4a9a-90b1-b3dde7711b31.png"> | A python package to retrieve asset trend and economic data. |
 | ------------- | ------------- |
 |<br> 
 [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/talkytrend?icon=pypi&label)](https://pypi.org/project/talkytrend/) [![Version](https://img.shields.io/pypi/v/talkytrend)]()<br> [![Pypi](https://img.shields.io/pypi/dm/talkytrend)]()<br> [![👷‍♂️Build](https://github.com/mraniki/talkytrend/actions/workflows/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml/badge.svg)]() <br>[![codecov](https://codecov.io/gh/mraniki/TalkyTrend/branch/main/graph/badge.svg?token=WAHUEMAJN6)](https://codecov.io/gh/mraniki/TalkyTrend) [![codebeat badge](https://codebeat.co/badges/24c90aab-02d7-4cd1-9ad8-5907e180c9e6)](https://codebeat.co/projects/github-com-mraniki-talkytrend-main) | Find Asset Trend |
 
 Key features:
 
-- trading view connectivity
+- trading view connectivity with signal scanner
+- news connectivity 
+- FOMC reminder
 
 ## Install
 
 `pip install talkytrend`
 
 ## How to use it
```

### Comparing `talkytrend-1.5.7/pyproject.toml` & `talkytrend-1.5.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.5.7"
+version = "1.5.8"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.5.7/talkytrend/config.py` & `talkytrend-1.5.8/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.7/talkytrend/default_settings.toml` & `talkytrend-1.5.8/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.7/talkytrend/main.py` & `talkytrend-1.5.8/talkytrend/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,8 +167,9 @@
                         yield signals
 
             except Exception as error:
                 self.logger.error("scanner %s", error)
 
             await asyncio.sleep(settings.scanner_frequency)
 
-
+    async def get_info(self):
+        return f"{__class__.__name__} {__version__}\n"
```

### Comparing `talkytrend-1.5.7/PKG-INFO` & `talkytrend-1.5.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.5.7
+Version: 1.5.8
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,17 @@
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/226854338-e900f69e-d884-4a9a-90b1-b3dde7711b31.png"> | A python package to retrieve asset trend and economic data. |
 | ------------- | ------------- |
 |<br> 
 [![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/talkytrend?icon=pypi&label)](https://pypi.org/project/talkytrend/) [![Version](https://img.shields.io/pypi/v/talkytrend)]()<br> [![Pypi](https://img.shields.io/pypi/dm/talkytrend)]()<br> [![👷‍♂️Build](https://github.com/mraniki/talkytrend/actions/workflows/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml/badge.svg)]() <br>[![codecov](https://codecov.io/gh/mraniki/TalkyTrend/branch/main/graph/badge.svg?token=WAHUEMAJN6)](https://codecov.io/gh/mraniki/TalkyTrend) [![codebeat badge](https://codebeat.co/badges/24c90aab-02d7-4cd1-9ad8-5907e180c9e6)](https://codebeat.co/projects/github-com-mraniki-talkytrend-main) | Find Asset Trend |
 
 Key features:
 
-- trading view connectivity
+- trading view connectivity with signal scanner
+- news connectivity 
+- FOMC reminder
 
 ## Install
 
 `pip install talkytrend`
 
 ## How to use it
```

