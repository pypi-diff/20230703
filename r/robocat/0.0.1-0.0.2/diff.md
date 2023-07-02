# Comparing `tmp/robocat-0.0.1.tar.gz` & `tmp/robocat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocat-0.0.1.tar", last modified: Sun Jul  2 22:35:43 2023, max compression
+gzip compressed data, was "robocat-0.0.2.tar", last modified: Sun Jul  2 22:47:42 2023, max compression
```

## Comparing `robocat-0.0.1.tar` & `robocat-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:35:43.249621 robocat-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-02 22:35:33.000000 robocat-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-02 22:35:43.245622 robocat-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-07-02 22:35:33.000000 robocat-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:35:43.245622 robocat-0.0.1/roboCAT/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-02 22:35:33.000000 robocat-0.0.1/roboCAT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-02 22:35:33.000000 robocat-0.0.1/roboCAT/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-02 22:35:33.000000 robocat-0.0.1/roboCAT/model2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-02 22:35:33.000000 robocat-0.0.1/roboCAT/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-07-02 22:35:33.000000 robocat-0.0.1/roboCAT/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:35:43.245622 robocat-0.0.1/robocat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-02 22:35:43.000000 robocat-0.0.1/robocat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-02 22:35:43.000000 robocat-0.0.1/robocat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:35:43.000000 robocat-0.0.1/robocat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-02 22:35:43.000000 robocat-0.0.1/robocat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 22:35:43.000000 robocat-0.0.1/robocat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 22:35:43.249621 robocat-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-02 22:35:33.000000 robocat-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:47:42.174958 robocat-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-02 22:47:32.000000 robocat-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-02 22:47:42.174958 robocat-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-07-02 22:47:32.000000 robocat-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:47:42.174958 robocat-0.0.2/roboCAT/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-02 22:47:32.000000 robocat-0.0.2/roboCAT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-02 22:47:32.000000 robocat-0.0.2/roboCAT/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-02 22:47:32.000000 robocat-0.0.2/roboCAT/model2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-02 22:47:32.000000 robocat-0.0.2/roboCAT/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-07-02 22:47:32.000000 robocat-0.0.2/roboCAT/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:47:42.174958 robocat-0.0.2/robocat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-02 22:47:42.000000 robocat-0.0.2/robocat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-02 22:47:42.000000 robocat-0.0.2/robocat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:47:42.000000 robocat-0.0.2/robocat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-02 22:47:42.000000 robocat-0.0.2/robocat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 22:47:42.000000 robocat-0.0.2/robocat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 22:47:42.174958 robocat-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-02 22:47:32.000000 robocat-0.0.2/setup.py
```

### Comparing `robocat-0.0.1/LICENSE` & `robocat-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robocat-0.0.1/PKG-INFO` & `robocat-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocat
-Version: 0.0.1
+Version: 0.0.2
 Summary: Robo CAT- Pytorch
 Home-page: https://github.com/kyegomez/RoboCAT
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,robotics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `robocat-0.0.1/README.md` & `robocat-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,44 @@
 
 
 
 # Usage
 There are 2 methods one is by pip `pip install robotcat` and the other is `git clone`
 
 
+## Method1
+* first `python3 -m pip install robocat`
+
+* Then:
+
+```python
+import torch
+from roboCAT import robo_cat
+
+#example usage
+video = torch.randn(2, 3, 6, 224, 224)
+instructions = [
+    'Bring me tthat apple on the table',
+    'Please bring me the butter'
+]
+
+train_logits = robo_cat.forward(video, instructions)
+robo_cat.model.eval()
+eval_logits = robo_cat.forward(video, instructions, cond_scale=3.0)
+```
+
+* Or train:
+
+```python
+from roboCAT import RoboCat_Train
+
+RoboCat_Train()
+
+```
+
 
 # Method 2
 
 * First `git clone` the repository: `git clone https://github.com/kyegomez/RoboCAT.git`
 
 * Then cd `cd RoboCAT` 
 
@@ -71,14 +101,18 @@
 
 The RoboCAT paper presents a self-improving foundation agent for robotic manipulation that addresses the challenges of generalization and transfer learning in the field of robotics. It offers insights into the model architecture, requirements, and experimental findings. The extensive empirical data, evaluation protocols, and comparisons provide valuable contributions to the research community.
 
 # Roadmap
 
 * Functional prototype
 
+* Integrate VQGAN to generate an image when it has not encountered an known environment
+
+` environment observation -> environment familarity rating [0.0-1.0] -> generate data if lower then [0.5] -> finetune -> action`
+
 * Train on massive datasets
 
 * Finetune as specified on paper
 
 * Release as paid API
 
 * Integrate more modalities like hearing, 3d mapping, nerfs, videos, lidar, locomotion, and the whole lot!
```

### Comparing `robocat-0.0.1/roboCAT/model.py` & `robocat-0.0.2/roboCAT/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from models.MechaZilla.models.rt1.robotic_transformer import MaxViT, RT1
+from robocat.models.MechaZilla.models.rt1.robotic_transformer import MaxViT, RT1
 
 class RoboCAT:
     def __init__(self, num_classes, dim_conv_stem, dim, dim_head, depth, window_size, mbconv_expansion_rate,
                  mbconv_shrinkage_rate, dropout, num_actions, rt_depth, heads, rt_dim_head, cond_drop_prob):
         self.vit = MaxViT(
             num_classes=num_classes,
             dim_conv_stem=dim_conv_stem,
```

### Comparing `robocat-0.0.1/roboCAT/model2.py` & `robocat-0.0.2/roboCAT/model2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from models.vqgan.VQGAN import VQGAN_F8_8192
-from models.gato.GATO.gato import GatoConfig, Gato
+from robocat.models.vqgan.VQGAN import VQGAN_F8_8192
+from robocat.models.gato.GATO.gato import GatoConfig, Gato
 import torch
 #
-class RoboCat:
+class RoboCat2:
     def __init__(self, device, vqgan_config=None, gato_config=None):
         self.device = device
         self.vqgan = VQGAN_F8_8192(self.device)
         self.gato_config = gato_config if gato_config else GatoConfig.small()
         self.gato = Gato(self.gato_config)
 
     def collect_and_preprocess_data(self, data_urls):
@@ -32,15 +32,15 @@
             hidden_states = self.gato((input_ids, (encoding, row_pos, col_pos), obs))
             return hidden_states
         except Exception as e:
             print("Error while feeding encoded images to GATO: ", e)
             return None
 
 device = torch.device('cuda:0' if torch.cuda.is_available() else "cpu")
-robocat = RoboCat(device)
+robocat = RoboCat2(device)
 
 data_urls = ["https://images.unsplash.com/photo-1592194996308-7b43878e84a6", 
              "https://images.unsplash.com/photo-1582719508461-905c673771fd"]
 
 preprocessed_data = robocat.collect_and_preprocess_data(data_urls)
 encoded_images = robocat.encode_images(preprocessed_data)
```

### Comparing `robocat-0.0.1/roboCAT/tokenize.py` & `robocat-0.0.2/roboCAT/tokenize.py`

 * *Files identical despite different names*

### Comparing `robocat-0.0.1/roboCAT/train.py` & `robocat-0.0.2/roboCAT/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,17 @@
                           get_linear_schedule_with_warmup, set_seed)
 
 
 # from utils.stable_adamw import StableAdamWUnfused
 from transformers import AutoModelForCausalLM, BitsAndBytesConfig
 
 
-from roboCAT.models.MechaZilla.models.rt1.robotic_transformer import TransformerAttention
-from roboCAT.model import robo_cat
-from roboCAT.utils.stabe_adam import StableAdamWUnfused
+from robocat.models.MechaZilla.models.rt1.robotic_transformer import TransformerAttention
+from robocat.model import robo_cat
+from robocat.utils.stabe_adam import StableAdamWUnfused
 
 ############ SETUP CONFIG
 # import torch.distributed as dist
 
 # dist.init_process_group(backend='nccl', init_method="env://")
 
 ################
```

### Comparing `robocat-0.0.1/robocat.egg-info/PKG-INFO` & `robocat-0.0.2/robocat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocat
-Version: 0.0.1
+Version: 0.0.2
 Summary: Robo CAT- Pytorch
 Home-page: https://github.com/kyegomez/RoboCAT
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,robotics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `robocat-0.0.1/setup.py` & `robocat-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'robocat',
   packages = find_packages(exclude=[]),
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'Robo CAT- Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/RoboCAT',
   keywords = [
@@ -17,14 +17,15 @@
     'attention mechanism',
     'robotics'
   ],
   install_requires=[
     'classifier-free-guidance-pytorch>=0.1.4',
     'einops>=0.6',
     'torch>=1.6',
+    ''
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

