# Comparing `tmp/robotframework-async-keyword-1.1.6.tar.gz` & `tmp/robotframework-async-keyword-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-async-keyword-1.1.6.tar", last modified: Mon Mar 20 19:55:12 2023, max compression
+gzip compressed data, was "robotframework-async-keyword-1.1.7.tar", last modified: Sun Jul  2 23:49:51 2023, max compression
```

## Comparing `robotframework-async-keyword-1.1.6.tar` & `robotframework-async-keyword-1.1.7.tar`

### file list

```diff
@@ -1,27 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:55:12.711837 robotframework-async-keyword-1.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:55:12.707837 robotframework-async-keyword-1.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:55:12.707837 robotframework-async-keyword-1.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-03-20 19:55:00.000000 robotframework-async-keyword-1.1.6/.github/workflows/pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-20 19:55:00.000000 robotframework-async-keyword-1.1.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-20 19:55:00.000000 robotframework-async-keyword-1.1.6/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:55:12.707837 robotframework-async-keyword-1.1.6/AsyncLibrary/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-20 19:55:00.000000 robotframework-async-keyword-1.1.6/AsyncLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-20 19:55:12.000000 robotframework-async-keyword-1.1.6/AsyncLibrary/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-20 19:55:00.000000 robotframework-async-keyword-1.1.6/AsyncLibrary/protected_ordered_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-03-20 19:55:00.000000 robotframework-async-keyword-1.1.6/AsyncLibrary/robot_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-03-20 19:55:00.000000 robotframework-async-keyword-1.1.6/AsyncLibrary/scoped_value.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-20 19:55:00.000000 robotframework-async-keyword-1.1.6/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-20 19:55:00.000000 robotframework-async-keyword-1.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-03-20 19:55:12.711837 robotframework-async-keyword-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-20 19:55:00.000000 robotframework-async-keyword-1.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-20 19:55:00.000000 robotframework-async-keyword-1.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:55:12.711837 robotframework-async-keyword-1.1.6/robotframework_async_keyword.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-03-20 19:55:12.000000 robotframework-async-keyword-1.1.6/robotframework_async_keyword.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-20 19:55:12.000000 robotframework-async-keyword-1.1.6/robotframework_async_keyword.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:55:12.000000 robotframework-async-keyword-1.1.6/robotframework_async_keyword.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-20 19:55:12.000000 robotframework-async-keyword-1.1.6/robotframework_async_keyword.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-20 19:55:12.000000 robotframework-async-keyword-1.1.6/robotframework_async_keyword.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 19:55:12.711837 robotframework-async-keyword-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-20 19:55:00.000000 robotframework-async-keyword-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:55:12.711837 robotframework-async-keyword-1.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-20 19:55:00.000000 robotframework-async-keyword-1.1.6/tests/test.robot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:49:51.265131 robotframework-async-keyword-1.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:49:51.265131 robotframework-async-keyword-1.1.7/AsyncLibrary/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-02 23:49:40.000000 robotframework-async-keyword-1.1.7/AsyncLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-02 23:49:51.000000 robotframework-async-keyword-1.1.7/AsyncLibrary/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-02 23:49:40.000000 robotframework-async-keyword-1.1.7/AsyncLibrary/protected_ordered_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-07-02 23:49:40.000000 robotframework-async-keyword-1.1.7/AsyncLibrary/robot_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-02 23:49:40.000000 robotframework-async-keyword-1.1.7/AsyncLibrary/scoped_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-02 23:49:40.000000 robotframework-async-keyword-1.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-02 23:49:40.000000 robotframework-async-keyword-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-02 23:49:51.265131 robotframework-async-keyword-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-02 23:49:40.000000 robotframework-async-keyword-1.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-02 23:49:40.000000 robotframework-async-keyword-1.1.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:49:51.265131 robotframework-async-keyword-1.1.7/robotframework_async_keyword.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-02 23:49:51.000000 robotframework-async-keyword-1.1.7/robotframework_async_keyword.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 23:49:51.000000 robotframework-async-keyword-1.1.7/robotframework_async_keyword.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 23:49:51.000000 robotframework-async-keyword-1.1.7/robotframework_async_keyword.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 23:49:51.000000 robotframework-async-keyword-1.1.7/robotframework_async_keyword.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-02 23:49:51.000000 robotframework-async-keyword-1.1.7/robotframework_async_keyword.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 23:49:51.265131 robotframework-async-keyword-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-02 23:49:40.000000 robotframework-async-keyword-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:49:51.265131 robotframework-async-keyword-1.1.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-02 23:49:40.000000 robotframework-async-keyword-1.1.7/test/test.robot
```

### Comparing `robotframework-async-keyword-1.1.6/AsyncLibrary/__init__.py` & `robotframework-async-keyword-1.1.7/AsyncLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-async-keyword-1.1.6/AsyncLibrary/protected_ordered_dict.py` & `robotframework-async-keyword-1.1.7/AsyncLibrary/protected_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `robotframework-async-keyword-1.1.6/AsyncLibrary/robot_async.py` & `robotframework-async-keyword-1.1.7/AsyncLibrary/robot_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from concurrent.futures import ThreadPoolExecutor, wait
 from functools import wraps
 from robot.api import logger
 from robot.libraries.BuiltIn import BuiltIn
 from robot.libraries.DateTime import convert_time
 from robot.running import Keyword
 from robot.output.logger import LOGGER
-from .scoped_value import scope_parameter, undefined
+from .scoped_value import scope_parameter, _UNDEFINED
 from .protected_ordered_dict import ProtectedOrderedDict
 
 
 class Postpone:
     '''
     wrapper which is used when tracing into the xml journal
     in oder to prevent that the file will corrupted.
@@ -192,20 +192,20 @@
     main thread
     This class creates a scope objectes for all of these objects,
     and provides methods which help to create an actual execution
     scope for threads and activation and deactivation methodes
     '''
     _attributes = [
         ['test'],
-        ['user_keywords'],
-        ['step_types'],
+        [['user_keywords'], []],
+        [['step_types'], ['steps']],
         ['timeout_occurred'],
         ['namespace', 'variables', '_scopes'],
         ['namespace', 'variables', '_variables_set', '_scopes'],
-        ['_started_keywords'],
+        [['_started_keywords'], []],
         ['in_suite_teardown'],
         ['in_test_teardown'],
         ['in_keyword_teardown'],
     ]
 
     _construct = {
         'test': None,
@@ -215,29 +215,45 @@
         'in_test_teardown': False,
         'in_keyword_teardown': 0,
     }
 
     def __init__(self):
         self._context = BuiltIn()._get_context()
         self._forks = []
-        for attibute in self._attributes:
-            current = self._context
-            for parameter in attibute:
-                parent = current
-                current = getattr(parent, parameter)
-            forkvalue = self._construct.get(parameter, undefined)
-            scope = scope_parameter(parent, parameter, forkvalue=forkvalue)
-            if not isinstance(self._context.namespace._kw_store.libraries,
-                              ProtectedOrderedDict):
-                self._context.namespace._kw_store.libraries = (
-                    ProtectedOrderedDict(
-                        self._context.namespace._kw_store.libraries
-                    )
+        for index, attributelist in reversed(
+                tuple(enumerate(self._attributes))):
+            if not isinstance(attributelist[0], list):
+                attributelist = [attributelist]
+            for count, attribute in reversed(tuple(enumerate(attributelist))):
+                if not attribute:
+                    del self._attributes[index]
+                    break
+                current = self._context
+                try:
+                    for parameter in attribute:
+                        parent = current
+                        current = getattr(parent, parameter)
+                except AttributeError:
+                    if count <= 0:
+                        raise
+                    continue
+                forkvalue = self._construct.get(parameter, _UNDEFINED)    # noqa, E501  pylint: disable=undefined-loop-variable
+                scope = scope_parameter(
+                    parent, parameter, forkvalue=forkvalue    # noqa, E501  pylint: disable=undefined-loop-variable
                 )
-            self._forks.append(scope.fork())
+                if not isinstance(self._context.namespace._kw_store.libraries,
+                                  ProtectedOrderedDict):
+                    self._context.namespace._kw_store.libraries = (
+                        ProtectedOrderedDict(
+                            self._context.namespace._kw_store.libraries
+                        )
+                    )
+                self._forks.append(scope.fork())
+                self._attributes[index] = attribute
+                break
 
         self._logger = logger_scope.fork()
         if CONSOLE_LOGGER_SCOPE:
             self._console_logger = CONSOLE_LOGGER_SCOPE.fork()
 
     def activate(self):
         '''
```

### Comparing `robotframework-async-keyword-1.1.6/AsyncLibrary/scoped_value.py` & `robotframework-async-keyword-1.1.7/AsyncLibrary/scoped_value.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 '''
 Wrapper around object to make values of parameters actually
 thread specific
 '''
 import threading
 
 
-undefined = []
+_UNDEFINED = object()
 
 
 class ScopedValue:
     '''
     scope content holder for the different execution
     path that will exists in robot framework, once
     we execute a keyword in a different thread
     '''
 
     def __init__(
             self,
-            original=undefined,
+            original=_UNDEFINED,
             *,
-            forkvalue=undefined,
-    ):    # pylint: disable=dangerous-default-value
+            forkvalue=_UNDEFINED,
+    ):
         self._scopeid = threading.local()
-        if original is undefined:
+        if original is _UNDEFINED:
             self._scopes = {}
         else:
             self._scopes = {None: original}
             try:
                 self.__name__ = original.__name__
             except AttributeError:
                 pass
             try:
                 self.__doc__ = original.__doc__
             except AttributeError:
                 pass
-        if forkvalue is not undefined:
+        if forkvalue is not _UNDEFINED:
             self._forkvalue = forkvalue
         self._lock = threading.Lock()
         self._next = 0
 
     @property
     def scope(self):
         '''
@@ -145,16 +145,16 @@
             return scope
 
 
 def scope_parameter(
         obj,
         parameter,
         *,
-        forkvalue=undefined,
-):    # pylint: disable=dangerous-default-value
+        forkvalue=_UNDEFINED,
+):
     '''
     decorator an paramter in an object through monkey patching
     so it can have different values in different threads
     as the code in Robot Framework is not prepared for having
     different execution paths
     '''
     try:
@@ -162,15 +162,15 @@
     except AttributeError:
         scope = None
 
     if not isinstance(scope, ScopedValue):
         original = getattr(obj, parameter)
 
         kwargs = {'original': original}
-        if forkvalue is not undefined:
+        if forkvalue is not _UNDEFINED:
             kwargs['forkvalue'] = forkvalue
         scope = ScopedValue(**kwargs)
         setattr(obj, f'_scoped_{parameter}', scope)
         delattr(obj, parameter)
 
         class PatchedClass(obj.__class__):    # noqa, E501 pylint: disable=too-few-public-methods
             '''
```

### Comparing `robotframework-async-keyword-1.1.6/LICENSE.txt` & `robotframework-async-keyword-1.1.7/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 The MIT License (MIT)
+
 Copyright (c) 2015-2023 Fredrik Reveny, René Lehfeld and others
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

### Comparing `robotframework-async-keyword-1.1.6/README.rst` & `robotframework-async-keyword-1.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework-async-keyword-1.1.6/pyproject.toml` & `robotframework-async-keyword-1.1.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [project]
 name = 'robotframework-async-keyword'
 authors = [
     {name = 'René Lehfeld', email = '54720674+rlehfeld@users.noreply.github.com'},
 ]
 description = 'Generic Robot Framework library for asynchronous keyword execution'
 requires-python = '>=3.7'
-license = {file = 'LICENSE.txt'}
+license = {text = 'MIT'}
 keywords = ['async', 'robotframework']
 classifiers = [
     'Programming Language :: Python :: 3',
     'Environment :: Other Environment',
     'Intended Audience :: Developers',
     'Operating System :: OS Independent',
     'Topic :: Software Development :: Libraries :: Python Modules',
@@ -25,13 +25,14 @@
 [project.urls]
 'Homepage' = 'https://github.com/rlehfeld/robotframework-async-keyword'
 'Bug Reports' = 'https://github.com/rlehfeld/robotframework-async-keyword/issues'
 'Source' = 'https://github.com/rlehfeld/robotframework-async-keyword/'
 
 [tool.setuptools]
 packages = ['AsyncLibrary']
+obsoletes = ['robotframework_async']
 
 [tool.setuptools.dynamic]
 readme = {file = ['README.rst']}
 
 [tool.setuptools_scm]
 write_to = 'AsyncLibrary/_version.py'
```

### Comparing `robotframework-async-keyword-1.1.6/tests/test.robot` & `robotframework-async-keyword-1.1.7/test/test.robot`

 * *Files 13% similar despite different names*

```diff
@@ -2,42 +2,51 @@
 Library    AsyncLibrary
 
 *** Test Cases ***
 Example
     ${handle 1}    Async Run    Deeply Nested Keyword    ${1}
     ${handle 2}    Async Run    Nested Keyword    ${2}
     ${handle 3}    Async Run    Set Variable    ${3}
-    ${handle 4}    Async Run    Deeply Nested Fail
-    ${handle 5}    Async Run    Deeply Nested Fail
-    
+    ${handle 4}    Async Run    Deeply Nested Fail    ${4}
+    ${handle 5}    Async Run    Deeply Nested Fail    ${5}
+    ${handle 6}    Async Run    Deeply Nested Fail    ${6}
+
     ${handles}    Create List
     ...    ${handle 3}
     ...    ${handle 2}
     ...    ${handle 1}
 
     ${return_value}    Async Get    ${handles}
     Log To Console    ${return_value}
 
     ${expected}    Create List   ${3}   ${2}    ${1}
     Log To Console    ${expected}
 
     Should Be True    $return_value==$expected
 
-    Run Keyword And Expect Error    should fail
+    Run Keyword And Expect Error    should fail ${4}
     ...    Async Get    ${handle 4}
 
+    [Teardown]        Run Keyword And Expect Error    should fail ${5}
+    ...    Async Get    ${handle 5}
 
 *** Keywords ***
 Nested Keyword
     [Arguments]    ${value}
+    Sleep    1 sec
     Log To Console    Got Value ${value}
     ${return}    Set Variable    ${value}
     RETURN    ${return}
 
 Deeply Nested Keyword
     [Arguments]    ${value}
     Log To Console    Deeply Nested Keyword ${value}
     ${return}    Nested Keyword    ${value}
     RETURN    ${return}
 
 Deeply Nested Fail
-    Fail    should fail
+    [Arguments]    ${value}
+    Sleep    1 sec
+    Fail    should fail ${value}
+    [Teardown]    Run Keywords
+    ...    Should Be Equal    ${KEYWORD MESSAGE}    should fail ${value}   AND
+    ...    Log To Console    Deeply Nested Fail ${KEYWORD MESSAGE}
```

