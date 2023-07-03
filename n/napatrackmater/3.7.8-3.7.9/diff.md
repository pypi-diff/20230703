# Comparing `tmp/napatrackmater-3.7.8.tar.gz` & `tmp/napatrackmater-3.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-00rw5a1q/napatrackmater-3.7.8.tar", last modified: Thu Jun 15 20:53:18 2023, max compression
+gzip compressed data, was "napatrackmater-3.7.9.tar", last modified: Mon Jul  3 08:07:13 2023, max compression
```

## Comparing `napatrackmater-3.7.8.tar` & `napatrackmater-3.7.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-15 20:53:18.562601 napatrackmater-3.7.8/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.7.8/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-15 20:53:18.558343 napatrackmater-3.7.8/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.7.8/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-15 20:53:18.357553 napatrackmater-3.7.8/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.7.8/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.7.8/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.7.8/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16426 2023-06-15 20:52:31.000000 napatrackmater-3.7.8/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.7.8/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    14304 2023-06-15 20:51:11.000000 napatrackmater-3.7.8/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.7.8/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.7.8/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.7.8/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-15 20:52:39.000000 napatrackmater-3.7.8/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-15 20:53:18.524700 napatrackmater-3.7.8/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-15 20:53:17.000000 napatrackmater-3.7.8/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-15 20:53:17.000000 napatrackmater-3.7.8/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-15 20:53:17.000000 napatrackmater-3.7.8/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-15 20:53:17.000000 napatrackmater-3.7.8/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-15 20:53:17.000000 napatrackmater-3.7.8/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-15 20:53:17.000000 napatrackmater-3.7.8/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-15 20:53:18.563779 napatrackmater-3.7.8/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.7.8/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 08:07:13.369219 napatrackmater-3.7.9/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.7.9/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-03 08:07:13.365217 napatrackmater-3.7.9/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.7.9/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 08:07:13.166513 napatrackmater-3.7.9/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.7.9/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.7.9/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.7.9/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16426 2023-06-15 20:52:31.000000 napatrackmater-3.7.9/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.7.9/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    14304 2023-06-15 20:51:11.000000 napatrackmater-3.7.9/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.7.9/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.7.9/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.7.9/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-07-03 07:55:51.000000 napatrackmater-3.7.9/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-03 08:07:13.334410 napatrackmater-3.7.9/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-03 08:07:12.000000 napatrackmater-3.7.9/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-07-03 08:07:12.000000 napatrackmater-3.7.9/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-03 08:07:12.000000 napatrackmater-3.7.9/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-07-03 08:07:12.000000 napatrackmater-3.7.9/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-07-03 08:07:12.000000 napatrackmater-3.7.9/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-07-03 08:07:12.000000 napatrackmater-3.7.9/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-07-03 08:07:13.371539 napatrackmater-3.7.9/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1410 2023-07-03 08:06:08.000000 napatrackmater-3.7.9/setup.py
```

### Comparing `napatrackmater-3.7.8/LICENSE` & `napatrackmater-3.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.8/PKG-INFO` & `napatrackmater-3.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.7.8
+Version: 3.7.9
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.7.8/README.md` & `napatrackmater-3.7.9/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.8/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.7.9/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.8/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.7.9/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.8/napatrackmater/Trackmate.py` & `napatrackmater-3.7.9/napatrackmater/Trackmate.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.8/napatrackmater/Trackvector.py` & `napatrackmater-3.7.9/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.8/napatrackmater/__init__.py` & `napatrackmater-3.7.9/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.8/napatrackmater/clustering.py` & `napatrackmater-3.7.9/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.8/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.7.9/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.8/napatrackmater/fate_mapping.py` & `napatrackmater-3.7.9/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.8/napatrackmater/pretrained.py` & `napatrackmater-3.7.9/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.8/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.7.9/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.7.8
+Version: 3.7.9
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.7.8/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.7.9/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.8/setup.py` & `napatrackmater-3.7.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,39 +45,45 @@
 000002c0: 6571 7569 7265 733d 5b0d 0a20 2020 2020  equires=[..     
 000002d0: 2020 2022 6c78 6d6c 222c 0d0a 2020 2020     "lxml",..    
 000002e0: 2020 2020 2276 6f6c 6c73 6567 222c 0d0a      "vollseg",..
 000002f0: 2020 2020 2020 2020 226e 6170 6172 6922          "napari"
 00000300: 2c0d 0a20 2020 2020 2020 2022 6e61 7473  ,..        "nats
 00000310: 6f72 7422 2c0d 0a20 2020 2020 2020 2022  ort",..        "
 00000320: 7365 6162 6f72 6e22 2c0d 0a20 2020 2020  seaborn",..     
-00000330: 2020 2022 6b61 706f 6f72 6c61 6273 2d6c     "kapoorlabs-l
-00000340: 6967 6874 6e69 6e67 222c 0d0a 2020 2020  ightning",..    
-00000350: 5d2c 0d0a 2020 2020 656e 7472 795f 706f  ],..    entry_po
-00000360: 696e 7473 203d 207b 0d0a 2020 2020 2020  ints = {..      
-00000370: 2020 2763 6f6e 736f 6c65 5f73 6372 6970    'console_scrip
-00000380: 7473 273a 205b 0d0a 2020 2020 2020 2020  ts': [..        
-00000390: 2020 2020 2774 7261 636b 203d 206e 6170      'track = nap
-000003a0: 6174 7261 636b 6d61 7465 722e 5f5f 6d61  atrackmater.__ma
-000003b0: 696e 5f5f 3a6d 6169 6e27 2c0d 0a20 2020  in__:main',..   
-000003c0: 2020 2020 205d 0d0a 2020 2020 7d2c 0d0a       ]..    },..
-000003d0: 2020 2020 7061 636b 6167 6573 3d73 6574      packages=set
-000003e0: 7570 746f 6f6c 732e 6669 6e64 5f70 6163  uptools.find_pac
-000003f0: 6b61 6765 7328 292c 0d0a 2020 2020 636c  kages(),..    cl
-00000400: 6173 7369 6669 6572 733d 5b0d 0a20 2020  assifiers=[..   
-00000410: 2020 2020 2027 4465 7665 6c6f 706d 656e       'Developmen
-00000420: 7420 5374 6174 7573 203a 3a20 3320 2d20  t Status :: 3 - 
-00000430: 416c 7068 6127 2c0d 0a20 2020 2020 2020  Alpha',..       
-00000440: 2027 4e61 7475 7261 6c20 4c61 6e67 7561   'Natural Langua
-00000450: 6765 203a 3a20 456e 676c 6973 6827 2c0d  ge :: English',.
-00000460: 0a20 2020 2020 2020 2027 4c69 6365 6e73  .        'Licens
-00000470: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000480: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-00000490: 272c 0d0a 2020 2020 2020 2020 274f 7065  ',..        'Ope
-000004a0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-000004b0: 204f 5320 496e 6465 7065 6e64 656e 7427   OS Independent'
-000004c0: 2c0d 0a20 2020 2020 2020 2027 5072 6f67  ,..        'Prog
-000004d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000004e0: 203a 3a20 5079 7468 6f6e 272c 0d0a 2020   :: Python',..  
-000004f0: 2020 2020 2020 2750 726f 6772 616d 6d69        'Programmi
-00000500: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000510: 7974 686f 6e20 3a3a 2033 2e37 272c 0d0a  ython :: 3.7',..
-00000520: 2020 2020 5d2c 0d0a 290d 0a0d 0a             ],..)....
+00000330: 2020 2022 6365 6c6c 7368 6170 652d 636c     "cellshape-cl
+00000340: 6f75 6422 2c0d 0a20 2020 2020 2020 2022  oud",..        "
+00000350: 6365 6c6c 7368 6170 652d 6865 6c70 6572  cellshape-helper
+00000360: 222c 0d0a 2020 2020 2020 2020 226b 6170  ",..        "kap
+00000370: 6f6f 726c 6162 732d 6c69 6768 746e 696e  oorlabs-lightnin
+00000380: 6722 2c0d 0a20 2020 2020 2020 2022 6c69  g",..        "li
+00000390: 6768 746e 696e 673e 3d32 2e30 2e34 220d  ghtning>=2.0.4".
+000003a0: 0a20 2020 205d 2c0d 0a20 2020 2065 6e74  .    ],..    ent
+000003b0: 7279 5f70 6f69 6e74 7320 3d20 7b0d 0a20  ry_points = {.. 
+000003c0: 2020 2020 2020 2027 636f 6e73 6f6c 655f         'console_
+000003d0: 7363 7269 7074 7327 3a20 5b0d 0a20 2020  scripts': [..   
+000003e0: 2020 2020 2020 2020 2027 7472 6163 6b20           'track 
+000003f0: 3d20 6e61 7061 7472 6163 6b6d 6174 6572  = napatrackmater
+00000400: 2e5f 5f6d 6169 6e5f 5f3a 6d61 696e 272c  .__main__:main',
+00000410: 0d0a 2020 2020 2020 2020 5d0d 0a20 2020  ..        ]..   
+00000420: 207d 2c0d 0a20 2020 2070 6163 6b61 6765   },..    package
+00000430: 733d 7365 7475 7074 6f6f 6c73 2e66 696e  s=setuptools.fin
+00000440: 645f 7061 636b 6167 6573 2829 2c0d 0a20  d_packages(),.. 
+00000450: 2020 2063 6c61 7373 6966 6965 7273 3d5b     classifiers=[
+00000460: 0d0a 2020 2020 2020 2020 2744 6576 656c  ..        'Devel
+00000470: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+00000480: 2033 202d 2041 6c70 6861 272c 0d0a 2020   3 - Alpha',..  
+00000490: 2020 2020 2020 274e 6174 7572 616c 204c        'Natural L
+000004a0: 616e 6775 6167 6520 3a3a 2045 6e67 6c69  anguage :: Engli
+000004b0: 7368 272c 0d0a 2020 2020 2020 2020 274c  sh',..        'L
+000004c0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+000004d0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+000004e0: 6365 6e73 6527 2c0d 0a20 2020 2020 2020  cense',..       
+000004f0: 2027 4f70 6572 6174 696e 6720 5379 7374   'Operating Syst
+00000500: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+00000510: 6465 6e74 272c 0d0a 2020 2020 2020 2020  dent',..        
+00000520: 2750 726f 6772 616d 6d69 6e67 204c 616e  'Programming Lan
+00000530: 6775 6167 6520 3a3a 2050 7974 686f 6e27  guage :: Python'
+00000540: 2c0d 0a20 2020 2020 2020 2027 5072 6f67  ,..        'Prog
+00000550: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000560: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000570: 3727 2c0d 0a20 2020 205d 2c0d 0a29 0d0a  7',..    ],..)..
+00000580: 0d0a                                     ..
```

