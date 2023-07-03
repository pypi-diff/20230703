# Comparing `tmp/otel-extensions-0.2.4.tar.gz` & `tmp/otel-extensions-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otel-extensions-0.2.4.tar", last modified: Wed Mar 15 22:18:37 2023, max compression
+gzip compressed data, was "otel-extensions-0.2.5.tar", last modified: Mon Jul  3 16:53:01 2023, max compression
```

## Comparing `otel-extensions-0.2.4.tar` & `otel-extensions-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 22:18:37.038624 otel-extensions-0.2.4/
--rw-rw-rw-   0        0        0    11558 2022-05-05 22:58:35.000000 otel-extensions-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     6753 2023-03-15 22:18:37.040635 otel-extensions-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     5491 2023-01-03 22:31:31.000000 otel-extensions-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-15 22:18:36.987642 otel-extensions-0.2.4/otel_extensions/
--rw-rw-rw-   0        0        0    11609 2023-03-15 22:17:36.000000 otel-extensions-0.2.4/otel_extensions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-15 22:18:37.031625 otel-extensions-0.2.4/otel_extensions.egg-info/
--rw-rw-rw-   0        0        0     6753 2023-03-15 22:18:36.000000 otel-extensions-0.2.4/otel_extensions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-03-15 22:18:36.000000 otel-extensions-0.2.4/otel_extensions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 22:18:36.000000 otel-extensions-0.2.4/otel_extensions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-03-15 22:18:36.000000 otel-extensions-0.2.4/otel_extensions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-15 22:18:36.000000 otel-extensions-0.2.4/otel_extensions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-03-15 22:18:36.000000 otel-extensions-0.2.4/otel_extensions.egg-info/zip-safe
--rw-rw-rw-   0        0        0      165 2022-05-07 00:16:58.000000 otel-extensions-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0     2408 2023-03-15 22:18:37.043628 otel-extensions-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0       66 2022-05-07 00:04:40.000000 otel-extensions-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:53:01.494428 otel-extensions-0.2.5/
+-rw-rw-rw-   0        0        0    11558 2022-05-05 22:58:35.000000 otel-extensions-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     6753 2023-07-03 16:53:01.495428 otel-extensions-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5491 2023-01-03 22:31:31.000000 otel-extensions-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 16:53:01.476428 otel-extensions-0.2.5/otel_extensions/
+-rw-rw-rw-   0        0        0    11609 2023-03-15 22:17:36.000000 otel-extensions-0.2.5/otel_extensions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:53:01.492429 otel-extensions-0.2.5/otel_extensions.egg-info/
+-rw-rw-rw-   0        0        0     6753 2023-07-03 16:53:01.000000 otel-extensions-0.2.5/otel_extensions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-07-03 16:53:01.000000 otel-extensions-0.2.5/otel_extensions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 16:53:01.000000 otel-extensions-0.2.5/otel_extensions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-03 16:53:01.000000 otel-extensions-0.2.5/otel_extensions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-03 16:53:01.000000 otel-extensions-0.2.5/otel_extensions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-03 16:53:01.000000 otel-extensions-0.2.5/otel_extensions.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      165 2022-05-07 00:16:58.000000 otel-extensions-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0     2413 2023-07-03 16:53:01.497428 otel-extensions-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0       66 2022-05-07 00:04:40.000000 otel-extensions-0.2.5/setup.py
```

### Comparing `otel-extensions-0.2.4/LICENSE` & `otel-extensions-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `otel-extensions-0.2.4/PKG-INFO` & `otel-extensions-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otel-extensions
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python extensions for OpenTelemetry
 Home-page: https://github.com/s4v4g3/otel-extensions-python
 Maintainer: Joe Savage
 Maintainer-email: joe.savage@gmail.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/s4v4g3/otel-extensions-python
 Project-URL: Tracker, https://github.com/s4v4g3/otel-extensions-python/issues
```

### Comparing `otel-extensions-0.2.4/README.md` & `otel-extensions-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `otel-extensions-0.2.4/otel_extensions/__init__.py` & `otel-extensions-0.2.5/otel_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `otel-extensions-0.2.4/otel_extensions.egg-info/PKG-INFO` & `otel-extensions-0.2.5/otel_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otel-extensions
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python extensions for OpenTelemetry
 Home-page: https://github.com/s4v4g3/otel-extensions-python
 Maintainer: Joe Savage
 Maintainer-email: joe.savage@gmail.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/s4v4g3/otel-extensions-python
 Project-URL: Tracker, https://github.com/s4v4g3/otel-extensions-python/issues
```

### Comparing `otel-extensions-0.2.4/setup.cfg` & `otel-extensions-0.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 6f6d 2f73 3476 3467 332f 6f74 656c 2d65  om/s4v4g3/otel-e
 000000d0: 7874 656e 7369 6f6e 732d 7079 7468 6f6e  xtensions-python
 000000e0: 0d0a 6d61 696e 7461 696e 6572 203d 204a  ..maintainer = J
 000000f0: 6f65 2053 6176 6167 650d 0a6d 6169 6e74  oe Savage..maint
 00000100: 6169 6e65 725f 656d 6169 6c20 3d20 6a6f  ainer_email = jo
 00000110: 652e 7361 7661 6765 4067 6d61 696c 2e63  e.savage@gmail.c
 00000120: 6f6d 0d0a 7665 7273 696f 6e20 3d20 302e  om..version = 0.
-00000130: 322e 340d 0a6c 6963 656e 7365 203d 2041  2.4..license = A
+00000130: 322e 350d 0a6c 6963 656e 7365 203d 2041  2.5..license = A
 00000140: 7061 6368 652d 322e 300d 0a6c 6963 656e  pache-2.0..licen
 00000150: 7365 5f66 696c 6520 3d20 4c49 4345 4e53  se_file = LICENS
 00000160: 450d 0a70 6c61 7466 6f72 6d73 203d 2061  E..platforms = a
 00000170: 6e79 0d0a 636c 6173 7369 6669 6572 7320  ny..classifiers 
 00000180: 3d20 0d0a 0949 6e74 656e 6465 6420 4175  = ...Intended Au
 00000190: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
 000001a0: 7065 7273 0d0a 094c 6963 656e 7365 203a  pers...License :
@@ -70,82 +70,82 @@
 00000450: 656e 7369 6f6e 732d 7079 7468 6f6e 2f69  ensions-python/i
 00000460: 7373 7565 730d 0a0d 0a5b 6f70 7469 6f6e  ssues....[option
 00000470: 735d 0d0a 7061 636b 6167 6573 203d 2066  s]..packages = f
 00000480: 696e 643a 0d0a 696e 7374 616c 6c5f 7265  ind:..install_re
 00000490: 7175 6972 6573 203d 200d 0a09 6f70 656e  quires = ...open
 000004a0: 7465 6c65 6d65 7472 792d 6170 690d 0a09  telemetry-api...
 000004b0: 6f70 656e 7465 6c65 6d65 7472 792d 7364  opentelemetry-sd
-000004c0: 6b0d 0a09 7079 6461 6e74 6963 0d0a 7079  k...pydantic..py
-000004d0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-000004e0: 3e3d 332e 360d 0a7a 6970 5f73 6166 6520  >=3.6..zip_safe 
-000004f0: 3d20 5472 7565 0d0a 0d0a 5b6f 7074 696f  = True....[optio
-00000500: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
-00000510: 5d0d 0a65 7863 6c75 6465 203d 200d 0a09  ]..exclude = ...
-00000520: 6578 616d 706c 650d 0a09 7465 7374 730d  example...tests.
-00000530: 0a09 746f 6f6c 730d 0a0d 0a5b 7364 6973  ..tools....[sdis
-00000540: 745d 0d0a 666f 726d 6174 7320 3d20 677a  t]..formats = gz
-00000550: 7461 720d 0a0d 0a5b 6264 6973 745f 7768  tar....[bdist_wh
-00000560: 6565 6c5d 0d0a 756e 6976 6572 7361 6c20  eel]..universal 
-00000570: 3d20 7472 7565 0d0a 0d0a 5b66 6c61 6b65  = true....[flake
-00000580: 385d 0d0a 6d61 782d 6c69 6e65 2d6c 656e  8]..max-line-len
-00000590: 6774 6820 3d20 3939 0d0a 0d0a 5b63 6f76  gth = 99....[cov
-000005a0: 6572 6167 653a 7265 706f 7274 5d0d 0a66  erage:report]..f
-000005b0: 6169 6c5f 756e 6465 7220 3d20 3130 300d  ail_under = 100.
-000005c0: 0a73 6b69 705f 636f 7665 7265 6420 3d20  .skip_covered = 
-000005d0: 7472 7565 0d0a 7368 6f77 5f6d 6973 7369  true..show_missi
-000005e0: 6e67 203d 2074 7275 650d 0a6f 6d69 7420  ng = true..omit 
-000005f0: 3d20 0d0a 0965 7861 6d70 6c65 2f65 7861  = ...example/exa
-00000600: 6d70 6c65 2e70 790d 0a0d 0a5b 636f 7665  mple.py....[cove
-00000610: 7261 6765 3a68 746d 6c5d 0d0a 7368 6f77  rage:html]..show
-00000620: 5f63 6f6e 7465 7874 7320 3d20 5472 7565  _contexts = True
-00000630: 0d0a 736b 6970 5f63 6f76 6572 6564 203d  ..skip_covered =
-00000640: 2046 616c 7365 0d0a 736b 6970 5f65 6d70   False..skip_emp
-00000650: 7479 203d 2046 616c 7365 0d0a 0d0a 5b63  ty = False....[c
-00000660: 6f76 6572 6167 653a 7061 7468 735d 0d0a  overage:paths]..
-00000670: 736f 7572 6365 203d 200d 0a09 7372 630d  source = ...src.
-00000680: 0a09 2e74 6f78 2a2f 2a2f 6c69 622f 7079  ...tox*/*/lib/py
-00000690: 7468 6f6e 2a2f 7369 7465 2d70 6163 6b61  thon*/site-packa
-000006a0: 6765 730d 0a09 2e74 6f78 2a2f 7079 7079  ges....tox*/pypy
-000006b0: 2a2f 7369 7465 2d70 6163 6b61 6765 730d  */site-packages.
-000006c0: 0a09 2e74 6f78 2a5c 2a5c 4c69 625c 7369  ...tox*\*\Lib\si
-000006d0: 7465 2d70 6163 6b61 6765 735c 0d0a 092a  te-packages\...*
-000006e0: 2f73 7263 0d0a 092a 5c73 7263 0d0a 0d0a  /src...*\src....
-000006f0: 5b74 6f6f 6c3a 7079 7465 7374 5d0d 0a61  [tool:pytest]..a
-00000700: 6464 6f70 7473 203d 202d 7261 202d 2d73  ddopts = -ra --s
-00000710: 686f 776c 6f63 616c 7320 2d76 760d 0a74  howlocals -vv..t
-00000720: 6573 7470 6174 6873 203d 2074 6573 7473  estpaths = tests
-00000730: 0d0a 7866 6169 6c5f 7374 7269 6374 203d  ..xfail_strict =
-00000740: 2054 7275 650d 0a6a 756e 6974 5f66 616d   True..junit_fam
-00000750: 696c 7920 3d20 7875 6e69 7432 0d0a 0d0a  ily = xunit2....
-00000760: 5b6d 7970 795d 0d0a 7079 7468 6f6e 5f76  [mypy]..python_v
-00000770: 6572 7369 6f6e 203d 2033 2e36 0d0a 6469  ersion = 3.6..di
-00000780: 7361 6c6c 6f77 5f61 6e79 5f67 656e 6572  sallow_any_gener
-00000790: 6963 7320 3d20 5472 7565 0d0a 6469 7361  ics = True..disa
-000007a0: 6c6c 6f77 5f73 7562 636c 6173 7369 6e67  llow_subclassing
-000007b0: 5f61 6e79 203d 2054 7275 650d 0a64 6973  _any = True..dis
-000007c0: 616c 6c6f 775f 756e 7479 7065 645f 6361  allow_untyped_ca
-000007d0: 6c6c 7320 3d20 5472 7565 0d0a 6469 7361  lls = True..disa
-000007e0: 6c6c 6f77 5f75 6e74 7970 6564 5f64 6566  llow_untyped_def
-000007f0: 7320 3d20 5472 7565 0d0a 6469 7361 6c6c  s = True..disall
-00000800: 6f77 5f69 6e63 6f6d 706c 6574 655f 6465  ow_incomplete_de
-00000810: 6673 203d 2054 7275 650d 0a64 6973 616c  fs = True..disal
-00000820: 6c6f 775f 756e 7479 7065 645f 6465 636f  low_untyped_deco
-00000830: 7261 746f 7273 203d 2054 7275 650d 0a73  rators = True..s
-00000840: 686f 775f 6572 726f 725f 636f 6465 7320  how_error_codes 
-00000850: 3d20 5472 7565 0d0a 6e6f 5f69 6d70 6c69  = True..no_impli
-00000860: 6369 745f 6f70 7469 6f6e 616c 203d 2054  cit_optional = T
-00000870: 7275 650d 0a77 6172 6e5f 7265 6475 6e64  rue..warn_redund
-00000880: 616e 745f 6361 7374 7320 3d20 5472 7565  ant_casts = True
-00000890: 0d0a 7761 726e 5f75 6e75 7365 645f 6967  ..warn_unused_ig
-000008a0: 6e6f 7265 7320 3d20 4661 6c73 650d 0a77  nores = False..w
-000008b0: 6172 6e5f 6e6f 5f72 6574 7572 6e20 3d20  arn_no_return = 
-000008c0: 5472 7565 0d0a 7761 726e 5f72 6574 7572  True..warn_retur
-000008d0: 6e5f 616e 7920 3d20 5472 7565 0d0a 696d  n_any = True..im
-000008e0: 706c 6963 6974 5f72 6565 7870 6f72 7420  plicit_reexport 
-000008f0: 3d20 4661 6c73 650d 0a73 7472 6963 745f  = False..strict_
-00000900: 6571 7561 6c69 7479 203d 2054 7275 650d  equality = True.
-00000910: 0a77 6172 6e5f 756e 7573 6564 5f63 6f6e  .warn_unused_con
-00000920: 6669 6773 203d 2054 7275 650d 0a70 7265  figs = True..pre
-00000930: 7474 7920 3d20 5472 7565 0d0a 0d0a 5b65  tty = True....[e
-00000940: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000950: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000960: 203d 2030 0d0a 0d0a                       = 0....
+000004c0: 6b0d 0a09 7079 6461 6e74 6963 3d3d 312e  k...pydantic==1.
+000004d0: 2a0d 0a70 7974 686f 6e5f 7265 7175 6972  *..python_requir
+000004e0: 6573 203d 203e 3d33 2e36 0d0a 7a69 705f  es = >=3.6..zip_
+000004f0: 7361 6665 203d 2054 7275 650d 0a0d 0a5b  safe = True....[
+00000500: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+00000510: 2e66 696e 645d 0d0a 6578 636c 7564 6520  .find]..exclude 
+00000520: 3d20 0d0a 0965 7861 6d70 6c65 0d0a 0974  = ...example...t
+00000530: 6573 7473 0d0a 0974 6f6f 6c73 0d0a 0d0a  ests...tools....
+00000540: 5b73 6469 7374 5d0d 0a66 6f72 6d61 7473  [sdist]..formats
+00000550: 203d 2067 7a74 6172 0d0a 0d0a 5b62 6469   = gztar....[bdi
+00000560: 7374 5f77 6865 656c 5d0d 0a75 6e69 7665  st_wheel]..unive
+00000570: 7273 616c 203d 2074 7275 650d 0a0d 0a5b  rsal = true....[
+00000580: 666c 616b 6538 5d0d 0a6d 6178 2d6c 696e  flake8]..max-lin
+00000590: 652d 6c65 6e67 7468 203d 2039 390d 0a0d  e-length = 99...
+000005a0: 0a5b 636f 7665 7261 6765 3a72 6570 6f72  .[coverage:repor
+000005b0: 745d 0d0a 6661 696c 5f75 6e64 6572 203d  t]..fail_under =
+000005c0: 2031 3030 0d0a 736b 6970 5f63 6f76 6572   100..skip_cover
+000005d0: 6564 203d 2074 7275 650d 0a73 686f 775f  ed = true..show_
+000005e0: 6d69 7373 696e 6720 3d20 7472 7565 0d0a  missing = true..
+000005f0: 6f6d 6974 203d 200d 0a09 6578 616d 706c  omit = ...exampl
+00000600: 652f 6578 616d 706c 652e 7079 0d0a 0d0a  e/example.py....
+00000610: 5b63 6f76 6572 6167 653a 6874 6d6c 5d0d  [coverage:html].
+00000620: 0a73 686f 775f 636f 6e74 6578 7473 203d  .show_contexts =
+00000630: 2054 7275 650d 0a73 6b69 705f 636f 7665   True..skip_cove
+00000640: 7265 6420 3d20 4661 6c73 650d 0a73 6b69  red = False..ski
+00000650: 705f 656d 7074 7920 3d20 4661 6c73 650d  p_empty = False.
+00000660: 0a0d 0a5b 636f 7665 7261 6765 3a70 6174  ...[coverage:pat
+00000670: 6873 5d0d 0a73 6f75 7263 6520 3d20 0d0a  hs]..source = ..
+00000680: 0973 7263 0d0a 092e 746f 782a 2f2a 2f6c  .src....tox*/*/l
+00000690: 6962 2f70 7974 686f 6e2a 2f73 6974 652d  ib/python*/site-
+000006a0: 7061 636b 6167 6573 0d0a 092e 746f 782a  packages....tox*
+000006b0: 2f70 7970 792a 2f73 6974 652d 7061 636b  /pypy*/site-pack
+000006c0: 6167 6573 0d0a 092e 746f 782a 5c2a 5c4c  ages....tox*\*\L
+000006d0: 6962 5c73 6974 652d 7061 636b 6167 6573  ib\site-packages
+000006e0: 5c0d 0a09 2a2f 7372 630d 0a09 2a5c 7372  \...*/src...*\sr
+000006f0: 630d 0a0d 0a5b 746f 6f6c 3a70 7974 6573  c....[tool:pytes
+00000700: 745d 0d0a 6164 646f 7074 7320 3d20 2d72  t]..addopts = -r
+00000710: 6120 2d2d 7368 6f77 6c6f 6361 6c73 202d  a --showlocals -
+00000720: 7676 0d0a 7465 7374 7061 7468 7320 3d20  vv..testpaths = 
+00000730: 7465 7374 730d 0a78 6661 696c 5f73 7472  tests..xfail_str
+00000740: 6963 7420 3d20 5472 7565 0d0a 6a75 6e69  ict = True..juni
+00000750: 745f 6661 6d69 6c79 203d 2078 756e 6974  t_family = xunit
+00000760: 320d 0a0d 0a5b 6d79 7079 5d0d 0a70 7974  2....[mypy]..pyt
+00000770: 686f 6e5f 7665 7273 696f 6e20 3d20 332e  hon_version = 3.
+00000780: 360d 0a64 6973 616c 6c6f 775f 616e 795f  6..disallow_any_
+00000790: 6765 6e65 7269 6373 203d 2054 7275 650d  generics = True.
+000007a0: 0a64 6973 616c 6c6f 775f 7375 6263 6c61  .disallow_subcla
+000007b0: 7373 696e 675f 616e 7920 3d20 5472 7565  ssing_any = True
+000007c0: 0d0a 6469 7361 6c6c 6f77 5f75 6e74 7970  ..disallow_untyp
+000007d0: 6564 5f63 616c 6c73 203d 2054 7275 650d  ed_calls = True.
+000007e0: 0a64 6973 616c 6c6f 775f 756e 7479 7065  .disallow_untype
+000007f0: 645f 6465 6673 203d 2054 7275 650d 0a64  d_defs = True..d
+00000800: 6973 616c 6c6f 775f 696e 636f 6d70 6c65  isallow_incomple
+00000810: 7465 5f64 6566 7320 3d20 5472 7565 0d0a  te_defs = True..
+00000820: 6469 7361 6c6c 6f77 5f75 6e74 7970 6564  disallow_untyped
+00000830: 5f64 6563 6f72 6174 6f72 7320 3d20 5472  _decorators = Tr
+00000840: 7565 0d0a 7368 6f77 5f65 7272 6f72 5f63  ue..show_error_c
+00000850: 6f64 6573 203d 2054 7275 650d 0a6e 6f5f  odes = True..no_
+00000860: 696d 706c 6963 6974 5f6f 7074 696f 6e61  implicit_optiona
+00000870: 6c20 3d20 5472 7565 0d0a 7761 726e 5f72  l = True..warn_r
+00000880: 6564 756e 6461 6e74 5f63 6173 7473 203d  edundant_casts =
+00000890: 2054 7275 650d 0a77 6172 6e5f 756e 7573   True..warn_unus
+000008a0: 6564 5f69 676e 6f72 6573 203d 2046 616c  ed_ignores = Fal
+000008b0: 7365 0d0a 7761 726e 5f6e 6f5f 7265 7475  se..warn_no_retu
+000008c0: 726e 203d 2054 7275 650d 0a77 6172 6e5f  rn = True..warn_
+000008d0: 7265 7475 726e 5f61 6e79 203d 2054 7275  return_any = Tru
+000008e0: 650d 0a69 6d70 6c69 6369 745f 7265 6578  e..implicit_reex
+000008f0: 706f 7274 203d 2046 616c 7365 0d0a 7374  port = False..st
+00000900: 7269 6374 5f65 7175 616c 6974 7920 3d20  rict_equality = 
+00000910: 5472 7565 0d0a 7761 726e 5f75 6e75 7365  True..warn_unuse
+00000920: 645f 636f 6e66 6967 7320 3d20 5472 7565  d_configs = True
+00000930: 0d0a 7072 6574 7479 203d 2054 7275 650d  ..pretty = True.
+00000940: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000950: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000960: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

