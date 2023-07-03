# Comparing `tmp/py-machineid-0.3.0.tar.gz` & `tmp/py-machineid-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-machineid-0.3.0.tar", last modified: Wed Feb  1 16:02:00 2023, max compression
+gzip compressed data, was "py-machineid-0.4.0.tar", last modified: Mon Jul  3 15:11:24 2023, max compression
```

## Comparing `py-machineid-0.3.0.tar` & `py-machineid-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 zeke       (501) staff       (20)        0 2023-02-01 16:02:00.422804 py-machineid-0.3.0/
--rw-r--r--   0 zeke       (501) staff       (20)     1067 2022-10-12 14:58:41.000000 py-machineid-0.3.0/LICENSE
--rw-r--r--   0 zeke       (501) staff       (20)     1436 2023-02-01 16:02:00.422553 py-machineid-0.3.0/PKG-INFO
--rw-r--r--   0 zeke       (501) staff       (20)      980 2023-02-01 15:57:09.000000 py-machineid-0.3.0/README.md
-drwxr-xr-x   0 zeke       (501) staff       (20)        0 2023-02-01 16:02:00.421266 py-machineid-0.3.0/machineid/
--rw-r--r--   0 zeke       (501) staff       (20)     2939 2023-02-01 15:59:06.000000 py-machineid-0.3.0/machineid/__init__.py
-drwxr-xr-x   0 zeke       (501) staff       (20)        0 2023-02-01 16:02:00.422293 py-machineid-0.3.0/py_machineid.egg-info/
--rw-r--r--   0 zeke       (501) staff       (20)     1436 2023-02-01 16:02:00.000000 py-machineid-0.3.0/py_machineid.egg-info/PKG-INFO
--rw-r--r--   0 zeke       (501) staff       (20)      227 2023-02-01 16:02:00.000000 py-machineid-0.3.0/py_machineid.egg-info/SOURCES.txt
--rw-r--r--   0 zeke       (501) staff       (20)        1 2023-02-01 16:02:00.000000 py-machineid-0.3.0/py_machineid.egg-info/dependency_links.txt
--rw-r--r--   0 zeke       (501) staff       (20)       12 2023-02-01 16:02:00.000000 py-machineid-0.3.0/py_machineid.egg-info/requires.txt
--rw-r--r--   0 zeke       (501) staff       (20)       10 2023-02-01 16:02:00.000000 py-machineid-0.3.0/py_machineid.egg-info/top_level.txt
--rw-r--r--   0 zeke       (501) staff       (20)       38 2023-02-01 16:02:00.422863 py-machineid-0.3.0/setup.cfg
--rw-r--r--   0 zeke       (501) staff       (20)      637 2023-02-01 15:58:57.000000 py-machineid-0.3.0/setup.py
+drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-03 15:11:24.318415 py-machineid-0.4.0/
+-rw-r--r--   0 zeke      (1000) zeke      (1000)     1826 2023-07-03 15:11:24.318415 py-machineid-0.4.0/PKG-INFO
+-rw-r--r--   0 zeke      (1000) zeke      (1000)      993 2023-07-03 15:10:46.000000 py-machineid-0.4.0/README.md
+drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-03 15:11:24.318415 py-machineid-0.4.0/machineid/
+-rw-r--r--   0 zeke      (1000) zeke      (1000)     3366 2023-07-03 15:10:46.000000 py-machineid-0.4.0/machineid/__init__.py
+drwxr-xr-x   0 zeke      (1000) zeke      (1000)        0 2023-07-03 15:11:24.318415 py-machineid-0.4.0/py_machineid.egg-info/
+-rw-r--r--   0 zeke      (1000) zeke      (1000)     1826 2023-07-03 15:11:24.000000 py-machineid-0.4.0/py_machineid.egg-info/PKG-INFO
+-rw-r--r--   0 zeke      (1000) zeke      (1000)      219 2023-07-03 15:11:24.000000 py-machineid-0.4.0/py_machineid.egg-info/SOURCES.txt
+-rw-r--r--   0 zeke      (1000) zeke      (1000)        1 2023-07-03 15:11:24.000000 py-machineid-0.4.0/py_machineid.egg-info/dependency_links.txt
+-rw-r--r--   0 zeke      (1000) zeke      (1000)       12 2023-07-03 15:11:24.000000 py-machineid-0.4.0/py_machineid.egg-info/requires.txt
+-rw-r--r--   0 zeke      (1000) zeke      (1000)       10 2023-07-03 15:11:24.000000 py-machineid-0.4.0/py_machineid.egg-info/top_level.txt
+-rw-r--r--   0 zeke      (1000) zeke      (1000)       38 2023-07-03 15:11:24.328415 py-machineid-0.4.0/setup.cfg
+-rw-r--r--   0 zeke      (1000) zeke      (1000)      637 2023-07-03 15:10:46.000000 py-machineid-0.4.0/setup.py
```

### Comparing `py-machineid-0.3.0/PKG-INFO` & `py-machineid-0.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,90 +1,115 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 2d6d  : 2.1.Name: py-m
 00000020: 6163 6869 6e65 6964 0a56 6572 7369 6f6e  achineid.Version
-00000030: 3a20 302e 332e 300a 5375 6d6d 6172 793a  : 0.3.0.Summary:
+00000030: 3a20 302e 342e 300a 5375 6d6d 6172 793a  : 0.4.0.Summary:
 00000040: 2047 6574 2074 6865 2075 6e69 7175 6520   Get the unique 
 00000050: 6d61 6368 696e 6520 4944 206f 6620 616e  machine ID of an
 00000060: 7920 686f 7374 2028 7769 7468 6f75 7420  y host (without 
 00000070: 6164 6d69 6e20 7072 6976 696c 6567 6573  admin privileges
 00000080: 290a 486f 6d65 2d70 6167 653a 2068 7474  ).Home-page: htt
 00000090: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 000000a0: 6b65 7967 656e 2d73 682f 7079 2d6d 6163  keygen-sh/py-mac
 000000b0: 6869 6e65 6964 0a41 7574 686f 723a 205a  hineid.Author: Z
 000000c0: 656b 6520 4761 6272 6965 6c73 650a 4175  eke Gabrielse.Au
 000000d0: 7468 6f72 2d65 6d61 696c 3a20 6f73 7340  thor-email: oss@
 000000e0: 6b65 7967 656e 2e73 680a 4c69 6365 6e73  keygen.sh.Licens
-000000f0: 653a 204d 4954 0a43 6c61 7373 6966 6965  e: MIT.Classifie
-00000100: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000110: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000120: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
-00000130: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
-00000140: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-00000150: 5420 4c69 6365 6e73 650a 436c 6173 7369  T License.Classi
-00000160: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-00000170: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000180: 6570 656e 6465 6e74 0a44 6573 6372 6970  ependent.Descrip
-00000190: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-000001a0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-000001b0: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
-000001c0: 4943 454e 5345 0a0a 2320 7079 2d6d 6163  ICENSE..# py-mac
-000001d0: 6869 6e65 6964 0a0a 4765 7420 7468 6520  hineid..Get the 
-000001e0: 756e 6971 7565 206d 6163 6869 6e65 2049  unique machine I
-000001f0: 4420 6f66 2061 6e79 2068 6f73 7420 2877  D of any host (w
-00000200: 6974 686f 7574 2061 646d 696e 2070 7269  ithout admin pri
-00000210: 7669 6c65 6765 7329 2e0a 0a53 706f 6e73  vileges)...Spons
-00000220: 6f72 6564 2062 793a 0a0a 5b21 5b4b 6579  ored by:..[![Key
-00000230: 6765 6e20 6c6f 676f 5d28 6874 7470 733a  gen logo](https:
-00000240: 2f2f 7573 6572 2d69 6d61 6765 732e 6769  //user-images.gi
-00000250: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00000260: 636f 6d2f 3639 3739 3733 372f 3137 3534  com/6979737/1754
-00000270: 3036 3136 392d 6264 3862 6630 3634 2d37  06169-bd8bf064-7
-00000280: 3334 332d 3462 6431 2d39 3462 372d 6137  343-4bd1-94b7-a7
-00000290: 3733 6563 6563 3037 6238 2e70 6e67 295d  73ecec07b8.png)]
-000002a0: 2868 7474 7073 3a2f 2f6b 6579 6765 6e2e  (https://keygen.
-000002b0: 7368 290a 0a5f 4120 736f 6674 7761 7265  sh).._A software
-000002c0: 206c 6963 656e 7369 6e67 2061 6e64 2064   licensing and d
-000002d0: 6973 7472 6962 7574 696f 6e20 4150 4920  istribution API 
-000002e0: 6275 696c 7420 666f 7220 6465 7665 6c6f  built for develo
-000002f0: 7065 7273 2e5f 0a0a 2323 2049 6e73 7461  pers._..## Insta
-00000300: 6c6c 0a0a 496e 7374 616c 6c20 7573 696e  ll..Install usin
-00000310: 6720 5b60 7069 7060 5d28 6874 7470 733a  g [`pip`](https:
-00000320: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
-00000330: 672f 332f 696e 7374 616c 6c69 6e67 2f69  g/3/installing/i
-00000340: 6e64 6578 2e68 746d 6c29 3a0a 0a60 6060  ndex.html):..```
-00000350: 6261 7368 0a70 7974 686f 6e33 202d 6d20  bash.python3 -m 
-00000360: 7069 7020 696e 7374 616c 6c20 7079 2d6d  pip install py-m
-00000370: 6163 6869 6e65 6964 0a60 6060 0a0a 2323  achineid.```..##
-00000380: 2055 7361 6765 0a0a 546f 206f 6274 6169   Usage..To obtai
-00000390: 6e20 7468 6520 7261 7720 4755 4944 206f  n the raw GUID o
-000003a0: 6620 7468 6520 6465 7669 6365 2c20 7573  f the device, us
-000003b0: 6520 6069 6428 2920 2d3e 2073 7472 603a  e `id() -> str`:
-000003c0: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
-000003d0: 7274 206d 6163 6869 6e65 6964 0a0a 7072  rt machineid..pr
-000003e0: 696e 7428 6d61 6368 696e 6569 642e 6964  int(machineid.id
-000003f0: 2829 290a 6060 600a 0a54 6f20 6f62 7461  ()).```..To obta
-00000400: 696e 2061 6e20 616e 6f6e 796d 697a 6564  in an anonymized
-00000410: 2028 6861 7368 6564 2920 7665 7273 696f   (hashed) versio
-00000420: 6e20 6f66 2074 6865 2047 5549 442c 2073  n of the GUID, s
-00000430: 6565 2062 656c 6f77 2e20 5468 650a 6068  ee below. The.`h
-00000440: 6173 6865 645f 6964 2873 7472 2920 2d3e  ashed_id(str) ->
-00000450: 2073 7472 6020 6675 6e63 7469 6f6e 2074   str` function t
-00000460: 616b 6573 2061 6e20 6f70 7469 6f6e 616c  akes an optional
-00000470: 2061 7070 6c69 6361 7469 6f6e 2049 442c   application ID,
-00000480: 0a77 6869 6368 2077 696c 6c20 656e 7375  .which will ensu
-00000490: 7265 2061 2075 6e69 7175 6520 4944 2070  re a unique ID p
-000004a0: 6572 2d61 7070 2066 6f72 2074 6865 2073  er-app for the s
-000004b0: 616d 6520 6465 7669 6365 2e0a 0a60 6060  ame device...```
-000004c0: 7079 7468 6f6e 0a69 6d70 6f72 7420 6d61  python.import ma
-000004d0: 6368 696e 6569 640a 0a70 7269 6e74 286d  chineid..print(m
-000004e0: 6163 6869 6e65 6964 2e68 6173 6865 645f  achineid.hashed_
-000004f0: 6964 2827 6d79 6170 7069 6427 2929 0a70  id('myappid')).p
-00000500: 7269 6e74 286d 6163 6869 6e65 6964 2e68  rint(machineid.h
-00000510: 6173 6865 645f 6964 2829 290a 6060 600a  ashed_id()).```.
-00000520: 0a23 2320 5468 616e 6b73 0a0a 5370 6563  .## Thanks..Spec
-00000530: 6961 6c20 7468 616e 6b73 2074 6f20 4465  ial thanks to De
-00000540: 6e69 7320 4272 6f64 6265 636b 2066 6f72  nis Brodbeck for
-00000550: 2068 6973 2047 6f20 7061 636b 6167 652c   his Go package,
-00000560: 205b 606d 6163 6869 6e65 6964 605d 2868   [`machineid`](h
-00000570: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000580: 6d2f 6465 6e69 7362 726f 6462 6563 6b2f  m/denisbrodbeck/
-00000590: 6d61 6368 696e 6569 6429 2e0a            machineid)..
+000000f0: 653a 204d 4954 0a44 6573 6372 6970 7469  e: MIT.Descripti
+00000100: 6f6e 3a20 2320 7079 2d6d 6163 6869 6e65  on: # py-machine
+00000110: 6964 0a20 2020 2020 2020 200a 2020 2020  id.        .    
+00000120: 2020 2020 4765 7420 7468 6520 756e 6971      Get the uniq
+00000130: 7565 206d 6163 6869 6e65 2049 4420 6f66  ue machine ID of
+00000140: 2061 6e79 2068 6f73 7420 2877 6974 686f   any host (witho
+00000150: 7574 2061 646d 696e 2070 7269 7669 6c65  ut admin privile
+00000160: 6765 7329 2e0a 2020 2020 2020 2020 0a20  ges)..        . 
+00000170: 2020 2020 2020 2053 706f 6e73 6f72 6564         Sponsored
+00000180: 2062 793a 0a20 2020 2020 2020 200a 2020   by:.        .  
+00000190: 2020 2020 2020 3c61 2068 7265 663d 2268        <a href="h
+000001a0: 7474 7073 3a2f 2f6b 6579 6765 6e2e 7368  ttps://keygen.sh
+000001b0: 3f72 6566 3d74 7970 6564 5f70 6172 616d  ?ref=typed_param
+000001c0: 7322 3e0a 2020 2020 2020 2020 2020 3c64  s">.          <d
+000001d0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+000001e0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000001f0: 2f2f 6b65 7967 656e 2e73 682f 696d 6167  //keygen.sh/imag
+00000200: 6573 2f6c 6f67 6f2d 7069 6c6c 2e70 6e67  es/logo-pill.png
+00000210: 2220 7769 6474 683d 2232 3030 2220 616c  " width="200" al
+00000220: 743d 224b 6579 6765 6e22 3e0a 2020 2020  t="Keygen">.    
+00000230: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+00000240: 2020 2020 203c 2f61 3e0a 2020 2020 2020       </a>.      
+00000250: 2020 0a20 2020 2020 2020 205f 416e 206f    .        _An o
+00000260: 7065 6e2c 2073 6f75 7263 652d 6176 6169  pen, source-avai
+00000270: 6c61 626c 6520 736f 6674 7761 7265 206c  lable software l
+00000280: 6963 656e 7369 6e67 2061 6e64 2064 6973  icensing and dis
+00000290: 7472 6962 7574 696f 6e20 4150 492e 5f0a  tribution API._.
+000002a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000002b0: 2023 2320 496e 7374 616c 6c0a 2020 2020   ## Install.    
+000002c0: 2020 2020 0a20 2020 2020 2020 2049 6e73      .        Ins
+000002d0: 7461 6c6c 2075 7369 6e67 205b 6070 6970  tall using [`pip
+000002e0: 605d 2868 7474 7073 3a2f 2f64 6f63 732e  `](https://docs.
+000002f0: 7079 7468 6f6e 2e6f 7267 2f33 2f69 6e73  python.org/3/ins
+00000300: 7461 6c6c 696e 672f 696e 6465 782e 6874  talling/index.ht
+00000310: 6d6c 293a 0a20 2020 2020 2020 200a 2020  ml):.        .  
+00000320: 2020 2020 2020 6060 6062 6173 680a 2020        ```bash.  
+00000330: 2020 2020 2020 7079 7468 6f6e 3320 2d6d        python3 -m
+00000340: 2070 6970 2069 6e73 7461 6c6c 2070 792d   pip install py-
+00000350: 6d61 6368 696e 6569 640a 2020 2020 2020  machineid.      
+00000360: 2020 6060 600a 2020 2020 2020 2020 0a20    ```.        . 
+00000370: 2020 2020 2020 2023 2320 5573 6167 650a         ## Usage.
+00000380: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000390: 2054 6f20 6f62 7461 696e 2074 6865 2072   To obtain the r
+000003a0: 6177 2047 5549 4420 6f66 2074 6865 2064  aw GUID of the d
+000003b0: 6576 6963 652c 2075 7365 2060 6964 2829  evice, use `id()
+000003c0: 202d 3e20 7374 7260 3a0a 2020 2020 2020   -> str`:.      
+000003d0: 2020 0a20 2020 2020 2020 2060 6060 7079    .        ```py
+000003e0: 7468 6f6e 0a20 2020 2020 2020 2069 6d70  thon.        imp
+000003f0: 6f72 7420 6d61 6368 696e 6569 640a 2020  ort machineid.  
+00000400: 2020 2020 2020 0a20 2020 2020 2020 2070        .        p
+00000410: 7269 6e74 286d 6163 6869 6e65 6964 2e69  rint(machineid.i
+00000420: 6428 2929 0a20 2020 2020 2020 2060 6060  d()).        ```
+00000430: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000440: 2020 546f 206f 6274 6169 6e20 616e 2061    To obtain an a
+00000450: 6e6f 6e79 6d69 7a65 6420 2868 6173 6865  nonymized (hashe
+00000460: 6429 2076 6572 7369 6f6e 206f 6620 7468  d) version of th
+00000470: 6520 4755 4944 2c20 7365 6520 6265 6c6f  e GUID, see belo
+00000480: 772e 2054 6865 0a20 2020 2020 2020 2060  w. The.        `
+00000490: 6861 7368 6564 5f69 6428 7374 7229 202d  hashed_id(str) -
+000004a0: 3e20 7374 7260 2066 756e 6374 696f 6e20  > str` function 
+000004b0: 7461 6b65 7320 616e 206f 7074 696f 6e61  takes an optiona
+000004c0: 6c20 6170 706c 6963 6174 696f 6e20 4944  l application ID
+000004d0: 2c0a 2020 2020 2020 2020 7768 6963 6820  ,.        which 
+000004e0: 7769 6c6c 2065 6e73 7572 6520 6120 756e  will ensure a un
+000004f0: 6971 7565 2049 4420 7065 722d 6170 7020  ique ID per-app 
+00000500: 666f 7220 7468 6520 7361 6d65 2064 6576  for the same dev
+00000510: 6963 652e 0a20 2020 2020 2020 200a 2020  ice..        .  
+00000520: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
+00000530: 2020 2020 2020 2020 696d 706f 7274 206d          import m
+00000540: 6163 6869 6e65 6964 0a20 2020 2020 2020  achineid.       
+00000550: 200a 2020 2020 2020 2020 7072 696e 7428   .        print(
+00000560: 6d61 6368 696e 6569 642e 6861 7368 6564  machineid.hashed
+00000570: 5f69 6428 276d 7961 7070 6964 2729 290a  _id('myappid')).
+00000580: 2020 2020 2020 2020 7072 696e 7428 6d61          print(ma
+00000590: 6368 696e 6569 642e 6861 7368 6564 5f69  chineid.hashed_i
+000005a0: 6428 2929 0a20 2020 2020 2020 2060 6060  d()).        ```
+000005b0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000005c0: 2020 2323 2054 6861 6e6b 730a 2020 2020    ## Thanks.    
+000005d0: 2020 2020 0a20 2020 2020 2020 2053 7065      .        Spe
+000005e0: 6369 616c 2074 6861 6e6b 7320 746f 2044  cial thanks to D
+000005f0: 656e 6973 2042 726f 6462 6563 6b20 666f  enis Brodbeck fo
+00000600: 7220 6869 7320 476f 2070 6163 6b61 6765  r his Go package
+00000610: 2c20 5b60 6d61 6368 696e 6569 6460 5d28  , [`machineid`](
+00000620: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000630: 6f6d 2f64 656e 6973 6272 6f64 6265 636b  om/denisbrodbeck
+00000640: 2f6d 6163 6869 6e65 6964 292e 0a20 2020  /machineid)..   
+00000650: 2020 2020 200a 506c 6174 666f 726d 3a20       .Platform: 
+00000660: 554e 4b4e 4f57 4e0a 436c 6173 7369 6669  UNKNOWN.Classifi
+00000670: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000680: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000690: 6f6e 203a 3a20 330a 436c 6173 7369 6669  on :: 3.Classifi
+000006a0: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
+000006b0: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+000006c0: 4954 204c 6963 656e 7365 0a43 6c61 7373  IT License.Class
+000006d0: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
+000006e0: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+000006f0: 6465 7065 6e64 656e 740a 4465 7363 7269  dependent.Descri
+00000700: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
+00000710: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
+00000720: 6e0a                                     n.
```

### Comparing `py-machineid-0.3.0/README.md` & `py-machineid-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 00000000: 2320 7079 2d6d 6163 6869 6e65 6964 0a0a  # py-machineid..
 00000010: 4765 7420 7468 6520 756e 6971 7565 206d  Get the unique m
 00000020: 6163 6869 6e65 2049 4420 6f66 2061 6e79  achine ID of any
 00000030: 2068 6f73 7420 2877 6974 686f 7574 2061   host (without a
 00000040: 646d 696e 2070 7269 7669 6c65 6765 7329  dmin privileges)
 00000050: 2e0a 0a53 706f 6e73 6f72 6564 2062 793a  ...Sponsored by:
-00000060: 0a0a 5b21 5b4b 6579 6765 6e20 6c6f 676f  ..[![Keygen logo
-00000070: 5d28 6874 7470 733a 2f2f 7573 6572 2d69  ](https://user-i
-00000080: 6d61 6765 732e 6769 7468 7562 7573 6572  mages.githubuser
-00000090: 636f 6e74 656e 742e 636f 6d2f 3639 3739  content.com/6979
-000000a0: 3733 372f 3137 3534 3036 3136 392d 6264  737/175406169-bd
-000000b0: 3862 6630 3634 2d37 3334 332d 3462 6431  8bf064-7343-4bd1
-000000c0: 2d39 3462 372d 6137 3733 6563 6563 3037  -94b7-a773ecec07
-000000d0: 6238 2e70 6e67 295d 2868 7474 7073 3a2f  b8.png)](https:/
-000000e0: 2f6b 6579 6765 6e2e 7368 290a 0a5f 4120  /keygen.sh).._A 
-000000f0: 736f 6674 7761 7265 206c 6963 656e 7369  software licensi
-00000100: 6e67 2061 6e64 2064 6973 7472 6962 7574  ng and distribut
-00000110: 696f 6e20 4150 4920 6275 696c 7420 666f  ion API built fo
-00000120: 7220 6465 7665 6c6f 7065 7273 2e5f 0a0a  r developers._..
-00000130: 2323 2049 6e73 7461 6c6c 0a0a 496e 7374  ## Install..Inst
-00000140: 616c 6c20 7573 696e 6720 5b60 7069 7060  all using [`pip`
-00000150: 5d28 6874 7470 733a 2f2f 646f 6373 2e70  ](https://docs.p
-00000160: 7974 686f 6e2e 6f72 672f 332f 696e 7374  ython.org/3/inst
-00000170: 616c 6c69 6e67 2f69 6e64 6578 2e68 746d  alling/index.htm
-00000180: 6c29 3a0a 0a60 6060 6261 7368 0a70 7974  l):..```bash.pyt
-00000190: 686f 6e33 202d 6d20 7069 7020 696e 7374  hon3 -m pip inst
-000001a0: 616c 6c20 7079 2d6d 6163 6869 6e65 6964  all py-machineid
-000001b0: 0a60 6060 0a0a 2323 2055 7361 6765 0a0a  .```..## Usage..
-000001c0: 546f 206f 6274 6169 6e20 7468 6520 7261  To obtain the ra
-000001d0: 7720 4755 4944 206f 6620 7468 6520 6465  w GUID of the de
-000001e0: 7669 6365 2c20 7573 6520 6069 6428 2920  vice, use `id() 
-000001f0: 2d3e 2073 7472 603a 0a0a 6060 6070 7974  -> str`:..```pyt
-00000200: 686f 6e0a 696d 706f 7274 206d 6163 6869  hon.import machi
-00000210: 6e65 6964 0a0a 7072 696e 7428 6d61 6368  neid..print(mach
-00000220: 696e 6569 642e 6964 2829 290a 6060 600a  ineid.id()).```.
-00000230: 0a54 6f20 6f62 7461 696e 2061 6e20 616e  .To obtain an an
-00000240: 6f6e 796d 697a 6564 2028 6861 7368 6564  onymized (hashed
-00000250: 2920 7665 7273 696f 6e20 6f66 2074 6865  ) version of the
-00000260: 2047 5549 442c 2073 6565 2062 656c 6f77   GUID, see below
-00000270: 2e20 5468 650a 6068 6173 6865 645f 6964  . The.`hashed_id
-00000280: 2873 7472 2920 2d3e 2073 7472 6020 6675  (str) -> str` fu
-00000290: 6e63 7469 6f6e 2074 616b 6573 2061 6e20  nction takes an 
-000002a0: 6f70 7469 6f6e 616c 2061 7070 6c69 6361  optional applica
-000002b0: 7469 6f6e 2049 442c 0a77 6869 6368 2077  tion ID,.which w
-000002c0: 696c 6c20 656e 7375 7265 2061 2075 6e69  ill ensure a uni
-000002d0: 7175 6520 4944 2070 6572 2d61 7070 2066  que ID per-app f
-000002e0: 6f72 2074 6865 2073 616d 6520 6465 7669  or the same devi
-000002f0: 6365 2e0a 0a60 6060 7079 7468 6f6e 0a69  ce...```python.i
-00000300: 6d70 6f72 7420 6d61 6368 696e 6569 640a  mport machineid.
-00000310: 0a70 7269 6e74 286d 6163 6869 6e65 6964  .print(machineid
-00000320: 2e68 6173 6865 645f 6964 2827 6d79 6170  .hashed_id('myap
-00000330: 7069 6427 2929 0a70 7269 6e74 286d 6163  pid')).print(mac
-00000340: 6869 6e65 6964 2e68 6173 6865 645f 6964  hineid.hashed_id
-00000350: 2829 290a 6060 600a 0a23 2320 5468 616e  ()).```..## Than
-00000360: 6b73 0a0a 5370 6563 6961 6c20 7468 616e  ks..Special than
-00000370: 6b73 2074 6f20 4465 6e69 7320 4272 6f64  ks to Denis Brod
-00000380: 6265 636b 2066 6f72 2068 6973 2047 6f20  beck for his Go 
-00000390: 7061 636b 6167 652c 205b 606d 6163 6869  package, [`machi
-000003a0: 6e65 6964 605d 2868 7474 7073 3a2f 2f67  neid`](https://g
-000003b0: 6974 6875 622e 636f 6d2f 6465 6e69 7362  ithub.com/denisb
-000003c0: 726f 6462 6563 6b2f 6d61 6368 696e 6569  rodbeck/machinei
-000003d0: 6429 2e0a                                d)..
+00000060: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+00000070: 3a2f 2f6b 6579 6765 6e2e 7368 3f72 6566  ://keygen.sh?ref
+00000080: 3d74 7970 6564 5f70 6172 616d 7322 3e0a  =typed_params">.
+00000090: 2020 3c64 6976 3e0a 2020 2020 3c69 6d67    <div>.    <img
+000000a0: 2073 7263 3d22 6874 7470 733a 2f2f 6b65   src="https://ke
+000000b0: 7967 656e 2e73 682f 696d 6167 6573 2f6c  ygen.sh/images/l
+000000c0: 6f67 6f2d 7069 6c6c 2e70 6e67 2220 7769  ogo-pill.png" wi
+000000d0: 6474 683d 2232 3030 2220 616c 743d 224b  dth="200" alt="K
+000000e0: 6579 6765 6e22 3e0a 2020 3c2f 6469 763e  eygen">.  </div>
+000000f0: 0a3c 2f61 3e0a 0a5f 416e 206f 7065 6e2c  .</a>.._An open,
+00000100: 2073 6f75 7263 652d 6176 6169 6c61 626c   source-availabl
+00000110: 6520 736f 6674 7761 7265 206c 6963 656e  e software licen
+00000120: 7369 6e67 2061 6e64 2064 6973 7472 6962  sing and distrib
+00000130: 7574 696f 6e20 4150 492e 5f0a 0a23 2320  ution API._..## 
+00000140: 496e 7374 616c 6c0a 0a49 6e73 7461 6c6c  Install..Install
+00000150: 2075 7369 6e67 205b 6070 6970 605d 2868   using [`pip`](h
+00000160: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
+00000170: 6f6e 2e6f 7267 2f33 2f69 6e73 7461 6c6c  on.org/3/install
+00000180: 696e 672f 696e 6465 782e 6874 6d6c 293a  ing/index.html):
+00000190: 0a0a 6060 6062 6173 680a 7079 7468 6f6e  ..```bash.python
+000001a0: 3320 2d6d 2070 6970 2069 6e73 7461 6c6c  3 -m pip install
+000001b0: 2070 792d 6d61 6368 696e 6569 640a 6060   py-machineid.``
+000001c0: 600a 0a23 2320 5573 6167 650a 0a54 6f20  `..## Usage..To 
+000001d0: 6f62 7461 696e 2074 6865 2072 6177 2047  obtain the raw G
+000001e0: 5549 4420 6f66 2074 6865 2064 6576 6963  UID of the devic
+000001f0: 652c 2075 7365 2060 6964 2829 202d 3e20  e, use `id() -> 
+00000200: 7374 7260 3a0a 0a60 6060 7079 7468 6f6e  str`:..```python
+00000210: 0a69 6d70 6f72 7420 6d61 6368 696e 6569  .import machinei
+00000220: 640a 0a70 7269 6e74 286d 6163 6869 6e65  d..print(machine
+00000230: 6964 2e69 6428 2929 0a60 6060 0a0a 546f  id.id()).```..To
+00000240: 206f 6274 6169 6e20 616e 2061 6e6f 6e79   obtain an anony
+00000250: 6d69 7a65 6420 2868 6173 6865 6429 2076  mized (hashed) v
+00000260: 6572 7369 6f6e 206f 6620 7468 6520 4755  ersion of the GU
+00000270: 4944 2c20 7365 6520 6265 6c6f 772e 2054  ID, see below. T
+00000280: 6865 0a60 6861 7368 6564 5f69 6428 7374  he.`hashed_id(st
+00000290: 7229 202d 3e20 7374 7260 2066 756e 6374  r) -> str` funct
+000002a0: 696f 6e20 7461 6b65 7320 616e 206f 7074  ion takes an opt
+000002b0: 696f 6e61 6c20 6170 706c 6963 6174 696f  ional applicatio
+000002c0: 6e20 4944 2c0a 7768 6963 6820 7769 6c6c  n ID,.which will
+000002d0: 2065 6e73 7572 6520 6120 756e 6971 7565   ensure a unique
+000002e0: 2049 4420 7065 722d 6170 7020 666f 7220   ID per-app for 
+000002f0: 7468 6520 7361 6d65 2064 6576 6963 652e  the same device.
+00000300: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00000310: 7274 206d 6163 6869 6e65 6964 0a0a 7072  rt machineid..pr
+00000320: 696e 7428 6d61 6368 696e 6569 642e 6861  int(machineid.ha
+00000330: 7368 6564 5f69 6428 276d 7961 7070 6964  shed_id('myappid
+00000340: 2729 290a 7072 696e 7428 6d61 6368 696e  ')).print(machin
+00000350: 6569 642e 6861 7368 6564 5f69 6428 2929  eid.hashed_id())
+00000360: 0a60 6060 0a0a 2323 2054 6861 6e6b 730a  .```..## Thanks.
+00000370: 0a53 7065 6369 616c 2074 6861 6e6b 7320  .Special thanks 
+00000380: 746f 2044 656e 6973 2042 726f 6462 6563  to Denis Brodbec
+00000390: 6b20 666f 7220 6869 7320 476f 2070 6163  k for his Go pac
+000003a0: 6b61 6765 2c20 5b60 6d61 6368 696e 6569  kage, [`machinei
+000003b0: 6460 5d28 6874 7470 733a 2f2f 6769 7468  d`](https://gith
+000003c0: 7562 2e63 6f6d 2f64 656e 6973 6272 6f64  ub.com/denisbrod
+000003d0: 6265 636b 2f6d 6163 6869 6e65 6964 292e  beck/machineid).
+000003e0: 0a                                       .
```

### Comparing `py-machineid-0.3.0/machineid/__init__.py` & `py-machineid-0.4.0/machineid/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,26 +18,27 @@
     ce2127ade536eaa9529f4a7b73141bbc2f094c46e32742c97679e186e7f13fde
 
 Special thanks to Denis Brodbeck for his Go package, machineid (https://github.com/denisbrodbeck/machineid).
 
 :license: MIT, see LICENSE for more details.
 """
 
-__version__ = '0.3.0'
+__version__ = '0.2.1'
 __author__  = 'Zeke Gabrielse'
 __credits__ = 'https://github.com/denisbrodbeck/machineid'
 
+from platform import uname
 from sys import platform
 import subprocess
 import hashlib
 import hmac
 
 def __exec__(cmd: str) -> str:
   try:
-    return subprocess.run(cmd, shell=True, capture_output=True, check=True, encoding="utf-8") \
+    return subprocess.run(cmd, shell=True, capture_output=True, check=True, encoding='utf-8') \
                      .stdout \
                      .strip()
   except:
     return None
 
 def __read__(path: str) -> str:
   try:
@@ -53,23 +54,26 @@
     with WinRegistry() as reg:
       return reg.read_entry(registry, key) \
                 .value \
                 .strip()
   except:
     return None
 
-def id() -> str:
+def id(winregistry: bool = True) -> str:
   """
   id returns the platform specific device GUID of the current host OS.
   """
   if platform == 'darwin':
     id = __exec__("ioreg -d2 -c IOPlatformExpertDevice | awk -F\\\" '/IOPlatformUUID/{print $(NF-1)}'")
 
   if platform == 'win32' or platform == 'cygwin' or platform == 'msys':
-    id = __reg__('HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Cryptography', 'MachineGuid')
+    if winregistry:
+      id = __reg__('HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Cryptography', 'MachineGuid')
+    else:
+      id = __exec__("powershell.exe -ExecutionPolicy bypass -command '(Get-CimInstance -Class Win32_ComputerSystemProduct).UUID'")
     if not id:
       id = __exec__('wmic csproduct get uuid').split('\n')[2] \
                                               .strip()
 
   if platform.startswith('linux'):
     id = __read__('/var/lib/dbus/machine-id')
     if not id:
@@ -80,24 +84,27 @@
         if 'docker' in cgroup:
           id = __exec__('head -1 /proc/self/cgroup | cut -d/ -f3')
     if not id:
       mountinfo = __read__('/proc/self/mountinfo')
       if mountinfo:
         if 'docker' in mountinfo:
           id = __exec__("grep 'systemd' /proc/self/mountinfo | cut -d/ -f3")
+    if not id:
+      if 'microsoft' in uname().release: # wsl
+        id = __exec__("powershell.exe -ExecutionPolicy bypass -command '(Get-CimInstance -Class Win32_ComputerSystemProduct).UUID'")
 
   if platform.startswith('openbsd') or platform.startswith('freebsd'):
     id = __read__('/etc/hostid')
     if not id:
       id = __exec__('kenv -q smbios.system.uuid')
 
   if not id:
     raise Exception('failed to obtain id on platform {}'.format(platform))
 
   return id
 
-def hashed_id(app_id: str = '') -> str:
+def hashed_id(app_id: str = '', **kwargs) -> str:
   """
   hashed_id returns the device's native GUID, hashed using HMAC-SHA256 with an optional application ID.
   """
 
-  return hmac.new(bytes(app_id.encode()), id().encode(), hashlib.sha256).hexdigest()
+  return hmac.new(bytes(app_id.encode()), id(**kwargs).encode(), hashlib.sha256).hexdigest()
```

### Comparing `py-machineid-0.3.0/py_machineid.egg-info/PKG-INFO` & `py-machineid-0.4.0/py_machineid.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,90 +1,115 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 2d6d  : 2.1.Name: py-m
 00000020: 6163 6869 6e65 6964 0a56 6572 7369 6f6e  achineid.Version
-00000030: 3a20 302e 332e 300a 5375 6d6d 6172 793a  : 0.3.0.Summary:
+00000030: 3a20 302e 342e 300a 5375 6d6d 6172 793a  : 0.4.0.Summary:
 00000040: 2047 6574 2074 6865 2075 6e69 7175 6520   Get the unique 
 00000050: 6d61 6368 696e 6520 4944 206f 6620 616e  machine ID of an
 00000060: 7920 686f 7374 2028 7769 7468 6f75 7420  y host (without 
 00000070: 6164 6d69 6e20 7072 6976 696c 6567 6573  admin privileges
 00000080: 290a 486f 6d65 2d70 6167 653a 2068 7474  ).Home-page: htt
 00000090: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 000000a0: 6b65 7967 656e 2d73 682f 7079 2d6d 6163  keygen-sh/py-mac
 000000b0: 6869 6e65 6964 0a41 7574 686f 723a 205a  hineid.Author: Z
 000000c0: 656b 6520 4761 6272 6965 6c73 650a 4175  eke Gabrielse.Au
 000000d0: 7468 6f72 2d65 6d61 696c 3a20 6f73 7340  thor-email: oss@
 000000e0: 6b65 7967 656e 2e73 680a 4c69 6365 6e73  keygen.sh.Licens
-000000f0: 653a 204d 4954 0a43 6c61 7373 6966 6965  e: MIT.Classifie
-00000100: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000110: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000120: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
-00000130: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
-00000140: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-00000150: 5420 4c69 6365 6e73 650a 436c 6173 7369  T License.Classi
-00000160: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-00000170: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000180: 6570 656e 6465 6e74 0a44 6573 6372 6970  ependent.Descrip
-00000190: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-000001a0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-000001b0: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
-000001c0: 4943 454e 5345 0a0a 2320 7079 2d6d 6163  ICENSE..# py-mac
-000001d0: 6869 6e65 6964 0a0a 4765 7420 7468 6520  hineid..Get the 
-000001e0: 756e 6971 7565 206d 6163 6869 6e65 2049  unique machine I
-000001f0: 4420 6f66 2061 6e79 2068 6f73 7420 2877  D of any host (w
-00000200: 6974 686f 7574 2061 646d 696e 2070 7269  ithout admin pri
-00000210: 7669 6c65 6765 7329 2e0a 0a53 706f 6e73  vileges)...Spons
-00000220: 6f72 6564 2062 793a 0a0a 5b21 5b4b 6579  ored by:..[![Key
-00000230: 6765 6e20 6c6f 676f 5d28 6874 7470 733a  gen logo](https:
-00000240: 2f2f 7573 6572 2d69 6d61 6765 732e 6769  //user-images.gi
-00000250: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00000260: 636f 6d2f 3639 3739 3733 372f 3137 3534  com/6979737/1754
-00000270: 3036 3136 392d 6264 3862 6630 3634 2d37  06169-bd8bf064-7
-00000280: 3334 332d 3462 6431 2d39 3462 372d 6137  343-4bd1-94b7-a7
-00000290: 3733 6563 6563 3037 6238 2e70 6e67 295d  73ecec07b8.png)]
-000002a0: 2868 7474 7073 3a2f 2f6b 6579 6765 6e2e  (https://keygen.
-000002b0: 7368 290a 0a5f 4120 736f 6674 7761 7265  sh).._A software
-000002c0: 206c 6963 656e 7369 6e67 2061 6e64 2064   licensing and d
-000002d0: 6973 7472 6962 7574 696f 6e20 4150 4920  istribution API 
-000002e0: 6275 696c 7420 666f 7220 6465 7665 6c6f  built for develo
-000002f0: 7065 7273 2e5f 0a0a 2323 2049 6e73 7461  pers._..## Insta
-00000300: 6c6c 0a0a 496e 7374 616c 6c20 7573 696e  ll..Install usin
-00000310: 6720 5b60 7069 7060 5d28 6874 7470 733a  g [`pip`](https:
-00000320: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
-00000330: 672f 332f 696e 7374 616c 6c69 6e67 2f69  g/3/installing/i
-00000340: 6e64 6578 2e68 746d 6c29 3a0a 0a60 6060  ndex.html):..```
-00000350: 6261 7368 0a70 7974 686f 6e33 202d 6d20  bash.python3 -m 
-00000360: 7069 7020 696e 7374 616c 6c20 7079 2d6d  pip install py-m
-00000370: 6163 6869 6e65 6964 0a60 6060 0a0a 2323  achineid.```..##
-00000380: 2055 7361 6765 0a0a 546f 206f 6274 6169   Usage..To obtai
-00000390: 6e20 7468 6520 7261 7720 4755 4944 206f  n the raw GUID o
-000003a0: 6620 7468 6520 6465 7669 6365 2c20 7573  f the device, us
-000003b0: 6520 6069 6428 2920 2d3e 2073 7472 603a  e `id() -> str`:
-000003c0: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
-000003d0: 7274 206d 6163 6869 6e65 6964 0a0a 7072  rt machineid..pr
-000003e0: 696e 7428 6d61 6368 696e 6569 642e 6964  int(machineid.id
-000003f0: 2829 290a 6060 600a 0a54 6f20 6f62 7461  ()).```..To obta
-00000400: 696e 2061 6e20 616e 6f6e 796d 697a 6564  in an anonymized
-00000410: 2028 6861 7368 6564 2920 7665 7273 696f   (hashed) versio
-00000420: 6e20 6f66 2074 6865 2047 5549 442c 2073  n of the GUID, s
-00000430: 6565 2062 656c 6f77 2e20 5468 650a 6068  ee below. The.`h
-00000440: 6173 6865 645f 6964 2873 7472 2920 2d3e  ashed_id(str) ->
-00000450: 2073 7472 6020 6675 6e63 7469 6f6e 2074   str` function t
-00000460: 616b 6573 2061 6e20 6f70 7469 6f6e 616c  akes an optional
-00000470: 2061 7070 6c69 6361 7469 6f6e 2049 442c   application ID,
-00000480: 0a77 6869 6368 2077 696c 6c20 656e 7375  .which will ensu
-00000490: 7265 2061 2075 6e69 7175 6520 4944 2070  re a unique ID p
-000004a0: 6572 2d61 7070 2066 6f72 2074 6865 2073  er-app for the s
-000004b0: 616d 6520 6465 7669 6365 2e0a 0a60 6060  ame device...```
-000004c0: 7079 7468 6f6e 0a69 6d70 6f72 7420 6d61  python.import ma
-000004d0: 6368 696e 6569 640a 0a70 7269 6e74 286d  chineid..print(m
-000004e0: 6163 6869 6e65 6964 2e68 6173 6865 645f  achineid.hashed_
-000004f0: 6964 2827 6d79 6170 7069 6427 2929 0a70  id('myappid')).p
-00000500: 7269 6e74 286d 6163 6869 6e65 6964 2e68  rint(machineid.h
-00000510: 6173 6865 645f 6964 2829 290a 6060 600a  ashed_id()).```.
-00000520: 0a23 2320 5468 616e 6b73 0a0a 5370 6563  .## Thanks..Spec
-00000530: 6961 6c20 7468 616e 6b73 2074 6f20 4465  ial thanks to De
-00000540: 6e69 7320 4272 6f64 6265 636b 2066 6f72  nis Brodbeck for
-00000550: 2068 6973 2047 6f20 7061 636b 6167 652c   his Go package,
-00000560: 205b 606d 6163 6869 6e65 6964 605d 2868   [`machineid`](h
-00000570: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000580: 6d2f 6465 6e69 7362 726f 6462 6563 6b2f  m/denisbrodbeck/
-00000590: 6d61 6368 696e 6569 6429 2e0a            machineid)..
+000000f0: 653a 204d 4954 0a44 6573 6372 6970 7469  e: MIT.Descripti
+00000100: 6f6e 3a20 2320 7079 2d6d 6163 6869 6e65  on: # py-machine
+00000110: 6964 0a20 2020 2020 2020 200a 2020 2020  id.        .    
+00000120: 2020 2020 4765 7420 7468 6520 756e 6971      Get the uniq
+00000130: 7565 206d 6163 6869 6e65 2049 4420 6f66  ue machine ID of
+00000140: 2061 6e79 2068 6f73 7420 2877 6974 686f   any host (witho
+00000150: 7574 2061 646d 696e 2070 7269 7669 6c65  ut admin privile
+00000160: 6765 7329 2e0a 2020 2020 2020 2020 0a20  ges)..        . 
+00000170: 2020 2020 2020 2053 706f 6e73 6f72 6564         Sponsored
+00000180: 2062 793a 0a20 2020 2020 2020 200a 2020   by:.        .  
+00000190: 2020 2020 2020 3c61 2068 7265 663d 2268        <a href="h
+000001a0: 7474 7073 3a2f 2f6b 6579 6765 6e2e 7368  ttps://keygen.sh
+000001b0: 3f72 6566 3d74 7970 6564 5f70 6172 616d  ?ref=typed_param
+000001c0: 7322 3e0a 2020 2020 2020 2020 2020 3c64  s">.          <d
+000001d0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+000001e0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000001f0: 2f2f 6b65 7967 656e 2e73 682f 696d 6167  //keygen.sh/imag
+00000200: 6573 2f6c 6f67 6f2d 7069 6c6c 2e70 6e67  es/logo-pill.png
+00000210: 2220 7769 6474 683d 2232 3030 2220 616c  " width="200" al
+00000220: 743d 224b 6579 6765 6e22 3e0a 2020 2020  t="Keygen">.    
+00000230: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+00000240: 2020 2020 203c 2f61 3e0a 2020 2020 2020       </a>.      
+00000250: 2020 0a20 2020 2020 2020 205f 416e 206f    .        _An o
+00000260: 7065 6e2c 2073 6f75 7263 652d 6176 6169  pen, source-avai
+00000270: 6c61 626c 6520 736f 6674 7761 7265 206c  lable software l
+00000280: 6963 656e 7369 6e67 2061 6e64 2064 6973  icensing and dis
+00000290: 7472 6962 7574 696f 6e20 4150 492e 5f0a  tribution API._.
+000002a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000002b0: 2023 2320 496e 7374 616c 6c0a 2020 2020   ## Install.    
+000002c0: 2020 2020 0a20 2020 2020 2020 2049 6e73      .        Ins
+000002d0: 7461 6c6c 2075 7369 6e67 205b 6070 6970  tall using [`pip
+000002e0: 605d 2868 7474 7073 3a2f 2f64 6f63 732e  `](https://docs.
+000002f0: 7079 7468 6f6e 2e6f 7267 2f33 2f69 6e73  python.org/3/ins
+00000300: 7461 6c6c 696e 672f 696e 6465 782e 6874  talling/index.ht
+00000310: 6d6c 293a 0a20 2020 2020 2020 200a 2020  ml):.        .  
+00000320: 2020 2020 2020 6060 6062 6173 680a 2020        ```bash.  
+00000330: 2020 2020 2020 7079 7468 6f6e 3320 2d6d        python3 -m
+00000340: 2070 6970 2069 6e73 7461 6c6c 2070 792d   pip install py-
+00000350: 6d61 6368 696e 6569 640a 2020 2020 2020  machineid.      
+00000360: 2020 6060 600a 2020 2020 2020 2020 0a20    ```.        . 
+00000370: 2020 2020 2020 2023 2320 5573 6167 650a         ## Usage.
+00000380: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000390: 2054 6f20 6f62 7461 696e 2074 6865 2072   To obtain the r
+000003a0: 6177 2047 5549 4420 6f66 2074 6865 2064  aw GUID of the d
+000003b0: 6576 6963 652c 2075 7365 2060 6964 2829  evice, use `id()
+000003c0: 202d 3e20 7374 7260 3a0a 2020 2020 2020   -> str`:.      
+000003d0: 2020 0a20 2020 2020 2020 2060 6060 7079    .        ```py
+000003e0: 7468 6f6e 0a20 2020 2020 2020 2069 6d70  thon.        imp
+000003f0: 6f72 7420 6d61 6368 696e 6569 640a 2020  ort machineid.  
+00000400: 2020 2020 2020 0a20 2020 2020 2020 2070        .        p
+00000410: 7269 6e74 286d 6163 6869 6e65 6964 2e69  rint(machineid.i
+00000420: 6428 2929 0a20 2020 2020 2020 2060 6060  d()).        ```
+00000430: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000440: 2020 546f 206f 6274 6169 6e20 616e 2061    To obtain an a
+00000450: 6e6f 6e79 6d69 7a65 6420 2868 6173 6865  nonymized (hashe
+00000460: 6429 2076 6572 7369 6f6e 206f 6620 7468  d) version of th
+00000470: 6520 4755 4944 2c20 7365 6520 6265 6c6f  e GUID, see belo
+00000480: 772e 2054 6865 0a20 2020 2020 2020 2060  w. The.        `
+00000490: 6861 7368 6564 5f69 6428 7374 7229 202d  hashed_id(str) -
+000004a0: 3e20 7374 7260 2066 756e 6374 696f 6e20  > str` function 
+000004b0: 7461 6b65 7320 616e 206f 7074 696f 6e61  takes an optiona
+000004c0: 6c20 6170 706c 6963 6174 696f 6e20 4944  l application ID
+000004d0: 2c0a 2020 2020 2020 2020 7768 6963 6820  ,.        which 
+000004e0: 7769 6c6c 2065 6e73 7572 6520 6120 756e  will ensure a un
+000004f0: 6971 7565 2049 4420 7065 722d 6170 7020  ique ID per-app 
+00000500: 666f 7220 7468 6520 7361 6d65 2064 6576  for the same dev
+00000510: 6963 652e 0a20 2020 2020 2020 200a 2020  ice..        .  
+00000520: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
+00000530: 2020 2020 2020 2020 696d 706f 7274 206d          import m
+00000540: 6163 6869 6e65 6964 0a20 2020 2020 2020  achineid.       
+00000550: 200a 2020 2020 2020 2020 7072 696e 7428   .        print(
+00000560: 6d61 6368 696e 6569 642e 6861 7368 6564  machineid.hashed
+00000570: 5f69 6428 276d 7961 7070 6964 2729 290a  _id('myappid')).
+00000580: 2020 2020 2020 2020 7072 696e 7428 6d61          print(ma
+00000590: 6368 696e 6569 642e 6861 7368 6564 5f69  chineid.hashed_i
+000005a0: 6428 2929 0a20 2020 2020 2020 2060 6060  d()).        ```
+000005b0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000005c0: 2020 2323 2054 6861 6e6b 730a 2020 2020    ## Thanks.    
+000005d0: 2020 2020 0a20 2020 2020 2020 2053 7065      .        Spe
+000005e0: 6369 616c 2074 6861 6e6b 7320 746f 2044  cial thanks to D
+000005f0: 656e 6973 2042 726f 6462 6563 6b20 666f  enis Brodbeck fo
+00000600: 7220 6869 7320 476f 2070 6163 6b61 6765  r his Go package
+00000610: 2c20 5b60 6d61 6368 696e 6569 6460 5d28  , [`machineid`](
+00000620: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000630: 6f6d 2f64 656e 6973 6272 6f64 6265 636b  om/denisbrodbeck
+00000640: 2f6d 6163 6869 6e65 6964 292e 0a20 2020  /machineid)..   
+00000650: 2020 2020 200a 506c 6174 666f 726d 3a20       .Platform: 
+00000660: 554e 4b4e 4f57 4e0a 436c 6173 7369 6669  UNKNOWN.Classifi
+00000670: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000680: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000690: 6f6e 203a 3a20 330a 436c 6173 7369 6669  on :: 3.Classifi
+000006a0: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
+000006b0: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+000006c0: 4954 204c 6963 656e 7365 0a43 6c61 7373  IT License.Class
+000006d0: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
+000006e0: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+000006f0: 6465 7065 6e64 656e 740a 4465 7363 7269  dependent.Descri
+00000700: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
+00000710: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
+00000720: 6e0a                                     n.
```

### Comparing `py-machineid-0.3.0/setup.py` & `py-machineid-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
   readme = fh.read()
 
 setup(
   name='py-machineid',
-  version='0.3.0',
+  version='0.4.0',
   description='Get the unique machine ID of any host (without admin privileges)',
   long_description_content_type='text/markdown',
   long_description=readme,
   url='https://github.com/keygen-sh/py-machineid',
   author='Zeke Gabrielse',
   author_email='oss@keygen.sh',
   license='MIT',
```

