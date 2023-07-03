# Comparing `tmp/napari-stable-diffusion-0.0.1.tar.gz` & `tmp/napari-stable-diffusion-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-stable-diffusion-0.0.1.tar", last modified: Thu Oct 27 21:23:03 2022, max compression
+gzip compressed data, was "napari-stable-diffusion-0.1.1.tar", last modified: Mon Jul  3 16:46:45 2023, max compression
```

## Comparing `napari-stable-diffusion-0.0.1.tar` & `napari-stable-diffusion-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 21:23:03.089047 napari-stable-diffusion-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-10-27 21:22:44.000000 napari-stable-diffusion-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-27 21:22:44.000000 napari-stable-diffusion-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5179 2022-10-27 21:23:03.089047 napari-stable-diffusion-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3889 2022-10-27 21:22:44.000000 napari-stable-diffusion-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-10-27 21:22:44.000000 napari-stable-diffusion-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1798 2022-10-27 21:23:03.089047 napari-stable-diffusion-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 21:23:03.089047 napari-stable-diffusion-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 21:23:03.089047 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-10-27 21:22:44.000000 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 21:23:03.089047 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 21:22:44.000000 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-10-27 21:22:44.000000 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     6080 2022-10-27 21:22:44.000000 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion/_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     6855 2022-10-27 21:22:44.000000 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion/_widget_img2img.py
--rw-r--r--   0 runner    (1001) docker     (121)     7424 2022-10-27 21:22:44.000000 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion/_widget_inpaint.py
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-10-27 21:22:44.000000 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 21:23:03.089047 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5179 2022-10-27 21:23:03.000000 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-10-27 21:23:03.000000 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 21:23:03.000000 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-27 21:23:03.000000 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-10-27 21:23:03.000000 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-27 21:23:03.000000 napari-stable-diffusion-0.0.1/src/napari_stable_diffusion.egg-info/top_level.txt
+drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-07-03 16:46:45.073327 napari-stable-diffusion-0.1.1/
+-rw-r--r--   0 kharrington   (503) staff       (20)     1490 2023-03-16 14:58:55.000000 napari-stable-diffusion-0.1.1/LICENSE
+-rw-r--r--   0 kharrington   (503) staff       (20)       96 2023-03-16 14:58:55.000000 napari-stable-diffusion-0.1.1/MANIFEST.in
+-rw-r--r--   0 kharrington   (503) staff       (20)     5237 2023-07-03 16:46:45.073397 napari-stable-diffusion-0.1.1/PKG-INFO
+-rw-r--r--   0 kharrington   (503) staff       (20)     3947 2023-07-03 13:45:00.000000 napari-stable-diffusion-0.1.1/README.md
+-rw-r--r--   0 kharrington   (503) staff       (20)      180 2023-03-16 14:58:55.000000 napari-stable-diffusion-0.1.1/pyproject.toml
+-rw-r--r--   0 kharrington   (503) staff       (20)     1798 2023-07-03 16:46:45.073758 napari-stable-diffusion-0.1.1/setup.cfg
+drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-07-03 16:46:45.069149 napari-stable-diffusion-0.1.1/src/
+drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-07-03 16:46:45.071595 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/
+-rw-r--r--   0 kharrington   (503) staff       (20)      297 2023-07-03 16:20:21.000000 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/__init__.py
+drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-07-03 16:46:45.072975 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/_tests/
+-rw-r--r--   0 kharrington   (503) staff       (20)        0 2023-03-16 14:58:55.000000 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/_tests/__init__.py
+-rw-r--r--   0 kharrington   (503) staff       (20)     1307 2023-03-16 14:58:55.000000 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/_tests/test_widget.py
+-rw-r--r--   0 kharrington   (503) staff       (20)     6299 2023-07-03 16:45:18.000000 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/_widget.py
+-rw-r--r--   0 kharrington   (503) staff       (20)     6963 2023-07-03 16:42:41.000000 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/_widget_img2img.py
+-rw-r--r--   0 kharrington   (503) staff       (20)     7650 2023-07-03 16:42:30.000000 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/_widget_inpaint.py
+-rw-r--r--   0 kharrington   (503) staff       (20)      943 2023-03-16 14:58:55.000000 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/napari.yaml
+-rw-r--r--   0 kharrington   (503) staff       (20)       78 2023-07-03 13:47:40.000000 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/utils.py
+drwxr-xr-x   0 kharrington   (503) staff       (20)        0 2023-07-03 16:46:45.072636 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion.egg-info/
+-rw-r--r--   0 kharrington   (503) staff       (20)     5237 2023-07-03 16:46:45.000000 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion.egg-info/PKG-INFO
+-rw-r--r--   0 kharrington   (503) staff       (20)      709 2023-07-03 16:46:45.000000 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion.egg-info/SOURCES.txt
+-rw-r--r--   0 kharrington   (503) staff       (20)        1 2023-07-03 16:46:45.000000 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion.egg-info/dependency_links.txt
+-rw-r--r--   0 kharrington   (503) staff       (20)       80 2023-07-03 16:46:45.000000 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion.egg-info/entry_points.txt
+-rw-r--r--   0 kharrington   (503) staff       (20)      140 2023-07-03 16:46:45.000000 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion.egg-info/requires.txt
+-rw-r--r--   0 kharrington   (503) staff       (20)       24 2023-07-03 16:46:45.000000 napari-stable-diffusion-0.1.1/src/napari_stable_diffusion.egg-info/top_level.txt
```

### Comparing `napari-stable-diffusion-0.0.1/LICENSE` & `napari-stable-diffusion-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-stable-diffusion-0.0.1/PKG-INFO` & `napari-stable-diffusion-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stable-diffusion
-Version: 0.0.1
+Version: 0.1.1
 Summary: A demo of stable diffusion in napari
 Home-page: https://github.com/kephale/napari-stable-diffusion
 Author: Kyle Harrington
 Author-email: napari@kyleharrington.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/kephale/napari-stable-diffusion/issues
 Project-URL: Documentation, https://github.com/kephale/napari-stable-diffusion#README.md
@@ -38,15 +38,15 @@
 
 A demo of stable diffusion in napari.
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
-![demo image of napari-stable-diffusion of the prompt "a unicorn and a dinosaur eating cookies and drinking tea"](./napari_stable_diffusion_demo.png)
+![demo image of napari-stable-diffusion of the prompt "a unicorn and a dinosaur eating cookies and drinking tea"](https://github.com/kephale/napari-stable-diffusion/raw/main/napari_stable_diffusion_demo.png)
 
 <!--
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
 
 and review the napari docs for plugin developers:
 https://napari.org/stable/plugins/index.html
```

### Comparing `napari-stable-diffusion-0.0.1/README.md` & `napari-stable-diffusion-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 A demo of stable diffusion in napari.
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
-![demo image of napari-stable-diffusion of the prompt "a unicorn and a dinosaur eating cookies and drinking tea"](./napari_stable_diffusion_demo.png)
+![demo image of napari-stable-diffusion of the prompt "a unicorn and a dinosaur eating cookies and drinking tea"](https://github.com/kephale/napari-stable-diffusion/raw/main/napari_stable_diffusion_demo.png)
 
 <!--
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
 
 and review the napari docs for plugin developers:
 https://napari.org/stable/plugins/index.html
```

### Comparing `napari-stable-diffusion-0.0.1/setup.cfg` & `napari-stable-diffusion-0.1.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-stable-diffusion
-version = 0.0.1
+version = 0.1.1
 description = A demo of stable diffusion in napari
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kephale/napari-stable-diffusion
 author = Kyle Harrington
 author_email = napari@kyleharrington.com
 license = BSD-3-Clause
```

### Comparing `napari-stable-diffusion-0.0.1/src/napari_stable_diffusion/_tests/test_widget.py` & `napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-stable-diffusion-0.0.1/src/napari_stable_diffusion/_widget.py` & `napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,39 +5,37 @@
 see: https://napari.org/stable/plugins/guides.html?#widgets
 
 Replace code below according to your needs.
 """
 from typing import TYPE_CHECKING
 
 from qtpy.QtWidgets import (
-    QHBoxLayout,
     QPushButton,
     QWidget,
     QComboBox,
-    QLineEdit,
     QSpinBox,
     QCheckBox,
     QVBoxLayout,
     QLabel,
     QPlainTextEdit,
 )
 
 import numpy as np
 
 import os
 
 import torch
 from diffusers import StableDiffusionPipeline
 
-# from diffusers import StableDiffusionImg2ImgPipeline
-
 if TYPE_CHECKING:
     import napari
 
-from napari.qt.threading import thread_worker, create_worker
+from napari.qt.threading import thread_worker
+
+from napari_stable_diffusion.utils import get_stable_diffusion_model
 
 
 class StableDiffusionWidget(QWidget):
     def __init__(self, napari_viewer):
         super().__init__()
         self.viewer = napari_viewer
 
@@ -94,14 +92,16 @@
         self.setLayout(QVBoxLayout())
 
         label = QLabel(self)
         label.setText("Prompt")
         self.layout().addWidget(label)
         self.layout().addWidget(self.prompt_textbox)
 
+        # negative prompt: ugly, disfigured, low quality, blurry, nsfw
+
         label = QLabel(self)
         label.setText("Number of images")
         self.layout().addWidget(label)
         self.layout().addWidget(self.gallery_size)
 
         label = QLabel(self)
         label.setText("Number of inference steps")
@@ -135,16 +135,29 @@
         # self.generate_images_batch()
 
         # worker = create_worker(self.generate_images_sequential)
         # worker.start()
 
         # TODO: Notify the user that things are processing
 
-        self.generate_images_sequential()
+        worker = self.generate_images_sequential()
+
+        def yield_catcher(payload):
+            array, title = payload
+
+            self.viewer.add_image(array, name=title, rgb=True)
 
+            # Show gallery as grid
+            self.viewer.grid.enabled = True
+
+        worker.yielded.connect(yield_catcher)
+
+        worker.start()
+
+    @thread_worker
     def generate_images_sequential(self):
         prompt = self.prompt_textbox.document().toPlainText()
         print(f"Prompt is {prompt}")
 
         # Get the device: cpu or gpu
         device = self.device_list.currentText()
 
@@ -160,15 +173,15 @@
         in_channels = 3
         height = self.height_input.value()
         width = self.width_input.value()
         latents_shape = (batch_size, in_channels, height // 8, width // 8)
 
         # Load the pipeline
         pipe = StableDiffusionPipeline.from_pretrained(
-            "CompVis/stable-diffusion-v1-4",
+            get_stable_diffusion_model(),
             use_auth_token=MY_SECRET_TOKEN,
             height=height,
             width=width,
             num_inference_steps=self.num_inference_steps.value(),
         )
         pipe.to(device)
 
@@ -195,13 +208,8 @@
             if image_list["nsfw_content_detected"][0]:
                 array = np.zeros_like(array)
 
             # Empty GPU cache as we generate images
             if torch.cuda.is_available():
                 torch.cuda.empty_cache()
 
-            self.viewer.add_image(
-                array, name=f"nsd_{prompt}-{gallery_id}", rgb=True
-            )
-
-        # Show gallery as grid
-        self.viewer.grid.enabled = True
+            yield (array, f"nsd_{prompt}-{gallery_id}")
```

### Comparing `napari-stable-diffusion-0.0.1/src/napari_stable_diffusion/_widget_img2img.py` & `napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/_widget_img2img.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,18 @@
 This module is an example of a barebones QWidget plugin for napari
 
 It implements the Widget specification.
 see: https://napari.org/stable/plugins/guides.html?#widgets
 
 Replace code below according to your needs.
 """
-from typing import TYPE_CHECKING
-
 from qtpy.QtWidgets import (
-    QHBoxLayout,
     QPushButton,
     QWidget,
     QComboBox,
-    QLineEdit,
     QSpinBox,
     QCheckBox,
     QVBoxLayout,
     QLabel,
     QPlainTextEdit,
 )
 
@@ -27,19 +23,19 @@
 import numpy as np
 
 import os
 
 import torch
 from diffusers import StableDiffusionImg2ImgPipeline
 
-# from diffusers import StableDiffusionImg2ImgPipeline
-
 import napari
 
-from napari.qt.threading import thread_worker, create_worker
+from napari.qt.threading import thread_worker
+
+from napari_stable_diffusion.utils import get_stable_diffusion_model
 
 
 class StableDiffusionImg2ImgWidget(QWidget):
     def __init__(self, napari_viewer):
         super().__init__()
         self.viewer = napari_viewer
 
@@ -140,16 +136,29 @@
         # self.generate_images_batch()
 
         # worker = create_worker(self.generate_images_sequential)
         # worker.start()
 
         # TODO: Notify the user that things are processing
 
-        self.generate_images_sequential()
+        worker = self.generate_images_sequential()
+
+        def yield_catcher(payload):
+            array, title = payload
+
+            self.viewer.add_image(array, name=title, rgb=True)
 
+            # Show gallery as grid
+            self.viewer.grid.enabled = True
+
+        worker.yielded.connect(yield_catcher)
+
+        worker.start()
+
+    @thread_worker
     def generate_images_sequential(self):
         prompt = self.prompt_textbox.document().toPlainText()
         print(f"Prompt is {prompt}")
 
         # Get the device: cpu or gpu
         device = self.device_list.currentText()
 
@@ -165,15 +174,15 @@
         in_channels = 3
         height = self.height_input.value()
         width = self.width_input.value()
         latents_shape = (batch_size, in_channels, height // 8, width // 8)
 
         # Load the pipeline
         pipe = StableDiffusionImg2ImgPipeline.from_pretrained(
-            "CompVis/stable-diffusion-v1-4",
+            get_stable_diffusion_model(),
             use_auth_token=MY_SECRET_TOKEN,
             height=height,
             width=width,
             num_inference_steps=self.num_inference_steps.value(),
         )
         pipe.to(device)
 
@@ -202,28 +211,23 @@
             )
             pipe.latents = latents
             pipe.to(device)
 
             # TODO add strength and guidance_scale to GUI
             image_list = pipe(
                 prompt=[prompt],
-                init_image=init_image,
+                image=init_image,
                 strength=0.75,
                 guidance_scale=7.5,
             )
 
             array = np.array(image_list.images[0])
 
             # If NSFW, then zero over image
             if image_list["nsfw_content_detected"][0]:
                 array = np.zeros_like(array)
 
             # Empty GPU cache as we generate images
             if torch.cuda.is_available():
                 torch.cuda.empty_cache()
 
-            self.viewer.add_image(
-                array, name=f"nsd_{prompt}-{gallery_id}", rgb=True
-            )
-
-        # Show gallery as grid
-        self.viewer.grid.enabled = True
+            yield (array, f"nsd_{prompt}-{gallery_id}")
```

### Comparing `napari-stable-diffusion-0.0.1/src/napari_stable_diffusion/_widget_inpaint.py` & `napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/_widget_inpaint.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,18 @@
 This module is an example of a barebones QWidget plugin for napari
 
 It implements the Widget specification.
 see: https://napari.org/stable/plugins/guides.html?#widgets
 
 Replace code below according to your needs.
 """
-from typing import TYPE_CHECKING
-
 from qtpy.QtWidgets import (
-    QHBoxLayout,
     QPushButton,
     QWidget,
     QComboBox,
-    QLineEdit,
     QSpinBox,
     QCheckBox,
     QVBoxLayout,
     QLabel,
     QPlainTextEdit,
 )
 
@@ -29,14 +25,17 @@
 import os
 
 import torch
 from diffusers import StableDiffusionInpaintPipeline
 
 import napari
 
+from napari.qt.threading import thread_worker
+
+from napari_stable_diffusion.utils import get_stable_diffusion_model
 
 class StableDiffusionInpaintWidget(QWidget):
     def __init__(self, napari_viewer):
         super().__init__()
         self.viewer = napari_viewer
 
         # Textbox for entering prompt
@@ -142,17 +141,30 @@
         # Has issues on mps and small GPUs
         # self.generate_images_batch()
 
         # worker = create_worker(self.generate_images_sequential)
         # worker.start()
 
         # TODO: Notify the user that things are processing
+ 
+        worker = self.generate_images_sequential()
+
+        def yield_catcher(payload):
+            array, title = payload
+
+            self.viewer.add_image(array, name=title, rgb=True)
 
-        self.generate_images_sequential()
+            # Show gallery as grid
+            self.viewer.grid.enabled = True
 
+        worker.yielded.connect(yield_catcher)
+
+        worker.start()
+
+    @thread_worker
     def generate_images_sequential(self):
         prompt = self.prompt_textbox.document().toPlainText()
         print(f"Prompt is {prompt}")
 
         # Get the device: cpu or gpu
         device = self.device_list.currentText()
 
@@ -168,15 +180,15 @@
         in_channels = 3
         height = self.height_input.value()
         width = self.width_input.value()
         latents_shape = (batch_size, in_channels, height // 8, width // 8)
 
         # Load the pipeline
         pipe = StableDiffusionInpaintPipeline.from_pretrained(
-            "CompVis/stable-diffusion-v1-4",
+            get_stable_diffusion_model(),
             use_auth_token=MY_SECRET_TOKEN,
             height=height,
             width=width,
             num_inference_steps=self.num_inference_steps.value(),
         )
         pipe.to(device)
 
@@ -214,15 +226,15 @@
             )
             pipe.latents = latents
             pipe.to(device)
 
             # TODO add strength and guidance_scale to GUI
             image_list = pipe(
                 prompt=[prompt],
-                init_image=init_image,
+                image=init_image,
                 mask_image=mask,
                 strength=0.75,
                 guidance_scale=7.5,
             )
 
             # This is the SD output
             array = np.array(image_list.images[0])
@@ -234,13 +246,8 @@
             if image_list["nsfw_content_detected"][0]:
                 array = np.zeros_like(array)
 
             # Empty GPU cache as we generate images
             if torch.cuda.is_available():
                 torch.cuda.empty_cache()
 
-            self.viewer.add_image(
-                array, name=f"nsd_{prompt}-{gallery_id}", rgb=True
-            )
-
-        # Show gallery as grid
-        self.viewer.grid.enabled = True
+            yield (array, f"nsd_{prompt}-{gallery_id}")
```

### Comparing `napari-stable-diffusion-0.0.1/src/napari_stable_diffusion/napari.yaml` & `napari-stable-diffusion-0.1.1/src/napari_stable_diffusion/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-stable-diffusion-0.0.1/src/napari_stable_diffusion.egg-info/PKG-INFO` & `napari-stable-diffusion-0.1.1/src/napari_stable_diffusion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stable-diffusion
-Version: 0.0.1
+Version: 0.1.1
 Summary: A demo of stable diffusion in napari
 Home-page: https://github.com/kephale/napari-stable-diffusion
 Author: Kyle Harrington
 Author-email: napari@kyleharrington.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/kephale/napari-stable-diffusion/issues
 Project-URL: Documentation, https://github.com/kephale/napari-stable-diffusion#README.md
@@ -38,15 +38,15 @@
 
 A demo of stable diffusion in napari.
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
-![demo image of napari-stable-diffusion of the prompt "a unicorn and a dinosaur eating cookies and drinking tea"](./napari_stable_diffusion_demo.png)
+![demo image of napari-stable-diffusion of the prompt "a unicorn and a dinosaur eating cookies and drinking tea"](https://github.com/kephale/napari-stable-diffusion/raw/main/napari_stable_diffusion_demo.png)
 
 <!--
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
 
 and review the napari docs for plugin developers:
 https://napari.org/stable/plugins/index.html
```

### Comparing `napari-stable-diffusion-0.0.1/src/napari_stable_diffusion.egg-info/SOURCES.txt` & `napari-stable-diffusion-0.1.1/src/napari_stable_diffusion.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.cfg
 src/napari_stable_diffusion/__init__.py
 src/napari_stable_diffusion/_widget.py
 src/napari_stable_diffusion/_widget_img2img.py
 src/napari_stable_diffusion/_widget_inpaint.py
 src/napari_stable_diffusion/napari.yaml
+src/napari_stable_diffusion/utils.py
 src/napari_stable_diffusion.egg-info/PKG-INFO
 src/napari_stable_diffusion.egg-info/SOURCES.txt
 src/napari_stable_diffusion.egg-info/dependency_links.txt
 src/napari_stable_diffusion.egg-info/entry_points.txt
 src/napari_stable_diffusion.egg-info/requires.txt
 src/napari_stable_diffusion.egg-info/top_level.txt
 src/napari_stable_diffusion/_tests/__init__.py
```

