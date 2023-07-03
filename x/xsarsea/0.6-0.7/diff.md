# Comparing `tmp/xsarsea-0.6.tar.gz` & `tmp/xsarsea-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsarsea-0.6.tar", last modified: Mon Jul  3 12:27:05 2023, max compression
+gzip compressed data, was "xsarsea-0.7.tar", last modified: Mon Jul  3 12:38:50 2023, max compression
```

## Comparing `xsarsea-0.6.tar` & `xsarsea-0.7.tar`

### file list

```diff
@@ -1,61 +1,58 @@
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-07-03 12:27:05.970697 xsarsea-0.6/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      107 2022-04-08 08:40:22.000000 xsarsea-0.6/.gitattributes
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      553 2022-04-08 08:40:22.000000 xsarsea-0.6/.gitconfig
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-07-03 12:27:05.590697 xsarsea-0.6/.github/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      117 2023-07-03 12:26:53.000000 xsarsea-0.6/.github/dependabot.yml
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-07-03 12:27:05.598697 xsarsea-0.6/.github/workflows/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      936 2023-07-03 12:26:53.000000 xsarsea-0.6/.github/workflows/main.yml
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      829 2023-07-03 12:26:53.000000 xsarsea-0.6/.github/workflows/publish.yml
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     1790 2022-04-08 08:40:22.000000 xsarsea-0.6/.gitignore
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      957 2023-07-03 12:26:53.000000 xsarsea-0.6/.pre-commit-config.yaml
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     1064 2022-04-08 08:40:22.000000 xsarsea-0.6/LICENSE
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      261 2023-07-03 12:27:05.970697 xsarsea-0.6/PKG-INFO
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      519 2022-11-15 13:34:36.000000 xsarsea-0.6/README.md
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-07-03 12:27:05.610697 xsarsea-0.6/docs/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      634 2022-04-08 08:40:22.000000 xsarsea-0.6/docs/Makefile
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-07-03 12:27:05.562697 xsarsea-0.6/docs/_static/
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-07-03 12:27:05.614697 xsarsea-0.6/docs/_static/css/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      127 2022-04-08 08:40:22.000000 xsarsea-0.6/docs/_static/css/xsarsea.css
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      565 2023-02-28 13:33:38.000000 xsarsea-0.6/docs/basic_api.rst
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     3270 2022-11-15 13:34:36.000000 xsarsea-0.6/docs/conf.py
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-07-03 12:27:05.854697 xsarsea-0.6/docs/examples/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    10800 2022-11-15 13:34:36.000000 xsarsea-0.6/docs/examples/gmfs_and_luts.ipynb
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    12273 2023-04-13 11:38:29.000000 xsarsea-0.6/docs/examples/streaks.ipynb
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    12008 2022-11-15 15:37:54.000000 xsarsea-0.6/docs/examples/windspeed_inversion.ipynb
--rw-rw-r--   0 agrouaze (54605) droos    (10042)  3931394 2023-07-03 12:26:53.000000 xsarsea-0.6/docs/examples/windspeed_retrieval_L1.ipynb
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     3466 2022-11-15 13:34:36.000000 xsarsea-0.6/docs/examples/xsarsea.ipynb
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     1611 2023-04-13 11:38:29.000000 xsarsea-0.6/docs/index.rst
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      960 2022-04-08 08:40:22.000000 xsarsea-0.6/docs/installing.rst
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      381 2022-12-16 14:14:18.000000 xsarsea-0.6/requirements.txt
--rw-rw-r--   0 agrouaze (54605) droos    (10042)       38 2023-07-03 12:27:05.970697 xsarsea-0.6/setup.cfg
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      816 2022-11-17 15:08:15.000000 xsarsea-0.6/setup.py
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-07-03 12:27:05.566697 xsarsea-0.6/src/
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-07-03 12:27:05.866697 xsarsea-0.6/src/scripts/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      551 2022-12-16 14:14:18.000000 xsarsea-0.6/src/scripts/configuration_L1B_xspectra_IW_SLC_IFR_v1.yml
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     8684 2023-07-03 12:26:53.000000 xsarsea-0.6/src/scripts/wind_speed_retrieval.py
--rwxrwxr-x   0 agrouaze (54605) droos    (10042)     1163 2022-11-17 13:03:25.000000 xsarsea-0.6/src/scripts/xsarsea_cli.py
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-07-03 12:27:05.926697 xsarsea-0.6/src/xsarsea/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      377 2023-02-28 13:33:38.000000 xsarsea-0.6/src/xsarsea/__init__.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)       57 2022-11-15 13:34:36.000000 xsarsea-0.6/src/xsarsea/config.yml
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     9078 2023-02-28 11:59:26.000000 xsarsea-0.6/src/xsarsea/cross_spectra_core_backup.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     2770 2023-02-28 11:59:13.000000 xsarsea-0.6/src/xsarsea/from_tiff_WV_to_modulation_backup.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    26004 2022-11-15 15:37:54.000000 xsarsea-0.6/src/xsarsea/gradients.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     4338 2023-02-28 11:58:57.000000 xsarsea-0.6/src/xsarsea/slc_image_normalization_backup.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     3455 2023-04-13 11:38:29.000000 xsarsea-0.6/src/xsarsea/utils.py
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-07-03 12:27:05.962697 xsarsea-0.6/src/xsarsea/windspeed/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      466 2023-04-13 11:38:29.000000 xsarsea-0.6/src/xsarsea/windspeed/__init__.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    12311 2022-11-15 13:34:36.000000 xsarsea-0.6/src/xsarsea/windspeed/gmfs.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     8218 2023-04-13 11:38:29.000000 xsarsea-0.6/src/xsarsea/windspeed/gmfs_impl.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    13902 2022-11-15 13:34:36.000000 xsarsea-0.6/src/xsarsea/windspeed/models.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     4108 2022-11-15 13:34:36.000000 xsarsea-0.6/src/xsarsea/windspeed/sarwing_luts.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     3208 2023-04-13 11:38:29.000000 xsarsea-0.6/src/xsarsea/windspeed/utils.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    15727 2022-11-15 15:37:54.000000 xsarsea-0.6/src/xsarsea/windspeed/windspeed.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     3216 2022-11-15 15:37:54.000000 xsarsea-0.6/src/xsarsea/xsarsea.py
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-07-03 12:27:05.942697 xsarsea-0.6/src/xsarsea.egg-info/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      261 2023-07-03 12:27:05.000000 xsarsea-0.6/src/xsarsea.egg-info/PKG-INFO
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     1269 2023-07-03 12:27:05.000000 xsarsea-0.6/src/xsarsea.egg-info/SOURCES.txt
--rw-rw-r--   0 agrouaze (54605) droos    (10042)        1 2023-07-03 12:27:05.000000 xsarsea-0.6/src/xsarsea.egg-info/dependency_links.txt
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      111 2023-07-03 12:27:05.000000 xsarsea-0.6/src/xsarsea.egg-info/requires.txt
--rw-rw-r--   0 agrouaze (54605) droos    (10042)        8 2023-07-03 12:27:05.000000 xsarsea-0.6/src/xsarsea.egg-info/top_level.txt
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-07-03 12:27:05.966697 xsarsea-0.6/test/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     5008 2023-07-03 12:15:14.000000 xsarsea-0.6/test/test_xsarsea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:38:50.308410 xsarsea-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-03 12:38:34.000000 xsarsea-0.7/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-03 12:38:34.000000 xsarsea-0.7/.gitconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:38:50.300410 xsarsea-0.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 12:38:34.000000 xsarsea-0.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:38:50.300410 xsarsea-0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-03 12:38:34.000000 xsarsea-0.7/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-03 12:38:34.000000 xsarsea-0.7/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-03 12:38:34.000000 xsarsea-0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-03 12:38:34.000000 xsarsea-0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 12:38:34.000000 xsarsea-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-03 12:38:50.308410 xsarsea-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-03 12:38:34.000000 xsarsea-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:38:50.304410 xsarsea-0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-03 12:38:34.000000 xsarsea-0.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:38:50.300410 xsarsea-0.7/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:38:50.304410 xsarsea-0.7/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-03 12:38:34.000000 xsarsea-0.7/docs/_static/css/xsarsea.css
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-03 12:38:34.000000 xsarsea-0.7/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-03 12:38:34.000000 xsarsea-0.7/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:38:50.308410 xsarsea-0.7/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-07-03 12:38:34.000000 xsarsea-0.7/docs/examples/gmfs_and_luts.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-03 12:38:34.000000 xsarsea-0.7/docs/examples/streaks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12008 2023-07-03 12:38:34.000000 xsarsea-0.7/docs/examples/windspeed_inversion.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  3931394 2023-07-03 12:38:34.000000 xsarsea-0.7/docs/examples/windspeed_retrieval_L1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-03 12:38:34.000000 xsarsea-0.7/docs/examples/xsarsea.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-03 12:38:34.000000 xsarsea-0.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-03 12:38:34.000000 xsarsea-0.7/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 12:38:34.000000 xsarsea-0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:38:50.308410 xsarsea-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-03 12:38:34.000000 xsarsea-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:38:50.300410 xsarsea-0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:38:50.308410 xsarsea-0.7/src/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-03 12:38:34.000000 xsarsea-0.7/src/scripts/configuration_L1B_xspectra_IW_SLC_IFR_v1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-03 12:38:34.000000 xsarsea-0.7/src/scripts/wind_speed_retrieval.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1163 2023-07-03 12:38:34.000000 xsarsea-0.7/src/scripts/xsarsea_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:38:50.308410 xsarsea-0.7/src/xsarsea/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-03 12:38:34.000000 xsarsea-0.7/src/xsarsea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-03 12:38:34.000000 xsarsea-0.7/src/xsarsea/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    26004 2023-07-03 12:38:34.000000 xsarsea-0.7/src/xsarsea/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-03 12:38:34.000000 xsarsea-0.7/src/xsarsea/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:38:50.308410 xsarsea-0.7/src/xsarsea/windspeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-03 12:38:34.000000 xsarsea-0.7/src/xsarsea/windspeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-07-03 12:38:34.000000 xsarsea-0.7/src/xsarsea/windspeed/gmfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-03 12:38:34.000000 xsarsea-0.7/src/xsarsea/windspeed/gmfs_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-07-03 12:38:34.000000 xsarsea-0.7/src/xsarsea/windspeed/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-03 12:38:34.000000 xsarsea-0.7/src/xsarsea/windspeed/sarwing_luts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-03 12:38:34.000000 xsarsea-0.7/src/xsarsea/windspeed/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15727 2023-07-03 12:38:34.000000 xsarsea-0.7/src/xsarsea/windspeed/windspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-03 12:38:34.000000 xsarsea-0.7/src/xsarsea/xsarsea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:38:50.308410 xsarsea-0.7/src/xsarsea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-03 12:38:50.000000 xsarsea-0.7/src/xsarsea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-03 12:38:50.000000 xsarsea-0.7/src/xsarsea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:38:50.000000 xsarsea-0.7/src/xsarsea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-03 12:38:50.000000 xsarsea-0.7/src/xsarsea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 12:38:50.000000 xsarsea-0.7/src/xsarsea.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:38:50.308410 xsarsea-0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-03 12:38:34.000000 xsarsea-0.7/test/test_xsarsea.py
```

### Comparing `xsarsea-0.6/.gitconfig` & `xsarsea-0.7/.gitconfig`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/.github/workflows/main.yml` & `xsarsea-0.7/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/.github/workflows/publish.yml` & `xsarsea-0.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/.gitignore` & `xsarsea-0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/.pre-commit-config.yaml` & `xsarsea-0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/LICENSE` & `xsarsea-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/README.md` & `xsarsea-0.7/README.md`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/docs/Makefile` & `xsarsea-0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/docs/basic_api.rst` & `xsarsea-0.7/docs/basic_api.rst`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/docs/conf.py` & `xsarsea-0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/docs/examples/gmfs_and_luts.ipynb` & `xsarsea-0.7/docs/examples/gmfs_and_luts.ipynb`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/docs/examples/streaks.ipynb` & `xsarsea-0.7/docs/examples/streaks.ipynb`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/docs/examples/windspeed_inversion.ipynb` & `xsarsea-0.7/docs/examples/windspeed_inversion.ipynb`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/docs/examples/windspeed_retrieval_L1.ipynb` & `xsarsea-0.7/docs/examples/windspeed_retrieval_L1.ipynb`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/docs/examples/xsarsea.ipynb` & `xsarsea-0.7/docs/examples/xsarsea.ipynb`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/docs/index.rst` & `xsarsea-0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/docs/installing.rst` & `xsarsea-0.7/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/src/scripts/configuration_L1B_xspectra_IW_SLC_IFR_v1.yml` & `xsarsea-0.7/src/scripts/configuration_L1B_xspectra_IW_SLC_IFR_v1.yml`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/src/scripts/wind_speed_retrieval.py` & `xsarsea-0.7/src/scripts/wind_speed_retrieval.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/src/scripts/xsarsea_cli.py` & `xsarsea-0.7/src/scripts/xsarsea_cli.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/src/xsarsea/gradients.py` & `xsarsea-0.7/src/xsarsea/gradients.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/src/xsarsea/utils.py` & `xsarsea-0.7/src/xsarsea/utils.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/src/xsarsea/windspeed/gmfs.py` & `xsarsea-0.7/src/xsarsea/windspeed/gmfs.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/src/xsarsea/windspeed/gmfs_impl.py` & `xsarsea-0.7/src/xsarsea/windspeed/gmfs_impl.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/src/xsarsea/windspeed/models.py` & `xsarsea-0.7/src/xsarsea/windspeed/models.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/src/xsarsea/windspeed/sarwing_luts.py` & `xsarsea-0.7/src/xsarsea/windspeed/sarwing_luts.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/src/xsarsea/windspeed/utils.py` & `xsarsea-0.7/src/xsarsea/windspeed/utils.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/src/xsarsea/windspeed/windspeed.py` & `xsarsea-0.7/src/xsarsea/windspeed/windspeed.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/src/xsarsea/xsarsea.py` & `xsarsea-0.7/src/xsarsea/xsarsea.py`

 * *Files identical despite different names*

### Comparing `xsarsea-0.6/src/xsarsea.egg-info/SOURCES.txt` & `xsarsea-0.7/src/xsarsea.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,18 +21,15 @@
 docs/examples/windspeed_retrieval_L1.ipynb
 docs/examples/xsarsea.ipynb
 src/scripts/configuration_L1B_xspectra_IW_SLC_IFR_v1.yml
 src/scripts/wind_speed_retrieval.py
 src/scripts/xsarsea_cli.py
 src/xsarsea/__init__.py
 src/xsarsea/config.yml
-src/xsarsea/cross_spectra_core_backup.py
-src/xsarsea/from_tiff_WV_to_modulation_backup.py
 src/xsarsea/gradients.py
-src/xsarsea/slc_image_normalization_backup.py
 src/xsarsea/utils.py
 src/xsarsea/xsarsea.py
 src/xsarsea.egg-info/PKG-INFO
 src/xsarsea.egg-info/SOURCES.txt
 src/xsarsea.egg-info/dependency_links.txt
 src/xsarsea.egg-info/requires.txt
 src/xsarsea.egg-info/top_level.txt
```

### Comparing `xsarsea-0.6/test/test_xsarsea.py` & `xsarsea-0.7/test/test_xsarsea.py`

 * *Files identical despite different names*

