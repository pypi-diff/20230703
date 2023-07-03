# Comparing `tmp/xiaogpt-1.50.tar.gz` & `tmp/xiaogpt-1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-1.50.tar", last modified: Tue Jun 27 13:12:47 2023, max compression
+gzip compressed data, was "xiaogpt-1.51.tar", last modified: Mon Jul  3 01:31:05 2023, max compression
```

## Comparing `xiaogpt-1.50.tar` & `xiaogpt-1.51.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-06-27 13:12:34.775396 xiaogpt-1.50/LICENSE
--rw-r--r--   0        0        0    11480 2023-06-27 13:12:34.775396 xiaogpt-1.50/README.md
--rw-r--r--   0        0        0      919 2023-06-27 13:12:47.207531 xiaogpt-1.50/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/__main__.py
--rw-r--r--   0        0        0      639 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0      554 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3280 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1605 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/bot/gpt3_bot.py
--rw-r--r--   0        0        0     1996 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3415 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/cli.py
--rw-r--r--   0        0        0     5318 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/config.py
--rw-r--r--   0        0        0     2071 2023-06-27 13:12:34.775396 xiaogpt-1.50/xiaogpt/utils.py
--rw-r--r--   0        0        0    18548 2023-06-27 13:12:34.779396 xiaogpt-1.50/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    12066 1970-01-01 00:00:00.000000 xiaogpt-1.50/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-03 01:30:57.265165 xiaogpt-1.51/LICENSE
+-rw-r--r--   0        0        0    11816 2023-07-03 01:30:57.265165 xiaogpt-1.51/README.md
+-rw-r--r--   0        0        0      934 2023-07-03 01:31:05.665095 xiaogpt-1.51/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/__main__.py
+-rw-r--r--   0        0        0      707 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0      554 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3280 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1252 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     1638 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/bot/gpt3_bot.py
+-rw-r--r--   0        0        0     1996 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3821 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/cli.py
+-rw-r--r--   0        0        0     5366 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/config.py
+-rw-r--r--   0        0        0     2071 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/utils.py
+-rw-r--r--   0        0        0    18700 2023-07-03 01:30:57.269165 xiaogpt-1.51/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    12425 1970-01-01 00:00:00.000000 xiaogpt-1.51/PKG-INFO
```

### Comparing `xiaogpt-1.50/LICENSE` & `xiaogpt-1.51/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.50/README.md` & `xiaogpt-1.51/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ![image](https://user-images.githubusercontent.com/15976103/226802344-9c71f543-b73c-4a47-8703-4c200c434dec.png)
 
 ## 支持的 AI 类型
 
 - GPT3
 - ChatGPT
 - New Bing 
+- [ChatGLM](http://open.bigmodel.cn/)
 
 ## Windows 获取小米音响DID
 
 1. `pip install miservice_fork`
 2. `set MI_USER=xxxx`
 3. `set MI_PASS=xxx`
 4. 得到did
@@ -87,14 +88,17 @@
 # 如果你想 mute 小米的回答
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai
 # 使用流式响应，获得更快的响应
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --stream
 # 如果你想使用 gpt3 ai
 export OPENAI_API_KEY=${your_api_key}
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gpt3
+
+# 如果你想使用 ChatGLM api
+python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_glm --glm_key ${glm_key}
 ```
 
 ## config.json
 如果想通过单一配置文件启动也是可以的, 可以通过 `--config` 参数指定配置文件, config 文件必须是合法的 JSON 格式
 参数优先级
 - cli args > default > config
 
@@ -118,22 +122,24 @@
         "temperature": 0.9,
         "top_p": 0.9,
     }
 }
 ```
 
 具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
+ChatGLM [文档](http://open.bigmodel.cn/doc/api#chatglm_130b)
 ## 配置项说明
 
 | 参数                  | 说明                                              | 默认值                              |
 | --------------------- | ------------------------------------------------- | ----------------------------------- |
 | hardware              | 设备型号                                          |                                     |
 | account               | 小爱账户                                          |                                     |
 | password              | 小爱账户密码                                      |                                     |
 | openai_key            | openai的apikey                                    |                                     |
+| glm_key               | chatglm 的 apikey                                    |                                     |
 | cookie                | 小爱账户cookie （如果用上面密码登录可以不填）     |                                     |
 | mi_did                | 设备did                                           |                                     |
 | use_command           | 使用 MI command 与小爱交互                        | `false`                             |
 | mute_xiaoai           | 快速停掉小爱自己的回答                            | `true`                              |
 | verbose               | 是否打印详细日志                                  | `false`                             |
 | bot                   | 使用的 bot 类型，目前支持gpt3,chatgptapi和newbing | `chatgptapi`                        |
 | enable_edge_tts       | 使用Edge TTS                                      | `false`                             |
```

### Comparing `xiaogpt-1.50/pyproject.toml` & `xiaogpt-1.51/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 ]
 requires-python = ">=3.7.1"
 dependencies = [
     "miservice_fork",
     "openai",
     "aiohttp",
     "rich",
+    "zhipuai",
     "edge-tts>=6.1.3",
     "EdgeGPT==0.1.26",
 ]
 dynamic = []
-version = "1.50"
+version = "1.51"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-1.50/xiaogpt/bot/__init__.py` & `xiaogpt-1.51/xiaogpt/bot/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 from xiaogpt.bot.base_bot import BaseBot
 from xiaogpt.bot.chatgptapi_bot import ChatGPTBot
 from xiaogpt.bot.gpt3_bot import GPT3Bot
 from xiaogpt.bot.newbing_bot import NewBingBot
+from xiaogpt.bot.glm_bot import GLMBot
 from xiaogpt.config import Config
 
 BOTS: dict[str, type[BaseBot]] = {
     "gpt3": GPT3Bot,
     "newbing": NewBingBot,
     "chatgptapi": ChatGPTBot,
+    "glm": GLMBot,
 }
 
 
 def get_bot(config: Config) -> BaseBot:
     try:
         return BOTS[config.bot].from_config(config)
     except KeyError:
         raise ValueError(f"Unsupported bot {config.bot}, must be one of {list(BOTS)}")
 
 
-__all__ = ["GPT3Bot", "ChatGPTBot", "NewBingBot", "get_bot"]
+__all__ = ["GPT3Bot", "ChatGPTBot", "NewBingBot", "GLMBot", "get_bot"]
```

### Comparing `xiaogpt-1.50/xiaogpt/bot/base_bot.py` & `xiaogpt-1.51/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.50/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-1.51/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.50/xiaogpt/bot/gpt3_bot.py` & `xiaogpt-1.51/xiaogpt/bot/gpt3_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,16 @@
             "stream": True,
             **options,
         }
         completion = await openai.Completion.acreate(**data)
 
         async def text_gen():
             async for event in completion:
-                print(event["text"], end="")
-                yield event["text"]
+                text = event["choices"][0]["text"]
+                print(text, end="")
+                yield text
 
         try:
             async for sentence in split_sentences(text_gen()):
                 yield sentence
         finally:
             print()
```

### Comparing `xiaogpt-1.50/xiaogpt/bot/newbing_bot.py` & `xiaogpt-1.51/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.50/xiaogpt/cli.py` & `xiaogpt-1.51/xiaogpt/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,19 @@
     )
     parser.add_argument(
         "--openai_key",
         dest="openai_key",
         help="openai api key",
     )
     parser.add_argument(
+        "--glm_key",
+        dest="glm_key",
+        help="chatglm api key",
+    )
+    parser.add_argument(
         "--proxy",
         dest="proxy",
         help="http proxy url like http://localhost:8080",
     )
     parser.add_argument(
         "--cookie",
         dest="cookie",
@@ -90,21 +95,31 @@
     group.add_argument(
         "--use_newbing",
         dest="bot",
         action="store_const",
         const="newbing",
         help="if use newbing",
     )
+    group.add_argument(
+        "--use_glm",
+        dest="bot",
+        action="store_const",
+        const="glm",
+        help="if use chatglm",
+    )
     parser.add_argument(
         "--bing_cookie_path",
         dest="bing_cookie_path",
         help="new bing cookies path if use new bing",
     )
     group.add_argument(
-        "--bot", dest="bot", help="bot type", choices=["gpt3", "chatgptapi", "newbing"]
+        "--bot",
+        dest="bot",
+        help="bot type",
+        choices=["gpt3", "chatgptapi", "newbing", "glm"],
     )
     parser.add_argument(
         "--config",
         dest="config",
         help="config file path",
     )
     # args to change api_base
@@ -125,14 +140,16 @@
     parser.add_argument(
         "--deployment_id",
         dest="deployment_id",
         help="specify deployment id, only used when api_base points to azure",
     )
 
     options = parser.parse_args()
+    if options.bot == "glm" and options.stream:
+        raise Exception("For now ChatGLM do not support stream")
     config = Config.from_options(options)
 
     miboy = MiGPT(config)
     loop = asyncio.get_event_loop()
     loop.run_until_complete(miboy.run_forever())
```

### Comparing `xiaogpt-1.50/xiaogpt/config.py` & `xiaogpt-1.51/xiaogpt/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
 @dataclass
 class Config:
     hardware: str = "LX06"
     account: str = os.getenv("MI_USER", "")
     password: str = os.getenv("MI_PASS", "")
     openai_key: str = os.getenv("OPENAI_API_KEY", "")
+    glm_key: str = os.getenv("CHATGLM_KEY", "")
     proxy: str | None = None
     mi_did: str = os.getenv("MI_DID", "")
     keyword: Iterable[str] = KEY_WORD
     change_prompt_keyword: Iterable[str] = CHANGE_PROMPT_KEY_WORD
     prompt: str = PROMPT
     mute_xiaoai: bool = False
     bot: str = "chatgpt"
```

### Comparing `xiaogpt-1.50/xiaogpt/utils.py` & `xiaogpt-1.51/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.50/xiaogpt/xiaogpt.py` & `xiaogpt-1.51/xiaogpt/xiaogpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,18 @@
         message = message.replace('"', "，")
         return message
 
     async def ask_gpt(self, query):
         if not self.config.stream:
             async with ClientSession(trust_env=True) as session:
                 openai.aiosession.set(session)
-                answer = await self.chatbot.ask(query, **self.config.gpt_options)
+                if self.config.bot == "glm":
+                    answer = self._chatbot.ask(query, **self.config.gpt_options)
+                else:
+                    answer = await self.chatbot.ask(query, **self.config.gpt_options)
                 message = self._normalize(answer) if answer else ""
                 yield message
                 return
 
         async def collect_stream(queue):
             async with ClientSession(trust_env=True) as session:
                 openai.aiosession.set(session)
```

### Comparing `xiaogpt-1.50/PKG-INFO` & `xiaogpt-1.51/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 1.50
+Version: 1.51
 Summary: Play ChatGPT with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
 Requires-Python: >=3.7.1
 Requires-Dist: miservice_fork
 Requires-Dist: openai
 Requires-Dist: aiohttp
 Requires-Dist: rich
+Requires-Dist: zhipuai
 Requires-Dist: edge-tts>=6.1.3
 Requires-Dist: EdgeGPT==0.1.26
 Description-Content-Type: text/markdown
 
 # xiaogpt
 
 [![PyPI](https://img.shields.io/pypi/v/xiaogpt?style=flat-square)](https://pypi.org/project/xiaogpt)
@@ -32,14 +33,15 @@
 ![image](https://user-images.githubusercontent.com/15976103/226802344-9c71f543-b73c-4a47-8703-4c200c434dec.png)
 
 ## 支持的 AI 类型
 
 - GPT3
 - ChatGPT
 - New Bing 
+- [ChatGLM](http://open.bigmodel.cn/)
 
 ## Windows 获取小米音响DID
 
 1. `pip install miservice_fork`
 2. `set MI_USER=xxxx`
 3. `set MI_PASS=xxx`
 4. 得到did
@@ -106,14 +108,17 @@
 # 如果你想 mute 小米的回答
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai
 # 使用流式响应，获得更快的响应
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --stream
 # 如果你想使用 gpt3 ai
 export OPENAI_API_KEY=${your_api_key}
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gpt3
+
+# 如果你想使用 ChatGLM api
+python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_glm --glm_key ${glm_key}
 ```
 
 ## config.json
 如果想通过单一配置文件启动也是可以的, 可以通过 `--config` 参数指定配置文件, config 文件必须是合法的 JSON 格式
 参数优先级
 - cli args > default > config
 
@@ -137,22 +142,24 @@
         "temperature": 0.9,
         "top_p": 0.9,
     }
 }
 ```
 
 具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
+ChatGLM [文档](http://open.bigmodel.cn/doc/api#chatglm_130b)
 ## 配置项说明
 
 | 参数                  | 说明                                              | 默认值                              |
 | --------------------- | ------------------------------------------------- | ----------------------------------- |
 | hardware              | 设备型号                                          |                                     |
 | account               | 小爱账户                                          |                                     |
 | password              | 小爱账户密码                                      |                                     |
 | openai_key            | openai的apikey                                    |                                     |
+| glm_key               | chatglm 的 apikey                                    |                                     |
 | cookie                | 小爱账户cookie （如果用上面密码登录可以不填）     |                                     |
 | mi_did                | 设备did                                           |                                     |
 | use_command           | 使用 MI command 与小爱交互                        | `false`                             |
 | mute_xiaoai           | 快速停掉小爱自己的回答                            | `true`                              |
 | verbose               | 是否打印详细日志                                  | `false`                             |
 | bot                   | 使用的 bot 类型，目前支持gpt3,chatgptapi和newbing | `chatgptapi`                        |
 | enable_edge_tts       | 使用Edge TTS                                      | `false`                             |
```

