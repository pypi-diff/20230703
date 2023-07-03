# Comparing `tmp/gwlandscape_python-0.3.3.tar.gz` & `tmp/gwlandscape_python-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwlandscape_python-0.3.3.tar", max compression
+gzip compressed data, was "gwlandscape_python-0.3.4.tar", max compression
```

## Comparing `gwlandscape_python-0.3.3.tar` & `gwlandscape_python-0.3.4.tar`

### file list

```diff
@@ -1,22 +1,38 @@
--rw-r--r--   0        0        0     1076 2022-08-25 03:57:12.620934 gwlandscape_python-0.3.3/LICENSE
--rw-r--r--   0        0        0      524 2023-03-27 03:08:09.587795 gwlandscape_python-0.3.3/README.rst
--rw-r--r--   0        0        0      342 2022-08-31 08:22:19.506487 gwlandscape_python-0.3.3/gwlandscape_python/__init__.py
--rw-r--r--   0        0        0     2170 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.3/gwlandscape_python/dataset_type.py
--rw-r--r--   0        0        0    17552 2023-04-21 06:22:03.415309 gwlandscape_python-0.3.3/gwlandscape_python/gwlandscape.py
--rw-r--r--   0        0        0     1608 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.3/gwlandscape_python/keyword_type.py
--rw-r--r--   0        0        0     1920 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.3/gwlandscape_python/model_type.py
--rw-r--r--   0        0        0     3801 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.3/gwlandscape_python/publication_type.py
--rw-r--r--   0        0        0      227 2022-08-31 07:40:02.705327 gwlandscape_python-0.3.3/gwlandscape_python/settings.py
--rw-r--r--   0        0        0        0 2022-08-25 03:57:12.624934 gwlandscape_python-0.3.3/gwlandscape_python/tests/__init__.py
--rw-r--r--   0        0        0     5874 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.3/gwlandscape_python/tests/conftest.py
--rw-r--r--   0        0        0     2657 2023-04-20 04:41:39.756269 gwlandscape_python-0.3.3/gwlandscape_python/tests/test_dataset_type.py
--rw-r--r--   0        0        0    16979 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.3/gwlandscape_python/tests/test_gwlandscape_python.py
--rw-r--r--   0        0        0     2234 2023-04-20 04:41:39.756269 gwlandscape_python-0.3.3/gwlandscape_python/tests/test_keyword_type.py
--rw-r--r--   0        0        0     2290 2023-04-20 04:41:39.756269 gwlandscape_python-0.3.3/gwlandscape_python/tests/test_model_type.py
--rw-r--r--   0        0        0     3938 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.3/gwlandscape_python/tests/test_publication_type.py
--rw-r--r--   0        0        0      152 2022-08-25 03:57:12.624934 gwlandscape_python-0.3.3/gwlandscape_python/tests/utils.py
--rw-r--r--   0        0        0       54 2022-08-31 07:40:02.709327 gwlandscape_python-0.3.3/gwlandscape_python/utils/__init__.py
--rw-r--r--   0        0        0     4075 2022-08-31 07:40:02.709327 gwlandscape_python-0.3.3/gwlandscape_python/utils/tests/test_utils.py
--rw-r--r--   0        0        0     1357 2022-08-31 07:40:02.713327 gwlandscape_python-0.3.3/gwlandscape_python/utils/utils.py
--rw-r--r--   0        0        0     1074 2023-06-26 02:45:08.714202 gwlandscape_python-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1722 1970-01-01 00:00:00.000000 gwlandscape_python-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-08-25 03:57:12.620934 gwlandscape_python-0.3.4/LICENSE
+-rw-r--r--   0        0        0      524 2023-03-27 03:08:09.587795 gwlandscape_python-0.3.4/README.rst
+-rw-r--r--   0        0        0       37 2022-08-30 05:41:07.806853 gwlandscape_python-0.3.4/gwlandscape_python/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      194 2022-08-30 05:41:07.806853 gwlandscape_python-0.3.4/gwlandscape_python/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      295 2022-08-30 05:41:07.806853 gwlandscape_python-0.3.4/gwlandscape_python/.pytest_cache/README.md
+-rw-r--r--   0        0        0     5924 2022-08-30 05:41:07.806853 gwlandscape_python-0.3.4/gwlandscape_python/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-08-30 05:41:07.806853 gwlandscape_python-0.3.4/gwlandscape_python/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      342 2022-08-31 08:22:19.506487 gwlandscape_python-0.3.4/gwlandscape_python/__init__.py
+-rw-r--r--   0        0        0     2170 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.4/gwlandscape_python/dataset_type.py
+-rw-r--r--   0        0        0    17787 2023-07-03 06:07:02.277366 gwlandscape_python-0.3.4/gwlandscape_python/gwlandscape.py
+-rw-r--r--   0        0        0     1608 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.4/gwlandscape_python/keyword_type.py
+-rw-r--r--   0        0        0     1920 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.4/gwlandscape_python/model_type.py
+-rw-r--r--   0        0        0     3801 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.4/gwlandscape_python/publication_type.py
+-rw-r--r--   0        0        0      227 2022-08-31 07:40:02.705327 gwlandscape_python-0.3.4/gwlandscape_python/settings.py
+-rw-r--r--   0        0        0        0 2022-08-25 03:57:12.624934 gwlandscape_python-0.3.4/gwlandscape_python/tests/__init__.py
+-rw-r--r--   0        0        0      176 2022-08-30 00:50:21.643802 gwlandscape_python-0.3.4/gwlandscape_python/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7216 2023-06-24 13:35:20.347960 gwlandscape_python-0.3.4/gwlandscape_python/tests/__pycache__/conftest.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2887 2023-04-20 22:06:01.648362 gwlandscape_python-0.3.4/gwlandscape_python/tests/__pycache__/test_dataset_type.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0    25182 2023-07-03 03:04:46.730826 gwlandscape_python-0.3.4/gwlandscape_python/tests/__pycache__/test_gwlandscape_python.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2421 2023-04-20 22:06:01.784364 gwlandscape_python-0.3.4/gwlandscape_python/tests/__pycache__/test_keyword_type.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2688 2023-04-20 22:06:01.788364 gwlandscape_python-0.3.4/gwlandscape_python/tests/__pycache__/test_model_type.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     5139 2023-06-24 13:35:20.523960 gwlandscape_python-0.3.4/gwlandscape_python/tests/__pycache__/test_publication_type.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0      374 2022-08-30 00:50:21.671802 gwlandscape_python-0.3.4/gwlandscape_python/tests/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     5874 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.4/gwlandscape_python/tests/conftest.py
+-rw-r--r--   0        0        0     2657 2023-04-20 04:41:39.756269 gwlandscape_python-0.3.4/gwlandscape_python/tests/test_dataset_type.py
+-rw-r--r--   0        0        0    16977 2023-07-03 06:07:02.277366 gwlandscape_python-0.3.4/gwlandscape_python/tests/test_gwlandscape_python.py
+-rw-r--r--   0        0        0     2234 2023-04-20 04:41:39.756269 gwlandscape_python-0.3.4/gwlandscape_python/tests/test_keyword_type.py
+-rw-r--r--   0        0        0     2290 2023-04-20 04:41:39.756269 gwlandscape_python-0.3.4/gwlandscape_python/tests/test_model_type.py
+-rw-r--r--   0        0        0     3938 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.4/gwlandscape_python/tests/test_publication_type.py
+-rw-r--r--   0        0        0      152 2022-08-25 03:57:12.624934 gwlandscape_python-0.3.4/gwlandscape_python/tests/utils.py
+-rw-r--r--   0        0        0       72 2023-07-03 06:07:02.277366 gwlandscape_python-0.3.4/gwlandscape_python/utils/__init__.py
+-rw-r--r--   0        0        0      276 2023-06-30 07:15:15.894524 gwlandscape_python-0.3.4/gwlandscape_python/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2406 2023-07-03 05:35:24.849883 gwlandscape_python-0.3.4/gwlandscape_python/utils/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     5638 2023-07-03 02:59:13.943136 gwlandscape_python-0.3.4/gwlandscape_python/utils/tests/__pycache__/test_utils.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     5189 2023-07-03 06:07:02.277366 gwlandscape_python-0.3.4/gwlandscape_python/utils/tests/test_utils.py
+-rw-r--r--   0        0        0     1809 2023-07-03 06:07:02.277366 gwlandscape_python-0.3.4/gwlandscape_python/utils/utils.py
+-rw-r--r--   0        0        0     1090 2023-07-03 06:07:02.277366 gwlandscape_python-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 gwlandscape_python-0.3.4/PKG-INFO
```

### Comparing `gwlandscape_python-0.3.3/LICENSE` & `gwlandscape_python-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gwlandscape_python-0.3.3/README.rst` & `gwlandscape_python-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `gwlandscape_python-0.3.3/gwlandscape_python/dataset_type.py` & `gwlandscape_python-0.3.4/gwlandscape_python/dataset_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape_python-0.3.3/gwlandscape_python/gwlandscape.py` & `gwlandscape_python-0.3.4/gwlandscape_python/gwlandscape.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 from gwdc_python import GWDC
 from gwdc_python.logger import create_logger
 
 import gwlandscape_python
-from gwlandscape_python.utils import mutually_exclusive
+from gwlandscape_python.utils import mutually_exclusive, validate_dataset
 from gwlandscape_python.settings import GWLANDSCAPE_ENDPOINT, GWLANDSCAPE_AUTH_ENDPOINT
 
 logger = create_logger(__name__)
 
 
 class GWLandscape:
     """
@@ -378,36 +378,40 @@
             gwlandscape_python.Model(client=self, **kw['node'])
             for kw in result['compas_models']['edges']
         ]
 
     def create_dataset(self, publication, model, datafile):
         """
         Creates a new dataset object with the specified publication and model.
+        Datasets must contain exactly one hdf5 file, and should either be a hdf5 file
+        or a tarfile containing the hdf5 file.
 
         Parameters
         ----------
         publication : Publication
             The Publication this dataset is for
         model : Model
             The model this dataset is for
-        datafile : Path
-            Local path to the COMPAS dataset file
+        datafile : str or Path
+            Local path to the COMPAS h5 file or tarfile
 
         Returns
         -------
         Dataset
             Created Dataset
         """
         query = """
             mutation UploadCompasDatasetModelMutation($input: UploadCompasDatasetModelMutationInput!) {
                 uploadCompasDatasetModel(input: $input) {
                     id
                 }
             }
         """
+        file_path = Path(datafile)
+        validate_dataset(file_path)
 
         with Path(datafile).open('rb') as f:
             variables = {
                 'input': {
                     "uploadToken": self._generate_compas_dataset_model_upload_token(),
                     'compas_publication': publication.id,
                     'compas_model': model.id,
```

### Comparing `gwlandscape_python-0.3.3/gwlandscape_python/keyword_type.py` & `gwlandscape_python-0.3.4/gwlandscape_python/keyword_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape_python-0.3.3/gwlandscape_python/model_type.py` & `gwlandscape_python-0.3.4/gwlandscape_python/model_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape_python-0.3.3/gwlandscape_python/publication_type.py` & `gwlandscape_python-0.3.4/gwlandscape_python/publication_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape_python-0.3.3/gwlandscape_python/tests/conftest.py` & `gwlandscape_python-0.3.4/gwlandscape_python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gwlandscape_python-0.3.3/gwlandscape_python/tests/test_dataset_type.py` & `gwlandscape_python-0.3.4/gwlandscape_python/tests/test_dataset_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape_python-0.3.3/gwlandscape_python/tests/test_gwlandscape_python.py` & `gwlandscape_python-0.3.4/gwlandscape_python/tests/test_gwlandscape_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
-from pathlib import Path
 from tempfile import NamedTemporaryFile
+import h5py
 
 import pytest
 
 from gwlandscape_python.tests.utils import compare_graphql_query
 
 
 @pytest.fixture
@@ -146,15 +146,14 @@
             }
         }
     """
 
 
 @pytest.fixture
 def create_dataset_request(setup_gwl_request, query_dataset_return):
-    print(query_dataset_return(n_datasets=1))
     response_data = [
         {
             "generate_compas_dataset_model_upload_token": {
                 "token": str(uuid.uuid4())
             }
         },
         {
@@ -514,16 +513,17 @@
 
 def test_create_dataset(create_dataset_request, mock_dataset_data, get_datasets_query):
     gwl, mock_request = create_dataset_request
 
     dataset_data = mock_dataset_data(gwl, i=1)
     dataset_id = 'mock_dataset_id1'
 
-    with NamedTemporaryFile() as tf:
-        dataset = gwl.create_dataset(dataset_data['publication'], dataset_data['model'], Path(tf.name))
+    with NamedTemporaryFile(suffix='.h5') as tf:
+        h5_file = h5py.File(tf.name, 'w')
+        dataset = gwl.create_dataset(dataset_data['publication'], dataset_data['model'], h5_file.filename)
 
     assert dataset.id == dataset_id
     assert dataset.files == ['mock_file1.h5']
 
     publication, model = dataset.publication, dataset.model
 
     for key, val in publication.__dict__.items():
```

### Comparing `gwlandscape_python-0.3.3/gwlandscape_python/tests/test_keyword_type.py` & `gwlandscape_python-0.3.4/gwlandscape_python/tests/test_keyword_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape_python-0.3.3/gwlandscape_python/tests/test_model_type.py` & `gwlandscape_python-0.3.4/gwlandscape_python/tests/test_model_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape_python-0.3.3/gwlandscape_python/tests/test_publication_type.py` & `gwlandscape_python-0.3.4/gwlandscape_python/tests/test_publication_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape_python-0.3.3/gwlandscape_python/utils/utils.py` & `gwlandscape_python-0.3.4/gwlandscape_python/utils/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from functools import wraps
+from pathlib import Path
+import tarfile
+import h5py
 
 
 # Taken from https://stackoverflow.com/a/40363565
 # Needed to be able to identify the names of arguments provided,
 # whether or not they were positional or keywords
 def _get_args_dict(fn, args, kwargs):
     args_names = fn.__code__.co_varnames[:fn.__code__.co_argcount]
@@ -29,7 +32,19 @@
             # If there is more than one of the mutually exclusive arguments, we have a problem
             if n_mutex_keywords > 1:
                 raise SyntaxError(error_msg)
 
             return func(*args, **kwargs)
         return inner
     return wrapper
+
+
+def validate_dataset(file_path):
+    if h5py.is_hdf5(file_path):
+        return None
+
+    if not tarfile.is_tarfile(file_path):
+        raise Exception('Upload is neither a tarfile nor a hdf5 file')
+
+    with tarfile.open(file_path) as f:
+        if sum(Path(name).suffix in ['.h5', '.hdf5'] for name in f.getnames()) != 1:
+            raise Exception('Tarfile must contain exactly one hdf5 file')
```

### Comparing `gwlandscape_python-0.3.3/pyproject.toml` & `gwlandscape_python-0.3.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "gwlandscape-python"
-version = "0.3.3"
+version = "0.3.4"
 description = "Wrapper of GWDC API, used for interacting with the GWLandscape endpoints"
 authors = ["Thomas Reichardt <treichardt@swin.edu.au>", "Lewis Lakerink <llakerink@swin.edu.au"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/gravitationalwavedc/gwlandscape_python"
 include = ["LICENSE",]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 gwdc-python = "^0.6.0"
 requests = "^2.25.1"
 jwt = "^1.2.0"
 graphene-file-upload = "^1.3.0"
 importlib-metadata = "^4.5.0"
 Sphinx = {version = "^4.0.2", optional = true}
 sphinx-rtd-theme = {version = "^0.5.2", optional = true}
 tqdm = "^4.61.2"
+h5py = "^3.9.0"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinx-rtd-theme"]
 
 [tool.poetry.dev-dependencies]
 gwdc-python = {path = "../gwdc-python/", develop = true}
 pytest = "^6.2"
```

### Comparing `gwlandscape_python-0.3.3/PKG-INFO` & `gwlandscape_python-0.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: gwlandscape-python
-Version: 0.3.3
+Version: 0.3.4
 Summary: Wrapper of GWDC API, used for interacting with the GWLandscape endpoints
 Home-page: https://github.com/gravitationalwavedc/gwlandscape_python
 License: MIT
 Author: Thomas Reichardt
 Author-email: treichardt@swin.edu.au
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=4.0.2,<5.0.0) ; extra == "docs"
 Requires-Dist: graphene-file-upload (>=1.3.0,<2.0.0)
 Requires-Dist: gwdc-python (>=0.6.0,<0.7.0)
+Requires-Dist: h5py (>=3.9.0,<4.0.0)
 Requires-Dist: importlib-metadata (>=4.5.0,<5.0.0)
 Requires-Dist: jwt (>=1.2.0,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0) ; extra == "docs"
 Requires-Dist: tqdm (>=4.61.2,<5.0.0)
 Project-URL: Repository, https://github.com/gravitationalwavedc/gwlandscape_python
 Description-Content-Type: text/x-rst
```

