# Comparing `tmp/ewoksxrpd-0.3.0.tar.gz` & `tmp/ewoksxrpd-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksxrpd-0.3.0.tar", last modified: Tue Apr 25 12:03:30 2023, max compression
+gzip compressed data, was "dist/ewoksxrpd-0.4.0.tar", last modified: Mon Jul  3 06:52:21 2023, max compression
```

## Comparing `ewoksxrpd-0.3.0.tar` & `ewoksxrpd-0.4.0.tar`

### file list

```diff
@@ -1,86 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1299 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1605 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 12:03:24.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20304 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     2667 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/gui/plots.py
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/gui/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     5302 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/gui/trigger_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     1582 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/init_matplotlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/ascii.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/background.py
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/bliss.py
--rw-rw-rw-   0 root         (0) root         (0)    15723 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/calibrate.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/convolution.py
--rw-rw-rw-   0 root         (0) root         (0)     2036 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/data_access.py
--rw-rw-rw-   0 root         (0) root         (0)     8789 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/diagnostics.py
--rw-rw-rw-   0 root         (0) root         (0)    14901 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/integrate.py
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/mask.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/morphology.py
--rw-rw-rw-   0 root         (0) root         (0)     3334 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     4144 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/pyfaiconfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 12:03:24.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2745 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/data_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/integrate_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9454 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/pyfai_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1774 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4419 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 12:03:24.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5823 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1629 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_ascii.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_background.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_batch_integrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1806 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py
--rw-rw-rw-   0 root         (0) root         (0)    10366 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_calibrate.py
--rw-rw-rw-   0 root         (0) root         (0)    20665 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_calint_workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     4297 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_integrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_mask.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     3795 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_nexus_integrated.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_pyfai_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1850 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/ewoksxrpd/tests/xrpd_theory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1299 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2668 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      177 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      257 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/orangecontrib/
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/ascii.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/background.py
--rw-rw-rw-   0 root         (0) root         (0)     1350 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/batchintegrate.py
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py
--rw-rw-rw-   0 root         (0) root         (0)     1510 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/calculategeometry.py
--rw-rw-rw-   0 root         (0) root         (0)    11135 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/calibratemulti.py
--rw-rw-rw-   0 root         (0) root         (0)     7826 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/calibratesingle.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py
--rw-rw-rw-   0 root         (0) root         (0)     1527 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 12:03:24.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   188527 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/icons/category.png
--rw-rw-rw-   0 root         (0) root         (0)   188527 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/icons/widget.png
--rw-rw-rw-   0 root         (0) root         (0)     2167 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/integrate1d.py
--rw-rw-rw-   0 root         (0) root         (0)     3246 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/mask.py
--rw-rw-rw-   0 root         (0) root         (0)     1958 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py
--rw-rw-rw-   0 root         (0) root         (0)     1396 2023-04-25 11:52:28.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 12:03:30.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 12:03:24.000000 ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/tutorials/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 06:52:15.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20304 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/gui/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)      960 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/gui/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     5302 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/gui/trigger_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     1582 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/init_matplotlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 06:52:15.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/ascii.py
+-rw-rw-rw-   0 root         (0) root         (0)      676 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/background.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)    15791 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/calibrate.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/convolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/data_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     8946 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/diagnostics.py
+-rw-rw-rw-   0 root         (0) root         (0)    18974 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/mask.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/morphology.py
+-rw-rw-rw-   0 root         (0) root         (0)     4159 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     4267 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/pyfaiconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/save_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     4876 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/sum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 06:52:15.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3754 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/data_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/integrate_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    10315 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/pyfai_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1774 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4419 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 06:52:15.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6318 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_ascii.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_background.py
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_batch_integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1806 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py
+-rw-rw-rw-   0 root         (0) root         (0)    10366 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_calibrate.py
+-rw-rw-rw-   0 root         (0) root         (0)    20665 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_calint_workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     4679 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     3795 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_nexus_integrated.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_pyfai_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_save_images.py
+-rw-rw-rw-   0 root         (0) root         (0)      683 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_sum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1850 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/xrpd_theory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2802 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      228 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      259 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/orangecontrib/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1448 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/ascii.py
+-rw-rw-rw-   0 root         (0) root         (0)     2635 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/background.py
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/batchintegrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/calculategeometry.py
+-rw-rw-rw-   0 root         (0) root         (0)    11146 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/calibratemulti.py
+-rw-rw-rw-   0 root         (0) root         (0)     7837 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/calibratesingle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     1443 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 06:52:15.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   188527 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/icons/category.png
+-rw-rw-rw-   0 root         (0) root         (0)   188527 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/icons/widget.png
+-rw-rw-rw-   0 root         (0) root         (0)     2178 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/integrate1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     3252 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 06:52:15.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/tutorials/__init__.py
```

### Comparing `ewoksxrpd-0.3.0/LICENSE.md` & `ewoksxrpd-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/PKG-INFO` & `ewoksxrpd-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ewoksxrpd
-Version: 0.3.0
+Version: 0.4.0
 Summary: Data processing workflows for SAXS/WAXS
 Home-page: https://gitlab.esrf.fr/workflow/ewoksxrpd/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksxrpd/
 Project-URL: Documentation, https://ewoksxrpd.readthedocs.io/
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoksxrpd/issues/
-Keywords: orange3 add-on
+Keywords: orange3 add-on,ewoks
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
```

### Comparing `ewoksxrpd-0.3.0/README.md` & `ewoksxrpd-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/setup.cfg` & `ewoksxrpd-0.4.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -13,29 +13,31 @@
 	Documentation = https://ewoksxrpd.readthedocs.io/
 	Tracker = https://gitlab.esrf.fr/workflow/ewoksxrpd/issues/
 classifiers = 
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 keywords = 
-	orange3 add-on
+	orange3 add-on,ewoks
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	numpy
 	scipy
 	silx >=1.1.0
 	pyopencl
-	pyfai >=2023.1,!=2023.2
-	ewoksdata >=0.2.5
+	pyfai >=2023.3
+	ewoksdata >=0.2.6
 	ewoks[orange] >=0.1.2
+	fabio
+	h5py
 namespace_packages = 
 	orangecontrib
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
@@ -54,30 +56,27 @@
 [options.entry_points]
 orange3.addon = 
 	ewoksxrpd=orangecontrib.ewoksxrpd
 orange.widgets = 
 	XRPD=orangecontrib.ewoksxrpd
 orange.canvas.help = 
 	html-index=orangecontrib.ewoksxrpd:WIDGET_HELP_PATH
+ewoks.tasks.class = 
+	ewoksxrpd.tasks.*=ewoksxrpd
 
 [options.package_data]
 * = *.ows, *.png, *.svg
 
 [flake8]
 ignore = E501, E203, W503
 max-line-length = 88
 exclude = 
 	.eggs
 	scraps/*
 
-[build_sphinx]
-project = ewoksxrpd
-version = attr: ewoksxrpd.__version__
-source-dir = ./doc
-
 [coverage:run]
 omit = 
 	setup.py
 	*/tests/*
 
 [egg_info]
 tag_build =
```

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/gui/forms.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/gui/forms.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/gui/plots.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/gui/plots.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/gui/serialize.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/gui/serialize.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/gui/trigger_widget.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/gui/trigger_widget.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/init_matplotlib.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/init_matplotlib.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/ascii.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/ascii.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 class SaveAsciiPattern1D(
     Task,
     input_names=["filename", "x", "y", "xunits"],
     optional_input_names=["header", "yerror", "metadata"],
     output_names=["saved"],
 ):
+    """Save single diffractogram in ASCII format"""
+
     def run(self):
         if is_data(self.inputs.yerror):
             data = [self.inputs.x, self.inputs.y, self.inputs.yerror]
         else:
             data = [self.inputs.x, self.inputs.y]
         data = numpy.stack(data, axis=1)
```

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/background.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/background.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class SubtractBackground(
     TaskWithDataAccess,
     input_names=["image", "monitor", "background", "background_monitor"],
     output_names=["image", "monitor"],
 ):
-    """The background will be normalized to the monitor:
+    """Background removal with normalization
 
     .. code:
 
         Icor = I  - B / Bmon * Imon
     """
 
     def run(self):
```

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/calibrate.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/calibrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -423,14 +423,16 @@
 
 
 class CalculateGeometry(
     TaskWithDataAccess,
     input_names=["parametrization", "parameters", "position"],
     output_names=["geometry", "energy"],
 ):
+    """Calculate energy and geometry from pyFAI parametrization"""
+
     def run(self):
         parametrization = data_utils.data_from_storage(self.inputs.parametrization)
         geometry, energy = calculate_geometry(
             parametrization,
             self.inputs.parameters,
             self.get_data(self.inputs.position),
         )
```

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/data_access.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/data_access.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/diagnostics.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/diagnostics.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,14 +129,16 @@
 
 
 class DiagnoseCalibrateSingleResults(
     _DiagnoseCalibrateResults,
     input_names=["image", "geometry", "energy"],
     optional_input_names=["rings"],
 ):
+    """Quality of a single-distance pyFAI calibration"""
+
     def run(self):
         if self.inputs.filename:
             if os.path.exists(self.inputs.filename):
                 self.outputs.saved = True
                 return
         if plt is None:
             raise RuntimeError("'matplotlib' is not installed")
@@ -168,14 +170,16 @@
         "images",
         "positions",
         "parametrization",
         "parameters",
     ],
     optional_input_names=["show", "pause", "rings"],
 ):
+    """Quality of a multi-distance pyFAI calibration"""
+
     def run(self):
         if self.inputs.filename:
             if os.path.exists(self.inputs.filename):
                 self.outputs.saved = True
                 return
         if plt is None:
             raise RuntimeError("'matplotlib' is not installed")
@@ -213,14 +217,16 @@
     input_names=[
         "x",
         "y",
         "xunits",
     ],
     optional_input_names=["calibrant", "energy", "yerror", "scaling"],
 ):
+    """Quality of a pyFAI integration"""
+
     def run(self):
         if self.inputs.filename:
             if os.path.exists(self.inputs.filename):
                 self.outputs.saved = True
                 return
         if plt is None:
             raise RuntimeError("'matplotlib' is not installed")
```

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/integrate.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/integrate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from numbers import Number
 from contextlib import contextmanager, ExitStack
-from typing import Union, Tuple
+from typing import Union, Tuple, List, Dict, Optional, Any
 
 import numpy
 import h5py
 from ewoksdata.data.hdf5.dataset_writer import DatasetWriter
 
 from .worker import persistent_worker
 from .worker import set_maximum_persistent_workers
@@ -24,14 +24,16 @@
     input_names=["detector", "geometry", "energy"],
     optional_input_names=[
         "detector_config",
         "mask",
         "integration_options",
         "fixed_integration_options",
         "maximum_persistent_workers",
+        "references",
+        "monitors",
     ],
     register=False,
 ):
     @contextmanager
     def _worker(self):
         nworkers = self.get_input_value("maximum_persistent_workers", None)
         if nworkers is not None:
@@ -67,74 +69,117 @@
             config["mask"] = self.get_image(
                 data_utils.data_from_storage(self.inputs.mask)
             )
         return config
 
     def _pyfai_normalization_factor(
         self,
-        monitor: Union[numpy.ndarray, Number, str, list, None],
-        reference: Union[numpy.ndarray, Number, str, list, None],
-    ) -> Tuple[float, float, float]:
-        r"""Returns the pyfai normalization factor based on a monitor and a reference value.
+        monitors: List[Union[numpy.ndarray, Number, str, list, None]],
+        references: List[Union[numpy.ndarray, Number, str, list, None]],
+        ptdata: Optional[Dict[str, numpy.ndarray]] = None,
+    ) -> Tuple[float, float]:
+        r"""Returns the pyfai normalization factor based on a monitor and a references.
 
         The pyfai normalization factor is defined as
 
         .. code::
 
-            Inorm = I / normalization_factor
+            Inorm = I / (normalization_factor1 * normalization_factor2 * ...)
 
         Monitor normalization is done like this
 
         .. code::
 
-            Inorm = I / monitor * reference
+            Inorm = I * reference1 / monitor1 * reference2 / monitor2 * ...
 
         which means that the normalization factor is
 
         .. code::
 
-            normalization_factor = monitor / reference
+            normalization_factor = monitor1 / reference1 * monitor2 / reference2 * ...
+
+        Both monitors and references can be defined by:
+
+         * scalar value
+         * array or list of numbers
+         * counter name
+         * data URL
         """
-        if data_utils.is_data(reference):
-            reference = self.get_data(reference)
-        else:
-            reference = 1
-        if data_utils.is_data(monitor):
-            monitor = self.get_data(monitor)
-        else:
-            monitor = 1
-        normalization_factor = monitor / reference
-        return normalization_factor, monitor, reference
+        numerator = 1.0
+        for value in monitors:
+            if not data_utils.is_data(value):
+                value = 1
+            elif _is_counter_name(value):
+                if ptdata is None:
+                    raise ValueError("monitor value cannot be a counter name")
+                value = ptdata[value]
+            else:
+                value = self.get_data(value)
+            numerator *= value
+
+        if not numpy.isscalar(numerator):
+            raise ValueError("monitor values need to be scalars")
+
+        denominator = 1.0
+        for value in references:
+            if not data_utils.is_data(value):
+                value = 1
+            elif _is_counter_name(value):
+                if ptdata is None:
+                    raise ValueError("reference value cannot be a counter name")
+                value = ptdata[value]
+            else:
+                value = self.get_data(value)
+            denominator *= value
+
+        if not numpy.isscalar(denominator):
+            raise ValueError("reference values need to be scalars")
+
+        return numerator, denominator
 
 
 class Integrate1D(
     _BaseIntegrate,
     input_names=["image"],
     optional_input_names=["monitor", "reference"],
     output_names=["x", "y", "yerror", "xunits", "info"],
 ):
     """1D integration of a single diffraction pattern."""
 
     def run(self):
         raw_data = self.get_image(self.inputs.image)
-        normalization_factor, monitor, reference = self._pyfai_normalization_factor(
-            self.inputs.monitor, self.inputs.reference
+
+        monitors = self.get_input_value("monitors", list())
+        references = self.get_input_value("references", list())
+        if len(monitors) != len(references):
+            raise ValueError(
+                "length of normalization monitors and references is not the same"
+            )
+        if not self.missing_inputs.monitor or not self.missing_inputs.reference:
+            monitors.append(self.get_input_value("monitor", None))
+            references.append(self.get_input_value("reference", None))
+
+        monitor_value, reference_value = self._pyfai_normalization_factor(
+            monitors, references
         )
+        normalization_factor = monitor_value / reference_value
 
         with self._worker() as (worker, config):
             result = worker.process(raw_data, normalization_factor=normalization_factor)
 
             self.outputs.x = result.radial
             self.outputs.y = result.intensity
             yerror = integrate_utils.get_yerror(result)
             self.outputs.yerror = numpy.abs(yerror)
             self.outputs.xunits = result.unit.name
 
             info = pyfai_utils.compile_integration_info(
-                config, monitor=monitor, reference=reference
+                config,
+                monitor_value=monitor_value,
+                reference_value=reference_value,
             )
             self.outputs.info = info
 
 
 class IntegrateBlissScan(
     _BaseIntegrate,
     input_names=["filename", "scan", "detector_name", "output_filename"],
@@ -143,48 +188,65 @@
         "monitor_name",
         "reference",
         "subscan",
         "retry_timeout",
         "retry_period",
         "demo",
         "scan_memory_url",
+        "external_output_filename",
         "nxprocess_name",
         "nxmeasurement_name",
         "nxprocess_as_default",
         "flush_period",
     ],
 ):
     """1D or 2D integration of a single detector in a single Bliss scan with saving."""
 
     def run(self):
         if self.inputs.counter_names:
-            counter_names = list(self.inputs.counter_names)
+            counter_names = set(self.inputs.counter_names)
         else:
-            counter_names = list()
+            counter_names = set()
 
         detector_name = self.inputs.detector_name
-        monitor_name = self.get_input_value("monitor_name", None)
-        if monitor_name and monitor_name not in counter_names:
-            counter_names.append(monitor_name)
-        reference = self.get_input_value("reference", None)
-        reference_name = None
-        if isinstance(reference, str):
-            reference_name = reference
-            if reference not in counter_names:
-                counter_names.append(reference)
+
+        monitors = self.get_input_value("monitors", list())
+        references = self.get_input_value("references", list())
+        if len(monitors) != len(references):
+            raise ValueError(
+                "length of normalization monitors and references is not the same"
+            )
+        if not self.missing_inputs.monitor_name or not self.missing_inputs.reference:
+            monitors.append(self.get_input_value("monitor_name", None))
+            references.append(self.get_input_value("reference", None))
+        for name in references:
+            if _is_counter_name(name):
+                counter_names.add(name)
+        for name in monitors:
+            if _is_counter_name(name):
+                counter_names.add(name)
+        counter_names = list(counter_names)
 
         scan = self.inputs.scan
         subscan = self.get_input_value("subscan", 1)
-        output_url = f"silx://{self.inputs.output_filename}?path=/{scan}.{subscan}"
+        output_filename = self.inputs.output_filename
+        output_url = f"silx://{output_filename}?path=/{scan}.{subscan}"
+        external_output_filename = self.get_input_value(
+            "external_output_filename", output_filename
+        )
+        external_output_url = (
+            f"silx://{external_output_filename}?path=/{scan}.{subscan}"
+        )
         input_url = f"silx://{self.inputs.filename}?path=/{scan}.{subscan}"
         flush_period = self.get_input_value("flush_period", None)
 
         with ExitStack() as stack:
             worker = None
-            parent = None
+            data_parent = None
+            master_parent = None
             nxprocess = None
             measurement = None
 
             intensity_writer = None
             error_writer = None
             ctr_writers = dict()
 
@@ -212,32 +274,44 @@
 
             for ptdata in data_iterator:
                 if worker is None:
                     # Start the worker + open the output file only after
                     # the first image is read
                     worker, config = stack.enter_context(self._worker())
                     info = pyfai_utils.compile_integration_info(
-                        config, reference=reference
+                        config,
+                        monitors=monitors,
+                        references=references,
                     )
 
-                    parent = stack.enter_context(
-                        self.open_h5item(output_url, mode="a", create=True)
-                    )
-                    assert isinstance(parent, h5py.Group)
-                    nxprocess = pyfai_utils.create_nxprocess(
-                        parent, self._nxprocess_name, info
+                    data_parent = stack.enter_context(
+                        self.open_h5item(external_output_url, mode="a", create=True)
                     )
+                    assert isinstance(data_parent, h5py.Group)
 
-                    if counter_names:
-                        measurement = parent.create_group("measurement")
-                        measurement.attrs["NX_class"] = "NXcollection"
+                    with self.open_h5item(
+                        output_url, mode="a", create=True
+                    ) as master_parent:
+                        assert isinstance(master_parent, h5py.Group)
+                        nxprocess = pyfai_utils.create_nxprocess(
+                            master_parent, data_parent, self._nxprocess_name, info
+                        )
+                        if counter_names:
+                            measurement = data_parent.require_group("measurement")
+                            measurement.attrs["NX_class"] = "NXcollection"
+                            if data_parent.file.filename != master_parent.file.filename:
+                                pyfai_utils.create_hdf5_link(
+                                    measurement, master_parent, "measurement"
+                                )
 
-                normalization_factor, *_ = self._pyfai_normalization_factor(
-                    ptdata.get(monitor_name), ptdata.get(reference_name, reference)
+                monitor_value, reference_value = self._pyfai_normalization_factor(
+                    monitors, references, ptdata
                 )
+                normalization_factor = monitor_value / reference_value
+
                 image = ptdata[detector_name]
                 if self.inputs.demo:
                     image = image[:-1, :-1]
                 result = worker.process(
                     image, normalization_factor=normalization_factor
                 )
                 if intensity_writer is None:
@@ -264,32 +338,38 @@
 
                 flush = intensity_writer.add_point(result.intensity)
                 if result.sigma is not None:
                     flush |= error_writer.add_point(result.sigma)
                 for name in counter_names:
                     flush |= ctr_writers[name].add_point(ptdata[name])
                 if flush:
-                    parent.file.flush()
+                    data_parent.file.flush()
 
             if intensity_writer is None:
                 raise RuntimeError("No scan data")
             intensity_writer.flush_buffer()
             if error_writer is not None:
                 error_writer.flush_buffer()
 
             nxdata["points"] = numpy.arange(intensity_writer.dataset.shape[0])
             axes = nxdata.attrs["axes"]
             axes[0] = "points"
             nxdata.attrs["axes"] = axes
 
-            self.link_bliss_scan(parent, input_url)
-            mark_as_default = self.get_input_value("nxprocess_as_default", True)
-            pyfai_utils.create_nxprocess_links(
-                nxprocess, self._nxmeasurement_name, mark_as_default=mark_as_default
-            )
+            with self.open_h5item(output_url, mode="a", create=True) as master_parent:
+                self.link_bliss_scan(master_parent, input_url)
+                mark_as_default = self.get_input_value("nxprocess_as_default", True)
+                measurement = master_parent.require_group("measurement")
+                measurement.attrs["NX_class"] = "NXcollection"
+                pyfai_utils.create_nxprocess_links(
+                    nxprocess,
+                    measurement,
+                    self._nxmeasurement_name,
+                    mark_as_default=mark_as_default,
+                )
 
     @property
     def _nxprocess_name(self):
         if self.inputs.nxprocess_name:
             return self.inputs.nxprocess_name
         default = "integrate"
         if self.inputs.detector_name:
@@ -329,27 +409,39 @@
     ],
 ):
     """1D or 2D integration of a single detector in a single Bliss scan without saving."""
 
     def run(self):
         with self._worker() as (worker, config):
             if self.inputs.counter_names:
-                counter_names = list(self.inputs.counter_names)
+                counter_names = set(self.inputs.counter_names)
             else:
-                counter_names = list()
+                counter_names = set()
             detector_name = self.inputs.detector_name
-            monitor_name = self.get_input_value("monitor_name", None)
-            if monitor_name and monitor_name not in counter_names:
-                counter_names.append(monitor_name)
-            reference = self.get_input_value("reference", None)
-            reference_name = None
-            if isinstance(reference, str):
-                reference_name = reference
-                if reference not in counter_names:
-                    counter_names.append(reference)
+
+            monitors = self.get_input_value("monitors", list())
+            references = self.get_input_value("references", list())
+            if len(monitors) != len(references):
+                raise ValueError(
+                    "length of normalization monitors and references is not the same"
+                )
+            if (
+                not self.missing_inputs.monitor_name
+                or not self.missing_inputs.reference
+            ):
+                monitors.append(self.get_input_value("monitor_name", None))
+                references.append(self.get_input_value("reference", None))
+            for name in references:
+                if _is_counter_name(name):
+                    counter_names.add(name)
+            for name in monitors:
+                if _is_counter_name(name):
+                    counter_names.add(name)
+            counter_names = list(counter_names)
+
             subscan = self.get_input_value("subscan", None)
 
             intensities = []
             sigmas = []
             radial = None
             unit = None
             azimuthal = None
@@ -372,18 +464,20 @@
                     self.inputs.filename,
                     self.inputs.scan,
                     lima_names=[detector_name],
                     counter_names=counter_names,
                     subscan=subscan,
                 )
 
+            normalization_factor = 0
             for ptdata in data_iterator:
-                normalization_factor, *_ = self._pyfai_normalization_factor(
-                    ptdata.get(monitor_name), ptdata.get(reference_name, reference)
+                monitor_value, reference_value = self._pyfai_normalization_factor(
+                    monitors, references, ptdata
                 )
+                normalization_factor = monitor_value / reference_value
                 image = ptdata[detector_name]
                 if self.inputs.demo:
                     image = image[:-1, :-1]
                 result = worker.process(
                     image, normalization_factor=normalization_factor
                 )
 
@@ -392,15 +486,21 @@
                 if radial is None:
                     radial = result.radial
                 if unit is None:
                     unit = result.unit.name
                 if worker.do_2D() and azimuthal is None:
                     azimuthal = result.azimuthal
 
-            info = pyfai_utils.compile_integration_info(config, reference=reference)
+            info = pyfai_utils.compile_integration_info(
+                config, monitors=monitors, references=references
+            )
 
             self.outputs.radial = radial
             self.outputs.azimuthal = azimuthal
             self.outputs.intensity = numpy.array(intensities)
             self.outputs.intensity_error = numpy.array(sigmas)
             self.outputs.radial_units = unit
             self.outputs.info = info
+
+
+def _is_counter_name(value: Any) -> bool:
+    return isinstance(value, str) and "://" not in value
```

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/mask.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/mask.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/morphology.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/morphology.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/nexus.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/nexus.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     input_names=["url"],
     optional_input_names=[
         "bliss_scan_url",
         "metadata",
         "nxprocess_name",
         "nxmeasurement_name",
         "nxprocess_as_default",
+        "external_url",
     ],
     output_names=["saved"],
     register=False,
 ):
     @property
     def _process_info(self):
         raise NotImplementedError
@@ -36,46 +37,59 @@
     def _nxmeasurement_name(self):
         if self.inputs.nxmeasurement_name:
             return self.inputs.nxmeasurement_name
         return "integrated"
 
     @contextmanager
     def _save_context(self):
-        with self.open_h5item(self.inputs.url, mode="a", create=True) as parent:
-            assert isinstance(parent, h5py.Group)
-            nxprocess = pyfai_utils.create_nxprocess(
-                parent, self._nxprocess_name, self._process_info
-            )
+        master_url = self.inputs.url
+        data_url = self.get_input_value("external_url", master_url)
+
+        with self.open_h5item(data_url, mode="a", create=True) as data_parent:
+            assert isinstance(data_parent, h5py.Group)
+            with self.open_h5item(master_url, mode="a", create=True) as master_parent:
+                assert isinstance(master_parent, h5py.Group)
+                nxprocess = pyfai_utils.create_nxprocess(
+                    master_parent, data_parent, self._nxprocess_name, self._process_info
+                )
 
             yield nxprocess
 
-            url = data_utils.data_from_storage(
-                self.inputs.bliss_scan_url, remove_numpy=True
-            )
-            if url:
-                self.link_bliss_scan(parent, url)
-            mark_as_default = self.get_input_value("nxprocess_as_default", True)
-            pyfai_utils.create_nxprocess_links(
-                nxprocess, self._nxmeasurement_name, mark_as_default=mark_as_default
-            )
-            if self.inputs.metadata:
-                dicttonx(
-                    self.inputs.metadata,
-                    parent,
-                    update_mode="add",
-                    add_nx_class=True,
+            with self.open_h5item(master_url, mode="a", create=True) as master_parent:
+                url = data_utils.data_from_storage(
+                    self.inputs.bliss_scan_url, remove_numpy=True
+                )
+                if url:
+                    self.link_bliss_scan(master_parent, url)
+                mark_as_default = self.get_input_value("nxprocess_as_default", True)
+                measurement = master_parent.require_group("measurement")
+                measurement.attrs["NX_class"] = "NXcollection"
+                pyfai_utils.create_nxprocess_links(
+                    nxprocess,
+                    measurement,
+                    self._nxmeasurement_name,
+                    mark_as_default=mark_as_default,
                 )
+                if self.inputs.metadata:
+                    dicttonx(
+                        self.inputs.metadata,
+                        master_parent,
+                        update_mode="add",
+                        add_nx_class=True,
+                    )
         self.outputs.saved = True
 
 
 class SaveNexusPattern1D(
     _BaseSaveNexusIntegrated,
     input_names=["x", "y", "xunits"],
     optional_input_names=["header", "yerror"],
 ):
+    """Save single diffractogram in HDF5/NeXus format"""
+
     def run(self):
         with self._save_context() as nxprocess:
             nxdata = pyfai_utils.create_nxdata(
                 nxprocess, self.inputs.y.ndim, self.inputs.x, self.inputs.xunits, None
             )
             nxdata["intensity"] = self.inputs.y
             if not self.missing_inputs.yerror:
@@ -87,14 +101,16 @@
 
 
 class SaveNexusIntegrated(
     _BaseSaveNexusIntegrated,
     input_names=["radial", "intensity", "radial_units"],
     optional_input_names=["info", "azimuthal", "intensity_error"],
 ):
+    """Save 1D or 2D integration diffraction patterns in HDF5/NeXus format"""
+
     def run(self):
         with self._save_context() as nxprocess:
             nxdata = pyfai_utils.create_nxdata(
                 nxprocess,
                 self.inputs.intensity.ndim,
                 self.inputs.radial,
                 self.inputs.radial_units,
```

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/pyfaiconfig.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/pyfaiconfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,21 +28,24 @@
         "detector",
         "detector_config",
         "calibrant",
         "mask",
         "integration_options",
     ],
 ):
+    """Parse pyFAI calibration and integration parameters"""
+
     def run(self):
         input_values = self.input_values
         integration_options = self.merged_integration_options()
 
-        energy = integration_options.pop("wavelength", None)
-        if energy is not None:
-            energy = xrpd_utils.energy_wavelength(energy)
+        wavelength = integration_options.pop("wavelength", None)
+        energy = integration_options.pop("energy", None)
+        if energy is None:
+            energy = xrpd_utils.energy_wavelength(wavelength)
         if not self.missing_inputs.energy:
             energy = input_values["energy"]
 
         detector = integration_options.pop("detector", None)
         if not self.missing_inputs.detector:
             detector = input_values["detector"]
```

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/pyfai_utils.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/pyfai_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import re
 import json
 from typing import Union, Dict, Optional, Any, Iterator, Tuple, List
 from collections.abc import Mapping, Sequence
 
 import numpy
 import h5py
@@ -23,14 +24,16 @@
     "/lbsram/": "/",
 }
 
 
 def parse_units(radial_units: Any) -> Tuple[str, str]:
     if isinstance(radial_units, Unit):
         radial_units = radial_units.name
+    if isinstance(radial_units, numpy.ndarray):
+        radial_units = radial_units.item()
     if not isinstance(radial_units, str):
         raise TypeError(type(radial_units))
     unit_tuple = tuple(radial_units.split("_"))
     if len(unit_tuple) != 2:
         raise ValueError(f"Expected unit to be of the form X_Y. Got {radial_units}")
     return unit_tuple
 
@@ -206,19 +209,24 @@
 
 def _add_extra(adict: Mapping, extra: Mapping):
     for k, v in extra.items():
         if v is not None:
             adict[k] = v
 
 
-def create_nxprocess(parent: h5py.Group, nxprocess_name: str, info) -> h5py.Group:
+def create_nxprocess(
+    master_parent: h5py.Group, data_parent: h5py.Group, nxprocess_name: str, info
+) -> h5py.Group:
     nxtree_dict = integration_info_for_nexus(info, integrated={"@NX_class": "NXdata"})
-    nxprocess_path = f"{parent.name}/{nxprocess_name}"
-    dicttonx(nxtree_dict, parent.file, h5path=nxprocess_path, update_mode="modify")
-    return parent[nxprocess_name]
+    nxprocess_path = f"{data_parent.name}/{nxprocess_name}"
+    dicttonx(nxtree_dict, data_parent.file, h5path=nxprocess_path, update_mode="modify")
+    nxprocess = data_parent[nxprocess_name]
+    if data_parent.file.filename != master_parent.file.filename:
+        create_hdf5_link(nxprocess, master_parent, nxprocess_name)
+    return nxprocess
 
 
 def create_nxdata(
     nxprocess: h5py.Group, intensity_dim: int, radial, radial_units, azimuthal
 ) -> h5py.Group:
     # Axes names and units
     radial_units = data_from_storage(radial_units, remove_numpy=True)
@@ -258,21 +266,39 @@
         dset = nxdata.create_dataset(azimuthal_name, data=azimuthal)
         dset.attrs["units"] = azimuthal_units
 
     return nxdata
 
 
 def create_nxprocess_links(
-    nxprocess: h5py.Group, nxmeasurement_name: str, mark_as_default: bool = True
+    nxprocess: h5py.Group,
+    target: h5py.Group,
+    link_name: str,
+    mark_as_default: bool = True,
 ) -> None:
     nxdata = nxprocess["integrated"]
     try:
         intensity = nxdata["intensity"]
     except KeyError:
         return
+    create_hdf5_link(intensity, target, link_name)
     if mark_as_default:
-        nexus.select_default_plot(nxprocess)
-    measurement = nxprocess.parent.require_group("measurement")
-    link_name = nxmeasurement_name
-    if link_name in measurement:
-        del measurement[link_name]
-    measurement[link_name] = h5py.SoftLink(intensity.name)
+        nexus.select_default_plot(intensity)
+        if intensity.file.filename != nxprocess.file.filename:
+            target.attrs["default"] = link_name
+            nexus.select_default_plot(target)
+
+
+def create_hdf5_link(
+    source: Union[h5py.Dataset, h5py.Group], target: h5py.Group, link_name: str
+) -> None:
+    if link_name in target:
+        return
+    source_filename = source.file.filename
+    target_filename = target.file.filename
+    if source_filename == target_filename:
+        target[link_name] = h5py.SoftLink(source.name)
+    else:
+        source_filename = os.path.relpath(
+            source_filename, os.path.dirname(target_filename)
+        )
+        target[link_name] = h5py.ExternalLink(source_filename, source.name)
```

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tasks/worker.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/worker.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/conftest.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -180,14 +180,34 @@
         lima_names=("p3",),
         counter_names=("diode1", "diode2"),
         sequence="multiply",
     )
 
 
 @pytest.fixture(scope="session")
+def bliss_perkinelmer_scan(tmpdir_factory, imageSetup1Calibrant1):
+    tmpdir = tmpdir_factory.mktemp("sample_dataset")
+    npoints_per_file = 3
+    npoints = 31
+    scannr = 2
+    image = imageSetup1Calibrant1.image
+    return save_bliss_scan(
+        tmpdir,
+        image,
+        npoints_per_file,
+        npoints,
+        scannr,
+        subscannr=1,
+        lima_names=("perkinelmer",),
+        counter_names=("mon",),
+        sequence="multiply",
+    )
+
+
+@pytest.fixture(scope="session")
 def bliss_task_inputs(bliss_lab6_scan, setup1) -> dict:
     return {
         "filename": str(bliss_lab6_scan),
         "scan": 2,
         "detector": setup1.detector,
         "energy": setup1.energy,
         "geometry": setup1.geometry,
```

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_ascii.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_ascii.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_background.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_background.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_batch_integrate.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_batch_integrate.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,27 +3,36 @@
 import pytest
 from ewoksorange.tests.utils import execute_task
 
 from orangecontrib.ewoksxrpd.batchintegrate import OWIntegrateBlissScan
 
 
 @pytest.mark.parametrize("ndims", [1, 2])
-def test_batch_integrate_task(ndims, bliss_task_inputs, tmpdir):
-    assert_batch_integrate(ndims, bliss_task_inputs, tmpdir)
+@pytest.mark.parametrize("external", [False, True])
+def test_batch_integrate_task(ndims, external, bliss_task_inputs, tmpdir):
+    assert_batch_integrate(ndims, bliss_task_inputs, tmpdir, external=external)
 
 
 @pytest.mark.parametrize("ndims", [1, 2])
-def test_batch_integrate_widget(ndims, bliss_task_inputs, tmpdir, qtapp):
-    assert_batch_integrate(ndims, bliss_task_inputs, tmpdir, qtapp=qtapp)
+@pytest.mark.parametrize("external", [False, True])
+def test_batch_integrate_widget(ndims, external, bliss_task_inputs, tmpdir, qtapp):
+    assert_batch_integrate(
+        ndims, bliss_task_inputs, tmpdir, external=external, qtapp=qtapp
+    )
 
 
-def assert_batch_integrate(ndims, bliss_task_inputs, tmpdir, qtapp=None):
+def assert_batch_integrate(
+    ndims, bliss_task_inputs, tmpdir, external: bool = False, qtapp=None
+):
+    inputs = dict(bliss_task_inputs)
     output_filename = str(tmpdir / "result.h5")
-    inputs = {**bliss_task_inputs, "output_filename": output_filename}
-
+    inputs["output_filename"] = output_filename
+    if external:
+        external_output_filename = str(tmpdir / "data.h5")
+        inputs["external_output_filename"] = external_output_filename
     if ndims == 2:
         inputs["integration_options"] = {
             "method": "no_csr_cython",
             "integrator_name": "integrate2d_ng",
             "nbpt_azim": 100,
             "error_model": "poisson",
         }
```

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_calibrate.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_calibrate.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_calint_workflow.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_calint_workflow.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_integrate.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_integrate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 from os import PathLike
+import pytest
 import numpy
 from ewoksorange.tests.utils import execute_task
 
 from orangecontrib.ewoksxrpd.integrate1d import OWIntegrate1D
 from orangecontrib.ewoksxrpd.diagnose_integrate1d import OWDiagnoseIntegrate1D
 from .xrpd_theory import Measurement, Setup, xPattern, yPattern
 
 
+@pytest.mark.parametrize("monitorlist", [False, True])
 def test_integrate1d_task(
     tmpdir: PathLike,
     imageSetup1SampleA: Measurement,
     setup1: Setup,
     xSampleA: xPattern,
     ySampleA: yPattern,
+    monitorlist: bool,
 ):
-    assert_integrate1d(imageSetup1SampleA, setup1, xSampleA, ySampleA, tmpdir, None)
+    assert_integrate1d(
+        imageSetup1SampleA,
+        setup1,
+        xSampleA,
+        ySampleA,
+        tmpdir,
+        None,
+        monitorlist=monitorlist,
+    )
 
 
 def test_integrate1d_widget(
     tmpdir: PathLike,
     imageSetup1SampleA: Measurement,
     setup1: Setup,
     xSampleA: xPattern,
@@ -106,27 +117,32 @@
     measurement: Measurement,
     setup: Setup,
     xpattern: xPattern,
     ypattern: yPattern,
     tmpdir: PathLike,
     qtapp,
     integration_options=None,
+    monitorlist: bool = False,
 ):
     integration_options2 = dict(xpattern.integration_options)
     if integration_options:
         integration_options2.update(integration_options)
     inputs = {
         "image": measurement.image,
-        "monitor": measurement.monitor,
-        "reference": ypattern.monitor,
         "detector": setup.detector,
         "geometry": setup.geometry,
         "energy": setup.energy,
         "integration_options": integration_options2,
     }
+    if monitorlist:
+        inputs["monitors"] = [measurement.monitor, 1, None, 1]
+        inputs["references"] = [ypattern.monitor, 1, 1, None]
+    else:
+        inputs["monitor"] = measurement.monitor
+        inputs["reference"] = ypattern.monitor
 
     output_values = execute_task(
         OWIntegrate1D.ewokstaskclass if qtapp is None else OWIntegrate1D, inputs=inputs
     )
 
     assert output_values["xunits"] == xpattern.units
     numpy.testing.assert_allclose(xpattern.x, output_values["x"], rtol=1e-6)
```

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_mask.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_nexus.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_nexus_integrated.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_nexus_integrated.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/test_pyfai_utils.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_pyfai_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd/tests/xrpd_theory.py` & `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/xrpd_theory.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/PKG-INFO` & `ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ewoksxrpd
-Version: 0.3.0
+Version: 0.4.0
 Summary: Data processing workflows for SAXS/WAXS
 Home-page: https://gitlab.esrf.fr/workflow/ewoksxrpd/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksxrpd/
 Project-URL: Documentation, https://ewoksxrpd.readthedocs.io/
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoksxrpd/issues/
-Keywords: orange3 add-on
+Keywords: orange3 add-on,ewoks
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
```

### Comparing `ewoksxrpd-0.3.0/src/ewoksxrpd.egg-info/SOURCES.txt` & `ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 src/ewoksxrpd/tasks/data_access.py
 src/ewoksxrpd/tasks/diagnostics.py
 src/ewoksxrpd/tasks/integrate.py
 src/ewoksxrpd/tasks/mask.py
 src/ewoksxrpd/tasks/morphology.py
 src/ewoksxrpd/tasks/nexus.py
 src/ewoksxrpd/tasks/pyfaiconfig.py
+src/ewoksxrpd/tasks/save_images.py
+src/ewoksxrpd/tasks/sum.py
 src/ewoksxrpd/tasks/worker.py
 src/ewoksxrpd/tasks/utils/__init__.py
 src/ewoksxrpd/tasks/utils/data_utils.py
 src/ewoksxrpd/tasks/utils/integrate_utils.py
 src/ewoksxrpd/tasks/utils/pyfai_utils.py
 src/ewoksxrpd/tasks/utils/xrpd_utils.py
 src/ewoksxrpd/tests/__init__.py
@@ -45,14 +47,16 @@
 src/ewoksxrpd/tests/test_calibrate.py
 src/ewoksxrpd/tests/test_calint_workflow.py
 src/ewoksxrpd/tests/test_integrate.py
 src/ewoksxrpd/tests/test_mask.py
 src/ewoksxrpd/tests/test_nexus.py
 src/ewoksxrpd/tests/test_nexus_integrated.py
 src/ewoksxrpd/tests/test_pyfai_utils.py
+src/ewoksxrpd/tests/test_save_images.py
+src/ewoksxrpd/tests/test_sum.py
 src/ewoksxrpd/tests/xrpd_theory.py
 src/orangecontrib/__init__.py
 src/orangecontrib/ewoksxrpd/__init__.py
 src/orangecontrib/ewoksxrpd/ascii.py
 src/orangecontrib/ewoksxrpd/background.py
 src/orangecontrib/ewoksxrpd/batchintegrate.py
 src/orangecontrib/ewoksxrpd/blissintegratenosave.py
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/__init__.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/ascii.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/ascii.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from AnyQt import QtWidgets
-from ewoksxrpd.tasks import SaveAsciiPattern1D
+from ewoksxrpd.tasks.ascii import SaveAsciiPattern1D
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui.forms import input_parameters_ascii
 
 
 __all__ = ["OWSaveAsciiPattern1D"]
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/background.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/background.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from AnyQt import QtWidgets
 from silx.gui.plot import Plot2D
 from ewoksdata.data import bliss
-from ewoksxrpd.tasks import SubtractBackground
+
+from ewoksxrpd.tasks.background import SubtractBackground
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.tasks.utils import data_utils
 from ewoksxrpd.gui.forms import input_parameters_background
 
 
 __all__ = ["OWSubtractBackground"]
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/batchintegrate.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/batchintegrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Dict, Mapping, Tuple
-from ewoksxrpd.tasks import IntegrateBlissScan
+
+from ewoksxrpd.tasks.integrate import IntegrateBlissScan
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui.forms import input_parameters_integrateblissscan
 from ewoksxrpd.gui.forms import pack_geometry
 from ewoksxrpd.gui.forms import unpack_geometry
 from ewoksxrpd.gui.forms import unpack_enabled_geometry
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Dict, Mapping, Tuple
 from silx.gui.plot import Plot2D
 from silx.gui.widgets.FrameBrowser import HorizontalSliderWithBrowser
+
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui.forms import input_parameters_integrateblissscan
 from ewoksxrpd.gui.forms import pack_geometry
 from ewoksxrpd.gui.forms import unpack_geometry
 from ewoksxrpd.gui.forms import unpack_enabled_geometry
-from ewoksxrpd.tasks import IntegrateBlissScanWithoutSaving
+from ewoksxrpd.tasks.integrate import IntegrateBlissScanWithoutSaving
 from ewoksxrpd.tasks.utils import data_utils
 
 
 __all__ = ["OWIntegrateBlissScanNoSave"]
 
 
 class OWIntegrateBlissScanNoSave(
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/calculategeometry.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/calculategeometry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Dict, Mapping, Tuple
-from ewoksxrpd.tasks import CalculateGeometry
+
+from ewoksxrpd.tasks.calibrate import CalculateGeometry
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui.forms import input_parameters_calculategeometry
 from ewoksxrpd.gui.forms import output_parameters_calculategeometry
 from ewoksxrpd.gui.forms import pack_geometry
 from ewoksxrpd.gui.forms import unpack_geometry
 from ewoksxrpd.gui.forms import unpack_enabled_geometry
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/calibratemulti.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/calibratemulti.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Dict, Iterable, List, Mapping, Tuple
 from AnyQt import QtWidgets
 from silx.gui.plot import ScatterView, PlotWidget
 from ewokscore.missing_data import is_missing_data
 from ewoksdata.data import bliss
-from ewoksxrpd.tasks import CalibrateMulti
+
+from ewoksxrpd.tasks.calibrate import CalibrateMulti
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui import plots
 from ewoksxrpd.tasks.utils import data_utils
 from ewoksxrpd.tasks.calibrate import calculate_geometry
 from ewoksxrpd.gui.forms import input_parameters_calibratemulti
 from ewoksxrpd.gui.forms import output_parameters_calibratemulti
 from ewoksxrpd.gui.forms import pack_geometry
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/calibratesingle.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/calibratesingle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Dict, List, Mapping, Optional, Tuple
 from AnyQt import QtWidgets
 from silx.gui.plot import ScatterView, PlotWidget
 from ewoksdata.data import bliss
-from ewoksxrpd.tasks import CalibrateSingle
+
+from ewoksxrpd.tasks.calibrate import CalibrateSingle
 from ewoksxrpd.tasks.utils import data_utils
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui import plots
 from ewoksxrpd.gui.forms import input_parameters_calibratesingle
 from ewoksxrpd.gui.forms import output_parameters_calibratesingle
 from ewoksxrpd.gui.forms import pack_geometry
 from ewoksxrpd.gui.forms import unpack_geometry
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from AnyQt import QtWidgets
 from AnyQt import QtGui
-from ewoksxrpd.tasks import DiagnoseIntegrate1D
+
+from ewoksxrpd.tasks.diagnostics import DiagnoseIntegrate1D
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui.forms import input_parameters_diagnose_integrate1d
 
 
 __all__ = ["OWDiagnoseIntegrate1D"]
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from AnyQt import QtWidgets
 from AnyQt import QtGui
-from ewoksxrpd.tasks import DiagnoseCalibrateMultiResults
+
+from ewoksxrpd.tasks.diagnostics import DiagnoseCalibrateMultiResults
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui.forms import input_parameters_diagnose_multicalib
 
 
 __all__ = ["OWDiagnoseCalibrateMultiResults"]
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from AnyQt import QtWidgets
 from AnyQt import QtGui
 
 # from AnyQt.QtCore import Qt
-from ewoksxrpd.tasks import DiagnoseCalibrateSingleResults
+from ewoksxrpd.tasks.diagnostics import DiagnoseCalibrateSingleResults
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui.forms import input_parameters_diagnose_singlecalib
 
 
 __all__ = ["OWDiagnoseCalibrateSingleResults"]
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/icons/category.png` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/icons/category.png`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/icons/widget.png` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/icons/widget.png`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/integrate1d.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/integrate1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Dict, Mapping, Tuple
 from silx.gui.plot import Plot1D
-from ewoksxrpd.tasks import Integrate1D
+
+from ewoksxrpd.tasks.integrate import Integrate1D
 from ewoksxrpd.tasks.utils import data_utils
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui.forms import input_parameters_integrate1d
 from ewoksxrpd.gui.forms import pack_geometry
 from ewoksxrpd.gui.forms import unpack_geometry
 from ewoksxrpd.gui.forms import unpack_enabled_geometry
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/mask.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/mask.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy
 from AnyQt import QtWidgets
 from silx.gui.plot import Plot2D
 from ewoksdata.data import bliss
-from ewoksxrpd.tasks import MaskDetection
+
+from ewoksxrpd.tasks.mask import MaskDetection
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.tasks.utils import data_utils
 from ewoksxrpd.gui.forms import input_parameters_mask
 
 
 __all__ = ["OWMaskDetection"]
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/nexus.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/nexus.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import h5py
 from silx.gui.plot import Plot1D
 from silx.io.url import DataUrl
-from ewoksxrpd.tasks import SaveNexusPattern1D
+
+from ewoksxrpd.tasks.nexus import SaveNexusPattern1D
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui.forms import input_parameters_nexus
 
 
 __all__ = ["OWSaveNexusPattern1D"]
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ewoksxrpd.gui import serialize
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui.forms import input_parameters_nexus
-from ewoksxrpd.tasks import SaveNexusIntegrated
+from ewoksxrpd.tasks.nexus import SaveNexusIntegrated
 
 
 __all__ = ["OWSaveNexusIntegrated"]
 
 
 class OWSaveNexusIntegrated(OWTriggerWidget, ewokstaskclass=SaveNexusIntegrated):
     name = "SaveNexusIntegrated"
```

### Comparing `ewoksxrpd-0.3.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py` & `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Dict, Mapping, Tuple
-from ewoksxrpd.tasks import PyFaiConfig
+
+from ewoksxrpd.tasks.pyfaiconfig import PyFaiConfig
 from ewoksxrpd.gui.trigger_widget import OWTriggerWidget
 from ewoksxrpd.gui.forms import input_parameters_pyfai_config
 from ewoksxrpd.gui.forms import output_parameters_pyfai_config
 from ewoksxrpd.gui.forms import pack_geometry
 from ewoksxrpd.gui.forms import unpack_geometry
 from ewoksxrpd.gui.forms import unpack_enabled_geometry
```

