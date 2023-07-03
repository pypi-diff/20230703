# Comparing `tmp/fsaa-0.0.3.tar.gz` & `tmp/fsaa-0.0.4.tar.gz`

## Comparing `fsaa-0.0.3.tar` & `fsaa-0.0.4.tar`

### file list

```diff
@@ -1,53 +1,55 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fsaa-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fsaa-0.0.3/CITATION.cff
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 fsaa-0.0.3/CODEOWNERS
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fsaa-0.0.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 fsaa-0.0.3/environment.yml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fsaa-0.0.3/requirements.txt
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fsaa-0.0.3/.vscode/launch.json
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fsaa-0.0.3/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/__init__.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/attack.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/core.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/utils.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/examples/tutorial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/initializers/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/initializers/random.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/initializers/random_sign.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/losses/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/losses/cossim_loss.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/losses/lpips_loss.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/losses/mse_loss.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/masks/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/masks/custom.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/masks/jnd.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/masks/nomask.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/models/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/models/dinov2/dinov2.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/models/hf_models/hf_models.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/models/ibot/ibot.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/models/ibot/utils.py
--rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/models/ibot/vits.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/transforms/__init__.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/transforms/compose.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/transforms/normalize.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/updaters/__init__.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/updaters/fgsm.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/updaters/langevin.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/updaters/pgd.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fsaa-0.0.3/fsaa/updaters/random.py
--rw-r--r--   0        0        0   730255 2020-02-02 00:00:00.000000 fsaa-0.0.3/imgs/adv.png
--rw-r--r--   0        0        0   450674 2020-02-02 00:00:00.000000 fsaa-0.0.3/imgs/mask.png
--rw-r--r--   0        0        0   694498 2020-02-02 00:00:00.000000 fsaa-0.0.3/imgs/orig.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fsaa-0.0.3/tests/test_attack.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fsaa-0.0.3/tests/test_initializers.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fsaa-0.0.3/tests/test_masks.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 fsaa-0.0.3/tests/test_models.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fsaa-0.0.3/tests/test_transforms.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fsaa-0.0.3/tests/test_updaters.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 fsaa-0.0.3/.gitignore
--rw-r--r--   0        0        0    19333 2020-02-02 00:00:00.000000 fsaa-0.0.3/LICENSE
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 fsaa-0.0.3/README.md
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 fsaa-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 fsaa-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fsaa-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fsaa-0.0.4/CITATION.cff
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 fsaa-0.0.4/CODEOWNERS
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fsaa-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 fsaa-0.0.4/environment.yml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fsaa-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fsaa-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fsaa-0.0.4/.vscode/launch.json
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fsaa-0.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0    22260 2020-02-02 00:00:00.000000 fsaa-0.0.4/assets/logo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/__init__.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/attack.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/core.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/utils.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/examples/tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/initializers/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/initializers/random.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/initializers/random_sign.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/losses/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/losses/cossim_loss.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/losses/lpips_loss.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/losses/mse_loss.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/masks/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/masks/custom.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/masks/jnd.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/masks/nomask.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/models/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/models/dinov2/dinov2.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/models/hf_models/hf_models.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/models/ibot/ibot.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/models/ibot/utils.py
+-rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/models/ibot/vits.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/transforms/__init__.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/transforms/compose.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/transforms/normalize.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/updaters/__init__.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/updaters/fgsm.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/updaters/langevin.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/updaters/pgd.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fsaa-0.0.4/fsaa/updaters/random.py
+-rw-r--r--   0        0        0   730255 2020-02-02 00:00:00.000000 fsaa-0.0.4/imgs/adv.png
+-rw-r--r--   0        0        0   450674 2020-02-02 00:00:00.000000 fsaa-0.0.4/imgs/mask.png
+-rw-r--r--   0        0        0   694498 2020-02-02 00:00:00.000000 fsaa-0.0.4/imgs/orig.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fsaa-0.0.4/tests/test_attack.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fsaa-0.0.4/tests/test_initializers.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fsaa-0.0.4/tests/test_masks.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 fsaa-0.0.4/tests/test_models.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fsaa-0.0.4/tests/test_transforms.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fsaa-0.0.4/tests/test_updaters.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 fsaa-0.0.4/.gitignore
+-rw-r--r--   0        0        0    19333 2020-02-02 00:00:00.000000 fsaa-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fsaa-0.0.4/README.md
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 fsaa-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 fsaa-0.0.4/PKG-INFO
```

### Comparing `fsaa-0.0.3/.pre-commit-config.yaml` & `fsaa-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/environment.yml` & `fsaa-0.0.4/environment.yml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/.vscode/launch.json` & `fsaa-0.0.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/fsaa/attack.py` & `fsaa-0.0.4/fsaa/attack.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/fsaa/core.py` & `fsaa-0.0.4/fsaa/core.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/fsaa/utils.py` & `fsaa-0.0.4/fsaa/utils.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/fsaa/examples/tutorial.py` & `fsaa-0.0.4/fsaa/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/fsaa/losses/lpips_loss.py` & `fsaa-0.0.4/fsaa/losses/lpips_loss.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/fsaa/masks/jnd.py` & `fsaa-0.0.4/fsaa/masks/jnd.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/fsaa/models/dinov2/dinov2.py` & `fsaa-0.0.4/fsaa/models/dinov2/dinov2.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/fsaa/models/hf_models/hf_models.py` & `fsaa-0.0.4/fsaa/models/hf_models/hf_models.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/fsaa/models/ibot/ibot.py` & `fsaa-0.0.4/fsaa/models/ibot/ibot.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/fsaa/models/ibot/utils.py` & `fsaa-0.0.4/fsaa/models/ibot/utils.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/fsaa/models/ibot/vits.py` & `fsaa-0.0.4/fsaa/models/ibot/vits.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/fsaa/updaters/langevin.py` & `fsaa-0.0.4/fsaa/updaters/langevin.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/fsaa/updaters/pgd.py` & `fsaa-0.0.4/fsaa/updaters/pgd.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/fsaa/updaters/random.py` & `fsaa-0.0.4/fsaa/updaters/random.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/imgs/adv.png` & `fsaa-0.0.4/imgs/adv.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/imgs/mask.png` & `fsaa-0.0.4/imgs/mask.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/imgs/orig.png` & `fsaa-0.0.4/imgs/orig.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/tests/test_attack.py` & `fsaa-0.0.4/tests/test_attack.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/tests/test_initializers.py` & `fsaa-0.0.4/tests/test_initializers.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/tests/test_masks.py` & `fsaa-0.0.4/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/tests/test_models.py` & `fsaa-0.0.4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/tests/test_updaters.py` & `fsaa-0.0.4/tests/test_updaters.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/.gitignore` & `fsaa-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/LICENSE` & `fsaa-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.3/README.md` & `fsaa-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+<h1 align="center">
+  <img width="auto" height="150px" src="assets/logo.png" />
+</h1>
+
+
 # FSAA: Feature Space Adversarial Attacks
 FSAA allows to create adversarial examples that corrupt the features of the victim models. Various attacks are possible, by altering initialization and update strategies, losses and perceptual masks.
 FSAA is written in Python and is based on PyTorch.
 ___
 
 
 ## Installation
@@ -100,14 +105,25 @@
 Contributions are highly welcome! Please refer to the [contributing guidelines](./CONTRIBUTING.md).
 ___
 ## License
 The code is distributed according to the **Attribution-NonCommercial 4.0 International** [LICENSE](./LICENSE).
 ___
 
 ## Citation
-If you used this library as part of your work, please cite the repository with the following URL: [https://github.com/BrianPulfer/fsaa](https://github.com/BrianPulfer/fsaa)
+If you used this library as part of your work, please cite the repository as follows:
+
+```
+@software{Pulfer_FSAA_2023,
+author = {Pulfer, Brian},
+month = jun,
+title = {{FSAA}},
+url = {https://github.com/BrianPulfer/fsaa},
+version = {0.0.4},
+year = {2023}
+}
+```
 ___
 
 ## Acknowledgements
 Part of the code was taken and adapted from the following repositories:
   - [facebookresearch/active_indexing](https://github.com/facebookresearch/active_indexing)
     - JND masking
```

### Comparing `fsaa-0.0.3/pyproject.toml` & `fsaa-0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 # Project metadata
 [project]
 name = "fsaa"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name="Brian Pulfer", email="brianpulfer95@gmail.com" }]
 description = "A simple library for adversarial attacks in feature space."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+    "accelerate",
+    "lpips",
     "numpy",
-    "scipy",
-    "scikit-learn",
-    "matplotlib",
     "torch",
     "torchvision",
-    "tqdm"
+    "tqdm",
+    "transformers",
+    "wget",
+    "xformers"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/BrianPulfer/fsaa"
 "Bug Tracker" = "https://github.com/BrianPulfer/fsaa/issues"
```

### Comparing `fsaa-0.0.3/PKG-INFO` & `fsaa-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: fsaa
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple library for adversarial attacks in feature space.
 Project-URL: Homepage, https://github.com/BrianPulfer/fsaa
 Project-URL: Bug Tracker, https://github.com/BrianPulfer/fsaa/issues
 Author-email: Brian Pulfer <brianpulfer95@gmail.com>
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: matplotlib
+Requires-Dist: accelerate
+Requires-Dist: lpips
 Requires-Dist: numpy
-Requires-Dist: scikit-learn
-Requires-Dist: scipy
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: tqdm
+Requires-Dist: transformers
+Requires-Dist: wget
+Requires-Dist: xformers
 Description-Content-Type: text/markdown
 
+<h1 align="center">
+  <img width="auto" height="150px" src="assets/logo.png" />
+</h1>
+
+
 # FSAA: Feature Space Adversarial Attacks
 FSAA allows to create adversarial examples that corrupt the features of the victim models. Various attacks are possible, by altering initialization and update strategies, losses and perceptual masks.
 FSAA is written in Python and is based on PyTorch.
 ___
 
 
 ## Installation
@@ -121,14 +128,25 @@
 Contributions are highly welcome! Please refer to the [contributing guidelines](./CONTRIBUTING.md).
 ___
 ## License
 The code is distributed according to the **Attribution-NonCommercial 4.0 International** [LICENSE](./LICENSE).
 ___
 
 ## Citation
-If you used this library as part of your work, please cite the repository with the following URL: [https://github.com/BrianPulfer/fsaa](https://github.com/BrianPulfer/fsaa)
+If you used this library as part of your work, please cite the repository as follows:
+
+```
+@software{Pulfer_FSAA_2023,
+author = {Pulfer, Brian},
+month = jun,
+title = {{FSAA}},
+url = {https://github.com/BrianPulfer/fsaa},
+version = {0.0.4},
+year = {2023}
+}
+```
 ___
 
 ## Acknowledgements
 Part of the code was taken and adapted from the following repositories:
   - [facebookresearch/active_indexing](https://github.com/facebookresearch/active_indexing)
     - JND masking
```

