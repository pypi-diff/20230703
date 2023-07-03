# Comparing `tmp/nonebot-plugin-mcqq-1.2.5.post1.tar.gz` & `tmp/nonebot-plugin-mcqq-1.2.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcqq-1.2.5.post1.tar", last modified: Sun Jun 25 05:26:49 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcqq-1.2.6.post1.tar", last modified: Mon Jul  3 03:50:31 2023, max compression
```

## Comparing `nonebot-plugin-mcqq-1.2.5.post1.tar` & `nonebot-plugin-mcqq-1.2.6.post1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:26:49.189223 nonebot-plugin-mcqq-1.2.5.post1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-25 05:26:43.000000 nonebot-plugin-mcqq-1.2.5.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-25 05:26:49.189223 nonebot-plugin-mcqq-1.2.5.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-25 05:26:43.000000 nonebot-plugin-mcqq-1.2.5.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:26:49.189223 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-25 05:26:43.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-25 05:26:43.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-25 05:26:43.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:26:49.189223 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-25 05:26:49.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-25 05:26:49.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:26:49.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-25 05:26:49.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-25 05:26:49.000000 nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 05:26:49.189223 nonebot-plugin-mcqq-1.2.5.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-25 05:26:43.000000 nonebot-plugin-mcqq-1.2.5.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:50:31.894468 nonebot-plugin-mcqq-1.2.6.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-03 03:50:24.000000 nonebot-plugin-mcqq-1.2.6.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-03 03:50:31.894468 nonebot-plugin-mcqq-1.2.6.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-03 03:50:24.000000 nonebot-plugin-mcqq-1.2.6.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:50:31.890468 nonebot-plugin-mcqq-1.2.6.post1/nonebot_plugin_mcqq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-03 03:50:24.000000 nonebot-plugin-mcqq-1.2.6.post1/nonebot_plugin_mcqq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-03 03:50:24.000000 nonebot-plugin-mcqq-1.2.6.post1/nonebot_plugin_mcqq/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-03 03:50:24.000000 nonebot-plugin-mcqq-1.2.6.post1/nonebot_plugin_mcqq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:50:31.894468 nonebot-plugin-mcqq-1.2.6.post1/nonebot_plugin_mcqq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-03 03:50:31.000000 nonebot-plugin-mcqq-1.2.6.post1/nonebot_plugin_mcqq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-03 03:50:31.000000 nonebot-plugin-mcqq-1.2.6.post1/nonebot_plugin_mcqq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 03:50:31.000000 nonebot-plugin-mcqq-1.2.6.post1/nonebot_plugin_mcqq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-03 03:50:31.000000 nonebot-plugin-mcqq-1.2.6.post1/nonebot_plugin_mcqq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 03:50:31.000000 nonebot-plugin-mcqq-1.2.6.post1/nonebot_plugin_mcqq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 03:50:31.894468 nonebot-plugin-mcqq-1.2.6.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-03 03:50:24.000000 nonebot-plugin-mcqq-1.2.6.post1/setup.py
```

### Comparing `nonebot-plugin-mcqq-1.2.5.post1/LICENSE` & `nonebot-plugin-mcqq-1.2.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.5.post1/PKG-INFO` & `nonebot-plugin-mcqq-1.2.6.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.2.5.post1
+Version: 1.2.6.post1
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -16,23 +16,21 @@
 # NoneBot-Plugin-MCQQ
 
 基于 `NoneBot` 的与 `Minecraft Server` 互通消息插件
 
 - 支持QQ群、QQ频道
 - 支持多个服务器与多个群聊的互通
 
-推荐使用功能更为完整的 [`青岚 Bot`](https://github.com/17TheWord/qinglan_bot)
-
 # 文档
 
 - [正在不断更新的文档](https://17theword.github.io/mc_qq/)
 
 # 支持的服务端列表
 
-- Spigot
+- Spigot API
     - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq`
 - MinecraftServer
     - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 - ForgeServer
     - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 - Fabric
     - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
```

### Comparing `nonebot-plugin-mcqq-1.2.5.post1/README.md` & `nonebot-plugin-mcqq-1.2.6.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 # NoneBot-Plugin-MCQQ
 
 基于 `NoneBot` 的与 `Minecraft Server` 互通消息插件
 
 - 支持QQ群、QQ频道
 - 支持多个服务器与多个群聊的互通
 
-推荐使用功能更为完整的 [`青岚 Bot`](https://github.com/17TheWord/qinglan_bot)
-
 # 文档
 
 - [正在不断更新的文档](https://17theword.github.io/mc_qq/)
 
 # 支持的服务端列表
 
-- Spigot
+- Spigot API
     - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq`
 - MinecraftServer
     - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 - ForgeServer
     - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 - Fabric
     - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
```

### Comparing `nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq/__init__.py` & `nonebot-plugin-mcqq-1.2.6.post1/nonebot_plugin_mcqq/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from typing import Union
 
-from nonebot import on_message, on_command, get_driver, require
-
-require("nonebot_plugin_guild_patch")
-
-from nonebot.params import CommandArg
-from nonebot.adapters import Message
-from nonebot.plugin import PluginMetadata
-from nonebot.permission import SUPERUSER
-from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, GROUP_ADMIN, GROUP_OWNER
-from mcqq_tool.config import Config
 from mcqq_tool.common import GUILD_ADMIN
+from mcqq_tool.config import Config
 from mcqq_tool.utils import send_msg_to_mc, send_cmd_to_mc
 
+from nonebot import on_message, on_command, get_driver, ReverseDriver
+from nonebot.adapters import Message
+from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, GROUP_ADMIN, GROUP_OWNER
+from nonebot.params import CommandArg
+from nonebot.permission import SUPERUSER
+from nonebot.plugin import PluginMetadata
 from nonebot_plugin_guild_patch import GuildMessageEvent
 
-from .data_source import start_ws_server, stop_ws_server
+from .data_source import set_route
 from .utils import msg_rule
 
 __plugin_meta__ = PluginMetadata(
     name="MC_QQ",
     description="基于NoneBot的与Minecraft Server互通消息的插件",
     homepage="https://github.com/17TheWord/nonebot-plugin-mcqq",
     usage="在群聊发送消息即可同步至 Minecraft 服务器",
@@ -34,24 +31,19 @@
 
 mc_qq_cmd = on_command("minecraft_command", aliases={"mcc"}, priority=1, rule=msg_rule, block=True)
 
 driver = get_driver()
 
 
 # bot连接时
-@driver.on_bot_connect
+@driver.on_startup
 async def on_start():
     # 启动 WebSocket 服务器
-    await start_ws_server()
-
-
-@driver.on_bot_disconnect
-async def on_close():
-    # 关闭 WebSocket 服务器
-    await stop_ws_server()
+    if isinstance(driver, ReverseDriver):
+        await set_route(driver=driver)
 
 
 # 收到消息时
 @mc_qq.handle()
 async def handle_msg(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]):
     await send_msg_to_mc(bot=bot, event=event)
```

### Comparing `nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq/data_source.py` & `nonebot-plugin-mcqq-1.2.6.post1/nonebot_plugin_mcqq/data_source.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,79 @@
-import aiomcrcon
-import websockets
-from mcqq_tool.config import Client, CLIENTS
-from mcqq_tool.utils import send_msg_to_qq, remove_client, rcon_connect
+from aiomcrcon import Client as RconClient
 from nonebot import logger, get_bot
+from nonebot.drivers import URL, ReverseDriver, WebSocketServerSetup
+from nonebot.drivers.websockets import WebSocket, WebSocketClosed
 
-from .utils import plugin_config
+from mcqq_tool.common import plugin_config
+from mcqq_tool.config import Client, CLIENTS
+from mcqq_tool.utils import send_msg_to_qq, rcon_connect, remove_client
 
 
-async def ws_client(websocket: websockets.WebSocketServerProtocol):
+async def _ws_handler(websocket: WebSocket):
     """WebSocket"""
     try:
-        server_name = websocket.request_headers["x-self-name"].encode('utf-8').decode('unicode_escape')
+        server_name = websocket.request.headers.get("x-self-name").encode('utf-8').decode('unicode_escape')
     except KeyError as e:
         # 服务器名为空
         logger.error(f"[MC_QQ]丨未获取到该服务器的名称，连接断开：{e}")
         await websocket.close(1008, "[MC_QQ]丨未获取到该服务器的名称，连接断开")
         return
     else:
 
-        if CLIENTS.get(server_name) is None:
+        if CLIENTS.get(server_name):
             # 服务器名已存在
             logger.error(f"[MC_QQ]丨已有相同服务器名的连接，连接断开")
             await websocket.close(1008, "[MC_QQ]丨已有相同服务器名的连接")
             return
 
         rcon_client = None
-        bot_id = ""
+        bot_self_id = None
         for server in plugin_config.mc_qq_server_list:
             if server_name == server.server_name:
-                bot_id = str(server.self_id)
                 if server.rcon_enable:
-                    rcon_client = aiomcrcon.Client(
-                        websocket.remote_address[0],
+                    rcon_client = RconClient(
+                        websocket.__dict__["websocket"].__dict__["scope"]["client"][0],
                         plugin_config.mc_qq_rcon_dict[server_name],
                         plugin_config.mc_qq_rcon_password
                     )
                     await rcon_connect(rcon_client=rcon_client, server_name=server_name)
+                    bot_self_id = str(server.self_id) if server.self_id else None
                     break
         CLIENTS[server_name] = Client(
             server_name=server_name,
             websocket=websocket,
             rcon=rcon_client
         )
+
+        await websocket.accept()
+
         logger.success(f"[MC_QQ]丨[Server:{server_name}] 已连接至 WebSocket 服务器")
 
         try:
-            async for message in websocket:
+            while True:
                 try:
+                    message = await websocket.receive()
                     # 获取指定ID Bot
-                    bot = get_bot(bot_id)
+                    bot = get_bot(bot_self_id)
                 except KeyError as e:
-                    logger.error(f"[MC_QQ]丨[Server:{server_name}] 的 Bot 未获取，将尝试使用其他Bot发送消息：{e}")
-                    try:
-                        # 获取可用 Bot
-                        bot = get_bot()
-                    except ValueError as e:
-                        logger.error(f"[MC_QQ]丨[Server:{server_name}] 没有可用的 Bot，无法发送消息：{e}")
-                    else:
-                        # 以可用 Bot 发送消息
-                        # 如果 Bot 未在指定群聊，则会报错
-                        await send_msg_to_qq(bot=bot, message=message)
+                    logger.warning(f"[MC_QQ]丨[Server:{server_name}] 对应 self_id 的 Bot 不存在：{e}")
+                except ValueError as e:
+                    logger.warning(f"[MC_QQ]丨[Server:{server_name}] 未指定Bot，且当前无其他Bot可用：{e}")
                 else:
                     # 以指定ID Bot 发送消息
                     await send_msg_to_qq(bot=bot, message=message)
 
-        except websockets.WebSocketException as e:
-            logger.error(f"[MC_QQ]丨[Server:{server_name}] 的 WebSocket 出现异常：{e}")
+        except WebSocketClosed as e:
+            logger.warning(f"[MC_QQ]丨[Server:{server_name}] 的 WebSocket 出现异常：{e}")
         finally:
-            if websocket.closed:
-                logger.error(f"[MC_QQ]丨[Server:{server_name}] 的 WebSocket 连接已断开")
             await remove_client(server_name=server_name)
 
 
-async def start_ws_server():
-    """启动 WebSocket 服务器"""
-    global ws
-    ws = await websockets.serve(ws_client, plugin_config.mc_qq_ws_ip, plugin_config.mc_qq_ws_port)
-    logger.success(f"[MC_QQ]丨WebSocket 服务器已在 {plugin_config.mc_qq_ws_ip}:{plugin_config.mc_qq_ws_port} 已开启")
-
-
-async def stop_ws_server():
-    """关闭 WebSocket 服务器"""
-    global ws
-    ws.close()
-    logger.success("[MC_QQ]丨WebSocket 服务器已关闭")
+async def set_route(driver: ReverseDriver):
+    driver.setup_websocket_server(
+        WebSocketServerSetup(
+            path=URL(plugin_config.mc_qq_ws_url),
+            name="mcqq",
+            handle_func=_ws_handler,
+        )
+    )
+    logger.success(f"[MC_QQ]丨WebSocket 服务器已启动，路由：{plugin_config.mc_qq_ws_url}")
```

### Comparing `nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq/utils.py` & `nonebot-plugin-mcqq-1.2.6.post1/nonebot_plugin_mcqq/utils.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from typing import Union
 from nonebot import get_driver
 from nonebot.adapters.onebot.v11 import GroupMessageEvent
 from nonebot_plugin_guild_patch import GuildMessageEvent
-from typing import Union
 
 from mcqq_tool.config import Config
 
 plugin_config: Config = Config.parse_obj(get_driver().config)
 
 rule_guild_list = []
 rule_group_list = []
```

### Comparing `nonebot-plugin-mcqq-1.2.5.post1/nonebot_plugin_mcqq.egg-info/PKG-INFO` & `nonebot-plugin-mcqq-1.2.6.post1/nonebot_plugin_mcqq.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.2.5.post1
+Version: 1.2.6.post1
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -16,23 +16,21 @@
 # NoneBot-Plugin-MCQQ
 
 基于 `NoneBot` 的与 `Minecraft Server` 互通消息插件
 
 - 支持QQ群、QQ频道
 - 支持多个服务器与多个群聊的互通
 
-推荐使用功能更为完整的 [`青岚 Bot`](https://github.com/17TheWord/qinglan_bot)
-
 # 文档
 
 - [正在不断更新的文档](https://17theword.github.io/mc_qq/)
 
 # 支持的服务端列表
 
-- Spigot
+- Spigot API
     - `MC_QQ_Spigot_XXX.jar` + `nonebot-plugin-mcqq`
 - MinecraftServer
     - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 - ForgeServer
     - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
 - Fabric
     - `MC_QQ_Minecraft_Server` + `nonebot-plugin-mcqq`
```

### Comparing `nonebot-plugin-mcqq-1.2.5.post1/setup.py` & `nonebot-plugin-mcqq-1.2.6.post1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-mcqq",
-    version="1.2.5-post1",
+    version="1.2.6-post1",
     author="17TheWord",
     author_email="17theword@gmail.com",
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通插件",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/17TheWord/nonebot-plugin-mcqq",
     packages=["nonebot_plugin_mcqq"],
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent"
     ],
     install_requires=[
-        'mcqq-tool>=0.0.5',
+        'mcqq-tool>=0.0.8',
         'nonebot2>=2.0.0',
+        'nonebot2[websockets]',
         'nonebot-adapter-onebot>=2.1.1',
         'nonebot-plugin-guild-patch>=0.2.0',
-        'websockets>=10.3',
         'aio-mc-rcon>=3.2.0'
     ]
 )
```

