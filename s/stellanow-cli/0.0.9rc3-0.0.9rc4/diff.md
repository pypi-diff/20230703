# Comparing `tmp/stellanow_cli-0.0.9rc3.tar.gz` & `tmp/stellanow_cli-0.0.9rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellanow_cli-0.0.9rc3.tar", last modified: Fri Jun 30 13:18:27 2023, max compression
+gzip compressed data, was "stellanow_cli-0.0.9rc4.tar", last modified: Mon Jul  3 20:20:51 2023, max compression
```

## Comparing `stellanow_cli-0.0.9rc3.tar` & `stellanow_cli-0.0.9rc4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.324788 stellanow_cli-0.0.9rc3/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       98 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/MANIFEST.in
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     8331 2023-06-30 13:18:27.324207 stellanow_cli-0.0.9rc3/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      225 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/Pipfile
--rw-r--r--   0 tom-kandziora   (501) staff       (20)    10889 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/README.md
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     8154 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/README.public
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-30 13:18:27.324874 stellanow_cli-0.0.9rc3/setup.cfg
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2284 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/setup.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.223629 stellanow_cli-0.0.9rc3/stellanow_cli/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.265027 stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1277 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1348 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/_run.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1307 2023-06-30 12:14:52.000000 stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/_version.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2100 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/cli.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1173 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/_run.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1117 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/_version.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.268261 stellanow_cli-0.0.9rc3/stellanow_cli/api/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1231 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/api/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.271755 stellanow_cli-0.0.9rc3/stellanow_cli/api/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1453 2023-06-29 22:10:25.000000 stellanow_cli-0.0.9rc3/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2272 2023-06-29 23:05:14.000000 stellanow_cli-0.0.9rc3/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5618 2023-06-30 10:39:47.000000 stellanow_cli-0.0.9rc3/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1537 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/api/datatypes.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     6564 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/api/stellanow_api.py
--rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     2058 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/cli.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.274985 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1146 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.279881 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1363 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2580 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     7205 2023-06-30 10:44:58.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2226 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/code_generator.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     6680 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/csharp_code_generator.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.282647 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/templates/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-10 10:14:46.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/templates/.footer.template
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      126 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/templates/.header.template
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      544 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/templates/csharp.template
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.288596 stellanow_cli-0.0.9rc3/stellanow_cli/commands/
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.297241 stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4538 2023-06-27 15:44:57.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3735 2023-06-30 12:21:54.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2135 2023-06-30 12:21:55.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/events.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5197 2023-06-30 12:19:26.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4617 2023-06-30 12:14:51.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/_init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4934 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/command_config.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4617 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/configure.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2005 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/events.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5246 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/generate.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5253 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/commands/plan.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.300490 stellanow_cli-0.0.9rc3/stellanow_cli/config/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1276 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.303453 stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1705 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2193 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1622 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/dev.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1618 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/int.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1612 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/config.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1246 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/dev.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1242 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/config/int.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.305559 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.308077 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1288 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3146 2023-06-30 10:39:47.000000 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__pycache__/api_exceptions.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3170 2023-06-30 10:39:47.000000 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__pycache__/cli_exceptions.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2201 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/api_exceptions.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2163 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/cli_exceptions.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.310624 stellanow_cli-0.0.9rc3/stellanow_cli/utils/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/utils/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.317469 stellanow_cli-0.0.9rc3/stellanow_cli/utils/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1283 2023-06-27 15:44:10.000000 stellanow_cli-0.0.9rc3/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1693 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc3/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2908 2023-06-27 15:44:40.000000 stellanow_cli-0.0.9rc3/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1631 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/utils/logger.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2240 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/stellanow_cli/utils/utils.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.252151 stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     8331 2023-06-30 13:18:26.000000 stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2958 2023-06-30 13:18:26.000000 stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-30 13:18:26.000000 stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-30 13:18:26.000000 stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/entry_points.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-30 13:18:26.000000 stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/requires.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-30 13:18:26.000000 stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/top_level.txt
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.319203 stellanow_cli-0.0.9rc3/tests/
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-30 13:18:27.323525 stellanow_cli-0.0.9rc3/tests/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2940 2023-06-30 10:44:58.000000 stellanow_cli-0.0.9rc3/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2853 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/tests/test_command_configure.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3313 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc3/tests/test_generate_class_handles_all_valueTypes.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.028105 stellanow_cli-0.0.9rc4/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       98 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/MANIFEST.in
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     8331 2023-07-03 20:20:51.027645 stellanow_cli-0.0.9rc4/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      225 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/Pipfile
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)    10889 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/README.md
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     8154 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/README.public
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-07-03 20:20:51.028188 stellanow_cli-0.0.9rc4/setup.cfg
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2284 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/setup.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:50.949078 stellanow_cli-0.0.9rc4/stellanow_cli/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:50.996114 stellanow_cli-0.0.9rc4/stellanow_cli/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1277 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc4/stellanow_cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1348 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc4/stellanow_cli/__pycache__/_run.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1307 2023-06-30 12:14:52.000000 stellanow_cli-0.0.9rc4/stellanow_cli/__pycache__/_version.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2100 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc4/stellanow_cli/__pycache__/cli.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1173 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/_run.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1117 2023-07-03 20:20:48.000000 stellanow_cli-0.0.9rc4/stellanow_cli/_version.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:50.998091 stellanow_cli-0.0.9rc4/stellanow_cli/api/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1231 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/api/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.001413 stellanow_cli-0.0.9rc4/stellanow_cli/api/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1453 2023-06-29 22:10:25.000000 stellanow_cli-0.0.9rc4/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2272 2023-06-29 23:05:14.000000 stellanow_cli-0.0.9rc4/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5618 2023-06-30 10:39:47.000000 stellanow_cli-0.0.9rc4/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1537 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/api/datatypes.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     6564 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/api/stellanow_api.py
+-rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     2058 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/cli.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.003453 stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1146 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.005222 stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1363 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2580 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7205 2023-06-30 10:44:58.000000 stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2226 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/code_generator.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     6687 2023-06-30 13:57:57.000000 stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/csharp_code_generator.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.006936 stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/templates/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-10 10:14:46.000000 stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/templates/.footer.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      126 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/templates/.header.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      544 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/templates/csharp.template
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.010398 stellanow_cli-0.0.9rc4/stellanow_cli/commands/
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.013873 stellanow_cli-0.0.9rc4/stellanow_cli/commands/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4538 2023-06-27 15:44:57.000000 stellanow_cli-0.0.9rc4/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3735 2023-06-30 12:21:54.000000 stellanow_cli-0.0.9rc4/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2135 2023-06-30 12:21:55.000000 stellanow_cli-0.0.9rc4/stellanow_cli/commands/__pycache__/events.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5197 2023-06-30 12:19:26.000000 stellanow_cli-0.0.9rc4/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4617 2023-06-30 12:14:51.000000 stellanow_cli-0.0.9rc4/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/commands/_init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4934 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/commands/command_config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4617 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/commands/configure.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2005 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/commands/events.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5246 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/commands/generate.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5253 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/commands/plan.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.016192 stellanow_cli-0.0.9rc4/stellanow_cli/config/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1276 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/config/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.018219 stellanow_cli-0.0.9rc4/stellanow_cli/config/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1705 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc4/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2193 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc4/stellanow_cli/config/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1622 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc4/stellanow_cli/config/__pycache__/dev.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1618 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc4/stellanow_cli/config/__pycache__/int.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1612 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/config/config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1246 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/config/dev.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1242 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/config/int.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.020217 stellanow_cli-0.0.9rc4/stellanow_cli/exceptions/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/exceptions/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.021895 stellanow_cli-0.0.9rc4/stellanow_cli/exceptions/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1288 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc4/stellanow_cli/exceptions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3146 2023-06-30 10:39:47.000000 stellanow_cli-0.0.9rc4/stellanow_cli/exceptions/__pycache__/api_exceptions.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3170 2023-06-30 10:39:47.000000 stellanow_cli-0.0.9rc4/stellanow_cli/exceptions/__pycache__/cli_exceptions.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2201 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/exceptions/api_exceptions.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2163 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/exceptions/cli_exceptions.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.023599 stellanow_cli-0.0.9rc4/stellanow_cli/utils/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1090 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/utils/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.025405 stellanow_cli-0.0.9rc4/stellanow_cli/utils/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1283 2023-06-27 15:44:10.000000 stellanow_cli-0.0.9rc4/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1693 2023-06-20 14:48:09.000000 stellanow_cli-0.0.9rc4/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2908 2023-06-27 15:44:40.000000 stellanow_cli-0.0.9rc4/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1631 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/utils/logger.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2240 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/stellanow_cli/utils/utils.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:50.993329 stellanow_cli-0.0.9rc4/stellanow_cli.egg-info/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     8331 2023-07-03 20:20:50.000000 stellanow_cli-0.0.9rc4/stellanow_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2958 2023-07-03 20:20:50.000000 stellanow_cli-0.0.9rc4/stellanow_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-07-03 20:20:50.000000 stellanow_cli-0.0.9rc4/stellanow_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-07-03 20:20:50.000000 stellanow_cli-0.0.9rc4/stellanow_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-07-03 20:20:50.000000 stellanow_cli-0.0.9rc4/stellanow_cli.egg-info/requires.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-07-03 20:20:50.000000 stellanow_cli-0.0.9rc4/stellanow_cli.egg-info/top_level.txt
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.026544 stellanow_cli-0.0.9rc4/tests/
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-07-03 20:20:51.027133 stellanow_cli-0.0.9rc4/tests/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2940 2023-06-30 10:44:58.000000 stellanow_cli-0.0.9rc4/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2853 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/tests/test_command_configure.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3313 2023-06-30 12:44:28.000000 stellanow_cli-0.0.9rc4/tests/test_generate_class_handles_all_valueTypes.py
```

### Comparing `stellanow_cli-0.0.9rc3/PKG-INFO` & `stellanow_cli-0.0.9rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellanow_cli
-Version: 0.0.9rc3
+Version: 0.0.9rc4
 Summary: Command-line interface for the StellaNow SDK code generation and comparison tool.
 Requires-Python: >=3.10
 
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
```

### Comparing `stellanow_cli-0.0.9rc3/README.md` & `stellanow_cli-0.0.9rc4/README.md`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/README.public` & `stellanow_cli-0.0.9rc4/README.public`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/setup.py` & `stellanow_cli-0.0.9rc4/setup.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/__init__.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/_run.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/__pycache__/_run.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/_version.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/__pycache__/_version.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/__pycache__/cli.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/__pycache__/cli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/_run.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/_run.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/_version.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 IN THE SOFTWARE.
 """
 
-__version__ = "0.0.9.rc3"
+__version__ = "0.0.9.rc4"
```

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/api/__init__.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/api/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/api/datatypes.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/api/datatypes.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/api/stellanow_api.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/api/stellanow_api.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/cli.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/cli.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__init__.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/code_generator.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/code_generator.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/csharp_code_generator.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/csharp_code_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 def field_format_mapping(value_type: str) -> str:
     mapping = {
         'Decimal': '.ToString("F2", CultureInfo.InvariantCulture)',
         'Integer': '.ToString()',
         'Boolean': '.ToString().ToLower()',
         'String': '',
         'Date': '.ToString("yyyy-MM-dd")',
-        'DateTime': '.ToString("yyyy-MM-ddTHH:mm:ssZ")'
+        'DateTime': '.ToString("yyyy-MM-ddTHH:mm:ss.ffffffZ")'
     }
     return mapping.get(value_type, '')
 
 
 def escape_reserved_words(word: str) -> str:
     reserved_words = [
         "abstract", "as", "base", "bool", "break", "byte", "case", "catch", "char", "checked",
```

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/code_generators/templates/csharp.template` & `stellanow_cli-0.0.9rc4/stellanow_cli/code_generators/templates/csharp.template`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/events.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/commands/__pycache__/events.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/commands/_init__.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/commands/_init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/commands/command_config.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/commands/command_config.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/commands/configure.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/commands/configure.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/commands/events.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/commands/events.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/commands/generate.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/commands/plan.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/commands/plan.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/config/__init__.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/config.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/config/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/dev.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/config/__pycache__/dev.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/config/__pycache__/int.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/config/__pycache__/int.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/config/config.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/config/dev.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/config/dev.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/config/int.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/config/int.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__init__.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/exceptions/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__pycache__/api_exceptions.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/exceptions/__pycache__/api_exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/__pycache__/cli_exceptions.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/exceptions/__pycache__/cli_exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/api_exceptions.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/exceptions/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/exceptions/cli_exceptions.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/exceptions/cli_exceptions.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/utils/__init__.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/utils/logger.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/utils/logger.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli/utils/utils.py` & `stellanow_cli-0.0.9rc4/stellanow_cli/utils/utils.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/PKG-INFO` & `stellanow_cli-0.0.9rc4/stellanow_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellanow-cli
-Version: 0.0.9rc3
+Version: 0.0.9rc4
 Summary: Command-line interface for the StellaNow SDK code generation and comparison tool.
 Requires-Python: >=3.10
 
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
```

### Comparing `stellanow_cli-0.0.9rc3/stellanow_cli.egg-info/SOURCES.txt` & `stellanow_cli-0.0.9rc4/stellanow_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc` & `stellanow_cli-0.0.9rc4/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/tests/test_command_configure.py` & `stellanow_cli-0.0.9rc4/tests/test_command_configure.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.9rc3/tests/test_generate_class_handles_all_valueTypes.py` & `stellanow_cli-0.0.9rc4/tests/test_generate_class_handles_all_valueTypes.py`

 * *Files identical despite different names*

