# Comparing `tmp/responsibleai_text-0.1.3.tar.gz` & `tmp/responsibleai_text-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/responsibleai_text-0.1.3.tar", last modified: Tue May 30 14:50:22 2023, max compression
+gzip compressed data, was "responsibleai_text-0.1.4.tar", last modified: Mon Jul  3 21:18:05 2023, max compression
```

## Comparing `responsibleai_text-0.1.3.tar` & `responsibleai_text-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text/common/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/common/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/managers/error_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/managers/explainer_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text/rai_text_insights/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/rai_text_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34598 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/rai_text_insights/rai_text_insights.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/utils/feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/utils/question_answering.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/responsibleai_text/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/responsibleai_text.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:50:22.000000 responsibleai_text-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/tests/test_feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/tests/test_rai_text_insights.py
--rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-05-30 14:47:39.000000 responsibleai_text-0.1.3/tests/test_rai_text_insights_save_and_load_scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:18:05.499501 responsibleai_text-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-03 21:18:05.499501 responsibleai_text-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:18:05.495501 responsibleai_text-0.1.4/responsibleai_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/responsibleai_text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:18:05.495501 responsibleai_text-0.1.4/responsibleai_text/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/responsibleai_text/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/responsibleai_text/common/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:18:05.495501 responsibleai_text-0.1.4/responsibleai_text/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/responsibleai_text/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/responsibleai_text/managers/error_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/responsibleai_text/managers/explainer_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:18:05.495501 responsibleai_text-0.1.4/responsibleai_text/rai_text_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/responsibleai_text/rai_text_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34898 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/responsibleai_text/rai_text_insights/rai_text_insights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:18:05.499501 responsibleai_text-0.1.4/responsibleai_text/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/responsibleai_text/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/responsibleai_text/utils/feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/responsibleai_text/utils/question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/responsibleai_text/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:18:05.495501 responsibleai_text-0.1.4/responsibleai_text.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-03 21:18:05.000000 responsibleai_text-0.1.4/responsibleai_text.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-03 21:18:05.000000 responsibleai_text-0.1.4/responsibleai_text.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 21:18:05.000000 responsibleai_text-0.1.4/responsibleai_text.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 21:18:05.000000 responsibleai_text-0.1.4/responsibleai_text.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 21:18:05.000000 responsibleai_text-0.1.4/responsibleai_text.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 21:18:05.499501 responsibleai_text-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:18:05.499501 responsibleai_text-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/tests/test_feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/tests/test_rai_text_insights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-07-03 21:15:08.000000 responsibleai_text-0.1.4/tests/test_rai_text_insights_save_and_load_scenarios.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `responsibleai_text-0.1.3/PKG-INFO` & `responsibleai_text-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_text
-Version: 0.1.3
+Version: 0.1.4
 Summary: SDK API to assess text Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_text-0.1.3/README.md` & `responsibleai_text-0.1.4/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 - `explainer.add()` explains the model
 
 ### Supported scenarios, models and datasets
 
 The Responsible AI Text SDK supports multiclass classification and question answering models on text data currently.
 
 The open source code for the visualization dashboard can be found here:
-https://github.com/microsoft/responsible-ai-toolbox
+https://github.com/microsoft/responsible-ai-toolbox
```

### Comparing `responsibleai_text-0.1.3/responsibleai_text/common/constants.py` & `responsibleai_text-0.1.4/responsibleai_text/common/constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.3/responsibleai_text/managers/error_analysis_manager.py` & `responsibleai_text-0.1.4/responsibleai_text/managers/error_analysis_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 import json
 from typing import Any, List, Optional, Union
 
 import jsonschema
 import numpy as np
 import pandas as pd
+from ml_wrappers import wrap_model
+
 from erroranalysis._internal.error_analyzer import ModelAnalyzer
 from erroranalysis._internal.error_report import as_error_report
-from ml_wrappers import wrap_model
 from responsibleai._tools.shared.state_directory_management import \
     DirectoryManager
 from responsibleai.managers.error_analysis_manager import \
     ErrorAnalysisManager as BaseErrorAnalysisManager
 from responsibleai.managers.error_analysis_manager import as_error_config
-
 from responsibleai_text.common.constants import ModelTask
 from responsibleai_text.utils.feature_extractors import get_text_columns
 
 LABELS = 'labels'
 
 
 def _concat_labels_column(dataset, target_column, classes):
@@ -33,15 +33,15 @@
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
@@ -63,20 +63,23 @@
         :type classes: list
         """
         self.model = model
         self.dataset = dataset
         self.classes = classes
         self.is_multilabel = is_multilabel
         self.task_type = task_type
-        if self.task_type in [ModelTask.TEXT_CLASSIFICATION, ModelTask.MULTILABEL_TEXT_CLASSIFICATION]:
+        classif_tasks = [ModelTask.TEXT_CLASSIFICATION,
+                         ModelTask.MULTILABEL_TEXT_CLASSIFICATION]
+        if self.task_type in classif_tasks:
             dataset = self.dataset.iloc[:, 0].tolist()
             self.predictions = self.model.predict(dataset)
             self.predict_proba = self.model.predict_proba(dataset)
         elif self.task_type == ModelTask.QUESTION_ANSWERING:
-            self.predictions = self.model.predict(self.dataset.loc[:, ['context', 'questions']])
+            self.predictions = self.model.predict(
+                self.dataset.loc[:, ['context', 'questions']])
             self.predictions = np.array(self.predictions)
         else:
             raise ValueError("Unknown task type: {}".format(self.task_type))
 
         if self.is_multilabel:
             predictions_joined = []
             for row in self.predictions:
```

### Comparing `responsibleai_text-0.1.3/responsibleai_text/managers/explainer_manager.py` & `responsibleai_text-0.1.4/responsibleai_text/managers/explainer_manager.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 import warnings
 from pathlib import Path
 from typing import Any, List, Optional
 
 import numpy as np
 import pandas as pd
 import shap
+
 from raiutils.data_processing import convert_to_list
 from responsibleai._interfaces import (FeatureImportance, ModelExplanationData,
                                        PrecomputedExplanations,
                                        TextFeatureImportance)
 from responsibleai._internal.constants import ExplainerManagerKeys as Keys
 from responsibleai._internal.constants import (ListProperties, ManagerNames,
                                                Metadata)
 from responsibleai._tools.shared.state_directory_management import \
     DirectoryManager
 from responsibleai.exceptions import UserConfigValidationException
 from responsibleai.managers.base_manager import BaseManager
-
 from responsibleai_text.common.constants import (ModelTask,
                                                  QuestionAnsweringFields,
                                                  Tokens)
 from responsibleai_text.utils.question_answering import QAPredictor
 
 CONTEXT = QuestionAnsweringFields.CONTEXT
 QUESTIONS = QuestionAnsweringFields.QUESTIONS
```

### Comparing `responsibleai_text-0.1.3/responsibleai_text/rai_text_insights/rai_text_insights.py` & `responsibleai_text-0.1.4/responsibleai_text/rai_text_insights/rai_text_insights.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 import warnings
 from enum import Enum
 from pathlib import Path
 from typing import Any, List, Optional, Union
 
 import numpy as np
 import pandas as pd
-from erroranalysis._internal.cohort_filter import FilterDataWithCohortFilters
 from ml_wrappers import wrap_model
+
+from erroranalysis._internal.cohort_filter import FilterDataWithCohortFilters
 from raiutils.data_processing import convert_to_list, serialize_json_safe
 from raiutils.models import SKLearn, is_classifier
 from responsibleai._interfaces import Dataset, RAIInsightsData
 from responsibleai._internal.constants import (ManagerNames, Metadata,
                                                SerializationAttributes)
 from responsibleai.exceptions import UserConfigValidationException
 from responsibleai.feature_metadata import FeatureMetadata
 from responsibleai.rai_insights.rai_base_insights import RAIBaseInsights
-
 from responsibleai_text.common.constants import ModelTask
 from responsibleai_text.managers.error_analysis_manager import \
     ErrorAnalysisManager
 from responsibleai_text.managers.explainer_manager import ExplainerManager
 from responsibleai_text.utils.feature_extractors import (extract_features,
                                                          get_text_columns)
 
@@ -369,15 +369,16 @@
                         target_column)
                 )
 
         if text_column:
             if task_type == ModelTask.QUESTION_ANSWERING.value:
                 if not isinstance(text_column, list):
                     raise UserConfigValidationException(
-                        'The text_column should be a list for question answering')
+                        'The text_column should be a list for question ' +
+                        'answering')
                 text_columns_set = set(text_column)
                 if not text_columns_set.issubset(set(test.columns)):
                     raise UserConfigValidationException(
                         'The list of text_column(s) should be in test data')
             else:
                 if text_column not in test.columns:
                     raise UserConfigValidationException(
@@ -752,15 +753,24 @@
         # load current state
         RAIBaseInsights._load(path, inst, manager_map,
                               RAITextInsights._load_metadata)
         inst._wrapped_model = wrap_model(inst.model, inst.test, inst.task_type)
         return inst
 
     def normalize_text(self, s):
-        """Removing articles and punctuation, and standardizing whitespace are all typical text processing steps."""
+        """Normalize the text.
+
+        Removing articles and punctuation, and standardizing whitespace
+        are all typical text processing steps.
+
+        :param s: The text to normalize.
+        :type s: str
+        :return: The normalized text.
+        :rtype: str
+        """
         import re
         import string
 
         def remove_articles(text):
             regex = re.compile(r"\b(a|an|the)\b", re.UNICODE)
             return re.sub(regex, " ", text)
 
@@ -776,15 +786,16 @@
 
         return white_space_fix(remove_articles(remove_punc(lower(s))))
 
     def compute_f1(self, prediction, truth):
         pred_tokens = self.normalize_text(prediction).split()
         truth_tokens = self.normalize_text(truth).split()
 
-        # if either the prediction or the truth is no-answer then f1 = 1 if they agree, 0 otherwise
+        # if either the prediction or the truth is no-answer
+        # then f1 = 1 if they agree, 0 otherwise
         if len(pred_tokens) == 0 or len(truth_tokens) == 0:
             return int(pred_tokens == truth_tokens)
 
         common_tokens = set(pred_tokens) & set(truth_tokens)
 
         # if there are no common tokens then f1 = 0
         if len(common_tokens) == 0:
@@ -803,27 +814,34 @@
         for cohort_indices in selection_indexes:
             true_y_cohort = [true_y[cohort_index] for cohort_index
                              in cohort_indices]
             predicted_y_cohort = [predicted_y[cohort_index] for cohort_index
                                   in cohort_indices]
             f1_score = []
             for cohort_index in cohort_indices:
-                f1_score.append(self.compute_f1(predicted_y[cohort_index], true_y[cohort_index]))
+                f1_score.append(self.compute_f1(predicted_y[cohort_index],
+                                                true_y[cohort_index]))
             try:
                 exact_match = evaluate.load('exact_match')
-                exact_match_results = exact_match.compute(predictions=predicted_y_cohort, references=true_y_cohort)
+                exact_match_results = exact_match.compute(
+                    predictions=predicted_y_cohort, references=true_y_cohort)
                 rouge = evaluate.load('rouge')
-                rouge_results = rouge.compute(predictions=predicted_y_cohort, references=true_y_cohort)
+                rouge_results = rouge.compute(
+                    predictions=predicted_y_cohort, references=true_y_cohort)
                 bleu = evaluate.load('bleu')
-                bleu_results = bleu.compute(predictions=predicted_y_cohort, references=true_y_cohort)
+                bleu_results = bleu.compute(
+                    predictions=predicted_y_cohort, references=true_y_cohort)
                 meteor = evaluate.load('meteor')
-                meteor_results = meteor.compute(predictions=predicted_y_cohort, references=true_y_cohort)
+                meteor_results = meteor.compute(
+                    predictions=predicted_y_cohort, references=true_y_cohort)
                 bert_score = evaluate.load('bertscore')
-                bert_score_results = bert_score.compute(predictions=predicted_y_cohort, references=true_y_cohort,
-                                                        model_type="distilbert-base-uncased")
+                bert_score_results = bert_score.compute(
+                    predictions=predicted_y_cohort, references=true_y_cohort,
+                    model_type="distilbert-base-uncased")
                 bert_f1_score = np.mean(bert_score_results['f1'])
-                all_cohort_metrics.append([exact_match_results['exact_match'], np.mean(f1_score),
-                                           meteor_results['meteor'], bleu_results['bleu'], bert_f1_score,
-                                           rouge_results['rougeL']])
+                all_cohort_metrics.append(
+                    [exact_match_results['exact_match'], np.mean(f1_score),
+                     meteor_results['meteor'], bleu_results['bleu'],
+                     bert_f1_score, rouge_results['rougeL']])
             except ValueError:
                 all_cohort_metrics.append([0, 0, 0, 0, 0, 0])
         return all_cohort_metrics
```

### Comparing `responsibleai_text-0.1.3/responsibleai_text/utils/feature_extractors.py` & `responsibleai_text-0.1.4/responsibleai_text/utils/feature_extractors.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 import re
 from typing import List, Optional, Union
 
 import pandas as pd
 import spacy
 from negspacy.termsets import termset
-from nlp_feature_extractors import attribute_extractors as exts
 from tqdm import tqdm
 
+from nlp_feature_extractors import attribute_extractors as exts
 from responsibleai_text.common.constants import (ModelTask,
                                                  QuestionAnsweringFields)
 
 nlp = None
 
 
 def extract_features(text_dataset: pd.DataFrame,
@@ -81,20 +81,24 @@
                                    extracted_features, has_dropped_features,
                                    dropped_features, column_names)
             results.append(extracted_features)
     elif task_type == ModelTask.QUESTION_ANSWERING:
         for i, row in tqdm(text_features.iterrows()):
             extracted_features = []
             add_extracted_features_for_sentence(
-                row[QuestionAnsweringFields.CONTEXT], extracted_features, task_type)
+                row[QuestionAnsweringFields.CONTEXT], extracted_features,
+                task_type)
             add_extracted_features_for_sentence(
-                row[QuestionAnsweringFields.QUESTIONS], extracted_features, task_type, sentence_type="QUESTION")
+                row[QuestionAnsweringFields.QUESTIONS], extracted_features,
+                task_type, sentence_type="QUESTION")
 
-            context_overlap = get_context_overlap(context=row[QuestionAnsweringFields.CONTEXT],
-                                                  question=row[QuestionAnsweringFields.QUESTIONS])
+            context = row[QuestionAnsweringFields.CONTEXT]
+            question = row[QuestionAnsweringFields.QUESTIONS]
+            context_overlap = get_context_overlap(context=context,
+                                                  question=question)
             extracted_features.append(context_overlap)
             # append all other metadata features
             append_metadata_values(start_meta_index, text_dataset, i,
                                    extracted_features, has_dropped_features,
                                    dropped_features, column_names)
             results.append(extracted_features)
     else:
@@ -153,15 +157,16 @@
     if text_exists and num_cols - text_cols > 0:
         if not is_list:
             text_column = [text_column]
         text_dataset = text_dataset[text_column]
     return text_dataset
 
 
-def add_extracted_features_for_sentence(sentence, extracted_features, task_type=None, sentence_type=None):
+def add_extracted_features_for_sentence(sentence, extracted_features,
+                                        task_type=None, sentence_type=None):
     """Add the extracted features for a sentence.
 
     Note this also modifies the input array in-place.
 
     :param sentence: The sentence to extract features from.
     :type sentence: str
     :param extracted_features: The list of extracted features.
@@ -209,38 +214,41 @@
     """Get the question type.
 
     :param qtext: The question text.
     :type qtext: str
     :return: The question type.
     :rtype: str
     """
-    if re.search(r'\b\A(can|could|will|would|have|has|do|does|did|is|are|was|may|might)\s',
-                 qtext, re.I):
+    if re.search(r'\b\A(can|could|will|would|have|has' +
+                 r'|do|does|did|is|are|was|may|might)\s', qtext, re.I):
         return "YES/NO"
     elif re.search(r'\b\A(what|which)(\'s|\'re)?\s+(\w+)', qtext, re.I):
-        nextword = re.search(r'\b\A(what|which)(\'s|\'re)?\s+(\w+)', qtext, re.I).group(3)
+        nextword = re.search(r'\b\A(what|which)(\'s|\'re)?\s+(\w+)',
+                             qtext, re.I).group(3)
         if nextword in ["year", "month", "date", "day"]:
             return "WHEN"
         else:
             return "WHAT"
     elif re.search(r'\bwho(\'s|\'re)?\s', qtext, re.I):
         return "WHO"
     elif re.search(r'\bwhy(\'s|\'re)?\s', qtext, re.I):
         return "WHY"
     elif re.search(r'\bwhere(\'s|\'re)?\s', qtext, re.I):
         return "WHERE"
     elif re.search(r'\bhow(\'s|\'re)?\s', qtext, re.I):
-        nextword = re.search(r'\b(how)(\'s|\'re)?\s(\w+)', qtext, re.I).group(3)
+        nextword = re.search(r'\b(how)(\'s|\'re)?\s(\w+)',
+                             qtext, re.I).group(3)
         if nextword in ["many", "much", "long", "old", "often"]:
             return "NUMBER"
         else:
             return "HOW"
     elif re.search(r'\bwhen(\'s|\'re)?\s', qtext, re.I):
         return "WHEN"
-    elif re.search(r'\b(in|on|at|by|for|to|from|during|within)\s+(what|which)\s+(year|month|day|date|time)\s',
+    elif re.search(r'\b(in|on|at|by|for|to|from|during|within)' +
+                   r'\s+(what|which)\s+(year|month|day|date|time)\s',
                    qtext, re.I):
         return "WHEN"
     elif re.search(r'\bto\swhom\s', qtext, re.I):
         return "WHO"
     else:
         return "OTHER"
 
@@ -269,15 +277,15 @@
     """
     roots = []
     for each in doc.sents:
         roots.append([token for token in each if token.head == token][0])
 
     parse_tree_depths = [get_parse_tree_depth(root) for root in roots]
 
-    return sum(parse_tree_depths)/len(parse_tree_depths)
+    return sum(parse_tree_depths) / len(parse_tree_depths)
 
 
 def get_max_depth(doc):
     """Get the maximum parse tree depth.
 
     :param doc: The document to process.
     :type doc: spacy.tokens.doc.Doc
@@ -287,14 +295,25 @@
     roots = []
     for each in doc.sents:
         roots.append([token for token in each if token.head == token][0])
 
     return max([get_parse_tree_depth(root) for root in roots])
 
 
+def is_base_token(token):
+    """Check if the token is a base token.
+
+    :param token: The token.
+    :type token: spacy.tokens.token.Token
+    :return: True if the token is a base token, False otherwise.
+    :rtype: bool
+    """
+    return not token.is_stop and not token.is_punct
+
+
 def get_context_overlap(context, question):
     """Get the context overlap.
 
     :param context: The context.
     :type context: str
     :param question: The question.
     :type question: str
@@ -305,16 +324,16 @@
     if nlp is None:
         nlp = spacy.load("en_core_web_sm")
 
     doc_q = nlp(question)
     doc_c = nlp(context)
 
     # get tokens in base form
-    tokens_q = set([token.lemma_ for token in doc_q if not token.is_stop and not token.is_punct])
-    tokens_c = set([token.lemma_ for token in doc_c if not token.is_stop and not token.is_punct])
+    tokens_q = set([token.lemma_ for token in doc_q if is_base_token(token)])
+    tokens_c = set([token.lemma_ for token in doc_c if is_base_token(token)])
 
     intersection = tokens_q.intersection(tokens_c)
 
-    # the size of the intersection token set /  the size of the question token set
+    # size of intersection token set / size of question token set
     overlap_ratio = len(intersection) / len(tokens_q)
 
     return round(overlap_ratio, 3)
```

### Comparing `responsibleai_text-0.1.3/responsibleai_text/utils/question_answering.py` & `responsibleai_text-0.1.4/responsibleai_text/utils/question_answering.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.3/responsibleai_text.egg-info/PKG-INFO` & `responsibleai_text-0.1.4/responsibleai_text.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai-text
-Version: 0.1.3
+Version: 0.1.4
 Summary: SDK API to assess text Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_text-0.1.3/responsibleai_text.egg-info/SOURCES.txt` & `responsibleai_text-0.1.4/responsibleai_text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.3/setup.py` & `responsibleai_text-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.1.3/tests/test_feature_extractors.py` & `responsibleai_text-0.1.4/tests/test_feature_extractors.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,45 +13,79 @@
 
 
 class TestFeatureExtractors(object):
 
     def test_question_type_extractor(self):
         # part of questions are from SQuAD 2.0 dev set article: Steam_engine
         test_data = [
-            {"question": "On what date did the first railway trip in the world occur?", "type": "WHEN"},
-            {"question": "When were attempts made to overcome stationary marketplaces?", "type": "WHEN"},
-            {"question": "What year saw the earliest recorded use of the steam engine indicator?", "type": "WHEN"},
-            {"question": "Where did the world's first railway journey terminate?", "type": "WHERE"},
-            {"question": "How many expansion stages are used by the triple expansion engine?", "type": "NUMBER"},
-            {"question": "Who was the inventor of the atmospheric engine?", "type": "WHO"},
-            {"question": "What types of engines are steam engines?", "type": "WHAT"},
-            {"question": "What's another term for the pivot mounting?", "type": "WHAT"},
-            {"question": "Why the Rankine cycle is often used as a bottoming cycle?", "type": "WHY"},
-            {"question": "Will this extractor work as expected?", "type": "YES/NO"},
+            {"question":
+             "On what date did the first railway trip in the world occur?",
+             "type": "WHEN"},
+            {"question":
+             "When were attempts made to overcome stationary marketplaces?",
+             "type": "WHEN"},
+            {"question":
+             "What year saw the earliest recorded use of the " +
+             "steam engine indicator?",
+             "type": "WHEN"},
+            {"question":
+             "Where did the world's first railway journey terminate?",
+             "type": "WHERE"},
+            {"question":
+             "How many expansion stages are used by the triple " +
+             "expansion engine?",
+             "type": "NUMBER"},
+            {"question":
+             "Who was the inventor of the atmospheric engine?",
+             "type": "WHO"},
+            {"question":
+             "What types of engines are steam engines?",
+             "type": "WHAT"},
+            {"question":
+             "What's another term for the pivot mounting?",
+             "type": "WHAT"},
+            {"question":
+             "Why the Rankine cycle is often used as a bottoming cycle?",
+             "type": "WHY"},
+            {"question":
+             "Will this extractor work as expected?",
+             "type": "YES/NO"},
             {"question": "Any questions?", "type": "OTHER"},
         ]
         for data in test_data:
             assert data["type"] == get_question_type(data["question"])
 
     def test_context_overlap_extractor(self):
         # from SQuAD 2.0 dev set article: Steam_engine
         test_context = '''
             Steam engines are external combustion engines,
-            where the working fluid is separate from the combustion products.
-            Non-combustion heat sources such as solar power, nuclear power or geothermal energy may be used.
-            The ideal thermodynamic cycle used to analyze this process is called the Rankine cycle.
-            In the cycle, water is heated and transforms into steam within a boiler operating at a high pressure.
-            When expanded through pistons or turbines, mechanical work is done.
-            The reduced-pressure steam is then condensed and pumped back into the boiler.
+            where the working fluid is separate from the
+            combustion products.
+            Non-combustion heat sources such as solar power,
+            nuclear power or geothermal energy may be used.
+            The ideal thermodynamic cycle used to analyze this
+            process is called the Rankine cycle.
+            In the cycle, water is heated and transforms into steam
+            within a boiler operating at a high pressure.
+            When expanded through pistons or turbines, mechanical
+            work is done.
+            The reduced-pressure steam is then condensed and pumped
+            back into the boiler.
         '''
 
         test_data = [
             {
-                "question": "At what pressure is water heated in the Rankine cycle?",
+                "question":
+                "At what pressure is water heated in the Rankine cycle?",
                 "context_overlap": 1.0
             },
-            {"question": "What types of engines are steam engines?", "context_overlap": 0.667},
-            {"question": "Which part of the immune system protects the brain?", "context_overlap": 0.0},
+            {"question": "What types of engines are steam engines?",
+             "context_overlap": 0.667},
+            {"question":
+             "Which part of the immune system protects the brain?",
+             "context_overlap": 0.0},
         ]
 
         for data in test_data:
-            assert data["context_overlap"] == get_context_overlap(test_context, data["question"])
+            context_overlap = get_context_overlap(
+                test_context, data["question"])
+            assert data["context_overlap"] == context_overlap
```

### Comparing `responsibleai_text-0.1.3/tests/test_rai_text_insights.py` & `responsibleai_text-0.1.4/tests/test_rai_text_insights.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
                                create_multilabel_pipeline,
                                create_question_answering_pipeline,
                                create_text_classification_pipeline,
                                load_blbooks_genre_dataset,
                                load_covid19_emergency_event_dataset,
                                load_emotion_dataset, load_squad_dataset)
 from rai_text_insights_validator import validate_rai_text_insights
-from responsibleai.feature_metadata import FeatureMetadata
 
+from responsibleai.feature_metadata import FeatureMetadata
 from responsibleai_text import ModelTask, RAITextInsights
 
 
 class TestRAITextInsights(object):
 
     def test_rai_insights_emotion_classification(self):
         data = load_emotion_dataset()
```

### Comparing `responsibleai_text-0.1.3/tests/test_rai_text_insights_save_and_load_scenarios.py` & `responsibleai_text-0.1.4/tests/test_rai_text_insights_save_and_load_scenarios.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
                                MultilabelTextClassificationSerializer,
                                TextClassificationPipelineSerializer,
                                create_multilabel_pipeline,
                                create_text_classification_pipeline,
                                load_covid19_emergency_event_dataset,
                                load_emotion_dataset)
 from rai_text_insights_validator import validate_rai_text_insights
+
 from responsibleai._internal.constants import ManagerNames
 from responsibleai.feature_metadata import FeatureMetadata
-
 from responsibleai_text import ModelTask, RAITextInsights
 
 
 class TestRAITextInsightsSaveAndLoadScenarios(object):
 
     def test_rai_insights_empty_save_load_save(self):
         data = load_emotion_dataset()
```

