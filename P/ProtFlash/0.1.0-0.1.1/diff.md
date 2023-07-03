# Comparing `tmp/ProtFlash-0.1.0.tar.gz` & `tmp/ProtFlash-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProtFlash-0.1.0.tar", last modified: Mon Feb 20 07:47:27 2023, max compression
+gzip compressed data, was "ProtFlash-0.1.1.tar", last modified: Mon Jul  3 13:35:44 2023, max compression
```

## Comparing `ProtFlash-0.1.0.tar` & `ProtFlash-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 07:47:27.939337 ProtFlash-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-20 07:47:17.000000 ProtFlash-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-02-20 07:47:27.939337 ProtFlash-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 07:47:27.935337 ProtFlash-0.1.0/ProtFlash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 07:47:17.000000 ProtFlash-0.1.0/ProtFlash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-02-20 07:47:17.000000 ProtFlash-0.1.0/ProtFlash/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-20 07:47:17.000000 ProtFlash-0.1.0/ProtFlash/pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-02-20 07:47:17.000000 ProtFlash-0.1.0/ProtFlash/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 07:47:27.939337 ProtFlash-0.1.0/ProtFlash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-02-20 07:47:27.000000 ProtFlash-0.1.0/ProtFlash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-20 07:47:27.000000 ProtFlash-0.1.0/ProtFlash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 07:47:27.000000 ProtFlash-0.1.0/ProtFlash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 07:47:27.000000 ProtFlash-0.1.0/ProtFlash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-20 07:47:27.000000 ProtFlash-0.1.0/ProtFlash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-20 07:47:27.000000 ProtFlash-0.1.0/ProtFlash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-20 07:47:17.000000 ProtFlash-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 07:47:27.939337 ProtFlash-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-02-20 07:47:17.000000 ProtFlash-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:35:44.779236 ProtFlash-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 13:35:35.000000 ProtFlash-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-03 13:35:44.779236 ProtFlash-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:35:44.775236 ProtFlash-0.1.1/ProtFlash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:35:35.000000 ProtFlash-0.1.1/ProtFlash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-07-03 13:35:35.000000 ProtFlash-0.1.1/ProtFlash/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-03 13:35:35.000000 ProtFlash-0.1.1/ProtFlash/pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-03 13:35:35.000000 ProtFlash-0.1.1/ProtFlash/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:35:44.779236 ProtFlash-0.1.1/ProtFlash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-03 13:35:44.000000 ProtFlash-0.1.1/ProtFlash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-03 13:35:44.000000 ProtFlash-0.1.1/ProtFlash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:35:44.000000 ProtFlash-0.1.1/ProtFlash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:35:44.000000 ProtFlash-0.1.1/ProtFlash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 13:35:44.000000 ProtFlash-0.1.1/ProtFlash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 13:35:44.000000 ProtFlash-0.1.1/ProtFlash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-03 13:35:35.000000 ProtFlash-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:35:44.779236 ProtFlash-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-03 13:35:35.000000 ProtFlash-0.1.1/setup.py
```

### Comparing `ProtFlash-0.1.0/LICENSE` & `ProtFlash-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ProtFlash-0.1.0/ProtFlash/model.py` & `ProtFlash-0.1.1/ProtFlash/model.py`

 * *Files identical despite different names*

### Comparing `ProtFlash-0.1.0/ProtFlash/pretrain.py` & `ProtFlash-0.1.1/ProtFlash/pretrain.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 """ 
 """
 import torch
 from .model import FLASHTransformer
 from .utils import load_hub_workaround
 
 MODEL_URL_BASE = "https://zenodo.org/record/7655858/files/protflash_large.pt"
+MODEL_URL_SMALL = "https://zenodo.org/record/7655858/files/flash_protein.pt"
 
 
 def load_prot_flash_base():
     model_data = load_hub_workaround(MODEL_URL_BASE)
     # model_data = torch.load("/mnt/d/protein-net/ProtBert/flash_protein.pt", map_location="cpu")
     hyper_parameter = model_data["hyper_parameters"]
     model = FLASHTransformer(hyper_parameter['dim'], hyper_parameter['num_tokens'], hyper_parameter['num_layer'], group_size=hyper_parameter['num_tokens'],
                              query_key_dim=hyper_parameter['qk_dim'], max_rel_dist=hyper_parameter['max_rel_dist'], expansion_factor=hyper_parameter['expansion_factor'])
 
     model.load_state_dict(model_data['state_dict'])
 
     return model
 
+def load_prot_flash_small():
+    model_data = load_hub_workaround(MODEL_URL_SMALL)
+    # model_data = torch.load("/mnt/d/protein-net/ProtBert/flash_protein.pt", map_location="cpu")
+    hyper_parameter = model_data["hyper_parameters"]
+    model = FLASHTransformer(hyper_parameter['dim'], hyper_parameter['num_tokens'], hyper_parameter['num_layers'], group_size=hyper_parameter['num_tokens'],
+                             query_key_dim=hyper_parameter['qk_dim'], max_rel_dist=hyper_parameter['max_rel_dist'], expansion_factor=hyper_parameter['expansion_factor'])
+
+    model.load_state_dict(model_data['state_dict'])
+
+    return model
+
 if __name__ == "__main__":
     model = load_prot_flash_base()
```

### Comparing `ProtFlash-0.1.0/ProtFlash/utils.py` & `ProtFlash-0.1.1/ProtFlash/utils.py`

 * *Files identical despite different names*

### Comparing `ProtFlash-0.1.0/setup.py` & `ProtFlash-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='ProtFlash',
-      version='0.1.0',
+      version='0.1.1',
       description='protein language model',
       long_description=long_description,
       long_description_content_type="text/markdown",
       keywords='protein language model',
       classifiers = [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

