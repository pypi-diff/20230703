# Comparing `tmp/pyshamir-1.0.1.tar.gz` & `tmp/pyshamir-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pyshamir/pyshamir/dist/.tmp-0f6if25r/pyshamir-1.0.1.tar", last modified: Mon Mar 20 16:31:11 2023, max compression
+gzip compressed data, was "/home/runner/work/pyshamir/pyshamir/dist/.tmp-uypzl72o/pyshamir-1.0.2.tar", last modified: Mon Jul  3 16:38:29 2023, max compression
```

## Comparing `pyshamir-1.0.1.tar` & `pyshamir-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 16:31:11.000000 pyshamir-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-03-20 16:31:11.000000 pyshamir-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-20 16:31:02.000000 pyshamir-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 16:31:11.000000 pyshamir-1.0.1/pyshamir/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-20 16:31:02.000000 pyshamir-1.0.1/pyshamir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-03-20 16:31:02.000000 pyshamir-1.0.1/pyshamir/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-03-20 16:31:02.000000 pyshamir-1.0.1/pyshamir/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-03-20 16:31:02.000000 pyshamir-1.0.1/pyshamir/shamir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 16:31:11.000000 pyshamir-1.0.1/pyshamir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-03-20 16:31:11.000000 pyshamir-1.0.1/pyshamir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-20 16:31:11.000000 pyshamir-1.0.1/pyshamir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 16:31:11.000000 pyshamir-1.0.1/pyshamir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 16:31:11.000000 pyshamir-1.0.1/pyshamir.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-20 16:31:11.000000 pyshamir-1.0.1/pyshamir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-20 16:31:11.000000 pyshamir-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-20 16:31:02.000000 pyshamir-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 16:31:11.000000 pyshamir-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-20 16:31:02.000000 pyshamir-1.0.1/tests/test_shamir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:38:29.000000 pyshamir-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-03 16:38:29.000000 pyshamir-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-03 16:38:18.000000 pyshamir-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:38:29.000000 pyshamir-1.0.2/pyshamir/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-03 16:38:18.000000 pyshamir-1.0.2/pyshamir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-03 16:38:18.000000 pyshamir-1.0.2/pyshamir/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-03 16:38:18.000000 pyshamir-1.0.2/pyshamir/shamir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:38:29.000000 pyshamir-1.0.2/pyshamir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-03 16:38:29.000000 pyshamir-1.0.2/pyshamir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-03 16:38:29.000000 pyshamir-1.0.2/pyshamir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:38:29.000000 pyshamir-1.0.2/pyshamir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:38:28.000000 pyshamir-1.0.2/pyshamir.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 16:38:29.000000 pyshamir-1.0.2/pyshamir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-03 16:38:29.000000 pyshamir-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-03 16:38:18.000000 pyshamir-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:38:29.000000 pyshamir-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-03 16:38:18.000000 pyshamir-1.0.2/tests/test_shamir.py
```

### Comparing `pyshamir-1.0.1/PKG-INFO` & `pyshamir-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshamir
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python port of Shamir key Split and Combine methods from Hashicorp Vault.
 Home-page: https://github.com/konidev20/pyshamir
 Author: Srigovind Nayak
 Author-email: sgovind.dev@outlook.com
 Maintainer: Srigovind Nayak
 Maintainer-email: sgovind.dev@outlook.com
 Project-URL: Documentation, https://github.com/konidev20/pyshamir
@@ -20,22 +20,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# pyshamir
+![pyshamir banner](https://user-images.githubusercontent.com/5201843/232241639-22034903-87c2-4bf0-9b36-2ae9a8481b71.png)
 
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=coverage)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/konidev20/pyshamir/badge)](https://api.securityscorecards.dev/projects/github.com/konidev20/pyshamir)
+
+## Description
 
 Python port of Shamir key Split and Combine methods from Hashicorp Vault.
 
 ## Installation
 
 ```sh
 pip install pyshamir
```

### Comparing `pyshamir-1.0.1/README.md` & `pyshamir-1.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-# pyshamir
+![pyshamir banner](https://user-images.githubusercontent.com/5201843/232241639-22034903-87c2-4bf0-9b36-2ae9a8481b71.png)
 
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=coverage)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/konidev20/pyshamir/badge)](https://api.securityscorecards.dev/projects/github.com/konidev20/pyshamir)
+
+## Description
 
 Python port of Shamir key Split and Combine methods from Hashicorp Vault.
 
 ## Installation
 
 ```sh
 pip install pyshamir
```

### Comparing `pyshamir-1.0.1/pyshamir/_utils.py` & `pyshamir-1.0.2/pyshamir/_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 import secrets
-from ._constants import LOG_TABLE, EXP_TABLE
+from ctypes import c_uint8
 
 def add(a, b)->int:
     """
     Adds two numbers in the finite field GF(256)
     """
     out = a ^ b
     return out
 
-def mul(a, b)->int:
-    """
-    Multiplies two numbers in the finite field GF(256)
-    """
-    log_a = LOG_TABLE[a]
-    log_b = LOG_TABLE[b]
-    log_sum = (int(log_a) + int(log_b)) % 255
-    ret = int(EXP_TABLE[log_sum])
 
-    if a == 0 or b == 0:
-        return 0
-    
-    return int(ret)
+def inverse(a):
+    b = mul(a, a)
+    c = mul(a, b)
+    b = mul(c, c)
+    b = mul(b, b)
+    c = mul(b, c)
+    b = mul(b, b)
+    b = mul(b, b)
+    b = mul(b, c)
+    b = mul(b, b)
+    b = mul(a, b)
+    return mul(b, b)
+
+
+def mul(a, b):
+    a = c_uint8(a)
+    b = c_uint8(b)
+    r = c_uint8(0)
+    i = 8
+
+    while i > 0:
+        i -= 1
+        p1 = (-(c_uint8(b.value >> i).value & 1) & a.value)
+        p2 = (-(c_uint8(r.value >> 7).value) & 0x1B)
+        p3 = c_uint8(2* r.value)
+        r = c_uint8(p1 ^ p2 ^ p3.value)
+
+    return r.value
+
 
 def div(a, b)->int:
-    """
-    Divides two numbers in the finite field GF(256)
-    """
-    if b == 0:
+    a = c_uint8(a)
+    b = c_uint8(b)
+
+    if b.value == 0:
         raise ZeroDivisionError("Divide by zero")
-    log_a = LOG_TABLE[a]
-    log_b = LOG_TABLE[b]
-    diff = ((int(log_a) - int(log_b)) + 255) % 255
-    ret = int(EXP_TABLE[diff])
+    ret = mul(a.value,inverse(b.value))
 
-    if a == 0:
+    if a.value == 0:
         return 0
 
-    return int(ret)
+    return ret
 
 class Polynomial:
     """
     Takes N sample points and returns the value of the polynomial at x using Lagrange interpolation
     """
     def __init__(self, degree):
         self.coefficients = bytearray(degree + 1)
```

### Comparing `pyshamir-1.0.1/pyshamir/shamir.py` & `pyshamir-1.0.2/pyshamir/shamir.py`

 * *Files identical despite different names*

### Comparing `pyshamir-1.0.1/pyshamir.egg-info/PKG-INFO` & `pyshamir-1.0.2/pyshamir.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshamir
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python port of Shamir key Split and Combine methods from Hashicorp Vault.
 Home-page: https://github.com/konidev20/pyshamir
 Author: Srigovind Nayak
 Author-email: sgovind.dev@outlook.com
 Maintainer: Srigovind Nayak
 Maintainer-email: sgovind.dev@outlook.com
 Project-URL: Documentation, https://github.com/konidev20/pyshamir
@@ -20,22 +20,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# pyshamir
+![pyshamir banner](https://user-images.githubusercontent.com/5201843/232241639-22034903-87c2-4bf0-9b36-2ae9a8481b71.png)
 
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=konidev20_pyshamir&metric=coverage)](https://sonarcloud.io/summary/new_code?id=konidev20_pyshamir)
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/konidev20/pyshamir/badge)](https://api.securityscorecards.dev/projects/github.com/konidev20/pyshamir)
+
+## Description
 
 Python port of Shamir key Split and Combine methods from Hashicorp Vault.
 
 ## Installation
 
 ```sh
 pip install pyshamir
```

### Comparing `pyshamir-1.0.1/setup.cfg` & `pyshamir-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyshamir-1.0.1/tests/test_shamir.py` & `pyshamir-1.0.2/tests/test_shamir.py`

 * *Files identical despite different names*

