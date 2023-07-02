# Comparing `tmp/py_luke-0.0.2.tar.gz` & `tmp/py_luke-0.0.3.tar.gz`

## Comparing `py_luke-0.0.2.tar` & `py_luke-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 py_luke-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 py_luke-0.0.2/petstore.yaml
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 py_luke-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 py_luke-0.0.2/.github/workflows/test-suite.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 py_luke-0.0.2/dockerfiles/python-3.10.Dockerfile
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 py_luke-0.0.2/dockerfiles/python-3.11.Dockerfile
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 py_luke-0.0.2/dockerfiles/python-3.7.Dockerfile
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 py_luke-0.0.2/dockerfiles/python-3.8.Dockerfile
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 py_luke-0.0.2/dockerfiles/python-3.9.Dockerfile
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 py_luke-0.0.2/luke/__init__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 py_luke-0.0.2/luke/format.py
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 py_luke-0.0.2/luke/generators.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 py_luke-0.0.2/luke/main.py
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 py_luke-0.0.2/luke/openapi.py
--rw-r--r--   0        0        0    35840 2020-02-02 00:00:00.000000 py_luke-0.0.2/luke/schemas.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 py_luke-0.0.2/luke/server.py
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 py_luke-0.0.2/scripts/build
--rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 py_luke-0.0.2/scripts/check
--rwxr-xr-x   0        0        0       31 2020-02-02 00:00:00.000000 py_luke-0.0.2/scripts/clean
--rwxr-xr-x   0        0        0      150 2020-02-02 00:00:00.000000 py_luke-0.0.2/scripts/coverage
--rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 py_luke-0.0.2/scripts/install
--rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 py_luke-0.0.2/scripts/sync-version
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 py_luke-0.0.2/scripts/test
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 py_luke-0.0.2/tests/test_data_generators.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 py_luke-0.0.2/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 py_luke-0.0.2/LICENSE
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 py_luke-0.0.2/README.md
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 py_luke-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 py_luke-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 py_luke-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_luke-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 py_luke-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 py_luke-0.0.3/.github/workflows/test-suite.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 py_luke-0.0.3/dockerfiles/python-3.10.Dockerfile
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 py_luke-0.0.3/dockerfiles/python-3.11.Dockerfile
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 py_luke-0.0.3/dockerfiles/python-3.7.Dockerfile
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 py_luke-0.0.3/dockerfiles/python-3.8.Dockerfile
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 py_luke-0.0.3/dockerfiles/python-3.9.Dockerfile
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 py_luke-0.0.3/luke/__init__.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 py_luke-0.0.3/luke/format.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 py_luke-0.0.3/luke/generators.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 py_luke-0.0.3/luke/main.py
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 py_luke-0.0.3/luke/openapi.py
+-rw-r--r--   0        0        0    35840 2020-02-02 00:00:00.000000 py_luke-0.0.3/luke/schemas.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 py_luke-0.0.3/luke/server.py
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 py_luke-0.0.3/scripts/build
+-rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 py_luke-0.0.3/scripts/check
+-rwxr-xr-x   0        0        0       31 2020-02-02 00:00:00.000000 py_luke-0.0.3/scripts/clean
+-rwxr-xr-x   0        0        0      150 2020-02-02 00:00:00.000000 py_luke-0.0.3/scripts/coverage
+-rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 py_luke-0.0.3/scripts/install
+-rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 py_luke-0.0.3/scripts/sync-version
+-rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 py_luke-0.0.3/scripts/test
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 py_luke-0.0.3/tests/test_data_generators.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 py_luke-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 py_luke-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 py_luke-0.0.3/README.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 py_luke-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 py_luke-0.0.3/PKG-INFO
```

### Comparing `py_luke-0.0.2/.github/workflows/test-suite.yml` & `py_luke-0.0.3/.github/workflows/test-suite.yml`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.2/luke/format.py` & `py_luke-0.0.3/luke/format.py`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.2/luke/generators.py` & `py_luke-0.0.3/luke/generators.py`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.2/luke/main.py` & `py_luke-0.0.3/luke/main.py`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.2/luke/openapi.py` & `py_luke-0.0.3/luke/openapi.py`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.2/luke/schemas.py` & `py_luke-0.0.3/luke/schemas.py`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.2/luke/server.py` & `py_luke-0.0.3/luke/server.py`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.2/tests/test_data_generators.py` & `py_luke-0.0.3/tests/test_data_generators.py`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.2/.gitignore` & `py_luke-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.2/LICENSE` & `py_luke-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.2/pyproject.toml` & `py_luke-0.0.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py-luke"
 description = "Mock server for OpenAPI documentation"
 readme = "README.md"
+keywords = ["openapi", "jsonschema", "mock server", "validate openapi", "bundle openapi"]
 requires-python = ">=3.7"
 authors = [
     { name = "Nguyen Khac Thanh", email = "nguyenkhacthanh244@gmail.com" },
 ]
 license = "MIT"
 dynamic = ["version"]
 classifiers = [
@@ -47,16 +48,19 @@
     "pytest-cov==4.0.0",
     "types-PyYAML",
 ]
 
 [project.scripts]
 luke = "luke.main:cli"
 
-[project-urls]
+[project.urls]
 Homepage = "https://github.com/magiskboy/luke"
+Documentation = "https://github.com/magiskboy/luke#features"
+Issues = "https://github.com/magiskboy/luke/issues/"
+Source = "https://github.com/magiskboy/luke"
 
 [tool.hatch.version]
 path = "luke/__init__.py"
 
 [tool.hatch.metadata]
 allow-direct-references = true
```

### Comparing `py_luke-0.0.2/PKG-INFO` & `py_luke-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Metadata-Version: 2.1
 Name: py-luke
-Version: 0.0.2
+Version: 0.0.3
 Summary: Mock server for OpenAPI documentation
+Project-URL: Homepage, https://github.com/magiskboy/luke
+Project-URL: Documentation, https://github.com/magiskboy/luke#features
+Project-URL: Issues, https://github.com/magiskboy/luke/issues/
+Project-URL: Source, https://github.com/magiskboy/luke
 Author-email: Nguyen Khac Thanh <nguyenkhacthanh244@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
+Keywords: bundle openapi,jsonschema,mock server,openapi,validate openapi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AnyIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,15 +38,15 @@
 Requires-Dist: pytest-cov==4.0.0; extra == 'dev'
 Requires-Dist: pytest==7.3.1; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <img width="420px" src="https://i.ibb.co/vL1MmML/luke.png" alt='py-luke'>
+  <img width="420px" src="https://i.ibb.co/0BPYdRk/luke.png" alt='py-luke'>
 </p>
 <p align="center">
     <em>Working on OpenAPI easily.</em>
 </p>
 <p align="center">
     <a href="https://github.com/magiskboy/luke/actions">
         <img src="https://github.com/magiskboy/luke/actions/workflows/test-suite.yml/badge.svg" alt="Build Status">
@@ -65,31 +70,33 @@
 
 
 ## Features
 
 Some of main features:
 
 - Create a mock server for OpenAPI document
-- Validate OpenAPI document
+- Validate OpenAPI document with readable error messages
 - Bundle OpenAPI fragments into the single document
 
 py-luke supports both json and yaml type. Besides, you can also open file via path or URL.
 
 ## Installation
 
-You can install py-luke from PyPi 
+You can install py-luke from PyPi or Docker
 
 ```bash
 $ pip install py-luke
+$ docker run nguyenkhacthanh/luke:latest
 ```
 
-Or from docker
+## Usage
 
 ```bash
-$ docker run nguyenkhacthanh/luke:latest
+$ luke mock https://raw.githubusercontent.com/OAI/OpenAPI-Specification/main/examples/v3.0/petstore.yaml
 ```
 
-## Usage
+or
 
 ```bash
-$ luke openapi.yaml
+$ docker run nguyenkhacthanh/latest validate https://raw.githubusercontent.com/OAI/OpenAPI-Specification/main/examples/v3.0/petstore.yaml
+$ docker run -p8000:8000 nguyenkhacthanh/luke:latest mock https://raw.githubusercontent.com/OAI/OpenAPI-Specification/main/examples/v3.0/petstore.yaml
 ```
```

#### html2text {}

```diff
@@ -1,14 +1,18 @@
-Metadata-Version: 2.1 Name: py-luke Version: 0.0.2 Summary: Mock server for
-OpenAPI documentation Author-email: Nguyen Khac Thanh
-gmail.com> License-Expression: MIT License-File: LICENSE Classifier:
-Development Status :: 3 - Alpha Classifier: Environment :: Web Environment
-Classifier: Framework :: AnyIO Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Metadata-Version: 2.1 Name: py-luke Version: 0.0.3 Summary: Mock server for
+OpenAPI documentation Project-URL: Homepage, https://github.com/magiskboy/luke
+Project-URL: Documentation, https://github.com/magiskboy/luke#features Project-
+URL: Issues, https://github.com/magiskboy/luke/issues/ Project-URL: Source,
+https://github.com/magiskboy/luke Author-email: Nguyen Khac Thanh
+gmail.com> License-Expression: MIT License-File: LICENSE Keywords: bundle
+openapi,jsonschema,mock server,openapi,validate openapi Classifier: Development
+Status :: 3 - Alpha Classifier: Environment :: Web Environment Classifier:
+Framework :: AnyIO Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.7
 Requires-Dist: faker Requires-Dist: httpx Requires-Dist: jsonschema Requires-
 Dist: py-xeger Requires-Dist: pyyaml Requires-Dist: starlette Requires-Dist:
 typer Requires-Dist: uvicorn Provides-Extra: dev Requires-Dist: mypy; extra ==
@@ -17,12 +21,18 @@
 Requires-Dist: ruff; extra == 'dev' Requires-Dist: types-pyyaml; extra == 'dev'
 Description-Content-Type: text/markdown
                                    [py-luke]
                           Working on OpenAPI easily.
     [Build_Status] [Code_coverage] [Download_PyPi] [MIT] [Py_version] [PyPi
                                    version]
 ## Features Some of main features: - Create a mock server for OpenAPI document
-- Validate OpenAPI document - Bundle OpenAPI fragments into the single document
-py-luke supports both json and yaml type. Besides, you can also open file via
-path or URL. ## Installation You can install py-luke from PyPi ```bash $ pip
-install py-luke ``` Or from docker ```bash $ docker run nguyenkhacthanh/luke:
-latest ``` ## Usage ```bash $ luke openapi.yaml ```
+- Validate OpenAPI document with readable error messages - Bundle OpenAPI
+fragments into the single document py-luke supports both json and yaml type.
+Besides, you can also open file via path or URL. ## Installation You can
+install py-luke from PyPi or Docker ```bash $ pip install py-luke $ docker run
+nguyenkhacthanh/luke:latest ``` ## Usage ```bash $ luke mock https://
+raw.githubusercontent.com/OAI/OpenAPI-Specification/main/examples/v3.0/
+petstore.yaml ``` or ```bash $ docker run nguyenkhacthanh/latest validate
+https://raw.githubusercontent.com/OAI/OpenAPI-Specification/main/examples/v3.0/
+petstore.yaml $ docker run -p8000:8000 nguyenkhacthanh/luke:latest mock https:/
+/raw.githubusercontent.com/OAI/OpenAPI-Specification/main/examples/v3.0/
+petstore.yaml ```
```

