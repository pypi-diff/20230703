# Comparing `tmp/wpdetect-1.4.7.tar.gz` & `tmp/wpdetect-1.4.8.tar.gz`

## Comparing `wpdetect-1.4.7.tar` & `wpdetect-1.4.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 wpdetect-1.4.7/CHANGELOG.md
--rw-r--r--   0        0        0     5224 2020-02-02 00:00:00.000000 wpdetect-1.4.7/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 wpdetect-1.4.7/CONTRIBUTING.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 wpdetect-1.4.7/SECURITY.md
--rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 wpdetect-1.4.7/generate-changelog.sh
--rwxr-xr-x   0        0        0     1033 2020-02-02 00:00:00.000000 wpdetect-1.4.7/release-tag.sh
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 wpdetect-1.4.7/requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.7/sample_urls.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 wpdetect-1.4.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 wpdetect-1.4.7/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wpdetect-1.4.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.7/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.7/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.4.7/.vscode/settings.json
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 wpdetect-1.4.7/utils/bump_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.7/wpdetect/__init__.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 wpdetect-1.4.7/wpdetect/__main__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.7/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.7/LICENSE.txt
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 wpdetect-1.4.7/README.md
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 wpdetect-1.4.7/pyproject.toml
--rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 wpdetect-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0    15828 2020-02-02 00:00:00.000000 wpdetect-1.4.8/CHANGELOG.md
+-rw-r--r--   0        0        0     5224 2020-02-02 00:00:00.000000 wpdetect-1.4.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 wpdetect-1.4.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 wpdetect-1.4.8/SECURITY.md
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 wpdetect-1.4.8/generate-changelog.sh
+-rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 wpdetect-1.4.8/install-local.sh
+-rwxr-xr-x   0        0        0     1089 2020-02-02 00:00:00.000000 wpdetect-1.4.8/release-tag.sh
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 wpdetect-1.4.8/requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.8/sample_urls.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 wpdetect-1.4.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 wpdetect-1.4.8/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wpdetect-1.4.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.8/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.8/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 wpdetect-1.4.8/.vscode/settings.json
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 wpdetect-1.4.8/utils/bump_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.8/wpdetect/__init__.py
+-rw-r--r--   0        0        0     7535 2020-02-02 00:00:00.000000 wpdetect-1.4.8/wpdetect/__main__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.8/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.8/LICENSE.txt
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 wpdetect-1.4.8/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 wpdetect-1.4.8/pyproject.toml
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 wpdetect-1.4.8/PKG-INFO
```

### Comparing `wpdetect-1.4.7/CODE_OF_CONDUCT.md` & `wpdetect-1.4.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.7/CONTRIBUTING.md` & `wpdetect-1.4.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.7/release-tag.sh` & `wpdetect-1.4.8/release-tag.sh`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #!/bin/sh
 
+# This script is used to tag a release of the package.
+
 echo "Running release-tag.sh"
 
 # Ensure we're on the master branch
 if [ "$(git rev-parse --abbrev-ref HEAD)" != "master" ]; then
     echo "Not on master branch, aborting"
     exit 1
 fi
```

### Comparing `wpdetect-1.4.7/.github/ISSUE_TEMPLATE/bug_report.md` & `wpdetect-1.4.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.7/.github/ISSUE_TEMPLATE/feature_request.md` & `wpdetect-1.4.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.7/.github/workflows/pylint.yml` & `wpdetect-1.4.8/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.7/.github/workflows/pypi-publish.yml` & `wpdetect-1.4.8/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.7/utils/bump_version.py` & `wpdetect-1.4.8/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.7/wpdetect/__main__.py` & `wpdetect-1.4.8/wpdetect/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 '''
 name: wpdetect
 description: A simple script to detect if a website is running WordPress.
 '''
 
 import sys
-import os
 import urllib.request
 from urllib.parse import urlparse
 import toml
 import click
 from pyfiglet import figlet_format
 
 HEADER = "'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.75.14" + \
@@ -29,17 +28,16 @@
     'scan_full': False,  # default value
 }
 
 
 def get_package_version():
     """Returns the version of the package."""
 
-    file_path = os.path.join(os.path.dirname(__file__), '..', 'pyproject.toml')
-
-    with open(file_path, 'r', encoding="utf-8") as pyproject_toml_file:
+    # using absolute path to open the file because of the issue: #31
+    with open('pyproject.toml', 'r', encoding="utf-8") as pyproject_toml_file:
         config = toml.load(pyproject_toml_file)
 
     return config['project']['version']
 
 
 def print_verbose(message):
     """Prints the message if verbose is true."""
```

### Comparing `wpdetect-1.4.7/.gitignore` & `wpdetect-1.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.7/LICENSE.txt` & `wpdetect-1.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.7/README.md` & `wpdetect-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.7/pyproject.toml` & `wpdetect-1.4.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wpdetect"
-version = "1.4.7"
+version = "1.4.8"
 dependencies = [
     "pyfiglet", "requests", "click", "toml"
 ]
 authors = [
   { name="S M Mahmudul Hasan", email="he@smmahmudulhasan.com" },
 ]
 description = "A WordPress detection tool, detects if a website is running WordPress"
@@ -22,10 +22,11 @@
     'Topic :: Software Development :: Build Tools',
     'Intended Audience :: Developers',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/IamLizu/wpdetect"
 "Bug Tracker" = "https://github.com/IamLizu/wpdetect/issues"
+"Changelog" = "https://github.com/IamLizu/wpdetect/blob/master/CHANGELOG.md"
 
 [project.scripts]
 wpdetect = "wpdetect.__main__:main"
```

### Comparing `wpdetect-1.4.7/PKG-INFO` & `wpdetect-1.4.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: wpdetect
-Version: 1.4.7
+Version: 1.4.8
 Summary: A WordPress detection tool, detects if a website is running WordPress
 Project-URL: Homepage, https://github.com/IamLizu/wpdetect
 Project-URL: Bug Tracker, https://github.com/IamLizu/wpdetect/issues
+Project-URL: Changelog, https://github.com/IamLizu/wpdetect/blob/master/CHANGELOG.md
 Author-email: S M Mahmudul Hasan <he@smmahmudulhasan.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

