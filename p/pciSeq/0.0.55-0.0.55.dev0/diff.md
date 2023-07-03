# Comparing `tmp/pciSeq-0.0.55-py3-none-any.whl.zip` & `tmp/pciSeq-0.0.55.dev0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 364270 bytes, number of entries: 73
+Zip file size: 364344 bytes, number of entries: 73
 -rw-rw-rw-  2.0 fat     2135 b- defN 23-Jun-25 20:54 pciSeq/__init__.py
 -rw-rw-rw-  2.0 fat    10919 b- defN 23-Jul-03 07:45 pciSeq/app.py
 -rw-rw-rw-  2.0 fat     3369 b- defN 23-Jul-02 23:15 pciSeq/config.py
 -rw-rw-rw-  2.0 fat     3678 b- defN 22-Apr-07 23:15 pciSeq/make_plot.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jan-19 17:53 pciSeq/src/__init__.py
--rw-rw-rw-  2.0 fat       22 b- defN 23-Jul-03 10:08 pciSeq/src/_version.py
+-rw-rw-rw-  2.0 fat       27 b- defN 23-Jul-03 09:22 pciSeq/src/_version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jan-19 17:53 pciSeq/src/cell_call/__init__.py
 -rw-rw-rw-  2.0 fat    20864 b- defN 23-Jun-29 10:21 pciSeq/src/cell_call/datatypes.py
 -rw-rw-rw-  2.0 fat     2995 b- defN 23-Apr-26 22:13 pciSeq/src/cell_call/log_config.py
 -rw-rw-rw-  2.0 fat    19103 b- defN 23-Jul-03 08:19 pciSeq/src/cell_call/main.py
 -rw-rw-rw-  2.0 fat     3104 b- defN 23-Jun-25 20:54 pciSeq/src/cell_call/summary.py
 -rw-rw-rw-  2.0 fat     9194 b- defN 23-Jun-25 20:54 pciSeq/src/cell_call/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-11 12:10 pciSeq/src/diagnostics/__init__.py
@@ -62,14 +62,14 @@
 -rw-rw-rw-  2.0 fat    15374 b- defN 23-Apr-26 22:13 pciSeq/static/2D/viewer/js/lib/js/leaflet-pip.js
 -rw-rw-rw-  2.0 fat     5927 b- defN 23-Apr-26 22:13 pciSeq/static/2D/viewer/js/lib/js/leaflet.textpath.js
 -rw-rw-rw-  2.0 fat      265 b- defN 23-Apr-26 22:13 pciSeq/static/2D/viewer/js/lib/js/preloader.js
 -rw-rw-rw-  2.0 fat     9097 b- defN 23-Apr-26 22:13 pciSeq/static/2D/viewer/js/lib/js/pixiOverlay/MarkerContainer.js
 -rw-rw-rw-  2.0 fat     4434 b- defN 23-Apr-26 22:13 pciSeq/static/2D/viewer/js/lib/js/pixiOverlay/bezier-easing.js
 -rw-rw-rw-  2.0 fat   613808 b- defN 23-Apr-26 22:13 pciSeq/static/2D/viewer/js/lib/js/pixiOverlay/example.min.js
 -rw-rw-rw-  2.0 fat    91874 b- defN 23-Apr-26 22:13 pciSeq/static/2D/viewer/js/lib/js/pixiOverlay/tools.min.js
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-03 10:09 pciSeq-0.0.55.dist-info/LICENCE
--rw-rw-rw-  2.0 fat     4183 b- defN 23-Jul-03 10:09 pciSeq-0.0.55.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-03 10:09 pciSeq-0.0.55.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       48 b- defN 23-Jul-03 10:09 pciSeq-0.0.55.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-03 10:09 pciSeq-0.0.55.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     6935 b- defN 23-Jul-03 10:09 pciSeq-0.0.55.dist-info/RECORD
-73 files, 1325341 bytes uncompressed, 353020 bytes compressed:  73.4%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-03 09:25 pciSeq-0.0.55.dev0.dist-info/LICENCE
+-rw-rw-rw-  2.0 fat     4188 b- defN 23-Jul-03 09:25 pciSeq-0.0.55.dev0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-03 09:25 pciSeq-0.0.55.dev0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       48 b- defN 23-Jul-03 09:25 pciSeq-0.0.55.dev0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-03 09:25 pciSeq-0.0.55.dev0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     6965 b- defN 23-Jul-03 09:25 pciSeq-0.0.55.dev0.dist-info/RECORD
+73 files, 1325381 bytes uncompressed, 353034 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -195,26 +195,26 @@
 
 Filename: pciSeq/static/2D/viewer/js/lib/js/pixiOverlay/example.min.js
 Comment: 
 
 Filename: pciSeq/static/2D/viewer/js/lib/js/pixiOverlay/tools.min.js
 Comment: 
 
-Filename: pciSeq-0.0.55.dist-info/LICENCE
+Filename: pciSeq-0.0.55.dev0.dist-info/LICENCE
 Comment: 
 
-Filename: pciSeq-0.0.55.dist-info/METADATA
+Filename: pciSeq-0.0.55.dev0.dist-info/METADATA
 Comment: 
 
-Filename: pciSeq-0.0.55.dist-info/WHEEL
+Filename: pciSeq-0.0.55.dev0.dist-info/WHEEL
 Comment: 
 
-Filename: pciSeq-0.0.55.dist-info/entry_points.txt
+Filename: pciSeq-0.0.55.dev0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pciSeq-0.0.55.dist-info/top_level.txt
+Filename: pciSeq-0.0.55.dev0.dist-info/top_level.txt
 Comment: 
 
-Filename: pciSeq-0.0.55.dist-info/RECORD
+Filename: pciSeq-0.0.55.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pciSeq/src/_version.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.55'
+__version__ = '0.0.55.dev0'
```

## Comparing `pciSeq-0.0.55.dist-info/LICENCE` & `pciSeq-0.0.55.dev0.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `pciSeq-0.0.55.dist-info/METADATA` & `pciSeq-0.0.55.dev0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pciSeq
-Version: 0.0.55
+Version: 0.0.55.dev0
 Summary: Probabilistic cell typing for spatial transcriptomics
 Home-page: https://github.com/acycliq/pciSeq
 Author: Dimitris Nicoloutsopoulos
 Author-email: dimitris.nicoloutsopoulos@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

## Comparing `pciSeq-0.0.55.dist-info/RECORD` & `pciSeq-0.0.55.dev0.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pciSeq/__init__.py,sha256=mxqjE8smLqDQuwzheJ_iA3gfcyV7c4x8lHQPwSEQwJk,2135
 pciSeq/app.py,sha256=OsFFq_u6K-G3SNWW7m4wX0P4p2fqhTOyMqT0cqKEy_I,10919
 pciSeq/config.py,sha256=u227HnbaSSGJs3wPopJju7GK59WPl7lN6G27JTkoPZc,3369
 pciSeq/make_plot.py,sha256=2AkncrVVvytr2keK505oMC0LV1Txli9WpsSGpjmht_4,3678
 pciSeq/src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pciSeq/src/_version.py,sha256=jTe9sUxnjY28guuRUoHbC3SW_3TDNMlQP4ONqhrHM-Y,22
+pciSeq/src/_version.py,sha256=TtiPwk0MiwYVFxAXL6egnEO8uDbyDCjmRQ22CY3kMUc,27
 pciSeq/src/cell_call/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pciSeq/src/cell_call/datatypes.py,sha256=om8kMxOUxKcAoQHSTgXEuX4UNMGtwTjFkOCGmeublqs,20864
 pciSeq/src/cell_call/log_config.py,sha256=vnm9TxlMEVG_GLPfl21GDEWTafEk3B-drTLsVQMfFEE,2995
 pciSeq/src/cell_call/main.py,sha256=PgOk1dngmqk357AYCZxmGFoFjyZBgW_nEKNb5F0CKK4,19103
 pciSeq/src/cell_call/summary.py,sha256=f2snLqJIeywtYuHrJLM-hRvifgqRU2u2aCKE_JrZJPs,3104
 pciSeq/src/cell_call/utils.py,sha256=M4KJrS82pIHuCoxg2ej6NE9fJAVCvJw90T7YmWI2T7o,9194
 pciSeq/src/diagnostics/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -61,13 +61,13 @@
 pciSeq/static/2D/viewer/js/lib/js/leaflet-pip.js,sha256=QqsilU0SHTaKA_qNSv_jEDH53cWO6T_RdforfybnbKM,15374
 pciSeq/static/2D/viewer/js/lib/js/leaflet.textpath.js,sha256=i5cmMPqpqXShZz0TvXU3ZQUi2Y07SIbIpMYbhPE8gWE,5927
 pciSeq/static/2D/viewer/js/lib/js/preloader.js,sha256=eaFWRf9yT-Td4C2t01P8fDEZYszYTaGDgQ1vjevNIDI,265
 pciSeq/static/2D/viewer/js/lib/js/pixiOverlay/MarkerContainer.js,sha256=Z8TADCqYEQr25OEF7wljsOVAOpx87UrjFPI2nvIty70,9097
 pciSeq/static/2D/viewer/js/lib/js/pixiOverlay/bezier-easing.js,sha256=yMoRDqJiglg0M0eWM25WGA5zzLWuJpOyC3a8aGFx0jw,4434
 pciSeq/static/2D/viewer/js/lib/js/pixiOverlay/example.min.js,sha256=bZEnK8XSnShrpLYtOS7Xq7wnp-nW_nMZh4aaDc1Gt6U,613808
 pciSeq/static/2D/viewer/js/lib/js/pixiOverlay/tools.min.js,sha256=A027Ub-oWXvKbz2B3pgMFS5xApmnEHXz9GQh79YZZnU,91874
-pciSeq-0.0.55.dist-info/LICENCE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-pciSeq-0.0.55.dist-info/METADATA,sha256=Ie0CksZB-oYOcgLMdkgp3tCys-__EpD71g16NVQV5oc,4183
-pciSeq-0.0.55.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pciSeq-0.0.55.dist-info/entry_points.txt,sha256=RGOkAd0S7rrTuEInj-jKu5B7630i4R3mK9v9vx6nqc8,48
-pciSeq-0.0.55.dist-info/top_level.txt,sha256=mSonMN0SaB51m5yLGm5hFE1Fthf-2U4sRKxSezY-JMk,7
-pciSeq-0.0.55.dist-info/RECORD,,
+pciSeq-0.0.55.dev0.dist-info/LICENCE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+pciSeq-0.0.55.dev0.dist-info/METADATA,sha256=YNDyJKWPgo8SYxRF1O2kTeQqO8R4TVT4aAeKFvysD_o,4188
+pciSeq-0.0.55.dev0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pciSeq-0.0.55.dev0.dist-info/entry_points.txt,sha256=RGOkAd0S7rrTuEInj-jKu5B7630i4R3mK9v9vx6nqc8,48
+pciSeq-0.0.55.dev0.dist-info/top_level.txt,sha256=mSonMN0SaB51m5yLGm5hFE1Fthf-2U4sRKxSezY-JMk,7
+pciSeq-0.0.55.dev0.dist-info/RECORD,,
```

