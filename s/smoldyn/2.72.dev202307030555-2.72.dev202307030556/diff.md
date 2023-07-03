# Comparing `tmp/smoldyn-2.72.dev202307030555-cp310-cp310-win_amd64.whl.zip` & `tmp/smoldyn-2.72.dev202307030556-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 869011 bytes, number of entries: 16
+Zip file size: 869168 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat      227 b- defN 23-Jul-03 05:57 smoldyn/__init__.py
 -rw-rw-rw-  2.0 fat      868 b- defN 23-Jul-03 05:57 smoldyn/__main__.py
--rw-rw-rw-  2.0 fat  1925632 b- defN 23-Jul-03 05:57 smoldyn/_smoldyn.cp310-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  1925632 b- defN 23-Jul-03 05:57 smoldyn/_smoldyn.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    80975 b- defN 23-Jul-03 05:57 smoldyn/smoldyn.py
 -rw-rw-rw-  2.0 fat     1193 b- defN 23-Jul-03 05:57 smoldyn/types.py
 -rw-rw-rw-  2.0 fat     1141 b- defN 23-Jul-03 05:57 smoldyn/utils.py
 -rw-rw-rw-  2.0 fat      510 b- defN 23-Jul-03 05:57 smoldyn/biosimulators/__init__.py
 -rw-rw-rw-  2.0 fat      605 b- defN 23-Jul-03 05:57 smoldyn/biosimulators/__main__.py
 -rw-rw-rw-  2.0 fat       47 b- defN 23-Jul-03 05:57 smoldyn/biosimulators/_version.py
 -rw-rw-rw-  2.0 fat    48535 b- defN 23-Jul-03 05:57 smoldyn/biosimulators/combine.py
 -rw-rw-rw-  2.0 fat     5443 b- defN 23-Jul-03 05:57 smoldyn/biosimulators/data_model.py
 -rw-rw-rw-  2.0 fat    17365 b- defN 23-Jul-03 05:57 smoldyn/biosimulators/utils.py
--rw-rw-rw-  2.0 fat     2908 b- defN 23-Jul-03 05:57 smoldyn-2.72.dev202307030555.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jul-03 05:57 smoldyn-2.72.dev202307030555.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-03 05:57 smoldyn-2.72.dev202307030555.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1362 b- defN 23-Jul-03 05:57 smoldyn-2.72.dev202307030555.dist-info/RECORD
-16 files, 2086921 bytes uncompressed, 866757 bytes compressed:  58.5%
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-Jul-03 05:57 smoldyn-2.72.dev202307030556.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-03 05:57 smoldyn-2.72.dev202307030556.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-03 05:57 smoldyn-2.72.dev202307030556.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1361 b- defN 23-Jul-03 05:57 smoldyn-2.72.dev202307030556.dist-info/RECORD
+16 files, 2086941 bytes uncompressed, 866916 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
 Filename: smoldyn/__init__.py
 Comment: 
 
 Filename: smoldyn/__main__.py
 Comment: 
 
-Filename: smoldyn/_smoldyn.cp310-win_amd64.pyd
+Filename: smoldyn/_smoldyn.cp39-win_amd64.pyd
 Comment: 
 
 Filename: smoldyn/smoldyn.py
 Comment: 
 
 Filename: smoldyn/types.py
 Comment: 
@@ -30,20 +30,20 @@
 
 Filename: smoldyn/biosimulators/data_model.py
 Comment: 
 
 Filename: smoldyn/biosimulators/utils.py
 Comment: 
 
-Filename: smoldyn-2.72.dev202307030555.dist-info/METADATA
+Filename: smoldyn-2.72.dev202307030556.dist-info/METADATA
 Comment: 
 
-Filename: smoldyn-2.72.dev202307030555.dist-info/WHEEL
+Filename: smoldyn-2.72.dev202307030556.dist-info/WHEEL
 Comment: 
 
-Filename: smoldyn-2.72.dev202307030555.dist-info/top_level.txt
+Filename: smoldyn-2.72.dev202307030556.dist-info/top_level.txt
 Comment: 
 
-Filename: smoldyn-2.72.dev202307030555.dist-info/RECORD
+Filename: smoldyn-2.72.dev202307030556.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `smoldyn-2.72.dev202307030555.dist-info/METADATA` & `smoldyn-2.72.dev202307030556.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: smoldyn
-Version: 2.72.dev202307030555
+Version: 2.72.dev202307030556
 Summary: Python package for the Smoldyn simulator
 Home-page: http://www.smoldyn.org/
 Author: Dilawar Singh
 Author-email: dilawar.s.rajput@gmail.com
 License: GNU LGPLv3
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -46,7 +47,9 @@
 Smoldyn is a particle-based biochemical simulator for modeling molecular
 diffusion, surface interactions, and chemical reactions.
 
 More information about Smoldyn is available at http://www.smoldyn.org. 
 Please visit this website to learn about Smoldyn, download the latest
 release, etc.
 
+
+
```

## Comparing `smoldyn-2.72.dev202307030555.dist-info/RECORD` & `smoldyn-2.72.dev202307030556.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 smoldyn/__init__.py,sha256=R3kO3jvZPyQEWwfy9LhSlz-tr0XbA6hg9gdzGXm-fTw,227
 smoldyn/__main__.py,sha256=XjjwMjJR-UjthM2oWeAlrWIe7lQqohNrf4XOxbPKtR4,868
-smoldyn/_smoldyn.cp310-win_amd64.pyd,sha256=L9jetaNa_gSsmi9YJIoIJ73yS8DDrp-b2HDsZnoHDVI,1925632
+smoldyn/_smoldyn.cp39-win_amd64.pyd,sha256=3fnpsYjw0eVqNoHJTooVsuzb8is3TmvSvz10nlW7aFg,1925632
 smoldyn/smoldyn.py,sha256=xOQCuC8blS9ytkVksRLXAjWV3prfgcTqlE64Y6zr768,80975
 smoldyn/types.py,sha256=VsMX56PF0mLvrMbn8p8ESBbYNJS3JtxJjpsQu-MMc50,1193
 smoldyn/utils.py,sha256=kQOHH7tLa9GjGsQb3e-5OfZLI_ssUjQ4EQEkN22wrOc,1141
 smoldyn/biosimulators/__init__.py,sha256=RG9Po9HQQy69-gQ5CQbxIIKIvqSPl2Lo3wlisENXe_M,510
 smoldyn/biosimulators/__main__.py,sha256=jivj09s_B0_NQajKBYZqbuHUJaS5GqEG0kykFa5fjww,605
 smoldyn/biosimulators/_version.py,sha256=FGh8vjjI-zkppjv7VjT8sKokqXeqK0jHeQzUVjlSMhk,47
 smoldyn/biosimulators/combine.py,sha256=gtxCePSZuJeCNEfwJSg0SXTAXb8il9uLlV4vXAAXivk,48535
 smoldyn/biosimulators/data_model.py,sha256=AWnWrZBADKzCux4FWHeFzAkN7vEZUzn07ldYmzPVlPo,5443
 smoldyn/biosimulators/utils.py,sha256=xR1a7oj_ZaRhAkZhshNB1n2Jiaxv8odDTLK5CJT6vL4,17365
-smoldyn-2.72.dev202307030555.dist-info/METADATA,sha256=NXJsNasprW7Q37H2nynbblr7c_unPCTAs3V4tkw6Jzg,2908
-smoldyn-2.72.dev202307030555.dist-info/WHEEL,sha256=jrOhEbqKwvzRFSJcbYXlJCyVkgVdHg4_7__YHrdTUfw,102
-smoldyn-2.72.dev202307030555.dist-info/top_level.txt,sha256=2FmedD0M8FnH4zNLmZCw84tbGuurvZfurkH4l4zSybQ,8
-smoldyn-2.72.dev202307030555.dist-info/RECORD,,
+smoldyn-2.72.dev202307030556.dist-info/METADATA,sha256=_3gfugQycPCihLDI0QAH5cjEEeX_uWU2qFiNQ2SxR-U,2931
+smoldyn-2.72.dev202307030556.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+smoldyn-2.72.dev202307030556.dist-info/top_level.txt,sha256=2FmedD0M8FnH4zNLmZCw84tbGuurvZfurkH4l4zSybQ,8
+smoldyn-2.72.dev202307030556.dist-info/RECORD,,
```

