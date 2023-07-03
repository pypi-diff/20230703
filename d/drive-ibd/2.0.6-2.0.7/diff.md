# Comparing `tmp/drive_ibd-2.0.6.tar.gz` & `tmp/drive_ibd-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drive_ibd-2.0.6.tar", max compression
+gzip compressed data, was "drive_ibd-2.0.7.tar", max compression
```

## Comparing `drive_ibd-2.0.6.tar` & `drive_ibd-2.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1096 2023-05-02 16:23:38.534742 drive_ibd-2.0.6/README.md
--rw-r--r--   0        0        0       22 2023-07-03 14:45:23.041250 drive_ibd-2.0.6/drive/__init__.py
--rw-r--r--   0        0        0       45 2023-05-04 19:56:44.572942 drive_ibd-2.0.6/drive/cluster/__init__.py
--rw-r--r--   0        0        0    17869 2023-05-23 17:27:33.288051 drive_ibd-2.0.6/drive/cluster/cluster.py
--rw-r--r--   0        0        0    10145 2023-07-03 14:46:25.807621 drive_ibd-2.0.6/drive/drive.py
--rw-r--r--   0        0        0      129 2023-04-11 15:57:06.666606 drive_ibd-2.0.6/drive/factory/__init__.py
--rw-r--r--   0        0        0     1529 2023-06-30 15:43:04.548543 drive_ibd-2.0.6/drive/factory/factory.py
--rw-r--r--   0        0        0      784 2023-05-03 21:40:36.649638 drive_ibd-2.0.6/drive/factory/loader.py
--rw-r--r--   0        0        0       30 2023-06-22 19:24:49.749173 drive_ibd-2.0.6/drive/filters/__init__.py
--rw-r--r--   0        0        0    17183 2023-06-27 18:29:28.100126 drive_ibd-2.0.6/drive/filters/filter.py
--rw-r--r--   0        0        0       37 2023-04-03 17:12:25.006647 drive_ibd-2.0.6/drive/log/.git
--rw-r--r--   0        0        0       12 2023-04-03 17:12:25.030646 drive_ibd-2.0.6/drive/log/.gitignore
--rw-r--r--   0        0        0     4433 2023-04-03 17:12:25.050646 drive_ibd-2.0.6/drive/log/README.md
--rw-r--r--   0        0        0       33 2023-05-04 22:00:40.780404 drive_ibd-2.0.6/drive/log/__init__.py
--rw-r--r--   0        0        0      225 2023-05-04 22:01:13.999559 drive_ibd-2.0.6/drive/log/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      303 2023-04-07 13:55:36.577011 drive_ibd-2.0.6/drive/log/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6230 2023-06-22 19:16:27.189955 drive_ibd-2.0.6/drive/log/__pycache__/logger.cpython-311.pyc
--rw-r--r--   0        0        0     2730 2023-04-14 16:19:44.018287 drive_ibd-2.0.6/drive/log/__pycache__/logger.cpython-39.pyc
--rw-r--r--   0        0        0     4240 2023-05-23 17:27:33.148055 drive_ibd-2.0.6/drive/log/logger.py
--rw-r--r--   0        0        0      248 2023-06-21 16:46:23.320291 drive_ibd-2.0.6/drive/models/__init__.py
--rw-r--r--   0        0        0      503 2023-06-21 16:46:16.772455 drive_ibd-2.0.6/drive/models/choices.py
--rw-r--r--   0        0        0      694 2023-05-04 22:02:59.468876 drive_ibd-2.0.6/drive/models/data_container.py
--rw-r--r--   0        0        0     4493 2023-06-27 18:13:44.556344 drive_ibd-2.0.6/drive/models/generate_indices.py
--rw-r--r--   0        0        0     2161 2023-05-04 16:45:00.827439 drive_ibd-2.0.6/drive/models/networks.py
--rw-r--r--   0        0        0      617 2023-04-13 21:14:00.109726 drive_ibd-2.0.6/drive/models/types.py
--rw-r--r--   0        0        0        0 2023-05-03 14:34:54.522918 drive_ibd-2.0.6/drive/plugins/__init__.py
--rw-r--r--   0        0        0     4352 2023-06-27 18:14:16.239555 drive_ibd-2.0.6/drive/plugins/network_writer.py
--rw-r--r--   0        0        0    10084 2023-05-23 17:30:22.059715 drive_ibd-2.0.6/drive/plugins/pvalues.py
--rw-r--r--   0        0        0       59 2023-05-03 21:40:36.641638 drive_ibd-2.0.6/drive/utilities/callbacks/__init__.py
--rw-r--r--   0        0        0     1520 2023-05-03 21:40:36.657638 drive_ibd-2.0.6/drive/utilities/callbacks/callbacks.py
--rw-r--r--   0        0        0     2222 2023-05-02 19:24:58.309743 drive_ibd-2.0.6/drive/utilities/load_phenotypes.py
--rw-r--r--   0        0        0      121 2023-05-03 21:42:41.142428 drive_ibd-2.0.6/drive/utilities/parser/__init__.py
--rw-r--r--   0        0        0     9196 2023-05-23 17:27:33.204053 drive_ibd-2.0.6/drive/utilities/parser/case_file_parser.py
--rw-r--r--   0        0        0      919 2023-05-04 20:29:24.747764 drive_ibd-2.0.6/drive/utilities/parser/phenotype_descriptions_parser.py
--rw-r--r--   0        0        0     2179 2023-07-03 14:54:08.915805 drive_ibd-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 drive_ibd-2.0.6/setup.py
--rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 drive_ibd-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-05-02 16:23:38.534742 drive_ibd-2.0.7/README.md
+-rw-r--r--   0        0        0       22 2023-07-03 14:45:23.041250 drive_ibd-2.0.7/drive/__init__.py
+-rw-r--r--   0        0        0       45 2023-05-04 19:56:44.572942 drive_ibd-2.0.7/drive/cluster/__init__.py
+-rw-r--r--   0        0        0    17869 2023-05-23 17:27:33.288051 drive_ibd-2.0.7/drive/cluster/cluster.py
+-rw-r--r--   0        0        0    10162 2023-07-03 15:00:06.722696 drive_ibd-2.0.7/drive/drive.py
+-rw-r--r--   0        0        0      129 2023-04-11 15:57:06.666606 drive_ibd-2.0.7/drive/factory/__init__.py
+-rw-r--r--   0        0        0     1529 2023-06-30 15:43:04.548543 drive_ibd-2.0.7/drive/factory/factory.py
+-rw-r--r--   0        0        0      784 2023-05-03 21:40:36.649638 drive_ibd-2.0.7/drive/factory/loader.py
+-rw-r--r--   0        0        0       30 2023-06-22 19:24:49.749173 drive_ibd-2.0.7/drive/filters/__init__.py
+-rw-r--r--   0        0        0    17183 2023-06-27 18:29:28.100126 drive_ibd-2.0.7/drive/filters/filter.py
+-rw-r--r--   0        0        0       37 2023-04-03 17:12:25.006647 drive_ibd-2.0.7/drive/log/.git
+-rw-r--r--   0        0        0       12 2023-04-03 17:12:25.030646 drive_ibd-2.0.7/drive/log/.gitignore
+-rw-r--r--   0        0        0     4433 2023-04-03 17:12:25.050646 drive_ibd-2.0.7/drive/log/README.md
+-rw-r--r--   0        0        0       33 2023-05-04 22:00:40.780404 drive_ibd-2.0.7/drive/log/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-04 22:01:13.999559 drive_ibd-2.0.7/drive/log/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      303 2023-04-07 13:55:36.577011 drive_ibd-2.0.7/drive/log/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     6230 2023-06-22 19:16:27.189955 drive_ibd-2.0.7/drive/log/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0        0        0     2730 2023-04-14 16:19:44.018287 drive_ibd-2.0.7/drive/log/__pycache__/logger.cpython-39.pyc
+-rw-r--r--   0        0        0     4240 2023-05-23 17:27:33.148055 drive_ibd-2.0.7/drive/log/logger.py
+-rw-r--r--   0        0        0      248 2023-06-21 16:46:23.320291 drive_ibd-2.0.7/drive/models/__init__.py
+-rw-r--r--   0        0        0      503 2023-06-21 16:46:16.772455 drive_ibd-2.0.7/drive/models/choices.py
+-rw-r--r--   0        0        0      694 2023-05-04 22:02:59.468876 drive_ibd-2.0.7/drive/models/data_container.py
+-rw-r--r--   0        0        0     4493 2023-06-27 18:13:44.556344 drive_ibd-2.0.7/drive/models/generate_indices.py
+-rw-r--r--   0        0        0     2161 2023-05-04 16:45:00.827439 drive_ibd-2.0.7/drive/models/networks.py
+-rw-r--r--   0        0        0      617 2023-04-13 21:14:00.109726 drive_ibd-2.0.7/drive/models/types.py
+-rw-r--r--   0        0        0        0 2023-05-03 14:34:54.522918 drive_ibd-2.0.7/drive/plugins/__init__.py
+-rw-r--r--   0        0        0     4352 2023-06-27 18:14:16.239555 drive_ibd-2.0.7/drive/plugins/network_writer.py
+-rw-r--r--   0        0        0    10084 2023-05-23 17:30:22.059715 drive_ibd-2.0.7/drive/plugins/pvalues.py
+-rw-r--r--   0        0        0       59 2023-05-03 21:40:36.641638 drive_ibd-2.0.7/drive/utilities/callbacks/__init__.py
+-rw-r--r--   0        0        0     1520 2023-05-03 21:40:36.657638 drive_ibd-2.0.7/drive/utilities/callbacks/callbacks.py
+-rw-r--r--   0        0        0     2222 2023-05-02 19:24:58.309743 drive_ibd-2.0.7/drive/utilities/load_phenotypes.py
+-rw-r--r--   0        0        0      121 2023-05-03 21:42:41.142428 drive_ibd-2.0.7/drive/utilities/parser/__init__.py
+-rw-r--r--   0        0        0     9196 2023-05-23 17:27:33.204053 drive_ibd-2.0.7/drive/utilities/parser/case_file_parser.py
+-rw-r--r--   0        0        0      919 2023-05-04 20:29:24.747764 drive_ibd-2.0.7/drive/utilities/parser/phenotype_descriptions_parser.py
+-rw-r--r--   0        0        0     2179 2023-07-03 15:00:15.986459 drive_ibd-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 drive_ibd-2.0.7/setup.py
+-rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 drive_ibd-2.0.7/PKG-INFO
```

### Comparing `drive_ibd-2.0.6/README.md` & `drive_ibd-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/cluster/cluster.py` & `drive_ibd-2.0.7/drive/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/drive.py` & `drive_ibd-2.0.7/drive/drive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import re
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
-import factory
+import drive.factory as factory
 import typer
 from cluster import ClusterHandler, cluster
 from filters import IbdFilter
 from log import CustomLogger
 from models import Data, FormatTypes, Genes, OverlapOptions, create_indices
 from utilities.callbacks import check_input_exists, check_json_path
 from utilities.parser import PhenotypeFileParser, load_phenotype_descriptions
```

### Comparing `drive_ibd-2.0.6/drive/factory/factory.py` & `drive_ibd-2.0.7/drive/factory/factory.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/factory/loader.py` & `drive_ibd-2.0.7/drive/factory/loader.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/filters/filter.py` & `drive_ibd-2.0.7/drive/filters/filter.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/log/README.md` & `drive_ibd-2.0.7/drive/log/README.md`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/log/__pycache__/logger.cpython-311.pyc` & `drive_ibd-2.0.7/drive/log/__pycache__/logger.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/log/__pycache__/logger.cpython-39.pyc` & `drive_ibd-2.0.7/drive/log/__pycache__/logger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/log/logger.py` & `drive_ibd-2.0.7/drive/log/logger.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/models/data_container.py` & `drive_ibd-2.0.7/drive/models/data_container.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/models/generate_indices.py` & `drive_ibd-2.0.7/drive/models/generate_indices.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/models/networks.py` & `drive_ibd-2.0.7/drive/models/networks.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/models/types.py` & `drive_ibd-2.0.7/drive/models/types.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/plugins/network_writer.py` & `drive_ibd-2.0.7/drive/plugins/network_writer.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/plugins/pvalues.py` & `drive_ibd-2.0.7/drive/plugins/pvalues.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/utilities/callbacks/callbacks.py` & `drive_ibd-2.0.7/drive/utilities/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/utilities/load_phenotypes.py` & `drive_ibd-2.0.7/drive/utilities/load_phenotypes.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/utilities/parser/case_file_parser.py` & `drive_ibd-2.0.7/drive/utilities/parser/case_file_parser.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/drive/utilities/parser/phenotype_descriptions_parser.py` & `drive_ibd-2.0.7/drive/utilities/parser/phenotype_descriptions_parser.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.0.6/pyproject.toml` & `drive_ibd-2.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drive-ibd"
-version = "2.0.6"
+version = "2.0.7"
 description = "cli tool to identify networks of individuals who share IBD segments overlapping loci of interest"
 authors = ["James Baker <james.baker@vanderbilt.edu>", "Hung-Hsin Chen <hung-hsin.chen.1@vumc.org>", "Jennifer E. Below <jennifer.e.below@vumc.org>"]
 maintainers = ["James Baker <james.baker@vanderbilt.edu>", "Hung-Hsin Chen <hung-hsin.chen.1@vumc.org>"]
 repository = "https://github.com/belowlab/drive"
 homepage = "https://belowlab.github.io/drive/"
 readme = "README.md"
 keywords = ["python", "genetics", "identity by descent", "relatedness"]
```

### Comparing `drive_ibd-2.0.6/setup.py` & `drive_ibd-2.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['drive = drive.drive:app']}
 
 setup_kwargs = {
     'name': 'drive-ibd',
-    'version': '2.0.6',
+    'version': '2.0.7',
     'description': 'cli tool to identify networks of individuals who share IBD segments overlapping loci of interest',
     'long_description': '# DRIVE:\n\nThis repository contains the source code for the tool DRIVE v1.0.0. Distant Relatedness for Identification and Variant Evaluation (DRIVE) is a novel approach to IBD-based genotype inference used to identify shared chromosomal segments in dense genetic arrays. DRIVE implemented a random walk algorithm that identifies clusters of individuals who pairwise share an IBD segment overlapping a locus of interest. This tool was developed in python by the Below Lab at Vanderbilt University. The documentation for how to use this tool can be found here [DRIVE documentation](https://belowlab.github.io/drive/)\n\n## Installing DRIVE:\nDRIVE is available on PYPI and can easily be installed using the following command:\n\n```bash\npip install drive-ibd\n```\n\nIf the user wishes to develop DRIVE or install the program from source then they can clone the repository. This process is described under the section called "Github Installation" in the documentation.\n\n### Reporting issues:\nIf you wish to report a bug or propose a feature you can find templates under the .github/ISSUE_TEMPLATE directory.',
     'author': 'James Baker',
     'author_email': 'james.baker@vanderbilt.edu',
     'maintainer': 'James Baker',
     'maintainer_email': 'james.baker@vanderbilt.edu',
     'url': 'https://belowlab.github.io/drive/',
```

### Comparing `drive_ibd-2.0.6/PKG-INFO` & `drive_ibd-2.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drive-ibd
-Version: 2.0.6
+Version: 2.0.7
 Summary: cli tool to identify networks of individuals who share IBD segments overlapping loci of interest
 Home-page: https://belowlab.github.io/drive/
 Keywords: python,genetics,identity by descent,relatedness
 Author: James Baker
 Author-email: james.baker@vanderbilt.edu
 Maintainer: James Baker
 Maintainer-email: james.baker@vanderbilt.edu
```

