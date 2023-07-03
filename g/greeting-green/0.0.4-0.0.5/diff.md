# Comparing `tmp/greeting_green-0.0.4.tar.gz` & `tmp/greeting_green-0.0.5.tar.gz`

## Comparing `greeting_green-0.0.4.tar` & `greeting_green-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/__init__.py
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/admin.py
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/apps.py
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/models.py
--rwxr-xr-x   0        0        0      381 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/tests.py
--rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/urls.py
--rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/views.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/migrations/__init__.py
--rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/static/greeting/style.css
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 greeting_green-0.0.4/greeting/templates/greeting/index.html
--rwxr-xr-x   0        0        0       29 2020-02-02 00:00:00.000000 greeting_green-0.0.4/.gitignore
--rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 greeting_green-0.0.4/LICENSE.txt
--rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 greeting_green-0.0.4/README.md
--rwxr-xr-x   0        0        0     1220 2020-02-02 00:00:00.000000 greeting_green-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 greeting_green-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 greeting_green-0.0.5/greeting/__init__.py
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 greeting_green-0.0.5/greeting/admin.py
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 greeting_green-0.0.5/greeting/apps.py
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 greeting_green-0.0.5/greeting/models.py
+-rwxr-xr-x   0        0        0      381 2020-02-02 00:00:00.000000 greeting_green-0.0.5/greeting/tests.py
+-rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 greeting_green-0.0.5/greeting/urls.py
+-rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 greeting_green-0.0.5/greeting/views.py
+-rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 greeting_green-0.0.5/greeting/static/greeting/style.css
+-rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 greeting_green-0.0.5/greeting/templates/greeting/index.html
+-rwxr-xr-x   0        0        0       29 2020-02-02 00:00:00.000000 greeting_green-0.0.5/.gitignore
+-rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 greeting_green-0.0.5/LICENSE.txt
+-rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 greeting_green-0.0.5/README.md
+-rwxr-xr-x   0        0        0     1227 2020-02-02 00:00:00.000000 greeting_green-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 greeting_green-0.0.5/PKG-INFO
```

### Comparing `greeting_green-0.0.4/LICENSE.txt` & `greeting_green-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `greeting_green-0.0.4/README.md` & `greeting_green-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `greeting_green-0.0.4/pyproject.toml` & `greeting_green-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -32,18 +32,17 @@
 Source = "https://github.com/unknown/greeting-green"
 
 [tool.hatch.version]
 path = "greeting/__init__.py"
 
 
 [tool.hatch.envs.default]
-dependencies = ["django"]
+dependencies = ["django", "greeting_green"]
 
 [tool.hatch.envs.default.scripts]
 test = "python3 manage.py test {args}"
 
 [tool.hatch.build]
 include = [
   "greeting/*",
-#  "greeting/templates",
-#  "greeting/static",
 ]
+exclude = ["greeting/migrations/*"]
```

### Comparing `greeting_green-0.0.4/PKG-INFO` & `greeting_green-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greeting-green
-Version: 0.0.4
+Version: 0.0.5
 Summary: test
 Project-URL: Documentation, https://github.com/unknown/greeting-green#readme
 Project-URL: Issues, https://github.com/unknown/greeting-green/issues
 Project-URL: Source, https://github.com/unknown/greeting-green
 Author-email: Warise <example@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

