# Comparing `tmp/openai_functions-0.6.7.tar.gz` & `tmp/openai_functions-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.6.7.tar", max compression
+gzip compressed data, was "openai_functions-0.6.8.tar", max compression
```

## Comparing `openai_functions-0.6.7.tar` & `openai_functions-0.6.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1065 2023-06-27 20:52:53.295744 openai_functions-0.6.7/LICENSE
--rw-r--r--   0        0        0     4343 2023-07-01 19:50:48.049062 openai_functions-0.6.7/README.md
--rw-r--r--   0        0        0      987 2023-07-01 15:53:29.387048 openai_functions-0.6.7/openai_functions/__init__.py
--rw-r--r--   0        0        0    13036 2023-07-03 16:07:21.552365 openai_functions-0.6.7/openai_functions/conversation.py
--rw-r--r--   0        0        0      613 2023-07-01 15:28:12.336941 openai_functions-0.6.7/openai_functions/functions/__init__.py
--rw-r--r--   0        0        0     3492 2023-07-03 15:54:52.480105 openai_functions-0.6.7/openai_functions/functions/basic_set.py
--rw-r--r--   0        0        0        0 2023-07-03 15:33:41.826717 openai_functions-0.6.7/openai_functions/functions/disabled_set.py
--rw-r--r--   0        0        0      378 2023-07-01 15:56:30.128412 openai_functions-0.6.7/openai_functions/functions/exceptions.py
--rw-r--r--   0        0        0     2859 2023-07-03 16:13:51.366353 openai_functions-0.6.7/openai_functions/functions/functions.py
--rw-r--r--   0        0        0     4684 2023-07-03 15:57:43.485303 openai_functions-0.6.7/openai_functions/functions/sets.py
--rw-r--r--   0        0        0     1678 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/functions/union.py
--rw-r--r--   0        0        0     7920 2023-07-03 16:16:22.501957 openai_functions-0.6.7/openai_functions/functions/wrapper.py
--rw-r--r--   0        0        0      160 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/json_type.py
--rw-r--r--   0        0        0     5511 2023-07-01 16:09:56.439055 openai_functions-0.6.7/openai_functions/nlp.py
--rw-r--r--   0        0        0     7790 2023-07-01 16:00:24.507942 openai_functions-0.6.7/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1788 2023-07-01 15:23:08.531382 openai_functions-0.6.7/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      975 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1641 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1194 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1067 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      520 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      993 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      691 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1273 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0        0 2023-06-27 20:52:53.296744 openai_functions-0.6.7/openai_functions/py.typed
--rw-r--r--   0        0        0     1038 2023-07-03 16:17:47.136263 openai_functions-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     5432 1970-01-01 00:00:00.000000 openai_functions-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-27 20:52:53.295744 openai_functions-0.6.8/LICENSE
+-rw-r--r--   0        0        0     4343 2023-07-01 19:50:48.049062 openai_functions-0.6.8/README.md
+-rw-r--r--   0        0        0      987 2023-07-01 15:53:29.387048 openai_functions-0.6.8/openai_functions/__init__.py
+-rw-r--r--   0        0        0    13619 2023-07-03 16:49:32.459764 openai_functions-0.6.8/openai_functions/conversation.py
+-rw-r--r--   0        0        0      673 2023-07-03 16:38:15.855619 openai_functions-0.6.8/openai_functions/functions/__init__.py
+-rw-r--r--   0        0        0     3492 2023-07-03 15:54:52.480105 openai_functions-0.6.8/openai_functions/functions/basic_set.py
+-rw-r--r--   0        0        0      378 2023-07-01 15:56:30.128412 openai_functions-0.6.8/openai_functions/functions/exceptions.py
+-rw-r--r--   0        0        0     2859 2023-07-03 16:13:51.366353 openai_functions-0.6.8/openai_functions/functions/functions.py
+-rw-r--r--   0        0        0     5312 2023-07-03 16:49:12.883833 openai_functions-0.6.8/openai_functions/functions/sets.py
+-rw-r--r--   0        0        0     2785 2023-07-03 16:36:09.343274 openai_functions-0.6.8/openai_functions/functions/togglable_set.py
+-rw-r--r--   0        0        0     1678 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/functions/union.py
+-rw-r--r--   0        0        0     8295 2023-07-03 16:59:44.909844 openai_functions-0.6.8/openai_functions/functions/wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/json_type.py
+-rw-r--r--   0        0        0     6563 2023-07-03 16:57:04.415522 openai_functions-0.6.8/openai_functions/nlp.py
+-rw-r--r--   0        0        0     7790 2023-07-01 16:00:24.507942 openai_functions-0.6.8/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1788 2023-07-01 15:23:08.531382 openai_functions-0.6.8/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      975 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1641 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1194 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1067 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      520 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      993 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      691 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1273 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2023-06-27 20:52:53.296744 openai_functions-0.6.8/openai_functions/py.typed
+-rw-r--r--   0        0        0     1038 2023-07-03 17:00:46.365851 openai_functions-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0     5432 1970-01-01 00:00:00.000000 openai_functions-0.6.8/PKG-INFO
```

### Comparing `openai_functions-0.6.7/LICENSE` & `openai_functions-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/README.md` & `openai_functions-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/__init__.py` & `openai_functions-0.6.8/openai_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/conversation.py` & `openai_functions-0.6.8/openai_functions/conversation.py`

 * *Files 3% similar despite different names*

```diff
@@ -289,48 +289,57 @@
         ...
 
     @overload
     def add_function(
         self,
         function: Callable[..., JsonType],
         *,
+        name: str | None = None,
+        description: str | None = None,
         save_return: bool = True,
         serialize: bool = True,
         remove_call: bool = False,
         interpret_as_response: bool = False,
     ) -> Callable[..., JsonType]:
         ...
 
     @overload
     def add_function(
         self,
         *,
+        name: str | None = None,
+        description: str | None = None,
         save_return: bool = True,
         serialize: bool = True,
         remove_call: bool = False,
         interpret_as_response: bool = False,
     ) -> Callable[[Callable[..., JsonType]], Callable[..., JsonType]]:
         ...
 
     def add_function(
         self,
         function: OpenAIFunction | Callable[..., JsonType] | None = None,
         *,
+        name: str | None = None,
+        description: str | None = None,
         save_return: bool = True,
         serialize: bool = True,
         remove_call: bool = False,
         interpret_as_response: bool = False,
     ) -> (
         Callable[[Callable[..., JsonType]], Callable[..., JsonType]]
         | Callable[..., JsonType]
     ):
         """Add a function to the functions available to the AI
 
         Args:
             function (OpenAIFunction | Callable[..., JsonType]): The function to add
+            name (str): The name of the function. Defaults to the function's name.
+            description (str): The description of the function. Defaults to getting
+                the short description from the function's docstring.
             save_return (bool): Whether to send the return value of this function back
                 to the AI. Defaults to True.
             serialize (bool): Whether to serialize the return value of this function.
                 Otherwise, the return value must be a string.
             remove_call (bool): Whether to remove the function call itself from the chat
                 history
             interpret_as_response (bool): Whether to interpret the return value of this
@@ -338,21 +347,25 @@
 
         Returns:
             Callable[[Callable[..., JsonType]], Callable[..., JsonType]]: A decorator
             Callable[..., JsonType]: The original function
         """
         if function is None:
             return self.skills.add_function(
+                name=name,
+                description=description,
                 save_return=save_return,
                 serialize=serialize,
                 remove_call=remove_call,
                 interpret_as_response=interpret_as_response,
             )
         return self.skills.add_function(
             function,
+            name=name,
+            description=description,
             save_return=save_return,
             serialize=serialize,
             remove_call=remove_call,
             interpret_as_response=interpret_as_response,
         )
 
     def remove_function(
```

### Comparing `openai_functions-0.6.7/openai_functions/functions/__init__.py` & `openai_functions-0.6.8/openai_functions/functions/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """A set of tools responsible for managing the functions themselves."""
 from .basic_set import BasicFunctionSet
 from .exceptions import FunctionNotFoundError
 from .functions import FunctionResult, RawFunctionResult
 from .sets import FunctionSet, MutableFunctionSet, OpenAIFunction
+from .togglable_set import TogglableSet
 from .union import UnionSkillSet
 from .wrapper import FunctionWrapper, WrapperConfig
 
 __all__ = [
     "BasicFunctionSet",
     "FunctionNotFoundError",
     "FunctionResult",
     "RawFunctionResult",
     "FunctionSet",
     "MutableFunctionSet",
     "OpenAIFunction",
+    "TogglableSet",
     "UnionSkillSet",
     "FunctionWrapper",
     "WrapperConfig",
 ]
```

### Comparing `openai_functions-0.6.7/openai_functions/functions/basic_set.py` & `openai_functions-0.6.8/openai_functions/functions/basic_set.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/functions/functions.py` & `openai_functions-0.6.8/openai_functions/functions/functions.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/functions/sets.py` & `openai_functions-0.6.8/openai_functions/functions/sets.py`

 * *Files 15% similar despite different names*

```diff
@@ -55,48 +55,57 @@
         ...
 
     @overload
     def add_function(
         self,
         function: Callable[..., JsonType],
         *,
+        name: str | None = None,
+        description: str | None = None,
         save_return: bool = True,
         serialize: bool = True,
         remove_call: bool = False,
         interpret_as_response: bool = False,
     ) -> Callable[..., JsonType]:
         ...
 
     @overload
     def add_function(
         self,
         *,
+        name: str | None = None,
+        description: str | None = None,
         save_return: bool = True,
         serialize: bool = True,
         remove_call: bool = False,
         interpret_as_response: bool = False,
     ) -> Callable[[Callable[..., JsonType]], Callable[..., JsonType]]:
         ...
 
     def add_function(
         self,
         function: OpenAIFunction | Callable[..., JsonType] | None = None,
         *,
+        name: str | None = None,
+        description: str | None = None,
         save_return: bool = True,
         serialize: bool = True,
         remove_call: bool = False,
         interpret_as_response: bool = False,
     ) -> (
         Callable[[Callable[..., JsonType]], Callable[..., JsonType]]
         | Callable[..., JsonType]
     ):
         """Add a function
 
         Args:
             function (OpenAIFunction | Callable[..., JsonType]): The function
+            name (str): The name of the function. Defaults to the function's name.
+            description (str): The description of the function. Defaults to getting
+                the short description from the function's docstring.
             save_return (bool): Whether to send the return value of this
                 function to the AI. Defaults to True.
             serialize (bool): Whether to serialize the return value of this
                 function. Defaults to True. Otherwise, the return value must be a
                 string.
             remove_call (bool): Whether to remove the function call from the AI's
                 chat history. Defaults to False.
@@ -113,22 +122,27 @@
         if callable(function):
             self._add_function(
                 FunctionWrapper(
                     function,
                     WrapperConfig(
                         None, save_return, serialize, remove_call, interpret_as_response
                     ),
+                    name=name,
+                    description=description,
                 )
             )
             return function
 
         return partial(
             self.add_function,
+            name=name,
+            description=description,
             save_return=save_return,
             serialize=serialize,
+            remove_call=remove_call,
             interpret_as_response=interpret_as_response,
         )
 
     @abstractmethod
     def _remove_function(self, name: str) -> None:
         ...
```

### Comparing `openai_functions-0.6.7/openai_functions/functions/union.py` & `openai_functions-0.6.8/openai_functions/functions/union.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/functions/wrapper.py` & `openai_functions-0.6.8/openai_functions/functions/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,23 +51,29 @@
         config (WrapperConfig | None, optional): The configuration for the wrapper.
     """
 
     def __init__(
         self,
         func: Callable[..., Any],
         config: WrapperConfig | None = None,
+        name: str | None = None,
+        description: str | None = None,
     ) -> None:
         """Initialize a FunctionWrapper
 
         Args:
             func (Callable[..., JsonType]): The function to wrap
             config (WrapperConfig | None, optional): The configuration for the wrapper.
+            name (str | None): The name override for the function.
+            description (str | None): The description override for the function.
         """
         self.func = func
         self.config = config or WrapperConfig()
+        self._name = name
+        self._description = description
 
     @property
     def parsers(self) -> list[Type[ArgSchemaParser]]:
         """Get the parsers for this function
 
         Returns:
             list[Type[ArgSchemaParser]]: The parsers
@@ -181,15 +187,15 @@
     @property
     def name(self) -> str:
         """Get the name of this function
 
         Returns:
             str: The name
         """
-        return self.func.__name__
+        return self._name or self.func.__name__
 
     @property
     def schema(self) -> dict[str, JsonType]:
         """Get the schema for this function
 
         Returns:
             dict[str, JsonType]: The schema
@@ -198,16 +204,18 @@
             "name": self.name,
             "parameters": {
                 "type": "object",
                 "properties": self.arguments_schema,
                 "required": self.required_arguments,
             },
         }
-        if self.parsed_docs.short_description:
-            schema["description"] = self.parsed_docs.short_description
+        if self.parsed_docs.short_description or self._description:
+            schema["description"] = (
+                self.parsed_docs.short_description or self._description
+            )
         return schema
 
     def parse_argument(self, argument: inspect.Parameter) -> ArgSchemaParser:
         """Parse an argument
 
         Args:
             argument (inspect.Parameter): The argument to parse
```

### Comparing `openai_functions-0.6.7/openai_functions/openai_types.py` & `openai_functions-0.6.8/openai_functions/openai_types.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/parsers/abc.py` & `openai_functions-0.6.8/openai_functions/parsers/abc.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.6.8/openai_functions/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.6.8/openai_functions/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/parsers/default.py` & `openai_functions-0.6.8/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/parsers/dict_parser.py` & `openai_functions-0.6.8/openai_functions/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/parsers/enum_parser.py` & `openai_functions-0.6.8/openai_functions/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/parsers/float_parser.py` & `openai_functions-0.6.8/openai_functions/parsers/float_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/parsers/int_parser.py` & `openai_functions-0.6.8/openai_functions/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/parsers/list_parser.py` & `openai_functions-0.6.8/openai_functions/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/parsers/none_parser.py` & `openai_functions-0.6.8/openai_functions/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/openai_functions/parsers/union_parser.py` & `openai_functions-0.6.8/openai_functions/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.7/pyproject.toml` & `openai_functions-0.6.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.6.7"
+version = "0.6.8"
 description = "Simplifies the usage of OpenAI ChatGPT's function calling by generating the schemas and parsing OpenAI's responses for you."
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/rizerphe/openai-functions"
 documentation = "https://openai-functions.readthedocs.io/"
 keywords = ["nlp", "openai", "openai-api", "chatgpt", "chatgpt-api", "wrapper", "functions", "chatgpt-api", "openai-functions", "chatgpt-functions", "typing", "docstring", "docstrings", "decorators", "signatures", "parsing"]
 license = "MIT"
```

### Comparing `openai_functions-0.6.7/PKG-INFO` & `openai_functions-0.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.6.7
+Version: 0.6.8
 Summary: Simplifies the usage of OpenAI ChatGPT's function calling by generating the schemas and parsing OpenAI's responses for you.
 Home-page: https://github.com/rizerphe/openai-functions
 License: MIT
 Keywords: nlp,openai,openai-api,chatgpt,chatgpt-api,wrapper,functions,chatgpt-api,openai-functions,chatgpt-functions,typing,docstring,docstrings,decorators,signatures,parsing
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

