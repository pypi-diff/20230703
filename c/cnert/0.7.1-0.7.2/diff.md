# Comparing `tmp/cnert-0.7.1.tar.gz` & `tmp/cnert-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnert-0.7.1.tar", max compression
+gzip compressed data, was "cnert-0.7.2.tar", max compression
```

## Comparing `cnert-0.7.1.tar` & `cnert-0.7.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.7.1/LICENSE
--rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.7.1/LICENSE.apache2
--rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.7.1/LICENSE.mit
--rw-r--r--   0        0        0     7748 2023-05-10 14:30:59.900805 cnert-0.7.1/README.md
--rw-r--r--   0        0        0     3150 2023-06-05 11:18:50.120161 cnert-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    26231 2023-06-05 11:18:50.151985 cnert-0.7.1/src/cnert/__init__.py
--rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.7.1/src/cnert/py.typed
--rw-r--r--   0        0        0     9512 1970-01-01 00:00:00.000000 cnert-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.7.2/LICENSE
+-rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.7.2/LICENSE.apache2
+-rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.7.2/LICENSE.mit
+-rw-r--r--   0        0        0     7748 2023-05-10 14:30:59.900805 cnert-0.7.2/README.md
+-rw-r--r--   0        0        0     3150 2023-07-03 15:17:00.331762 cnert-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    26269 2023-07-03 15:17:00.361496 cnert-0.7.2/src/cnert/__init__.py
+-rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.7.2/src/cnert/py.typed
+-rw-r--r--   0        0        0     9312 1970-01-01 00:00:00.000000 cnert-0.7.2/PKG-INFO
```

### Comparing `cnert-0.7.1/LICENSE.apache2` & `cnert-0.7.2/LICENSE.apache2`

 * *Files identical despite different names*

### Comparing `cnert-0.7.1/LICENSE.mit` & `cnert-0.7.2/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `cnert-0.7.1/README.md` & `cnert-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `cnert-0.7.1/pyproject.toml` & `cnert-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cnert"
-version = "0.7.1"
+version = "0.7.2"
 description = "Cnert is trying to be a simple API for creating TLS Certificates testing purposes."
 authors = ["Maarten <ikmaarten@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/maartenq/cnert"
 repository = "https://github.com/maartenq/cnert"
 documentation = "https://cnert.readthedocs.io/en/latest/"
```

### Comparing `cnert-0.7.1/src/cnert/__init__.py` & `cnert-0.7.2/src/cnert/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # cnert/__init__.py
 
 from __future__ import annotations  # for Python 3.7-3.9
 
 from datetime import datetime, timedelta
 from ipaddress import ip_address, ip_network
+from typing import ClassVar
 
 import idna
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.x509.oid import ExtendedKeyUsageOID, NameOID
 
 """
 Cnert makes TLS private keys, CSRs, private CAs and certificates.
 """
 
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 __title__ = "Cnert"
 __description__ = (
     "Cnert makes TLS private keys, CSRs, private CAs and certificates."
 )
 __uri__ = "https://github.com/maartenq/cnert"
 __author__ = "Maarten"
 __email__ = "ikmaarten@gmail.com"
@@ -80,15 +81,15 @@
 
 
 class Freezer:
     """
     Freeze any class such that instantiated objects become immutable.
     """
 
-    __slots__: list[str] = []
+    __slots__: ClassVar[list[str]] = []
     _frozen: bool = False
 
     def __init__(self):
         for attr_name in dir(self):
             self.__slots__.append(attr_name)
         self._frozen = True
```

### Comparing `cnert-0.7.1/PKG-INFO` & `cnert-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnert
-Version: 0.7.1
+Version: 0.7.2
 Summary: Cnert is trying to be a simple API for creating TLS Certificates testing purposes.
 Home-page: https://github.com/maartenq/cnert
 License: MIT
 Keywords: certificate,X.509,TLS,cryptography,testing
 Author: Maarten
 Author-email: ikmaarten@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -17,19 +17,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Requires-Dist: cryptography (>=41.0.0,<42.0.0)
 Requires-Dist: idna (>=3.3,<4.0)
```

