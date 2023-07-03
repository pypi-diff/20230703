# Comparing `tmp/openai_functions-0.6.8.tar.gz` & `tmp/openai_functions-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.6.8.tar", max compression
+gzip compressed data, was "openai_functions-0.6.9.tar", max compression
```

## Comparing `openai_functions-0.6.8.tar` & `openai_functions-0.6.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1065 2023-06-27 20:52:53.295744 openai_functions-0.6.8/LICENSE
--rw-r--r--   0        0        0     4343 2023-07-01 19:50:48.049062 openai_functions-0.6.8/README.md
--rw-r--r--   0        0        0      987 2023-07-01 15:53:29.387048 openai_functions-0.6.8/openai_functions/__init__.py
--rw-r--r--   0        0        0    13619 2023-07-03 16:49:32.459764 openai_functions-0.6.8/openai_functions/conversation.py
--rw-r--r--   0        0        0      673 2023-07-03 16:38:15.855619 openai_functions-0.6.8/openai_functions/functions/__init__.py
--rw-r--r--   0        0        0     3492 2023-07-03 15:54:52.480105 openai_functions-0.6.8/openai_functions/functions/basic_set.py
--rw-r--r--   0        0        0      378 2023-07-01 15:56:30.128412 openai_functions-0.6.8/openai_functions/functions/exceptions.py
--rw-r--r--   0        0        0     2859 2023-07-03 16:13:51.366353 openai_functions-0.6.8/openai_functions/functions/functions.py
--rw-r--r--   0        0        0     5312 2023-07-03 16:49:12.883833 openai_functions-0.6.8/openai_functions/functions/sets.py
--rw-r--r--   0        0        0     2785 2023-07-03 16:36:09.343274 openai_functions-0.6.8/openai_functions/functions/togglable_set.py
--rw-r--r--   0        0        0     1678 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/functions/union.py
--rw-r--r--   0        0        0     8295 2023-07-03 16:59:44.909844 openai_functions-0.6.8/openai_functions/functions/wrapper.py
--rw-r--r--   0        0        0      160 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/json_type.py
--rw-r--r--   0        0        0     6563 2023-07-03 16:57:04.415522 openai_functions-0.6.8/openai_functions/nlp.py
--rw-r--r--   0        0        0     7790 2023-07-01 16:00:24.507942 openai_functions-0.6.8/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1788 2023-07-01 15:23:08.531382 openai_functions-0.6.8/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      975 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1641 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1194 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1067 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      520 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      993 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      691 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1273 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0        0 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/py.typed
--rw-r--r--   0        0        0     1038 2023-07-03 17:00:46.365851 openai_functions-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     5432 1970-01-01 00:00:00.000000 openai_functions-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-27 20:52:53.295744 openai_functions-0.6.9/LICENSE
+-rw-r--r--   0        0        0     4343 2023-07-01 19:50:48.049062 openai_functions-0.6.9/README.md
+-rw-r--r--   0        0        0     1025 2023-07-03 17:02:22.824536 openai_functions-0.6.9/openai_functions/__init__.py
+-rw-r--r--   0        0        0    13619 2023-07-03 16:49:32.459764 openai_functions-0.6.9/openai_functions/conversation.py
+-rw-r--r--   0        0        0      673 2023-07-03 16:38:15.855619 openai_functions-0.6.9/openai_functions/functions/__init__.py
+-rw-r--r--   0        0        0     3492 2023-07-03 15:54:52.480105 openai_functions-0.6.9/openai_functions/functions/basic_set.py
+-rw-r--r--   0        0        0      378 2023-07-01 15:56:30.128412 openai_functions-0.6.9/openai_functions/functions/exceptions.py
+-rw-r--r--   0        0        0     2859 2023-07-03 16:13:51.366353 openai_functions-0.6.9/openai_functions/functions/functions.py
+-rw-r--r--   0        0        0     5312 2023-07-03 16:49:12.883833 openai_functions-0.6.9/openai_functions/functions/sets.py
+-rw-r--r--   0        0        0     2866 2023-07-03 17:12:00.200359 openai_functions-0.6.9/openai_functions/functions/togglable_set.py
+-rw-r--r--   0        0        0     1678 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/functions/union.py
+-rw-r--r--   0        0        0     8295 2023-07-03 16:59:44.909844 openai_functions-0.6.9/openai_functions/functions/wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/json_type.py
+-rw-r--r--   0        0        0     6563 2023-07-03 16:57:04.415522 openai_functions-0.6.9/openai_functions/nlp.py
+-rw-r--r--   0        0        0     7790 2023-07-01 16:00:24.507942 openai_functions-0.6.9/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1788 2023-07-01 15:23:08.531382 openai_functions-0.6.9/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      975 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1641 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1194 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1067 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      520 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      993 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      691 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1273 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/py.typed
+-rw-r--r--   0        0        0     1038 2023-07-03 17:14:53.297242 openai_functions-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     5432 1970-01-01 00:00:00.000000 openai_functions-0.6.9/PKG-INFO
```

### Comparing `openai_functions-0.6.8/LICENSE` & `openai_functions-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/README.md` & `openai_functions-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/__init__.py` & `openai_functions-0.6.9/openai_functions/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     FunctionNotFoundError,
     FunctionResult,
     FunctionSet,
     FunctionWrapper,
     MutableFunctionSet,
     OpenAIFunction,
     RawFunctionResult,
+    TogglableSet,
     UnionSkillSet,
     WrapperConfig,
 )
 from .nlp import NaturalLanguageAnnotated, Wrapper, nlp
 from .openai_types import FinalResponseMessage, FunctionCall, GenericMessage, Message
 from .parsers import ArgSchemaParser, defargparsers
 
@@ -24,14 +25,15 @@
     "defargparsers",
     "ArgSchemaParser",
     "FunctionWrapper",
     "MutableFunctionSet",
     "OpenAIFunction",
     "FunctionResult",
     "RawFunctionResult",
+    "TogglableSet",
     "UnionSkillSet",
     "WrapperConfig",
     "NaturalLanguageAnnotated",
     "nlp",
     "Wrapper",
     "FinalResponseMessage",
     "FunctionCall",
```

### Comparing `openai_functions-0.6.8/openai_functions/conversation.py` & `openai_functions-0.6.9/openai_functions/conversation.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/functions/__init__.py` & `openai_functions-0.6.9/openai_functions/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/functions/basic_set.py` & `openai_functions-0.6.9/openai_functions/functions/basic_set.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/functions/functions.py` & `openai_functions-0.6.9/openai_functions/functions/functions.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/functions/sets.py` & `openai_functions-0.6.9/openai_functions/functions/sets.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/functions/togglable_set.py` & `openai_functions-0.6.9/openai_functions/functions/togglable_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,18 @@
         self.enabled = True
 
     @property
     def _enable_function_schema(self) -> dict[str, JsonType]:
         """Get the schema for the enable function."""
         schema: dict[str, JsonType] = {
             "name": self.enable_function_name,
-            "parameters": {},
+            "parameters": {
+                "type": "object",
+                "properties": {},
+            },
         }
         if self.enable_function_description:
             schema["description"] = self.enable_function_description
         return schema
 
     @property
     def functions_schema(self) -> list[JsonType]:
```

### Comparing `openai_functions-0.6.8/openai_functions/functions/union.py` & `openai_functions-0.6.9/openai_functions/functions/union.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/functions/wrapper.py` & `openai_functions-0.6.9/openai_functions/functions/wrapper.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/nlp.py` & `openai_functions-0.6.9/openai_functions/nlp.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/openai_types.py` & `openai_functions-0.6.9/openai_functions/openai_types.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/parsers/abc.py` & `openai_functions-0.6.9/openai_functions/parsers/abc.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.6.9/openai_functions/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.6.9/openai_functions/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/parsers/default.py` & `openai_functions-0.6.9/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/parsers/dict_parser.py` & `openai_functions-0.6.9/openai_functions/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/parsers/enum_parser.py` & `openai_functions-0.6.9/openai_functions/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/parsers/float_parser.py` & `openai_functions-0.6.9/openai_functions/parsers/float_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/parsers/int_parser.py` & `openai_functions-0.6.9/openai_functions/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/parsers/list_parser.py` & `openai_functions-0.6.9/openai_functions/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/parsers/none_parser.py` & `openai_functions-0.6.9/openai_functions/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/openai_functions/parsers/union_parser.py` & `openai_functions-0.6.9/openai_functions/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.8/pyproject.toml` & `openai_functions-0.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.6.8"
+version = "0.6.9"
 description = "Simplifies the usage of OpenAI ChatGPT's function calling by generating the schemas and parsing OpenAI's responses for you."
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/rizerphe/openai-functions"
 documentation = "https://openai-functions.readthedocs.io/"
 keywords = ["nlp", "openai", "openai-api", "chatgpt", "chatgpt-api", "wrapper", "functions", "chatgpt-api", "openai-functions", "chatgpt-functions", "typing", "docstring", "docstrings", "decorators", "signatures", "parsing"]
 license = "MIT"
```

### Comparing `openai_functions-0.6.8/PKG-INFO` & `openai_functions-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.6.8
+Version: 0.6.9
 Summary: Simplifies the usage of OpenAI ChatGPT's function calling by generating the schemas and parsing OpenAI's responses for you.
 Home-page: https://github.com/rizerphe/openai-functions
 License: MIT
 Keywords: nlp,openai,openai-api,chatgpt,chatgpt-api,wrapper,functions,chatgpt-api,openai-functions,chatgpt-functions,typing,docstring,docstrings,decorators,signatures,parsing
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

