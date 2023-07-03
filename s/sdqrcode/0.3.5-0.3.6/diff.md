# Comparing `tmp/sdqrcode-0.3.5.tar.gz` & `tmp/sdqrcode-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdqrcode-0.3.5.tar", max compression
+gzip compressed data, was "sdqrcode-0.3.6.tar", max compression
```

## Comparing `sdqrcode-0.3.5.tar` & `sdqrcode-0.3.6.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-06-27 22:29:11.086199 sdqrcode-0.3.5/LICENSE
--rw-r--r--   0        0        0    10185 2023-06-27 22:29:11.086199 sdqrcode-0.3.5/README.md
--rw-r--r--   0        0        0      495 2023-06-27 22:29:11.146199 sdqrcode-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     3305 2023-06-27 22:29:11.150199 sdqrcode-0.3.5/src/sdqrcode/Engines/AutoEngine.py
--rw-r--r--   0        0        0     8100 2023-06-27 22:29:11.150199 sdqrcode-0.3.5/src/sdqrcode/Engines/DiffusersEngine.py
--rw-r--r--   0        0        0      186 2023-06-27 22:29:11.150199 sdqrcode-0.3.5/src/sdqrcode/Engines/Engine.py
--rw-r--r--   0        0        0      426 2023-06-27 22:29:11.150199 sdqrcode-0.3.5/src/sdqrcode/Engines/engine_util.py
--rw-r--r--   0        0        0       32 2023-06-27 22:29:11.150199 sdqrcode-0.3.5/src/sdqrcode/__init__.py
--rw-r--r--   0        0        0       22 2023-06-27 22:29:11.150199 sdqrcode-0.3.5/src/sdqrcode/configs/custom.yaml
--rw-r--r--   0        0        0      737 2023-06-27 22:29:11.150199 sdqrcode-0.3.5/src/sdqrcode/configs/default.yaml
--rw-r--r--   0        0        0      719 2023-06-27 22:29:11.150199 sdqrcode-0.3.5/src/sdqrcode/configs/default_auto.yaml
--rw-r--r--   0        0        0      777 2023-06-27 22:29:11.150199 sdqrcode-0.3.5/src/sdqrcode/configs/default_diffusers.yaml
--rw-r--r--   0        0        0      624 2023-06-27 22:29:11.150199 sdqrcode-0.3.5/src/sdqrcode/configs/img2img_tile_auto.yaml
--rw-r--r--   0        0        0      644 2023-06-27 22:29:11.150199 sdqrcode-0.3.5/src/sdqrcode/configs/img2img_tile_diffusers.yaml
--rw-r--r--   0        0        0    12834 2023-06-27 22:29:11.150199 sdqrcode-0.3.5/src/sdqrcode/sdqrcode.py
--rw-r--r--   0        0        0    11018 1970-01-01 00:00:00.000000 sdqrcode-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-03 10:27:17.188494 sdqrcode-0.3.6/LICENSE
+-rw-r--r--   0        0        0    10567 2023-07-03 10:27:17.188494 sdqrcode-0.3.6/README.md
+-rw-r--r--   0        0        0      495 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3305 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/Engines/AutoEngine.py
+-rw-r--r--   0        0        0     8787 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/Engines/DiffusersEngine.py
+-rw-r--r--   0        0        0      186 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/Engines/Engine.py
+-rw-r--r--   0        0        0      502 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/Engines/engine_util.py
+-rw-r--r--   0        0        0       32 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/__init__.py
+-rw-r--r--   0        0        0      719 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/brightness_auto.yaml
+-rw-r--r--   0        0        0      610 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/brightness_diffusers.yaml
+-rw-r--r--   0        0        0       22 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/custom.yaml
+-rw-r--r--   0        0        0      737 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/default.yaml
+-rw-r--r--   0        0        0      719 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/default_auto.yaml
+-rw-r--r--   0        0        0      777 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/default_diffusers.yaml
+-rw-r--r--   0        0        0      624 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/img2img_tile_auto.yaml
+-rw-r--r--   0        0        0      644 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/img2img_tile_diffusers.yaml
+-rw-r--r--   0        0        0    13545 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/sdqrcode.py
+-rw-r--r--   0        0        0    11400 1970-01-01 00:00:00.000000 sdqrcode-0.3.6/PKG-INFO
```

### Comparing `sdqrcode-0.3.5/LICENSE` & `sdqrcode-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.5/README.md` & `sdqrcode-0.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -232,7 +232,13 @@
 - [ ] try to install the webui in demo colab
 - [x] add diffusers backend
 - [ ] add docs
 - [ ] allow to change models
 
 # Contrib
 Please don't hesitate to submit a PR to improve the code or submit a config
+
+# Other projects
+You can checkout [our website](https://koll.ai) to discover more of our projects such as:
+- [Seg2Sat](https://huggingface.co/spaces/rgres/Seg2Sat): Controlnet model to generate aerial pictures 
+- [PoetGPT](https://poetgpt.koll.ai): generate beautiful poems and lyrics with AI 
+- [ThisSCPDoesNotExist](https://thisscpdoesnotexist.ml/): generate custom SCP entities
```

### Comparing `sdqrcode-0.3.5/src/sdqrcode/Engines/AutoEngine.py` & `sdqrcode-0.3.6/src/sdqrcode/Engines/AutoEngine.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.5/src/sdqrcode/Engines/DiffusersEngine.py` & `sdqrcode-0.3.6/src/sdqrcode/Engines/DiffusersEngine.py`

 * *Files 19% similar despite different names*

```diff
@@ -49,32 +49,36 @@
 from diffusers.schedulers.scheduling_dpmsolver_multistep import (
     DPMSolverMultistepScheduler,
 )
 from diffusers.schedulers.scheduling_pndm import PNDMScheduler
 
 
 class DiffusersEngine(Engine.Engine):
-    def __init__(self, config):
+    def __init__(self, config, torch_dtype):
         super().__init__(config)
 
         self.controlnet_units = []
         for name, unit in self.config["controlnet_units"].items():
-            cn_unit = ControlNetModel.from_pretrained(unit["model"])
+            cn_unit = ControlNetModel.from_pretrained(unit["model"], torch_dtype=torch_dtype)
             self.controlnet_units.append(cn_unit)
+        if len(self.controlnet_units) == 1:
+            self.controlnet_units = self.controlnet_units[0]
             
         if self.config["global"]["mode"] == "txt2img":  
             self.pipeline = StableDiffusionControlNetPipeline.from_pretrained(
                 self.config["global"]["model_name_or_path"],
                 controlnet=self.controlnet_units,
+                torch_dtype=torch_dtype,
             )
         
         if self.config["global"]["mode"] == "img2img":
             self.pipeline = StableDiffusionControlNetImg2ImgPipeline.from_pretrained(
                 self.config["global"]["model_name_or_path"],
                 controlnet=self.controlnet_units,
+                torch_dtype=torch_dtype,
             )
         self.pipeline.enable_xformers_memory_efficient_attention()
         self.pipeline = self.pipeline.to("cuda")
 
 
     def generate_sd_qrcode(
         self,
@@ -98,14 +102,25 @@
             self.pipeline.scheduler.config,
         )
         
         seeded_generator = torch.Generator(device="cuda").manual_seed(
             self.config["global"]["seed"]
         ) if self.config["global"]["seed"] != -1 else None
 
+        
+        # fix bug when only one image is provided in the list
+        if len(controlnet_input_images) == 1:
+            controlnet_input_images = controlnet_input_images[0]
+        if len(controlnet_weights) == 1:
+            controlnet_weights = controlnet_weights[0]
+        if len(guidance_starts) == 1:
+            guidance_starts = guidance_starts[0]
+        if len(guidance_stops) == 1:
+            guidance_stops = guidance_stops[0]
+            
         if self.config["global"]["mode"] == "txt2img":
             r = self.pipeline(
                 generator=seeded_generator,
                 prompt=self.config["global"]["prompt"],
                 negative_prompt=self.config["global"]["negative_prompt"],
                 width=self.config["global"]["width"],
                 height=self.config["global"]["height"],
```

### Comparing `sdqrcode-0.3.5/src/sdqrcode/configs/default.yaml` & `sdqrcode-0.3.6/src/sdqrcode/configs/default.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.5/src/sdqrcode/configs/default_auto.yaml` & `sdqrcode-0.3.6/src/sdqrcode/configs/brightness_auto.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.5/src/sdqrcode/configs/default_diffusers.yaml` & `sdqrcode-0.3.6/src/sdqrcode/configs/default_diffusers.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.5/src/sdqrcode/configs/img2img_tile_auto.yaml` & `sdqrcode-0.3.6/src/sdqrcode/configs/img2img_tile_auto.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.5/src/sdqrcode/configs/img2img_tile_diffusers.yaml` & `sdqrcode-0.3.6/src/sdqrcode/configs/img2img_tile_diffusers.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.5/src/sdqrcode/sdqrcode.py` & `sdqrcode-0.3.6/src/sdqrcode/sdqrcode.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,23 @@
 import os
 import urllib.request
 from pathlib import Path
 import requests
 from io import BytesIO
 import sdqrcode.Engines.engine_util as engine_util
 from typing import Union
+import torch
 
 CONFIGS = {
-    "default_auto": Path(__file__).parent / "configs" / "default_auto.yaml",
-    "default_diffusers": Path(__file__).parent / "configs" / "default_diffusers.yaml",
-    # Add more configuration files as needed
+    "default_auto":           Path(__file__).parent / "configs" / "default_auto.yaml",
+    "default_diffusers":      Path(__file__).parent / "configs" / "default_diffusers.yaml",
+    "brightness_auto":        Path(__file__).parent / "configs" / "brightness_auto.yaml",
+    "brightness_diffusers":   Path(__file__).parent / "configs" / "brightness_diffusers.yaml",
+    "img2img_tile_auto":      Path(__file__).parent / "configs" / "img2img_tile_auto.yaml",
+    "img2img_tile_diffusers": Path(__file__).parent / "configs" / "img2img_tile_diffusers.yaml",
 }
 
 
 # Backend enum, one of auto_api, diffusers
 class constants:
     AUTO_API = 0
     DIFFUSERS = 1
@@ -28,25 +32,27 @@
         self,
         config_name_or_path_or_dict: str,
         auto_api_hostname: str = None,
         auto_api_port: int = None,
         auto_api_https: bool = None,
         auto_api_username: str = None,
         auto_api_password: str = None,
+        torch_dtype: torch.dtype = torch.float32,
     ):
         """
         Args:
             backend: Backend enum, one of auto_api, diffusers
             model: Model name or path to a pretrained model
             config_name_or_path: Pretrained config name or path if not the same as model_name
             auto_api_hostname: Hostname of the Automatic1111 server
             auto_api_port: Port of the Automatic1111 server (default: 7860)
             auto_api_https: Use HTTPS for the Automatic1111 server
             auto_api_username: Username for the Automatic1111 server (if any)
             auto_api_password: Password for the Automatic1111 server (if any)
+            torch_dtype: (only diffusers) Torch dtype to use for the model (default: torch.float32)
         """
 
         # Load backend
         self.backend = (
             constants.AUTO_API if auto_api_hostname is None else constants.DIFFUSERS
         )
         if config_name_or_path_or_dict is not dict:
@@ -55,14 +61,15 @@
         self.engine = engine_util.init_engine(
             hostname=auto_api_hostname,
             port=auto_api_port,
             https=auto_api_https,
             username=auto_api_username,
             password=auto_api_password,
             config=self.config,
+            torch_dtype=torch_dtype,
         )
 
     def generate_sd_qrcode(
         self,
         qr_img: PIL.Image.Image = None,
         input_image: PIL.Image.Image = None, # for img2img
         controlnet_input_images: list[Union[PIL.Image.Image, str]] = None,
@@ -238,14 +245,15 @@
 def init(
     config: str = "default_diffusers",
     auto_api_hostname: str = None,
     auto_api_port: int = None,
     auto_api_https: bool = None,
     auto_api_username: str = None,
     auto_api_password: str = None,
+    torch_dtype: torch.dtype = torch.float32,
     **config_kwargs,
 ):
     """
     config_kwargs:
         model_name_or_path: str = None,
         steps: int = None,
         cfg_scale: float = None,
@@ -273,24 +281,27 @@
     return Sdqrcode(
         config_name_or_path_or_dict=config,
         auto_api_hostname=auto_api_hostname,
         auto_api_port=auto_api_port,
         auto_api_https=auto_api_https,
         auto_api_username=auto_api_username,
         auto_api_password=auto_api_password,
+        torch_dtype=torch_dtype,
+        
     )
 
 
 def init_and_generate_sd_qrcode(
     config_name_or_path: str = "default_diffusers",
     auto_api_hostname: str = "",
     auto_api_port: int = 7860,
     auto_api_https: bool = True,
     auto_api_username: str = "",
     auto_api_password: str = "",
+    torch_dtype: torch.dtype = torch.float32,
     **config_kwargs,
 ) -> tuple[PIL.Image.Image, Sdqrcode]:
     # check if variables are set in env
     auto_api_hostname = (
         os.getenv("AUTO_API_HOSTNAME", "")
         if auto_api_hostname == ""
         else auto_api_hostname
@@ -315,14 +326,15 @@
     sd_qr_generator = init(
         config=config_name_or_path,
         auto_api_hostname=auto_api_hostname,
         auto_api_port=auto_api_port,
         auto_api_https=auto_api_https,
         auto_api_username=auto_api_username,
         auto_api_password=auto_api_password,
+        torch_dtype=torch_dtype,
         **config_kwargs,
     )
 
     sd_qr_img = sd_qr_generator.generate_sd_qrcode()
 
     return sd_qr_img, sd_qr_generator
```

### Comparing `sdqrcode-0.3.5/PKG-INFO` & `sdqrcode-0.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdqrcode
-Version: 0.3.5
+Version: 0.3.6
 Summary: Generate ai qr codes with stable diffusion and controlnet with standardised methods
 License: MIT
 Author: PhilSad
 Author-email: philippe.henri.saade@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -255,7 +255,13 @@
 - [x] add diffusers backend
 - [ ] add docs
 - [ ] allow to change models
 
 # Contrib
 Please don't hesitate to submit a PR to improve the code or submit a config
 
+# Other projects
+You can checkout [our website](https://koll.ai) to discover more of our projects such as:
+- [Seg2Sat](https://huggingface.co/spaces/rgres/Seg2Sat): Controlnet model to generate aerial pictures 
+- [PoetGPT](https://poetgpt.koll.ai): generate beautiful poems and lyrics with AI 
+- [ThisSCPDoesNotExist](https://thisscpdoesnotexist.ml/): generate custom SCP entities
+
```

