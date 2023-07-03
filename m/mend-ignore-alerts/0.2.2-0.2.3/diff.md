# Comparing `tmp/mend_ignore_alerts-0.2.2-py3-none-any.whl.zip` & `tmp/mend_ignore_alerts-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11809 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 17:10 mend_ignore_alerts/__init__.py
--rw-r--r--  2.0 unx      107 b- defN 23-Jul-02 17:10 mend_ignore_alerts/_version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 17:10 mend_ignore_alerts/conftest.py
--rw-r--r--  2.0 unx     1554 b- defN 23-Jul-02 17:10 mend_ignore_alerts/const.py
--rw-r--r--  2.0 unx    10673 b- defN 23-Jul-02 17:10 mend_ignore_alerts/ignore_alerts.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-02 17:11 mend_ignore_alerts-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     5250 b- defN 23-Jul-02 17:11 mend_ignore_alerts-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 17:11 mend_ignore_alerts-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Jul-02 17:11 mend_ignore_alerts-0.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-02 17:11 mend_ignore_alerts-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      979 b- defN 23-Jul-02 17:11 mend_ignore_alerts-0.2.2.dist-info/RECORD
-11 files, 30103 bytes uncompressed, 10117 bytes compressed:  66.4%
+Zip file size: 11948 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 08:04 mend_ignore_alerts/__init__.py
+-rw-r--r--  2.0 unx      107 b- defN 23-Jul-03 08:04 mend_ignore_alerts/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 08:04 mend_ignore_alerts/conftest.py
+-rw-r--r--  2.0 unx     1554 b- defN 23-Jul-03 08:04 mend_ignore_alerts/const.py
+-rw-r--r--  2.0 unx    10673 b- defN 23-Jul-03 08:04 mend_ignore_alerts/ignore_alerts.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-03 08:04 mend_ignore_alerts-0.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5030 b- defN 23-Jul-03 08:04 mend_ignore_alerts-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 08:04 mend_ignore_alerts-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jul-03 08:04 mend_ignore_alerts-0.2.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-03 08:04 mend_ignore_alerts-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      979 b- defN 23-Jul-03 08:04 mend_ignore_alerts-0.2.3.dist-info/RECORD
+11 files, 29883 bytes uncompressed, 10256 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: mend_ignore_alerts/const.py
 Comment: 
 
 Filename: mend_ignore_alerts/ignore_alerts.py
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.2.dist-info/LICENSE
+Filename: mend_ignore_alerts-0.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.2.dist-info/METADATA
+Filename: mend_ignore_alerts-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.2.dist-info/WHEEL
+Filename: mend_ignore_alerts-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.2.dist-info/entry_points.txt
+Filename: mend_ignore_alerts-0.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.2.dist-info/top_level.txt
+Filename: mend_ignore_alerts-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.2.dist-info/RECORD
+Filename: mend_ignore_alerts-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_ignore_alerts/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 __tool_name__ = "ignore_alerts"
 __description__ = "Parse yml file and update alerts"
```

## Comparing `mend_ignore_alerts-0.2.2.dist-info/LICENSE` & `mend_ignore_alerts-0.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_ignore_alerts-0.2.2.dist-info/RECORD` & `mend_ignore_alerts-0.2.3.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mend_ignore_alerts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mend_ignore_alerts/_version.py,sha256=sgUoIkAzzAZN0kmMa245HjNk3cgZrn5b053E8Ban0Wg,107
+mend_ignore_alerts/_version.py,sha256=tdDSzTdcjTFoV2BbgFNb9liCaapuzTZYR7rgPlR7DdA,107
 mend_ignore_alerts/conftest.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mend_ignore_alerts/const.py,sha256=aRDadkUul_6NZB_LDIZTkGf5VkWTPqfnj6eap-1Y7As,1554
 mend_ignore_alerts/ignore_alerts.py,sha256=DWhEp-fVihaQYfcG9btezfxFcvWr9tm8WLuC307DqJs,10673
-mend_ignore_alerts-0.2.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mend_ignore_alerts-0.2.2.dist-info/METADATA,sha256=V3K_x8rEsS2UYl4kN8BAF5um30QawXU1aqNcq7-QcVk,5250
-mend_ignore_alerts-0.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mend_ignore_alerts-0.2.2.dist-info/entry_points.txt,sha256=b_q3jF-WbTVm6sR0BrVXts8u1OhXtD1aM2IZ5CfWmpE,72
-mend_ignore_alerts-0.2.2.dist-info/top_level.txt,sha256=ookvTXlTz4JKFzjrBd6U6MmV6RzYs9C8B2E2vMscaZ8,19
-mend_ignore_alerts-0.2.2.dist-info/RECORD,,
+mend_ignore_alerts-0.2.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mend_ignore_alerts-0.2.3.dist-info/METADATA,sha256=cxZGTYfiaPvpPJEEbZNjWTaiRLECyVWctzj8z0jxChY,5030
+mend_ignore_alerts-0.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mend_ignore_alerts-0.2.3.dist-info/entry_points.txt,sha256=b_q3jF-WbTVm6sR0BrVXts8u1OhXtD1aM2IZ5CfWmpE,72
+mend_ignore_alerts-0.2.3.dist-info/top_level.txt,sha256=ookvTXlTz4JKFzjrBd6U6MmV6RzYs9C8B2E2vMscaZ8,19
+mend_ignore_alerts-0.2.3.dist-info/RECORD,,
```

