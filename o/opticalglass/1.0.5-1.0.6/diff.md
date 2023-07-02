# Comparing `tmp/opticalglass-1.0.5.tar.gz` & `tmp/opticalglass-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opticalglass-1.0.5.tar", last modified: Mon May 15 18:06:56 2023, max compression
+gzip compressed data, was "opticalglass-1.0.6.tar", last modified: Wed Jun 14 23:12:37 2023, max compression
```

## Comparing `opticalglass-1.0.5.tar` & `opticalglass-1.0.6.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.629862 opticalglass-1.0.5/
--rw-r--r--   0 Mike       (501) staff       (20)      409 2022-10-12 21:26:35.000000 opticalglass-1.0.5/.gitignore
--rw-r--r--   0 Mike       (501) staff       (20)      511 2022-10-12 18:00:24.000000 opticalglass-1.0.5/.readthedocs.yaml
--rw-r--r--   0 Mike       (501) staff       (20)       82 2022-08-22 05:03:42.000000 opticalglass-1.0.5/AUTHORS.rst
--rw-r--r--   0 Mike       (501) staff       (20)     1937 2023-05-15 17:59:41.000000 opticalglass-1.0.5/CHANGELOG.rst
--rw-r--r--   0 Mike       (501) staff       (20)     1530 2022-05-27 23:29:36.000000 opticalglass-1.0.5/LICENSE
--rw-r--r--   0 Mike       (501) staff       (20)     2135 2023-05-15 18:06:56.630163 opticalglass-1.0.5/PKG-INFO
--rw-r--r--   0 Mike       (501) staff       (20)     1405 2023-05-15 18:04:09.000000 opticalglass-1.0.5/README.rst
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.450422 opticalglass-1.0.5/docs/
--rw-r--r--   0 Mike       (501) staff       (20)      580 2022-08-22 05:07:24.000000 opticalglass-1.0.5/docs/Makefile
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.456154 opticalglass-1.0.5/docs/OG_Pandas_intro/
--rw-r--r--   0 Mike       (501) staff       (20)    12795 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Pandas_intro/OG_Pandas_intro.rst
--rw-r--r--   0 Mike       (501) staff       (20)     7299 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Pandas_intro/output_22_1.png
--rw-r--r--   0 Mike       (501) staff       (20)    61882 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Pandas_intro/output_24_1.png
--rw-r--r--   0 Mike       (501) staff       (20)    10963 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Pandas_intro/output_26_1.png
--rw-r--r--   0 Mike       (501) staff       (20)     6723 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Pandas_intro/output_38_1.png
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.462107 opticalglass-1.0.5/docs/OG_Quickstart/
--rw-r--r--   0 Mike       (501) staff       (20)     4552 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Quickstart/OG_Quickstart.rst
--rw-r--r--   0 Mike       (501) staff       (20)     9253 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Quickstart/output_16_1.png
--rw-r--r--   0 Mike       (501) staff       (20)     9253 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Quickstart/output_17_1.png
--rw-r--r--   0 Mike       (501) staff       (20)    42503 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Quickstart/output_19_0.png
--rw-r--r--   0 Mike       (501) staff       (20)     7172 2022-05-27 23:29:36.000000 opticalglass-1.0.5/docs/OG_Quickstart/output_28_1.png
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.488668 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/
--rw-------   0 Mike       (501) staff       (20)     7402 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/OG_RefractiveIndexInfo.rst
--rw-r--r--   0 Mike       (501) staff       (20)   408002 2022-05-28 05:13:35.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_copy_data_link.png
--rw-r--r--   0 Mike       (501) staff       (20)   119917 2022-05-28 05:12:53.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_data_links.png
--rw-r--r--   0 Mike       (501) staff       (20)   222578 2022-05-28 05:20:25.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_rindexdata.png
--rw-r--r--   0 Mike       (501) staff       (20)   130825 2022-05-28 05:20:03.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_top.png
--rw-------   0 Mike       (501) staff       (20)    13628 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_19_1.png
--rw-------   0 Mike       (501) staff       (20)    10140 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_21_1.png
--rw-------   0 Mike       (501) staff       (20)    13000 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_23_1.png
--rw-------   0 Mike       (501) staff       (20)    16537 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_26_1.png
--rw-------   0 Mike       (501) staff       (20)    12405 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_29_1.png
--rw-------   0 Mike       (501) staff       (20)    11717 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_33_1.png
--rw-------   0 Mike       (501) staff       (20)    13641 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_36_1.png
--rw-------   0 Mike       (501) staff       (20)    32051 2022-05-29 17:40:46.000000 opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_9_1.png
--rw-r--r--   0 Mike       (501) staff       (20)     3842 2022-08-22 05:07:34.000000 opticalglass-1.0.5/docs/README.rst
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.529918 opticalglass-1.0.5/docs/_images/
--rw-r--r--   0 Mike       (501) staff       (20)   738660 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/BuchdahlCoefficients.png
--rw-r--r--   0 Mike       (501) staff       (20)   726663 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/BuchdahlDispersion.png
--rw-r--r--   0 Mike       (501) staff       (20)   762462 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/CatalogSelection.png
--rw-r--r--   0 Mike       (501) staff       (20)   224020 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/GlassMap.png
--rw-r--r--   0 Mike       (501) staff       (20)    11091 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/IndexVsWvl.png
--rw-r--r--   0 Mike       (501) staff       (20)   765658 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/PartialDispersion.png
--rw-r--r--   0 Mike       (501) staff       (20)   244335 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/PartialMap.png
--rw-r--r--   0 Mike       (501) staff       (20)   840039 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/RefractiveIndex.png
--rw-r--r--   0 Mike       (501) staff       (20)    42333 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/_images/output_11_0.png
--rw-r--r--   0 Mike       (501) staff       (20)       41 2022-08-22 04:12:02.000000 opticalglass-1.0.5/docs/authors.rst
--rw-r--r--   0 Mike       (501) staff       (20)       43 2022-08-22 04:12:02.000000 opticalglass-1.0.5/docs/changelog.rst
--rw-r--r--   0 Mike       (501) staff       (20)     6569 2023-05-15 17:57:53.000000 opticalglass-1.0.5/docs/conf.py
--rw-r--r--   0 Mike       (501) staff       (20)      737 2022-08-22 05:06:20.000000 opticalglass-1.0.5/docs/index.rst
--rw-r--r--   0 Mike       (501) staff       (20)       63 2022-08-22 05:06:31.000000 opticalglass-1.0.5/docs/license.rst
--rw-r--r--   0 Mike       (501) staff       (20)      787 2021-09-21 20:40:59.000000 opticalglass-1.0.5/docs/make.bat
--rw-r--r--   0 Mike       (501) staff       (20)     2362 2022-08-24 19:03:29.000000 opticalglass-1.0.5/docs/opticalglass.rst
--rw-r--r--   0 Mike       (501) staff       (20)      361 2022-08-25 21:42:02.000000 opticalglass-1.0.5/docs/requirements.txt
--rw-r--r--   0 Mike       (501) staff       (20)      346 2022-08-24 19:03:29.000000 opticalglass-1.0.5/pyproject.toml
--rw-r--r--   0 Mike       (501) staff       (20)     1566 2023-05-15 18:06:56.631671 opticalglass-1.0.5/setup.cfg
--rw-r--r--   0 Mike       (501) staff       (20)      724 2022-10-12 17:49:38.000000 opticalglass-1.0.5/setup.py
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.431683 opticalglass-1.0.5/src/
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.550873 opticalglass-1.0.5/src/opticalglass/
--rw-r--r--   0 Mike       (501) staff       (20)     2228 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/__init__.py
--rwxr-xr-x   0 Mike       (501) staff       (20)     5766 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/buchdahl.py
--rwxr-xr-x   0 Mike       (501) staff       (20)     1851 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/caselessDictionary.py
--rw-r--r--   0 Mike       (501) staff       (20)     2804 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/cdgm.py
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.614461 opticalglass-1.0.5/src/opticalglass/data/
--rw-r--r--   0 Mike       (501) staff       (20)   674304 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/CDGM.xls
--rw-r--r--   0 Mike       (501) staff       (20)   454924 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/HIKARI.xlsx
--rw-r--r--   0 Mike       (501) staff       (20)   731648 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/HIKARI_prev.xls
--rw-r--r--   0 Mike       (501) staff       (20)  1234441 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/HOYA.xlsx
--rw-r--r--   0 Mike       (501) staff       (20)  1269672 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/HOYA_prev.xlsx
--rw-r--r--   0 Mike       (501) staff       (20)   252743 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/OHARA.xlsx
--rw-r--r--   0 Mike       (501) staff       (20)   265141 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/OHARA_prev.xlsx
--rw-r--r--   0 Mike       (501) staff       (20)   450048 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/SCHOTT.xls
--rw-r--r--   0 Mike       (501) staff       (20)   449024 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/SCHOTT_prev.xls
--rw-r--r--   0 Mike       (501) staff       (20)   160596 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/SUMITA.xlsx
--rw-r--r--   0 Mike       (501) staff       (20)    58113 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/robb1983_data_final.txt
--rw-r--r--   0 Mike       (501) staff       (20)      165 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/data/~$HIKARI.xlsx
--rw-r--r--   0 Mike       (501) staff       (20)    27474 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/glass.py
--rw-r--r--   0 Mike       (501) staff       (20)      834 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/glasserror.py
--rw-r--r--   0 Mike       (501) staff       (20)     4040 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/glassfactory.py
--rwxr-xr-x   0 Mike       (501) staff       (20)    15776 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/glassmap.py
--rw-r--r--   0 Mike       (501) staff       (20)    10922 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/glassmapviewer.py
--rw-r--r--   0 Mike       (501) staff       (20)     2283 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/glasspolygons.py
--rwxr-xr-x   0 Mike       (501) staff       (20)     3525 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/hikari.py
--rw-r--r--   0 Mike       (501) staff       (20)     3021 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/hoya.py
--rw-r--r--   0 Mike       (501) staff       (20)     2211 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/modelglass.py
--rw-r--r--   0 Mike       (501) staff       (20)     2921 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/ohara.py
--rw-r--r--   0 Mike       (501) staff       (20)     2919 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/openpyxl_script.py
--rw-r--r--   0 Mike       (501) staff       (20)     7531 2023-01-01 20:40:31.000000 opticalglass-1.0.5/src/opticalglass/optical_glass_agf_class.py
--rw-r--r--   0 Mike       (501) staff       (20)     7638 2023-05-15 05:55:23.000000 opticalglass-1.0.5/src/opticalglass/opticalmedium.py
--rw-r--r--   0 Mike       (501) staff       (20)    14320 2023-05-15 06:40:19.000000 opticalglass-1.0.5/src/opticalglass/rindexinfo.py
--rw-r--r--   0 Mike       (501) staff       (20)     3163 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/schott.py
--rw-r--r--   0 Mike       (501) staff       (20)     3783 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/spectral_lines.py
--rwxr-xr-x   0 Mike       (501) staff       (20)     3223 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/sumita.py
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.627024 opticalglass-1.0.5/src/opticalglass/test/
--rwxr-xr-x   0 Mike       (501) staff       (20)      879 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/cmd_line_example.py
--rw-r--r--   0 Mike       (501) staff       (20)     1969 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_cdgm.py
--rw-r--r--   0 Mike       (501) staff       (20)     3050 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_glassfactory.py
--rwxr-xr-x   0 Mike       (501) staff       (20)     2200 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_hikari.py
--rw-r--r--   0 Mike       (501) staff       (20)     2060 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_hoya.py
--rw-r--r--   0 Mike       (501) staff       (20)     2071 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_ohara.py
--rw-r--r--   0 Mike       (501) staff       (20)     1814 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_schott.py
--rwxr-xr-x   0 Mike       (501) staff       (20)     2452 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_sumita.py
--rw-r--r--   0 Mike       (501) staff       (20)     3767 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/test_transmission.py
--rw-r--r--   0 Mike       (501) staff       (20)     1193 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/test/util.py
--rwxr-xr-x   0 Mike       (501) staff       (20)     1941 2022-08-24 19:03:29.000000 opticalglass-1.0.5/src/opticalglass/util.py
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.554262 opticalglass-1.0.5/src/opticalglass.egg-info/
--rw-r--r--   0 Mike       (501) staff       (20)     2135 2023-05-15 18:06:56.000000 opticalglass-1.0.5/src/opticalglass.egg-info/PKG-INFO
--rw-r--r--   0 Mike       (501) staff       (20)     3324 2023-05-15 18:06:56.000000 opticalglass-1.0.5/src/opticalglass.egg-info/SOURCES.txt
--rw-r--r--   0 Mike       (501) staff       (20)        1 2023-05-15 18:06:56.000000 opticalglass-1.0.5/src/opticalglass.egg-info/dependency_links.txt
--rw-r--r--   0 Mike       (501) staff       (20)       58 2023-05-15 18:06:56.000000 opticalglass-1.0.5/src/opticalglass.egg-info/entry_points.txt
--rw-r--r--   0 Mike       (501) staff       (20)        1 2022-08-23 03:14:07.000000 opticalglass-1.0.5/src/opticalglass.egg-info/not-zip-safe
--rw-r--r--   0 Mike       (501) staff       (20)      167 2023-05-15 18:06:56.000000 opticalglass-1.0.5/src/opticalglass.egg-info/requires.txt
--rw-r--r--   0 Mike       (501) staff       (20)       13 2023-05-15 18:06:56.000000 opticalglass-1.0.5/src/opticalglass.egg-info/top_level.txt
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-15 18:06:56.628398 opticalglass-1.0.5/update/
--rw-r--r--   0 Mike       (501) staff       (20)     1266 2019-01-17 05:29:49.000000 opticalglass-1.0.5/update/catupdate.py
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-06-14 23:12:37.304493 opticalglass-1.0.6/
+-rw-r--r--   0 Mike       (501) staff       (20)      409 2022-10-12 21:26:35.000000 opticalglass-1.0.6/.gitignore
+-rw-r--r--   0 Mike       (501) staff       (20)      512 2023-06-14 18:31:47.000000 opticalglass-1.0.6/.readthedocs.yaml
+-rw-r--r--   0 Mike       (501) staff       (20)       82 2022-08-22 05:03:42.000000 opticalglass-1.0.6/AUTHORS.rst
+-rw-r--r--   0 Mike       (501) staff       (20)     2037 2023-06-14 18:09:38.000000 opticalglass-1.0.6/CHANGELOG.rst
+-rw-r--r--   0 Mike       (501) staff       (20)     1530 2022-05-27 23:29:36.000000 opticalglass-1.0.6/LICENSE
+-rw-r--r--   0 Mike       (501) staff       (20)     2135 2023-06-14 23:12:37.304662 opticalglass-1.0.6/PKG-INFO
+-rw-r--r--   0 Mike       (501) staff       (20)     1405 2023-05-15 18:04:09.000000 opticalglass-1.0.6/README.rst
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-06-14 23:12:37.114484 opticalglass-1.0.6/docs/
+-rw-r--r--   0 Mike       (501) staff       (20)      580 2022-08-22 05:07:24.000000 opticalglass-1.0.6/docs/Makefile
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-06-14 23:12:37.120046 opticalglass-1.0.6/docs/OG_Pandas_intro/
+-rw-r--r--   0 Mike       (501) staff       (20)    12795 2022-05-27 23:29:36.000000 opticalglass-1.0.6/docs/OG_Pandas_intro/OG_Pandas_intro.rst
+-rw-r--r--   0 Mike       (501) staff       (20)     7299 2022-05-27 23:29:36.000000 opticalglass-1.0.6/docs/OG_Pandas_intro/output_22_1.png
+-rw-r--r--   0 Mike       (501) staff       (20)    61882 2022-05-27 23:29:36.000000 opticalglass-1.0.6/docs/OG_Pandas_intro/output_24_1.png
+-rw-r--r--   0 Mike       (501) staff       (20)    10963 2022-05-27 23:29:36.000000 opticalglass-1.0.6/docs/OG_Pandas_intro/output_26_1.png
+-rw-r--r--   0 Mike       (501) staff       (20)     6723 2022-05-27 23:29:36.000000 opticalglass-1.0.6/docs/OG_Pandas_intro/output_38_1.png
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-06-14 23:12:37.124586 opticalglass-1.0.6/docs/OG_Quickstart/
+-rw-r--r--   0 Mike       (501) staff       (20)     4552 2022-05-27 23:29:36.000000 opticalglass-1.0.6/docs/OG_Quickstart/OG_Quickstart.rst
+-rw-r--r--   0 Mike       (501) staff       (20)     9253 2022-05-27 23:29:36.000000 opticalglass-1.0.6/docs/OG_Quickstart/output_16_1.png
+-rw-r--r--   0 Mike       (501) staff       (20)     9253 2022-05-27 23:29:36.000000 opticalglass-1.0.6/docs/OG_Quickstart/output_17_1.png
+-rw-r--r--   0 Mike       (501) staff       (20)    42503 2022-05-27 23:29:36.000000 opticalglass-1.0.6/docs/OG_Quickstart/output_19_0.png
+-rw-r--r--   0 Mike       (501) staff       (20)     7172 2022-05-27 23:29:36.000000 opticalglass-1.0.6/docs/OG_Quickstart/output_28_1.png
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-06-14 23:12:37.150588 opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/
+-rw-------   0 Mike       (501) staff       (20)     7402 2022-05-29 17:40:46.000000 opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/OG_RefractiveIndexInfo.rst
+-rw-r--r--   0 Mike       (501) staff       (20)   408002 2022-05-28 05:13:35.000000 opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/RII_page_copy_data_link.png
+-rw-r--r--   0 Mike       (501) staff       (20)   119917 2022-05-28 05:12:53.000000 opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/RII_page_data_links.png
+-rw-r--r--   0 Mike       (501) staff       (20)   222578 2022-05-28 05:20:25.000000 opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/RII_page_rindexdata.png
+-rw-r--r--   0 Mike       (501) staff       (20)   130825 2022-05-28 05:20:03.000000 opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/RII_page_top.png
+-rw-------   0 Mike       (501) staff       (20)    13628 2022-05-29 17:40:46.000000 opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_19_1.png
+-rw-------   0 Mike       (501) staff       (20)    10140 2022-05-29 17:40:46.000000 opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_21_1.png
+-rw-------   0 Mike       (501) staff       (20)    13000 2022-05-29 17:40:46.000000 opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_23_1.png
+-rw-------   0 Mike       (501) staff       (20)    16537 2022-05-29 17:40:46.000000 opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_26_1.png
+-rw-------   0 Mike       (501) staff       (20)    12405 2022-05-29 17:40:46.000000 opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_29_1.png
+-rw-------   0 Mike       (501) staff       (20)    11717 2022-05-29 17:40:46.000000 opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_33_1.png
+-rw-------   0 Mike       (501) staff       (20)    13641 2022-05-29 17:40:46.000000 opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_36_1.png
+-rw-------   0 Mike       (501) staff       (20)    32051 2022-05-29 17:40:46.000000 opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_9_1.png
+-rw-r--r--   0 Mike       (501) staff       (20)     3842 2022-08-22 05:07:34.000000 opticalglass-1.0.6/docs/README.rst
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-06-14 23:12:37.207522 opticalglass-1.0.6/docs/_images/
+-rw-r--r--   0 Mike       (501) staff       (20)   738660 2021-09-21 20:40:59.000000 opticalglass-1.0.6/docs/_images/BuchdahlCoefficients.png
+-rw-r--r--   0 Mike       (501) staff       (20)   726663 2021-09-21 20:40:59.000000 opticalglass-1.0.6/docs/_images/BuchdahlDispersion.png
+-rw-r--r--   0 Mike       (501) staff       (20)   762462 2021-09-21 20:40:59.000000 opticalglass-1.0.6/docs/_images/CatalogSelection.png
+-rw-r--r--   0 Mike       (501) staff       (20)   224020 2021-09-21 20:40:59.000000 opticalglass-1.0.6/docs/_images/GlassMap.png
+-rw-r--r--   0 Mike       (501) staff       (20)    11091 2021-09-21 20:40:59.000000 opticalglass-1.0.6/docs/_images/IndexVsWvl.png
+-rw-r--r--   0 Mike       (501) staff       (20)   765658 2021-09-21 20:40:59.000000 opticalglass-1.0.6/docs/_images/PartialDispersion.png
+-rw-r--r--   0 Mike       (501) staff       (20)   244335 2021-09-21 20:40:59.000000 opticalglass-1.0.6/docs/_images/PartialMap.png
+-rw-r--r--   0 Mike       (501) staff       (20)   840039 2021-09-21 20:40:59.000000 opticalglass-1.0.6/docs/_images/RefractiveIndex.png
+-rw-r--r--   0 Mike       (501) staff       (20)    42333 2021-09-21 20:40:59.000000 opticalglass-1.0.6/docs/_images/output_11_0.png
+-rw-r--r--   0 Mike       (501) staff       (20)       41 2022-08-22 04:12:02.000000 opticalglass-1.0.6/docs/authors.rst
+-rw-r--r--   0 Mike       (501) staff       (20)       43 2022-08-22 04:12:02.000000 opticalglass-1.0.6/docs/changelog.rst
+-rw-r--r--   0 Mike       (501) staff       (20)     6567 2023-06-14 17:39:24.000000 opticalglass-1.0.6/docs/conf.py
+-rw-r--r--   0 Mike       (501) staff       (20)      737 2022-08-22 05:06:20.000000 opticalglass-1.0.6/docs/index.rst
+-rw-r--r--   0 Mike       (501) staff       (20)       63 2022-08-22 05:06:31.000000 opticalglass-1.0.6/docs/license.rst
+-rw-r--r--   0 Mike       (501) staff       (20)      787 2021-09-21 20:40:59.000000 opticalglass-1.0.6/docs/make.bat
+-rw-r--r--   0 Mike       (501) staff       (20)     2362 2022-08-24 19:03:29.000000 opticalglass-1.0.6/docs/opticalglass.rst
+-rw-r--r--   0 Mike       (501) staff       (20)      377 2023-06-14 21:32:19.000000 opticalglass-1.0.6/docs/requirements.txt
+-rw-r--r--   0 Mike       (501) staff       (20)      346 2022-08-24 19:03:29.000000 opticalglass-1.0.6/pyproject.toml
+-rw-r--r--   0 Mike       (501) staff       (20)     1567 2023-06-14 23:12:37.305929 opticalglass-1.0.6/setup.cfg
+-rw-r--r--   0 Mike       (501) staff       (20)      724 2022-10-12 17:49:38.000000 opticalglass-1.0.6/setup.py
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-06-14 23:12:37.099268 opticalglass-1.0.6/src/
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-06-14 23:12:37.228230 opticalglass-1.0.6/src/opticalglass/
+-rw-r--r--   0 Mike       (501) staff       (20)     2228 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/__init__.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)     5766 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/buchdahl.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)     1851 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/caselessDictionary.py
+-rw-r--r--   0 Mike       (501) staff       (20)     2804 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/cdgm.py
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-06-14 23:12:37.297607 opticalglass-1.0.6/src/opticalglass/data/
+-rw-r--r--   0 Mike       (501) staff       (20)   674304 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/data/CDGM.xls
+-rw-r--r--   0 Mike       (501) staff       (20)   454924 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/data/HIKARI.xlsx
+-rw-r--r--   0 Mike       (501) staff       (20)   731648 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/data/HIKARI_prev.xls
+-rw-r--r--   0 Mike       (501) staff       (20)  1234441 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/data/HOYA.xlsx
+-rw-r--r--   0 Mike       (501) staff       (20)  1269672 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/data/HOYA_prev.xlsx
+-rw-r--r--   0 Mike       (501) staff       (20)   252743 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/data/OHARA.xlsx
+-rw-r--r--   0 Mike       (501) staff       (20)   265141 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/data/OHARA_prev.xlsx
+-rw-r--r--   0 Mike       (501) staff       (20)   450048 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/data/SCHOTT.xls
+-rw-r--r--   0 Mike       (501) staff       (20)   449024 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/data/SCHOTT_prev.xls
+-rw-r--r--   0 Mike       (501) staff       (20)   160596 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/data/SUMITA.xlsx
+-rw-r--r--   0 Mike       (501) staff       (20)    58113 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/data/robb1983_data_final.txt
+-rw-r--r--   0 Mike       (501) staff       (20)      165 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/data/~$HIKARI.xlsx
+-rw-r--r--   0 Mike       (501) staff       (20)    27474 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/glass.py
+-rw-r--r--   0 Mike       (501) staff       (20)      834 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/glasserror.py
+-rw-r--r--   0 Mike       (501) staff       (20)     4094 2023-06-14 03:17:14.000000 opticalglass-1.0.6/src/opticalglass/glassfactory.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)    15776 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/glassmap.py
+-rw-r--r--   0 Mike       (501) staff       (20)    10922 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/glassmapviewer.py
+-rw-r--r--   0 Mike       (501) staff       (20)     2283 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/glasspolygons.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)     3525 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/hikari.py
+-rw-r--r--   0 Mike       (501) staff       (20)     3021 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/hoya.py
+-rw-r--r--   0 Mike       (501) staff       (20)     2211 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/modelglass.py
+-rw-r--r--   0 Mike       (501) staff       (20)     2921 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/ohara.py
+-rw-r--r--   0 Mike       (501) staff       (20)     2919 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/openpyxl_script.py
+-rw-r--r--   0 Mike       (501) staff       (20)     7531 2023-01-01 20:40:31.000000 opticalglass-1.0.6/src/opticalglass/optical_glass_agf_class.py
+-rw-r--r--   0 Mike       (501) staff       (20)     7638 2023-05-15 05:55:23.000000 opticalglass-1.0.6/src/opticalglass/opticalmedium.py
+-rw-r--r--   0 Mike       (501) staff       (20)    14320 2023-05-15 06:40:19.000000 opticalglass-1.0.6/src/opticalglass/rindexinfo.py
+-rw-r--r--   0 Mike       (501) staff       (20)     3163 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/schott.py
+-rw-r--r--   0 Mike       (501) staff       (20)     3783 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/spectral_lines.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)     3223 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/sumita.py
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-06-14 23:12:37.303010 opticalglass-1.0.6/src/opticalglass/test/
+-rwxr-xr-x   0 Mike       (501) staff       (20)      879 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/test/cmd_line_example.py
+-rw-r--r--   0 Mike       (501) staff       (20)     1969 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/test/test_cdgm.py
+-rw-r--r--   0 Mike       (501) staff       (20)     1738 2023-06-14 03:22:34.000000 opticalglass-1.0.6/src/opticalglass/test/test_create_glass.py
+-rw-r--r--   0 Mike       (501) staff       (20)     3050 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/test/test_glassfactory.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)     2200 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/test/test_hikari.py
+-rw-r--r--   0 Mike       (501) staff       (20)     2060 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/test/test_hoya.py
+-rw-r--r--   0 Mike       (501) staff       (20)     2071 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/test/test_ohara.py
+-rw-r--r--   0 Mike       (501) staff       (20)     1814 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/test/test_schott.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)     2452 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/test/test_sumita.py
+-rw-r--r--   0 Mike       (501) staff       (20)     3767 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/test/test_transmission.py
+-rw-r--r--   0 Mike       (501) staff       (20)     1193 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/test/util.py
+-rwxr-xr-x   0 Mike       (501) staff       (20)     1941 2022-08-24 19:03:29.000000 opticalglass-1.0.6/src/opticalglass/util.py
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-06-14 23:12:37.231765 opticalglass-1.0.6/src/opticalglass.egg-info/
+-rw-r--r--   0 Mike       (501) staff       (20)     2135 2023-06-14 23:12:36.000000 opticalglass-1.0.6/src/opticalglass.egg-info/PKG-INFO
+-rw-r--r--   0 Mike       (501) staff       (20)     3367 2023-06-14 23:12:37.000000 opticalglass-1.0.6/src/opticalglass.egg-info/SOURCES.txt
+-rw-r--r--   0 Mike       (501) staff       (20)        1 2023-06-14 23:12:36.000000 opticalglass-1.0.6/src/opticalglass.egg-info/dependency_links.txt
+-rw-r--r--   0 Mike       (501) staff       (20)       58 2023-06-14 23:12:36.000000 opticalglass-1.0.6/src/opticalglass.egg-info/entry_points.txt
+-rw-r--r--   0 Mike       (501) staff       (20)        1 2022-08-23 03:14:07.000000 opticalglass-1.0.6/src/opticalglass.egg-info/not-zip-safe
+-rw-r--r--   0 Mike       (501) staff       (20)      168 2023-06-14 23:12:36.000000 opticalglass-1.0.6/src/opticalglass.egg-info/requires.txt
+-rw-r--r--   0 Mike       (501) staff       (20)       13 2023-06-14 23:12:36.000000 opticalglass-1.0.6/src/opticalglass.egg-info/top_level.txt
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-06-14 23:12:37.303807 opticalglass-1.0.6/update/
+-rw-r--r--   0 Mike       (501) staff       (20)     1266 2019-01-17 05:29:49.000000 opticalglass-1.0.6/update/catupdate.py
```

### Comparing `opticalglass-1.0.5/CHANGELOG.rst` & `opticalglass-1.0.6/CHANGELOG.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 .. currentmodule:: opticalglass
 
 =========
 Changelog
 =========
 
+Version 1.0.6
+=============
+Bullet-proof and add testcase for :func:`~.glassfactory.create_glass`.
+
 Version 1.0.5
 =============
 Enable :class:`~.rindexinfo.RIIMedium` to be saved and restored as JSON files.
 
 Version 1.0.4
 =============
 Allow extrapolation for :class:`~.opticalmedium.InterpolatedMedium` refractive index interpolation function. Cleanup help and other references to transported classes from **ray-optics**. Fix version export in build process.
```

### Comparing `opticalglass-1.0.5/LICENSE` & `opticalglass-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/PKG-INFO` & `opticalglass-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opticalglass
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tools for reading optical glass catalogs
 Home-page: https://github.com/mjhoptics/opticalglass
 Author: Michael J Hayford
 Author-email: mjhoptics@gmail.com
 License: BSD-3-Clause
 Keywords: glass, optical glass, refractive index, optics,,glass catalog
 Platform: any
```

### Comparing `opticalglass-1.0.5/README.rst` & `opticalglass-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/Makefile` & `opticalglass-1.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_Pandas_intro/OG_Pandas_intro.rst` & `opticalglass-1.0.6/docs/OG_Pandas_intro/OG_Pandas_intro.rst`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_Pandas_intro/output_22_1.png` & `opticalglass-1.0.6/docs/OG_Pandas_intro/output_22_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_Pandas_intro/output_24_1.png` & `opticalglass-1.0.6/docs/OG_Pandas_intro/output_24_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_Pandas_intro/output_26_1.png` & `opticalglass-1.0.6/docs/OG_Pandas_intro/output_26_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_Pandas_intro/output_38_1.png` & `opticalglass-1.0.6/docs/OG_Pandas_intro/output_38_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_Quickstart/OG_Quickstart.rst` & `opticalglass-1.0.6/docs/OG_Quickstart/OG_Quickstart.rst`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_Quickstart/output_16_1.png` & `opticalglass-1.0.6/docs/OG_Quickstart/output_16_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_Quickstart/output_17_1.png` & `opticalglass-1.0.6/docs/OG_Quickstart/output_17_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_Quickstart/output_19_0.png` & `opticalglass-1.0.6/docs/OG_Quickstart/output_19_0.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_Quickstart/output_28_1.png` & `opticalglass-1.0.6/docs/OG_Quickstart/output_28_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/OG_RefractiveIndexInfo.rst` & `opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/OG_RefractiveIndexInfo.rst`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_copy_data_link.png` & `opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/RII_page_copy_data_link.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_data_links.png` & `opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/RII_page_data_links.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_rindexdata.png` & `opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/RII_page_rindexdata.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/RII_page_top.png` & `opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/RII_page_top.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_19_1.png` & `opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_19_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_21_1.png` & `opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_21_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_23_1.png` & `opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_23_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_26_1.png` & `opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_26_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_29_1.png` & `opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_29_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_33_1.png` & `opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_33_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_36_1.png` & `opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_36_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/OG_RefractiveIndexInfo/output_9_1.png` & `opticalglass-1.0.6/docs/OG_RefractiveIndexInfo/output_9_1.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/README.rst` & `opticalglass-1.0.6/docs/README.rst`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/_images/BuchdahlCoefficients.png` & `opticalglass-1.0.6/docs/_images/BuchdahlCoefficients.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/_images/BuchdahlDispersion.png` & `opticalglass-1.0.6/docs/_images/BuchdahlDispersion.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/_images/CatalogSelection.png` & `opticalglass-1.0.6/docs/_images/CatalogSelection.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/_images/GlassMap.png` & `opticalglass-1.0.6/docs/_images/GlassMap.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/_images/IndexVsWvl.png` & `opticalglass-1.0.6/docs/_images/IndexVsWvl.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/_images/PartialDispersion.png` & `opticalglass-1.0.6/docs/_images/PartialDispersion.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/_images/PartialMap.png` & `opticalglass-1.0.6/docs/_images/PartialMap.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/_images/RefractiveIndex.png` & `opticalglass-1.0.6/docs/_images/RefractiveIndex.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/_images/output_11_0.png` & `opticalglass-1.0.6/docs/_images/output_11_0.png`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/conf.py` & `opticalglass-1.0.6/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,16 @@
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = 'friendly'
 # pygments_style = 'xcode'
 # pygments_style = 'solarize-light'
 
 rst_prolog = """
-.. |minimum_python_version| replace:: 3.8
-.. |minimum_numpy_version| replace:: 1.21.5
+.. |minimum_python_version| replace:: 3.10
+.. |minimum_numpy_version| replace:: 1.24.3
 .. |Series| replace:: :class:`~pandas.Series`
 .. |DataFrame| replace:: :class:`~pandas.DataFrame`
 """
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
@@ -204,12 +204,12 @@
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 python_version = ".".join(map(str, sys.version_info[0:2]))
 intersphinx_mapping = {
     "python": ("https://docs.python.org/" + python_version, None),
-    'matplotlib': ('https://matplotlib.org', None),
+    'matplotlib': ('https://matplotlib.org/stable', None),
     'numpy': ('https://numpy.org/doc/stable', None),
     'pandas': ('https://pandas.pydata.org/pandas-docs/stable', None),
-    'scipy': ('https://docs.scipy.org/doc/scipy/reference', None),
+    'scipy': ('https://docs.scipy.org/doc/scipy', None),
     }
```

### Comparing `opticalglass-1.0.5/docs/index.rst` & `opticalglass-1.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/make.bat` & `opticalglass-1.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/docs/opticalglass.rst` & `opticalglass-1.0.6/docs/opticalglass.rst`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/setup.cfg` & `opticalglass-1.0.6/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
-	numpy>=1.21.5
-	scipy>=1.7.3
-	matplotlib>=3.5.1
-	pandas>=1.3.5
+	numpy>=1.24.3
+	scipy>=1.10.1
+	matplotlib>=3.7.1
+	pandas>=2.0.2
 	xlrd>=2.0.1
-	openpyxl>=3.0.9
-	requests>=2.27.1
+	openpyxl>=3.1.2
+	requests>=2.31.0
 	pyyaml>=6.0
 	pyqt5<5.16
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `opticalglass-1.0.5/setup.py` & `opticalglass-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/__init__.py` & `opticalglass-1.0.6/src/opticalglass/__init__.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/buchdahl.py` & `opticalglass-1.0.6/src/opticalglass/buchdahl.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/caselessDictionary.py` & `opticalglass-1.0.6/src/opticalglass/caselessDictionary.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/cdgm.py` & `opticalglass-1.0.6/src/opticalglass/cdgm.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/data/CDGM.xls` & `opticalglass-1.0.6/src/opticalglass/data/CDGM.xls`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/data/HIKARI.xlsx` & `opticalglass-1.0.6/src/opticalglass/data/HIKARI.xlsx`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/data/HIKARI_prev.xls` & `opticalglass-1.0.6/src/opticalglass/data/HIKARI_prev.xls`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/data/HOYA.xlsx` & `opticalglass-1.0.6/src/opticalglass/data/HOYA.xlsx`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/data/HOYA_prev.xlsx` & `opticalglass-1.0.6/src/opticalglass/data/HOYA_prev.xlsx`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/data/OHARA.xlsx` & `opticalglass-1.0.6/src/opticalglass/data/OHARA.xlsx`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/data/OHARA_prev.xlsx` & `opticalglass-1.0.6/src/opticalglass/data/OHARA_prev.xlsx`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/data/SCHOTT.xls` & `opticalglass-1.0.6/src/opticalglass/data/SCHOTT.xls`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/data/SCHOTT_prev.xls` & `opticalglass-1.0.6/src/opticalglass/data/SCHOTT_prev.xls`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/data/SUMITA.xlsx` & `opticalglass-1.0.6/src/opticalglass/data/SUMITA.xlsx`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/data/robb1983_data_final.txt` & `opticalglass-1.0.6/src/opticalglass/data/robb1983_data_final.txt`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/glass.py` & `opticalglass-1.0.6/src/opticalglass/glass.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/glasserror.py` & `opticalglass-1.0.6/src/opticalglass/glasserror.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/glassfactory.py` & `opticalglass-1.0.6/src/opticalglass/glassfactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,16 @@
             logging.info('glass catalog %s not found', catalog)
             raise ge.GlassCatalogNotFoundError(catalog)
 
     if len(name_catalog) == 2:
         name, catalog = name_catalog
     else:
         name, catalog = name_catalog[0].split(',')
+    name = name.strip()
+    catalog = catalog.strip()
 
     if isinstance(catalog, str):
         return _create_glass(name, catalog)
 
     else:  # treat catalog as a list
         for cat in catalog:
             try:
```

### Comparing `opticalglass-1.0.5/src/opticalglass/glassmap.py` & `opticalglass-1.0.6/src/opticalglass/glassmap.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/glassmapviewer.py` & `opticalglass-1.0.6/src/opticalglass/glassmapviewer.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/glasspolygons.py` & `opticalglass-1.0.6/src/opticalglass/glasspolygons.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/hikari.py` & `opticalglass-1.0.6/src/opticalglass/hikari.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/hoya.py` & `opticalglass-1.0.6/src/opticalglass/hoya.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/modelglass.py` & `opticalglass-1.0.6/src/opticalglass/modelglass.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/ohara.py` & `opticalglass-1.0.6/src/opticalglass/ohara.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/openpyxl_script.py` & `opticalglass-1.0.6/src/opticalglass/openpyxl_script.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/optical_glass_agf_class.py` & `opticalglass-1.0.6/src/opticalglass/optical_glass_agf_class.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/opticalmedium.py` & `opticalglass-1.0.6/src/opticalglass/opticalmedium.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/rindexinfo.py` & `opticalglass-1.0.6/src/opticalglass/rindexinfo.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/schott.py` & `opticalglass-1.0.6/src/opticalglass/schott.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/spectral_lines.py` & `opticalglass-1.0.6/src/opticalglass/spectral_lines.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/sumita.py` & `opticalglass-1.0.6/src/opticalglass/sumita.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/test/cmd_line_example.py` & `opticalglass-1.0.6/src/opticalglass/test/cmd_line_example.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/test/test_cdgm.py` & `opticalglass-1.0.6/src/opticalglass/test/test_cdgm.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/test/test_glassfactory.py` & `opticalglass-1.0.6/src/opticalglass/test/test_glassfactory.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/test/test_hikari.py` & `opticalglass-1.0.6/src/opticalglass/test/test_hikari.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/test/test_hoya.py` & `opticalglass-1.0.6/src/opticalglass/test/test_hoya.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/test/test_ohara.py` & `opticalglass-1.0.6/src/opticalglass/test/test_ohara.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/test/test_schott.py` & `opticalglass-1.0.6/src/opticalglass/test/test_schott.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/test/test_sumita.py` & `opticalglass-1.0.6/src/opticalglass/test/test_sumita.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/test/test_transmission.py` & `opticalglass-1.0.6/src/opticalglass/test/test_transmission.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/test/util.py` & `opticalglass-1.0.6/src/opticalglass/test/util.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass/util.py` & `opticalglass-1.0.6/src/opticalglass/util.py`

 * *Files identical despite different names*

### Comparing `opticalglass-1.0.5/src/opticalglass.egg-info/PKG-INFO` & `opticalglass-1.0.6/src/opticalglass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opticalglass
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tools for reading optical glass catalogs
 Home-page: https://github.com/mjhoptics/opticalglass
 Author: Michael J Hayford
 Author-email: mjhoptics@gmail.com
 License: BSD-3-Clause
 Keywords: glass, optical glass, refractive index, optics,,glass catalog
 Platform: any
```

### Comparing `opticalglass-1.0.5/src/opticalglass.egg-info/SOURCES.txt` & `opticalglass-1.0.6/src/opticalglass.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 src/opticalglass/data/SCHOTT.xls
 src/opticalglass/data/SCHOTT_prev.xls
 src/opticalglass/data/SUMITA.xlsx
 src/opticalglass/data/robb1983_data_final.txt
 src/opticalglass/data/~$HIKARI.xlsx
 src/opticalglass/test/cmd_line_example.py
 src/opticalglass/test/test_cdgm.py
+src/opticalglass/test/test_create_glass.py
 src/opticalglass/test/test_glassfactory.py
 src/opticalglass/test/test_hikari.py
 src/opticalglass/test/test_hoya.py
 src/opticalglass/test/test_ohara.py
 src/opticalglass/test/test_schott.py
 src/opticalglass/test/test_sumita.py
 src/opticalglass/test/test_transmission.py
```

### Comparing `opticalglass-1.0.5/update/catupdate.py` & `opticalglass-1.0.6/update/catupdate.py`

 * *Files identical despite different names*

