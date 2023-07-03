# Comparing `tmp/dms_collector-2.0.4-py3-none-any.whl.zip` & `tmp/dms_collector-2.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9728 bytes, number of entries: 8
+Zip file size: 9780 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      451 b- defN 23-May-30 08:20 dms_collector/__init__.py
 -rw-r--r--  2.0 unx     7628 b- defN 23-May-30 09:15 dms_collector/__main__.py
--rw-r--r--  2.0 unx    10164 b- defN 23-May-30 08:49 dms_collector/dms.py
--rwxr-xr-x  2.0 unx      106 b- defN 22-Jan-07 20:33 dms_collector-2.0.4.data/scripts/dms-collector
--rw-r--r--  2.0 unx     5115 b- defN 23-May-30 20:38 dms_collector-2.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-30 20:38 dms_collector-2.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-May-30 20:38 dms_collector-2.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      665 b- defN 23-May-30 20:38 dms_collector-2.0.4.dist-info/RECORD
-8 files, 24235 bytes uncompressed, 8562 bytes compressed:  64.7%
+-rw-r--r--  2.0 unx    10375 b- defN 23-Jul-03 13:04 dms_collector/dms.py
+-rwxr-xr-x  2.0 unx      106 b- defN 22-Jan-07 20:33 dms_collector-2.0.5.data/scripts/dms-collector
+-rw-r--r--  2.0 unx     5115 b- defN 23-Jul-03 13:07 dms_collector-2.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 13:07 dms_collector-2.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-03 13:07 dms_collector-2.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      665 b- defN 23-Jul-03 13:07 dms_collector-2.0.5.dist-info/RECORD
+8 files, 24446 bytes uncompressed, 8614 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: dms_collector/__main__.py
 Comment: 
 
 Filename: dms_collector/dms.py
 Comment: 
 
-Filename: dms_collector-2.0.4.data/scripts/dms-collector
+Filename: dms_collector-2.0.5.data/scripts/dms-collector
 Comment: 
 
-Filename: dms_collector-2.0.4.dist-info/METADATA
+Filename: dms_collector-2.0.5.dist-info/METADATA
 Comment: 
 
-Filename: dms_collector-2.0.4.dist-info/WHEEL
+Filename: dms_collector-2.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: dms_collector-2.0.4.dist-info/top_level.txt
+Filename: dms_collector-2.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: dms_collector-2.0.4.dist-info/RECORD
+Filename: dms_collector-2.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dms_collector/dms.py

```diff
@@ -3,14 +3,15 @@
 import os
 
 import xml.etree.ElementTree as ET
 
 import urllib3
 import requests
 
+from xml.etree.ElementTree import ParseError
 from importlib.metadata import version, PackageNotFoundError
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 TBML_VERSIONS = ["11.0"]
 
 # DMS REQESTS URLs
@@ -264,19 +265,22 @@
         Retrieves the DMS table as a list of dict where a dict represents a row with fields and values.
         The `include` parameter provides a list of fields that should be included in the result, the `exclude` parameter
         provides a list of fields that should be excluded from the result and `filter` defines a Python expression
         that is used to filter our the table rows. The expression can contain conditions with table fields.
         """
         start_time = time.time()
 
-        header = self.get_header(table, check_tbl_version)
-        root, _ = self.retrieve_data(
-            DMSREQUEST_DATA % (self.admin_url, table),
-            check_tbl_version=check_tbl_version,
-        )
+        try:
+            header = self.get_header(table, check_tbl_version)
+            root, _ = self.retrieve_data(
+                DMSREQUEST_DATA % (self.admin_url, table),
+                check_tbl_version=check_tbl_version,
+            )
+        except ParseError as e:
+            raise Exception(f"Cannot parse table data '{table}'. The data is empty or invalid. {e}")
 
         rows = []
         for rw in root.findall(".//row"):
             row = {}
             for key in header.keys():
                 nkey = normalize(key, preserve_orig_header=preserve_orig_header)
                 if (nkey not in exclude and len(include) == 0) or nkey in include:
```

## Comparing `dms_collector-2.0.4.dist-info/METADATA` & `dms_collector-2.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-collector
-Version: 2.0.4
+Version: 2.0.5
 Summary: Oracle FMW DMS Spy collector utility
 Home-page: UNKNOWN
 Author: Tomas Vitvar
 Author-email: tomas@vitvar.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `dms_collector-2.0.4.dist-info/RECORD` & `dms_collector-2.0.5.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 dms_collector/__init__.py,sha256=yQrVBot8RKv4KqwICcs-5P9Be1yttUxnuo969dfgfls,451
 dms_collector/__main__.py,sha256=aH4hFgtYh8ZThlwQGTO2RUKtHBpe71ZWtARzH2-lhgk,7628
-dms_collector/dms.py,sha256=GFRAFtbSYdCspEGQubZAzofoAAgGtUVPWQ5wN1SYBbI,10164
-dms_collector-2.0.4.data/scripts/dms-collector,sha256=sjr-8lKbIKcth2XQo-EJoxwP7gT2MKDSxwSnNDSoOF8,106
-dms_collector-2.0.4.dist-info/METADATA,sha256=SYCxZJRAKlmkEtApjmRYfVCpIY8oFzm6jbREgGGE8Ok,5115
-dms_collector-2.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-dms_collector-2.0.4.dist-info/top_level.txt,sha256=RuQQjBW50aAGTJtqCZ82BNqd1M-Rmvd_rYrG7UeV-9E,14
-dms_collector-2.0.4.dist-info/RECORD,,
+dms_collector/dms.py,sha256=VsFvtygO6Uaxz_7fqSLhqfztlXNjbDD82Pc3qetytmE,10375
+dms_collector-2.0.5.data/scripts/dms-collector,sha256=sjr-8lKbIKcth2XQo-EJoxwP7gT2MKDSxwSnNDSoOF8,106
+dms_collector-2.0.5.dist-info/METADATA,sha256=UHl03CJJDuIEHsBJ85adiyv5gm7L42kY49sObVUtYb4,5115
+dms_collector-2.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+dms_collector-2.0.5.dist-info/top_level.txt,sha256=RuQQjBW50aAGTJtqCZ82BNqd1M-Rmvd_rYrG7UeV-9E,14
+dms_collector-2.0.5.dist-info/RECORD,,
```

