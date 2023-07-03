# Comparing `tmp/pyproject_ops-0.2.2.tar.gz` & `tmp/pyproject_ops-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_ops-0.2.2.tar", last modified: Thu Jun 15 01:00:46 2023, max compression
+gzip compressed data, was "pyproject_ops-0.2.3.tar", last modified: Mon Jul  3 16:36:32 2023, max compression
```

## Comparing `pyproject_ops-0.2.2.tar` & `pyproject_ops-0.2.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 01:00:46.810494 pyproject_ops-0.2.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-23 02:11:51.000000 pyproject_ops-0.2.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1123 2023-05-23 02:11:51.000000 pyproject_ops-0.2.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      321 2023-05-23 02:11:51.000000 pyproject_ops-0.2.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)    10325 2023-06-15 01:00:46.810310 pyproject_ops-0.2.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     9171 2023-06-14 13:29:02.000000 pyproject_ops-0.2.2/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 01:00:46.806795 pyproject_ops-0.2.2/pyproject_ops/
--rw-r--r--   0 sanhehu    (501) staff       (20)      423 2023-06-03 06:48:33.000000 pyproject_ops-0.2.2/pyproject_ops/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-15 00:58:08.000000 pyproject_ops-0.2.2/pyproject_ops/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-03 05:51:29.000000 pyproject_ops-0.2.2/pyproject_ops/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5122 2023-06-15 00:58:04.000000 pyproject_ops-0.2.2/pyproject_ops/cli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      163 2023-05-22 19:51:02.000000 pyproject_ops-0.2.2/pyproject_ops/compat.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 01:00:46.807638 pyproject_ops-0.2.2/pyproject_ops/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-23 02:11:51.000000 pyproject_ops-0.2.2/pyproject_ops/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      219 2023-04-27 16:12:50.000000 pyproject_ops-0.2.2/pyproject_ops/helpers.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      154 2023-05-23 00:56:49.000000 pyproject_ops-0.2.2/pyproject_ops/logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      144 2023-05-23 01:06:08.000000 pyproject_ops-0.2.2/pyproject_ops/operation_system.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1020 2023-06-03 06:39:10.000000 pyproject_ops-0.2.2/pyproject_ops/ops.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      657 2023-05-22 19:25:03.000000 pyproject_ops-0.2.2/pyproject_ops/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      470 2023-06-03 06:22:27.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3885 2023-06-03 06:21:16.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_aws_lambda.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1305 2023-06-03 06:09:59.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_build.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1206 2023-06-03 06:02:21.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_config_management.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    13420 2023-06-03 05:59:35.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_deps.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3399 2023-06-03 05:59:07.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_docs.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    12633 2023-06-14 13:22:05.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-06-03 06:38:24.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_publish.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2416 2023-06-14 13:23:14.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_tests.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1997 2023-06-03 05:56:13.000000 pyproject_ops-0.2.2/pyproject_ops/pyproject_venv.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 01:00:46.808330 pyproject_ops-0.2.2/pyproject_ops/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-22 19:25:03.000000 pyproject_ops-0.2.2/pyproject_ops/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-05-23 01:08:52.000000 pyproject_ops-0.2.2/pyproject_ops/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 01:00:46.809573 pyproject_ops-0.2.2/pyproject_ops/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-05-23 00:53:52.000000 pyproject_ops-0.2.2/pyproject_ops/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3224 2023-06-03 06:06:50.000000 pyproject_ops-0.2.2/pyproject_ops/vendor/build_dist.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1406 2023-06-03 06:50:12.000000 pyproject_ops-0.2.2/pyproject_ops/vendor/jsonutils.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-23 00:53:57.000000 pyproject_ops-0.2.2/pyproject_ops/vendor/nested_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-23 00:54:59.000000 pyproject_ops-0.2.2/pyproject_ops/vendor/os_platform.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-23 00:54:22.000000 pyproject_ops-0.2.2/pyproject_ops/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 01:00:46.807512 pyproject_ops-0.2.2/pyproject_ops.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)    10325 2023-06-15 01:00:46.000000 pyproject_ops-0.2.2/pyproject_ops.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1354 2023-06-15 01:00:46.000000 pyproject_ops-0.2.2/pyproject_ops.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-15 01:00:46.000000 pyproject_ops-0.2.2/pyproject_ops.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       49 2023-06-15 01:00:46.000000 pyproject_ops-0.2.2/pyproject_ops.egg-info/entry_points.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      253 2023-06-15 01:00:46.000000 pyproject_ops-0.2.2/pyproject_ops.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       14 2023-06-15 01:00:46.000000 pyproject_ops-0.2.2/pyproject_ops.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     1226 2023-06-15 01:00:02.000000 pyproject_ops-0.2.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)       37 2023-05-23 02:30:18.000000 pyproject_ops-0.2.2/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      352 2023-05-23 02:18:02.000000 pyproject_ops-0.2.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-03 06:28:54.000000 pyproject_ops-0.2.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      400 2023-06-03 07:40:12.000000 pyproject_ops-0.2.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-15 00:58:31.000000 pyproject_ops-0.2.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-15 01:00:46.810539 pyproject_ops-0.2.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7839 2023-06-14 13:30:02.000000 pyproject_ops-0.2.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-15 01:00:46.810012 pyproject_ops-0.2.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-06-03 07:45:37.000000 pyproject_ops-0.2.2/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1733 2023-06-03 07:14:18.000000 pyproject_ops-0.2.2/tests/test_pyproject_ops.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 16:36:32.354181 pyproject_ops-0.2.3/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-23 02:11:51.000000 pyproject_ops-0.2.3/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1123 2023-05-23 02:11:51.000000 pyproject_ops-0.2.3/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      321 2023-05-23 02:11:51.000000 pyproject_ops-0.2.3/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10513 2023-07-03 16:36:32.353953 pyproject_ops-0.2.3/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     9359 2023-07-03 16:35:56.000000 pyproject_ops-0.2.3/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 16:36:32.350668 pyproject_ops-0.2.3/pyproject_ops/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      423 2023-06-03 06:48:33.000000 pyproject_ops-0.2.3/pyproject_ops/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-03 16:32:58.000000 pyproject_ops-0.2.3/pyproject_ops/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-03 05:51:29.000000 pyproject_ops-0.2.3/pyproject_ops/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5122 2023-06-15 00:58:04.000000 pyproject_ops-0.2.3/pyproject_ops/cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      163 2023-05-22 19:51:02.000000 pyproject_ops-0.2.3/pyproject_ops/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 16:36:32.351620 pyproject_ops-0.2.3/pyproject_ops/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-23 02:11:51.000000 pyproject_ops-0.2.3/pyproject_ops/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      219 2023-04-27 16:12:50.000000 pyproject_ops-0.2.3/pyproject_ops/helpers.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      154 2023-05-23 00:56:49.000000 pyproject_ops-0.2.3/pyproject_ops/logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      144 2023-05-23 01:06:08.000000 pyproject_ops-0.2.3/pyproject_ops/operation_system.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1020 2023-06-03 06:39:10.000000 pyproject_ops-0.2.3/pyproject_ops/ops.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      657 2023-05-22 19:25:03.000000 pyproject_ops-0.2.3/pyproject_ops/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      470 2023-06-03 06:22:27.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4237 2023-07-03 16:34:10.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_aws_lambda.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1305 2023-06-03 06:09:59.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_build.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1206 2023-06-03 06:02:21.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_config_management.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    13420 2023-06-03 05:59:35.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_deps.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3399 2023-06-03 05:59:07.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_docs.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12633 2023-06-14 13:22:05.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-06-03 06:38:24.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_publish.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2416 2023-06-14 13:23:14.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_tests.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1997 2023-06-03 05:56:13.000000 pyproject_ops-0.2.3/pyproject_ops/pyproject_venv.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 16:36:32.352092 pyproject_ops-0.2.3/pyproject_ops/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-05-22 19:25:03.000000 pyproject_ops-0.2.3/pyproject_ops/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-05-23 01:08:52.000000 pyproject_ops-0.2.3/pyproject_ops/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 16:36:32.353241 pyproject_ops-0.2.3/pyproject_ops/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-05-23 00:53:52.000000 pyproject_ops-0.2.3/pyproject_ops/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3224 2023-06-03 06:06:50.000000 pyproject_ops-0.2.3/pyproject_ops/vendor/build_dist.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1406 2023-06-03 06:50:12.000000 pyproject_ops-0.2.3/pyproject_ops/vendor/jsonutils.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-23 00:53:57.000000 pyproject_ops-0.2.3/pyproject_ops/vendor/nested_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-23 00:54:59.000000 pyproject_ops-0.2.3/pyproject_ops/vendor/os_platform.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-23 00:54:22.000000 pyproject_ops-0.2.3/pyproject_ops/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 16:36:32.351470 pyproject_ops-0.2.3/pyproject_ops.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10513 2023-07-03 16:36:32.000000 pyproject_ops-0.2.3/pyproject_ops.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1354 2023-07-03 16:36:32.000000 pyproject_ops-0.2.3/pyproject_ops.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-03 16:36:32.000000 pyproject_ops-0.2.3/pyproject_ops.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       49 2023-07-03 16:36:32.000000 pyproject_ops-0.2.3/pyproject_ops.egg-info/entry_points.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      253 2023-07-03 16:36:32.000000 pyproject_ops-0.2.3/pyproject_ops.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       14 2023-07-03 16:36:32.000000 pyproject_ops-0.2.3/pyproject_ops.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1399 2023-07-03 16:33:24.000000 pyproject_ops-0.2.3/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)       37 2023-05-23 02:30:18.000000 pyproject_ops-0.2.3/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      352 2023-05-23 02:18:02.000000 pyproject_ops-0.2.3/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-03 06:28:54.000000 pyproject_ops-0.2.3/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      400 2023-06-03 07:40:12.000000 pyproject_ops-0.2.3/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-15 00:58:31.000000 pyproject_ops-0.2.3/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-03 16:36:32.354234 pyproject_ops-0.2.3/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7839 2023-06-14 13:30:02.000000 pyproject_ops-0.2.3/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 16:36:32.353624 pyproject_ops-0.2.3/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-06-03 07:45:37.000000 pyproject_ops-0.2.3/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1733 2023-06-03 07:14:18.000000 pyproject_ops-0.2.3/tests/test_pyproject_ops.py
```

### Comparing `pyproject_ops-0.2.2/LICENSE.txt` & `pyproject_ops-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/PKG-INFO` & `pyproject_ops-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyproject_ops
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python project Ops automation.
 Home-page: https://github.com/MacHu-GWU/pyproject_ops-project
-Download-URL: https://pypi.python.org/pypi/pyproject_ops/0.2.2#downloads
+Download-URL: https://pypi.python.org/pypi/pyproject_ops/0.2.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -108,19 +108,18 @@
 Folder Structure
 ------------------------------------------------------------------------------
 Below is the folder structured used in ``pyproject_ops``. The first item is the relative path from the project root directory. The second item is the attribute name that you can use to access the path in ``pyproject_ops``. The third item is the description of the path.
 
 - ``.venv``: ``PyProjectOps.dir_venv``, The virtualenv directory.
 - ``.venv/bin``: ``PyProjectOps.dir_venv_bin``, The bin folder in virtualenv.
 - ``.venv/bin/pip``: ``PyProjectOps.path_venv_bin_pip``, The pip command in virtualenv.
-- ``.venv/bin/poetry``: ``PyProjectOps.path_bin_poetry``, The poetry CLI command path.
 - ``.venv/bin/pytest``: ``PyProjectOps.path_venv_bin_pytest``, The pytest command in virtualenv.
+- ``.venv/bin/python``: ``PyProjectOps.path_sys_executable``, The current Python interpreter path.
 - ``.venv/bin/python``: ``PyProjectOps.path_venv_bin_python``, The python executable in virtualenv.
 - ``.venv/bin/twine``: ``PyProjectOps.path_bin_twine``, The twine CLI command path.
-- ``.venv/bin/virtualenv``: ``PyProjectOps.path_bin_virtualenv``, The virtualenv CLI command path.
 - ``build``: ``PyProjectOps.dir_build``, The build folder for Python or artifacts build.
 - ``build/lambda``: ``PyProjectOps.dir_build_lambda``, The AWS Lambda artifacts build folder.
 - ``build/lambda/layer.zip``: ``PyProjectOps.path_build_lambda_layer_zip``, The AWS Lambda layer zip file path.
 - ``build/lambda/python``: ``PyProjectOps.dir_build_lambda_python``, The AWS Lambda layer build folder. This folder contains the dependencies.
 - ``build/lambda/python/aws``: ``PyProjectOps.path_build_lambda_bin_aws``, This is the AWS CLI executable path in Lambda layer.
 - ``build/lambda/source.zip``: ``PyProjectOps.path_build_lambda_source_zip``, The AWS Lambda source code deployment package zip file path.
 - ``config``: ``PyProjectOps.dir_config``, The folder that stores the config files.
@@ -130,21 +129,23 @@
 - ``docs/build``: ``PyProjectOps.dir_sphinx_doc_build``, The temp Sphinx doc build folder.
 - ``docs/build/html``: ``PyProjectOps.dir_sphinx_doc_build_html``, The built Sphinx doc build HTML folder.
 - ``docs/build/html/index.html``: ``PyProjectOps.path_sphinx_doc_build_index_html``, The built Sphinx doc site entry HTML file path.
 - ``docs/source``: ``PyProjectOps.dir_sphinx_doc_source``, Sphinx docs source code folder.
 - ``docs/source/conf.py``: ``PyProjectOps.dir_sphinx_doc_source_conf_py``, Sphinx docs ``conf.py`` file path.
 - ``docs/source/pyproject_ops``: ``PyProjectOps.dir_sphinx_doc_source_python_lib``, The generated Python library API reference Sphinx docs folder.
 - ``htmlcov``: ``PyProjectOps.dir_htmlcov``, The code coverage test results HTML output folder.
+- ``htmlcov/index.html``: ``PyProjectOps.path_htmlcov_index_html``, The code coverage test results HTML file.
 - ``lambda_app``: ``PyProjectOps.dir_lambda_app``, The AWS Lambda app handler file and Lambda related code directory.
 - ``lambda_app/.chalice/config.json``: ``PyProjectOps.path_chalice_config``, The AWS Chalice framework's config file path.
 - ``lambda_app/.chalice/deployed``: ``PyProjectOps.dir_lambda_app_deployed``, The generated ``deployed.json`` file for AWS Chalice framework's.
 - ``lambda_app/app.py``: ``PyProjectOps.path_lambda_app_py``, The app.py file for AWS Chalice framework.
 - ``lambda_app/lambda_function.py``: ``PyProjectOps.path_lambda_function_py``, The lambda_function.py handler file for AWS Lambda, if you are not using
 - ``lambda_app/update_chalice_config.py``: ``PyProjectOps.path_lambda_update_chalice_config_script``, Example: ``${dir_project_root}/lambda_app/update_chalice_config.py``
 - ``lambda_app/vendor``: ``PyProjectOps.dir_lambda_app_vendor``, The vendor folder for AWS Chalice framework's packaging.
+- ``lambda_app/vendor/pyproject_ops``: ``PyProjectOps.dir_lambda_app_vendor_python_lib``, The source python library folder in AWS Chalice framework's vendor folder.
 - ``poetry-lock-hash.json``: ``PyProjectOps.path_poetry_lock_hash_json``, The poetry-lock-hash.json file path. It is the cache of the poetry.lock file hash.
 - ``poetry.lock``: ``PyProjectOps.path_poetry_lock``, The poetry.lock file path.
 - ``pyproject.toml``: ``PyProjectOps.path_pyproject_toml``, The pyproject.toml file path.
 - ``pyproject_ops``: ``PyProjectOps.dir_python_lib``, The current Python library directory.
 - ``pyproject_ops/_version.py``: ``PyProjectOps.path_version_py``, Path to the ``_version.py`` file where the package version is defined.
 - ``requirements-automation.txt``: ``PyProjectOps.path_requirements_automation``, The requirements-automation.txt file path.
 - ``requirements-dev.txt``: ``PyProjectOps.path_requirements_dev``, The requirements-dev.txt file path.
```

### Comparing `pyproject_ops-0.2.2/README.rst` & `pyproject_ops-0.2.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -75,19 +75,18 @@
 Folder Structure
 ------------------------------------------------------------------------------
 Below is the folder structured used in ``pyproject_ops``. The first item is the relative path from the project root directory. The second item is the attribute name that you can use to access the path in ``pyproject_ops``. The third item is the description of the path.
 
 - ``.venv``: ``PyProjectOps.dir_venv``, The virtualenv directory.
 - ``.venv/bin``: ``PyProjectOps.dir_venv_bin``, The bin folder in virtualenv.
 - ``.venv/bin/pip``: ``PyProjectOps.path_venv_bin_pip``, The pip command in virtualenv.
-- ``.venv/bin/poetry``: ``PyProjectOps.path_bin_poetry``, The poetry CLI command path.
 - ``.venv/bin/pytest``: ``PyProjectOps.path_venv_bin_pytest``, The pytest command in virtualenv.
+- ``.venv/bin/python``: ``PyProjectOps.path_sys_executable``, The current Python interpreter path.
 - ``.venv/bin/python``: ``PyProjectOps.path_venv_bin_python``, The python executable in virtualenv.
 - ``.venv/bin/twine``: ``PyProjectOps.path_bin_twine``, The twine CLI command path.
-- ``.venv/bin/virtualenv``: ``PyProjectOps.path_bin_virtualenv``, The virtualenv CLI command path.
 - ``build``: ``PyProjectOps.dir_build``, The build folder for Python or artifacts build.
 - ``build/lambda``: ``PyProjectOps.dir_build_lambda``, The AWS Lambda artifacts build folder.
 - ``build/lambda/layer.zip``: ``PyProjectOps.path_build_lambda_layer_zip``, The AWS Lambda layer zip file path.
 - ``build/lambda/python``: ``PyProjectOps.dir_build_lambda_python``, The AWS Lambda layer build folder. This folder contains the dependencies.
 - ``build/lambda/python/aws``: ``PyProjectOps.path_build_lambda_bin_aws``, This is the AWS CLI executable path in Lambda layer.
 - ``build/lambda/source.zip``: ``PyProjectOps.path_build_lambda_source_zip``, The AWS Lambda source code deployment package zip file path.
 - ``config``: ``PyProjectOps.dir_config``, The folder that stores the config files.
@@ -97,21 +96,23 @@
 - ``docs/build``: ``PyProjectOps.dir_sphinx_doc_build``, The temp Sphinx doc build folder.
 - ``docs/build/html``: ``PyProjectOps.dir_sphinx_doc_build_html``, The built Sphinx doc build HTML folder.
 - ``docs/build/html/index.html``: ``PyProjectOps.path_sphinx_doc_build_index_html``, The built Sphinx doc site entry HTML file path.
 - ``docs/source``: ``PyProjectOps.dir_sphinx_doc_source``, Sphinx docs source code folder.
 - ``docs/source/conf.py``: ``PyProjectOps.dir_sphinx_doc_source_conf_py``, Sphinx docs ``conf.py`` file path.
 - ``docs/source/pyproject_ops``: ``PyProjectOps.dir_sphinx_doc_source_python_lib``, The generated Python library API reference Sphinx docs folder.
 - ``htmlcov``: ``PyProjectOps.dir_htmlcov``, The code coverage test results HTML output folder.
+- ``htmlcov/index.html``: ``PyProjectOps.path_htmlcov_index_html``, The code coverage test results HTML file.
 - ``lambda_app``: ``PyProjectOps.dir_lambda_app``, The AWS Lambda app handler file and Lambda related code directory.
 - ``lambda_app/.chalice/config.json``: ``PyProjectOps.path_chalice_config``, The AWS Chalice framework's config file path.
 - ``lambda_app/.chalice/deployed``: ``PyProjectOps.dir_lambda_app_deployed``, The generated ``deployed.json`` file for AWS Chalice framework's.
 - ``lambda_app/app.py``: ``PyProjectOps.path_lambda_app_py``, The app.py file for AWS Chalice framework.
 - ``lambda_app/lambda_function.py``: ``PyProjectOps.path_lambda_function_py``, The lambda_function.py handler file for AWS Lambda, if you are not using
 - ``lambda_app/update_chalice_config.py``: ``PyProjectOps.path_lambda_update_chalice_config_script``, Example: ``${dir_project_root}/lambda_app/update_chalice_config.py``
 - ``lambda_app/vendor``: ``PyProjectOps.dir_lambda_app_vendor``, The vendor folder for AWS Chalice framework's packaging.
+- ``lambda_app/vendor/pyproject_ops``: ``PyProjectOps.dir_lambda_app_vendor_python_lib``, The source python library folder in AWS Chalice framework's vendor folder.
 - ``poetry-lock-hash.json``: ``PyProjectOps.path_poetry_lock_hash_json``, The poetry-lock-hash.json file path. It is the cache of the poetry.lock file hash.
 - ``poetry.lock``: ``PyProjectOps.path_poetry_lock``, The poetry.lock file path.
 - ``pyproject.toml``: ``PyProjectOps.path_pyproject_toml``, The pyproject.toml file path.
 - ``pyproject_ops``: ``PyProjectOps.dir_python_lib``, The current Python library directory.
 - ``pyproject_ops/_version.py``: ``PyProjectOps.path_version_py``, Path to the ``_version.py`` file where the package version is defined.
 - ``requirements-automation.txt``: ``PyProjectOps.path_requirements_automation``, The requirements-automation.txt file path.
 - ``requirements-dev.txt``: ``PyProjectOps.path_requirements_dev``, The requirements-dev.txt file path.
```

### Comparing `pyproject_ops-0.2.2/pyproject_ops/cli.py` & `pyproject_ops-0.2.3/pyproject_ops/cli.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops/ops.py` & `pyproject_ops-0.2.3/pyproject_ops/ops.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops/paths.py` & `pyproject_ops-0.2.3/pyproject_ops/paths.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops/pyproject_aws_lambda.py` & `pyproject_ops-0.2.3/pyproject_ops/pyproject_aws_lambda.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,14 +96,23 @@
         Example: ``${dir_project_root}/lambda_app/vendor``
 
         See: https://aws.github.io/chalice/topics/packaging.html
         """
         return self.dir_lambda_app.joinpath("vendor")
 
     @property
+    def dir_lambda_app_vendor_python_lib(self: "PyProjectOps") -> Path:
+        """
+        The source python library folder in AWS Chalice framework's vendor folder.
+
+        Example: ``${dir_project_root}/lambda_app/vendor/${package_name}``
+        """
+        return self.dir_lambda_app_vendor.joinpath(self.package_name)
+
+    @property
     def dir_lambda_app_deployed(self) -> Path:
         """
         The generated ``deployed.json`` file for AWS Chalice framework's.
 
         Example: ``${dir_project_root}/lambda_app/.chalice/deployed``
         """
         return self.dir_lambda_app.joinpath(".chalice", "deployed")
@@ -126,10 +135,10 @@
 
     @property
     def path_lambda_function_py(self) -> Path:
         """
         The lambda_function.py handler file for AWS Lambda, if you are not using
         framework.
 
-        Example: ``${dir_project_root}/lambda_app/app.py``
+        Example: ``${dir_project_root}/lambda_app/lambda_function.py``
         """
         return self.dir_lambda_app.joinpath("lambda_function.py")
```

### Comparing `pyproject_ops-0.2.2/pyproject_ops/pyproject_build.py` & `pyproject_ops-0.2.3/pyproject_ops/pyproject_build.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops/pyproject_config_management.py` & `pyproject_ops-0.2.3/pyproject_ops/pyproject_config_management.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops/pyproject_deps.py` & `pyproject_ops-0.2.3/pyproject_ops/pyproject_deps.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops/pyproject_docs.py` & `pyproject_ops-0.2.3/pyproject_ops/pyproject_docs.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops/pyproject_paths.py` & `pyproject_ops-0.2.3/pyproject_ops/pyproject_paths.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops/pyproject_publish.py` & `pyproject_ops-0.2.3/pyproject_ops/pyproject_publish.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops/pyproject_tests.py` & `pyproject_ops-0.2.3/pyproject_ops/pyproject_tests.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops/pyproject_venv.py` & `pyproject_ops-0.2.3/pyproject_ops/pyproject_venv.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops/vendor/build_dist.py` & `pyproject_ops-0.2.3/pyproject_ops/vendor/build_dist.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops/vendor/jsonutils.py` & `pyproject_ops-0.2.3/pyproject_ops/vendor/jsonutils.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops/vendor/nested_logger.py` & `pyproject_ops-0.2.3/pyproject_ops/vendor/nested_logger.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops/vendor/pytest_cov_helper.py` & `pyproject_ops-0.2.3/pyproject_ops/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/pyproject_ops.egg-info/PKG-INFO` & `pyproject_ops-0.2.3/pyproject_ops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyproject-ops
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python project Ops automation.
 Home-page: https://github.com/MacHu-GWU/pyproject_ops-project
-Download-URL: https://pypi.python.org/pypi/pyproject_ops/0.2.2#downloads
+Download-URL: https://pypi.python.org/pypi/pyproject_ops/0.2.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -108,19 +108,18 @@
 Folder Structure
 ------------------------------------------------------------------------------
 Below is the folder structured used in ``pyproject_ops``. The first item is the relative path from the project root directory. The second item is the attribute name that you can use to access the path in ``pyproject_ops``. The third item is the description of the path.
 
 - ``.venv``: ``PyProjectOps.dir_venv``, The virtualenv directory.
 - ``.venv/bin``: ``PyProjectOps.dir_venv_bin``, The bin folder in virtualenv.
 - ``.venv/bin/pip``: ``PyProjectOps.path_venv_bin_pip``, The pip command in virtualenv.
-- ``.venv/bin/poetry``: ``PyProjectOps.path_bin_poetry``, The poetry CLI command path.
 - ``.venv/bin/pytest``: ``PyProjectOps.path_venv_bin_pytest``, The pytest command in virtualenv.
+- ``.venv/bin/python``: ``PyProjectOps.path_sys_executable``, The current Python interpreter path.
 - ``.venv/bin/python``: ``PyProjectOps.path_venv_bin_python``, The python executable in virtualenv.
 - ``.venv/bin/twine``: ``PyProjectOps.path_bin_twine``, The twine CLI command path.
-- ``.venv/bin/virtualenv``: ``PyProjectOps.path_bin_virtualenv``, The virtualenv CLI command path.
 - ``build``: ``PyProjectOps.dir_build``, The build folder for Python or artifacts build.
 - ``build/lambda``: ``PyProjectOps.dir_build_lambda``, The AWS Lambda artifacts build folder.
 - ``build/lambda/layer.zip``: ``PyProjectOps.path_build_lambda_layer_zip``, The AWS Lambda layer zip file path.
 - ``build/lambda/python``: ``PyProjectOps.dir_build_lambda_python``, The AWS Lambda layer build folder. This folder contains the dependencies.
 - ``build/lambda/python/aws``: ``PyProjectOps.path_build_lambda_bin_aws``, This is the AWS CLI executable path in Lambda layer.
 - ``build/lambda/source.zip``: ``PyProjectOps.path_build_lambda_source_zip``, The AWS Lambda source code deployment package zip file path.
 - ``config``: ``PyProjectOps.dir_config``, The folder that stores the config files.
@@ -130,21 +129,23 @@
 - ``docs/build``: ``PyProjectOps.dir_sphinx_doc_build``, The temp Sphinx doc build folder.
 - ``docs/build/html``: ``PyProjectOps.dir_sphinx_doc_build_html``, The built Sphinx doc build HTML folder.
 - ``docs/build/html/index.html``: ``PyProjectOps.path_sphinx_doc_build_index_html``, The built Sphinx doc site entry HTML file path.
 - ``docs/source``: ``PyProjectOps.dir_sphinx_doc_source``, Sphinx docs source code folder.
 - ``docs/source/conf.py``: ``PyProjectOps.dir_sphinx_doc_source_conf_py``, Sphinx docs ``conf.py`` file path.
 - ``docs/source/pyproject_ops``: ``PyProjectOps.dir_sphinx_doc_source_python_lib``, The generated Python library API reference Sphinx docs folder.
 - ``htmlcov``: ``PyProjectOps.dir_htmlcov``, The code coverage test results HTML output folder.
+- ``htmlcov/index.html``: ``PyProjectOps.path_htmlcov_index_html``, The code coverage test results HTML file.
 - ``lambda_app``: ``PyProjectOps.dir_lambda_app``, The AWS Lambda app handler file and Lambda related code directory.
 - ``lambda_app/.chalice/config.json``: ``PyProjectOps.path_chalice_config``, The AWS Chalice framework's config file path.
 - ``lambda_app/.chalice/deployed``: ``PyProjectOps.dir_lambda_app_deployed``, The generated ``deployed.json`` file for AWS Chalice framework's.
 - ``lambda_app/app.py``: ``PyProjectOps.path_lambda_app_py``, The app.py file for AWS Chalice framework.
 - ``lambda_app/lambda_function.py``: ``PyProjectOps.path_lambda_function_py``, The lambda_function.py handler file for AWS Lambda, if you are not using
 - ``lambda_app/update_chalice_config.py``: ``PyProjectOps.path_lambda_update_chalice_config_script``, Example: ``${dir_project_root}/lambda_app/update_chalice_config.py``
 - ``lambda_app/vendor``: ``PyProjectOps.dir_lambda_app_vendor``, The vendor folder for AWS Chalice framework's packaging.
+- ``lambda_app/vendor/pyproject_ops``: ``PyProjectOps.dir_lambda_app_vendor_python_lib``, The source python library folder in AWS Chalice framework's vendor folder.
 - ``poetry-lock-hash.json``: ``PyProjectOps.path_poetry_lock_hash_json``, The poetry-lock-hash.json file path. It is the cache of the poetry.lock file hash.
 - ``poetry.lock``: ``PyProjectOps.path_poetry_lock``, The poetry.lock file path.
 - ``pyproject.toml``: ``PyProjectOps.path_pyproject_toml``, The pyproject.toml file path.
 - ``pyproject_ops``: ``PyProjectOps.dir_python_lib``, The current Python library directory.
 - ``pyproject_ops/_version.py``: ``PyProjectOps.path_version_py``, Path to the ``_version.py`` file where the package version is defined.
 - ``requirements-automation.txt``: ``PyProjectOps.path_requirements_automation``, The requirements-automation.txt file path.
 - ``requirements-dev.txt``: ``PyProjectOps.path_requirements_dev``, The requirements-dev.txt file path.
```

### Comparing `pyproject_ops-0.2.2/pyproject_ops.egg-info/SOURCES.txt` & `pyproject_ops-0.2.3/pyproject_ops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/release-history.rst` & `pyproject_ops-0.2.3/release-history.rst`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.2.3 (2023-07-03)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Minor Improvements**
+
+- add ``dir_lambda_app_vendor_python_lib`` path.
+
+
 0.2.2 (2023-06-14)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - fix a bug that ``pyops publish`` command forget to install dev dependencies.
 
 **Miscellaneous**
```

### Comparing `pyproject_ops-0.2.2/requirements-doc.txt` & `pyproject_ops-0.2.3/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/setup.py` & `pyproject_ops-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyproject_ops-0.2.2/tests/test_pyproject_ops.py` & `pyproject_ops-0.2.3/tests/test_pyproject_ops.py`

 * *Files identical despite different names*

