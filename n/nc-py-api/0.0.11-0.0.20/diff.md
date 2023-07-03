# Comparing `tmp/nc_py_api-0.0.11.tar.gz` & `tmp/nc_py_api-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nc_py_api-0.0.11.tar", last modified: Wed Mar 22 16:52:12 2023, max compression
+gzip compressed data, was "nc_py_api-0.0.20.tar", last modified: Mon Jul  3 13:27:53 2023, max compression
```

## Comparing `nc_py_api-0.0.11.tar` & `nc_py_api-0.0.20.tar`

### file list

```diff
@@ -1,30 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:52:12.724581 nc_py_api-0.0.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-03-22 16:52:12.724581 nc_py_api-0.0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:52:12.724581 nc_py_api-0.0.11/nc_py_api/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/db_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/db_connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/db_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/db_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/mimetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/occ.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/signal_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/nc_py_api/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 16:52:12.724581 nc_py_api-0.0.11/nc_py_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-03-22 16:52:12.000000 nc_py_api-0.0.11/nc_py_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-22 16:52:12.000000 nc_py_api-0.0.11/nc_py_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 16:52:12.000000 nc_py_api-0.0.11/nc_py_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 16:52:02.000000 nc_py_api-0.0.11/nc_py_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-22 16:52:12.000000 nc_py_api-0.0.11/nc_py_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-22 16:52:12.000000 nc_py_api-0.0.11/nc_py_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-22 16:52:12.724581 nc_py_api-0.0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-22 16:51:50.000000 nc_py_api-0.0.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:27:53.575614 nc_py_api-0.0.20/
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3620 2023-07-03 13:27:53.575614 nc_py_api-0.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:27:53.571613 nc_py_api-0.0.20/nc_py_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12312 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/_session.py
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/appconfig_preferences_ex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15409 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/integration_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4016 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/nextcloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/theming.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/ui_files_actions_menu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/users.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/users_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4232 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/users_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/nc_py_api/weather_status.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:27:53.575614 nc_py_api-0.0.20/nc_py_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3620 2023-07-03 13:27:53.000000 nc_py_api-0.0.20/nc_py_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2023-07-03 13:27:53.000000 nc_py_api-0.0.20/nc_py_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:27:53.000000 nc_py_api-0.0.20/nc_py_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-03 13:27:53.000000 nc_py_api-0.0.20/nc_py_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-03 13:27:53.000000 nc_py_api-0.0.20/nc_py_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:27:46.000000 nc_py_api-0.0.20/nc_py_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-07-03 13:27:53.575614 nc_py_api-0.0.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-03 13:27:37.000000 nc_py_api-0.0.20/setup.py
```

### Comparing `nc_py_api-0.0.11/LICENSE` & `nc_py_api-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.11/PKG-INFO` & `nc_py_api-0.0.20/nc_py_api.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,79 @@
 Metadata-Version: 2.1
-Name: nc_py_api
-Version: 0.0.11
-Summary: Backend API for Python 3.9+ to work with Nextcloud
-Home-page: https://github.com/cloud-py-api/cloud-py-api
+Name: nc-py-api
+Version: 0.0.20
+Summary: Nextcloud Python Framework
+Home-page: https://github.com/cloud-py-api/nc_py_api
 Author: Alexander Piskun
-Author-email: bigcat88@users.noreply.github.com
 License: Apache License 3.0
-Project-URL: Source, https://github.com/cloud-py-api/cloud-py-api
+Project-URL: Source, https://github.com/cloud-py-api/nc_py_api
 Keywords: nextcloud,api,framework
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
-# Nextcloud Python Framework
+# Official Nextcloud Python Framework
 
-[![(Py)Analysis & Coverage](https://github.com/cloud-py-api/cloud_py_api/actions/workflows/py_analysis-coverage.yml/badge.svg)](https://github.com/cloud-py-api/cloud_py_api/actions/workflows/py_analysis-coverage.yml)
-![PythonVersion](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)
+[![Analysis & Coverage](https://github.com/cloud-py-api/nc_py_api/actions/workflows/analysis-coverage.yml/badge.svg)](https://github.com/cloud-py-api/nc_py_api/actions/workflows/analysis-coverage.yml)
+![PythonVersion](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 ![impl](https://img.shields.io/pypi/implementation/nc_py_api)
 ![pypi](https://img.shields.io/pypi/v/nc_py_api.svg)
-[![codecov](https://codecov.io/gh/cloud-py-api/cloud_py_api/branch/main/graph/badge.svg?token=6IHPKUYUU9)](https://codecov.io/gh/cloud-py-api/cloud_py_api)
+[![codecov](https://codecov.io/github/cloud-py-api/nc_py_api/branch/main/graph/badge.svg?token=C91PL3FYDQ)](https://codecov.io/github/cloud-py-api/nc_py_api)
 
-Framework(App) for Nextcloud to develop apps, that using Python.
+### Remark
 
-Consists of PHP part(**cloud_py_api app**) and a Python module(**nc-py-api**).
-
-| **Currently in development, all is in a design state**
-
-## Provides Convenient Functions for Python
-
-- Read & Write File System objects
-- Working with Database
-- Wrapper around `OCC` calls
-- Calling your python function from php part of app and return a result
-
-## 🚀 Installation
-
-In your Nextcloud, simply enable the `cloud_py_api` app through the Apps management and then install apps, that using it.
-
-The Nextcloud `cloud_py_api` app supports Nextcloud version 25 and higher.
-
-#### More information can be found on [Wiki page](https://github.com/cloud-py-api/cloud_py_api/wiki)
-
-## Maintainers
-
-* [Andrey Borysenko](https://github.com/andrey18106)
-* [Alexander Piskun](https://github.com/bigcat88)
-
-## Apps using this
-
-- [MediaDC](https://github.com/andrey18106/mediadc) - Nextcloud Media Duplicate collector app. Python part - core logics for duplicates search.
-
-## Support
-
-You can support us in several ways:
-
-- ⭐ Star our work (it really motivates)
-- ❗ Create an Issue or feature request (bring to us an excellent idea)
-- 💁 Resolve some Issue or create a Pull Request (contribute to this project)
-- 🪙 Donate with any amount with one of the links below (fund this project)
-
-[![PayPal](https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif)](https://www.paypal.com/donate?hosted_button_id=H5PLJJMWLDNJQ)
-[![Liberapay](https://liberapay.com/assets/widgets/donate.svg)](https://liberapay.com/cloud_py_api/donate)
+Project cloud-py-api was **abandoned** and divided into two parts:
+ * `nc_py_api` - this repository, which contains Python Framework to work with Nextcloud and `app_ecosystem_v2`
+ * `app_ecosystem_v2` - New [Nextcloud Application Ecosystem](https://github.com/cloud-py-api/app_ecosystem_v2) that allows writing applications for Nextcloud in any language
+
+**_Projects stage: under heavy prototyping and developing_**
+
+### Basic Features:
+ * Listing, enabling and disabling of the applications
+ * Operations with Files and Folders
+ * ~~Operations with Trash bin and File versions~~
+ * Operations with Users and User Groups
+ * User status manipulation
+ * Weather status
+ * ~~Nextcloud notifications support~~
+ * ~~Shares operations support~~
+ * ~~Talk support~~
+
+### Extended Features with installed App_ecosystem_v2:
+ * Defining callback routes with FastAPI for Nextcloud
+ * Registering UI elements in Nextcloud
+ * Storing logs to the `nextcloud.log` file
+ * Get/save key-value pairs in AppConfigEx/PreferencesEx tables.
+ * **Tons of the cool stuff that is coming soon**
+
+### 🚀 How to start
+
+In very close near future we will publish examples
+
+### More Information
+
+- [Documentation](https://nc_py_api.readthedocs.io/)
+  - [Using it as a simple client](to-do)
+  - [Writing a simple Nextcloud application](to-do)
+  - [Writing a Nextcloud system application](to-do)
+- [Examples](https://github.com/cloud-py-api/nc_py_api/tree/main/examples)
+- [Contribute](https://github.com/cloud-py-api/nc_py_api/blob/main/.github/CONTRIBUTING.md)
+  - [Discussions](https://github.com/cloud-py-api/nc_py_api/discussions)
+  - [Issues](https://github.com/cloud-py-api/nc_py_api/issues)
+  - [Setting up dev environment](to-do)
+- [Changelog](https://github.com/cloud-py-api/nc_py_api/blob/main/CHANGELOG.md)
```

### Comparing `nc_py_api-0.0.11/pyproject.toml` & `nc_py_api-0.0.20/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,70 @@
 [build-system]
-requires = ["setuptools>=60", "wheel"]
-# build-backend = "setuptools.build_meta"
+requires = [
+  "setuptools>=60",
+  "wheel",
+]
+
+[tool.black]
+line-length = 120
+target-versions = ["py39"]
+preview = true
+
+[tool.isort]
+profile = "black"
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+testpaths = [
+    "tests",
+]
+filterwarnings = [
+    "ignore::DeprecationWarning",
+]
+log_cli = true
+addopts = "-rs --color=yes"
 
 [tool.coverage.run]
 cover_pylib = true
 include = ["*/nc_py_api/*"]
-omit = ["*/tests/nc_py_api/*"]
+omit = ["*/tests/*"]
+
+[tool.coverage.paths]
+source = [
+    "nc_py_api/",
+    "*/site-packages/nc_py_api/"
+]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "raise NotImplementedError",
     "DeprecationWarning",
     "DEPRECATED"
 ]
 
-[tool.black]
-line-length = 120
-target-versions = ["py39"]
-preview = true
-
-[tool.isort]
-profile = "black"
+[tool.mypy]
+ignore_missing_imports = false
+warn_no_return = true
+strict_optional = true
+check_untyped_defs = true
 
 [tool.pylint]
 master.py-version = "3.9"
-master.extension-pkg-allow-list = [""]
-design.max-attributes = 9
+master.extension-pkg-allow-list = ["pydantic"]
+design.max-attributes = 8
 design.max-locals = 16
+design.max-branches = 16
 design.max-returns = 8
+design.max-args = 6
 basic.good-names = [
-    "a", "b", "c", "d", "e", "f", "i", "j", "k", "v",
-    "ex", "_", "fp", "im",
+    "a", "b", "c", "d", "e", "f", "i", "j", "k", "r", "v",
+    "ex", "_", "fp", "im", "nc",
 ]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.disable = [
-    "missing-module-docstring",
     "missing-class-docstring",
     "missing-function-docstring",
     "line-too-long",
+    "too-few-public-methods",
 ]
-
-[tool.mypy]
-ignore_missing_imports = false
-warn_no_return = true
-strict_optional = true
-
-[tool.pytest.ini_options]
-minversion = "6.0"
-testpaths = [
-    "tests/nc_py_api",
-]
-filterwarnings = [
-    "ignore::DeprecationWarning",
-]
-log_cli = true
```

### Comparing `nc_py_api-0.0.11/setup.cfg` & `nc_py_api-0.0.20/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 [metadata]
 name = nc_py_api
-description = Backend API for Python 3.9+ to work with Nextcloud
+description = Nextcloud Python Framework
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/cloud-py-api/cloud-py-api
+url = https://github.com/cloud-py-api/nc_py_api
 author = Alexander Piskun
-author_email = bigcat88@users.noreply.github.com
 keywords = nextcloud, api, framework
 classifiers = 
 	Development Status :: 1 - Planning
 	Intended Audience :: Developers
 	Topic :: Software Development
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: Libraries :: Application Frameworks
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
+	Programming Language :: Python :: Implementation :: PyPy
 	License :: OSI Approved :: GNU Affero General Public License v3
 	Operating System :: POSIX :: Linux
 license = Apache License 3.0
 project_urls = 
-	Source=https://github.com/cloud-py-api/cloud-py-api
+	Source=https://github.com/cloud-py-api/nc_py_api
 
 [options]
 python_requires = >=3.9
-zip_safe = False
+zip_safe = True
 packages = find:
 install_requires = 
-	pg8000
-	pymysql
-	pynacl
-	cryptography
+	requests
+	httpx
+	xmltodict
+	pydantic
+	xxhash
+	fastapi
 
 [options.extras_require]
+docs = 
+	sphinx>=4.4
+	sphinx-issues>=3.0.1
+	sphinx-rtd-theme>=1.0
 dev = 
 	pytest
 	pre-commit
 	pylint
 	coverage
+	pillow
+	uvicorn
 
 [flake8]
 max-line-length = 120
 target-version = ["py39"]
 ignore = 
 	E203,
 	W503,
```

