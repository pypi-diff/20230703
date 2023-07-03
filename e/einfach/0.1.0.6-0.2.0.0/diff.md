# Comparing `tmp/einfach-0.1.0.6.tar.gz` & `tmp/einfach-0.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "einfach-0.1.0.6.tar", last modified: Sat Apr  1 23:30:33 2023, max compression
+gzip compressed data, was "einfach-0.2.0.0.tar", last modified: Mon Jul  3 13:57:50 2023, max compression
```

## Comparing `einfach-0.1.0.6.tar` & `einfach-0.2.0.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 23:30:33.237932 einfach-0.1.0.6/
--rw-rw-rw-   0        0        0     1068 2023-04-01 23:30:33.237932 einfach-0.1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-04-01 23:23:39.000000 einfach-0.1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-01 23:30:33.213887 einfach-0.1.0.6/einfach/
--rw-rw-rw-   0        0        0       45 2023-04-01 08:56:09.000000 einfach-0.1.0.6/einfach/__init__.py
--rw-rw-rw-   0        0        0      486 2023-04-01 09:07:23.000000 einfach-0.1.0.6/einfach/clip.py
--rw-rw-rw-   0        0        0     1690 2023-04-01 08:47:51.000000 einfach-0.1.0.6/einfach/pathdialog.py
-drwxrwxrwx   0        0        0        0 2023-04-01 23:30:33.233938 einfach-0.1.0.6/einfach.egg-info/
--rw-rw-rw-   0        0        0     1068 2023-04-01 23:30:33.000000 einfach-0.1.0.6/einfach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-04-01 23:30:33.000000 einfach-0.1.0.6/einfach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 23:30:33.000000 einfach-0.1.0.6/einfach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-01 23:30:33.000000 einfach-0.1.0.6/einfach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-01 23:30:33.237932 einfach-0.1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1462 2023-04-01 23:30:27.000000 einfach-0.1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:57:50.662972 einfach-0.2.0.0/
+-rw-rw-rw-   0        0        0     1144 2023-07-03 13:57:50.662972 einfach-0.2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2023-04-02 00:01:01.000000 einfach-0.2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 13:57:50.630982 einfach-0.2.0.0/einfach/
+-rw-rw-rw-   0        0        0      156 2023-07-03 13:38:13.000000 einfach-0.2.0.0/einfach/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-07-03 13:11:00.000000 einfach-0.2.0.0/einfach/clip.py
+-rw-rw-rw-   0        0        0      286 2023-07-03 13:29:22.000000 einfach-0.2.0.0/einfach/floatutils.py
+-rw-rw-rw-   0        0        0     1690 2023-07-03 13:29:04.000000 einfach-0.2.0.0/einfach/pathdialog.py
+-rw-rw-rw-   0        0        0     1480 2023-07-03 13:27:32.000000 einfach-0.2.0.0/einfach/termutils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:57:50.654975 einfach-0.2.0.0/einfach.egg-info/
+-rw-rw-rw-   0        0        0     1144 2023-07-03 13:57:50.000000 einfach-0.2.0.0/einfach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-03 13:57:50.000000 einfach-0.2.0.0/einfach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 13:57:50.000000 einfach-0.2.0.0/einfach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 13:57:50.000000 einfach-0.2.0.0/einfach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 13:57:50.662972 einfach-0.2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1553 2023-07-03 13:57:22.000000 einfach-0.2.0.0/setup.py
```

### Comparing `einfach-0.1.0.6/PKG-INFO` & `einfach-0.2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: einfach
-Version: 0.1.0.6
+Version: 0.2.0.0
 Summary: A collection of useful code "snippets"
 Home-page: https://github.com/rotgruengelb/einfach
 Author: rotgruengelb (Daniel)
 Author-email: <code@rotgruengelb.net>
 License: MIT
 Project-URL: Source, https://github.com/rotgruengelb/einfach
 Project-URL: Issues, https://github.com/rotgruengelb/einfach/issues
 Project-URL: Wiki, https://github.com/rotgruengelb/einfach/wiki/Features
 Keywords: python,helper,helpers,help,easy code,ease of use,snippets,code snippets
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: User Interfaces
 Description-Content-Type: text/markdown
 
 A collection of useful code "snippets" or "helpers" that implement little but annoying to add things for you
 
 # Install
 ```shell
 pip install einfach
 ```
 
 # Use/Features
-[List of Features in the wiki](https://github.com/rotgruengelb/einfach/wiki/Features)
+[List of Features on the Features Wiki Page](https://github.com/rotgruengelb/einfach/wiki/Features)
```

### Comparing `einfach-0.1.0.6/einfach/pathdialog.py` & `einfach-0.2.0.0/einfach/pathdialog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import tkinter as tk
 from tkinter import filedialog
 
+
+
 def open_file(mode, **filedialogargs):
     root = tk.Tk()
     root.withdraw()
     try:
         if mode == "file":
             file_path = filedialog.askopenfile(**filedialogargs); return file_path
         elif mode == "file_name":
@@ -14,15 +16,14 @@
         elif mode == "file_names":
             file_path = filedialog.askopenfilenames(**filedialogargs); return file_path
         else: raise ValueError("mode was not 'file', 'file_name', 'files' or 'file_names'!")
     except Exception as e:
         raise e
 
 
-
 def save_file(mode, **filedialogargs):
     root = tk.Tk()
     root.withdraw()
     try:
         if mode == "file":
             file_path = filedialog.asksaveasfile(**filedialogargs); return file_path
         elif mode == "file_name":
@@ -32,15 +33,14 @@
         elif mode == "file_names":
             file_path = filedialog.askopenfilenames(**filedialogargs); return file_path
         else: raise ValueError("mode was not 'file', 'file_name', 'files' or 'file_names'!")
     except Exception as e:
         raise e
 
 
-
 def open_dir(**filedialogargs):
     root = tk.Tk()
     root.withdraw()
     try:
         dir_path = filedialog.askdirectory(**filedialogargs); return dir_path
     except Exception as e:
         raise e
```

### Comparing `einfach-0.1.0.6/einfach.egg-info/PKG-INFO` & `einfach-0.2.0.0/einfach.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: einfach
-Version: 0.1.0.6
+Version: 0.2.0.0
 Summary: A collection of useful code "snippets"
 Home-page: https://github.com/rotgruengelb/einfach
 Author: rotgruengelb (Daniel)
 Author-email: <code@rotgruengelb.net>
 License: MIT
 Project-URL: Source, https://github.com/rotgruengelb/einfach
 Project-URL: Issues, https://github.com/rotgruengelb/einfach/issues
 Project-URL: Wiki, https://github.com/rotgruengelb/einfach/wiki/Features
 Keywords: python,helper,helpers,help,easy code,ease of use,snippets,code snippets
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: User Interfaces
 Description-Content-Type: text/markdown
 
 A collection of useful code "snippets" or "helpers" that implement little but annoying to add things for you
 
 # Install
 ```shell
 pip install einfach
 ```
 
 # Use/Features
-[List of Features in the wiki](https://github.com/rotgruengelb/einfach/wiki/Features)
+[List of Features on the Features Wiki Page](https://github.com/rotgruengelb/einfach/wiki/Features)
```

### Comparing `einfach-0.1.0.6/setup.py` & `einfach-0.2.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,92 +1,98 @@
-00000000: 0d0a 0d0a 6672 6f6d 2073 6574 7570 746f  ....from setupto
-00000010: 6f6c 7320 696d 706f 7274 2073 6574 7570  ols import setup
-00000020: 2c20 6669 6e64 5f70 6163 6b61 6765 730d  , find_packages.
-00000030: 0a69 6d70 6f72 7420 636f 6465 6373 0d0a  .import codecs..
-00000040: 696d 706f 7274 206f 730d 0a0d 0a68 6572  import os....her
-00000050: 6520 3d20 6f73 2e70 6174 682e 6162 7370  e = os.path.absp
-00000060: 6174 6828 6f73 2e70 6174 682e 6469 726e  ath(os.path.dirn
-00000070: 616d 6528 5f5f 6669 6c65 5f5f 2929 0d0a  ame(__file__))..
-00000080: 0d0a 7769 7468 2063 6f64 6563 732e 6f70  ..with codecs.op
-00000090: 656e 286f 732e 7061 7468 2e6a 6f69 6e28  en(os.path.join(
-000000a0: 6865 7265 2c20 2252 4541 444d 452e 6d64  here, "README.md
-000000b0: 2229 2c20 656e 636f 6469 6e67 3d22 7574  "), encoding="ut
-000000c0: 662d 3822 2920 6173 2066 683a 0d0a 2020  f-8") as fh:..  
-000000d0: 2020 6c6f 6e67 5f64 6573 6372 6970 7469    long_descripti
-000000e0: 6f6e 203d 2022 5c6e 2220 2b20 6668 2e72  on = "\n" + fh.r
-000000f0: 6561 6428 290d 0a0d 0a56 4552 5349 4f4e  ead()....VERSION
-00000100: 203d 2027 302e 312e 302e 3627 0d0a 4445   = '0.1.0.6'..DE
-00000110: 5343 5249 5054 494f 4e20 3d20 2741 2063  SCRIPTION = 'A c
-00000120: 6f6c 6c65 6374 696f 6e20 6f66 2075 7365  ollection of use
-00000130: 6675 6c20 636f 6465 2022 736e 6970 7065  ful code "snippe
-00000140: 7473 2227 0d0a 4c4f 4e47 5f44 4553 4352  ts"'..LONG_DESCR
-00000150: 4950 5449 4f4e 203d 2027 4120 636f 6c6c  IPTION = 'A coll
-00000160: 6563 7469 6f6e 206f 6620 7573 6566 756c  ection of useful
-00000170: 2063 6f64 6520 2273 6e69 7070 6574 7322   code "snippets"
-00000180: 206f 7220 2268 656c 7065 7273 2220 7468   or "helpers" th
-00000190: 6174 2069 6d70 6c65 6d65 6e74 206c 6974  at implement lit
-000001a0: 746c 6520 6275 7420 616e 6e6f 7969 6e67  tle but annoying
-000001b0: 2074 6f20 6164 6420 7468 696e 6773 2066   to add things f
-000001c0: 6f72 2079 6f75 270d 0a0d 0a23 2053 6574  or you'....# Set
-000001d0: 7469 6e67 2075 700d 0a73 6574 7570 280d  ting up..setup(.
-000001e0: 0a20 2020 206e 616d 653d 2265 696e 6661  .    name="einfa
-000001f0: 6368 222c 0d0a 2020 2020 7665 7273 696f  ch",..    versio
-00000200: 6e3d 5645 5253 494f 4e2c 0d0a 2020 2020  n=VERSION,..    
-00000210: 6175 7468 6f72 3d22 726f 7467 7275 656e  author="rotgruen
-00000220: 6765 6c62 2028 4461 6e69 656c 2922 2c0d  gelb (Daniel)",.
-00000230: 0a20 2020 2061 7574 686f 725f 656d 6169  .    author_emai
-00000240: 6c3d 223c 636f 6465 4072 6f74 6772 7565  l="<code@rotgrue
-00000250: 6e67 656c 622e 6e65 743e 222c 0d0a 2020  ngelb.net>",..  
-00000260: 2020 6465 7363 7269 7074 696f 6e3d 4445    description=DE
-00000270: 5343 5249 5054 494f 4e2c 0d0a 2020 2020  SCRIPTION,..    
-00000280: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000290: 5f63 6f6e 7465 6e74 5f74 7970 653d 2274  _content_type="t
-000002a0: 6578 742f 6d61 726b 646f 776e 222c 0d0a  ext/markdown",..
-000002b0: 2020 2020 6c6f 6e67 5f64 6573 6372 6970      long_descrip
-000002c0: 7469 6f6e 3d4c 4f4e 475f 4445 5343 5249  tion=LONG_DESCRI
-000002d0: 5054 494f 4e20 2b20 225c 6e22 202b 206c  PTION + "\n" + l
-000002e0: 6f6e 675f 6465 7363 7269 7074 696f 6e2c  ong_description,
-000002f0: 0d0a 2020 2020 7061 636b 6167 6573 3d66  ..    packages=f
-00000300: 696e 645f 7061 636b 6167 6573 2829 2c0d  ind_packages(),.
-00000310: 0a20 2020 206c 6963 656e 7365 3d22 4d49  .    license="MI
-00000320: 5422 2c0d 0a20 2020 2075 726c 3d22 6874  T",..    url="ht
-00000330: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000340: 2f72 6f74 6772 7565 6e67 656c 622f 6569  /rotgruengelb/ei
-00000350: 6e66 6163 6822 2c0d 0a20 2020 2070 726f  nfach",..    pro
-00000360: 6a65 6374 5f75 726c 733d 7b0d 0a20 2020  ject_urls={..   
-00000370: 2027 536f 7572 6365 273a 2027 6874 7470   'Source': 'http
-00000380: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
-00000390: 6f74 6772 7565 6e67 656c 622f 6569 6e66  otgruengelb/einf
-000003a0: 6163 6827 2c0d 0a20 2020 2027 4973 7375  ach',..    'Issu
-000003b0: 6573 273a 2027 6874 7470 733a 2f2f 6769  es': 'https://gi
-000003c0: 7468 7562 2e63 6f6d 2f72 6f74 6772 7565  thub.com/rotgrue
-000003d0: 6e67 656c 622f 6569 6e66 6163 682f 6973  ngelb/einfach/is
-000003e0: 7375 6573 272c 0d0a 2020 2020 2757 696b  sues',..    'Wik
-000003f0: 6927 3a20 2768 7474 7073 3a2f 2f67 6974  i': 'https://git
-00000400: 6875 622e 636f 6d2f 726f 7467 7275 656e  hub.com/rotgruen
-00000410: 6765 6c62 2f65 696e 6661 6368 2f77 696b  gelb/einfach/wik
-00000420: 692f 4665 6174 7572 6573 270d 0a20 2020  i/Features'..   
-00000430: 207d 2c0d 0a20 2020 2069 6e73 7461 6c6c   },..    install
-00000440: 5f72 6571 7569 7265 733d 5b5d 2c0d 0a20  _requires=[],.. 
-00000450: 2020 206b 6579 776f 7264 733d 5b27 7079     keywords=['py
-00000460: 7468 6f6e 272c 2027 6865 6c70 6572 272c  thon', 'helper',
-00000470: 2027 6865 6c70 6572 7327 2c20 2768 656c   'helpers', 'hel
-00000480: 7027 2c20 2765 6173 7920 636f 6465 272c  p', 'easy code',
-00000490: 2027 6561 7365 206f 6620 7573 6527 2c20   'ease of use', 
-000004a0: 2273 6e69 7070 6574 7322 2c20 2263 6f64  "snippets", "cod
-000004b0: 6520 736e 6970 7065 7473 225d 2c0d 0a20  e snippets"],.. 
-000004c0: 2020 2063 6c61 7373 6966 6965 7273 3d5b     classifiers=[
-000004d0: 0d0a 2020 2020 2020 2020 2244 6576 656c  ..        "Devel
-000004e0: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-000004f0: 2033 202d 2041 6c70 6861 222c 0d0a 2020   3 - Alpha",..  
-00000500: 2020 2020 2020 2249 6e74 656e 6465 6420        "Intended 
-00000510: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
-00000520: 6c6f 7065 7273 222c 0d0a 2020 2020 2020  lopers",..      
-00000530: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
-00000540: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000550: 6e22 2c0d 0a20 2020 2020 2020 2022 5072  n",..        "Pr
-00000560: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000570: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000580: 3322 2c0d 0a20 2020 2020 2020 2022 546f  3",..        "To
-00000590: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
-000005a0: 4465 7665 6c6f 706d 656e 7422 0d0a 2020  Development"..  
-000005b0: 2020 5d0d 0a29                             ]..)
+00000000: 6672 6f6d 2073 6574 7570 746f 6f6c 7320  from setuptools 
+00000010: 696d 706f 7274 2073 6574 7570 2c20 6669  import setup, fi
+00000020: 6e64 5f70 6163 6b61 6765 730d 0a69 6d70  nd_packages..imp
+00000030: 6f72 7420 636f 6465 6373 0d0a 696d 706f  ort codecs..impo
+00000040: 7274 206f 730d 0a66 726f 6d20 6569 6e66  rt os..from einf
+00000050: 6163 6820 696d 706f 7274 205f 5f76 6572  ach import __ver
+00000060: 7369 6f6e 5f5f 0d0a 0d0a 6865 7265 203d  sion__....here =
+00000070: 206f 732e 7061 7468 2e61 6273 7061 7468   os.path.abspath
+00000080: 286f 732e 7061 7468 2e64 6972 6e61 6d65  (os.path.dirname
+00000090: 285f 5f66 696c 655f 5f29 290d 0a0d 0a77  (__file__))....w
+000000a0: 6974 6820 636f 6465 6373 2e6f 7065 6e28  ith codecs.open(
+000000b0: 6f73 2e70 6174 682e 6a6f 696e 2868 6572  os.path.join(her
+000000c0: 652c 2022 5245 4144 4d45 2e6d 6422 292c  e, "README.md"),
+000000d0: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
+000000e0: 2229 2061 7320 6668 3a0d 0a20 2020 206c  ") as fh:..    l
+000000f0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
+00000100: 3d20 225c 6e22 202b 2066 682e 7265 6164  = "\n" + fh.read
+00000110: 2829 0d0a 0d0a 5645 5253 494f 4e20 3d20  ()....VERSION = 
+00000120: 5f5f 7665 7273 696f 6e5f 5f0d 0a44 4553  __version__..DES
+00000130: 4352 4950 5449 4f4e 203d 2027 4120 636f  CRIPTION = 'A co
+00000140: 6c6c 6563 7469 6f6e 206f 6620 7573 6566  llection of usef
+00000150: 756c 2063 6f64 6520 2273 6e69 7070 6574  ul code "snippet
+00000160: 7322 270d 0a4c 4f4e 475f 4445 5343 5249  s"'..LONG_DESCRI
+00000170: 5054 494f 4e20 3d20 2741 2063 6f6c 6c65  PTION = 'A colle
+00000180: 6374 696f 6e20 6f66 2075 7365 6675 6c20  ction of useful 
+00000190: 636f 6465 2022 736e 6970 7065 7473 2220  code "snippets" 
+000001a0: 6f72 2022 6865 6c70 6572 7322 2074 6861  or "helpers" tha
+000001b0: 7420 696d 706c 656d 656e 7420 6c69 7474  t implement litt
+000001c0: 6c65 2062 7574 2061 6e6e 6f79 696e 6720  le but annoying 
+000001d0: 746f 2061 6464 2074 6869 6e67 7320 666f  to add things fo
+000001e0: 7220 796f 7527 0d0a 0d0a 2320 5365 7474  r you'....# Sett
+000001f0: 696e 6720 7570 0d0a 7365 7475 7028 0d0a  ing up..setup(..
+00000200: 2020 2020 6e61 6d65 3d22 6569 6e66 6163      name="einfac
+00000210: 6822 2c0d 0a20 2020 2076 6572 7369 6f6e  h",..    version
+00000220: 3d56 4552 5349 4f4e 2c0d 0a20 2020 2061  =VERSION,..    a
+00000230: 7574 686f 723d 2272 6f74 6772 7565 6e67  uthor="rotgrueng
+00000240: 656c 6220 2844 616e 6965 6c29 222c 0d0a  elb (Daniel)",..
+00000250: 2020 2020 6175 7468 6f72 5f65 6d61 696c      author_email
+00000260: 3d22 3c63 6f64 6540 726f 7467 7275 656e  ="<code@rotgruen
+00000270: 6765 6c62 2e6e 6574 3e22 2c0d 0a20 2020  gelb.net>",..   
+00000280: 2064 6573 6372 6970 7469 6f6e 3d44 4553   description=DES
+00000290: 4352 4950 5449 4f4e 2c0d 0a20 2020 206c  CRIPTION,..    l
+000002a0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
+000002b0: 636f 6e74 656e 745f 7479 7065 3d22 7465  content_type="te
+000002c0: 7874 2f6d 6172 6b64 6f77 6e22 2c0d 0a20  xt/markdown",.. 
+000002d0: 2020 206c 6f6e 675f 6465 7363 7269 7074     long_descript
+000002e0: 696f 6e3d 4c4f 4e47 5f44 4553 4352 4950  ion=LONG_DESCRIP
+000002f0: 5449 4f4e 202b 2022 5c6e 2220 2b20 6c6f  TION + "\n" + lo
+00000300: 6e67 5f64 6573 6372 6970 7469 6f6e 2c0d  ng_description,.
+00000310: 0a20 2020 2070 6163 6b61 6765 733d 6669  .    packages=fi
+00000320: 6e64 5f70 6163 6b61 6765 7328 292c 0d0a  nd_packages(),..
+00000330: 2020 2020 6c69 6365 6e73 653d 224d 4954      license="MIT
+00000340: 222c 0d0a 2020 2020 7572 6c3d 2268 7474  ",..    url="htt
+00000350: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000360: 726f 7467 7275 656e 6765 6c62 2f65 696e  rotgruengelb/ein
+00000370: 6661 6368 222c 0d0a 2020 2020 7072 6f6a  fach",..    proj
+00000380: 6563 745f 7572 6c73 3d7b 0d0a 2020 2020  ect_urls={..    
+00000390: 2753 6f75 7263 6527 3a20 2768 7474 7073  'Source': 'https
+000003a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 726f  ://github.com/ro
+000003b0: 7467 7275 656e 6765 6c62 2f65 696e 6661  tgruengelb/einfa
+000003c0: 6368 272c 0d0a 2020 2020 2749 7373 7565  ch',..    'Issue
+000003d0: 7327 3a20 2768 7474 7073 3a2f 2f67 6974  s': 'https://git
+000003e0: 6875 622e 636f 6d2f 726f 7467 7275 656e  hub.com/rotgruen
+000003f0: 6765 6c62 2f65 696e 6661 6368 2f69 7373  gelb/einfach/iss
+00000400: 7565 7327 2c0d 0a20 2020 2027 5769 6b69  ues',..    'Wiki
+00000410: 273a 2027 6874 7470 733a 2f2f 6769 7468  ': 'https://gith
+00000420: 7562 2e63 6f6d 2f72 6f74 6772 7565 6e67  ub.com/rotgrueng
+00000430: 656c 622f 6569 6e66 6163 682f 7769 6b69  elb/einfach/wiki
+00000440: 2f46 6561 7475 7265 7327 0d0a 2020 2020  /Features'..    
+00000450: 7d2c 0d0a 2020 2020 696e 7374 616c 6c5f  },..    install_
+00000460: 7265 7175 6972 6573 3d5b 5d2c 0d0a 2020  requires=[],..  
+00000470: 2020 6b65 7977 6f72 6473 3d5b 2770 7974    keywords=['pyt
+00000480: 686f 6e27 2c20 2768 656c 7065 7227 2c20  hon', 'helper', 
+00000490: 2768 656c 7065 7273 272c 2027 6865 6c70  'helpers', 'help
+000004a0: 272c 2027 6561 7379 2063 6f64 6527 2c20  ', 'easy code', 
+000004b0: 2765 6173 6520 6f66 2075 7365 272c 2022  'ease of use', "
+000004c0: 736e 6970 7065 7473 222c 2022 636f 6465  snippets", "code
+000004d0: 2073 6e69 7070 6574 7322 5d2c 0d0a 2020   snippets"],..  
+000004e0: 2020 636c 6173 7369 6669 6572 733d 5b0d    classifiers=[.
+000004f0: 0a20 2020 2020 2020 2022 4465 7665 6c6f  .        "Develo
+00000500: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+00000510: 3420 2d20 4265 7461 222c 0d0a 2020 2020  4 - Beta",..    
+00000520: 2020 2020 2249 6e74 656e 6465 6420 4175      "Intended Au
+00000530: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
+00000540: 7065 7273 222c 0d0a 2020 2020 2020 2020  pers",..        
+00000550: 2250 726f 6772 616d 6d69 6e67 204c 616e  "Programming Lan
+00000560: 6775 6167 6520 3a3a 2050 7974 686f 6e22  guage :: Python"
+00000570: 2c0d 0a20 2020 2020 2020 2022 5072 6f67  ,..        "Prog
+00000580: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000590: 203a 3a20 5079 7468 6f6e 203a 3a20 3322   :: Python :: 3"
+000005a0: 2c0d 0a20 2020 2020 2020 2022 546f 7069  ,..        "Topi
+000005b0: 6320 3a3a 2053 6f66 7477 6172 6520 4465  c :: Software De
+000005c0: 7665 6c6f 706d 656e 7422 2c0d 0a20 2020  velopment",..   
+000005d0: 2020 2020 2022 546f 7069 6320 3a3a 2053       "Topic :: S
+000005e0: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
+000005f0: 656e 7420 3a3a 2055 7365 7220 496e 7465  ent :: User Inte
+00000600: 7266 6163 6573 220d 0a20 2020 205d 0d0a  rfaces"..    ]..
+00000610: 29                                       )
```

