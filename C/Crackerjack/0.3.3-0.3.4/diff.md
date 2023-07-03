# Comparing `tmp/crackerjack-0.3.3.tar.gz` & `tmp/crackerjack-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.3.3.tar", last modified: Sun Jun 18 16:35:05 2023, max compression
+gzip compressed data, was "crackerjack-0.3.4.tar", last modified: Mon Jul  3 01:09:59 2023, max compression
```

## Comparing `crackerjack-0.3.3.tar` & `crackerjack-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.3/LICENSE
--rw-r--r--   0        0        0     5917 2023-06-18 16:33:36.904528 crackerjack-0.3.3/README.md
--rw-r--r--   0        0        0        0 2023-06-18 16:34:30.410683 crackerjack-0.3.3/crackerjack/.crackerjack-config.yaml
--rw-r--r--   0        0        0      223 2023-06-18 16:34:30.363852 crackerjack-0.3.3/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-06-18 16:34:30.395365 crackerjack-0.3.3/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2913 2023-06-18 16:34:30.379571 crackerjack-0.3.3/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.3/crackerjack/.pyanalyze-report.json
--rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.3/crackerjack/.pyanalyze-report.md
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.3/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.3/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.3/crackerjack/__init__.py
--rw-r--r--   0        0        0     1413 2023-06-12 11:12:35.268625 crackerjack-0.3.3/crackerjack/__main__.py
--rw-r--r--   0        0        0     6093 2023-06-18 10:42:33.340722 crackerjack-0.3.3/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1658 2023-06-18 16:34:31.122892 crackerjack-0.3.3/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     2009 2023-06-18 16:35:05.831269 crackerjack-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 crackerjack-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.4/LICENSE
+-rw-r--r--   0        0        0     5917 2023-06-18 16:33:36.904528 crackerjack-0.3.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 01:09:19.930137 crackerjack-0.3.4/crackerjack/.crackerjack-config.yaml
+-rw-r--r--   0        0        0      229 2023-07-03 01:09:19.880908 crackerjack-0.3.4/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-07-03 01:09:19.914538 crackerjack-0.3.4/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2917 2023-07-03 01:09:19.898753 crackerjack-0.3.4/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.4/crackerjack/.pyanalyze-report.json
+-rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.4/crackerjack/.pyanalyze-report.md
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.4/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.4/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.4/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1413 2023-06-12 11:12:35.268625 crackerjack-0.3.4/crackerjack/__main__.py
+-rw-r--r--   0        0        0     6145 2023-06-19 10:49:19.257226 crackerjack-0.3.4/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1657 2023-07-03 01:09:20.698148 crackerjack-0.3.4/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     2008 2023-07-03 01:09:59.734847 crackerjack-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     6908 1970-01-01 00:00:00.000000 crackerjack-0.3.4/PKG-INFO
```

### Comparing `crackerjack-0.3.3/LICENSE` & `crackerjack-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.3/README.md` & `crackerjack-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.3/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.3.4/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.3/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.3.4/crackerjack/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/pdm-project/pdm
-    rev: 2.7.4  # a PDM release exposing the hook
+    rev: 2.8.0a2  # a PDM release exposing the hook
     hooks:
       - id: pdm-lock-check
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
         name: trailing-whitspace
@@ -18,28 +18,28 @@
         name: check-added-large-files
   - repo: https://github.com/psf/black
     rev: '23.3.0'
     hooks:
       - id: black
         language_version: python3.11
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.272
+    rev: v0.0.275
     hooks:
       - id: ruff
   - repo: https://github.com/fredrikaverpil/creosote
     rev: v2.6.2
     hooks:
       - id: creosote
         args: [--paths, "crackerjack", --exclude-deps, "pdm-bump", "tomli-w"]
   - repo: https://github.com/ikamensh/flynt/
     rev: '0.78'
     hooks:
       - id: flynt
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.5
     hooks:
       - id: codespell
         additional_dependencies:
           - tomli
   - repo: local
     hooks:
       - id: pyanalyze
@@ -65,39 +65,39 @@
         types_or: [ python, pyi ]
         language: python
         files: \.py$
         additional_dependencies:
           - autotyping>=23.3.0
           - libcst>=0.4.9
   - repo: https://github.com/dosisod/refurb
-    rev: v1.16.0
+    rev: v1.17.0
     hooks:
       - id: refurb
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.313
+    rev: v1.1.316
     hooks:
       - id: pyright
   #  - repo: https://github.com/pdoc3/pdoc
   #    rev: master
   #    hooks:
   #      - id: pdoc
   #        name: pdoc
   #        entry: pdoc --html -f -o docs module1 module2 module3
   #        language_version: python3.11
   #        require_serial: true
   #        types: [ python ]
   #        always_run: true
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.272
+    rev: v0.0.275
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
     rev: '23.3.0'
     hooks:
       - id: black
         language_version: python3.11
   - repo: https://github.com/pdm-project/pdm
-    rev: 2.7.4 # a PDM release exposing the hook
+    rev: 2.8.0a2 # a PDM release exposing the hook
     hooks:
       - id: pdm-export
         args: [ '-o', 'requirements.txt', '--without-hashes' ]
         files: ^pdm.lock$
```

### Comparing `crackerjack-0.3.3/crackerjack/.pyanalyze-report.json` & `crackerjack-0.3.4/crackerjack/.pyanalyze-report.json`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.3/crackerjack/.pyanalyze-report.md` & `crackerjack-0.3.4/crackerjack/.pyanalyze-report.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.3/crackerjack/__main__.py` & `crackerjack-0.3.4/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.3/crackerjack/crackerjack.py` & `crackerjack-0.3.4/crackerjack/crackerjack.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,14 +135,15 @@
         if options.interactive:
             for hook in ("refurb", "pyright"):
                 await self.run_interactive(hook)
         check_all = call(["pre-commit", "run", "--all-files"])
         if check_all > 0:
             call(["pre-commit", "run", "--all-files"])
         if options.publish:
+            run(["git", "add", "requirements.txt"])
             run(["pdm", "publish"])
         if options.commit:
             commit_msg = input("Commit message: ")
             call(["git", "commit", "-m", f"'{commit_msg}'", "--no-verify", "--", "."])
             call(["git", "push", "origin", "main"])
```

### Comparing `crackerjack-0.3.3/crackerjack/pyproject.toml` & `crackerjack-0.3.4/crackerjack/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm.dev-dependencies]
 dev = [
-    "pytest>=7.3.2",
+    "pytest>=7.4.0",
     "icecream>=2.1.3",
-    "pre-commit>=3.3.2",
+    "pre-commit>=3.3.3",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
 fix = true
 show-fixes = true
@@ -40,15 +40,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.3"
+version = "0.3.4"
 description = "Crackerjack code style"
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -61,19 +61,19 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "click>=8.1.3",
     "aiopath>=0.6.11",
     "aioconsole>=0.6.1",
-    "pydantic>=2.0b2",
+    "pydantic>=2.0",
     "inflection>=0.5.1",
-    "acb>=0.1.8",
+    "acb>=0.1.10",
     "tomli-w>=1.0.0",
-    "pdm-bump>=0.7.0",
+    "pdm-bump>=0.7.1",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

### Comparing `crackerjack-0.3.3/pyproject.toml` & `crackerjack-0.3.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 config = [
     "python.use_venv",
     "true",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "pytest>=7.3.2",
+    "pytest>=7.4.0",
     "icecream>=2.1.3",
-    "pre-commit>=3.3.2",
+    "pre-commit>=3.3.3",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
 fix = true
 show-fixes = true
@@ -59,15 +59,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.3"
+version = "0.3.4"
 description = "Crackerjack code style"
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -80,19 +80,19 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "click>=8.1.3",
     "aiopath>=0.6.11",
     "aioconsole>=0.6.1",
-    "pydantic>=2.0b2",
+    "pydantic>=2.0",
     "inflection>=0.5.1",
-    "acb>=0.1.8",
+    "acb>=0.1.10",
     "tomli-w>=1.0.0",
-    "pdm-bump>=0.7.0",
+    "pdm-bump>=0.7.1",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

### Comparing `crackerjack-0.3.3/PKG-INFO` & `crackerjack-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: crackerjack
-Version: 0.3.3
+Name: Crackerjack
+Version: 0.3.4
 Summary: Crackerjack code style
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
@@ -14,19 +14,19 @@
 Project-URL: Homepage, https://github.com/lesleslie/crackerjack
 Project-URL: Documentation, https://github.com/lesleslie/crackerjack
 Project-URL: Repository, https://github.com/lesleslie/crackerjack
 Requires-Python: >=3.11
 Requires-Dist: click>=8.1.3
 Requires-Dist: aiopath>=0.6.11
 Requires-Dist: aioconsole>=0.6.1
-Requires-Dist: pydantic>=2.0b2
+Requires-Dist: pydantic>=2.0
 Requires-Dist: inflection>=0.5.1
-Requires-Dist: acb>=0.1.8
+Requires-Dist: acb>=0.1.10
 Requires-Dist: tomli-w>=1.0.0
-Requires-Dist: pdm-bump>=0.7.0
+Requires-Dist: pdm-bump>=0.7.1
 Description-Content-Type: text/markdown
 
 # Crackerjack Python
 
 [![Python: 3.11](https://img.shields.io/badge/python-3.11%2B-blue)](https://docs.python.org/3/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
```

