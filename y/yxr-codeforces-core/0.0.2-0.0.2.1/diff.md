# Comparing `tmp/yxr_codeforces_core-0.0.2.tar.gz` & `tmp/yxr_codeforces_core-0.0.2.1.tar.gz`

## Comparing `yxr_codeforces_core-0.0.2.tar` & `yxr_codeforces_core-0.0.2.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/__init__.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/account.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/constants.py
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/contest_list.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/contest_meta.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/contest_register.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/contest_standing.py
--rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/httphelper.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/language.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/problem.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/problems.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/submit.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/url.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/util.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/websocket.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/interfaces/AioHttpHelper.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/codeforces_core/interfaces/__init__.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/LICENSE
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/README.md
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/__init__.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/account.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/constants.py
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/contest_list.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/contest_meta.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/contest_register.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/contest_standing.py
+-rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/httphelper.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/language.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/problem.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/problems.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/py.typed
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/submit.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/url.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/util.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/websocket.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/interfaces/AioHttpHelper.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/interfaces/__init__.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/LICENSE
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/README.md
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/PKG-INFO
```

### Comparing `yxr_codeforces_core-0.0.2/codeforces_core/account.py` & `yxr_codeforces_core-0.0.2.1/codeforces_core/account.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/codeforces_core/contest_list.py` & `yxr_codeforces_core-0.0.2.1/codeforces_core/contest_list.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/codeforces_core/contest_meta.py` & `yxr_codeforces_core-0.0.2.1/codeforces_core/contest_meta.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/codeforces_core/contest_register.py` & `yxr_codeforces_core-0.0.2.1/codeforces_core/contest_register.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/codeforces_core/contest_standing.py` & `yxr_codeforces_core-0.0.2.1/codeforces_core/contest_standing.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/codeforces_core/httphelper.py` & `yxr_codeforces_core-0.0.2.1/codeforces_core/httphelper.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/codeforces_core/language.py` & `yxr_codeforces_core-0.0.2.1/codeforces_core/language.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/codeforces_core/problem.py` & `yxr_codeforces_core-0.0.2.1/codeforces_core/problem.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/codeforces_core/problems.py` & `yxr_codeforces_core-0.0.2.1/codeforces_core/problems.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/codeforces_core/submit.py` & `yxr_codeforces_core-0.0.2.1/codeforces_core/submit.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/codeforces_core/url.py` & `yxr_codeforces_core-0.0.2.1/codeforces_core/url.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/codeforces_core/util.py` & `yxr_codeforces_core-0.0.2.1/codeforces_core/util.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/codeforces_core/websocket.py` & `yxr_codeforces_core-0.0.2.1/codeforces_core/websocket.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/codeforces_core/interfaces/AioHttpHelper.py` & `yxr_codeforces_core-0.0.2.1/codeforces_core/interfaces/AioHttpHelper.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/.gitignore` & `yxr_codeforces_core-0.0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/LICENSE` & `yxr_codeforces_core-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/README.md` & `yxr_codeforces_core-0.0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# yxr-codeforces-core(WIP)
+# yxr-codeforces-core
 
 python3.8+ ([typing.Protocol](https://docs.python.org/3/library/typing.html#typing.Protocol) New in version 3.8.)
 
 | feature                          | code | inline example doc | unit test | e2e test |
 | -------------------------------- | ---- | ------------------ | --------- | -------- |
 | account login                    | ✅    | ✅                  | ✅         | ✅        |
 | submit code                      | ✅    | ✅                  | ✅         | ❌        |
@@ -18,8 +18,8 @@
 | pid/url parser                   | ✅    | ✅                  | ❌         | ❌        |
 | domain 2 ip dig tool             | ❌    | ❌                  | ❌         | ❌        |
 
 ## Docs
 
 [User](https://cromarmot.github.io/yxr-codeforces-core/user/index.html)
 
-[Developer](https://cromarmot.github.io/yxr-codeforces-core/dev/index.html)
+[Developer](https://cromarmot.github.io/yxr-codeforces-core/dev/index.html)
```

### Comparing `yxr_codeforces_core-0.0.2/pyproject.toml` & `yxr_codeforces_core-0.0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2/PKG-INFO` & `yxr_codeforces_core-0.0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yxr-codeforces-core
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Simple Codeforces core api
 Project-URL: Homepage, https://github.com/CroMarmot/yxr-codeforces-core
 Project-URL: Bug Tracker, https://github.com/CroMarmot/yxr-codeforces-core/issues
 Author-email: YeXiaoRain <yexiaorain@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 陈鼫RWHTYFZ
@@ -50,15 +50,15 @@
 Requires-Dist: mypy; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.20; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
 Requires-Dist: types-beautifulsoup4; extra == 'test'
 Description-Content-Type: text/markdown
 
-# yxr-codeforces-core(WIP)
+# yxr-codeforces-core
 
 python3.8+ ([typing.Protocol](https://docs.python.org/3/library/typing.html#typing.Protocol) New in version 3.8.)
 
 | feature                          | code | inline example doc | unit test | e2e test |
 | -------------------------------- | ---- | ------------------ | --------- | -------- |
 | account login                    | ✅    | ✅                  | ✅         | ✅        |
 | submit code                      | ✅    | ✅                  | ✅         | ❌        |
@@ -74,8 +74,8 @@
 | pid/url parser                   | ✅    | ✅                  | ❌         | ❌        |
 | domain 2 ip dig tool             | ❌    | ❌                  | ❌         | ❌        |
 
 ## Docs
 
 [User](https://cromarmot.github.io/yxr-codeforces-core/user/index.html)
 
-[Developer](https://cromarmot.github.io/yxr-codeforces-core/dev/index.html)
+[Developer](https://cromarmot.github.io/yxr-codeforces-core/dev/index.html)
```

