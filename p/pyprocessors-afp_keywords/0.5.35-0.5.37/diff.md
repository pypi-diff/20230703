# Comparing `tmp/pyprocessors_afp_keywords-0.5.35.tar.gz` & `tmp/pyprocessors_afp_keywords-0.5.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors_afp_keywords-0.5.35.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyprocessors_afp_keywords-0.5.37.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyprocessors_afp_keywords-0.5.35.tar` & `pyprocessors_afp_keywords-0.5.37.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      501 2023-06-16 14:12:55.547285 pyprocessors_afp_keywords-0.5.35/.bumpversion.cfg
--rw-r--r--   0        0        0     1760 2023-06-16 14:12:55.547285 pyprocessors_afp_keywords-0.5.35/.gitignore
--rw-r--r--   0        0        0      419 2023-06-16 14:12:55.548285 pyprocessors_afp_keywords-0.5.35/.pre-commit-config.yaml
--rw-r--r--   0        0        0      202 2023-06-16 14:12:55.548285 pyprocessors_afp_keywords-0.5.35/.readthedocs.yml
--rw-r--r--   0        0        0      121 2023-06-16 14:12:55.549285 pyprocessors_afp_keywords-0.5.35/AUTHORS.md
--rw-r--r--   0        0        0      268 2023-06-16 14:12:55.549285 pyprocessors_afp_keywords-0.5.35/CHANGELOG.md
--rw-r--r--   0        0        0      476 2023-06-16 14:12:55.550285 pyprocessors_afp_keywords-0.5.35/Dockerfile
--rw-r--r--   0        0        0     8602 2023-06-16 14:12:55.550285 pyprocessors_afp_keywords-0.5.35/Jenkinsfile
--rw-r--r--   0        0        0     1082 2023-06-16 14:12:55.551285 pyprocessors_afp_keywords-0.5.35/LICENSE
--rw-r--r--   0        0        0     1613 2023-06-16 14:12:55.551285 pyprocessors_afp_keywords-0.5.35/README.md
--rw-r--r--   0        0        0      949 2023-06-16 14:12:55.551285 pyprocessors_afp_keywords-0.5.35/RELEASE.md
--rw-r--r--   0        0        0     1559 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.35/bumpversion.py
--rw-r--r--   0        0        0       62 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.35/docs/.gitignore
--rw-r--r--   0        0        0      268 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.35/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.35/docs/LICENSE
--rw-r--r--   0        0        0        0 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.35/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-16 14:12:55.553285 pyprocessors_afp_keywords-0.5.35/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     2899 2023-06-16 14:12:55.553285 pyprocessors_afp_keywords-0.5.35/docs/conf.py
--rw-r--r--   0        0        0      146 2023-06-16 14:12:55.553285 pyprocessors_afp_keywords-0.5.35/docs/index.rst
--rw-r--r--   0        0        0       98 2023-06-16 14:12:55.554285 pyprocessors_afp_keywords-0.5.35/mypy.ini
--rw-r--r--   0        0        0     2191 2023-06-16 14:12:55.554285 pyprocessors_afp_keywords-0.5.35/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 14:12:55.554285 pyprocessors_afp_keywords-0.5.35/src/__init__.py
--rw-r--r--   0        0        0      107 2023-06-16 14:16:11.251565 pyprocessors_afp_keywords-0.5.35/src/pyprocessors_afp_keywords/__init__.py
--rw-r--r--   0        0        0     1885 2023-06-16 14:12:55.555285 pyprocessors_afp_keywords-0.5.35/src/pyprocessors_afp_keywords/afp_keywords.py
--rw-r--r--   0        0        0     4662 2023-06-16 14:12:55.555285 pyprocessors_afp_keywords-0.5.35/tests/data/afp_doc_fr.json
--rw-r--r--   0        0        0     1026 2023-06-16 14:12:55.556285 pyprocessors_afp_keywords-0.5.35/tests/test_afp_keywords.py
--rw-r--r--   0        0        0      428 2023-06-16 14:12:55.556285 pyprocessors_afp_keywords-0.5.35/tox.ini
--rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 pyprocessors_afp_keywords-0.5.35/setup.py
--rw-r--r--   0        0        0     3306 1970-01-01 00:00:00.000000 pyprocessors_afp_keywords-0.5.35/PKG-INFO
+-rw-r--r--   0        0        0      501 2023-06-16 14:12:55.547285 pyprocessors_afp_keywords-0.5.37/.bumpversion.cfg
+-rw-r--r--   0        0        0     1760 2023-06-16 14:12:55.547285 pyprocessors_afp_keywords-0.5.37/.gitignore
+-rw-r--r--   0        0        0      419 2023-06-16 14:12:55.548285 pyprocessors_afp_keywords-0.5.37/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      202 2023-06-16 14:12:55.548285 pyprocessors_afp_keywords-0.5.37/.readthedocs.yml
+-rw-r--r--   0        0        0      121 2023-06-16 14:12:55.549285 pyprocessors_afp_keywords-0.5.37/AUTHORS.md
+-rw-r--r--   0        0        0      268 2023-06-16 14:12:55.549285 pyprocessors_afp_keywords-0.5.37/CHANGELOG.md
+-rw-r--r--   0        0        0      476 2023-06-16 14:12:55.550285 pyprocessors_afp_keywords-0.5.37/Dockerfile
+-rw-r--r--   0        0        0     8602 2023-06-16 14:12:55.550285 pyprocessors_afp_keywords-0.5.37/Jenkinsfile
+-rw-r--r--   0        0        0     1082 2023-06-16 14:12:55.551285 pyprocessors_afp_keywords-0.5.37/LICENSE
+-rw-r--r--   0        0        0     1613 2023-06-16 14:12:55.551285 pyprocessors_afp_keywords-0.5.37/README.md
+-rw-r--r--   0        0        0      949 2023-06-16 14:12:55.551285 pyprocessors_afp_keywords-0.5.37/RELEASE.md
+-rw-r--r--   0        0        0     1559 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.37/bumpversion.py
+-rw-r--r--   0        0        0       62 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.37/docs/.gitignore
+-rw-r--r--   0        0        0      268 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.37/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.37/docs/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-16 14:12:55.552285 pyprocessors_afp_keywords-0.5.37/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-16 14:12:55.553285 pyprocessors_afp_keywords-0.5.37/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     2899 2023-06-16 14:12:55.553285 pyprocessors_afp_keywords-0.5.37/docs/conf.py
+-rw-r--r--   0        0        0      146 2023-06-16 14:12:55.553285 pyprocessors_afp_keywords-0.5.37/docs/index.rst
+-rw-r--r--   0        0        0       98 2023-06-16 14:12:55.554285 pyprocessors_afp_keywords-0.5.37/mypy.ini
+-rw-r--r--   0        0        0     2191 2023-06-16 14:12:55.554285 pyprocessors_afp_keywords-0.5.37/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 14:12:55.554285 pyprocessors_afp_keywords-0.5.37/src/__init__.py
+-rw-r--r--   0        0        0      107 2023-07-03 10:34:32.840204 pyprocessors_afp_keywords-0.5.37/src/pyprocessors_afp_keywords/__init__.py
+-rw-r--r--   0        0        0     1651 2023-07-03 10:31:18.707655 pyprocessors_afp_keywords-0.5.37/src/pyprocessors_afp_keywords/afp_keywords.py
+-rw-r--r--   0        0        0     4662 2023-06-16 14:12:55.555285 pyprocessors_afp_keywords-0.5.37/tests/data/afp_doc_fr.json
+-rw-r--r--   0        0        0     1026 2023-06-16 14:12:55.556285 pyprocessors_afp_keywords-0.5.37/tests/test_afp_keywords.py
+-rw-r--r--   0        0        0      428 2023-06-16 14:12:55.556285 pyprocessors_afp_keywords-0.5.37/tox.ini
+-rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 pyprocessors_afp_keywords-0.5.37/setup.py
+-rw-r--r--   0        0        0     3306 1970-01-01 00:00:00.000000 pyprocessors_afp_keywords-0.5.37/PKG-INFO
```

### Comparing `pyprocessors_afp_keywords-0.5.35/.gitignore` & `pyprocessors_afp_keywords-0.5.37/.gitignore`

 * *Files identical despite different names*

### Comparing `pyprocessors_afp_keywords-0.5.35/Jenkinsfile` & `pyprocessors_afp_keywords-0.5.37/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyprocessors_afp_keywords-0.5.35/LICENSE` & `pyprocessors_afp_keywords-0.5.37/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors_afp_keywords-0.5.35/README.md` & `pyprocessors_afp_keywords-0.5.37/README.md`

 * *Files identical despite different names*

### Comparing `pyprocessors_afp_keywords-0.5.35/RELEASE.md` & `pyprocessors_afp_keywords-0.5.37/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyprocessors_afp_keywords-0.5.35/bumpversion.py` & `pyprocessors_afp_keywords-0.5.37/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_afp_keywords-0.5.35/docs/LICENSE` & `pyprocessors_afp_keywords-0.5.37/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors_afp_keywords-0.5.35/docs/conf.py` & `pyprocessors_afp_keywords-0.5.37/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_afp_keywords-0.5.35/pyproject.toml` & `pyprocessors_afp_keywords-0.5.37/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyprocessors_afp_keywords-0.5.35/src/pyprocessors_afp_keywords/afp_keywords.py` & `pyprocessors_afp_keywords-0.5.37/src/pyprocessors_afp_keywords/afp_keywords.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 import os
-from enum import Enum
-from functools import lru_cache
-from functools import partial
-from pathlib import Path
 from typing import List
 from typing import Type, cast
-from cytoolz import functoolz
-from fasttext.FastText import _FastText, load_model
+
 from pydantic import Field, BaseModel
 from pymultirole_plugins.v1.processor import ProcessorBase, ProcessorParameters
-from pymultirole_plugins.v1.schema import Document, Category, AltText
-from textacy import preprocessing
+from pymultirole_plugins.v1.schema import Document, AltText
 
 _home = os.path.expanduser("~")
 
 class AFPKeywordsParameters(ProcessorParameters):
     threshold: float = Field(0.0, description="""Score threshold to keep the keyword.""")
     as_altText: str = Field(
         "slug",
```

### Comparing `pyprocessors_afp_keywords-0.5.35/tests/data/afp_doc_fr.json` & `pyprocessors_afp_keywords-0.5.37/tests/data/afp_doc_fr.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_afp_keywords-0.5.35/tests/test_afp_keywords.py` & `pyprocessors_afp_keywords-0.5.37/tests/test_afp_keywords.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_afp_keywords-0.5.35/setup.py` & `pyprocessors_afp_keywords-0.5.37/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
           'tox']}
 
 entry_points = \
 {'pyprocessors.plugins': ['afp_keywords = '
                           'pyprocessors_afp_keywords.afp_keywords:AFPKeywordsProcessor']}
 
 setup(name='pyprocessors-afp_keywords',
-      version='0.5.35',
+      version='0.5.37',
       description='Processor based on Huggingface transformers zero-shot classification pipeline',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://github.com/oterrier/pyprocessors_afp_keywords/',
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
```

### Comparing `pyprocessors_afp_keywords-0.5.35/PKG-INFO` & `pyprocessors_afp_keywords-0.5.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-afp_keywords
-Version: 0.5.35
+Version: 0.5.37
 Summary: Processor based on Huggingface transformers zero-shot classification pipeline
 Home-page: https://github.com/oterrier/pyprocessors_afp_keywords/
 Keywords: 
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

