# Comparing `tmp/inflect-6.1.1.tar.gz` & `tmp/inflect-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inflect-6.1.1.tar", last modified: Mon Jul  3 10:02:55 2023, max compression
+gzip compressed data, was "inflect-6.2.0.tar", last modified: Mon Jul  3 18:53:02 2023, max compression
```

## Comparing `inflect-6.1.1.tar` & `inflect-6.2.0.tar`

### file list

```diff
@@ -1,50 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:02:55.858889 inflect-6.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-03 10:02:25.000000 inflect-6.1.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 10:02:25.000000 inflect-6.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:02:55.842889 inflect-6.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 10:02:25.000000 inflect-6.1.1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-03 10:02:25.000000 inflect-6.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:02:55.842889 inflect-6.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-03 10:02:25.000000 inflect-6.1.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-03 10:02:25.000000 inflect-6.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 10:02:25.000000 inflect-6.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 10:02:25.000000 inflect-6.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-03 10:02:25.000000 inflect-6.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-03 10:02:25.000000 inflect-6.1.1/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-03 10:02:55.862889 inflect-6.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-07-03 10:02:25.000000 inflect-6.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:02:55.846889 inflect-6.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-03 10:02:25.000000 inflect-6.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-03 10:02:25.000000 inflect-6.1.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-03 10:02:25.000000 inflect-6.1.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:02:55.846889 inflect-6.1.1/inflect/
--rw-r--r--   0 runner    (1001) docker     (123)   103434 2023-07-03 10:02:25.000000 inflect-6.1.1/inflect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:02:25.000000 inflect-6.1.1/inflect/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:02:55.850889 inflect-6.1.1/inflect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-03 10:02:55.000000 inflect-6.1.1/inflect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-03 10:02:55.000000 inflect-6.1.1/inflect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:02:55.000000 inflect-6.1.1/inflect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-03 10:02:55.000000 inflect-6.1.1/inflect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 10:02:55.000000 inflect-6.1.1/inflect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-03 10:02:25.000000 inflect-6.1.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-03 10:02:25.000000 inflect-6.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-03 10:02:25.000000 inflect-6.1.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-03 10:02:55.862889 inflect-6.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:02:55.858889 inflect-6.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    36011 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/inflections.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/test_an.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/test_classical_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/test_classical_ancient.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/test_classical_herd.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/test_classical_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/test_classical_person.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/test_classical_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/test_compounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/test_inflections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/test_join.py
--rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/test_numwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/test_pl_si.py
--rw-r--r--   0 runner    (1001) docker     (123)    46037 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/test_pwd.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-03 10:02:25.000000 inflect-6.1.1/tests/test_unicode.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-03 10:02:25.000000 inflect-6.1.1/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 10:02:25.000000 inflect-6.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.198320 inflect-6.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-03 18:52:38.000000 inflect-6.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 18:52:38.000000 inflect-6.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.190320 inflect-6.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 18:52:38.000000 inflect-6.2.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-03 18:52:38.000000 inflect-6.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.190320 inflect-6.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-03 18:52:38.000000 inflect-6.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-03 18:52:38.000000 inflect-6.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 18:52:38.000000 inflect-6.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 18:52:38.000000 inflect-6.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-03 18:52:38.000000 inflect-6.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-03 18:52:38.000000 inflect-6.2.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-03 18:53:02.198320 inflect-6.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-07-03 18:52:38.000000 inflect-6.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.190320 inflect-6.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-03 18:52:38.000000 inflect-6.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-03 18:52:38.000000 inflect-6.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-03 18:52:38.000000 inflect-6.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.190320 inflect-6.2.0/inflect/
+-rw-r--r--   0 runner    (1001) docker     (123)   103758 2023-07-03 18:52:38.000000 inflect-6.2.0/inflect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.198320 inflect-6.2.0/inflect/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:52:38.000000 inflect-6.2.0/inflect/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-03 18:52:38.000000 inflect-6.2.0/inflect/compat/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-03 18:52:38.000000 inflect-6.2.0/inflect/compat/pydantic1.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:52:38.000000 inflect-6.2.0/inflect/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.194320 inflect-6.2.0/inflect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-03 18:53:02.000000 inflect-6.2.0/inflect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 18:53:02.000000 inflect-6.2.0/inflect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:53:02.000000 inflect-6.2.0/inflect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 18:53:02.000000 inflect-6.2.0/inflect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 18:53:02.000000 inflect-6.2.0/inflect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-03 18:52:38.000000 inflect-6.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-03 18:52:38.000000 inflect-6.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-03 18:52:38.000000 inflect-6.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-03 18:53:02.198320 inflect-6.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:53:02.198320 inflect-6.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    36011 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/inflections.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_an.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_classical_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_classical_ancient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_classical_herd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_classical_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_classical_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_classical_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_compounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_inflections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_numwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_pl_si.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46096 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_pwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-03 18:52:38.000000 inflect-6.2.0/tests/test_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-03 18:52:38.000000 inflect-6.2.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-03 18:52:38.000000 inflect-6.2.0/tox.ini
```

### Comparing `inflect-6.1.1/.github/workflows/main.yml` & `inflect-6.2.0/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,18 @@
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
         - python: pypy3.9
           platform: ubuntu-latest
+        - python: "3.x"
+          platform: ubuntu-latest
+          env:
+            TOX_ENV: pydantic1
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.12' }}
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
```

### Comparing `inflect-6.1.1/LICENSE` & `inflect-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/NEWS.rst` & `inflect-6.2.0/NEWS.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v6.2.0
+======
+
+Features
+--------
+
+- Project now supports Pydantic 2 while retaining support for Pydantic 1. (#187)
+
+
+Bugfixes
+--------
+
+- Added validation of user-defined words and amended the type declarations to match, allowing for null values but not empty strings. (#187)
+
+
 v6.1.1
 ======
 
 Bugfixes
 --------
 
 - ``ordinal`` now handles float types correctly without first coercing them to strings. (#178)
```

### Comparing `inflect-6.1.1/PKG-INFO` & `inflect-6.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inflect
-Version: 6.1.1
+Version: 6.2.0
 Summary: Correctly generate plurals, singular nouns, ordinals, indefinite articles; convert numbers to words
 Home-page: https://github.com/jaraco/inflect
 Author: Paul Dyson
 Author-email: pwdyson@yahoo.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `inflect-6.1.1/README.rst` & `inflect-6.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/docs/conf.py` & `inflect-6.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/inflect/__init__.py` & `inflect-6.2.0/inflect/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,20 @@
     Sequence,
     cast,
     Any,
 )
 from numbers import Number
 
 
-from pydantic import Field, validate_arguments
-from pydantic.typing import Annotated
+from pydantic import Field
+from typing_extensions import Annotated
+
+
+from .compat.pydantic1 import validate_call
+from .compat.pydantic import same_method
 
 
 class UnknownClassicalModeError(Exception):
     pass
 
 
 class BadNumValueError(Exception):
@@ -2030,19 +2034,19 @@
 
 
 class engine:
     def __init__(self) -> None:
         self.classical_dict = def_classical.copy()
         self.persistent_count: Optional[int] = None
         self.mill_count = 0
-        self.pl_sb_user_defined: List[str] = []
-        self.pl_v_user_defined: List[str] = []
-        self.pl_adj_user_defined: List[str] = []
-        self.si_sb_user_defined: List[str] = []
-        self.A_a_user_defined: List[str] = []
+        self.pl_sb_user_defined: List[Optional[Word]] = []
+        self.pl_v_user_defined: List[Optional[Word]] = []
+        self.pl_adj_user_defined: List[Optional[Word]] = []
+        self.si_sb_user_defined: List[Optional[Word]] = []
+        self.A_a_user_defined: List[Optional[Word]] = []
         self.thegender = "neuter"
         self.__number_args: Optional[Dict[str, str]] = None
 
     @property
     def _number_args(self):
         return cast(Dict[str, str], self.__number_args)
 
@@ -2067,26 +2071,36 @@
 
     def __getattr__(self, meth):
         if meth in self.deprecated_methods:
             print3(f"{meth}() deprecated, use {self.deprecated_methods[meth]}()")
             raise DeprecationWarning
         raise AttributeError
 
-    def defnoun(self, singular: str, plural: str) -> int:
+    @validate_call
+    def defnoun(self, singular: Optional[Word], plural: Optional[Word]) -> int:
         """
         Set the noun plural of singular to plural.
 
         """
         self.checkpat(singular)
         self.checkpatplural(plural)
         self.pl_sb_user_defined.extend((singular, plural))
         self.si_sb_user_defined.extend((plural, singular))
         return 1
 
-    def defverb(self, s1: str, p1: str, s2: str, p2: str, s3: str, p3: str) -> int:
+    @validate_call
+    def defverb(
+        self,
+        s1: Optional[Word],
+        p1: Optional[Word],
+        s2: Optional[Word],
+        p2: Optional[Word],
+        s3: Optional[Word],
+        p3: Optional[Word],
+    ) -> int:
         """
         Set the verb plurals for s1, s2 and s3 to p1, p2 and p3 respectively.
 
         Where 1, 2 and 3 represent the 1st, 2nd and 3rd person forms of the verb.
 
         """
         self.checkpat(s1)
@@ -2094,61 +2108,64 @@
         self.checkpat(s3)
         self.checkpatplural(p1)
         self.checkpatplural(p2)
         self.checkpatplural(p3)
         self.pl_v_user_defined.extend((s1, p1, s2, p2, s3, p3))
         return 1
 
-    def defadj(self, singular: str, plural: str) -> int:
+    @validate_call
+    def defadj(self, singular: Optional[Word], plural: Optional[Word]) -> int:
         """
         Set the adjective plural of singular to plural.
 
         """
         self.checkpat(singular)
         self.checkpatplural(plural)
         self.pl_adj_user_defined.extend((singular, plural))
         return 1
 
-    def defa(self, pattern: str) -> int:
+    @validate_call
+    def defa(self, pattern: Optional[Word]) -> int:
         """
         Define the indefinite article as 'a' for words matching pattern.
 
         """
         self.checkpat(pattern)
         self.A_a_user_defined.extend((pattern, "a"))
         return 1
 
-    def defan(self, pattern: str) -> int:
+    @validate_call
+    def defan(self, pattern: Optional[Word]) -> int:
         """
         Define the indefinite article as 'an' for words matching pattern.
 
         """
         self.checkpat(pattern)
         self.A_a_user_defined.extend((pattern, "an"))
         return 1
 
-    def checkpat(self, pattern: Optional[str]) -> None:
+    def checkpat(self, pattern: Optional[Word]) -> None:
         """
         check for errors in a regex pattern
         """
         if pattern is None:
             return
         try:
             re.match(pattern, "")
         except re.error:
             print3(f"\nBad user-defined singular pattern:\n\t{pattern}\n")
             raise BadUserDefinedPatternError
 
-    def checkpatplural(self, pattern: str) -> None:
+    def checkpatplural(self, pattern: Optional[Word]) -> None:
         """
         check for errors in a regex replace pattern
         """
         return
 
-    @validate_arguments
+    @validate_call
     def ud_match(self, word: Word, wordlist: Sequence[Optional[Word]]) -> Optional[str]:
         for i in range(len(wordlist) - 2, -2, -2):  # backwards through even elements
             mo = re.search(fr"^{wordlist[i]}$", word, re.IGNORECASE)
             if mo:
                 if wordlist[i + 1] is None:
                     return None
                 pl = DOLLAR_DIGITS.sub(
@@ -2280,15 +2297,15 @@
         }
 
         # Call the corresponding function
         return methods_dict[f_name](*args_list, **kwargs_list)
 
     # 0. PERFORM GENERAL INFLECTIONS IN A STRING
 
-    @validate_arguments
+    @validate_call
     def inflect(self, text: Word) -> str:
         """
         Perform inflections in a string.
 
         e.g. inflect('The plural of cat is plural(cat)') returns
         'The plural of cat is cats'
 
@@ -2357,15 +2374,15 @@
     def partition_word(self, text: str) -> Tuple[str, str, str]:
         mo = PARTITION_WORD.search(text)
         if mo:
             return mo.group(1), mo.group(2), mo.group(3)
         else:
             return "", "", ""
 
-    @validate_arguments
+    @validate_call
     def plural(self, text: Word, count: Optional[Union[str, int, Any]] = None) -> str:
         """
         Return the plural of text.
 
         If count supplied, then return text if count is one of:
             1, a, an, one, each, every, this, that
 
@@ -2381,15 +2398,15 @@
             word,
             self._pl_special_adjective(word, count)
             or self._pl_special_verb(word, count)
             or self._plnoun(word, count),
         )
         return f"{pre}{plural}{post}"
 
-    @validate_arguments
+    @validate_call
     def plural_noun(
         self, text: Word, count: Optional[Union[str, int, Any]] = None
     ) -> str:
         """
         Return the plural of text, where text is a noun.
 
         If count supplied, then return text if count is one of:
@@ -2402,15 +2419,15 @@
         """
         pre, word, post = self.partition_word(text)
         if not word:
             return text
         plural = self.postprocess(word, self._plnoun(word, count))
         return f"{pre}{plural}{post}"
 
-    @validate_arguments
+    @validate_call
     def plural_verb(
         self, text: Word, count: Optional[Union[str, int, Any]] = None
     ) -> str:
         """
         Return the plural of text, where text is a verb.
 
         If count supplied, then return text if count is one of:
@@ -2426,15 +2443,15 @@
             return text
         plural = self.postprocess(
             word,
             self._pl_special_verb(word, count) or self._pl_general_verb(word, count),
         )
         return f"{pre}{plural}{post}"
 
-    @validate_arguments
+    @validate_call
     def plural_adj(
         self, text: Word, count: Optional[Union[str, int, Any]] = None
     ) -> str:
         """
         Return the plural of text, where text is an adjective.
 
         If count supplied, then return text if count is one of:
@@ -2447,15 +2464,15 @@
         """
         pre, word, post = self.partition_word(text)
         if not word:
             return text
         plural = self.postprocess(word, self._pl_special_adjective(word, count) or word)
         return f"{pre}{plural}{post}"
 
-    @validate_arguments
+    @validate_call
     def compare(self, word1: Word, word2: Word) -> Union[str, bool]:
         """
         compare word1 and word2 for equality regardless of plurality
 
         return values:
         eq - the strings are equal
         p:s - word1 is the plural of word2
@@ -2470,23 +2487,23 @@
         'eq'
 
         Words should not be empty.
 
         >>> compare('egg', '')
         Traceback (most recent call last):
         ...
-        pydantic.error_wrappers.ValidationError: 1 validation error for Compare
-        word2
-          ensure this value has at least 1 characters...
+        pydantic...ValidationError: ...
+        ...
+          ...at least 1 characters...
         """
         norms = self.plural_noun, self.plural_verb, self.plural_adj
         results = (self._plequal(word1, word2, norm) for norm in norms)
         return next(filter(None, results), False)
 
-    @validate_arguments
+    @validate_call
     def compare_nouns(self, word1: Word, word2: Word) -> Union[str, bool]:
         """
         compare word1 and word2 for equality regardless of plurality
         word1 and word2 are to be treated as nouns
 
         return values:
         eq - the strings are equal
@@ -2494,15 +2511,15 @@
         s:p - word2 is the plural of word1
         p:p - word1 and word2 are two different plural forms of the one word
         False - otherwise
 
         """
         return self._plequal(word1, word2, self.plural_noun)
 
-    @validate_arguments
+    @validate_call
     def compare_verbs(self, word1: Word, word2: Word) -> Union[str, bool]:
         """
         compare word1 and word2 for equality regardless of plurality
         word1 and word2 are to be treated as verbs
 
         return values:
         eq - the strings are equal
@@ -2510,15 +2527,15 @@
         s:p - word2 is the plural of word1
         p:p - word1 and word2 are two different plural forms of the one word
         False - otherwise
 
         """
         return self._plequal(word1, word2, self.plural_verb)
 
-    @validate_arguments
+    @validate_call
     def compare_adjs(self, word1: Word, word2: Word) -> Union[str, bool]:
         """
         compare word1 and word2 for equality regardless of plurality
         word1 and word2 are to be treated as adjectives
 
         return values:
         eq - the strings are equal
@@ -2526,15 +2543,15 @@
         s:p - word2 is the plural of word1
         p:p - word1 and word2 are two different plural forms of the one word
         False - otherwise
 
         """
         return self._plequal(word1, word2, self.plural_adj)
 
-    @validate_arguments
+    @validate_call
     def singular_noun(
         self,
         text: Word,
         count: Optional[Union[int, str, Any]] = None,
         gender: Optional[str] = None,
     ) -> Union[str, bool]:
         """
@@ -2584,20 +2601,20 @@
         self.classical_dict = no_classical.copy()
         if word1 == pl(word2):
             return "p:s"
         if pl(word1) == word2:
             return "s:p"
         self.classical_dict = classval.copy()
 
-        if pl == self.plural or pl == self.plural_noun:
+        if same_method(pl, self.plural) or same_method(pl, self.plural_noun):
             if self._pl_check_plurals_N(word1, word2):
                 return "p:p"
             if self._pl_check_plurals_N(word2, word1):
                 return "p:p"
-        if pl == self.plural or pl == self.plural_adj:
+        if same_method(pl, self.plural) or same_method(pl, self.plural_adj):
             if self._pl_check_plurals_adj(word1, word2):
                 return "p:p"
         return False
 
     def _pl_reg_plurals(self, pair: str, stems: str, end1: str, end2: str) -> bool:
         pattern = fr"({stems})({end1}\|\1{end2}|{end2}\|\1{end1})"
         return bool(re.search(pattern, pair))
@@ -3460,15 +3477,15 @@
 
         # COULD NOT FIND SINGULAR
 
         return False
 
     # ADJECTIVES
 
-    @validate_arguments
+    @validate_call
     def a(self, text: Word, count: Optional[Union[int, str, Any]] = 1) -> str:
         """
         Return the appropriate indefinite article followed by text.
 
         The indefinite article is either 'a' or 'an'.
 
         If count is not one, then return count followed by text
@@ -3541,15 +3558,15 @@
 
         # OTHERWISE, GUESS "a"
         fallback = f'a {word}'
         return next(matches, fallback)
 
     # 2. TRANSLATE ZERO-QUANTIFIED $word TO "no plural($word)"
 
-    @validate_arguments
+    @validate_call
     def no(self, text: Word, count: Optional[Union[int, str]] = None) -> str:
         """
         If count is 0, no, zero or nil, return 'no' followed by the plural
         of text.
 
         If count is one of:
             1, a, an, one, each, every, this, that
@@ -3579,15 +3596,15 @@
 
         if str(count).lower() in pl_count_zero:
             count = 'no'
         return f"{pre}{count} {self.plural(word, count)}{post}"
 
     # PARTICIPLES
 
-    @validate_arguments
+    @validate_call
     def present_participle(self, word: Word) -> str:
         """
         Return the present participle for word.
 
         word is the 3rd person singular verb.
 
         """
@@ -3598,15 +3615,15 @@
             ans, num = regexen.subn(repl, plv)
             if num:
                 return f"{ans}ing"
         return f"{ans}ing"
 
     # NUMERICAL INFLECTIONS
 
-    @validate_arguments(config=dict(arbitrary_types_allowed=True))
+    @validate_call(config=dict(arbitrary_types_allowed=True))
     def ordinal(self, num: Union[Number, Word]) -> str:
         """
         Return the ordinal of num.
 
         >>> ordinal = engine().ordinal
         >>> ordinal(1)
         '1st'
@@ -3758,15 +3775,15 @@
             while mo:
                 num = THREE_DIGITS_WORD.sub(self.hundsub, num, 1)
                 mo = THREE_DIGITS_WORD.search(num)
             num = TWO_DIGITS_WORD.sub(self.tensub, num, 1)
             num = ONE_DIGIT_WORD.sub(self.unitsub, num, 1)
         return num
 
-    @validate_arguments(config=dict(arbitrary_types_allowed=True))  # noqa: C901
+    @validate_call(config=dict(arbitrary_types_allowed=True))  # noqa: C901
     def number_to_words(  # noqa: C901
         self,
         num: Union[Number, Word],
         wantlist: bool = False,
         group: int = 0,
         comma: Union[Falsish, str] = ",",
         andword: str = "and",
@@ -3910,15 +3927,15 @@
                     num += f"{comma} {nc}"
                 else:
                     num += f" {nc}"
             return num
 
     # Join words with commas and a trailing 'and' (when appropriate)...
 
-    @validate_arguments
+    @validate_call
     def join(
         self,
         words: Optional[Sequence[Word]],
         sep: Optional[str] = None,
         sep_spaced: bool = True,
         final_sep: Optional[str] = None,
         conj: str = "and",
```

### Comparing `inflect-6.1.1/inflect.egg-info/PKG-INFO` & `inflect-6.2.0/inflect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inflect
-Version: 6.1.1
+Version: 6.2.0
 Summary: Correctly generate plurals, singular nouns, ordinals, indefinite articles; convert numbers to words
 Home-page: https://github.com/jaraco/inflect
 Author: Paul Dyson
 Author-email: pwdyson@yahoo.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `inflect-6.1.1/inflect.egg-info/SOURCES.txt` & `inflect-6.2.0/inflect.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 inflect/__init__.py
 inflect/py.typed
 inflect.egg-info/PKG-INFO
 inflect.egg-info/SOURCES.txt
 inflect.egg-info/dependency_links.txt
 inflect.egg-info/requires.txt
 inflect.egg-info/top_level.txt
+inflect/compat/__init__.py
+inflect/compat/pydantic.py
+inflect/compat/pydantic1.py
 tests/inflections.txt
 tests/test_an.py
 tests/test_classical_all.py
 tests/test_classical_ancient.py
 tests/test_classical_herd.py
 tests/test_classical_names.py
 tests/test_classical_person.py
```

### Comparing `inflect-6.1.1/pytest.ini` & `inflect-6.2.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/setup.cfg` & `inflect-6.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 	Topic :: Text Processing :: Linguistic
 
 [options]
 packages = find_namespace:
 include_package_data = true
 python_requires = >=3.8
 install_requires = 
-	pydantic >= 1.9.1, < 2
+	pydantic >= 1.9.1
+	typing_extensions
 keywords = plural inflect participle
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
```

### Comparing `inflect-6.1.1/tests/inflections.txt` & `inflect-6.2.0/tests/inflections.txt`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/tests/test_an.py` & `inflect-6.2.0/tests/test_an.py`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/tests/test_classical_all.py` & `inflect-6.2.0/tests/test_classical_all.py`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/tests/test_classical_ancient.py` & `inflect-6.2.0/tests/test_classical_ancient.py`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/tests/test_classical_herd.py` & `inflect-6.2.0/tests/test_classical_herd.py`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/tests/test_classical_names.py` & `inflect-6.2.0/tests/test_classical_names.py`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/tests/test_classical_person.py` & `inflect-6.2.0/tests/test_classical_person.py`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/tests/test_classical_zero.py` & `inflect-6.2.0/tests/test_classical_zero.py`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/tests/test_compounds.py` & `inflect-6.2.0/tests/test_compounds.py`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/tests/test_inflections.py` & `inflect-6.2.0/tests/test_inflections.py`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/tests/test_join.py` & `inflect-6.2.0/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/tests/test_numwords.py` & `inflect-6.2.0/tests/test_numwords.py`

 * *Files identical despite different names*

### Comparing `inflect-6.1.1/tests/test_pwd.py` & `inflect-6.2.0/tests/test_pwd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-#!/usr/bin/python
-
 import unittest
 
 import pytest
 
 from inflect import (
     BadChunkingOptionError,
     NumOutOfRangeError,
     BadNumValueError,
     BadGenderError,
     UnknownClassicalModeError,
 )
 import inflect
+from inflect.compat.pydantic import same_method
+
+
+missing = object()
 
 
 class test(unittest.TestCase):
     def TODO(
         self,
         ans,
         answer_wanted,
-        answer_gives_now="default_that_will_never_occur__can't_use_None"
-        "_as_that_is_a_possible_valid_value",
+        answer_gives_now=missing,
     ):
         """
         make this test for future testing
 
         so can easily rename these to assertEqual when code ready
         """
         if ans == answer_wanted:
             print("test unexpectedly passed!: {} == {}".format(ans, answer_wanted))
-        if answer_gives_now != (
-            "default_that_will_never_occur__can't_use_None"
-            "_as_that_is_a_possible_valid_value"
-        ):
+        if answer_gives_now is not missing:
             self.assertEqual(ans, answer_gives_now)
 
     def test_enclose(self):
         # def enclose
         self.assertEqual(inflect.enclose("test"), "(?:test)")
 
     def test_joinstem(self):
@@ -191,15 +189,15 @@
         p.defnoun("(cat)", r"$1s")
         self.assertEqual(p.plural("cat"), "cats")
 
         inflect.STDOUT_ON = False
         self.assertRaises(inflect.BadUserDefinedPatternError, p.defnoun, "(??", None)
         inflect.STDOUT_ON = True
 
-        p.defnoun(None, "")  # check None doesn't crash it
+        p.defnoun(None, "any")  # check None doesn't crash it
 
         # defverb
         p.defverb("will", "shall", "will", "will", "will", "will")
         self.assertEqual(p.ud_match("will", p.pl_v_user_defined), "will")
         self.assertEqual(p.plural("will"), "will")
         # TODO: will -> shall. Tests below fail
         self.TODO(p.compare("will", "shall"), "s:p")
@@ -479,14 +477,16 @@
             (p.compare_verbs, "run", "run", "eq"),
             (p.compare_adjs, "my", "my", "eq"),
             (p.compare_adjs, "my", "our", "s:p"),
             (p.compare_adjs, "our", "our", "eq"),
         ):
             self.assertEqual(fn(sing, plur), res)
 
+    def test_plequal_todos(self):
+        p = inflect.engine()
         for fn, sing, plur, res, badres in (
             (
                 p.compare,
                 "dresses's",
                 "dresses'",
                 "p:p",
                 "p:s",
@@ -799,18 +799,22 @@
             ("a ant", "an ant"),
         ):
             self.assertEqual(p.a(sing), plur)
 
         self.assertEqual(p.a("cat", 1), "a cat")
         self.assertEqual(p.a("cat", 2), "2 cat")
 
-        self.assertEqual(p.a, p.an)
         with pytest.raises(Exception):
             p.a("")
 
+    def test_a_and_an_same_method(self):
+        assert same_method(inflect.engine.a, inflect.engine.an)
+        p = inflect.engine()
+        assert same_method(p.a, p.an)
+
     def test_no(self):
         p = inflect.engine()
         self.assertEqual(p.no("cat"), "no cats")
         self.assertEqual(p.no("cat", count=3), "3 cats")
         self.assertEqual(p.no("cat", count="three"), "three cats")
         self.assertEqual(p.no("cat", count=1), "1 cat")
         self.assertEqual(p.no("cat", count="one"), "one cat")
```

### Comparing `inflect-6.1.1/tox.ini` & `inflect-6.2.0/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 	PYTHONWARNDEFAULTENCODING = 1
 commands =
 	pytest {posargs}
 usedevelop = True
 extras =
 	testing
 
+[testenv:pydantic1]
+deps =
+	pydantic < 2
+
 [testenv:docs]
 extras =
 	docs
 	testing
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
```

