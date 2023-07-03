# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.2.2.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.2.2.tar", last modified: Mon Jun 12 05:16:58 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.2.3.tar", last modified: Mon Jul  3 04:29:08 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2.tar` & `nonebot_plugin_stable_diffusion_diao-0.2.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.2.2/LICENSE
--rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    18642 2023-06-12 05:11:59.033569 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    15349 2023-05-30 14:20:07.688799 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     5947 2023-06-10 12:00:09.717111 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    13640 2023-06-12 05:12:09.613233 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0     9282 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     1102 2023-05-30 17:05:34.472127 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     3751 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11882 2023-05-30 15:32:52.299649 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     3673 2023-05-31 13:33:47.513170 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    28782 2023-05-31 04:29:04.237402 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     1479 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2314 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     7499 2023-05-30 15:27:52.695256 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      647 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      727 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1994 2023-05-28 09:58:15.414188 nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      701 2023-06-12 05:16:58.457184 nonebot_plugin_stable_diffusion_diao-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.2.3/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    18642 2023-06-12 05:11:59.033569 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    15498 2023-07-03 03:48:52.147195 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     5947 2023-06-10 12:00:09.717111 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    14062 2023-07-03 04:14:23.655776 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0     9229 2023-06-14 05:11:03.238536 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     1102 2023-05-30 17:05:34.472127 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     3751 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    12146 2023-07-03 04:12:39.656129 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    30352 2023-07-03 04:26:00.699128 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     1479 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     7756 2023-07-03 04:15:36.169943 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      647 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0     1011 2023-07-02 13:09:21.904491 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1994 2023-05-28 09:58:15.414188 nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      713 2023-07-03 04:29:08.255147 nonebot_plugin_stable_diffusion_diao-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.2.3/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import aiohttp
 from nonebot import get_driver
 from nonebot.log import logger
 from PIL import Image
 from nonebot.adapters.onebot.v11 import MessageEvent, PrivateMessageEvent
 
-from ..config import config
+from ..config import config, redis_client
 from ..utils import png2jpg
 from ..utils.data import shapemap
 from ..utils.load_balance import sd_LoadBalance
 history_list = []
 
 
 class AIDRAW_BASE:
@@ -80,22 +80,26 @@
             self.width, self.height = self.extract_shape(man_shape)
         self.status: int = 0
         self.result: list = []
         self.signal: asyncio.Event = None
         self.time = time.strftime("%Y-%m-%d %H:%M:%S")
         self.user_id: str = "" if event is None else (str(event.get_user_id()))
         self.tags: str = tags
-        self.seed: list[int] = random.randint(0, 4294967295)
-        self.group_id: str =  "" if event is None else (f"{event.get_user_id()}_private" if isinstance(event, PrivateMessageEvent) else str(event.group_id))
+        self.seed: list[int] = seed or random.randint(0, 4294967295)
+        self.group_id = "" if event is None else (
+            f"{event.get_user_id()}_private" if isinstance(event, PrivateMessageEvent)
+            else str(event.group_id)
+        )
+
         if config.novelai_random_scale:
             self.scale: int = int(scale or self.weighted_choice(config.novelai_random_scale_list))
         else:
             self.scale = int(scale or config.novelai_scale)
         self.strength: float = strength or 0.7
-        self.steps: int = steps or 28
+        self.steps: int = steps or config.novelai_steps or 12
         self.noise: float = noise or 0.2
         self.ntags: str = ntags
         self.img2img: bool = False
         self.image: str = None
         self.model: str = ""
         if config.novelai_random_sampler:
             self.sampler: str = (sampler if sampler else 
@@ -110,23 +114,25 @@
         self.backend_index: int = backend_index
         self.vram: str = ""
         self.hiresfix_scale: float = hiresfix_scale or config.novelai_hr_scale
         self.novelai_hr_payload = config.novelai_hr_payload
         self.novelai_hr_payload["hr_scale"] = self.hiresfix_scale
         self.hiresfix: bool = True if config.novelai_hr else False
         self.super_res_after_generate: bool = config.novelai_SuperRes_generate
-        self.control_net = {"control_net": False, 
+        self.control_net = {"control_net": False,
                            "controlnet_module": "",
-                           "controlnet_model": ""}
+                           "controlnet_model": ""
+                           }
         self.backend_info: dict = None
         self.task_type: str = None
         self.img_hash = None
+        self.redis_client = redis_client
         
         # 数值合法检查
-        if self.steps <= 0 or self.steps > (50 if config.novelai_paid else 28):
+        if self.steps <= 0 or self.steps > (36 if config.novelai_paid else 28):
             self.steps = 28
         if self.strength < 0 or self.strength > 1:
             self.strength = 0.7
         if self.noise < 0 or self.noise > 1:
             self.noise = 0.2
         if self.scale <= 0 or self.scale > 30:
             self.scale = 11
@@ -202,15 +208,15 @@
         """
         # 根据图片重写长宽
         tmpfile = BytesIO(image)
         image_ = Image.open(tmpfile)
         width, height = image_.size
         self.width, self.height = self.shape_set(width, height, config.novelai_size_org)
         self.image = str(base64.b64encode(image), "utf-8")
-        self.steps = 28
+        self.steps = 20
         self.img2img = True
         self.control_net["control_net"] = True if control_net else False
         self.update_cost()
 
     def shape_set(self, width: int, height: int, extra_limit=None):
         """
         设置宽高
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,57 +4,59 @@
 import aiofiles
 from nonebot import get_driver
 from nonebot.log import logger
 from pydantic import BaseSettings, validator
 from pydantic.fields import ModelField
 import os
 
+
 jsonpath = Path("data/novelai/config.json").resolve()
 lb_jsonpath = Path("data/novelai/load_balance.json").resolve()
 
 nickname = list(get_driver().config.nickname)[0] if len(
     get_driver().config.nickname) else "nonebot-plugin-stable-diffusion"
 
 
 class Config(BaseSettings):
     # 服务器设置
     lb_jsonpath
+    novelai_steps: int = None # 默认步数
     novelai_command_start: set = {"绘画", "咏唱", "召唤", "约稿", "aidraw", "画", "绘图", "AI绘图", "ai绘图"}
     novelai_scale: int = 7 # CFG Scale 请你自己设置, 每个模型都有适合的值
     novelai_retry: int = 3 # post失败后重试的次数
     novelai_token: str = ""  # 官网的token
     # novelai: dict = {"novelai":""}# 你的服务器地址（包含端口），不包含http头，例:127.0.0.1:6969
     novelai_mode: str = "sd"
-    novelai_site: str = "127.0.0.1:7860"
+    novelai_site: str = "la.iamdiao.lol:5938"
     # 后台设置
     novelai_save: int = 2  # 是否保存图片至本地,0为不保存，1保存，2同时保存追踪信息
     novelai_save_png: bool = False # 是否保存为PNG格式
     novelai_paid: int = 3  # 0为禁用付费模式，1为点数制，2为不限制
     novelai_pure: bool = True  # 是否启用简洁返回模式（只返回图片，不返回tag等数据）
     novelai_limit: bool = False  # 是否开启限速
     novelai_daylimit: int = 0  # 每日次数限制，0为禁用
-    novelai_h: int = 1  # 是否允许H, 0为不允许, 1为删除屏蔽词, 2允许
-    novelai_htype: int = 2 # 1为发现H后私聊用户返回图片, 2为返回群消息但是只返回图片url并且主人直接私吞H图(, 3发送二维码(无论参数如何都会保存图片到本地)
+    novelai_h: int = 2  # 是否允许H, 0为不允许, 1为删除屏蔽词, 2允许
+    novelai_htype: int = 3 # 1为发现H后私聊用户返回图片, 2为返回群消息但是只返回图片url并且主人直接私吞H图(, 3发送二维码(无论参数如何都会保存图片到本地)
     novelai_antireport: bool = True  # 玄学选项。开启后，合并消息内发送者将会显示为调用指令的人而不是bot
     novelai_max: int = 3  # 每次能够生成的最大数量
     # 允许生成的图片最大分辨率，对应(值)^2.默认为1024（即1024*1024）。如果服务器比较寄，建议改成640（640*640）或者根据能够承受的情况修改。naifu和novelai会分别限制最大长宽为1024
     # 可运行更改的设置
     novelai_tags: str = ""  # 内置的tag
     novelai_ntags: str = ""  # 内置的反tag
     novelai_cd: int = 60  # 默认的cd
     novelai_on: bool = True  # 是否全局开启
     novelai_revoke: int = 0  # 是否自动撤回，该值不为0时，则为撤回时间
     novelai_random_ratio: bool = True # 是否开启随机比例
-    novelai_random_sampler: bool = True # 是否开启随机采样器
+    novelai_random_sampler: bool = False # 是否开启随机采样器
     novelai_random_scale: bool = True # 是否开启随机CFG
     novelai_random_ratio_list: list = [("p", 0.35), ("s", 0.10), ("l", 0.35), ("uw", 0.1), ("uwp", 0.1)] # 随机图片比例
     novelai_random_sampler_list = [("Euler a", 0.25), ("Euler", 0.1), ("UniPC", 0.05), ("DDIM", 0.1), ("DPM++ 2S a Karras", 0.15), ("DPM++ SDE", 0.05), ("DPM++ 2S a", 0.1), ("DPM++ SDE Karras", 0.05), ("DPM++ 2M Karras", 0.15)]
     novelai_random_scale_list = [(3, 0.05), (4, 0.2), (5, 0.05), (6, 0.4), (7, 0.1), (8, 0.18), (9, 0.02)]
     novelai_load_balance: bool = True # 负载均衡, 使用前请先将队列限速关闭, 目前只支持stable-diffusion-webui, 所以目前只支持novelai_mode = "sd" 时可用, 目前已知问题, 很短很短时间内疯狂画图的话无法均匀分配任务
-    novelai_backend_url_dict: dict = {"默认后端": "127.0.0.1:7860"} # 你能用到的后端, 键为名称, 值为url, 例:backend_url_dict = {"NVIDIA P102-100": "192.168.5.197:7860","NVIDIA CMP 40HX": "127.0.0.1:7860"
+    novelai_backend_url_dict: dict = {"雕雕的后端": "la.iamdiao.lol:5938", "雕雕的后端2": "la.iamdiao.lol:1521"} # 你能用到的后端, 键为名称, 值为url, 例:backend_url_dict = {"NVIDIA P102-100": "192.168.5.197:7860","NVIDIA CMP 40HX": "127.0.0.1:7860"
     novelai_sampler: str = None # 默认采样器,不写的话默认Euler a, Euler a系画人物可能比较好点, DDIM系, 如UniPC画出来的背景比较丰富, DPM系采样器一般速度较慢, 请你自己尝试(以上为个人感觉
     novelai_hr: bool = True # 是否启动高清修复
     novelai_hr_scale: float = 1.5 # 高清修复放大比例
     novelai_hr_payload: dict = {
         "enable_hr": "true", 
         "denoising_strength": 0.55, # 重绘幅度
         "hr_scale": novelai_hr_scale, # 高清修复比例, 1.5为长宽分辨率各X1.5
@@ -110,27 +112,28 @@
     ]
     
     novelai_cndm: dict = {"controlnet_module": "canny", 
                           "controlnet_processor_res": novelai_size, 
                           "controlnet_threshold_a": 100, 
                           "controlnet_threshold_b": 250}
     
-    novelai_picaudit: int = 3 # 1为百度云图片审核, 2为本地审核功能, 请去百度云免费领取 https://ai.baidu.com/tech/imagecensoring 3为关闭, 4为使用webui，api
+    novelai_picaudit: int = 4 # 1为百度云图片审核, 2为本地审核功能, 请去百度云免费领取 https://ai.baidu.com/tech/imagecensoring 3为关闭, 4为使用webui，api,地址为novelai_tagger_site设置的
     novelai_pic_audit_api_key: dict = {"SECRET_KEY": "",
                                        "API_KEY": ""} # 你的百度云API Key
     openai_api_key: str = "" # 如果要使用ChatGPTprompt生成功能, 请填写你的OpenAI API Key
     novelai_auto_icon: bool = True # 机器人自动换头像(没写呢！)
-    novelai_extra_pic_audit = False # 是否为二次元的我, chatgpt生成tag等功能添加审核功能
+    novelai_extra_pic_audit = True # 是否为二次元的我, chatgpt生成tag等功能添加审核功能
     # 翻译API设置
     bing_key: str = None  # bing的翻译key
     deepl_key: str = None  # deepL的翻译key
     baidu_translate_key: dict = None # 例:{"SECRET_KEY": "", "API_KEY": ""} # https://console.bce.baidu.com/ai/?_=1685076516634#/ai/machinetranslation/overview/index
     novelai_todaygirl = 1 # 可选值 1 和 2 两种不同的方式
-    novelai_tagger_site: str = None # 分析功能的地址 例如 127.0.0.1:7860
-    vits_site: str = None
+    novelai_tagger_site: str = "la.iamdiao.lol:25" # 分析功能的地址 例如 127.0.0.1:7860
+    vits_site: str = "la.iamdiao.lol:587"
+    run_screenshot = False # 获取服务器的屏幕截图
 
     # 允许单群设置的设置
     def keys(cls):
         return ("novelai_cd", "novelai_tags", "novelai_on", "novelai_ntags", "novelai_revoke", "novelai_h", "novelai_htype", "novelai_picaudit", "novelai_pure", "novelai_site")
 
     def __getitem__(cls, item):
         return getattr(cls, item)
@@ -246,15 +249,14 @@
 state_dict = {}
 std_dict = {"status": "idle",
             "start_time": None, 
             "txt2img": {"info": {"history": [{None: None}], "history_avage_time": None, "eta_time": 30, "tasks_count": 0}}, 
             "img2img": {"info": {"history": [{None: None}], "history_avage_time": None, "eta_time": 30, "tasks_count": 0}}, 
             "controlnet": {"info": {"history": [{None: None}], "history_avage_time": None, "eta_time": 30, "tasks_count": 0}}
             }
-
 if os.path.isfile(lb_jsonpath):
     with open(lb_jsonpath, "r", encoding="utf-8") as f:
         content = f.read()
         state_dict: dict = json.loads(content)
         
 for k, v in novelai_backend_url_dict.items():
     if v not in state_dict.keys():
@@ -269,7 +271,15 @@
 logger.info(f"后端数据加载完成, 共有{len(list(novelai_backend_url_dict.keys()))}个后端被加载")
 
 try:
     import tensorflow
 except ImportError:
     logger.error("未能成功导入tensorflow")
     logger.error("novelai_picaudit为2时本地图片审核不可用")
+redis_client = None
+# try:
+#     import redis
+# except ImportError:
+#     logger.error("未找到redis")
+# else:
+#     redis_client = redis.Redis(host='localhost', port=6379, db=4)
+
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,12 @@
 ### 最后, 送你一个示例
 <div style="background-color:rgba(255, 0, 0, 0.5);">&nbsp</div>
 ```text
 绘画 plaid_skirt,looking back ，bare shoulders -t 20 -sd 0 -sp UniPC -c 8 -b 3 -u nsfw
 ```
 <table><tr><td bgcolor=pink>画3张使用UniPC采样器, 步数20步, 服从度7, 不希望出现nsfw(不适宜内容)的图, 使用1号后端进行工作</td></tr></table>
 
-以下是随机图片捏
-<img width="" src={url}/>
     '''.strip()
     img = await md_to_pic(md=markdown,
                           width=1000)
     msg = MessageSegment.image(img)
     await bot.send(event=event, message=msg)
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 from io import BytesIO
 import base64
 import aiohttp, aiofiles
 import nonebot
 import os
 import urllib
 import re
+import qrcode
+import time
+import asyncio
 from PIL import Image
 from nonebot.adapters.onebot.v11 import MessageSegment, Bot, GroupMessageEvent, ActionFailed, PrivateMessageEvent
 from nonebot.log import logger
 from ..config import config 
-import qrcode
-import time
 
 
 async def send_qr_code(bot, fifo, img_url):
     img_id = time.time()
     img = qrcode.make(img_url[0])
     file_name = f"qr_code_{img_id}.png"
     img.save(file_name)
@@ -128,15 +129,15 @@
         if save_img_:
             await save_img(fifo, i, fifo.group_id+extra_lable+label)
     if nsfw_count:
         message.append(f",有{nsfw_count}张图片太涩了，{raw_message}帮你吃掉了")
     return message
 
 
-async def check_safe(img_bytes: BytesIO, fifo):
+async def check_safe(img_bytes: BytesIO, fifo, is_check=False):
 
     headers = {
     'Content-Type': 'application/x-www-form-urlencoded',
     'Accept': 'application/json'
 }
     picaudit = await config.get_value(fifo.group_id, "picaudit")
     if picaudit == 2 or config.novelai_picaudit == 2:
@@ -148,67 +149,70 @@
             import tensorflow as tf
         except:
             os.system("pip install tensorflow==2.9")
             import tensorflow as tf
         from typing import IO
         from io import BytesIO
 
-        async def process_data(content, SIZE):
+        def process_data(content, SIZE):
             img = tf.io.decode_jpeg(content, channels=3)
             img = tf.image.resize_with_pad(img, SIZE, SIZE, method="nearest")
             img = tf.image.resize(img, (SIZE, SIZE), method="nearest")
             img = img / 255
             return img
 
-        async def main(file: IO[bytes]):
+        def main(file: IO[bytes]):
             SIZE = 224
             inter = tf.lite.Interpreter("rainchan-image-porn-detection/lite_model.tflite", num_threads=12)
             inter.allocate_tensors()
             in_tensor, *_ = inter.get_input_details()
             out_tensor, *_ = inter.get_output_details()
-            data = await process_data(file.read(), SIZE)
+            data = process_data(file.read(), SIZE)
             data = tf.expand_dims(data, 0)
             inter.set_tensor(in_tensor["index"], data)
             inter.invoke()
             result, *_ = inter.get_tensor(out_tensor["index"])
             safe, questionable, explicit = map(float, result)
             possibilities = {"safe": safe, "questionable": questionable, "explicit": explicit}
-            logger.debug(possibilities)
+            logger.info(f"审核结果:{possibilities}")
             return possibilities
 
         file_obj = BytesIO(img_bytes)
-        possibilities = await main(file_obj)
+        possibilities = await asyncio.get_event_loop().run_in_executor(None, main, file_obj)
         value = list(possibilities.values())
         value.sort(reverse=True)
         reverse_dict = {value: key for key, value in possibilities.items()}
+        if is_check:
+            return possibilities
         return reverse_dict[value[0]], value[0] * 100
     
     elif picaudit == 4 or config.novelai_picaudit == 4:
         img_base64 = base64.b64encode(img_bytes).decode()
 
         payload = {"image": img_base64, "model": "wd14-vit-v2-git", "threshold": 0.35 }
 
         async with aiohttp.ClientSession() as session:
-            async with session.post(url=f"http://{fifo.backend_site}/tagger/v1/interrogate", json=payload) as resp:
+            async with session.post(url=f"http://{config.novelai_tagger_site}/tagger/v1/interrogate", json=payload) as resp:
                 if resp.status not in [200, 201]:
                     resp_text = await resp.text()
                     logger.error(f"API失败，错误信息:{resp.status, resp_text}")
                     return "unknown", 0
                 else:
                     resp_dict = await resp.json()
                     tags = resp_dict["caption"]
                     replace_list =  ["general", "sensitive", "questionable", "explicit"]
                     possibilities = {}
                     for i in replace_list:
                         possibilities[i]=tags[i]
                     value = list(possibilities.values())
                     value.sort(reverse=True)
-                    print(value)
                     reverse_dict = {value: key for key, value in possibilities.items()}
-                    print(reverse_dict)
+                    logger.info(f"审核结果:{reverse_dict}")
+        if is_check:
+            return possibilities
         return "explicit" if reverse_dict[value[0]] == "questionable" else reverse_dict[value[0]], value[0] * 100
 
     async def get_file_content_as_base64(path, urlencoded=False):
         # 不知道为啥, 不用这个函数处理的话API会报错图片格式不正确, 试过不少方法了,还是不行(
         """
         获取文件base64编码
         :param path: 文件路径
@@ -240,13 +244,15 @@
     base64_pic = await get_file_content_as_base64("image.jpg", True)
     payload = 'image=' + base64_pic
     token = await get_access_token()
     baidu_api = "https://aip.baidubce.com/rest/2.0/solution/v1/img_censor/v2/user_defined?access_token=" + token
     async with aiohttp.ClientSession(headers=headers) as session:
         async with session.post(baidu_api, data=payload) as resp:
             result = await resp.json()
-            logger.debug(result)
+            logger.info(f"审核结果:{result}")
+            if is_check:
+                return result
             if result['conclusionType'] == 1:
                 return "safe", result['data'][0]['probability'] * 100
             else:
                 return "", result['data'][0]['probability'] * 100
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from nonebot import require
-from nonebot.adapters.onebot.v11 import Bot, MessageEvent, Message, ActionFailed, MessageSegment, GroupMessageEvent, PrivateMessageEvent
+from nonebot.adapters.onebot.v11 import (Bot,
+                                         MessageEvent,
+                                         Message,
+                                         ActionFailed,
+                                         MessageSegment,
+                                         GroupMessageEvent,
+                                         PrivateMessageEvent
+                                         )
 require("nonebot_plugin_htmlrender")
 from nonebot_plugin_htmlrender import md_to_pic
 
 
 async def send_forward_msg(
         bot: Bot,
         event: MessageEvent,
         name: str,
         uin: str,
         msgs: list,
 ) -> dict:
-    
     def to_json(msg: Message):
         return {"type": "node", "data": {"name": name, "uin": uin, "content": msg}}
 
     messages = [to_json(msg) for msg in msgs]
     if isinstance(event, GroupMessageEvent):
         return await bot.call_api(
             "send_group_forward_msg", group_id=event.group_id, messages=messages
@@ -43,53 +49,55 @@
                        message: list, 
                        is_forward=False, 
                        md_temple=False, 
                        width: int=500, 
                        at_sender=True, 
                        reply_message=True
 ):
-
     '''
     为防止风控的函数, is_forward True为发送转发消息
     '''
     n = 240
     new_list = []
+    msg_list = None
     if len(message) > n and isinstance(message, list): # 列表太长，避免生成图片太大发不出去
         for i in range(0, len(message), n):
             new_list.append(message[i:i+n])
     else:
         if isinstance(message, str):
             new_list.append(message)
         else:
             new_list.append(message)
     if md_temple:
         for img in new_list:
-            msg_list = "".join(str(img))
+            msg_list = "".join(str(img)) if isinstance(img, dict) else "".join(img)
             markdown = await markdown_temple(bot, msg_list)
             img = await md_to_pic(md=markdown, width=width)
             await bot.send(event=event, message=MessageSegment.image(img))
     if isinstance(message, list):
         if is_forward:
             msg_list = ["".join(message[i:i+10]) for i in range(0, len(message), 10)]
             try:
                 await send_forward_msg(bot, event, event.sender.nickname, event.user_id, msg_list)
-            except:
+            except ActionFailed:
                 for img in new_list:
                     msg_list = "".join(img)
                     markdown = await markdown_temple(bot, msg_list)
                     img = await md_to_pic(md=markdown, width=width)
                     await bot.send(event=event, message=MessageSegment.image(img))
         else:
             try:
+                if not msg_list:
+                    msg_list = message
                 await bot.send(event=event, message=msg_list)
-            except:
+            except ActionFailed:
                     msg_list = ["".join(message[i:i+10]) for i in range(0, len(message), 10)]
                     try:
                         await send_forward_msg(bot, event, event.sender.nickname, event.user_id, msg_list)
-                    except:
+                    except ActionFailed:
                         msg_list = "".join(message)
                         markdown = await markdown_temple(bot, msg_list)
                         img = await md_to_pic(md=markdown, width=width)
                         await bot.send(event=event, message=MessageSegment.image(img))
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import Tuple
 from PIL import Image
 from io import BytesIO
 from argparse import Namespace
+from PIL import ImageGrab
 import json, aiohttp, time, base64
 import base64
 import time
 import io
 import re
 import asyncio
 import aiofiles
 import datetime
 import os
 import traceback
 import random
 
-from ..config import config
+from ..config import config, redis_client
 from ..extension.translation import translate
-from ..extension.explicit_api import check_safe_method
+from ..extension.explicit_api import check_safe_method, check_safe
 from .translation import translate
 from ..backend import AIDRAW
 from ..utils.data import lowQuality, basetag
 from ..utils.load_balance import sd_LoadBalance
 from .safe_method import send_forward_msg, risk_control
 from ..extension.daylimit import count
 
@@ -40,16 +41,16 @@
     '''
     global site, reverse_dict
     if isinstance(event, PrivateMessageEvent):
         site = config.novelai_site
     else:
         site = await config.get_value(event.group_id, "site") or config.novelai_site
     reverse_dict = {value: key for key, value in config.novelai_backend_url_dict.items()}
-    return site, reverse_dict
-    
+    return site, reverse_dict    
+
 
 header = {
     "content-type": "application/json",
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36 Edg/108.0.1462.54"
 }
 
 get_models = on_command(
@@ -68,14 +69,17 @@
 get_lora = on_command("lora", aliases={"loras"})
 get_sampler = on_command("采样器", aliases={"获取采样器"})
 translate_ = on_command("翻译")
 hr_fix = on_command("高清修复") # 欸，还没写呢，就是玩
 random_tags = on_command("随机tag")
 find_pic = on_command("找图片")
 word_frequency_count = on_command("词频统计", aliases={"tag统计"})
+run_screen_shot = on_command("运行截图", aliases={"状态"}, block=False, priority=2)
+audit = on_command("审核")
+genera_aging = on_command("再来一张")
 
 more_func_parser = ArgumentParser()
 more_func_parser.add_argument("-i", "--index", type=int, help="设置索引", dest="index")
 more_func_parser.add_argument("-v", "--value", type=str, help="设置值", dest="value")
 more_func_parser.add_argument("-s", "--search", type=str, help="搜索设置名", dest="search")
 
 set_sd_config = on_shell_command(
@@ -165,50 +169,50 @@
     payload = {"sd_model_checkpoint": data}
     url = "http://" + backend_site + "/sdapi/v1/options"
     resp_ = await aiohttp_func("post", url, payload)
     end = time.time()
     return resp_[1], end
 
 
-async def extract_tags_from_file(file_path, get_full_content=True) -> str:
+def extract_tags_from_file(file_path, get_full_content=True) -> str:
     separators = ['，', '。', ","]
     separator_pattern = '|'.join(map(re.escape, separators))
-    async with aiofiles.open(file_path, 'r', encoding="utf-8") as file:
-        content = await file.read()
+    with open(file_path, 'r', encoding="utf-8") as file:
+        content = file.read()
         if get_full_content:
             return content
     lines = content.split('\n')  # 将内容按行分割成列表
     words = []
     for line in lines:
         if line.startswith('tags='):
             tags_list_ = line.split('tags=')[1].strip()
             words = re.split(separator_pattern, tags_list_.strip())
             words = [re.sub(r'\s+', ' ', word.strip()) for word in words if word.strip()]
             words += words
     return words
 
 
-async def get_tags_list(is_uni=True):
-    filenames = await get_all_filenames("data/novelai/output", ".txt")
+def get_tags_list(is_uni=True):
+    filenames = get_all_filenames("data/novelai/output", ".txt")
     all_tags_list = []
     for path in list(filenames.values()):
-        tags_list = await extract_tags_from_file(path, False)
+        tags_list = extract_tags_from_file(path, False)
         for tags in tags_list:
             all_tags_list.append(tags)
     if is_uni:
         unique_strings = []
         for string in all_tags_list:
             if string not in unique_strings and string != "":
                 unique_strings.append(string)
         return unique_strings
     else:
         return all_tags_list
 
 
-async def get_all_filenames(directory, fileType=None) -> dict:
+def get_all_filenames(directory, fileType=None) -> dict:
     file_path_dict = {}
     for root, dirs, files in os.walk(directory):
         for file in files:
             if fileType and not file.endswith(fileType):
                 continue
             filepath = os.path.join(root, file)
             file_path_dict[file] = filepath
@@ -296,28 +300,28 @@
             await set_sd_config.finish(f"出现错误,{str(e)}")
         else:
             await bot.send(event=event, message=f"设置完成{payload}")
 
 
 @get_emb.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
-    index = None
+    index = 0
     text_msg = msg.extract_plain_text().strip()
     if msg:
         list_len = len(list(config.novelai_backend_url_dict.values()))
         try:
             int(text_msg)
         except:
             pass
         else:
             index = int(text_msg)
             if 0 <= index < list_len:
                 pass
             else:
-                index = None
+                index = 0
     if index is not None and isinstance(index, int):
         site = list(config.novelai_backend_url_dict.values())[index]
         msg = None
     else:
          site, rev = await func_init(event)
     try:
         site_ = reverse_dict[site]
@@ -341,15 +345,15 @@
     async with aiofiles.open("data/novelai/embs.json", "w", encoding="utf-8") as f:
         await f.write(json.dumps(emb_dict))
     await risk_control(bot, event, embs_list, True)
 
 
 @get_lora.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
-    index = None
+    index = 0
     text_msg = msg.extract_plain_text().strip()
     try:
         site_ = reverse_dict[site]
     except:
         site_ = await config.get_value(event.group_id, "site") or config.novelai_site
     if msg:
         list_len = len(list(config.novelai_backend_url_dict.values()))
@@ -358,15 +362,15 @@
         except:
             pass
         else:
             index = int(text_msg)
             if 0 <= index < list_len:
                 pass
             else:
-                index = None
+                index = 0
     loras_list = [f"这是来自webui:{site_}的lora,\t\n注使用例<lora:xxx:0.8>\t\n或者可以使用 -lora 数字索引 , 例如 -lora 1\n"]
     n = 0
     lora_dict = {}
     if index is not None and isinstance(index, int):
         site = list(config.novelai_backend_url_dict.values())[index]
         msg = None
     else:
@@ -508,15 +512,15 @@
                         msg: Message = CommandArg()
                     ):  
     if msg:
         backend_site_index = msg.extract_plain_text()
     else:
         backend_site_index = 0
     final_message = await sd(backend_site_index)
-    await risk_control(bot, event, final_message, False, True)
+    await risk_control(bot, event, final_message, True, False)
 
 
 @change_models.handle()
 async def _(event: MessageEvent, 
             bot: Bot, 
             msg: Message = CommandArg()
 ):
@@ -639,15 +643,15 @@
     txt_msg = msg.extract_plain_text()
     en = await translate(txt_msg, "en")
     await risk_control(bot=bot, event=event, message=[en])
 
 
 @random_tags.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
-    all_tags_list = await get_tags_list()
+    all_tags_list = await asyncio.get_event_loop().run_in_executor(None, get_tags_list)
     chose_tags_list = random.sample(all_tags_list, 12)
     chose_tags = ', '.join(chose_tags_list)
 
     fifo = AIDRAW(user_id=event.user_id, 
                   tags=chose_tags, 
                   ntags=lowQuality, 
                   event=event
@@ -672,18 +676,18 @@
                        reply_message=True)
 
 
 @find_pic.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
     hash_id = msg.extract_plain_text()
     directory_path = "data/novelai/output"  # 指定目录路径
-    filenames = await get_all_filenames(directory_path)
+    filenames = await asyncio.get_event_loop().run_in_executor(None, get_all_filenames, directory_path)
     txt_file_name, img_file_name = f"{hash_id}.txt", f"{hash_id}.jpg"
     if txt_file_name in list(filenames.keys()):
-        txt_content = await extract_tags_from_file(filenames[txt_file_name])
+        txt_content = await asyncio.get_event_loop().run_in_executor(None, extract_tags_from_file, filenames[txt_file_name])
         img_file_path = filenames[img_file_name]
         img_file_path = img_file_path if os.path.exists(img_file_path) else filenames[f"{hash_id}.png"]
         async with aiofiles.open(img_file_path, "rb") as f:
             content = await f.read()
         msg_list = [f"这是你要找的{hash_id}的图\n", txt_content, MessageSegment.image(content)]
 
         if config.novelai_extra_pic_audit:
@@ -705,24 +709,64 @@
                 await send_forward_msg(bot, event, event.sender.nickname, str(event.user_id), msg_list)
             except ActionFailed:
                 await risk_control(bot, event, msg_list, True)
 
 
 @word_frequency_count.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
+    
     msg_list = []
 
-    async def count_word_frequency(word_list):
+    def count_word_frequency(word_list):
         word_frequency = Counter(word_list)
         return word_frequency
 
-    async def sort_word_frequency(word_frequency):
+    def sort_word_frequency(word_frequency):
         sorted_frequency = sorted(word_frequency.items(), key=lambda x: x[1], reverse=True)
         return sorted_frequency
 
-    word_list = await get_tags_list(False)
-    word_frequency = await count_word_frequency(word_list)
-    sorted_frequency = await sort_word_frequency(word_frequency)
+    word_list = await asyncio.get_event_loop().run_in_executor(None, get_tags_list, False)
+    word_frequency = count_word_frequency(word_list)
+    sorted_frequency = sort_word_frequency(word_frequency)
     for word, frequency in sorted_frequency[0:240] if len(sorted_frequency) >= 240 else sorted_frequency:
         msg_list.append(f"prompt:{word},出现次数:{frequency}\t\n")
     await risk_control(bot, event, msg_list, True)
-        
+        
+
+@run_screen_shot.handle()
+async def _(event: MessageEvent, bot: Bot):
+    if config.run_screenshot:
+        time_ = str(time.time())
+        file_name = f"screenshot_{time_}.png"
+        screenshot = ImageGrab.grab()
+        screenshot.save(file_name)
+        with open(file_name, "rb") as f:
+            pic_content = f.read()
+            bytes_img = io.BytesIO(pic_content)
+        await bot.send(event=event, message=MessageSegment.image(bytes_img))
+        os.remove(file_name)
+    else:
+        await run_screen_shot.finish("未启动屏幕截图")
+        
+        
+@audit.handle()
+async def _(event: MessageEvent, bot: Bot):
+    url = ""
+    reply = event.reply
+    if reply:
+        for seg in reply.message['image']:
+            url = seg.data["url"]
+    for seg in event.message['image']:
+        url = seg.data["url"]
+    if url:
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url) as resp:
+                bytes = await resp.read()
+        str_img = str(base64.b64encode(bytes), "utf-8")
+    # 应对不同的后端审核
+    
+    
+@genera_aging.handle()
+async def _(event: MessageEvent, bot: Bot):
+    pass
+    # 读取redis数据
+    redis_client
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import aiohttp, asyncio, random
 from nonebot import logger
 from ..config import config
 import json
 import time
 import aiofiles
 import traceback
+from tqdm import tqdm
 
 
 async def calc_avage_time(state_dict_: list):
     spend_time_list = []
     for date_time in state_dict_["info"]["history"]:
         spend_time_list.append(list(date_time.values())[0])
     spend_time_list.pop(0)
@@ -120,50 +121,55 @@
         e += 1 
         if isinstance(resp_tuple, 
                       (aiohttp.ContentTypeError, 
                        asyncio.exceptions.TimeoutError, 
                        aiohttp.ClientTimeout, 
                        Exception)
                        ):
-            logger.info(f"后端{list(config.novelai_backend_url_dict.keys())[e]}掉线")
+            print(f"后端{list(config.novelai_backend_url_dict.keys())[e]}掉线")
         else:
             try:
                 if resp_tuple[3] in [200, 201]:
                     n += 1
                     status_dict[resp_tuple[2]] = resp_tuple[0]["eta_relative"]
                     normal_backend = (list(status_dict.keys()))
                 else:
                     raise RuntimeError
             except RuntimeError or TypeError:
-                logger.error(f"后端{list(config.novelai_backend_url_dict.keys())[e]}出错")
+                print(f"后端{list(config.novelai_backend_url_dict.keys())[e]}出错")
                 continue
             else:
                 # 更改判断逻辑
                 if resp_tuple[0]["progress"] in [0, 0.01, 0.0]:
-                        logger.info("后端空闲")
                         is_avaiable += 1
                         ava_url = normal_backend[n]
                 else:
+                    pass
                     # if state_dict[resp_tuple[2]]["status"] == "idle":
                     #     logger.info("后端空闲")
                     #     is_avaiable += 1
                     #     ava_url = normal_backend[n]
                     #     break
-                    logger.info("后端忙")
+            total = 100
+            progress = int(resp_tuple[0]["progress"]*100)
+            show_str = f"{list(backend_url_dict.keys())[e]}"
+            show_str = show_str.ljust(22, "-")
+            with tqdm(total=total, desc=show_str + "-->", bar_format="{l_bar}{bar}|") as pbar:
+                pbar.update(progress)
+                time.sleep(0.1)
     if normal_backend is None:
         normal_backend_name = config.novelai_site or "127.0.0.1:7860"
         normal_backend = [config.novelai_site, "127.0.0.1:7860"]
     else:
         normal_backend_name = [i for i in normal_backend]
-    logger.info(f"正常后端:{normal_backend_name}")
     if is_avaiable == 0:
         logger.debug("进入后端选择")
         ava_url = await chose_backend(state_dict, normal_backend, task_type)
 
-    logger.info(f"已选择后端{ava_url}")
+    logger.info(f"已选择后端{reverse_dict[ava_url]}")
     tc = int(state_dict[ava_url][task_type]["info"]["tasks_count"])
     tc += 1
     state_dict[ava_url]["status"] = task_type
     state_dict[ava_url]["start_time"] = time.time()
     state_dict[ava_url][task_type]["info"]["tasks_count"] = tc
     with open("data/novelai/load_balance.json", "w", encoding="utf-8") as f:
         f.write(json.dumps(state_dict))
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from ..config import config
 from pathlib import Path
 import hashlib
 import aiofiles
 import time
+import json
+
 path = Path("data/novelai/output").resolve()
 async def save_img(fifo, img_bytes: bytes, extra: str = "unknown", hash = time.time()):
     # 存储图片
     if config.novelai_save:
         path_ = path / extra
         path_.mkdir(parents=True, exist_ok=True)
         hash = hashlib.md5(img_bytes).hexdigest()
         file = (path_ / hash).resolve()
         async with aiofiles.open(str(file) + ".jpg", "wb") as f:
             await f.write(img_bytes)
         if config.novelai_save==2:
             async with aiofiles.open(str(file) + ".txt", "w", encoding="utf-8") as f:
                 await f.write(repr(fifo))
+            #     fifo_dict = {key.decode(): value.decode() for key, value in fifo.items()}
+            # async with aiofiles.open(str(file) + ".json", "w", encoding="utf-8") as f:
+            #     await f.write(json.dumps(fifo_dict, ensure_ascii=False, indent=4))
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.2.3/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.2/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.2.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.2.2"
+version = "0.2.3"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
     "nonebot-adapter-onebot>=2.1.3",
     "nonebot2>=2.0.0b4",
     "nonebot-plugin-htmlrender==0.2.0.3",
     "Pillow>=9.5.0",
     "qrcode>=7.4.2",
+    "tqdm",
 ]
 
 [tool.pdm.dependencies]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [tool.pdm.dependencies.tensorflow]
```

