# Comparing `tmp/est-0.4.0.tar.gz` & `tmp/est-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/est-0.4.0.tar", last modified: Sun Dec  4 11:09:38 2022, max compression
+gzip compressed data, was "dist/est-0.5.0.tar", last modified: Sun Jul  2 11:10:27 2023, max compression
```

## Comparing `est-0.4.0.tar` & `est-0.5.0.tar`

### file list

```diff
@@ -1,246 +1,246 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1868 2022-12-04 11:03:25.000000 est-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1451 2022-12-04 11:09:38.000000 est-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      652 2022-12-04 11:03:25.000000 est-0.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2022-12-04 11:03:25.000000 est-0.4.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1837 2022-12-04 11:09:38.000000 est-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-12-04 11:03:25.000000 est-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-12-04 11:03:25.000000 est-0.4.0/src/est/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1103 2022-12-04 11:03:25.000000 est-0.4.0/src/est/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/app/
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-12-04 11:03:25.000000 est-0.4.0/src/est/app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/app/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/est/app/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-04 11:03:25.000000 est-0.4.0/src/est/app/utils/url.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2022-12-04 11:03:25.000000 est-0.4.0/src/est/app/utils/xasobj.py
--rw-rw-rw-   0 root         (0) root         (0)     4888 2022-12-04 11:03:25.000000 est-0.4.0/src/est/app/xas_viewer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/core/
--rw-rw-rw-   0 root         (0) root         (0)       68 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6355 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/core/process/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2387 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/energyroi.py
--rw-rw-rw-   0 root         (0) root         (0)      718 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/ignoreprocess.py
--rw-rw-rw-   0 root         (0) root         (0)     1541 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/core/process/larch/
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/larch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4112 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/larch/autobk.py
--rw-rw-rw-   0 root         (0) root         (0)     3667 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/larch/mback.py
--rw-rw-rw-   0 root         (0) root         (0)     3978 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/larch/mback_norm.py
--rw-rw-rw-   0 root         (0) root         (0)     4059 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/larch/pre_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     4748 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/larch/xftf.py
--rw-rw-rw-   0 root         (0) root         (0)     5055 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/noise.py
--rw-rw-rw-   0 root         (0) root         (0)     3123 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/plotspectrumdata.py
--rw-rw-rw-   0 root         (0) root         (0)     3289 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/process.py
--rw-rw-rw-   0 root         (0) root         (0)     1811 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/core/process/pymca/
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/pymca/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5084 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/pymca/exafs.py
--rw-rw-rw-   0 root         (0) root         (0)     5339 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/pymca/ft.py
--rw-rw-rw-   0 root         (0) root         (0)     6385 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/pymca/k_weight.py
--rw-rw-rw-   0 root         (0) root         (0)     5037 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/pymca/normalization.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/roi.py
--rw-rw-rw-   0 root         (0) root         (0)     1027 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/process/setconfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/core/types/
--rw-rw-rw-   0 root         (0) root         (0)      239 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1159 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/types/dimensions.py
--rw-rw-rw-   0 root         (0) root         (0)      231 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/types/sample.py
--rw-rw-rw-   0 root         (0) root         (0)     8477 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/types/spectra.py
--rw-rw-rw-   0 root         (0) root         (0)    14576 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/types/spectrum.py
--rw-rw-rw-   0 root         (0) root         (0)    11557 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/types/xasobject.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/core/utils/
--rw-rw-rw-   0 root         (0) root         (0)      983 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2023 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/utils/converter.py
--rw-rw-rw-   0 root         (0) root         (0)      464 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/utils/designpattern.py
--rw-rw-rw-   0 root         (0) root         (0)      878 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/utils/larchutils.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2022-12-04 11:03:25.000000 est-0.4.0/src/est/core/utils/symbol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/gui/
--rw-rw-rw-   0 root         (0) root         (0)    31641 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/XasObjectViewer.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11555 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/e0calculator.py
--rw-rw-rw-   0 root         (0) root         (0)     4937 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/energyroi.py
--rw-rw-rw-   0 root         (0) root         (0)     2504 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/icons.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/gui/larch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/est/gui/larch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10421 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/larch/autobk.py
--rw-rw-rw-   0 root         (0) root         (0)     8302 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/larch/mback.py
--rw-rw-rw-   0 root         (0) root         (0)     9454 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/larch/pre_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     3450 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/larch/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/larch/xftf.py
--rw-rw-rw-   0 root         (0) root         (0)     8298 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/noise.py
--rw-rw-rw-   0 root         (0) root         (0)      707 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/qtapplicationmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     5507 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/roiselector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/gui/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/est/gui/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1219 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/unit/energy.py
--rw-rw-rw-   0 root         (0) root         (0)    35106 2022-12-04 11:03:25.000000 est-0.4.0/src/est/gui/xas_object_definition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/io/
--rw-rw-rw-   0 root         (0) root         (0)       63 2022-12-04 11:03:25.000000 est-0.4.0/src/est/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17517 2022-12-04 11:03:25.000000 est-0.4.0/src/est/io/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/io/utils/
--rw-rw-rw-   0 root         (0) root         (0)       84 2022-12-04 11:03:25.000000 est-0.4.0/src/est/io/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4478 2022-12-04 11:03:25.000000 est-0.4.0/src/est/io/utils/information.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2022-12-04 11:03:25.000000 est-0.4.0/src/est/io/utils/larch.py
--rw-rw-rw-   0 root         (0) root         (0)     4947 2022-12-04 11:03:25.000000 est-0.4.0/src/est/io/utils/read.py
--rw-rw-rw-   0 root         (0) root         (0)     2909 2022-12-04 11:03:25.000000 est-0.4.0/src/est/io/utils/spec.py
--rw-rw-rw-   0 root         (0) root         (0)     1219 2022-12-04 11:03:25.000000 est-0.4.0/src/est/io/utils/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2556 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/resources/exafs/
--rw-rw-rw-   0 root         (0) root         (0)    27981 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/exafs/EXAFS_Cu.dat
--rw-rw-rw-   0 root         (0) root         (0)    21064 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/exafs/EXAFS_Ge.dat
--rw-rw-rw-   0 root         (0) root         (0)      329 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/exafs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19150 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/exafs/cu_rt01.xmu
--rw-rw-rw-   0 root         (0) root         (0)    10239 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/resources/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/est/resources/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3608 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/icons/est.png
--rw-rw-rw-   0 root         (0) root         (0)     2831 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/icons/est.svg
--rw-rw-rw-   0 root         (0) root         (0)      849 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/icons/item-1dim-black.png
--rw-rw-rw-   0 root         (0) root         (0)     2037 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/icons/item-1dim-black.svg
--rw-rw-rw-   0 root         (0) root         (0)      674 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/icons/item-1dim.png
--rw-rw-rw-   0 root         (0) root         (0)      328 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/icons/item-1dim.svg
--rw-rw-rw-   0 root         (0) root         (0)      991 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/icons/item-1dim_mean.png
--rw-rw-rw-   0 root         (0) root         (0)     2176 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/icons/item-1dim_mean.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/resources/workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/est/resources/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2443 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/workflows/example_bm23.ows
--rw-rw-rw-   0 root         (0) root         (0)     3085 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/workflows/example_larch.ows
--rw-rw-rw-   0 root         (0) root         (0)     3685 2022-12-04 11:03:25.000000 est-0.4.0/src/est/resources/workflows/example_pymca.ows
--rw-rw-rw-   0 root         (0) root         (0)       80 2022-12-04 11:03:25.000000 est-0.4.0/src/est/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/est/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/tests/larch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/est/tests/larch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1633 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/larch/test_autobk.py
--rw-rw-rw-   0 root         (0) root         (0)     2041 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/larch/test_larch_chain.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/larch/test_mback.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/larch/test_mback_norm.py
--rw-rw-rw-   0 root         (0) root         (0)     1824 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/larch/test_pre_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     2560 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/larch/test_xftf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/tests/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/est/tests/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    38284 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/notebooks/larch_xas_processing.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   399418 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/notebooks/pymca_xas_process.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2562 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/nxwriter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/tests/pymca/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/est/tests/pymca/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2199 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/pymca/test_exafs.py
--rw-rw-rw-   0 root         (0) root         (0)     1870 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/pymca/test_ft.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/pymca/test_io_with_pymca.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/pymca/test_k_weight.py
--rw-rw-rw-   0 root         (0) root         (0)     5114 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/pymca/test_pymca_chain.py
--rw-rw-rw-   0 root         (0) root         (0)     2871 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/pymca/test_pymca_normalization.py
--rw-rw-rw-   0 root         (0) root         (0)     2931 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_acquisition.py
--rw-rw-rw-   0 root         (0) root         (0)     1363 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     2954 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_ewoks.py
--rw-rw-rw-   0 root         (0) root         (0)     4912 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_example_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     1611 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_input_information.py
--rw-rw-rw-   0 root         (0) root         (0)     3541 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_io.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_notebooks.py
--rw-rw-rw-   0 root         (0) root         (0)     4325 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_plotspectrumdata.py
--rw-rw-rw-   0 root         (0) root         (0)     2737 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_process_chain.py
--rw-rw-rw-   0 root         (0) root         (0)     1254 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_roi.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_spectra.py
--rw-rw-rw-   0 root         (0) root         (0)      761 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_spectrum.py
--rw-rw-rw-   0 root         (0) root         (0)     3885 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_types.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_url.py
--rw-rw-rw-   0 root         (0) root         (0)     1565 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_write.py
--rw-rw-rw-   0 root         (0) root         (0)     2286 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/test_xas_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/tests/widgets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/est/tests/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1458 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/widgets/test_energyroi.py
--rw-rw-rw-   0 root         (0) root         (0)     1656 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/widgets/test_noise.py
--rw-rw-rw-   0 root         (0) root         (0)     1252 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/widgets/test_roiselector.py
--rw-rw-rw-   0 root         (0) root         (0)     3173 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/widgets/test_xas_input.py
--rw-rw-rw-   0 root         (0) root         (0)      316 2022-12-04 11:03:25.000000 est-0.4.0/src/est/tests/widgets/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est/units/
--rw-rw-rw-   0 root         (0) root         (0)      829 2022-12-04 11:03:25.000000 est-0.4.0/src/est/units/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/est.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1451 2022-12-04 11:09:38.000000 est-0.4.0/src/est.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7868 2022-12-04 11:09:38.000000 est-0.4.0/src/est.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-04 11:09:38.000000 est-0.4.0/src/est.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      218 2022-12-04 11:09:38.000000 est-0.4.0/src/est.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-12-04 11:09:38.000000 est-0.4.0/src/est.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      451 2022-12-04 11:09:38.000000 est-0.4.0/src/est.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-12-04 11:09:38.000000 est-0.4.0/src/est.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/orangecontrib/
--rw-rw-rw-   0 root         (0) root         (0)      164 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/orangecontrib/est/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/orangecontrib/est/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1160 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/orangecontrib/est/screenshots/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/orangecontrib/est/screenshots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   190148 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/screenshots/main_workflow.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/orangecontrib/est/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1178 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2684 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/
--rw-rw-rw-   0 root         (0) root         (0)      208 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5430 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/autobk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3111 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/icons/autobk.png
--rw-rw-rw-   0 root         (0) root         (0)     2151 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/icons/autobk.svg
--rw-rw-rw-   0 root         (0) root         (0)   169850 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/icons/larch.png
--rw-rw-rw-   0 root         (0) root         (0)     2498 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/icons/mback.png
--rw-rw-rw-   0 root         (0) root         (0)     2157 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/icons/mback.svg
--rw-rw-rw-   0 root         (0) root         (0)    19874 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/icons/mbacknorm.svg
--rw-rw-rw-   0 root         (0) root         (0)     2472 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/icons/pre_edge.png
--rw-rw-rw-   0 root         (0) root         (0)     2129 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/icons/pre_edge.svg
--rw-rw-rw-   0 root         (0) root         (0)     1849 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/icons/xftf.png
--rw-rw-rw-   0 root         (0) root         (0)     2123 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/icons/xftf.svg
--rw-rw-rw-   0 root         (0) root         (0)     4242 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/mback.py
--rw-rw-rw-   0 root         (0) root         (0)     4260 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/mback_norm.py
--rw-rw-rw-   0 root         (0) root         (0)     4795 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/pre_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     4709 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/larch/xftf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/orangecontrib/est/widgets/pymca/
--rw-rw-rw-   0 root         (0) root         (0)      206 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/pymca/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4118 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/pymca/exafs.py
--rw-rw-rw-   0 root         (0) root         (0)     4779 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/pymca/ft.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/orangecontrib/est/widgets/pymca/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/orangecontrib/est/widgets/pymca/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3991 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/pymca/icons/exafs.png
--rw-rw-rw-   0 root         (0) root         (0)     1686 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/pymca/icons/ft.png
--rw-rw-rw-   0 root         (0) root         (0)     1671 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/pymca/icons/k_weight.png
--rw-rw-rw-   0 root         (0) root         (0)     3033 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/pymca/icons/normalization.png
--rw-rw-rw-   0 root         (0) root         (0)   158500 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/pymca/icons/pymca.png
--rw-rw-rw-   0 root         (0) root         (0)     2033 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/pymca/k_weight.py
--rw-rw-rw-   0 root         (0) root         (0)     7575 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/pymca/normalization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/
--rw-rw-rw-   0 root         (0) root         (0)      236 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1276 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/converter.py
--rw-rw-rw-   0 root         (0) root         (0)     3120 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/e0calculator.py
--rw-rw-rw-   0 root         (0) root         (0)     3303 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/energyroi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-04 11:09:38.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-04 11:09:32.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4212 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/converter.png
--rw-rw-rw-   0 root         (0) root         (0)     5189 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/converter.svg
--rw-rw-rw-   0 root         (0) root         (0)      978 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/curveroi.png
--rw-rw-rw-   0 root         (0) root         (0)     2766 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/curveroi.svg
--rw-rw-rw-   0 root         (0) root         (0)      370 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/e0.png
--rw-rw-rw-   0 root         (0) root         (0)     3923 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/e0.svg
--rw-rw-rw-   0 root         (0) root         (0)      143 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/iconverter.png
--rw-rw-rw-   0 root         (0) root         (0)     5200 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/iconverter.svg
--rwxrwxrwx   0 root         (0) root         (0)     3036 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/image-select-box.png
--rw-rw-rw-   0 root         (0) root         (0)    64642 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/image-select-box.svg
--rw-rw-rw-   0 root         (0) root         (0)    98073 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/input.png
--rw-rw-rw-   0 root         (0) root         (0)      520 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/noise.png
--rw-rw-rw-   0 root         (0) root         (0)     2250 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/noise.svg
--rw-rw-rw-   0 root         (0) root         (0)    77669 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/output.png
--rw-rw-rw-   0 root         (0) root         (0)     5909 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/plot_spectrum.png
--rw-rw-rw-   0 root         (0) root         (0)    22339 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/plot_spectrum.svg
--rwxrwxrwx   0 root         (0) root         (0)      535 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/saving.png
--rw-rw-rw-   0 root         (0) root         (0)      749 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/saving.svg
--rw-rw-rw-   0 root         (0) root         (0)     3704 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/xas.png
--rw-rw-rw-   0 root         (0) root         (0)     3174 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/icons/xas.svg
--rw-rw-rw-   0 root         (0) root         (0)     1326 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/iconverter.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/noise.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/plotspectrumdata.py
--rw-rw-rw-   0 root         (0) root         (0)     3560 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/roi.py
--rw-rw-rw-   0 root         (0) root         (0)     8278 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/xas_input.py
--rw-rw-rw-   0 root         (0) root         (0)     3459 2022-12-04 11:03:25.000000 est-0.4.0/src/orangecontrib/est/widgets/utils/xas_output.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2023-07-02 11:03:12.000000 est-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-07-02 11:10:27.000000 est-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-07-02 11:03:12.000000 est-0.5.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-02 11:03:12.000000 est-0.5.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2023-07-02 11:10:27.000000 est-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-02 11:03:12.000000 est-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-02 11:03:12.000000 est-0.5.0/src/est/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-07-02 11:03:12.000000 est-0.5.0/src/est/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/app/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-07-02 11:03:12.000000 est-0.5.0/src/est/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/app/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/est/app/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-02 11:03:12.000000 est-0.5.0/src/est/app/utils/url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-02 11:03:12.000000 est-0.5.0/src/est/app/utils/xasobj.py
+-rw-rw-rw-   0 root         (0) root         (0)     4888 2023-07-02 11:03:12.000000 est-0.5.0/src/est/app/xas_viewer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/core/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6355 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/core/process/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/energyroi.py
+-rw-rw-rw-   0 root         (0) root         (0)      718 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/ignoreprocess.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/core/process/larch/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/larch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4112 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/larch/autobk.py
+-rw-rw-rw-   0 root         (0) root         (0)     3667 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/larch/mback.py
+-rw-rw-rw-   0 root         (0) root         (0)     3978 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/larch/mback_norm.py
+-rw-rw-rw-   0 root         (0) root         (0)     4059 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/larch/pre_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     4748 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/larch/xftf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5055 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/noise.py
+-rw-rw-rw-   0 root         (0) root         (0)     3123 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/plotspectrumdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     3289 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/process.py
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/core/process/pymca/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/pymca/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5084 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/pymca/exafs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5339 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/pymca/ft.py
+-rw-rw-rw-   0 root         (0) root         (0)     6385 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/pymca/k_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)     5037 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/pymca/normalization.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/roi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/process/setconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/core/types/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/types/dimensions.py
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/types/sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     8477 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/types/spectra.py
+-rw-rw-rw-   0 root         (0) root         (0)    14575 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/types/spectrum.py
+-rw-rw-rw-   0 root         (0) root         (0)    11557 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/types/xasobject.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/core/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2023 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/utils/converter.py
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/utils/designpattern.py
+-rw-rw-rw-   0 root         (0) root         (0)      878 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/utils/larchutils.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-02 11:03:12.000000 est-0.5.0/src/est/core/utils/symbol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/gui/
+-rw-rw-rw-   0 root         (0) root         (0)    31640 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/XasObjectViewer.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11555 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/e0calculator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4955 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/energyroi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2504 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/icons.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/gui/larch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/est/gui/larch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10421 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/larch/autobk.py
+-rw-rw-rw-   0 root         (0) root         (0)     8302 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/larch/mback.py
+-rw-rw-rw-   0 root         (0) root         (0)     9454 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/larch/pre_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     3450 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/larch/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/larch/xftf.py
+-rw-rw-rw-   0 root         (0) root         (0)     8298 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/noise.py
+-rw-rw-rw-   0 root         (0) root         (0)      707 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/qtapplicationmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5507 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/roiselector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/gui/unit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/est/gui/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1219 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/unit/energy.py
+-rw-rw-rw-   0 root         (0) root         (0)    35106 2023-07-02 11:03:12.000000 est-0.5.0/src/est/gui/xas_object_definition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/io/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-02 11:03:12.000000 est-0.5.0/src/est/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17517 2023-07-02 11:03:12.000000 est-0.5.0/src/est/io/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/io/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-02 11:03:12.000000 est-0.5.0/src/est/io/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4478 2023-07-02 11:03:12.000000 est-0.5.0/src/est/io/utils/information.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-07-02 11:03:12.000000 est-0.5.0/src/est/io/utils/larch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4947 2023-07-02 11:03:12.000000 est-0.5.0/src/est/io/utils/read.py
+-rw-rw-rw-   0 root         (0) root         (0)     2909 2023-07-02 11:03:12.000000 est-0.5.0/src/est/io/utils/spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     1219 2023-07-02 11:03:12.000000 est-0.5.0/src/est/io/utils/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2556 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/resources/exafs/
+-rw-rw-rw-   0 root         (0) root         (0)    27981 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/exafs/EXAFS_Cu.dat
+-rw-rw-rw-   0 root         (0) root         (0)    21064 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/exafs/EXAFS_Ge.dat
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/exafs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19150 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/exafs/cu_rt01.xmu
+-rw-rw-rw-   0 root         (0) root         (0)    10239 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/resources/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/est/resources/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3608 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/icons/est.png
+-rw-rw-rw-   0 root         (0) root         (0)     2831 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/icons/est.svg
+-rw-rw-rw-   0 root         (0) root         (0)      849 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/icons/item-1dim-black.png
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/icons/item-1dim-black.svg
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/icons/item-1dim.png
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/icons/item-1dim.svg
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/icons/item-1dim_mean.png
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/icons/item-1dim_mean.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/resources/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/est/resources/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2443 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/workflows/example_bm23.ows
+-rw-rw-rw-   0 root         (0) root         (0)     3085 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/workflows/example_larch.ows
+-rw-rw-rw-   0 root         (0) root         (0)     3685 2023-07-02 11:03:12.000000 est-0.5.0/src/est/resources/workflows/example_pymca.ows
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-02 11:03:12.000000 est-0.5.0/src/est/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/est/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/tests/larch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/est/tests/larch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1633 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/larch/test_autobk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2041 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/larch/test_larch_chain.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/larch/test_mback.py
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/larch/test_mback_norm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1824 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/larch/test_pre_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     2560 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/larch/test_xftf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/tests/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/est/tests/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    38284 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/notebooks/larch_xas_processing.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   399418 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/notebooks/pymca_xas_process.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/nxwriter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/tests/pymca/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/est/tests/pymca/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2199 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/pymca/test_exafs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/pymca/test_ft.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/pymca/test_io_with_pymca.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/pymca/test_k_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)     5114 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/pymca/test_pymca_chain.py
+-rw-rw-rw-   0 root         (0) root         (0)     2871 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/pymca/test_pymca_normalization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_acquisition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2954 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_ewoks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4912 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_example_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_input_information.py
+-rw-rw-rw-   0 root         (0) root         (0)     3541 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_io.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_notebooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4325 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_plotspectrumdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2737 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_process_chain.py
+-rw-rw-rw-   0 root         (0) root         (0)     1254 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_roi.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_spectra.py
+-rw-rw-rw-   0 root         (0) root         (0)      761 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_spectrum.py
+-rw-rw-rw-   0 root         (0) root         (0)     3885 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_write.py
+-rw-rw-rw-   0 root         (0) root         (0)     2286 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/test_xas_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/tests/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/est/tests/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1458 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/widgets/test_energyroi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1656 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/widgets/test_noise.py
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/widgets/test_roiselector.py
+-rw-rw-rw-   0 root         (0) root         (0)     3173 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/widgets/test_xas_input.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-07-02 11:03:12.000000 est-0.5.0/src/est/tests/widgets/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est/units/
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-02 11:03:12.000000 est-0.5.0/src/est/units/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/est.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-07-02 11:10:27.000000 est-0.5.0/src/est.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7868 2023-07-02 11:10:27.000000 est-0.5.0/src/est.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 11:10:27.000000 est-0.5.0/src/est.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      264 2023-07-02 11:10:27.000000 est-0.5.0/src/est.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-02 11:10:27.000000 est-0.5.0/src/est.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      472 2023-07-02 11:10:27.000000 est-0.5.0/src/est.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-02 11:10:27.000000 est-0.5.0/src/est.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/orangecontrib/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/orangecontrib/est/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/orangecontrib/est/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/orangecontrib/est/screenshots/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/orangecontrib/est/screenshots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   190148 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/screenshots/main_workflow.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/orangecontrib/est/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2684 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5430 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/autobk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3111 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/icons/autobk.png
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/icons/autobk.svg
+-rw-rw-rw-   0 root         (0) root         (0)   169850 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/icons/larch.png
+-rw-rw-rw-   0 root         (0) root         (0)     2498 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/icons/mback.png
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/icons/mback.svg
+-rw-rw-rw-   0 root         (0) root         (0)    19874 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/icons/mbacknorm.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/icons/pre_edge.png
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/icons/pre_edge.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/icons/xftf.png
+-rw-rw-rw-   0 root         (0) root         (0)     2123 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/icons/xftf.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4242 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/mback.py
+-rw-rw-rw-   0 root         (0) root         (0)     4260 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/mback_norm.py
+-rw-rw-rw-   0 root         (0) root         (0)     4795 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/pre_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     4709 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/larch/xftf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/orangecontrib/est/widgets/pymca/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/pymca/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4118 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/pymca/exafs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4779 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/pymca/ft.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/orangecontrib/est/widgets/pymca/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/orangecontrib/est/widgets/pymca/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3991 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/pymca/icons/exafs.png
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/pymca/icons/ft.png
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/pymca/icons/k_weight.png
+-rw-rw-rw-   0 root         (0) root         (0)     3033 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/pymca/icons/normalization.png
+-rw-rw-rw-   0 root         (0) root         (0)   158500 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/pymca/icons/pymca.png
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/pymca/k_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)     7575 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/pymca/normalization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1276 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3120 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/e0calculator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3303 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/energyroi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:10:27.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:10:21.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4212 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/converter.png
+-rw-rw-rw-   0 root         (0) root         (0)     5189 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/converter.svg
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/curveroi.png
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/curveroi.svg
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/e0.png
+-rw-rw-rw-   0 root         (0) root         (0)     3923 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/e0.svg
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/iconverter.png
+-rw-rw-rw-   0 root         (0) root         (0)     5200 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/iconverter.svg
+-rwxrwxrwx   0 root         (0) root         (0)     3036 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/image-select-box.png
+-rw-rw-rw-   0 root         (0) root         (0)    64642 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/image-select-box.svg
+-rw-rw-rw-   0 root         (0) root         (0)    98073 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/input.png
+-rw-rw-rw-   0 root         (0) root         (0)      520 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/noise.png
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/noise.svg
+-rw-rw-rw-   0 root         (0) root         (0)    77669 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/output.png
+-rw-rw-rw-   0 root         (0) root         (0)     5909 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/plot_spectrum.png
+-rw-rw-rw-   0 root         (0) root         (0)    22339 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/plot_spectrum.svg
+-rwxrwxrwx   0 root         (0) root         (0)      535 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/saving.png
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/saving.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/xas.png
+-rw-rw-rw-   0 root         (0) root         (0)     3174 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/icons/xas.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/iconverter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/noise.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/plotspectrumdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     3560 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/roi.py
+-rw-rw-rw-   0 root         (0) root         (0)     8278 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/xas_input.py
+-rw-rw-rw-   0 root         (0) root         (0)     3459 2023-07-02 11:03:12.000000 est-0.5.0/src/orangecontrib/est/widgets/utils/xas_output.py
```

### Comparing `est-0.4.0/LICENSE` & `est-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `est-0.4.0/PKG-INFO` & `est-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: est
-Version: 0.4.0
+Version: 0.5.0
 Summary: Spectroscopy workflows
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/est
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/est/
 Project-URL: Documentation, https://ewoksest.readthedocs.io/
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoksapps/est/issues/
+Keywords: orange3 add-on,ewoks
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pymca
 Provides-Extra: larch
@@ -37,13 +38,13 @@
 ``` python
 pip install est[full]
 ```
 
 ## Test
 
 ```bash
-python3 -m pytest --pyargs est.tests
+pytest --pyargs est.tests
 ```
 
 ## Documentation
 
 https://ewoksest.readthedocs.io/
```

### Comparing `est-0.4.0/README.md` & `est-0.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 ``` python
 pip install est[full]
 ```
 
 ## Test
 
 ```bash
-python3 -m pytest --pyargs est.tests
+pytest --pyargs est.tests
 ```
 
 ## Documentation
 
 https://ewoksest.readthedocs.io/
```

### Comparing `est-0.4.0/setup.cfg` & `est-0.5.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 	Source = https://gitlab.esrf.fr/workflow/ewoksapps/est/
 	Documentation = https://ewoksest.readthedocs.io/
 	Tracker = https://gitlab.esrf.fr/workflow/ewoksapps/est/issues/
 classifiers = 
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
+keywords = 
+	orange3 add-on,ewoks
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.6
 install_requires = 
@@ -40,21 +42,23 @@
 	est=est.__main__:main
 orange3.addon = 
 	est-add-on=orangecontrib.est
 orange.widgets = 
 	Est=orangecontrib.est.widgets
 orange.canvas.help = 
 	html-index=orangecontrib.est.widgets:WIDGET_HELP_PATH
+ewoks.tasks.class = 
+	est.core.process.*=est
 
 [options.package_data]
 * = *.ows, *.png, *.svg, *.dat, *.xmu, *.ipynb
 
 [options.extras_require]
 pymca = 
-	pymca
+	pymca >=5.8.1
 larch = 
 	xraylarch >=0.9.64
 	sqlalchemy <2
 orange = 
 	Orange3
 full = 
 	%(pymca)s
@@ -90,16 +94,11 @@
 max-line-length = 88
 
 [coverage:run]
 omit = 
 	setup.py
 	*/tests/*
 
-[build_sphinx]
-project = est
-version = attr: est.__version__
-source-dir = ./doc
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `est-0.4.0/src/est/__main__.py` & `est-0.5.0/src/est/__main__.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/app/utils/url.py` & `est-0.5.0/src/est/app/utils/url.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/app/utils/xasobj.py` & `est-0.5.0/src/est/app/utils/xasobj.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/app/xas_viewer.py` & `est-0.5.0/src/est/app/xas_viewer.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/io.py` & `est-0.5.0/src/est/core/io.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/energyroi.py` & `est-0.5.0/src/est/core/process/energyroi.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/ignoreprocess.py` & `est-0.5.0/src/est/core/process/ignoreprocess.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/io.py` & `est-0.5.0/src/est/core/process/io.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/larch/autobk.py` & `est-0.5.0/src/est/core/process/larch/autobk.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/larch/mback.py` & `est-0.5.0/src/est/core/process/larch/mback.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/larch/mback_norm.py` & `est-0.5.0/src/est/core/process/larch/mback_norm.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/larch/pre_edge.py` & `est-0.5.0/src/est/core/process/larch/pre_edge.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/larch/xftf.py` & `est-0.5.0/src/est/core/process/larch/xftf.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/noise.py` & `est-0.5.0/src/est/core/process/noise.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/plotspectrumdata.py` & `est-0.5.0/src/est/core/process/plotspectrumdata.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/process.py` & `est-0.5.0/src/est/core/process/process.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/progress.py` & `est-0.5.0/src/est/core/process/progress.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/pymca/exafs.py` & `est-0.5.0/src/est/core/process/pymca/exafs.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/pymca/ft.py` & `est-0.5.0/src/est/core/process/pymca/ft.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/pymca/k_weight.py` & `est-0.5.0/src/est/core/process/pymca/k_weight.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/pymca/normalization.py` & `est-0.5.0/src/est/core/process/pymca/normalization.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/roi.py` & `est-0.5.0/src/est/core/process/roi.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/process/setconfig.py` & `est-0.5.0/src/est/core/process/setconfig.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/types/dimensions.py` & `est-0.5.0/src/est/core/types/dimensions.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/types/spectra.py` & `est-0.5.0/src/est/core/types/spectra.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/types/spectrum.py` & `est-0.5.0/src/est/core/types/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,14 @@
         the indexes should be defined during Spectra or Spectrum construction
         once for all"""
         self.__x = x
         self.__y = y
 
 
 class _FT:
-
     _RADIUS_KEY = "FTRadius"
 
     _INTENSITY_KEY = "FTIntensity"
 
     _IMAGINARY_KEY = "FTImaginary"
 
     def __init__(self, ddict):
```

### Comparing `est-0.4.0/src/est/core/types/xasobject.py` & `est-0.5.0/src/est/core/types/xasobject.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/utils/__init__.py` & `est-0.5.0/src/est/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/utils/converter.py` & `est-0.5.0/src/est/core/utils/converter.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/core/utils/larchutils.py` & `est-0.5.0/src/est/core/utils/larchutils.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/gui/XasObjectViewer.py` & `est-0.5.0/src/est/gui/XasObjectViewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,14 @@
         self.setRowCount(0)
         self.setColumnCount(2)
         self.setSortingEnabled(True)
         self.verticalHeader().hide()
 
 
 class SpectrumViewer(qt.QMainWindow):
-
     sigSpectrumChanged = qt.Signal()
     """Signal emitted when the spectrum change"""
 
     def __init__(self, parent=None):
         self._curveOperations = []
         """List of callaback to produce plot regarding the XASObject.
         Callback function should return a _curve_operation"""
```

### Comparing `est-0.4.0/src/est/gui/e0calculator.py` & `est-0.5.0/src/est/gui/e0calculator.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/gui/energyroi.py` & `est-0.5.0/src/est/gui/energyroi.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from silx.gui import qt
 from est.core.types.xasobject import XASObject
 from est.gui.xas_object_definition import _SpectrumPlot
 from ewokscore.missing_data import is_missing_data
 
 
 class _RoiSettings(qt.QWidget):
-
     sigValueChanged = qt.Signal()
     """signal emitted when roi value is changed"""
 
     MAX_VALUE = 999999999
 
     def __init__(self, parent=None):
         qt.QWidget.__init__(self, parent)
@@ -109,15 +108,15 @@
 
         # connect signal / slot
         self._widget.sigValueChanged.connect(self._updateROIAnchors)
         self._getMinMarker().sigDragFinished.connect(self._updateMinValuefrmMarker)
         self._getMaxMarker().sigDragFinished.connect(self._updateMaxValuefrmMarker)
 
     def setXasObject(self, xas_obj):
-        if is_missing_data(xas_obj):
+        if is_missing_data(xas_obj) or xas_obj is None:
             self._plot.clear()
         else:
             self._plot.setXasObject(xas_obj)
             if self._widget.hasntBeenModified() and xas_obj.energy is not None:
                 self._widget.setRangeE(xas_obj.energy.min(), xas_obj.energy.max())
 
     def getXasObject(self) -> Optional[XASObject]:
```

### Comparing `est-0.4.0/src/est/gui/icons.py` & `est-0.5.0/src/est/gui/icons.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/gui/larch/autobk.py` & `est-0.5.0/src/est/gui/larch/autobk.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/gui/larch/mback.py` & `est-0.5.0/src/est/gui/larch/mback.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/gui/larch/pre_edge.py` & `est-0.5.0/src/est/gui/larch/pre_edge.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/gui/larch/utils.py` & `est-0.5.0/src/est/gui/larch/utils.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/gui/larch/xftf.py` & `est-0.5.0/src/est/gui/larch/xftf.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/gui/noise.py` & `est-0.5.0/src/est/gui/noise.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/gui/qtapplicationmanager.py` & `est-0.5.0/src/est/gui/qtapplicationmanager.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/gui/roiselector.py` & `est-0.5.0/src/est/gui/roiselector.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/gui/unit/energy.py` & `est-0.5.0/src/est/gui/unit/energy.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/gui/xas_object_definition.py` & `est-0.5.0/src/est/gui/xas_object_definition.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/io/io.py` & `est-0.5.0/src/est/io/io.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/io/utils/information.py` & `est-0.5.0/src/est/io/utils/information.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/io/utils/read.py` & `est-0.5.0/src/est/io/utils/read.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/io/utils/spec.py` & `est-0.5.0/src/est/io/utils/spec.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/io/utils/url.py` & `est-0.5.0/src/est/io/utils/url.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/__init__.py` & `est-0.5.0/src/est/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/exafs/EXAFS_Cu.dat` & `est-0.5.0/src/est/resources/exafs/EXAFS_Cu.dat`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/exafs/EXAFS_Ge.dat` & `est-0.5.0/src/est/resources/exafs/EXAFS_Ge.dat`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/exafs/cu_rt01.xmu` & `est-0.5.0/src/est/resources/exafs/cu_rt01.xmu`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/generate.py` & `est-0.5.0/src/est/resources/generate.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/icons/est.png` & `est-0.5.0/src/est/resources/icons/est.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/icons/est.svg` & `est-0.5.0/src/est/resources/icons/est.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/icons/item-1dim-black.png` & `est-0.5.0/src/est/resources/icons/item-1dim-black.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/icons/item-1dim-black.svg` & `est-0.5.0/src/est/resources/icons/item-1dim-black.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/icons/item-1dim.png` & `est-0.5.0/src/est/resources/icons/item-1dim.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/icons/item-1dim_mean.png` & `est-0.5.0/src/est/resources/icons/item-1dim_mean.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/icons/item-1dim_mean.svg` & `est-0.5.0/src/est/resources/icons/item-1dim_mean.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/workflows/example_bm23.ows` & `est-0.5.0/src/est/resources/workflows/example_bm23.ows`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/workflows/example_larch.ows` & `est-0.5.0/src/est/resources/workflows/example_larch.ows`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/resources/workflows/example_pymca.ows` & `est-0.5.0/src/est/resources/workflows/example_pymca.ows`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/conftest.py` & `est-0.5.0/src/est/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/data.py` & `est-0.5.0/src/est/tests/data.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/larch/test_autobk.py` & `est-0.5.0/src/est/tests/larch/test_autobk.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/larch/test_larch_chain.py` & `est-0.5.0/src/est/tests/larch/test_larch_chain.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/larch/test_mback.py` & `est-0.5.0/src/est/tests/larch/test_mback.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/larch/test_mback_norm.py` & `est-0.5.0/src/est/tests/larch/test_mback_norm.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/larch/test_pre_edge.py` & `est-0.5.0/src/est/tests/larch/test_pre_edge.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/larch/test_xftf.py` & `est-0.5.0/src/est/tests/larch/test_xftf.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/notebooks/larch_xas_processing.ipynb` & `est-0.5.0/src/est/tests/notebooks/larch_xas_processing.ipynb`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/notebooks/pymca_xas_process.ipynb` & `est-0.5.0/src/est/tests/notebooks/pymca_xas_process.ipynb`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/nxwriter.py` & `est-0.5.0/src/est/tests/nxwriter.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/pymca/test_exafs.py` & `est-0.5.0/src/est/tests/pymca/test_exafs.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/pymca/test_ft.py` & `est-0.5.0/src/est/tests/pymca/test_ft.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/pymca/test_io_with_pymca.py` & `est-0.5.0/src/est/tests/pymca/test_io_with_pymca.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/pymca/test_k_weight.py` & `est-0.5.0/src/est/tests/pymca/test_k_weight.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/pymca/test_pymca_chain.py` & `est-0.5.0/src/est/tests/pymca/test_pymca_chain.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/pymca/test_pymca_normalization.py` & `est-0.5.0/src/est/tests/pymca/test_pymca_normalization.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_acquisition.py` & `est-0.5.0/src/est/tests/test_acquisition.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_converter.py` & `est-0.5.0/src/est/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_ewoks.py` & `est-0.5.0/src/est/tests/test_ewoks.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_example_workflows.py` & `est-0.5.0/src/est/tests/test_example_workflows.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_input_information.py` & `est-0.5.0/src/est/tests/test_input_information.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_io.py` & `est-0.5.0/src/est/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_plotspectrumdata.py` & `est-0.5.0/src/est/tests/test_plotspectrumdata.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_process_chain.py` & `est-0.5.0/src/est/tests/test_process_chain.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_roi.py` & `est-0.5.0/src/est/tests/test_roi.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_spectra.py` & `est-0.5.0/src/est/tests/test_spectra.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_spectrum.py` & `est-0.5.0/src/est/tests/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_types.py` & `est-0.5.0/src/est/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_url.py` & `est-0.5.0/src/est/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_write.py` & `est-0.5.0/src/est/tests/test_write.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/test_xas_object.py` & `est-0.5.0/src/est/tests/test_xas_object.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/widgets/test_energyroi.py` & `est-0.5.0/src/est/tests/widgets/test_energyroi.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/widgets/test_noise.py` & `est-0.5.0/src/est/tests/widgets/test_noise.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/widgets/test_roiselector.py` & `est-0.5.0/src/est/tests/widgets/test_roiselector.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/tests/widgets/test_xas_input.py` & `est-0.5.0/src/est/tests/widgets/test_xas_input.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est/units/__init__.py` & `est-0.5.0/src/est/units/__init__.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/est.egg-info/PKG-INFO` & `est-0.5.0/src/est.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: est
-Version: 0.4.0
+Version: 0.5.0
 Summary: Spectroscopy workflows
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/est
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/est/
 Project-URL: Documentation, https://ewoksest.readthedocs.io/
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoksapps/est/issues/
+Keywords: orange3 add-on,ewoks
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pymca
 Provides-Extra: larch
@@ -37,13 +38,13 @@
 ``` python
 pip install est[full]
 ```
 
 ## Test
 
 ```bash
-python3 -m pytest --pyargs est.tests
+pytest --pyargs est.tests
 ```
 
 ## Documentation
 
 https://ewoksest.readthedocs.io/
```

### Comparing `est-0.4.0/src/est.egg-info/SOURCES.txt` & `est-0.5.0/src/est.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/process.py` & `est-0.5.0/src/orangecontrib/est/process.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/screenshots/main_workflow.png` & `est-0.5.0/src/orangecontrib/est/screenshots/main_workflow.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/__init__.py` & `est-0.5.0/src/orangecontrib/est/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/container.py` & `est-0.5.0/src/orangecontrib/est/widgets/container.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/autobk.py` & `est-0.5.0/src/orangecontrib/est/widgets/larch/autobk.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/icons/autobk.png` & `est-0.5.0/src/orangecontrib/est/widgets/larch/icons/autobk.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/icons/autobk.svg` & `est-0.5.0/src/orangecontrib/est/widgets/larch/icons/autobk.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/icons/larch.png` & `est-0.5.0/src/orangecontrib/est/widgets/larch/icons/larch.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/icons/mback.png` & `est-0.5.0/src/orangecontrib/est/widgets/larch/icons/mback.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/icons/mback.svg` & `est-0.5.0/src/orangecontrib/est/widgets/larch/icons/mback.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/icons/mbacknorm.svg` & `est-0.5.0/src/orangecontrib/est/widgets/larch/icons/mbacknorm.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/icons/pre_edge.png` & `est-0.5.0/src/orangecontrib/est/widgets/larch/icons/pre_edge.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/icons/pre_edge.svg` & `est-0.5.0/src/orangecontrib/est/widgets/larch/icons/pre_edge.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/icons/xftf.png` & `est-0.5.0/src/orangecontrib/est/widgets/larch/icons/xftf.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/icons/xftf.svg` & `est-0.5.0/src/orangecontrib/est/widgets/larch/icons/xftf.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/mback.py` & `est-0.5.0/src/orangecontrib/est/widgets/larch/mback.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/mback_norm.py` & `est-0.5.0/src/orangecontrib/est/widgets/larch/mback_norm.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/pre_edge.py` & `est-0.5.0/src/orangecontrib/est/widgets/larch/pre_edge.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/larch/xftf.py` & `est-0.5.0/src/orangecontrib/est/widgets/larch/xftf.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/pymca/exafs.py` & `est-0.5.0/src/orangecontrib/est/widgets/pymca/exafs.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/pymca/ft.py` & `est-0.5.0/src/orangecontrib/est/widgets/pymca/ft.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/pymca/icons/exafs.png` & `est-0.5.0/src/orangecontrib/est/widgets/pymca/icons/exafs.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/pymca/icons/ft.png` & `est-0.5.0/src/orangecontrib/est/widgets/pymca/icons/ft.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/pymca/icons/k_weight.png` & `est-0.5.0/src/orangecontrib/est/widgets/pymca/icons/k_weight.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/pymca/icons/normalization.png` & `est-0.5.0/src/orangecontrib/est/widgets/pymca/icons/normalization.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/pymca/icons/pymca.png` & `est-0.5.0/src/orangecontrib/est/widgets/pymca/icons/pymca.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/pymca/k_weight.py` & `est-0.5.0/src/orangecontrib/est/widgets/pymca/k_weight.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/pymca/normalization.py` & `est-0.5.0/src/orangecontrib/est/widgets/pymca/normalization.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/converter.py` & `est-0.5.0/src/orangecontrib/est/widgets/utils/converter.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/e0calculator.py` & `est-0.5.0/src/orangecontrib/est/widgets/utils/e0calculator.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/energyroi.py` & `est-0.5.0/src/orangecontrib/est/widgets/utils/energyroi.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/converter.png` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/converter.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/converter.svg` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/converter.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/curveroi.png` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/curveroi.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/curveroi.svg` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/curveroi.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/e0.svg` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/e0.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/iconverter.svg` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/iconverter.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/image-select-box.png` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/image-select-box.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/image-select-box.svg` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/image-select-box.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/input.png` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/input.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/noise.png` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/noise.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/noise.svg` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/noise.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/output.png` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/output.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/plot_spectrum.png` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/plot_spectrum.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/plot_spectrum.svg` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/plot_spectrum.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/saving.png` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/saving.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/saving.svg` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/saving.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/xas.png` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/xas.png`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/icons/xas.svg` & `est-0.5.0/src/orangecontrib/est/widgets/utils/icons/xas.svg`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/iconverter.py` & `est-0.5.0/src/orangecontrib/est/widgets/utils/iconverter.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/noise.py` & `est-0.5.0/src/orangecontrib/est/widgets/utils/noise.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/roi.py` & `est-0.5.0/src/orangecontrib/est/widgets/utils/roi.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/xas_input.py` & `est-0.5.0/src/orangecontrib/est/widgets/utils/xas_input.py`

 * *Files identical despite different names*

### Comparing `est-0.4.0/src/orangecontrib/est/widgets/utils/xas_output.py` & `est-0.5.0/src/orangecontrib/est/widgets/utils/xas_output.py`

 * *Files identical despite different names*

