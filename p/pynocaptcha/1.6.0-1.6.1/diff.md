# Comparing `tmp/pynocaptcha-1.6.0.tar.gz` & `tmp/pynocaptcha-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynocaptcha-1.6.0.tar", last modified: Wed Jun 28 09:30:02 2023, max compression
+gzip compressed data, was "dist/pynocaptcha-1.6.1.tar", last modified: Mon Jul  3 06:08:31 2023, max compression
```

## Comparing `pynocaptcha-1.6.0.tar` & `pynocaptcha-1.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-28 09:30:02.000000 pynocaptcha-1.6.0/
--rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-06-28 09:30:02.000000 pynocaptcha-1.6.0/PKG-INFO
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-28 09:30:02.000000 pynocaptcha-1.6.0/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)      630 2023-06-14 09:34:47.000000 pynocaptcha-1.6.0/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-28 09:30:02.000000 pynocaptcha-1.6.0/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)     1055 2023-06-19 12:27:32.000000 pynocaptcha-1.6.0/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)     4785 2023-06-15 08:58:13.000000 pynocaptcha-1.6.0/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.6.0/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1187 2023-06-28 06:35:47.000000 pynocaptcha-1.6.0/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)   222287 2023-06-28 09:28:19.000000 pynocaptcha-1.6.0/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.6.0/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1639 2023-06-15 08:25:19.000000 pynocaptcha-1.6.0/pynocaptcha/crackers/tls.py
--rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-06-28 09:29:31.000000 pynocaptcha-1.6.0/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-07-03 06:08:31.000000 pynocaptcha-1.6.1/
+-rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-07-03 06:08:31.000000 pynocaptcha-1.6.1/PKG-INFO
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-07-03 06:08:31.000000 pynocaptcha-1.6.1/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)      630 2023-06-14 09:34:47.000000 pynocaptcha-1.6.1/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-07-03 06:08:31.000000 pynocaptcha-1.6.1/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1055 2023-06-19 12:27:32.000000 pynocaptcha-1.6.1/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     4785 2023-06-15 08:58:13.000000 pynocaptcha-1.6.1/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.6.1/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1221 2023-07-03 06:08:01.000000 pynocaptcha-1.6.1/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)   222301 2023-07-03 06:06:27.000000 pynocaptcha-1.6.1/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.6.1/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1639 2023-06-15 08:25:19.000000 pynocaptcha-1.6.1/pynocaptcha/crackers/tls.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-07-03 06:08:16.000000 pynocaptcha-1.6.1/setup.py
```

### Comparing `pynocaptcha-1.6.0/PKG-INFO` & `pynocaptcha-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pynocaptcha
-Version: 1.6.0
+Version: 1.6.1
 Summary: nocaptcha.io api
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: nocaptcha.io python api
 Keywords: nocaptcha
```

### Comparing `pynocaptcha-1.6.0/pynocaptcha/__init__.py` & `pynocaptcha-1.6.1/pynocaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.6.0/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.6.1/pynocaptcha/crackers/akamai.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.6.0/pynocaptcha/crackers/base.py` & `pynocaptcha-1.6.1/pynocaptcha/crackers/base.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.6.0/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.6.1/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.6.0/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.6.1/pynocaptcha/crackers/hcaptcha.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,10 +30,11 @@
     
     # 必传参数
     must_check_params = ["sitekey", "referer"]
     # 默认可选参数
     option_params = {
         "mode": "picture",   # 验证模式, 默认图片验证, 可选 question 题库验证
         "rqdata": "",
+        "domain": "hcaptcha.com",
         "device": "chrome",
     }
```

### Comparing `pynocaptcha-1.6.0/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.6.1/pynocaptcha/crackers/incapsula.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,13 +54,13 @@
         # proxy=proxy,
         # submit=False
     )
     ret = cracker.crack()
     """
     
     # 必传参数
-    must_check_params = ["href", "cookies"]
+    must_check_params = ["href", "cookies", "user_agent"]
     # 可选参数
     option_params = {
         "proxy": "",
         "submit": False
     }
```

### Comparing `pynocaptcha-1.6.0/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.6.1/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.6.0/pynocaptcha/crackers/tls.py` & `pynocaptcha-1.6.1/pynocaptcha/crackers/tls.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.6.0/setup.py` & `pynocaptcha-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 
 setup(
     name='pynocaptcha',
-    version='1.6.0',
+    version='1.6.1',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

