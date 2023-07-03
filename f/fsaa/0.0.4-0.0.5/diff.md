# Comparing `tmp/fsaa-0.0.4.tar.gz` & `tmp/fsaa-0.0.5.tar.gz`

## Comparing `fsaa-0.0.4.tar` & `fsaa-0.0.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fsaa-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fsaa-0.0.4/CITATION.cff
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 fsaa-0.0.4/CODEOWNERS
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fsaa-0.0.4/CONTRIBUTING.md
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 fsaa-0.0.4/environment.yml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fsaa-0.0.4/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fsaa-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fsaa-0.0.4/.vscode/launch.json
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fsaa-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0    22260 2020-02-02 00:00:00.000000 fsaa-0.0.4/assets/logo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/__init__.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/attack.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/core.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/utils.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/examples/tutorial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/initializers/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/initializers/random.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/initializers/random_sign.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/losses/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/losses/cossim_loss.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/losses/lpips_loss.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/losses/mse_loss.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/masks/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/masks/custom.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/masks/jnd.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/masks/nomask.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/models/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/models/dinov2/dinov2.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/models/hf_models/hf_models.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/models/ibot/ibot.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/models/ibot/utils.py
--rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/models/ibot/vits.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/transforms/__init__.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/transforms/compose.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/transforms/normalize.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/updaters/__init__.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/updaters/fgsm.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/updaters/langevin.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/updaters/pgd.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/updaters/random.py
--rw-r--r--   0        0        0   730255 2020-02-02 00:00:00.000000 fsaa-0.0.4/imgs/adv.png
--rw-r--r--   0        0        0   450674 2020-02-02 00:00:00.000000 fsaa-0.0.4/imgs/mask.png
--rw-r--r--   0        0        0   694498 2020-02-02 00:00:00.000000 fsaa-0.0.4/imgs/orig.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fsaa-0.0.4/tests/test_attack.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fsaa-0.0.4/tests/test_initializers.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fsaa-0.0.4/tests/test_masks.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 fsaa-0.0.4/tests/test_models.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fsaa-0.0.4/tests/test_transforms.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fsaa-0.0.4/tests/test_updaters.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 fsaa-0.0.4/.gitignore
--rw-r--r--   0        0        0    19333 2020-02-02 00:00:00.000000 fsaa-0.0.4/LICENSE
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fsaa-0.0.4/README.md
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 fsaa-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 fsaa-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fsaa-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fsaa-0.0.5/CITATION.cff
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 fsaa-0.0.5/CODEOWNERS
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fsaa-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 fsaa-0.0.5/environment.yml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fsaa-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fsaa-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fsaa-0.0.5/.vscode/launch.json
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fsaa-0.0.5/.vscode/settings.json
+-rw-r--r--   0        0        0    22260 2020-02-02 00:00:00.000000 fsaa-0.0.5/assets/logo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/__init__.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/attack.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/core.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/utils.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/examples/tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/initializers/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/initializers/random.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/initializers/random_sign.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/losses/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/losses/cossim_loss.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/losses/lpips_loss.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/losses/mse_loss.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/masks/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/masks/custom.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/masks/jnd.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/masks/nomask.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/models/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/models/dinov2/dinov2.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/models/hf_models/hf_models.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/models/ibot/ibot.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/models/ibot/utils.py
+-rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/models/ibot/vits.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/transforms/__init__.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/transforms/compose.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/transforms/normalize.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/updaters/__init__.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/updaters/fgsm.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/updaters/langevin.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/updaters/pgd.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/updaters/random.py
+-rw-r--r--   0        0        0   730255 2020-02-02 00:00:00.000000 fsaa-0.0.5/imgs/adv.png
+-rw-r--r--   0        0        0   450674 2020-02-02 00:00:00.000000 fsaa-0.0.5/imgs/mask.png
+-rw-r--r--   0        0        0   694498 2020-02-02 00:00:00.000000 fsaa-0.0.5/imgs/orig.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fsaa-0.0.5/tests/test_attack.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fsaa-0.0.5/tests/test_initializers.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fsaa-0.0.5/tests/test_masks.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 fsaa-0.0.5/tests/test_models.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fsaa-0.0.5/tests/test_transforms.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fsaa-0.0.5/tests/test_updaters.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 fsaa-0.0.5/.gitignore
+-rw-r--r--   0        0        0    19333 2020-02-02 00:00:00.000000 fsaa-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fsaa-0.0.5/README.md
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 fsaa-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 fsaa-0.0.5/PKG-INFO
```

### Comparing `fsaa-0.0.4/.pre-commit-config.yaml` & `fsaa-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/environment.yml` & `fsaa-0.0.5/environment.yml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/.github/workflows/python-publish.yml` & `fsaa-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/.vscode/launch.json` & `fsaa-0.0.5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/assets/logo.png` & `fsaa-0.0.5/assets/logo.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/fsaa/attack.py` & `fsaa-0.0.5/fsaa/attack.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/fsaa/core.py` & `fsaa-0.0.5/fsaa/core.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/fsaa/utils.py` & `fsaa-0.0.5/fsaa/utils.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/fsaa/examples/tutorial.py` & `fsaa-0.0.5/fsaa/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/fsaa/losses/lpips_loss.py` & `fsaa-0.0.5/fsaa/losses/lpips_loss.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/fsaa/masks/jnd.py` & `fsaa-0.0.5/fsaa/masks/jnd.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/fsaa/models/dinov2/dinov2.py` & `fsaa-0.0.5/fsaa/models/dinov2/dinov2.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/fsaa/models/hf_models/hf_models.py` & `fsaa-0.0.5/fsaa/models/hf_models/hf_models.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/fsaa/models/ibot/ibot.py` & `fsaa-0.0.5/fsaa/models/ibot/ibot.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/fsaa/models/ibot/utils.py` & `fsaa-0.0.5/fsaa/models/ibot/utils.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/fsaa/models/ibot/vits.py` & `fsaa-0.0.5/fsaa/models/ibot/vits.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/fsaa/transforms/normalize.py` & `fsaa-0.0.5/fsaa/transforms/normalize.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from warnings import warn
 
-import torch
 from torch import Tensor
-
 from torchvision.transforms import Normalize as TorchNormalize
 
 from fsaa.core import DifferentiableTransform
 
 HALF_NORMALIZATION_MEAN = [0.5, 0.5, 0.5]
 HALF_NORMALIZATION_STD = [0.5, 0.5, 0.5]
 
@@ -29,14 +27,11 @@
             mean = IMAGENET_MEAN
             warn("No mean provided for Normalization: using ImageNet mean.")
 
         if std is None:
             std = IMAGENET_STD
             warn("No std provided for Normalization: using ImageNet std.")
 
-        self.register_buffer("norm_mean", mean)
-        self.register_buffer("norm_std", std)
-        self.transform = TorchNormalize(mean, std)
+        self.transform = TorchNormalize(mean=mean, std=std)
 
     def process(self, x: Tensor) -> Tensor:
-        self.transform = self.transform.to(x.device)
         return self.transform(x)
```

### Comparing `fsaa-0.0.4/fsaa/updaters/langevin.py` & `fsaa-0.0.5/fsaa/updaters/langevin.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/fsaa/updaters/pgd.py` & `fsaa-0.0.5/fsaa/updaters/pgd.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/fsaa/updaters/random.py` & `fsaa-0.0.5/fsaa/updaters/random.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/imgs/adv.png` & `fsaa-0.0.5/imgs/adv.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/imgs/mask.png` & `fsaa-0.0.5/imgs/mask.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/imgs/orig.png` & `fsaa-0.0.5/imgs/orig.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/tests/test_attack.py` & `fsaa-0.0.5/tests/test_attack.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/tests/test_initializers.py` & `fsaa-0.0.5/tests/test_initializers.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/tests/test_masks.py` & `fsaa-0.0.5/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/tests/test_models.py` & `fsaa-0.0.5/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/tests/test_updaters.py` & `fsaa-0.0.5/tests/test_updaters.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/.gitignore` & `fsaa-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/LICENSE` & `fsaa-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/README.md` & `fsaa-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.4/PKG-INFO` & `fsaa-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsaa
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple library for adversarial attacks in feature space.
 Project-URL: Homepage, https://github.com/BrianPulfer/fsaa
 Project-URL: Bug Tracker, https://github.com/BrianPulfer/fsaa/issues
 Author-email: Brian Pulfer <brianpulfer95@gmail.com>
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

