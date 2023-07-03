# Comparing `tmp/flaxsr-0.0.6.tar.gz` & `tmp/flaxsr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaxsr-0.0.6.tar", last modified: Sat Jun  3 08:57:01 2023, max compression
+gzip compressed data, was "flaxsr-0.0.7.tar", last modified: Mon Jul  3 10:03:35 2023, max compression
```

## Comparing `flaxsr-0.0.6.tar` & `flaxsr-0.0.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-03 08:57:01.268914 flaxsr-0.0.6/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)    11313 2023-05-12 09:22:40.000000 flaxsr-0.0.6/LICENSE
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2800 2023-06-03 08:57:01.268914 flaxsr-0.0.6/PKG-INFO
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2176 2023-06-03 08:09:59.000000 flaxsr-0.0.6/README.md
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-03 08:57:01.264914 flaxsr-0.0.6/flaxsr/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      111 2023-05-17 15:18:45.000000 flaxsr-0.0.6/flaxsr/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      661 2023-05-12 10:02:07.000000 flaxsr-0.0.6/flaxsr/_utils.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-03 08:57:01.268914 flaxsr-0.0.6/flaxsr/layers/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      179 2023-05-12 09:22:40.000000 flaxsr-0.0.6/flaxsr/layers/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1651 2023-05-16 13:28:13.000000 flaxsr-0.0.6/flaxsr/layers/stochastic.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1673 2023-05-16 13:28:27.000000 flaxsr-0.0.6/flaxsr/layers/upscale.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-03 08:57:01.268914 flaxsr-0.0.6/flaxsr/losses/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1647 2023-06-03 08:08:49.000000 flaxsr-0.0.6/flaxsr/losses/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4806 2023-06-03 04:02:44.000000 flaxsr-0.0.6/flaxsr/losses/adversarial_losses.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2506 2023-06-03 03:59:09.000000 flaxsr-0.0.6/flaxsr/losses/perceptual_losses.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2230 2023-06-03 03:58:37.000000 flaxsr-0.0.6/flaxsr/losses/pixel_wise_losses.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     6448 2023-06-03 08:48:01.000000 flaxsr-0.0.6/flaxsr/losses/regularization_losses.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     3321 2023-06-03 08:38:58.000000 flaxsr-0.0.6/flaxsr/losses/utils.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-03 08:57:01.268914 flaxsr-0.0.6/flaxsr/models/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      392 2023-06-02 11:31:44.000000 flaxsr-0.0.6/flaxsr/models/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     3749 2023-05-12 09:48:06.000000 flaxsr-0.0.6/flaxsr/models/edsr.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      922 2023-05-12 09:48:06.000000 flaxsr-0.0.6/flaxsr/models/espcn.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1138 2023-05-12 09:48:06.000000 flaxsr-0.0.6/flaxsr/models/fsrcnn.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     6677 2023-05-12 09:48:06.000000 flaxsr-0.0.6/flaxsr/models/nafssr.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      994 2023-05-12 09:48:06.000000 flaxsr-0.0.6/flaxsr/models/ncnet.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1078 2023-05-12 09:49:43.000000 flaxsr-0.0.6/flaxsr/models/srcnn.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4161 2023-06-02 11:35:45.000000 flaxsr-0.0.6/flaxsr/models/srgan.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      954 2023-05-12 09:50:48.000000 flaxsr-0.0.6/flaxsr/models/vdsr.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-03 08:57:01.268914 flaxsr-0.0.6/flaxsr/training/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      149 2023-06-01 05:21:42.000000 flaxsr-0.0.6/flaxsr/training/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      503 2023-06-01 00:48:20.000000 flaxsr-0.0.6/flaxsr/training/train_states.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1345 2023-06-03 08:06:45.000000 flaxsr-0.0.6/flaxsr/training/train_step.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-03 08:57:01.268914 flaxsr-0.0.6/flaxsr.egg-info/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2800 2023-06-03 08:57:01.000000 flaxsr-0.0.6/flaxsr.egg-info/PKG-INFO
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      784 2023-06-03 08:57:01.000000 flaxsr-0.0.6/flaxsr.egg-info/SOURCES.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)        1 2023-06-03 08:57:01.000000 flaxsr-0.0.6/flaxsr.egg-info/dependency_links.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)       46 2023-06-03 08:57:01.000000 flaxsr-0.0.6/flaxsr.egg-info/requires.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)        7 2023-06-03 08:57:01.000000 flaxsr-0.0.6/flaxsr.egg-info/top_level.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)       38 2023-06-03 08:57:01.268914 flaxsr-0.0.6/setup.cfg
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      960 2023-06-03 08:56:02.000000 flaxsr-0.0.6/setup.py
+drwxrwxr-x   0 dslisleedh  (1001) dslisleedh  (1001)        0 2023-07-03 10:03:35.828839 flaxsr-0.0.7/
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)    11313 2023-07-03 08:32:18.000000 flaxsr-0.0.7/LICENSE
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     2962 2023-07-03 10:03:35.828839 flaxsr-0.0.7/PKG-INFO
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     2339 2023-07-03 08:32:18.000000 flaxsr-0.0.7/README.md
+drwxrwxr-x   0 dslisleedh  (1001) dslisleedh  (1001)        0 2023-07-03 10:03:35.824839 flaxsr-0.0.7/flaxsr/
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)      162 2023-07-03 09:55:56.000000 flaxsr-0.0.7/flaxsr/__init__.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)      661 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/_utils.py
+drwxrwxr-x   0 dslisleedh  (1001) dslisleedh  (1001)        0 2023-07-03 10:03:35.824839 flaxsr-0.0.7/flaxsr/layers/
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)      179 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/layers/__init__.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     1651 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/layers/stochastic.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     1673 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/layers/upscale.py
+drwxrwxr-x   0 dslisleedh  (1001) dslisleedh  (1001)        0 2023-07-03 10:03:35.824839 flaxsr-0.0.7/flaxsr/losses/
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     1647 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/losses/__init__.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     4890 2023-07-03 08:49:00.000000 flaxsr-0.0.7/flaxsr/losses/adversarial_losses.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     2506 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/losses/perceptual_losses.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     2230 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/losses/pixel_wise_losses.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     6448 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/losses/regularization_losses.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     3478 2023-07-03 08:36:57.000000 flaxsr-0.0.7/flaxsr/losses/utils.py
+drwxrwxr-x   0 dslisleedh  (1001) dslisleedh  (1001)        0 2023-07-03 10:03:35.828839 flaxsr-0.0.7/flaxsr/models/
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)      392 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/models/__init__.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     3749 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/models/edsr.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)      922 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/models/espcn.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     1138 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/models/fsrcnn.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     6677 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/models/nafssr.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)      994 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/models/ncnet.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     1078 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/models/srcnn.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     4161 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/models/srgan.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)      954 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/models/vdsr.py
+drwxrwxr-x   0 dslisleedh  (1001) dslisleedh  (1001)        0 2023-07-03 10:03:35.828839 flaxsr-0.0.7/flaxsr/training/
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)      149 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/training/__init__.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)      503 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/training/train_states.py
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     1345 2023-07-03 08:32:18.000000 flaxsr-0.0.7/flaxsr/training/train_step.py
+drwxrwxr-x   0 dslisleedh  (1001) dslisleedh  (1001)        0 2023-07-03 10:03:35.824839 flaxsr-0.0.7/flaxsr.egg-info/
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)     2962 2023-07-03 10:03:35.000000 flaxsr-0.0.7/flaxsr.egg-info/PKG-INFO
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)      784 2023-07-03 10:03:35.000000 flaxsr-0.0.7/flaxsr.egg-info/SOURCES.txt
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)        1 2023-07-03 10:03:35.000000 flaxsr-0.0.7/flaxsr.egg-info/dependency_links.txt
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)       51 2023-07-03 10:03:35.000000 flaxsr-0.0.7/flaxsr.egg-info/requires.txt
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)        7 2023-07-03 10:03:35.000000 flaxsr-0.0.7/flaxsr.egg-info/top_level.txt
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)       38 2023-07-03 10:03:35.828839 flaxsr-0.0.7/setup.cfg
+-rw-rw-r--   0 dslisleedh  (1001) dslisleedh  (1001)      976 2023-07-03 09:55:13.000000 flaxsr-0.0.7/setup.py
```

### Comparing `flaxsr-0.0.6/LICENSE` & `flaxsr-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/PKG-INFO` & `flaxsr-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaxsr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Super Resolution tools with Jax/Flax
 Home-page: https://github.com/dslisleedh/FlaxSR
 Author: dslisleedh
 Author-email: dslisleedh@gmail.com
 Project-URL: Bug Tracker, https://github.com/dslisleedh/FlaxSR/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,14 +15,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FlaxSR
 
 Super Resolution models with Jax/Flax
 
+<b>Currently, Flax is using CUDA/CuDNN from wheel, but TensorFlow is using local CUDA/CuDNN, which is causing conflicts. We will fix it as soon as possible.<\b>
+
 ## HOW TO USE
 
 ### Install
 ```shell
 pip install flaxsr
 ```
```

### Comparing `flaxsr-0.0.6/README.md` & `flaxsr-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # FlaxSR
 
 Super Resolution models with Jax/Flax
 
+<b>Currently, Flax is using CUDA/CuDNN from wheel, but TensorFlow is using local CUDA/CuDNN, which is causing conflicts. We will fix it as soon as possible.<\b>
+
 ## HOW TO USE
 
 ### Install
 ```shell
 pip install flaxsr
 ```
 
@@ -79,8 +81,8 @@
    - DropPath: droppath
    - DropPathFast: droppath_fast
    - PixelShuffle: pixelshuffle
    - NearestConv: nearestconv
  
  - train_step
    - discriminative_train_step: discriminative
- 
+
```

### Comparing `flaxsr-0.0.6/flaxsr/_utils.py` & `flaxsr-0.0.7/flaxsr/_utils.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/layers/stochastic.py` & `flaxsr-0.0.7/flaxsr/layers/stochastic.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/layers/upscale.py` & `flaxsr-0.0.7/flaxsr/layers/upscale.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/losses/__init__.py` & `flaxsr-0.0.7/flaxsr/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/losses/adversarial_losses.py` & `flaxsr-0.0.7/flaxsr/losses/adversarial_losses.py`

 * *Files 7% similar despite different names*

```diff
@@ -109,33 +109,37 @@
         super().__init__(reduce)
         self.from_logits = from_logits
 
     def __call__(self, fake: jnp.ndarray, *args, **kwargs):
         return least_square_generator_loss(fake, self.from_logits, self.reduce)
 
 
+def d_ra(x: jnp.ndarray, y: jnp.ndarray) -> jnp.ndarray:
+    return x - jnp.mean(y)
+
+
 @partial(jax.jit, static_argnums=(2,))
 def relativistic_discriminator_loss(
         fake: jnp.ndarray, true: jnp.ndarray, reduce: str | Reduce = 'mean',
         *args, **kwargs
 ):
-    true_loss = -jax.nn.log_sigmoid(true - jnp.mean(fake))
-    fake_loss = -jax.nn.log_sigmoid(-fake + jnp.mean(true))
+    true_loss = -jax.nn.log_sigmoid(d_ra(true, fake))
+    fake_loss = -jnp.log(1. - jax.nn.sigmoid(d_ra(fake, true)))
 
     loss = true_loss + fake_loss
     return reduce_fn(loss, reduce)
 
 
 @partial(jax.jit, static_argnums=(2,))
 def relativistic_generator_loss(
         fake: jnp.ndarray, true: jnp.ndarray, reduce: str | Reduce = 'mean',
         *args, **kwargs
 ):
-    true_loss = -jax.nn.log_sigmoid(-true + jnp.mean(fake))
-    fake_loss = -jax.nn.log_sigmoid(fake - jnp.mean(true))
+    true_loss = -jnp.log(1. - jax.nn.sigmoid(d_ra(true, fake)))
+    fake_loss = -jax.nn.log_sigmoid(d_ra(fake, true))
 
     loss = true_loss + fake_loss
     return reduce_fn(loss, reduce)
 
 
 @register('losses', 'relativistic_discriminator')
 class RelativisticDiscriminatorLoss(Loss):
```

### Comparing `flaxsr-0.0.6/flaxsr/losses/perceptual_losses.py` & `flaxsr-0.0.7/flaxsr/losses/perceptual_losses.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/losses/pixel_wise_losses.py` & `flaxsr-0.0.7/flaxsr/losses/pixel_wise_losses.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/losses/regularization_losses.py` & `flaxsr-0.0.7/flaxsr/losses/regularization_losses.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/losses/utils.py` & `flaxsr-0.0.7/flaxsr/losses/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,19 @@
 def check_vgg_params_exists():
     dir_path = _get_package_dir()
     state = os.path.exists(os.path.join(dir_path, 'vgg19_weights.pkl'))
 
     if not state:
         print('VGG19 weights not found !!!')
         print('Downloading VGG19 weights ...')
+        # To prevent errors when using jax and tensorflow together
+        a = jnp.ones((1,))
+        del a
         import tensorflow as tf
+        tf.config.set_visible_devices([], 'GPU')
         vgg19 = tf.keras.applications.VGG19(include_top=False, weights='imagenet')
         weights = []
         for layer in vgg19.layers:
             if isinstance(layer, tf.keras.layers.Conv2D):
                 weights.append(
                     (
                         jnp.asarray(layer.weights[0].numpy()),
```

### Comparing `flaxsr-0.0.6/flaxsr/models/edsr.py` & `flaxsr-0.0.7/flaxsr/models/edsr.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/models/espcn.py` & `flaxsr-0.0.7/flaxsr/models/espcn.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/models/fsrcnn.py` & `flaxsr-0.0.7/flaxsr/models/fsrcnn.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/models/nafssr.py` & `flaxsr-0.0.7/flaxsr/models/nafssr.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/models/ncnet.py` & `flaxsr-0.0.7/flaxsr/models/ncnet.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/models/srcnn.py` & `flaxsr-0.0.7/flaxsr/models/srcnn.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/models/srgan.py` & `flaxsr-0.0.7/flaxsr/models/srgan.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/models/vdsr.py` & `flaxsr-0.0.7/flaxsr/models/vdsr.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr/training/train_step.py` & `flaxsr-0.0.7/flaxsr/training/train_step.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/flaxsr.egg-info/PKG-INFO` & `flaxsr-0.0.7/flaxsr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaxsr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Super Resolution tools with Jax/Flax
 Home-page: https://github.com/dslisleedh/FlaxSR
 Author: dslisleedh
 Author-email: dslisleedh@gmail.com
 Project-URL: Bug Tracker, https://github.com/dslisleedh/FlaxSR/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,14 +15,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FlaxSR
 
 Super Resolution models with Jax/Flax
 
+<b>Currently, Flax is using CUDA/CuDNN from wheel, but TensorFlow is using local CUDA/CuDNN, which is causing conflicts. We will fix it as soon as possible.<\b>
+
 ## HOW TO USE
 
 ### Install
 ```shell
 pip install flaxsr
 ```
```

### Comparing `flaxsr-0.0.6/flaxsr.egg-info/SOURCES.txt` & `flaxsr-0.0.7/flaxsr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.6/setup.py` & `flaxsr-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="flaxsr",
-    version="0.0.6",
+    version="0.0.7",
     author="dslisleedh",
     author_email="dslisleedh@gmail.com",
     description="Super Resolution tools with Jax/Flax",
     long_description=open('README.md', 'rt').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/dslisleedh/FlaxSR",
     project_urls={
@@ -23,12 +23,13 @@
     install_requires=[
         "jax",
         "jaxlib",
         "flax",
         "einops",
         "tensorflow",
         "numpy",
-        "optax"
+        "optax",
+        "tqdm"
     ],
     packages=setuptools.find_packages(),
     python_requires=">=3.6",
 )
```

