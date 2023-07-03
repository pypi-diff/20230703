# Comparing `tmp/openai_functions-0.6.4.tar.gz` & `tmp/openai_functions-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.6.4.tar", max compression
+gzip compressed data, was "openai_functions-0.6.5.tar", max compression
```

## Comparing `openai_functions-0.6.4.tar` & `openai_functions-0.6.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1065 2023-06-27 20:52:53.295744 openai_functions-0.6.4/LICENSE
--rw-r--r--   0        0        0     4343 2023-07-01 19:50:48.049062 openai_functions-0.6.4/README.md
--rw-r--r--   0        0        0      987 2023-07-01 15:53:29.387048 openai_functions-0.6.4/openai_functions/__init__.py
--rw-r--r--   0        0        0    12149 2023-07-01 19:46:31.233610 openai_functions-0.6.4/openai_functions/conversation.py
--rw-r--r--   0        0        0      613 2023-07-01 15:28:12.336941 openai_functions-0.6.4/openai_functions/functions/__init__.py
--rw-r--r--   0        0        0     3448 2023-07-01 15:32:10.388033 openai_functions-0.6.4/openai_functions/functions/basic_set.py
--rw-r--r--   0        0        0      378 2023-07-01 15:56:30.128412 openai_functions-0.6.4/openai_functions/functions/exceptions.py
--rw-r--r--   0        0        0     2625 2023-07-01 16:03:49.607132 openai_functions-0.6.4/openai_functions/functions/functions.py
--rw-r--r--   0        0        0     4389 2023-07-01 15:57:49.401955 openai_functions-0.6.4/openai_functions/functions/sets.py
--rw-r--r--   0        0        0     1678 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/functions/union.py
--rw-r--r--   0        0        0     7500 2023-07-01 16:09:18.414864 openai_functions-0.6.4/openai_functions/functions/wrapper.py
--rw-r--r--   0        0        0      160 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/json_type.py
--rw-r--r--   0        0        0     5511 2023-07-01 16:09:56.439055 openai_functions-0.6.4/openai_functions/nlp.py
--rw-r--r--   0        0        0     7790 2023-07-01 16:00:24.507942 openai_functions-0.6.4/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1788 2023-07-01 15:23:08.531382 openai_functions-0.6.4/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      975 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1641 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1194 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1067 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      520 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      993 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      691 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1273 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0        0 2023-06-27 20:52:53.296744 openai_functions-0.6.4/openai_functions/py.typed
--rw-r--r--   0        0        0     1038 2023-07-01 20:03:34.727316 openai_functions-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     5432 1970-01-01 00:00:00.000000 openai_functions-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-27 20:52:53.295744 openai_functions-0.6.5/LICENSE
+-rw-r--r--   0        0        0     4343 2023-07-01 19:50:48.049062 openai_functions-0.6.5/README.md
+-rw-r--r--   0        0        0      987 2023-07-01 15:53:29.387048 openai_functions-0.6.5/openai_functions/__init__.py
+-rw-r--r--   0        0        0    12205 2023-07-03 15:26:12.278168 openai_functions-0.6.5/openai_functions/conversation.py
+-rw-r--r--   0        0        0      613 2023-07-01 15:28:12.336941 openai_functions-0.6.5/openai_functions/functions/__init__.py
+-rw-r--r--   0        0        0     3448 2023-07-01 15:32:10.388033 openai_functions-0.6.5/openai_functions/functions/basic_set.py
+-rw-r--r--   0        0        0      378 2023-07-01 15:56:30.128412 openai_functions-0.6.5/openai_functions/functions/exceptions.py
+-rw-r--r--   0        0        0     2625 2023-07-01 16:03:49.607132 openai_functions-0.6.5/openai_functions/functions/functions.py
+-rw-r--r--   0        0        0     4389 2023-07-01 15:57:49.401955 openai_functions-0.6.5/openai_functions/functions/sets.py
+-rw-r--r--   0        0        0     1678 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/functions/union.py
+-rw-r--r--   0        0        0     7500 2023-07-01 16:09:18.414864 openai_functions-0.6.5/openai_functions/functions/wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/json_type.py
+-rw-r--r--   0        0        0     5511 2023-07-01 16:09:56.439055 openai_functions-0.6.5/openai_functions/nlp.py
+-rw-r--r--   0        0        0     7790 2023-07-01 16:00:24.507942 openai_functions-0.6.5/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1788 2023-07-01 15:23:08.531382 openai_functions-0.6.5/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      975 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1641 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1194 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1067 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      520 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      993 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      691 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1273 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2023-06-27 20:52:53.296744 openai_functions-0.6.5/openai_functions/py.typed
+-rw-r--r--   0        0        0     1038 2023-07-03 15:26:55.573413 openai_functions-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     5432 1970-01-01 00:00:00.000000 openai_functions-0.6.5/PKG-INFO
```

### Comparing `openai_functions-0.6.4/LICENSE` & `openai_functions-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/README.md` & `openai_functions-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/__init__.py` & `openai_functions-0.6.5/openai_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/conversation.py` & `openai_functions-0.6.5/openai_functions/conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,22 +363,23 @@
         """Add a skill to those available to the AI
 
         Args:
             skill (FunctionSet): The skill to add
         """
         self.skills.add_skill(skill)
 
-    def run(self, function: str, prompt: str) -> Any:
+    def run(self, function: str, prompt: str | None = None) -> Any:
         """Run a specified function and return the raw function result
 
         Args:
-            prompt (str): The prompt to use
             function (str): The function to run
+            prompt (str | None): The prompt to use
 
         Returns:
             The raw function result
         """
-        self.add_message(prompt)
+        if prompt is not None:
+            self.add_message(prompt)
         # We can do type: ignore as we know we're forcing a function call
         response: FunctionCallMessage
         response = self.generate_message({"name": function})  # type: ignore
         return self.skills(response.function_call)
```

### Comparing `openai_functions-0.6.4/openai_functions/functions/__init__.py` & `openai_functions-0.6.5/openai_functions/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/functions/basic_set.py` & `openai_functions-0.6.5/openai_functions/functions/basic_set.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/functions/functions.py` & `openai_functions-0.6.5/openai_functions/functions/functions.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/functions/sets.py` & `openai_functions-0.6.5/openai_functions/functions/sets.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/functions/union.py` & `openai_functions-0.6.5/openai_functions/functions/union.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/functions/wrapper.py` & `openai_functions-0.6.5/openai_functions/functions/wrapper.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/nlp.py` & `openai_functions-0.6.5/openai_functions/nlp.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/openai_types.py` & `openai_functions-0.6.5/openai_functions/openai_types.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/parsers/abc.py` & `openai_functions-0.6.5/openai_functions/parsers/abc.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.6.5/openai_functions/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.6.5/openai_functions/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/parsers/default.py` & `openai_functions-0.6.5/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/parsers/dict_parser.py` & `openai_functions-0.6.5/openai_functions/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/parsers/enum_parser.py` & `openai_functions-0.6.5/openai_functions/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/parsers/float_parser.py` & `openai_functions-0.6.5/openai_functions/parsers/float_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/parsers/int_parser.py` & `openai_functions-0.6.5/openai_functions/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/parsers/list_parser.py` & `openai_functions-0.6.5/openai_functions/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/parsers/none_parser.py` & `openai_functions-0.6.5/openai_functions/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/openai_functions/parsers/union_parser.py` & `openai_functions-0.6.5/openai_functions/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.4/pyproject.toml` & `openai_functions-0.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.6.4"
+version = "0.6.5"
 description = "Simplifies the usage of OpenAI ChatGPT's function calling by generating the schemas and parsing OpenAI's responses for you."
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/rizerphe/openai-functions"
 documentation = "https://openai-functions.readthedocs.io/"
 keywords = ["nlp", "openai", "openai-api", "chatgpt", "chatgpt-api", "wrapper", "functions", "chatgpt-api", "openai-functions", "chatgpt-functions", "typing", "docstring", "docstrings", "decorators", "signatures", "parsing"]
 license = "MIT"
```

### Comparing `openai_functions-0.6.4/PKG-INFO` & `openai_functions-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.6.4
+Version: 0.6.5
 Summary: Simplifies the usage of OpenAI ChatGPT's function calling by generating the schemas and parsing OpenAI's responses for you.
 Home-page: https://github.com/rizerphe/openai-functions
 License: MIT
 Keywords: nlp,openai,openai-api,chatgpt,chatgpt-api,wrapper,functions,chatgpt-api,openai-functions,chatgpt-functions,typing,docstring,docstrings,decorators,signatures,parsing
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

