# Comparing `tmp/jdeskew-0.2.1.tar.gz` & `tmp/jdeskew-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdeskew-0.2.1.tar", last modified: Thu Jan  5 12:04:03 2023, max compression
+gzip compressed data, was "jdeskew-0.2.2.tar", last modified: Mon Jul  3 13:54:24 2023, max compression
```

## Comparing `jdeskew-0.2.1.tar` & `jdeskew-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 12:04:03.803184 jdeskew-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-05 12:03:53.000000 jdeskew-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-01-05 12:04:03.803184 jdeskew-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-01-05 12:03:53.000000 jdeskew-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 12:04:03.799183 jdeskew-0.2.1/jdeskew/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-05 12:03:53.000000 jdeskew-0.2.1/jdeskew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-01-05 12:03:53.000000 jdeskew-0.2.1/jdeskew/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-01-05 12:03:53.000000 jdeskew-0.2.1/jdeskew/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-05 12:04:03.000000 jdeskew-0.2.1/jdeskew/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 12:04:03.799183 jdeskew-0.2.1/jdeskew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-01-05 12:04:03.000000 jdeskew-0.2.1/jdeskew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-05 12:04:03.000000 jdeskew-0.2.1/jdeskew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 12:04:03.000000 jdeskew-0.2.1/jdeskew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-05 12:04:03.000000 jdeskew-0.2.1/jdeskew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-05 12:04:03.000000 jdeskew-0.2.1/jdeskew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-05 12:03:53.000000 jdeskew-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 12:04:03.803184 jdeskew-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-01-05 12:03:53.000000 jdeskew-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:54:24.019718 jdeskew-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:54:24.015718 jdeskew-0.2.2/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-03 13:54:10.000000 jdeskew-0.2.2/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-03 13:54:10.000000 jdeskew-0.2.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-03 13:54:10.000000 jdeskew-0.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:54:24.015718 jdeskew-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:54:24.019718 jdeskew-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-03 13:54:10.000000 jdeskew-0.2.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-03 13:54:10.000000 jdeskew-0.2.2/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-03 13:54:10.000000 jdeskew-0.2.2/.github/workflows/docker-build-and-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-03 13:54:10.000000 jdeskew-0.2.2/.github/workflows/greetings.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-03 13:54:10.000000 jdeskew-0.2.2/.github/workflows/label.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-03 13:54:10.000000 jdeskew-0.2.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-03 13:54:10.000000 jdeskew-0.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-03 13:54:10.000000 jdeskew-0.2.2/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-03 13:54:10.000000 jdeskew-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 13:54:10.000000 jdeskew-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-03 13:54:10.000000 jdeskew-0.2.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-03 13:54:10.000000 jdeskew-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-07-03 13:54:24.019718 jdeskew-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-03 13:54:10.000000 jdeskew-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-03 13:54:10.000000 jdeskew-0.2.2/cog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-03 13:54:10.000000 jdeskew-0.2.2/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:54:24.019718 jdeskew-0.2.2/jdeskew/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 13:54:10.000000 jdeskew-0.2.2/jdeskew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-03 13:54:10.000000 jdeskew-0.2.2/jdeskew/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 13:54:10.000000 jdeskew-0.2.2/jdeskew/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:54:24.019718 jdeskew-0.2.2/jdeskew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-07-03 13:54:23.000000 jdeskew-0.2.2/jdeskew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-03 13:54:24.000000 jdeskew-0.2.2/jdeskew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:54:23.000000 jdeskew-0.2.2/jdeskew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-03 13:54:23.000000 jdeskew-0.2.2/jdeskew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 13:54:23.000000 jdeskew-0.2.2/jdeskew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-03 13:54:10.000000 jdeskew-0.2.2/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-03 13:54:10.000000 jdeskew-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    18673 2023-07-03 13:54:10.000000 jdeskew-0.2.2/reproduce.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:54:24.019718 jdeskew-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-03 13:54:10.000000 jdeskew-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:54:24.019718 jdeskew-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   319963 2023-07-03 13:54:10.000000 jdeskew-0.2.2/tests/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-03 13:54:10.000000 jdeskew-0.2.2/tests/test.py
```

### Comparing `jdeskew-0.2.1/LICENSE` & `jdeskew-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jdeskew-0.2.1/PKG-INFO` & `jdeskew-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,13 @@
-Metadata-Version: 2.1
-Name: jdeskew
-Version: 0.2.1
-Summary: Document Image Skew Estimation using Adaptive Radial Projection
-Author: Luan Pham
-Author-email: phamquiluan@gmail.com
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Document Image Skew Estimation
 
-[![pypi package](https://img.shields.io/badge/version-v0.2.1-blue)](https://pypi.org/project/jdeskew)
-[![CircleCI](https://circleci.com/gh/phamquiluan/jdeskew/tree/master.svg?style=shield&circle-token=37f6b4ef126f3e985db7c624d1d76f22a223cf41)](https://circleci.com/gh/phamquiluan/jdeskew/tree/master)
+*To my love, Jenna*
+
+[![pypi package](https://img.shields.io/pypi/v/jdeskew.svg)](https://pypi.org/project/jdeskew)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/phamquiluan/jdeskew/tree/master.svg?style=svg&circle-token=f409daaab0e6671c81bb4b266b387fe933c131eb)](https://dl.circleci.com/status-badge/redirect/gh/phamquiluan/jdeskew/tree/master)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/25553a5195074e37a01dd3370c55abaa)](https://www.codacy.com/gh/phamquiluan/jdeskew/dashboard?utm_source=github.com&utm_medium=referral&utm_content=phamquiluan/jdeskew&utm_campaign=Badge_Coverage)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/25553a5195074e37a01dd3370c55abaa)](https://www.codacy.com/gh/phamquiluan/jdeskew/dashboard?utm_source=github.com&utm_medium=referral&utm_content=phamquiluan/jdeskew&utm_campaign=Badge_Grade)
 [![Downloads](https://static.pepy.tech/personalized-badge/jdeskew?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/jdeskew)
 ![example workflow](https://github.com/phamquiluan/jdeskew/actions/workflows/dependency-review.yml/badge.svg)
 ![example workflow](https://github.com/phamquiluan/jdeskew/actions/workflows/python-package.yml/badge.svg)
 ![example workflow](https://github.com/phamquiluan/jdeskew/actions/workflows/docker-build-and-push.yml/badge.svg)
 ![example workflow](https://github.com/phamquiluan/jdeskew/actions/workflows/python-publish.yml/badge.svg)
```

#### html2text {}

```diff
@@ -1,15 +1,13 @@
-Metadata-Version: 2.1 Name: jdeskew Version: 0.2.1 Summary: Document Image Skew
-Estimation using Adaptive Radial Projection Author: Luan Pham Author-email:
-phamquiluan@gmail.com Description-Content-Type: text/markdown Provides-Extra:
-dev License-File: LICENSE # Document Image Skew Estimation [![pypi package]
-(https://img.shields.io/badge/version-v0.2.1-blue)](https://pypi.org/project/
-jdeskew) [![CircleCI](https://circleci.com/gh/phamquiluan/jdeskew/tree/
-master.svg?style=shield&circle-token=37f6b4ef126f3e985db7c624d1d76f22a223cf41)]
-(https://circleci.com/gh/phamquiluan/jdeskew/tree/master) [![Codacy Badge]
+# Document Image Skew Estimation *To my love, Jenna* [![pypi package](https://
+img.shields.io/pypi/v/jdeskew.svg)](https://pypi.org/project/jdeskew) [!
+[CircleCI](https://dl.circleci.com/status-badge/img/gh/phamquiluan/jdeskew/
+tree/master.svg?style=svg&circle-
+token=f409daaab0e6671c81bb4b266b387fe933c131eb)](https://dl.circleci.com/
+status-badge/redirect/gh/phamquiluan/jdeskew/tree/master) [![Codacy Badge]
 (https://app.codacy.com/project/badge/Coverage/
 25553a5195074e37a01dd3370c55abaa)](https://www.codacy.com/gh/phamquiluan/
 jdeskew/
 dashboard?utm_source=github.com&utm_medium=referral&utm_content=phamquiluan/
 jdeskew&utm_campaign=Badge_Coverage) [![Codacy Badge](https://app.codacy.com/
 project/badge/Grade/25553a5195074e37a01dd3370c55abaa)](https://www.codacy.com/
 gh/phamquiluan/jdeskew/
```

### Comparing `jdeskew-0.2.1/jdeskew/estimator.py` & `jdeskew-0.2.2/jdeskew/estimator.py`

 * *Files identical despite different names*

### Comparing `jdeskew-0.2.1/jdeskew/utility.py` & `jdeskew-0.2.2/jdeskew/utility.py`

 * *Files identical despite different names*

### Comparing `jdeskew-0.2.1/jdeskew.egg-info/PKG-INFO` & `jdeskew-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,44 @@
 Metadata-Version: 2.1
 Name: jdeskew
-Version: 0.2.1
+Version: 0.2.2
 Summary: Document Image Skew Estimation using Adaptive Radial Projection
-Author: Luan Pham
-Author-email: phamquiluan@gmail.com
+Author-email: Luan Pham <phamquiluan@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2022 Luan Pham
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Document Image Skew Estimation
 
-[![pypi package](https://img.shields.io/badge/version-v0.2.1-blue)](https://pypi.org/project/jdeskew)
-[![CircleCI](https://circleci.com/gh/phamquiluan/jdeskew/tree/master.svg?style=shield&circle-token=37f6b4ef126f3e985db7c624d1d76f22a223cf41)](https://circleci.com/gh/phamquiluan/jdeskew/tree/master)
+*To my love, Jenna*
+
+[![pypi package](https://img.shields.io/pypi/v/jdeskew.svg)](https://pypi.org/project/jdeskew)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/phamquiluan/jdeskew/tree/master.svg?style=svg&circle-token=f409daaab0e6671c81bb4b266b387fe933c131eb)](https://dl.circleci.com/status-badge/redirect/gh/phamquiluan/jdeskew/tree/master)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/25553a5195074e37a01dd3370c55abaa)](https://www.codacy.com/gh/phamquiluan/jdeskew/dashboard?utm_source=github.com&utm_medium=referral&utm_content=phamquiluan/jdeskew&utm_campaign=Badge_Coverage)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/25553a5195074e37a01dd3370c55abaa)](https://www.codacy.com/gh/phamquiluan/jdeskew/dashboard?utm_source=github.com&utm_medium=referral&utm_content=phamquiluan/jdeskew&utm_campaign=Badge_Grade)
 [![Downloads](https://static.pepy.tech/personalized-badge/jdeskew?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/jdeskew)
 ![example workflow](https://github.com/phamquiluan/jdeskew/actions/workflows/dependency-review.yml/badge.svg)
 ![example workflow](https://github.com/phamquiluan/jdeskew/actions/workflows/python-package.yml/badge.svg)
 ![example workflow](https://github.com/phamquiluan/jdeskew/actions/workflows/docker-build-and-push.yml/badge.svg)
 ![example workflow](https://github.com/phamquiluan/jdeskew/actions/workflows/python-publish.yml/badge.svg)
```

#### html2text {}

```diff
@@ -1,15 +1,30 @@
-Metadata-Version: 2.1 Name: jdeskew Version: 0.2.1 Summary: Document Image Skew
-Estimation using Adaptive Radial Projection Author: Luan Pham Author-email:
-phamquiluan@gmail.com Description-Content-Type: text/markdown Provides-Extra:
-dev License-File: LICENSE # Document Image Skew Estimation [![pypi package]
-(https://img.shields.io/badge/version-v0.2.1-blue)](https://pypi.org/project/
-jdeskew) [![CircleCI](https://circleci.com/gh/phamquiluan/jdeskew/tree/
-master.svg?style=shield&circle-token=37f6b4ef126f3e985db7c624d1d76f22a223cf41)]
-(https://circleci.com/gh/phamquiluan/jdeskew/tree/master) [![Codacy Badge]
+Metadata-Version: 2.1 Name: jdeskew Version: 0.2.2 Summary: Document Image Skew
+Estimation using Adaptive Radial Projection Author-email: Luan Pham
+gmail.com> License: MIT License Copyright (c) 2022 Luan Pham Permission is
+hereby granted, free of charge, to any person obtaining a copy of this software
+and associated documentation files (the "Software"), to deal in the Software
+without restriction, including without limitation the rights to use, copy,
+modify, merge, publish, distribute, sublicense, and/or sell copies of the
+Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions: The above copyright notice and this
+permission notice shall be included in all copies or substantial portions of
+the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
+EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
+OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE. Description-Content-Type: text/markdown Provides-
+Extra: dev License-File: LICENSE # Document Image Skew Estimation *To my love,
+Jenna* [![pypi package](https://img.shields.io/pypi/v/jdeskew.svg)](https://
+pypi.org/project/jdeskew) [![CircleCI](https://dl.circleci.com/status-badge/
+img/gh/phamquiluan/jdeskew/tree/master.svg?style=svg&circle-
+token=f409daaab0e6671c81bb4b266b387fe933c131eb)](https://dl.circleci.com/
+status-badge/redirect/gh/phamquiluan/jdeskew/tree/master) [![Codacy Badge]
 (https://app.codacy.com/project/badge/Coverage/
 25553a5195074e37a01dd3370c55abaa)](https://www.codacy.com/gh/phamquiluan/
 jdeskew/
 dashboard?utm_source=github.com&utm_medium=referral&utm_content=phamquiluan/
 jdeskew&utm_campaign=Badge_Coverage) [![Codacy Badge](https://app.codacy.com/
 project/badge/Grade/25553a5195074e37a01dd3370c55abaa)](https://www.codacy.com/
 gh/phamquiluan/jdeskew/
```

