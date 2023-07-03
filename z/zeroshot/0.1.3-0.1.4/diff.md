# Comparing `tmp/zeroshot-0.1.3.tar.gz` & `tmp/zeroshot-0.1.4.tar.gz`

## Comparing `zeroshot-0.1.3.tar` & `zeroshot-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,33 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeroshot-0.1.3/.git
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 zeroshot-0.1.3/requirements.txt
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 zeroshot-0.1.3/requirements_dev.txt
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 zeroshot-0.1.3/.github/workflows/integration_python.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 zeroshot-0.1.3/.github/workflows/lint_python.yml
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 zeroshot-0.1.3/.github/workflows/test_python.yml
--rw-r--r--   0        0        0   651012 2020-02-02 00:00:00.000000 zeroshot-0.1.3/examples/run_classification.ipynb
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 zeroshot-0.1.3/scripts/integration_test.py
--rw-r--r--   0        0        0   448620 2020-02-02 00:00:00.000000 zeroshot-0.1.3/scripts/test_files/giraffe.png
--rw-r--r--   0        0        0    33317 2020-02-02 00:00:00.000000 zeroshot-0.1.3/scripts/test_files/test_model.json
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/__init__.py
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/classifier.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/classifier_test.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/downloader.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/downloader_test.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/feature_extractor.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/feature_extractor_test.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/logistic_regression.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/logistic_regression_test.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/preprocessing.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/utils.py
--rw-r--r--   0        0        0    40312 2020-02-02 00:00:00.000000 zeroshot-0.1.3/zeroshot/test_files/test_model.json
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 zeroshot-0.1.3/.gitignore
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 zeroshot-0.1.3/README.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 zeroshot-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 zeroshot-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeroshot-0.1.4/.git
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 zeroshot-0.1.4/requirements.txt
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 zeroshot-0.1.4/requirements_dev.txt
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 zeroshot-0.1.4/.github/workflows/integration_python.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 zeroshot-0.1.4/.github/workflows/lint_python.yml
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 zeroshot-0.1.4/.github/workflows/test_python.yml
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 zeroshot-0.1.4/docs/getting_started.md
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 zeroshot-0.1.4/docs/prompting_tips.md
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 zeroshot-0.1.4/docs/under_the_hood.md
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 zeroshot-0.1.4/docs/why_zeroshot.md
+-rw-r--r--   0        0        0  1825009 2020-02-02 00:00:00.000000 zeroshot-0.1.4/docs/images/example_prompt.png
+-rw-r--r--   0        0        0  1225951 2020-02-02 00:00:00.000000 zeroshot-0.1.4/docs/images/example_result.png
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 zeroshot-0.1.4/examples/run_classification.ipynb
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 zeroshot-0.1.4/scripts/integration_test.py
+-rw-r--r--   0        0        0   448620 2020-02-02 00:00:00.000000 zeroshot-0.1.4/scripts/test_files/giraffe.png
+-rw-r--r--   0        0        0     8382 2020-02-02 00:00:00.000000 zeroshot-0.1.4/scripts/test_files/test_binary.json
+-rw-r--r--   0        0        0    33317 2020-02-02 00:00:00.000000 zeroshot-0.1.4/scripts/test_files/test_model.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 zeroshot-0.1.4/zeroshot/__init__.py
+-rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 zeroshot-0.1.4/zeroshot/classifier.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 zeroshot-0.1.4/zeroshot/classifier_test.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 zeroshot-0.1.4/zeroshot/downloader.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 zeroshot-0.1.4/zeroshot/downloader_test.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 zeroshot-0.1.4/zeroshot/feature_extractor.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 zeroshot-0.1.4/zeroshot/feature_extractor_test.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 zeroshot-0.1.4/zeroshot/logistic_regression.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 zeroshot-0.1.4/zeroshot/logistic_regression_test.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 zeroshot-0.1.4/zeroshot/preprocessing.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 zeroshot-0.1.4/zeroshot/utils.py
+-rw-r--r--   0        0        0    40312 2020-02-02 00:00:00.000000 zeroshot-0.1.4/zeroshot/test_files/test_model.json
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 zeroshot-0.1.4/.gitignore
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 zeroshot-0.1.4/README.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 zeroshot-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 zeroshot-0.1.4/PKG-INFO
```

### Comparing `zeroshot-0.1.3/.github/workflows/integration_python.yml` & `zeroshot-0.1.4/.github/workflows/integration_python.yml`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/.github/workflows/lint_python.yml` & `zeroshot-0.1.4/.github/workflows/lint_python.yml`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/.github/workflows/test_python.yml` & `zeroshot-0.1.4/.github/workflows/test_python.yml`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/scripts/test_files/giraffe.png` & `zeroshot-0.1.4/scripts/test_files/giraffe.png`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/scripts/test_files/test_model.json` & `zeroshot-0.1.4/scripts/test_files/test_model.json`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/zeroshot/classifier.py` & `zeroshot-0.1.4/zeroshot/classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         possible_types = ("infer", "guid", "file")
         if path_type not in possible_types:
             raise ValueError(
                 f"Path type must be one of {possible_types}, got {path_type}"
             )
 
         self.path = path
-        self.class_list = []
+        self.classes = []
 
         # Load the preprocessor for the model.
         if preprocessor is None:
             self.preprocess_fn = None
         else:
             self.preprocess_fn = create_preprocess_fn(preprocessor)
```

### Comparing `zeroshot-0.1.3/zeroshot/classifier_test.py` & `zeroshot-0.1.4/zeroshot/classifier_test.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/zeroshot/downloader.py` & `zeroshot-0.1.4/zeroshot/downloader.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/zeroshot/downloader_test.py` & `zeroshot-0.1.4/zeroshot/downloader_test.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/zeroshot/feature_extractor.py` & `zeroshot-0.1.4/zeroshot/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/zeroshot/feature_extractor_test.py` & `zeroshot-0.1.4/zeroshot/feature_extractor_test.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/zeroshot/logistic_regression_test.py` & `zeroshot-0.1.4/zeroshot/logistic_regression_test.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/zeroshot/preprocessing.py` & `zeroshot-0.1.4/zeroshot/preprocessing.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/zeroshot/utils.py` & `zeroshot-0.1.4/zeroshot/utils.py`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/zeroshot/test_files/test_model.json` & `zeroshot-0.1.4/zeroshot/test_files/test_model.json`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/.gitignore` & `zeroshot-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.3/README.md` & `zeroshot-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Zeroshot (Python)
+
 Image classification for the masses
 
 ## Installation
+
 Install via pip: `pip install zeroshot`
 
 ## Usage
-First, go to usezeroshot.com and create a classifier. See [here]() for more instructions.
+
+First, go to usezeroshot.com and create a classifier. See [here](<>) for more instructions.
 
 Then, in Python (`image` should be an RGB numpy array with channels last):
 
 ```python
 import zeroshot
 
 # Create the classifier and preprocessing function.
@@ -18,8 +21,9 @@
 
 # Run the model!
 prediction = classifier.predict(preprocess_fn(image))
 print(f"The image is class {prediction}")
 ```
 
 ## Read the docs
-PUT DOCS HERE.
+
+See the [docs](docs/getting_started.md) folder for some details.
```

### Comparing `zeroshot-0.1.3/pyproject.toml` & `zeroshot-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zeroshot"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     {name = "Zeroshot Maintainers", email = "hello@usezeroshot.com"},
 ]
 description = "Image classifier with zero-shot learning."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `zeroshot-0.1.3/PKG-INFO` & `zeroshot-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: zeroshot
-Version: 0.1.3
+Version: 0.1.4
 Summary: Image classifier with zero-shot learning.
 Project-URL: Homepage, https://github.com/moonshinelabs/zeroshot-python
 Author-email: Zeroshot Maintainers <hello@usezeroshot.com>
 Keywords: classifier,cv,zeroshot
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: numpy
 Requires-Dist: onnxruntime
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # Zeroshot (Python)
+
 Image classification for the masses
 
 ## Installation
+
 Install via pip: `pip install zeroshot`
 
 ## Usage
-First, go to usezeroshot.com and create a classifier. See [here]() for more instructions.
+
+First, go to usezeroshot.com and create a classifier. See [here](<>) for more instructions.
 
 Then, in Python (`image` should be an RGB numpy array with channels last):
 
 ```python
 import zeroshot
 
 # Create the classifier and preprocessing function.
@@ -32,8 +35,9 @@
 
 # Run the model!
 prediction = classifier.predict(preprocess_fn(image))
 print(f"The image is class {prediction}")
 ```
 
 ## Read the docs
-PUT DOCS HERE.
+
+See the [docs](docs/getting_started.md) folder for some details.
```

