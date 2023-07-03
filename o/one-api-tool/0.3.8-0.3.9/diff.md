# Comparing `tmp/one-api-tool-0.3.8.tar.gz` & `tmp/one-api-tool-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.3.8.tar", last modified: Mon Jul  3 07:06:00 2023, max compression
+gzip compressed data, was "one-api-tool-0.3.9.tar", last modified: Mon Jul  3 07:21:13 2023, max compression
```

## Comparing `one-api-tool-0.3.8.tar` & `one-api-tool-0.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 07:06:00.577672 one-api-tool-0.3.8/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.3.8/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-03 07:06:00.577437 one-api-tool-0.3.8/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     4172 2023-07-02 05:43:55.000000 one-api-tool-0.3.8/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 07:06:00.576206 one-api-tool-0.3.8/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-03 07:06:00.000000 one-api-tool-0.3.8/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-07-03 07:06:00.000000 one-api-tool-0.3.8/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-03 07:06:00.000000 one-api-tool-0.3.8/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-03 07:06:00.000000 one-api-tool-0.3.8/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-07-03 07:06:00.000000 one-api-tool-0.3.8/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-03 07:06:00.000000 one-api-tool-0.3.8/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 07:06:00.576711 one-api-tool-0.3.8/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.3.8/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 07:06:00.576976 one-api-tool-0.3.8/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.3.8/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.3.8/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    12671 2023-07-03 07:04:34.000000 one-api-tool-0.3.8/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-03 07:06:00.577720 one-api-tool-0.3.8/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-07-03 07:05:56.000000 one-api-tool-0.3.8/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 07:21:13.770939 one-api-tool-0.3.9/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.3.9/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-03 07:21:13.770717 one-api-tool-0.3.9/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4172 2023-07-02 05:43:55.000000 one-api-tool-0.3.9/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 07:21:13.769925 one-api-tool-0.3.9/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-03 07:21:13.000000 one-api-tool-0.3.9/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-07-03 07:21:13.000000 one-api-tool-0.3.9/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-03 07:21:13.000000 one-api-tool-0.3.9/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-03 07:21:13.000000 one-api-tool-0.3.9/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-07-03 07:21:13.000000 one-api-tool-0.3.9/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-03 07:21:13.000000 one-api-tool-0.3.9/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 07:21:13.770201 one-api-tool-0.3.9/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.3.9/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 07:21:13.770502 one-api-tool-0.3.9/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.3.9/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.3.9/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    12685 2023-07-03 07:20:51.000000 one-api-tool-0.3.9/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-03 07:21:13.770987 one-api-tool-0.3.9/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-07-03 07:21:05.000000 one-api-tool-0.3.9/setup.py
```

### Comparing `one-api-tool-0.3.8/LICENSE` & `one-api-tool-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.8/PKG-INFO` & `one-api-tool-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.3.8
+Version: 0.3.9
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.3.8/README.md` & `one-api-tool-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.8/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.3.9/one_api_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.3.8
+Version: 0.3.9
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.3.8/oneapi/commands/one_api_requst.py` & `one-api-tool-0.3.9/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.8/oneapi/one_api.py` & `one-api-tool-0.3.9/oneapi/one_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
         https://learn.microsoft.com/en-us/azure/cognitive-services/openai/how-to/chatgpt?pivots=programming-language-chat-completions
         https://platform.openai.com/docs/api-reference/chat
         """
         data = args.dict()
         is_function_call = data.get("functions", None) is not None
         if is_function_call:
             data["stream"] = False  
+        else:
             data.pop("functions")
             data.pop("function_call")
         completion = openai.ChatCompletion.create(**data)
         if data.get("stream", False):
             # create variables to collect the stream of chunks
             collected_chunks = []
             collected_messages = []
```

### Comparing `one-api-tool-0.3.8/setup.py` & `one-api-tool-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.3.8",
+    version="0.3.9",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

