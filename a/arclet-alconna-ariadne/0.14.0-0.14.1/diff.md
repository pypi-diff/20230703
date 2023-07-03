# Comparing `tmp/arclet-alconna-ariadne-0.14.0.tar.gz` & `tmp/arclet_alconna_ariadne-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-ariadne-0.14.0.tar", last modified: Fri May 26 10:13:38 2023, max compression
+gzip compressed data, was "arclet_alconna_ariadne-0.14.1.tar", last modified: Mon Jul  3 11:56:00 2023, max compression
```

## Comparing `arclet-alconna-ariadne-0.14.0.tar` & `arclet_alconna_ariadne-0.14.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ariadne-0.14.0/LICENSE
--rw-r--r--   0        0        0     6165 2023-05-26 10:11:22.219776 arclet-alconna-ariadne-0.14.0/pyproject.toml
--rw-r--r--   0        0        0     7388 2023-05-26 09:21:34.997183 arclet-alconna-ariadne-0.14.0/README.md
--rw-r--r--   0        0        0       81 2023-02-20 07:51:15.898481 arclet-alconna-ariadne-0.14.0/src/arclet/alconna/ariadne/__init__.py
--rw-r--r--   0        0        0     4725 2023-05-26 09:57:30.809955 arclet-alconna-ariadne-0.14.0/src/arclet/alconna/ariadne/adapter.py
--rw-r--r--   0        0        0     1262 2023-05-08 17:03:36.101915 arclet-alconna-ariadne-0.14.0/src/arclet/alconna/ariadne/typings.py
--rw-r--r--   0        0        0     7821 1970-01-01 00:00:00.000000 arclet-alconna-ariadne-0.14.0/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet_alconna_ariadne-0.14.1/LICENSE
+-rw-r--r--   0        0        0     7388 2023-05-26 09:21:34.997183 arclet_alconna_ariadne-0.14.1/README.md
+-rw-r--r--   0        0        0     6207 2023-07-03 11:56:00.662817 arclet_alconna_ariadne-0.14.1/pyproject.toml
+-rw-r--r--   0        0        0       81 2023-02-20 07:51:15.898481 arclet_alconna_ariadne-0.14.1/src/arclet/alconna/ariadne/__init__.py
+-rw-r--r--   0        0        0     5488 2023-06-30 17:20:01.730941 arclet_alconna_ariadne-0.14.1/src/arclet/alconna/ariadne/adapter.py
+-rw-r--r--   0        0        0     1262 2023-05-08 17:03:36.101915 arclet_alconna_ariadne-0.14.1/src/arclet/alconna/ariadne/typings.py
+-rw-r--r--   0        0        0     7922 1970-01-01 00:00:00.000000 arclet_alconna_ariadne-0.14.1/PKG-INFO
```

### Comparing `arclet-alconna-ariadne-0.14.0/LICENSE` & `arclet_alconna_ariadne-0.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ariadne-0.14.0/pyproject.toml` & `arclet_alconna_ariadne-0.14.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arclet-alconna-ariadne"
-version = "0.14.0"
+version = "0.14.1"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "graia-ariadne<1.0.0,>=0.7.14",
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
@@ -30,55 +30,59 @@
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
+    "src/arclet/alconna/ariadne",
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
@@ -107,25 +111,25 @@
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
-    "graia-ariadne<1.0.0, >=0.7.14",
+    "graia-ariadne<1.0.0,>=0.7.14",
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "alconna",
     "graia",
@@ -148,20 +152,20 @@
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
@@ -190,20 +194,20 @@
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

### Comparing `arclet-alconna-ariadne-0.14.0/README.md` & `arclet_alconna_ariadne-0.14.1/README.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ariadne-0.14.0/src/arclet/alconna/ariadne/adapter.py` & `arclet_alconna_ariadne-0.14.1/src/arclet/alconna/ariadne/adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 from typing import Any, Callable, Union
 
 from arclet.alconna.exceptions import SpecialOptionTriggered
 from graia.ariadne.app import Ariadne
 from graia.ariadne.event.message import FriendMessage, GroupMessage, MessageEvent
 from graia.ariadne.message.chain import MessageChain
 from graia.ariadne.message.element import At, Plain, Source, File, Quote
-from graia.ariadne.model import Friend, Member, Client, Stranger
+from graia.ariadne.model import Friend, Member, Client, Stranger, Group
 from graia.ariadne.util.interrupt import FunctionWaiter
 from graia.broadcast import BaseDispatcher
 from graia.broadcast.builtin.decorators import Depend
 from graia.broadcast.exceptions import ExecutionStop
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
 from graia.broadcast.interrupt import Waiter
 from graia.broadcast.utilles import run_always_await
 
 from arclet.alconna import Arparma, argv_config, set_default_argv_type
+from arclet.alconna.tools.construct import FuncMounter
+from tarina import is_awaitable
 
 from ..graia.model import CommandResult, TConvert
 from ..graia.adapter import AlconnaGraiaAdapter
 from ..graia.argv import BaseMessageChainArgv
 from ..graia.dispatcher import AlconnaDispatcher
 from ..graia.utils import listen
 
@@ -88,28 +90,44 @@
 
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
 
+    def handle_command(self, alc: FuncMounter[Any, MessageChain]) -> Callable:
+        async def wrapper(app: Ariadne, sender: Union[Group, Friend], message: MessageChain):
+            try:
+                arp, res = alc.exec(message)
+            except Exception as e:
+                await app.send_message(sender, str(e))
+                return
+            if arp.matched:
+                if is_awaitable(res):
+                    res = await res
+                if isinstance(res, (str, MessageChain)):
+                    await app.send_message(sender, res)
+        return wrapper
+
 
 class AriadneMessageChainArgv(BaseMessageChainArgv):
     ...
 
 
 set_default_argv_type(AriadneMessageChainArgv)
 argv_config(
```

### Comparing `arclet-alconna-ariadne-0.14.0/src/arclet/alconna/ariadne/typings.py` & `arclet_alconna_ariadne-0.14.1/src/arclet/alconna/ariadne/typings.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ariadne-0.14.0/PKG-INFO` & `arclet_alconna_ariadne-0.14.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-ariadne
-Version: 0.14.0
+Version: 0.14.1
 Summary: Support Alconna to GraiaProject/Ariadne
+Keywords: alconna graia arclet
+Home-page: https://github.com/ArcletProject/Alconna-Graia
+Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: AGPL-3.0
-Keywords: alconna,graia,arclet
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
+Requires-Dist: graia-ariadne<1.0.0,>=0.7.14
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

