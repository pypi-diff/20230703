# Comparing `tmp/responsibleai_vision-0.2.2.tar.gz` & `tmp/responsibleai_vision-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsibleai_vision-0.2.2.tar", last modified: Fri Jun 16 18:59:55 2023, max compression
+gzip compressed data, was "responsibleai_vision-0.2.3.tar", last modified: Mon Jul  3 20:08:22 2023, max compression
```

## Comparing `responsibleai_vision-0.2.2.tar` & `responsibleai_vision-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.839594 responsibleai_vision-0.2.2/
--rw-rw-rw-   0        0        0     1403 2023-06-16 18:59:55.836377 responsibleai_vision-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      691 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.332246 responsibleai_vision-0.2.2/responsibleai_vision/
--rw-rw-rw-   0        0        0      367 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.2/responsibleai_vision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.459308 responsibleai_vision-0.2.2/responsibleai_vision/common/
--rw-rw-rw-   0        0        0      127 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.2/responsibleai_vision/common/__init__.py
--rw-rw-rw-   0        0        0     2634 2023-06-16 18:35:38.000000 responsibleai_vision-0.2.2/responsibleai_vision/common/constants.py
--rw-rw-rw-   0        0        0      223 2022-09-01 02:31:14.000000 responsibleai_vision-0.2.2/responsibleai_vision/common/interfaces.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.551491 responsibleai_vision-0.2.2/responsibleai_vision/managers/
--rw-rw-rw-   0        0        0      109 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.2/responsibleai_vision/managers/__init__.py
--rw-rw-rw-   0        0        0    13897 2023-05-05 19:17:38.000000 responsibleai_vision-0.2.2/responsibleai_vision/managers/error_analysis_manager.py
--rw-rw-rw-   0        0        0    26875 2023-06-16 18:35:38.000000 responsibleai_vision-0.2.2/responsibleai_vision/managers/explainer_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.607855 responsibleai_vision-0.2.2/responsibleai_vision/rai_vision_insights/
--rw-rw-rw-   0        0        0      253 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.2/responsibleai_vision/rai_vision_insights/__init__.py
--rw-rw-rw-   0        0        0    50360 2023-06-16 18:35:38.000000 responsibleai_vision-0.2.2/responsibleai_vision/rai_vision_insights/rai_vision_insights.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.718725 responsibleai_vision-0.2.2/responsibleai_vision/utils/
--rw-rw-rw-   0        0        0      129 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.2/responsibleai_vision/utils/__init__.py
--rw-rw-rw-   0        0        0     2443 2023-05-12 20:02:09.000000 responsibleai_vision-0.2.2/responsibleai_vision/utils/feature_extractors.py
--rw-rw-rw-   0        0        0     2824 2023-04-18 20:29:06.000000 responsibleai_vision-0.2.2/responsibleai_vision/utils/image_reader.py
--rw-rw-rw-   0        0        0     4907 2023-06-16 18:35:38.000000 responsibleai_vision-0.2.2/responsibleai_vision/utils/image_utils.py
--rw-rw-rw-   0        0        0      194 2023-06-16 18:59:00.000000 responsibleai_vision-0.2.2/responsibleai_vision/version.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.396288 responsibleai_vision-0.2.2/responsibleai_vision.egg-info/
--rw-rw-rw-   0        0        0     1403 2023-06-16 18:59:54.000000 responsibleai_vision-0.2.2/responsibleai_vision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1030 2023-06-16 18:59:54.000000 responsibleai_vision-0.2.2/responsibleai_vision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 18:59:54.000000 responsibleai_vision-0.2.2/responsibleai_vision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2023-06-16 18:59:54.000000 responsibleai_vision-0.2.2/responsibleai_vision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-16 18:59:54.000000 responsibleai_vision-0.2.2/responsibleai_vision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 18:59:55.840618 responsibleai_vision-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1417 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.827954 responsibleai_vision-0.2.2/tests/
--rw-rw-rw-   0        0        0     2067 2023-06-16 18:35:38.000000 responsibleai_vision-0.2.2/tests/test_image_utils.py
--rw-rw-rw-   0        0        0     4575 2023-04-17 19:05:16.000000 responsibleai_vision-0.2.2/tests/test_rai_vision_automl_images_insights.py
--rw-rw-rw-   0        0        0    12099 2023-06-16 18:35:38.000000 responsibleai_vision-0.2.2/tests/test_rai_vision_insights.py
--rw-rw-rw-   0        0        0     3088 2023-06-08 15:48:16.000000 responsibleai_vision-0.2.2/tests/test_rai_vision_insights_save_and_load_scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.212848 responsibleai_vision-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-03 20:08:22.212848 responsibleai_vision-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.208848 responsibleai_vision-0.2.3/responsibleai_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.208848 responsibleai_vision-0.2.3/responsibleai_vision/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/common/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.208848 responsibleai_vision-0.2.3/responsibleai_vision/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/managers/error_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27682 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/managers/explainer_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.212848 responsibleai_vision-0.2.3/responsibleai_vision/rai_vision_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/rai_vision_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47582 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/rai_vision_insights/rai_vision_insights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.212848 responsibleai_vision-0.2.3/responsibleai_vision/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/utils/feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/utils/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/responsibleai_vision/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.208848 responsibleai_vision-0.2.3/responsibleai_vision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-03 20:08:22.000000 responsibleai_vision-0.2.3/responsibleai_vision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-03 20:08:22.000000 responsibleai_vision-0.2.3/responsibleai_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:08:22.000000 responsibleai_vision-0.2.3/responsibleai_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-03 20:08:22.000000 responsibleai_vision-0.2.3/responsibleai_vision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 20:08:22.000000 responsibleai_vision-0.2.3/responsibleai_vision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 20:08:22.212848 responsibleai_vision-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:08:22.212848 responsibleai_vision-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/tests/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/tests/test_rai_vision_automl_images_insights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13696 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/tests/test_rai_vision_insights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-03 20:03:14.000000 responsibleai_vision-0.2.3/tests/test_rai_vision_insights_save_and_load_scenarios.py
```

### Comparing `responsibleai_vision-0.2.2/PKG-INFO` & `responsibleai_vision-0.2.3/responsibleai_vision.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1
-Name: responsibleai_vision
-Version: 0.2.2
-Summary: SDK API to assess image Machine Learning models.
-Home-page: https://github.com/microsoft/responsible-ai-toolbox
-Author: Roman Lutz, Ilya Matiach, Ke Xu
-Author-email: raiwidgets-maintain@microsoft.com
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# Responsible AI Vision SDK for Python
-
-### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
-
-The Responsible AI Vision sdk enables users to analyze their machine learning models for computer vision in one API. Users will be able to analyze errors, explain the most important features, and understand their data using a single API.
-
-Highlights of the package include:
-
-- `explainer.add()` explains the model
-
-### Supported scenarios, models and datasets
-
-The Responsible AI Vision SDK supports multiclass classification models on image data currently.
-
-The open source code for the visualization dashboard can be found here:
-https://github.com/microsoft/responsible-ai-widgets
+Metadata-Version: 2.1
+Name: responsibleai-vision
+Version: 0.2.3
+Summary: SDK API to assess image Machine Learning models.
+Home-page: https://github.com/microsoft/responsible-ai-toolbox
+Author: Roman Lutz, Ilya Matiach, Ke Xu
+Author-email: raiwidgets-maintain@microsoft.com
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# Responsible AI Vision SDK for Python
+
+### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
+
+The Responsible AI Vision SDK enables users to analyze their machine learning models for computer vision in one API. Users will be able to analyze errors, explain the most important features, and understand their data using a single API.
+
+Highlights of the package include:
+
+- `explainer.add()` explains the model
+
+### Supported scenarios, models and datasets
+
+The Responsible AI Vision SDK supports multiclass classification models on image data currently.
+
+The open source code for the visualization dashboard can be found here:
+https://github.com/microsoft/responsible-ai-widgets
```

### Comparing `responsibleai_vision-0.2.2/README.md` & `responsibleai_vision-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Responsible AI Vision SDK for Python
 
 ### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
 
-The Responsible AI Vision sdk enables users to analyze their machine learning models for computer vision in one API. Users will be able to analyze errors, explain the most important features, and understand their data using a single API.
+The Responsible AI Vision SDK enables users to analyze their machine learning models for computer vision in one API. Users will be able to analyze errors, explain the most important features, and understand their data using a single API.
 
 Highlights of the package include:
 
 - `explainer.add()` explains the model
 
 ### Supported scenarios, models and datasets
```

### Comparing `responsibleai_vision-0.2.2/responsibleai_vision/common/constants.py` & `responsibleai_vision-0.2.3/responsibleai_vision/common/constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.2/responsibleai_vision/managers/error_analysis_manager.py` & `responsibleai_vision-0.2.3/responsibleai_vision/managers/error_analysis_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
 """Defines the Error Analysis Manager class."""
 
-from typing import Any, List, Optional
-
-import pandas as pd
-import numpy as np
-
 import json
+from typing import Any, List, Optional
 
 import jsonschema
-
+import numpy as np
+import pandas as pd
 from ml_wrappers import wrap_model
 
 from erroranalysis._internal.error_analyzer import ModelAnalyzer
 from erroranalysis._internal.error_report import as_error_report
-from responsibleai._tools.shared.state_directory_management import (
-    DirectoryManager)
-from responsibleai.managers.error_analysis_manager import (
-    as_error_config, ErrorAnalysisManager as BaseErrorAnalysisManager)
-from responsibleai_vision.utils.image_utils import get_images
-from responsibleai_vision.common.constants import (
-    ModelTask, MLFlowSchemaLiterals)
+from responsibleai._tools.shared.state_directory_management import \
+    DirectoryManager
+from responsibleai.managers.error_analysis_manager import \
+    ErrorAnalysisManager as BaseErrorAnalysisManager
+from responsibleai.managers.error_analysis_manager import as_error_config
+from responsibleai_vision.common.constants import (MLFlowSchemaLiterals,
+                                                   ModelTask)
 from responsibleai_vision.utils.image_reader import (
     get_base64_string_from_path, is_automl_image_model)
+from responsibleai_vision.utils.image_utils import get_images
 
 LABELS = 'labels'
 
 
 def _concat_labels_column(dataset, target_column, classes):
     """Concatenate labels column for multilabel models.
 
@@ -38,15 +36,15 @@
     :type target_column: list[str]
     :param classes: The list of labels in multilabel task.
     :type classes: list
     :return: The labels column concatenated.
     :rtype: list
     """
     labels = []
-    for index, row in dataset[target_column].iterrows():
+    for _, row in dataset[target_column].iterrows():
         row_idxs = range(len(row))
         pred_classes = [classes[i] for i in row_idxs if row[i]]
         labels.append(','.join(pred_classes))
     return labels
 
 
 class WrappedIndexPredictorModel:
@@ -291,15 +289,16 @@
         dataset = rai_insights._ext_test_df.drop(columns=dropped_cols)
         inst.__dict__['_dataset'] = dataset
         feature_names = list(dataset.columns)
         inst.__dict__['_feature_names'] = feature_names
         task_type = rai_insights.task_type
         wrapped_model = wrap_model(rai_insights.model, dataset,
                                    rai_insights.task_type,
-                                   classes=rai_insights._classes)
+                                   classes=rai_insights._classes,
+                                   device=rai_insights.device)
         inst.__dict__['_task_type'] = task_type
         index_classes = rai_insights._classes
         is_od = task_type == ModelTask.OBJECT_DETECTION
         index_dataset = rai_insights.test
         if isinstance(target_column, list) and not is_od:
             # create copy of dataset as we will make modifications to it
             index_dataset = index_dataset.copy()
```

### Comparing `responsibleai_vision-0.2.2/responsibleai_vision/managers/explainer_manager.py` & `responsibleai_vision-0.2.3/responsibleai_vision/managers/explainer_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
 """Defines the Explainer Manager class."""
 
-import cv2
 import base64
 import io
 import json
 import pickle
 import warnings
 from pathlib import Path
 from typing import Any, List, Optional
 
+import cv2
 import matplotlib.pyplot as pl
 import numpy as np
 import pandas as pd
 import shap
 from ml_wrappers import wrap_model
+from ml_wrappers.common.constants import Device
+from ml_wrappers.model.image_model_wrapper import (MLflowDRiseWrapper,
+                                                   PytorchDRiseWrapper)
+from PIL import Image, ImageDraw, ImageFont
+from shap.plots import colors
+from shap.utils._legacy import kmeans
+from vision_explanation_methods.DRISE_runner import get_drise_saliency_map
+
 from responsibleai._interfaces import ModelExplanationData
 from responsibleai._internal.constants import ExplainerManagerKeys as Keys
 from responsibleai._internal.constants import (ListProperties, ManagerNames,
                                                Metadata)
 from responsibleai._tools.shared.state_directory_management import \
     DirectoryManager
 from responsibleai.exceptions import UserConfigValidationException
@@ -29,33 +37,28 @@
                                                    ExplainabilityDefaults,
                                                    ExplainabilityLiterals,
                                                    MLFlowSchemaLiterals,
                                                    ModelTask,
                                                    XAIPredictionLiterals)
 from responsibleai_vision.utils.image_reader import (
     get_base64_string_from_path, get_image_from_path, is_automl_image_model)
-from shap.plots import colors
-from shap.utils._legacy import kmeans
-from vision_explanation_methods.DRISE_runner import get_drise_saliency_map
-from ml_wrappers.model.image_model_wrapper import (PytorchDRiseWrapper,
-                                                   MLflowDRiseWrapper)
-from PIL import Image, ImageDraw, ImageFont
 
 IS_RUN = 'is_run'
 IS_ADDED = 'is_added'
 CLASSES = 'classes'
 U_EVALUATION_EXAMPLES = '_evaluation_examples'
 FEATURES = 'features'
 META_JSON = Metadata.META_JSON
 MODEL = Metadata.MODEL
 EXPLANATION = '_explanation'
 TASK_TYPE = 'task_type'
 _MAX_EVALS = '_max_evals'
 _NUM_MASKS = '_num_masks'
 _MASK_RES = '_mask_res'
+_DEVICE = '_device'
 DEFAULT_MAX_EVALS = ExplainabilityDefaults.DEFAULT_MAX_EVALS
 DEFAULT_MASK_RES = ExplainabilityDefaults.DEFAULT_MASK_RES
 DEFAULT_NUM_MASKS = ExplainabilityDefaults.DEFAULT_NUM_MASKS
 
 
 class ExplainerManager(BaseManager):
 
@@ -65,15 +68,16 @@
                  evaluation_examples: pd.DataFrame,
                  target_column: str,
                  task_type: str,
                  classes: Optional[List] = None,
                  image_mode: str = None,
                  max_evals: Optional[int] = DEFAULT_MAX_EVALS,
                  num_masks: Optional[int] = DEFAULT_NUM_MASKS,
-                 mask_res: Optional[int] = DEFAULT_MASK_RES):
+                 mask_res: Optional[int] = DEFAULT_MASK_RES,
+                 device: Optional[str] = Device.AUTO.value):
         """Creates an ExplainerManager object.
 
         :param model: The model to explain.
             A model that implements sklearn.predict or sklearn.predict_proba
             or function that accepts a 2d ndarray.
         :type model: object
         :param evaluation_examples: A matrix of feature vector
@@ -100,21 +104,25 @@
             DRISE image explainer for object detection.
             If not specified defaults to 50.
         :type num_masks: int
         :param mask_res: The resolution of the masks to use for the
             DRISE image explainer for object detection.
             If not specified defaults to 4.
         :type mask_res: int
+        :param device: The device to run the model on.
+            If not specified defaults to Device.AUTO.
+        :type device: str
         """
         self._image_mode = image_mode
         if task_type == ModelTask.OBJECT_DETECTION:
             if is_automl_image_model(model):
                 self._model = MLflowDRiseWrapper(model._model, classes)
             else:
-                self._model = PytorchDRiseWrapper(model._model, len(classes))
+                self._model = PytorchDRiseWrapper(
+                    model._model, len(classes), device=device)
         else:
             self._model = model
         self._target_column = target_column
         if not isinstance(target_column, list):
             target_column = [target_column]
         self._evaluation_examples = \
             evaluation_examples.drop(columns=target_column)
@@ -123,14 +131,15 @@
         self._features = list(self._evaluation_examples.columns)
         self._classes = classes
         self._explanation = None
         self._task_type = task_type
         self._max_evals = max_evals
         self._num_masks = num_masks
         self._mask_res = mask_res
+        self._device = device
 
     def add(self):
         """Add an explainer to be computed later."""
         if self._model is None:
             raise UserConfigValidationException(
                 'Model is required for model explanations')
 
@@ -207,15 +216,15 @@
         if self._explanation is not None and index < len(self._explanation):
             if self._task_type == ModelTask.OBJECT_DETECTION:
                 return self._explanation[index][object_index]
             else:
                 return self._explanation[index]
         if self._is_classification_task:
             ex = self._evaluation_examples
-            image = ex.iloc[index:index+1, 0].values[0]
+            image = ex.iloc[index:index + 1, 0].values[0]
             if isinstance(image, str):
                 if not self.automl_image_model:
                     image = get_image_from_path(image, self._image_mode)
             if xai_algo_name == ExplainabilityLiterals.SHAP:
                 if not self.automl_image_model:
                     explanation = self.get_shap_explanations(image, max_evals)
                     return self.image(explanation, 0)
@@ -235,33 +244,39 @@
                     raise ValueError(
                         '{} is not supported for the model type: {}'.format(
                             xai_algo_name, type(self._model)
                         )
                     )
         if self._is_object_detection_task:
             ex = self._evaluation_examples
-            img = ex.iloc[index:index+1, 0].values[0]
+            img = ex.iloc[index:index + 1, 0].values[0]
             try:
                 if (type(self._model) is not MLflowDRiseWrapper and
                    type(self._model) is not PytorchDRiseWrapper):
                     if is_automl_image_model(self._model):
                         self._model = MLflowDRiseWrapper(self._model._model,
                                                          self._classes)
                     else:
                         self._model = PytorchDRiseWrapper(self._model._model,
-                                                          len(self._classes))
+                                                          len(self._classes),
+                                                          self._device)
 
                 # calling DRISE to generate saliency maps for all objects
                 mask_res_tuple = (self._mask_res, self._mask_res)
+                device = self._device
+                # get_drise_saliency_map only recognizes GPU and CPU
+                if device == Device.AUTO.value:
+                    device = None
                 fl, _, _, = get_drise_saliency_map(img,
                                                    self._model,
                                                    len(self._classes),
                                                    savename=str(index),
                                                    nummasks=self._num_masks,
                                                    maskres=mask_res_tuple,
+                                                   devicechoice=device,
                                                    max_figures=5000)
                 if object_index is None:
                     return fl
                 b64_string = fl[object_index]
             except BaseException:
                 if object_index is None:
                     return [self._get_fail_str()]
@@ -413,23 +428,23 @@
                     x_curr /= 255.
                 except Exception:
                     # In-place divide can fail for certain types
                     x_curr = x_curr / 255.
 
             # get a grayscale version of the image
             if len(x_curr.shape) == 3 and x_curr.shape[2] == 3:
-                x_curr_gray = (0.2989 * x_curr[:, :, 0]
-                               + 0.5870 * x_curr[:, :, 1]
-                               + 0.1140 * x_curr[:, :, 2])  # rgb to gray
+                x_curr_gray = (0.2989 * x_curr[:, :, 0] +
+                               0.5870 * x_curr[:, :, 1] +
+                               0.1140 * x_curr[:, :, 2])  # rgb to gray
                 x_curr_disp = x_curr
             elif len(x_curr.shape) == 3:
                 x_curr_gray = x_curr.mean(2)
 
                 # for non-RGB multi-channel data
-                flat_vals = x_curr.reshape([x_curr.shape[0]*x_curr.shape[1],
+                flat_vals = x_curr.reshape([x_curr.shape[0] * x_curr.shape[1],
                                             x_curr.shape[2]]).T
                 flat_vals = (flat_vals.T - flat_vals.mean(1)).T
                 means = kmeans(flat_vals, 3, round_values=False)
                 means = means.data.T.reshape([x_curr.shape[0],
                                               x_curr.shape[1], 3])
                 x_curr_disp = ((means - np.percentile(means, 0.5, (0, 1))) /
                                (np.percentile(means, 99.5, (0, 1)) -
@@ -449,36 +464,36 @@
             else:
                 abs_vals = np.stack([np.abs(s_vals[i].sum(-1))
                                      for i in s_range], 0)
             abs_vals = abs_vals.flatten()
             max_val = np.nanpercentile(abs_vals, 99.9)
             for i in s_range:
                 if labels is not None:
-                    axes[row, i+1].set_title(labels[row, i], **label_kwargs)
+                    axes[row, i + 1].set_title(labels[row, i], **label_kwargs)
                 sv = (s_vals[i][row]
                       if len(s_vals[i][row].shape) == 2
                       else s_vals[i][row].sum(-1))
-                axes[row, i+1].imshow(x_curr_gray, cmap=pl.get_cmap('gray'),
-                                      alpha=0.15,
-                                      extent=(-1, sv.shape[1],
-                                      sv.shape[0], -1))
-                im = axes[row, i+1].imshow(sv,
-                                           cmap=colors.red_transparent_blue,
-                                           vmin=-max_val,
-                                           vmax=max_val)
-                axes[row, i+1].axis('off')
+                axes[row, i + 1].imshow(x_curr_gray, cmap=pl.get_cmap('gray'),
+                                        alpha=0.15,
+                                        extent=(-1, sv.shape[1],
+                                        sv.shape[0], -1))
+                im = axes[row, i + 1].imshow(sv,
+                                             cmap=colors.red_transparent_blue,
+                                             vmin=-max_val,
+                                             vmax=max_val)
+                axes[row, i + 1].axis('off')
         if hspace == 'auto':
             fig.tight_layout()
         else:
             fig.subplots_adjust(hspace=hspace)
         cb = fig.colorbar(im,
                           ax=np.ravel(axes).tolist(),
                           label='SHAP value',
                           orientation='horizontal',
-                          aspect=fig_size[0]/aspect)
+                          aspect=fig_size[0] / aspect)
         cb.outline.set_visible(False)
         s = io.BytesIO()
         pl.savefig(s, format='jpg')
         s.seek(0)
         b64 = base64.b64encode(s.read())
         b64 = b64.decode(CommonTags.IMAGE_DECODE_UTF_FORMAT)
         pl.clf()
@@ -635,20 +650,22 @@
         else:
             inst.__dict__['_' + IS_RUN] = False
             inst.__dict__['_' + IS_ADDED] = False
             inst.__dict__[EXPLANATION] = None
 
         wrapped_model = wrap_model(rai_insights.model, rai_insights.test,
                                    rai_insights.task_type,
-                                   classes=rai_insights._classes)
+                                   classes=rai_insights._classes,
+                                   device=rai_insights.device)
         inst.__dict__['_' + MODEL] = wrapped_model
         inst.__dict__['_' + CLASSES] = rai_insights._classes
         inst.__dict__[_MAX_EVALS] = rai_insights.max_evals
         inst.__dict__[_NUM_MASKS] = rai_insights.num_masks
         inst.__dict__[_MASK_RES] = rai_insights.mask_res
+        inst.__dict__[_DEVICE] = rai_insights.device
         target_column = rai_insights.target_column
         if not isinstance(target_column, list):
             target_column = [target_column]
         test = rai_insights.test.drop(columns=target_column)
         inst.__dict__[U_EVALUATION_EXAMPLES] = test
         inst.__dict__['_' + FEATURES] = list(test.columns)
         inst.__dict__['_' + TASK_TYPE] = rai_insights.task_type
```

### Comparing `responsibleai_vision-0.2.2/responsibleai_vision/rai_vision_insights/rai_vision_insights.py` & `responsibleai_vision-0.2.3/responsibleai_vision/rai_vision_insights/rai_vision_insights.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,40 +10,40 @@
 import pickle
 import shutil
 import warnings
 from enum import Enum
 from pathlib import Path
 from typing import Any, Optional
 
-import cv2
 import matplotlib.pyplot as pl
 import numpy as np
 import pandas as pd
 import torch
+from ml_wrappers import wrap_model
+from ml_wrappers.common.constants import Device
 from torchmetrics.detection.mean_ap import MeanAveragePrecision
 
 from erroranalysis._internal.cohort_filter import FilterDataWithCohortFilters
-from ml_wrappers import wrap_model
 from raiutils.data_processing import convert_to_list
 from raiutils.models.model_utils import SKLearn
 from responsibleai._interfaces import Dataset, RAIInsightsData
 from responsibleai._internal.constants import (ManagerNames, Metadata,
                                                SerializationAttributes)
 from responsibleai.exceptions import UserConfigValidationException
 from responsibleai.feature_metadata import FeatureMetadata
 from responsibleai.rai_insights.rai_base_insights import RAIBaseInsights
 from responsibleai.serialization_utilities import serialize_json_safe
-
-from responsibleai_vision.common.constants import (CommonTags, ImageColumns,
+from responsibleai_vision.common.constants import (CommonTags,
+                                                   ExplainabilityDefaults,
+                                                   ImageColumns,
                                                    MLFlowSchemaLiterals,
-                                                   ModelTask,
-                                                   ExplainabilityDefaults)
+                                                   ModelTask)
+from responsibleai_vision.managers.error_analysis_manager import \
+    ErrorAnalysisManager
 from responsibleai_vision.managers.explainer_manager import ExplainerManager
-from responsibleai_vision.managers.error_analysis_manager import (
-    ErrorAnalysisManager)
 from responsibleai_vision.utils.feature_extractors import extract_features
 from responsibleai_vision.utils.image_reader import (
     get_base64_string_from_path, get_image_from_path, is_automl_image_model)
 from responsibleai_vision.utils.image_utils import (
     convert_images, get_images, transform_object_detection_labels)
 
 IMAGE = ImageColumns.IMAGE.value
@@ -53,14 +53,15 @@
 DEFAULT_MASK_RES = ExplainabilityDefaults.DEFAULT_MASK_RES
 _IMAGE_MODE = 'image_mode'
 _IMAGE_DOWNLOADER = 'image_downloader'
 _IMAGE_WIDTH = 'image_width'
 _MAX_EVALS = 'max_evals'
 _NUM_MASKS = 'num_masks'
 _MASK_RES = 'mask_res'
+_DEVICE = 'device'
 _PREDICTIONS = 'predictions'
 _TEST = 'test'
 _TARGET_COLUMN = 'target_column'
 _TASK_TYPE = 'task_type'
 _CLASSES = 'classes'
 _META_JSON = Metadata.META_JSON
 _JSON_EXTENSION = '.json'
@@ -114,15 +115,16 @@
                  test_data_path: Optional[str] = None,
                  transformations: Optional[Any] = None,
                  image_downloader: Optional[Any] = None,
                  feature_metadata: Optional[FeatureMetadata] = None,
                  image_width: Optional[float] = None,
                  max_evals: Optional[int] = DEFAULT_MAX_EVALS,
                  num_masks: Optional[int] = DEFAULT_NUM_MASKS,
-                 mask_res: Optional[int] = DEFAULT_MASK_RES):
+                 mask_res: Optional[int] = DEFAULT_MASK_RES,
+                 device: Optional[str] = Device.AUTO.value):
         """Creates an RAIVisionInsights object.
 
         :param model: The model to compute RAI insights for.
             A model that implements sklearn.predict or sklearn.predict_proba
             or function that accepts a 2d ndarray.
         :type model: object
         :param test: The test dataframe including the label column.
@@ -172,14 +174,17 @@
             DRISE image explainer for object detection.
             If not specified defaults to 50.
         :type num_masks: int
         :param mask_res: The resolution of the masks to use for the
             DRISE image explainer for object detection.
             If not specified defaults to 4.
         :type mask_res: int
+        :param device: The device to run the model on.
+            If not specified defaults to Device.AUTO.
+        :type device: str
         """
         # drop index as this can cause issues later like when copying
         # target column below from test dataset to _ext_test_df
         test = test.reset_index(drop=True)
         if feature_metadata is None:
             # initialize to avoid having to keep checking if it is None
             feature_metadata = FeatureMetadata()
@@ -194,24 +199,27 @@
             num_masks = DEFAULT_NUM_MASKS
         elif num_masks < 1:
             raise ValueError('num_masks must be greater than 0')
         if mask_res is None:
             mask_res = DEFAULT_MASK_RES
         elif mask_res < 1:
             raise ValueError('mask_res must be greater than 0')
+        if device is None:
+            device = Device.AUTO.value
         self.max_evals = max_evals
         self.num_masks = num_masks
         self.mask_res = mask_res
+        self.device = device
         self.test_mltable_path = test_data_path
         self._transformations = transformations
         self._image_downloader = image_downloader
         sample = test.iloc[0:2]
         sample = get_images(sample, self.image_mode, self._transformations)
         self._wrapped_model = wrap_model(
-            model, sample, task_type, classes=classes)
+            model, sample, task_type, classes=classes, device=device)
 
         # adding this field to use in _get_single_image and _save_predictions
         self._task_type = task_type
 
         self.automl_image_model = is_automl_image_model(self._wrapped_model)
 
         self._validate_rai_insights_input_parameters(
@@ -614,39 +622,28 @@
         elif IMAGE_URL in column_names:
             images = self.test[:].image_url
         else:
             raise ValueError('No image column found in test data')
         encoded_images = []
         image_dimensions = []
 
-        for i, image in enumerate(images):
+        for _, image in enumerate(images):
             if isinstance(image, str):
                 image = get_image_from_path(image, self.image_mode)
             s = io.BytesIO()
             # IMshow only accepts floats in range [0, 1]
             try:
                 image /= 255
             except Exception:
                 # In-place divide can fail for certain types
                 image = image / 255
             axes = pl.gca()
             axes.get_xaxis().set_visible(False)
             axes.get_yaxis().set_visible(False)
 
-            # TODO: remove condition after drawing bboxes in the frontend
-            if tasktype == ModelTask.OBJECT_DETECTION:
-                num_classes = len(dashboard_dataset.class_names)
-                colors = np.random.uniform(0, 255, size=(num_classes, 3))
-                image = self._draw_bounding_boxes(
-                    image=image,
-                    image_gt=dashboard_dataset.true_y[i],
-                    image_prediction=dashboard_dataset.predicted_y[i],
-                    class_names=dashboard_dataset.class_names,
-                    colors=colors
-                )
             pl.imshow(image)
             # resize image as optimization
             size = pl.gcf().get_size_inches()
             curr_width = size[0]
             curr_height = size[1]
             image_dimensions.append([image.shape[1], image.shape[0]])
             new_width = self.image_width
@@ -696,85 +693,19 @@
         """
         formatted_labels = []
 
         for image in y:
             object_labels_lst = [0] * len(class_names)
             for detection in image:
                 # tracking number of same objects in the image
-                object_labels_lst[int(detection[0]-1)] += 1
+                object_labels_lst[int(detection[0] - 1)] += 1
             formatted_labels.append(object_labels_lst)
 
         return formatted_labels
 
-    def _draw_bounding_boxes(self,
-                             image,
-                             image_gt,
-                             image_prediction,
-                             class_names,
-                             colors):
-        """Annotates the specified image with labels, confidence scores, and
-        ground truth and predicted bounding boxes.
-
-        :param image: Single image/example.
-        :type image: numpy.ndarray
-        :param image_gt: Ground truth labels for the image.
-        :type image_gt: list
-        :param image_prediction: Prediction labels for the image.
-        :type image_prediction: list
-        :param class_names: The class labels in the dataset.
-        :type class_names: list
-        :return: Image augmented with boxes, labels, and confidence scores.
-        :rtype: numpy.ndarray
-        """
-
-        pred_boxes, pred_labels, pred_scores = [], [], []
-        for object_prediction in image_prediction:
-            pred_labels.append(int(object_prediction[0]))
-            pred_boxes.append(object_prediction[1:5])
-            pred_scores.append(object_prediction[-1])
-        label_classes = [class_names[label_idx-1] for label_idx in pred_labels]
-
-        gt_boxes, gt_labels = [], []
-        for object_gt in image_gt:
-            gt_labels.append(int(object_gt[0]))
-            gt_boxes.append(object_gt[1:5])
-
-        # ground truth bounding boxes
-        for gt_box in gt_boxes:
-            # TODO: replace with pointer to yellow in Fluent UI
-            color = (255, 255, 0)  # yellow in RGB
-            cv2.rectangle(
-                image,
-                (int(gt_box[0]), int(gt_box[1])),
-                (int(gt_box[2]), int(gt_box[3])),
-                color, thickness=2
-            )
-
-        # predicted bounding boxes & annotations
-        for k, pred_box in enumerate(pred_boxes):
-            color = tuple(colors[pred_labels[k]-1])
-            cv2.rectangle(
-                image,
-                (int(pred_box[0]), int(pred_box[1])),
-                (int(pred_box[2]), int(pred_box[3])),
-                color, thickness=3
-            )
-            label_text = str(k) + ". " + label_classes[k] + ' (' \
-                + str(round(pred_scores[k] * 100)) + '%)'
-            cv2.putText(image, label_text, (int(pred_box[0]),
-                                            int(pred_box[1]-5)),
-                        cv2.FONT_HERSHEY_SIMPLEX, 0.8, (0, 0, 0), 4,
-                        lineType=cv2.LINE_AA)
-            cv2.putText(image, label_text, (int(pred_box[0]),
-                                            int(pred_box[1]-5)),
-                        cv2.FONT_HERSHEY_SIMPLEX, 0.8, color, 2,
-                        lineType=cv2.LINE_AA)
-
-        return image
-
     def _convert_images(self, dataset):
         """Converts the images to the format required by the model.
 
         If the images are base64 encoded, they are decoded and converted to
         numpy arrays. If the images are already numpy arrays, they are
         returned as is.
 
@@ -981,15 +912,16 @@
             _TASK_TYPE: self.task_type,
             _CLASSES: classes,
             _IMAGE_MODE: self.image_mode,
             _FEATURE_METADATA: feature_metadata_dict,
             _IMAGE_WIDTH: self.image_width,
             _MAX_EVALS: self.max_evals,
             _NUM_MASKS: self.num_masks,
-            _MASK_RES: self.mask_res
+            _MASK_RES: self.mask_res,
+            _DEVICE: self.device
         }
         with open(top_dir / _META_JSON, 'w') as file:
             json.dump(meta, file)
 
     @staticmethod
     def _load_metadata(inst, path):
         """Load the metadata.
@@ -1006,16 +938,17 @@
         inst.__dict__[_TARGET_COLUMN] = meta[_TARGET_COLUMN]
         inst.__dict__[_TASK_TYPE] = meta[_TASK_TYPE]
         inst.__dict__[_IMAGE_MODE] = meta[_IMAGE_MODE]
         if _IMAGE_WIDTH in meta:
             inst.__dict__[_IMAGE_WIDTH] = meta[_IMAGE_WIDTH]
         else:
             inst.__dict__[_IMAGE_WIDTH] = None
-        params = [_MAX_EVALS, _NUM_MASKS, _MASK_RES]
-        defaults = [DEFAULT_MAX_EVALS, DEFAULT_NUM_MASKS, DEFAULT_MASK_RES]
+        params = [_MAX_EVALS, _NUM_MASKS, _MASK_RES, _DEVICE]
+        defaults = [DEFAULT_MAX_EVALS, DEFAULT_NUM_MASKS,
+                    DEFAULT_MASK_RES, Device.AUTO.value]
         for param, default in zip(params, defaults):
             if param in meta:
                 inst.__dict__[param] = meta[param]
             else:
                 inst.__dict__[param] = default
         classes = meta[_CLASSES]
 
@@ -1138,15 +1071,16 @@
             ManagerNames.ERROR_ANALYSIS: ErrorAnalysisManager,
         }
 
         # load current state
         RAIBaseInsights._load(
             path, inst, manager_map, RAIVisionInsights._load_metadata)
         inst._wrapped_model = wrap_model(inst.model, inst.test, inst.task_type,
-                                         classes=inst._classes)
+                                         classes=inst._classes,
+                                         device=inst.device)
         inst.automl_image_model = is_automl_image_model(inst._wrapped_model)
         inst.predict_output = None
         return inst
 
     def compute_object_detection_metrics(
             self,
             selection_indexes,
@@ -1156,15 +1090,15 @@
         dashboard_dataset = self.get_data().dataset
         true_y = dashboard_dataset.object_detection_true_y
         predicted_y = dashboard_dataset.object_detection_predicted_y
         dashboard_dataset = self.get_data().dataset
         true_y = dashboard_dataset.object_detection_true_y
         predicted_y = dashboard_dataset.object_detection_predicted_y
 
-        iou_thresh = [iou_thresh/100.0]
+        iou_thresh = [iou_thresh / 100.0]
         all_cohort_metrics = []
         for cohort_indices in selection_indexes:
             metric_OD = MeanAveragePrecision(
                 class_metrics=True,
                 iou_thresholds=iou_thresh,
                 average=aggregate_method)
             true_y_cohort = [true_y[cohort_index] for cohort_index
@@ -1199,15 +1133,15 @@
                 )
             ]
 
             # this is to find the class index given
             # that there might not all classes in the cohort to predict or gt
             classes = self._classes
             classes = list(classes)
-            cohort_classes = list(set([classes[i-1]
+            cohort_classes = list(set([classes[i - 1]
                                   for i in pred_labels + gt_labels]))
             cohort_classes.sort(
                 key=lambda class_name: classes.index(class_name))
             # to catch if the class is not in the cohort
             try:
                 index = cohort_classes.index(class_name)
             except ValueError:
```

### Comparing `responsibleai_vision-0.2.2/responsibleai_vision/utils/feature_extractors.py` & `responsibleai_vision-0.2.3/responsibleai_vision/utils/feature_extractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
 """Defines the feature extractors."""
 
+from typing import List, Optional
+
 import pandas as pd
 from tqdm import tqdm
-from typing import List, Optional
+
 from responsibleai_vision.utils.image_reader import get_image_from_path
 
 
 def extract_features(image_dataset: pd.DataFrame,
                      target_column: str, task_type: str,
                      image_mode: str = None,
                      dropped_features: Optional[List[str]] = None):
```

### Comparing `responsibleai_vision-0.2.2/responsibleai_vision/utils/image_reader.py` & `responsibleai_vision-0.2.3/responsibleai_vision/utils/image_reader.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.2/responsibleai_vision/utils/image_utils.py` & `responsibleai_vision-0.2.3/responsibleai_vision/utils/image_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
 """Contains image handling utilities."""
 
 import numpy as np
-from responsibleai_vision.utils.image_reader import get_image_from_path
+
 from responsibleai_vision.common.constants import ImageColumns
+from responsibleai_vision.utils.image_reader import get_image_from_path
 
 IMAGE = ImageColumns.IMAGE.value
 IMAGE_URL = ImageColumns.IMAGE_URL.value
 IMAGE_DETAILS = 'image_details'
 LABEL = 'label'
 WIDTH = 'width'
 HEIGHT = 'height'
```

### Comparing `responsibleai_vision-0.2.2/responsibleai_vision.egg-info/PKG-INFO` & `responsibleai_vision-0.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1
-Name: responsibleai-vision
-Version: 0.2.2
-Summary: SDK API to assess image Machine Learning models.
-Home-page: https://github.com/microsoft/responsible-ai-toolbox
-Author: Roman Lutz, Ilya Matiach, Ke Xu
-Author-email: raiwidgets-maintain@microsoft.com
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# Responsible AI Vision SDK for Python
-
-### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
-
-The Responsible AI Vision sdk enables users to analyze their machine learning models for computer vision in one API. Users will be able to analyze errors, explain the most important features, and understand their data using a single API.
-
-Highlights of the package include:
-
-- `explainer.add()` explains the model
-
-### Supported scenarios, models and datasets
-
-The Responsible AI Vision SDK supports multiclass classification models on image data currently.
-
-The open source code for the visualization dashboard can be found here:
-https://github.com/microsoft/responsible-ai-widgets
+Metadata-Version: 2.1
+Name: responsibleai_vision
+Version: 0.2.3
+Summary: SDK API to assess image Machine Learning models.
+Home-page: https://github.com/microsoft/responsible-ai-toolbox
+Author: Roman Lutz, Ilya Matiach, Ke Xu
+Author-email: raiwidgets-maintain@microsoft.com
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# Responsible AI Vision SDK for Python
+
+### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
+
+The Responsible AI Vision SDK enables users to analyze their machine learning models for computer vision in one API. Users will be able to analyze errors, explain the most important features, and understand their data using a single API.
+
+Highlights of the package include:
+
+- `explainer.add()` explains the model
+
+### Supported scenarios, models and datasets
+
+The Responsible AI Vision SDK supports multiclass classification models on image data currently.
+
+The open source code for the visualization dashboard can be found here:
+https://github.com/microsoft/responsible-ai-widgets
```

### Comparing `responsibleai_vision-0.2.2/responsibleai_vision.egg-info/SOURCES.txt` & `responsibleai_vision-0.2.3/responsibleai_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.2/setup.py` & `responsibleai_vision-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.2/tests/test_image_utils.py` & `responsibleai_vision-0.2.3/tests/test_image_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
-import numpy as np
 from math import isclose
 
+import numpy as np
+from common_vision_utils import load_fridge_object_detection_dataset
+
 from responsibleai_vision.common.constants import ImageColumns
 from responsibleai_vision.utils.image_utils import (
-    transform_object_detection_labels, WIDTH, HEIGHT, TOP_X, TOP_Y, BOTTOM_X,
-    BOTTOM_Y, IS_CROWD, classes_to_dict)
-from common_vision_utils import (
-    load_fridge_object_detection_dataset)
-
+    BOTTOM_X, BOTTOM_Y, HEIGHT, IS_CROWD, TOP_X, TOP_Y, WIDTH, classes_to_dict,
+    transform_object_detection_labels)
 
 LABEL = ImageColumns.LABEL.value
 IMAGE_DETAILS = ImageColumns.IMAGE_DETAILS.value
 TOL = 1
 
 
 class TestImageUtils(object):
```

### Comparing `responsibleai_vision-0.2.2/tests/test_rai_vision_automl_images_insights.py` & `responsibleai_vision-0.2.3/tests/test_rai_vision_automl_images_insights.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
-from responsibleai_vision import ModelTask
-from common_vision_utils import load_fridge_dataset
-from test_rai_vision_insights import run_rai_insights
-from responsibleai_vision.common.constants import ImageColumns
 import copy
+import json
 import os
+import sys
 import tempfile
-import json
-import torch
+
 import pytest
-import sys
+import torch
+from common_vision_utils import load_fridge_dataset
+from test_rai_vision_insights import run_rai_insights
+
+from responsibleai_vision import ModelTask
+from responsibleai_vision.common.constants import ImageColumns
 
 try:
-    import mlflow
     import azureml.automl.core.shared.constants as shared_constants
-    from azureml.automl.dnn.vision.classification.common.constants import (
-        ModelNames,
-    )
-    from azureml.automl.dnn.vision.classification.models import (
-        ModelFactory,
-    )
-    from azureml.automl.dnn.vision.common.mlflow.mlflow_model_wrapper \
-        import (
-            MLFlowImagesModelWrapper,
-            )
+    import mlflow
+    from azureml.automl.dnn.vision.classification.common.constants import \
+        ModelNames
+    from azureml.automl.dnn.vision.classification.models import ModelFactory
+    from azureml.automl.dnn.vision.common.mlflow.mlflow_model_wrapper import \
+        MLFlowImagesModelWrapper
     from azureml.automl.dnn.vision.common.model_export_utils import (
-        _get_mlflow_signature,
-        _get_scoring_method,
-    )
+        _get_mlflow_signature, _get_scoring_method)
 except Exception:
     pass
 
 
 def get_automl_images_mlflow_model(class_names):
     model_name = ModelNames.SERESNEXT
     multilabel = False
```

### Comparing `responsibleai_vision-0.2.2/tests/test_rai_vision_insights.py` & `responsibleai_vision-0.2.3/tests/test_rai_vision_insights.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
-import numpy as np
-import pytest
 import sys
+
+import numpy as np
 import PIL
+import pytest
+from common_vision_utils import (FRIDGE_MULTILABEL_TARGETS, ImageTransformEnum,
+                                 ImageTransforms, create_dummy_model,
+                                 create_image_classification_pipeline,
+                                 create_pytorch_vision_model,
+                                 gridify_fridge_multilabel_labels,
+                                 load_flowers_dataset, load_fridge_dataset,
+                                 load_fridge_object_detection_dataset,
+                                 load_imagenet_dataset, load_imagenet_labels,
+                                 load_mnist_dataset,
+                                 load_multilabel_fridge_dataset,
+                                 retrieve_fridge_object_detection_model,
+                                 retrieve_or_train_fridge_model)
+from ml_wrappers.common.constants import Device
+from rai_vision_insights_validator import validate_rai_vision_insights
 
 from responsibleai.feature_metadata import FeatureMetadata
-from responsibleai_vision import RAIVisionInsights, ModelTask
-from common_vision_utils import (
-    create_pytorch_vision_model,
-    gridify_fridge_multilabel_labels,
-    load_multilabel_fridge_dataset,
-    load_fridge_dataset, load_imagenet_dataset,
-    load_fridge_object_detection_dataset,
-    load_mnist_dataset,
-    create_image_classification_pipeline,
-    load_imagenet_labels, retrieve_or_train_fridge_model,
-    retrieve_fridge_object_detection_model,
-    FRIDGE_MULTILABEL_TARGETS,
-    ImageTransforms,
-    ImageTransformEnum,
-    load_flowers_dataset,
-    create_dummy_model)
-from responsibleai_vision.common.constants import (
-    ImageColumns, ExplainabilityDefaults)
-from rai_vision_insights_validator import validate_rai_vision_insights
+from responsibleai_vision import ModelTask, RAIVisionInsights
+from responsibleai_vision.common.constants import (ExplainabilityDefaults,
+                                                   ImageColumns)
 
 DEFAULT_MAX_EVALS = ExplainabilityDefaults.DEFAULT_MAX_EVALS
 DEFAULT_NUM_MASKS = ExplainabilityDefaults.DEFAULT_NUM_MASKS
 DEFAULT_MASK_RES = ExplainabilityDefaults.DEFAULT_MASK_RES
 
 
 class TestRAIVisionInsights(object):
@@ -136,14 +135,35 @@
         class_names = np.array(['can', 'carton',
                                 'milk_bottle', 'water_bottle'])
         with pytest.raises(ValueError,
                            match="mask_res must be greater than 0"):
             run_rai_insights(model, data[:1], ImageColumns.LABEL,
                              task_type, class_names, mask_res=mask_res)
 
+    @pytest.mark.parametrize('device', [None, 'cpu'])
+    def test_rai_insights_device(self, device):
+        data = load_fridge_object_detection_dataset()
+        model = retrieve_fridge_object_detection_model()
+        task_type = ModelTask.OBJECT_DETECTION
+        class_names = np.array(['can', 'carton',
+                                'milk_bottle', 'water_bottle'])
+        run_rai_insights(model, data[:1], ImageColumns.LABEL,
+                         task_type, class_names, device=device)
+
+    @pytest.mark.parametrize('device', ["bad_device", ""])
+    def test_rai_insights_invalid_device(self, device):
+        data = load_fridge_object_detection_dataset()
+        model = retrieve_fridge_object_detection_model()
+        task_type = ModelTask.OBJECT_DETECTION
+        class_names = np.array(['can', 'carton',
+                                'milk_bottle', 'water_bottle'])
+        with pytest.raises(ValueError, match="Selected device is invalid"):
+            run_rai_insights(model, data[:1], ImageColumns.LABEL,
+                             task_type, class_names, device=device)
+
     @pytest.mark.skip("This test fails in the build due to \
                       incompatibility between fastai and pytorch \
                       2.0.0. TODO: fix may be to ping pytorch <2.0.0 \
                       in the build until fastai updates.")
     def test_rai_insights_object_detection_fridge_label_format(self):
         data = load_fridge_object_detection_dataset()
         model = retrieve_fridge_object_detection_model()
@@ -231,15 +251,16 @@
 
 def run_rai_insights(model, test_data, target_column,
                      task_type, classes=None, test_explainer=False,
                      test_error_analysis=False,
                      image_mode=None, dropped_features=None,
                      upscale=False, max_evals=DEFAULT_MAX_EVALS,
                      num_masks=DEFAULT_NUM_MASKS,
-                     mask_res=DEFAULT_MASK_RES):
+                     mask_res=DEFAULT_MASK_RES,
+                     device=Device.AUTO.value):
     feature_metadata = None
     if dropped_features:
         feature_metadata = FeatureMetadata(dropped_features=dropped_features)
     image_width = None
     if upscale:
         image_width = 2
     rai_insights = RAIVisionInsights(model, test_data,
@@ -247,15 +268,16 @@
                                      task_type=task_type,
                                      classes=classes,
                                      image_mode=image_mode,
                                      feature_metadata=feature_metadata,
                                      image_width=image_width,
                                      max_evals=max_evals,
                                      num_masks=num_masks,
-                                     mask_res=mask_res)
+                                     mask_res=mask_res,
+                                     device=device)
     # Note: this seems too resource-intensive
     # TODO: re-add when we get beefier test machines
     if test_explainer:
         rai_insights.explainer.add()
     if test_error_analysis:
         rai_insights.error_analysis.add()
     if test_explainer or test_error_analysis:
```

### Comparing `responsibleai_vision-0.2.2/tests/test_rai_vision_insights_save_and_load_scenarios.py` & `responsibleai_vision-0.2.3/tests/test_rai_vision_insights_save_and_load_scenarios.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
+import shutil
 from pathlib import Path
 from tempfile import TemporaryDirectory
-import PIL
 
+import PIL
 import pytest
-import shutil
-
-from responsibleai_vision import RAIVisionInsights, ModelTask
-from responsibleai_vision.common.constants import ImageColumns
+from common_vision_utils import (DummyFlowersPipelineSerializer,
+                                 ImageClassificationPipelineSerializer,
+                                 create_dummy_model,
+                                 create_image_classification_pipeline,
+                                 load_flowers_dataset, load_imagenet_dataset,
+                                 load_imagenet_labels)
 from rai_vision_insights_validator import run_and_validate_serialization
 
-from common_vision_utils import (
-    load_imagenet_dataset,
-    create_image_classification_pipeline,
-    load_imagenet_labels,
-    ImageClassificationPipelineSerializer,
-    load_flowers_dataset,
-    DummyFlowersPipelineSerializer,
-    create_dummy_model)
+from responsibleai_vision import ModelTask, RAIVisionInsights
+from responsibleai_vision.common.constants import ImageColumns
 
 
 class TestRAIVisionInsightsSaveAndLoadScenarios(object):
 
     def test_rai_insights_empty_save_load_save(self):
         data = load_imagenet_dataset()
         pred = create_image_classification_pipeline()
```

