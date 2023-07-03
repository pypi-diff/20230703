# Comparing `tmp/exceptiongroup-1.1.1.tar.gz` & `tmp/exceptiongroup-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exceptiongroup-1.1.1.tar", last modified: Sun Mar 12 21:29:08 2023, max compression
+gzip compressed data, was "exceptiongroup-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `exceptiongroup-1.1.1.tar` & `exceptiongroup-1.1.2.tar`

### file list

```diff
@@ -1,10 +1,16 @@
--rw-r--r--   0        0        0     3704 2023-03-12 21:28:58.867359 exceptiongroup-1.1.1/LICENSE
--rw-r--r--   0        0        0     5276 2023-03-12 21:28:58.867359 exceptiongroup-1.1.1/README.rst
--rw-r--r--   0        0        0     1845 2023-03-12 21:28:58.871358 exceptiongroup-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      920 2023-03-12 21:28:58.871358 exceptiongroup-1.1.1/src/exceptiongroup/__init__.py
--rw-r--r--   0        0        0     3578 2023-03-12 21:28:58.871358 exceptiongroup-1.1.1/src/exceptiongroup/_catch.py
--rw-r--r--   0        0        0     9772 2023-03-12 21:28:58.871358 exceptiongroup-1.1.1/src/exceptiongroup/_exceptions.py
--rw-r--r--   0        0        0    19475 2023-03-12 21:28:58.871358 exceptiongroup-1.1.1/src/exceptiongroup/_formatting.py
--rw-r--r--   0        0        0      160 2023-03-12 21:29:08.819463 exceptiongroup-1.1.1/src/exceptiongroup/_version.py
--rw-r--r--   0        0        0        0 2023-03-12 21:28:58.871358 exceptiongroup-1.1.1/src/exceptiongroup/py.typed
--rw-r--r--   0        0        0     6083 1970-01-01 00:00:00.000000 exceptiongroup-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3704 2023-07-03 09:54:37.650307 exceptiongroup-1.1.2/LICENSE
+-rw-r--r--   0        0        0     5276 2023-07-03 09:54:37.650307 exceptiongroup-1.1.2/README.rst
+-rw-r--r--   0        0        0     2064 2023-07-03 09:54:37.650307 exceptiongroup-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      920 2023-07-03 09:54:37.650307 exceptiongroup-1.1.2/src/exceptiongroup/__init__.py
+-rw-r--r--   0        0        0     3656 2023-07-03 09:54:37.650307 exceptiongroup-1.1.2/src/exceptiongroup/_catch.py
+-rw-r--r--   0        0        0     9768 2023-07-03 09:54:37.650307 exceptiongroup-1.1.2/src/exceptiongroup/_exceptions.py
+-rw-r--r--   0        0        0    19475 2023-07-03 09:54:37.650307 exceptiongroup-1.1.2/src/exceptiongroup/_formatting.py
+-rw-r--r--   0        0        0      160 2023-07-03 09:54:46.502484 exceptiongroup-1.1.2/src/exceptiongroup/_version.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:54:37.654307 exceptiongroup-1.1.2/src/exceptiongroup/py.typed
+-rw-r--r--   0        0        0        0 2023-07-03 09:54:37.654307 exceptiongroup-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0       84 2023-07-03 09:54:37.654307 exceptiongroup-1.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     5261 2023-07-03 09:54:37.654307 exceptiongroup-1.1.2/tests/test_catch.py
+-rw-r--r--   0        0        0     4479 2023-07-03 09:54:37.654307 exceptiongroup-1.1.2/tests/test_catch_py311.py
+-rw-r--r--   0        0        0    30667 2023-07-03 09:54:37.654307 exceptiongroup-1.1.2/tests/test_exceptions.py
+-rw-r--r--   0        0        0    18256 2023-07-03 09:54:37.654307 exceptiongroup-1.1.2/tests/test_formatting.py
+-rw-r--r--   0        0        0     6083 1970-01-01 00:00:00.000000 exceptiongroup-1.1.2/PKG-INFO
```

### Comparing `exceptiongroup-1.1.1/LICENSE` & `exceptiongroup-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `exceptiongroup-1.1.1/README.rst` & `exceptiongroup-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `exceptiongroup-1.1.1/pyproject.toml` & `exceptiongroup-1.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -26,35 +26,41 @@
 
 [project.optional-dependencies]
 test = [
     "pytest >= 6"
 ]
 
 [tool.flit.sdist]
+include = [
+    "tests",
+]
 exclude = [
     ".github/*",
     ".gitignore",
     ".pre-commit-config.yaml"
 ]
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
 local_scheme = "dirty-tag"
 write_to = "src/exceptiongroup/_version.py"
 
-[tool.black]
-target-version = ['py37']
-
-[tool.isort]
-src_paths = ["src"]
-skip_gitignore = true
-profile = "black"
+[tool.ruff]
+line-length = 88
+select = [
+    "E", "F", "W",  # default flake-8
+    "I",            # isort
+    "ISC",          # flake8-implicit-str-concat
+    "PGH",          # pygrep-hooks
+    "RUF100",       # unused noqa (yesqa)
+]
+target-version = "py37"
 
-[tool.flake8]
-max-line-length = 88
+[tool.ruff.isort]
+known-first-party = ["exceptiongroup"]
 
 [tool.pytest.ini_options]
 addopts = "-rsx --tb=short --strict-config --strict-markers"
 testpaths = ["tests"]
 
 [tool.coverage.run]
 source = ["exceptiongroup"]
@@ -65,20 +71,21 @@
     "pragma: no cover",
     "if TYPE_CHECKING:"
 ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py37, py38, py39, py310, py311, pypy3
+envlist = py37, py38, py39, py310, py311, py312, pypy3
 skip_missing_interpreters = true
 minversion = 4.0
 
 [testenv]
 extras = test
 commands = python -m pytest {posargs}
+usedevelop = true
 
 [testenv:pyright]
 deps = pyright
 commands = pyright --verifytypes exceptiongroup
 usedevelop = true
 """
```

### Comparing `exceptiongroup-1.1.1/src/exceptiongroup/__init__.py` & `exceptiongroup-1.1.2/src/exceptiongroup/__init__.py`

 * *Files identical despite different names*

### Comparing `exceptiongroup-1.1.1/src/exceptiongroup/_catch.py` & `exceptiongroup-1.1.2/src/exceptiongroup/_catch.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             elif unhandled is None:
                 return True
             else:
                 raise unhandled from None
 
         return False
 
-    def handle_exception(self, exc: BaseException) -> BaseExceptionGroup | None:
+    def handle_exception(self, exc: BaseException) -> BaseException | None:
         excgroup: BaseExceptionGroup | None
         if isinstance(exc, BaseExceptionGroup):
             excgroup = exc
         else:
             excgroup = BaseExceptionGroup("", [exc])
 
         new_exceptions: list[BaseException] = []
@@ -53,14 +53,17 @@
                 except BaseException as new_exc:
                     new_exceptions.append(new_exc)
 
             if not excgroup:
                 break
 
         if new_exceptions:
+            if len(new_exceptions) == 1:
+                return new_exceptions[0]
+
             if excgroup:
                 new_exceptions.append(excgroup)
 
             return BaseExceptionGroup("", new_exceptions)
         elif (
             excgroup and len(excgroup.exceptions) == 1 and excgroup.exceptions[0] is exc
         ):
```

### Comparing `exceptiongroup-1.1.1/src/exceptiongroup/_exceptions.py` & `exceptiongroup-1.1.2/src/exceptiongroup/_exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             raise ValueError(
                 "second argument (exceptions) must be a non-empty sequence"
             )
 
         for i, exc in enumerate(__exceptions):
             if not isinstance(exc, BaseException):
                 raise ValueError(
-                    f"Item {i} of second argument (exceptions) is not an " f"exception"
+                    f"Item {i} of second argument (exceptions) is not an exception"
                 )
 
         if cls is BaseExceptionGroup:
             if all(isinstance(exc, Exception) for exc in __exceptions):
                 cls = ExceptionGroup
 
         if issubclass(cls, Exception):
```

### Comparing `exceptiongroup-1.1.1/src/exceptiongroup/_formatting.py` & `exceptiongroup-1.1.2/src/exceptiongroup/_formatting.py`

 * *Files identical despite different names*

### Comparing `exceptiongroup-1.1.1/PKG-INFO` & `exceptiongroup-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exceptiongroup
-Version: 1.1.1
+Version: 1.1.2
 Summary: Backport of PEP 654 (exception groups)
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

