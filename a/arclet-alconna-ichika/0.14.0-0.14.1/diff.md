# Comparing `tmp/arclet-alconna-ichika-0.14.0.tar.gz` & `tmp/arclet_alconna_ichika-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-ichika-0.14.0.tar", last modified: Fri May 26 10:13:43 2023, max compression
+gzip compressed data, was "arclet_alconna_ichika-0.14.1.tar", last modified: Mon Jul  3 11:56:04 2023, max compression
```

## Comparing `arclet-alconna-ichika-0.14.0.tar` & `arclet_alconna_ichika-0.14.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ichika-0.14.0/LICENSE
--rw-r--r--   0        0        0     6164 2023-05-26 10:11:22.219776 arclet-alconna-ichika-0.14.0/pyproject.toml
--rw-r--r--   0        0        0     7388 2023-05-26 09:21:34.997183 arclet-alconna-ichika-0.14.0/README.md
--rw-r--r--   0        0        0       80 2023-05-09 04:08:01.631055 arclet-alconna-ichika-0.14.0/src/arclet/alconna/ichika/__init__.py
--rw-r--r--   0        0        0     4735 2023-05-26 09:57:30.836953 arclet-alconna-ichika-0.14.0/src/arclet/alconna/ichika/adapter.py
--rw-r--r--   0        0        0     1256 2023-05-09 04:21:37.796354 arclet-alconna-ichika-0.14.0/src/arclet/alconna/ichika/typings.py
--rw-r--r--   0        0        0     7828 1970-01-01 00:00:00.000000 arclet-alconna-ichika-0.14.0/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet_alconna_ichika-0.14.1/LICENSE
+-rw-r--r--   0        0        0     7388 2023-05-26 09:21:34.997183 arclet_alconna_ichika-0.14.1/README.md
+-rw-r--r--   0        0        0     6206 2023-07-03 11:56:04.972662 arclet_alconna_ichika-0.14.1/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-05-09 04:08:01.631055 arclet_alconna_ichika-0.14.1/src/arclet/alconna/ichika/__init__.py
+-rw-r--r--   0        0        0     5822 2023-06-30 17:20:01.758718 arclet_alconna_ichika-0.14.1/src/arclet/alconna/ichika/adapter.py
+-rw-r--r--   0        0        0     1256 2023-05-09 04:21:37.796354 arclet_alconna_ichika-0.14.1/src/arclet/alconna/ichika/typings.py
+-rw-r--r--   0        0        0     7914 1970-01-01 00:00:00.000000 arclet_alconna_ichika-0.14.1/PKG-INFO
```

### Comparing `arclet-alconna-ichika-0.14.0/LICENSE` & `arclet_alconna_ichika-0.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ichika-0.14.0/pyproject.toml` & `arclet_alconna_ichika-0.14.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arclet-alconna-ichika"
-version = "0.14.0"
+version = "0.14.1"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "ichika>=0.0.5",
 ]
 description = "Support Alconna to BlueGlassBlock/Ichika"
@@ -31,55 +31,59 @@
 [project.urls]
 homepage = "https://github.com/ArcletProject/Alconna-Graia"
 repository = "https://github.com/ArcletProject/Alconna-Graia"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "fix-future-annotations>=0.5.0",
-    "mina-build>=0.2.6",
     "textual~=0.11.1",
     "avilla-console @ file:///${PROJECT_ROOT}/avilla_console-0.1.1-py3-none-any.whl",
 ]
 
 [tool.pdm.scripts]
 buildall = "pdm mina build -a"
 pub = "pdm publish --no-build"
 
 [tool.pdm.scripts.puball]
 composite = [
     "buildall",
     "pub",
 ]
 
+[tool.pdm.build]
+includes = [
+    "src/arclet/alconna/ichika",
+]
+
 [tool.mina]
 enabled = false
 
 [tool.mina.packages.core]
 includes = [
     "src/arclet/alconna/graia",
 ]
 
 [tool.mina.packages.core.project]
 name = "arclet-alconna-graia"
-version = "0.14.0"
+version = "0.14.1"
 description = "Support Alconna to GraiaProject"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "alconna",
     "graia",
     "arclet",
     "ariadne",
 ]
 dependencies = [
-    "arclet-alconna<2.0.0, >=1.7.7",
-    "arclet-alconna-tools<0.7.0, >=0.6.0",
+    "arclet-alconna<2.0.0, >=1.7.10",
+    "arclet-alconna-tools<0.7.0, >=0.6.3",
     "tarina>=0.3.3",
     "nepattern<0.6.0, >=0.5.8",
     "creart-graia>=0.1.5",
     "creart>=0.2.1",
     "graia-amnesia>=0.5.0",
     "graia-broadcast>=0.18.2",
     "graia-saya>=0.0.17",
@@ -108,20 +112,20 @@
 alconna_behavior = "arclet.alconna.graia.create:AlconnaBehaviorCreator"
 
 [tool.mina.packages.ariadne]
 includes = [
     "src/arclet/alconna/ariadne",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.14.0, >= 0.14.0",
+    "arclet-alconna-graia<0.15.0, >= 0.14.1",
 ]
 
 [tool.mina.packages.ariadne.project]
 name = "arclet-alconna-ariadne"
-version = "0.14.0"
+version = "0.14.1"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "graia-ariadne<1.0.0, >=0.7.14",
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
@@ -149,20 +153,20 @@
 repository = "https://github.com/ArcletProject/Alconna-Graia"
 
 [tool.mina.packages.avilla]
 includes = [
     "src/arclet/alconna/avilla",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.14.0, >= 0.14.0",
+    "arclet-alconna-graia<0.15.0, >= 0.14.1",
 ]
 
 [tool.mina.packages.avilla.project]
 name = "arclet-alconna-avilla"
-version = "0.14.0"
+version = "0.14.1"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "avilla-core>=1.0.0a5",
 ]
 description = "Support Alconna to GraiaProject/Avilla"
@@ -191,20 +195,20 @@
 repository = "https://github.com/ArcletProject/Alconna-Graia"
 
 [tool.mina.packages.ichika]
 includes = [
     "src/arclet/alconna/ichika",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.14.0, >= 0.14.0",
+    "arclet-alconna-graia<0.15.0, >= 0.14.1",
 ]
 
 [tool.mina.packages.ichika.project]
 name = "arclet-alconna-ichika"
-version = "0.14.0"
+version = "0.14.1"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "ichika>=0.0.5",
 ]
 description = "Support Alconna to BlueGlassBlock/Ichika"
```

### Comparing `arclet-alconna-ichika-0.14.0/README.md` & `arclet_alconna_ichika-0.14.1/README.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ichika-0.14.0/src/arclet/alconna/ichika/adapter.py` & `arclet_alconna_ichika-0.14.1/src/arclet/alconna/ichika/adapter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from __future__ import annotations
 
-from typing import Any, Callable, Iterable
+from typing import Any, Callable, Iterable, Union
 
 from graia.amnesia.message import MessageChain
 from graia.broadcast import BaseDispatcher
 from graia.broadcast.builtin.decorators import Depend
 from graia.broadcast.exceptions import ExecutionStop
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
 from graia.broadcast.interrupt import Waiter
 from graia.broadcast.utilles import (
     T_Dispatcher,
     dispatcher_mixin_handler,
     run_always_await,
 )
 from ichika.client import Client
-from ichika.core import Friend, Member
+from ichika.core import Friend, Member, Group
 from ichika.graia import CLIENT_INSTANCE
 from ichika.graia.event import FriendMessage, GroupMessage, MessageEvent
 from ichika.message.elements import At, Text
 
 from arclet.alconna import Arparma
 from arclet.alconna.exceptions import SpecialOptionTriggered
+from arclet.alconna.tools.construct import FuncMounter
+from tarina import is_awaitable
 
 from ..graia.model import CommandResult, TConvert
 from ..graia.adapter import AlconnaGraiaAdapter
 from ..graia.dispatcher import AlconnaDispatcher
 from ..graia.utils import listen
 
 AlconnaDispatcher.default_send_handler = lambda _, x: MessageChain([Text(x)])
@@ -111,20 +113,43 @@
 
         return Depend(__wrapper__)
 
     def handle_listen(
         self,
         func: Callable,
         buffer: dict[str, Any],
-        dispatcher: BaseDispatcher,
+        dispatcher: BaseDispatcher | None,
         guild: bool,
         private: bool,
         private_name: str,
         guild_name: str
     ) -> None:
         events = []
         if guild:
             events.append(GroupMessage)
         if private:
             events.append(FriendMessage)
-        buffer.setdefault("dispatchers", []).append(dispatcher)
+        buffer.setdefault("dispatchers", [])
+        if dispatcher:
+            buffer["dispatchers"].append(dispatcher)
         listen(*events)(func)
+
+
+    def handle_command(self, alc: FuncMounter[Any, MessageChain]) -> Callable:
+        async def wrapper(client: Client, sender: Union[Group, Friend], message: MessageChain):
+            try:
+                arp, res = alc.exec(message)
+            except Exception as e:
+                if isinstance(sender, Group):
+                    await client.send_group_message(sender, str(e))
+                else:
+                    await client.send_friend_message(sender, str(e))
+                return
+            if arp.matched:
+                if is_awaitable(res):
+                    res = await res
+                if isinstance(res, (str, MessageChain)):
+                    if isinstance(sender, Group):
+                        await client.send_group_message(sender, res)
+                    else:
+                        await client.send_friend_message(sender, res)
+        return wrapper
```

### Comparing `arclet-alconna-ichika-0.14.0/src/arclet/alconna/ichika/typings.py` & `arclet_alconna_ichika-0.14.1/src/arclet/alconna/ichika/typings.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ichika-0.14.0/PKG-INFO` & `arclet_alconna_ichika-0.14.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-ichika
-Version: 0.14.0
+Version: 0.14.1
 Summary: Support Alconna to BlueGlassBlock/Ichika
+Keywords: alconna graia arclet ichika
+Home-page: https://github.com/ArcletProject/Alconna-Graia
+Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: AGPL-3.0
-Keywords: alconna,graia,arclet,ichika
-Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
-Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Project-URL: homepage, https://github.com/ArcletProject/Alconna-Graia
-Project-URL: repository, https://github.com/ArcletProject/Alconna-Graia
+Project-URL: Homepage, https://github.com/ArcletProject/Alconna-Graia
+Project-URL: Repository, https://github.com/ArcletProject/Alconna-Graia
+Requires-Python: >=3.8
+Requires-Dist: ichika>=0.0.5
 Description-Content-Type: text/markdown
 
 # Alconna Graia
 
 该项目为 [`Alconna`](https://github.com/ArcletProject/Alconna) 为 [`GraiaProject`](https://github.com/GraiaProject) 下项目的内建支持
 
 包括解析器、Dispatcher、SayaSchema 和 附加组件
@@ -317,8 +319,8 @@
 @channel.use(ListenerSchema([...]))
 async def test2(sth: Match[str]):
     print("match", sth.available, sth.result)
 ```
 
 ## 文档
 
-[链接](https://graiax.cn/guide/alconna.html#kirakira%E2%98%86dokidoki%E7%9A%84dispatcher)
+[链接](https://graiax.cn/guide/alconna.html#kirakira%E2%98%86dokidoki%E7%9A%84dispatcher)
```

