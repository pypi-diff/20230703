# Comparing `tmp/bx_py_utils-85.tar.gz` & `tmp/bx_py_utils-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bx_py_utils-85.tar", max compression
+gzip compressed data, was "bx_py_utils-9.tar", last modified: Tue Dec  1 10:30:17 2020, max compression
```

## Comparing `bx_py_utils-85.tar` & `bx_py_utils-9.tar`

### file list

```diff
@@ -1,52 +1,19 @@
--rw-r--r--   0        0        0     1068 2022-10-27 04:56:32.000000 bx_py_utils-85/LICENSE
--rw-r--r--   0        0        0    19616 2023-07-03 10:10:49.832467 bx_py_utils-85/README.md
--rw-r--r--   0        0        0       78 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/__init__.py
--rw-r--r--   0        0        0     1273 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/anonymize.py
--rw-r--r--   0        0        0     6775 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/auto_doc.py
--rw-r--r--   0        0        0        0 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/aws/__init__.py
--rw-r--r--   0        0        0     2267 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/aws/client_side_cert_manager.py
--rw-r--r--   0        0        0      989 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/aws/secret_manager.py
--rw-r--r--   0        0        0      425 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/compat.py
--rw-r--r--   0        0        0      817 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/dict_utils.py
--rw-r--r--   0        0        0     2204 2023-07-03 11:13:53.724492 bx_py_utils-85/bx_py_utils/doc_write/README.md
--rw-r--r--   0        0        0      110 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/doc_write/__init__.py
--rw-r--r--   0        0        0      556 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/doc_write/__main__.py
--rw-r--r--   0        0        0     2230 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/doc_write/api.py
--rw-r--r--   0        0        0     1793 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/doc_write/cfg.py
--rw-r--r--   0        0        0     2878 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/doc_write/docstrings.py
--rw-r--r--   0        0        0      164 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/doc_write/walk.py
--rw-r--r--   0        0        0     1472 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/environ.py
--rw-r--r--   0        0        0     2239 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/error_handling.py
--rw-r--r--   0        0        0     6986 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/file_utils.py
--rw-r--r--   0        0        0      696 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/filename_matcher.py
--rw-r--r--   0        0        0     3320 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/graphql_introspection.py
--rw-r--r--   0        0        0     1330 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/hash_utils.py
--rw-r--r--   0        0        0     2850 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/html_utils.py
--rw-r--r--   0        0        0        0 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/humanize/__init__.py
--rw-r--r--   0        0        0      419 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/humanize/pformat.py
--rw-r--r--   0        0        0     1286 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/humanize/time.py
--rw-r--r--   0        0        0      592 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/iteration.py
--rw-r--r--   0        0        0     1673 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/path.py
--rw-r--r--   0        0        0     1511 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/processify.py
--rw-r--r--   0        0        0     1257 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/pyproject_toml.py
--rw-r--r--   0        0        0      862 2023-07-03 08:26:58.165749 bx_py_utils-85/bx_py_utils/rison.py
--rw-r--r--   0        0        0     1150 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/stack_info.py
--rw-r--r--   0        0        0     3741 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/string_utils.py
--rw-r--r--   0        0        0        0 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/test_utils/__init__.py
--rw-r--r--   0        0        0     3000 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/test_utils/assertion.py
--rw-r--r--   0        0        0      646 2023-06-13 01:48:26.665179 bx_py_utils-85/bx_py_utils/test_utils/context_managers.py
--rw-r--r--   0        0        0      384 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/test_utils/datetime.py
--rw-r--r--   0        0        0     1335 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/test_utils/filesystem_utils.py
--rw-r--r--   0        0        0      873 2023-07-03 11:10:20.482163 bx_py_utils-85/bx_py_utils/test_utils/log_utils.py
--rw-r--r--   0        0        0      443 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/test_utils/mock_aws_secret_manager.py
--rw-r--r--   0        0        0     1388 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/test_utils/mock_boto3session.py
--rw-r--r--   0        0        0      618 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/test_utils/mock_uuid.py
--rw-r--r--   0        0        0     8046 2023-06-13 01:48:26.669179 bx_py_utils-85/bx_py_utils/test_utils/mocks3.py
--rw-r--r--   0        0        0      890 2023-06-13 01:48:26.669179 bx_py_utils-85/bx_py_utils/test_utils/redirect.py
--rw-r--r--   0        0        0     2763 2023-06-13 01:48:26.669179 bx_py_utils-85/bx_py_utils/test_utils/requests_mock_assertion.py
--rw-r--r--   0        0        0    12530 2023-06-13 01:48:26.669179 bx_py_utils-85/bx_py_utils/test_utils/snapshot.py
--rw-r--r--   0        0        0      430 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/test_utils/time.py
--rw-r--r--   0        0        0     3072 2023-06-13 01:48:26.669179 bx_py_utils-85/bx_py_utils/test_utils/unittest_utils.py
--rw-r--r--   0        0        0      906 2022-10-27 04:56:32.000000 bx_py_utils-85/bx_py_utils/text_tools.py
--rw-r--r--   0        0        0     4291 2023-07-03 11:13:48.956441 bx_py_utils-85/pyproject.toml
--rw-r--r--   0        0        0    20472 1970-01-01 00:00:00.000000 bx_py_utils-85/PKG-INFO
+-rw-r--r--   0        0        0     1068 2020-10-06 11:18:24.585248 bx_py_utils-9/LICENSE
+-rw-r--r--   0        0        0     1076 2020-11-11 13:09:04.294093 bx_py_utils-9/README.md
+-rw-r--r--   0        0        0       18 2020-12-01 09:39:26.919684 bx_py_utils-9/bx_py_utils/__init__.py
+-rw-r--r--   0        0        0      792 2020-11-20 07:55:57.394159 bx_py_utils-9/bx_py_utils/dict_utils.py
+-rw-r--r--   0        0        0     2239 2020-10-29 14:48:12.468364 bx_py_utils-9/bx_py_utils/error_handling.py
+-rw-r--r--   0        0        0     1207 2020-11-09 08:12:19.613621 bx_py_utils-9/bx_py_utils/filename.py
+-rw-r--r--   0        0        0      586 2020-10-16 13:19:54.440559 bx_py_utils-9/bx_py_utils/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      591 2020-10-16 13:13:10.852321 bx_py_utils-9/bx_py_utils/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      574 2020-10-16 13:19:54.444559 bx_py_utils-9/bx_py_utils/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      579 2020-10-16 13:13:10.848321 bx_py_utils-9/bx_py_utils/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-10-06 11:34:03.065746 bx_py_utils-9/bx_py_utils/models/__init__.py
+-rw-r--r--   0        0        0     1155 2020-12-01 09:37:02.157158 bx_py_utils-9/bx_py_utils/models/manipulate.py
+-rw-r--r--   0        0        0     1744 2020-10-16 13:05:21.808604 bx_py_utils-9/bx_py_utils/models/timetracking.py
+-rw-r--r--   0        0        0        0 2020-11-11 13:06:05.859777 bx_py_utils-9/bx_py_utils/test_utils/__init__.py
+-rw-r--r--   0        0        0      802 2020-11-11 13:07:27.819001 bx_py_utils-9/bx_py_utils/test_utils/datetime.py
+-rw-r--r--   0        0        0     2667 2020-11-30 14:16:06.000000 bx_py_utils-9/bx_py_utils/test_utils/model_clean_assert.py
+-rw-r--r--   0        0        0      926 2020-12-01 10:30:13.639173 bx_py_utils-9/pyproject.toml
+-rw-r--r--   0        0        0     2000 2020-12-01 10:30:17.219518 bx_py_utils-9/setup.py
+-rw-r--r--   0        0        0     1860 2020-12-01 10:30:17.219777 bx_py_utils-9/PKG-INFO
```

### Comparing `bx_py_utils-85/LICENSE` & `bx_py_utils-9/LICENSE`

 * *Files identical despite different names*

### Comparing `bx_py_utils-85/bx_py_utils/dict_utils.py` & `bx_py_utils-9/bx_py_utils/dict_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Iterable
 
 
 def dict_get(item, *keys):
     """
-    nested dict `get()`
-
     >>> example={1: {2: 'X'}}
     >>> dict_get(example, 1, 2)
     'X'
     >>> dict_get(example, 1)
     {2: 'X'}
     >>> dict_get(example, 1, 2, 3) is None
     True
```

### Comparing `bx_py_utils-85/bx_py_utils/error_handling.py` & `bx_py_utils-9/bx_py_utils/error_handling.py`

 * *Files identical despite different names*

