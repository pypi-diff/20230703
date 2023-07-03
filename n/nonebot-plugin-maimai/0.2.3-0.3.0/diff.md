# Comparing `tmp/nonebot_plugin_maimai-0.2.3.tar.gz` & `tmp/nonebot_plugin_maimai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_maimai-0.2.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_maimai-0.3.0.tar", max compression
```

## Comparing `nonebot_plugin_maimai-0.2.3.tar` & `nonebot_plugin_maimai-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-06-24 14:36:40.711175 nonebot_plugin_maimai-0.2.3/LICENSE
--rw-r--r--   0        0        0     3492 2023-06-24 14:36:40.711175 nonebot_plugin_maimai-0.2.3/README.md
--rw-r--r--   0        0        0    15374 2023-06-24 14:36:40.711175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/__init__.py
--rw-r--r--   0        0        0        0 2023-06-24 14:36:40.711175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/__init__.py
--rw-r--r--   0        0        0     1556 2023-06-24 14:36:40.711175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/image.py
--rw-r--r--   0        0        0    17432 2023-06-24 14:36:40.711175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/maimai_best_40.py
--rw-r--r--   0        0        0    17520 2023-06-24 14:36:40.715175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/maimai_best_50.py
--rw-r--r--   0        0        0     5353 2023-06-24 14:36:40.715175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/maimaidx_music.py
--rw-r--r--   0        0        0      385 2023-06-24 14:36:40.715175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/tool.py
--rw-r--r--   0        0        0     7312 2023-06-24 14:36:40.715175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/public.py
--rw-r--r--   0        0        0     1098 2023-06-24 14:36:40.715175 nonebot_plugin_maimai-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4587 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-03 16:15:36.011619 nonebot_plugin_maimai-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3693 2023-07-03 16:15:36.011619 nonebot_plugin_maimai-0.3.0/README.md
+-rw-r--r--   0        0        0    15337 2023-07-03 16:15:36.011619 nonebot_plugin_maimai-0.3.0/nonebot_plugin_maimai/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 16:15:36.011619 nonebot_plugin_maimai-0.3.0/nonebot_plugin_maimai/libraries/__init__.py
+-rw-r--r--   0        0        0     1556 2023-07-03 16:15:36.011619 nonebot_plugin_maimai-0.3.0/nonebot_plugin_maimai/libraries/image.py
+-rw-r--r--   0        0        0    17432 2023-07-03 16:15:36.011619 nonebot_plugin_maimai-0.3.0/nonebot_plugin_maimai/libraries/maimai_best_40.py
+-rw-r--r--   0        0        0    17520 2023-07-03 16:15:36.011619 nonebot_plugin_maimai-0.3.0/nonebot_plugin_maimai/libraries/maimai_best_50.py
+-rw-r--r--   0        0        0     5353 2023-07-03 16:15:36.011619 nonebot_plugin_maimai-0.3.0/nonebot_plugin_maimai/libraries/maimaidx_music.py
+-rw-r--r--   0        0        0      385 2023-07-03 16:15:36.011619 nonebot_plugin_maimai-0.3.0/nonebot_plugin_maimai/libraries/tool.py
+-rw-r--r--   0        0        0     7807 2023-07-03 16:15:36.011619 nonebot_plugin_maimai-0.3.0/nonebot_plugin_maimai/public.py
+-rw-r--r--   0        0        0     1059 2023-07-03 16:15:36.011619 nonebot_plugin_maimai-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4726 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_maimai-0.2.3/LICENSE` & `nonebot_plugin_maimai-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.2.3/README.md` & `nonebot_plugin_maimai-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,30 +14,34 @@
 </a>
 <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai/issues">
         <img alt="GitHub issues" src="https://img.shields.io/github/issues/Umamusume-Agnes-Digital/nonebot_plugin_maimai" alt="issues">
 </a>
 <a href="https://jq.qq.com/?_wv=1027&k=l82tMuPG">
         <img src="https://img.shields.io/badge/QQ%E7%BE%A4-424506063-orange?style=flat-square" alt="QQ Chat Group">
 </a>
-    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
 </div>
 
 ## 说明（已更新舞萌国服2023，重新下载资源）
 
 从[mai-bot](https://github.com/Diving-Fish/mai-bot)适配nonebot2插件，测试环境nonebot2.0.0
 
 修改部分：
  - b40/b50可以艾特人查询
  - static文件可以放maimai插件文件夹中，或机器人路径下/data/maimai/static
  - （可循）env设置 `maimai_font`,是str对象的`字体`
- - 新增指令`b站搜索[text]`
+ - 新增指令`搜手元`,`搜理论`,`搜谱面确认`，后面带上搜索的对象
 
 我做的适配有问题请冲我来不要打扰原作者捏，可以提iss或者[加群qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)反馈,
 
+## env(可选)
+
+        maimai_font = 'simsun.ttc'  # 替换你有的字体
+
 ## 前置步骤（和原项目一样）
 
 安装（仍选其一）:
 
     pip3 install nonebot_plugin_maimai
     nb plugin install nonebot_plugin_maimai
     git clone https://github.com/Agnes4m/nonebot_plugin_maimai.git
@@ -67,14 +71,15 @@
 今日舞萌 | 查看今天的舞萌运势
 XXXmaimaiXXX什么 | 随机一首歌
 随个[dx/标准][绿黄红紫白]<难度> | 随机一首指定条件的乐曲
 查歌<乐曲标题的一部分> | 查询符合条件的乐曲
 [绿黄红紫白]id<歌曲编号> | 查询乐曲信息或谱面信息
 定数查歌 <定数> <br> 定数查歌 <定数下限> <定数上限> |  查询定数对应的乐曲
 分数线 <难度+歌曲id> <分数线> | 展示歌曲的分数线
+搜<手元><理论><谱面确认> | 从b站获取对应的手元视频
 
 ## 原作者
 
 [Diving-Fish](https://github.com/Diving-Fish),感谢大佬为音游人的无私奉献
 
 ## License
```

#### html2text {}

```diff
@@ -4,17 +4,18 @@
               [GitHub_issues] [QQ_Chat_Group] [python] [NoneBot]
 ## è¯´æï¼å·²æ´æ°èèå½æ2023ï¼éæ°ä¸è½½èµæºï¼ ä»[mai-bot]
 (https://github.com/Diving-Fish/mai-
 bot)éénonebot2æä»¶ï¼æµè¯ç¯å¢nonebot2.0.0 ä¿®æ¹é¨åï¼ - b40/
 b50å¯ä»¥è¾ç¹äººæ¥è¯¢ -
 staticæä»¶å¯ä»¥æ¾maimaiæä»¶æä»¶å¤¹ä¸­ï¼ææºå¨äººè·¯å¾ä¸/data/
 maimai/static - ï¼å¯å¾ªï¼envè®¾ç½® `maimai_font`,æ¯strå¯¹è±¡ç`å­ä½` -
-æ°å¢æä»¤`bç«æç´¢[text]`
+æ°å¢æä»¤`ææå`,`æçè®º`,`æè°±é¢ç¡®è®¤`ï¼åé¢å¸¦ä¸æç´¢çå¯¹è±¡
 æåçééæé®é¢è¯·å²ææ¥ä¸è¦ææ°åä½èæï¼å¯ä»¥æissæè
-[å ç¾¤qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦, ##
+[å ç¾¤qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦, ## env(å¯é)
+maimai_font = 'simsun.ttc' # æ¿æ¢ä½ æçå­ä½ ##
 åç½®æ­¥éª¤ï¼ååé¡¹ç®ä¸æ ·ï¼ å®è£ï¼ä»éå¶ä¸ï¼: pip3 install
 nonebot_plugin_maimai nb plugin install nonebot_plugin_maimai git clone https:/
 /github.com/Agnes4m/nonebot_plugin_maimai.git æ¨éè¦ä»[æ­¤é¾æ¥](https://
 www.diving-fish.com/maibot/
 static.zip)ä¸è½½èµæºæä»¶å¹¶ï¼å¹¶å°å¶staticæä»¶è§£åå°:
 (ä»¥ä¸æ¹æ³2é1) - pypi`nonebot_plugin_maimai`æä»¶å¤¹ä¸­ -
 æç»è·¯å¾ç±»ä¼¼æ¯/path/to/nonebot_plugin_maimai/static - æºå¨äººç®å½ä¸
@@ -28,12 +29,13 @@
 ## è¯´æ æ¬ bot æä¾äºå¦ä¸åè½ï¼ å½ä»¤ | åè½ --- | --- help |
 æ¥çå¸®å©ææ¡£ ä»æ¥èè | æ¥çä»å¤©çèèè¿å¿
 XXXmaimaiXXXä»ä¹ | éæºä¸é¦æ­ éä¸ª[dx/æ å][ç»¿é»çº¢ç´«ç½]<é¾åº¦>
 | éæºä¸é¦æå®æ¡ä»¶çä¹æ² æ¥æ­<ä¹æ²æ é¢çä¸é¨å> |
 æ¥è¯¢ç¬¦åæ¡ä»¶çä¹æ² [ç»¿é»çº¢ç´«ç½]id<æ­æ²ç¼å·> |
 æ¥è¯¢ä¹æ²ä¿¡æ¯æè°±é¢ä¿¡æ¯ å®æ°æ¥æ­ <å®æ°>
 å®æ°æ¥æ­ <å®æ°ä¸é> <å®æ°ä¸é> | æ¥è¯¢å®æ°å¯¹åºçä¹æ²
-åæ°çº¿ <é¾åº¦+æ­æ²id> <åæ°çº¿> | å±ç¤ºæ­æ²çåæ°çº¿ ## åä½è
-[Diving-Fish](https://github.com/Diving-
+åæ°çº¿ <é¾åº¦+æ­æ²id> <åæ°çº¿> | å±ç¤ºæ­æ²çåæ°çº¿
+æ<æå><çè®º><è°±é¢ç¡®è®¤> | ä»bç«è·åå¯¹åºçæåè§é¢ ##
+åä½è [Diving-Fish](https://github.com/Diving-
 Fish),æè°¢å¤§ä½¬ä¸ºé³æ¸¸äººçæ ç§å¥ç® ## License MIT
 æ¨å¯ä»¥èªç±ä½¿ç¨æ¬é¡¹ç®çä»£ç ç¨äºåä¸æéåä¸çç¨éï¼ä½å¿é¡»éå¸¦
 MIT ææåè®®ã
```

### Comparing `nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/__init__.py` & `nonebot_plugin_maimai-0.3.0/nonebot_plugin_maimai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from nonebot import require
-require('nonebot_plugin_htmlrender')
 require('nonebot_plugin_txt2img')
 from nonebot import on_command, on_regex,get_driver
 from nonebot.params import CommandArg, EventMessage
 from nonebot.adapters import Event
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 from nonebot.plugin import PluginMetadata
 
@@ -57,15 +56,15 @@
     ...... .^...,.=O=@...OO@\      ,[O\=.    ./`.*.*OOOOO..OOO*..OO.,OOO
     ....../O....../^=O@`..O@@@@@]`    .* .,/@@/..../OOOOO*.,OOO..,OO`=OO
     @OO\ooO....,*/@^,@@@\..@^[\@@@@@@O]*]//[`@^*^*=OOOOOO^..=OO\...\^.\@
     OOooo^..`./oOO@/ =^\/^.^\\....=]......,/@@^O^*O.... .,][],OO\....\`.
     @Oooo\/]OOOOOO/  .  \.=^....,..........[.,OO^=^.    /    ,`\OO`.....
     """
 
-__version__ = "0.2.3"
+__version__ = "0.3.0"
 __plugin_meta__ = PluginMetadata(
     name="舞萌maimai",
     description='指令：舞萌帮助',
     usage=logo,
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_maimai",
     supported_adapters={"~onebot.v11"},
```

### Comparing `nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/image.py` & `nonebot_plugin_maimai-0.3.0/nonebot_plugin_maimai/libraries/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/maimai_best_40.py` & `nonebot_plugin_maimai-0.3.0/nonebot_plugin_maimai/libraries/maimai_best_40.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/maimai_best_50.py` & `nonebot_plugin_maimai-0.3.0/nonebot_plugin_maimai/libraries/maimai_best_50.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/maimaidx_music.py` & `nonebot_plugin_maimai-0.3.0/nonebot_plugin_maimai/libraries/maimaidx_music.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/public.py` & `nonebot_plugin_maimai-0.3.0/nonebot_plugin_maimai/public.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from nonebot import on_command, on_notice
 from nonebot.typing import T_State
 from nonebot.adapters.onebot.v11 import Message, Event, Bot, MessageSegment
 from nonebot.exception import IgnoredException
 from nonebot.message import event_preprocessor
 from nonebot_plugin_txt2img import Txt2Img
+from nonebot.log import logger
 from nonebot import get_driver
-from nonebot.params import CommandArg
+from nonebot.params import CommandArg,RawCommand
 from nonebot.matcher import Matcher
 from .libraries.image import *
 
 from bs4 import BeautifulSoup
 from typing import Dict,List
 import aiohttp
 from io import BytesIO
 import json
+import random
 
 try:
     maimai_font: str = get_driver().config.maimai_font
 except:
     maimai_font: str = 'simsun.ttc'
 try:
     b_cookie: str = get_driver().config.b_cookie
@@ -57,34 +59,45 @@
     try:
         await help.send(MessageSegment.image(pic))
     except:
         await help.send(help_str)
 
 
 
-search = on_command('search',aliases={'b站搜索','mai搜索'})
+search = on_command('搜手元',aliases={'搜理论','搜谱面确认'})
 @search.handle()
-async def _(state: T_State,matcher:Matcher ,arg:Message = CommandArg()):
+async def _(state: T_State,matcher:Matcher ,command: str = RawCommand(),arg:Message = CommandArg()):
+    keyword = command.replace('搜','')
     msg = arg.extract_plain_text()
-    data_list:List[Dict[str,Dict[str,str]]] = await get_target(msg)
+    if not msg:
+        await matcher.finish('请把要搜索的内容放在后面哦')
+    data_list:List[Dict[str,Dict[str,str]]] = await get_target(keyword+msg)
     state['msg'] = data_list
-    result_img = await data_to_img(data_list)
-    img = BytesIO()
-    result_img.save(img,format="png")
-    img_bytes = img.getvalue()
-    await matcher.send(MessageSegment.image(img_bytes))
-
-@search.got("tap",prompt="请输入需要的序号")
-async def _(state: T_State,matcher:Matcher ):
-    tag:Message = state['tap']
-    tag = tag.extract_plain_text()
-    if tag.isdigit() and int(tag) in range(1, 10):
-        msg:List[Dict[str,Dict[str,str]]] = state['msg']
-        Url = msg[int(tag)-1]['url']['视频链接:']
-        print(msg[int(tag)-1])
+    
+    choice_dict = random.randint(1,len(data_list))
+#     result_img = await data_to_img(data_list)
+#     img = BytesIO()
+#     result_img.save(img,format="png")
+#     img_bytes = img.getvalue()
+#     await matcher.send(MessageSegment.image(img_bytes))
+
+# @search.got("tap",prompt="请输入需要的序号")
+# async def _(state: T_State,matcher:Matcher ):
+    # tags:Message = state['tap']
+    # tag = tags.extract_plain_text()
+    # if tag.isdigit() and int(tag) in range(1, 10):
+    
+        # msg:List[Dict[str,Dict[str,str]]] = state['msg']
+    Url = msg[int(choice_dict)-1]['url']['视频链接:']
+    title = msg[int(choice_dict)-1]['data']['视频标题:']
+    await matcher.send(title)
+    try:
+        await matcher.finish(MessageSegment.video(Url))
+    except Exception as E:
+        logger.warning(E)
         await matcher.finish(Url)
     
 async def fetch_page(url, headers):
     async with aiohttp.ClientSession(headers=headers) as session:
         async with session.get(url) as response:
             return await response.text()
```

### Comparing `nonebot_plugin_maimai-0.2.3/pyproject.toml` & `nonebot_plugin_maimai-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_maimai"
-version = "0.2.3"
+version = "0.3.0"
 description= "Maimai DX plugin for NoneBot"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_maimai"
 repository = "https://github.com/Agnes4m/nonebot_plugin_maimai"
 keywords = ["maimai", "nonebot2", "plugin"]
@@ -23,15 +23,14 @@
 ]
  
 [tool.poetry.dependencies]
 python = "^3.9"
 aiohttp = "^3.8.3"
 nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = ">=2.1.3"
-nonebot_plugin_htmlrender = "^0.2.0.3"
 pillow = ">=9.3.0"
 httpx = ">=0.22.0"
 nonebot-plugin-txt2img = "^0.3.0"
 bs4 = "^0.0.1"
  
 [tool.poetry.dev-dependencies]
```

### Comparing `nonebot_plugin_maimai-0.2.3/PKG-INFO` & `nonebot_plugin_maimai-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-maimai
-Version: 0.2.3
+Version: 0.3.0
 Summary: Maimai DX plugin for NoneBot
 Home-page: https://github.com/Agnes4m/nonebot_plugin_maimai
 License: MIT
 Keywords: maimai,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: httpx (>=0.22.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.3)
 Requires-Dist: nonebot-plugin-txt2img (>=0.3.0,<0.4.0)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
-Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.3,<0.3.0.0)
 Requires-Dist: pillow (>=9.3.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_maimai
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180" alt="NoneBotPluginLogo">
   <br>
@@ -42,30 +41,34 @@
 </a>
 <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_maimai/issues">
         <img alt="GitHub issues" src="https://img.shields.io/github/issues/Umamusume-Agnes-Digital/nonebot_plugin_maimai" alt="issues">
 </a>
 <a href="https://jq.qq.com/?_wv=1027&k=l82tMuPG">
         <img src="https://img.shields.io/badge/QQ%E7%BE%A4-424506063-orange?style=flat-square" alt="QQ Chat Group">
 </a>
-    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
 </div>
 
 ## 说明（已更新舞萌国服2023，重新下载资源）
 
 从[mai-bot](https://github.com/Diving-Fish/mai-bot)适配nonebot2插件，测试环境nonebot2.0.0
 
 修改部分：
  - b40/b50可以艾特人查询
  - static文件可以放maimai插件文件夹中，或机器人路径下/data/maimai/static
  - （可循）env设置 `maimai_font`,是str对象的`字体`
- - 新增指令`b站搜索[text]`
+ - 新增指令`搜手元`,`搜理论`,`搜谱面确认`，后面带上搜索的对象
 
 我做的适配有问题请冲我来不要打扰原作者捏，可以提iss或者[加群qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)反馈,
 
+## env(可选)
+
+        maimai_font = 'simsun.ttc'  # 替换你有的字体
+
 ## 前置步骤（和原项目一样）
 
 安装（仍选其一）:
 
     pip3 install nonebot_plugin_maimai
     nb plugin install nonebot_plugin_maimai
     git clone https://github.com/Agnes4m/nonebot_plugin_maimai.git
@@ -95,14 +98,15 @@
 今日舞萌 | 查看今天的舞萌运势
 XXXmaimaiXXX什么 | 随机一首歌
 随个[dx/标准][绿黄红紫白]<难度> | 随机一首指定条件的乐曲
 查歌<乐曲标题的一部分> | 查询符合条件的乐曲
 [绿黄红紫白]id<歌曲编号> | 查询乐曲信息或谱面信息
 定数查歌 <定数> <br> 定数查歌 <定数下限> <定数上限> |  查询定数对应的乐曲
 分数线 <难度+歌曲id> <分数线> | 展示歌曲的分数线
+搜<手元><理论><谱面确认> | 从b站获取对应的手元视频
 
 ## 原作者
 
 [Diving-Fish](https://github.com/Diving-Fish),感谢大佬为音游人的无私奉献
 
 ## License
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-maimai Version: 0.2.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-maimai Version: 0.3.0 Summary:
 Maimai DX plugin for NoneBot Home-page: https://github.com/Agnes4m/
 nonebot_plugin_maimai License: MIT Keywords: maimai,nonebot2,plugin Author:
 Agnes_Digital Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist: httpx (>=0.22.0) Requires-
 Dist: nonebot-adapter-onebot (>=2.1.3) Requires-Dist: nonebot-plugin-txt2img
-(>=0.3.0,<0.4.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist:
-nonebot_plugin_htmlrender (>=0.2.0.3,<0.3.0.0) Requires-Dist: pillow (>=9.3.0)
-Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_maimai
-Description-Content-Type: text/markdown
+(>=0.3.0,<0.4.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: pillow
+(>=9.3.0) Project-URL: Repository, https://github.com/Agnes4m/
+nonebot_plugin_maimai Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # nonebot_plugin_maimai _â¨maimaiDXï¼nonebot2æä»¶çæ¬â¨_ [GitHub_stars]
               [GitHub_issues] [QQ_Chat_Group] [python] [NoneBot]
 ## è¯´æï¼å·²æ´æ°èèå½æ2023ï¼éæ°ä¸è½½èµæºï¼ ä»[mai-bot]
 (https://github.com/Diving-Fish/mai-
 bot)éénonebot2æä»¶ï¼æµè¯ç¯å¢nonebot2.0.0 ä¿®æ¹é¨åï¼ - b40/
 b50å¯ä»¥è¾ç¹äººæ¥è¯¢ -
 staticæä»¶å¯ä»¥æ¾maimaiæä»¶æä»¶å¤¹ä¸­ï¼ææºå¨äººè·¯å¾ä¸/data/
 maimai/static - ï¼å¯å¾ªï¼envè®¾ç½® `maimai_font`,æ¯strå¯¹è±¡ç`å­ä½` -
-æ°å¢æä»¤`bç«æç´¢[text]`
+æ°å¢æä»¤`ææå`,`æçè®º`,`æè°±é¢ç¡®è®¤`ï¼åé¢å¸¦ä¸æç´¢çå¯¹è±¡
 æåçééæé®é¢è¯·å²ææ¥ä¸è¦ææ°åä½èæï¼å¯ä»¥æissæè
-[å ç¾¤qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦, ##
+[å ç¾¤qq](https://jq.qq.com/?_wv=1027&k=l82tMuPG)åé¦, ## env(å¯é)
+maimai_font = 'simsun.ttc' # æ¿æ¢ä½ æçå­ä½ ##
 åç½®æ­¥éª¤ï¼ååé¡¹ç®ä¸æ ·ï¼ å®è£ï¼ä»éå¶ä¸ï¼: pip3 install
 nonebot_plugin_maimai nb plugin install nonebot_plugin_maimai git clone https:/
 /github.com/Agnes4m/nonebot_plugin_maimai.git æ¨éè¦ä»[æ­¤é¾æ¥](https://
 www.diving-fish.com/maibot/
 static.zip)ä¸è½½èµæºæä»¶å¹¶ï¼å¹¶å°å¶staticæä»¶è§£åå°:
 (ä»¥ä¸æ¹æ³2é1) - pypi`nonebot_plugin_maimai`æä»¶å¤¹ä¸­ -
 æç»è·¯å¾ç±»ä¼¼æ¯/path/to/nonebot_plugin_maimai/static - æºå¨äººç®å½ä¸
@@ -43,12 +43,13 @@
 ## è¯´æ æ¬ bot æä¾äºå¦ä¸åè½ï¼ å½ä»¤ | åè½ --- | --- help |
 æ¥çå¸®å©ææ¡£ ä»æ¥èè | æ¥çä»å¤©çèèè¿å¿
 XXXmaimaiXXXä»ä¹ | éæºä¸é¦æ­ éä¸ª[dx/æ å][ç»¿é»çº¢ç´«ç½]<é¾åº¦>
 | éæºä¸é¦æå®æ¡ä»¶çä¹æ² æ¥æ­<ä¹æ²æ é¢çä¸é¨å> |
 æ¥è¯¢ç¬¦åæ¡ä»¶çä¹æ² [ç»¿é»çº¢ç´«ç½]id<æ­æ²ç¼å·> |
 æ¥è¯¢ä¹æ²ä¿¡æ¯æè°±é¢ä¿¡æ¯ å®æ°æ¥æ­ <å®æ°>
 å®æ°æ¥æ­ <å®æ°ä¸é> <å®æ°ä¸é> | æ¥è¯¢å®æ°å¯¹åºçä¹æ²
-åæ°çº¿ <é¾åº¦+æ­æ²id> <åæ°çº¿> | å±ç¤ºæ­æ²çåæ°çº¿ ## åä½è
-[Diving-Fish](https://github.com/Diving-
+åæ°çº¿ <é¾åº¦+æ­æ²id> <åæ°çº¿> | å±ç¤ºæ­æ²çåæ°çº¿
+æ<æå><çè®º><è°±é¢ç¡®è®¤> | ä»bç«è·åå¯¹åºçæåè§é¢ ##
+åä½è [Diving-Fish](https://github.com/Diving-
 Fish),æè°¢å¤§ä½¬ä¸ºé³æ¸¸äººçæ ç§å¥ç® ## License MIT
 æ¨å¯ä»¥èªç±ä½¿ç¨æ¬é¡¹ç®çä»£ç ç¨äºåä¸æéåä¸çç¨éï¼ä½å¿é¡»éå¸¦
 MIT ææåè®®ã
```

