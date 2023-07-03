# Comparing `tmp/e2eqavn-0.1.6-py2.py3-none-any.whl.zip` & `tmp/e2eqavn-0.1.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 37581 bytes, number of entries: 40
--rw-rw-r--  2.0 unx      498 b- defN 23-Jul-03 15:42 e2eqavn/__init__.py
+Zip file size: 38774 bytes, number of entries: 40
+-rw-rw-r--  2.0 unx      498 b- defN 23-Jul-03 15:47 e2eqavn/__init__.py
 -rw-rw-r--  2.0 unx    10774 b- defN 23-Jul-01 11:37 e2eqavn/cli.py
 -rw-rw-r--  2.0 unx     2716 b- defN 23-Jul-01 11:37 e2eqavn/keywords.py
 -rw-rw-r--  2.0 unx     3639 b- defN 23-Jul-01 11:37 e2eqavn/datasets/MRCDataset.py
 -rw-rw-r--  2.0 unx     1386 b- defN 23-Jul-01 11:32 e2eqavn/datasets/TripletDataset.py
 -rw-rw-r--  2.0 unx      124 b- defN 23-Jul-01 11:32 e2eqavn/datasets/__init__.py
 -rw-rw-r--  2.0 unx     3814 b- defN 23-Jul-01 11:32 e2eqavn/datasets/data_collator.py
 -rw-rw-r--  2.0 unx       85 b- defN 23-Jul-01 11:32 e2eqavn/documents/__init__.py
@@ -30,13 +30,13 @@
 -rw-rw-r--  2.0 unx    10419 b- defN 23-Jul-01 11:32 e2eqavn/retrieval/sbert_retrieval.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-01 11:32 e2eqavn/utils/__init__.py
 -rw-rw-r--  2.0 unx    12985 b- defN 23-Jul-01 11:32 e2eqavn/utils/calculate.py
 -rw-rw-r--  2.0 unx      603 b- defN 23-Jul-01 11:32 e2eqavn/utils/io.py
 -rw-rw-r--  2.0 unx      998 b- defN 23-Jul-01 11:32 e2eqavn/utils/preprocess.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-01 11:32 test/__init__.py
 -rw-rw-r--  2.0 unx      334 b- defN 23-Jul-01 11:32 test/test_chunking.py
--rw-rw-r--  2.0 unx      679 b- defN 23-Jul-03 15:42 e2eqavn-0.1.6.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jul-03 15:42 e2eqavn-0.1.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       52 b- defN 23-Jul-03 15:42 e2eqavn-0.1.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       13 b- defN 23-Jul-03 15:42 e2eqavn-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3378 b- defN 23-Jul-03 15:42 e2eqavn-0.1.6.dist-info/RECORD
-40 files, 113137 bytes uncompressed, 32165 bytes compressed:  71.6%
+-rw-rw-r--  2.0 unx     4990 b- defN 23-Jul-03 15:47 e2eqavn-0.1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jul-03 15:47 e2eqavn-0.1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       52 b- defN 23-Jul-03 15:47 e2eqavn-0.1.7.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       13 b- defN 23-Jul-03 15:47 e2eqavn-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3379 b- defN 23-Jul-03 15:47 e2eqavn-0.1.7.dist-info/RECORD
+40 files, 117449 bytes uncompressed, 33358 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -99,23 +99,23 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test_chunking.py
 Comment: 
 
-Filename: e2eqavn-0.1.6.dist-info/METADATA
+Filename: e2eqavn-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: e2eqavn-0.1.6.dist-info/WHEEL
+Filename: e2eqavn-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: e2eqavn-0.1.6.dist-info/entry_points.txt
+Filename: e2eqavn-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: e2eqavn-0.1.6.dist-info/top_level.txt
+Filename: e2eqavn-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: e2eqavn-0.1.6.dist-info/RECORD
+Filename: e2eqavn-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## e2eqavn/__init__.py

```diff
@@ -16,9 +16,9 @@
 
 stream_handler.setFormatter(formatted)
 logger.addHandler(stream_handler)
 logger.setLevel(logging.INFO)
 logger.propagate = False
 
 __author__ = 'khanhdm'
-__version__ = '0.1.6'
+__version__ = '0.1.7'
```

## Comparing `e2eqavn-0.1.6.dist-info/RECORD` & `e2eqavn-0.1.7.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-e2eqavn/__init__.py,sha256=uB1SptyJH6zlU9vkHKtDZfYv6M6Iw60SUbYtDndOZbs,498
+e2eqavn/__init__.py,sha256=54lwLY5cq5gKPvQLikORk_bjRCGEVJrPOYuE3lxjieI,498
 e2eqavn/cli.py,sha256=YV4JVKLr_kQLre7rbWUh9E76e9KWYif8m9PEu6Rgmus,10774
 e2eqavn/keywords.py,sha256=RUpkhbJ14i4XbIojmiSaXpjN9lI4bgPnpIY_ZnivTrc,2716
 e2eqavn/datasets/MRCDataset.py,sha256=EDQ656zUVz-PFZoBbA8D1WpyrMSdyTUzDHWbfheHdsk,3639
 e2eqavn/datasets/TripletDataset.py,sha256=UalsiPb-sVq79gE923C_Gu8mqih_KJ-NCAI2MEV-VCY,1386
 e2eqavn/datasets/__init__.py,sha256=PVd6KkEbmwFhGlSdv8lCnLcyIT6MrIOU2zeLEDnNBQM,124
 e2eqavn/datasets/data_collator.py,sha256=9anyZh7fMzgr0R3tmqO63d-kBUE2UgnrBbU0jPuTEJc,3814
 e2eqavn/documents/__init__.py,sha256=KhJ-7DiMYhKRaNBXpMFooJ4EioOOXKxFqjTVB__1JG8,85
@@ -29,12 +29,12 @@
 e2eqavn/retrieval/sbert_retrieval.py,sha256=KhdDq2CBF_E9nhWpQExyNtcjQOtxvOaZybj1ZAV7idQ,10419
 e2eqavn/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 e2eqavn/utils/calculate.py,sha256=LOaXVbVNIkhbH9UyKD004Evb_lbDY0SMnVSC7CnMgcI,12985
 e2eqavn/utils/io.py,sha256=StKqF8nRhuApqlI0vPlme8Y50Do4epId8KeW4oJ5uTI,603
 e2eqavn/utils/preprocess.py,sha256=1yhNSGZ5FRzIglW0IRiZyxS1b3Rr5CNzLN78lQsRQjQ,998
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_chunking.py,sha256=tW3Cg_Ll8mtfYjmPmNy5MgElUSe8eIKhcWAND20SRDA,334
-e2eqavn-0.1.6.dist-info/METADATA,sha256=IRRJvGv4sb-yfteozcjUqnuJOSsOcy5S4IrhQEC7JSU,679
-e2eqavn-0.1.6.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-e2eqavn-0.1.6.dist-info/entry_points.txt,sha256=pPUmMeBtyeitA4rbQwBo_glm5HRGPLREjN9eeAGu_Bk,52
-e2eqavn-0.1.6.dist-info/top_level.txt,sha256=Qu5Dlk8CtzRo5i3_O722D1zBatiVaNkiPAbSDCOA2pA,13
-e2eqavn-0.1.6.dist-info/RECORD,,
+e2eqavn-0.1.7.dist-info/METADATA,sha256=qOt6UWzeH6JF0pnBmOwTKTG4lTDFzYBVRixLpdYgPEE,4990
+e2eqavn-0.1.7.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+e2eqavn-0.1.7.dist-info/entry_points.txt,sha256=pPUmMeBtyeitA4rbQwBo_glm5HRGPLREjN9eeAGu_Bk,52
+e2eqavn-0.1.7.dist-info/top_level.txt,sha256=Qu5Dlk8CtzRo5i3_O722D1zBatiVaNkiPAbSDCOA2pA,13
+e2eqavn-0.1.7.dist-info/RECORD,,
```

