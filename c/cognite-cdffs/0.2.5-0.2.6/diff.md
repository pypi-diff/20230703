# Comparing `tmp/cognite_cdffs-0.2.5.tar.gz` & `tmp/cognite_cdffs-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_cdffs-0.2.5.tar", max compression
+gzip compressed data, was "cognite_cdffs-0.2.6.tar", max compression
```

## Comparing `cognite_cdffs-0.2.5.tar` & `cognite_cdffs-0.2.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2423 2023-06-23 07:26:50.271973 cognite_cdffs-0.2.5/README.md
--rw-r--r--   0        0        0      205 2023-06-23 07:26:50.271973 cognite_cdffs-0.2.5/cognite/cdffs/__init__.py
--rw-r--r--   0        0        0     3907 2023-06-23 07:26:50.271973 cognite_cdffs-0.2.5/cognite/cdffs/credentials.py
--rw-r--r--   0        0        0     3134 2023-06-23 07:26:50.271973 cognite_cdffs-0.2.5/cognite/cdffs/file_handler.py
--rw-r--r--   0        0        0    30135 2023-06-23 07:26:50.271973 cognite_cdffs-0.2.5/cognite/cdffs/spec.py
--rw-r--r--   0        0        0     1663 2023-06-23 07:26:50.275973 cognite_cdffs-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.5/setup.py
--rw-r--r--   0        0        0     3148 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     2423 2023-07-03 06:45:17.375764 cognite_cdffs-0.2.6/README.md
+-rw-r--r--   0        0        0      205 2023-07-03 06:45:17.375764 cognite_cdffs-0.2.6/cognite/cdffs/__init__.py
+-rw-r--r--   0        0        0     3907 2023-07-03 06:45:17.375764 cognite_cdffs-0.2.6/cognite/cdffs/credentials.py
+-rw-r--r--   0        0        0     3134 2023-07-03 06:45:17.375764 cognite_cdffs-0.2.6/cognite/cdffs/file_handler.py
+-rw-r--r--   0        0        0    30443 2023-07-03 06:45:17.375764 cognite_cdffs-0.2.6/cognite/cdffs/spec.py
+-rw-r--r--   0        0        0     1663 2023-07-03 06:45:17.379764 cognite_cdffs-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3331 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.6/setup.py
+-rw-r--r--   0        0        0     3142 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.6/PKG-INFO
```

### Comparing `cognite_cdffs-0.2.5/README.md` & `cognite_cdffs-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `cognite_cdffs-0.2.5/cognite/cdffs/credentials.py` & `cognite_cdffs-0.2.6/cognite/cdffs/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_cdffs-0.2.5/cognite/cdffs/file_handler.py` & `cognite_cdffs-0.2.6/cognite/cdffs/file_handler.py`

 * *Files identical despite different names*

### Comparing `cognite_cdffs-0.2.5/cognite/cdffs/spec.py` & `cognite_cdffs-0.2.6/cognite/cdffs/spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,21 @@
         inp_path = Path(root_dir, external_id)
         file_meta = {"type": "file", "name": str(inp_path).lstrip("/"), "size": file_size}
         parent_path = str(inp_path.parent).lstrip("/")
 
         if parent_path not in self.dircache:
             self.dircache[parent_path] = [file_meta]
         else:
-            self.dircache[parent_path].append(file_meta)
+            # Update the size information if the file name already exists.
+            for file_info in self.dircache[parent_path]:
+                if file_info["name"] == file_meta["name"]:
+                    file_info["size"] = file_size
+                    break
+            else:
+                self.dircache[parent_path].append(file_meta)
 
         grand_parent_path = str(Path(parent_path).parent).lstrip("/")
         dir_meta = {"type": "directory", "name": parent_path.lstrip("/")}
         if grand_parent_path not in self.dircache:
             self.dircache[grand_parent_path] = [dir_meta]
         else:
             self.dircache[grand_parent_path].append(dir_meta)
@@ -374,15 +380,15 @@
         Raises:
             FileNotFoundError: When a file is not found.
         """
         _, external_id_prefix, _ = self.split_path(path, validate_suffix=False)
         if external_id_prefix:
             try:
                 self.cognite_client.files.delete(external_id=external_id_prefix)
-            except CogniteNotFoundError as cognite_exp:
+            except (CogniteNotFoundError, CogniteAPIError) as cognite_exp:
                 raise FileNotFoundError from cognite_exp
 
     def rm_files(self, paths: List) -> None:
         """Remove the list of files.
 
         Args:
             paths (List): List of files to remove.
```

### Comparing `cognite_cdffs-0.2.5/pyproject.toml` & `cognite_cdffs-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "cognite-cdffs"
-version = "0.2.5"
+version = "0.2.6"
 description = "File System Interface for CDF Files"
 license = "Apache-2.0"
 authors = ["Infant Alex <infant.alex@cognite.com>"]
 readme = "README.md"
 packages = [
     { include="cognite", from="." },
 ]
 [tool.poetry.group.test.dependencies]
 pandas = "^1.5.1"
 pyarrow = "^12.0.0"
 zarr = "^2.13.3"
-dask = "^2023.6.0"
-xarray = "^2023.5.0"
+dask = "^2023.6.1"
+xarray = "^2023.6.0"
 geodatasets = "^2023.3.0"
 geopandas = "^0.13.2"
 
 [tool.poetry.group.dev.dependencies]
 types-requests = "^2.28.11.5"
 pytest-cov = "^4.1.0"
 black = "^23.3.0"
@@ -64,19 +64,19 @@
 commands =
     coverage run --source cognite -m pytest -v tests
     coverage xml
 """
 
 [tool.poetry.dependencies]
 python = "^3.9.10"
-cognite-sdk = "^6.4.0"
+cognite-sdk = "^6.5.8"
 fsspec = "^2023.6.0"
 requests = "^2.31.0"
 twine = "^4.0.2"
-pydantic = "^1.10.9"
+pydantic = "1.10.10"
 python-dotenv = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `cognite_cdffs-0.2.5/setup.py` & `cognite_cdffs-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 packages = \
 ['cognite', 'cognite.cdffs']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['cognite-sdk>=6.4.0,<7.0.0',
+['cognite-sdk>=6.5.8,<7.0.0',
  'fsspec>=2023.6.0,<2024.0.0',
- 'pydantic>=1.10.9,<2.0.0',
+ 'pydantic==1.10.10',
  'python-dotenv>=1.0.0,<2.0.0',
  'requests>=2.31.0,<3.0.0',
  'twine>=4.0.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'cognite-cdffs',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'File System Interface for CDF Files',
     'long_description': '<a href="https://cognite.com/">\n  <img alt="Cognite" src="https://raw.githubusercontent.com/cognitedata/cognite-python-docs/master/img/cognite_logo_black.png" alt="Cognite logo" title="Cognite" align="right" height="80">\n</a>\n\n[![GitHub](https://img.shields.io/github/license/cognitedata/cdffs)](https://github.com/cognitedata/cdffs/blob/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/cdffs/badge/?version=latest)](https://cdffs.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![codecov](https://codecov.io/gh/cognitedata/cdffs/branch/main/graph/badge.svg)](https://codecov.io/gh/cognitedata/cdffs)\n![PyPI](https://img.shields.io/pypi/v/cognite-cdffs)\n\n# cdffs\n\nA file system interface (`cdffs`) to allow users to work with CDF Files using the [fsspec](https://filesystem-spec.readthedocs.io/en/latest/) supported/compatible python packages (`pandas`, `xarray` etc).\n\n`fsspec` provides an abstract file system interface to work with local/cloud storages and based on the protocol name (example, `s3` or `abfs`) provided in the path, `fsspec` translates the incoming requests to storage specific implementations and send the responses back to the upstream package to work with the desired data.\n\nRefer [fsspec documentation](https://filesystem-spec.readthedocs.io/en/latest/#who-uses-fsspec) to get the list of all supported/compatible python packages.\n\n## Installation\n\n`cdffs` is available on PyPI. Install using,\n\n```shell\npip install cognite-cdffs\n```\n\n## Usage\n\nImportant steps to follow when working with CDF Files using the `fsspec` supported python packages.\n\n1) Import `cdffs` package\n```python\n  from cognite import cdffs  # noqa\n```\n\n2) Follow instructions from [Authentication](https://cdffs.readthedocs.io/en/latest/authentication.html) to authenticate.\n\n3) Read/write the files from/to CDF using `fsspec` supported packages. Example,\n\n    * Read `zarr` files using using `xarray`.\n\n    ```python\n    ds = xarray.open_zarr("cdffs://sample_data/test.zarr")\n    ```\n    * Write `zarr` files using `xarray`.\n\n    ```python\n    ds.to_zarr("cdffs://sample_data/test.zarr", storage_options={"file_metadata": metadata})\n    ```\n\nRefer [cdffs.readthedocs.io](https://cdffs.readthedocs.io) for more details.\n\n## Contributing\nWant to contribute? Check out [CONTRIBUTING](CONTRIBUTING.md).\n',
     'author': 'Infant Alex',
     'author_email': 'infant.alex@cognite.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'': '.'}
 packages = \ ['cognite', 'cognite.cdffs'] package_data = \ {'': ['*']}
-install_requires = \ ['cognite-sdk>=6.4.0,<7.0.0',
-'fsspec>=2023.6.0,<2024.0.0', 'pydantic>=1.10.9,<2.0.0', 'python-
+install_requires = \ ['cognite-sdk>=6.5.8,<7.0.0',
+'fsspec>=2023.6.0,<2024.0.0', 'pydantic==1.10.10', 'python-
 dotenv>=1.0.0,<2.0.0', 'requests>=2.31.0,<3.0.0', 'twine>=4.0.2,<5.0.0']
-setup_kwargs = { 'name': 'cognite-cdffs', 'version': '0.2.5', 'description':
+setup_kwargs = { 'name': 'cognite-cdffs', 'version': '0.2.6', 'description':
 'File System Interface for CDF Files', 'long_description': '\n_[Cognite]\n\n\n
 [![GitHub](https://img.shields.io/github/license/cognitedata/cdffs)](https://
 github.com/cognitedata/cdffs/blob/main/LICENSE)\n[![Documentation Status]
 (https://readthedocs.org/projects/cdffs/badge/?version=latest)](https://
 cdffs.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/
 black)\n[![codecov](https://codecov.io/gh/cognitedata/cdffs/branch/main/graph/
```

### Comparing `cognite_cdffs-0.2.5/PKG-INFO` & `cognite_cdffs-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cognite-cdffs
-Version: 0.2.5
+Version: 0.2.6
 Summary: File System Interface for CDF Files
 License: Apache-2.0
 Author: Infant Alex
 Author-email: infant.alex@cognite.com
 Requires-Python: >=3.9.10,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cognite-sdk (>=6.4.0,<7.0.0)
+Requires-Dist: cognite-sdk (>=6.5.8,<7.0.0)
 Requires-Dist: fsspec (>=2023.6.0,<2024.0.0)
-Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Requires-Dist: pydantic (==1.10.10)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: twine (>=4.0.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 <a href="https://cognite.com/">
   <img alt="Cognite" src="https://raw.githubusercontent.com/cognitedata/cognite-python-docs/master/img/cognite_logo_black.png" alt="Cognite logo" title="Cognite" align="right" height="80">
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: cognite-cdffs Version: 0.2.5 Summary: File System
+Metadata-Version: 2.1 Name: cognite-cdffs Version: 0.2.6 Summary: File System
 Interface for CDF Files License: Apache-2.0 Author: Infant Alex Author-email:
 infant.alex@cognite.com Requires-Python: >=3.9.10,<4.0.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: cognite-sdk
-(>=6.4.0,<7.0.0) Requires-Dist: fsspec (>=2023.6.0,<2024.0.0) Requires-Dist:
-pydantic (>=1.10.9,<2.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: twine (>=4.0.2,<5.0.0)
+(>=6.5.8,<7.0.0) Requires-Dist: fsspec (>=2023.6.0,<2024.0.0) Requires-Dist:
+pydantic (==1.10.10) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0) Requires-
+Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: twine (>=4.0.2,<5.0.0)
 Description-Content-Type: text/markdown [Cognite] [![GitHub](https://
 img.shields.io/github/license/cognitedata/cdffs)](https://github.com/
 cognitedata/cdffs/blob/main/LICENSE) [![Documentation Status](https://
 readthedocs.org/projects/cdffs/badge/?version=latest)](https://
 cdffs.readthedocs.io/en/latest/?badge=latest) [![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/
 black) [![codecov](https://codecov.io/gh/cognitedata/cdffs/branch/main/graph/
```

