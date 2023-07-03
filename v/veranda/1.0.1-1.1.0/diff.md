# Comparing `tmp/veranda-1.0.1.tar.gz` & `tmp/veranda-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/veranda-1.0.1.tar", last modified: Thu Feb  2 08:20:22 2023, max compression
+gzip compressed data, was "dist/veranda-1.1.0.tar", last modified: Mon Jul  3 08:34:52 2023, max compression
```

## Comparing `veranda-1.0.1.tar` & `veranda-1.1.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-02 08:20:08.000000 veranda-1.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-02 08:20:08.000000 veranda-1.0.1/.github/workflows/upload_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-02-02 08:20:08.000000 veranda-1.0.1/.github/workflows/veranda_ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-02-02 08:20:08.000000 veranda-1.0.1/.github/workflows/veranda_windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-02 08:20:08.000000 veranda-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-02 08:20:08.000000 veranda-1.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-02-02 08:20:08.000000 veranda-1.0.1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-02 08:20:08.000000 veranda-1.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-02-02 08:20:08.000000 veranda-1.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-02-02 08:20:08.000000 veranda-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-02-02 08:20:22.000000 veranda-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-02-02 08:20:08.000000 veranda-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-02 08:20:08.000000 veranda-1.0.1/conda_env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-02-02 08:20:08.000000 veranda-1.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-02 08:20:08.000000 veranda-1.0.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-02 08:20:08.000000 veranda-1.0.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-02 08:20:08.000000 veranda-1.0.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-02 08:20:08.000000 veranda-1.0.1/docs/conda_env_docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-02-02 08:20:08.000000 veranda-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-02-02 08:20:08.000000 veranda-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-02-02 08:20:08.000000 veranda-1.0.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-02 08:20:08.000000 veranda-1.0.1/docs/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   269748 2023-02-02 08:20:08.000000 veranda-1.0.1/docs/notebooks/mosaic.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-02-02 08:20:22.000000 veranda-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-02 08:20:08.000000 veranda-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/src/veranda/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-02-02 08:20:08.000000 veranda-1.0.1/src/veranda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/src/veranda/raster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:08.000000 veranda-1.0.1/src/veranda/raster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-02-02 08:20:08.000000 veranda-1.0.1/src/veranda/raster/gdalport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/src/veranda/raster/mosaic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:08.000000 veranda-1.0.1/src/veranda/raster/mosaic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43894 2023-02-02 08:20:08.000000 veranda-1.0.1/src/veranda/raster/mosaic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    34640 2023-02-02 08:20:08.000000 veranda-1.0.1/src/veranda/raster/mosaic/geotiff.py
--rw-r--r--   0 runner    (1001) docker     (123)    39967 2023-02-02 08:20:08.000000 veranda-1.0.1/src/veranda/raster/mosaic/netcdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/src/veranda/raster/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:08.000000 veranda-1.0.1/src/veranda/raster/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-02-02 08:20:08.000000 veranda-1.0.1/src/veranda/raster/native/geotiff.py
--rw-r--r--   0 runner    (1001) docker     (123)    57612 2023-02-02 08:20:08.000000 veranda-1.0.1/src/veranda/raster/native/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-02-02 08:20:08.000000 veranda-1.0.1/src/veranda/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/src/veranda/vector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:08.000000 veranda-1.0.1/src/veranda/vector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/src/veranda/vector/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:08.000000 veranda-1.0.1/src/veranda/vector/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-02 08:20:08.000000 veranda-1.0.1/src/veranda/vector/native/shp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/src/veranda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-02-02 08:20:22.000000 veranda-1.0.1/src/veranda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-02-02 08:20:22.000000 veranda-1.0.1/src/veranda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 08:20:22.000000 veranda-1.0.1/src/veranda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 08:20:22.000000 veranda-1.0.1/src/veranda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-02 08:20:22.000000 veranda-1.0.1/src/veranda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-02 08:20:22.000000 veranda-1.0.1/src/veranda.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/tests/raster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/tests/raster/mosaic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/mosaic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/tests/raster/mosaic/geotiff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/mosaic/geotiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/mosaic/geotiff/test_geotiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/mosaic/mosaic_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/tests/raster/mosaic/netcdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/mosaic/netcdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/mosaic/netcdf/test_netcdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/tests/raster/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/tests/raster/native/geotiff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/native/geotiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/native/geotiff/test_geotiff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:22.000000 veranda-1.0.1/tests/raster/native/netcdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/native/netcdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/native/netcdf/netcdf_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/native/netcdf/test_netcdf4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/native/netcdf/test_xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/test_gdal.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-02 08:20:08.000000 veranda-1.0.1/tests/raster/test_gdalport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-03 08:34:35.000000 veranda-1.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-03 08:34:35.000000 veranda-1.1.0/.github/workflows/upload_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-03 08:34:35.000000 veranda-1.1.0/.github/workflows/veranda_ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-03 08:34:35.000000 veranda-1.1.0/.github/workflows/veranda_windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-03 08:34:35.000000 veranda-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-03 08:34:35.000000 veranda-1.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-03 08:34:35.000000 veranda-1.1.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-03 08:34:35.000000 veranda-1.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-03 08:34:35.000000 veranda-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-03 08:34:35.000000 veranda-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-07-03 08:34:52.000000 veranda-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-03 08:34:35.000000 veranda-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-03 08:34:35.000000 veranda-1.1.0/conda_env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-03 08:34:35.000000 veranda-1.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 08:34:35.000000 veranda-1.1.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 08:34:35.000000 veranda-1.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 08:34:35.000000 veranda-1.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-03 08:34:35.000000 veranda-1.1.0/docs/conda_env_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-07-03 08:34:35.000000 veranda-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-03 08:34:35.000000 veranda-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-03 08:34:35.000000 veranda-1.1.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 08:34:35.000000 veranda-1.1.0/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   269748 2023-07-03 08:34:35.000000 veranda-1.1.0/docs/notebooks/mosaic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-03 08:34:52.000000 veranda-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-03 08:34:35.000000 veranda-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/src/veranda/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-03 08:34:35.000000 veranda-1.1.0/src/veranda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/src/veranda/raster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:35.000000 veranda-1.1.0/src/veranda/raster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-07-03 08:34:35.000000 veranda-1.1.0/src/veranda/raster/gdalport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/src/veranda/raster/mosaic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:35.000000 veranda-1.1.0/src/veranda/raster/mosaic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43998 2023-07-03 08:34:35.000000 veranda-1.1.0/src/veranda/raster/mosaic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34984 2023-07-03 08:34:35.000000 veranda-1.1.0/src/veranda/raster/mosaic/geotiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39967 2023-07-03 08:34:35.000000 veranda-1.1.0/src/veranda/raster/mosaic/netcdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/src/veranda/raster/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:35.000000 veranda-1.1.0/src/veranda/raster/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26537 2023-07-03 08:34:35.000000 veranda-1.1.0/src/veranda/raster/native/geotiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57612 2023-07-03 08:34:35.000000 veranda-1.1.0/src/veranda/raster/native/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 08:34:35.000000 veranda-1.1.0/src/veranda/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/src/veranda/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:35.000000 veranda-1.1.0/src/veranda/vector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/src/veranda/vector/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:35.000000 veranda-1.1.0/src/veranda/vector/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-03 08:34:35.000000 veranda-1.1.0/src/veranda/vector/native/shp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/src/veranda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-07-03 08:34:52.000000 veranda-1.1.0/src/veranda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-03 08:34:52.000000 veranda-1.1.0/src/veranda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:34:52.000000 veranda-1.1.0/src/veranda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:34:52.000000 veranda-1.1.0/src/veranda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 08:34:52.000000 veranda-1.1.0/src/veranda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 08:34:52.000000 veranda-1.1.0/src/veranda.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/tests/raster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/tests/raster/mosaic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/mosaic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/tests/raster/mosaic/geotiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/mosaic/geotiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/mosaic/geotiff/test_geotiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/mosaic/mosaic_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/tests/raster/mosaic/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/mosaic/netcdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/mosaic/netcdf/test_netcdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/tests/raster/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/tests/raster/native/geotiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/native/geotiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/native/geotiff/test_geotiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:52.000000 veranda-1.1.0/tests/raster/native/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/native/netcdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/native/netcdf/netcdf_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/native/netcdf/test_netcdf4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/native/netcdf/test_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/test_gdal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-03 08:34:35.000000 veranda-1.1.0/tests/raster/test_gdalport.py
```

### Comparing `veranda-1.0.1/.coveragerc` & `veranda-1.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/.github/workflows/upload_pypi.yml` & `veranda-1.1.0/.github/workflows/upload_pypi.yml`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/.github/workflows/veranda_ubuntu.yml` & `veranda-1.1.0/.github/workflows/veranda_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/.github/workflows/veranda_windows.yml` & `veranda-1.1.0/.github/workflows/veranda_windows.yml`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/.gitignore` & `veranda-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/.travis.yml` & `veranda-1.1.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/CHANGELOG.rst` & `veranda-1.1.0/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 Changelog
 =========
 
+Version 1.1.0
+=============
+
+- enabled reading GeoTIFF files from ZIP files
+- fixed bug in parallel VRT stack reading (#16) and layer assignment (#19)
+
 Version 1.0.1
 =============
 
 - introduced rounding of spatial coordinates when accessing an xarray dataset
 
 Version 1.0.0
 =============
```

### Comparing `veranda-1.0.1/LICENSE.txt` & `veranda-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/PKG-INFO` & `veranda-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veranda
-Version: 1.0.1
+Version: 1.1.0
 Summary: veranda is a place for IO related classes and operations dealing with multi-dimensional vector and raster data.
 Home-page: https://github.com/TUW-GEO/veranda
 Author: Research Unit Remote Sensing at GEO Department
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: MIT
 Description: # veranda
         [![Build Status](https://travis-ci.com/TUW-GEO/veranda.svg?branch=master)](https://travis-ci.org/TUW-GEO/veranda)
```

### Comparing `veranda-1.0.1/README.md` & `veranda-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/docs/Makefile` & `veranda-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/docs/conf.py` & `veranda-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/docs/index.rst` & `veranda-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/docs/install.rst` & `veranda-1.1.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/docs/notebooks/mosaic.ipynb` & `veranda-1.1.0/docs/notebooks/mosaic.ipynb`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/setup.cfg` & `veranda-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/setup.py` & `veranda-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/src/veranda/raster/gdalport.py` & `veranda-1.1.0/src/veranda/raster/gdalport.py`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/src/veranda/raster/mosaic/base.py` & `veranda-1.1.0/src/veranda/raster/mosaic/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,17 +133,22 @@
 
     @property
     def data_geom(self) -> RasterGeometry:
         """ Raster/tile geometry of the raster mosaic files. """
         return self._data_geom
 
     @property
+    def layer_ids(self) -> list:
+        """ List : Sorted layers. """
+        return list(sorted(self._file_register[self._file_dim].unique()))
+
+    @property
     def n_layers(self) -> int:
         """ Maximum number of layers. """
-        return self._file_register.groupby([self._tile_dim])[self._tile_dim].count().max()
+        return len(self.layer_ids)
 
     @property
     def n_tiles(self) -> int:
         """ Number of tiles. """
         return len(self._mosaic.all_tiles)
 
     @property
```

### Comparing `veranda-1.0.1/src/veranda/raster/mosaic/geotiff.py` & `veranda-1.1.0/src/veranda/raster/mosaic/geotiff.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,21 +20,22 @@
 from veranda.raster.native.geotiff import create_vrt_file
 from veranda.raster.gdalport import GDAL_TO_NUMPY_DTYPE
 from veranda.raster.mosaic.base import RasterDataReader, RasterDataWriter, RasterAccess
 
 PROC_OBJS = {}
 
 
-def read_init(fr, am, sm, sd, td, ad, dc, dk):
+def read_init(fr, am, sm, sd, td, si, ad, dc, dk):
     """ Helper method for setting the entries of global variable `PROC_OBJS` to be available during multiprocessing. """
     PROC_OBJS['global_file_register'] = fr
     PROC_OBJS['access_map'] = am
     PROC_OBJS['shm_map'] = sm
     PROC_OBJS['stack_dimension'] = sd
     PROC_OBJS['tile_dimension'] = td
+    PROC_OBJS['stack_ids'] = si
     PROC_OBJS['auto_decode'] = ad
     PROC_OBJS['decoder'] = dc
     PROC_OBJS['decoder_kwargs'] = dk
 
 
 class GeoTiffAccess(RasterAccess):
     """
@@ -388,15 +389,15 @@
             Keyword arguments for the decoder.
 
         """
         decoder_kwargs = decoder_kwargs or dict()
         global_file_register = self._file_register
 
         with Pool(n_cores, initializer=read_init, initargs=(global_file_register, access_map, shm_map,
-                                                            self._file_dim, self._tile_dim,
+                                                            self._file_dim, self._tile_dim, self.layer_ids,
                                                             auto_decode, decoder, decoder_kwargs)) as p:
             p.map(read_vrt_stack, access_map.keys())
 
     def __read_parallel(self, access_map, shm_map, n_cores=1,
                         auto_decode=False, decoder=None, decoder_kwargs=None):
         """
         Reads GeoTIFF mosaic on a file-by-file basis, in a parallel manner.
@@ -651,34 +652,40 @@
         Tile/geometry ID coming from the Pool's mapping function.
 
     """
     global_file_register = PROC_OBJS['global_file_register']
     access_map = PROC_OBJS['access_map']
     shm_map = PROC_OBJS['shm_map']
     tile_dimension = PROC_OBJS['tile_dimension']
+    stack_dimension = PROC_OBJS['stack_dimension']
+    stack_ids = PROC_OBJS['stack_ids']
 
     gt_access = access_map[tile_id]
     bands = list(shm_map.keys())
     file_register = global_file_register.loc[global_file_register[tile_dimension] == tile_id]
 
-    path = tempfile.gettempdir()
-    vrt_filepath = os.path.join(path, f"{datetime.utcnow().strftime('%Y%m%d%H%M%S')}-{uuid.uuid4().hex}.vrt")
-    while os.path.exists(vrt_filepath):
+    if len(file_register) > 0:
+        path = tempfile.gettempdir()
         vrt_filepath = os.path.join(path, f"{datetime.utcnow().strftime('%Y%m%d%H%M%S')}-{uuid.uuid4().hex}.vrt")
-    filepaths = list(file_register['filepath'])
-    create_vrt_file(filepaths, vrt_filepath, gt_access.src_shape, gt_access.src_wkt, gt_access.src_geotrans,
-                    bands=bands)
+        while os.path.exists(vrt_filepath):
+            vrt_filepath = os.path.join(path, f"{datetime.utcnow().strftime('%Y%m%d%H%M%S')}-{uuid.uuid4().hex}.vrt")
+
+        filepaths = list(file_register['filepath'])
+        create_vrt_file(filepaths, vrt_filepath, gt_access.src_shape, gt_access.src_wkt, gt_access.src_geotrans,
+                        bands=bands)
+
+        layer_ids = [stack_ids.index(stack_id) for stack_id in file_register[stack_dimension]]
 
-    src = gdal.Open(vrt_filepath, gdal.GA_ReadOnly)
-    vrt_data = src.ReadAsArray(*gt_access.gdal_args)
-    for band in bands:
-        _assign_vrt_stack_per_band(tile_id, band, src, vrt_data)
+        src = gdal.Open(vrt_filepath, gdal.GA_ReadOnly)
+        vrt_data = src.ReadAsArray(*gt_access.gdal_args)
+        for band in bands:
+            _assign_vrt_stack_per_band(tile_id, layer_ids, band, src, vrt_data)
 
 
-def _assign_vrt_stack_per_band(tile_id, band, src, vrt_data):
+def _assign_vrt_stack_per_band(tile_id, layer_ids, band, src, vrt_data):
     """
     Assigns loaded raster data to shared memory array for a specific band.
 
     Parameters
     ----------
     tile_id : str
         Tile/geometry ID coming from the Pool's mapping function.
@@ -714,15 +721,15 @@
         if decoder is not None:
             band_data = decoder(band_data, nodataval=nodataval, band=band, scale_factor=scale_factor,
                                 offset=offset,
                                 dtype=dtype, **decoder_kwargs)
 
     shm_rar, shm_ar_shape = shm_map[band]
     shm_data = np.frombuffer(shm_rar, dtype=dtype).reshape(shm_ar_shape)
-    shm_data[:, gt_access.dst_row_slice, gt_access.dst_col_slice] = band_data
+    shm_data[layer_ids, gt_access.dst_row_slice, gt_access.dst_col_slice] = band_data
 
 
 def read_single_files(file_idx):
     """
     Function being responsible to read data from a single GeoTIFF file and assign it to a shared memory array.
     This function is meant to be executed in parallel on different cores.
```

### Comparing `veranda-1.0.1/src/veranda/raster/mosaic/netcdf.py` & `veranda-1.1.0/src/veranda/raster/mosaic/netcdf.py`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/src/veranda/raster/native/geotiff.py` & `veranda-1.1.0/src/veranda/raster/native/geotiff.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Manages I/O for a GeoTIFF file. """
 
 import os
 import struct
+from zipfile import ZipFile
 import numpy as np
 from osgeo import gdal
 from typing import List
 from collections import defaultdict
 import xml.etree.ElementTree as ET
 
 from veranda.utils import to_list
@@ -124,16 +125,24 @@
 
         Returns
         -------
         bool :
             True if the given file is a BigTIFF, else False.
 
         """
-        with open(filepath, 'rb') as f:
-            header = f.read(4)
+        if '.zip' in filepath:
+            if filepath.startswith('/vsizip/'):
+                filepath = filepath[len('/vsizip/'):]  # removes gdal virtual file system prefix to open w ZipFile
+            zip_filepath, inzip_filepath = filepath.split('.zip')
+            with ZipFile(zip_filepath + '.zip') as zip:
+                with zip.open(inzip_filepath[1:], 'r') as f:
+                    header = f.read(4)  # tests reads bytes not str, no need covert to bytearray
+        else:
+            with open(filepath, 'rb') as f:
+                header = f.read(4)
         byteorder = {b'II': '<', b'MM': '>', b'EP': '<'}[header[:2]]
         version = struct.unpack(byteorder + "H", header[2:4])[0]
         return version == 43
 
     @property
     def scale_factors(self) -> List[float]:
         """ Scale factors of the different bands. """
@@ -167,15 +176,28 @@
     def _open(self):
         """
         Helper function supporting the different file modes, i.e. either opening an existing file or creating a new
         file source.
 
         """
         if self.mode == 'r':
-            if not os.path.exists(self.filepath):
+            if '.zip' in self.filepath:
+                if self.filepath.startswith('/vsizip/'):
+                    self.filepath = self.filepath[len('/vsizip/'):]  # removes gdal virtual file system prefix if its there
+                zip_filepath, inzip_filepath = self.filepath.split('.zip')
+                zip_filepath += '.zip'
+                if not os.path.exists(zip_filepath):  # checks zip file
+                    err_msg = f"File '{zip_filepath}' does not exist."
+                    raise FileNotFoundError(err_msg)
+                with ZipFile(zip_filepath) as zip:
+                    if inzip_filepath[1:] not in zip.namelist():  # checks file in zip
+                        err_msg = f"File '{self.filepath}' does not exist."
+                        raise FileNotFoundError(err_msg)
+                self.filepath = '/vsizip/' + self.filepath  # adds the gdal vsi prefix
+            elif not os.path.exists(self.filepath):
                 err_msg = f"File '{self.filepath}' does not exist."
                 raise FileNotFoundError(err_msg)
             self.src = gdal.Open(self.filepath, gdal.GA_ReadOnly)
             self.raster_shape = self.src.RasterYSize, self.src.RasterXSize
             self.geotrans = self.src.GetGeoTransform()
             self.sref_wkt = self.src.GetProjection()
             self.metadata = self.src.GetMetadata()
@@ -617,8 +639,8 @@
     scale_factor = 1 if scale_factor is None else scale_factor
     ET.SubElement(band_elem, "NodataValue").text = str(band_attr_dict['nodataval'][band_idx])
     ET.SubElement(band_elem, "Scale").text = str(scale_factor)
     ET.SubElement(band_elem, "Offset").text = str(band_attr_dict['offset'][band_idx])
 
 
 if __name__ == '__main__':
-    pass
+    pass
```

### Comparing `veranda-1.0.1/src/veranda/raster/native/netcdf.py` & `veranda-1.1.0/src/veranda/raster/native/netcdf.py`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/src/veranda/utils.py` & `veranda-1.1.0/src/veranda/utils.py`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/src/veranda/vector/native/shp.py` & `veranda-1.1.0/src/veranda/vector/native/shp.py`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/src/veranda.egg-info/PKG-INFO` & `veranda-1.1.0/src/veranda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veranda
-Version: 1.0.1
+Version: 1.1.0
 Summary: veranda is a place for IO related classes and operations dealing with multi-dimensional vector and raster data.
 Home-page: https://github.com/TUW-GEO/veranda
 Author: Research Unit Remote Sensing at GEO Department
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: MIT
 Description: # veranda
         [![Build Status](https://travis-ci.com/TUW-GEO/veranda.svg?branch=master)](https://travis-ci.org/TUW-GEO/veranda)
```

### Comparing `veranda-1.0.1/src/veranda.egg-info/SOURCES.txt` & `veranda-1.1.0/src/veranda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/tests/raster/mosaic/geotiff/test_geotiff.py` & `veranda-1.1.0/tests/raster/mosaic/geotiff/test_geotiff.py`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/tests/raster/mosaic/mosaic_common.py` & `veranda-1.1.0/tests/raster/mosaic/mosaic_common.py`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/tests/raster/mosaic/netcdf/test_netcdf.py` & `veranda-1.1.0/tests/raster/mosaic/netcdf/test_netcdf.py`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/tests/raster/native/geotiff/test_geotiff.py` & `veranda-1.1.0/tests/raster/native/geotiff/test_geotiff.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import pytest
 import numpy as np
 from osgeo import gdal
 from tempfile import mkdtemp
+from zipfile import ZipFile
 
 from veranda.raster.native.geotiff import GeoTiffFile
 
 
 @pytest.fixture
 def filepath():
     return os.path.join(mkdtemp(), 'test.tif')
@@ -133,7 +134,31 @@
         with GeoTiffFile(filepath, mode='w', sref_wkt=sref_ref) as src:
             src.write(data)
 
         with GeoTiffFile(filepath) as src:
             sref_val = src.sref_wkt
 
         assert sref_val == sref_ref
+
+
+def test_read_one_band_zip(filepath):
+
+    data = np.ones((1, 100, 100), dtype=np.float32)
+
+    filename = os.path.basename(filepath)
+    zip_filepath = os.path.splitext(filepath)[0] + r'.zip'
+
+    with ZipFile(zip_filepath, 'w') as zip:
+        with GeoTiffFile(filepath, mode='w') as src:
+            src.write(data)
+        zip.write(filepath)
+
+        in_zip_filename = [name for name in zip.namelist() if name.endswith('.tif')][0]
+
+    read_filepath = os.path.join(zip_filepath, in_zip_filename)
+
+    with GeoTiffFile(read_filepath) as src:
+        ds = src.read()
+
+    np.testing.assert_array_equal(ds[1], data[0, :, :])
+
+    os.remove(zip_filepath)
```

### Comparing `veranda-1.0.1/tests/raster/native/netcdf/netcdf_common.py` & `veranda-1.1.0/tests/raster/native/netcdf/netcdf_common.py`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/tests/raster/native/netcdf/test_netcdf4.py` & `veranda-1.1.0/tests/raster/native/netcdf/test_netcdf4.py`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/tests/raster/native/netcdf/test_xarray.py` & `veranda-1.1.0/tests/raster/native/netcdf/test_xarray.py`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/tests/raster/test_gdal.py` & `veranda-1.1.0/tests/raster/test_gdal.py`

 * *Files identical despite different names*

### Comparing `veranda-1.0.1/tests/raster/test_gdalport.py` & `veranda-1.1.0/tests/raster/test_gdalport.py`

 * *Files identical despite different names*

