# Comparing `tmp/simpleaichat-0.2.0.tar.gz` & `tmp/simpleaichat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleaichat-0.2.0.tar", last modified: Mon Jun 19 02:40:51 2023, max compression
+gzip compressed data, was "simpleaichat-0.2.1.tar", last modified: Mon Jul  3 17:55:16 2023, max compression
```

## Comparing `simpleaichat-0.2.0.tar` & `simpleaichat-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-19 02:40:51.970991 simpleaichat-0.2.0/
--rw-r--r--   0 root         (0) staff       (20)     1066 2023-02-18 01:00:20.000000 simpleaichat-0.2.0/LICENSE
--rw-r--r--   0 root         (0) staff       (20)    17755 2023-06-19 02:40:51.970713 simpleaichat-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)    17318 2023-06-19 02:32:32.000000 simpleaichat-0.2.0/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2023-06-19 02:40:51.971068 simpleaichat-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      972 2023-06-19 02:15:51.000000 simpleaichat-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-19 02:40:51.968694 simpleaichat-0.2.0/simpleaichat/
--rw-r--r--   0 root         (0) staff       (20)       46 2023-06-05 04:46:22.000000 simpleaichat-0.2.0/simpleaichat/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    13454 2023-06-19 00:55:23.000000 simpleaichat-0.2.0/simpleaichat/chatgpt.py
--rw-r--r--   0 root         (0) staff       (20)      549 2023-06-08 03:28:41.000000 simpleaichat-0.2.0/simpleaichat/cli.py
--rw-r--r--   0 root         (0) staff       (20)     3185 2023-06-19 01:04:00.000000 simpleaichat-0.2.0/simpleaichat/models.py
--rw-r--r--   0 root         (0) staff       (20)    13529 2023-06-19 02:08:48.000000 simpleaichat-0.2.0/simpleaichat/simpleaichat.py
--rw-r--r--   0 root         (0) staff       (20)     2461 2023-06-19 00:52:23.000000 simpleaichat-0.2.0/simpleaichat/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-19 02:40:51.970078 simpleaichat-0.2.0/simpleaichat.egg-info/
--rw-r--r--   0 root         (0) staff       (20)    17755 2023-06-19 02:40:51.000000 simpleaichat-0.2.0/simpleaichat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      387 2023-06-19 02:40:51.000000 simpleaichat-0.2.0/simpleaichat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-06-19 02:40:51.000000 simpleaichat-0.2.0/simpleaichat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       67 2023-06-19 02:40:51.000000 simpleaichat-0.2.0/simpleaichat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)      112 2023-06-19 02:40:51.000000 simpleaichat-0.2.0/simpleaichat.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       13 2023-06-19 02:40:51.000000 simpleaichat-0.2.0/simpleaichat.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-03 17:55:16.962859 simpleaichat-0.2.1/
+-rw-r--r--   0 root         (0) staff       (20)     1066 2023-02-18 01:00:20.000000 simpleaichat-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)    17755 2023-07-03 17:55:16.962521 simpleaichat-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)    17318 2023-06-19 02:32:32.000000 simpleaichat-0.2.1/README.md
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-07-03 17:55:16.962959 simpleaichat-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      971 2023-07-03 17:43:58.000000 simpleaichat-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-03 17:55:16.960523 simpleaichat-0.2.1/simpleaichat/
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-06-05 04:46:22.000000 simpleaichat-0.2.1/simpleaichat/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    13878 2023-07-03 17:43:58.000000 simpleaichat-0.2.1/simpleaichat/chatgpt.py
+-rw-r--r--   0 root         (0) staff       (20)      549 2023-06-08 03:28:41.000000 simpleaichat-0.2.1/simpleaichat/cli.py
+-rw-r--r--   0 root         (0) staff       (20)     3098 2023-07-03 17:43:58.000000 simpleaichat-0.2.1/simpleaichat/models.py
+-rw-r--r--   0 root         (0) staff       (20)    13550 2023-07-03 17:43:58.000000 simpleaichat-0.2.1/simpleaichat/simpleaichat.py
+-rw-r--r--   0 root         (0) staff       (20)     2800 2023-07-03 17:43:58.000000 simpleaichat-0.2.1/simpleaichat/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-03 17:55:16.962075 simpleaichat-0.2.1/simpleaichat.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)    17755 2023-07-03 17:55:16.000000 simpleaichat-0.2.1/simpleaichat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      387 2023-07-03 17:55:16.000000 simpleaichat-0.2.1/simpleaichat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-07-03 17:55:16.000000 simpleaichat-0.2.1/simpleaichat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       67 2023-07-03 17:55:16.000000 simpleaichat-0.2.1/simpleaichat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)      111 2023-07-03 17:55:16.000000 simpleaichat-0.2.1/simpleaichat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       13 2023-07-03 17:55:16.000000 simpleaichat-0.2.1/simpleaichat.egg-info/top_level.txt
```

### Comparing `simpleaichat-0.2.0/LICENSE` & `simpleaichat-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.2.0/PKG-INFO` & `simpleaichat-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleaichat
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.
 Home-page: https://github.com/minimaxir/simpleaichat
 Author: Max Woolf
 Author-email: max@minimaxir.com
 License: MIT
 Keywords: chatgpt,openai,text generation,ai
 Platform: UNKNOWN
```

### Comparing `simpleaichat-0.2.0/README.md` & `simpleaichat-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.2.0/setup.py` & `simpleaichat-0.2.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup
 
 setup(
     name="simpleaichat",
     packages=["simpleaichat"],  # this must be the same as the name above
-    version="0.2.0",
+    version="0.2.1",
     description="A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="Max Woolf",
     author_email="max@minimaxir.com",
     url="https://github.com/minimaxir/simpleaichat",
     keywords=["chatgpt", "openai", "text generation", "ai"],
     classifiers=[],
     license="MIT",
     entry_points={
         "console_scripts": ["simpleaichat=simpleaichat.cli:interactive_chat"]
     },
     python_requires=">=3.8",
     install_requires=[
-        "pydantic>=1.10",
+        "pydantic>=2.0",
         "fire>=0.3.0",
         "httpx>=0.24.1",
         "python-dotenv>=1.0.0",
         "orjson>=3.9.0",
         "rich>=13.4.1",
         "python-dateutil>=2.8.2",
     ],
```

### Comparing `simpleaichat-0.2.0/simpleaichat/chatgpt.py` & `simpleaichat-0.2.1/simpleaichat/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,55 @@
-from pydantic import HttpUrl
+from pydantic import HttpUrl, ConfigDict
 from httpx import Client, AsyncClient
 from typing import List, Dict, Union, Set, Any
 import orjson
 
 from .models import ChatMessage, ChatSession
+from .utils import remove_a_key
 
 tool_prompt = """From the list of tools below:
 - Reply ONLY with the number of the tool appropriate in response to the user's last message.
 - If no tool is appropriate, ONLY reply with \"0\".
 
 {tools}"""
 
 
 class ChatGPTSession(ChatSession):
     api_url: HttpUrl = "https://api.openai.com/v1/chat/completions"
     input_fields: Set[str] = {"role", "content", "name"}
     system: str = "You are a helpful assistant."
     params: Dict[str, Any] = {"temperature": 0.7}
+    model_config: ConfigDict(arbitrary_types_allowed=True)
 
     def prepare_request(
         self,
         prompt: str,
         system: str = None,
         params: Dict[str, Any] = None,
         stream: bool = False,
         input_schema: Any = None,
         output_schema: Any = None,
+        is_function_calling_required: bool = True,
     ):
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.auth['api_key'].get_secret_value()}",
         }
 
         system_message = ChatMessage(role="system", content=system or self.system)
         if not input_schema:
             user_message = ChatMessage(role="user", content=prompt)
         else:
             assert isinstance(
                 prompt, input_schema
             ), f"prompt must be an instance of {input_schema.__name__}"
             user_message = ChatMessage(
-                role="function", content=prompt.json(), name=input_schema.__name__
+                role="function",
+                content=prompt.model_dump_json(),
+                name=input_schema.__name__,
             )
 
         gen_params = params or self.params
         data = {
             "model": self.model,
             "messages": self.format_input_messages(system_message, user_message),
             "stream": stream,
@@ -55,26 +60,32 @@
         if input_schema or output_schema:
             functions = []
             if input_schema:
                 input_function = self.schema_to_function(input_schema)
                 functions.append(input_function)
             if output_schema:
                 output_function = self.schema_to_function(output_schema)
-                functions.append(output_function)
-                data["function_call"] = {"name": output_schema.__name__}
+                functions.append(
+                    output_function
+                ) if output_function not in functions else None
+                if is_function_calling_required:
+                    data["function_call"] = {"name": output_schema.__name__}
             data["functions"] = functions
 
         return headers, data, user_message
 
     def schema_to_function(self, schema: Any):
         assert schema.__doc__, f"{schema.__name__} is missing a docstring."
+        schema_dict = schema.model_json_schema()
+        remove_a_key(schema_dict, "title")
+
         return {
             "name": schema.__name__,
             "description": schema.__doc__,
-            "parameters": schema.schema(),
+            "parameters": schema_dict,
         }
 
     def gen(
         self,
         prompt: str,
         client: Union[Client, AsyncClient],
         system: str = None,
```

### Comparing `simpleaichat-0.2.0/simpleaichat/cli.py` & `simpleaichat-0.2.1/simpleaichat/cli.py`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.2.0/simpleaichat/models.py` & `simpleaichat-0.2.1/simpleaichat/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,28 +16,24 @@
     # https://stackoverflow.com/a/24666683
     return datetime.datetime.now(datetime.timezone.utc)
 
 
 class ChatMessage(BaseModel):
     role: str
     content: str
-    name: Optional[str]
-    function_call: Optional[str]
+    name: Optional[str] = None
+    function_call: Optional[str] = None
     received_at: datetime.datetime = Field(default_factory=now_tz)
-    finish_reason: Optional[str]
-    prompt_length: Optional[int]
-    completion_length: Optional[int]
-    total_length: Optional[int]
-
-    class Config:
-        json_loads = orjson.loads
-        json_dumps = orjson_dumps
+    finish_reason: Optional[str] = None
+    prompt_length: Optional[int] = None
+    completion_length: Optional[int] = None
+    total_length: Optional[int] = None
 
     def __str__(self) -> str:
-        return self.content
+        return str(self.model_dump(exclude_none=True))
 
 
 class ChatSession(BaseModel):
     id: Union[str, UUID] = Field(default_factory=uuid4)
     created_at: datetime.datetime = Field(default_factory=now_tz)
     auth: Dict[str, SecretStr]
     api_url: HttpUrl
@@ -49,18 +45,14 @@
     recent_messages: Optional[int] = None
     save_messages: Optional[bool] = True
     total_prompt_length: int = 0
     total_completion_length: int = 0
     total_length: int = 0
     title: Optional[str] = None
 
-    class Config:
-        json_loads = orjson.loads
-        json_dumps = orjson_dumps
-
     def __str__(self) -> str:
         sess_start_str = self.created_at.strftime("%Y-%m-%d %H:%M:%S")
         last_message_str = self.messages[-1].received_at.strftime("%Y-%m-%d %H:%M:%S")
         return f"""Chat session started at {sess_start_str}:
         - {len(self.messages):,} Messages
         - Last message sent at {last_message_str}"""
 
@@ -69,20 +61,20 @@
     ) -> list:
         recent_messages = (
             self.messages[-self.recent_messages :]
             if self.recent_messages
             else self.messages
         )
         return (
-            [system_message.dict(include=self.input_fields, exclude_none=True)]
+            [system_message.model_dump(include=self.input_fields, exclude_none=True)]
             + [
-                m.dict(include=self.input_fields, exclude_none=True)
+                m.model_dump(include=self.input_fields, exclude_none=True)
                 for m in recent_messages
             ]
-            + [user_message.dict(include=self.input_fields, exclude_none=True)]
+            + [user_message.model_dump(include=self.input_fields, exclude_none=True)]
         )
 
     def add_messages(
         self,
         user_message: ChatMessage,
         assistant_message: ChatMessage,
         save_messages: bool = None,
```

### Comparing `simpleaichat-0.2.0/simpleaichat/simpleaichat.py` & `simpleaichat-0.2.1/simpleaichat/simpleaichat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 import os
 import datetime
 import dateutil
 from uuid import uuid4, UUID
 from contextlib import contextmanager, asynccontextmanager
 import csv
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 from httpx import Client, AsyncClient
 from typing import List, Dict, Union, Optional, Any
 import orjson
 from dotenv import load_dotenv
 from rich.console import Console
 
 from .utils import wikipedia_search_lookup
-from .models import ChatMessage, ChatSession, orjson_dumps
+from .models import ChatMessage, ChatSession
 from .chatgpt import ChatGPTSession
 
 load_dotenv()
 
 
 class AIChat(BaseModel):
-    client: Union[Client, AsyncClient]
+    client: Any
     default_session: Optional[ChatSession]
     sessions: Dict[Union[str, UUID], ChatSession] = {}
-
-    class Config:
-        arbitrary_types_allowed = True
-        json_loads = orjson.loads
-        json_dumps = orjson_dumps
+    model_config: ConfigDict(arbitrary_types_allowed=True)
 
     def __init__(
         self,
         character: str = None,
         character_command: str = None,
         system: str = None,
         id: Union[str, UUID] = uuid4(),
         prime: bool = True,
         default_session: bool = True,
         console: bool = True,
         **kwargs,
     ):
 
-        client = Client()
+        client = Client(proxies=os.getenv("https_proxy"))
         system_format = self.build_system(character, character_command, system)
 
         sessions = {}
         new_default_session = None
         if default_session:
             new_session = self.new_session(
                 return_session=True, system=system_format, id=id, **kwargs
@@ -69,15 +65,15 @@
         **kwargs,
     ) -> Optional[ChatGPTSession]:
 
         if "model" not in kwargs:  # set default
             kwargs["model"] = "gpt-3.5-turbo"
         # TODO: Add support for more models (PaLM, Claude)
         if "gpt-" in kwargs["model"]:
-            gpt_api_key = os.getenv("OPENAI_API_KEY") or kwargs.get("api_key")
+            gpt_api_key = kwargs.get("api_key") or os.getenv("OPENAI_API_KEY")
             assert gpt_api_key, f"An API key for {kwargs['model'] } was not defined."
             sess = ChatGPTSession(
                 auth={
                     "api_key": gpt_api_key,
                 },
                 **kwargs,
             )
@@ -218,15 +214,15 @@
                 for chunk in sess.stream(user_input, self.client):
                     console.print(chunk["delta"], end="", style=ai_text_color)
             except KeyboardInterrupt:
                 break
 
     def __str__(self) -> str:
         if self.default_session:
-            return self.default_session.json(
+            return self.default_session.model_dump_json(
                 exclude={"api_key", "api_url"},
                 exclude_none=True,
                 option=orjson.OPT_INDENT_2,
             )
 
     def __repr__(self) -> str:
         return ""
@@ -236,15 +232,15 @@
         self,
         output_path: str = None,
         id: Union[str, UUID] = None,
         format: str = "csv",
         minify: bool = False,
     ):
         sess = self.get_session(id)
-        sess_dict = sess.dict(
+        sess_dict = sess.model_dump(
             exclude={"auth", "api_url", "input_fields"},
             exclude_none=True,
         )
         output_path = output_path or f"chat_session.{format}"
         if format == "csv":
             with open(output_path, "w", encoding="utf-8") as f:
                 fields = [
@@ -339,15 +335,15 @@
         params: Dict[str, Any] = None,
         tools: List[Any] = None,
         input_schema: Any = None,
         output_schema: Any = None,
     ) -> str:
         # TODO: move to a __post_init__ in Pydantic 2.0
         if isinstance(self.client, Client):
-            self.client = AsyncClient()
+            self.client = AsyncClient(proxies=os.getenv("https_proxy"))
         sess = self.get_session(id)
         if tools:
             for tool in tools:
                 assert tool.__doc__, f"Tool {tool} does not have a docstring."
             assert len(tools) <= 9, "You can only have a maximum of 9 tools."
             return await sess.gen_with_tools_async(
                 prompt,
@@ -375,15 +371,15 @@
         system: str = None,
         save_messages: bool = None,
         params: Dict[str, Any] = None,
         input_schema: Any = None,
     ) -> str:
         # TODO: move to a __post_init__ in Pydantic 2.0
         if isinstance(self.client, Client):
-            self.client = AsyncClient()
+            self.client = AsyncClient(proxies=os.getenv("https_proxy"))
         sess = self.get_session(id)
         return sess.stream_async(
             prompt,
             client=self.client,
             system=system,
             save_messages=save_messages,
             params=params,
```

### Comparing `simpleaichat-0.2.0/simpleaichat/utils.py` & `simpleaichat-0.2.1/simpleaichat/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import httpx
 from typing import List, Union
 from pydantic import Field
 
 WIKIPEDIA_API_URL = "https://en.wikipedia.org/w/api.php"
 
 
@@ -49,15 +50,15 @@
         "format": "json",
         "srlimit": n,
         "srsearch": query,
         "srwhat": "text",
         "srprop": "",
     }
 
-    async with httpx.AsyncClient() as client:
+    async with httpx.AsyncClient(proxies=os.getenv("https_proxy")) as client:
         r_search = await client.get(WIKIPEDIA_API_URL, params=SEARCH_PARAMS)
     results = [x["title"] for x in r_search.json()["query"]["search"]]
 
     return results[0] if n == 1 else results
 
 
 async def wikipedia_lookup_async(query: str, sentences: int = 1) -> str:
@@ -68,20 +69,30 @@
         "exlimit": "1",
         "explaintext": "1",
         "formatversion": "2",
         "format": "json",
         "titles": query,
     }
 
-    async with httpx.AsyncClient() as client:
+    async with httpx.AsyncClient(proxies=os.getenv("https_proxy")) as client:
         r_lookup = await client.get(WIKIPEDIA_API_URL, params=LOOKUP_PARAMS)
     return r_lookup.json()["query"]["pages"][0]["extract"]
 
 
 async def wikipedia_search_lookup_async(query: str, sentences: int = 1) -> str:
     return await wikipedia_lookup_async(
         await wikipedia_search_async(query, 1), sentences
     )
 
 
 def fd(description: str):
     return Field(description=description)
+
+
+# https://stackoverflow.com/a/58938747
+def remove_a_key(d, remove_key):
+    if isinstance(d, dict):
+        for key in list(d.keys()):
+            if key == remove_key:
+                del d[key]
+            else:
+                remove_a_key(d[key], remove_key)
```

### Comparing `simpleaichat-0.2.0/simpleaichat.egg-info/PKG-INFO` & `simpleaichat-0.2.1/simpleaichat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleaichat
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.
 Home-page: https://github.com/minimaxir/simpleaichat
 Author: Max Woolf
 Author-email: max@minimaxir.com
 License: MIT
 Keywords: chatgpt,openai,text generation,ai
 Platform: UNKNOWN
```

