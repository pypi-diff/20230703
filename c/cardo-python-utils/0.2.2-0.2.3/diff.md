# Comparing `tmp/cardo-python-utils-0.2.2.tar.gz` & `tmp/cardo-python-utils-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardo-python-utils-0.2.2.tar", last modified: Mon Jun 12 10:11:27 2023, max compression
+gzip compressed data, was "cardo-python-utils-0.2.3.tar", last modified: Mon Jul  3 15:47:26 2023, max compression
```

## Comparing `cardo-python-utils-0.2.2.tar` & `cardo-python-utils-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-12 10:11:27.452061 cardo-python-utils-0.2.2/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/LICENSE
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       60 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/MANIFEST.in
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-06-12 10:11:27.452061 cardo-python-utils-0.2.2/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1114 2023-06-09 16:11:25.000000 cardo-python-utils-0.2.2/README.rst
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-12 10:11:27.448061 cardo-python-utils-0.2.2/cardo_python_utils.egg-info/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-06-12 10:11:27.000000 cardo-python-utils-0.2.2/cardo_python_utils.egg-info/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      610 2023-06-12 10:11:27.000000 cardo-python-utils-0.2.2/cardo_python_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-06-12 10:11:27.000000 cardo-python-utils-0.2.2/cardo_python_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      187 2023-06-12 10:11:27.000000 cardo-python-utils-0.2.2/cardo_python_utils.egg-info/requires.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       13 2023-06-12 10:11:27.000000 cardo-python-utils-0.2.2/cardo_python_utils.egg-info/top_level.txt
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-12 10:11:27.452061 cardo-python-utils-0.2.2/python_utils/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1949 2023-06-09 16:10:08.000000 cardo-python-utils-0.2.2/python_utils/choices.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16820 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/data_structures.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      455 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/db.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    17515 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/django_utils.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    14437 2023-06-12 10:10:18.000000 cardo-python-utils-0.2.2/python_utils/esma_choices.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      751 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/exceptions.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      913 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/imports.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5603 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/math.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6159 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/pandas_utils.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1290 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/rest.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3740 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/text.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     9614 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/time.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      120 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/types_hinting.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1137 2023-06-12 10:11:27.452061 cardo-python-utils-0.2.2/setup.cfg
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      142 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/setup.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-03 15:47:26.026253 cardo-python-utils-0.2.3/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/LICENSE
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       60 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/MANIFEST.in
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-07-03 15:47:26.026253 cardo-python-utils-0.2.3/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1114 2023-06-09 16:11:25.000000 cardo-python-utils-0.2.3/README.rst
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-03 15:47:26.026253 cardo-python-utils-0.2.3/cardo_python_utils.egg-info/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-07-03 15:47:26.000000 cardo-python-utils-0.2.3/cardo_python_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      610 2023-07-03 15:47:26.000000 cardo-python-utils-0.2.3/cardo_python_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-07-03 15:47:26.000000 cardo-python-utils-0.2.3/cardo_python_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      187 2023-07-03 15:47:26.000000 cardo-python-utils-0.2.3/cardo_python_utils.egg-info/requires.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       13 2023-07-03 15:47:26.000000 cardo-python-utils-0.2.3/cardo_python_utils.egg-info/top_level.txt
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-07-03 15:47:26.026253 cardo-python-utils-0.2.3/python_utils/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1949 2023-06-09 16:10:08.000000 cardo-python-utils-0.2.3/python_utils/choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16820 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/data_structures.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      455 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/db.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    17515 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/django_utils.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    15143 2023-07-03 15:47:15.000000 cardo-python-utils-0.2.3/python_utils/esma_choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      751 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/exceptions.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      913 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/imports.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5603 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/math.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6159 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/pandas_utils.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1290 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/rest.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3740 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/text.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     9614 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/time.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      120 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/python_utils/types_hinting.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1137 2023-07-03 15:47:26.026253 cardo-python-utils-0.2.3/setup.cfg
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      142 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.3/setup.py
```

### Comparing `cardo-python-utils-0.2.2/LICENSE` & `cardo-python-utils-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.2/PKG-INFO` & `cardo-python-utils-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardo-python-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python library enhanced with a wide range of functions for different scenarios.
 Home-page: https://github.com/CardoAI/cardo-python-utils
 Author: Kristi Kotini
 Author-email: hello@cardoai.com
 License: MIT (X11)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `cardo-python-utils-0.2.2/README.rst` & `cardo-python-utils-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.2/cardo_python_utils.egg-info/PKG-INFO` & `cardo-python-utils-0.2.3/cardo_python_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardo-python-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python library enhanced with a wide range of functions for different scenarios.
 Home-page: https://github.com/CardoAI/cardo-python-utils
 Author: Kristi Kotini
 Author-email: hello@cardoai.com
 License: MIT (X11)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `cardo-python-utils-0.2.2/cardo_python_utils.egg-info/SOURCES.txt` & `cardo-python-utils-0.2.3/cardo_python_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.2/python_utils/choices.py` & `cardo-python-utils-0.2.3/python_utils/choices.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.2/python_utils/data_structures.py` & `cardo-python-utils-0.2.3/python_utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.2/python_utils/django_utils.py` & `cardo-python-utils-0.2.3/python_utils/django_utils.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.2/python_utils/esma_choices.py` & `cardo-python-utils-0.2.3/python_utils/esma_choices.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,19 +145,19 @@
     EEMO = 5, "Existing customer and an employee/affiliated with the originator's group"
     ENRO = 6, "Existing customer and employee/affiliation not recorded"
     OTHR = 10, "Other"
 
 
 class ESMAAmortisationTypeChoices(ChoiceEnum):
     FRXX = 1, "French - i.e. Amortisation in which the total amount — principal plus interest — repaid in each " \
-                "instalment is the same."
+              "instalment is the same."
     DEXX = 2, "German - i.e. Amortisation in which the first instalment is interest-only and the remaining " \
-                "instalments are constant, including capital amortisation and interest."
+              "instalments are constant, including capital amortisation and interest."
     FIXE = 3, "Fixed amortisation schedule - i.e. Amortisation in which the principal amount repaid in each " \
-               "instalment is the same."
+              "instalment is the same."
     BLLT = 4, "Bullet - i.e. Amortisation in which the full principal amount is repaid in the last instalment."
     OTHR = 10, "Other"
 
 
 class ESMAOriginationChannelChoices(ChoiceEnum):
     BRAN = 1, "Office or Branch Network"
     BROK = 2, "Broker"
@@ -397,7 +397,33 @@
     DAIL = 1, "Daily"
     WEEK = 2, "Weekly"
     MNTH = 3, "Monthly"
     QUTR = 4, "Quarterly"
     SEMI = 5, "Semi Annual"
     YEAR = 6, "Annual"
     OTHR = 10, "Other"
+
+
+class SPVExtensionClauseChoices(ChoiceEnum):
+    ISUR = 1, "SSPE only"
+    NHLD = 2, "Noteholder"
+    ISNH = 3, "Either SSPE or noteholder"
+    NOPT = 4, "No option"
+
+
+class SPVLiabilitySettlementConventionChoice(ChoiceEnum):
+    TONE = 1, "T Plus One"
+    TTWO = 2, "T Plus Two"
+    TTRE = 3, "T Plus Three"
+    ASAP = 4, "As soon as possible"
+    ENDC = 5, "At the end of Contract"
+    MONT = 6, "End of Month"
+    FUTU = 7, "Future"
+    NXTD = 8, "Next Day"
+    REGU = 9, "Regular"
+    TFIV = 10, "T Plus Five"
+    TFOR = 11, "T Plus Four"
+    WHIF = 12, "When and if issued"
+    WDIS = 13, "When Distributed"
+    WISS = 14, "When Issued"
+    WHID = 15, "When Issued or Distributed"
+    OTHR = 16, "Other"
```

### Comparing `cardo-python-utils-0.2.2/python_utils/exceptions.py` & `cardo-python-utils-0.2.3/python_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.2/python_utils/imports.py` & `cardo-python-utils-0.2.3/python_utils/imports.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.2/python_utils/math.py` & `cardo-python-utils-0.2.3/python_utils/math.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.2/python_utils/pandas_utils.py` & `cardo-python-utils-0.2.3/python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.2/python_utils/rest.py` & `cardo-python-utils-0.2.3/python_utils/rest.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.2/python_utils/text.py` & `cardo-python-utils-0.2.3/python_utils/text.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.2/python_utils/time.py` & `cardo-python-utils-0.2.3/python_utils/time.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.2/setup.cfg` & `cardo-python-utils-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardo-python-utils
-version = 0.2.2
+version = 0.2.3
 description = Python library enhanced with a wide range of functions for different scenarios.
 long_description = file: README.rst
 url = https://github.com/CardoAI/cardo-python-utils
 author = Kristi Kotini
 author_email = hello@cardoai.com
 license = MIT (X11)
 classifiers =
```

