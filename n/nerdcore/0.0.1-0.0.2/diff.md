# Comparing `tmp/nerdcore-0.0.1.tar.gz` & `tmp/nerdcore-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nerdcore-0.0.1.tar", last modified: Mon Jul  3 20:59:38 2023, max compression
+gzip compressed data, was "nerdcore-0.0.2.tar", last modified: Mon Jul  3 21:24:17 2023, max compression
```

## Comparing `nerdcore-0.0.1.tar` & `nerdcore-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:59:38.000000 nerdcore-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      848 2023-07-03 20:59:38.000000 nerdcore-0.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 20:59:14.000000 nerdcore-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:59:38.000000 nerdcore-0.0.1/nerdcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      848 2023-07-03 20:59:37.000000 nerdcore-0.0.1/nerdcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-07-03 20:59:37.000000 nerdcore-0.0.1/nerdcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 20:59:37.000000 nerdcore-0.0.1/nerdcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-03 20:59:37.000000 nerdcore-0.0.1/nerdcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 20:59:37.000000 nerdcore-0.0.1/nerdcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 20:59:37.000000 nerdcore-0.0.1/nerdcore.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:59:38.000000 nerdcore-0.0.1/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2903 2023-07-03 20:59:14.000000 nerdcore-0.0.1/scripts/nerd
--rw-rw-rw-   0 root         (0) root         (0)     3580 2023-07-03 20:59:14.000000 nerdcore-0.0.1/scripts/nerd-new
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 20:59:38.000000 nerdcore-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1319 2023-07-03 20:59:14.000000 nerdcore-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:24:17.730085 nerdcore-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 21:24:17.730085 nerdcore-0.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 21:23:59.000000 nerdcore-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:24:17.730085 nerdcore-0.0.2/nerdcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-03 21:24:17.000000 nerdcore-0.0.2/nerdcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-07-03 21:24:17.000000 nerdcore-0.0.2/nerdcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 21:24:17.000000 nerdcore-0.0.2/nerdcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-03 21:24:17.000000 nerdcore-0.0.2/nerdcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 21:24:17.000000 nerdcore-0.0.2/nerdcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 21:24:17.000000 nerdcore-0.0.2/nerdcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:24:17.730085 nerdcore-0.0.2/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2905 2023-07-03 21:23:59.000000 nerdcore-0.0.2/scripts/nerd
+-rw-rw-rw-   0 root         (0) root         (0)     3586 2023-07-03 21:23:59.000000 nerdcore-0.0.2/scripts/nerd-new
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 21:24:17.730085 nerdcore-0.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2023-07-03 21:23:59.000000 nerdcore-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nerdcore-0.0.1/scripts/nerd` & `nerdcore-0.0.2/scripts/nerd`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from nerdcore.utils.env.update_env_class import update_env_class
 from nerdcore.utils.nerd.find_entity import find_entity
 from nerdcore.utils.nerd.generate_nerd_configs import generate_nerd_configs
 from nerdcore.utils.nerd.parse_nerd_args import parse_nerd_args
 from nerdcore.utils.nerd.run_entities import run_deployment, run_command
 from nerdcore.utils.nerd.theme_functions import print_t
 from nerdcore.utils.nerd_config.update_nerd_config_class import update_nerd_config_class
-from defs import nl, PYTHON_COMMAND
+from ..defs import nl, PYTHON_COMMAND
 
 
 # Some basic environment checks
 nerd_env_checks()
 
 # Regenerate "magic" config/env stuff
 update_env_class()
```

### Comparing `nerdcore-0.0.1/scripts/nerd-new` & `nerdcore-0.0.2/scripts/nerd-new`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 import os
 import shutil
 import sys
 
 from termcolor import colored
 
-from ncdefs import (NC_ENV_DEFAULT_PATH, NC_NERD_MANIFEST_DEFAULT_PATH, NC_NERD_CONFIG_DEFAULTS_DEFAULT_PATH,
-                    NC_THEME_CONFIG_PATH, NC_ENV_CLASS_PATH, NC_NERD_CONFIG_CLASS_PATH, NC_DEFAULT_DEPLOYMENT_PATH,
-                    NC_GITIGNORE_DEFAULT_PATH, NC_README_DEFAULT_PATH, NC_CONTEXT_FILE_EXAMPLE_PATH)
+from ..ncdefs import (NC_ENV_DEFAULT_PATH, NC_NERD_MANIFEST_DEFAULT_PATH, NC_NERD_CONFIG_DEFAULTS_DEFAULT_PATH,
+                      NC_THEME_CONFIG_PATH, NC_ENV_CLASS_PATH, NC_NERD_CONFIG_CLASS_PATH, NC_DEFAULT_DEPLOYMENT_PATH,
+                      NC_GITIGNORE_DEFAULT_PATH, NC_README_DEFAULT_PATH, NC_CONTEXT_FILE_EXAMPLE_PATH)
 
 top_level_dirs = [
     'abilities',
     'deployments',
     'commands',
     'config',
     'tasks',
```

### Comparing `nerdcore-0.0.1/setup.py` & `nerdcore-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nerdcore',
-    version='0.0.1',
+    version='0.0.2',
     __description__="Nerd CLI is a Fivable-specific and highly configurable CLI tool for creating/running deployments, " \
                     "commands, and more.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/fivable/nerd-cli.git',
     author='David Wallace Cooley Jr',
     author_email='david@fivable.com',
```

