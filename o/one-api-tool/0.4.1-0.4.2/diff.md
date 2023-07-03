# Comparing `tmp/one-api-tool-0.4.1.tar.gz` & `tmp/one-api-tool-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.4.1.tar", last modified: Mon Jul  3 11:08:23 2023, max compression
+gzip compressed data, was "one-api-tool-0.4.2.tar", last modified: Mon Jul  3 11:12:54 2023, max compression
```

## Comparing `one-api-tool-0.4.1.tar` & `one-api-tool-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 11:08:23.926305 one-api-tool-0.4.1/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.4.1/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-03 11:08:23.926020 one-api-tool-0.4.1/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     4172 2023-07-02 05:43:55.000000 one-api-tool-0.4.1/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 11:08:23.924371 one-api-tool-0.4.1/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-03 11:08:23.000000 one-api-tool-0.4.1/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      359 2023-07-03 11:08:23.000000 one-api-tool-0.4.1/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-03 11:08:23.000000 one-api-tool-0.4.1/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-03 11:08:23.000000 one-api-tool-0.4.1/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       86 2023-07-03 11:08:23.000000 one-api-tool-0.4.1/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-03 11:08:23.000000 one-api-tool-0.4.1/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 11:08:23.925028 one-api-tool-0.4.1/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.4.1/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 11:08:23.925486 one-api-tool-0.4.1/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.4.1/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.4.1/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    13366 2023-07-03 11:07:07.000000 one-api-tool-0.4.1/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3696 2023-07-03 10:39:09.000000 one-api-tool-0.4.1/oneapi/utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-03 11:08:23.926452 one-api-tool-0.4.1/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1078 2023-07-03 10:58:20.000000 one-api-tool-0.4.1/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 11:12:54.436479 one-api-tool-0.4.2/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.4.2/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-03 11:12:54.436247 one-api-tool-0.4.2/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4172 2023-07-02 05:43:55.000000 one-api-tool-0.4.2/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 11:12:54.435044 one-api-tool-0.4.2/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-03 11:12:54.000000 one-api-tool-0.4.2/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      359 2023-07-03 11:12:54.000000 one-api-tool-0.4.2/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-03 11:12:54.000000 one-api-tool-0.4.2/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-03 11:12:54.000000 one-api-tool-0.4.2/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       86 2023-07-03 11:12:54.000000 one-api-tool-0.4.2/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-03 11:12:54.000000 one-api-tool-0.4.2/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 11:12:54.435652 one-api-tool-0.4.2/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.4.2/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 11:12:54.436016 one-api-tool-0.4.2/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.4.2/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.4.2/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    13366 2023-07-03 11:07:07.000000 one-api-tool-0.4.2/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3598 2023-07-03 11:12:47.000000 one-api-tool-0.4.2/oneapi/utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-03 11:12:54.436555 one-api-tool-0.4.2/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1078 2023-07-03 11:12:40.000000 one-api-tool-0.4.2/setup.py
```

### Comparing `one-api-tool-0.4.1/LICENSE` & `one-api-tool-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.1/PKG-INFO` & `one-api-tool-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.4.1
+Version: 0.4.2
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.4.1/README.md` & `one-api-tool-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.1/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.4.2/one_api_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.4.1
+Version: 0.4.2
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.4.1/oneapi/commands/one_api_requst.py` & `one-api-tool-0.4.2/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.1/oneapi/one_api.py` & `one-api-tool-0.4.2/oneapi/one_api.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.4.1/oneapi/utils.py` & `one-api-tool-0.4.2/oneapi/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         default_value = arg.default if arg.default != inspect.Parameter.empty else None
         type_annotation = arg.annotation if arg.annotation != inspect.Parameter.empty else None
         param_description = {}
         # if default_value is not None:
             # param_description["default"] = default_value
         if type_annotation is not None:
             json_schema_type_name = python_type_to_json_type(type_annotation)
-            print(f'tyoename: {type_annotation}, json_schema_type_name: {json_schema_type_name}')
             param_description["type"] = json_schema_type_name
             if json_schema_type_name == 'array':
                 if '__args__' in dir(type_annotation) and len(type_annotation.__args__) > 0:
                     param_description["items"] = {
                         "type": python_type_to_json_type(type_annotation.__args__[0])
                     }
                 else:
```

### Comparing `one-api-tool-0.4.1/setup.py` & `one-api-tool-0.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.4.1",
+    version="0.4.2",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

