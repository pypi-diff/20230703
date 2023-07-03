# Comparing `tmp/fusionprov-1.2.1-py3-none-any.whl.zip` & `tmp/fusionprov-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 15874 bytes, number of entries: 10
--rw-r--r--  2.0 unx      794 b- defN 23-Jun-23 13:39 fusionprov/__init__.py
+Zip file size: 15861 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      794 b- defN 23-Jul-03 12:23 fusionprov/__init__.py
 -rw-r--r--  2.0 unx     9390 b- defN 23-Jun-22 10:40 fusionprov/imasprov.py
--rw-r--r--  2.0 unx    20670 b- defN 23-Jun-23 11:57 fusionprov/mastprov.py
+-rw-r--r--  2.0 unx    20659 b- defN 23-Jul-03 12:11 fusionprov/mastprov.py
 -rw-r--r--  2.0 unx      749 b- defN 23-Jun-22 10:40 fusionprov/utilities.py
--rw-r--r--  2.0 unx    11345 b- defN 23-Jun-23 13:41 fusionprov-1.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4927 b- defN 23-Jun-23 13:41 fusionprov-1.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 13:41 fusionprov-1.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       91 b- defN 23-Jun-23 13:41 fusionprov-1.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 13:41 fusionprov-1.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      816 b- defN 23-Jun-23 13:41 fusionprov-1.2.1.dist-info/RECORD
-10 files, 48885 bytes uncompressed, 14480 bytes compressed:  70.4%
+-rw-r--r--  2.0 unx    11345 b- defN 23-Jul-03 12:28 fusionprov-1.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4927 b- defN 23-Jul-03 12:28 fusionprov-1.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 12:28 fusionprov-1.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       91 b- defN 23-Jul-03 12:28 fusionprov-1.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-03 12:28 fusionprov-1.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      816 b- defN 23-Jul-03 12:28 fusionprov-1.2.2.dist-info/RECORD
+10 files, 48874 bytes uncompressed, 14467 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: fusionprov/mastprov.py
 Comment: 
 
 Filename: fusionprov/utilities.py
 Comment: 
 
-Filename: fusionprov-1.2.1.dist-info/LICENSE
+Filename: fusionprov-1.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: fusionprov-1.2.1.dist-info/METADATA
+Filename: fusionprov-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: fusionprov-1.2.1.dist-info/WHEEL
+Filename: fusionprov-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: fusionprov-1.2.1.dist-info/entry_points.txt
+Filename: fusionprov-1.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: fusionprov-1.2.1.dist-info/top_level.txt
+Filename: fusionprov-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: fusionprov-1.2.1.dist-info/RECORD
+Filename: fusionprov-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fusionprov/__init__.py

```diff
@@ -15,8 +15,8 @@
 try:
     from .mastprov import write_provenance
 except ModuleNotFoundError as error:
     logging.info(f"{error}. A UDA installation is required write provenance for MAST signals.")
 except ImportError as error:
     logging.info(f"{error}. A UDA installation is required write provenance for MAST signals.")
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
```

## fusionprov/mastprov.py

```diff
@@ -274,17 +274,16 @@
 
     def get_log(self, file_code=None):
         """
         Retrieves the log file for the signal as a string.
         """
         if not file_code:
             file_code = self.data
-        filename = f"{file_code}_0{self.shot}.log"
-        path = f"/net/raidsrvr/data/MAST_Data/{self.shot}/Pass{self.run}/{filename}"
-
+        filename = f"{file_code.lower()}_0{self.shot}.log"
+        path = f"$MAST_DATA/{self.shot}/Pass{self.run}/{filename}"
         if FREIA:
             log = self.client.get_text(path)
         else:
             signal = f'TESTPLUGIN::nathan(filename="{path}")'
             log = self.client.get(signal, "", raw=True).str
 
         return log
```

## Comparing `fusionprov-1.2.1.dist-info/LICENSE` & `fusionprov-1.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fusionprov-1.2.1.dist-info/METADATA` & `fusionprov-1.2.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionprov
-Version: 1.2.1
+Version: 1.2.2
 Summary: A python package for retrieving and documenting the provenance of fusion data.
 Home-page: https://gitlab.com/fair-for-fusion/fusionprov
 Author: Nathan Cummings
 Author-email: nathan.cummings@ukaea.uk
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `fusionprov-1.2.1.dist-info/RECORD` & `fusionprov-1.2.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-fusionprov/__init__.py,sha256=Xh9oK53lcpcnWVDQ57_CIqc_FcDpprIE7Rocv3iIpjI,794
+fusionprov/__init__.py,sha256=4MtIBAWUHEZpzzr4frTXRZEC5qoDvznEaH43pKcw5S0,794
 fusionprov/imasprov.py,sha256=zHWNdcn7aSgR5JibUiDaCb95yUN9HmcR8uRXniLI43c,9390
-fusionprov/mastprov.py,sha256=JFS-6csuVvA5tiKFVWgWDrOLeZ0x3Dt0jv37lwmvYfo,20670
+fusionprov/mastprov.py,sha256=azKhnEJOWAhqindlSuaX-BZ6yUYXJeTM5p_rQLHhCMk,20659
 fusionprov/utilities.py,sha256=cq0xU4rErDMSVWc0uBNxboXsMyE84lsz1I20yCGxI5M,749
-fusionprov-1.2.1.dist-info/LICENSE,sha256=nWy-cQl2dVZGb5nuNnCIKy23ToY1xnb0oJ8tUmtrKUc,11345
-fusionprov-1.2.1.dist-info/METADATA,sha256=4tVuitu8P6rGHkWjlfStGANfLqWpsY27VbtbRq1vEjY,4927
-fusionprov-1.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fusionprov-1.2.1.dist-info/entry_points.txt,sha256=l116zSk3D6w87ZQ2JUvMzY32bp3nYWAqJJExuXlQeZ4,91
-fusionprov-1.2.1.dist-info/top_level.txt,sha256=zUlig65HQFDHJG-3DhxRFEpTQ9g2KthDgSQL89j0bAI,11
-fusionprov-1.2.1.dist-info/RECORD,,
+fusionprov-1.2.2.dist-info/LICENSE,sha256=nWy-cQl2dVZGb5nuNnCIKy23ToY1xnb0oJ8tUmtrKUc,11345
+fusionprov-1.2.2.dist-info/METADATA,sha256=sHHSsS36aZm9uBbCY5_pKWv3hGPyXLlU2bcignqgK4M,4927
+fusionprov-1.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fusionprov-1.2.2.dist-info/entry_points.txt,sha256=l116zSk3D6w87ZQ2JUvMzY32bp3nYWAqJJExuXlQeZ4,91
+fusionprov-1.2.2.dist-info/top_level.txt,sha256=zUlig65HQFDHJG-3DhxRFEpTQ9g2KthDgSQL89j0bAI,11
+fusionprov-1.2.2.dist-info/RECORD,,
```

