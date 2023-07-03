# Comparing `tmp/salesforce_functions-0.5.1.tar.gz` & `tmp/salesforce_functions-0.6.0.tar.gz`

## Comparing `salesforce_functions-0.5.1.tar` & `salesforce_functions-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/__main__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/__version__.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/context.py
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/invocation_event.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/py.typed
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/_internal/__init__.py
--rw-r--r--   0        0        0     7208 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/_internal/app.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/_internal/cli.py
--rw-r--r--   0        0        0     6300 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/_internal/cloud_event.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/_internal/config.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/_internal/function_loader.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/_internal/logging.py
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/data_api/__init__.py
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/data_api/_requests.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/data_api/exceptions.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/data_api/record.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/data_api/reference_id.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/salesforce_functions/data_api/unit_of_work.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/LICENSE
--rw-r--r--   0        0        0    11173 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/README.md
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 salesforce_functions-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/__main__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/__version__.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/context.py
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/invocation_event.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/py.typed
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/_internal/__init__.py
+-rw-r--r--   0        0        0     7208 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/_internal/app.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/_internal/cli.py
+-rw-r--r--   0        0        0     6300 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/_internal/cloud_event.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/_internal/config.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/_internal/function_loader.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/_internal/logging.py
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/data_api/__init__.py
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/data_api/_requests.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/data_api/exceptions.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/data_api/record.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/data_api/reference_id.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/salesforce_functions/data_api/unit_of_work.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/LICENSE
+-rw-r--r--   0        0        0    11183 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/README.md
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    12807 2020-02-02 00:00:00.000000 salesforce_functions-0.6.0/PKG-INFO
```

### Comparing `salesforce_functions-0.5.1/salesforce_functions/context.py` & `salesforce_functions-0.6.0/salesforce_functions/context.py`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/salesforce_functions/invocation_event.py` & `salesforce_functions-0.6.0/salesforce_functions/invocation_event.py`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/salesforce_functions/testing.py` & `salesforce_functions-0.6.0/salesforce_functions/testing.py`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/salesforce_functions/_internal/app.py` & `salesforce_functions-0.6.0/salesforce_functions/_internal/app.py`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/salesforce_functions/_internal/cli.py` & `salesforce_functions-0.6.0/salesforce_functions/_internal/cli.py`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/salesforce_functions/_internal/cloud_event.py` & `salesforce_functions-0.6.0/salesforce_functions/_internal/cloud_event.py`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/salesforce_functions/_internal/config.py` & `salesforce_functions-0.6.0/salesforce_functions/_internal/config.py`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/salesforce_functions/_internal/function_loader.py` & `salesforce_functions-0.6.0/salesforce_functions/_internal/function_loader.py`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/salesforce_functions/_internal/logging.py` & `salesforce_functions-0.6.0/salesforce_functions/_internal/logging.py`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/salesforce_functions/data_api/__init__.py` & `salesforce_functions-0.6.0/salesforce_functions/data_api/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/salesforce_functions/data_api/_requests.py` & `salesforce_functions-0.6.0/salesforce_functions/data_api/_requests.py`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/salesforce_functions/data_api/exceptions.py` & `salesforce_functions-0.6.0/salesforce_functions/data_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/salesforce_functions/data_api/record.py` & `salesforce_functions-0.6.0/salesforce_functions/data_api/record.py`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/salesforce_functions/data_api/unit_of_work.py` & `salesforce_functions-0.6.0/salesforce_functions/data_api/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/LICENSE` & `salesforce_functions-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `salesforce_functions-0.5.1/README.md` & `salesforce_functions-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 ```
 
 > See the [Python documentation](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment) for help with setting up a virtual environment.
 
 Finally, install the dependencies into the virtual environment.
 
 ```sh
-pip3 install -r requirements.txt
+pip3 install --upgrade -r requirements.txt
 ```
 
 Using a virtual environment ensures your function has all required dependencies before you run it.  
 
 > Note: Starting the Function locally without setting up your virtual environment results in an error.
 
 ### Run the Python Function Locally
```

### Comparing `salesforce_functions-0.5.1/pyproject.toml` & `salesforce_functions-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 ]
 # httptools and uvloop are optional uvicorn dependencies that improve performance.
 dependencies = [
     "aiohttp>=3.8.3,<4",
     "httptools>=0.5.0,<0.6",
     "orjson>=3.8.5,<4",
     "python-dateutil>=2.8.2,<3; python_version < '3.11'",
-    "starlette>=0.23.1,<0.24",
-    "structlog>=22.3.0,<23",
+    "starlette>=0.28.0,<0.29",
+    "structlog>=23.1.0,<24",
     "tomli>=2.0.1,<3; python_version < '3.11'",
-    "uvicorn>=0.20.0,<0.21",
+    "uvicorn>=0.22.0,<0.23",
     "uvloop>=0.17.0,<0.18; sys_platform != 'win32' and sys_platform != 'cygwin'",
 ]
 
 [project.optional-dependencies]
 development = [
-    "black==23.1.0",
-    "coverage-conditional-plugin==0.8.0",
+    "black==23.3.0",
+    "coverage-conditional-plugin==0.9.0",
     "flake8==6.0.0",
     "isort[colors]==5.12.0",
     # httpx is required for starlette's `TestClient`.
-    "httpx==0.23.3",
-    "mypy==0.991",
-    "pylint==2.16.1",
-    "pytest==7.2.1",
-    "pytest-asyncio==0.20.3",
-    "pytest-cov==4.0.0",
+    "httpx==0.24.1",
+    "mypy==1.4.1",
+    "pylint==2.17.4",
+    "pytest==7.4.0",
+    "pytest-asyncio==0.21.0",
+    "pytest-cov==4.1.0",
 ]
 
 [project.scripts]
 sf-functions-python = "salesforce_functions._internal.cli:main"
 
 [project.urls]
 Changelog = "https://github.com/heroku/sf-functions-python/blob/main/CHANGELOG.md"
```

### Comparing `salesforce_functions-0.5.1/PKG-INFO` & `salesforce_functions-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: salesforce-functions
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python support for Salesforce Functions
 Project-URL: Changelog, https://github.com/heroku/sf-functions-python/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/heroku/sf-functions-python
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: functions,salesforce
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.10
 Requires-Dist: aiohttp<4,>=3.8.3
 Requires-Dist: httptools<0.6,>=0.5.0
 Requires-Dist: orjson<4,>=3.8.5
 Requires-Dist: python-dateutil<3,>=2.8.2; python_version < '3.11'
-Requires-Dist: starlette<0.24,>=0.23.1
-Requires-Dist: structlog<23,>=22.3.0
+Requires-Dist: starlette<0.29,>=0.28.0
+Requires-Dist: structlog<24,>=23.1.0
 Requires-Dist: tomli<3,>=2.0.1; python_version < '3.11'
-Requires-Dist: uvicorn<0.21,>=0.20.0
+Requires-Dist: uvicorn<0.23,>=0.22.0
 Requires-Dist: uvloop<0.18,>=0.17.0; sys_platform != 'win32' and sys_platform != 'cygwin'
 Provides-Extra: development
-Requires-Dist: black==23.1.0; extra == 'development'
-Requires-Dist: coverage-conditional-plugin==0.8.0; extra == 'development'
+Requires-Dist: black==23.3.0; extra == 'development'
+Requires-Dist: coverage-conditional-plugin==0.9.0; extra == 'development'
 Requires-Dist: flake8==6.0.0; extra == 'development'
-Requires-Dist: httpx==0.23.3; extra == 'development'
+Requires-Dist: httpx==0.24.1; extra == 'development'
 Requires-Dist: isort[colors]==5.12.0; extra == 'development'
-Requires-Dist: mypy==0.991; extra == 'development'
-Requires-Dist: pylint==2.16.1; extra == 'development'
-Requires-Dist: pytest-asyncio==0.20.3; extra == 'development'
-Requires-Dist: pytest-cov==4.0.0; extra == 'development'
-Requires-Dist: pytest==7.2.1; extra == 'development'
+Requires-Dist: mypy==1.4.1; extra == 'development'
+Requires-Dist: pylint==2.17.4; extra == 'development'
+Requires-Dist: pytest-asyncio==0.21.0; extra == 'development'
+Requires-Dist: pytest-cov==4.1.0; extra == 'development'
+Requires-Dist: pytest==7.4.0; extra == 'development'
 Description-Content-Type: text/markdown
 
 # sf-functions-python
 
 [![PyPI](https://img.shields.io/pypi/v/salesforce-functions.svg?label=PyPI)](https://pypi.org/project/salesforce-functions/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/salesforce-functions.svg?label=Python)](https://pypi.org/project/salesforce-functions/)
 [![CI](https://github.com/heroku/sf-functions-python/actions/workflows/ci.yml/badge.svg)](https://github.com/heroku/sf-functions-python/actions/workflows/ci.yml)
@@ -259,15 +259,15 @@
 ```
 
 > See the [Python documentation](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment) for help with setting up a virtual environment.
 
 Finally, install the dependencies into the virtual environment.
 
 ```sh
-pip3 install -r requirements.txt
+pip3 install --upgrade -r requirements.txt
 ```
 
 Using a virtual environment ensures your function has all required dependencies before you run it.  
 
 > Note: Starting the Function locally without setting up your virtual environment results in an error.
 
 ### Run the Python Function Locally
```

