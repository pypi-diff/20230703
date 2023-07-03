# Comparing `tmp/opendr-toolkit-ambiguity-measure-2.1.0.tar.gz` & `tmp/opendr-toolkit-ambiguity-measure-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendr-toolkit-ambiguity-measure-2.1.0.tar", last modified: Wed Feb 22 08:10:32 2023, max compression
+gzip compressed data, was "opendr-toolkit-ambiguity-measure-2.2.0.tar", last modified: Mon Jul  3 13:34:55 2023, max compression
```

## Comparing `opendr-toolkit-ambiguity-measure-2.1.0.tar` & `opendr-toolkit-ambiguity-measure-2.2.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:32.955868 opendr-toolkit-ambiguity-measure-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/Dockerfile-cuda
--rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/Dockerfile-embedded
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-02-22 08:10:32.000000 opendr-toolkit-ambiguity-measure-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-02-22 08:10:32.955868 opendr-toolkit-ambiguity-measure-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/description.txt
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-02-22 08:10:02.000000 opendr-toolkit-ambiguity-measure-2.1.0/packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-22 08:10:32.955868 opendr-toolkit-ambiguity-measure-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-02-22 08:10:32.000000 opendr-toolkit-ambiguity-measure-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:32.951868 opendr-toolkit-ambiguity-measure-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:32.955868 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:32.955868 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/control/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:32.955868 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/engine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/engine/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/engine/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/engine/example_learner.py
--rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/engine/learners.py
--rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/engine/target.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:32.955868 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/perception/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/perception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:32.955868 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/planning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:32.955868 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/simulation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:32.955868 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:32.955868 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/utils/ambiguity_measure/
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/utils/ambiguity_measure/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/utils/ambiguity_measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6684 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/utils/ambiguity_measure/ambiguity_measure.py
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/utils/ambiguity_measure/dependencies.ini
--rw-r--r--   0 runner    (1001) docker     (122)     4651 2023-02-22 08:10:03.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/utils/ambiguity_measure/persistence.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-22 08:10:32.955868 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr_toolkit_ambiguity_measure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-02-22 08:10:32.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr_toolkit_ambiguity_measure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-02-22 08:10:32.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr_toolkit_ambiguity_measure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-22 08:10:32.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr_toolkit_ambiguity_measure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-02-22 08:10:32.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr_toolkit_ambiguity_measure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-02-22 08:10:32.000000 opendr-toolkit-ambiguity-measure-2.1.0/src/opendr_toolkit_ambiguity_measure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:55.198943 opendr-toolkit-ambiguity-measure-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/Dockerfile-cuda
+-rw-r--r--   0 runner    (1001) docker     (122)     6871 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/Dockerfile-embedded
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-07-03 13:34:55.000000 opendr-toolkit-ambiguity-measure-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-07-03 13:34:55.198943 opendr-toolkit-ambiguity-measure-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/description.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-03 13:34:25.000000 opendr-toolkit-ambiguity-measure-2.2.0/packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 13:34:55.198943 opendr-toolkit-ambiguity-measure-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-03 13:34:54.000000 opendr-toolkit-ambiguity-measure-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:55.194943 opendr-toolkit-ambiguity-measure-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:55.198943 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:55.198943 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/control/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/control/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:55.198943 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/engine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/engine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21773 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/engine/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3923 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/engine/example_learner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23609 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/engine/learners.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34699 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/engine/target.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:55.198943 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/perception/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/perception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:55.198943 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/planning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:55.198943 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/simulation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:55.198943 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:55.198943 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/utils/ambiguity_measure/
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/utils/ambiguity_measure/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/utils/ambiguity_measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6684 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/utils/ambiguity_measure/ambiguity_measure.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/utils/ambiguity_measure/dependencies.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     4651 2023-07-03 13:34:26.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/utils/ambiguity_measure/persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:34:55.198943 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr_toolkit_ambiguity_measure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-07-03 13:34:55.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr_toolkit_ambiguity_measure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-07-03 13:34:55.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr_toolkit_ambiguity_measure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:34:55.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr_toolkit_ambiguity_measure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-03 13:34:55.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr_toolkit_ambiguity_measure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-03 13:34:55.000000 opendr-toolkit-ambiguity-measure-2.2.0/src/opendr_toolkit_ambiguity_measure.egg-info/top_level.txt
```

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/.clang-format` & `opendr-toolkit-ambiguity-measure-2.2.0/.clang-format`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/.gitignore` & `opendr-toolkit-ambiguity-measure-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/CHANGELOG.md` & `opendr-toolkit-ambiguity-measure-2.2.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # OpenDR Toolkit Change Log
 
+## Version 2.2.0
+Released on July, 3rd, 2023.
+
+  - Dependency Updates ([#431](https://github.com/opendr-eu/opendr/pull/431)):
+    - Updated PyTorch version from 1.9.0 to 1.13.1.
+    - Updated Torchvision version from 0.10.0 to 0.14.1.
+    - Updated Torchaudio version from 0.9.0 to 0.13.1.
+    - Downgraded wheel version to 0.38.4 due to bug in recent version.
+
 ## Version 2.1.0
 Released on February, 22nd, 2023.
 
   - New Features:
-    - Added YOLOv5 as an inference-only tool ([#360](https://github.com/opendr-eu/opendr/pull/360)).
     - Added Efficient LiDAR Panoptic Segmentation ([#359](https://github.com/opendr-eu/opendr/pull/359)).
     - Added Nanodet 2D Object Detection tool ([#352](https://github.com/opendr-eu/opendr/pull/352)).
     - Added C API implementations of NanoDet 2D Object Detection tool ([#352](https://github.com/opendr-eu/opendr/pull/352)).
     - Added C API implementations of forward pass of DETR 2D Object Detection tool ([#383](https://github.com/opendr-eu/opendr/pull/383)).
     - Added C API implementations of forward pass of DeepSORT 2D Object Tracking tool ([#383](https://github.com/opendr-eu/opendr/pull/383)).
     - Added C API implementations of forward pass of Lightweight OpenPose, Pose Estimator tool ([#383](https://github.com/opendr-eu/opendr/pull/383)).
     - Added C API implementations of forward pass of X3D 2D Activity Recognition tool ([#383](https://github.com/opendr-eu/opendr/pull/383)).
```

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/CODE_OF_CONDUCT` & `opendr-toolkit-ambiguity-measure-2.2.0/CODE_OF_CONDUCT`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/Dockerfile` & `opendr-toolkit-ambiguity-measure-2.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/Dockerfile-cuda` & `opendr-toolkit-ambiguity-measure-2.2.0/Dockerfile-cuda`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/Dockerfile-embedded` & `opendr-toolkit-ambiguity-measure-2.2.0/Dockerfile-embedded`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/LICENSE` & `opendr-toolkit-ambiguity-measure-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/Makefile` & `opendr-toolkit-ambiguity-measure-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/PKG-INFO` & `opendr-toolkit-ambiguity-measure-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-ambiguity-measure
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: utils/ambiguity_measure)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/README.md` & `opendr-toolkit-ambiguity-measure-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/description.txt` & `opendr-toolkit-ambiguity-measure-2.2.0/description.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/packages.txt` & `opendr-toolkit-ambiguity-measure-2.2.0/packages.txt`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/_setup.py` & `opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/_setup.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/_version.py` & `opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/engine/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "2.1.0"
+OPENDR_SERVER_URL = "ftp://opendrdata.csd.auth.gr/"
```

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/engine/constants.py` & `opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/_version.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-OPENDR_SERVER_URL = "ftp://opendrdata.csd.auth.gr/"
+__version__ = "2.2.0"
```

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/engine/data.py` & `opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/engine/data.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/engine/datasets.py` & `opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/engine/datasets.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/engine/example_learner.py` & `opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/engine/example_learner.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/engine/learners.py` & `opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/engine/learners.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/engine/target.py` & `opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/engine/target.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/utils/ambiguity_measure/README.md` & `opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/utils/ambiguity_measure/README.md`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/utils/ambiguity_measure/ambiguity_measure.py` & `opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/utils/ambiguity_measure/ambiguity_measure.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/src/opendr/utils/ambiguity_measure/persistence.py` & `opendr-toolkit-ambiguity-measure-2.2.0/src/opendr/utils/ambiguity_measure/persistence.py`

 * *Files identical despite different names*

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/src/opendr_toolkit_ambiguity_measure.egg-info/PKG-INFO` & `opendr-toolkit-ambiguity-measure-2.2.0/src/opendr_toolkit_ambiguity_measure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: opendr-toolkit-ambiguity-measure
-Version: 2.1.0
+Version: 2.2.0
 Summary: Open Deep Learning Toolkit for Robotics (submodule: utils/ambiguity_measure)
 Home-page: https://github.com/opendr-eu/opendr
 Author: OpenDR consortium
 Author-email: tefas@csd.auth.gr
 License: LICENSE
 Description: The aim of OpenDR is to develop a modular, open and non-proprietary toolkit for core robotic functionalities by harnessing deep learning to provide advanced perception and cognition capabilities, meeting in this way the general requirements of robotics applications in the applications areas of healthcare, agri-food and agile production. The term toolkit in OpenDR refers to a set of deep learning software functions, packages and utilities used to help roboticists to develop and test a robotic application that incorporates deep learning. OpenDR will provide the means to link the robotics applications to software libraries (deep learning frameworks, e.g., Tensorflow) and to link it with the operating environment (ROS). OpenDR focuses on the AI and Cognition core technology in order to provide tools that make robotic systems cognitive, giving them the ability to a) interact with people and environments by developing deep learning methods for human centric and environment active perception and cognition, b) learn and categorise by developing deep learning tools for training and inference in common robotics settings, and c) make decisions and derive knowledge by developing deep learning tools for cognitive robot action and decision making (WP5). As a result, the developed OpenDR toolkit will also enable cooperative human-robot interaction as well as the development of cognitive mechatronics where sensing and actuation are closely coupled with cognitive systems thus contributing to another two core technologies beyond AI and Cognition. OpenDR will develop, train, deploy and evaluate deep learning models that improve the technical capabilities of the core technologies beyond the current state of the art. It will enable a greater range of robotics applications that can be demonstrated at TRL 3 and above, thus lowering the technical barriers within the prioritised application areas. OpenDR aims to an easily adopted methodology to adapt the provided tools in order to solve any robotics task without restricting it to any specific application.
 Platform: UNKNOWN
```

### Comparing `opendr-toolkit-ambiguity-measure-2.1.0/src/opendr_toolkit_ambiguity_measure.egg-info/SOURCES.txt` & `opendr-toolkit-ambiguity-measure-2.2.0/src/opendr_toolkit_ambiguity_measure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

