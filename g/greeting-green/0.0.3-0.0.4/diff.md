# Comparing `tmp/greeting_green-0.0.3.tar.gz` & `tmp/greeting_green-0.0.4.tar.gz`

## Comparing `greeting_green-0.0.3.tar` & `greeting_green-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/__init__.py
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/admin.py
--rwxr-xr-x   0        0        0      160 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/apps.py
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/models.py
--rwxr-xr-x   0        0        0      381 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/tests.py
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/urls.py
--rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/views.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/migrations/__init__.py
--rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/static/greeting/style.css
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/templates/greeting/index.html
--rwxr-xr-x   0        0        0       29 2020-02-02 00:00:00.000000 greeting_green-0.0.3/.gitignore
--rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 greeting_green-0.0.3/LICENSE.txt
--rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 greeting_green-0.0.3/README.md
--rwxr-xr-x   0        0        0     3297 2020-02-02 00:00:00.000000 greeting_green-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 greeting_green-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/__init__.py
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/admin.py
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/apps.py
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/models.py
+-rwxr-xr-x   0        0        0      381 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/tests.py
+-rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/urls.py
+-rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/views.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/migrations/__init__.py
+-rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/static/greeting/style.css
+-rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/templates/greeting/index.html
+-rwxr-xr-x   0        0        0       29 2020-02-02 00:00:00.000000 greeting_green-0.0.4/.gitignore
+-rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 greeting_green-0.0.4/LICENSE.txt
+-rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 greeting_green-0.0.4/README.md
+-rwxr-xr-x   0        0        0     1220 2020-02-02 00:00:00.000000 greeting_green-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 greeting_green-0.0.4/PKG-INFO
```

### Comparing `greeting_green-0.0.3/LICENSE.txt` & `greeting_green-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `greeting_green-0.0.3/README.md` & `greeting_green-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `greeting_green-0.0.3/PKG-INFO` & `greeting_green-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: greeting-green
-Version: 0.0.3
-Summary: 挨拶アプリ
+Version: 0.0.4
+Summary: test
 Project-URL: Documentation, https://github.com/unknown/greeting-green#readme
 Project-URL: Issues, https://github.com/unknown/greeting-green/issues
 Project-URL: Source, https://github.com/unknown/greeting-green
-Author-email: Kenno-Warise <wariken0523@gmail.com>
+Author-email: Warise <example@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

