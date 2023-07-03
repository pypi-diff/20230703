# Comparing `tmp/one-api-tool-0.3.9.tar.gz` & `tmp/one-api-tool-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.3.9.tar", last modified: Mon Jul  3 07:21:13 2023, max compression
+gzip compressed data, was "one-api-tool-0.4.0.tar", last modified: Mon Jul  3 10:51:46 2023, max compression
```

## Comparing `one-api-tool-0.3.9.tar` & `one-api-tool-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 07:21:13.770939 one-api-tool-0.3.9/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.3.9/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-03 07:21:13.770717 one-api-tool-0.3.9/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     4172 2023-07-02 05:43:55.000000 one-api-tool-0.3.9/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 07:21:13.769925 one-api-tool-0.3.9/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-03 07:21:13.000000 one-api-tool-0.3.9/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-07-03 07:21:13.000000 one-api-tool-0.3.9/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-03 07:21:13.000000 one-api-tool-0.3.9/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-03 07:21:13.000000 one-api-tool-0.3.9/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-07-03 07:21:13.000000 one-api-tool-0.3.9/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-03 07:21:13.000000 one-api-tool-0.3.9/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 07:21:13.770201 one-api-tool-0.3.9/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.3.9/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 07:21:13.770502 one-api-tool-0.3.9/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.3.9/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.3.9/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    12685 2023-07-03 07:20:51.000000 one-api-tool-0.3.9/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-03 07:21:13.770987 one-api-tool-0.3.9/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-07-03 07:21:05.000000 one-api-tool-0.3.9/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 10:51:46.470474 one-api-tool-0.4.0/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.4.0/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-03 10:51:46.470238 one-api-tool-0.4.0/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4172 2023-07-02 05:43:55.000000 one-api-tool-0.4.0/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 10:51:46.469347 one-api-tool-0.4.0/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-03 10:51:46.000000 one-api-tool-0.4.0/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      359 2023-07-03 10:51:46.000000 one-api-tool-0.4.0/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-03 10:51:46.000000 one-api-tool-0.4.0/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-03 10:51:46.000000 one-api-tool-0.4.0/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-07-03 10:51:46.000000 one-api-tool-0.4.0/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-03 10:51:46.000000 one-api-tool-0.4.0/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 10:51:46.469753 one-api-tool-0.4.0/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.4.0/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-03 10:51:46.470038 one-api-tool-0.4.0/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.4.0/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.4.0/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    13358 2023-07-03 10:50:07.000000 one-api-tool-0.4.0/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3696 2023-07-03 10:39:09.000000 one-api-tool-0.4.0/oneapi/utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-03 10:51:46.470515 one-api-tool-0.4.0/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-07-03 10:51:43.000000 one-api-tool-0.4.0/setup.py
```

### Comparing `one-api-tool-0.3.9/LICENSE` & `one-api-tool-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.9/PKG-INFO` & `one-api-tool-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.3.9
+Version: 0.4.0
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.3.9/README.md` & `one-api-tool-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.9/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.4.0/one_api_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.3.9
+Version: 0.4.0
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.3.9/oneapi/commands/one_api_requst.py` & `one-api-tool-0.4.0/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.9/oneapi/one_api.py` & `one-api-tool-0.4.0/oneapi/one_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 from typing import Optional, Sequence, List
 import openai
 import anthropic
 from pydantic import BaseModel
 from abc import ABC, abstractmethod
 import sys
 import os
+from typing import Callable, Optional, Sequence, List
 import tiktoken
 sys.path.append(os.path.normpath(f"{os.path.dirname(os.path.abspath(__file__))}/.."))
+from utils import generate_function_description
 
 CLAUDE_TEMPLATE = "\n\nHuman: {prompt}\n\nAssistant:"
 
 class ChatGPTMessage(BaseModel):
     role: str
     content: str
     
@@ -143,15 +145,17 @@
                 chunk_message = chunk_choice["delta"]  # extract the message
                 finish_reason = chunk_choice["finish_reason"]
                 collected_messages.append(chunk_message)  # save the message
             full_reply_content = "".join([m.get("content", "") for m in collected_messages])
             return full_reply_content
         else:
             if is_function_call:
-                return completion.choices[0].message.get("function_call")
+                function_args = completion.choices[0].message.get("function_call")
+                if function_args is not None:
+                    return function_args
             return completion.choices[0].message.get("content", "")
 
 
     def get_embeddings(self, texts: List[str], engine="text-embedding-ada-002") -> List[List[float]]:
         assert len(texts) <= 2048, "The batch size should not be larger than 2048."
         # replace newlines, which can negatively affect performance.
         texts = [text.replace("\n", " ") for text in texts]
@@ -249,29 +253,35 @@
 
 
     @staticmethod
     def load_json(file_path):
         with open(file_path, "r") as f:
             return json.load(f)
 
-    def simple_chat(self, prompt, system="", functions=None, model="", temperature=1, max_new_tokens=2048, stream=True, **kwargs):
+    def simple_chat(self, prompt: str|list|dict|ChatGPTMessage, system:str="", functions:List[Callable]=None, function_call:Optional[str|dict]=None, model:str="", temperature:int=1, max_new_tokens:int=2048, stream:bool=True, **kwargs):
         if isinstance(self.tool, OpenAITool):
             msgs = [] if not system else [ChatGPTMessage(role="system", content=system)]
             if isinstance(prompt, str):
                 msgs.append(ChatGPTMessage(role="user", content=prompt))
             elif isinstance(prompt, list):
                 msgs.extend(prompt)
             elif isinstance(prompt, (dict, ChatGPTMessage)):
                 msgs.append(prompt)
             else:
                 raise AssertionError(f"Prompt must be a string, list of strings, or ChatGPTMessage. Got {type(prompt)} instead.")
             if isinstance(self.tool.method, AzureMethod):
                 args = AzureDecodingArguments(messages=msgs, engine=model if model else "gpt-35-turbo", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
             elif isinstance(self.tool.method, OpenAIMethod):
-                args = OpenAIDecodingArguments(messages=msgs, functions=functions, function_call="auto" if functions else None, model=model if model else "gpt-3.5-turbo-0613", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
+                if functions is not None and isinstance(functions, list):
+                    functions = [generate_function_description(func) for func in functions]
+                if function_call is None and functions is not None:
+                    function_call = "auto"
+                if function_call is not None and functions is None:
+                    function_call = None
+                args = OpenAIDecodingArguments(messages=msgs, functions=functions, function_call=function_call, model=model if model else "gpt-3.5-turbo-0613", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
         elif isinstance(self.tool, ClaudeAITool):
             args = ClaudeDecodingArguments(prompt=f"{anthropic.HUMAN_PROMPT} {prompt}{anthropic.AI_PROMPT}", model=model if model else "claude-v1.3-100k", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
         else:
             raise AssertionError(f"Not supported api type: {type(self.tool)}")
 
         response = self.tool.simple_chat(args)
         return response
```

### Comparing `one-api-tool-0.3.9/setup.py` & `one-api-tool-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.3.9",
+    version="0.4.0",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

