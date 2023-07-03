# Comparing `tmp/PyFGHTest-0.0.1-py3-none-any.whl.zip` & `tmp/PyFGHTest-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1525 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-03 15:27 PyFGHTest/__init__.py
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-03 15:22 PyFGHTest/test.py
--rw-rw-rw-  2.0 fat      645 b- defN 23-Jul-03 15:32 PyFGHTest-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-03 15:32 PyFGHTest-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-03 15:32 PyFGHTest-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      452 b- defN 23-Jul-03 15:32 PyFGHTest-0.0.1.dist-info/RECORD
-6 files, 1217 bytes uncompressed, 699 bytes compressed:  42.6%
+Zip file size: 1530 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-03 15:37 PyFGHTest/__init__.py
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-03 15:38 PyFGHTest/main.py
+-rw-rw-rw-  2.0 fat      645 b- defN 23-Jul-03 15:41 PyFGHTest-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-03 15:41 PyFGHTest-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-03 15:41 PyFGHTest-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      452 b- defN 23-Jul-03 15:41 PyFGHTest-0.0.2.dist-info/RECORD
+6 files, 1219 bytes uncompressed, 704 bytes compressed:  42.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: PyFGHTest/__init__.py
 Comment: 
 
-Filename: PyFGHTest/test.py
+Filename: PyFGHTest/main.py
 Comment: 
 
-Filename: PyFGHTest-0.0.1.dist-info/METADATA
+Filename: PyFGHTest-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: PyFGHTest-0.0.1.dist-info/WHEEL
+Filename: PyFGHTest-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: PyFGHTest-0.0.1.dist-info/top_level.txt
+Filename: PyFGHTest-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: PyFGHTest-0.0.1.dist-info/RECORD
+Filename: PyFGHTest-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `PyFGHTest-0.0.1.dist-info/METADATA` & `PyFGHTest-0.0.2.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFGHTest
-Version: 0.0.1
+Version: 0.0.2
 Summary: PyFGH Test library
 Author: Josiah Randleman, Nelson Maxey, Tyler Law, Dr. Jeffrey Woodford
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

