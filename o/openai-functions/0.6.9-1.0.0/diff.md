# Comparing `tmp/openai_functions-0.6.9.tar.gz` & `tmp/openai_functions-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.6.9.tar", max compression
+gzip compressed data, was "openai_functions-1.0.0.tar", max compression
```

## Comparing `openai_functions-0.6.9.tar` & `openai_functions-1.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1065 2023-06-27 20:52:53.295744 openai_functions-0.6.9/LICENSE
--rw-r--r--   0        0        0     4343 2023-07-01 19:50:48.049062 openai_functions-0.6.9/README.md
--rw-r--r--   0        0        0     1025 2023-07-03 17:02:22.824536 openai_functions-0.6.9/openai_functions/__init__.py
--rw-r--r--   0        0        0    13619 2023-07-03 16:49:32.459764 openai_functions-0.6.9/openai_functions/conversation.py
--rw-r--r--   0        0        0      673 2023-07-03 16:38:15.855619 openai_functions-0.6.9/openai_functions/functions/__init__.py
--rw-r--r--   0        0        0     3492 2023-07-03 15:54:52.480105 openai_functions-0.6.9/openai_functions/functions/basic_set.py
--rw-r--r--   0        0        0      378 2023-07-01 15:56:30.128412 openai_functions-0.6.9/openai_functions/functions/exceptions.py
--rw-r--r--   0        0        0     2859 2023-07-03 16:13:51.366353 openai_functions-0.6.9/openai_functions/functions/functions.py
--rw-r--r--   0        0        0     5312 2023-07-03 16:49:12.883833 openai_functions-0.6.9/openai_functions/functions/sets.py
--rw-r--r--   0        0        0     2866 2023-07-03 17:12:00.200359 openai_functions-0.6.9/openai_functions/functions/togglable_set.py
--rw-r--r--   0        0        0     1678 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/functions/union.py
--rw-r--r--   0        0        0     8295 2023-07-03 16:59:44.909844 openai_functions-0.6.9/openai_functions/functions/wrapper.py
--rw-r--r--   0        0        0      160 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/json_type.py
--rw-r--r--   0        0        0     6563 2023-07-03 16:57:04.415522 openai_functions-0.6.9/openai_functions/nlp.py
--rw-r--r--   0        0        0     7790 2023-07-01 16:00:24.507942 openai_functions-0.6.9/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1788 2023-07-01 15:23:08.531382 openai_functions-0.6.9/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      975 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1641 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1194 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1067 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      520 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      993 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      691 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1273 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0        0 2023-06-27 20:52:53.296744 openai_functions-0.6.9/openai_functions/py.typed
--rw-r--r--   0        0        0     1038 2023-07-03 17:14:53.297242 openai_functions-0.6.9/pyproject.toml
--rw-r--r--   0        0        0     5432 1970-01-01 00:00:00.000000 openai_functions-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-27 20:52:53.295744 openai_functions-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4343 2023-07-01 19:50:48.049062 openai_functions-1.0.0/README.md
+-rw-r--r--   0        0        0     1321 2023-07-03 18:45:03.184251 openai_functions-1.0.0/openai_functions/__init__.py
+-rw-r--r--   0        0        0    16086 2023-07-03 19:17:19.125358 openai_functions-1.0.0/openai_functions/conversation.py
+-rw-r--r--   0        0        0     3143 2023-07-03 19:09:31.548559 openai_functions-1.0.0/openai_functions/exceptions.py
+-rw-r--r--   0        0        0      598 2023-07-03 18:11:05.502726 openai_functions-1.0.0/openai_functions/functions/__init__.py
+-rw-r--r--   0        0        0     3721 2023-07-03 19:21:05.142443 openai_functions-1.0.0/openai_functions/functions/basic_set.py
+-rw-r--r--   0        0        0     2925 2023-07-03 18:11:37.691842 openai_functions-1.0.0/openai_functions/functions/functions.py
+-rw-r--r--   0        0        0     5223 2023-07-03 18:05:56.209166 openai_functions-1.0.0/openai_functions/functions/sets.py
+-rw-r--r--   0        0        0     2938 2023-07-03 19:08:39.118417 openai_functions-1.0.0/openai_functions/functions/togglable_set.py
+-rw-r--r--   0        0        0     1679 2023-07-03 18:11:52.146897 openai_functions-1.0.0/openai_functions/functions/union.py
+-rw-r--r--   0        0        0     8767 2023-07-03 19:21:15.762496 openai_functions-1.0.0/openai_functions/functions/wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-27 20:52:53.296744 openai_functions-1.0.0/openai_functions/json_type.py
+-rw-r--r--   0        0        0     7584 2023-07-03 19:24:01.157342 openai_functions-1.0.0/openai_functions/nlp.py
+-rw-r--r--   0        0        0     7790 2023-07-01 16:00:24.507942 openai_functions-1.0.0/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-27 20:52:53.296744 openai_functions-1.0.0/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1919 2023-07-03 18:25:04.287540 openai_functions-1.0.0/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0     1010 2023-07-03 18:26:32.249168 openai_functions-1.0.0/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-27 20:52:53.296744 openai_functions-1.0.0/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     2409 2023-07-03 18:31:30.405075 openai_functions-1.0.0/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-27 20:52:53.296744 openai_functions-1.0.0/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1243 2023-07-03 18:31:57.903109 openai_functions-1.0.0/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1441 2023-07-03 19:30:06.934301 openai_functions-1.0.0/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      568 2023-07-03 18:34:25.855420 openai_functions-1.0.0/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      690 2023-07-03 18:34:22.874412 openai_functions-1.0.0/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0     1042 2023-07-03 18:35:08.777545 openai_functions-1.0.0/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      734 2023-07-03 18:35:27.350603 openai_functions-1.0.0/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-27 20:52:53.296744 openai_functions-1.0.0/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1303 2023-07-03 18:36:04.876727 openai_functions-1.0.0/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2023-06-27 20:52:53.296744 openai_functions-1.0.0/openai_functions/py.typed
+-rw-r--r--   0        0        0     1038 2023-07-03 19:33:27.956411 openai_functions-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5432 1970-01-01 00:00:00.000000 openai_functions-1.0.0/PKG-INFO
```

### Comparing `openai_functions-0.6.9/LICENSE` & `openai_functions-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.9/README.md` & `openai_functions-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.9/openai_functions/__init__.py` & `openai_functions-1.0.0/openai_functions/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 """ChatGPT function calling based on function docstrings."""
 from .conversation import Conversation
+from .exceptions import (
+    BrokenSchemaError,
+    CannotParseTypeError,
+    FunctionNotFoundError,
+    InvalidJsonError,
+    NonSerializableOutputError,
+    OpenAIFunctionsError,
+)
 from .functions import (
     BasicFunctionSet,
-    FunctionNotFoundError,
     FunctionResult,
     FunctionSet,
     FunctionWrapper,
     MutableFunctionSet,
     OpenAIFunction,
     RawFunctionResult,
     TogglableSet,
@@ -15,16 +22,21 @@
 )
 from .nlp import NaturalLanguageAnnotated, Wrapper, nlp
 from .openai_types import FinalResponseMessage, FunctionCall, GenericMessage, Message
 from .parsers import ArgSchemaParser, defargparsers
 
 __all__ = [
     "Conversation",
-    "BasicFunctionSet",
+    "BrokenSchemaError",
+    "CannotParseTypeError",
     "FunctionNotFoundError",
+    "InvalidJsonError",
+    "NonSerializableOutputError",
+    "OpenAIFunctionsError",
+    "BasicFunctionSet",
     "FunctionSet",
     "defargparsers",
     "ArgSchemaParser",
     "FunctionWrapper",
     "MutableFunctionSet",
     "OpenAIFunction",
     "FunctionResult",
```

### Comparing `openai_functions-0.6.9/openai_functions/conversation.py` & `openai_functions-1.0.0/openai_functions/conversation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """A module for running OpenAI functions"""
 from __future__ import annotations
+import time
 from typing import Any, Callable, Literal, TYPE_CHECKING, overload
 
 import openai
+import openai.error
 
 from .functions.union import UnionSkillSet
 from .openai_types import (
     FinalResponseMessage,
     FinalResponseMessageType,
     ForcedFunctionCall,
     FunctionCallMessage,
@@ -95,48 +97,98 @@
 
     def clear_messages(self) -> None:
         """Fully clear the messages, but keep the skillset"""
         self.messages = []
 
     @overload
     def _generate_message(
-        self, function_call: ForcedFunctionCall
+        self, function_call: ForcedFunctionCall, retries: int | None = 1
     ) -> IntermediateResponseMessageType:
         ...
 
     @overload
     def _generate_message(
-        self, function_call: Literal["none"]
+        self, function_call: Literal["none"], retries: int | None = 1
     ) -> FinalResponseMessageType:
         ...
 
     @overload
     def _generate_message(
-        self, function_call: Literal["auto"] = "auto"
+        self, function_call: Literal["auto"] = "auto", retries: int | None = 1
     ) -> NonFunctionMessageType:
         ...
 
     def _generate_message(
-        self, function_call: OpenAiFunctionCallInput = "auto"
+        self, function_call: OpenAiFunctionCallInput = "auto", retries: int | None = 1
     ) -> NonFunctionMessageType:
-        """Generate a response
+        """Generate a response, retrying if necessary
 
         Args:
             function_call (OpenAiFunctionCallInput): The function call.
+            retries (int | None): The number of retries. Defaults to 4.
+                Will retry indefinitely if None.
+
+        Raises:
+            openai.error.RateLimitError: If the rate limit is exceeded
 
         Returns:
             NonFunctionMessageType: The response
         """
-        response = openai.ChatCompletion.create(
+        if retries is None:
+            retries = -1
+        while True:
+            try:
+                response = self._generate_raw_message(function_call)
+            except openai.error.RateLimitError as error:
+                if retries == 0:
+                    raise
+                retries -= 1
+                time.sleep(self._retry_time_from_headers(error.headers))
+            else:
+                return response["choices"][0]["message"]  # type: ignore
+
+    def _parse_retry_time(self, wait_for: str) -> float:
+        """Parse the time returned by an x-ratelimit-reset-requests header
+
+        Args:
+            wait_for (str): The time
+
+        Returns:
+            float: The time to the next reset
+        """
+        return float(wait_for[:-1]) * {"s": 1, "m": 60, "h": 3600}[wait_for[-1]]
+
+    def _retry_time_from_headers(self, headers: dict[str, str]) -> float:
+        """Get the time returned by the headers of an 429 reply
+
+        Args:
+            headers (dict[str, str]): The headers of the reply
+
+        Returns:
+            float: The time to wait for before retrying
+        """
+        return self._parse_retry_time(headers["x-ratelimit-reset-requests"]) / int(
+            headers["x-ratelimit-limit-requests"]
+        )
+
+    def _generate_raw_message(self, function_call: OpenAiFunctionCallInput) -> Any:
+        """Generate a raw OpenAI response
+
+        Args:
+            function_call (OpenAiFunctionCallInput): The function call.
+
+        Returns:
+            The raw OpenAI response
+        """
+        return openai.ChatCompletion.create(
             model=self.model,
             messages=[message.as_dict() for message in self.messages],
             functions=self.functions_schema,
             function_call=function_call,
         )
-        return response["choices"][0]["message"]  # type: ignore
 
     def remove_function_call(self, function_name: str) -> None:
         """Remove a function call from the messages, if it is the last message
 
         Args:
             function_name (str): The function name
         """
@@ -242,48 +294,53 @@
         function_call = self.messages[-1].function_call
         if not function_call:
             return False
 
         return self.run_function_and_substitute(function_call)
 
     def generate_message(
-        self, function_call: OpenAiFunctionCallInput = "auto"
+        self, function_call: OpenAiFunctionCallInput = "auto", retries: int | None = 1
     ) -> GenericMessage:
         """Generate the next message. Will run a function if the last message
         was a function call and the function call is not being overridden;
         if the function does not save the return a message will still be generated.
 
         Args:
             function_call (OpenAiFunctionCallInput): The function call
+            retries (int | None): The number of retries; if None, will retry
+                indefinitely
 
         Returns:
             GenericMessage: The response
         """
         if function_call in ["auto", "none"] and self.run_function_if_needed():
             return self.messages[-1]
 
-        message: NonFunctionMessageType = self._generate_message(function_call)
+        message: NonFunctionMessageType = self._generate_message(function_call, retries)
         self.add_message(message)
         return Message(message)
 
     def run_until_response(
-        self, allow_function_calls: bool = True
+        self, allow_function_calls: bool = True, retries: int | None = 1
     ) -> FinalResponseMessage:
         """Run functions query the AI until a response is generated
 
         Args:
             allow_function_calls (bool): Whether to allow the AI to call functions
+            retries (int | None): The number of retries; if None, will retry
+                indefinitely
 
         Returns:
             FinalResponseMessage: The final response, either from the AI or a function
                 that has interpret_as_response set to True
         """
         while True:
             message = self.generate_message(
-                function_call="auto" if allow_function_calls else "none"
+                function_call="auto" if allow_function_calls else "none",
+                retries=retries,
             )
             if is_final_response_message(message):
                 return message
 
     @overload
     def add_function(self, function: OpenAIFunction) -> OpenAIFunction:
         ...
@@ -374,43 +431,51 @@
         """Remove a function
 
         Args:
             function (str | OpenAIFunction | Callable[..., JsonType]): The function
         """
         self.skills.remove_function(function)
 
-    def ask(self, question: str) -> str:
+    def ask(self, question: str, retries: int | None = 1) -> str:
         """Ask the AI a question, running until a response is generated
 
         Args:
             question (str): The question
+            retries (int | None): The number of retries; if None, will retry
+                indefinitely
 
         Returns:
             str: The answer to the question
         """
         self.add_message(question)
-        return self.run_until_response().content
+        return self.run_until_response(retries=retries).content
 
     def add_skill(self, skill: FunctionSet) -> None:
         """Add a skill to those available to the AI
 
         Args:
             skill (FunctionSet): The skill to add
         """
         self.skills.add_skill(skill)
 
-    def run(self, function: str, prompt: str | None = None) -> Any:
+    def run(
+        self, function: str, prompt: str | None = None, retries: int | None = 1
+    ) -> Any:
         """Run a specified function and return the raw function result
 
         Args:
             function (str): The function to run
             prompt (str | None): The prompt to use
+            retries (int | None): The number of retries; if None, will retry
+                indefinitely
 
         Returns:
             The raw function result
         """
         if prompt is not None:
             self.add_message(prompt)
         # We can do type: ignore as we know we're forcing a function call
         response: FunctionCallMessage
-        response = self.generate_message({"name": function})  # type: ignore
+        response = self.generate_message(
+            {"name": function}, retries=retries
+        )  # type: ignore
         return self.skills(response.function_call)
```

### Comparing `openai_functions-0.6.9/openai_functions/functions/__init__.py` & `openai_functions-1.0.0/openai_functions/functions/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """A set of tools responsible for managing the functions themselves."""
 from .basic_set import BasicFunctionSet
-from .exceptions import FunctionNotFoundError
 from .functions import FunctionResult, RawFunctionResult
 from .sets import FunctionSet, MutableFunctionSet, OpenAIFunction
 from .togglable_set import TogglableSet
 from .union import UnionSkillSet
 from .wrapper import FunctionWrapper, WrapperConfig
 
 __all__ = [
     "BasicFunctionSet",
-    "FunctionNotFoundError",
     "FunctionResult",
     "RawFunctionResult",
     "FunctionSet",
     "MutableFunctionSet",
     "OpenAIFunction",
     "TogglableSet",
     "UnionSkillSet",
```

### Comparing `openai_functions-0.6.9/openai_functions/functions/basic_set.py` & `openai_functions-1.0.0/openai_functions/functions/basic_set.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """A module for running OpenAI functions"""
 from __future__ import annotations
 import json
 from typing import TYPE_CHECKING
 
-from .exceptions import FunctionNotFoundError
+from ..exceptions import FunctionNotFoundError, InvalidJsonError
 from .functions import FunctionResult, OpenAIFunction, RawFunctionResult
 from .sets import MutableFunctionSet
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
     from ..openai_types import FunctionCall
 
@@ -43,17 +43,22 @@
             input_data (FunctionCall): The function call
 
         Returns:
             FunctionResult: The function output
 
         Raises:
             FunctionNotFoundError: If the function is not found
+            InvalidJsonError: If the arguments are not valid JSON
         """
         function = self.find_function(input_data["name"])
-        result = self.get_function_result(function, json.loads(input_data["arguments"]))
+        try:
+            arguments = json.loads(input_data["arguments"])
+        except json.decoder.JSONDecodeError as err:
+            raise InvalidJsonError(input_data["arguments"]) from err
+        result = self.get_function_result(function, arguments)
         return FunctionResult(
             function.name, result, function.remove_call, function.interpret_as_response
         )
 
     def find_function(self, function_name: str) -> OpenAIFunction:
         """Find a function in the skillset
 
@@ -65,15 +70,15 @@
 
         Raises:
             FunctionNotFoundError: If the function is not found
         """
         for function in self.functions:
             if function.name == function_name:
                 return function
-        raise FunctionNotFoundError(f"Function {function_name} not found")
+        raise FunctionNotFoundError(function_name)
 
     def get_function_result(
         self, function: OpenAIFunction, arguments: dict[str, JsonType]
     ) -> RawFunctionResult | None:
         """Get the result of a function's execution
 
         Args:
```

### Comparing `openai_functions-0.6.9/openai_functions/functions/functions.py` & `openai_functions-1.0.0/openai_functions/functions/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """A module for running OpenAI functions"""
 from __future__ import annotations
 from dataclasses import dataclass
 import json
 from typing import Any, Protocol, TYPE_CHECKING, runtime_checkable
 
-from .exceptions import NonSerializableOutputError
+from ..exceptions import NonSerializableOutputError
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
 
 
 @runtime_checkable
 class OpenAIFunction(Protocol):
     """A protocol for OpenAI functions.
 
     Requires a __call__ method, a schema property, and a name property,
     as well as those that define the treatment of the return value.
     """
 
-    def __call__(self, arguments: dict[str, JsonType]) -> JsonType:
+    def __call__(self, arguments: dict[str, JsonType]) -> Any:
         ...
 
     @property
     def schema(self) -> JsonType:
         """Get the schema for this function"""
 
     @property
@@ -60,24 +60,25 @@
     serialize: bool = True
 
     @property
     def serialized(self) -> str:
         """Get the serialized result
 
         Raises:
-            NonSerializableOutputError: If the result is not a string
+            NonSerializableOutputError: If the result cannot be serialized
 
         Returns:
             str: The serialized result
         """
         if self.serialize:
-            return json.dumps(self.result)
-        if isinstance(self.result, str):
-            return self.result
-        raise NonSerializableOutputError()
+            try:
+                return json.dumps(self.result)
+            except TypeError as error:
+                raise NonSerializableOutputError(self.result) from error
+        return str(self.result)
 
 
 @dataclass
 class FunctionResult:
     """A result of a function's execution"""
 
     name: str
@@ -95,12 +96,12 @@
         return self.raw_result.serialized if self.raw_result else None
 
     @property
     def result(self) -> Any | None:
         """Get the result of this function call
 
         Returns:
-            JsonType: The result
+            The raw result of the function call
         """
         if self.raw_result:
             return self.raw_result.result
         return None
```

### Comparing `openai_functions-0.6.9/openai_functions/functions/sets.py` & `openai_functions-1.0.0/openai_functions/functions/sets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A module for running OpenAI functions"""
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from functools import partial
-from typing import Callable, TYPE_CHECKING, overload
+from typing import Any, Callable, TYPE_CHECKING, overload
 
 from .functions import FunctionResult, OpenAIFunction
 from .wrapper import FunctionWrapper, WrapperConfig
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
     from ..openai_types import FunctionCall
@@ -53,72 +53,69 @@
     @overload
     def add_function(self, function: OpenAIFunction) -> OpenAIFunction:
         ...
 
     @overload
     def add_function(
         self,
-        function: Callable[..., JsonType],
+        function: Callable[..., Any],
         *,
         name: str | None = None,
         description: str | None = None,
         save_return: bool = True,
         serialize: bool = True,
         remove_call: bool = False,
         interpret_as_response: bool = False,
-    ) -> Callable[..., JsonType]:
+    ) -> Callable[..., Any]:
         ...
 
     @overload
     def add_function(
         self,
         *,
         name: str | None = None,
         description: str | None = None,
         save_return: bool = True,
         serialize: bool = True,
         remove_call: bool = False,
         interpret_as_response: bool = False,
-    ) -> Callable[[Callable[..., JsonType]], Callable[..., JsonType]]:
+    ) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
         ...
 
     def add_function(
         self,
-        function: OpenAIFunction | Callable[..., JsonType] | None = None,
+        function: OpenAIFunction | Callable[..., Any] | None = None,
         *,
         name: str | None = None,
         description: str | None = None,
         save_return: bool = True,
         serialize: bool = True,
         remove_call: bool = False,
         interpret_as_response: bool = False,
-    ) -> (
-        Callable[[Callable[..., JsonType]], Callable[..., JsonType]]
-        | Callable[..., JsonType]
-    ):
+    ) -> Callable[[Callable[..., Any]], Callable[..., Any]] | Callable[..., Any]:
         """Add a function
 
         Args:
-            function (OpenAIFunction | Callable[..., JsonType]): The function
+            function (OpenAIFunction | Callable[..., Any]): The function
             name (str): The name of the function. Defaults to the function's name.
             description (str): The description of the function. Defaults to getting
                 the short description from the function's docstring.
             save_return (bool): Whether to send the return value of this
                 function to the AI. Defaults to True.
             serialize (bool): Whether to serialize the return value of this
                 function. Defaults to True. Otherwise, the return value must be a
                 string.
             remove_call (bool): Whether to remove the function call from the AI's
                 chat history. Defaults to False.
             interpret_as_response (bool): Whether to interpret the return
                 value of this function as a response of the agent. Defaults to False.
 
         Returns:
-            Callable[[Callable[..., JsonType]], Callable[..., JsonType]]: A decorator
-            Callable[..., JsonType]: The original function
+            Callable[[Callable[..., Any]], Callable[..., Any]]: A decorator
+            Callable[..., Any]: The original function
         """
         if isinstance(function, OpenAIFunction):
             self._add_function(function)
             return function
         if callable(function):
             self._add_function(
                 FunctionWrapper(
@@ -143,20 +140,20 @@
         )
 
     @abstractmethod
     def _remove_function(self, name: str) -> None:
         ...
 
     def remove_function(
-        self, function: str | OpenAIFunction | Callable[..., JsonType]
+        self, function: str | OpenAIFunction | Callable[..., Any]
     ) -> None:
         """Remove a function
 
         Args:
-            function (str | OpenAIFunction | Callable[..., JsonType]): The function
+            function (str | OpenAIFunction | Callable[..., Any]): The function
         """
         if isinstance(function, str):
             self._remove_function(function)
             return
         if isinstance(function, OpenAIFunction):
             self._remove_function(function.name)
             return
```

### Comparing `openai_functions-0.6.9/openai_functions/functions/togglable_set.py` & `openai_functions-1.0.0/openai_functions/functions/togglable_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """A function set disabled by default that exposes a function to enable it."""
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
+from ..exceptions import FunctionNotFoundError
 from .basic_set import BasicFunctionSet
-from .exceptions import FunctionNotFoundError
 from .functions import FunctionResult
 from .functions import OpenAIFunction
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
     from ..openai_types import FunctionCall
 
@@ -35,15 +35,19 @@
 
     def enable(self) -> None:
         """Enable the function set."""
         self.enabled = True
 
     @property
     def _enable_function_schema(self) -> dict[str, JsonType]:
-        """Get the schema for the enable function."""
+        """Get the schema for the enable function.
+
+        Returns:
+            dict[str, JsonType]: The schema for the enable function
+        """
         schema: dict[str, JsonType] = {
             "name": self.enable_function_name,
             "parameters": {
                 "type": "object",
                 "properties": {},
             },
         }
@@ -74,9 +78,9 @@
         Raises:
             FunctionNotFoundError: If the function is not found
         """
         if not self.enabled:
             if input_data["name"] == self.enable_function_name:
                 self.enable()
                 return FunctionResult(self.enable_function_name, None, True)
-            raise FunctionNotFoundError(f"Function {input_data['name']} not found")
+            raise FunctionNotFoundError(input_data["name"])
         return super().run_function(input_data)
```

### Comparing `openai_functions-0.6.9/openai_functions/functions/union.py` & `openai_functions-1.0.0/openai_functions/functions/union.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """A function set that's a union of other function sets."""
 from __future__ import annotations
 import contextlib
 from typing import TYPE_CHECKING
 
+from ..exceptions import FunctionNotFoundError
 from .basic_set import BasicFunctionSet
-from .exceptions import FunctionNotFoundError
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
     from ..openai_types import FunctionCall
     from .functions import FunctionResult
     from .sets import FunctionSet
```

### Comparing `openai_functions-0.6.9/openai_functions/functions/wrapper.py` & `openai_functions-1.0.0/openai_functions/functions/wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 from dataclasses import dataclass
 import inspect
 from typing import Any, Callable, OrderedDict, TYPE_CHECKING, Type
 
 from docstring_parser import Docstring, parse
 
+from ..exceptions import BrokenSchemaError, CannotParseTypeError
 from ..parsers import ArgSchemaParser, defargparsers
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
 
 
 @dataclass
@@ -43,29 +44,29 @@
 
     Provides a function schema and a function runner - the function schema is
     generated from the function's docstring and argument type annotations, and
     the function runner parses the arguments from JSON and runs the function.
     They are accessed via the `schema` property and a `__call__` method respectively.
 
     Args:
-        func (Callable[..., JsonType]): The function to wrap
+        func (Callable[..., Any]): The function to wrap
         config (WrapperConfig | None, optional): The configuration for the wrapper.
     """
 
     def __init__(
         self,
         func: Callable[..., Any],
         config: WrapperConfig | None = None,
         name: str | None = None,
         description: str | None = None,
     ) -> None:
         """Initialize a FunctionWrapper
 
         Args:
-            func (Callable[..., JsonType]): The function to wrap
+            func (Callable[..., Any]): The function to wrap
             config (WrapperConfig | None, optional): The configuration for the wrapper.
             name (str | None): The name override for the function.
             description (str | None): The description override for the function.
         """
         self.func = func
         self.config = config or WrapperConfig()
         self._name = name
@@ -217,40 +218,49 @@
     def parse_argument(self, argument: inspect.Parameter) -> ArgSchemaParser:
         """Parse an argument
 
         Args:
             argument (inspect.Parameter): The argument to parse
 
         Raises:
-            TypeError: If the argument cannot be parsed
+            CannotParseTypeError: If the argument cannot be parsed
 
         Returns:
             ArgSchemaParser: The parser for the argument
         """
         # The reasoning behind not using pydantic is OpenAI's apparent inability to
         # parse JSON Schemas with $ref's in them - or at least, that's what I've
         # gathered from the error messages.
         for parser in self.parsers:
             if parser.can_parse(argument.annotation):
                 return parser(argument.annotation, self.parsers)
-        raise TypeError(f"Cannot parse argument {argument}")
+        raise CannotParseTypeError(argument.annotation)
 
     def parse_arguments(self, arguments: dict[str, JsonType]) -> OrderedDict[str, Any]:
         """Parse arguments
 
         Args:
             arguments (dict[str, JsonType]): The arguments to parse
 
+        Raises:
+            BrokenSchemaError: If the arguments do not match the schema
+
         Returns:
             OrderedDict[str, Any]: The parsed arguments
         """
-        return OrderedDict(
-            (name, self.argument_parsers[name].parse_value(value))
-            for name, value in arguments.items()
-        )
+        argument_parsers = self.argument_parsers
+        if not all(name in arguments for name in argument_parsers):
+            raise BrokenSchemaError(arguments, self.arguments_schema)
+        try:
+            return OrderedDict(
+                (name, argument_parsers[name].parse_value(value))
+                for name, value in arguments.items()
+            )
+        except KeyError as err:
+            raise BrokenSchemaError(arguments, self.arguments_schema) from err
 
     def __call__(self, arguments: dict[str, JsonType]) -> Any:
         """Call the wrapped function
 
         Args:
             arguments (dict[str, JsonType]): The arguments to call the function with
```

### Comparing `openai_functions-0.6.9/openai_functions/openai_types.py` & `openai_functions-1.0.0/openai_functions/openai_types.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.9/openai_functions/parsers/abc.py` & `openai_functions-1.0.0/openai_functions/parsers/abc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Abstract base class for argument schema parsers"""
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from typing import Any, Generic, TYPE_CHECKING, Type, TypeVar
 
+from ..exceptions import CannotParseTypeError
+
 if TYPE_CHECKING:
     from ..json_type import JsonType
     from typing_extensions import TypeGuard
 
 T = TypeVar("T")
 S = TypeVar("S")
 
@@ -30,20 +32,20 @@
         Args:
             argtype (Type[S]): The type to parse
 
         Returns:
             ArgSchemaParser[S]: The parser for the type
 
         Raises:
-            ValueError: If the type cannot be parsed
+            CannotParseTypeError: If the type cannot be parsed
         """
         for parser in self.rec_parsers:
             if parser.can_parse(argtype):
                 return parser(argtype, self.rec_parsers)
-        raise ValueError(f"Cannot parse type {argtype}")
+        raise CannotParseTypeError(argtype)
 
     @classmethod
     @abstractmethod
     def can_parse(cls, argtype: Any) -> TypeGuard[Type[T]]:
         """Whether this parser can parse a specific arg type
 
         Args:
@@ -57,8 +59,11 @@
 
     @abstractmethod
     def parse_value(self, value: JsonType) -> T:
         """Parse a value of a specific type
 
         Args:
             value (JsonType): The value to parse
+
+        Raises:
+            BrokenSchemaError: If the value does not match the schema
         """
```

### Comparing `openai_functions-0.6.9/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-1.0.0/openai_functions/parsers/dict_parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,44 @@
-"""Parser for atomic json types"""
+"""Parser for dict types"""
 from __future__ import annotations
-from abc import abstractmethod
-from typing import Any, TYPE_CHECKING, Type, TypeVar
+from typing import Any, Dict, TYPE_CHECKING, Type, TypeVar, get_args, get_origin
 
+from ..exceptions import BrokenSchemaError
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
     from typing_extensions import TypeGuard
 
 T = TypeVar("T")
 
 
-class AtomicParser(ArgSchemaParser[T]):
-    """Parser for atomic json values"""
-
-    _type: Type[T]
-
-    @property
-    @abstractmethod
-    def schema_type_name(self) -> str:
-        """Name of the type in the json schema"""
+class DictParser(ArgSchemaParser[Dict[str, T]]):
+    """Parser for dict types"""
 
     @classmethod
-    def can_parse(cls, argtype: Any) -> TypeGuard[Type[T]]:
-        return argtype is cls._type
+    def can_parse(cls, argtype: Any) -> TypeGuard[Type[Dict[str, T]]]:
+        return (
+            get_origin(argtype)
+            in [
+                dict,
+                Dict,
+            ]
+            and get_args(argtype)[0] is str
+        )
 
     @property
-    def argument_schema(self) -> dict[str, JsonType]:
+    def argument_schema(self) -> Dict[str, JsonType]:
         return {
-            "type": self.schema_type_name,
+            "type": "object",
+            "additionalProperties": self.parse_rec(
+                get_args(self.argtype)[1]
+            ).argument_schema,
         }
 
-    def parse_value(self, value: JsonType) -> T:
-        if not isinstance(value, self._type):
-            raise TypeError(f"Expected {self._type}, got {type(value)}")
-        return value
+    def parse_value(self, value: JsonType) -> Dict[str, T]:
+        if not isinstance(value, dict):
+            raise BrokenSchemaError(value, self.argument_schema)
+        return {
+            k: self.parse_rec(get_args(self.argtype)[1]).parse_value(v)
+            for k, v in value.items()
+        }
```

### Comparing `openai_functions-0.6.9/openai_functions/parsers/dataclass_parser.py` & `openai_functions-1.0.0/openai_functions/parsers/union_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,45 @@
-"""Parser for dataclass types"""
+"""Parser for union types"""
 from __future__ import annotations
-import dataclasses
-from typing import Any, ClassVar, Protocol, TYPE_CHECKING, Type
+import contextlib
 
+from ..exceptions import BrokenSchemaError
 from .abc import ArgSchemaParser
 
+try:
+    from types import UnionType
+    from typing import Any, TYPE_CHECKING, Type, Union, get_args, get_origin
+except ImportError:
+    # This is for Python 3.8
+    from typing import (  # type: ignore
+        Any,
+        TYPE_CHECKING,
+        Type,
+        Union,
+        get_args,
+        get_origin,
+        _GenericAlias as UnionType,
+    )
+
 if TYPE_CHECKING:
     from ..json_type import JsonType
     from typing_extensions import TypeGuard
 
 
-class IsDataclass(Protocol):  # pylint: disable=too-few-public-methods
-    """A protocol for checking if a class is a dataclass"""
-
-    __dataclass_fields__: ClassVar[dict]
-
-
-class DataclassParser(ArgSchemaParser[IsDataclass]):
-    """Parser for dataclass types"""
+class UnionParser(ArgSchemaParser[UnionType]):
+    """Parser for union types"""
 
     @classmethod
-    def can_parse(cls, argtype: Any) -> TypeGuard[Type[IsDataclass]]:
-        return dataclasses.is_dataclass(argtype)
+    def can_parse(cls, argtype: Any) -> TypeGuard[Type[UnionType]]:
+        return get_origin(argtype) is Union
 
     @property
     def argument_schema(self) -> dict[str, JsonType]:
         return {
-            "type": "object",
-            "description": self.argtype.__doc__,
-            "properties": {
-                field.name: self.parse_rec(field.type).argument_schema
-                for field in dataclasses.fields(self.argtype)
-            },
-            "required": [
-                field.name
-                for field in dataclasses.fields(self.argtype)
-                if field.default is dataclasses.MISSING
-            ],
+            "anyOf": [self.parse_rec(t).argument_schema for t in get_args(self.argtype)]
         }
 
-    def parse_value(self, value: JsonType) -> IsDataclass:
-        if not isinstance(value, dict):
-            raise TypeError(f"Expected dict, got {value}")
-        return self.argtype(
-            **{
-                field.name: self.parse_rec(field.type).parse_value(value[field.name])
-                for field in dataclasses.fields(self.argtype)
-                if field.name in value
-            }
-        )
+    def parse_value(self, value: JsonType) -> UnionType:
+        for single_type in get_args(self.argtype):
+            with contextlib.suppress(BrokenSchemaError):
+                return self.parse_rec(single_type).parse_value(value)
+        raise BrokenSchemaError(value, self.argument_schema)
```

### Comparing `openai_functions-0.6.9/openai_functions/parsers/default.py` & `openai_functions-1.0.0/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.6.9/openai_functions/parsers/dict_parser.py` & `openai_functions-1.0.0/openai_functions/parsers/enum_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""Parser for dict types"""
+"""Parser for enum types"""
 from __future__ import annotations
-from typing import Any, Dict, TYPE_CHECKING, Type, TypeVar, get_args, get_origin
+import enum
+from typing import Any, TYPE_CHECKING, Type, TypeVar
 
+from ..exceptions import BrokenSchemaError
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
     from typing_extensions import TypeGuard
 
-T = TypeVar("T")
+T = TypeVar("T", bound=enum.Enum)
 
 
-class DictParser(ArgSchemaParser[Dict[str, T]]):
-    """Parser for dict types"""
+class EnumParser(ArgSchemaParser[T]):
+    """Parser for enum types"""
 
     @classmethod
-    def can_parse(cls, argtype: Any) -> TypeGuard[Type[Dict[str, T]]]:
-        return (
-            get_origin(argtype)
-            in [
-                dict,
-                Dict,
-            ]
-            and get_args(argtype)[0] is str
-        )
+    def can_parse(cls, argtype: Any) -> TypeGuard[Type[T]]:
+        if not isinstance(argtype, type):
+            return False
+        return issubclass(argtype, enum.Enum)
 
     @property
-    def argument_schema(self) -> Dict[str, JsonType]:
-        return {
-            "type": "object",
-            "additionalProperties": self.parse_rec(
-                get_args(self.argtype)[1]
-            ).argument_schema,
-        }
-
-    def parse_value(self, value: JsonType) -> Dict[str, T]:
-        if not isinstance(value, dict):
-            raise TypeError(f"Expected dict, got {value}")
-        return {
-            k: self.parse_rec(get_args(self.argtype)[1]).parse_value(v)
-            for k, v in value.items()
+    def argument_schema(self) -> dict[str, JsonType]:
+        schema: dict[str, JsonType] = {
+            "type": "string",
+            "enum": [e.name for e in self.argtype],
         }
+        if self.argtype.__doc__ is not None:
+            schema["description"] = self.argtype.__doc__
+        return schema
+
+    def parse_value(self, value: JsonType) -> T:
+        if not isinstance(value, str):
+            raise BrokenSchemaError(value, self.argument_schema)
+        if value not in self.argument_schema["enum"]:  # type: ignore
+            # TODO: consider using something other than JsonType for
+            #       all of these, because disabling mypy is definitely
+            #       not the right way to do this
+            raise BrokenSchemaError(value, self.argument_schema)
+        return self.argtype[value]
```

### Comparing `openai_functions-0.6.9/openai_functions/parsers/enum_parser.py` & `openai_functions-1.0.0/openai_functions/parsers/none_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,26 @@
-"""Parser for enum types"""
+"""Parser for null types"""
 from __future__ import annotations
-import enum
-from typing import Any, TYPE_CHECKING, Type, TypeVar
+from typing import Any, TYPE_CHECKING, Type
 
+from ..exceptions import BrokenSchemaError
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
     from typing_extensions import TypeGuard
 
-T = TypeVar("T", bound=enum.Enum)
 
-
-class EnumParser(ArgSchemaParser[T]):
-    """Parser for enum types"""
+class NoneParser(ArgSchemaParser[None]):
+    """Parser for null types"""
 
     @classmethod
-    def can_parse(cls, argtype: Any) -> TypeGuard[Type[T]]:
-        if not isinstance(argtype, type):
-            return False
-        return issubclass(argtype, enum.Enum)
+    def can_parse(cls, argtype: Any) -> TypeGuard[Type[None]]:
+        return argtype in [None, type(None)]
 
     @property
     def argument_schema(self) -> dict[str, JsonType]:
-        schema: dict[str, JsonType] = {
-            "type": "string",
-            "enum": [e.name for e in self.argtype],
-        }
-        if self.argtype.__doc__ is not None:
-            schema["description"] = self.argtype.__doc__
-        return schema
-
-    def parse_value(self, value: JsonType) -> T:
-        if not isinstance(value, str):
-            raise TypeError(f"Expected str, got {value}")
-        return self.argtype[value]
+        return {"type": "null"}
+
+    def parse_value(self, value: JsonType) -> None:
+        if value is not None:
+            raise BrokenSchemaError(value, self.argument_schema)
```

### Comparing `openai_functions-0.6.9/openai_functions/parsers/float_parser.py` & `openai_functions-1.0.0/openai_functions/parsers/float_parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Parser for float types"""
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
+from ..exceptions import BrokenSchemaError
 from .atomic_type_parser import AtomicParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
 
 
 class FloatParser(AtomicParser[float]):
     """Parser for float types"""
 
     _type = float
     schema_type_name: str = "number"
 
     def parse_value(self, value: JsonType) -> float:
         if not isinstance(value, (float, int)):
-            raise TypeError(f"Expected float, got {value}")
+            raise BrokenSchemaError(value, self.argument_schema)
         return float(value)
```

### Comparing `openai_functions-0.6.9/openai_functions/parsers/list_parser.py` & `openai_functions-1.0.0/openai_functions/parsers/list_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Parser for list types"""
 from __future__ import annotations
 from typing import Any, List, TYPE_CHECKING, Type, TypeVar, get_args, get_origin
 
+from ..exceptions import BrokenSchemaError
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
     from typing_extensions import TypeGuard
 
 T = TypeVar("T")
@@ -26,9 +27,9 @@
         return {
             "type": "array",
             "items": self.parse_rec(get_args(self.argtype)[0]).argument_schema,
         }
 
     def parse_value(self, value: JsonType) -> List[T]:
         if not isinstance(value, list):
-            raise TypeError(f"Expected list, got {value}")
+            raise BrokenSchemaError(value, self.argument_schema)
         return [self.parse_rec(get_args(self.argtype)[0]).parse_value(v) for v in value]
```

### Comparing `openai_functions-0.6.9/openai_functions/parsers/none_parser.py` & `openai_functions-1.0.0/openai_functions/parsers/atomic_type_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,39 @@
-"""Parser for null types"""
+"""Parser for atomic json types"""
 from __future__ import annotations
-from typing import Any, TYPE_CHECKING, Type
+from abc import abstractmethod
+from typing import Any, TYPE_CHECKING, Type, TypeVar
 
+from ..exceptions import BrokenSchemaError
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
     from typing_extensions import TypeGuard
 
+T = TypeVar("T")
 
-class NoneParser(ArgSchemaParser[None]):
-    """Parser for null types"""
+
+class AtomicParser(ArgSchemaParser[T]):
+    """Parser for atomic json values"""
+
+    _type: Type[T]
+
+    @property
+    @abstractmethod
+    def schema_type_name(self) -> str:
+        """Name of the type in the json schema"""
 
     @classmethod
-    def can_parse(cls, argtype: Any) -> TypeGuard[Type[None]]:
-        return argtype in [None, type(None)]
+    def can_parse(cls, argtype: Any) -> TypeGuard[Type[T]]:
+        return argtype is cls._type
 
     @property
     def argument_schema(self) -> dict[str, JsonType]:
-        return {"type": "null"}
-
-    def parse_value(self, value: JsonType) -> None:
-        if value is not None:
-            raise TypeError(f"Expected None, got {type(value)}")
+        return {
+            "type": self.schema_type_name,
+        }
+
+    def parse_value(self, value: JsonType) -> T:
+        if not isinstance(value, self._type):
+            raise BrokenSchemaError(value, self.argument_schema)
+        return value
```

### Comparing `openai_functions-0.6.9/pyproject.toml` & `openai_functions-1.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.6.9"
+version = "1.0.0"
 description = "Simplifies the usage of OpenAI ChatGPT's function calling by generating the schemas and parsing OpenAI's responses for you."
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/rizerphe/openai-functions"
 documentation = "https://openai-functions.readthedocs.io/"
 keywords = ["nlp", "openai", "openai-api", "chatgpt", "chatgpt-api", "wrapper", "functions", "chatgpt-api", "openai-functions", "chatgpt-functions", "typing", "docstring", "docstrings", "decorators", "signatures", "parsing"]
 license = "MIT"
```

### Comparing `openai_functions-0.6.9/PKG-INFO` & `openai_functions-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.6.9
+Version: 1.0.0
 Summary: Simplifies the usage of OpenAI ChatGPT's function calling by generating the schemas and parsing OpenAI's responses for you.
 Home-page: https://github.com/rizerphe/openai-functions
 License: MIT
 Keywords: nlp,openai,openai-api,chatgpt,chatgpt-api,wrapper,functions,chatgpt-api,openai-functions,chatgpt-functions,typing,docstring,docstrings,decorators,signatures,parsing
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

