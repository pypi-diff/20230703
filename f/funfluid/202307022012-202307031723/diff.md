# Comparing `tmp/funfluid-202307022012.tar.gz` & `tmp/funfluid-202307031723.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funfluid-202307022012.tar", last modified: Sun Jul  2 12:12:03 2023, max compression
+gzip compressed data, was "funfluid-202307031723.tar", last modified: Mon Jul  3 09:23:20 2023, max compression
```

## Comparing `funfluid-202307022012.tar` & `funfluid-202307031723.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.778704 funfluid-202307022012/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:49:06.000000 funfluid-202307022012/LICENSE
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-02 12:12:03.778704 funfluid-202307022012/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      145 2023-06-30 08:49:06.000000 funfluid-202307022012/README.md
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.766703 funfluid-202307022012/funfluid/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        2 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.766703 funfluid-202307022012/funfluid/common/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/common/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.766703 funfluid-202307022012/funfluid/common/base/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/common/base/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2837 2023-06-30 08:49:51.000000 funfluid-202307022012/funfluid/common/base/cache.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.770703 funfluid-202307022012/funfluid/common/flow/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/common/flow/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.770703 funfluid-202307022012/funfluid/common/particle/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/common/particle/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.770703 funfluid-202307022012/funfluid/experiment/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/experiment/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.770703 funfluid-202307022012/funfluid/experiment/chlamydomonas/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.770703 funfluid-202307022012/funfluid/experiment/chlamydomonas/analyse/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/analyse/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4563 2023-06-30 08:50:16.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/analyse/analyse.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.770703 funfluid-202307022012/funfluid/experiment/chlamydomonas/base/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/base/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3815 2023-06-30 08:50:20.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/base/base.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/base/globalconfig.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.774703 funfluid-202307022012/funfluid/experiment/chlamydomonas/detect/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/detect/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2977 2023-06-30 08:50:23.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/detect/background.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4707 2023-06-30 08:50:30.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/detect/contain.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     9205 2023-06-30 08:50:37.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/detect/particle.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.774703 funfluid-202307022012/funfluid/experiment/chlamydomonas/plot/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/plot/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/plot/core.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      239 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/plot/property.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.774703 funfluid-202307022012/funfluid/experiment/chlamydomonas/progress/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/progress/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2909 2023-06-30 08:50:45.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/progress/video_progress.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1573 2023-06-30 08:50:10.000000 funfluid-202307022012/funfluid/experiment/chlamydomonas/run.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.774703 funfluid-202307022012/funfluid/lbm/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       64 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/lbm/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.774703 funfluid-202307022012/funfluid/lbm/core/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       70 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/lbm/core/__init__.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/lbm/core/buff.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    21837 2023-06-30 08:50:49.000000 funfluid-202307022012/funfluid/lbm/core/lattice.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    13442 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/lbm/core/shape.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    10645 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/lbm/core/speed_nb.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.774703 funfluid-202307022012/funfluid/lbm/example/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/lbm/example/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1921 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/lbm/example/example_cavity1.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1994 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/lbm/example/example_cavity3.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3324 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/lbm/example/example_obstacle.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2581 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/lbm/example/example_poiseuille.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3349 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/lbm/example/example_turek.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3662 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/lbm/obs_array.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2364 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/lbm/params.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.774703 funfluid-202307022012/funfluid/simulate/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:53:23.000000 funfluid-202307022012/funfluid/simulate/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.774703 funfluid-202307022012/funfluid/simulate/ellipse/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/simulate/ellipse/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:54:13.000000 funfluid-202307022012/funfluid/simulate/ellipse/analyse.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.778704 funfluid-202307022012/funfluid/simulate/ellipse/example/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/simulate/ellipse/example/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3179 2023-06-30 08:49:55.000000 funfluid-202307022012/funfluid/simulate/ellipse/example/largs_plot_example.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1379 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/simulate/ellipse/plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.778704 funfluid-202307022012/funfluid/simulate/ellipse/project/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:31:46.000000 funfluid-202307022012/funfluid/simulate/ellipse/project/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.778704 funfluid-202307022012/funfluid/simulate/ellipse/project/models/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:36.000000 funfluid-202307022012/funfluid/simulate/ellipse/project/models/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:30.000000 funfluid-202307022012/funfluid/simulate/ellipse/project/models/flow.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1053 2023-07-02 11:30:32.000000 funfluid-202307022012/funfluid/simulate/ellipse/project/project.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.778704 funfluid-202307022012/funfluid/simulate/ellipse/project/track/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       49 2023-06-30 13:36:34.000000 funfluid-202307022012/funfluid/simulate/ellipse/project/track/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     6710 2023-07-02 12:10:06.000000 funfluid-202307022012/funfluid/simulate/ellipse/project/track/plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.778704 funfluid-202307022012/funfluid/simulate/ellipse/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/simulate/ellipse/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      563 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/simulate/ellipse/utils/largs_plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.778704 funfluid-202307022012/funfluid/tecplot/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/tecplot/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.778704 funfluid-202307022012/funfluid/tecplot/templates/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/tecplot/templates/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    15193 2023-06-30 08:50:52.000000 funfluid-202307022012/funfluid/tecplot/templates/templates1.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.778704 funfluid-202307022012/funfluid/tecplot/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/tecplot/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/tecplot/utils/connect.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.778704 funfluid-202307022012/funfluid/temp/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/temp/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1405 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/temp/data_fit.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       98 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/temp/temp1.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.778704 funfluid-202307022012/funfluid/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307022012/funfluid/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      262 2023-06-30 08:50:57.000000 funfluid-202307022012/funfluid/utils/log.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      729 2023-06-30 08:50:55.000000 funfluid-202307022012/funfluid/utils/timer.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-02 12:12:03.766703 funfluid-202307022012/funfluid.egg-info/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-02 12:12:03.000000 funfluid-202307022012/funfluid.egg-info/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2625 2023-07-02 12:12:03.000000 funfluid-202307022012/funfluid.egg-info/SOURCES.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-07-02 12:12:03.000000 funfluid-202307022012/funfluid.egg-info/dependency_links.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       30 2023-07-02 12:12:03.000000 funfluid-202307022012/funfluid.egg-info/requires.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        9 2023-07-02 12:12:03.000000 funfluid-202307022012/funfluid.egg-info/top_level.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-07-02 12:12:03.778704 funfluid-202307022012/setup.cfg
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      421 2023-07-02 11:44:45.000000 funfluid-202307022012/setup.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.676069 funfluid-202307031723/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:49:06.000000 funfluid-202307031723/LICENSE
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-03 09:23:20.676069 funfluid-202307031723/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       84 2023-07-03 09:06:44.000000 funfluid-202307031723/README.md
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.664069 funfluid-202307031723/funfluid/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        2 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.664069 funfluid-202307031723/funfluid/common/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/common/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.668069 funfluid-202307031723/funfluid/common/base/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/common/base/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2837 2023-06-30 08:49:51.000000 funfluid-202307031723/funfluid/common/base/cache.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.668069 funfluid-202307031723/funfluid/common/flow/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/common/flow/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.668069 funfluid-202307031723/funfluid/common/particle/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/common/particle/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.668069 funfluid-202307031723/funfluid/experiment/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/experiment/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.668069 funfluid-202307031723/funfluid/experiment/chlamydomonas/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.668069 funfluid-202307031723/funfluid/experiment/chlamydomonas/analyse/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/analyse/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4563 2023-06-30 08:50:16.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/analyse/analyse.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.672069 funfluid-202307031723/funfluid/experiment/chlamydomonas/base/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/base/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3815 2023-06-30 08:50:20.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/base/base.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/base/globalconfig.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.672069 funfluid-202307031723/funfluid/experiment/chlamydomonas/detect/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/detect/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2977 2023-06-30 08:50:23.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/detect/background.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4707 2023-06-30 08:50:30.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/detect/contain.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     9205 2023-06-30 08:50:37.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/detect/particle.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.672069 funfluid-202307031723/funfluid/experiment/chlamydomonas/plot/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/plot/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/plot/core.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      239 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/plot/property.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.672069 funfluid-202307031723/funfluid/experiment/chlamydomonas/progress/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/progress/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2909 2023-06-30 08:50:45.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/progress/video_progress.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1573 2023-06-30 08:50:10.000000 funfluid-202307031723/funfluid/experiment/chlamydomonas/run.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.672069 funfluid-202307031723/funfluid/lbm/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       64 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/lbm/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.672069 funfluid-202307031723/funfluid/lbm/core/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       70 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/lbm/core/__init__.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/lbm/core/buff.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    21837 2023-06-30 08:50:49.000000 funfluid-202307031723/funfluid/lbm/core/lattice.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    13442 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/lbm/core/shape.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    10645 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/lbm/core/speed_nb.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.676069 funfluid-202307031723/funfluid/lbm/example/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/lbm/example/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1921 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/lbm/example/example_cavity1.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1994 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/lbm/example/example_cavity3.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3324 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/lbm/example/example_obstacle.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2581 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/lbm/example/example_poiseuille.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3349 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/lbm/example/example_turek.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3662 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/lbm/obs_array.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2364 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/lbm/params.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.676069 funfluid-202307031723/funfluid/simulate/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:53:23.000000 funfluid-202307031723/funfluid/simulate/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.676069 funfluid-202307031723/funfluid/simulate/ellipse/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/simulate/ellipse/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:54:13.000000 funfluid-202307031723/funfluid/simulate/ellipse/analyse.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.676069 funfluid-202307031723/funfluid/simulate/ellipse/example/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/simulate/ellipse/example/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3179 2023-06-30 08:49:55.000000 funfluid-202307031723/funfluid/simulate/ellipse/example/largs_plot_example.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1379 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/simulate/ellipse/plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.676069 funfluid-202307031723/funfluid/simulate/ellipse/project/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:31:46.000000 funfluid-202307031723/funfluid/simulate/ellipse/project/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1441 2023-07-03 09:06:44.000000 funfluid-202307031723/funfluid/simulate/ellipse/project/example.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.676069 funfluid-202307031723/funfluid/simulate/ellipse/project/models/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:36.000000 funfluid-202307031723/funfluid/simulate/ellipse/project/models/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:30.000000 funfluid-202307031723/funfluid/simulate/ellipse/project/models/flow.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1053 2023-07-02 11:30:32.000000 funfluid-202307031723/funfluid/simulate/ellipse/project/project.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.676069 funfluid-202307031723/funfluid/simulate/ellipse/project/track/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       49 2023-06-30 13:36:34.000000 funfluid-202307031723/funfluid/simulate/ellipse/project/track/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     7642 2023-07-03 09:23:17.000000 funfluid-202307031723/funfluid/simulate/ellipse/project/track/plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.676069 funfluid-202307031723/funfluid/simulate/ellipse/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/simulate/ellipse/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      563 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/simulate/ellipse/utils/largs_plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.676069 funfluid-202307031723/funfluid/tecplot/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/tecplot/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.676069 funfluid-202307031723/funfluid/tecplot/templates/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/tecplot/templates/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    15193 2023-06-30 08:50:52.000000 funfluid-202307031723/funfluid/tecplot/templates/templates1.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.676069 funfluid-202307031723/funfluid/tecplot/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/tecplot/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/tecplot/utils/connect.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.676069 funfluid-202307031723/funfluid/temp/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/temp/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1405 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/temp/data_fit.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       98 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/temp/temp1.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.676069 funfluid-202307031723/funfluid/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307031723/funfluid/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      262 2023-06-30 08:50:57.000000 funfluid-202307031723/funfluid/utils/log.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      729 2023-06-30 08:50:55.000000 funfluid-202307031723/funfluid/utils/timer.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-03 09:23:20.664069 funfluid-202307031723/funfluid.egg-info/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-03 09:23:20.000000 funfluid-202307031723/funfluid.egg-info/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2670 2023-07-03 09:23:20.000000 funfluid-202307031723/funfluid.egg-info/SOURCES.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-07-03 09:23:20.000000 funfluid-202307031723/funfluid.egg-info/dependency_links.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       30 2023-07-03 09:23:20.000000 funfluid-202307031723/funfluid.egg-info/requires.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        9 2023-07-03 09:23:20.000000 funfluid-202307031723/funfluid.egg-info/top_level.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-07-03 09:23:20.676069 funfluid-202307031723/setup.cfg
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      421 2023-07-02 11:44:45.000000 funfluid-202307031723/setup.py
```

### Comparing `funfluid-202307022012/LICENSE` & `funfluid-202307031723/LICENSE`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/common/base/cache.py` & `funfluid-202307031723/funfluid/common/base/cache.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/experiment/chlamydomonas/analyse/analyse.py` & `funfluid-202307031723/funfluid/experiment/chlamydomonas/analyse/analyse.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/experiment/chlamydomonas/base/base.py` & `funfluid-202307031723/funfluid/experiment/chlamydomonas/base/base.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/experiment/chlamydomonas/base/globalconfig.py` & `funfluid-202307031723/funfluid/experiment/chlamydomonas/base/globalconfig.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/experiment/chlamydomonas/detect/background.py` & `funfluid-202307031723/funfluid/experiment/chlamydomonas/detect/background.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/experiment/chlamydomonas/detect/contain.py` & `funfluid-202307031723/funfluid/experiment/chlamydomonas/detect/contain.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/experiment/chlamydomonas/detect/particle.py` & `funfluid-202307031723/funfluid/experiment/chlamydomonas/detect/particle.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/experiment/chlamydomonas/progress/video_progress.py` & `funfluid-202307031723/funfluid/experiment/chlamydomonas/progress/video_progress.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/experiment/chlamydomonas/run.py` & `funfluid-202307031723/funfluid/experiment/chlamydomonas/run.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/lbm/core/buff.py` & `funfluid-202307031723/funfluid/lbm/core/buff.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/lbm/core/lattice.py` & `funfluid-202307031723/funfluid/lbm/core/lattice.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/lbm/core/shape.py` & `funfluid-202307031723/funfluid/lbm/core/shape.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/lbm/core/speed_nb.py` & `funfluid-202307031723/funfluid/lbm/core/speed_nb.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/lbm/example/example_cavity1.py` & `funfluid-202307031723/funfluid/lbm/example/example_cavity1.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/lbm/example/example_cavity3.py` & `funfluid-202307031723/funfluid/lbm/example/example_cavity3.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/lbm/example/example_obstacle.py` & `funfluid-202307031723/funfluid/lbm/example/example_obstacle.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/lbm/example/example_poiseuille.py` & `funfluid-202307031723/funfluid/lbm/example/example_poiseuille.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/lbm/example/example_turek.py` & `funfluid-202307031723/funfluid/lbm/example/example_turek.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/lbm/obs_array.py` & `funfluid-202307031723/funfluid/lbm/obs_array.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/lbm/params.py` & `funfluid-202307031723/funfluid/lbm/params.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/simulate/ellipse/example/largs_plot_example.py` & `funfluid-202307031723/funfluid/simulate/ellipse/example/largs_plot_example.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/simulate/ellipse/plot.py` & `funfluid-202307031723/funfluid/simulate/ellipse/plot.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/simulate/ellipse/project/project.py` & `funfluid-202307031723/funfluid/simulate/ellipse/project/project.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/simulate/ellipse/project/track/plot.py` & `funfluid-202307031723/funfluid/simulate/ellipse/project/track/plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,42 +18,45 @@
     df.columns = cols
     df['theta'] = (df['theta']) * math.pi
     df = df.reset_index(names='step')
     df['index'] = index
     return df
 
 
-class FlowBase:
-    def __init__(self, width=800, height=200, x_start=0, y_start=0):
+class Canvas:
+    def __init__(self, width=800, height=100, x_start=0, y_start=-0.5, aspect=1, scale=1):
         self.width = width
         self.height = height
         self.x_start = x_start
         self.y_start = y_start
+        self.aspect = aspect
+        self.scale = scale
 
     def plot(self):
         plt.axis([self.x_start, self.width, self.y_start, self.height])
         plt.grid(True)
 
     def figure(self, ax):
         ax.set_xlim(self.x_start, self.x_start + self.width)
         ax.set_ylim(self.y_start, self.y_start + self.height)
-        ax.set_aspect(1)
+        ax.set_aspect(self.aspect)
 
 
 class EllipseTrack:
-    def __init__(self, df, a=10, b=5, color=None, marker=None, *args, **kwargs):
+    def __init__(self, df, a=10, b=5, color=None, marker=None, line_width=1, *args, **kwargs):
         if isinstance(df, str):
             self.df = _load(df)
         else:
             self.df = df
 
         self.a = a
         self.b = b
         self.color = color
         self.marker = marker
+        self.line_width = line_width
         self.snapshot_steps = []
         self.lns = []
 
     def transform(self):
         self.df['xx'] = self.df['x']
         self.df['x'] = self.df['y']
         self.df['y'] = self.df['xx']
@@ -75,76 +78,81 @@
     def max_y(self):
         return self.df['y'].max()
 
     @property
     def max_step(self):
         return self.df['step'].max()
 
-    def add_snapshot(self, step=0, color=None, marker=None):
+    def add_snapshot(self, step=0, color=None, marker=None, line_width=None):
         self.snapshot_steps.append({
             "step": step,
             "color": color or self.color,
-            "marker": marker or self.marker
+            "marker": marker or self.marker,
+            "line_width": line_width or self.line_width
         })
 
-    def plot_ref(self, line_width=0.3):
+    def plot_ref(self, canvas: Canvas):
         self.lns = []
-        self.lns.append(plt.plot([], [], color=self.color, marker=self.marker, linewidth=line_width, alpha=0.8)[0])
-        self.lns.append(plt.plot([], [], color=self.color, marker=self.marker, linewidth=line_width)[0])
+        self.lns.append(plt.plot([], [], color=self.color, marker=self.marker, linewidth=self.line_width, alpha=0.8)[0])
+        self.lns.append(plt.plot([], [], color=self.color, marker=self.marker, linewidth=self.line_width)[0])
 
         for i, record in enumerate(self.snapshot_steps):
-            self.lns.append(plt.plot([], [], color=record['color'], marker=record['marker'], linewidth=line_width)[0])
+            self.lns.append(
+                plt.plot([], [], color=record['color'], marker=record['marker'], linewidth=record['line_width'])[0])
         return self.lns
 
-    def _get_ellipse_data(self, step):
+    def _get_ellipse_data(self, step, canvas: Canvas):
         x0 = self.df['x'][step]
         y0 = self.df['y'][step]
         theta = self.df['theta'][step]
-        phi = np.array([i / 100. * np.pi for i in range(201)])
+        phi = np.array([i / 100. * np.pi for i in range(-1, 201)])
         x = np.cos(theta) * self.a * np.cos(phi) - np.sin(theta) * self.b * np.sin(phi) + x0
         y = np.sin(theta) * self.a * np.cos(phi) + np.cos(theta) * self.b * np.sin(phi) + y0
+        y = y * canvas.aspect
+        x[0] = x0
+        y[0] = y0
         return x, y
 
-    def plot_update(self, step):
+    def plot_update(self, step, canvas: Canvas):
         self.lns[0].set_data(self.df['x'][:step], self.df['y'][:step])
-        self.lns[1].set_data(*self._get_ellipse_data(step=step))
+        self.lns[1].set_data(*self._get_ellipse_data(step=step, canvas=canvas))
 
         for i, record in enumerate(self.snapshot_steps):
             if record['step'] <= step:
-                self.lns[i + 2].set_data(*self._get_ellipse_data(record['step']))
-
+                self.lns[i + 2].set_data(*self._get_ellipse_data(record['step'], canvas=canvas))
+            else:
+                self.lns[i + 2].set_data([], [])
         return self.lns
 
-    def plot(self, step=10):
+    def plot(self, canvas: Canvas = None, step=10):
         fig, ax = plt.subplots()
         ax.set_xlim(0, 100)
         ax.set_ylim(0, 1200)
         ax.set_aspect(1)
         self.plot_ref()
         ani = animation.FuncAnimation(fig=fig,
                                       func=self.plot_update,
                                       frames=[i for i in range(2, self.df['step'].max() - 2, step)],
                                       interval=100,
                                       # init_func=self.plot_ref,
                                       blit=True,
                                       repeat=False
                                       )
-
         plt.show()
         # ani.save("a.gif", writer='imagemagick')
 
 
 class FlowTrack:
-    def __init__(self, flow: FlowBase = None):
-        self.flow = flow
+    def __init__(self, canvas: Canvas = None):
+        self.canvas = canvas
         self.ellipses: List[EllipseTrack] = []
         self.lns = []
 
-    def set_flow(self, flow):
-        self.flow = flow
+    def set_canvas(self, canvas):
+        self.canvas = canvas
 
     def transform(self):
         for ellipse in self.ellipses:
             ellipse.transform()
 
     @property
     def max_x(self):
@@ -169,48 +177,56 @@
             steps = max(steps, ellipse.max_step)
         return steps
 
     def add_ellipse(self, ellipse: EllipseTrack):
         self.ellipses.append(ellipse)
 
     def plot_ref(self, ax):
-        self.flow.figure(ax)
+        self.canvas.figure(ax)
         for ellipse in self.ellipses:
-            self.lns.extend(ellipse.plot_ref())
+            self.lns.extend(ellipse.plot_ref(self.canvas))
 
     def plot_update(self, step=10, title='', *args, **kwargs):
         for ellipse in self.ellipses:
-            ellipse.plot_update(step=step)
-        # self.lns[-1].set_text(f'step={step}')
+            ellipse.plot_update(step=step, canvas=self.canvas)
         self.lns[-1].set_text(title.replace("{step}", str(step)))
         return self.lns
 
-    def plot(self, min_step=2, max_step=None, step=10, title='', gif_path='./trak.gif'):
+    def plot(self, min_step=2, max_step=None, step=10, title='', dpi=1000, gif_path='./trak.gif'):
         max_step = max_step or self.max_step
-
-        fig, ax = plt.subplots()
+        fig, ax = plt.subplots(figsize=(12, 2))
 
         plt.grid(ls='--')
-        plt.xlabel(r'$x/L$')
-        plt.ylabel(r'$y/L$')
-        ax.set_xlim(0, 100)
-        ax.set_ylim(0, 1200)
-        ax.set_aspect(1)
-        plt.tick_params(labelsize=11)
+        font = {'fontfamily': 'Times New Roman', 'style': 'italic'}
+        plt.xlabel(r'x', **font)
+        plt.ylabel(r'y', **font)
+        plt.tick_params(labelsize=11, direction='in')
+
+        def scale_x(temp, position):
+            return temp / self.canvas.scale
+
+        def scale_y(temp, position):
+            return temp / self.canvas.scale - 0.5
+
+        # ax.xaxis.set_major_formatter(FuncFormatter(scale_x))
+        # ax.yaxis.set_major_formatter(FuncFormatter(scale_y))
+
         labels = ax.get_xticklabels() + ax.get_yticklabels()
         [label.set_fontname('Times New Roman') for label in labels]
 
         self.plot_ref(ax)
-        self.lns.append(plt.title('', fontsize=12))
+        self.lns.append(plt.title('', fontsize=12, **font))
 
         ani = animation.FuncAnimation(fig=fig,
                                       # func=self.plot_update,
                                       func=partial(self.plot_update, title=title),
                                       frames=[i for i in range(min_step, max_step, step)],
                                       interval=100,
                                       blit=False,
                                       repeat=False
                                       )
         plt.show()
-        ani.save(gif_path, writer='imagemagick',savefig_kwargs={
-            "bbox_inches" :"tight"
-        })
+        savefig_kwargs = {"bbox_inches": "tight"}
+        ani.save(gif_path, writer='imagemagick',
+                 # dpi=1000,
+                 savefig_kwargs=savefig_kwargs)
+        fig.savefig(gif_path.replace('gif', 'png'), dpi=1000)
```

### Comparing `funfluid-202307022012/funfluid/simulate/ellipse/utils/largs_plot.py` & `funfluid-202307031723/funfluid/simulate/ellipse/utils/largs_plot.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/tecplot/templates/templates1.py` & `funfluid-202307031723/funfluid/tecplot/templates/templates1.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/temp/data_fit.py` & `funfluid-202307031723/funfluid/temp/data_fit.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid/utils/timer.py` & `funfluid-202307031723/funfluid/utils/timer.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307022012/funfluid.egg-info/SOURCES.txt` & `funfluid-202307031723/funfluid.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 funfluid/simulate/__init__.py
 funfluid/simulate/ellipse/__init__.py
 funfluid/simulate/ellipse/analyse.py
 funfluid/simulate/ellipse/plot.py
 funfluid/simulate/ellipse/example/__init__.py
 funfluid/simulate/ellipse/example/largs_plot_example.py
 funfluid/simulate/ellipse/project/__init__.py
+funfluid/simulate/ellipse/project/example.py
 funfluid/simulate/ellipse/project/project.py
 funfluid/simulate/ellipse/project/models/__init__.py
 funfluid/simulate/ellipse/project/models/flow.py
 funfluid/simulate/ellipse/project/track/__init__.py
 funfluid/simulate/ellipse/project/track/plot.py
 funfluid/simulate/ellipse/utils/__init__.py
 funfluid/simulate/ellipse/utils/largs_plot.py
```

