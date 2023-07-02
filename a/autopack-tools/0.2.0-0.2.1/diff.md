# Comparing `tmp/autopack_tools-0.2.0.tar.gz` & `tmp/autopack_tools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.2.0.tar", max compression
+gzip compressed data, was "autopack_tools-0.2.1.tar", max compression
```

## Comparing `autopack_tools-0.2.0.tar` & `autopack_tools-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.0/LICENSE
--rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.0/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.0/autopack/VERSION
--rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.0/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.0/autopack/__main__.py
--rw-r--r--   0        0        0     2870 2023-06-30 20:09:47.859652 autopack_tools-0.2.0/autopack/api.py
--rw-r--r--   0        0        0     1116 2023-06-30 20:09:47.833824 autopack_tools-0.2.0/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.0/autopack/errors.py
--rw-r--r--   0        0        0     2698 2023-06-30 20:09:48.256517 autopack_tools-0.2.0/autopack/get_pack.py
--rw-r--r--   0        0        0     3877 2023-07-02 21:30:44.097116 autopack_tools-0.2.0/autopack/installation.py
--rw-r--r--   0        0        0     2921 2023-06-30 20:09:47.867664 autopack_tools-0.2.0/autopack/pack.py
--rw-r--r--   0        0        0      636 2023-06-30 20:05:59.914181 autopack_tools-0.2.0/autopack/pack_response.py
--rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.0/autopack/search.py
--rw-r--r--   0        0        0     2628 2023-07-02 21:50:44.992073 autopack_tools-0.2.0/autopack/selection.py
--rw-r--r--   0        0        0     4450 2023-07-02 21:30:44.111776 autopack_tools-0.2.0/autopack/utils.py
--rw-r--r--   0        0        0      910 2023-07-02 21:53:27.971841 autopack_tools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3666 1970-01-01 00:00:00.000000 autopack_tools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.1/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.1/autopack/VERSION
+-rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.1/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.1/autopack/__main__.py
+-rw-r--r--   0        0        0     2870 2023-06-30 20:09:47.859652 autopack_tools-0.2.1/autopack/api.py
+-rw-r--r--   0        0        0     1116 2023-06-30 20:09:47.833824 autopack_tools-0.2.1/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.1/autopack/errors.py
+-rw-r--r--   0        0        0     2698 2023-06-30 20:09:48.256517 autopack_tools-0.2.1/autopack/get_pack.py
+-rw-r--r--   0        0        0     3877 2023-07-02 21:30:44.097116 autopack_tools-0.2.1/autopack/installation.py
+-rw-r--r--   0        0        0     2921 2023-06-30 20:09:47.867664 autopack_tools-0.2.1/autopack/pack.py
+-rw-r--r--   0        0        0      636 2023-06-30 20:05:59.914181 autopack_tools-0.2.1/autopack/pack_response.py
+-rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.1/autopack/search.py
+-rw-r--r--   0        0        0     2773 2023-07-02 22:58:29.476822 autopack_tools-0.2.1/autopack/selection.py
+-rw-r--r--   0        0        0     4450 2023-07-02 21:30:44.111776 autopack_tools-0.2.1/autopack/utils.py
+-rw-r--r--   0        0        0      910 2023-07-02 22:58:35.269800 autopack_tools-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3666 1970-01-01 00:00:00.000000 autopack_tools-0.2.1/PKG-INFO
```

### Comparing `autopack_tools-0.2.0/LICENSE` & `autopack_tools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.0/README.md` & `autopack_tools-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.0/autopack/api.py` & `autopack_tools-0.2.1/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.0/autopack/cli.py` & `autopack_tools-0.2.1/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.0/autopack/get_pack.py` & `autopack_tools-0.2.1/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.0/autopack/installation.py` & `autopack_tools-0.2.1/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.0/autopack/pack.py` & `autopack_tools-0.2.1/autopack/pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.0/autopack/pack_response.py` & `autopack_tools-0.2.1/autopack/pack_response.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.0/autopack/selection.py` & `autopack_tools-0.2.1/autopack/selection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
+from json import JSONDecodeError
 
 from langchain.chat_models.base import BaseChatModel
 from langchain.schema import HumanMessage
 
 from autopack.api import pack_search
 
 TOOL_SELECTION_PROMPT = """
-I have a list of tools to choose from and a task I need to accomplish. Please tell me all of the tools that are
-necessary for me to accomplish my task. Respond only with the tool_ids as a valid JSON array.
+I have a list of tools to choose from and a task I need to accomplish. Give me, as a valid JSON array, a list of the
+Tool IDs that are necessary to complete this task. Return only the JSON array and no other content.
 
 ---- TASK ----
 {user_input}
 ---- TOOLS ----
 {tools_string}
 """
 
@@ -69,8 +70,13 @@
 
 
 def ask_llm(prompt: str, llm: BaseChatModel):
     """Encapsulate the OpenAI specific stuff to easier support other frameworks in the future"""
     message = HumanMessage(content=prompt)
 
     response = llm(messages=[message])
-    return json.loads(response.content)
+
+    try:
+        return json.loads(response.content)
+    except JSONDecodeError as e:
+        # TODO: Better handle error
+        return []
```

### Comparing `autopack_tools-0.2.0/autopack/utils.py` & `autopack_tools-0.2.1/autopack/utils.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.0/pyproject.toml` & `autopack_tools-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.2.0"
+version = "0.2.1"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
```

### Comparing `autopack_tools-0.2.0/PKG-INFO` & `autopack_tools-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.2.0
+Version: 0.2.1
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

