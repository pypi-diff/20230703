# Comparing `tmp/func_ai-0.0.6.tar.gz` & `tmp/func_ai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_ai-0.0.6.tar", max compression
+gzip compressed data, was "func_ai-0.0.7.tar", max compression
```

## Comparing `func_ai-0.0.6.tar` & `func_ai-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1076 2023-06-28 17:45:39.671843 func_ai-0.0.6/LICENSE
--rw-r--r--   0        0        0     3375 2023-06-30 11:34:34.818711 func_ai-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-06-28 16:40:13.608045 func_ai-0.0.6/func_ai/__init__.py
--rw-r--r--   0        0        0     4082 2023-06-28 17:47:54.691621 func_ai-0.0.6/func_ai/function_indexer.py
--rw-r--r--   0        0        0        0 2023-06-28 17:11:55.264886 func_ai-0.0.6/func_ai/utils/__init__.py
--rw-r--r--   0        0        0     4645 2023-06-30 11:52:33.930306 func_ai-0.0.6/func_ai/utils/jinja_template_functions.py
--rw-r--r--   0        0        0    10241 2023-06-30 09:42:46.148402 func_ai-0.0.6/func_ai/utils/llm_tools.py
--rw-r--r--   0        0        0     5701 2023-06-30 06:36:30.640188 func_ai-0.0.6/func_ai/utils/openapi_function_parser.py
--rw-r--r--   0        0        0     3392 2023-06-30 06:36:30.641465 func_ai-0.0.6/func_ai/utils/py_function_parser.py
--rw-r--r--   0        0        0     5337 2023-06-30 06:36:30.641834 func_ai-0.0.6/func_ai/workflow_creator.py
--rw-r--r--   0        0        0      907 2023-06-30 12:10:48.672915 func_ai-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 func_ai-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-28 17:45:39.671843 func_ai-0.0.7/LICENSE
+-rw-r--r--   0        0        0     4323 2023-07-03 07:47:52.395570 func_ai-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-28 16:40:13.608045 func_ai-0.0.7/func_ai/__init__.py
+-rw-r--r--   0        0        0     4082 2023-06-28 17:47:54.691621 func_ai-0.0.7/func_ai/function_indexer.py
+-rw-r--r--   0        0        0        0 2023-06-28 17:11:55.264886 func_ai-0.0.7/func_ai/utils/__init__.py
+-rw-r--r--   0        0        0     4852 2023-07-03 07:47:52.396052 func_ai-0.0.7/func_ai/utils/jinja_template_functions.py
+-rw-r--r--   0        0        0    15155 2023-07-03 07:47:52.396377 func_ai-0.0.7/func_ai/utils/llm_tools.py
+-rw-r--r--   0        0        0    11068 2023-07-03 07:47:52.396708 func_ai-0.0.7/func_ai/utils/openapi_function_parser.py
+-rw-r--r--   0        0        0     3444 2023-07-03 07:47:52.397246 func_ai-0.0.7/func_ai/utils/py_function_parser.py
+-rw-r--r--   0        0        0     5337 2023-06-30 06:36:30.641834 func_ai-0.0.7/func_ai/workflow_creator.py
+-rw-r--r--   0        0        0      907 2023-07-03 07:47:52.399129 func_ai-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 func_ai-0.0.7/PKG-INFO
```

### Comparing `func_ai-0.0.6/LICENSE` & `func_ai-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.6/func_ai/function_indexer.py` & `func_ai-0.0.7/func_ai/function_indexer.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.6/func_ai/utils/jinja_template_functions.py` & `func_ai-0.0.7/func_ai/utils/jinja_template_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,23 +35,25 @@
         self._environment.get_template(template_name)
         source = self._environment.loader.get_source(self._environment, template_name)[0]
         ast = self._environment.parse(source)
 
         # Get the undeclared variables
         _template_vars = meta.find_undeclared_variables(ast)
         _response = self._lm_interface.send(prompt=prompt,
+                                            #TODO: Move this to OpenAIFunctionWrapper
                                             functions=[{"name": "render_template",
                                                         "description": "Render a template with given parameters",
                                                         "parameters": {
                                                             "type": "object",
                                                             "properties": {k: {"type": "string",
                                                                                "description": f"{k}"} for
                                                                            k
                                                                            in _template_vars},
-                                                            "required": list(_template_vars)}}])
+                                                            "required": list(
+                                                                _template_vars)}}])  # TODO this is a bug should be moved inside parameters
         if "function_call" in _response:
             args = json.loads(_response["function_call"]["arguments"])
             return self._environment.get_template(template_name).render(**args)
 
     @classmethod
     def from_string_template(cls, template_string: str, llm_interface: LLMInterface,
                              **kwargs) -> "JinjaOpenAITemplateFunction":
```

### Comparing `func_ai-0.0.6/func_ai/utils/llm_tools.py` & `func_ai-0.0.7/func_ai/utils/llm_tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+A module for interacting with the Language Learning Model
+"""
+import functools
 import json
 import logging
 import os
 import traceback
 from abc import abstractmethod
 from enum import Enum
 from typing import Any
@@ -121,14 +125,23 @@
     def get_conversation(self) -> list[any]:
         """
         Returns the conversation
         :return:
         """
         return self.conversation_store.get_conversation()
 
+    def add_conversation_message(self, message: any) -> "LLMInterface":
+        """
+        Adds a message to the conversation
+        :param message:
+        :return:
+        """
+        self.conversation_store.add_message(message)
+        return self
+
 
 class OpenAIInterface(LLMInterface):
     """
     Interface for interacting with the OpenAI API
     """
     max_tokens: int = Field(default=256, description="The maximum number of tokens to return")
     model: str = Field(default="gpt-3.5-turbo-0613", description="The model to use")
@@ -204,15 +217,14 @@
                 "total_tokens": 0
             }
         self.usage[model]["prompt_tokens"] += api_response['usage']['prompt_tokens']
         self.usage[model]["completion_tokens"] += api_response['usage']['completion_tokens']
         self.usage[model]["total_tokens"] += api_response['usage']['total_tokens']
 
 
-
 class OpenAISchema(BaseModel):
     @classmethod
     @property
     def openai_schema(cls):
         schema = cls.schema()
 
         return {
@@ -279,7 +291,155 @@
         :param throw_error: whether to throw error if function call is not present
         :return:
         """
         completion = llm_interface.send(prompt, functions=[cls.openai_schema])
         # print(llm_interface.get_conversation())
         # TODO add crud interface functions here
         return cls.from_response(completion, throw_error)
+
+
+class OpenAIFunctionWrapper(object):
+    """
+    A wrapper class for OpenAI functions.
+    """
+
+    def __init__(self, llm_interface: LLMInterface, name: str, description: str, parameters: dict[str, any],
+                 func: callable, **kwargs) -> None:
+        """
+        Initializes the OpenAI function wrapper
+        :param llm_interface:
+        :param name:
+        :param description:
+        :param parameters:
+        :param func:
+        :param kwargs: All these are treated as metadata that can be used by other tooling to augment the function
+        """
+        self.llm_interface = llm_interface
+        self._name = name
+        self._description = description
+        assert "required" in parameters, "Required field not present in parameters"
+        self._parameters = parameters
+        assert callable(func) or isinstance(func, functools.partial), "Function must be callable"
+        self.func = functools.partial(func, action=self)
+        self._metadata = kwargs
+        self._llm_calls = []
+
+    @property
+    def name(self) -> str:
+        """
+        Returns the name of the function
+
+        :return: name of the function
+        """
+        return self._name
+
+    @property
+    def description(self) -> str:
+        """
+        Returns the description of the function
+
+        :return: description of the function
+        """
+        return self._description
+
+    @property
+    def parameters(self) -> dict[str, any]:
+        """
+        Returns the parameters of the function
+
+        :return: parameters of the function
+        """
+        return self._parameters
+
+    def call(self, **kwargs) -> dict[str, any]:
+        """
+        Calls the function with the given arguments
+
+        :param kwargs: arguments to be passed to the function
+        :return:
+        """
+        return self.func(**kwargs)
+
+    @property
+    def metadata(self) -> dict[str, any]:
+        """
+        Returns the metadata of the function
+
+        :return: dict containing the metadata
+        """
+        return self._metadata
+
+    @property
+    def schema(self) -> dict[str, any]:
+        """
+        Returns the schema of the function that can be passed to OpenAI API
+
+        :return: dict containing the schema
+        """
+        return {
+            "name": self.name,
+            "description": self.description,
+            "parameters": self.parameters,
+        }
+
+    def __str__(self) -> str:
+        return f"{self.schema}"
+
+    def __repr__(self):
+        return f"{self.schema}"
+
+    @property
+    def last_call(self) -> dict[str, any]:
+        """
+        Returns the last response from the function call
+
+        :return: dict containing the last response
+        """
+        return self._llm_calls[-1]
+
+    @property
+    def calls(self) -> list[dict[str, any]]:
+        """
+        Returns the list of responses from the function call
+
+        :return: list containing the responses
+        """
+        return self._llm_calls
+
+    def from_response(self, llm_response: dict[str, any]) -> "OpenAIFunctionWrapper":
+        """
+        Returns an instance of the class from LLM completion response
+
+        :param llm_response: completion response from LLM
+        :return: The response from the function call
+        """
+        if "function_call" not in llm_response:
+            raise ValueError(f"No function call detected: {llm_response}")
+        if llm_response["function_call"]["name"] != self.name:
+            raise ValueError(f"Function name does not match: {llm_response}")
+        try:
+            _func_response = self.func(**json.loads(llm_response["function_call"]["arguments"]))
+        except Exception as e:
+            _func_response = f"Error: {repr(e)}"
+            traceback.print_exc()
+        _function_call_llm_response = {
+            "role": "function",
+            "name": self.name,
+            "content": f"{_func_response}",
+        }
+        self._llm_calls.append({
+            "function_call": llm_response["function_call"],
+            "function_response": _function_call_llm_response,
+        })
+        self.llm_interface.add_conversation_message(_function_call_llm_response)
+        return self
+
+    def from_prompt(self, prompt: str, **kwargs) -> "OpenAIFunctionWrapper":
+        """
+        Returns an instance of the class from LLM prompt
+
+        :param prompt: User prompt
+        :param kwargs: arguments to be passed to the function
+        :return: The response from the function call
+        """
+        self.from_response(self.llm_interface.send(prompt, functions=[self.schema]))
+        return self
```

### Comparing `func_ai-0.0.6/func_ai/utils/py_function_parser.py` & `func_ai-0.0.7/func_ai/utils/py_function_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,16 +83,18 @@
     # _required = [arg for arg in argspec.args if arg not in fixed_args]
     _required = [i for i in argspec.args if i not in fixed_args.keys()]
     if inspect.getfullargspec(_func).defaults:
         _required = [argspec.args[i] for i, a in enumerate(argspec.args) if
                      argspec.args[i] not in inspect.getfullargspec(_func).defaults and argspec.args[
                          i] not in fixed_args.keys()]
     # then return everything in dict
+    #TODO: Move this to OpenAIFunctionWrapper
     return {
         "name": func_name,
         "description": func_description,
         "parameters": {
             "type": "object",
-            "properties": params
+            "properties": params,
+            "required": _required
         },
-        "required": _required
+
     }
```

### Comparing `func_ai-0.0.6/func_ai/workflow_creator.py` & `func_ai-0.0.7/func_ai/workflow_creator.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.6/pyproject.toml` & `func_ai-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "func-ai"
-version = "0.0.6"
+version = "0.0.7"
 description = "AI Functional Catalog - OpenAI functions on steriods"
 authors = ["Trayan Azarov <trayan.azarov@amikos.tech>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "func_ai" }]
 
 [tool.poetry.urls]
```

### Comparing `func_ai-0.0.6/PKG-INFO` & `func_ai-0.0.7/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: func-ai
-Version: 0.0.6
-Summary: AI Functional Catalog - OpenAI functions on steriods
-License: MIT
-Author: Trayan Azarov
-Author-email: trayan.azarov@amikos.tech
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: chromadb (>=0.3.26,<0.4.0)
-Requires-Dist: fastapi (>=0.98.0,<0.99.0)
-Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
-Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: python-ulid (>=1.1.0,<2.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: tenacity (>=8.2.2,<9.0.0)
-Project-URL: Bug Tracker, https://github.com/amikos-tech/func-ai/issues
-Project-URL: Homepage, https://github.com/amikos-tech/func-ai/
-Project-URL: Source, https://github.com/amikos-tech/func-ai/
-Description-Content-Type: text/markdown
-
 # AI Functional Catalog
 
 Your OpenAI function calling on steroids
 
 Features:
 
 - Index any python function and use it in your AI workflows
@@ -74,51 +47,46 @@
     """
 
 ```
 
 ### OpenAPI Mapping
 
 ```python
-import json
-
 from dotenv import load_dotenv
 
 from func_ai.utils.llm_tools import OpenAIInterface
-from func_ai.utils.openapi_function_parser import get_spec_from_url, parse_spec, call_api
+from func_ai.utils.openapi_function_parser import OpenAPISpecOpenAIWrapper
 
 load_dotenv()
-spec = get_spec_from_url('http://petstore.swagger.io/v2/swagger.json')
-_funcs = parse_spec(spec)
-print(f"Function to all {_funcs['getPetById']}")
-inf = OpenAIInterface()
-resp = inf.send(
-    # prompt="Add new pet named Rocky with following photoUrl: http://rocky.me/pic.png. Tag the Rocky with 'dog' and 'pet'",
-    prompt="Get pet with id 10",
-    functions=[_funcs['getPetById']['func']])
-print(f"LLM Response: {resp}")
-if "function_call" in resp:
-    fc = resp["function_call"]
-    call_api(fc, spec, _funcs)
+_spec = OpenAPISpecOpenAIWrapper.from_url('http://petstore.swagger.io/v2/swagger.json',
+                                          llm_interface=OpenAIInterface())
+print(_spec.from_prompt("Get pet with id 10", "getPetById").last_call)
 """
-Function to all {'details': {'name': 'getPetById', 'description': 'Returns a single pet', 'parameters': [{'name': 'petId', 'in': 'path', 'description': 'ID of pet to return', 'required': True, 'type': 'integer', 'format': 'int64'}], 'summary': 'Find pet by ID', 'method': 'get', 'path': '/pet/{petId}'}, 'func': {'name': 'getPetById', 'description': 'Find pet by IDReturns a single pet', 'parameters': {'type': 'object', 'properties': {'petId': {'description': 'ID of pet to return', 'type': 'string', 'in': 'path'}}, 'required': ['petId']}}}
-LLM Response: {
-"role": "assistant",
-"content": null,
-"function_call": {
- "name": "getPetById",
- "arguments": "{\n  \"petId\": \"10\"\n}"
-}
-}
-Calling getPetById - get https://petstore.swagger.io/v2/pet/{petId}
-2023-06-30 07:57:40,306 - urllib3.connectionpool - DEBUG - https://petstore.swagger.io:443 "GET /v2/pet/10 HTTP/1.1" 200 None
-{"id":10,"category":{"id":10,"name":"sample string"},"name":"doggie","photoUrls":[],"tags":[],"status":"pending"}
+2023-07-03 10:43:04 DEBUG Starting new HTTP connection (1): petstore.swagger.io:80
+2023-07-03 10:43:04 DEBUG http://petstore.swagger.io:80 "GET /v2/swagger.json HTTP/1.1" 301 134
+2023-07-03 10:43:04 DEBUG Starting new HTTPS connection (1): petstore.swagger.io:443
+2023-07-03 10:43:04 DEBUG https://petstore.swagger.io:443 "GET /v2/swagger.json HTTP/1.1" 200 None
+2023-07-03 10:43:04 DEBUG Prompt: Get pet with id 10
+2023-07-03 10:43:04 DEBUG message='Request to OpenAI API' method=post path=https://api.openai.com/v1/chat/completions
+2023-07-03 10:43:04 DEBUG api_version=None data='{"model": "gpt-3.5-turbo-0613", "messages": [{"role": "user", "content": "Get pet with id 10"}], "functions": [{"name": "getPetById", "description": "Find pet by IDReturns a single pet", "parameters": {"type": "object", "properties": {"petId": {"description": "ID of pet to return", "type": "string", "in": "path"}}, "required": ["petId"]}}], "function_call": "auto", "temperature": 0.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty": 0.0, "max_tokens": 256}' message='Post details'
+2023-07-03 10:43:04 DEBUG Converted retries value: 2 -> Retry(total=2, connect=None, read=None, redirect=None, status=None)
+2023-07-03 10:43:05 DEBUG Starting new HTTPS connection (1): api.openai.com:443
+2023-07-03 10:43:06 DEBUG https://api.openai.com:443 "POST /v1/chat/completions HTTP/1.1" 200 None
+2023-07-03 10:43:06 DEBUG message='OpenAI API response' path=https://api.openai.com/v1/chat/completions processing_ms=876 request_id=f38d1625ae785681b53686492fd1d7e3 response_code=200
+2023-07-03 10:43:06 DEBUG Starting new HTTPS connection (1): petstore.swagger.io:443
+2023-07-03 10:43:07 DEBUG https://petstore.swagger.io:443 "GET /v2/pet/10 HTTP/1.1" 200 None
+PASSED                                                                   [100%]{'function_call': <OpenAIObject at 0x10a5f2c30> JSON: {
+  "name": "getPetById",
+  "arguments": "{\n  \"petId\": \"10\"\n}"
+}, 'function_response': {'role': 'function', 'name': 'getPetById', 'content': '{\'status_code\': 200, \'response\': \'{"id":10,"category":{"id":10,"name":"sample string"},"name":"doggie","photoUrls":["sample 1","sample 2","sample 3"],"tags":[{"id":10,"name":"sample string"},{"id":10,"name":"sample string"}],"status":"available"}\'}'}}
+
 """
 ```
 
-> Note: the above is pretty naive implementation of OpenAPI parsing and calling. It is not production ready.
+> Note: The above example is still in beta and is not production ready.
 
 ### Jinja2 Templating
 
 ```python
 from dotenv import load_dotenv
 from func_ai.utils.jinja_template_functions import JinjaOpenAITemplateFunction
 from func_ai.utils.llm_tools import OpenAIInterface
@@ -134,8 +102,8 @@
 """
 ```
 
 ## Inspiration
 
 - https://github.com/jxnl/openai_function_call
 - https://github.com/rizerphe/openai-functions
-- https://github.com/aurelio-labs/funkagent
+- https://github.com/aurelio-labs/funkagent
```

