# Comparing `tmp/pyatlan-0.2.0.tar.gz` & `tmp/pyatlan-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.2.0.tar", last modified: Fri Jun 30 12:17:20 2023, max compression
+gzip compressed data, was "pyatlan-0.3.0.tar", last modified: Mon Jul  3 11:36:01 2023, max compression
```

## Comparing `pyatlan-0.2.0.tar` & `pyatlan-0.3.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.100695 pyatlan-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-30 12:17:06.000000 pyatlan-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 12:17:06.000000 pyatlan-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-30 12:17:06.000000 pyatlan-0.2.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-30 12:17:20.100695 pyatlan-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-30 12:17:06.000000 pyatlan-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.080695 pyatlan-0.2.0/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.084695 pyatlan-0.2.0/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/cache/atlan_tag_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.084695 pyatlan-0.2.0/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47536 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.084695 pyatlan-0.2.0/pyatlan/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/events/atlan_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/events/atlan_lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.084695 pyatlan-0.2.0/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.084695 pyatlan-0.2.0/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.088696 pyatlan-0.2.0/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   982643 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/atlan_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    56219 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    60973 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24877 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 12:17:06.000000 pyatlan-0.2.0/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.080695 pyatlan-0.2.0/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-30 12:17:20.000000 pyatlan-0.2.0/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-30 12:17:20.000000 pyatlan-0.2.0/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:17:20.000000 pyatlan-0.2.0/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:17:19.000000 pyatlan-0.2.0/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 12:17:20.000000 pyatlan-0.2.0/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 12:17:20.000000 pyatlan-0.2.0/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:17:20.100695 pyatlan-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-30 12:17:06.000000 pyatlan-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.088696 pyatlan-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.092696 pyatlan-0.2.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/atlan_tag_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    35670 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/lineage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/persona_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/purpose_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/s3_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/test_index_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/integration/test_sql_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.096696 pyatlan-0.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:20.100695 pyatlan-0.2.0/tests/unit/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/badge_condition_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/badge_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/column_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/glossary_category_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/glossary_term_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/materialised_view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/process_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/readme_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/s3_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/s3object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/model/view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_atlan_tag_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    30532 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    30268 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36634 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-30 12:17:06.000000 pyatlan-0.2.0/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.562886 pyatlan-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-07-03 11:35:48.000000 pyatlan-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 11:35:48.000000 pyatlan-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 11:35:48.000000 pyatlan-0.3.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-03 11:36:01.562886 pyatlan-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-03 11:35:48.000000 pyatlan-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.542884 pyatlan-0.3.0/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.546885 pyatlan-0.3.0/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/cache/atlan_tag_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.546885 pyatlan-0.3.0/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47536 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.546885 pyatlan-0.3.0/pyatlan/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/events/atlan_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/events/atlan_lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.546885 pyatlan-0.3.0/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.546885 pyatlan-0.3.0/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.550885 pyatlan-0.3.0/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   982643 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/atlan_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56208 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60973 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.542884 pyatlan-0.3.0/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-03 11:36:01.000000 pyatlan-0.3.0/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-03 11:36:01.000000 pyatlan-0.3.0/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:36:01.000000 pyatlan-0.3.0/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:36:01.000000 pyatlan-0.3.0/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 11:36:01.000000 pyatlan-0.3.0/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 11:36:01.000000 pyatlan-0.3.0/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:36:01.562886 pyatlan-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-03 11:35:48.000000 pyatlan-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.550885 pyatlan-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.554885 pyatlan-0.3.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/atlan_tag_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35670 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/persona_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/purpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/test_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/test_sql_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.558885 pyatlan-0.3.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.562886 pyatlan-0.3.0/tests/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/badge_condition_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/badge_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/column_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/glossary_category_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/glossary_term_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/materialised_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/process_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/readme_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/s3_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/s3object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_atlan_tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30532 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30268 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36634 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.2.0/LICENSE` & `pyatlan-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/PKG-INFO` & `pyatlan-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.2.0
+Version: 0.3.0
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.2.0/README.md` & `pyatlan-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/cache/atlan_tag_cache.py` & `pyatlan-0.3.0/pyatlan/cache/atlan_tag_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.3.0/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/cache/enum_cache.py` & `pyatlan-0.3.0/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/cache/group_cache.py` & `pyatlan-0.3.0/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/cache/role_cache.py` & `pyatlan-0.3.0/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/cache/user_cache.py` & `pyatlan-0.3.0/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/client/atlan.py` & `pyatlan-0.3.0/pyatlan/client/atlan.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/client/constants.py` & `pyatlan-0.3.0/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/error.py` & `pyatlan-0.3.0/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/events/atlan_event_handler.py` & `pyatlan-0.3.0/pyatlan/events/atlan_event_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/events/atlan_lambda_handler.py` & `pyatlan-0.3.0/pyatlan/events/atlan_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/exceptions.py` & `pyatlan-0.3.0/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.3.0/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/model/assets.py` & `pyatlan-0.3.0/pyatlan/model/assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/model/atlan_image.py` & `pyatlan-0.3.0/pyatlan/model/atlan_image.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/model/core.py` & `pyatlan-0.3.0/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/model/custom_metadata.py` & `pyatlan-0.3.0/pyatlan/model/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/model/enums.py` & `pyatlan-0.3.0/pyatlan/model/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
     PPT = "ppt"
     TXT = "txt"
     XLS = "xls"
     XML = "xml"
     ZIP = "zip"
 
 
-class AtlanClassificationColor(str, Enum):
+class AtlanTagColor(str, Enum):
     GREEN = "Green"
     YELLOW = "Yellow"
     RED = "Red"
     GRAY = "Gray"
 
 
 class QueryParserSourceType(str, Enum):
```

### Comparing `pyatlan-0.2.0/pyatlan/model/events.py` & `pyatlan-0.3.0/pyatlan/model/events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/model/group.py` & `pyatlan-0.3.0/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/model/lineage.py` & `pyatlan-0.3.0/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/model/query.py` & `pyatlan-0.3.0/pyatlan/model/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/model/response.py` & `pyatlan-0.3.0/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/model/role.py` & `pyatlan-0.3.0/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/model/search.py` & `pyatlan-0.3.0/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/model/structs.py` & `pyatlan-0.3.0/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/model/typedef.py` & `pyatlan-0.3.0/pyatlan/model/typedef.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from typing import Any, Dict, List, Optional
 
 from pydantic import Field
 
 from pyatlan.model.atlan_image import AtlanImage
 from pyatlan.model.core import AtlanObject
 from pyatlan.model.enums import (
-    AtlanClassificationColor,
     AtlanCustomAttributePrimitiveType,
     AtlanIcon,
+    AtlanTagColor,
     AtlanTypeCategory,
     Cardinality,
     IconType,
     IndexType,
 )
 
 _complete_type_list = (
@@ -492,15 +492,15 @@
         description="Name used for display purposes (in user interfaces)."
     )
     skip_display_name_uniqueness_check: Optional[bool] = Field(description="TBC")
 
     @staticmethod
     def create(
         name: str,
-        color: AtlanClassificationColor,
+        color: AtlanTagColor,
         icon: AtlanIcon = AtlanIcon.ATLAN_TAG,
         image: Optional[AtlanImage] = None,
     ) -> AtlanTagDef:
         from pyatlan.model.assets import validate_required_fields
 
         validate_required_fields(
             ["name", "color"],
```

### Comparing `pyatlan-0.2.0/pyatlan/model/user.py` & `pyatlan-0.3.0/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/multipart_data_generator.py` & `pyatlan-0.3.0/pyatlan/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan/utils.py` & `pyatlan-0.3.0/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.3.0/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.2.0
+Version: 0.3.0
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.2.0/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.3.0/pyatlan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/setup.py` & `pyatlan-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/integration/admin_test.py` & `pyatlan-0.3.0/tests/integration/admin_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/integration/client.py` & `pyatlan-0.3.0/tests/integration/client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/integration/connection_test.py` & `pyatlan-0.3.0/tests/integration/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/integration/custom_metadata_test.py` & `pyatlan-0.3.0/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/integration/file_test.py` & `pyatlan-0.3.0/tests/integration/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/integration/glossary_test.py` & `pyatlan-0.3.0/tests/integration/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/integration/lineage_test.py` & `pyatlan-0.3.0/tests/integration/lineage_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/integration/persona_test.py` & `pyatlan-0.3.0/tests/integration/persona_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/integration/purpose_test.py` & `pyatlan-0.3.0/tests/integration/purpose_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import pytest
 
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.assets import AuthPolicy, Purpose
 from pyatlan.model.enums import (
     AssetSidebarTab,
-    AtlanClassificationColor,
+    AtlanTagColor,
     AuthPolicyType,
     DataAction,
     DataMaskingType,
     PurposeMetadataAction,
 )
 from pyatlan.model.typedef import AtlanTagDef
 from tests.integration.client import TestId, delete_asset
@@ -21,17 +21,15 @@
 MODULE_NAME = TestId.make_unique("Purpose")
 
 
 @pytest.fixture(scope="module")
 def atlan_tag(
     client: AtlanClient,
 ) -> Generator[AtlanTagDef, None, None]:
-    atlan_tag_def = AtlanTagDef.create(
-        name=MODULE_NAME, color=AtlanClassificationColor.GREEN
-    )
+    atlan_tag_def = AtlanTagDef.create(name=MODULE_NAME, color=AtlanTagColor.GREEN)
     typedef = client.create_typedef(atlan_tag_def)
     yield typedef.atlan_tag_defs[0]
     client.purge_typedef(MODULE_NAME, typedef_type=AtlanTagDef)
 
 
 @pytest.fixture(scope="module")
 def purpose(
```

### Comparing `pyatlan-0.2.0/tests/integration/query_parser_test.py` & `pyatlan-0.3.0/tests/integration/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/integration/s3_asset_test.py` & `pyatlan-0.3.0/tests/integration/s3_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/integration/test_client.py` & `pyatlan-0.3.0/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/integration/test_index_search.py` & `pyatlan-0.3.0/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/integration/test_sql_assets.py` & `pyatlan-0.3.0/tests/integration/test_sql_assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/conftest.py` & `pyatlan-0.3.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/badge_condition_test.py` & `pyatlan-0.3.0/tests/unit/model/badge_condition_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/badge_test.py` & `pyatlan-0.3.0/tests/unit/model/badge_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/column_test.py` & `pyatlan-0.3.0/tests/unit/model/column_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/connection_test.py` & `pyatlan-0.3.0/tests/unit/model/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/constants.py` & `pyatlan-0.3.0/tests/unit/model/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/database_test.py` & `pyatlan-0.3.0/tests/unit/model/database_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/file_test.py` & `pyatlan-0.3.0/tests/unit/model/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/glossary_category_test.py` & `pyatlan-0.3.0/tests/unit/model/glossary_category_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/glossary_term_test.py` & `pyatlan-0.3.0/tests/unit/model/glossary_term_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/glossary_test.py` & `pyatlan-0.3.0/tests/unit/model/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/materialised_view_test.py` & `pyatlan-0.3.0/tests/unit/model/materialised_view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/process_test.py` & `pyatlan-0.3.0/tests/unit/model/process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/readme_test.py` & `pyatlan-0.3.0/tests/unit/model/readme_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/s3_bucket_test.py` & `pyatlan-0.3.0/tests/unit/model/s3_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/s3object_test.py` & `pyatlan-0.3.0/tests/unit/model/s3object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/schema_test.py` & `pyatlan-0.3.0/tests/unit/model/schema_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/table_test.py` & `pyatlan-0.3.0/tests/unit/model/table_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/model/view_test.py` & `pyatlan-0.3.0/tests/unit/model/view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/test_atlan_tag_name.py` & `pyatlan-0.3.0/tests/unit/test_atlan_tag_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/test_client.py` & `pyatlan-0.3.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/test_custom_metadata.py` & `pyatlan-0.3.0/tests/unit/test_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/test_events.py` & `pyatlan-0.3.0/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/test_glossary_term.py` & `pyatlan-0.3.0/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/test_lineage.py` & `pyatlan-0.3.0/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/test_model.py` & `pyatlan-0.3.0/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/test_search_model.py` & `pyatlan-0.3.0/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.2.0/tests/unit/test_typedef_model.py` & `pyatlan-0.3.0/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

