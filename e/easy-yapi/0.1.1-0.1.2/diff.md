# Comparing `tmp/easy_yapi-0.1.1.tar.gz` & `tmp/easy_yapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_yapi-0.1.1.tar", last modified: Mon Jul  3 07:57:32 2023, max compression
+gzip compressed data, was "easy_yapi-0.1.2.tar", last modified: Mon Jul  3 08:22:23 2023, max compression
```

## Comparing `easy_yapi-0.1.1.tar` & `easy_yapi-0.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-03 07:57:32.519938 easy_yapi-0.1.1/
--rw-r--r--   0 admin      (501) staff       (20)      151 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/AUTHORS.rst
--rw-r--r--   0 admin      (501) staff       (20)     3541 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 admin      (501) staff       (20)       89 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/HISTORY.rst
--rw-r--r--   0 admin      (501) staff       (20)     1068 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)      262 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     1893 2023-07-03 07:57:32.520423 easy_yapi-0.1.1/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     1122 2023-07-03 07:41:28.000000 easy_yapi-0.1.1/README.rst
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-03 07:57:32.506281 easy_yapi-0.1.1/docs/
--rw-r--r--   0 admin      (501) staff       (20)      610 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/docs/Makefile
--rw-r--r--   0 admin      (501) staff       (20)       28 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/docs/authors.rst
--rwxr-xr-x   0 admin      (501) staff       (20)     4795 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/docs/conf.py
--rw-r--r--   0 admin      (501) staff       (20)       33 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/docs/contributing.rst
--rw-r--r--   0 admin      (501) staff       (20)       28 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/docs/history.rst
--rw-r--r--   0 admin      (501) staff       (20)      306 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/docs/index.rst
--rw-r--r--   0 admin      (501) staff       (20)     1142 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/docs/installation.rst
--rw-r--r--   0 admin      (501) staff       (20)      807 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/docs/make.bat
--rw-r--r--   0 admin      (501) staff       (20)       27 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/docs/readme.rst
--rw-r--r--   0 admin      (501) staff       (20)       73 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/docs/usage.rst
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-03 07:57:32.511954 easy_yapi-0.1.1/easy_yapi/
--rw-r--r--   0 admin      (501) staff       (20)      177 2023-07-03 07:57:29.000000 easy_yapi-0.1.1/easy_yapi/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1259 2023-06-29 09:29:09.000000 easy_yapi-0.1.1/easy_yapi/base_api.py
--rw-r--r--   0 admin      (501) staff       (20)      405 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/easy_yapi/cli.py
--rw-r--r--   0 admin      (501) staff       (20)      548 2023-06-29 10:59:03.000000 easy_yapi-0.1.1/easy_yapi/easy_yapi.py
--rw-r--r--   0 admin      (501) staff       (20)     2488 2023-06-29 10:59:10.000000 easy_yapi-0.1.1/easy_yapi/group.py
--rw-r--r--   0 admin      (501) staff       (20)     4399 2023-06-29 10:59:19.000000 easy_yapi-0.1.1/easy_yapi/project.py
--rw-r--r--   0 admin      (501) staff       (20)     2353 2023-06-29 10:58:41.000000 easy_yapi-0.1.1/easy_yapi/user.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-03 07:57:32.516244 easy_yapi-0.1.1/easy_yapi.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1893 2023-07-03 07:57:32.000000 easy_yapi-0.1.1/easy_yapi.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      671 2023-07-03 07:57:32.000000 easy_yapi-0.1.1/easy_yapi.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-03 07:57:32.000000 easy_yapi-0.1.1/easy_yapi.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       49 2023-07-03 07:57:32.000000 easy_yapi-0.1.1/easy_yapi.egg-info/entry_points.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-29 09:43:10.000000 easy_yapi-0.1.1/easy_yapi.egg-info/not-zip-safe
--rw-r--r--   0 admin      (501) staff       (20)       20 2023-07-03 07:57:32.000000 easy_yapi-0.1.1/easy_yapi.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       10 2023-07-03 07:57:32.000000 easy_yapi-0.1.1/easy_yapi.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)      426 2023-07-03 07:57:32.521665 easy_yapi-0.1.1/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1388 2023-07-03 07:57:29.000000 easy_yapi-0.1.1/setup.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-03 07:57:32.517686 easy_yapi-0.1.1/tests/
--rw-r--r--   0 admin      (501) staff       (20)       39 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/tests/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      989 2023-06-29 09:16:28.000000 easy_yapi-0.1.1/tests/test_easy_yapi.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-03 08:22:23.454563 easy_yapi-0.1.2/
+-rw-r--r--   0 admin      (501) staff       (20)      151 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/AUTHORS.rst
+-rw-r--r--   0 admin      (501) staff       (20)     3541 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 admin      (501) staff       (20)       89 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/HISTORY.rst
+-rw-r--r--   0 admin      (501) staff       (20)     1068 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)      262 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)     2110 2023-07-03 08:22:23.454756 easy_yapi-0.1.2/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1339 2023-07-03 08:20:38.000000 easy_yapi-0.1.2/README.rst
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-03 08:22:23.445445 easy_yapi-0.1.2/docs/
+-rw-r--r--   0 admin      (501) staff       (20)      610 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/docs/Makefile
+-rw-r--r--   0 admin      (501) staff       (20)       28 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/docs/authors.rst
+-rwxr-xr-x   0 admin      (501) staff       (20)     4795 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/docs/conf.py
+-rw-r--r--   0 admin      (501) staff       (20)       33 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/docs/contributing.rst
+-rw-r--r--   0 admin      (501) staff       (20)       28 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/docs/history.rst
+-rw-r--r--   0 admin      (501) staff       (20)      306 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/docs/index.rst
+-rw-r--r--   0 admin      (501) staff       (20)     1142 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/docs/installation.rst
+-rw-r--r--   0 admin      (501) staff       (20)      807 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/docs/make.bat
+-rw-r--r--   0 admin      (501) staff       (20)       27 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/docs/readme.rst
+-rw-r--r--   0 admin      (501) staff       (20)       73 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/docs/usage.rst
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-03 08:22:23.450193 easy_yapi-0.1.2/easy_yapi/
+-rw-r--r--   0 admin      (501) staff       (20)      177 2023-07-03 08:21:43.000000 easy_yapi-0.1.2/easy_yapi/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1259 2023-06-29 09:29:09.000000 easy_yapi-0.1.2/easy_yapi/base_api.py
+-rw-r--r--   0 admin      (501) staff       (20)      405 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/easy_yapi/cli.py
+-rw-r--r--   0 admin      (501) staff       (20)      357 2023-07-03 08:16:19.000000 easy_yapi-0.1.2/easy_yapi/easy_yapi.py
+-rw-r--r--   0 admin      (501) staff       (20)     2488 2023-06-29 10:59:10.000000 easy_yapi-0.1.2/easy_yapi/group.py
+-rw-r--r--   0 admin      (501) staff       (20)     4399 2023-06-29 10:59:19.000000 easy_yapi-0.1.2/easy_yapi/project.py
+-rw-r--r--   0 admin      (501) staff       (20)     2312 2023-07-03 08:19:32.000000 easy_yapi-0.1.2/easy_yapi/user.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-03 08:22:23.452722 easy_yapi-0.1.2/easy_yapi.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     2110 2023-07-03 08:22:23.000000 easy_yapi-0.1.2/easy_yapi.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      671 2023-07-03 08:22:23.000000 easy_yapi-0.1.2/easy_yapi.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-03 08:22:23.000000 easy_yapi-0.1.2/easy_yapi.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       49 2023-07-03 08:22:23.000000 easy_yapi-0.1.2/easy_yapi.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-29 09:43:10.000000 easy_yapi-0.1.2/easy_yapi.egg-info/not-zip-safe
+-rw-r--r--   0 admin      (501) staff       (20)       20 2023-07-03 08:22:23.000000 easy_yapi-0.1.2/easy_yapi.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       10 2023-07-03 08:22:23.000000 easy_yapi-0.1.2/easy_yapi.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)      426 2023-07-03 08:22:23.455568 easy_yapi-0.1.2/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1388 2023-07-03 08:21:43.000000 easy_yapi-0.1.2/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-03 08:22:23.453837 easy_yapi-0.1.2/tests/
+-rw-r--r--   0 admin      (501) staff       (20)       39 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/tests/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      989 2023-06-29 09:16:28.000000 easy_yapi-0.1.2/tests/test_easy_yapi.py
```

### Comparing `easy_yapi-0.1.1/CONTRIBUTING.rst` & `easy_yapi-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `easy_yapi-0.1.1/LICENSE` & `easy_yapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_yapi-0.1.1/PKG-INFO` & `easy_yapi-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_yapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Yapi Python SDK
 Home-page: https://github.com/nocoding126/easy_yapi
 Author: 派大星
 Author-email: nocoding@126.com
 License: MIT license
 Keywords: easy_yapi,yapi
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -37,20 +37,32 @@
 
 
 
 Yapi Python SDK
 
 
 * Free software: MIT license
-* Documentation: https://easy-yapi.readthedocs.io.
+* Documentation:
 
 Installation and Usage
 ----------------------
-pip install easy_yapi
+.. code-block:: python
 
+   pip install easy_yapi
+
+示例-login
+----------
+.. code-block:: python
+
+    from easy_yapi import Yapi
+
+
+    yapi = Yapi(base_url='http://82.156.152.141:3000')
+    res = yapi.login(email='nocoding@126.com', password='ymfe.org')
+    print(res.text)
 
 
 Features
 --------
 
 * 该库主要用于快速生成yapi接口文档
 * 该库是一个练习项目，并未完全实现所有Yapi接口的封装
```

### Comparing `easy_yapi-0.1.1/README.rst` & `easy_yapi-0.1.2/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -16,20 +16,32 @@
 
 
 
 Yapi Python SDK
 
 
 * Free software: MIT license
-* Documentation: https://easy-yapi.readthedocs.io.
+* Documentation:
 
 Installation and Usage
 ----------------------
-pip install easy_yapi
+.. code-block:: python
 
+   pip install easy_yapi
+
+示例-login
+----------
+.. code-block:: python
+
+    from easy_yapi import Yapi
+
+
+    yapi = Yapi(base_url='http://82.156.152.141:3000')
+    res = yapi.login(email='nocoding@126.com', password='ymfe.org')
+    print(res.text)
 
 
 Features
 --------
 
 * 该库主要用于快速生成yapi接口文档
 * 该库是一个练习项目，并未完全实现所有Yapi接口的封装
```

### Comparing `easy_yapi-0.1.1/docs/Makefile` & `easy_yapi-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `easy_yapi-0.1.1/docs/conf.py` & `easy_yapi-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `easy_yapi-0.1.1/docs/installation.rst` & `easy_yapi-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `easy_yapi-0.1.1/docs/make.bat` & `easy_yapi-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `easy_yapi-0.1.1/easy_yapi/base_api.py` & `easy_yapi-0.1.2/easy_yapi/base_api.py`

 * *Files identical despite different names*

### Comparing `easy_yapi-0.1.1/easy_yapi/group.py` & `easy_yapi-0.1.2/easy_yapi/group.py`

 * *Files identical despite different names*

### Comparing `easy_yapi-0.1.1/easy_yapi/project.py` & `easy_yapi-0.1.2/easy_yapi/project.py`

 * *Files identical despite different names*

### Comparing `easy_yapi-0.1.1/easy_yapi/user.py` & `easy_yapi-0.1.2/easy_yapi/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """用户相关接口"""
     def login(self, email, password):
         """登录"""
         res = self.post('/api/user/login', json={"email": email, "password": password})
         res.raise_for_status()
         _cookie = res.headers.get('Set-Cookie', '')
         self._session.cookies.update({"Cookie": _cookie})
-        # self._session.headers.update({"Cookie": _cookie})
+        return res
 
     def logout(self):
         """退出登录"""
         res = self.get('/api/user/logout')
         res.raise_for_status()
         return res
```

### Comparing `easy_yapi-0.1.1/easy_yapi.egg-info/PKG-INFO` & `easy_yapi-0.1.2/easy_yapi.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-yapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Yapi Python SDK
 Home-page: https://github.com/nocoding126/easy_yapi
 Author: 派大星
 Author-email: nocoding@126.com
 License: MIT license
 Keywords: easy_yapi,yapi
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -37,20 +37,32 @@
 
 
 
 Yapi Python SDK
 
 
 * Free software: MIT license
-* Documentation: https://easy-yapi.readthedocs.io.
+* Documentation:
 
 Installation and Usage
 ----------------------
-pip install easy_yapi
+.. code-block:: python
 
+   pip install easy_yapi
+
+示例-login
+----------
+.. code-block:: python
+
+    from easy_yapi import Yapi
+
+
+    yapi = Yapi(base_url='http://82.156.152.141:3000')
+    res = yapi.login(email='nocoding@126.com', password='ymfe.org')
+    print(res.text)
 
 
 Features
 --------
 
 * 该库主要用于快速生成yapi接口文档
 * 该库是一个练习项目，并未完全实现所有Yapi接口的封装
```

### Comparing `easy_yapi-0.1.1/easy_yapi.egg-info/SOURCES.txt` & `easy_yapi-0.1.2/easy_yapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easy_yapi-0.1.1/setup.py` & `easy_yapi-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,10 +42,10 @@
     include_package_data=True,
     keywords=['easy_yapi', 'yapi'],
     name='easy_yapi',
     packages=find_packages(include=['easy_yapi', 'easy_yapi.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/nocoding126/easy_yapi',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

### Comparing `easy_yapi-0.1.1/tests/test_easy_yapi.py` & `easy_yapi-0.1.2/tests/test_easy_yapi.py`

 * *Files identical despite different names*

