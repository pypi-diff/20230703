# Comparing `tmp/sreddit-1.2.5.tar.gz` & `tmp/sreddit-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sreddit-1.2.5.tar", last modified: Tue Oct 26 20:22:41 2021, max compression
+gzip compressed data, was "sreddit-1.2.6.tar", last modified: Sun Jul  2 21:13:00 2023, max compression
```

## Comparing `sreddit-1.2.5.tar` & `sreddit-1.2.6.tar`

### file list

```diff
@@ -1,16 +1,11 @@
-drwxrwxrwx   0        0        0        0 2021-10-26 20:22:41.500506 sreddit-1.2.5/
--rw-rw-rw-   0        0        0     1092 2021-10-21 23:23:26.000000 sreddit-1.2.5/LICENSE
--rw-rw-rw-   0        0        0     1392 2021-10-26 20:22:41.501307 sreddit-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      925 2021-10-25 01:21:36.000000 sreddit-1.2.5/README.md
--rw-rw-rw-   0        0        0      108 2021-10-21 23:18:29.000000 sreddit-1.2.5/pyproject.toml
--rw-rw-rw-   0        0        0      618 2021-10-26 20:22:41.506677 sreddit-1.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2021-10-26 20:22:41.382363 sreddit-1.2.5/src/
-drwxrwxrwx   0        0        0        0 2021-10-26 20:22:41.408129 sreddit-1.2.5/src/sreddit/
--rw-rw-rw-   0        0        0        2 2021-10-21 23:12:48.000000 sreddit-1.2.5/src/sreddit/__init__.py
--rw-rw-rw-   0        0        0     4499 2021-10-26 19:55:09.000000 sreddit-1.2.5/src/sreddit/srtitles.py
-drwxrwxrwx   0        0        0        0 2021-10-26 20:22:41.497469 sreddit-1.2.5/src/sreddit.egg-info/
--rw-rw-rw-   0        0        0     1392 2021-10-26 20:22:41.000000 sreddit-1.2.5/src/sreddit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2021-10-26 20:22:41.000000 sreddit-1.2.5/src/sreddit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-26 20:22:41.000000 sreddit-1.2.5/src/sreddit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2021-10-26 20:22:41.000000 sreddit-1.2.5/src/sreddit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2021-10-26 20:22:41.000000 sreddit-1.2.5/src/sreddit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 21:13:00.104478 sreddit-1.2.6/
+-rw-rw-rw-   0        0        0      402 2023-07-02 21:13:00.104478 sreddit-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-07-02 21:13:00.106470 sreddit-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-07-02 21:07:01.000000 sreddit-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 21:13:00.086472 sreddit-1.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 21:13:00.102471 sreddit-1.2.6/src/sreddit.egg-info/
+-rw-rw-rw-   0        0        0      402 2023-07-02 21:13:00.000000 sreddit-1.2.6/src/sreddit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-02 21:13:00.000000 sreddit-1.2.6/src/sreddit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 21:13:00.000000 sreddit-1.2.6/src/sreddit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-02 21:13:00.000000 sreddit-1.2.6/src/sreddit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 21:13:00.000000 sreddit-1.2.6/src/sreddit.egg-info/top_level.txt
```

### Comparing `sreddit-1.2.5/setup.cfg` & `sreddit-1.2.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7265 6464 6974 0d0a 7665 7273   = sreddit..vers
-00000020: 696f 6e20 3d20 312e 322e 350d 0a61 7574  ion = 1.2.5..aut
-00000030: 686f 7220 3d20 4d61 6e64 7943 7962 6572  hor = MandyCyber
-00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
-00000050: 200d 0a64 6573 6372 6970 7469 6f6e 203d   ..description =
-00000060: 2057 6562 2073 6372 6170 6572 2066 6f72   Web scraper for
-00000070: 2073 7562 7265 6464 6974 730d 0a6c 6f6e   subreddits..lon
-00000080: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
-00000090: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
-000000a0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000b0: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-000000c0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-000000d0: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-000000e0: 7468 7562 2e63 6f6d 2f4d 616e 6479 2d63  thub.com/Mandy-c
-000000f0: 7962 6572 2f53 7562 5265 6464 6974 5363  yber/SubRedditSc
-00000100: 7261 7065 720d 0a63 6c61 7373 6966 6965  raper..classifie
-00000110: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
-00000120: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000130: 5079 7468 6f6e 203a 3a20 330d 0a09 4c69  Python :: 3...Li
-00000140: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-00000150: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
-00000160: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
-00000170: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000180: 6465 7065 6e64 656e 740d 0a0d 0a5b 6f70  dependent....[op
-00000190: 7469 6f6e 735d 0d0a 7061 636b 6167 655f  tions]..package_
-000001a0: 6469 7220 3d20 0d0a 093d 2073 7263 0d0a  dir = ...= src..
-000001b0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
-000001c0: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-000001d0: 6573 203d 200d 0a09 7365 6c65 6e69 756d  es = ...selenium
-000001e0: 0d0a 0974 696d 650d 0a09 6765 745f 6368  ...time...get_ch
-000001f0: 726f 6d65 5f64 7269 7665 720d 0a70 7974  rome_driver..pyt
-00000200: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-00000210: 3d33 2e36 0d0a 0d0a 5b6f 7074 696f 6e73  =3.6....[options
-00000220: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-00000230: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-00000240: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000250: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000260: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000020: 696f 6e20 3d20 312e 322e 360d 0a61 7574  ion = 1.2.6..aut
+00000030: 686f 7220 3d20 4d61 6e64 792d 6379 6265  hor = Mandy-cybe
+00000040: 720d 0a61 7574 686f 725f 656d 6169 6c20  r..author_email 
+00000050: 3d20 0d0a 6465 7363 7269 7074 696f 6e20  = ..description 
+00000060: 3d20 5765 6220 7363 7261 7065 7220 666f  = Web scraper fo
+00000070: 7220 7375 6272 6564 6469 7473 0d0a 6c6f  r subreddits..lo
+00000080: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
+00000090: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
+000000a0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000b0: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+000000c0: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
+000000d0: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
+000000e0: 6974 6875 622e 636f 6d2f 4d61 6e64 792d  ithub.com/Mandy-
+000000f0: 6379 6265 722f 5375 6252 6564 6469 7453  cyber/SubRedditS
+00000100: 6372 6170 6572 0d0a 636c 6173 7369 6669  craper..classifi
+00000110: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
+00000120: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000130: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
+00000140: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000150: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+00000160: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
+00000170: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+00000180: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
+00000190: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
+000001a0: 5f64 6972 203d 200d 0a09 3d20 7372 630d  _dir = ...= src.
+000001b0: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+000001c0: 3a0d 0a69 6e73 7461 6c6c 5f72 6571 7569  :..install_requi
+000001d0: 7265 7320 3d20 0d0a 0973 656c 656e 6975  res = ...seleniu
+000001e0: 6d0d 0a09 7469 6d65 0d0a 0967 6574 5f63  m...time...get_c
+000001f0: 6872 6f6d 655f 6472 6976 6572 0d0a 7079  hrome_driver..py
+00000200: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000210: 3e3d 332e 360d 0a0d 0a5b 6f70 7469 6f6e  >=3.6....[option
+00000220: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000230: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+00000240: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+00000250: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+00000260: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

