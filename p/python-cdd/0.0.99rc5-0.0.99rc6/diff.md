# Comparing `tmp/python-cdd-0.0.99rc5.tar.gz` & `tmp/python-cdd-0.0.99rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-cdd-0.0.99rc5.tar", last modified: Sat Jul  1 02:50:09 2023, max compression
+gzip compressed data, was "python-cdd-0.0.99rc6.tar", last modified: Mon Jul  3 02:34:41 2023, max compression
```

## Comparing `python-cdd-0.0.99rc5.tar` & `python-cdd-0.0.99rc6.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.181331 python-cdd-0.0.99rc5/
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (123)    33371 2023-07-01 02:50:09.181331 python-cdd-0.0.99rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31663 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.157331 python-cdd-0.0.99rc5/cdd/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17081 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.157331 python-cdd-0.0.99rc5/cdd/argparse_function/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/argparse_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/argparse_function/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/argparse_function/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.157331 python-cdd-0.0.99rc5/cdd/argparse_function/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/argparse_function/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/argparse_function/utils/emit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.157331 python-cdd-0.0.99rc5/cdd/class_/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/class_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/class_/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/class_/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.157331 python-cdd-0.0.99rc5/cdd/class_/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/class_/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/class_/utils/emit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/class_/utils/parse_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/compound/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/doctrans.py
--rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/doctrans_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/exmod.py
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/exmod_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/gen_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/compound/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/gen_openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/gen_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/compound/openapi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/utils/emit_openapi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25134 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/utils/emit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/utils/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/sync_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/docstring/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/docstring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/docstring/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/docstring/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/docstring/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/docstring/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/docstring/utils/emit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/function/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/function/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/function/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/function/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/function/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/function/utils/emit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/function/utils/parse_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/json_schema/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/json_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/json_schema/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/json_schema/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/json_schema/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/json_schema/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/json_schema/utils/emit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/json_schema/utils/parse_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/pydantic/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/pydantic/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/routes/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/routes/emit/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/emit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/emit/bottle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/emit/bottle_constants_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/routes/parse/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/parse/bottle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/parse/bottle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/parse/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/parse/fastapi_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/ast_cst_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    59574 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/cst.py
--rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/cst_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/defaults_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36707 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/docstring_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    24541 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/docstring_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/shared/emit/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/emit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/emit/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/shared/emit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/emit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/emit/utils/emitter_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/shared/parse/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/parse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/shared/parse/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/parse/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/parse/utils/parser_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/pkg_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35026 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/pure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/source_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/sqlalchemy/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/sqlalchemy/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.169331 python-cdd-0.0.99rc5/cdd/sqlalchemy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/sqlalchemy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/sqlalchemy/utils/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/sqlalchemy/utils/shared_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.169331 python-cdd-0.0.99rc5/cdd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.169331 python-cdd-0.0.99rc5/cdd/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34014 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    47192 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/cst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/cstify.py
--rw-r--r--   0 runner    (1001) docker     (123)    35593 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/doctrans.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/exmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/fastapi_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    42393 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    33730 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)    18892 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.169331 python-cdd-0.0.99rc5/cdd/tests/test_argparse_function/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_argparse_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_argparse_function/test_emit_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_argparse_function/test_parse_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_ast_equality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.169331 python-cdd-0.0.99rc5/cdd/tests/test_class/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_class/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_class/test_emit_class_.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_class/test_parse_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.173331 python-cdd-0.0.99rc5/cdd/tests/test_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_doctrans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_exmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_gen_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_sync_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.173331 python-cdd-0.0.99rc5/cdd/tests/test_compound/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_doctrans.py
--rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_doctrans_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24367 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_exmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_exmod_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_gen_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_gen_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_openapi_bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_openapi_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_sync_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.173331 python-cdd-0.0.99rc5/cdd/tests/test_docstring/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_docstring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_docstring/test_emit_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_docstring/test_parse_docstring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.177332 python-cdd-0.0.99rc5/cdd/tests/test_emit/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_emit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_emit/test_emit_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_emit/test_emitter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_emit/test_emitters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.177332 python-cdd-0.0.99rc5/cdd/tests/test_function/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_function/test_emit_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_function/test_parse_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.177332 python-cdd-0.0.99rc5/cdd/tests/test_json_schema/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_json_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_emit_json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_emit_json_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_parse_json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_parse_json_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_marshall_docstring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.177332 python-cdd-0.0.99rc5/cdd/tests/test_parse/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_parse/test_parser_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_parse/test_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.177332 python-cdd-0.0.99rc5/cdd/tests/test_pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_pydantic/test_emit_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_pydantic/test_parse_pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.177332 python-cdd-0.0.99rc5/cdd/tests/test_routes/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_routes/test_bottle_route_emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_routes/test_bottle_route_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_routes/test_fastapi_routes_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_routes/test_route_emit.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_routes/test_route_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.181331 python-cdd-0.0.99rc5/cdd/tests/test_shared/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_ast_cst_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    41239 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_cst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_cst_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_default_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_docstring_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_pkg_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_pure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_source_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.181331 python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_utils_for_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    12968 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/utils_for_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.181331 python-cdd-0.0.99rc5/python_cdd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33371 2023-07-01 02:50:09.000000 python-cdd-0.0.99rc5/python_cdd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-07-01 02:50:09.000000 python-cdd-0.0.99rc5/python_cdd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 02:50:09.000000 python-cdd-0.0.99rc5/python_cdd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-01 02:50:09.000000 python-cdd-0.0.99rc5/python_cdd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-01 02:50:09.000000 python-cdd-0.0.99rc5/python_cdd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 02:50:09.181331 python-cdd-0.0.99rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.354981 python-cdd-0.0.99rc6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (123)    33371 2023-07-03 02:34:41.354981 python-cdd-0.0.99rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31663 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.334981 python-cdd-0.0.99rc6/cdd/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17081 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.334981 python-cdd-0.0.99rc6/cdd/argparse_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/argparse_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/argparse_function/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/argparse_function/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.334981 python-cdd-0.0.99rc6/cdd/argparse_function/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/argparse_function/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/argparse_function/utils/emit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.334981 python-cdd-0.0.99rc6/cdd/class_/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/class_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/class_/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/class_/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.334981 python-cdd-0.0.99rc6/cdd/class_/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/class_/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/class_/utils/emit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/class_/utils/parse_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.334981 python-cdd-0.0.99rc6/cdd/compound/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/doctrans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/doctrans_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/exmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/exmod_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/gen_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.334981 python-cdd-0.0.99rc6/cdd/compound/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/openapi/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/openapi/gen_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/openapi/gen_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/openapi/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.334981 python-cdd-0.0.99rc6/cdd/compound/openapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/openapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/openapi/utils/emit_openapi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25134 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/openapi/utils/emit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/openapi/utils/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/compound/sync_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.338981 python-cdd-0.0.99rc6/cdd/docstring/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/docstring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/docstring/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/docstring/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.338981 python-cdd-0.0.99rc6/cdd/docstring/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/docstring/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/docstring/utils/emit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.338981 python-cdd-0.0.99rc6/cdd/function/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/function/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/function/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.338981 python-cdd-0.0.99rc6/cdd/function/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/function/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/function/utils/emit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/function/utils/parse_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.338981 python-cdd-0.0.99rc6/cdd/json_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/json_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/json_schema/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/json_schema/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.338981 python-cdd-0.0.99rc6/cdd/json_schema/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/json_schema/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/json_schema/utils/emit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/json_schema/utils/parse_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.338981 python-cdd-0.0.99rc6/cdd/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/pydantic/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/pydantic/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.338981 python-cdd-0.0.99rc6/cdd/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.338981 python-cdd-0.0.99rc6/cdd/routes/emit/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/routes/emit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/routes/emit/bottle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/routes/emit/bottle_constants_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.338981 python-cdd-0.0.99rc6/cdd/routes/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/routes/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/routes/parse/bottle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/routes/parse/bottle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/routes/parse/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/routes/parse/fastapi_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.342981 python-cdd-0.0.99rc6/cdd/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/ast_cst_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59574 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/cst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/cst_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/defaults_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36707 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/docstring_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24541 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/docstring_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.342981 python-cdd-0.0.99rc6/cdd/shared/emit/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/emit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/emit/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.342981 python-cdd-0.0.99rc6/cdd/shared/emit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/emit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/emit/utils/emitter_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.342981 python-cdd-0.0.99rc6/cdd/shared/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/parse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.342981 python-cdd-0.0.99rc6/cdd/shared/parse/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/parse/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/parse/utils/parser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/pkg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35026 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/pure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/shared/source_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.342981 python-cdd-0.0.99rc6/cdd/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/sqlalchemy/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/sqlalchemy/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.342981 python-cdd-0.0.99rc6/cdd/sqlalchemy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/sqlalchemy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/sqlalchemy/utils/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/sqlalchemy/utils/shared_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.342981 python-cdd-0.0.99rc6/cdd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.346981 python-cdd-0.0.99rc6/cdd/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34014 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47192 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/cst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/cstify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35593 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/doctrans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/exmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/fastapi_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42393 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33730 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18892 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/mocks/sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.346981 python-cdd-0.0.99rc6/cdd/tests/test_argparse_function/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_argparse_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_argparse_function/test_emit_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_argparse_function/test_parse_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_ast_equality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.346981 python-cdd-0.0.99rc6/cdd/tests/test_class/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_class/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_class/test_emit_class_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_class/test_parse_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.346981 python-cdd-0.0.99rc6/cdd/tests/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli_doctrans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli_exmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli_gen_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli_sync_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.346981 python-cdd-0.0.99rc6/cdd/tests/test_compound/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_compound/test_doctrans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_compound/test_doctrans_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25230 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_compound/test_exmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_compound/test_exmod_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_compound/test_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_compound/test_gen_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_compound/test_gen_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_compound/test_openapi_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_compound/test_openapi_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_compound/test_sync_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.350981 python-cdd-0.0.99rc6/cdd/tests/test_docstring/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_docstring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_docstring/test_emit_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_docstring/test_parse_docstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.350981 python-cdd-0.0.99rc6/cdd/tests/test_emit/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_emit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_emit/test_emit_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_emit/test_emitter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_emit/test_emitters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.350981 python-cdd-0.0.99rc6/cdd/tests/test_function/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_function/test_emit_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_function/test_parse_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.350981 python-cdd-0.0.99rc6/cdd/tests/test_json_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_json_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_json_schema/test_emit_json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_json_schema/test_emit_json_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_json_schema/test_parse_json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_json_schema/test_parse_json_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_marshall_docstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.350981 python-cdd-0.0.99rc6/cdd/tests/test_parse/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_parse/test_parser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_parse/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.350981 python-cdd-0.0.99rc6/cdd/tests/test_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_pydantic/test_emit_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_pydantic/test_parse_pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.350981 python-cdd-0.0.99rc6/cdd/tests/test_routes/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_routes/test_bottle_route_emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_routes/test_bottle_route_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_routes/test_fastapi_routes_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_routes/test_route_emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_routes/test_route_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.354981 python-cdd-0.0.99rc6/cdd/tests/test_shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_shared/test_ast_cst_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41239 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_shared/test_ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_shared/test_conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_shared/test_cst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_shared/test_cst_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_shared/test_default_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_shared/test_docstring_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_shared/test_pkg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_shared/test_pure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_shared/test_source_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.354981 python-cdd-0.0.99rc6/cdd/tests/test_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/test_utils_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12968 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/cdd/tests/utils_for_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:34:41.354981 python-cdd-0.0.99rc6/python_cdd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33371 2023-07-03 02:34:41.000000 python-cdd-0.0.99rc6/python_cdd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-07-03 02:34:41.000000 python-cdd-0.0.99rc6/python_cdd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 02:34:41.000000 python-cdd-0.0.99rc6/python_cdd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 02:34:41.000000 python-cdd-0.0.99rc6/python_cdd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-03 02:34:41.000000 python-cdd-0.0.99rc6/python_cdd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 02:34:41.354981 python-cdd-0.0.99rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-03 02:33:59.000000 python-cdd-0.0.99rc6/setup.py
```

### Comparing `python-cdd-0.0.99rc5/LICENSE-APACHE` & `python-cdd-0.0.99rc6/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/LICENSE-MIT` & `python-cdd-0.0.99rc6/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/PKG-INFO` & `python-cdd-0.0.99rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cdd
-Version: 0.0.99rc5
+Version: 0.0.99rc6
 Summary: Open API to/fro routes, models, and tests. Convert between docstrings, classes, methods, argparse, pydantic, and SQLalchemy.
 Home-page: https://github.com/offscale/cdd-python
 Author: Samuel Marks
 Author-email: 807580+SamuelMarks@users.noreply.github.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `python-cdd-0.0.99rc5/README.md` & `python-cdd-0.0.99rc6/README.md`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/__main__.py` & `python-cdd-0.0.99rc6/cdd/__main__.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/argparse_function/emit.py` & `python-cdd-0.0.99rc6/cdd/argparse_function/emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/argparse_function/parse.py` & `python-cdd-0.0.99rc6/cdd/argparse_function/parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/argparse_function/utils/emit_utils.py` & `python-cdd-0.0.99rc6/cdd/argparse_function/utils/emit_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/class_/emit.py` & `python-cdd-0.0.99rc6/cdd/class_/emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/class_/parse.py` & `python-cdd-0.0.99rc6/cdd/class_/parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/class_/utils/emit_utils.py` & `python-cdd-0.0.99rc6/cdd/class_/utils/emit_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/class_/utils/parse_utils.py` & `python-cdd-0.0.99rc6/cdd/class_/utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/compound/doctrans.py` & `python-cdd-0.0.99rc6/cdd/compound/doctrans.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/compound/doctrans_utils.py` & `python-cdd-0.0.99rc6/cdd/compound/doctrans_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/compound/exmod.py` & `python-cdd-0.0.99rc6/cdd/compound/exmod.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/compound/exmod_utils.py` & `python-cdd-0.0.99rc6/cdd/compound/exmod_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/compound/gen.py` & `python-cdd-0.0.99rc6/cdd/compound/gen.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/compound/gen_utils.py` & `python-cdd-0.0.99rc6/cdd/compound/gen_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/compound/openapi/emit.py` & `python-cdd-0.0.99rc6/cdd/compound/openapi/emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/compound/openapi/gen_openapi.py` & `python-cdd-0.0.99rc6/cdd/compound/openapi/gen_openapi.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/compound/openapi/gen_routes.py` & `python-cdd-0.0.99rc6/cdd/compound/openapi/gen_routes.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/compound/openapi/parse.py` & `python-cdd-0.0.99rc6/cdd/compound/openapi/parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/compound/openapi/utils/emit_openapi_utils.py` & `python-cdd-0.0.99rc6/cdd/compound/openapi/utils/emit_openapi_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/compound/openapi/utils/emit_utils.py` & `python-cdd-0.0.99rc6/cdd/compound/openapi/utils/emit_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/compound/openapi/utils/parse_utils.py` & `python-cdd-0.0.99rc6/cdd/compound/openapi/utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/compound/sync_properties.py` & `python-cdd-0.0.99rc6/cdd/compound/sync_properties.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/docstring/emit.py` & `python-cdd-0.0.99rc6/cdd/docstring/emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/docstring/parse.py` & `python-cdd-0.0.99rc6/cdd/docstring/parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/docstring/utils/emit_utils.py` & `python-cdd-0.0.99rc6/cdd/docstring/utils/emit_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/function/emit.py` & `python-cdd-0.0.99rc6/cdd/function/emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/function/parse.py` & `python-cdd-0.0.99rc6/cdd/function/parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/function/utils/emit_utils.py` & `python-cdd-0.0.99rc6/cdd/function/utils/emit_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/function/utils/parse_utils.py` & `python-cdd-0.0.99rc6/cdd/function/utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/json_schema/emit.py` & `python-cdd-0.0.99rc6/cdd/json_schema/emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/json_schema/parse.py` & `python-cdd-0.0.99rc6/cdd/json_schema/parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/json_schema/utils/emit_utils.py` & `python-cdd-0.0.99rc6/cdd/json_schema/utils/emit_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/json_schema/utils/parse_utils.py` & `python-cdd-0.0.99rc6/cdd/json_schema/utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/routes/emit/bottle.py` & `python-cdd-0.0.99rc6/cdd/routes/emit/bottle.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/routes/emit/bottle_constants_utils.py` & `python-cdd-0.0.99rc6/cdd/routes/emit/bottle_constants_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/routes/parse/bottle.py` & `python-cdd-0.0.99rc6/cdd/routes/parse/bottle.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/routes/parse/bottle_utils.py` & `python-cdd-0.0.99rc6/cdd/routes/parse/bottle_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/routes/parse/fastapi.py` & `python-cdd-0.0.99rc6/cdd/routes/parse/fastapi.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/routes/parse/fastapi_utils.py` & `python-cdd-0.0.99rc6/cdd/routes/parse/fastapi_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/ast_cst_utils.py` & `python-cdd-0.0.99rc6/cdd/shared/ast_cst_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/ast_utils.py` & `python-cdd-0.0.99rc6/cdd/shared/ast_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/conformance.py` & `python-cdd-0.0.99rc6/cdd/shared/conformance.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/cst.py` & `python-cdd-0.0.99rc6/cdd/shared/cst.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/cst_utils.py` & `python-cdd-0.0.99rc6/cdd/shared/cst_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/defaults_utils.py` & `python-cdd-0.0.99rc6/cdd/shared/defaults_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/docstring_parsers.py` & `python-cdd-0.0.99rc6/cdd/shared/docstring_parsers.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/docstring_utils.py` & `python-cdd-0.0.99rc6/cdd/shared/docstring_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/emit/__init__.py` & `python-cdd-0.0.99rc6/cdd/shared/emit/__init__.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/emit/file.py` & `python-cdd-0.0.99rc6/cdd/shared/emit/file.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/emit/utils/emitter_utils.py` & `python-cdd-0.0.99rc6/cdd/shared/emit/utils/emitter_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/parse/__init__.py` & `python-cdd-0.0.99rc6/cdd/shared/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/parse/utils/parser_utils.py` & `python-cdd-0.0.99rc6/cdd/shared/parse/utils/parser_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/pkg_utils.py` & `python-cdd-0.0.99rc6/cdd/shared/pkg_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/pure_utils.py` & `python-cdd-0.0.99rc6/cdd/shared/pure_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/shared/source_transformer.py` & `python-cdd-0.0.99rc6/cdd/shared/source_transformer.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/sqlalchemy/emit.py` & `python-cdd-0.0.99rc6/cdd/sqlalchemy/emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/sqlalchemy/parse.py` & `python-cdd-0.0.99rc6/cdd/sqlalchemy/parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/sqlalchemy/utils/parse_utils.py` & `python-cdd-0.0.99rc6/cdd/sqlalchemy/utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/sqlalchemy/utils/shared_utils.py` & `python-cdd-0.0.99rc6/cdd/sqlalchemy/utils/shared_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/__init__.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/argparse.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/argparse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/classes.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/classes.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/cst.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/cst.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/cstify.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/cstify.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/docstrings.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/docstrings.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/doctrans.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/doctrans.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/exmod.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/exmod.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/fastapi_routes.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/fastapi_routes.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/gen.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/gen.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/ir.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/ir.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/json_schema.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/json_schema.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/methods.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/methods.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/openapi.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/openapi.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/pydantic.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/pydantic.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/routes.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/routes.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/mocks/sqlalchemy.py` & `python-cdd-0.0.99rc6/cdd/tests/mocks/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_argparse_function/test_emit_argparse.py` & `python-cdd-0.0.99rc6/cdd/tests/test_argparse_function/test_emit_argparse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_argparse_function/test_parse_argparse.py` & `python-cdd-0.0.99rc6/cdd/tests/test_argparse_function/test_parse_argparse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_ast_equality.py` & `python-cdd-0.0.99rc6/cdd/tests/test_ast_equality.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_class/test_emit_class_.py` & `python-cdd-0.0.99rc6/cdd/tests/test_class/test_emit_class_.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_class/test_parse_class.py` & `python-cdd-0.0.99rc6/cdd/tests/test_class/test_parse_class.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli.py` & `python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_doctrans.py` & `python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli_doctrans.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_exmod.py` & `python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli_exmod.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_gen.py` & `python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli_gen.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_gen_routes.py` & `python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli_gen_routes.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_openapi.py` & `python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli_openapi.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_sync.py` & `python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_sync_properties.py` & `python-cdd-0.0.99rc6/cdd/tests/test_cli/test_cli_sync_properties.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_doctrans.py` & `python-cdd-0.0.99rc6/cdd/tests/test_compound/test_doctrans.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_doctrans_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_compound/test_doctrans_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_exmod.py` & `python-cdd-0.0.99rc6/cdd/tests/test_compound/test_exmod.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,37 @@
         )
         cls.module_hierarchy = (
             (cls.parent_name, cls.parent_dir),
             (cls.child_name, cls.child_dir),
             (cls.grandchild_name, cls.grandchild_dir),
         )
 
+    @staticmethod
+    def normalise_double_paths(*dictionaries):
+        """
+        On Windows the paths can come up weird, like C:\\\\foo instead of C:\\foo
+
+        This fixes that issue, and also safe to work on non-Windows
+
+        :param dictionaries: Dictionaries
+        :type dictionaries: ```Tuple[dictionaries]```
+
+        :return: `map` of normalised `dictionaries`
+        :rtype: ```map```
+        """
+        return map(
+            lambda d: {
+                k: tuple(
+                    map(repr, map(rpartial(str.replace, path.sep * 2, path.sep), v))
+                )
+                for k, v in d.items()
+            },
+            dictionaries,
+        )
+
     def test_exmod(self) -> None:
         """Tests `exmod`"""
 
         try:
             with TemporaryDirectory(prefix="search_root", suffix="search_path") as root:
                 _, new_module_dir = self.create_and_install_pkg(root)
 
@@ -89,15 +112,18 @@
                     mock_imports=True,
                     output_directory=new_module_dir,
                     target_module_name=None,
                     no_word_wrap=None,
                     dry_run=False,
                 )
                 self.assertListEqual(
-                    listdir(new_module_dir), [INIT_FILENAME, self.parent_dir]
+                    *map(
+                        sorted,
+                        (listdir(new_module_dir), [INIT_FILENAME, self.parent_dir]),
+                    ),
                 )
         finally:
             self._pip(["uninstall", "-y", self.package_root_name])
 
     def test_exmod_whitelist(self) -> None:
         """Tests `exmod` whitelist"""
 
@@ -284,16 +310,15 @@
                         )
                         for k, v in {
                             "mkdir": ("", *map(itemgetter(1), self.module_hierarchy)),
                             "write": (INIT_FILENAME,),
                         }.items()
                     },
                 )
-                self.maxDiff = None
-                self.assertDictEqual(result, gold)
+                self.assertDictEqual(*self.normalise_double_paths(result, gold))
 
                 self._check_emission(new_module_dir, dry_run=True)
         finally:
             self._pip(["uninstall", "-y", self.package_root_name])
 
     def create_and_install_pkg(self, root):
         """
@@ -328,14 +353,15 @@
                                             "*",
                                             None,
                                             identifier=None,
                                             identifier_name=None,
                                         )
                                     ],
                                     level=0,
+                                    identifier=None,
                                 ),
                                 Assign(
                                     targets=[Name("__author__", Store())],
                                     value=set_value(
                                         environ.get("CDD_AUTHOR", "Samuel Marks")
                                     ),
                                     expr=None,
@@ -440,14 +466,15 @@
                                         name,
                                         None,
                                         identifier=None,
                                         identifier_name=None,
                                     )
                                 ],
                                 level=0,
+                                identifier=None,
                             )
                             for name, directory in self.module_hierarchy
                         ),
                         (
                             Assign(
                                 targets=[Name("__all__", Store())],
                                 value=List(
```

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_exmod_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_compound/test_exmod_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_gen.py` & `python-cdd-0.0.99rc6/cdd/tests/test_compound/test_gen.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_gen_routes.py` & `python-cdd-0.0.99rc6/cdd/tests/test_compound/test_gen_routes.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_gen_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_compound/test_gen_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_openapi_bulk.py` & `python-cdd-0.0.99rc6/cdd/tests/test_compound/test_openapi_bulk.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_openapi_sub.py` & `python-cdd-0.0.99rc6/cdd/tests/test_compound/test_openapi_sub.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_sync_properties.py` & `python-cdd-0.0.99rc6/cdd/tests/test_compound/test_sync_properties.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_docstring/test_emit_docstring.py` & `python-cdd-0.0.99rc6/cdd/tests/test_docstring/test_emit_docstring.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_docstring/test_parse_docstring.py` & `python-cdd-0.0.99rc6/cdd/tests/test_docstring/test_parse_docstring.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_emit/test_emit_file.py` & `python-cdd-0.0.99rc6/cdd/tests/test_emit/test_emit_file.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_emit/test_emitter_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_emit/test_emitter_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_emit/test_emitters.py` & `python-cdd-0.0.99rc6/cdd/tests/test_emit/test_emitters.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_function/test_emit_function.py` & `python-cdd-0.0.99rc6/cdd/tests/test_function/test_emit_function.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_function/test_parse_function.py` & `python-cdd-0.0.99rc6/cdd/tests/test_function/test_parse_function.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_emit_json_schema.py` & `python-cdd-0.0.99rc6/cdd/tests/test_json_schema/test_emit_json_schema.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_emit_json_schema_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_json_schema/test_emit_json_schema_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_parse_json_schema.py` & `python-cdd-0.0.99rc6/cdd/tests/test_json_schema/test_parse_json_schema.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_parse_json_schema_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_json_schema/test_parse_json_schema_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_marshall_docstring.py` & `python-cdd-0.0.99rc6/cdd/tests/test_marshall_docstring.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_parse/test_parser_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_parse/test_parser_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_parse/test_parsers.py` & `python-cdd-0.0.99rc6/cdd/tests/test_parse/test_parsers.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_pydantic/test_emit_pydantic.py` & `python-cdd-0.0.99rc6/cdd/tests/test_pydantic/test_emit_pydantic.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_pydantic/test_parse_pydantic.py` & `python-cdd-0.0.99rc6/cdd/tests/test_pydantic/test_parse_pydantic.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_routes/test_bottle_route_emit.py` & `python-cdd-0.0.99rc6/cdd/tests/test_routes/test_bottle_route_emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_routes/test_bottle_route_parse.py` & `python-cdd-0.0.99rc6/cdd/tests/test_routes/test_bottle_route_parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_routes/test_fastapi_routes_parse.py` & `python-cdd-0.0.99rc6/cdd/tests/test_routes/test_fastapi_routes_parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_routes/test_route_emit.py` & `python-cdd-0.0.99rc6/cdd/tests/test_routes/test_route_emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_routes/test_route_parse.py` & `python-cdd-0.0.99rc6/cdd/tests/test_routes/test_route_parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_setup.py` & `python-cdd-0.0.99rc6/cdd/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_ast_cst_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_shared/test_ast_cst_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_ast_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_shared/test_ast_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_conformance.py` & `python-cdd-0.0.99rc6/cdd/tests/test_shared/test_conformance.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_cst.py` & `python-cdd-0.0.99rc6/cdd/tests/test_shared/test_cst.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_cst_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_shared/test_cst_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_default_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_shared/test_default_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_docstring_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_shared/test_docstring_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_pure_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_shared/test_pure_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_source_transformer.py` & `python-cdd-0.0.99rc6/cdd/tests/test_shared/test_source_transformer.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy.py` & `python-cdd-0.0.99rc6/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy.py` & `python-cdd-0.0.99rc6/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy_utils.py` & `python-cdd-0.0.99rc6/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/test_utils_for_tests.py` & `python-cdd-0.0.99rc6/cdd/tests/test_utils_for_tests.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/cdd/tests/utils_for_tests.py` & `python-cdd-0.0.99rc6/cdd/tests/utils_for_tests.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/python_cdd.egg-info/PKG-INFO` & `python-cdd-0.0.99rc6/python_cdd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cdd
-Version: 0.0.99rc5
+Version: 0.0.99rc6
 Summary: Open API to/fro routes, models, and tests. Convert between docstrings, classes, methods, argparse, pydantic, and SQLalchemy.
 Home-page: https://github.com/offscale/cdd-python
 Author: Samuel Marks
 Author-email: 807580+SamuelMarks@users.noreply.github.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `python-cdd-0.0.99rc5/python_cdd.egg-info/SOURCES.txt` & `python-cdd-0.0.99rc6/python_cdd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc5/setup.py` & `python-cdd-0.0.99rc6/setup.py`

 * *Files identical despite different names*

