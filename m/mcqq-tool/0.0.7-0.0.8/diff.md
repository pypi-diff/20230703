# Comparing `tmp/mcqq-tool-0.0.7.tar.gz` & `tmp/mcqq-tool-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcqq-tool-0.0.7.tar", last modified: Sun Jun 18 17:08:34 2023, max compression
+gzip compressed data, was "mcqq-tool-0.0.8.tar", last modified: Mon Jul  3 03:49:39 2023, max compression
```

## Comparing `mcqq-tool-0.0.7.tar` & `mcqq-tool-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:08:34.324747 mcqq-tool-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-18 17:08:34.324747 mcqq-tool-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:08:34.320747 mcqq-tool-0.0.7/mcqq_tool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:08:34.324747 mcqq-tool-0.0.7/mcqq_tool/model/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/model/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/model/minecraft.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/model/model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/model/spigot.py
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/mcqq_tool/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:08:34.320747 mcqq-tool-0.0.7/mcqq_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-18 17:08:34.000000 mcqq-tool-0.0.7/mcqq_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-18 17:08:34.000000 mcqq-tool-0.0.7/mcqq_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:08:34.000000 mcqq-tool-0.0.7/mcqq_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-18 17:08:34.000000 mcqq-tool-0.0.7/mcqq_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 17:08:34.000000 mcqq-tool-0.0.7/mcqq_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 17:08:34.324747 mcqq-tool-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-18 17:08:19.000000 mcqq-tool-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:49:39.384939 mcqq-tool-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-03 03:49:39.384939 mcqq-tool-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:49:39.384939 mcqq-tool-0.0.8/mcqq_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:49:39.384939 mcqq-tool-0.0.8/mcqq_tool/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/model/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/model/minecraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/model/model_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/model/spigot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/mcqq_tool/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:49:39.384939 mcqq-tool-0.0.8/mcqq_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-03 03:49:39.000000 mcqq-tool-0.0.8/mcqq_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-03 03:49:39.000000 mcqq-tool-0.0.8/mcqq_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 03:49:39.000000 mcqq-tool-0.0.8/mcqq_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-03 03:49:39.000000 mcqq-tool-0.0.8/mcqq_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 03:49:39.000000 mcqq-tool-0.0.8/mcqq_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 03:49:39.384939 mcqq-tool-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-03 03:49:28.000000 mcqq-tool-0.0.8/setup.py
```

### Comparing `mcqq-tool-0.0.7/LICENSE` & `mcqq-tool-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.7/PKG-INFO` & `mcqq-tool-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcqq-tool
-Version: 0.0.7
+Version: 0.0.8
 Summary: MC_QQ 工具包
 Home-page: https://github.com/17TheWord/mcqq-tool
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mcqq-tool-0.0.7/mcqq_tool/common.py` & `mcqq-tool-0.0.8/mcqq_tool/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,37 +28,37 @@
     return bool(roles & set(plugin_config.mc_qq_guild_admin_roles))
 
 
 GUILD_ADMIN: Permission = Permission(_guild_admin)
 """频道管理员权限"""
 
 
-async def msg_to_qq_process(event: BaseEvent) -> str:
+async def _msg_to_qq_process(event: BaseEvent) -> str:
     """处理来自MC的消息，并返回处理后的消息"""
     if isinstance(event, BaseChatEvent):
         return f"{event.player.nickname} 说：{event.message}"
     elif isinstance(event, BaseDeathEvent):
         return f"{event.player.nickname} {event.death_message}"
     elif isinstance(event, BaseJoinEvent):
         return f"{event.player.nickname} 加入了游戏"
     elif isinstance(event, BaseQuitEvent):
         return f"{event.player.nickname} 离开了游戏"
     else:
         return "未知消息"
 
 
-async def send_msg_to_qq_common(
+async def _send_msg_to_qq_common(
         bot: Bot,
         message: str,
 ):
     """发送消息到 QQ"""
     json_msg = json.loads(message)
     event = event_dict[json_msg["event_name"]].parse_obj(json_msg)
 
-    msg = await msg_to_qq_process(event)
+    msg = await _msg_to_qq_process(event)
     if plugin_config.mc_qq_display_server_name:
         msg = f"[{event.server_name}] {msg}"
     # 循环服务器列表并发送消息
     if plugin_config.mc_qq_server_list:
         for per_server in plugin_config.mc_qq_server_list:
             # 判断服务器名称是否相同
             if per_server.server_name == event.server_name:
```

### Comparing `mcqq-tool-0.0.7/mcqq_tool/config.py` & `mcqq-tool-0.0.8/mcqq_tool/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import aiomcrcon
-import websockets
+from aiomcrcon import Client as RconClient
+from nonebot.drivers.websockets import WebSocket
 from typing import Optional, List, Dict
 from pydantic import BaseModel, Extra, Field
 
 
 class Client:
     """MC_QQ 客户端"""
     server_name: str
-    websocket: websockets.WebSocketServerProtocol
-    rcon: Optional[aiomcrcon.Client] = None
+    websocket: WebSocket
+    rcon: Optional[RconClient] = None
 
     def __init__(
             self, server_name: str,
-            websocket: websockets.WebSocketServerProtocol,
-            rcon: Optional[aiomcrcon.Client] = None
+            websocket: WebSocket,
+            rcon: Optional[RconClient] = None
     ):
         self.server_name: str = server_name
-        self.websocket: websockets.WebSocketServerProtocol = websocket
-        self.rcon: Optional[aiomcrcon.Client] = rcon
+        self.websocket: WebSocket = websocket
+        self.rcon: Optional[RconClient] = rcon
 
 
 CLIENTS: Dict[str, Client] = {}
 
 
 class Guild(BaseModel):
     """频道配置"""
@@ -43,18 +43,16 @@
     rcon_enable: Optional[bool] = False
     # 该群Bot ID
     self_id: Optional[int] = None
 
 
 class Config(BaseModel, extra=Extra.ignore):
     """配置"""
-    # 服务器地址
-    mc_qq_ws_ip: Optional[str] = "127.0.0.1"
-    # 服务器端口
-    mc_qq_ws_port: Optional[int] = 8765
+    # 路由地址
+    mc_qq_ws_url: Optional[str] = "/onebot/v11/mcqq"
     # 是否发送群聊名称
     mc_qq_send_group_name: Optional[bool] = False
     # 是否显示服务器名称
     mc_qq_display_server_name: Optional[bool] = False
     # 服务器列表
     mc_qq_server_list: Optional[List[Server]] = Field(default_factory=list)
     # MCRcon 密码
```

### Comparing `mcqq-tool-0.0.7/mcqq_tool/model/__init__.py` & `mcqq-tool-0.0.8/mcqq_tool/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.7/mcqq_tool/model/basemodel.py` & `mcqq-tool-0.0.8/mcqq_tool/model/basemodel.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.7/mcqq_tool/model/minecraft.py` & `mcqq-tool-0.0.8/mcqq_tool/model/minecraft.py`

 * *Files identical despite different names*

### Comparing `mcqq-tool-0.0.7/mcqq_tool/model/spigot.py` & `mcqq-tool-0.0.8/mcqq_tool/model/spigot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 from typing import Optional
-from pydantic import BaseModel
 from .basemodel import BasePlayer, BaseChatEvent, BaseDeathEvent, BaseJoinEvent, BaseQuitEvent
 
 
-class Address(BaseModel):
-    address: str
-    port: int
-
-
 class SpigotPlayer(BasePlayer):
     """玩家信息"""
     uuid: str
     display_name: str
     player_list_name: str
     is_health_scaled: bool
-    address: Address
+    address: Optional[str] = None
     is_sprinting: bool
     walk_speed: float
     fly_speed: float
     is_sneaking: bool
     level: int
     is_flying: bool
     ping: Optional[int] = None
```

### Comparing `mcqq-tool-0.0.7/mcqq_tool/utils.py` & `mcqq-tool-0.0.8/mcqq_tool/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,189 +1,179 @@
 import json
-from typing import List, Union, Optional, Tuple
+import contextlib
+from typing import List, Union, Tuple
 
-import aiomcrcon
-import websockets
+from aiomcrcon import (
+    Client as RconClient,
+    ClientNotConnectedError,
+    RCONConnectionError,
+    IncorrectPasswordError
+)
 from nonebot import logger
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent
+from nonebot.drivers.websockets import WebSocketClosed
 from nonebot_plugin_guild_patch import GuildMessageEvent
 
-from .common import get_member_nickname, send_msg_to_qq_common, plugin_config
+from .common import get_member_nickname, _send_msg_to_qq_common, plugin_config
 from .config import Client, CLIENTS
 
 
 async def send_msg_to_mc(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]):
     """
     发送消息到 MC
     :param bot: Bot
     :param event: 事件
     """
     # 处理来自QQ的消息
-    if client_list := await get_clients(event=event):
+    if client_list := await _get_clients(event=event):
         for client in client_list:
             if client:
                 # 先判断是否有Rcon进行发送
                 if client.rcon:
-                    rcon_text_msg, msgCmd = await msg_process_to_cmd(bot=bot, event=event)
+                    rcon_text_msg, msg_cmd = await _msg_process_to_cmd(bot=bot, event=event)
                     try:
-                        await client.rcon.send_cmd(msgCmd)
-                    except aiomcrcon.errors.ClientNotConnectedError as e:
+                        await client.rcon.send_cmd(msg_cmd)
+                        logger.success(f"[MC_QQ_Rcon]丨发送至 [server:{client.server_name}] 的消息 \"{rcon_text_msg}\"")
+                    except ClientNotConnectedError as e:
                         logger.error(f"[MC_QQ_Rcon]丨发送至 [Server:{client.server_name}] 的过程中出现了错误：{e}")
                         await remove_client(client.server_name)
-                    else:
-                        logger.success(f"[MC_QQ_Rcon]丨发送至 [server:{client.server_name}] 的消息 \"{rcon_text_msg}\"")
                 elif client.websocket:
-                    text_msg, msgJson = await msg_process_to_json(bot=bot, event=event)
+                    text_msg, msg_json = await _msg_process_to_json(bot=bot, event=event)
                     try:
-                        await client.websocket.send(msgJson)
-                    except websockets.WebSocketException as e:
+                        await client.websocket.send(msg_json)
+                        logger.success(f"[MC_QQ]丨发送至 [server:{client.server_name}] 的消息 \"{text_msg}\"")
+                    except WebSocketClosed as e:
                         logger.error(f"[MC_QQ]丨发送至 [Server:{client.server_name}] 的过程中出现了错误：{e}")
                         await remove_client(client.server_name)
-                    else:
-                        logger.success(f"[MC_QQ]丨发送至 [server:{client.server_name}] 的消息 \"{text_msg}\"")
                 else:
-                    logger.error(f"[MC_QQ]丨发送至 [Server:{client.server_name}] 的过程中出现了错误：该客户端没有连接")
+                    logger.error(f"[MC_QQ]丨发送至 [Server:{client.server_name}] 的过程中出现了错误：该服务器没有连接")
                     await remove_client(client.server_name)
 
 
 async def send_cmd_to_mc(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent], cmd: str):
     """
     发送命令到 MC
     :param bot: Bot
     :param event: 事件
     :param cmd: 命令
     """
     # 处理来自QQ的消息
-    if client_list := await get_clients(event=event):
+    if client_list := await _get_clients(event=event):
         for client in client_list:
             if client:
                 # 先判断是否有Rcon进行发送
                 if client.rcon:
                     try:
                         back_msg = await client.rcon.send_cmd(cmd)
                         await bot.send(event=event, message=f"服务器返回：{back_msg[0]}")
-                    except aiomcrcon.errors.ClientNotConnectedError as e:
+                        logger.success(f"[MC_QQ_Rcon]丨发送至 [server:{client.server_name}] 的消息 \"{cmd}\"")
+                    except ClientNotConnectedError as e:
                         logger.error(f"[MC_QQ_Rcon]丨发送至 [Server:{client.server_name}] 的过程中出现了错误：{e}")
                         await remove_client(client.server_name)
-                    else:
-                        logger.success(f"[MC_QQ_Rcon]丨发送至 [server:{client.server_name}] 的消息 \"{cmd}\"")
                 elif client.websocket:
                     await bot.send(event=event, message="该服务器不支持Rcon，无法执行该命令")
                 else:
                     logger.error(f"[MC_QQ]丨发送至 [Server:{client.server_name}] 的过程中出现了错误：该客户端没有连接")
                     await remove_client(client.server_name)
 
 
-async def get_clients(event: Union[GroupMessageEvent, GuildMessageEvent]) -> List[Client]:
+async def _get_clients(event: Union[GroupMessageEvent, GuildMessageEvent]) -> List[Client]:
     """
     获取 服务器名、ws客户端, 返回client列表
     :param event: 事件
     :return: client列表
     """
     res: List[Client] = []
     for per_server in plugin_config.mc_qq_server_list:
         if isinstance(event, GroupMessageEvent):
             if event.group_id in per_server.group_list:
-                res.append(get_client(per_server.server_name))
+                res.append(CLIENTS.get(per_server.server_name))
         if isinstance(event, GuildMessageEvent):
             for per_guild in per_server.guild_list:
                 if per_guild.guild_id == event.guild_id and per_guild.channel_id == event.channel_id:
-                    res.append(get_client(per_server.server_name))
+                    res.append(CLIENTS.get(per_server.server_name))
     return res
 
 
-def get_client(server_name: str) -> Optional[Client]:
-    """
-    获取客户端
-    :param server_name: 服务器名
-    :return: 客户端
-    """
-    try:
-        return CLIENTS[server_name]
-    except KeyError as e:
-        logger.error(f"[MC_QQ_Rcon]丨获取客户端时出现了错误，该客户端不在列表中：{e}")
-        return None
-
-
 async def remove_client(server_name: str):
     """
     移除客户端
     :param server_name: 服务器名
     """
-    if client := get_client(server_name):
+    if client := CLIENTS.get(server_name):
         if client.websocket:
-            await client.websocket.close()
+            with contextlib.suppress(Exception):
+                await client.websocket.close()
         if client.rcon:
             await client.rcon.close()
         del CLIENTS[server_name]
 
 
-async def rcon_connect(rcon_client: aiomcrcon.Client, server_name: str):
+async def rcon_connect(rcon_client: RconClient, server_name: str):
     """
     连接 Rcon
     :param rcon_client: Rcon 客户端
     :param server_name: 服务器名
     """
     try:
         await rcon_client.connect()
-    except aiomcrcon.RCONConnectionError as e:
+        logger.success(f"[MC_QQ]丨[Server:{server_name}] 的Rcon连接成功")
+    except RCONConnectionError as e:
         logger.error(f"[MC_QQ]丨[Server:{server_name}] 的Rcon连接失败：{str(e)}")
-    except aiomcrcon.IncorrectPasswordError as e:
+    except IncorrectPasswordError as e:
         logger.error(f"[MC_QQ]丨[Server:{server_name}] 的Rcon密码错误：{str(e)}")
-    else:
-        logger.success(f"[MC_QQ]丨[Server:{server_name}] 的Rcon连接成功")
 
 
 async def send_msg_to_qq(
         bot: Bot,
         message: str
 ):
     """
     发送消息到 QQ
     :param bot: Bot
     :param message: 消息
     """
-    await send_msg_to_qq_common(
+    await _send_msg_to_qq_common(
         bot=bot,
         message=message
     )
 
 
-async def msg_process_to_json(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]) -> Tuple[str, str]:
+async def _msg_process_to_json(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]) -> Tuple[str, str]:
     """
     消息处理为 JSON
     :param bot: Bot
     :param event: 事件
     :return: text_msg, msgJson
     """
     # 获取昵称
     member_nickname = await get_member_nickname(bot, event, event.user_id)
 
     # 初始化消息
     text_msg = member_nickname + "说："
 
     # 初始化消息字典
-    messageList = []
+    message_list = []
 
     # 发送群聊名称
     if plugin_config.mc_qq_send_group_name:
         group_name = {'msgType': "group_name"}
         if isinstance(event, GroupMessageEvent):
             group_name['msgData'] = (await bot.get_group_info(group_id=event.group_id))['group_name']
         elif isinstance(event, GuildMessageEvent):
             guild_name = (await bot.get_guild_meta_by_guest(guild_id=event.guild_id))['guild_name']
             for per_channel in (await bot.get_guild_channel_list(guild_id=event.guild_id, no_cache=True)):
                 if str(event.channel_id) == per_channel['channel_id']:
                     channel_name = per_channel['channel_name']
                     group_name['msgData'] = f"{guild_name}丨{channel_name}"
                     break
-        messageList.append({"msgType": "group_name", "msgData": group_name})
+        message_list.append({"msgType": "group_name", "msgData": group_name})
 
     # 将群成员昵称装入消息列表
-    messageList.append({"msgType": "senderName", "msgData": member_nickname})
+    message_list.append({"msgType": "senderName", "msgData": member_nickname})
 
     for msg in event.message:
         per_msg = {'msgType': msg.type}
         # 文本
         if msg.type == "text":
             msgData = msg.data['text'].replace("\r", "").replace("\n", "\n * ")
             text_msg += msgData
@@ -224,20 +214,20 @@
             text_msg += '[' + msg.type + '] '
 
         text_msg += " "
 
         # 装入消息数据
         per_msg['msgData'] = msgData
         # 放入消息列表
-        messageList.append(per_msg)
+        message_list.append(per_msg)
 
-    return text_msg, str({"message": messageList})
+    return text_msg, str({"message": message_list})
 
 
-async def msg_process_to_cmd(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]) -> Tuple[str, str]:
+async def _msg_process_to_cmd(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]) -> Tuple[str, str]:
     """
     消息处理为 命令
     :param bot: Bot
     :param event: 事件
     :return: text_msg, command_msg
     """
     # 获取昵称
@@ -255,15 +245,16 @@
         if isinstance(event, GroupMessageEvent):
             message_list.append(
                 {"text": (await bot.get_group_info(group_id=event.group_id))['group_name'] + " ", "color": "aqua"})
         elif isinstance(event, GuildMessageEvent):
             guild_name = (await bot.get_guild_meta_by_guest(guild_id=event.guild_id))['guild_name']
             for per_channel in (await bot.get_guild_channel_list(guild_id=event.guild_id, no_cache=True)):
                 if str(event.channel_id) == per_channel['channel_id']:
-                    message_list.append({"text": guild_name + "丨" + per_channel['channel_name'] + " ", "color": "aqua"})
+                    message_list.append(
+                        {"text": guild_name + "丨" + per_channel['channel_name'] + " ", "color": "aqua"})
                     break
     message_list.append({"text": member_nickname, "color": "aqua"})
     message_list.append({"text": " 说：", "color": "yellow"})
 
     for msg in event.message:
         # 文本
         if msg.type == "text":
@@ -284,15 +275,16 @@
         elif msg.type == "record":
             msg_dict = {"text": "[语音] ", "color": "light_purple"}
             text_msg += '[语音]'
         # 视频
         elif msg.type == "video":
             msg_dict = {"text": "[视频] ", "color": "light_purple",
                         "clickEvent": {"action": "open_url", "value": msg.data['url']},
-                        "hoverEvent": {"action": "show_text", "contents": [{"text": "查看视频", "color": "dark_purple"}]}
+                        "hoverEvent": {"action": "show_text",
+                                       "contents": [{"text": "查看视频", "color": "dark_purple"}]}
                         }
             text_msg += '[视频]'
         # @
         elif msg.type == "at":
             # 获取被@ 群/频道 昵称
             at_member_nickname = await get_member_nickname(bot, event, msg.data['qq'])
             msg_dict = {"text": "@" + at_member_nickname + " ", "color": "green"}
```

### Comparing `mcqq-tool-0.0.7/mcqq_tool.egg-info/PKG-INFO` & `mcqq-tool-0.0.8/mcqq_tool.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcqq-tool
-Version: 0.0.7
+Version: 0.0.8
 Summary: MC_QQ 工具包
 Home-page: https://github.com/17TheWord/mcqq-tool
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

