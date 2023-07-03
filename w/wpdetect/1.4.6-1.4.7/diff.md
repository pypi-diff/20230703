# Comparing `tmp/wpdetect-1.4.6.tar.gz` & `tmp/wpdetect-1.4.7.tar.gz`

## Comparing `wpdetect-1.4.6.tar` & `wpdetect-1.4.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 wpdetect-1.4.6/CHANGELOG.md
--rw-r--r--   0        0        0     5224 2020-02-02 00:00:00.000000 wpdetect-1.4.6/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 wpdetect-1.4.6/CONTRIBUTING.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 wpdetect-1.4.6/SECURITY.md
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 wpdetect-1.4.6/release-tag.sh
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 wpdetect-1.4.6/requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.6/sample_urls.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 wpdetect-1.4.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 wpdetect-1.4.6/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wpdetect-1.4.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.6/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.6/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.4.6/.vscode/settings.json
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 wpdetect-1.4.6/utils/bump_version.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 wpdetect-1.4.6/utils/generate_changelog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.6/wpdetect/__init__.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 wpdetect-1.4.6/wpdetect/__main__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.6/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.6/LICENSE.txt
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 wpdetect-1.4.6/README.md
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 wpdetect-1.4.6/pyproject.toml
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 wpdetect-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 wpdetect-1.4.7/CHANGELOG.md
+-rw-r--r--   0        0        0     5224 2020-02-02 00:00:00.000000 wpdetect-1.4.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 wpdetect-1.4.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 wpdetect-1.4.7/SECURITY.md
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 wpdetect-1.4.7/generate-changelog.sh
+-rwxr-xr-x   0        0        0     1033 2020-02-02 00:00:00.000000 wpdetect-1.4.7/release-tag.sh
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 wpdetect-1.4.7/requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wpdetect-1.4.7/sample_urls.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 wpdetect-1.4.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 wpdetect-1.4.7/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 wpdetect-1.4.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 wpdetect-1.4.7/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 wpdetect-1.4.7/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wpdetect-1.4.7/.vscode/settings.json
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 wpdetect-1.4.7/utils/bump_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.4.7/wpdetect/__init__.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 wpdetect-1.4.7/wpdetect/__main__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 wpdetect-1.4.7/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wpdetect-1.4.7/LICENSE.txt
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 wpdetect-1.4.7/README.md
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 wpdetect-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 wpdetect-1.4.7/PKG-INFO
```

### Comparing `wpdetect-1.4.6/CODE_OF_CONDUCT.md` & `wpdetect-1.4.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.6/CONTRIBUTING.md` & `wpdetect-1.4.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.6/.github/ISSUE_TEMPLATE/bug_report.md` & `wpdetect-1.4.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.6/.github/ISSUE_TEMPLATE/feature_request.md` & `wpdetect-1.4.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.6/.github/workflows/pylint.yml` & `wpdetect-1.4.7/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.6/.github/workflows/pypi-publish.yml` & `wpdetect-1.4.7/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.6/utils/bump_version.py` & `wpdetect-1.4.7/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.6/wpdetect/__main__.py` & `wpdetect-1.4.7/wpdetect/__main__.py`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.6/.gitignore` & `wpdetect-1.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.6/LICENSE.txt` & `wpdetect-1.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wpdetect-1.4.6/pyproject.toml` & `wpdetect-1.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wpdetect"
-version = "1.4.6"
+version = "1.4.7"
 dependencies = [
     "pyfiglet", "requests", "click", "toml"
 ]
 authors = [
   { name="S M Mahmudul Hasan", email="he@smmahmudulhasan.com" },
 ]
 description = "A WordPress detection tool, detects if a website is running WordPress"
```

