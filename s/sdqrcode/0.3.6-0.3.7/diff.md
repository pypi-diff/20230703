# Comparing `tmp/sdqrcode-0.3.6.tar.gz` & `tmp/sdqrcode-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdqrcode-0.3.6.tar", max compression
+gzip compressed data, was "sdqrcode-0.3.7.tar", max compression
```

## Comparing `sdqrcode-0.3.6.tar` & `sdqrcode-0.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-07-03 10:27:17.188494 sdqrcode-0.3.6/LICENSE
--rw-r--r--   0        0        0    10567 2023-07-03 10:27:17.188494 sdqrcode-0.3.6/README.md
--rw-r--r--   0        0        0      495 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     3305 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/Engines/AutoEngine.py
--rw-r--r--   0        0        0     8787 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/Engines/DiffusersEngine.py
--rw-r--r--   0        0        0      186 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/Engines/Engine.py
--rw-r--r--   0        0        0      502 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/Engines/engine_util.py
--rw-r--r--   0        0        0       32 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/__init__.py
--rw-r--r--   0        0        0      719 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/brightness_auto.yaml
--rw-r--r--   0        0        0      610 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/brightness_diffusers.yaml
--rw-r--r--   0        0        0       22 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/custom.yaml
--rw-r--r--   0        0        0      737 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/default.yaml
--rw-r--r--   0        0        0      719 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/default_auto.yaml
--rw-r--r--   0        0        0      777 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/default_diffusers.yaml
--rw-r--r--   0        0        0      624 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/img2img_tile_auto.yaml
--rw-r--r--   0        0        0      644 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/configs/img2img_tile_diffusers.yaml
--rw-r--r--   0        0        0    13545 2023-07-03 10:27:17.252494 sdqrcode-0.3.6/src/sdqrcode/sdqrcode.py
--rw-r--r--   0        0        0    11400 1970-01-01 00:00:00.000000 sdqrcode-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-03 15:33:07.035703 sdqrcode-0.3.7/LICENSE
+-rw-r--r--   0        0        0    10681 2023-07-03 15:33:07.039704 sdqrcode-0.3.7/README.md
+-rw-r--r--   0        0        0      659 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     3305 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/Engines/AutoEngine.py
+-rw-r--r--   0        0        0     8787 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/Engines/DiffusersEngine.py
+-rw-r--r--   0        0        0      186 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/Engines/Engine.py
+-rw-r--r--   0        0        0      502 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/Engines/engine_util.py
+-rw-r--r--   0        0        0       32 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/__init__.py
+-rw-r--r--   0        0        0      719 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/brightness_auto.yaml
+-rw-r--r--   0        0        0      610 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/brightness_diffusers.yaml
+-rw-r--r--   0        0        0       22 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/custom.yaml
+-rw-r--r--   0        0        0      737 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/default.yaml
+-rw-r--r--   0        0        0      719 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/default_auto.yaml
+-rw-r--r--   0        0        0      777 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/default_diffusers.yaml
+-rw-r--r--   0        0        0      624 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/img2img_tile_auto.yaml
+-rw-r--r--   0        0        0      644 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/configs/img2img_tile_diffusers.yaml
+-rw-r--r--   0        0        0    13545 2023-07-03 15:33:07.111708 sdqrcode-0.3.7/src/sdqrcode/sdqrcode.py
+-rw-r--r--   0        0        0    11593 1970-01-01 00:00:00.000000 sdqrcode-0.3.7/PKG-INFO
```

### Comparing `sdqrcode-0.3.6/LICENSE` & `sdqrcode-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.6/README.md` & `sdqrcode-0.3.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,19 @@
 click to expand, cherry picked, will add more results later
 
 | ![Dalmatian qrcode](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/a33a7ae9-3842-4290-b5b2-0104f5339323) | ![Swimming pool girl qrcode](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/435d4a3c-5eca-498e-a8bd-47d2658e6305) |
 | --------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
 
 # Install
 ```
-pip install sdqrcode
-pip install git+https://github.com/huggingface/diffusers
+pip install sdqrcode # Automatic1111 engine
+#or
+pip install sdqrcode[diffusers] # Diffusers engine
+
+pip install git+https://github.com/huggingface/diffusers # require dev version of diffusers
 ```
 # Usage Diffusers
 
 ```python
 import sdqrcode
 # init with a default config
 generator = sdqrcode.init(config = "default_diffusers")
```

### Comparing `sdqrcode-0.3.6/src/sdqrcode/Engines/AutoEngine.py` & `sdqrcode-0.3.7/src/sdqrcode/Engines/AutoEngine.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.6/src/sdqrcode/Engines/DiffusersEngine.py` & `sdqrcode-0.3.7/src/sdqrcode/Engines/DiffusersEngine.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.6/src/sdqrcode/configs/brightness_auto.yaml` & `sdqrcode-0.3.7/src/sdqrcode/configs/brightness_auto.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.6/src/sdqrcode/configs/brightness_diffusers.yaml` & `sdqrcode-0.3.7/src/sdqrcode/configs/brightness_diffusers.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.6/src/sdqrcode/configs/default.yaml` & `sdqrcode-0.3.7/src/sdqrcode/configs/default.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.6/src/sdqrcode/configs/default_auto.yaml` & `sdqrcode-0.3.7/src/sdqrcode/configs/default_auto.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.6/src/sdqrcode/configs/default_diffusers.yaml` & `sdqrcode-0.3.7/src/sdqrcode/configs/default_diffusers.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.6/src/sdqrcode/configs/img2img_tile_auto.yaml` & `sdqrcode-0.3.7/src/sdqrcode/configs/img2img_tile_auto.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.6/src/sdqrcode/configs/img2img_tile_diffusers.yaml` & `sdqrcode-0.3.7/src/sdqrcode/configs/img2img_tile_diffusers.yaml`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.6/src/sdqrcode/sdqrcode.py` & `sdqrcode-0.3.7/src/sdqrcode/sdqrcode.py`

 * *Files identical despite different names*

### Comparing `sdqrcode-0.3.6/PKG-INFO` & `sdqrcode-0.3.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: sdqrcode
-Version: 0.3.6
+Version: 0.3.7
 Summary: Generate ai qr codes with stable diffusion and controlnet with standardised methods
 License: MIT
 Author: PhilSad
 Author-email: philippe.henri.saade@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: diffusers
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: accelerate (>=0.20.0,<0.21.0)
+Requires-Dist: accelerate (==0.20.0) ; extra == "diffusers"
 Requires-Dist: qrcode (>=7.4.1,<8.0.0)
-Requires-Dist: transformers (==4.30.0)
+Requires-Dist: transformers (==4.30.0) ; extra == "diffusers"
 Requires-Dist: webuiapi (>=0.9.3,<0.10.0)
-Requires-Dist: xformers (>=0.0.20,<0.0.21)
+Requires-Dist: xformers (==0.0.20) ; extra == "diffusers"
 Description-Content-Type: text/markdown
 
 
 # Stable Diffusion QR Code
 alpha version, expect breaking changes
 
 call diffusers pipeline or [Automatic1111 webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) api to generate qrcodes.
@@ -62,16 +63,19 @@
 click to expand, cherry picked, will add more results later
 
 | ![Dalmatian qrcode](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/a33a7ae9-3842-4290-b5b2-0104f5339323) | ![Swimming pool girl qrcode](https://github.com/koll-ai/stable-difusion-qrcode/assets/22277706/435d4a3c-5eca-498e-a8bd-47d2658e6305) |
 | --------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
 
 # Install
 ```
-pip install sdqrcode
-pip install git+https://github.com/huggingface/diffusers
+pip install sdqrcode # Automatic1111 engine
+#or
+pip install sdqrcode[diffusers] # Diffusers engine
+
+pip install git+https://github.com/huggingface/diffusers # require dev version of diffusers
 ```
 # Usage Diffusers
 
 ```python
 import sdqrcode
 # init with a default config
 generator = sdqrcode.init(config = "default_diffusers")
```

