# Comparing `tmp/VMedNLP-1.0.0-py38-none-any.whl.zip` & `tmp/VMedNLP-1.1.0-py38-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,8 @@
-Zip file size: 13897 bytes, number of entries: 7
--rw-------  2.0 unx      139 b- defN 23-Jun-12 10:44 VMedNLP/__init__.pyc
--rw-------  2.0 unx    19235 b- defN 23-Jun-12 10:44 VMedNLP/medToolkit.pyc
--rw-------  2.0 unx     3013 b- defN 23-Jun-12 10:44 VMedNLP/models.pyc
--rw-------  2.0 unx    13070 b- defN 23-Jun-12 10:44 VMedNLP-1.0.0.dist-info/METADATA
--rw-------  2.0 unx       82 b- defN 23-Jun-12 10:44 VMedNLP-1.0.0.dist-info/WHEEL
--rw-------  2.0 unx        8 b- defN 23-Jun-12 10:44 VMedNLP-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      529 b- defN 23-Jun-12 10:44 VMedNLP-1.0.0.dist-info/RECORD
-7 files, 36076 bytes uncompressed, 12967 bytes compressed:  64.1%
+Zip file size: 5770 bytes, number of entries: 6
+-rw-------  2.0 unx      139 b- defN 23-Jul-03 12:36 VMedNLP/__init__.pyc
+-rw-------  2.0 unx     3013 b- defN 23-Jul-03 12:36 VMedNLP/models.pyc
+-rw-------  2.0 unx    13070 b- defN 23-Jul-03 12:36 VMedNLP-1.1.0.dist-info/METADATA
+-rw-------  2.0 unx       82 b- defN 23-Jul-03 12:36 VMedNLP-1.1.0.dist-info/WHEEL
+-rw-------  2.0 unx        8 b- defN 23-Jul-03 12:36 VMedNLP-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      449 b- defN 23-Jul-03 12:36 VMedNLP-1.1.0.dist-info/RECORD
+6 files, 16761 bytes uncompressed, 4960 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -1,22 +1,19 @@
 Filename: VMedNLP/__init__.pyc
 Comment: 
 
-Filename: VMedNLP/medToolkit.pyc
-Comment: 
-
 Filename: VMedNLP/models.pyc
 Comment: 
 
-Filename: VMedNLP-1.0.0.dist-info/METADATA
+Filename: VMedNLP-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: VMedNLP-1.0.0.dist-info/WHEEL
+Filename: VMedNLP-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: VMedNLP-1.0.0.dist-info/top_level.txt
+Filename: VMedNLP-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: VMedNLP-1.0.0.dist-info/RECORD
+Filename: VMedNLP-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## VMedNLP/__init__.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May 15 06:22:10 2023 UTC, .py size: 0 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 92cf 6164 0000 0000  U.........ad....
+00000000: 550d 0d0a 0000 0000 655b 8964 0000 0000  U.......e[.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0400 0000 6400  .....@...s....d.
 00000030: 5300 2901 4ea9 0072 0100 0000 7201 0000  S.).N..r....r...
 00000040: 0072 0100 0000 fa30 6275 696c 642f 6264  .r.....0build/bd
 00000050: 6973 742e 6c69 6e75 782d 7838 365f 3634  ist.linux-x86_64
 00000060: 2f65 6767 2f56 4d65 644e 4c50 2f5f 5f69  /egg/VMedNLP/__i
 00000070: 6e69 745f 5f2e 7079 da08 3c6d 6f64 756c  nit__.py..<modul
```

## VMedNLP/models.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed May 17 09:59:42 2023 UTC, .py size: 4021 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 8ea5 6464 b50f 0000  U.........dd....
+00000000: 550d 0d0a 0000 0000 655b 8964 b50f 0000  U.......e[.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4e02 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6401 6c04  ..d.d.l.Z.d.d.l.
 00000050: 5a04 6403 6404 8400 5a05 6504 6a06 a007  Z.d.d...Z.e.j...
 00000060: 6504 6a06 a008 6509 a101 a101 5a0a 6504  e.j...e.....Z.e.
 00000070: 6a06 a00b 650a 6405 a102 5a0c 6504 6a0d  j...e.d...Z.e.j.
```

## Comparing `VMedNLP-1.0.0.dist-info/METADATA` & `VMedNLP-1.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VMedNLP
-Version: 1.0.0
+Version: 1.1.0
 Summary: Medical NLP Toolkit
 Author: vLife|Virtusa
 Author-email: vlife@virtusa.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -20,15 +20,15 @@
 Requires-Dist: scispacy (==0.5.1)
 Requires-Dist: pyMupdf
 Requires-Dist: pydicom
 Requires-Dist: presidio-analyzer
 Requires-Dist: presidio-image-redactor
 Requires-Dist: pytesseract
 
-# vLife | Virtusa - vMedNLP
+# vLife | Virtusa - VMedNLP
 
 #### A comprehensive, user-friendly toolkit designed completely using opensource models that would aid users in performing NLP-related tasks such as entity identification, extraction, and deidentification from clinical notes, medical images, and documents.
 
 ## Basic Library Import
 ```
 from VMedNLP import models
 ```
```

