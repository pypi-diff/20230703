# Comparing `tmp/nonebot-plugin-alconna-0.8.4.tar.gz` & `tmp/nonebot-plugin-alconna-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-alconna-0.8.4.tar", last modified: Thu Jun 29 04:33:23 2023, max compression
+gzip compressed data, was "nonebot-plugin-alconna-0.9.0.tar", last modified: Mon Jul  3 13:04:57 2023, max compression
```

## Comparing `nonebot-plugin-alconna-0.8.4.tar` & `nonebot-plugin-alconna-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.8.4/LICENSE
--rw-r--r--   0        0        0     1524 2023-06-29 04:17:15.910056 nonebot-plugin-alconna-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     8588 2023-06-22 14:46:56.528495 nonebot-plugin-alconna-0.8.4/README.md
--rw-r--r--   0        0        0     1912 2023-06-29 04:17:15.890561 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/__init__.py
--rw-r--r--   0        0        0     6364 2023-06-29 04:17:15.903159 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/__init__.py
--rw-r--r--   0        0        0      523 2023-05-31 10:32:51.256024 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/bilibili.py
--rw-r--r--   0        0        0     1052 2023-05-31 10:32:51.263057 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/console.py
--rw-r--r--   0        0        0     1661 2023-05-31 10:32:51.272058 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/ding.py
--rw-r--r--   0        0        0     2120 2023-05-31 10:32:51.280029 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/feishu.py
--rw-r--r--   0        0        0      519 2023-05-31 10:32:51.286108 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/github.py
--rw-r--r--   0        0        0     1163 2023-05-31 10:32:51.293032 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/kook.py
--rw-r--r--   0        0        0      761 2023-05-31 10:32:51.300025 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/minecraft.py
--rw-r--r--   0        0        0     3129 2023-05-31 10:32:51.308024 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/mirai.py
--rw-r--r--   0        0        0     1088 2023-05-31 10:32:51.314025 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/ntchat.py
--rw-r--r--   0        0        0     3151 2023-05-31 10:32:51.321077 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/onebot11.py
--rw-r--r--   0        0        0     2496 2023-05-31 10:32:51.327029 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/onebot12.py
--rw-r--r--   0        0        0     3251 2023-05-31 10:32:51.334314 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/qqguild.py
--rw-r--r--   0        0        0     3224 2023-06-22 16:21:04.989803 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/telegram.py
--rw-r--r--   0        0        0      579 2023-05-31 10:32:51.160062 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/argv.py
--rw-r--r--   0        0        0      405 2023-05-31 10:32:51.165611 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/config.py
--rw-r--r--   0        0        0      182 2023-05-31 10:31:14.855148 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/consts.py
--rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/i18n/.config.json
--rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/i18n/en-US.json
--rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0     2277 2023-06-01 08:39:16.821566 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/matcher.py
--rw-r--r--   0        0        0     1091 2023-05-31 10:32:51.198463 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/matcher.pyi
--rw-r--r--   0        0        0     1478 2023-05-31 10:32:51.204511 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/model.py
--rw-r--r--   0        0        0     3830 2023-05-31 10:32:51.214457 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/params.py
--rw-r--r--   0        0        0     8779 2023-06-28 10:23:05.446107 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/rule.py
--rw-r--r--   0        0        0     2357 2023-06-29 04:28:10.876299 nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/typings.py
--rw-r--r--   0        0        0     8665 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1551 2023-07-03 12:34:25.733263 nonebot-plugin-alconna-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8878 2023-07-03 13:02:02.807832 nonebot-plugin-alconna-0.9.0/README.md
+-rw-r--r--   0        0        0     1959 2023-07-03 12:27:47.197059 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/__init__.py
+-rw-r--r--   0        0        0     6364 2023-06-29 04:17:15.903159 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-31 10:32:51.256024 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/bilibili.py
+-rw-r--r--   0        0        0     1052 2023-05-31 10:32:51.263057 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/console.py
+-rw-r--r--   0        0        0     1661 2023-05-31 10:32:51.272058 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/ding.py
+-rw-r--r--   0        0        0     2120 2023-05-31 10:32:51.280029 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/feishu.py
+-rw-r--r--   0        0        0      519 2023-05-31 10:32:51.286108 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/github.py
+-rw-r--r--   0        0        0     1163 2023-05-31 10:32:51.293032 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/kook.py
+-rw-r--r--   0        0        0      761 2023-05-31 10:32:51.300025 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/minecraft.py
+-rw-r--r--   0        0        0     3129 2023-05-31 10:32:51.308024 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/mirai.py
+-rw-r--r--   0        0        0     1088 2023-05-31 10:32:51.314025 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/ntchat.py
+-rw-r--r--   0        0        0     3151 2023-05-31 10:32:51.321077 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/onebot11.py
+-rw-r--r--   0        0        0     2496 2023-05-31 10:32:51.327029 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/onebot12.py
+-rw-r--r--   0        0        0     3251 2023-05-31 10:32:51.334314 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/qqguild.py
+-rw-r--r--   0        0        0     3224 2023-06-22 16:21:04.989803 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/telegram.py
+-rw-r--r--   0        0        0      579 2023-05-31 10:32:51.160062 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/argv.py
+-rw-r--r--   0        0        0      405 2023-05-31 10:32:51.165611 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/config.py
+-rw-r--r--   0        0        0      182 2023-05-31 10:31:14.855148 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/consts.py
+-rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/i18n/.config.json
+-rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/i18n/en-US.json
+-rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0     3638 2023-07-03 12:51:09.077940 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/matcher.py
+-rw-r--r--   0        0        0     1323 2023-07-03 13:01:00.887691 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/matcher.pyi
+-rw-r--r--   0        0        0     1478 2023-05-31 10:32:51.204511 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/model.py
+-rw-r--r--   0        0        0     3830 2023-05-31 10:32:51.214457 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/params.py
+-rw-r--r--   0        0        0     8779 2023-06-28 10:23:05.446107 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/rule.py
+-rw-r--r--   0        0        0     2528 2023-07-03 13:01:00.957077 nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/typings.py
+-rw-r--r--   0        0        0     8945 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.9.0/PKG-INFO
```

### Comparing `nonebot-plugin-alconna-0.8.4/LICENSE` & `nonebot-plugin-alconna-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/pyproject.toml` & `nonebot-plugin-alconna-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "nonebot-plugin-alconna"
-version = "0.8.4"
+version = "0.9.0"
 description = "Alconna Adapter for Nonebot"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc4",
-    "arclet-alconna<2.0.0, >=1.7.7",
-    "arclet-alconna-tools<0.7.0, >=0.6.1",
+    "arclet-alconna<2.0.0, >=1.7.10",
+    "arclet-alconna-tools<0.7.0, >=0.6.3",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "command",
     "argparse",
     "cli",
@@ -30,15 +30,15 @@
 requires = [
     "pdm-pep517>=1.0",
 ]
 build-backend = "pdm.pep517.api"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "nonebot2>=2.0.0",
+    "nonebot2[fastapi,httpx,websockets]>=2.0.0",
     "fix-future-annotations>=0.5.0",
     "nonebot-adapter-onebot>=2.2.3",
     "nonebot-adapter-feishu>=2.0.0b8",
     "nonebot-adapter-console>=0.3.2",
     "nonebot-adapter-ding>=2.0.0a16",
     "nonebot-adapter-mirai2>=0.0.22",
     "nonebot-adapter-minecraft>=0.1.1",
```

### Comparing `nonebot-plugin-alconna-0.8.4/README.md` & `nonebot-plugin-alconna-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -270,12 +270,22 @@
 | [开黑啦](https://developer.kookapp.cn/)                                | adapters.kook                        |
 | [Mirai](https://docs.mirai.mamoe.net/mirai-api-http/)               | adapters.mirai                       |
 | [Ntchat](https://github.com/JustUndertaker/adapter-ntchat)          | adapters.ntchat                      |
 | [MineCraft](https://github.com/17TheWord/nonebot-adapter-minecraft) | adapters.minecraft                   |
 | [BiliBili Live](https://github.com/wwweww/adapter-bilibili)         | adapters.bilibili                    |
 
 
+### 便捷装饰器
 
+`funcommand` 装饰器用于将一个接受任意参数，返回 `str` 或 `Message` 或 `MessageSegment` 的函数转换为命令响应器。
+
+```python
+from nonebot_plugin_alconna import funcommand
+
+@funcommand()
+async def echo(msg: str):
+    return msg
+```
 
 ## 体验
 
 [demo bot](./src/test/plugins/demo.py)
```

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/__init__.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from nonebot import __version__ as nonebot_version
 from nonebot.plugin import PluginMetadata
 
 from .argv import MessageArgv as MessageArgv
 from .consts import ALCONNA_RESULT as ALCONNA_RESULT
 from .matcher import on_alconna as on_alconna
+from .matcher import funcommand as funcommand
 from .model import CommandResult as CommandResult
 from .model import Match as Match
 from .model import Query as Query
 from .params import AlcMatches as AlcMatches
 from .params import AlcResult as AlcResult
 from .params import AlconnaDuplication as AlconnaDuplication
 from .params import AlconnaMatch as AlconnaMatch
@@ -18,15 +19,15 @@
 from .params import assign as assign
 from .params import match_path as match_path
 from .params import match_value as match_value
 from .rule import alconna as alconna
 from .rule import set_output_converter as set_output_converter
 from .config import Config
 
-__version__ = "0.8.4"
+__version__ = "0.9.0"
 
 _meta_source = {
     "name": "Alconna 插件",
     "description": "提供 [Alconna](https://github.com/ArcletProject/Alconna) 的 Nonebot2 适配版本与工具",
     "usage": "matcher = on_alconna(...)",
     "homepage": "https://github.com/ArcletProject/Alconna",
     "type": "library",
```

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/__init__.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/bilibili.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/bilibili.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/console.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/ding.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/ding.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/feishu.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/feishu.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/github.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/github.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/kook.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/kook.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/minecraft.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/minecraft.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/mirai.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/mirai.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/ntchat.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/ntchat.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/onebot11.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/onebot11.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/onebot12.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/onebot12.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/qqguild.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/adapters/telegram.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/argv.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/argv.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/matcher.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/matcher.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from __future__ import annotations
 
+from typing import Callable
+
 from arclet.alconna import Alconna, command_manager
 from arclet.alconna.tools import AlconnaFormat
+from arclet.alconna.tools.construct import FuncMounter
+from tarina import is_awaitable
 from nonebot.matcher import Matcher
 from nonebot.plugin.on import on_message
 from nonebot.rule import Rule
 from nonebot.typing import T_RuleChecker
+from nonebot.internal.adapter import Bot, Event, Message, MessageSegment
 
 from .model import CompConfig
 from .rule import alconna
 from .typings import TConvert
 
 
 def on_alconna(
@@ -58,7 +63,45 @@
             output_converter,
             comp_config
         ) & rule,
         *args,
         **kwargs,
         _depth=_depth + 1  # type: ignore
     )
+
+
+def funcommand(
+    name: str | None = None,
+    prefixes: list[str] | None = None,
+    description: str | None = None,
+):
+    _config = {"raise_exception": False}
+    if name:
+        _config["name"] = name
+    if prefixes:
+        _config["prefixes"] = prefixes
+    if description:
+        _config["description"] = description
+    def wrapper(func: Callable) -> type[Matcher]:
+        alc = FuncMounter(func, _config)  # type: ignore
+
+        async def handle(bot: Bot, event: Event):
+            msg = getattr(event, "original_message", event.get_message())
+            try:
+                arp, res = alc.exec(msg)
+            except Exception as e:
+                if _config["raise_exception"]:
+                    raise e
+                await bot.send(event, str(e))
+                return
+            if arp.matched:
+                if is_awaitable(res):
+                    res = await res
+                if isinstance(res, (str, Message, MessageSegment)):
+                    await bot.send(event, res)
+
+        matcher = on_alconna(alc)
+        matcher.handle()(handle)
+
+        return matcher
+
+    return wrapper
```

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/matcher.pyi` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/matcher.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 from datetime import datetime, timedelta
+from typing import Callable
 
 from arclet.alconna import Alconna
 from nonebot.dependencies import Dependent
 from nonebot.matcher import Matcher
 from nonebot.permission import Permission
 from nonebot.rule import Rule
 from nonebot.typing import T_Handler, T_PermissionChecker, T_RuleChecker, T_State
 from nonebot_plugin_alconna.model import CompConfig
-from nonebot_plugin_alconna.typings import TConvert
+from nonebot_plugin_alconna.typings import TConvert, MReturn
 
 def on_alconna(
     command: Alconna | str,
     rule: Rule | T_RuleChecker | None = None,
     skip_for_unmatch: bool = True,
     auto_send_output: bool = False,
     output_converter: TConvert | None = None,
@@ -24,7 +25,15 @@
     handlers: list[T_Handler | Dependent] | None = ...,
     temp: bool = ...,
     expire_time: datetime | timedelta | None = ...,
     priority: int = ...,
     block: bool = ...,
     state: T_State | None = ...,
 ) -> type[Matcher]: ...
+
+
+def funcommand(
+    name: str | None = None,
+    prefixes: list[str] | None = None,
+    description: str | None = None,
+) -> Callable[[Callable[..., MReturn]], type[Matcher]]:
+    ...
```

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/model.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/model.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/params.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/params.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/rule.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.8.4/src/nonebot_plugin_alconna/typings.py` & `nonebot-plugin-alconna-0.9.0/src/nonebot_plugin_alconna/typings.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from nepattern import BasePattern, MatchFailed, PatternModel
 from nonebot.internal.adapter.message import Message, MessageSegment
 from tarina import lang
 
 T = TypeVar("T")
 TMS = TypeVar("TMS", bound=MessageSegment)
+TCallable = TypeVar("TCallable", bound=Callable[..., Any])
 P = ParamSpec("P")
 
 
 class SegmentPattern(BasePattern[TMS], Generic[TMS, P]):
     def __init__(
         self,
         name: str,
@@ -43,15 +44,15 @@
 
     def __call__(self, *args: P.args, **kwargs: P.kwargs) -> TMS:
         return self.call(*args, **kwargs)  # type: ignore
 
 
 OutputType = Literal["help", "shortcut", "completion"]
 TConvert: TypeAlias = Callable[[OutputType, str], Union[Message, Awaitable[Message]]]
-
+MReturn: TypeAlias = Union[Union[str, Message, MessageSegment], Awaitable[Union[str, Message, MessageSegment]]]
 
 def _isinstance(seg: MessageSegment, mapping: dict[str, Callable[[MessageSegment], Any]]):
     if (key := seg.type) in mapping and (res := mapping[key](seg)):
         return res
     if "*" in mapping and (res := mapping["*"](seg)):
         return res
```

### Comparing `nonebot-plugin-alconna-0.8.4/PKG-INFO` & `nonebot-plugin-alconna-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-alconna
-Version: 0.8.4
+Version: 0.9.0
 Summary: Alconna Adapter for Nonebot
 License: MIT
 Keywords: command,argparse,cli,alconna,nonebot
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Project-URL: repository, https://github.com/ArcletProject/nonebot-plugin-alconna
 Description-Content-Type: text/markdown
@@ -281,13 +281,23 @@
 | [开黑啦](https://developer.kookapp.cn/)                                | adapters.kook                        |
 | [Mirai](https://docs.mirai.mamoe.net/mirai-api-http/)               | adapters.mirai                       |
 | [Ntchat](https://github.com/JustUndertaker/adapter-ntchat)          | adapters.ntchat                      |
 | [MineCraft](https://github.com/17TheWord/nonebot-adapter-minecraft) | adapters.minecraft                   |
 | [BiliBili Live](https://github.com/wwweww/adapter-bilibili)         | adapters.bilibili                    |
 
 
+### 便捷装饰器
 
+`funcommand` 装饰器用于将一个接受任意参数，返回 `str` 或 `Message` 或 `MessageSegment` 的函数转换为命令响应器。
+
+```python
+from nonebot_plugin_alconna import funcommand
+
+@funcommand()
+async def echo(msg: str):
+    return msg
+```
 
 ## 体验
 
 [demo bot](./src/test/plugins/demo.py)
```

