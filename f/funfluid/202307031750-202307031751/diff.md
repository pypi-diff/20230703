# Comparing `tmp/funfluid-202307031750.tar.gz` & `tmp/funfluid-202307031751.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funfluid-202307031750.tar", last modified: Mon Jul  3 09:50:59 2023, max compression
+gzip compressed data, was "funfluid-202307031751.tar", last modified: Mon Jul  3 09:51:57 2023, max compression
```

## Comparing `funfluid-202307031750.tar` & `funfluid-202307031751.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.483595 funfluid-202307031750/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:49:06.000000 funfluid-202307031750/LICENSE
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-03 09:50:59.483595 funfluid-202307031750/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       84 2023-07-03 09:06:44.000000 funfluid-202307031750/README.md
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.467595 funfluid-202307031750/funfluid/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        2 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.467595 funfluid-202307031750/funfluid/common/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/common/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.467595 funfluid-202307031750/funfluid/common/base/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/common/base/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2837 2023-06-30 08:49:51.000000 funfluid-202307031750/funfluid/common/base/cache.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.467595 funfluid-202307031750/funfluid/common/flow/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/common/flow/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.471595 funfluid-202307031750/funfluid/common/particle/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/common/particle/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.471595 funfluid-202307031750/funfluid/experiment/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/experiment/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.471595 funfluid-202307031750/funfluid/experiment/chlamydomonas/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.471595 funfluid-202307031750/funfluid/experiment/chlamydomonas/analyse/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/analyse/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4563 2023-06-30 08:50:16.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/analyse/analyse.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.471595 funfluid-202307031750/funfluid/experiment/chlamydomonas/base/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/base/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3815 2023-06-30 08:50:20.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/base/base.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/base/globalconfig.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.471595 funfluid-202307031750/funfluid/experiment/chlamydomonas/detect/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/detect/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2977 2023-06-30 08:50:23.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/detect/background.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4707 2023-06-30 08:50:30.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/detect/contain.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     9205 2023-06-30 08:50:37.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/detect/particle.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.471595 funfluid-202307031750/funfluid/experiment/chlamydomonas/plot/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/plot/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/plot/core.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      239 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/plot/property.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.475595 funfluid-202307031750/funfluid/experiment/chlamydomonas/progress/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/progress/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2909 2023-06-30 08:50:45.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/progress/video_progress.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1573 2023-06-30 08:50:10.000000 funfluid-202307031750/funfluid/experiment/chlamydomonas/run.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.475595 funfluid-202307031750/funfluid/lbm/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       64 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/lbm/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.475595 funfluid-202307031750/funfluid/lbm/core/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       70 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/lbm/core/__init__.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/lbm/core/buff.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    21837 2023-06-30 08:50:49.000000 funfluid-202307031750/funfluid/lbm/core/lattice.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    13442 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/lbm/core/shape.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    10645 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/lbm/core/speed_nb.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.475595 funfluid-202307031750/funfluid/lbm/example/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/lbm/example/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1921 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/lbm/example/example_cavity1.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1994 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/lbm/example/example_cavity3.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3324 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/lbm/example/example_obstacle.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2581 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/lbm/example/example_poiseuille.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3349 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/lbm/example/example_turek.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3662 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/lbm/obs_array.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2364 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/lbm/params.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.475595 funfluid-202307031750/funfluid/simulate/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:53:23.000000 funfluid-202307031750/funfluid/simulate/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.479595 funfluid-202307031750/funfluid/simulate/ellipse/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/simulate/ellipse/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:54:13.000000 funfluid-202307031750/funfluid/simulate/ellipse/analyse.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.479595 funfluid-202307031750/funfluid/simulate/ellipse/example/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/simulate/ellipse/example/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3179 2023-06-30 08:49:55.000000 funfluid-202307031750/funfluid/simulate/ellipse/example/largs_plot_example.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1379 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/simulate/ellipse/plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.479595 funfluid-202307031750/funfluid/simulate/ellipse/project/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:31:46.000000 funfluid-202307031750/funfluid/simulate/ellipse/project/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1441 2023-07-03 09:06:44.000000 funfluid-202307031750/funfluid/simulate/ellipse/project/example.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.479595 funfluid-202307031750/funfluid/simulate/ellipse/project/models/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:36.000000 funfluid-202307031750/funfluid/simulate/ellipse/project/models/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:30.000000 funfluid-202307031750/funfluid/simulate/ellipse/project/models/flow.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1053 2023-07-02 11:30:32.000000 funfluid-202307031750/funfluid/simulate/ellipse/project/project.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.479595 funfluid-202307031750/funfluid/simulate/ellipse/project/track/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       47 2023-07-03 09:47:30.000000 funfluid-202307031750/funfluid/simulate/ellipse/project/track/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     7633 2023-07-03 09:50:57.000000 funfluid-202307031750/funfluid/simulate/ellipse/project/track/plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.479595 funfluid-202307031750/funfluid/simulate/ellipse/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/simulate/ellipse/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      563 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/simulate/ellipse/utils/largs_plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.479595 funfluid-202307031750/funfluid/tecplot/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/tecplot/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.479595 funfluid-202307031750/funfluid/tecplot/templates/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/tecplot/templates/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    15193 2023-06-30 08:50:52.000000 funfluid-202307031750/funfluid/tecplot/templates/templates1.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.479595 funfluid-202307031750/funfluid/tecplot/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/tecplot/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/tecplot/utils/connect.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.483595 funfluid-202307031750/funfluid/temp/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/temp/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1405 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/temp/data_fit.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       98 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/temp/temp1.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.483595 funfluid-202307031750/funfluid/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031750/funfluid/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      262 2023-06-30 08:50:57.000000 funfluid-202307031750/funfluid/utils/log.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      729 2023-06-30 08:50:55.000000 funfluid-202307031750/funfluid/utils/timer.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:50:59.467595 funfluid-202307031750/funfluid.egg-info/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-03 09:50:59.000000 funfluid-202307031750/funfluid.egg-info/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2670 2023-07-03 09:50:59.000000 funfluid-202307031750/funfluid.egg-info/SOURCES.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-07-03 09:50:59.000000 funfluid-202307031750/funfluid.egg-info/dependency_links.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       30 2023-07-03 09:50:59.000000 funfluid-202307031750/funfluid.egg-info/requires.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        9 2023-07-03 09:50:59.000000 funfluid-202307031750/funfluid.egg-info/top_level.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-07-03 09:50:59.483595 funfluid-202307031750/setup.cfg
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      421 2023-07-02 11:44:45.000000 funfluid-202307031750/setup.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.529257 funfluid-202307031751/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:49:06.000000 funfluid-202307031751/LICENSE
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-03 09:51:57.529257 funfluid-202307031751/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       84 2023-07-03 09:06:44.000000 funfluid-202307031751/README.md
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.521257 funfluid-202307031751/funfluid/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        2 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.521257 funfluid-202307031751/funfluid/common/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/common/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.521257 funfluid-202307031751/funfluid/common/base/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/common/base/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2837 2023-06-30 08:49:51.000000 funfluid-202307031751/funfluid/common/base/cache.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.521257 funfluid-202307031751/funfluid/common/flow/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/common/flow/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.521257 funfluid-202307031751/funfluid/common/particle/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/common/particle/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.521257 funfluid-202307031751/funfluid/experiment/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/experiment/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.521257 funfluid-202307031751/funfluid/experiment/chlamydomonas/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.521257 funfluid-202307031751/funfluid/experiment/chlamydomonas/analyse/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/analyse/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4563 2023-06-30 08:50:16.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/analyse/analyse.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.521257 funfluid-202307031751/funfluid/experiment/chlamydomonas/base/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/base/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3815 2023-06-30 08:50:20.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/base/base.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/base/globalconfig.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/experiment/chlamydomonas/detect/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/detect/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2977 2023-06-30 08:50:23.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/detect/background.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4707 2023-06-30 08:50:30.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/detect/contain.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     9205 2023-06-30 08:50:37.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/detect/particle.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/experiment/chlamydomonas/plot/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/plot/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/plot/core.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      239 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/plot/property.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/experiment/chlamydomonas/progress/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/progress/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2909 2023-06-30 08:50:45.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/progress/video_progress.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1573 2023-06-30 08:50:10.000000 funfluid-202307031751/funfluid/experiment/chlamydomonas/run.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/lbm/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       64 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/lbm/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/lbm/core/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       70 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/lbm/core/__init__.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/lbm/core/buff.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    21837 2023-06-30 08:50:49.000000 funfluid-202307031751/funfluid/lbm/core/lattice.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    13442 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/lbm/core/shape.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    10645 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/lbm/core/speed_nb.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/lbm/example/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/lbm/example/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1921 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/lbm/example/example_cavity1.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1994 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/lbm/example/example_cavity3.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3324 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/lbm/example/example_obstacle.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2581 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/lbm/example/example_poiseuille.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3349 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/lbm/example/example_turek.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3662 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/lbm/obs_array.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2364 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/lbm/params.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/simulate/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:53:23.000000 funfluid-202307031751/funfluid/simulate/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/simulate/ellipse/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/simulate/ellipse/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:54:13.000000 funfluid-202307031751/funfluid/simulate/ellipse/analyse.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/simulate/ellipse/example/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/simulate/ellipse/example/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3179 2023-06-30 08:49:55.000000 funfluid-202307031751/funfluid/simulate/ellipse/example/largs_plot_example.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1379 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/simulate/ellipse/plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/simulate/ellipse/project/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:31:46.000000 funfluid-202307031751/funfluid/simulate/ellipse/project/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1441 2023-07-03 09:06:44.000000 funfluid-202307031751/funfluid/simulate/ellipse/project/example.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/simulate/ellipse/project/models/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:36.000000 funfluid-202307031751/funfluid/simulate/ellipse/project/models/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:30.000000 funfluid-202307031751/funfluid/simulate/ellipse/project/models/flow.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1053 2023-07-02 11:30:32.000000 funfluid-202307031751/funfluid/simulate/ellipse/project/project.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/simulate/ellipse/project/track/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       47 2023-07-03 09:47:30.000000 funfluid-202307031751/funfluid/simulate/ellipse/project/track/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     7633 2023-07-03 09:51:55.000000 funfluid-202307031751/funfluid/simulate/ellipse/project/track/plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/simulate/ellipse/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/simulate/ellipse/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      563 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/simulate/ellipse/utils/largs_plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/tecplot/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/tecplot/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/tecplot/templates/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/tecplot/templates/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    15193 2023-06-30 08:50:52.000000 funfluid-202307031751/funfluid/tecplot/templates/templates1.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.525256 funfluid-202307031751/funfluid/tecplot/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/tecplot/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/tecplot/utils/connect.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.529257 funfluid-202307031751/funfluid/temp/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/temp/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1405 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/temp/data_fit.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       98 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/temp/temp1.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.529257 funfluid-202307031751/funfluid/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031751/funfluid/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      262 2023-06-30 08:50:57.000000 funfluid-202307031751/funfluid/utils/log.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      729 2023-06-30 08:50:55.000000 funfluid-202307031751/funfluid/utils/timer.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:51:57.521257 funfluid-202307031751/funfluid.egg-info/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-03 09:51:57.000000 funfluid-202307031751/funfluid.egg-info/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2670 2023-07-03 09:51:57.000000 funfluid-202307031751/funfluid.egg-info/SOURCES.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-07-03 09:51:57.000000 funfluid-202307031751/funfluid.egg-info/dependency_links.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       30 2023-07-03 09:51:57.000000 funfluid-202307031751/funfluid.egg-info/requires.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        9 2023-07-03 09:51:57.000000 funfluid-202307031751/funfluid.egg-info/top_level.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-07-03 09:51:57.529257 funfluid-202307031751/setup.cfg
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      421 2023-07-02 11:44:45.000000 funfluid-202307031751/setup.py
```

### Comparing `funfluid-202307031750/LICENSE` & `funfluid-202307031751/LICENSE`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/common/base/cache.py` & `funfluid-202307031751/funfluid/common/base/cache.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/experiment/chlamydomonas/analyse/analyse.py` & `funfluid-202307031751/funfluid/experiment/chlamydomonas/analyse/analyse.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/experiment/chlamydomonas/base/base.py` & `funfluid-202307031751/funfluid/experiment/chlamydomonas/base/base.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/experiment/chlamydomonas/base/globalconfig.py` & `funfluid-202307031751/funfluid/experiment/chlamydomonas/base/globalconfig.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/experiment/chlamydomonas/detect/background.py` & `funfluid-202307031751/funfluid/experiment/chlamydomonas/detect/background.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/experiment/chlamydomonas/detect/contain.py` & `funfluid-202307031751/funfluid/experiment/chlamydomonas/detect/contain.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/experiment/chlamydomonas/detect/particle.py` & `funfluid-202307031751/funfluid/experiment/chlamydomonas/detect/particle.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/experiment/chlamydomonas/progress/video_progress.py` & `funfluid-202307031751/funfluid/experiment/chlamydomonas/progress/video_progress.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/experiment/chlamydomonas/run.py` & `funfluid-202307031751/funfluid/experiment/chlamydomonas/run.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/lbm/core/buff.py` & `funfluid-202307031751/funfluid/lbm/core/buff.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/lbm/core/lattice.py` & `funfluid-202307031751/funfluid/lbm/core/lattice.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/lbm/core/shape.py` & `funfluid-202307031751/funfluid/lbm/core/shape.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/lbm/core/speed_nb.py` & `funfluid-202307031751/funfluid/lbm/core/speed_nb.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/lbm/example/example_cavity1.py` & `funfluid-202307031751/funfluid/lbm/example/example_cavity1.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/lbm/example/example_cavity3.py` & `funfluid-202307031751/funfluid/lbm/example/example_cavity3.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/lbm/example/example_obstacle.py` & `funfluid-202307031751/funfluid/lbm/example/example_obstacle.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/lbm/example/example_poiseuille.py` & `funfluid-202307031751/funfluid/lbm/example/example_poiseuille.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/lbm/example/example_turek.py` & `funfluid-202307031751/funfluid/lbm/example/example_turek.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/lbm/obs_array.py` & `funfluid-202307031751/funfluid/lbm/obs_array.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/lbm/params.py` & `funfluid-202307031751/funfluid/lbm/params.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/simulate/ellipse/example/largs_plot_example.py` & `funfluid-202307031751/funfluid/simulate/ellipse/example/largs_plot_example.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/simulate/ellipse/plot.py` & `funfluid-202307031751/funfluid/simulate/ellipse/plot.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/simulate/ellipse/project/example.py` & `funfluid-202307031751/funfluid/simulate/ellipse/project/example.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/simulate/ellipse/project/project.py` & `funfluid-202307031751/funfluid/simulate/ellipse/project/project.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/simulate/ellipse/project/track/plot.py` & `funfluid-202307031751/funfluid/simulate/ellipse/project/track/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
     def _get_ellipse_data(self, step, canvas: Canvas):
         a, b = self.a, self.b
         x0, y0 = self.df['x'][step], self.df['y'][step]
         theta = self.df['theta'][step]
         phi = np.array([i / 100. * np.pi for i in range(-1, 201)])
         x = x0 + np.cos(theta) * a * np.cos(phi) - np.sin(theta) * b * np.sin(phi)
-        y = y0 + (np.sin(theta) * a * np.cos(phi) + np.cos(theta) * b * np.sin(phi)) * canvas.aspect
+        y = y0 + (np.sin(theta) * a * np.cos(phi) + np.cos(theta) * b * np.sin(phi)) / canvas.aspect
 
         x[0] = x0
         y[0] = y0
         return x, y
 
     def plot_update(self, step, canvas: Canvas):
         self.lns[0].set_data(self.df['x'][:step], self.df['y'][:step])
```

### Comparing `funfluid-202307031750/funfluid/simulate/ellipse/utils/largs_plot.py` & `funfluid-202307031751/funfluid/simulate/ellipse/utils/largs_plot.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/tecplot/templates/templates1.py` & `funfluid-202307031751/funfluid/tecplot/templates/templates1.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/temp/data_fit.py` & `funfluid-202307031751/funfluid/temp/data_fit.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid/utils/timer.py` & `funfluid-202307031751/funfluid/utils/timer.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307031750/funfluid.egg-info/SOURCES.txt` & `funfluid-202307031751/funfluid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

