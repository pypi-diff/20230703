# Comparing `tmp/mvc4kivy-0.1.7.tar.gz` & `tmp/mvc4kivy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvc4kivy-0.1.7.tar", max compression
+gzip compressed data, was "mvc4kivy-0.1.8.tar", max compression
```

## Comparing `mvc4kivy-0.1.7.tar` & `mvc4kivy-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3255 2023-04-29 08:24:08.275191 mvc4kivy-0.1.7/mvc4kivy/__init__.py
--rw-r--r--   0        0        0     7099 2023-07-02 20:32:36.495234 mvc4kivy-0.1.7/mvc4kivy/add_view.py
--rw-r--r--   0        0        0    42626 2023-07-02 20:30:59.819997 mvc4kivy-0.1.7/mvc4kivy/create_project.py
--rw-r--r--   0        0        0        0 2023-04-28 04:02:52.301767 mvc4kivy-0.1.7/mvc4kivy/MVC/__init__.py
--rw-r--r--   0        0        0      425 2023-04-28 04:02:52.308770 mvc4kivy-0.1.7/mvc4kivy/MVC/data/locales/po/en.po
--rw-r--r--   0        0        0      425 2023-04-28 04:02:52.309769 mvc4kivy-0.1.7/mvc4kivy/MVC/data/locales/po/ru.po
--rw-r--r--   0        0        0     1202 2023-04-29 08:55:56.501660 mvc4kivy-0.1.7/mvc4kivy/MVC/libs/__init__.py
--rw-r--r--   0        0        0     1411 2023-04-28 04:02:52.312767 mvc4kivy-0.1.7/mvc4kivy/MVC/libs/translation.py
--rw-r--r--   0        0        0      582 2023-04-28 04:02:52.302769 mvc4kivy-0.1.7/mvc4kivy/MVC/messages.pot
--rw-r--r--   0        0        0        0 2023-04-28 04:02:52.303773 mvc4kivy-0.1.7/mvc4kivy/MVC/Model/__init__.py
--rw-r--r--   0        0        0      827 2023-04-28 04:21:40.764773 mvc4kivy-0.1.7/mvc4kivy/MVC/Model/database_firebase.py
--rw-r--r--   0        0        0     3675 2023-04-28 04:21:40.785037 mvc4kivy-0.1.7/mvc4kivy/MVC/Model/database_restdb.py
--rw-r--r--   0        0        0      537 2023-07-02 20:33:44.551613 mvc4kivy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      231 2023-04-29 04:31:06.582521 mvc4kivy-0.1.7/README.md
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 mvc4kivy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3255 2023-04-29 08:24:08.275191 mvc4kivy-0.1.8/mvc4kivy/__init__.py
+-rw-r--r--   0        0        0     7101 2023-07-02 22:44:12.570310 mvc4kivy-0.1.8/mvc4kivy/add_view.py
+-rw-r--r--   0        0        0    42628 2023-07-02 22:44:12.533157 mvc4kivy-0.1.8/mvc4kivy/create_project.py
+-rw-r--r--   0        0        0        0 2023-04-28 04:02:52.301767 mvc4kivy-0.1.8/mvc4kivy/MVC/__init__.py
+-rw-r--r--   0        0        0      425 2023-04-28 04:02:52.308770 mvc4kivy-0.1.8/mvc4kivy/MVC/data/locales/po/en.po
+-rw-r--r--   0        0        0      425 2023-04-28 04:02:52.309769 mvc4kivy-0.1.8/mvc4kivy/MVC/data/locales/po/ru.po
+-rw-r--r--   0        0        0     1202 2023-04-29 08:55:56.501660 mvc4kivy-0.1.8/mvc4kivy/MVC/libs/__init__.py
+-rw-r--r--   0        0        0     1411 2023-04-28 04:02:52.312767 mvc4kivy-0.1.8/mvc4kivy/MVC/libs/translation.py
+-rw-r--r--   0        0        0      582 2023-04-28 04:02:52.302769 mvc4kivy-0.1.8/mvc4kivy/MVC/messages.pot
+-rw-r--r--   0        0        0        0 2023-04-28 04:02:52.303773 mvc4kivy-0.1.8/mvc4kivy/MVC/Model/__init__.py
+-rw-r--r--   0        0        0      827 2023-04-28 04:21:40.764773 mvc4kivy-0.1.8/mvc4kivy/MVC/Model/database_firebase.py
+-rw-r--r--   0        0        0     3675 2023-04-28 04:21:40.785037 mvc4kivy-0.1.8/mvc4kivy/MVC/Model/database_restdb.py
+-rw-r--r--   0        0        0      537 2023-07-02 22:45:06.187260 mvc4kivy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      231 2023-04-29 04:31:06.582521 mvc4kivy-0.1.8/README.md
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 mvc4kivy-0.1.8/PKG-INFO
```

### Comparing `mvc4kivy-0.1.7/mvc4kivy/__init__.py` & `mvc4kivy-0.1.8/mvc4kivy/__init__.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.7/mvc4kivy/add_view.py` & `mvc4kivy-0.1.8/mvc4kivy/add_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             "from Model.*Model|from Controller.*Controller", screen_module
         )
         screens = ""
         path_to_view = os.path.join(path_to_project, "View")
 
         for name in os.listdir(path_to_view):
             if os.path.isdir(os.path.join(path_to_view, name)):
-                res = re.findall("[A-Z][a-z]*", name)
+                res = re.findall(r"[A-Z][^A-Z]*", name)
                 # if res and len(res) == 2 and res[-1] == "Screen":
                 if res and len(res) > 1 and res[-1] == "Screen":
                     screens += (
                             "\n    '%s': {"
                             "\n        'model': %s,"
                             "\n        'controller': %s,"
                             "\n        'kv': %s"
```

### Comparing `mvc4kivy-0.1.7/mvc4kivy/create_project.py` & `mvc4kivy-0.1.8/mvc4kivy/create_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1196,15 +1196,15 @@
     os.rename(
         os.path.join(path_to_project, "Model", f"database_{name_database}.py"),
         os.path.join(path_to_project, "Model", "database.py"),
     )
 
 
 def chek_camel_case_name_project(name_project) -> Union[bool, list]:
-    result = re.findall("[A-Z][a-z]*", name_project)
+    result = re.findall(r"[A-Z][^A-Z]*", name_project)
     return False if len(result) == 1 else result
 
 
 def create_argument_parser() -> ArgumentParserWithHelp:
     parser = ArgumentParserWithHelp(
         prog="create_project.py",
         allow_abbrev=False,
```

### Comparing `mvc4kivy-0.1.7/mvc4kivy/MVC/libs/__init__.py` & `mvc4kivy-0.1.8/mvc4kivy/MVC/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.7/mvc4kivy/MVC/libs/translation.py` & `mvc4kivy-0.1.8/mvc4kivy/MVC/libs/translation.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.7/mvc4kivy/MVC/messages.pot` & `mvc4kivy-0.1.8/mvc4kivy/MVC/messages.pot`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.7/mvc4kivy/MVC/Model/database_firebase.py` & `mvc4kivy-0.1.8/mvc4kivy/MVC/Model/database_firebase.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.7/mvc4kivy/MVC/Model/database_restdb.py` & `mvc4kivy-0.1.8/mvc4kivy/MVC/Model/database_restdb.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.7/pyproject.toml` & `mvc4kivy-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mvc4kivy"
-version = "0.1.7"
+version = "0.1.8"
 description = "tool to create MVC project for kivy"
 authors = ["Kenechukwu Akubue <kengoon19@gmail.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "kivy"
 url = "https://kivy.org/downloads/simple"
```

### Comparing `mvc4kivy-0.1.7/PKG-INFO` & `mvc4kivy-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvc4kivy
-Version: 0.1.7
+Version: 0.1.8
 Summary: tool to create MVC project for kivy
 Author: Kenechukwu Akubue
 Author-email: kengoon19@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

