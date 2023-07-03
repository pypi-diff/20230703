# Comparing `tmp/mindflow-0.5.3.tar.gz` & `tmp/mindflow-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindflow-0.5.3.tar", last modified: Sat Jun 24 21:52:29 2023, max compression
+gzip compressed data, was "mindflow-0.5.4.tar", last modified: Mon Jul  3 02:53:02 2023, max compression
```

## Comparing `mindflow-0.5.3.tar` & `mindflow-0.5.4.tar`

### file list

```diff
@@ -1,104 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.295261 mindflow-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-24 21:52:14.000000 mindflow-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-24 21:52:14.000000 mindflow-0.5.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 21:52:14.000000 mindflow-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-24 21:52:14.000000 mindflow-0.5.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-24 21:52:29.295261 mindflow-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-06-24 21:52:14.000000 mindflow-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-24 21:52:14.000000 mindflow-0.5.3/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.287261 mindflow-0.5.3/mindflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.287261 mindflow-0.5.3/mindflow/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.287261 mindflow-0.5.3/mindflow/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/cli/commands/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/git/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/git/mr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/git/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/git/push.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/command_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/core/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/core/commands/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/git/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/execute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/core/file_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/file_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/file_processing/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/file_processing/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/prompt_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/core/resolving/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/resolving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/resolving/resolve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/core/resolving/resolvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/resolving/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/resolving/resolvers/document_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/resolving/resolvers/file_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/core/text_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/text_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/text_processing/utf8.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/text_processing/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/token_counting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.295261 mindflow-0.5.3/mindflow/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.295261 mindflow-0.5.3/mindflow/core/types/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/definitions/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/definitions/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/definitions/mind_flow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/definitions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/definitions/model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/definitions/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/mindflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16802 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.295261 mindflow-0.5.3/mindflow/core/types/store_traits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/store_traits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/store_traits/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/store_traits/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/store_traits/static.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.295261 mindflow-0.5.3/mindflow/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/unit_tests/dummy_diff.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/unit_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/unit_tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.287261 mindflow-0.5.3/mindflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-24 21:52:29.000000 mindflow-0.5.3/mindflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-24 21:52:29.000000 mindflow-0.5.3/mindflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:52:29.000000 mindflow-0.5.3/mindflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-24 21:52:29.000000 mindflow-0.5.3/mindflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-24 21:52:29.000000 mindflow-0.5.3/mindflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 21:52:29.000000 mindflow-0.5.3/mindflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-24 21:52:14.000000 mindflow-0.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 21:52:29.295261 mindflow-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-24 21:52:14.000000 mindflow-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.105474 mindflow-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-03 02:52:51.000000 mindflow-0.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-03 02:52:51.000000 mindflow-0.5.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 02:52:51.000000 mindflow-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-03 02:52:51.000000 mindflow-0.5.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-07-03 02:53:02.105474 mindflow-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-03 02:52:51.000000 mindflow-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-03 02:52:51.000000 mindflow-0.5.4/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.089473 mindflow-0.5.4/mindflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.093473 mindflow-0.5.4/mindflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.093473 mindflow-0.5.4/mindflow/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.097473 mindflow-0.5.4/mindflow/cli/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/git/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/git/mr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/git/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/git/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/cli/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.097473 mindflow-0.5.4/mindflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.097473 mindflow-0.5.4/mindflow/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/commands/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.097473 mindflow-0.5.4/mindflow/core/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/commands/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/commands/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/commands/git/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/commands/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.097473 mindflow-0.5.4/mindflow/core/file_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/file_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/file_processing/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/file_processing/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/prompt_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.101474 mindflow-0.5.4/mindflow/core/resolving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/resolving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/resolving/resolve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.101474 mindflow-0.5.4/mindflow/core/resolving/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/resolving/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/resolving/resolvers/document_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/resolving/resolvers/file_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.101474 mindflow-0.5.4/mindflow/core/text_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/text_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/text_processing/utf8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/text_processing/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/token_counting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.101474 mindflow-0.5.4/mindflow/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.101474 mindflow-0.5.4/mindflow/core/types/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/definitions/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/definitions/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/definitions/mind_flow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/definitions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/definitions/model_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/definitions/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/mindflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18846 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.101474 mindflow-0.5.4/mindflow/core/types/store_traits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/store_traits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/store_traits/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/store_traits/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/core/types/store_traits/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.101474 mindflow-0.5.4/mindflow/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/unit_tests/dummy_diff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/unit_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-07-03 02:52:51.000000 mindflow-0.5.4/mindflow/unit_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:53:02.089473 mindflow-0.5.4/mindflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-07-03 02:53:02.000000 mindflow-0.5.4/mindflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-03 02:53:02.000000 mindflow-0.5.4/mindflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 02:53:02.000000 mindflow-0.5.4/mindflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-03 02:53:02.000000 mindflow-0.5.4/mindflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-03 02:53:02.000000 mindflow-0.5.4/mindflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 02:53:02.000000 mindflow-0.5.4/mindflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-03 02:52:51.000000 mindflow-0.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 02:53:02.105474 mindflow-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-03 02:52:51.000000 mindflow-0.5.4/setup.py
```

### Comparing `mindflow-0.5.3/.gitignore` & `mindflow-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.3/Makefile` & `mindflow-0.5.4/Makefile`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.3/PKG-INFO` & `mindflow-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindflow
-Version: 0.5.3
+Version: 0.5.4
 Summary: AI-powered search engine for your code!
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # :brain: mindflow :ocean:
 The [ChatGPT](https://openai.com/blog/chatgpt)-powered swiss army knife for the modern developer! We provide an AI-powered CLI git wrapper, boilerplate code generator, code search engine, a conversation history manager, and much more!
 
@@ -23,20 +23,20 @@
 1. Follow us on [Twitter](https://twitter.com/mindflow_ai)
 2. Join our [discord](https://discord.com/invite/P2cQACzB)
 3. BONUS: Consider [becoming a patron](https://www.patreon.com/MindFlowAI) :heart:
 
 ## Getting Started
 
 Pre-requisite: 
-- You'll need to create an [OpenAI](https://openai.com/blog/openai-api) account or request early access from [Anthropic](https://www.anthropic.com/earlyaccess).
+- You'll need to create an [OpenAI](https://openai.com/blog/openai-api) account.
 - Also, create a [Pinecone](https://www.pinecone.io/start) account to use their vector database.
 
 1. Run `pip install mindflow`, or you can clone this repo and run `pip install -e path/to/mindflow`.
 2. Run `mf login`:
-    - Register with OpenAI or Anthropic to use their models. You can find your OpenAI API key [here](https://platform.openai.com/account/api-keys).
+    - Register with OpenAI to use their models. You can find your OpenAI API key [here](https://platform.openai.com/account/api-keys).
     - Register with Pinecone to use their vector database. You can find your Pinecone API key and Environment [here](https://www.pinecone.io/start).
 3. Now, you're ready to start using MindFlow!
 
 ## Basic Usage
 
 ### Configuration (Optional)
 Configure the model used for generating responses by running `mf config` and selecting either GPT 3.5 Turbo (default) or GPT 4. In order to use GPT 4, you'll need to have special access to the API. If you have access, you can run `mf config` and select GPT 4. If you don't have access, you'll get an error message. 
@@ -45,22 +45,22 @@
 ### Chats
 There are multiple levels to using mindflow's chat feature.
 
 1. Simplest
 - `mf chat "explain what a programming language is"`
     - Interact with chatGPT directly just like on the chatGPT website. We also have chat persistence, so it will remember the previous chat messages.
 2. With File Context
-- `mf chat "please summarize what this code does" path/to/code.py`
+- `mf chat path/to/code.py "please summarize what this code does"`
     - You can provide single or multi-file context to chatGPT by passing in any number of files as a separate argument in the `mf chat` call. For sufficiently small files (see: [chatGPT token limits](https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them)), this will work and also maintain chat history.
 3. With Directory Context
-- `mf chat "what are these submodules responsible for? path/to/submodule1/ path/to/submodule2/`
+- `mf chat path/to/submodule1/ path/to/submodule2/ "what are these submodules responsible for?"`
     - Providing directories will actually run an indexer over your code subdirectories/files recursively. So it may take a while to fully index everything -- don't worry; we'll warn you if the cost becomes a concern! Right now the warning triggers if the index job costs >$0.50USD.
 4. Custom pre-indexed context
 - `mf index path/to/subdir/file1.txt path/to/file2.txt`
-- `mf chat -s "How do all of my classes relate to one another?" ./`
+- `mf chat -s ./ "How do all of my classes relate to one another?"`
     - If you pre-index your repository, you can narrow the scope for the context provided to the chat. Passing `-s` will skip the auto-indexing, and instead will defer to the currently existing index. This index is generated in the first step `mf index` where only those files/subdirs will be included.
     - This can save you time and money if your repository is significantly large.
 
 ### Code Generator
 You can use mindflow to generate boilerplate code in an instant using `mf gen`! It should only generate code and comments, and will save the file in the path given.
 
 Here's a couple examples:
@@ -121,11 +121,11 @@
 ### Generating a setup.py
 ![Screenshot 2023-03-11 at 8 39 47 PM](https://user-images.githubusercontent.com/26421036/224524762-e80f134b-5fc6-4f9f-af4e-d858549ccff8.png)
 
 ### Generating an arbitrary program file
 ![Screenshot 2023-03-11 at 8 42 11 PM](https://user-images.githubusercontent.com/26421036/224524839-45093b5d-b4d9-4dc4-a129-867d819a2136.png)
 
 ## How does it work?
-This tool allows you to build an index of text documents and search through them using GPT-based embeddings. The tool takes document paths as input, extracts the text, splits the documents into chunks, summarizes them, and builds a summarization tree. The tool then uses this tree to generate embeddings of the indexed documents and your query and selects the top text chunks based on the cosine similarity between these embeddings. The generated index can be saved to a JSON file for later reuse, making subsequent searches faster and cheaper.
+MindFlow uses state-of-the-art methods for high-throughput segmentation, processing, storage, and retrieval of documents using a recursive hierarchical summarization and embedding technique to store embedding vectors for document chunks and then achieve fast, and high-quality responses to questions and tasks by appending similar document chunks based on the hierarchically embedded text and using them as context for you query. Additionally, chat history will persist if it can fit in the context for queries over indexed documents or for regular chat.
 
 ## What's next for MindFlow
 In the future, MindFlow plans on becoming an even more integral part of the modern developer's toolkit. We plan on adding the ability to ditch traditional documentation and instead integrate directly with your private documents and communication channels, allowing for a more seamless and intuitive experience. With MindFlow, you can have a true "stream of consciousness" with your code, documentation, and communication channels, making it easier than ever to stay on top of your projects and collaborate with your team. We are excited to continue pushing the boundaries of what's possible with language models and revolutionizing how developers work.
```

### Comparing `mindflow-0.5.3/README.md` & `mindflow-0.5.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 1. Follow us on [Twitter](https://twitter.com/mindflow_ai)
 2. Join our [discord](https://discord.com/invite/P2cQACzB)
 3. BONUS: Consider [becoming a patron](https://www.patreon.com/MindFlowAI) :heart:
 
 ## Getting Started
 
 Pre-requisite: 
-- You'll need to create an [OpenAI](https://openai.com/blog/openai-api) account or request early access from [Anthropic](https://www.anthropic.com/earlyaccess).
+- You'll need to create an [OpenAI](https://openai.com/blog/openai-api) account.
 - Also, create a [Pinecone](https://www.pinecone.io/start) account to use their vector database.
 
 1. Run `pip install mindflow`, or you can clone this repo and run `pip install -e path/to/mindflow`.
 2. Run `mf login`:
-    - Register with OpenAI or Anthropic to use their models. You can find your OpenAI API key [here](https://platform.openai.com/account/api-keys).
+    - Register with OpenAI to use their models. You can find your OpenAI API key [here](https://platform.openai.com/account/api-keys).
     - Register with Pinecone to use their vector database. You can find your Pinecone API key and Environment [here](https://www.pinecone.io/start).
 3. Now, you're ready to start using MindFlow!
 
 ## Basic Usage
 
 ### Configuration (Optional)
 Configure the model used for generating responses by running `mf config` and selecting either GPT 3.5 Turbo (default) or GPT 4. In order to use GPT 4, you'll need to have special access to the API. If you have access, you can run `mf config` and select GPT 4. If you don't have access, you'll get an error message. 
@@ -38,22 +38,22 @@
 ### Chats
 There are multiple levels to using mindflow's chat feature.
 
 1. Simplest
 - `mf chat "explain what a programming language is"`
     - Interact with chatGPT directly just like on the chatGPT website. We also have chat persistence, so it will remember the previous chat messages.
 2. With File Context
-- `mf chat "please summarize what this code does" path/to/code.py`
+- `mf chat path/to/code.py "please summarize what this code does"`
     - You can provide single or multi-file context to chatGPT by passing in any number of files as a separate argument in the `mf chat` call. For sufficiently small files (see: [chatGPT token limits](https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them)), this will work and also maintain chat history.
 3. With Directory Context
-- `mf chat "what are these submodules responsible for? path/to/submodule1/ path/to/submodule2/`
+- `mf chat path/to/submodule1/ path/to/submodule2/ "what are these submodules responsible for?"`
     - Providing directories will actually run an indexer over your code subdirectories/files recursively. So it may take a while to fully index everything -- don't worry; we'll warn you if the cost becomes a concern! Right now the warning triggers if the index job costs >$0.50USD.
 4. Custom pre-indexed context
 - `mf index path/to/subdir/file1.txt path/to/file2.txt`
-- `mf chat -s "How do all of my classes relate to one another?" ./`
+- `mf chat -s ./ "How do all of my classes relate to one another?"`
     - If you pre-index your repository, you can narrow the scope for the context provided to the chat. Passing `-s` will skip the auto-indexing, and instead will defer to the currently existing index. This index is generated in the first step `mf index` where only those files/subdirs will be included.
     - This can save you time and money if your repository is significantly large.
 
 ### Code Generator
 You can use mindflow to generate boilerplate code in an instant using `mf gen`! It should only generate code and comments, and will save the file in the path given.
 
 Here's a couple examples:
@@ -114,11 +114,11 @@
 ### Generating a setup.py
 ![Screenshot 2023-03-11 at 8 39 47 PM](https://user-images.githubusercontent.com/26421036/224524762-e80f134b-5fc6-4f9f-af4e-d858549ccff8.png)
 
 ### Generating an arbitrary program file
 ![Screenshot 2023-03-11 at 8 42 11 PM](https://user-images.githubusercontent.com/26421036/224524839-45093b5d-b4d9-4dc4-a129-867d819a2136.png)
 
 ## How does it work?
-This tool allows you to build an index of text documents and search through them using GPT-based embeddings. The tool takes document paths as input, extracts the text, splits the documents into chunks, summarizes them, and builds a summarization tree. The tool then uses this tree to generate embeddings of the indexed documents and your query and selects the top text chunks based on the cosine similarity between these embeddings. The generated index can be saved to a JSON file for later reuse, making subsequent searches faster and cheaper.
+MindFlow uses state-of-the-art methods for high-throughput segmentation, processing, storage, and retrieval of documents using a recursive hierarchical summarization and embedding technique to store embedding vectors for document chunks and then achieve fast, and high-quality responses to questions and tasks by appending similar document chunks based on the hierarchically embedded text and using them as context for you query. Additionally, chat history will persist if it can fit in the context for queries over indexed documents or for regular chat.
 
 ## What's next for MindFlow
 In the future, MindFlow plans on becoming an even more integral part of the modern developer's toolkit. We plan on adding the ability to ditch traditional documentation and instead integrate directly with your private documents and communication channels, allowing for a more seamless and intuitive experience. With MindFlow, you can have a true "stream of consciousness" with your code, documentation, and communication channels, making it easier than ever to stay on top of your projects and collaborate with your team. We are excited to continue pushing the boundaries of what's possible with language models and revolutionizing how developers work.
```

### Comparing `mindflow-0.5.3/mindflow/cli/cli_main.py` & `mindflow-0.5.4/mindflow/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.3/mindflow/cli/commands/chat.py` & `mindflow-0.5.4/mindflow/cli/commands/chat.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,14 @@
-import asyncio
 import click
 from typing import Tuple
-import os
-
-from result import Result
-
-from mindflow.core.commands.chat import run_chat
-from mindflow.core.commands.index import run_index
-from mindflow.core.commands.query import run_query
-from mindflow.core.settings import Settings
-from mindflow.core.types.model import ModelApiCallError
-from mindflow.core.types.store_traits.json import save_json_store
-from mindflow.core.types.conversation import Conversation
-from mindflow.core.types.definitions.conversation import ConversationID
 
 
 def parse_chat_prompt_and_paths_from_args(prompt_args: Tuple[str]):
+    import os
+
     prompt = " ".join(prompt_args)  # include files/directories in prompt
     paths = []
 
     for arg in prompt_args:
         if os.path.exists(arg):
             paths.append(arg)
 
@@ -28,59 +17,88 @@
 
 @click.command(
     help='Interact with ChatGPT, you can reference files and directories by passing them as arguments. Example: `mf chat "Please summarize this file" path/to/file.txt`'
 )
 @click.option("-s", "--skip-index", type=bool, default=False, is_flag=True)
 @click.argument("prompt_args", nargs=-1, type=str, required=True)
 def chat(prompt_args: Tuple[str], skip_index: bool):
+    import click
+    import asyncio
+
+    from typing import List
+    from result import Ok
+
+    from mindflow.core.commands.chat import run_chat
+    from mindflow.core.commands.index import run_index
+    from mindflow.core.commands.query import run_query
+    from mindflow.core.settings import Settings
+    from mindflow.core.types.store_traits.json import save_json_store
+
+    async def stream_chat(settings: Settings, prompt: str):
+        print("\nGPT:")
+        async for char_stream_chunk in run_chat(settings, [], prompt):
+            if isinstance(char_stream_chunk, Ok):
+                click.echo(char_stream_chunk.value, nl=False)
+            else:
+                click.echo(char_stream_chunk.value)
+
+    async def stream_query(settings: Settings, file_paths: List[str], prompt: str):
+        print("\nGPT:")
+        async for char_stream_chunk in run_query(settings, file_paths, prompt):
+            if isinstance(char_stream_chunk, Ok):
+                click.echo(char_stream_chunk.value, nl=False)
+            else:
+                click.echo(char_stream_chunk.value)
+
     prompt, paths = parse_chat_prompt_and_paths_from_args(prompt_args)
     settings = Settings()
     if paths:
         if skip_index:
             click.echo(
                 "Skipping indexing step, only using the current index for context. You can run `mf index` to pre-index specific paths."
             )
         else:
             click.echo(
                 "Indexing paths... Note: this may take a while, if you want to skip this step, use the `--skip-index` flag. If you do so, you can pre-select specific paths to index with `mf index`.\n"
             )
 
             asyncio.run(run_index(settings, paths))
 
-        run_query_result: Result[str, ModelApiCallError] = asyncio.run(
-            run_query(settings, paths, prompt)
-        )
-        click.echo(run_query_result.value)
+        asyncio.run(stream_query(settings, paths, prompt))
 
         save_json_store()
         return
 
-    run_chat_result: Result[str, ModelApiCallError] = asyncio.run(
-        run_chat(settings, [], prompt)
-    )
-    click.echo(run_chat_result.value)
+    asyncio.run(stream_chat(settings, prompt))
+
     save_json_store()
 
 
 @click.group(help="Manage conversation histories.")
 def history():
     pass
 
 
 @history.command(help="View chat history stats.")
 def stats():
+    from mindflow.core.types.conversation import Conversation
+    from mindflow.core.types.definitions.conversation import ConversationID
+
     if (conversation := Conversation.load(ConversationID.CHAT_0.value)) is None:
         print("No conversation history found.")
         return
 
     print("Num messages:", len(conversation.messages))
     print("Total tokens:", conversation.total_tokens)
 
 
 @history.command(help="Clear the chat history.")
 def clear():
+    from mindflow.core.types.conversation import Conversation
+    from mindflow.core.types.definitions.conversation import ConversationID
+
     if (conversation := Conversation.load(ConversationID.CHAT_0.value)) is None:
         print("No conversation history found.")
         return
 
     conversation.messages = []
     conversation.save()
```

### Comparing `mindflow-0.5.3/mindflow/cli/commands/config.py` & `mindflow-0.5.4/mindflow/cli/commands/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,143 +1,129 @@
-import sys
-from typing import List
 import click
-from mindflow.core.types.store_traits.json import save_json_store
-from mindflow.core.types.mindflow_model import (
-    MindFlowModel,
-    MindFlowModelConfig,
-    MindFlowModelID,
-)
-
-from mindflow.core.types.definitions.model import (
-    ModelID,
-)
-from mindflow.core.types.model import Model
+from typing import List
 
 
 @click.command(
     help="Configure MindFlow. For example, you can configure the model to use."
 )
 def config():
+    from mindflow.core.types.store_traits.json import save_json_store
+    from mindflow.core.types.mindflow_model import (
+        MindFlowModel,
+        MindFlowModelConfig,
+        MindFlowModelID,
+    )
+
+    from mindflow.core.types.definitions.model import (
+        ModelID,
+    )
+    from mindflow.core.types.model import Model
+
+    def configure_model():
+        mindflow_model_ids = [
+            MindFlowModelID.QUERY.value,
+            MindFlowModelID.INDEX.value,
+            MindFlowModelID.EMBEDDING.value,
+        ]
+        mindflow_model_options: List[MindFlowModel] = [
+            MindFlowModel.load(mindflow_model_id)
+            for mindflow_model_id in mindflow_model_ids
+        ]
+        mindflow_model_descriptions: List[str] = [
+            mindflow_model.name for mindflow_model in mindflow_model_options
+        ]
+
+        selected_mindflow_model: MindFlowModel = select_option(
+            "Select MindFlow model. Enter #",
+            mindflow_model_options,
+            mindflow_model_descriptions,
+        )
+        if selected_mindflow_model.id == MindFlowModelID.QUERY.value:
+            configure_query_model()
+        elif selected_mindflow_model.id == MindFlowModelID.INDEX.value:
+            configure_index_model()
+        elif selected_mindflow_model.id == MindFlowModelID.EMBEDDING.value:
+            configure_embedding_model()
+
+    def configure_query_model():
+        model_ids = [
+            ModelID.GPT_3_5_TURBO.value,
+            ModelID.GPT_4.value,
+        ]
+        model_options: List[Model] = [Model.load(model_id) for model_id in model_ids]
+        model_descriptions: List[str] = [
+            model.config_description for model in model_options
+        ]
+
+        selected_model: Model = select_option(
+            "Select chat model. Recommended GPT-4/Claude V1. Enter #",
+            model_options,
+            model_descriptions,
+        )
+        mindflow_model_config: MindFlowModelConfig = MindFlowModelConfig.load(
+            f"{MindFlowModelID.QUERY.value}_config"
+        ) or MindFlowModelConfig(f"{MindFlowModelID.QUERY.value}_config")
+        mindflow_model_config.model = selected_model.id
+        mindflow_model_config.save()
+
+        print(f"Query Model: {selected_model.id} saved!")
+
+    def configure_index_model():
+        model_ids = [
+            ModelID.GPT_3_5_TURBO.value,
+            ModelID.GPT_4.value,
+        ]
+        model_options: List[Model] = [Model.load(model_id) for model_id in model_ids]
+        model_descriptions: List[str] = [
+            model.config_description for model in model_options
+        ]
+
+        selected_model: Model = select_option(
+            "Select chat model. Recommended GPT-3.5 Turbo/Claude Instant V1. Enter #",
+            model_options,
+            model_descriptions,
+        )
+        mindflow_model_config: MindFlowModelConfig = MindFlowModelConfig.load(
+            f"{MindFlowModelID.INDEX.value}_config"
+        ) or MindFlowModelConfig(f"{MindFlowModelID.INDEX.value}_config")
+        mindflow_model_config.model = selected_model.id
+        mindflow_model_config.save()
+
+        print(f"Index Model: {selected_model.id} saved!")
+
+    def configure_embedding_model():
+        model_ids = [ModelID.TEXT_EMBEDDING_ADA_002.value]
+        model_options: List[Model] = [Model.load(model_id) for model_id in model_ids]
+        model_descriptions: List[str] = [
+            model.config_description for model in model_options
+        ]
+
+        selected_model: Model = select_option(
+            "Select chat model. Only one option... for now :) Enter #",
+            model_options,
+            model_descriptions,
+        )
+        mindflow_model_config: MindFlowModelConfig = MindFlowModelConfig.load(
+            f"{MindFlowModelID.EMBEDDING.value}_config"
+        ) or MindFlowModelConfig(f"{MindFlowModelID.EMBEDDING.value}_config")
+        mindflow_model_config.model = selected_model.id
+        mindflow_model_config.save()
+
+        print(f"Embedding Model: {selected_model.id} saved!")
+
     config_options = ["model"]
     selected_config = select_option(
         "What do you want to configure? Enter #", config_options, config_options
     )
     if selected_config == "model":
         configure_model()
 
     save_json_store()
 
 
-def configure_model():
-    mindflow_model_ids = [
-        MindFlowModelID.QUERY.value,
-        MindFlowModelID.INDEX.value,
-        MindFlowModelID.EMBEDDING.value,
-    ]
-    mindflow_model_options: List[MindFlowModel] = [
-        MindFlowModel.load(mindflow_model_id)
-        for mindflow_model_id in mindflow_model_ids
-    ]
-    mindflow_model_descriptions: List[str] = [
-        mindflow_model.name for mindflow_model in mindflow_model_options
-    ]
-
-    selected_mindflow_model: MindFlowModel = select_option(
-        "Select MindFlow model. Enter #",
-        mindflow_model_options,
-        mindflow_model_descriptions,
-    )
-    if selected_mindflow_model.id == MindFlowModelID.QUERY.value:
-        configure_query_model()
-    elif selected_mindflow_model.id == MindFlowModelID.INDEX.value:
-        configure_index_model()
-    elif selected_mindflow_model.id == MindFlowModelID.EMBEDDING.value:
-        configure_embedding_model()
-
-
-def configure_query_model():
-    model_ids = [
-        ModelID.GPT_3_5_TURBO.value,
-        ModelID.GPT_4.value,
-        ModelID.CLAUDE_INSTANT_V1.value,
-        ModelID.CLAUDE_V1.value,
-    ]
-    model_options: List[Model] = [Model.load(model_id) for model_id in model_ids]
-    model_descriptions: List[str] = [
-        model.config_description for model in model_options
-    ]
-
-    selected_model: Model = select_option(
-        "Select chat model. Recommended GPT-4/Claude V1. Enter #",
-        model_options,
-        model_descriptions,
-    )
-    mindflow_model_config: MindFlowModelConfig = MindFlowModelConfig.load(
-        f"{MindFlowModelID.QUERY.value}_config"
-    ) or MindFlowModelConfig(f"{MindFlowModelID.QUERY.value}_config")
-    mindflow_model_config.model = selected_model.id
-    mindflow_model_config.save()
-
-    print(f"Query Model: {selected_model.id} saved!")
-
-
-def configure_index_model():
-    model_ids = [
-        ModelID.GPT_3_5_TURBO.value,
-        ModelID.GPT_4.value,
-        ModelID.CLAUDE_INSTANT_V1.value,
-        ModelID.CLAUDE_V1.value,
-    ]
-    model_options: List[Model] = [Model.load(model_id) for model_id in model_ids]
-    model_descriptions: List[str] = [
-        model.config_description for model in model_options
-    ]
-
-    selected_model: Model = select_option(
-        "Select chat model. Recommended GPT-3.5 Turbo/Claude Instant V1. Enter #",
-        model_options,
-        model_descriptions,
-    )
-    mindflow_model_config: MindFlowModelConfig = MindFlowModelConfig.load(
-        f"{MindFlowModelID.INDEX.value}_config"
-    ) or MindFlowModelConfig(f"{MindFlowModelID.INDEX.value}_config")
-    mindflow_model_config.model = selected_model.id
-    mindflow_model_config.save()
-
-    print(f"Index Model: {selected_model.id} saved!")
-
-
-def configure_embedding_model():
-    model_ids = [ModelID.TEXT_EMBEDDING_ADA_002.value]
-    model_options: List[Model] = [Model.load(model_id) for model_id in model_ids]
-    model_descriptions: List[str] = [
-        model.config_description for model in model_options
-    ]
-
-    selected_model: Model = select_option(
-        "Select chat model. Only one option... for now :) Enter #",
-        model_options,
-        model_descriptions,
-    )
-    mindflow_model_config: MindFlowModelConfig = MindFlowModelConfig.load(
-        f"{MindFlowModelID.EMBEDDING.value}_config"
-    ) or MindFlowModelConfig(f"{MindFlowModelID.EMBEDDING.value}_config")
-    mindflow_model_config.model = selected_model.id
-    mindflow_model_config.save()
-
-    print(f"Embedding Model: {selected_model.id} saved!")
-
-
-def clear_console(lines: int):
-    for _ in range(lines):
-        sys.stdout.write("\033[F")  # Move cursor up one line
-        sys.stdout.write("\033[K")  # Clear the line
-
-
 def select_option(prompt: str, options: List, descriptions: List[str]) -> int:
     for i, description in enumerate(descriptions, 1):
         click.echo(f"{i}: {description}")
 
     lines_to_clear = len(descriptions)
     while True:
         lines_to_clear += 1
@@ -148,7 +134,15 @@
         ):
             break
         click.echo("Invalid selection. Please try again.")
         lines_to_clear += 1
 
     clear_console(lines_to_clear)
     return options[selected_option_index - 1]
+
+
+def clear_console(lines: int):
+    import sys
+
+    for _ in range(lines):
+        sys.stdout.write("\033[F")  # Move cursor up one line
+        sys.stdout.write("\033[K")  # Clear the line
```

### Comparing `mindflow-0.5.3/mindflow/cli/commands/delete.py` & `mindflow-0.5.4/mindflow/cli/commands/delete.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-import asyncio
-from typing import List
-
 import click
-from result import Result
-
-from mindflow.core.commands.delete import run_delete
-from mindflow.core.resolving.resolve import resolve_paths_to_document_references
-from mindflow.core.types.document import DocumentReference, get_document_id
+from typing import List
 
 
 @click.command(help="Delete your MindFlow index")
 @click.argument("document_paths", type=str, nargs=-1)
 def delete(document_paths: List[str]):
+    import asyncio
+
+    from result import Result
+
+    from mindflow.core.commands.delete import run_delete
+    from mindflow.core.resolving.resolve import resolve_paths_to_document_references
+    from mindflow.core.types.document import DocumentReference, get_document_id
+
     document_references: List[DocumentReference] = resolve_paths_to_document_references(
         document_paths
     )
 
     document_ids = [
         document_id
         for document_id in [
```

### Comparing `mindflow-0.5.3/mindflow/cli/commands/gen.py` & `mindflow-0.5.4/mindflow/cli/commands/gen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-import asyncio
-import os
 import click
-from result import Result, Err
-
-from mindflow.core.commands.gen import run_code_generation
-from mindflow.core.settings import Settings
-from mindflow.core.types.model import ModelApiCallError
 
 
 @click.command(help="AI powered boilerplate code generation.")
 @click.argument("output_path", type=str)
 @click.argument("prompt", type=str)
 def gen(output_path: str, prompt: str):
+    import os
+    import asyncio
+
+    from result import Result, Err
+
+    from mindflow.core.commands.gen import run_code_generation
+    from mindflow.core.settings import Settings
+    from mindflow.core.types.model import ModelApiCallError
+
     if os.path.exists(output_path):
         click.confirm(
             f"The output path '{output_path}' already exists. Do you want to overwrite it?",
             abort=True,
         )
         os.remove(output_path)
```

### Comparing `mindflow-0.5.3/mindflow/cli/commands/git/commit.py` & `mindflow-0.5.4/mindflow/cli/commands/git/commit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-import asyncio
-from typing import Tuple, Optional
-
 import click
-from result import Err, Result
-
+from typing import Tuple, Optional
 from mindflow.cli.util import passthrough_command
-from mindflow.core.commands.git.commit import create_gpt_commit_message
-from mindflow.core.execute import execute_command_without_trace
-from mindflow.core.settings import Settings
-from mindflow.core.types.model import ModelApiCallError
 
 
 @passthrough_command(help="Generate a git commit response by feeding git diff to gpt")
-# @overloaded_option(
-#     "-m",
-#     "--message",
-#     help="Don't use mindflow to generate a commit message, use this one instead.",
-#     default=None,
-# )
 @click.option(
     "-m",
     "--message",
     help="Don't use mindflow to generate a commit message, use this one instead.",
     default=None,
 )
 def commit(args: Tuple[str], message: Optional[str] = None):
+    import asyncio
+
+    from result import Err, Result
+
+    from mindflow.cli.util import execute_command_without_trace
+    from mindflow.core.commands.git.commit import create_gpt_commit_message
+    from mindflow.core.settings import Settings
+    from mindflow.core.types.model import ModelApiCallError
+    from termcolor import colored
+
     if message is not None:
         click.echo(
-            f"Warning: Using message '{message}' instead of mindflow generated message."
+            colored(
+                f"Warning: Using message '{message}' instead of mindflow generated message.",
+                "yellow",
+            )
         )
         click.echo("It's recommended that you don't use the -m/--message flag.")
 
     if not message:
         diff_output = execute_command_without_trace(["git", "diff", "--cached"])
         run_commit_result: Result[str, ModelApiCallError] = asyncio.run(
             create_gpt_commit_message(Settings(), diff_output)
```

### Comparing `mindflow-0.5.3/mindflow/cli/commands/git/mr.py` & `mindflow-0.5.4/mindflow/cli/commands/git/mr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-import asyncio
-import subprocess
-from typing import Optional, Tuple
-
 import click
-from result import Err
+from typing import Optional, Tuple
 from mindflow.cli.util import passthrough_command
-from mindflow.core.command_parse import get_flag_values_from_args
-from mindflow.core.commands.git.pr import create_gpt_title_and_body
-from mindflow.core.execute import execute_command_without_trace
-from mindflow.core.settings import Settings
 
 
 @click.group()
 def mr():
     """
     MR command.
     """
@@ -31,26 +23,42 @@
     "--description",
     help="Don't use mindflow to generate a pr body, use this one instead.",
     default=None,
 )
 def create(
     args: Tuple[str], title: Optional[str] = None, description: Optional[str] = None
 ):
+    import asyncio
+    import subprocess
+
+    from result import Err
+
+    from mindflow.cli.util import (
+        execute_command_without_trace,
+        get_flag_values_from_args,
+    )
+    from mindflow.core.commands.git.pr import create_gpt_title_and_body
+    from mindflow.core.settings import Settings
+    from termcolor import colored
+
     if title is not None:
         click.echo(
-            f"Warning: Using message '{title}' instead of mindflow generated message."
+            colored(
+                f"Warning: Using message '{title}' instead of mindflow generated message. It's recommended that you don't use the -t/--title flag.",
+                "yellow",
+            )
         )
-        click.echo("It's recommended that you don't use the -t/--title flag.")
 
     if description is not None:
         click.echo(
-            f"Warning: Using message '{description}' instead of mindflow generated message."
+            colored(
+                f"Warning: Using message '{description}' instead of mindflow generated message. It's recommended that you don't use the -d/--description flag.",
+                "yellow",
+            )
         )
-        click.echo("It's recommended that you don't use the -d/--description flag.")
-
     if (
         base_branch_name := get_flag_values_from_args(args, ["--target-branch", "-b"])
     ) is None:
         base_branch_name = (
             subprocess.check_output(["git", "symbolic-ref", "refs/remotes/origin/HEAD"])
             .decode()
             .strip()
```

### Comparing `mindflow-0.5.3/mindflow/cli/commands/git/pr.py` & `mindflow-0.5.4/mindflow/cli/commands/git/pr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-import asyncio
-import subprocess
-from typing import Optional, Tuple
-
 import click
-from result import Err
+from typing import Optional, Tuple
 from mindflow.cli.util import passthrough_command
-from mindflow.core.command_parse import get_flag_values_from_args
-from mindflow.core.commands.git.pr import create_gpt_title_and_body
-from mindflow.core.execute import execute_command_without_trace
-from mindflow.core.settings import Settings
 
 
 @click.group()
 def pr():
     """
     PR command.
     """
@@ -29,25 +21,41 @@
 @click.option(
     "-b",
     "--body",
     help="Don't use mindflow to generate a pr body, use this one instead.",
     default=None,
 )
 def create(args: Tuple[str], title: Optional[str] = None, body: Optional[str] = None):
+    import asyncio
+    import subprocess
+
+    from result import Err
+    from termcolor import colored
+
+    from mindflow.cli.util import (
+        execute_command_without_trace,
+        get_flag_values_from_args,
+    )
+    from mindflow.core.commands.git.pr import create_gpt_title_and_body
+    from mindflow.core.settings import Settings
+
     if title is not None:
         click.echo(
-            f"Warning: Using message '{title}' instead of mindflow generated message."
+            colored(
+                f"Warning: Using message '{title}' instead of mindflow generated message. It's recommended that you don't use the -t/--title flag.",
+                "yellow",
+            )
         )
-        click.echo("It's recommended that you don't use the -t/--title flag.")
-
     if body is not None:
         click.echo(
-            f"Warning: Using message '{body}' instead of mindflow generated message."
+            colored(
+                f"Warning: Using message '{body}' instead of mindflow generated message. It's recommended that you don't use the -b/--body flag.",
+                "yellow",
+            )
         )
-        click.echo("It's recommended that you don't use the -d/--description flag.")
 
     if (base_branch_name := get_flag_values_from_args(args, ["--base", "-B"])) is None:
         base_branch_name = (
             subprocess.check_output(["git", "symbolic-ref", "refs/remotes/origin/HEAD"])
             .decode()
             .strip()
             .split("/")[-1]
```

### Comparing `mindflow-0.5.3/mindflow/cli/commands/inspect.py` & `mindflow-0.5.4/mindflow/cli/commands/inspect.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-import asyncio
-from typing import List
 import click
-from result import Result
 
-from mindflow.core.commands.inspect import run_inspect
-from mindflow.core.resolving.resolve import resolve_paths_to_document_references
-from mindflow.core.types.document import DocumentReference, get_document_id
+from typing import List
 
 
 @click.command(help="Inspect your MindFlow index")
 @click.argument("document_paths", type=str, nargs=-1)
 def inspect(document_paths: List[str]):
+    import asyncio
+
+    from typing import List
+    from result import Result
+
+    from mindflow.core.commands.inspect import run_inspect
+    from mindflow.core.resolving.resolve import resolve_paths_to_document_references
+    from mindflow.core.types.document import DocumentReference, get_document_id
+
     document_references: List[DocumentReference] = resolve_paths_to_document_references(
         document_paths
     )
     document_ids: List[str] = [
         document_id
         for document_reference in document_references
         if (
```

### Comparing `mindflow-0.5.3/mindflow/cli/commands/login.py` & `mindflow-0.5.4/mindflow/cli/commands/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import click
-from mindflow.cli.commands.config import select_option
-
-from mindflow.core.types.definitions.service import ServiceConfigID
-from mindflow.core.types.service import ServiceConfig
-from mindflow.core.types.store_traits.json import save_json_store
 
 
 @click.command(help="Set your API Key")
 def login():
+    from mindflow.cli.commands.config import select_option
+    from mindflow.core.types.definitions.service import ServiceConfigID
+    from mindflow.core.types.service import ServiceConfig
+    from mindflow.core.types.store_traits.json import save_json_store
+
     service_ids = [
         ServiceConfigID.OPENAI.value,
-        ServiceConfigID.ANTHROPIC.value,
         ServiceConfigID.PINECONE.value,
     ]
     service_options = [
         ServiceConfig.load(service_id, False) for service_id in service_ids
     ]
-    service_descriptions = ["OpenAI", "Anthropic", "Pinecone: (Vector DB)"]
+    service_descriptions = ["OpenAI", "Pinecone: (Vector DB)"]
     service_config: ServiceConfig = select_option(
         "Choose service to configure. Enter #",
         service_options,
         service_descriptions,
     )
 
     service_config.api_key = input("Enter API key: ")
```

### Comparing `mindflow-0.5.3/mindflow/cli/util.py` & `mindflow-0.5.4/mindflow/cli/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,26 @@
 import click
+import subprocess
+
+from typing import List, Tuple, Optional
+
+
+def get_flag_values_from_args(args: Tuple[str], flag: List[str]) -> Optional[str]:
+    for i, arg in enumerate(args):
+        if arg in flag:
+            try:
+                return args[i + 1]
+            except IndexError:
+                return None
+    return None
+
+
+def execute_command_without_trace(command: List[str]) -> str:
+    output = subprocess.Popen(command, stdout=subprocess.PIPE)
+    return output.communicate()[0].decode("utf-8")
 
 
 def passthrough_command(*command_args, **command_kwargs):
     """Just like the @click.command decorator, but allows all args to pass through (for wrapper cli commands)."""
 
     def _decorator(func):
         context_settings = command_kwargs.get("context_settings", {})
```

### Comparing `mindflow-0.5.3/mindflow/core/commands/chat.py` & `mindflow-0.5.4/mindflow/core/commands/chat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from typing import List
-
+from typing import AsyncGenerator, List
 from result import Err, Result
 
 from mindflow.core.types.conversation import Conversation
 from mindflow.core.types.definitions.conversation import ConversationID
 from mindflow.core.settings import Settings
 from mindflow.core.prompt_builders import (
     Role,
@@ -17,15 +16,15 @@
     get_token_count_from_document_query_for_model,
 )
 from mindflow.core.types.model import ConfiguredTextCompletionModel, ModelApiCallError
 
 
 async def run_chat(
     settings: Settings, document_paths: List[str], user_query: str
-) -> Result[str, ModelApiCallError]:
+) -> AsyncGenerator[Result[str, ModelApiCallError], None]:
     query_model: ConfiguredTextCompletionModel = settings.mindflow_models.query
     if (conversation := Conversation.load(ConversationID.CHAT_0.value)) is None:
         first_message = create_conversation_message(
             Role.SYSTEM.value, DEFAULT_CONVERSATION_SYSTEM_PROMPT
         )
         conversation = Conversation(
             {"id": ConversationID.CHAT_0.value, "messages": [first_message]}
@@ -42,22 +41,26 @@
     conversation.messages.append(
         create_conversation_message(Role.USER.value, "\n".join(texts))
     )
     conversation.messages = prune_messages_to_fit_context_window(
         conversation.messages, query_model
     )
 
-    query_model_result: Result[str, ModelApiCallError] = await query_model.call_api(
+    result = ""
+    async for char_stream_chunk in query_model.call_api_stream(  # type: ignore
         build_prompt_from_conversation_messages(conversation.messages, query_model)
-    )
-    if isinstance(query_model_result, Err):
-        return query_model_result
+    ):
+        if isinstance(char_stream_chunk, Err):
+            yield char_stream_chunk
+            return
+
+        result += char_stream_chunk.value
+        yield char_stream_chunk
 
     conversation.messages.append(
-        create_conversation_message(Role.ASSISTANT.value, query_model_result.value)
+        create_conversation_message(Role.ASSISTANT.value, result)
     )
     conversation.total_tokens = get_token_count_of_messages_for_model(
         query_model.tokenizer, conversation.messages
     )
 
     conversation.save()
-    return query_model_result
```

### Comparing `mindflow-0.5.3/mindflow/core/commands/delete.py` & `mindflow-0.5.4/mindflow/core/commands/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
-from typing import List
 
+from typing import List
 from result import Err, Ok, Result
 
 from mindflow.core.types.document import (
     Document,
     DocumentChunk,
     get_document_chunk_ids,
 )
```

### Comparing `mindflow-0.5.3/mindflow/core/commands/gen.py` & `mindflow-0.5.4/mindflow/core/commands/gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from result import Err, Ok, Result
+
 from mindflow.core.types.conversation import Conversation
 from mindflow.core.types.definitions.conversation import ConversationID
 from mindflow.core.settings import Settings
 from mindflow.core.text_processing.xml import get_text_within_xml
 
 from mindflow.core.prompt_builders import (
     Role,
```

### Comparing `mindflow-0.5.3/mindflow/core/commands/git/commit.py` & `mindflow-0.5.4/mindflow/core/commands/git/commit.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,20 +24,21 @@
 
     if (
         get_token_count_of_text_for_model(
             query_model.tokenizer, diff_output + COMMIT_PROMPT_PREFIX
         )
         > query_model.model.hard_token_limit
     ):
-        gpt_summarize_diff_result = await create_gpt_summarized_diff(
-            settings, diff_output
-        )
-        if isinstance(gpt_summarize_diff_result, Err):
-            return gpt_summarize_diff_result
-        commit_context = gpt_summarize_diff_result.value
+        summarized_diff = ""
+        async for char_stream_chunk in create_gpt_summarized_diff(
+            settings, diff_output, True
+        ):
+            if isinstance(char_stream_chunk, Err):
+                return char_stream_chunk
+            summarized_diff += char_stream_chunk.value
 
     response: Result[str, ModelApiCallError] = await query_model.call_api(
         build_prompt_from_conversation_messages(
             [
                 create_conversation_message(Role.SYSTEM.value, COMMIT_PROMPT_PREFIX),
                 create_conversation_message(Role.USER.value, commit_context),
             ],
```

### Comparing `mindflow-0.5.3/mindflow/core/commands/git/diff.py` & `mindflow-0.5.4/mindflow/core/commands/git/diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import os
 
-from typing import Dict, List, Tuple
+from typing import AsyncGenerator, Dict, List, Tuple
 from result import Ok, Result, Err
 
 from mindflow.core.types.model import (
     ConfiguredModel,
     ConfiguredTextCompletionModel,
     ModelApiCallError,
 )
@@ -22,15 +22,15 @@
 from mindflow.core.token_counting import get_token_count_of_text_for_model
 
 
 async def create_gpt_summarized_diff(
     settings: Settings,
     diff_output: str,
     detailed: bool = False,  # True
-) -> Result[str, ModelApiCallError]:
+) -> AsyncGenerator[Result[str, ModelApiCallError], None]:
     """Execute git diff and summarize with GPT."""
     index_model: ConfiguredTextCompletionModel = settings.mindflow_models.index
 
     diff_dict, excluded_filenames = parse_git_diff(diff_output)
     batched_parsed_diff_result = batch_git_diffs(diff_dict, index_model)
 
     diff_summary: str = ""
@@ -48,35 +48,37 @@
             index_model,
         )
         tasks.append(asyncio.create_task(index_model.call_api(prompt)))
 
     results: List[Result[str, ModelApiCallError]] = await asyncio.gather(*tasks)
     for result in results:
         if isinstance(result, Err):
-            return result
+            yield result
+            return
         diff_summary += result.value
 
     if len(excluded_filenames) > 0:
         diff_summary += f"\n\nNOTE: The following files were excluded from the diff: {', '.join(excluded_filenames)}"
 
     if detailed:
-        return Ok(diff_summary)
+        yield Ok(diff_summary)
 
     query_model: ConfiguredTextCompletionModel = settings.mindflow_models.query
-    return await query_model.call_api(
+    async for char_stream_chunk in query_model.call_api_stream(  # type: ignore
         build_prompt_from_conversation_messages(
             [
                 create_conversation_message(
                     Role.SYSTEM.value, GIT_DIFF_SUMMARIZE_PROMPT
                 ),
                 create_conversation_message(Role.USER.value, diff_summary),
             ],
             query_model,
         )
-    )
+    ):
+        yield char_stream_chunk
 
 
 # NOTE: make sure to have a the "." in the file extension (if applicable)
 # NOTE: these are things that WON'T already be git ignored.
 IGNORE_FILE_EXTENSIONS = [
     ".pyc",
     ".ipynb",
```

### Comparing `mindflow-0.5.3/mindflow/core/commands/git/pr.py` & `mindflow-0.5.4/mindflow/core/commands/git/pr.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,20 +23,21 @@
 
     if (
         get_token_count_of_text_for_model(
             query_model.tokenizer, diff_output + PR_TITLE_PREFIX
         )
         > query_model.model.hard_token_limit
     ):
-        gpt_summarize_diff_result = await create_gpt_summarized_diff(
-            settings, diff_output
-        )
-        if isinstance(gpt_summarize_diff_result, Err):
-            return gpt_summarize_diff_result
-        pr_context = gpt_summarize_diff_result.value
+        pr_context = ""
+        async for char_stream_chunk in create_gpt_summarized_diff(
+            settings, diff_output, True
+        ):
+            if isinstance(char_stream_chunk, Err):
+                return char_stream_chunk
+            pr_context += char_stream_chunk.value
 
     tasks: List[asyncio.Task[Result[str, ModelApiCallError]]] = []
     if title is None:
         tasks.append(
             asyncio.create_task(
                 query_model.call_api(
                     build_prompt_from_conversation_messages(
```

### Comparing `mindflow-0.5.3/mindflow/core/commands/index.py` & `mindflow-0.5.4/mindflow/core/commands/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+import sys
 import asyncio
 import hashlib
-import sys
+import numpy as np
 
 from typing import List, Optional
-
-from alive_progress import alive_bar
-import numpy as np
 from result import Err, Ok, Result
 
+from alive_progress import alive_bar  # type: ignore
+
 from mindflow.core.types.document import (
     Document,
     DocumentChunk,
     DocumentReference,
     get_document_id,
 )
 from mindflow.core.types.model import (
@@ -360,15 +360,15 @@
     return Ok(
         DocumentChunk(
             {
                 "id": id,
                 "start_pos": start_pos,
                 "end_pos": end_pos,
                 "summary": appended_summaries,
-                "embedding": list(embedding_result.value),
+                "embedding": embedding_result.value,
             }
         )
     )
 
 
 async def collect_leaves_with_embeddings_from_appended_branch_summaries(
     document_hash: str,
```

### Comparing `mindflow-0.5.3/mindflow/core/commands/inspect.py` & `mindflow-0.5.4/mindflow/core/commands/inspect.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
-from typing import List
 
+from typing import List
 from result import Err, Ok, Result
 
 from mindflow.core.types.document import (
     Document,
     DocumentChunk,
     get_document_chunk_ids,
 )
```

### Comparing `mindflow-0.5.3/mindflow/core/commands/query.py` & `mindflow-0.5.4/mindflow/core/commands/query.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
-from typing import Dict, List, Tuple
-from result import Err, Ok, Result
 
-import numpy as np
+from io import TextIOWrapper
+
+from typing import AsyncGenerator, Dict, List, Optional, Tuple
+from result import Err, Ok, Result
 
 from mindflow.core.types.document import (
     Document,
     DocumentChunk,
     get_document_chunk_ids,
     get_document_id,
 )
@@ -26,15 +27,15 @@
     ConfiguredEmbeddingModel,
     ModelApiCallError,
 )
 
 
 async def run_query(
     settings: Settings, document_paths: List[str], query: str
-) -> Result[str, ModelApiCallError]:
+) -> AsyncGenerator[Result[str, ModelApiCallError], None]:
     """Query files, folders, and websites."""
     completion_model: ConfiguredTextCompletionModel = settings.mindflow_models.query
     embedding_model: ConfiguredEmbeddingModel = settings.mindflow_models.embedding
 
     document_hash_to_path: Dict[str, str] = {
         document_id: doc_reference.path
         for doc_reference in resolve_paths_to_document_references(document_paths)
@@ -52,73 +53,95 @@
     )
     query_embedding_task = embedding_model.call_api(query)
 
     # Now await both tasks at the same time
     documents, query_embedding_result = await asyncio.gather(
         document_task, query_embedding_task
     )
-
     if isinstance(query_embedding_result, Err):
-        return query_embedding_result
+        yield query_embedding_result
+        return
 
     document_chunk_ids: List[str] = get_document_chunk_ids(documents)
     if not (
         top_document_chunks := await DocumentChunk.query(
-            vector=np.array(query_embedding_result.value).reshape(1, -1),
+            vector=query_embedding_result.value,
             ids=document_chunk_ids,
-            top_k=100,
+            top_k=25,
         )
     ):
-        return Ok(
+        yield Ok(
             "No index for requested hashes. Please generate index for passed content."
         )
 
     document_selection_batch: List[Tuple[str, DocumentChunk]] = [
         (document_hash_to_path[document_chunk.id.split("_")[0]], document_chunk)
         for document_chunk in top_document_chunks
     ]
 
     trimmed_content: str = select_and_trim_text_to_fit_context_window(
         completion_model, query, document_selection_batch
     )
-    return await completion_model.call_api(
+
+    async for char_stream_chunk in completion_model.call_api_stream(  # type: ignore
         build_prompt_from_conversation_messages(
             [
                 create_conversation_message(Role.SYSTEM.value, QUERY_PROMPT_PREFIX),
                 create_conversation_message(
                     Role.USER.value, f"{query}\n\n{trimmed_content}"
                 ),
             ],
             completion_model,
         )
-    )
+    ):
+        yield char_stream_chunk
 
 
 def select_and_trim_text_to_fit_context_window(
     configured_model: ConfiguredModel,
     query: str,
     top_document_chunks: List[Tuple[str, DocumentChunk]],
 ) -> str:
-    selected_content: str = ""
-    for path, document_chunk in top_document_chunks:
-        with open(path, "r", encoding="utf-8") as file:
+    selected_content: str
+    selected_content_parts: List[str] = []
+    prev_path = None
+    file: Optional[TextIOWrapper] = None
+    top_document_chunks.sort(key=lambda x: x[0])  # Sorting by path
+    try:
+        for path, document_chunk in top_document_chunks:
+            if path != prev_path:
+                if file is not None:
+                    file.close()
+                file = open(path, "r", encoding="utf-8")
+                prev_path = path
+
+            assert file is not None
             file.seek(document_chunk.start_pos)
-            selected_content += formatted_chunk(
-                path,
-                document_chunk,
-                file.read(int(document_chunk.end_pos) - int(document_chunk.start_pos)),
+            selected_content_parts.append(
+                formatted_chunk(
+                    path,
+                    document_chunk,
+                    file.read(
+                        int(document_chunk.end_pos) - int(document_chunk.start_pos)
+                    ),
+                )
             )
+            selected_content = "".join(selected_content_parts)
             if (
                 get_token_count_of_text_for_model(
                     configured_model.tokenizer, query + selected_content
                 )
                 > configured_model.model.hard_token_limit
             ):
                 break
+    finally:
+        if file is not None:
+            file.close()
 
+    selected_content = "".join(selected_content_parts)
     left, right = 0, len(selected_content)
     while left <= right:
         mid = (left + right) // 2
         if (
             get_token_count_of_text_for_model(
                 configured_model.tokenizer, query + selected_content[:mid]
             )
```

### Comparing `mindflow-0.5.3/mindflow/core/file_processing/extract.py` & `mindflow-0.5.4/mindflow/core/file_processing/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import logging
 import os
+import logging
+
 from typing import List
 
 from mindflow.core.file_processing.git import (
     is_path_within_git_repo,
     get_all_unignored_git_files_from_path,
 )
```

### Comparing `mindflow-0.5.3/mindflow/core/file_processing/git.py` & `mindflow-0.5.4/mindflow/core/file_processing/git.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Handles git related operations."""
-import logging
 import os
+import logging
 import subprocess
-from typing import List
-from typing import Union
+
+from typing import List, Union
 
 
 def is_path_within_git_repo(path: Union[str, os.PathLike]) -> bool:
     try:
         output = subprocess.run(
             ["git", "-C", str(path), "rev-parse", "--git-dir"],
             capture_output=True,
```

### Comparing `mindflow-0.5.3/mindflow/core/prompt_builders.py` & `mindflow-0.5.4/mindflow/core/prompt_builders.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from enum import Enum
-from typing import Dict, Union
-from typing import List
-from mindflow.core.types.model import ConfiguredModel
+import json
+import anthropic  # type: ignore
 
-import anthropic
+from enum import Enum
+from typing import Dict, Union, List
 
+from mindflow.core.types.model import ConfiguredModel
 from mindflow.core.types.definitions.service import ServiceID
 from mindflow.core.constants import MinimumReservedLength
 from mindflow.core.token_counting import get_token_count_of_text_for_model
 
 
 class Role(Enum):
     SYSTEM = "system"
@@ -18,48 +18,46 @@
 
 def create_conversation_message(role: str, prompt: str) -> Dict[str, str]:
     return {"role": role, "content": prompt}
 
 
 def build_prompt_from_conversation_messages(
     messages: List[Dict[str, str]], configured_model: ConfiguredModel
-) -> Union[List[Dict], str]:
-    if configured_model.model.service == ServiceID.OPENAI.value:
-        return messages
-
-    prompt_parts = []
-    for message in messages:
-        role = message["role"]
-        prompt = message["content"]
-
-        if role == Role.SYSTEM.value:
-            prompt_parts.append(anthropic.HUMAN_PROMPT + prompt)
-            prompt_parts.append(
-                anthropic.AI_PROMPT
-                + " Sure! I will respond to all following messages with a response like you have just outlined for me."
-            )
-        elif role in [Role.USER.value, Role.ASSISTANT.value]:
-            prompt_parts.append(
-                (
-                    anthropic.HUMAN_PROMPT
-                    if role == Role.USER.value
-                    else anthropic.AI_PROMPT
-                )
-                + prompt
-            )
+) -> List[Dict]:
+    return messages
+
+    # prompt_parts = []
+    # for message in messages:
+    #     role = message["role"]
+    #     prompt = message["content"]
+
+    #     if role == Role.SYSTEM.value:
+    #         prompt_parts.append(anthropic.HUMAN_PROMPT + prompt)
+    #         prompt_parts.append(
+    #             anthropic.AI_PROMPT
+    #             + " Sure! I will respond to all following messages with a response like you have just outlined for me."
+    #         )
+    #     elif role in [Role.USER.value, Role.ASSISTANT.value]:
+    #         prompt_parts.append(
+    #             (
+    #                 anthropic.HUMAN_PROMPT
+    #                 if role == Role.USER.value
+    #                 else anthropic.AI_PROMPT
+    #             )
+    #             + prompt
+    #         )
 
-    return "".join(prompt_parts) + anthropic.AI_PROMPT
+    # return "".join(prompt_parts) + anthropic.AI_PROMPT
 
 
 def prune_messages_to_fit_context_window(
     messages: List[Dict[str, str]], configured_model: ConfiguredModel
 ) -> List[Dict[str, str]]:
-    # Improvement can be made on the estimation here for Anthropic system messages
-    content = ""
     for i in range(0, len(messages)):
-        content += f"{messages[i]['role']}\n\n {messages[i]['content']}"
         if (
-            get_token_count_of_text_for_model(configured_model.tokenizer, content)
-            > configured_model.model.hard_token_limit - MinimumReservedLength.CHAT.value
+            get_token_count_of_text_for_model(
+                configured_model.tokenizer, json.dumps(messages[i : len(messages) - 1])
+            )
+            < configured_model.model.hard_token_limit - 1500
         ):
-            return messages[:i]
-    return messages
+            return messages[i : len(messages) - 1]
+    return []
```

### Comparing `mindflow-0.5.3/mindflow/core/prompts.py` & `mindflow-0.5.4/mindflow/core/prompts.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.3/mindflow/core/resolving/resolve.py` & `mindflow-0.5.4/mindflow/core/resolving/resolve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Module for resolving documents types."""
 import sys
+
 from typing import List
 from mindflow.core.types.document import DocumentReference
 
 from mindflow.core.resolving.resolvers.file_resolver import FileResolver
 
 
 def resolve_path_to_document_reference(
```

### Comparing `mindflow-0.5.3/mindflow/core/resolving/resolvers/file_resolver.py` & `mindflow-0.5.4/mindflow/core/resolving/resolvers/file_resolver.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from typing import List, Union
-from mindflow.core.types.document import DocumentReference
 
+from mindflow.core.types.document import DocumentReference
 from mindflow.core.types.definitions.document import DocumentType
 from mindflow.core.resolving.resolvers.document_resolver import DocumentResolver
 from mindflow.core.file_processing.extract import extract_files_from_directory
 
 
 class FileResolver(DocumentResolver):
     @staticmethod
```

### Comparing `mindflow-0.5.3/mindflow/core/token_counting.py` & `mindflow-0.5.4/mindflow/core/token_counting.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
-from typing import Dict, List
-
 import tiktoken
 
+from typing import Dict, List
+
 
 def get_token_count_of_text_for_model(tokenizer: tiktoken.Encoding, text: str) -> int:
     try:
         return len(tokenizer.encode(text))
     except Exception:
         return len(text) // 3
```

### Comparing `mindflow-0.5.3/mindflow/core/types/definitions/mind_flow_model.py` & `mindflow-0.5.4/mindflow/core/types/definitions/mind_flow_model.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.3/mindflow/core/types/definitions/model.py` & `mindflow-0.5.4/mindflow/core/types/definitions/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         ModelParameterKey.NAME.value: "GPT 3.5 Turbo",
         ModelParameterKey.SERVICE.value: "openai",
         ModelParameterKey.MODEL_TYPE.value: ModelType.TEXT_COMPLETION.value,
         ModelParameterKey.URL.value: "https://api.openai.com/v1/chat/completions",
         ModelParameterKey.DEFAULT_SOFT_TOKEN_LIMIT.value: 500,
         ModelParameterKey.HARD_TOKEN_LIMIT.value: 4_000,
         ModelParameterKey.MAX_REQUESTS_PER_MINUTE.value: 3_500,
-        ModelParameterKey.MAX_TOKENS_PER_MINUTE.value: 90_000,
+        ModelParameterKey.MAX_TOKENS_PER_MINUTE.value: 40_000,
         ModelParameterKey.TOKEN_COST.value: 0.002,
         ModelParameterKey.TOKEN_COST_UNIT.value: 1_000,
         ModelParameterKey.CONFIG_DESCRIPTION.value: f"GPT 3.5 Turbo:       OpenAI's Fast, cheap, and still powerful model.       Token Limit: {4_000}.",
     },
     ModelID.GPT_3_5_TURBO_0301.value: {
         ModelParameterKey.ID.value: ModelID.GPT_3_5_TURBO_0301.value,
         ModelParameterKey.NAME.value: "GPT 3.5 Turbo March 1st",
@@ -72,15 +72,15 @@
         ModelParameterKey.NAME.value: "GPT 4",
         ModelParameterKey.SERVICE.value: "openai",
         ModelParameterKey.MODEL_TYPE.value: ModelType.TEXT_COMPLETION.value,
         ModelParameterKey.URL.value: "https://api.openai.com/v1/chat/completions",
         ModelParameterKey.DEFAULT_SOFT_TOKEN_LIMIT.value: 500,
         ModelParameterKey.HARD_TOKEN_LIMIT.value: 8_192,
         ModelParameterKey.MAX_REQUESTS_PER_MINUTE.value: 3_500,
-        ModelParameterKey.MAX_TOKENS_PER_MINUTE.value: 90_000,
+        ModelParameterKey.MAX_TOKENS_PER_MINUTE.value: 40_000,
         ModelParameterKey.TOKEN_COST.value: 0.002,
         ModelParameterKey.TOKEN_COST_UNIT.value: 1_000,
         ModelParameterKey.CONFIG_DESCRIPTION.value: f"GPT 4:               OpenAI's most powerful model (slower + expensive).    Token Limit: {str(8192)}. Get access -> https://openai.com/waitlist/gpt-4-api.",
     },
     ModelID.GPT_4_0314.value: {
         ModelParameterKey.ID.value: ModelID.GPT_4_0314.value,
         ModelParameterKey.NAME.value: "GPT 4 32K March 14th",
```

### Comparing `mindflow-0.5.3/mindflow/core/types/definitions/service.py` & `mindflow-0.5.4/mindflow/core/types/definitions/service.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.3/mindflow/core/types/document.py` & `mindflow-0.5.4/mindflow/core/types/document.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import hashlib
+
 from typing import List, Optional, Union
-from mindflow.core.errors import ModelError
-from mindflow.core.types.model import ConfiguredModel
 
 from mindflow.core.types.store_traits.pinecone import PineconeStore
 from mindflow.core.types.definitions.document import DocumentType
 
 
 class DocumentReference:
     path: str
```

### Comparing `mindflow-0.5.3/mindflow/core/types/mindflow_model.py` & `mindflow-0.5.4/mindflow/core/types/mindflow_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from functools import cached_property
 import sys
+
 from typing import Dict
+from functools import cached_property
+
 from mindflow.core.types.definitions.model import ModelID
 from mindflow.core.types.store_traits.static import StaticStore
 from mindflow.core.types.store_traits.json import JsonStore
 
 from mindflow.core.types.model import (
     ConfiguredEmbeddingModel,
     ConfiguredOpenAIChatCompletionModel,
-    ConfiguredAnthropicChatCompletionModel,
     ConfiguredOpenAITextEmbeddingModel,
     ConfiguredTextCompletionModel,
 )
 from mindflow.core.types.service import ConfiguredServices
 from mindflow.core.types.definitions.mind_flow_model import MindFlowModelID
 from mindflow.core.types.definitions.service import (
     ServiceConfigParameterKey,
@@ -48,16 +49,14 @@
             mindflow_model = MindFlowModel.load(MindFlowModelID.INDEX.value)
             model_id = self.get_default_model_id(
                 MindFlowModelID.INDEX.value, mindflow_model.defaults
             )
 
         if model_id in [ModelID.GPT_3_5_TURBO.value, ModelID.GPT_4.value]:
             return ConfiguredOpenAIChatCompletionModel(model_id)
-        elif model_id in [ModelID.CLAUDE_INSTANT_V1.value, ModelID.CLAUDE_V1.value]:
-            return ConfiguredAnthropicChatCompletionModel(model_id)
         raise Exception("Unsupported model: " + model_id)
 
     @cached_property
     def query(self) -> ConfiguredTextCompletionModel:
         if (
             model_id := getattr(
                 MindFlowModelConfig.load(f"{MindFlowModelID.QUERY.value}_config"),
@@ -68,16 +67,14 @@
             mindflow_model = MindFlowModel.load(MindFlowModelID.QUERY.value)
             model_id = self.get_default_model_id(
                 MindFlowModelID.QUERY.value, mindflow_model.defaults
             )
 
         if model_id in [ModelID.GPT_3_5_TURBO.value, ModelID.GPT_4.value]:
             return ConfiguredOpenAIChatCompletionModel(model_id)
-        elif model_id in [ModelID.CLAUDE_INSTANT_V1.value, ModelID.CLAUDE_V1.value]:
-            return ConfiguredAnthropicChatCompletionModel(model_id)
         raise Exception("Unsupported model: " + model_id)
 
     @cached_property
     def embedding(self) -> ConfiguredEmbeddingModel:
         if (
             model_id := getattr(
                 MindFlowModelConfig.load(f"{MindFlowModelID.EMBEDDING.value}_config"),
```

### Comparing `mindflow-0.5.3/mindflow/core/types/model.py` & `mindflow-0.5.4/mindflow/core/types/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from abc import ABC, abstractmethod
-import asyncio
-
+import json
+import time
 import aiohttp
 import logging
-import time
-from result import Err, Ok, Result
+import asyncio
+import tiktoken
 
-from typing import Dict, Optional, Tuple, Union
+from abc import ABC, abstractmethod
+from result import Err, Ok, Result
+from typing import Any, AsyncGenerator, Dict, List, Optional, Tuple, Union
 
-import numpy as np
-import tiktoken
 from mindflow.core.token_counting import (
     get_token_count_of_messages_for_model,
     get_token_count_of_text_for_model,
 )
 
 from mindflow.core.types.store_traits.json import JsonStore
 from mindflow.core.types.store_traits.static import StaticStore
@@ -214,18 +213,29 @@
 
 
 class ApiTextCompletionModel(ABC):
     @abstractmethod
     async def call_api(self, *args, **kwargs) -> Result[str, ModelApiCallError]:
         pass
 
+    @abstractmethod
+    async def call_api_stream(
+        self,
+        messages: List[Any],
+        temperature: float = 0.0,
+        max_tokens: Optional[int] = None,
+        stop: Optional[List[Any]] = None,
+        request_tokens: Optional[int] = None,
+    ) -> AsyncGenerator[Result[str, ModelApiCallError], None]:
+        pass
+
 
 class ApiEmbeddingModel(ABC):
     @abstractmethod
-    async def call_api(self, *args, **kwargs) -> Result[np.ndarray, ModelApiCallError]:
+    async def call_api(self, *args, **kwargs) -> Result[List[float], ModelApiCallError]:
         pass
 
 
 class ConfiguredTextCompletionModel(ApiTextCompletionModel, ConfiguredModel, ABC):
     pass
 
 
@@ -279,22 +289,26 @@
         await self.status_tracker.increment_requests_count_total()
         await self.status_tracker.increment_requests_count_in_progress()
         await self.status_tracker.add_tokens_count_total(request_tokens)
         async with aiohttp.ClientSession() as session:
             while try_count < 5:
                 try:
                     async with session.post(
-                        self.model.url, headers=self.headers, json=payload
+                        self.model.url,
+                        headers={
+                            "Authorization": f"Bearer {self.api_key}",
+                            "Content-Type": "application/json",
+                        },
+                        json=payload,
                     ) as response:
                         result = await response.json()
 
                         if "error" not in result:
                             await self.status_tracker.increment_requests_count_successful()
                             await self.status_tracker.decrement_requests_count_in_progress()
-                            # print(result)
                             return Ok(result["choices"][0]["message"]["content"])
 
                         logging.warning(
                             f"Request {payload} failed with error {result['error']}"
                         )
                         try_count += 1
                         if "Rate limit" in result["error"].get("message", ""):
@@ -309,38 +323,41 @@
                 except Exception as e:
                     logging.warning(f"Request {payload} failed with exception {e}")
                     await self.status_tracker.increment_error_count_other()
                     return Err(UncaughtModelException(str(e)))
 
             return model_error
 
-
-class ConfiguredAnthropicChatCompletionModel(ConfiguredTextCompletionModel):
-    async def call_api(
+    async def call_api_stream(  # type: ignore
         self,
-        prompt: str,
+        messages: list,
         temperature: float = 0.0,
-        max_tokens: Optional[int] = 100,
+        max_tokens: Optional[int] = None,
+        stop: Optional[list] = None,
         request_tokens: Optional[int] = None,
-    ) -> Result[str, ModelApiCallError]:
-        assert isinstance(prompt, str) and prompt != ""
+    ) -> AsyncGenerator[Result[str, ModelApiCallError], None]:
+        assert isinstance(messages, list) and len(messages) > 0
         assert request_tokens is None or request_tokens > 0
         assert max_tokens is None or max_tokens > 0
         assert temperature >= 0.0 and temperature <= 1.0
+        assert stop is None or isinstance(stop, list)
 
         payload = {
             "model": self.model.id,
-            "prompt": prompt,
-            "stop_sequences": [],
-            "max_tokens": max_tokens,
+            "messages": messages,
             "temperature": temperature,
+            "max_tokens": max_tokens,
+            "stop": stop,
+            "stream": True,
         }
 
         if request_tokens is None:
-            request_tokens = get_token_count_of_text_for_model(self.tokenizer, prompt)
+            request_tokens = get_token_count_of_messages_for_model(
+                self.tokenizer, messages
+            )
 
         while True:
             (
                 available_request_capacity,
                 available_token_capacity,
             ) = await self.status_tracker.get_available_capacities()
             if (
@@ -352,48 +369,69 @@
             break
 
         try_count = 0
         model_error: Err
         await self.status_tracker.increment_requests_count_total()
         await self.status_tracker.increment_requests_count_in_progress()
         await self.status_tracker.add_tokens_count_total(request_tokens)
+
+        # The rest of your setup remains the same...
         async with aiohttp.ClientSession() as session:
             while try_count < 5:
                 try:
                     async with session.post(
-                        self.model.url, headers=self.headers, json=payload
+                        self.model.url,
+                        headers={
+                            "Authorization": f"Bearer {self.api_key}",
+                            "Content-Type": "application/json",
+                        },
+                        json=payload,
                     ) as response:
-                        result = await response.json()
-
-                        if "error" not in result:
-                            await self.status_tracker.increment_requests_count_successful()
-                            await self.status_tracker.decrement_requests_count_in_progress()
-                            return Ok(result["completion"])
-
-                        logging.warning(
-                            f"Request {payload} failed with exception {result['error']}"
-                        )
-
-                        # Figure out how to catch rate limiting errors
-                        try_count += 1
-                        model_error = Err(APIError(result["error"]))
-                        await self.status_tracker.increment_error_count_other()
-
+                        buffer = ""
+                        async for data in response.content.iter_any():
+                            buffer += data.decode("utf-8")
+                            event, buffer = buffer.split("\n\n", 1)
+                            lines = event.split("\n")
+                            try:
+                                result = json.loads(lines[-1][5:])  # remove "data: "
+                            except Exception as e:
+                                return
+                            if "error" not in result:
+                                await self.status_tracker.increment_requests_count_successful()
+                                await self.status_tracker.decrement_requests_count_in_progress()
+                                if not result["choices"][0]["delta"]:
+                                    print("No delta")
+                                    continue
+                                yield Ok(
+                                    result["choices"][0]["delta"]["content"]
+                                )  # Yield the result
+                            else:
+                                logging.warning(
+                                    f"Request {payload} failed with error {result['error']}"
+                                )
+                                try_count += 1
+                                if "Rate limit" in result["error"].get("message", ""):
+                                    model_error = Err(RateLimitError(result["error"]))
+                                    await self.status_tracker.increment_error_count_rate_limit()
+                                    await asyncio.sleep(5)
+                                    continue
+                                model_error = Err(APIError(result["error"]))
+                                await self.status_tracker.increment_error_count_api()
+                                yield model_error
+                        return
                 except Exception as e:
                     logging.warning(f"Request {payload} failed with exception {e}")
                     await self.status_tracker.increment_error_count_other()
-                    return Err(UncaughtModelException(str(e)))
-
-            return model_error
+                    yield Err(UncaughtModelException(str(e)))
 
 
 class ConfiguredOpenAITextEmbeddingModel(ConfiguredEmbeddingModel):
     async def call_api(
         self, text: str, request_tokens: Optional[int] = None
-    ) -> Result[np.ndarray, ModelApiCallError]:
+    ) -> Result[List[float], ModelApiCallError]:
         assert isinstance(text, str) and text != ""
 
         payload = {
             "model": self.model.id,
             "input": text,
         }
 
@@ -426,15 +464,15 @@
                         self.model.url, headers=self.headers, json=payload
                     ) as response:
                         result = await response.json()
 
                         if "error" not in result:
                             await self.status_tracker.increment_requests_count_successful()
                             await self.status_tracker.decrement_requests_count_in_progress()
-                            return Ok(np.array(result["data"][0]["embedding"]))
+                            return Ok(result["data"][0]["embedding"])
 
                         e = str(result["error"])
                         logging.warning(
                             f"Request {payload} failed with error {result['error']}"
                         )
                         try_count += 1
                         if "Rate limit" in result["error"].get("message", ""):
```

### Comparing `mindflow-0.5.3/mindflow/core/types/service.py` & `mindflow-0.5.4/mindflow/core/types/service.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.3/mindflow/core/types/store_traits/json.py` & `mindflow-0.5.4/mindflow/core/types/store_traits/json.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import json
 import os
+import json
 
-from typing import List, Type, TypeVar, Union
-from typing import Optional
+from typing import List, Type, TypeVar, Union, Optional
 
 
 def get_mindflow_dir():
     config_dir = (
         os.getenv("APPDATA")
         if os.name == "nt"
         else os.path.join(os.path.expanduser("~"), ".config")
```

### Comparing `mindflow-0.5.3/mindflow/core/types/store_traits/pinecone.py` & `mindflow-0.5.4/mindflow/core/types/store_traits/pinecone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
-from typing import List, Tuple, Type, TypeVar, Union
-from typing import Optional
 import numpy as np
-
 import pinecone  # type: ignore
+
+from typing import List, Tuple, Type, TypeVar, Union, Optional
+
 from mindflow.core.settings import Settings
 
 
 def return_values_as_dict(values: List[dict]) -> dict:
     return {value["name"]: value["value"] for value in values}
 
 
@@ -119,21 +119,21 @@
     async def save_bulk(cls, objects: List[T]):
         vectors = [object._convert_object_to_pinecone_format() for object in objects]
         pinecone_db.get_index(cls.__name__).upsert(vectors=vectors)
 
     @classmethod
     async def query(
         cls: Type[T],
-        vector: np.ndarray,
+        vector: List[float],
         ids: List[str],
         top_k=100,
         include_metadata=True,
     ) -> List[T]:
         results = pinecone_db.get_index(cls.__name__).query(
-            vector=vector.tolist(),
+            vector=vector,
             filter={"id": {"$in": ids}},
             top_k=top_k,
             include_metadata=include_metadata,
         )
         return [
             cls(cls._convert_pinecone_format_to_object_format(result))
             for result in results["matches"]
```

### Comparing `mindflow-0.5.3/mindflow/core/types/store_traits/static.py` & `mindflow-0.5.4/mindflow/core/types/store_traits/static.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Type, TypeVar, Union
+
 from mindflow.core.types import Collection
 from mindflow.core.types.definitions.mind_flow_model import (
     MINDFLOW_MODEL_STATIC,
 )
 from mindflow.core.types.definitions.model import MODEL_STATIC
 from mindflow.core.types.definitions.service import SERVICE_STATIC
```

### Comparing `mindflow-0.5.3/mindflow/unit_tests/dummy_diff.txt` & `mindflow-0.5.4/mindflow/unit_tests/dummy_diff.txt`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.3/mindflow/unit_tests/test_utils.py` & `mindflow-0.5.4/mindflow/unit_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.3/mindflow.egg-info/PKG-INFO` & `mindflow-0.5.4/mindflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindflow
-Version: 0.5.3
+Version: 0.5.4
 Summary: AI-powered search engine for your code!
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # :brain: mindflow :ocean:
 The [ChatGPT](https://openai.com/blog/chatgpt)-powered swiss army knife for the modern developer! We provide an AI-powered CLI git wrapper, boilerplate code generator, code search engine, a conversation history manager, and much more!
 
@@ -23,20 +23,20 @@
 1. Follow us on [Twitter](https://twitter.com/mindflow_ai)
 2. Join our [discord](https://discord.com/invite/P2cQACzB)
 3. BONUS: Consider [becoming a patron](https://www.patreon.com/MindFlowAI) :heart:
 
 ## Getting Started
 
 Pre-requisite: 
-- You'll need to create an [OpenAI](https://openai.com/blog/openai-api) account or request early access from [Anthropic](https://www.anthropic.com/earlyaccess).
+- You'll need to create an [OpenAI](https://openai.com/blog/openai-api) account.
 - Also, create a [Pinecone](https://www.pinecone.io/start) account to use their vector database.
 
 1. Run `pip install mindflow`, or you can clone this repo and run `pip install -e path/to/mindflow`.
 2. Run `mf login`:
-    - Register with OpenAI or Anthropic to use their models. You can find your OpenAI API key [here](https://platform.openai.com/account/api-keys).
+    - Register with OpenAI to use their models. You can find your OpenAI API key [here](https://platform.openai.com/account/api-keys).
     - Register with Pinecone to use their vector database. You can find your Pinecone API key and Environment [here](https://www.pinecone.io/start).
 3. Now, you're ready to start using MindFlow!
 
 ## Basic Usage
 
 ### Configuration (Optional)
 Configure the model used for generating responses by running `mf config` and selecting either GPT 3.5 Turbo (default) or GPT 4. In order to use GPT 4, you'll need to have special access to the API. If you have access, you can run `mf config` and select GPT 4. If you don't have access, you'll get an error message. 
@@ -45,22 +45,22 @@
 ### Chats
 There are multiple levels to using mindflow's chat feature.
 
 1. Simplest
 - `mf chat "explain what a programming language is"`
     - Interact with chatGPT directly just like on the chatGPT website. We also have chat persistence, so it will remember the previous chat messages.
 2. With File Context
-- `mf chat "please summarize what this code does" path/to/code.py`
+- `mf chat path/to/code.py "please summarize what this code does"`
     - You can provide single or multi-file context to chatGPT by passing in any number of files as a separate argument in the `mf chat` call. For sufficiently small files (see: [chatGPT token limits](https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them)), this will work and also maintain chat history.
 3. With Directory Context
-- `mf chat "what are these submodules responsible for? path/to/submodule1/ path/to/submodule2/`
+- `mf chat path/to/submodule1/ path/to/submodule2/ "what are these submodules responsible for?"`
     - Providing directories will actually run an indexer over your code subdirectories/files recursively. So it may take a while to fully index everything -- don't worry; we'll warn you if the cost becomes a concern! Right now the warning triggers if the index job costs >$0.50USD.
 4. Custom pre-indexed context
 - `mf index path/to/subdir/file1.txt path/to/file2.txt`
-- `mf chat -s "How do all of my classes relate to one another?" ./`
+- `mf chat -s ./ "How do all of my classes relate to one another?"`
     - If you pre-index your repository, you can narrow the scope for the context provided to the chat. Passing `-s` will skip the auto-indexing, and instead will defer to the currently existing index. This index is generated in the first step `mf index` where only those files/subdirs will be included.
     - This can save you time and money if your repository is significantly large.
 
 ### Code Generator
 You can use mindflow to generate boilerplate code in an instant using `mf gen`! It should only generate code and comments, and will save the file in the path given.
 
 Here's a couple examples:
@@ -121,11 +121,11 @@
 ### Generating a setup.py
 ![Screenshot 2023-03-11 at 8 39 47 PM](https://user-images.githubusercontent.com/26421036/224524762-e80f134b-5fc6-4f9f-af4e-d858549ccff8.png)
 
 ### Generating an arbitrary program file
 ![Screenshot 2023-03-11 at 8 42 11 PM](https://user-images.githubusercontent.com/26421036/224524839-45093b5d-b4d9-4dc4-a129-867d819a2136.png)
 
 ## How does it work?
-This tool allows you to build an index of text documents and search through them using GPT-based embeddings. The tool takes document paths as input, extracts the text, splits the documents into chunks, summarizes them, and builds a summarization tree. The tool then uses this tree to generate embeddings of the indexed documents and your query and selects the top text chunks based on the cosine similarity between these embeddings. The generated index can be saved to a JSON file for later reuse, making subsequent searches faster and cheaper.
+MindFlow uses state-of-the-art methods for high-throughput segmentation, processing, storage, and retrieval of documents using a recursive hierarchical summarization and embedding technique to store embedding vectors for document chunks and then achieve fast, and high-quality responses to questions and tasks by appending similar document chunks based on the hierarchically embedded text and using them as context for you query. Additionally, chat history will persist if it can fit in the context for queries over indexed documents or for regular chat.
 
 ## What's next for MindFlow
 In the future, MindFlow plans on becoming an even more integral part of the modern developer's toolkit. We plan on adding the ability to ditch traditional documentation and instead integrate directly with your private documents and communication channels, allowing for a more seamless and intuitive experience. With MindFlow, you can have a true "stream of consciousness" with your code, documentation, and communication channels, making it easier than ever to stay on top of your projects and collaborate with your team. We are excited to continue pushing the boundaries of what's possible with language models and revolutionizing how developers work.
```

### Comparing `mindflow-0.5.3/mindflow.egg-info/SOURCES.txt` & `mindflow-0.5.4/mindflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,18 +29,15 @@
 mindflow/cli/commands/git/add.py
 mindflow/cli/commands/git/commit.py
 mindflow/cli/commands/git/diff.py
 mindflow/cli/commands/git/mr.py
 mindflow/cli/commands/git/pr.py
 mindflow/cli/commands/git/push.py
 mindflow/core/__init__.py
-mindflow/core/command_parse.py
 mindflow/core/constants.py
-mindflow/core/errors.py
-mindflow/core/execute.py
 mindflow/core/prompt_builders.py
 mindflow/core/prompts.py
 mindflow/core/settings.py
 mindflow/core/token_counting.py
 mindflow/core/commands/__init__.py
 mindflow/core/commands/chat.py
 mindflow/core/commands/delete.py
```

### Comparing `mindflow-0.5.3/setup.py` & `mindflow-0.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import find_packages, setup
+from setuptools import find_packages, setup  # type: ignore
 
 # get version from mindflow/__init__.py
 with open("mindflow/__init__.py", "r") as f:
     for line in f:
         if line.startswith("__version__"):
             version = line.split("=")[1].strip().strip('"')
             break
```

