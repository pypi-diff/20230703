# Comparing `tmp/cici-tools-0.2.4.tar.gz` & `tmp/cici-tools-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cici-tools-0.2.4.tar", last modified: Thu Jun 22 06:23:12 2023, max compression
+gzip compressed data, was "cici-tools-0.2.5.tar", last modified: Sun Jul  2 22:15:39 2023, max compression
```

## Comparing `cici-tools-0.2.4.tar` & `cici-tools-0.2.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:23:12.765753 cici-tools-0.2.4/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-22 06:23:10.000000 cici-tools-0.2.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-22 06:23:10.000000 cici-tools-0.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2689 2023-06-22 06:23:12.765753 cici-tools-0.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1856 2023-06-22 06:23:10.000000 cici-tools-0.2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:23:12.760753 cici-tools-0.2.4/cici/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/__main__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:23:12.761753 cici-tools-0.2.4/cici/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1510 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/cli/build.py
--rwxrwxrwx   0 root         (0) root         (0)     3073 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/cli/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/cli/fmt.py
--rw-rw-rw-   0 root         (0) root         (0)     3140 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/cli/update.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:23:12.762753 cici-tools-0.2.4/cici/providers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:23:12.763753 cici-tools-0.2.4/cici/providers/gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/providers/gitlab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/providers/gitlab/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     5760 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/providers/gitlab/converter.py
--rw-rw-rw-   0 root         (0) root         (0)     6415 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/providers/gitlab/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3091 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/providers/gitlab/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/providers/gitlab/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:23:12.763753 cici-tools-0.2.4/cici/schema/
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/schema/LICENSE.gitlab
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    70638 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/schema/gitlab-ci.json
--rw-rw-rw-   0 root         (0) root         (0)     1829 2023-06-22 06:23:10.000000 cici-tools-0.2.4/cici/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 06:23:12.765753 cici-tools-0.2.4/cici_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2689 2023-06-22 06:23:12.000000 cici-tools-0.2.4/cici_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-22 06:23:12.000000 cici-tools-0.2.4/cici_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 06:23:12.000000 cici-tools-0.2.4/cici_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-06-22 06:23:12.000000 cici-tools-0.2.4/cici_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-22 06:23:12.000000 cici-tools-0.2.4/cici_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-22 06:23:12.000000 cici-tools-0.2.4/cici_tools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-22 06:23:12.765753 cici-tools-0.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1360 2023-06-22 06:23:10.000000 cici-tools-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 22:15:39.244760 cici-tools-0.2.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-02 22:15:36.000000 cici-tools-0.2.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-02 22:15:36.000000 cici-tools-0.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-07-02 22:15:39.244760 cici-tools-0.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1856 2023-07-02 22:15:36.000000 cici-tools-0.2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 22:15:39.240760 cici-tools-0.2.5/cici/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 22:15:39.241760 cici-tools-0.2.5/cici/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/cli/_build.py
+-rwxrwxrwx   0 root         (0) root         (0)     3088 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/cli/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/cli/fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/cli/update.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 22:15:39.241760 cici-tools-0.2.5/cici/providers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 22:15:39.242760 cici-tools-0.2.5/cici/providers/gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/providers/gitlab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/providers/gitlab/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     5760 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/providers/gitlab/converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6415 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/providers/gitlab/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3091 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/providers/gitlab/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/providers/gitlab/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 22:15:39.243760 cici-tools-0.2.5/cici/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/schema/LICENSE.gitlab
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    70638 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/schema/gitlab-ci.json
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2023-07-02 22:15:36.000000 cici-tools-0.2.5/cici/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 22:15:39.244760 cici-tools-0.2.5/cici_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-07-02 22:15:39.000000 cici-tools-0.2.5/cici_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      753 2023-07-02 22:15:39.000000 cici-tools-0.2.5/cici_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 22:15:39.000000 cici-tools-0.2.5/cici_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-02 22:15:39.000000 cici-tools-0.2.5/cici_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-02 22:15:39.000000 cici-tools-0.2.5/cici_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-02 22:15:39.000000 cici-tools-0.2.5/cici_tools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-02 22:15:39.245760 cici-tools-0.2.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1360 2023-07-02 22:15:36.000000 cici-tools-0.2.5/setup.py
```

### Comparing `cici-tools-0.2.4/LICENSE` & `cici-tools-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.4/PKG-INFO` & `cici-tools-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cici-tools
-Version: 0.2.4
+Version: 0.2.5
 Summary: Power tools for CI/CD.
 Home-page: https://gitlab.com/brettops/tools/cici
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: ci pipeline python
 Platform: UNKNOWN
```

### Comparing `cici-tools-0.2.4/README.md` & `cici-tools-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.4/cici/cli/build.py` & `cici-tools-0.2.5/cici/cli/_build.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.4/cici/cli/bundle.py` & `cici-tools-0.2.5/cici/cli/bundle.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         with open(bundle_filename, "w") as stream:
             provider.dump(bundle, stream)
         print(colored("created", "magenta"), bundle_filename.name)
 
 
 def bundle_parser(subparsers):
     parser = subparsers.add_parser(
-        "bundle", help="distill a CI file to a job and its dependencies"
+        "bundle", help="bundle CI jobs with dependencies into standalone distributions"
     )
     parser.add_argument(
         "config_path",
         metavar="DIR",
         nargs="?",
         type=Path,
         default=(Path.cwd() / CONFIG_DIR_NAME).absolute(),
```

### Comparing `cici-tools-0.2.4/cici/cli/fmt.py` & `cici-tools-0.2.5/cici/cli/fmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,11 +20,11 @@
         file = provider.load(filename)
         with open(filename, "w") as stream:
             provider.dump(file, stream)
         print(colored(filename, "magenta"), "formatted")
 
 
 def fmt_parser(subparsers):
-    parser = subparsers.add_parser("fmt", help="Reformat CI file")
+    parser = subparsers.add_parser("fmt", help="format CI files")
     parser.add_argument("filenames", metavar="FILE", nargs="*")
     parser.set_defaults(func=fmt_command)
     return parser
```

### Comparing `cici-tools-0.2.4/cici/cli/update.py` & `cici-tools-0.2.5/cici/cli/update.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,11 +102,13 @@
 
     with open(args.filename, "w") as handle:
         yaml.indent(mapping=2, sequence=4, offset=2)
         yaml.dump(data, handle)
 
 
 def update_parser(subparsers):
-    parser = subparsers.add_parser("update")
+    parser = subparsers.add_parser(
+        "update", help="pin CI includes to the latest versions"
+    )
     parser.add_argument("filename", nargs="?", default=".gitlab-ci.yml")
     parser.set_defaults(func=update_command)
     return parser
```

### Comparing `cici-tools-0.2.4/cici/constants.py` & `cici-tools-0.2.5/cici/constants.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.4/cici/providers/gitlab/constants.py` & `cici-tools-0.2.5/cici/providers/gitlab/constants.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.4/cici/providers/gitlab/converter.py` & `cici-tools-0.2.5/cici/providers/gitlab/converter.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.4/cici/providers/gitlab/models.py` & `cici-tools-0.2.5/cici/providers/gitlab/models.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.4/cici/providers/gitlab/serializers.py` & `cici-tools-0.2.5/cici/providers/gitlab/serializers.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.4/cici/providers/gitlab/utils.py` & `cici-tools-0.2.5/cici/providers/gitlab/utils.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.4/cici/schema/LICENSE.gitlab` & `cici-tools-0.2.5/cici/schema/LICENSE.gitlab`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.4/cici/schema/gitlab-ci.json` & `cici-tools-0.2.5/cici/schema/gitlab-ci.json`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.4/cici/utils.py` & `cici-tools-0.2.5/cici/utils.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.4/cici_tools.egg-info/PKG-INFO` & `cici-tools-0.2.5/cici_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cici-tools
-Version: 0.2.4
+Version: 0.2.5
 Summary: Power tools for CI/CD.
 Home-page: https://gitlab.com/brettops/tools/cici
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: ci pipeline python
 Platform: UNKNOWN
```

### Comparing `cici-tools-0.2.4/cici_tools.egg-info/SOURCES.txt` & `cici-tools-0.2.5/cici_tools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 cici/__init__.py
 cici/__main__.py
 cici/_version.py
 cici/constants.py
 cici/main.py
 cici/utils.py
 cici/cli/__init__.py
-cici/cli/build.py
+cici/cli/_build.py
 cici/cli/bundle.py
 cici/cli/fmt.py
 cici/cli/update.py
 cici/providers/__init__.py
 cici/providers/gitlab/__init__.py
 cici/providers/gitlab/constants.py
 cici/providers/gitlab/converter.py
```

### Comparing `cici-tools-0.2.4/setup.py` & `cici-tools-0.2.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
```

