# Comparing `tmp/choosy-0.0.3.tar.gz` & `tmp/choosy-0.0.4.tar.gz`

## Comparing `choosy-0.0.3.tar` & `choosy-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 choosy-0.0.3/requirements.txt
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 choosy-0.0.3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 choosy-0.0.3/src/choosy/__about__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 choosy-0.0.3/src/choosy/__init__.py
--rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 choosy-0.0.3/src/choosy/base.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 choosy-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 choosy-0.0.3/tests/test_base.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 choosy-0.0.3/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 choosy-0.0.3/LICENSE
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 choosy-0.0.3/README.md
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 choosy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 choosy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 choosy-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 choosy-0.0.4/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 choosy-0.0.4/src/choosy/__about__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 choosy-0.0.4/src/choosy/__init__.py
+-rw-r--r--   0        0        0    11194 2020-02-02 00:00:00.000000 choosy-0.0.4/src/choosy/base.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 choosy-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 choosy-0.0.4/tests/test_base.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 choosy-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 choosy-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 choosy-0.0.4/README.md
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 choosy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 choosy-0.0.4/PKG-INFO
```

### Comparing `choosy-0.0.3/.github/workflows/python-package.yml` & `choosy-0.0.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `choosy-0.0.3/tests/__init__.py` & `choosy-0.0.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `choosy-0.0.3/tests/test_base.py` & `choosy-0.0.4/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `choosy-0.0.3/.gitignore` & `choosy-0.0.4/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+.vscode/settings.json
```

### Comparing `choosy-0.0.3/LICENSE` & `choosy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `choosy-0.0.3/README.md` & `choosy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `choosy-0.0.3/pyproject.toml` & `choosy-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `choosy-0.0.3/PKG-INFO` & `choosy-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: choosy
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Documentation, https://github.com/ceesem/choosy#readme
 Project-URL: Issues, https://github.com/ceesem/choosy/issues
 Project-URL: Source, https://github.com/ceesem/choosy
 Author-email: Casey Schneider-Mizell <caseysm@gmail.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

