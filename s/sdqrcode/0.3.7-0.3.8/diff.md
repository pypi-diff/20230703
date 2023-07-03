# Comparing `tmp/sdqrcode-0.3.7.tar.gz` & `tmp/sdqrcode-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdqrcode-0.3.7.tar", max compression
+gzip compressed data, was "sdqrcode-0.3.8.tar", max compression
```

## Comparing `sdqrcode-0.3.7.tar` & `sdqrcode-0.3.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-07-03 15:33:07.035703 sdqrcode-0.3.7/LICENSE
--rw-r--r--   0        0        0    10681 2023-07-03 15:33:07.039704 sdqrcode-0.3.7/README.md
--rw-r--r--   0        0        0      659 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     3305 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/Engines/AutoEngine.py
--rw-r--r--   0        0        0     8787 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/Engines/DiffusersEngine.py
--rw-r--r--   0        0        0      186 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/Engines/Engine.py
--rw-r--r--   0        0        0      502 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/Engines/engine_util.py
--rw-r--r--   0        0        0       32 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/__init__.py
--rw-r--r--   0        0        0      719 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/brightness_auto.yaml
--rw-r--r--   0        0        0      610 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/brightness_diffusers.yaml
--rw-r--r--   0        0        0       22 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/custom.yaml
--rw-r--r--   0        0        0      737 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/default.yaml
--rw-r--r--   0        0        0      719 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/default_auto.yaml
--rw-r--r--   0        0        0      777 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/default_diffusers.yaml
--rw-r--r--   0        0        0      624 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/img2img_tile_auto.yaml
--rw-r--r--   0        0        0      644 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/img2img_tile_diffusers.yaml
--rw-r--r--   0        0        0    13545 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/sdqrcode.py
--rw-r--r--   0        0        0    11593 1970-01-01 00:00:00.000000 sdqrcode-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-03 16:24:12.660349 sdqrcode-0.3.8/LICENSE
+-rw-r--r--   0        0        0    10777 2023-07-03 16:24:12.660349 sdqrcode-0.3.8/README.md
+-rw-r--r--   0        0        0      659 2023-07-03 16:24:12.724351 sdqrcode-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     3458 2023-07-03 16:24:12.724351 sdqrcode-0.3.8/src/sdqrcode/Engines/AutoEngine.py
+-rw-r--r--   0        0        0     8787 2023-07-03 16:24:12.724351 sdqrcode-0.3.8/src/sdqrcode/Engines/DiffusersEngine.py
+-rw-r--r--   0        0        0      186 2023-07-03 16:24:12.724351 sdqrcode-0.3.8/src/sdqrcode/Engines/Engine.py
+-rw-r--r--   0        0        0      599 2023-07-03 16:24:12.724351 sdqrcode-0.3.8/src/sdqrcode/Engines/engine_util.py
+-rw-r--r--   0        0        0       32 2023-07-03 16:24:12.724351 sdqrcode-0.3.8/src/sdqrcode/__init__.py
+-rw-r--r--   0        0        0      719 2023-07-03 16:24:12.724351 sdqrcode-0.3.8/src/sdqrcode/configs/brightness_auto.yaml
+-rw-r--r--   0        0        0      610 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/configs/brightness_diffusers.yaml
+-rw-r--r--   0        0        0       22 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/configs/custom.yaml
+-rw-r--r--   0        0        0      737 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/configs/default.yaml
+-rw-r--r--   0        0        0      719 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/configs/default_auto.yaml
+-rw-r--r--   0        0        0      777 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/configs/default_diffusers.yaml
+-rw-r--r--   0        0        0      624 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/configs/img2img_tile_auto.yaml
+-rw-r--r--   0        0        0      644 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/configs/img2img_tile_diffusers.yaml
+-rw-r--r--   0        0        0    13545 2023-07-03 16:24:12.728351 sdqrcode-0.3.8/src/sdqrcode/sdqrcode.py
+-rw-r--r--   0        0        0    11689 1970-01-01 00:00:00.000000 sdqrcode-0.3.8/PKG-INFO
```

### Comparing `sdqrcode-0.3.7/LICENSE` & `sdqrcode-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.7/README.md` & `sdqrcode-0.3.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,21 @@
 # get available controlnet modules
 generator.engine.api.controlnet_module_list()
 
 # get available controlnet models
 generator.engine.api.controlnet_model_list()
 
 ```
+
+# Get default configs
+```python
+import sdqrcode
+sdqrcode.CONFIGS()
+```
+
 # Config File
 
 This lib uses a yaml file to describe the qrcode generation process. You can change any parameters to experiment. Exemple:
 ``` yaml
 global:
   mode: txt2img
   prompt: "a beautiful minecraft landscape, lights and shadows"
@@ -164,15 +171,15 @@
 
 * **``global``**
   * ``mode``: txt2img or img2img (str)
   * ``prompt``: the prompt to use (str)
   * ``negative_prompt``: the negative prompt to use (str)
   * ``model_name_or_path``: stable diffusion checkpoint to use (str)
     * for diffusers, you can use the model name or local path
-    * for automatic1111, not implemented yet, it will use the current webui checkpoint
+    * for automatic1111, you should use one of the installed models (see utils methods above to get the list)
   * ``steps``: the number of steps (int)
   * ``scheduler_name``: the scheduler to use (str)
     * ``DDIM``, ``Euler``, ``Euler a``, ``LMS``, ``DPM2 Karras``, ``DPM2 a Karras``, ``Heun``, ``DDPM``, ``UniPC``, ``PNDM``, ``DEI``, ``DPM++ SDE``, ``DPM++ 2S a``, ``DPM++ 2M``, ``DPM++ SDE Karras``, ``DPM++ 2S a Karras``, ``DPM++ 2M Karras``
   * ``cfg_scale``: the cfg scale (float)
   * ``width``: the width of the output image (int)
   * ``height``: the height of the output image (int)
   * ``seed``: the seed to use, -1 for random (int)
```

### Comparing `sdqrcode-0.3.7/pyproject.toml` & `sdqrcode-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdqrcode"
-version = "0.3.7"
+version = "0.3.8"
 description = "Generate ai qr codes with stable diffusion and controlnet with standardised methods"
 authors = ["PhilSad <philippe.henri.saade@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `sdqrcode-0.3.7/src/sdqrcode/Engines/AutoEngine.py` & `sdqrcode-0.3.8/src/sdqrcode/Engines/AutoEngine.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,19 @@
 
     def generate_sd_qrcode(
         self,
         input_image: PIL.Image.Image = None,
         controlnet_input_images: PIL.Image.Image = None,
         return_cn_imgs=False,
     ) -> PIL.Image.Image:
+        
+        # set the model
+        self.api.util_set_model(self.config["global"]["model_name_or_path"])
+        
+        # define controlnet units
         cn_units = []
         for cn_input_img, (name, unit) in zip(
             controlnet_input_images, self.config["controlnet_units"].items()
         ):
             print("unit", unit)
             cn_unit = webuiapi.ControlNetUnit(
                 input_image=cn_input_img,
```

### Comparing `sdqrcode-0.3.7/src/sdqrcode/Engines/DiffusersEngine.py` & `sdqrcode-0.3.8/src/sdqrcode/Engines/DiffusersEngine.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.7/src/sdqrcode/configs/brightness_auto.yaml` & `sdqrcode-0.3.8/src/sdqrcode/configs/brightness_auto.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.7/src/sdqrcode/configs/brightness_diffusers.yaml` & `sdqrcode-0.3.8/src/sdqrcode/configs/brightness_diffusers.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.7/src/sdqrcode/configs/default.yaml` & `sdqrcode-0.3.8/src/sdqrcode/configs/default.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.7/src/sdqrcode/configs/default_auto.yaml` & `sdqrcode-0.3.8/src/sdqrcode/configs/default_auto.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.7/src/sdqrcode/configs/default_diffusers.yaml` & `sdqrcode-0.3.8/src/sdqrcode/configs/default_diffusers.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.7/src/sdqrcode/configs/img2img_tile_auto.yaml` & `sdqrcode-0.3.8/src/sdqrcode/configs/img2img_tile_auto.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.7/src/sdqrcode/configs/img2img_tile_diffusers.yaml` & `sdqrcode-0.3.8/src/sdqrcode/configs/img2img_tile_diffusers.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.7/src/sdqrcode/sdqrcode.py` & `sdqrcode-0.3.8/src/sdqrcode/sdqrcode.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.7/PKG-INFO` & `sdqrcode-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdqrcode
-Version: 0.3.7
+Version: 0.3.8
 Summary: Generate ai qr codes with stable diffusion and controlnet with standardised methods
 License: MIT
 Author: PhilSad
 Author-email: philippe.henri.saade@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -134,14 +134,21 @@
 # get available controlnet modules
 generator.engine.api.controlnet_module_list()
 
 # get available controlnet models
 generator.engine.api.controlnet_model_list()
 
 ```
+
+# Get default configs
+```python
+import sdqrcode
+sdqrcode.CONFIGS()
+```
+
 # Config File
 
 This lib uses a yaml file to describe the qrcode generation process. You can change any parameters to experiment. Exemple:
 ``` yaml
 global:
   mode: txt2img
   prompt: "a beautiful minecraft landscape, lights and shadows"
@@ -187,15 +194,15 @@
 
 * **``global``**
   * ``mode``: txt2img or img2img (str)
   * ``prompt``: the prompt to use (str)
   * ``negative_prompt``: the negative prompt to use (str)
   * ``model_name_or_path``: stable diffusion checkpoint to use (str)
     * for diffusers, you can use the model name or local path
-    * for automatic1111, not implemented yet, it will use the current webui checkpoint
+    * for automatic1111, you should use one of the installed models (see utils methods above to get the list)
   * ``steps``: the number of steps (int)
   * ``scheduler_name``: the scheduler to use (str)
     * ``DDIM``, ``Euler``, ``Euler a``, ``LMS``, ``DPM2 Karras``, ``DPM2 a Karras``, ``Heun``, ``DDPM``, ``UniPC``, ``PNDM``, ``DEI``, ``DPM++ SDE``, ``DPM++ 2S a``, ``DPM++ 2M``, ``DPM++ SDE Karras``, ``DPM++ 2S a Karras``, ``DPM++ 2M Karras``
   * ``cfg_scale``: the cfg scale (float)
   * ``width``: the width of the output image (int)
   * ``height``: the height of the output image (int)
   * ``seed``: the seed to use, -1 for random (int)
```

