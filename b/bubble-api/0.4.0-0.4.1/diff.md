# Comparing `tmp/bubble_api-0.4.0.tar.gz` & `tmp/bubble_api-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bubble_api-0.4.0.tar", last modified: Thu Jun 22 10:25:13 2023, max compression
+gzip compressed data, was "bubble_api-0.4.1.tar", last modified: Mon Jul  3 14:20:33 2023, max compression
```

## Comparing `bubble_api-0.4.0.tar` & `bubble_api-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 10:25:13.530379 bubble_api-0.4.0/
--rw-rw-rw-   0        0        0     1105 2023-06-22 10:19:29.000000 bubble_api-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     3422 2023-06-22 10:25:13.530379 bubble_api-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2575 2023-06-22 10:19:29.000000 bubble_api-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 10:25:13.505137 bubble_api-0.4.0/bubble_api/
--rw-rw-rw-   0        0        0       98 2023-06-22 10:19:29.000000 bubble_api-0.4.0/bubble_api/__init__.py
--rw-rw-rw-   0        0        0     1230 2023-06-22 10:19:29.000000 bubble_api-0.4.0/bubble_api/constraint.py
--rw-rw-rw-   0        0        0     2438 2023-06-22 10:19:29.000000 bubble_api-0.4.0/bubble_api/field.py
--rw-rw-rw-   0        0        0     9600 2023-06-22 10:19:29.000000 bubble_api-0.4.0/bubble_api/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 10:25:13.517645 bubble_api-0.4.0/bubble_api.egg-info/
--rw-rw-rw-   0        0        0     3422 2023-06-22 10:25:13.000000 bubble_api-0.4.0/bubble_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-06-22 10:25:13.000000 bubble_api-0.4.0/bubble_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 10:25:13.000000 bubble_api-0.4.0/bubble_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 10:25:13.000000 bubble_api-0.4.0/bubble_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-22 10:25:13.000000 bubble_api-0.4.0/bubble_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1015 2023-06-22 10:19:29.000000 bubble_api-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-06-22 10:25:13.530379 bubble_api-0.4.0/setup.cfg
+drwxrwxr-x   0 settorac  (1000) settorac  (1000)        0 2023-07-03 14:20:33.037136 bubble_api-0.4.1/
+-rw-rw-r--   0 settorac  (1000) settorac  (1000)     1084 2023-07-03 11:50:55.000000 bubble_api-0.4.1/LICENSE
+-rw-rw-r--   0 settorac  (1000) settorac  (1000)     3706 2023-07-03 14:20:33.037136 bubble_api-0.4.1/PKG-INFO
+-rw-rw-r--   0 settorac  (1000) settorac  (1000)     2878 2023-07-03 14:14:27.000000 bubble_api-0.4.1/README.md
+drwxrwxr-x   0 settorac  (1000) settorac  (1000)        0 2023-07-03 14:20:33.033136 bubble_api-0.4.1/bubble_api/
+-rw-rw-r--   0 settorac  (1000) settorac  (1000)       93 2023-07-03 14:14:27.000000 bubble_api-0.4.1/bubble_api/__init__.py
+-rw-rw-r--   0 settorac  (1000) settorac  (1000)     9475 2023-07-03 14:14:27.000000 bubble_api-0.4.1/bubble_api/client.py
+-rw-rw-r--   0 settorac  (1000) settorac  (1000)     1191 2023-07-03 11:50:55.000000 bubble_api-0.4.1/bubble_api/constraint.py
+-rw-rw-r--   0 settorac  (1000) settorac  (1000)     2327 2023-07-03 11:50:55.000000 bubble_api-0.4.1/bubble_api/field.py
+drwxrwxr-x   0 settorac  (1000) settorac  (1000)        0 2023-07-03 14:20:33.037136 bubble_api-0.4.1/bubble_api.egg-info/
+-rw-rw-r--   0 settorac  (1000) settorac  (1000)     3706 2023-07-03 14:20:33.000000 bubble_api-0.4.1/bubble_api.egg-info/PKG-INFO
+-rw-rw-r--   0 settorac  (1000) settorac  (1000)      300 2023-07-03 14:20:33.000000 bubble_api-0.4.1/bubble_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 settorac  (1000) settorac  (1000)        1 2023-07-03 14:20:33.000000 bubble_api-0.4.1/bubble_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 settorac  (1000) settorac  (1000)        9 2023-07-03 14:20:33.000000 bubble_api-0.4.1/bubble_api.egg-info/requires.txt
+-rw-rw-r--   0 settorac  (1000) settorac  (1000)       11 2023-07-03 14:20:33.000000 bubble_api-0.4.1/bubble_api.egg-info/top_level.txt
+-rw-rw-r--   0 settorac  (1000) settorac  (1000)      980 2023-07-03 14:14:27.000000 bubble_api-0.4.1/pyproject.toml
+-rw-rw-r--   0 settorac  (1000) settorac  (1000)       92 2023-07-03 14:20:33.037136 bubble_api-0.4.1/setup.cfg
```

### Comparing `bubble_api-0.4.0/LICENSE` & `bubble_api-0.4.1/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Dylan Nina & Mathis Bourdin
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Dylan Nina & Mathis Bourdin
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `bubble_api-0.4.0/PKG-INFO` & `bubble_api-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,214 +1,232 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2062 7562  : 2.1..Name: bub
-00000020: 626c 655f 6170 690d 0a56 6572 7369 6f6e  ble_api..Version
-00000030: 3a20 302e 342e 300d 0a53 756d 6d61 7279  : 0.4.0..Summary
-00000040: 3a20 496e 7465 7261 6374 696f 6e73 2077  : Interactions w
-00000050: 6974 6820 4275 6262 6c65 2e69 6f20 4150  ith Bubble.io AP
-00000060: 4920 696e 2050 7974 686f 6e20 6d61 6465  I in Python made
-00000070: 2065 6173 7920 210d 0a41 7574 686f 722d   easy !..Author-
-00000080: 656d 6169 6c3a 2044 796c 616e 204e 494e  email: Dylan NIN
-00000090: 4120 3c73 6574 746f 7261 632e 6e69 6e61  A <settorac.nina
-000000a0: 4067 6d61 696c 2e63 6f6d 3e2c 204d 6174  @gmail.com>, Mat
-000000b0: 6869 7320 426f 7572 6469 6e20 3c6d 6174  his Bourdin <mat
-000000c0: 6869 7362 7264 6e40 676d 6169 6c2e 636f  hisbrdn@gmail.co
-000000d0: 6d3e 0d0a 5072 6f6a 6563 742d 5552 4c3a  m>..Project-URL:
-000000e0: 2048 6f6d 6570 6167 652c 2068 7474 7073   Homepage, https
-000000f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
-00000100: 7474 6f72 6163 2d6e 696e 612f 6275 6262  ttorac-nina/bubb
-00000110: 6c65 2d61 7069 0d0a 5072 6f6a 6563 742d  le-api..Project-
-00000120: 5552 4c3a 2042 7567 2054 7261 636b 6572  URL: Bug Tracker
-00000130: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-00000140: 2e63 6f6d 2f73 6574 746f 7261 632d 6e69  .com/settorac-ni
-00000150: 6e61 2f62 7562 626c 652d 6170 692f 6973  na/bubble-api/is
-00000160: 7375 6573 0d0a 436c 6173 7369 6669 6572  sues..Classifier
-00000170: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000180: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000190: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
-000001a0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001b0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001c0: 330d 0a43 6c61 7373 6966 6965 723a 2050  3..Classifier: P
-000001d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000001e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000001f0: 2033 2e38 0d0a 436c 6173 7369 6669 6572   3.8..Classifier
-00000200: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000210: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000220: 203a 3a20 332e 390d 0a43 6c61 7373 6966   :: 3.9..Classif
-00000230: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000240: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000250: 686f 6e20 3a3a 2033 2e31 300d 0a43 6c61  hon :: 3.10..Cla
-00000260: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000270: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000280: 2050 7974 686f 6e20 3a3a 2033 2e31 310d   Python :: 3.11.
-00000290: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
-000002a0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-000002b0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-000002c0: 6e73 650d 0a43 6c61 7373 6966 6965 723a  nse..Classifier:
-000002d0: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-000002e0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-000002f0: 656e 740d 0a52 6571 7569 7265 732d 5079  ent..Requires-Py
-00000300: 7468 6f6e 3a20 3e3d 332e 380d 0a44 6573  thon: >=3.8..Des
-00000310: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-00000320: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00000330: 646f 776e 0d0a 4c69 6365 6e73 652d 4669  down..License-Fi
-00000340: 6c65 3a20 4c49 4345 4e53 450d 0a0d 0a3c  le: LICENSE....<
-00000350: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-00000360: 7222 3e0d 0a20 2020 203c 6831 3e3c 636f  r">..    <h1><co
-00000370: 6465 3e42 7562 626c 6520 4170 693c 2f63  de>Bubble Api</c
-00000380: 6f64 653e 3c2f 6831 3e0d 0a20 2020 203c  ode></h1>..    <
-00000390: 703e 3c73 7472 6f6e 673e 496e 7465 7261  p><strong>Intera
-000003a0: 6374 696f 6e73 2077 6974 6820 4275 6262  ctions with Bubb
-000003b0: 6c65 2e69 6f20 4150 4920 696e 2050 7974  le.io API in Pyt
-000003c0: 686f 6e20 6d61 6465 2065 6173 7920 213c  hon made easy !<
-000003d0: 2f73 7472 6f6e 673e 3c2f 703e 0d0a 2020  /strong></p>..  
-000003e0: 2020 3c69 6d67 2061 6c74 3d22 5079 7468    <img alt="Pyth
-000003f0: 6f6e 2042 6164 6765 2220 7372 633d 2268  on Badge" src="h
-00000400: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000410: 6473 2e69 6f2f 6261 6467 652f 2d50 7974  ds.io/badge/-Pyt
-00000420: 686f 6e2d 4436 4436 4436 3f6c 6f67 6f3d  hon-D6D6D6?logo=
-00000430: 7079 7468 6f6e 222f 3e0d 0a20 2020 203c  python"/>..    <
-00000440: 696d 6720 616c 743d 2250 6950 5920 4261  img alt="PiPY Ba
-00000450: 6467 6522 2073 7263 3d22 6874 7470 733a  dge" src="https:
-00000460: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000470: 2f70 7970 692f 762f 6275 6262 6c65 2d61  /pypi/v/bubble-a
-00000480: 7069 222f 3e0d 0a20 2020 203c 696d 6720  pi"/>..    <img 
-00000490: 616c 743d 2243 692f 4344 2042 6164 6765  alt="Ci/CD Badge
-000004a0: 2220 7372 633d 2268 7474 7073 3a2f 2f67  " src="https://g
-000004b0: 6974 6875 622e 636f 6d2f 7365 7474 6f72  ithub.com/settor
-000004c0: 6163 2d6e 696e 612f 6275 6262 6c65 2d61  ac-nina/bubble-a
-000004d0: 7069 2f61 6374 696f 6e73 2f77 6f72 6b66  pi/actions/workf
-000004e0: 6c6f 7773 2f63 6963 642e 7961 6d6c 2f62  lows/cicd.yaml/b
-000004f0: 6164 6765 2e73 7667 3f62 7261 6e63 683d  adge.svg?branch=
-00000500: 6d61 696e 2922 2f3e 0d0a 2020 2020 3c69  main)"/>..    <i
-00000510: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000520: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000530: 6164 6765 2f4d 6164 6525 3230 5769 7468  adge/Made%20With
-00000540: 2d4c 6f76 652d 6566 3764 3136 2e73 7667  -Love-ef7d16.svg
-00000550: 222f 3e0d 0a3c 2f64 6976 3e0d 0a0d 0a2d  "/>..</div>....-
-00000560: 2d2d 0d0a 0d0a 2323 2049 6e73 7461 6c6c  --....## Install
-00000570: 696e 670d 0a0d 0a54 6865 2065 6173 6965  ing....The easie
-00000580: 7374 2077 6179 2074 6f20 696e 7374 616c  st way to instal
-00000590: 6c20 6974 2069 7320 7468 726f 7567 6820  l it is through 
-000005a0: 2a2a 7069 7079 2a2a 203a 0d0a 0d0a 6060  **pipy** :....``
-000005b0: 6073 6865 6c6c 0d0a 7069 7020 696e 7374  `shell..pip inst
-000005c0: 616c 6c20 6275 6262 6c65 2d61 7069 0d0a  all bubble-api..
-000005d0: 6060 600d 0a0d 0a23 2320 486f 7720 746f  ```....## How to
-000005e0: 2075 7365 2069 740d 0a0d 0a41 7420 7468   use it....At th
-000005f0: 6520 6d6f 6d65 6e74 2c20 7468 6572 6520  e moment, there 
-00000600: 6973 206e 6f20 646f 6375 6d65 6e74 6174  is no documentat
-00000610: 696f 6e20 666f 7220 7468 6973 206c 6962  ion for this lib
-00000620: 7261 7279 2e0d 0a59 6f75 2063 616e 2c20  rary...You can, 
-00000630: 686f 7765 7665 722c 2072 656c 7920 6f6e  however, rely on
-00000640: 2074 6865 2069 6e74 6567 7261 7469 6f6e   the integration
-00000650: 2074 6573 7473 2077 6520 7573 6520 746f   tests we use to
-00000660: 2065 6e73 7572 6520 7072 6f70 6572 2069   ensure proper i
-00000670: 6e74 6567 7261 7469 6f6e 2077 6974 6820  ntegration with 
-00000680: 4275 6262 6c65 2e0d 0a59 6f75 2063 616e  Bubble...You can
-00000690: 2066 696e 6420 7468 656d 205b 6865 7265   find them [here
-000006a0: 5d28 7465 7374 732f 696e 7465 6772 6174  ](tests/integrat
-000006b0: 696f 6e29 2e0d 0a0d 0a23 2323 2043 7265  ion).....### Cre
-000006c0: 6174 696e 6720 6120 4275 6262 6c65 5772  ating a BubbleWr
-000006d0: 6170 7065 7220 696e 7374 616e 6365 203a  apper instance :
-000006e0: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a66  ....```python..f
-000006f0: 726f 6d20 6275 6262 6c65 5f61 7069 2069  rom bubble_api i
-00000700: 6d70 6f72 7420 4275 6262 6c65 5772 6170  mport BubbleWrap
-00000710: 7065 720d 0a0d 0a62 7562 626c 655f 7772  per....bubble_wr
-00000720: 6170 7065 7220 3d20 4275 6262 6c65 5772  apper = BubbleWr
-00000730: 6170 7065 7228 0d0a 2020 2020 6261 7365  apper(..    base
-00000740: 5f75 726c 3d22 6874 7470 733a 2f2f 6375  _url="https://cu
-00000750: 7572 652e 636f 6d22 2c0d 0a20 2020 2061  ure.com",..    a
-00000760: 7069 5f74 6f6b 656e 3d22 594f 5552 5f41  pi_token="YOUR_A
-00000770: 5049 5f54 4f4b 454e 222c 0d0a 2020 2020  PI_TOKEN",..    
-00000780: 6275 6262 6c65 5f76 6572 7369 6f6e 3d22  bubble_version="
-00000790: 6c69 7665 220d 0a29 0d0a 6060 600d 0a0d  live"..)..```...
-000007a0: 0a23 2323 2049 6e74 6572 6163 7420 7769  .### Interact wi
-000007b0: 7468 2062 7562 626c 6520 6461 7461 203a  th bubble data :
-000007c0: 0d0a 0d0a 4672 6f6d 2074 6865 2060 4275  ....From the `Bu
-000007d0: 6262 6c65 5772 6170 7065 7260 2069 6e73  bbleWrapper` ins
-000007e0: 7461 6e63 6520 796f 7520 6361 6e20 6e6f  tance you can no
-000007f0: 7720 696e 7465 7261 6374 2077 6974 6820  w interact with 
-00000800: 7468 6520 6461 7461 2061 7069 2065 6173  the data api eas
-00000810: 696c 792e 0d0a 0d0a 6060 6070 7974 686f  ily.....```pytho
-00000820: 6e0d 0a6f 626a 6563 745f 6461 7461 203d  n..object_data =
-00000830: 2062 7562 626c 655f 7772 6170 7065 722e   bubble_wrapper.
-00000840: 6765 7428 0d0a 2020 2020 2274 6162 6c65  get(..    "table
-00000850: 5f6e 616d 6522 2c0d 0a20 2020 2062 7562  _name",..    bub
-00000860: 626c 655f 6964 3d22 6275 6262 6c65 5f6f  ble_id="bubble_o
-00000870: 626a 6563 745f 6964 222c 0d0a 290d 0a60  bject_id",..)..`
-00000880: 6060 0d0a 416e 6420 736f 206f 6e20 7769  ``..And so on wi
-00000890: 7468 2061 6c6c 2074 6865 2062 6173 6963  th all the basic
-000008a0: 2069 6e74 6572 6163 7469 6f6e 7320 7769   interactions wi
-000008b0: 7468 2074 6865 2061 7069 3a20 2a2a 6465  th the api: **de
-000008c0: 6c65 7465 2a2a 2c20 2a2a 7570 6461 7465  lete**, **update
-000008d0: 2a2a 2c20 2a2a 7265 706c 6163 652a 2a2c  **, **replace**,
-000008e0: 202e 2e2e 0d0a 0d0a 596f 7520 6361 6e20   .......You can 
-000008f0: 616c 736f 2075 7365 2063 6f6e 7374 7261  also use constra
-00000900: 696e 7473 2066 6f72 2067 6574 7469 6e67  ints for getting
-00000910: 206f 7220 6465 6c65 7469 6e67 206f 626a   or deleting obj
-00000920: 6563 7473 2e0d 0a54 6869 7320 6973 2064  ects...This is d
-00000930: 6f6e 6520 7468 726f 7567 6820 6120 6c69  one through a li
-00000940: 7374 206f 6620 6043 6f6e 7472 6169 6e74  st of `Contraint
-00000950: 6020 6f62 6a65 6374 2079 6f75 2063 616e  ` object you can
-00000960: 2064 6563 6c61 7265 2062 7920 6f70 6572   declare by oper
-00000970: 6174 696f 6e73 2077 6974 6820 7468 6520  ations with the 
-00000980: 6046 6965 6c64 6020 636c 6173 732e 0d0a  `Field` class...
-00000990: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
-000009a0: 6d20 6275 6262 6c65 5f61 7069 2069 6d70  m bubble_api imp
-000009b0: 6f72 7420 4275 6262 6c65 5772 6170 7065  ort BubbleWrappe
-000009c0: 722c 2046 6965 6c64 0d0a 6672 6f6d 2064  r, Field..from d
-000009d0: 6174 6574 696d 6520 696d 706f 7274 2064  atetime import d
-000009e0: 6174 6574 696d 650d 0a0d 0a62 7562 626c  atetime....bubbl
-000009f0: 655f 7772 6170 7065 7220 3d20 4275 6262  e_wrapper = Bubb
-00000a00: 6c65 5772 6170 7065 7228 202e 2e2e 2029  leWrapper( ... )
-00000a10: 0d0a 0d0a 636f 6e73 7472 6169 6e74 7320  ....constraints 
-00000a20: 3d20 5b0d 0a20 2020 2046 6965 6c64 2822  = [..    Field("
-00000a30: 6e61 6d65 2229 203d 3d20 2242 6f62 222c  name") == "Bob",
-00000a40: 0d0a 2020 2020 4669 656c 6428 2243 7265  ..    Field("Cre
-00000a50: 6174 6564 2229 203e 2064 6174 6574 696d  ated") > datetim
-00000a60: 6528 3230 3233 2c20 312c 2031 292c 0d0a  e(2023, 1, 1),..
-00000a70: 5d0d 0a0d 0a64 6174 6120 3d20 6275 6262  ]....data = bubb
-00000a80: 6c65 5f77 7261 7070 6572 2e67 6574 280d  le_wrapper.get(.
-00000a90: 0a20 2020 2022 7461 626c 655f 6e61 6d65  .    "table_name
-00000aa0: 222c 0d0a 2020 2020 636f 6e73 7472 6169  ",..    constrai
-00000ab0: 6e74 733d 636f 6e73 7472 6169 6e74 730d  nts=constraints.
-00000ac0: 0a29 0d0a 6060 600d 0a0d 0a41 6c6c 2074  .)..```....All t
-00000ad0: 6865 2066 6965 6c64 7320 6e61 6d65 7320  he fields names 
-00000ae0: 616e 6420 636f 6e73 7472 6169 6e74 7320  and constraints 
-00000af0: 7661 6c75 6573 2066 6f72 6d61 7474 696e  values formattin
-00000b00: 6720 6973 2068 616e 646c 6520 6279 2074  g is handle by t
-00000b10: 6865 206c 6962 7261 7279 2e0d 0a0d 0a23  he library.....#
-00000b20: 2320 496e 636f 6d69 6e67 2066 6561 7475  # Incoming featu
-00000b30: 7265 730d 0a0d 0a2d 205b 205d 2042 6967  res....- [ ] Big
-00000b40: 2072 6571 7565 7374 206f 7074 696d 697a   request optimiz
-00000b50: 6174 696f 6e20 7573 696e 6720 7265 6d61  ation using rema
-00000b60: 696e 696e 6720 6170 7072 6f78 696d 6174  ining approximat
-00000b70: 696f 6e20 2865 7863 6c75 6465 5f72 656d  ion (exclude_rem
-00000b80: 6169 6e69 6e67 290d 0a2d 205b 205d 204d  aining)..- [ ] M
-00000b90: 756c 7469 7468 7265 6164 696e 670d 0a2d  ultithreading..-
-00000ba0: 205b 205d 2044 6566 6175 6c74 2066 6965   [ ] Default fie
-00000bb0: 6c64 7320 284d 6f64 6966 6965 6420 4461  lds (Modified Da
-00000bc0: 7465 2c20 756e 6971 7565 2069 642c 2043  te, unique id, C
-00000bd0: 7265 6174 6564 2044 6174 652c 202e 2e2e  reated Date, ...
-00000be0: 290d 0a2d 205b 205d 204c 6966 6574 696d  )..- [ ] Lifetim
-00000bf0: 6520 6f62 6a65 6374 206d 616e 6167 656d  e object managem
-00000c00: 656e 7420 2875 7064 6174 652c 2072 6566  ent (update, ref
-00000c10: 7265 7368 2c20 7265 706c 6163 6529 0d0a  resh, replace)..
-00000c20: 2d20 5b20 5d20 446f 6375 6d65 6e74 6174  - [ ] Documentat
-00000c30: 696f 6e0d 0a0d 0a23 2320 4175 7468 6f72  ion....## Author
-00000c40: 730d 0a0d 0a2a 202a 2a44 796c 616e 204e  s....* **Dylan N
-00000c50: 696e 612a 2a20 2d20 2a49 6e69 7469 616c  ina** - *Initial
-00000c60: 2077 6f72 6b2a 202d 205b 7365 7474 6f72   work* - [settor
-00000c70: 6163 2d6e 696e 615d 2868 7474 7073 3a2f  ac-nina](https:/
-00000c80: 2f67 6974 6875 622e 636f 6d2f 7365 7474  /github.com/sett
-00000c90: 6f72 6163 2d6e 696e 6129 0d0a 2a20 2a2a  orac-nina)..* **
-00000ca0: 4d61 7468 6973 2042 6f75 7264 696e 2a2a  Mathis Bourdin**
-00000cb0: 202d 202a 436f 6e74 7269 6275 746f 722a   - *Contributor*
-00000cc0: 202d 205b 6d61 7468 6973 6272 646e 5d28   - [mathisbrdn](
-00000cd0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000ce0: 6f6d 2f6d 6174 6869 7362 7264 6e29 0d0a  om/mathisbrdn)..
-00000cf0: 0d0a 2323 204c 6963 656e 7365 0d0a 0d0a  ..## License....
-00000d00: 5468 6973 2070 726f 6a65 6374 2069 7320  This project is 
-00000d10: 6c69 6365 6e73 6564 2075 6e64 6572 2074  licensed under t
-00000d20: 6865 204d 4954 204c 6963 656e 7365 202d  he MIT License -
-00000d30: 2073 6565 2074 6865 205b 4c49 4345 4e53   see the [LICENS
-00000d40: 455d 284c 4943 454e 5345 2920 6669 6c65  E](LICENSE) file
-00000d50: 2066 6f72 2064 6574 6169 6c73 0d0a        for details..
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6275 6262  : 2.1.Name: bubb
+00000020: 6c65 5f61 7069 0a56 6572 7369 6f6e 3a20  le_api.Version: 
+00000030: 302e 342e 310a 5375 6d6d 6172 793a 2049  0.4.1.Summary: I
+00000040: 6e74 6572 6163 7469 6f6e 7320 7769 7468  nteractions with
+00000050: 2042 7562 626c 652e 696f 2041 5049 2069   Bubble.io API i
+00000060: 6e20 5079 7468 6f6e 206d 6164 6520 6561  n Python made ea
+00000070: 7379 2021 0a41 7574 686f 722d 656d 6169  sy !.Author-emai
+00000080: 6c3a 2044 796c 616e 204e 494e 4120 3c73  l: Dylan NINA <s
+00000090: 6574 746f 7261 632e 6e69 6e61 4067 6d61  ettorac.nina@gma
+000000a0: 696c 2e63 6f6d 3e2c 204d 6174 6869 7320  il.com>, Mathis 
+000000b0: 426f 7572 6469 6e20 3c6d 6174 6869 7362  Bourdin <mathisb
+000000c0: 7264 6e40 676d 6169 6c2e 636f 6d3e 0a50  rdn@gmail.com>.P
+000000d0: 726f 6a65 6374 2d55 524c 3a20 486f 6d65  roject-URL: Home
+000000e0: 7061 6765 2c20 6874 7470 733a 2f2f 6769  page, https://gi
+000000f0: 7468 7562 2e63 6f6d 2f73 6574 746f 7261  thub.com/settora
+00000100: 632d 6e69 6e61 2f62 7562 626c 652d 6170  c-nina/bubble-ap
+00000110: 690a 5072 6f6a 6563 742d 5552 4c3a 2042  i.Project-URL: B
+00000120: 7567 2054 7261 636b 6572 2c20 6874 7470  ug Tracker, http
+00000130: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000140: 6574 746f 7261 632d 6e69 6e61 2f62 7562  ettorac-nina/bub
+00000150: 626c 652d 6170 692f 6973 7375 6573 0a43  ble-api/issues.C
+00000160: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000170: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000180: 3a3a 2050 7974 686f 6e0a 436c 6173 7369  :: Python.Classi
+00000190: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000001a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001b0: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
+000001c0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000001d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001e0: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
+000001f0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000200: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000210: 5079 7468 6f6e 203a 3a20 332e 390a 436c  Python :: 3.9.Cl
+00000220: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000230: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000240: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000250: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000260: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000270: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000280: 2e31 310a 436c 6173 7369 6669 6572 3a20  .11.Classifier: 
+00000290: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+000002a0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+000002b0: 6963 656e 7365 0a43 6c61 7373 6966 6965  icense.Classifie
+000002c0: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+000002d0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000002e0: 6e64 656e 740a 5265 7175 6972 6573 2d50  ndent.Requires-P
+000002f0: 7974 686f 6e3a 203e 3d33 2e38 0a44 6573  ython: >=3.8.Des
+00000300: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00000310: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00000320: 646f 776e 0a4c 6963 656e 7365 2d46 696c  down.License-Fil
+00000330: 653a 204c 4943 454e 5345 0a0a 3c64 6976  e: LICENSE..<div
+00000340: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000350: 0a20 2020 203c 6831 3e3c 636f 6465 3e42  .    <h1><code>B
+00000360: 7562 626c 6520 4170 693c 2f63 6f64 653e  ubble Api</code>
+00000370: 3c2f 6831 3e0a 2020 2020 3c70 3e3c 7374  </h1>.    <p><st
+00000380: 726f 6e67 3e49 6e74 6572 6163 7469 6f6e  rong>Interaction
+00000390: 7320 7769 7468 2042 7562 626c 652e 696f  s with Bubble.io
+000003a0: 2041 5049 2069 6e20 5079 7468 6f6e 206d   API in Python m
+000003b0: 6164 6520 6561 7379 2021 3c2f 7374 726f  ade easy !</stro
+000003c0: 6e67 3e3c 2f70 3e0a 2020 2020 3c69 6d67  ng></p>.    <img
+000003d0: 2061 6c74 3d22 5079 7468 6f6e 2042 6164   alt="Python Bad
+000003e0: 6765 2220 7372 633d 2268 7474 7073 3a2f  ge" src="https:/
+000003f0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000400: 6261 6467 652f 2d50 7974 686f 6e2d 4436  badge/-Python-D6
+00000410: 4436 4436 3f6c 6f67 6f3d 7079 7468 6f6e  D6D6?logo=python
+00000420: 222f 3e0a 2020 2020 3c69 6d67 2061 6c74  "/>.    <img alt
+00000430: 3d22 5069 5059 2042 6164 6765 2220 7372  ="PiPY Badge" sr
+00000440: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000450: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+00000460: 2f62 7562 626c 652d 6170 6922 2f3e 0a20  /bubble-api"/>. 
+00000470: 2020 203c 696d 6720 616c 743d 2243 492f     <img alt="CI/
+00000480: 4344 2042 6164 6765 2220 7372 633d 2268  CD Badge" src="h
+00000490: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000004a0: 6d2f 7365 7474 6f72 6163 2d6e 696e 612f  m/settorac-nina/
+000004b0: 6275 6262 6c65 2d61 7069 2f61 6374 696f  bubble-api/actio
+000004c0: 6e73 2f77 6f72 6b66 6c6f 7773 2f63 6963  ns/workflows/cic
+000004d0: 642e 7961 6d6c 2f62 6164 6765 2e73 7667  d.yaml/badge.svg
+000004e0: 3f62 7261 6e63 683d 6d61 696e 2922 2f3e  ?branch=main)"/>
+000004f0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+00000500: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000510: 6473 2e69 6f2f 6261 6467 652f 4d61 6465  ds.io/badge/Made
+00000520: 2532 3057 6974 682d 4c6f 7665 2d65 6637  %20With-Love-ef7
+00000530: 6431 362e 7376 6722 2f3e 0a20 2020 203c  d16.svg"/>.    <
+00000540: 703e 0a20 2020 2020 2020 203c 6120 6872  p>.        <a hr
+00000550: 6566 3d22 6874 7470 733a 2f2f 6375 7572  ef="https://cuur
+00000560: 652e 636f 6d3f 7574 6d5f 736f 7572 6365  e.com?utm_source
+00000570: 3d67 6974 6875 6226 7574 6d5f 6d65 6469  =github&utm_medi
+00000580: 756d 3d72 6566 6572 7261 6c22 3e0a 2020  um=referral">.  
+00000590: 2020 2020 2020 2020 2020 506f 7765 7265            Powere
+000005a0: 6420 6279 203c 7374 726f 6e67 3e43 7575  d by <strong>Cuu
+000005b0: 7265 3c2f 7374 726f 6e67 3e0a 2020 2020  re</strong>.    
+000005c0: 2020 2020 3c2f 613e 0a20 2020 2020 2020      </a>.       
+000005d0: 2026 6e62 7370 3b26 6e62 7370 3b0a 2020   &nbsp;&nbsp;.  
+000005e0: 2020 2020 2020 3c61 2068 7265 663d 2268        <a href="h
+000005f0: 7474 7073 3a2f 2f63 7575 7265 2e63 6f6d  ttps://cuure.com
+00000600: 3f75 746d 5f73 6f75 7263 653d 6769 7468  ?utm_source=gith
+00000610: 7562 2675 746d 5f6d 6564 6975 6d3d 7265  ub&utm_medium=re
+00000620: 6665 7272 616c 223e 0a20 2020 2020 2020  ferral">.       
+00000630: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
+00000640: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000650: 6d2f 7365 7474 6f72 6163 2d6e 696e 612f  m/settorac-nina/
+00000660: 6275 6262 6c65 2d61 7069 2f62 6c6f 622f  bubble-api/blob/
+00000670: 6d61 696e 2f61 7373 6574 732f 6375 7572  main/assets/cuur
+00000680: 655f 6c6f 676f 2e67 6966 2220 7769 6474  e_logo.gif" widt
+00000690: 683d 2236 3022 2068 6569 6768 743d 2236  h="60" height="6
+000006a0: 3022 2061 6c69 676e 3d22 6365 6e74 6572  0" align="center
+000006b0: 222f 3e0a 2020 2020 2020 2020 3c2f 613e  "/>.        </a>
+000006c0: 0a20 2020 203c 2f70 3e0a 3c2f 6469 763e  .    </p>.</div>
+000006d0: 0a0a 2d2d 2d0a 0a23 2320 496e 7374 616c  ..---..## Instal
+000006e0: 6c69 6e67 0a0a 5468 6520 6561 7369 6573  ling..The easies
+000006f0: 7420 7761 7920 746f 2069 6e73 7461 6c6c  t way to install
+00000700: 2069 7420 6973 2074 6872 6f75 6768 202a   it is through *
+00000710: 2a70 6970 792a 2a20 3a0a 0a60 6060 7368  *pipy** :..```sh
+00000720: 656c 6c0a 7069 7020 696e 7374 616c 6c20  ell.pip install 
+00000730: 6275 6262 6c65 2d61 7069 0a60 6060 0a0a  bubble-api.```..
+00000740: 2323 2048 6f77 2074 6f20 7573 6520 6974  ## How to use it
+00000750: 0a0a 4174 2074 6865 206d 6f6d 656e 742c  ..At the moment,
+00000760: 2074 6865 7265 2069 7320 6e6f 2064 6f63   there is no doc
+00000770: 756d 656e 7461 7469 6f6e 2066 6f72 2074  umentation for t
+00000780: 6869 7320 6c69 6272 6172 792e 0a59 6f75  his library..You
+00000790: 2063 616e 2c20 686f 7765 7665 722c 2072   can, however, r
+000007a0: 656c 7920 6f6e 2074 6865 2069 6e74 6567  ely on the integ
+000007b0: 7261 7469 6f6e 2074 6573 7473 2077 6520  ration tests we 
+000007c0: 7573 6520 746f 2065 6e73 7572 6520 7072  use to ensure pr
+000007d0: 6f70 6572 2069 6e74 6567 7261 7469 6f6e  oper integration
+000007e0: 2077 6974 6820 4275 6262 6c65 2e0a 596f   with Bubble..Yo
+000007f0: 7520 6361 6e20 6669 6e64 2074 6865 6d20  u can find them 
+00000800: 5b68 6572 655d 2874 6573 7473 2f69 6e74  [here](tests/int
+00000810: 6567 7261 7469 6f6e 292e 0a0a 2323 2320  egration)...### 
+00000820: 4372 6561 7469 6e67 2061 2042 7562 626c  Creating a Bubbl
+00000830: 6543 6c69 656e 7420 696e 7374 616e 6365  eClient instance
+00000840: 203a 0a0a 6060 6070 7974 686f 6e0a 6672   :..```python.fr
+00000850: 6f6d 2062 7562 626c 655f 6170 6920 696d  om bubble_api im
+00000860: 706f 7274 2042 7562 626c 6543 6c69 656e  port BubbleClien
+00000870: 740a 0a62 7562 626c 655f 636c 6965 6e74  t..bubble_client
+00000880: 203d 2042 7562 626c 6543 6c69 656e 7428   = BubbleClient(
+00000890: 0a20 2020 2062 6173 655f 7572 6c3d 2268  .    base_url="h
+000008a0: 7474 7073 3a2f 2f63 7575 7265 2e63 6f6d  ttps://cuure.com
+000008b0: 222c 0a20 2020 2061 7069 5f74 6f6b 656e  ",.    api_token
+000008c0: 3d22 594f 5552 5f41 5049 5f54 4f4b 454e  ="YOUR_API_TOKEN
+000008d0: 222c 0a20 2020 2062 7562 626c 655f 7665  ",.    bubble_ve
+000008e0: 7273 696f 6e3d 226c 6976 6522 0a29 0a60  rsion="live".).`
+000008f0: 6060 0a0a 2323 2320 496e 7465 7261 6374  ``..### Interact
+00000900: 2077 6974 6820 6275 6262 6c65 2064 6174   with bubble dat
+00000910: 6120 3a0a 0a46 726f 6d20 7468 6520 6042  a :..From the `B
+00000920: 7562 626c 6543 6c69 656e 7460 2069 6e73  ubbleClient` ins
+00000930: 7461 6e63 6520 796f 7520 6361 6e20 6e6f  tance you can no
+00000940: 7720 696e 7465 7261 6374 2077 6974 6820  w interact with 
+00000950: 7468 6520 6461 7461 2061 7069 2065 6173  the data api eas
+00000960: 696c 792e 0a0a 6060 6070 7974 686f 6e0a  ily...```python.
+00000970: 6f62 6a65 6374 5f64 6174 6120 3d20 6275  object_data = bu
+00000980: 6262 6c65 5f63 6c69 656e 742e 6765 7428  bble_client.get(
+00000990: 0a20 2020 2022 7461 626c 655f 6e61 6d65  .    "table_name
+000009a0: 222c 0a20 2020 2062 7562 626c 655f 6964  ",.    bubble_id
+000009b0: 3d22 6275 6262 6c65 5f6f 626a 6563 745f  ="bubble_object_
+000009c0: 6964 222c 0a29 0a60 6060 0a0a 416e 6420  id",.).```..And 
+000009d0: 736f 206f 6e20 7769 7468 2061 6c6c 2074  so on with all t
+000009e0: 6865 2062 6173 6963 2069 6e74 6572 6163  he basic interac
+000009f0: 7469 6f6e 7320 7769 7468 2074 6865 2061  tions with the a
+00000a00: 7069 3a20 2a2a 6465 6c65 7465 2a2a 2c20  pi: **delete**, 
+00000a10: 2a2a 7570 6461 7465 2a2a 2c20 2a2a 7265  **update**, **re
+00000a20: 706c 6163 652a 2a2c 202e 2e2e 0a0a 596f  place**, .....Yo
+00000a30: 7520 6361 6e20 616c 736f 2075 7365 2063  u can also use c
+00000a40: 6f6e 7374 7261 696e 7473 2066 6f72 2067  onstraints for g
+00000a50: 6574 7469 6e67 206f 7220 6465 6c65 7469  etting or deleti
+00000a60: 6e67 206f 626a 6563 7473 2e0a 5468 6973  ng objects..This
+00000a70: 2069 7320 646f 6e65 2074 6872 6f75 6768   is done through
+00000a80: 2061 206c 6973 7420 6f66 2060 436f 6e74   a list of `Cont
+00000a90: 7261 696e 7460 206f 626a 6563 7420 796f  raint` object yo
+00000aa0: 7520 6361 6e20 6465 636c 6172 6520 6279  u can declare by
+00000ab0: 206f 7065 7261 7469 6f6e 7320 7769 7468   operations with
+00000ac0: 2074 6865 2060 4669 656c 6460 2063 6c61   the `Field` cla
+00000ad0: 7373 2e0a 0a60 6060 7079 7468 6f6e 0a66  ss...```python.f
+00000ae0: 726f 6d20 6275 6262 6c65 5f61 7069 2069  rom bubble_api i
+00000af0: 6d70 6f72 7420 4275 6262 6c65 436c 6965  mport BubbleClie
+00000b00: 6e74 2c20 4669 656c 640a 6672 6f6d 2064  nt, Field.from d
+00000b10: 6174 6574 696d 6520 696d 706f 7274 2064  atetime import d
+00000b20: 6174 6574 696d 650a 0a62 7562 626c 655f  atetime..bubble_
+00000b30: 636c 6965 6e74 203d 2042 7562 626c 6543  client = BubbleC
+00000b40: 6c69 656e 7428 202e 2e2e 2029 0a0a 636f  lient( ... )..co
+00000b50: 6e73 7472 6169 6e74 7320 3d20 5b0a 2020  nstraints = [.  
+00000b60: 2020 4669 656c 6428 226e 616d 6522 2920    Field("name") 
+00000b70: 3d3d 2022 426f 6222 2c0a 2020 2020 4669  == "Bob",.    Fi
+00000b80: 656c 6428 2243 7265 6174 6564 2229 203e  eld("Created") >
+00000b90: 2064 6174 6574 696d 6528 3230 3233 2c20   datetime(2023, 
+00000ba0: 312c 2031 292c 0a5d 0a0a 6461 7461 203d  1, 1),.]..data =
+00000bb0: 2062 7562 626c 655f 636c 6965 6e74 2e67   bubble_client.g
+00000bc0: 6574 280a 2020 2020 2274 6162 6c65 5f6e  et(.    "table_n
+00000bd0: 616d 6522 2c0a 2020 2020 636f 6e73 7472  ame",.    constr
+00000be0: 6169 6e74 733d 636f 6e73 7472 6169 6e74  aints=constraint
+00000bf0: 730a 290a 6060 600a 0a41 6c6c 2074 6865  s.).```..All the
+00000c00: 2066 6965 6c64 7320 6e61 6d65 7320 616e   fields names an
+00000c10: 6420 636f 6e73 7472 6169 6e74 7320 7661  d constraints va
+00000c20: 6c75 6573 2066 6f72 6d61 7474 696e 6720  lues formatting 
+00000c30: 6973 2068 616e 646c 6520 6279 2074 6865  is handle by the
+00000c40: 206c 6962 7261 7279 2e0a 0a23 2320 496e   library...## In
+00000c50: 636f 6d69 6e67 2066 6561 7475 7265 730a  coming features.
+00000c60: 0a2d 205b 205d 2042 6967 2072 6571 7565  .- [ ] Big reque
+00000c70: 7374 206f 7074 696d 697a 6174 696f 6e20  st optimization 
+00000c80: 7573 696e 6720 7265 6d61 696e 696e 6720  using remaining 
+00000c90: 6170 7072 6f78 696d 6174 696f 6e20 2865  approximation (e
+00000ca0: 7863 6c75 6465 5f72 656d 6169 6e69 6e67  xclude_remaining
+00000cb0: 290a 2d20 5b20 5d20 4d75 6c74 6974 6872  ).- [ ] Multithr
+00000cc0: 6561 6469 6e67 0a2d 205b 205d 2044 6566  eading.- [ ] Def
+00000cd0: 6175 6c74 2066 6965 6c64 7320 284d 6f64  ault fields (Mod
+00000ce0: 6966 6965 6420 4461 7465 2c20 756e 6971  ified Date, uniq
+00000cf0: 7565 2069 642c 2043 7265 6174 6564 2044  ue id, Created D
+00000d00: 6174 652c 202e 2e2e 290a 2d20 5b20 5d20  ate, ...).- [ ] 
+00000d10: 4c69 6665 7469 6d65 206f 626a 6563 7420  Lifetime object 
+00000d20: 6d61 6e61 6765 6d65 6e74 2028 7570 6461  management (upda
+00000d30: 7465 2c20 7265 6672 6573 682c 2072 6570  te, refresh, rep
+00000d40: 6c61 6365 290a 2d20 5b20 5d20 446f 6375  lace).- [ ] Docu
+00000d50: 6d65 6e74 6174 696f 6e0a 0a23 2320 4175  mentation..## Au
+00000d60: 7468 6f72 730a 0a2a 202a 2a44 796c 616e  thors..* **Dylan
+00000d70: 204e 696e 612a 2a20 2d20 2a49 6e69 7469   Nina** - *Initi
+00000d80: 616c 2077 6f72 6b2a 202d 205b 7365 7474  al work* - [sett
+00000d90: 6f72 6163 2d6e 696e 615d 2868 7474 7073  orac-nina](https
+00000da0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
+00000db0: 7474 6f72 6163 2d6e 696e 6129 0a2a 202a  ttorac-nina).* *
+00000dc0: 2a4d 6174 6869 7320 426f 7572 6469 6e2a  *Mathis Bourdin*
+00000dd0: 2a20 2d20 2a43 6f6e 7472 6962 7574 6f72  * - *Contributor
+00000de0: 2a20 2d20 5b6d 6174 6869 7362 7264 6e5d  * - [mathisbrdn]
+00000df0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000e00: 636f 6d2f 6d61 7468 6973 6272 646e 290a  com/mathisbrdn).
+00000e10: 0a23 2320 4c69 6365 6e73 650a 0a54 6869  .## License..Thi
+00000e20: 7320 7072 6f6a 6563 7420 6973 206c 6963  s project is lic
+00000e30: 656e 7365 6420 756e 6465 7220 7468 6520  ensed under the 
+00000e40: 4d49 5420 4c69 6365 6e73 6520 2d20 7365  MIT License - se
+00000e50: 6520 7468 6520 5b4c 4943 454e 5345 5d28  e the [LICENSE](
+00000e60: 4c49 4345 4e53 4529 2066 696c 6520 666f  LICENSE) file fo
+00000e70: 7220 6465 7461 696c 730a                 r details.
```

### Comparing `bubble_api-0.4.0/README.md` & `bubble_api-0.4.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,161 +1,180 @@
 00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
-00000010: 6572 223e 0d0a 2020 2020 3c68 313e 3c63  er">..    <h1><c
-00000020: 6f64 653e 4275 6262 6c65 2041 7069 3c2f  ode>Bubble Api</
-00000030: 636f 6465 3e3c 2f68 313e 0d0a 2020 2020  code></h1>..    
-00000040: 3c70 3e3c 7374 726f 6e67 3e49 6e74 6572  <p><strong>Inter
-00000050: 6163 7469 6f6e 7320 7769 7468 2042 7562  actions with Bub
-00000060: 626c 652e 696f 2041 5049 2069 6e20 5079  ble.io API in Py
-00000070: 7468 6f6e 206d 6164 6520 6561 7379 2021  thon made easy !
-00000080: 3c2f 7374 726f 6e67 3e3c 2f70 3e0d 0a20  </strong></p>.. 
-00000090: 2020 203c 696d 6720 616c 743d 2250 7974     <img alt="Pyt
-000000a0: 686f 6e20 4261 6467 6522 2073 7263 3d22  hon Badge" src="
-000000b0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000000c0: 6c64 732e 696f 2f62 6164 6765 2f2d 5079  lds.io/badge/-Py
-000000d0: 7468 6f6e 2d44 3644 3644 363f 6c6f 676f  thon-D6D6D6?logo
-000000e0: 3d70 7974 686f 6e22 2f3e 0d0a 2020 2020  =python"/>..    
-000000f0: 3c69 6d67 2061 6c74 3d22 5069 5059 2042  <img alt="PiPY B
-00000100: 6164 6765 2220 7372 633d 2268 7474 7073  adge" src="https
-00000110: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000120: 6f2f 7079 7069 2f76 2f62 7562 626c 652d  o/pypi/v/bubble-
-00000130: 6170 6922 2f3e 0d0a 2020 2020 3c69 6d67  api"/>..    <img
-00000140: 2061 6c74 3d22 4369 2f43 4420 4261 6467   alt="Ci/CD Badg
-00000150: 6522 2073 7263 3d22 6874 7470 733a 2f2f  e" src="https://
-00000160: 6769 7468 7562 2e63 6f6d 2f73 6574 746f  github.com/setto
-00000170: 7261 632d 6e69 6e61 2f62 7562 626c 652d  rac-nina/bubble-
-00000180: 6170 692f 6163 7469 6f6e 732f 776f 726b  api/actions/work
-00000190: 666c 6f77 732f 6369 6364 2e79 616d 6c2f  flows/cicd.yaml/
-000001a0: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
-000001b0: 3d6d 6169 6e29 222f 3e0d 0a20 2020 203c  =main)"/>..    <
-000001c0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000001d0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000001e0: 6261 6467 652f 4d61 6465 2532 3057 6974  badge/Made%20Wit
-000001f0: 682d 4c6f 7665 2d65 6637 6431 362e 7376  h-Love-ef7d16.sv
-00000200: 6722 2f3e 0d0a 3c2f 6469 763e 0d0a 0d0a  g"/>..</div>....
-00000210: 2d2d 2d0d 0a0d 0a23 2320 496e 7374 616c  ---....## Instal
-00000220: 6c69 6e67 0d0a 0d0a 5468 6520 6561 7369  ling....The easi
-00000230: 6573 7420 7761 7920 746f 2069 6e73 7461  est way to insta
-00000240: 6c6c 2069 7420 6973 2074 6872 6f75 6768  ll it is through
-00000250: 202a 2a70 6970 792a 2a20 3a0d 0a0d 0a60   **pipy** :....`
-00000260: 6060 7368 656c 6c0d 0a70 6970 2069 6e73  ``shell..pip ins
-00000270: 7461 6c6c 2062 7562 626c 652d 6170 690d  tall bubble-api.
-00000280: 0a60 6060 0d0a 0d0a 2323 2048 6f77 2074  .```....## How t
-00000290: 6f20 7573 6520 6974 0d0a 0d0a 4174 2074  o use it....At t
-000002a0: 6865 206d 6f6d 656e 742c 2074 6865 7265  he moment, there
-000002b0: 2069 7320 6e6f 2064 6f63 756d 656e 7461   is no documenta
-000002c0: 7469 6f6e 2066 6f72 2074 6869 7320 6c69  tion for this li
-000002d0: 6272 6172 792e 0d0a 596f 7520 6361 6e2c  brary...You can,
-000002e0: 2068 6f77 6576 6572 2c20 7265 6c79 206f   however, rely o
-000002f0: 6e20 7468 6520 696e 7465 6772 6174 696f  n the integratio
-00000300: 6e20 7465 7374 7320 7765 2075 7365 2074  n tests we use t
-00000310: 6f20 656e 7375 7265 2070 726f 7065 7220  o ensure proper 
-00000320: 696e 7465 6772 6174 696f 6e20 7769 7468  integration with
-00000330: 2042 7562 626c 652e 0d0a 596f 7520 6361   Bubble...You ca
-00000340: 6e20 6669 6e64 2074 6865 6d20 5b68 6572  n find them [her
-00000350: 655d 2874 6573 7473 2f69 6e74 6567 7261  e](tests/integra
-00000360: 7469 6f6e 292e 0d0a 0d0a 2323 2320 4372  tion).....### Cr
-00000370: 6561 7469 6e67 2061 2042 7562 626c 6557  eating a BubbleW
-00000380: 7261 7070 6572 2069 6e73 7461 6e63 6520  rapper instance 
-00000390: 3a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  :....```python..
-000003a0: 6672 6f6d 2062 7562 626c 655f 6170 6920  from bubble_api 
-000003b0: 696d 706f 7274 2042 7562 626c 6557 7261  import BubbleWra
-000003c0: 7070 6572 0d0a 0d0a 6275 6262 6c65 5f77  pper....bubble_w
-000003d0: 7261 7070 6572 203d 2042 7562 626c 6557  rapper = BubbleW
-000003e0: 7261 7070 6572 280d 0a20 2020 2062 6173  rapper(..    bas
-000003f0: 655f 7572 6c3d 2268 7474 7073 3a2f 2f63  e_url="https://c
-00000400: 7575 7265 2e63 6f6d 222c 0d0a 2020 2020  uure.com",..    
-00000410: 6170 695f 746f 6b65 6e3d 2259 4f55 525f  api_token="YOUR_
-00000420: 4150 495f 544f 4b45 4e22 2c0d 0a20 2020  API_TOKEN",..   
-00000430: 2062 7562 626c 655f 7665 7273 696f 6e3d   bubble_version=
-00000440: 226c 6976 6522 0d0a 290d 0a60 6060 0d0a  "live"..)..```..
-00000450: 0d0a 2323 2320 496e 7465 7261 6374 2077  ..### Interact w
-00000460: 6974 6820 6275 6262 6c65 2064 6174 6120  ith bubble data 
-00000470: 3a0d 0a0d 0a46 726f 6d20 7468 6520 6042  :....From the `B
-00000480: 7562 626c 6557 7261 7070 6572 6020 696e  ubbleWrapper` in
-00000490: 7374 616e 6365 2079 6f75 2063 616e 206e  stance you can n
-000004a0: 6f77 2069 6e74 6572 6163 7420 7769 7468  ow interact with
-000004b0: 2074 6865 2064 6174 6120 6170 6920 6561   the data api ea
-000004c0: 7369 6c79 2e0d 0a0d 0a60 6060 7079 7468  sily.....```pyth
-000004d0: 6f6e 0d0a 6f62 6a65 6374 5f64 6174 6120  on..object_data 
-000004e0: 3d20 6275 6262 6c65 5f77 7261 7070 6572  = bubble_wrapper
-000004f0: 2e67 6574 280d 0a20 2020 2022 7461 626c  .get(..    "tabl
-00000500: 655f 6e61 6d65 222c 0d0a 2020 2020 6275  e_name",..    bu
-00000510: 6262 6c65 5f69 643d 2262 7562 626c 655f  bble_id="bubble_
-00000520: 6f62 6a65 6374 5f69 6422 2c0d 0a29 0d0a  object_id",..)..
-00000530: 6060 600d 0a41 6e64 2073 6f20 6f6e 2077  ```..And so on w
-00000540: 6974 6820 616c 6c20 7468 6520 6261 7369  ith all the basi
-00000550: 6320 696e 7465 7261 6374 696f 6e73 2077  c interactions w
-00000560: 6974 6820 7468 6520 6170 693a 202a 2a64  ith the api: **d
-00000570: 656c 6574 652a 2a2c 202a 2a75 7064 6174  elete**, **updat
-00000580: 652a 2a2c 202a 2a72 6570 6c61 6365 2a2a  e**, **replace**
-00000590: 2c20 2e2e 2e0d 0a0d 0a59 6f75 2063 616e  , .......You can
-000005a0: 2061 6c73 6f20 7573 6520 636f 6e73 7472   also use constr
-000005b0: 6169 6e74 7320 666f 7220 6765 7474 696e  aints for gettin
-000005c0: 6720 6f72 2064 656c 6574 696e 6720 6f62  g or deleting ob
-000005d0: 6a65 6374 732e 0d0a 5468 6973 2069 7320  jects...This is 
-000005e0: 646f 6e65 2074 6872 6f75 6768 2061 206c  done through a l
-000005f0: 6973 7420 6f66 2060 436f 6e74 7261 696e  ist of `Contrain
-00000600: 7460 206f 626a 6563 7420 796f 7520 6361  t` object you ca
-00000610: 6e20 6465 636c 6172 6520 6279 206f 7065  n declare by ope
-00000620: 7261 7469 6f6e 7320 7769 7468 2074 6865  rations with the
-00000630: 2060 4669 656c 6460 2063 6c61 7373 2e0d   `Field` class..
-00000640: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
-00000650: 6f6d 2062 7562 626c 655f 6170 6920 696d  om bubble_api im
-00000660: 706f 7274 2042 7562 626c 6557 7261 7070  port BubbleWrapp
-00000670: 6572 2c20 4669 656c 640d 0a66 726f 6d20  er, Field..from 
-00000680: 6461 7465 7469 6d65 2069 6d70 6f72 7420  datetime import 
-00000690: 6461 7465 7469 6d65 0d0a 0d0a 6275 6262  datetime....bubb
-000006a0: 6c65 5f77 7261 7070 6572 203d 2042 7562  le_wrapper = Bub
-000006b0: 626c 6557 7261 7070 6572 2820 2e2e 2e20  bleWrapper( ... 
-000006c0: 290d 0a0d 0a63 6f6e 7374 7261 696e 7473  )....constraints
-000006d0: 203d 205b 0d0a 2020 2020 4669 656c 6428   = [..    Field(
-000006e0: 226e 616d 6522 2920 3d3d 2022 426f 6222  "name") == "Bob"
-000006f0: 2c0d 0a20 2020 2046 6965 6c64 2822 4372  ,..    Field("Cr
-00000700: 6561 7465 6422 2920 3e20 6461 7465 7469  eated") > dateti
-00000710: 6d65 2832 3032 332c 2031 2c20 3129 2c0d  me(2023, 1, 1),.
-00000720: 0a5d 0d0a 0d0a 6461 7461 203d 2062 7562  .]....data = bub
-00000730: 626c 655f 7772 6170 7065 722e 6765 7428  ble_wrapper.get(
-00000740: 0d0a 2020 2020 2274 6162 6c65 5f6e 616d  ..    "table_nam
-00000750: 6522 2c0d 0a20 2020 2063 6f6e 7374 7261  e",..    constra
-00000760: 696e 7473 3d63 6f6e 7374 7261 696e 7473  ints=constraints
-00000770: 0d0a 290d 0a60 6060 0d0a 0d0a 416c 6c20  ..)..```....All 
-00000780: 7468 6520 6669 656c 6473 206e 616d 6573  the fields names
-00000790: 2061 6e64 2063 6f6e 7374 7261 696e 7473   and constraints
-000007a0: 2076 616c 7565 7320 666f 726d 6174 7469   values formatti
-000007b0: 6e67 2069 7320 6861 6e64 6c65 2062 7920  ng is handle by 
-000007c0: 7468 6520 6c69 6272 6172 792e 0d0a 0d0a  the library.....
-000007d0: 2323 2049 6e63 6f6d 696e 6720 6665 6174  ## Incoming feat
-000007e0: 7572 6573 0d0a 0d0a 2d20 5b20 5d20 4269  ures....- [ ] Bi
-000007f0: 6720 7265 7175 6573 7420 6f70 7469 6d69  g request optimi
-00000800: 7a61 7469 6f6e 2075 7369 6e67 2072 656d  zation using rem
-00000810: 6169 6e69 6e67 2061 7070 726f 7869 6d61  aining approxima
-00000820: 7469 6f6e 2028 6578 636c 7564 655f 7265  tion (exclude_re
-00000830: 6d61 696e 696e 6729 0d0a 2d20 5b20 5d20  maining)..- [ ] 
-00000840: 4d75 6c74 6974 6872 6561 6469 6e67 0d0a  Multithreading..
-00000850: 2d20 5b20 5d20 4465 6661 756c 7420 6669  - [ ] Default fi
-00000860: 656c 6473 2028 4d6f 6469 6669 6564 2044  elds (Modified D
-00000870: 6174 652c 2075 6e69 7175 6520 6964 2c20  ate, unique id, 
-00000880: 4372 6561 7465 6420 4461 7465 2c20 2e2e  Created Date, ..
-00000890: 2e29 0d0a 2d20 5b20 5d20 4c69 6665 7469  .)..- [ ] Lifeti
-000008a0: 6d65 206f 626a 6563 7420 6d61 6e61 6765  me object manage
-000008b0: 6d65 6e74 2028 7570 6461 7465 2c20 7265  ment (update, re
-000008c0: 6672 6573 682c 2072 6570 6c61 6365 290d  fresh, replace).
-000008d0: 0a2d 205b 205d 2044 6f63 756d 656e 7461  .- [ ] Documenta
-000008e0: 7469 6f6e 0d0a 0d0a 2323 2041 7574 686f  tion....## Autho
-000008f0: 7273 0d0a 0d0a 2a20 2a2a 4479 6c61 6e20  rs....* **Dylan 
-00000900: 4e69 6e61 2a2a 202d 202a 496e 6974 6961  Nina** - *Initia
-00000910: 6c20 776f 726b 2a20 2d20 5b73 6574 746f  l work* - [setto
-00000920: 7261 632d 6e69 6e61 5d28 6874 7470 733a  rac-nina](https:
-00000930: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6574  //github.com/set
-00000940: 746f 7261 632d 6e69 6e61 290d 0a2a 202a  torac-nina)..* *
-00000950: 2a4d 6174 6869 7320 426f 7572 6469 6e2a  *Mathis Bourdin*
-00000960: 2a20 2d20 2a43 6f6e 7472 6962 7574 6f72  * - *Contributor
-00000970: 2a20 2d20 5b6d 6174 6869 7362 7264 6e5d  * - [mathisbrdn]
-00000980: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000990: 636f 6d2f 6d61 7468 6973 6272 646e 290d  com/mathisbrdn).
-000009a0: 0a0d 0a23 2320 4c69 6365 6e73 650d 0a0d  ...## License...
-000009b0: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
-000009c0: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
-000009d0: 7468 6520 4d49 5420 4c69 6365 6e73 6520  the MIT License 
-000009e0: 2d20 7365 6520 7468 6520 5b4c 4943 454e  - see the [LICEN
-000009f0: 5345 5d28 4c49 4345 4e53 4529 2066 696c  SE](LICENSE) fil
-00000a00: 6520 666f 7220 6465 7461 696c 730d 0a    e for details..
+00000010: 6572 223e 0a20 2020 203c 6831 3e3c 636f  er">.    <h1><co
+00000020: 6465 3e42 7562 626c 6520 4170 693c 2f63  de>Bubble Api</c
+00000030: 6f64 653e 3c2f 6831 3e0a 2020 2020 3c70  ode></h1>.    <p
+00000040: 3e3c 7374 726f 6e67 3e49 6e74 6572 6163  ><strong>Interac
+00000050: 7469 6f6e 7320 7769 7468 2042 7562 626c  tions with Bubbl
+00000060: 652e 696f 2041 5049 2069 6e20 5079 7468  e.io API in Pyth
+00000070: 6f6e 206d 6164 6520 6561 7379 2021 3c2f  on made easy !</
+00000080: 7374 726f 6e67 3e3c 2f70 3e0a 2020 2020  strong></p>.    
+00000090: 3c69 6d67 2061 6c74 3d22 5079 7468 6f6e  <img alt="Python
+000000a0: 2042 6164 6765 2220 7372 633d 2268 7474   Badge" src="htt
+000000b0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000000c0: 2e69 6f2f 6261 6467 652f 2d50 7974 686f  .io/badge/-Pytho
+000000d0: 6e2d 4436 4436 4436 3f6c 6f67 6f3d 7079  n-D6D6D6?logo=py
+000000e0: 7468 6f6e 222f 3e0a 2020 2020 3c69 6d67  thon"/>.    <img
+000000f0: 2061 6c74 3d22 5069 5059 2042 6164 6765   alt="PiPY Badge
+00000100: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+00000110: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000120: 7069 2f76 2f62 7562 626c 652d 6170 6922  pi/v/bubble-api"
+00000130: 2f3e 0a20 2020 203c 696d 6720 616c 743d  />.    <img alt=
+00000140: 2243 492f 4344 2042 6164 6765 2220 7372  "CI/CD Badge" sr
+00000150: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00000160: 622e 636f 6d2f 7365 7474 6f72 6163 2d6e  b.com/settorac-n
+00000170: 696e 612f 6275 6262 6c65 2d61 7069 2f61  ina/bubble-api/a
+00000180: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000190: 2f63 6963 642e 7961 6d6c 2f62 6164 6765  /cicd.yaml/badge
+000001a0: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
+000001b0: 2922 2f3e 0a20 2020 203c 696d 6720 7372  )"/>.    <img sr
+000001c0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+000001d0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000001e0: 4d61 6465 2532 3057 6974 682d 4c6f 7665  Made%20With-Love
+000001f0: 2d65 6637 6431 362e 7376 6722 2f3e 0a20  -ef7d16.svg"/>. 
+00000200: 2020 203c 703e 0a20 2020 2020 2020 203c     <p>.        <
+00000210: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000220: 6375 7572 652e 636f 6d3f 7574 6d5f 736f  cuure.com?utm_so
+00000230: 7572 6365 3d67 6974 6875 6226 7574 6d5f  urce=github&utm_
+00000240: 6d65 6469 756d 3d72 6566 6572 7261 6c22  medium=referral"
+00000250: 3e0a 2020 2020 2020 2020 2020 2020 506f  >.            Po
+00000260: 7765 7265 6420 6279 203c 7374 726f 6e67  wered by <strong
+00000270: 3e43 7575 7265 3c2f 7374 726f 6e67 3e0a  >Cuure</strong>.
+00000280: 2020 2020 2020 2020 3c2f 613e 0a20 2020          </a>.   
+00000290: 2020 2020 2026 6e62 7370 3b26 6e62 7370       &nbsp;&nbsp
+000002a0: 3b0a 2020 2020 2020 2020 3c61 2068 7265  ;.        <a hre
+000002b0: 663d 2268 7474 7073 3a2f 2f63 7575 7265  f="https://cuure
+000002c0: 2e63 6f6d 3f75 746d 5f73 6f75 7263 653d  .com?utm_source=
+000002d0: 6769 7468 7562 2675 746d 5f6d 6564 6975  github&utm_mediu
+000002e0: 6d3d 7265 6665 7272 616c 223e 0a20 2020  m=referral">.   
+000002f0: 2020 2020 2020 2020 203c 696d 6720 7372           <img sr
+00000300: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00000310: 622e 636f 6d2f 7365 7474 6f72 6163 2d6e  b.com/settorac-n
+00000320: 696e 612f 6275 6262 6c65 2d61 7069 2f62  ina/bubble-api/b
+00000330: 6c6f 622f 6d61 696e 2f61 7373 6574 732f  lob/main/assets/
+00000340: 6375 7572 655f 6c6f 676f 2e67 6966 2220  cuure_logo.gif" 
+00000350: 7769 6474 683d 2236 3022 2068 6569 6768  width="60" heigh
+00000360: 743d 2236 3022 2061 6c69 676e 3d22 6365  t="60" align="ce
+00000370: 6e74 6572 222f 3e0a 2020 2020 2020 2020  nter"/>.        
+00000380: 3c2f 613e 0a20 2020 203c 2f70 3e0a 3c2f  </a>.    </p>.</
+00000390: 6469 763e 0a0a 2d2d 2d0a 0a23 2320 496e  div>..---..## In
+000003a0: 7374 616c 6c69 6e67 0a0a 5468 6520 6561  stalling..The ea
+000003b0: 7369 6573 7420 7761 7920 746f 2069 6e73  siest way to ins
+000003c0: 7461 6c6c 2069 7420 6973 2074 6872 6f75  tall it is throu
+000003d0: 6768 202a 2a70 6970 792a 2a20 3a0a 0a60  gh **pipy** :..`
+000003e0: 6060 7368 656c 6c0a 7069 7020 696e 7374  ``shell.pip inst
+000003f0: 616c 6c20 6275 6262 6c65 2d61 7069 0a60  all bubble-api.`
+00000400: 6060 0a0a 2323 2048 6f77 2074 6f20 7573  ``..## How to us
+00000410: 6520 6974 0a0a 4174 2074 6865 206d 6f6d  e it..At the mom
+00000420: 656e 742c 2074 6865 7265 2069 7320 6e6f  ent, there is no
+00000430: 2064 6f63 756d 656e 7461 7469 6f6e 2066   documentation f
+00000440: 6f72 2074 6869 7320 6c69 6272 6172 792e  or this library.
+00000450: 0a59 6f75 2063 616e 2c20 686f 7765 7665  .You can, howeve
+00000460: 722c 2072 656c 7920 6f6e 2074 6865 2069  r, rely on the i
+00000470: 6e74 6567 7261 7469 6f6e 2074 6573 7473  ntegration tests
+00000480: 2077 6520 7573 6520 746f 2065 6e73 7572   we use to ensur
+00000490: 6520 7072 6f70 6572 2069 6e74 6567 7261  e proper integra
+000004a0: 7469 6f6e 2077 6974 6820 4275 6262 6c65  tion with Bubble
+000004b0: 2e0a 596f 7520 6361 6e20 6669 6e64 2074  ..You can find t
+000004c0: 6865 6d20 5b68 6572 655d 2874 6573 7473  hem [here](tests
+000004d0: 2f69 6e74 6567 7261 7469 6f6e 292e 0a0a  /integration)...
+000004e0: 2323 2320 4372 6561 7469 6e67 2061 2042  ### Creating a B
+000004f0: 7562 626c 6543 6c69 656e 7420 696e 7374  ubbleClient inst
+00000500: 616e 6365 203a 0a0a 6060 6070 7974 686f  ance :..```pytho
+00000510: 6e0a 6672 6f6d 2062 7562 626c 655f 6170  n.from bubble_ap
+00000520: 6920 696d 706f 7274 2042 7562 626c 6543  i import BubbleC
+00000530: 6c69 656e 740a 0a62 7562 626c 655f 636c  lient..bubble_cl
+00000540: 6965 6e74 203d 2042 7562 626c 6543 6c69  ient = BubbleCli
+00000550: 656e 7428 0a20 2020 2062 6173 655f 7572  ent(.    base_ur
+00000560: 6c3d 2268 7474 7073 3a2f 2f63 7575 7265  l="https://cuure
+00000570: 2e63 6f6d 222c 0a20 2020 2061 7069 5f74  .com",.    api_t
+00000580: 6f6b 656e 3d22 594f 5552 5f41 5049 5f54  oken="YOUR_API_T
+00000590: 4f4b 454e 222c 0a20 2020 2062 7562 626c  OKEN",.    bubbl
+000005a0: 655f 7665 7273 696f 6e3d 226c 6976 6522  e_version="live"
+000005b0: 0a29 0a60 6060 0a0a 2323 2320 496e 7465  .).```..### Inte
+000005c0: 7261 6374 2077 6974 6820 6275 6262 6c65  ract with bubble
+000005d0: 2064 6174 6120 3a0a 0a46 726f 6d20 7468   data :..From th
+000005e0: 6520 6042 7562 626c 6543 6c69 656e 7460  e `BubbleClient`
+000005f0: 2069 6e73 7461 6e63 6520 796f 7520 6361   instance you ca
+00000600: 6e20 6e6f 7720 696e 7465 7261 6374 2077  n now interact w
+00000610: 6974 6820 7468 6520 6461 7461 2061 7069  ith the data api
+00000620: 2065 6173 696c 792e 0a0a 6060 6070 7974   easily...```pyt
+00000630: 686f 6e0a 6f62 6a65 6374 5f64 6174 6120  hon.object_data 
+00000640: 3d20 6275 6262 6c65 5f63 6c69 656e 742e  = bubble_client.
+00000650: 6765 7428 0a20 2020 2022 7461 626c 655f  get(.    "table_
+00000660: 6e61 6d65 222c 0a20 2020 2062 7562 626c  name",.    bubbl
+00000670: 655f 6964 3d22 6275 6262 6c65 5f6f 626a  e_id="bubble_obj
+00000680: 6563 745f 6964 222c 0a29 0a60 6060 0a0a  ect_id",.).```..
+00000690: 416e 6420 736f 206f 6e20 7769 7468 2061  And so on with a
+000006a0: 6c6c 2074 6865 2062 6173 6963 2069 6e74  ll the basic int
+000006b0: 6572 6163 7469 6f6e 7320 7769 7468 2074  eractions with t
+000006c0: 6865 2061 7069 3a20 2a2a 6465 6c65 7465  he api: **delete
+000006d0: 2a2a 2c20 2a2a 7570 6461 7465 2a2a 2c20  **, **update**, 
+000006e0: 2a2a 7265 706c 6163 652a 2a2c 202e 2e2e  **replace**, ...
+000006f0: 0a0a 596f 7520 6361 6e20 616c 736f 2075  ..You can also u
+00000700: 7365 2063 6f6e 7374 7261 696e 7473 2066  se constraints f
+00000710: 6f72 2067 6574 7469 6e67 206f 7220 6465  or getting or de
+00000720: 6c65 7469 6e67 206f 626a 6563 7473 2e0a  leting objects..
+00000730: 5468 6973 2069 7320 646f 6e65 2074 6872  This is done thr
+00000740: 6f75 6768 2061 206c 6973 7420 6f66 2060  ough a list of `
+00000750: 436f 6e74 7261 696e 7460 206f 626a 6563  Contraint` objec
+00000760: 7420 796f 7520 6361 6e20 6465 636c 6172  t you can declar
+00000770: 6520 6279 206f 7065 7261 7469 6f6e 7320  e by operations 
+00000780: 7769 7468 2074 6865 2060 4669 656c 6460  with the `Field`
+00000790: 2063 6c61 7373 2e0a 0a60 6060 7079 7468   class...```pyth
+000007a0: 6f6e 0a66 726f 6d20 6275 6262 6c65 5f61  on.from bubble_a
+000007b0: 7069 2069 6d70 6f72 7420 4275 6262 6c65  pi import Bubble
+000007c0: 436c 6965 6e74 2c20 4669 656c 640a 6672  Client, Field.fr
+000007d0: 6f6d 2064 6174 6574 696d 6520 696d 706f  om datetime impo
+000007e0: 7274 2064 6174 6574 696d 650a 0a62 7562  rt datetime..bub
+000007f0: 626c 655f 636c 6965 6e74 203d 2042 7562  ble_client = Bub
+00000800: 626c 6543 6c69 656e 7428 202e 2e2e 2029  bleClient( ... )
+00000810: 0a0a 636f 6e73 7472 6169 6e74 7320 3d20  ..constraints = 
+00000820: 5b0a 2020 2020 4669 656c 6428 226e 616d  [.    Field("nam
+00000830: 6522 2920 3d3d 2022 426f 6222 2c0a 2020  e") == "Bob",.  
+00000840: 2020 4669 656c 6428 2243 7265 6174 6564    Field("Created
+00000850: 2229 203e 2064 6174 6574 696d 6528 3230  ") > datetime(20
+00000860: 3233 2c20 312c 2031 292c 0a5d 0a0a 6461  23, 1, 1),.]..da
+00000870: 7461 203d 2062 7562 626c 655f 636c 6965  ta = bubble_clie
+00000880: 6e74 2e67 6574 280a 2020 2020 2274 6162  nt.get(.    "tab
+00000890: 6c65 5f6e 616d 6522 2c0a 2020 2020 636f  le_name",.    co
+000008a0: 6e73 7472 6169 6e74 733d 636f 6e73 7472  nstraints=constr
+000008b0: 6169 6e74 730a 290a 6060 600a 0a41 6c6c  aints.).```..All
+000008c0: 2074 6865 2066 6965 6c64 7320 6e61 6d65   the fields name
+000008d0: 7320 616e 6420 636f 6e73 7472 6169 6e74  s and constraint
+000008e0: 7320 7661 6c75 6573 2066 6f72 6d61 7474  s values formatt
+000008f0: 696e 6720 6973 2068 616e 646c 6520 6279  ing is handle by
+00000900: 2074 6865 206c 6962 7261 7279 2e0a 0a23   the library...#
+00000910: 2320 496e 636f 6d69 6e67 2066 6561 7475  # Incoming featu
+00000920: 7265 730a 0a2d 205b 205d 2042 6967 2072  res..- [ ] Big r
+00000930: 6571 7565 7374 206f 7074 696d 697a 6174  equest optimizat
+00000940: 696f 6e20 7573 696e 6720 7265 6d61 696e  ion using remain
+00000950: 696e 6720 6170 7072 6f78 696d 6174 696f  ing approximatio
+00000960: 6e20 2865 7863 6c75 6465 5f72 656d 6169  n (exclude_remai
+00000970: 6e69 6e67 290a 2d20 5b20 5d20 4d75 6c74  ning).- [ ] Mult
+00000980: 6974 6872 6561 6469 6e67 0a2d 205b 205d  ithreading.- [ ]
+00000990: 2044 6566 6175 6c74 2066 6965 6c64 7320   Default fields 
+000009a0: 284d 6f64 6966 6965 6420 4461 7465 2c20  (Modified Date, 
+000009b0: 756e 6971 7565 2069 642c 2043 7265 6174  unique id, Creat
+000009c0: 6564 2044 6174 652c 202e 2e2e 290a 2d20  ed Date, ...).- 
+000009d0: 5b20 5d20 4c69 6665 7469 6d65 206f 626a  [ ] Lifetime obj
+000009e0: 6563 7420 6d61 6e61 6765 6d65 6e74 2028  ect management (
+000009f0: 7570 6461 7465 2c20 7265 6672 6573 682c  update, refresh,
+00000a00: 2072 6570 6c61 6365 290a 2d20 5b20 5d20   replace).- [ ] 
+00000a10: 446f 6375 6d65 6e74 6174 696f 6e0a 0a23  Documentation..#
+00000a20: 2320 4175 7468 6f72 730a 0a2a 202a 2a44  # Authors..* **D
+00000a30: 796c 616e 204e 696e 612a 2a20 2d20 2a49  ylan Nina** - *I
+00000a40: 6e69 7469 616c 2077 6f72 6b2a 202d 205b  nitial work* - [
+00000a50: 7365 7474 6f72 6163 2d6e 696e 615d 2868  settorac-nina](h
+00000a60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000a70: 6d2f 7365 7474 6f72 6163 2d6e 696e 6129  m/settorac-nina)
+00000a80: 0a2a 202a 2a4d 6174 6869 7320 426f 7572  .* **Mathis Bour
+00000a90: 6469 6e2a 2a20 2d20 2a43 6f6e 7472 6962  din** - *Contrib
+00000aa0: 7574 6f72 2a20 2d20 5b6d 6174 6869 7362  utor* - [mathisb
+00000ab0: 7264 6e5d 2868 7474 7073 3a2f 2f67 6974  rdn](https://git
+00000ac0: 6875 622e 636f 6d2f 6d61 7468 6973 6272  hub.com/mathisbr
+00000ad0: 646e 290a 0a23 2320 4c69 6365 6e73 650a  dn)..## License.
+00000ae0: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
+00000af0: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
+00000b00: 7468 6520 4d49 5420 4c69 6365 6e73 6520  the MIT License 
+00000b10: 2d20 7365 6520 7468 6520 5b4c 4943 454e  - see the [LICEN
+00000b20: 5345 5d28 4c49 4345 4e53 4529 2066 696c  SE](LICENSE) fil
+00000b30: 6520 666f 7220 6465 7461 696c 730a       e for details.
```

### Comparing `bubble_api-0.4.0/bubble_api/constraint.py` & `bubble_api-0.4.1/bubble_api/constraint.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from __future__ import annotations
-
-import datetime
-from collections.abc import Iterable
-from numbers import Number
-from typing import Any
-
-
-class Constraint:
-    def __init__(self, key: str, constraint_type: str, value: Any | None = None):
-        self.key = key
-        self.constraint_type = constraint_type
-        self.value = self.format_constraint_value(value)
-
-    @staticmethod
-    def format_constraint_value(value: Any) -> str | list[str] | None:
-        if value is None:
-            return None
-        if isinstance(value, str):
-            return value
-        if isinstance(value, Number):
-            return str(value)
-        if isinstance(value, datetime.datetime):
-            return value.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
-        if isinstance(value, datetime.date):
-            return value.strftime("%Y-%m-%d")
-        if isinstance(value, Iterable):
-            return [Constraint.format_constraint_value(v) for v in value]
-        return value
-
-    def to_dict(self) -> dict:
-        res = {
-            "key": self.key,
-            "constraint_type": self.constraint_type,
-        }
-
-        if self.value:
-            res["value"] = self.value
-        return res
+from __future__ import annotations
+
+import datetime
+from collections.abc import Iterable
+from numbers import Number
+from typing import Any
+
+
+class Constraint:
+    def __init__(self, key: str, constraint_type: str, value: Any | None = None):
+        self.key = key
+        self.constraint_type = constraint_type
+        self.value = self.format_constraint_value(value)
+
+    @staticmethod
+    def format_constraint_value(value: Any) -> str | list[str] | None:
+        if value is None:
+            return None
+        if isinstance(value, str):
+            return value
+        if isinstance(value, Number):
+            return str(value)
+        if isinstance(value, datetime.datetime):
+            return value.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
+        if isinstance(value, datetime.date):
+            return value.strftime("%Y-%m-%d")
+        if isinstance(value, Iterable):
+            return [Constraint.format_constraint_value(v) for v in value]
+        return value
+
+    def to_dict(self) -> dict:
+        res = {
+            "key": self.key,
+            "constraint_type": self.constraint_type,
+        }
+
+        if self.value:
+            res["value"] = self.value
+        return res
```

### Comparing `bubble_api-0.4.0/bubble_api/wrapper.py` & `bubble_api-0.4.1/bubble_api/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,285 +1,291 @@
-from __future__ import annotations
-
-import json
-import time
-from collections.abc import Iterable
-from itertools import islice
-
-import requests
-
-from .constraint import Constraint
-from .field import Field
-
-API_VERSION = "1.1"
-
-
-class BubbleWrapper:
-    def __init__(
-        self,
-        base_url: str,
-        api_token: str | None = None,
-        bubble_version: str = "test",
-        *args,
-        **kwargs,
-    ):
-        if bubble_version != "live":
-            base_url = f"{base_url}/version-{bubble_version}"
-        self.base_url = f"{base_url}/api/{API_VERSION}"
-        self.api_token = api_token
-
-    def _get_headers(self) -> dict | None:
-        return (
-            {
-                "Authorization": f"Bearer {self.api_token}",
-            }
-            if self.api_token is not None
-            else None
-        )
-
-    @staticmethod
-    def _format_constraints(
-        constraints: Constraint | Iterable[Constraint] | None = None,
-    ) -> str:
-        if constraints is None:
-            constraints = list()
-        if isinstance(constraints, Constraint):
-            constraints = [constraints]
-        return json.dumps([constraint.to_dict() for constraint in constraints])
-
-    @staticmethod
-    def format_bubble_type(bubble_type: str):
-        return bubble_type.lower().replace(" ", "")
-
-    def make_request(
-        self,
-        nb_retries: int = 3,
-        sleep_time: float = 0.2,
-        exponential_backoff: bool = False,
-        **kwargs,
-    ) -> requests.Response:
-        if kwargs.get("headers") is None:
-            kwargs["headers"] = self._get_headers()
-
-        response = requests.request(**kwargs)
-
-        if response.status_code // 100 == 2:
-            return response
-
-        if nb_retries == 0 or response.status_code // 100 == 4:
-            print(response.text)
-            response.raise_for_status()
-
-        time.sleep(sleep_time)
-
-        if exponential_backoff:
-            sleep_time *= 2
-
-        return self.make_request(
-            nb_retries=nb_retries - 1,
-            sleep_time=sleep_time,
-            exponential_backoff=exponential_backoff,
-            **kwargs,
-        )
-
-    def get(
-        self,
-        bubble_type: str,
-        bubble_id: str | None = None,
-        column_name: str | None = None,
-        constraints: list[Constraint] | None = None,
-        **kwargs,
-    ):
-        bubble_type = self.format_bubble_type(bubble_type)
-        if bubble_id is not None:
-            return self.get_by_id(bubble_type, bubble_id, column_name, **kwargs)
-        return self.get_objects(bubble_type, constraints, **kwargs)
-
-    def create(self, bubble_type: str, fields: dict | list[dict] = None, **kwargs):
-        bubble_type = self.format_bubble_type(bubble_type)
-        if isinstance(fields, list):
-            return self.create_bulk(bubble_type, fields=fields, **kwargs)
-        return self.create_object(bubble_type, fields, **kwargs)
-
-    def delete(
-        self,
-        bubble_type: str,
-        bubble_id: str | Iterable[str] | None = None,
-        constraints: Constraint | Iterable[Constraint] | None = None,
-        **kwargs,
-    ):
-        bubble_type = self.format_bubble_type(bubble_type)
-        if bubble_id is not None and constraints is not None:
-            raise TypeError("You can't specify both bubble_id and constraints.")
-        if isinstance(bubble_id, str):
-            return self.delete_by_id(bubble_type, bubble_id, **kwargs)
-        if isinstance(bubble_id, Iterable):
-            return self.delete_by_ids(bubble_type, bubble_id, **kwargs)
-        if constraints is not None:
-            return self.delete_objects(bubble_type, constraints, **kwargs)
-        raise Warning(
-            "You must specify at least one of bubble_id, bubble_ids or constraints.",
-            "If you intend to delete the whole table, please use the delete_all method.",
-        )
-
-    def get_by_id(self, bubble_type, bubble_id, column_name=None, **kwargs):
-        bubble_type = self.format_bubble_type(bubble_type)
-        if column_name is not None:
-            objs = self.get_objects(
-                bubble_type,
-                [Field(column_name) == bubble_id],
-            )
-            return objs[0] if len(objs) > 0 else None
-
-        url = f"{self.base_url}/obj/{bubble_type}/{bubble_id}"
-
-        resp = self.make_request(method="GET", url=url, **kwargs)
-
-        return resp.json()["response"]
-
-    def create_object(self, bubble_type: str, fields: dict | None = None, **kwargs):
-        bubble_type = self.format_bubble_type(bubble_type)
-        url = f"{self.base_url}/obj/{bubble_type}"
-
-        resp = self.make_request(method="POST", url=url, json=fields, **kwargs)
-
-        return resp.json()["id"]
-
-    def update_object(self, bubble_type: str, bubble_id: str, fields: dict, **kwargs):
-        bubble_type = self.format_bubble_type(bubble_type)
-        url = f"{self.base_url}/obj/{bubble_type}/{bubble_id}"
-
-        self.make_request(method="PATCH", url=url, json=fields, **kwargs)
-
-    def replace_object(self, bubble_type: str, bubble_id: str, fields: dict, **kwargs):
-        bubble_type = self.format_bubble_type(bubble_type)
-        url = f"{self.base_url}/obj/{bubble_type}/{bubble_id}"
-
-        self.make_request(method="PUT", url=url, json=fields, **kwargs)
-
-    def delete_by_id(self, bubble_type: str, bubble_id: str, **kwargs):
-        bubble_type = self.format_bubble_type(bubble_type)
-        url = f"{self.base_url}/obj/{bubble_type}/{bubble_id}"
-
-        self.make_request(method="DELETE", url=url, **kwargs)
-
-    def delete_by_ids(self, bubble_type: str, ids: Iterable[str], **kwargs):
-        bubble_type = self.format_bubble_type(bubble_type)
-        for _id in ids:
-            self.delete_by_id(bubble_type, _id, **kwargs)
-
-    def delete_objects(
-        self,
-        bubble_type: str,
-        constraints: Constraint | Iterable[Constraint] | None = None,
-        **kwargs,
-    ):
-        bubble_type = self.format_bubble_type(bubble_type)
-        self.delete_by_ids(
-            bubble_type,
-            (
-                obj["_id"]
-                for obj in self.get_objects_gen(bubble_type, constraints, **kwargs)
-            ),
-            **kwargs,
-        )
-
-    def delete_all(self, bubble_type, **kwargs):
-        bubble_type = self.format_bubble_type(bubble_type)
-        self.delete_objects(bubble_type, list(), **kwargs)
-
-    def create_bulk(self, bubble_type: str, fields: list[dict], **kwargs) -> list:
-        bubble_type = self.format_bubble_type(bubble_type)
-        url = f"{self.base_url}/obj/{bubble_type}/bulk"
-        headers = {
-            **self._get_headers(),
-            "Content-Type": "text/plain",
-        }
-
-        resp = self.make_request(
-            method="POST",
-            url=url,
-            data="\n".join(json.dumps(f) for f in fields),
-            headers=headers,
-            **kwargs,
-        )
-
-        return [json.loads(r) for r in resp.text.split("\n")]
-
-    def count_objects(
-        self,
-        bubble_type: str,
-        constraints: Constraint | Iterable[Constraint] | None = None,
-        **kwargs,
-    ):
-        bubble_type = self.format_bubble_type(bubble_type)
-        url = f"{self.base_url}/obj/{bubble_type}"
-        constraints = self._format_constraints(constraints)
-
-        params = {
-            "constraints": constraints,
-            "cursor": 0,
-            "limit": 1,
-        }
-
-        resp = self.make_request(method="GET", url=url, params=params, **kwargs)
-        json_resp = resp.json()["response"]
-
-        return json_resp["count"] + json_resp["remaining"]
-
-    def get_objects_gen(
-        self,
-        bubble_type: str,
-        constraints: Constraint | Iterable[Constraint] | None = None,
-        sort_field: str = None,
-        descending: bool = False,
-        limit: int = 100,
-        **kwargs,
-    ):
-        bubble_type = self.format_bubble_type(bubble_type)
-        url = f"{self.base_url}/obj/{bubble_type}"
-
-        constraints = self._format_constraints(constraints)
-
-        if isinstance(sort_field, Field):
-            sort_field = sort_field.field_name
-
-        params = {
-            "constraints": constraints,
-            "cursor": 0,
-            "limit": limit,
-            "sort_field": sort_field,
-            "descending": descending,
-        }
-
-        while True:
-            resp = self.make_request(method="GET", url=url, params=params, **kwargs)
-            json_resp = resp.json()["response"]
-            yield from json_resp["results"]
-
-            params["cursor"] = json_resp["cursor"] + json_resp["count"]
-
-            if json_resp["remaining"] == 0:
-                break
-
-    def get_objects(
-        self,
-        bubble_type: str,
-        constraints: Constraint | Iterable[Constraint] | None = None,
-        max_objects: int | None = None,
-        **kwargs,
-    ):
-        bubble_type = self.format_bubble_type(bubble_type)
-        return list(
-            islice(
-                self.get_objects_gen(bubble_type, constraints, **kwargs), max_objects
-            )
-        )
-
-    def run_workflow(
-        self, wf_name: str, params: dict | None = None, method: str = "POST", **kwargs
-    ):
-        url = f"{self.base_url}/wf/{wf_name}"
-
-        resp = self.make_request(method=method, url=url, json=params, **kwargs)
-
-        return resp.json()["response"]
+from __future__ import annotations
+
+import json
+import time
+from collections.abc import Iterable
+from itertools import islice
+
+import requests
+
+from .constraint import Constraint
+from .field import Field
+
+API_VERSION = "1.1"
+
+
+class BubbleClient:
+    def __init__(
+        self,
+        base_url: str,
+        api_token: str | None = None,
+        bubble_version: str = "test",
+        *args,
+        **kwargs,
+    ):
+        if bubble_version != "live":
+            base_url = f"{base_url}/version-{bubble_version}"
+        self.base_url = f"{base_url}/api/{API_VERSION}"
+        self.api_token = api_token
+
+    def _get_headers(self) -> dict | None:
+        return (
+            {
+                "Authorization": f"Bearer {self.api_token}",
+            }
+            if self.api_token is not None
+            else None
+        )
+
+    @staticmethod
+    def _format_constraints(
+        constraints: Constraint | Iterable[Constraint] | None = None,
+    ) -> str:
+        if constraints is None:
+            constraints = list()
+        if isinstance(constraints, Constraint):
+            constraints = [constraints]
+        return json.dumps([constraint.to_dict() for constraint in constraints])
+
+    @staticmethod
+    def format_bubble_type(bubble_type: str):
+        return bubble_type.lower().replace(" ", "")
+
+    def make_request(
+        self,
+        nb_retries: int = 3,
+        sleep_time: float = 0.2,
+        exponential_backoff: bool = False,
+        **kwargs,
+    ) -> requests.Response:
+        if kwargs.get("headers") is None:
+            kwargs["headers"] = self._get_headers()
+
+        response = requests.request(**kwargs)
+
+        if response.status_code // 100 == 2:
+            return response
+
+        if nb_retries == 0 or response.status_code // 100 == 4:
+            print(response.text)
+            response.raise_for_status()
+
+        time.sleep(sleep_time)
+
+        if exponential_backoff:
+            sleep_time *= 2
+
+        return self.make_request(
+            nb_retries=nb_retries - 1,
+            sleep_time=sleep_time,
+            exponential_backoff=exponential_backoff,
+            **kwargs,
+        )
+
+    def get(
+        self,
+        bubble_type: str,
+        bubble_id: str | None = None,
+        column_name: str | None = None,
+        constraints: list[Constraint] | None = None,
+        **kwargs,
+    ):
+        bubble_type = self.format_bubble_type(bubble_type)
+        if bubble_id is not None:
+            return self.get_by_id(bubble_type, bubble_id, column_name, **kwargs)
+        return self.get_objects(bubble_type, constraints, **kwargs)
+
+    def create(self, bubble_type: str, fields: dict | list[dict] = None, **kwargs):
+        bubble_type = self.format_bubble_type(bubble_type)
+        if isinstance(fields, list):
+            return self.create_bulk(bubble_type, fields=fields, **kwargs)
+        return self.create_object(bubble_type, fields, **kwargs)
+
+    def delete(
+        self,
+        bubble_type: str,
+        bubble_id: str | Iterable[str] | None = None,
+        constraints: Constraint | Iterable[Constraint] | None = None,
+        **kwargs,
+    ):
+        bubble_type = self.format_bubble_type(bubble_type)
+        if bubble_id is not None and constraints is not None:
+            raise TypeError("You can't specify both bubble_id and constraints.")
+        if isinstance(bubble_id, str):
+            return self.delete_by_id(bubble_type, bubble_id, **kwargs)
+        if isinstance(bubble_id, Iterable):
+            return self.delete_by_ids(bubble_type, bubble_id, **kwargs)
+        if constraints is not None:
+            return self.delete_objects(bubble_type, constraints, **kwargs)
+        raise Warning(
+            "You must specify at least one of bubble_id, bubble_ids or constraints.",
+            "If you intend to delete the whole table, please use the delete_all method.",
+        )
+
+    def get_by_id(self, bubble_type, bubble_id, column_name=None, **kwargs):
+        bubble_type = self.format_bubble_type(bubble_type)
+        if column_name is not None:
+            objs = self.get_objects(
+                bubble_type,
+                [Field(column_name) == bubble_id],
+            )
+
+            if not objs:
+                raise requests.exceptions.HTTPError(
+                    f"Could not find object with id {bubble_id} in column {column_name}."
+                )
+
+            return objs[0]
+
+        url = f"{self.base_url}/obj/{bubble_type}/{bubble_id}"
+
+        resp = self.make_request(method="GET", url=url, **kwargs)
+
+        return resp.json()["response"]
+
+    def create_object(self, bubble_type: str, fields: dict | None = None, **kwargs):
+        bubble_type = self.format_bubble_type(bubble_type)
+        url = f"{self.base_url}/obj/{bubble_type}"
+
+        resp = self.make_request(method="POST", url=url, json=fields, **kwargs)
+
+        return resp.json()["id"]
+
+    def update_object(self, bubble_type: str, bubble_id: str, fields: dict, **kwargs):
+        bubble_type = self.format_bubble_type(bubble_type)
+        url = f"{self.base_url}/obj/{bubble_type}/{bubble_id}"
+
+        self.make_request(method="PATCH", url=url, json=fields, **kwargs)
+
+    def replace_object(self, bubble_type: str, bubble_id: str, fields: dict, **kwargs):
+        bubble_type = self.format_bubble_type(bubble_type)
+        url = f"{self.base_url}/obj/{bubble_type}/{bubble_id}"
+
+        self.make_request(method="PUT", url=url, json=fields, **kwargs)
+
+    def delete_by_id(self, bubble_type: str, bubble_id: str, **kwargs):
+        bubble_type = self.format_bubble_type(bubble_type)
+        url = f"{self.base_url}/obj/{bubble_type}/{bubble_id}"
+
+        self.make_request(method="DELETE", url=url, **kwargs)
+
+    def delete_by_ids(self, bubble_type: str, ids: Iterable[str], **kwargs):
+        bubble_type = self.format_bubble_type(bubble_type)
+        for _id in ids:
+            self.delete_by_id(bubble_type, _id, **kwargs)
+
+    def delete_objects(
+        self,
+        bubble_type: str,
+        constraints: Constraint | Iterable[Constraint] | None = None,
+        **kwargs,
+    ):
+        bubble_type = self.format_bubble_type(bubble_type)
+        self.delete_by_ids(
+            bubble_type,
+            (
+                obj["_id"]
+                for obj in self.get_objects_gen(bubble_type, constraints, **kwargs)
+            ),
+            **kwargs,
+        )
+
+    def delete_all(self, bubble_type, **kwargs):
+        bubble_type = self.format_bubble_type(bubble_type)
+        self.delete_objects(bubble_type, list(), **kwargs)
+
+    def create_bulk(self, bubble_type: str, fields: list[dict], **kwargs) -> list:
+        bubble_type = self.format_bubble_type(bubble_type)
+        url = f"{self.base_url}/obj/{bubble_type}/bulk"
+        headers = {
+            **self._get_headers(),
+            "Content-Type": "text/plain",
+        }
+
+        resp = self.make_request(
+            method="POST",
+            url=url,
+            data="\n".join(json.dumps(f) for f in fields),
+            headers=headers,
+            **kwargs,
+        )
+
+        return [json.loads(r) for r in resp.text.split("\n")]
+
+    def count_objects(
+        self,
+        bubble_type: str,
+        constraints: Constraint | Iterable[Constraint] | None = None,
+        **kwargs,
+    ):
+        bubble_type = self.format_bubble_type(bubble_type)
+        url = f"{self.base_url}/obj/{bubble_type}"
+        constraints = self._format_constraints(constraints)
+
+        params = {
+            "constraints": constraints,
+            "cursor": 0,
+            "limit": 1,
+        }
+
+        resp = self.make_request(method="GET", url=url, params=params, **kwargs)
+        json_resp = resp.json()["response"]
+
+        return json_resp["count"] + json_resp["remaining"]
+
+    def get_objects_gen(
+        self,
+        bubble_type: str,
+        constraints: Constraint | Iterable[Constraint] | None = None,
+        sort_field: str = None,
+        descending: bool = False,
+        limit: int = 100,
+        **kwargs,
+    ):
+        bubble_type = self.format_bubble_type(bubble_type)
+        url = f"{self.base_url}/obj/{bubble_type}"
+
+        constraints = self._format_constraints(constraints)
+
+        if isinstance(sort_field, Field):
+            sort_field = sort_field.field_name
+
+        params = {
+            "constraints": constraints,
+            "cursor": 0,
+            "limit": limit,
+            "sort_field": sort_field,
+            "descending": descending,
+        }
+
+        while True:
+            resp = self.make_request(method="GET", url=url, params=params, **kwargs)
+            json_resp = resp.json()["response"]
+            yield from json_resp["results"]
+
+            params["cursor"] = json_resp["cursor"] + json_resp["count"]
+
+            if json_resp["remaining"] == 0:
+                break
+
+    def get_objects(
+        self,
+        bubble_type: str,
+        constraints: Constraint | Iterable[Constraint] | None = None,
+        max_objects: int | None = None,
+        **kwargs,
+    ):
+        bubble_type = self.format_bubble_type(bubble_type)
+        return list(
+            islice(
+                self.get_objects_gen(bubble_type, constraints, **kwargs), max_objects
+            )
+        )
+
+    def run_workflow(
+        self, wf_name: str, params: dict | None = None, method: str = "POST", **kwargs
+    ):
+        url = f"{self.base_url}/wf/{wf_name}"
+
+        resp = self.make_request(method=method, url=url, json=params, **kwargs)
+
+        return resp.json()["response"]
```

### Comparing `bubble_api-0.4.0/bubble_api.egg-info/PKG-INFO` & `bubble_api-0.4.1/bubble_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,214 +1,232 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2062 7562  : 2.1..Name: bub
-00000020: 626c 652d 6170 690d 0a56 6572 7369 6f6e  ble-api..Version
-00000030: 3a20 302e 342e 300d 0a53 756d 6d61 7279  : 0.4.0..Summary
-00000040: 3a20 496e 7465 7261 6374 696f 6e73 2077  : Interactions w
-00000050: 6974 6820 4275 6262 6c65 2e69 6f20 4150  ith Bubble.io AP
-00000060: 4920 696e 2050 7974 686f 6e20 6d61 6465  I in Python made
-00000070: 2065 6173 7920 210d 0a41 7574 686f 722d   easy !..Author-
-00000080: 656d 6169 6c3a 2044 796c 616e 204e 494e  email: Dylan NIN
-00000090: 4120 3c73 6574 746f 7261 632e 6e69 6e61  A <settorac.nina
-000000a0: 4067 6d61 696c 2e63 6f6d 3e2c 204d 6174  @gmail.com>, Mat
-000000b0: 6869 7320 426f 7572 6469 6e20 3c6d 6174  his Bourdin <mat
-000000c0: 6869 7362 7264 6e40 676d 6169 6c2e 636f  hisbrdn@gmail.co
-000000d0: 6d3e 0d0a 5072 6f6a 6563 742d 5552 4c3a  m>..Project-URL:
-000000e0: 2048 6f6d 6570 6167 652c 2068 7474 7073   Homepage, https
-000000f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
-00000100: 7474 6f72 6163 2d6e 696e 612f 6275 6262  ttorac-nina/bubb
-00000110: 6c65 2d61 7069 0d0a 5072 6f6a 6563 742d  le-api..Project-
-00000120: 5552 4c3a 2042 7567 2054 7261 636b 6572  URL: Bug Tracker
-00000130: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-00000140: 2e63 6f6d 2f73 6574 746f 7261 632d 6e69  .com/settorac-ni
-00000150: 6e61 2f62 7562 626c 652d 6170 692f 6973  na/bubble-api/is
-00000160: 7375 6573 0d0a 436c 6173 7369 6669 6572  sues..Classifier
-00000170: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000180: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000190: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
-000001a0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001b0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001c0: 330d 0a43 6c61 7373 6966 6965 723a 2050  3..Classifier: P
-000001d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000001e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000001f0: 2033 2e38 0d0a 436c 6173 7369 6669 6572   3.8..Classifier
-00000200: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000210: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000220: 203a 3a20 332e 390d 0a43 6c61 7373 6966   :: 3.9..Classif
-00000230: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000240: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000250: 686f 6e20 3a3a 2033 2e31 300d 0a43 6c61  hon :: 3.10..Cla
-00000260: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000270: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000280: 2050 7974 686f 6e20 3a3a 2033 2e31 310d   Python :: 3.11.
-00000290: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
-000002a0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-000002b0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-000002c0: 6e73 650d 0a43 6c61 7373 6966 6965 723a  nse..Classifier:
-000002d0: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-000002e0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-000002f0: 656e 740d 0a52 6571 7569 7265 732d 5079  ent..Requires-Py
-00000300: 7468 6f6e 3a20 3e3d 332e 380d 0a44 6573  thon: >=3.8..Des
-00000310: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-00000320: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00000330: 646f 776e 0d0a 4c69 6365 6e73 652d 4669  down..License-Fi
-00000340: 6c65 3a20 4c49 4345 4e53 450d 0a0d 0a3c  le: LICENSE....<
-00000350: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-00000360: 7222 3e0d 0a20 2020 203c 6831 3e3c 636f  r">..    <h1><co
-00000370: 6465 3e42 7562 626c 6520 4170 693c 2f63  de>Bubble Api</c
-00000380: 6f64 653e 3c2f 6831 3e0d 0a20 2020 203c  ode></h1>..    <
-00000390: 703e 3c73 7472 6f6e 673e 496e 7465 7261  p><strong>Intera
-000003a0: 6374 696f 6e73 2077 6974 6820 4275 6262  ctions with Bubb
-000003b0: 6c65 2e69 6f20 4150 4920 696e 2050 7974  le.io API in Pyt
-000003c0: 686f 6e20 6d61 6465 2065 6173 7920 213c  hon made easy !<
-000003d0: 2f73 7472 6f6e 673e 3c2f 703e 0d0a 2020  /strong></p>..  
-000003e0: 2020 3c69 6d67 2061 6c74 3d22 5079 7468    <img alt="Pyth
-000003f0: 6f6e 2042 6164 6765 2220 7372 633d 2268  on Badge" src="h
-00000400: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000410: 6473 2e69 6f2f 6261 6467 652f 2d50 7974  ds.io/badge/-Pyt
-00000420: 686f 6e2d 4436 4436 4436 3f6c 6f67 6f3d  hon-D6D6D6?logo=
-00000430: 7079 7468 6f6e 222f 3e0d 0a20 2020 203c  python"/>..    <
-00000440: 696d 6720 616c 743d 2250 6950 5920 4261  img alt="PiPY Ba
-00000450: 6467 6522 2073 7263 3d22 6874 7470 733a  dge" src="https:
-00000460: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000470: 2f70 7970 692f 762f 6275 6262 6c65 2d61  /pypi/v/bubble-a
-00000480: 7069 222f 3e0d 0a20 2020 203c 696d 6720  pi"/>..    <img 
-00000490: 616c 743d 2243 692f 4344 2042 6164 6765  alt="Ci/CD Badge
-000004a0: 2220 7372 633d 2268 7474 7073 3a2f 2f67  " src="https://g
-000004b0: 6974 6875 622e 636f 6d2f 7365 7474 6f72  ithub.com/settor
-000004c0: 6163 2d6e 696e 612f 6275 6262 6c65 2d61  ac-nina/bubble-a
-000004d0: 7069 2f61 6374 696f 6e73 2f77 6f72 6b66  pi/actions/workf
-000004e0: 6c6f 7773 2f63 6963 642e 7961 6d6c 2f62  lows/cicd.yaml/b
-000004f0: 6164 6765 2e73 7667 3f62 7261 6e63 683d  adge.svg?branch=
-00000500: 6d61 696e 2922 2f3e 0d0a 2020 2020 3c69  main)"/>..    <i
-00000510: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000520: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000530: 6164 6765 2f4d 6164 6525 3230 5769 7468  adge/Made%20With
-00000540: 2d4c 6f76 652d 6566 3764 3136 2e73 7667  -Love-ef7d16.svg
-00000550: 222f 3e0d 0a3c 2f64 6976 3e0d 0a0d 0a2d  "/>..</div>....-
-00000560: 2d2d 0d0a 0d0a 2323 2049 6e73 7461 6c6c  --....## Install
-00000570: 696e 670d 0a0d 0a54 6865 2065 6173 6965  ing....The easie
-00000580: 7374 2077 6179 2074 6f20 696e 7374 616c  st way to instal
-00000590: 6c20 6974 2069 7320 7468 726f 7567 6820  l it is through 
-000005a0: 2a2a 7069 7079 2a2a 203a 0d0a 0d0a 6060  **pipy** :....``
-000005b0: 6073 6865 6c6c 0d0a 7069 7020 696e 7374  `shell..pip inst
-000005c0: 616c 6c20 6275 6262 6c65 2d61 7069 0d0a  all bubble-api..
-000005d0: 6060 600d 0a0d 0a23 2320 486f 7720 746f  ```....## How to
-000005e0: 2075 7365 2069 740d 0a0d 0a41 7420 7468   use it....At th
-000005f0: 6520 6d6f 6d65 6e74 2c20 7468 6572 6520  e moment, there 
-00000600: 6973 206e 6f20 646f 6375 6d65 6e74 6174  is no documentat
-00000610: 696f 6e20 666f 7220 7468 6973 206c 6962  ion for this lib
-00000620: 7261 7279 2e0d 0a59 6f75 2063 616e 2c20  rary...You can, 
-00000630: 686f 7765 7665 722c 2072 656c 7920 6f6e  however, rely on
-00000640: 2074 6865 2069 6e74 6567 7261 7469 6f6e   the integration
-00000650: 2074 6573 7473 2077 6520 7573 6520 746f   tests we use to
-00000660: 2065 6e73 7572 6520 7072 6f70 6572 2069   ensure proper i
-00000670: 6e74 6567 7261 7469 6f6e 2077 6974 6820  ntegration with 
-00000680: 4275 6262 6c65 2e0d 0a59 6f75 2063 616e  Bubble...You can
-00000690: 2066 696e 6420 7468 656d 205b 6865 7265   find them [here
-000006a0: 5d28 7465 7374 732f 696e 7465 6772 6174  ](tests/integrat
-000006b0: 696f 6e29 2e0d 0a0d 0a23 2323 2043 7265  ion).....### Cre
-000006c0: 6174 696e 6720 6120 4275 6262 6c65 5772  ating a BubbleWr
-000006d0: 6170 7065 7220 696e 7374 616e 6365 203a  apper instance :
-000006e0: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a66  ....```python..f
-000006f0: 726f 6d20 6275 6262 6c65 5f61 7069 2069  rom bubble_api i
-00000700: 6d70 6f72 7420 4275 6262 6c65 5772 6170  mport BubbleWrap
-00000710: 7065 720d 0a0d 0a62 7562 626c 655f 7772  per....bubble_wr
-00000720: 6170 7065 7220 3d20 4275 6262 6c65 5772  apper = BubbleWr
-00000730: 6170 7065 7228 0d0a 2020 2020 6261 7365  apper(..    base
-00000740: 5f75 726c 3d22 6874 7470 733a 2f2f 6375  _url="https://cu
-00000750: 7572 652e 636f 6d22 2c0d 0a20 2020 2061  ure.com",..    a
-00000760: 7069 5f74 6f6b 656e 3d22 594f 5552 5f41  pi_token="YOUR_A
-00000770: 5049 5f54 4f4b 454e 222c 0d0a 2020 2020  PI_TOKEN",..    
-00000780: 6275 6262 6c65 5f76 6572 7369 6f6e 3d22  bubble_version="
-00000790: 6c69 7665 220d 0a29 0d0a 6060 600d 0a0d  live"..)..```...
-000007a0: 0a23 2323 2049 6e74 6572 6163 7420 7769  .### Interact wi
-000007b0: 7468 2062 7562 626c 6520 6461 7461 203a  th bubble data :
-000007c0: 0d0a 0d0a 4672 6f6d 2074 6865 2060 4275  ....From the `Bu
-000007d0: 6262 6c65 5772 6170 7065 7260 2069 6e73  bbleWrapper` ins
-000007e0: 7461 6e63 6520 796f 7520 6361 6e20 6e6f  tance you can no
-000007f0: 7720 696e 7465 7261 6374 2077 6974 6820  w interact with 
-00000800: 7468 6520 6461 7461 2061 7069 2065 6173  the data api eas
-00000810: 696c 792e 0d0a 0d0a 6060 6070 7974 686f  ily.....```pytho
-00000820: 6e0d 0a6f 626a 6563 745f 6461 7461 203d  n..object_data =
-00000830: 2062 7562 626c 655f 7772 6170 7065 722e   bubble_wrapper.
-00000840: 6765 7428 0d0a 2020 2020 2274 6162 6c65  get(..    "table
-00000850: 5f6e 616d 6522 2c0d 0a20 2020 2062 7562  _name",..    bub
-00000860: 626c 655f 6964 3d22 6275 6262 6c65 5f6f  ble_id="bubble_o
-00000870: 626a 6563 745f 6964 222c 0d0a 290d 0a60  bject_id",..)..`
-00000880: 6060 0d0a 416e 6420 736f 206f 6e20 7769  ``..And so on wi
-00000890: 7468 2061 6c6c 2074 6865 2062 6173 6963  th all the basic
-000008a0: 2069 6e74 6572 6163 7469 6f6e 7320 7769   interactions wi
-000008b0: 7468 2074 6865 2061 7069 3a20 2a2a 6465  th the api: **de
-000008c0: 6c65 7465 2a2a 2c20 2a2a 7570 6461 7465  lete**, **update
-000008d0: 2a2a 2c20 2a2a 7265 706c 6163 652a 2a2c  **, **replace**,
-000008e0: 202e 2e2e 0d0a 0d0a 596f 7520 6361 6e20   .......You can 
-000008f0: 616c 736f 2075 7365 2063 6f6e 7374 7261  also use constra
-00000900: 696e 7473 2066 6f72 2067 6574 7469 6e67  ints for getting
-00000910: 206f 7220 6465 6c65 7469 6e67 206f 626a   or deleting obj
-00000920: 6563 7473 2e0d 0a54 6869 7320 6973 2064  ects...This is d
-00000930: 6f6e 6520 7468 726f 7567 6820 6120 6c69  one through a li
-00000940: 7374 206f 6620 6043 6f6e 7472 6169 6e74  st of `Contraint
-00000950: 6020 6f62 6a65 6374 2079 6f75 2063 616e  ` object you can
-00000960: 2064 6563 6c61 7265 2062 7920 6f70 6572   declare by oper
-00000970: 6174 696f 6e73 2077 6974 6820 7468 6520  ations with the 
-00000980: 6046 6965 6c64 6020 636c 6173 732e 0d0a  `Field` class...
-00000990: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
-000009a0: 6d20 6275 6262 6c65 5f61 7069 2069 6d70  m bubble_api imp
-000009b0: 6f72 7420 4275 6262 6c65 5772 6170 7065  ort BubbleWrappe
-000009c0: 722c 2046 6965 6c64 0d0a 6672 6f6d 2064  r, Field..from d
-000009d0: 6174 6574 696d 6520 696d 706f 7274 2064  atetime import d
-000009e0: 6174 6574 696d 650d 0a0d 0a62 7562 626c  atetime....bubbl
-000009f0: 655f 7772 6170 7065 7220 3d20 4275 6262  e_wrapper = Bubb
-00000a00: 6c65 5772 6170 7065 7228 202e 2e2e 2029  leWrapper( ... )
-00000a10: 0d0a 0d0a 636f 6e73 7472 6169 6e74 7320  ....constraints 
-00000a20: 3d20 5b0d 0a20 2020 2046 6965 6c64 2822  = [..    Field("
-00000a30: 6e61 6d65 2229 203d 3d20 2242 6f62 222c  name") == "Bob",
-00000a40: 0d0a 2020 2020 4669 656c 6428 2243 7265  ..    Field("Cre
-00000a50: 6174 6564 2229 203e 2064 6174 6574 696d  ated") > datetim
-00000a60: 6528 3230 3233 2c20 312c 2031 292c 0d0a  e(2023, 1, 1),..
-00000a70: 5d0d 0a0d 0a64 6174 6120 3d20 6275 6262  ]....data = bubb
-00000a80: 6c65 5f77 7261 7070 6572 2e67 6574 280d  le_wrapper.get(.
-00000a90: 0a20 2020 2022 7461 626c 655f 6e61 6d65  .    "table_name
-00000aa0: 222c 0d0a 2020 2020 636f 6e73 7472 6169  ",..    constrai
-00000ab0: 6e74 733d 636f 6e73 7472 6169 6e74 730d  nts=constraints.
-00000ac0: 0a29 0d0a 6060 600d 0a0d 0a41 6c6c 2074  .)..```....All t
-00000ad0: 6865 2066 6965 6c64 7320 6e61 6d65 7320  he fields names 
-00000ae0: 616e 6420 636f 6e73 7472 6169 6e74 7320  and constraints 
-00000af0: 7661 6c75 6573 2066 6f72 6d61 7474 696e  values formattin
-00000b00: 6720 6973 2068 616e 646c 6520 6279 2074  g is handle by t
-00000b10: 6865 206c 6962 7261 7279 2e0d 0a0d 0a23  he library.....#
-00000b20: 2320 496e 636f 6d69 6e67 2066 6561 7475  # Incoming featu
-00000b30: 7265 730d 0a0d 0a2d 205b 205d 2042 6967  res....- [ ] Big
-00000b40: 2072 6571 7565 7374 206f 7074 696d 697a   request optimiz
-00000b50: 6174 696f 6e20 7573 696e 6720 7265 6d61  ation using rema
-00000b60: 696e 696e 6720 6170 7072 6f78 696d 6174  ining approximat
-00000b70: 696f 6e20 2865 7863 6c75 6465 5f72 656d  ion (exclude_rem
-00000b80: 6169 6e69 6e67 290d 0a2d 205b 205d 204d  aining)..- [ ] M
-00000b90: 756c 7469 7468 7265 6164 696e 670d 0a2d  ultithreading..-
-00000ba0: 205b 205d 2044 6566 6175 6c74 2066 6965   [ ] Default fie
-00000bb0: 6c64 7320 284d 6f64 6966 6965 6420 4461  lds (Modified Da
-00000bc0: 7465 2c20 756e 6971 7565 2069 642c 2043  te, unique id, C
-00000bd0: 7265 6174 6564 2044 6174 652c 202e 2e2e  reated Date, ...
-00000be0: 290d 0a2d 205b 205d 204c 6966 6574 696d  )..- [ ] Lifetim
-00000bf0: 6520 6f62 6a65 6374 206d 616e 6167 656d  e object managem
-00000c00: 656e 7420 2875 7064 6174 652c 2072 6566  ent (update, ref
-00000c10: 7265 7368 2c20 7265 706c 6163 6529 0d0a  resh, replace)..
-00000c20: 2d20 5b20 5d20 446f 6375 6d65 6e74 6174  - [ ] Documentat
-00000c30: 696f 6e0d 0a0d 0a23 2320 4175 7468 6f72  ion....## Author
-00000c40: 730d 0a0d 0a2a 202a 2a44 796c 616e 204e  s....* **Dylan N
-00000c50: 696e 612a 2a20 2d20 2a49 6e69 7469 616c  ina** - *Initial
-00000c60: 2077 6f72 6b2a 202d 205b 7365 7474 6f72   work* - [settor
-00000c70: 6163 2d6e 696e 615d 2868 7474 7073 3a2f  ac-nina](https:/
-00000c80: 2f67 6974 6875 622e 636f 6d2f 7365 7474  /github.com/sett
-00000c90: 6f72 6163 2d6e 696e 6129 0d0a 2a20 2a2a  orac-nina)..* **
-00000ca0: 4d61 7468 6973 2042 6f75 7264 696e 2a2a  Mathis Bourdin**
-00000cb0: 202d 202a 436f 6e74 7269 6275 746f 722a   - *Contributor*
-00000cc0: 202d 205b 6d61 7468 6973 6272 646e 5d28   - [mathisbrdn](
-00000cd0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000ce0: 6f6d 2f6d 6174 6869 7362 7264 6e29 0d0a  om/mathisbrdn)..
-00000cf0: 0d0a 2323 204c 6963 656e 7365 0d0a 0d0a  ..## License....
-00000d00: 5468 6973 2070 726f 6a65 6374 2069 7320  This project is 
-00000d10: 6c69 6365 6e73 6564 2075 6e64 6572 2074  licensed under t
-00000d20: 6865 204d 4954 204c 6963 656e 7365 202d  he MIT License -
-00000d30: 2073 6565 2074 6865 205b 4c49 4345 4e53   see the [LICENS
-00000d40: 455d 284c 4943 454e 5345 2920 6669 6c65  E](LICENSE) file
-00000d50: 2066 6f72 2064 6574 6169 6c73 0d0a        for details..
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6275 6262  : 2.1.Name: bubb
+00000020: 6c65 2d61 7069 0a56 6572 7369 6f6e 3a20  le-api.Version: 
+00000030: 302e 342e 310a 5375 6d6d 6172 793a 2049  0.4.1.Summary: I
+00000040: 6e74 6572 6163 7469 6f6e 7320 7769 7468  nteractions with
+00000050: 2042 7562 626c 652e 696f 2041 5049 2069   Bubble.io API i
+00000060: 6e20 5079 7468 6f6e 206d 6164 6520 6561  n Python made ea
+00000070: 7379 2021 0a41 7574 686f 722d 656d 6169  sy !.Author-emai
+00000080: 6c3a 2044 796c 616e 204e 494e 4120 3c73  l: Dylan NINA <s
+00000090: 6574 746f 7261 632e 6e69 6e61 4067 6d61  ettorac.nina@gma
+000000a0: 696c 2e63 6f6d 3e2c 204d 6174 6869 7320  il.com>, Mathis 
+000000b0: 426f 7572 6469 6e20 3c6d 6174 6869 7362  Bourdin <mathisb
+000000c0: 7264 6e40 676d 6169 6c2e 636f 6d3e 0a50  rdn@gmail.com>.P
+000000d0: 726f 6a65 6374 2d55 524c 3a20 486f 6d65  roject-URL: Home
+000000e0: 7061 6765 2c20 6874 7470 733a 2f2f 6769  page, https://gi
+000000f0: 7468 7562 2e63 6f6d 2f73 6574 746f 7261  thub.com/settora
+00000100: 632d 6e69 6e61 2f62 7562 626c 652d 6170  c-nina/bubble-ap
+00000110: 690a 5072 6f6a 6563 742d 5552 4c3a 2042  i.Project-URL: B
+00000120: 7567 2054 7261 636b 6572 2c20 6874 7470  ug Tracker, http
+00000130: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000140: 6574 746f 7261 632d 6e69 6e61 2f62 7562  ettorac-nina/bub
+00000150: 626c 652d 6170 692f 6973 7375 6573 0a43  ble-api/issues.C
+00000160: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000170: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000180: 3a3a 2050 7974 686f 6e0a 436c 6173 7369  :: Python.Classi
+00000190: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000001a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001b0: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
+000001c0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000001d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001e0: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
+000001f0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000200: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000210: 5079 7468 6f6e 203a 3a20 332e 390a 436c  Python :: 3.9.Cl
+00000220: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000230: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000240: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000250: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000260: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000270: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000280: 2e31 310a 436c 6173 7369 6669 6572 3a20  .11.Classifier: 
+00000290: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+000002a0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+000002b0: 6963 656e 7365 0a43 6c61 7373 6966 6965  icense.Classifie
+000002c0: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+000002d0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000002e0: 6e64 656e 740a 5265 7175 6972 6573 2d50  ndent.Requires-P
+000002f0: 7974 686f 6e3a 203e 3d33 2e38 0a44 6573  ython: >=3.8.Des
+00000300: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00000310: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00000320: 646f 776e 0a4c 6963 656e 7365 2d46 696c  down.License-Fil
+00000330: 653a 204c 4943 454e 5345 0a0a 3c64 6976  e: LICENSE..<div
+00000340: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000350: 0a20 2020 203c 6831 3e3c 636f 6465 3e42  .    <h1><code>B
+00000360: 7562 626c 6520 4170 693c 2f63 6f64 653e  ubble Api</code>
+00000370: 3c2f 6831 3e0a 2020 2020 3c70 3e3c 7374  </h1>.    <p><st
+00000380: 726f 6e67 3e49 6e74 6572 6163 7469 6f6e  rong>Interaction
+00000390: 7320 7769 7468 2042 7562 626c 652e 696f  s with Bubble.io
+000003a0: 2041 5049 2069 6e20 5079 7468 6f6e 206d   API in Python m
+000003b0: 6164 6520 6561 7379 2021 3c2f 7374 726f  ade easy !</stro
+000003c0: 6e67 3e3c 2f70 3e0a 2020 2020 3c69 6d67  ng></p>.    <img
+000003d0: 2061 6c74 3d22 5079 7468 6f6e 2042 6164   alt="Python Bad
+000003e0: 6765 2220 7372 633d 2268 7474 7073 3a2f  ge" src="https:/
+000003f0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000400: 6261 6467 652f 2d50 7974 686f 6e2d 4436  badge/-Python-D6
+00000410: 4436 4436 3f6c 6f67 6f3d 7079 7468 6f6e  D6D6?logo=python
+00000420: 222f 3e0a 2020 2020 3c69 6d67 2061 6c74  "/>.    <img alt
+00000430: 3d22 5069 5059 2042 6164 6765 2220 7372  ="PiPY Badge" sr
+00000440: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000450: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+00000460: 2f62 7562 626c 652d 6170 6922 2f3e 0a20  /bubble-api"/>. 
+00000470: 2020 203c 696d 6720 616c 743d 2243 492f     <img alt="CI/
+00000480: 4344 2042 6164 6765 2220 7372 633d 2268  CD Badge" src="h
+00000490: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000004a0: 6d2f 7365 7474 6f72 6163 2d6e 696e 612f  m/settorac-nina/
+000004b0: 6275 6262 6c65 2d61 7069 2f61 6374 696f  bubble-api/actio
+000004c0: 6e73 2f77 6f72 6b66 6c6f 7773 2f63 6963  ns/workflows/cic
+000004d0: 642e 7961 6d6c 2f62 6164 6765 2e73 7667  d.yaml/badge.svg
+000004e0: 3f62 7261 6e63 683d 6d61 696e 2922 2f3e  ?branch=main)"/>
+000004f0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+00000500: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000510: 6473 2e69 6f2f 6261 6467 652f 4d61 6465  ds.io/badge/Made
+00000520: 2532 3057 6974 682d 4c6f 7665 2d65 6637  %20With-Love-ef7
+00000530: 6431 362e 7376 6722 2f3e 0a20 2020 203c  d16.svg"/>.    <
+00000540: 703e 0a20 2020 2020 2020 203c 6120 6872  p>.        <a hr
+00000550: 6566 3d22 6874 7470 733a 2f2f 6375 7572  ef="https://cuur
+00000560: 652e 636f 6d3f 7574 6d5f 736f 7572 6365  e.com?utm_source
+00000570: 3d67 6974 6875 6226 7574 6d5f 6d65 6469  =github&utm_medi
+00000580: 756d 3d72 6566 6572 7261 6c22 3e0a 2020  um=referral">.  
+00000590: 2020 2020 2020 2020 2020 506f 7765 7265            Powere
+000005a0: 6420 6279 203c 7374 726f 6e67 3e43 7575  d by <strong>Cuu
+000005b0: 7265 3c2f 7374 726f 6e67 3e0a 2020 2020  re</strong>.    
+000005c0: 2020 2020 3c2f 613e 0a20 2020 2020 2020      </a>.       
+000005d0: 2026 6e62 7370 3b26 6e62 7370 3b0a 2020   &nbsp;&nbsp;.  
+000005e0: 2020 2020 2020 3c61 2068 7265 663d 2268        <a href="h
+000005f0: 7474 7073 3a2f 2f63 7575 7265 2e63 6f6d  ttps://cuure.com
+00000600: 3f75 746d 5f73 6f75 7263 653d 6769 7468  ?utm_source=gith
+00000610: 7562 2675 746d 5f6d 6564 6975 6d3d 7265  ub&utm_medium=re
+00000620: 6665 7272 616c 223e 0a20 2020 2020 2020  ferral">.       
+00000630: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
+00000640: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000650: 6d2f 7365 7474 6f72 6163 2d6e 696e 612f  m/settorac-nina/
+00000660: 6275 6262 6c65 2d61 7069 2f62 6c6f 622f  bubble-api/blob/
+00000670: 6d61 696e 2f61 7373 6574 732f 6375 7572  main/assets/cuur
+00000680: 655f 6c6f 676f 2e67 6966 2220 7769 6474  e_logo.gif" widt
+00000690: 683d 2236 3022 2068 6569 6768 743d 2236  h="60" height="6
+000006a0: 3022 2061 6c69 676e 3d22 6365 6e74 6572  0" align="center
+000006b0: 222f 3e0a 2020 2020 2020 2020 3c2f 613e  "/>.        </a>
+000006c0: 0a20 2020 203c 2f70 3e0a 3c2f 6469 763e  .    </p>.</div>
+000006d0: 0a0a 2d2d 2d0a 0a23 2320 496e 7374 616c  ..---..## Instal
+000006e0: 6c69 6e67 0a0a 5468 6520 6561 7369 6573  ling..The easies
+000006f0: 7420 7761 7920 746f 2069 6e73 7461 6c6c  t way to install
+00000700: 2069 7420 6973 2074 6872 6f75 6768 202a   it is through *
+00000710: 2a70 6970 792a 2a20 3a0a 0a60 6060 7368  *pipy** :..```sh
+00000720: 656c 6c0a 7069 7020 696e 7374 616c 6c20  ell.pip install 
+00000730: 6275 6262 6c65 2d61 7069 0a60 6060 0a0a  bubble-api.```..
+00000740: 2323 2048 6f77 2074 6f20 7573 6520 6974  ## How to use it
+00000750: 0a0a 4174 2074 6865 206d 6f6d 656e 742c  ..At the moment,
+00000760: 2074 6865 7265 2069 7320 6e6f 2064 6f63   there is no doc
+00000770: 756d 656e 7461 7469 6f6e 2066 6f72 2074  umentation for t
+00000780: 6869 7320 6c69 6272 6172 792e 0a59 6f75  his library..You
+00000790: 2063 616e 2c20 686f 7765 7665 722c 2072   can, however, r
+000007a0: 656c 7920 6f6e 2074 6865 2069 6e74 6567  ely on the integ
+000007b0: 7261 7469 6f6e 2074 6573 7473 2077 6520  ration tests we 
+000007c0: 7573 6520 746f 2065 6e73 7572 6520 7072  use to ensure pr
+000007d0: 6f70 6572 2069 6e74 6567 7261 7469 6f6e  oper integration
+000007e0: 2077 6974 6820 4275 6262 6c65 2e0a 596f   with Bubble..Yo
+000007f0: 7520 6361 6e20 6669 6e64 2074 6865 6d20  u can find them 
+00000800: 5b68 6572 655d 2874 6573 7473 2f69 6e74  [here](tests/int
+00000810: 6567 7261 7469 6f6e 292e 0a0a 2323 2320  egration)...### 
+00000820: 4372 6561 7469 6e67 2061 2042 7562 626c  Creating a Bubbl
+00000830: 6543 6c69 656e 7420 696e 7374 616e 6365  eClient instance
+00000840: 203a 0a0a 6060 6070 7974 686f 6e0a 6672   :..```python.fr
+00000850: 6f6d 2062 7562 626c 655f 6170 6920 696d  om bubble_api im
+00000860: 706f 7274 2042 7562 626c 6543 6c69 656e  port BubbleClien
+00000870: 740a 0a62 7562 626c 655f 636c 6965 6e74  t..bubble_client
+00000880: 203d 2042 7562 626c 6543 6c69 656e 7428   = BubbleClient(
+00000890: 0a20 2020 2062 6173 655f 7572 6c3d 2268  .    base_url="h
+000008a0: 7474 7073 3a2f 2f63 7575 7265 2e63 6f6d  ttps://cuure.com
+000008b0: 222c 0a20 2020 2061 7069 5f74 6f6b 656e  ",.    api_token
+000008c0: 3d22 594f 5552 5f41 5049 5f54 4f4b 454e  ="YOUR_API_TOKEN
+000008d0: 222c 0a20 2020 2062 7562 626c 655f 7665  ",.    bubble_ve
+000008e0: 7273 696f 6e3d 226c 6976 6522 0a29 0a60  rsion="live".).`
+000008f0: 6060 0a0a 2323 2320 496e 7465 7261 6374  ``..### Interact
+00000900: 2077 6974 6820 6275 6262 6c65 2064 6174   with bubble dat
+00000910: 6120 3a0a 0a46 726f 6d20 7468 6520 6042  a :..From the `B
+00000920: 7562 626c 6543 6c69 656e 7460 2069 6e73  ubbleClient` ins
+00000930: 7461 6e63 6520 796f 7520 6361 6e20 6e6f  tance you can no
+00000940: 7720 696e 7465 7261 6374 2077 6974 6820  w interact with 
+00000950: 7468 6520 6461 7461 2061 7069 2065 6173  the data api eas
+00000960: 696c 792e 0a0a 6060 6070 7974 686f 6e0a  ily...```python.
+00000970: 6f62 6a65 6374 5f64 6174 6120 3d20 6275  object_data = bu
+00000980: 6262 6c65 5f63 6c69 656e 742e 6765 7428  bble_client.get(
+00000990: 0a20 2020 2022 7461 626c 655f 6e61 6d65  .    "table_name
+000009a0: 222c 0a20 2020 2062 7562 626c 655f 6964  ",.    bubble_id
+000009b0: 3d22 6275 6262 6c65 5f6f 626a 6563 745f  ="bubble_object_
+000009c0: 6964 222c 0a29 0a60 6060 0a0a 416e 6420  id",.).```..And 
+000009d0: 736f 206f 6e20 7769 7468 2061 6c6c 2074  so on with all t
+000009e0: 6865 2062 6173 6963 2069 6e74 6572 6163  he basic interac
+000009f0: 7469 6f6e 7320 7769 7468 2074 6865 2061  tions with the a
+00000a00: 7069 3a20 2a2a 6465 6c65 7465 2a2a 2c20  pi: **delete**, 
+00000a10: 2a2a 7570 6461 7465 2a2a 2c20 2a2a 7265  **update**, **re
+00000a20: 706c 6163 652a 2a2c 202e 2e2e 0a0a 596f  place**, .....Yo
+00000a30: 7520 6361 6e20 616c 736f 2075 7365 2063  u can also use c
+00000a40: 6f6e 7374 7261 696e 7473 2066 6f72 2067  onstraints for g
+00000a50: 6574 7469 6e67 206f 7220 6465 6c65 7469  etting or deleti
+00000a60: 6e67 206f 626a 6563 7473 2e0a 5468 6973  ng objects..This
+00000a70: 2069 7320 646f 6e65 2074 6872 6f75 6768   is done through
+00000a80: 2061 206c 6973 7420 6f66 2060 436f 6e74   a list of `Cont
+00000a90: 7261 696e 7460 206f 626a 6563 7420 796f  raint` object yo
+00000aa0: 7520 6361 6e20 6465 636c 6172 6520 6279  u can declare by
+00000ab0: 206f 7065 7261 7469 6f6e 7320 7769 7468   operations with
+00000ac0: 2074 6865 2060 4669 656c 6460 2063 6c61   the `Field` cla
+00000ad0: 7373 2e0a 0a60 6060 7079 7468 6f6e 0a66  ss...```python.f
+00000ae0: 726f 6d20 6275 6262 6c65 5f61 7069 2069  rom bubble_api i
+00000af0: 6d70 6f72 7420 4275 6262 6c65 436c 6965  mport BubbleClie
+00000b00: 6e74 2c20 4669 656c 640a 6672 6f6d 2064  nt, Field.from d
+00000b10: 6174 6574 696d 6520 696d 706f 7274 2064  atetime import d
+00000b20: 6174 6574 696d 650a 0a62 7562 626c 655f  atetime..bubble_
+00000b30: 636c 6965 6e74 203d 2042 7562 626c 6543  client = BubbleC
+00000b40: 6c69 656e 7428 202e 2e2e 2029 0a0a 636f  lient( ... )..co
+00000b50: 6e73 7472 6169 6e74 7320 3d20 5b0a 2020  nstraints = [.  
+00000b60: 2020 4669 656c 6428 226e 616d 6522 2920    Field("name") 
+00000b70: 3d3d 2022 426f 6222 2c0a 2020 2020 4669  == "Bob",.    Fi
+00000b80: 656c 6428 2243 7265 6174 6564 2229 203e  eld("Created") >
+00000b90: 2064 6174 6574 696d 6528 3230 3233 2c20   datetime(2023, 
+00000ba0: 312c 2031 292c 0a5d 0a0a 6461 7461 203d  1, 1),.]..data =
+00000bb0: 2062 7562 626c 655f 636c 6965 6e74 2e67   bubble_client.g
+00000bc0: 6574 280a 2020 2020 2274 6162 6c65 5f6e  et(.    "table_n
+00000bd0: 616d 6522 2c0a 2020 2020 636f 6e73 7472  ame",.    constr
+00000be0: 6169 6e74 733d 636f 6e73 7472 6169 6e74  aints=constraint
+00000bf0: 730a 290a 6060 600a 0a41 6c6c 2074 6865  s.).```..All the
+00000c00: 2066 6965 6c64 7320 6e61 6d65 7320 616e   fields names an
+00000c10: 6420 636f 6e73 7472 6169 6e74 7320 7661  d constraints va
+00000c20: 6c75 6573 2066 6f72 6d61 7474 696e 6720  lues formatting 
+00000c30: 6973 2068 616e 646c 6520 6279 2074 6865  is handle by the
+00000c40: 206c 6962 7261 7279 2e0a 0a23 2320 496e   library...## In
+00000c50: 636f 6d69 6e67 2066 6561 7475 7265 730a  coming features.
+00000c60: 0a2d 205b 205d 2042 6967 2072 6571 7565  .- [ ] Big reque
+00000c70: 7374 206f 7074 696d 697a 6174 696f 6e20  st optimization 
+00000c80: 7573 696e 6720 7265 6d61 696e 696e 6720  using remaining 
+00000c90: 6170 7072 6f78 696d 6174 696f 6e20 2865  approximation (e
+00000ca0: 7863 6c75 6465 5f72 656d 6169 6e69 6e67  xclude_remaining
+00000cb0: 290a 2d20 5b20 5d20 4d75 6c74 6974 6872  ).- [ ] Multithr
+00000cc0: 6561 6469 6e67 0a2d 205b 205d 2044 6566  eading.- [ ] Def
+00000cd0: 6175 6c74 2066 6965 6c64 7320 284d 6f64  ault fields (Mod
+00000ce0: 6966 6965 6420 4461 7465 2c20 756e 6971  ified Date, uniq
+00000cf0: 7565 2069 642c 2043 7265 6174 6564 2044  ue id, Created D
+00000d00: 6174 652c 202e 2e2e 290a 2d20 5b20 5d20  ate, ...).- [ ] 
+00000d10: 4c69 6665 7469 6d65 206f 626a 6563 7420  Lifetime object 
+00000d20: 6d61 6e61 6765 6d65 6e74 2028 7570 6461  management (upda
+00000d30: 7465 2c20 7265 6672 6573 682c 2072 6570  te, refresh, rep
+00000d40: 6c61 6365 290a 2d20 5b20 5d20 446f 6375  lace).- [ ] Docu
+00000d50: 6d65 6e74 6174 696f 6e0a 0a23 2320 4175  mentation..## Au
+00000d60: 7468 6f72 730a 0a2a 202a 2a44 796c 616e  thors..* **Dylan
+00000d70: 204e 696e 612a 2a20 2d20 2a49 6e69 7469   Nina** - *Initi
+00000d80: 616c 2077 6f72 6b2a 202d 205b 7365 7474  al work* - [sett
+00000d90: 6f72 6163 2d6e 696e 615d 2868 7474 7073  orac-nina](https
+00000da0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
+00000db0: 7474 6f72 6163 2d6e 696e 6129 0a2a 202a  ttorac-nina).* *
+00000dc0: 2a4d 6174 6869 7320 426f 7572 6469 6e2a  *Mathis Bourdin*
+00000dd0: 2a20 2d20 2a43 6f6e 7472 6962 7574 6f72  * - *Contributor
+00000de0: 2a20 2d20 5b6d 6174 6869 7362 7264 6e5d  * - [mathisbrdn]
+00000df0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000e00: 636f 6d2f 6d61 7468 6973 6272 646e 290a  com/mathisbrdn).
+00000e10: 0a23 2320 4c69 6365 6e73 650a 0a54 6869  .## License..Thi
+00000e20: 7320 7072 6f6a 6563 7420 6973 206c 6963  s project is lic
+00000e30: 656e 7365 6420 756e 6465 7220 7468 6520  ensed under the 
+00000e40: 4d49 5420 4c69 6365 6e73 6520 2d20 7365  MIT License - se
+00000e50: 6520 7468 6520 5b4c 4943 454e 5345 5d28  e the [LICENSE](
+00000e60: 4c49 4345 4e53 4529 2066 696c 6520 666f  LICENSE) file fo
+00000e70: 7220 6465 7461 696c 730a                 r details.
```

### Comparing `bubble_api-0.4.0/pyproject.toml` & `bubble_api-0.4.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-[build-system]
-requires = ["setuptools>=61"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "bubble_api"
-version = "0.4.0"
-authors = [
-    { name="Dylan NINA", email="settorac.nina@gmail.com" },
-    { name="Mathis Bourdin", email="mathisbrdn@gmail.com" },
-]
-description = "Interactions with Bubble.io API in Python made easy !"
-readme = "README.md"
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-dependencies = [
-    'requests',
-]
-
-[tool.setuptools]
-packages = ["bubble_api"]
-
-[project.urls]
-"Homepage" = "https://github.com/settorac-nina/bubble-api"
-"Bug Tracker" = "https://github.com/settorac-nina/bubble-api/issues"
+[build-system]
+requires = ["setuptools>=61"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "bubble_api"
+version = "0.4.1"
+authors = [
+    { name="Dylan NINA", email="settorac.nina@gmail.com" },
+    { name="Mathis Bourdin", email="mathisbrdn@gmail.com" },
+]
+description = "Interactions with Bubble.io API in Python made easy !"
+readme = "README.md"
+requires-python = ">=3.8"
+classifiers = [
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+dependencies = [
+    'requests',
+]
+
+[tool.setuptools]
+packages = ["bubble_api"]
+
+[project.urls]
+"Homepage" = "https://github.com/settorac-nina/bubble-api"
+"Bug Tracker" = "https://github.com/settorac-nina/bubble-api/issues"
```

