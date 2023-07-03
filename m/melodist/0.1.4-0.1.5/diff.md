# Comparing `tmp/melodist-0.1.4.tar.gz` & `tmp/melodist-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/melodist-0.1.4.tar", last modified: Tue May  5 19:56:48 2020, max compression
+gzip compressed data, was "melodist-0.1.5.tar", last modified: Mon Jul  3 14:26:47 2023, max compression
```

## Comparing `melodist-0.1.4.tar` & `melodist-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,39 @@
-drwxr-xr-x   0 flo        (501) staff       (20)        0 2020-05-05 19:56:48.000000 melodist-0.1.4/
--rw-r--r--   0 flo        (501) staff       (20)     1654 2020-05-05 19:56:48.000000 melodist-0.1.4/PKG-INFO
--rw-r--r--   0 flo        (501) staff       (20)    14073 2020-05-05 19:39:51.000000 melodist-0.1.4/README.md
-drwxr-xr-x   0 flo        (501) staff       (20)        0 2020-05-05 19:56:48.000000 melodist-0.1.4/melodist/
--rw-r--r--   0 flo        (501) staff       (20)     3718 2017-12-21 08:23:47.000000 melodist-0.1.4/melodist/__init__.py
--rw-r--r--   0 flo        (501) staff       (20)     7705 2017-12-13 19:08:37.000000 melodist-0.1.4/melodist/cascade.py
--rw-r--r--   0 flo        (501) staff       (20)    13873 2017-12-21 08:16:03.000000 melodist-0.1.4/melodist/data_io.py
--rw-r--r--   0 flo        (501) staff       (20)     7298 2020-05-05 19:39:51.000000 melodist-0.1.4/melodist/humidity.py
--rw-r--r--   0 flo        (501) staff       (20)    27609 2018-11-21 12:58:44.000000 melodist-0.1.4/melodist/precipitation.py
--rw-r--r--   0 flo        (501) staff       (20)    13699 2020-05-05 19:39:51.000000 melodist-0.1.4/melodist/radiation.py
--rw-r--r--   0 flo        (501) staff       (20)    16151 2020-05-05 19:39:51.000000 melodist-0.1.4/melodist/station.py
--rw-r--r--   0 flo        (501) staff       (20)    11910 2020-05-05 19:39:51.000000 melodist-0.1.4/melodist/stationstatistics.py
--rw-r--r--   0 flo        (501) staff       (20)    13532 2020-05-05 19:39:51.000000 melodist-0.1.4/melodist/temperature.py
-drwxr-xr-x   0 flo        (501) staff       (20)        0 2020-05-05 19:56:48.000000 melodist-0.1.4/melodist/util/
--rw-r--r--   0 flo        (501) staff       (20)        0 2016-03-01 10:35:19.000000 melodist-0.1.4/melodist/util/__init__.py
--rw-r--r--   0 flo        (501) staff       (20)     3046 2017-11-02 10:42:58.000000 melodist-0.1.4/melodist/util/bunch.py
--rw-r--r--   0 flo        (501) staff       (20)    14946 2020-05-05 19:39:51.000000 melodist-0.1.4/melodist/util/util.py
--rw-r--r--   0 flo        (501) staff       (20)     4942 2017-12-15 08:51:06.000000 melodist-0.1.4/melodist/wind.py
-drwxr-xr-x   0 flo        (501) staff       (20)        0 2020-05-05 19:56:48.000000 melodist-0.1.4/melodist.egg-info/
--rw-r--r--   0 flo        (501) staff       (20)     1654 2020-05-05 19:56:47.000000 melodist-0.1.4/melodist.egg-info/PKG-INFO
--rw-r--r--   0 flo        (501) staff       (20)      469 2020-05-05 19:56:48.000000 melodist-0.1.4/melodist.egg-info/SOURCES.txt
--rw-r--r--   0 flo        (501) staff       (20)        1 2020-05-05 19:56:47.000000 melodist-0.1.4/melodist.egg-info/dependency_links.txt
--rw-r--r--   0 flo        (501) staff       (20)       27 2020-05-05 19:56:47.000000 melodist-0.1.4/melodist.egg-info/requires.txt
--rw-r--r--   0 flo        (501) staff       (20)        9 2020-05-05 19:56:47.000000 melodist-0.1.4/melodist.egg-info/top_level.txt
--rw-r--r--   0 flo        (501) staff       (20)       38 2020-05-05 19:56:48.000000 melodist-0.1.4/setup.cfg
--rw-r--r--   0 flo        (501) staff       (20)     1880 2020-05-05 19:55:32.000000 melodist-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:26:47.861371 melodist-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-03 14:26:19.000000 melodist-0.1.5/Licence_GPLv3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15325 2023-07-03 14:26:47.861371 melodist-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-07-03 14:26:19.000000 melodist-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:26:47.857371 melodist-0.1.5/melodist/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-03 14:26:19.000000 melodist-0.1.5/melodist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 14:26:19.000000 melodist-0.1.5/melodist/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-03 14:26:19.000000 melodist-0.1.5/melodist/cascade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-07-03 14:26:19.000000 melodist-0.1.5/melodist/data_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-03 14:26:19.000000 melodist-0.1.5/melodist/humidity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27148 2023-07-03 14:26:19.000000 melodist-0.1.5/melodist/precipitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-07-03 14:26:19.000000 melodist-0.1.5/melodist/radiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-07-03 14:26:19.000000 melodist-0.1.5/melodist/station.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-03 14:26:19.000000 melodist-0.1.5/melodist/stationstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-07-03 14:26:19.000000 melodist-0.1.5/melodist/temperature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:26:47.857371 melodist-0.1.5/melodist/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:26:19.000000 melodist-0.1.5/melodist/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-03 14:26:19.000000 melodist-0.1.5/melodist/util/bunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-07-03 14:26:19.000000 melodist-0.1.5/melodist/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-03 14:26:19.000000 melodist-0.1.5/melodist/wind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:26:47.857371 melodist-0.1.5/melodist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15325 2023-07-03 14:26:47.000000 melodist-0.1.5/melodist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-03 14:26:47.000000 melodist-0.1.5/melodist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:26:47.000000 melodist-0.1.5/melodist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:26:47.000000 melodist-0.1.5/melodist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-03 14:26:47.000000 melodist-0.1.5/melodist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 14:26:47.000000 melodist-0.1.5/melodist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-03 14:26:19.000000 melodist-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-03 14:26:47.861371 melodist-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-03 14:26:19.000000 melodist-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:26:47.861371 melodist-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 14:26:19.000000 melodist-0.1.5/tests/test_humidity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-03 14:26:19.000000 melodist-0.1.5/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-03 14:26:19.000000 melodist-0.1.5/tests/test_precipitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-03 14:26:19.000000 melodist-0.1.5/tests/test_precipitation_5min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-03 14:26:19.000000 melodist-0.1.5/tests/test_radiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 14:26:19.000000 melodist-0.1.5/tests/test_station.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-03 14:26:19.000000 melodist-0.1.5/tests/test_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-03 14:26:19.000000 melodist-0.1.5/tests/test_wind.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `melodist-0.1.4/README.md` & `melodist-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Build Status](https://www.travis-ci.org/kristianfoerster/melodist.svg?branch=master)](https://www.travis-ci.org/kristianfoerster/melodist)
+[![Build Status](https://github.com/kristianfoerster/melodist/actions/workflows/ci.yml/badge.svg)](https://github.com/kristianfoerster/melodist/actions/workflows/ci.yml)
 
 # MELODIST - An open-source MEteoroLOgical observation time series DISaggregation Tool
 
 *Welcome to MELODIST - MEteoroLOgical observation time series DISaggregation Tool*
 
 MELODIST is an open-source toolbox written in Python for disaggregating daily meteorological time series to hourly time steps. It is licensed under GPLv3 (see license file). The software framework consists of disaggregation functions for each variable including temperature, humidity, precipitation, shortwave radiation, and wind speed. These functions can simply be called from a station object, which includes all relevant information about site characteristics. The data management of time series is handled using data frame objects as defined in the pandas package. In this way, input and output data can be easily prepared and processed. For instance, the pandas package is data i/o capable and includes functions to plot time series using the matplotlib library.
 
@@ -121,14 +121,16 @@
 ## References
 Förster, K., Hanzer, F., Winter, B., Marke, T., and Strasser, U.: An open-source MEteoroLOgical observation time series DISaggregation Tool (MELODIST v0.1.1), *Geosci. Model Dev.*, 9, 2315-2333, [doi:10.5194/gmd-9-2315-2016](https://doi.org/10.5194/gmd-9-2315-2016), 2016.
 
 Hanzer, F., Förster, K., Nemec, J., and Strasser, U.: Projected cryospheric and hydrological impacts of 21st century climate change in the Ötztal Alps (Austria) simulated using a physically based approach, *Hydrol. Earth Syst. Sci.*, 22, 1593-1614, [doi:10.5194/hess-22-1593-2018](https://doi.org/10.5194/hess-22-1593-2018), 2018. 
 
 ## Version history
 
+* 0.1.5 (03 Jul 2023):
+  * Fix compatibility with recent numpy/pandas versions
 * 0.1.4 (05 May 2020):
   * Upgraded to warrant pandas compatibility
 * 0.1.3 (21 Nov 2018):
   * Sub-hourly precipitation disaggregation capabilities added along with a [new Jupyter notebook](examples/precip5min_example.ipynb)
   * bugfix in `precipitation.py`
   * speed-up of cascade statistics
 * 0.1.2 (21 Dec 2017):
```

### Comparing `melodist-0.1.4/melodist/__init__.py` & `melodist-0.1.5/melodist/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-# -*- coding: utf-8 -*-
-###############################################################################################################
-# This file is part of MELODIST - MEteoroLOgical observation time series DISaggregation Tool                  #
-# a program to disaggregate daily values of meteorological variables to hourly values                         #
-#                                                                                                             #
-# Copyright (C) 2016  Florian Hanzer (1,2), Kristian Förster (1,2), Benjamin Winter (1,2), Thomas Marke (1)   #
-#                                                                                                             #
-# (1) Institute of Geography, University of Innsbruck, Austria                                                #
-# (2) alpS - Centre for Climate Change Adaptation, Innsbruck, Austria                                         #
-#                                                                                                             #
-# MELODIST is free software: you can redistribute it and/or modify                                            #
-# it under the terms of the GNU General Public License as published by                                        #
-# the Free Software Foundation, either version 3 of the License, or                                           #
-# (at your option) any later version.                                                                         #
-#                                                                                                             #
-# MELODIST is distributed in the hope that it will be useful,                                                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                                              #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the                                                #
-# GNU General Public License for more details.                                                                #
-#                                                                                                             #
-# You should have received a copy of the GNU General Public License                                           #
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.                                       #
-#                                                                                                             #
-###############################################################################################################
+################################################################################
+# This file is part of MELODIST - MEteoroLOgical observation time series       #
+# DISaggregation Tool.                                                         #
+#                                                                              #
+# Copyright (C) 2016-2023 Florian Hanzer, Kristian Förster, Benjamin Winter,   #
+# Thomas Marke                                                                 #
+#                                                                              #
+# MELODIST is free software: you can redistribute it and/or modify it under    #
+# the terms of the GNU General Public License as published by the Free         #
+# Software Foundation, either version 3 of the License, or (at your option)    #
+# any later version.                                                           #
+#                                                                              #
+# MELODIST is distributed in the hope that it will be useful, but WITHOUT ANY  #
+# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS    #
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more        #
+# details.                                                                     #
+#                                                                              #
+# You should have received a copy of the GNU General Public License along with #
+# this program.  If not, see <http://www.gnu.org/licenses/>.                   #
+################################################################################
+from . __version__ import __version__
 
-from __future__ import print_function, division, absolute_import
 from . import cascade
+from .data_io import *
+from .humidity import *
 from .precipitation import *
-from .temperature import *
 from .radiation import *
-from .humidity import *
-from .wind import *
-from .data_io import *
-from .util.util import distribute_equally
 from .station import Station
 from .stationstatistics import StationStatistics
+from .temperature import *
+from .util.util import distribute_equally
+from .wind import *
 
 columns_daily = [
     'tmean',
     'tmin',
     'tmax',
     'precip',
     'glob',
```

### Comparing `melodist-0.1.4/melodist/cascade.py` & `melodist-0.1.5/melodist/cascade.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,101 +1,129 @@
-# -*- coding: utf-8 -*-
-###############################################################################################################
-# This file is part of MELODIST - MEteoroLOgical observation time series DISaggregation Tool                  #
-# a program to disaggregate daily values of meteorological variables to hourly values                         #
-#                                                                                                             #
-# Copyright (C) 2016  Florian Hanzer (1,2), Kristian Förster (1,2), Benjamin Winter (1,2), Thomas Marke (1)   #
-#                                                                                                             #
-# (1) Institute of Geography, University of Innsbruck, Austria                                                #
-# (2) alpS - Centre for Climate Change Adaptation, Innsbruck, Austria                                         #
-#                                                                                                             #
-# MELODIST is free software: you can redistribute it and/or modify                                            #
-# it under the terms of the GNU General Public License as published by                                        #
-# the Free Software Foundation, either version 3 of the License, or                                           #
-# (at your option) any later version.                                                                         #
-#                                                                                                             #
-# MELODIST is distributed in the hope that it will be useful,                                                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                                              #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the                                                #
-# GNU General Public License for more details.                                                                #
-#                                                                                                             #
-# You should have received a copy of the GNU General Public License                                           #
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.                                       #
-#                                                                                                             #
-###############################################################################################################
-
-from __future__ import print_function, division, absolute_import
+################################################################################
+# This file is part of MELODIST - MEteoroLOgical observation time series       #
+# DISaggregation Tool.                                                         #
+#                                                                              #
+# Copyright (C) 2016-2023 Florian Hanzer, Kristian Förster, Benjamin Winter,   #
+# Thomas Marke                                                                 #
+#                                                                              #
+# MELODIST is free software: you can redistribute it and/or modify it under    #
+# the terms of the GNU General Public License as published by the Free         #
+# Software Foundation, either version 3 of the License, or (at your option)    #
+# any later version.                                                           #
+#                                                                              #
+# MELODIST is distributed in the hope that it will be useful, but WITHOUT ANY  #
+# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS    #
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more        #
+# details.                                                                     #
+#                                                                              #
+# You should have received a copy of the GNU General Public License along with #
+# this program.  If not, see <http://www.gnu.org/licenses/>.                   #
+################################################################################
 import numpy as np
 
 """
 cascade.py provides basic definitions for the precipitation disaggregation
 procedure using the cascade model by Olsson (1998)
 """
 
+
 class BoxTypes:
     """BoxTypes represents the type of each box, which can be seen as one
     single value, with respect to its antecessor and follower along the time
     axis, respectively."""
+
     dry, starting, enclosed, ending, isolated = range(5)
 
+
 class CascadeStatistics:
     """CascadeStatistics is a simple data structure including all relevant
     information based on statistical evaluation of hourly data in order to
     run the cascade based disaggregation applying these statistics for
     arbitrary daily precipitation time series."""
+
     def __init__(self):
         """constructor, initializes probability fields"""
-        self.p01 = np.zeros((2,4))
-        self.p10 = np.zeros((2,4))
-        self.pxx = np.zeros((2,4))
-        self.wxx = np.zeros((7,2,4))
-        self.threshold = np.array([ 1.67093133,  2.46694444,  3.66730902,  5.39878419,  8.04924471])
+        self.p01 = np.zeros((2, 4))
+        self.p10 = np.zeros((2, 4))
+        self.pxx = np.zeros((2, 4))
+        self.wxx = np.zeros((7, 2, 4))
+        self.threshold = np.array([1.67093133, 2.46694444, 3.66730902, 5.39878419, 8.04924471])
         self.percentile = 50
 
     def fill_with_sample_data(self):
         """This function fills the corresponding object with sample data."""
         # replace these sample data with another dataset later
         # this function is deprecated as soon as a common file format for this
         # type of data will be available
-        self.p01 = np.array([[0.576724636119866,  0.238722774405744,  0.166532122130638,  0.393474644666218],
-                             [0.303345245644811,  0.0490956843857575, 0.0392403031072856, 0.228441890034704]])
-
-        self.p10 = np.array([[0.158217002255554,  0.256581140990052,  0.557852226779526,  0.422638238585814],
-                             [0.0439831163244427, 0.0474928027621488, 0.303675296728195,  0.217512052135178]])
-
-        self.pxx = np.array([[0.265058361624580,  0.504696084604205,  0.275615651089836,  0.183887116747968],
-                             [0.652671638030746,  0.903411512852094,  0.657084400164519,  0.554046057830118]])
-
-        self.wxx = np.array([[[0.188389148850583, 0.0806836453984190, 0.0698113025807722, 0.0621499191745602],
-                              [0.240993281622128, 0.0831019646519721, 0.0415130545715575, 0.155284541403192]],
-                             [[0.190128959522795, 0.129220679033862,  0.0932213021787505, 0.193080698516532],
-                              [0.196379692358065, 0.108549414860949,  0.0592714297292217, 0.0421945385836429]],
-                             [[0.163043672107111, 0.152063537378127,  0.102823783410167,  0.0906028835221283],
-                              [0.186579466868095, 0.189705690316132,  0.0990207345993082, 0.107831389238912]],
-                             [[0.197765724699431, 0.220046257566978,  0.177876233348082,  0.261288786454262],
-                              [0.123823472714948, 0.220514673922285,  0.102486496386323,  0.101975538893918]],
-                             [[0.114435243444815, 0.170857634762767,  0.177327072603662,  0.135362730582518],
-                              [0.0939211776723413,0.174291820501902,  0.125275822078525,  0.150842841725936]],
-                             [[0.0988683809545079, 0.152323481100248, 0.185606883566286, 0.167242856061538],
-                              [0.0760275616817939, 0.127275603247149,  0.202466168603738,  0.186580243138018]],
-                             [[0.0473688704207573, 0.0948047647595988, 0.193333422312280,  0.0902721256884624],
-                              [0.0822753470826286, 0.0965608324996108, 0.369966294031327,  0.255290907016382]]])
+        self.p01 = np.array(
+            [
+                [0.576724636119866, 0.238722774405744, 0.166532122130638, 0.393474644666218],
+                [0.303345245644811, 0.0490956843857575, 0.0392403031072856, 0.228441890034704],
+            ]
+        )
+
+        self.p10 = np.array(
+            [
+                [0.158217002255554, 0.256581140990052, 0.557852226779526, 0.422638238585814],
+                [0.0439831163244427, 0.0474928027621488, 0.303675296728195, 0.217512052135178],
+            ]
+        )
+
+        self.pxx = np.array(
+            [
+                [0.265058361624580, 0.504696084604205, 0.275615651089836, 0.183887116747968],
+                [0.652671638030746, 0.903411512852094, 0.657084400164519, 0.554046057830118],
+            ]
+        )
+
+        self.wxx = np.array(
+            [
+                [
+                    [0.188389148850583, 0.0806836453984190, 0.0698113025807722, 0.0621499191745602],
+                    [0.240993281622128, 0.0831019646519721, 0.0415130545715575, 0.155284541403192],
+                ],
+                [
+                    [0.190128959522795, 0.129220679033862, 0.0932213021787505, 0.193080698516532],
+                    [0.196379692358065, 0.108549414860949, 0.0592714297292217, 0.0421945385836429],
+                ],
+                [
+                    [0.163043672107111, 0.152063537378127, 0.102823783410167, 0.0906028835221283],
+                    [0.186579466868095, 0.189705690316132, 0.0990207345993082, 0.107831389238912],
+                ],
+                [
+                    [0.197765724699431, 0.220046257566978, 0.177876233348082, 0.261288786454262],
+                    [0.123823472714948, 0.220514673922285, 0.102486496386323, 0.101975538893918],
+                ],
+                [
+                    [0.114435243444815, 0.170857634762767, 0.177327072603662, 0.135362730582518],
+                    [0.0939211776723413, 0.174291820501902, 0.125275822078525, 0.150842841725936],
+                ],
+                [
+                    [0.0988683809545079, 0.152323481100248, 0.185606883566286, 0.167242856061538],
+                    [0.0760275616817939, 0.127275603247149, 0.202466168603738, 0.186580243138018],
+                ],
+                [
+                    [0.0473688704207573, 0.0948047647595988, 0.193333422312280, 0.0902721256884624],
+                    [0.0822753470826286, 0.0965608324996108, 0.369966294031327, 0.255290907016382],
+                ],
+            ]
+        )
 
     def __add__(self, other_casc_obj):
-        self.p01 = self.p01[:,:] + other_casc_obj.p01[:,:]
-        self.p10 = self.p10[:,:] + other_casc_obj.p10[:,:]
-        self.pxx = self.pxx[:,:] + other_casc_obj.pxx[:,:]
-        for k in range(0,7):
-            self.wxx[k,:,:] = self.wxx[k,:,:] + other_casc_obj.wxx[k,:,:]
+        self.p01 = self.p01[:, :] + other_casc_obj.p01[:, :]
+        self.p10 = self.p10[:, :] + other_casc_obj.p10[:, :]
+        self.pxx = self.pxx[:, :] + other_casc_obj.pxx[:, :]
+        for k in range(0, 7):
+            self.wxx[k, :, :] = self.wxx[k, :, :] + other_casc_obj.wxx[k, :, :]
 
     def __mul__(self, factor):
-        self.p01 = self.p01[:,:] * factor
-        self.p10 = self.p10[:,:] * factor
-        self.pxx = self.pxx[:,:] * factor
-        self.wxx = self.wxx[:,:,:] * factor
+        self.p01 = self.p01[:, :] * factor
+        self.p10 = self.p10[:, :] * factor
+        self.pxx = self.pxx[:, :] * factor
+        self.wxx = self.wxx[:, :, :] * factor
 
     def __eq__(self, other):
         return (
             np.array_equal(self.p01, other.p01)
             and np.array_equal(self.p10, other.p10)
             and np.array_equal(self.pxx, other.pxx)
             and np.array_equal(self.wxx, other.wxx)
```

### Comparing `melodist-0.1.4/melodist/data_io.py` & `melodist-0.1.5/melodist/data_io.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-# -*- coding: utf-8 -*-
-###############################################################################################################
-# This file is part of MELODIST - MEteoroLOgical observation time series DISaggregation Tool                  #
-# a program to disaggregate daily values of meteorological variables to hourly values                         #
-#                                                                                                             #
-# Copyright (C) 2016  Florian Hanzer (1,2), Kristian Förster (1,2), Benjamin Winter (1,2), Thomas Marke (1)   #
-#                                                                                                             #
-# (1) Institute of Geography, University of Innsbruck, Austria                                                #
-# (2) alpS - Centre for Climate Change Adaptation, Innsbruck, Austria                                         #
-#                                                                                                             #
-# MELODIST is free software: you can redistribute it and/or modify                                            #
-# it under the terms of the GNU General Public License as published by                                        #
-# the Free Software Foundation, either version 3 of the License, or                                           #
-# (at your option) any later version.                                                                         #
-#                                                                                                             #
-# MELODIST is distributed in the hope that it will be useful,                                                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                                              #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the                                                #
-# GNU General Public License for more details.                                                                #
-#                                                                                                             #
-# You should have received a copy of the GNU General Public License                                           #
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.                                       #
-#                                                                                                             #
-###############################################################################################################
-
+################################################################################
+# This file is part of MELODIST - MEteoroLOgical observation time series       #
+# DISaggregation Tool.                                                         #
+#                                                                              #
+# Copyright (C) 2016-2023 Florian Hanzer, Kristian Förster, Benjamin Winter,   #
+# Thomas Marke                                                                 #
+#                                                                              #
+# MELODIST is free software: you can redistribute it and/or modify it under    #
+# the terms of the GNU General Public License as published by the Free         #
+# Software Foundation, either version 3 of the License, or (at your option)    #
+# any later version.                                                           #
+#                                                                              #
+# MELODIST is distributed in the hope that it will be useful, but WITHOUT ANY  #
+# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS    #
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more        #
+# details.                                                                     #
+#                                                                              #
+# You should have received a copy of the GNU General Public License along with #
+# this program.  If not, see <http://www.gnu.org/licenses/>.                   #
+################################################################################
+import collections
 import glob
-import melodist
+
 import pandas as pd
-import numpy as np
-import collections
 
 
 def read_smet(filename, mode):
     """Reads smet data and returns the data in required dataformat (pd df)
 
     See https://models.slf.ch/docserver/meteoio/SMET_specifications.pdf
     for further details on the specifications of this file format.
@@ -47,36 +41,33 @@
     header:    header as dict
     data :     data as pd df
     """
 
     # dictionary
     # based on smet spec V.1.1 and self defined
     # daily data
-    dict_d = {'TA': 'tmean',
-              'TMAX': 'tmax',   # no spec
-              'TMIN': 'tmin',   # no spec
-              'PSUM': 'precip',
-              'ISWR': 'glob',     # no spec
-              'RH': 'hum',
-              'VW': 'wind'}
+    dict_d = {
+        'TA': 'tmean',
+        'TMAX': 'tmax',  # no spec
+        'TMIN': 'tmin',  # no spec
+        'PSUM': 'precip',
+        'ISWR': 'glob',  # no spec
+        'RH': 'hum',
+        'VW': 'wind',
+    }
 
     # hourly data
-    dict_h = {'TA': 'temp',
-              'PSUM': 'precip',
-              'ISWR': 'glob',     # no spec
-              'RH': 'hum',
-              'VW': 'wind'}
+    dict_h = {'TA': 'temp', 'PSUM': 'precip', 'ISWR': 'glob', 'RH': 'hum', 'VW': 'wind'}
 
     with open(filename) as f:
         in_header = False
         data_start = None
         header = collections.OrderedDict()
 
         for line_num, line in enumerate(f):
-
             if line.strip() == '[HEADER]':
                 in_header = True
                 continue
             elif line.strip() == '[DATA]':
                 data_start = line_num + 1
                 break
 
@@ -94,92 +85,93 @@
         filename,
         sep=r'\s+',
         na_values=[-999],
         skiprows=data_start,
         names=columns,
         index_col='timestamp',
         parse_dates=True,
-        )
+    )
 
-    data = data*multiplier
+    data = data * multiplier
 
     del data.index.name
 
     # rename columns
     if mode == "d":
         data = data.rename(columns=dict_d)
     if mode == "h":
         data = data.rename(columns=dict_h)
 
     return header, data
-    
+
 
 def read_dwd(filename, metadata, mode="d", skip_last=True):
     """Reads dwd (German Weather Service) data and returns the data in required
     dataformat (pd df)
 
     Parameters
     ----
-    filename : DWD file to read (full path) / list of hourly files (RR+TU+FF) 
+    filename : DWD file to read (full path) / list of hourly files (RR+TU+FF)
     metadata : corresponding DWD metadata file to read
     mode :    "d" for daily and "h" for hourly input
     skip_last : boolen, skips last line due to file format
 
     Returns
     ----
     [header, data]
     header:    header as dict
     data :     data as pd df
     """
 
     def read_single_dwd(filename, metadata, mode, skip_last):
         # Param names {'DWD':'dissag_def'}
-        dict_d = {'LUFTTEMPERATUR': 'tmean',
-                  'LUFTTEMPERATUR_MINIMUM': 'tmin',   # no spec
-                  'LUFTTEMPERATUR_MAXIMUM': 'tmax',   # no spec
-                  'NIEDERSCHLAGSHOEHE': 'precip',
-                  'GLOBAL_KW_J': 'glob',     # no spec
-                  'REL_FEUCHTE': 'hum',
-                  'WINDGESCHWINDIGKEIT': 'wind',
-                  'SONNENSCHEINDAUER': 'sun_h'}
+        dict_d = {
+            'LUFTTEMPERATUR': 'tmean',
+            'LUFTTEMPERATUR_MINIMUM': 'tmin',  # no spec
+            'LUFTTEMPERATUR_MAXIMUM': 'tmax',  # no spec
+            'NIEDERSCHLAGSHOEHE': 'precip',
+            'GLOBAL_KW_J': 'glob',  # no spec
+            'REL_FEUCHTE': 'hum',
+            'WINDGESCHWINDIGKEIT': 'wind',
+            'SONNENSCHEINDAUER': 'sun_h',
+        }
 
         # ---read meta------------------
-        meta = pd.read_csv(
-            metadata,
-            sep=';'
-            )
+        meta = pd.read_csv(metadata, sep=';')
 
         # remove whitespace from header columns
         meta.rename(columns=lambda x: x.strip(), inplace=True)
 
-        header = {"Stations_id": meta.Stations_id[meta.last_valid_index()],
-                  "Stationsname": meta.Stationsname[meta.last_valid_index()],
-                  # workaround for colnames with . (Geogr.Breite)
-                  "Breite": meta.iloc[meta.last_valid_index(), 2],  # DezDeg
-                  "Laenge": meta.iloc[meta.last_valid_index(), 3]   # DezDeg
-                  }
+        header = {
+            "Stations_id": meta.Stations_id[meta.last_valid_index()],
+            "Stationsname": meta.Stationsname[meta.last_valid_index()],
+            # workaround for colnames with . (Geogr.Breite)
+            "Breite": meta.iloc[meta.last_valid_index(), 2],  # DezDeg
+            "Laenge": meta.iloc[meta.last_valid_index(), 3],  # DezDeg
+        }
 
         # ---read data------------------
         if skip_last is not None:
             num_lines = sum(1 for line in open(filename))
-            skip_last = [num_lines-1]
+            skip_last = [num_lines - 1]
 
         # hourly data must be parsed by custom definition
         if mode == "d":
             data = pd.read_csv(
                 filename,
                 sep=';',
                 na_values='-999',
                 index_col=' MESS_DATUM',
                 parse_dates=True,
-                skiprows=skip_last
-                )
+                skiprows=skip_last,
+            )
 
         # hourly data must be parsed by custom definition
         if mode == "h":
+
             def date_parser(date_time):
                 hour = date_time[8:10]
                 day = date_time[6:8]
                 month = date_time[4:6]
                 year = date_time[0:4]
                 minute = '00'
                 sec = '00'
@@ -187,16 +179,16 @@
 
             data = pd.read_csv(
                 filename,
                 sep=';',
                 na_values='-999',
                 index_col=' MESS_DATUM',
                 date_parser=date_parser,
-                skiprows=skip_last
-                )
+                skiprows=skip_last,
+            )
 
         # remove whitespace from header columns
         data.rename(columns=lambda x: x.strip(), inplace=True)
 
         # rename to dissag definition
         data = data.rename(columns=dict_d)
         # get colums which are not defined
@@ -239,80 +231,75 @@
     Parameters
     ----
     filename :    filename/loction of output
     data :        data to write as pandas df
     metadata:     header to write input as dict
     nodata_value: Nodata Value to write/use
     mode:         defines if to write daily ("d") or continuos data (default 'h')
-    check_nan:    will check if only nans in data and if true will not write this colums (default True)
+    check_nan:    will check if only nans in data and if true will not write this columns
+                  (default True)
     """
 
     # dictionary
     # based on smet spec V.1.1 and selfdefined
     # daily data
-    dict_d=   {'tmean':'TA',
-               'tmin':'TMAX',   #no spec
-               'tmax':'TMIN',   #no spec
-               'precip':'PSUM',
-               'glob':'ISWR',     #no spec
-               'hum':'RH',
-               'wind':'VW'
-                }
-
-    #hourly data
-    dict_h=   {'temp':'TA',
-               'precip':'PSUM',
-               'glob':'ISWR',     #no spec
-               'hum':'RH',
-               'wind':'VW'
-                }
-                
-    #rename columns
+    dict_d = {
+        'tmean': 'TA',
+        'tmin': 'TMAX',  # no spec
+        'tmax': 'TMIN',  # no spec
+        'precip': 'PSUM',
+        'glob': 'ISWR',  # no spec
+        'hum': 'RH',
+        'wind': 'VW',
+    }
+
+    # hourly data
+    dict_h = {'temp': 'TA', 'precip': 'PSUM', 'glob': 'ISWR', 'hum': 'RH', 'wind': 'VW'}
+
+    # rename columns
     if mode == "d":
         data = data.rename(columns=dict_d)
     if mode == "h":
         data = data.rename(columns=dict_h)
 
-    if check_nan:     
-        #get all colums with data
+    if check_nan:
+        # get all columns with data
         datas_in = data.sum().dropna().to_frame().T
-        #get colums with no datas
-        drop = [data_nan for data_nan in data.columns if data_nan not in datas_in]    
-        #delete columns
+        # get colums with no datas
+        drop = [data_nan for data_nan in data.columns if data_nan not in datas_in]
+        # delete columns
         data = data.drop(drop, axis=1)
-    
-    with open(filename, 'w') as f:
 
-        #preparing data
-        #converte date_times to SMET timestamps
+    with open(filename, 'w') as f:
+        # preparing data
+        # convert date_times to SMET timestamps
         if mode == "d":
             t = '%Y-%m-%dT00:00'
         if mode == "h":
             t = '%Y-%m-%dT%H:%M'
 
         data['timestamp'] = [d.strftime(t) for d in data.index]
-        
+
         cols = data.columns.tolist()
         cols = cols[-1:] + cols[:-1]
         data = data[cols]
 
-
-        #metadatas update
+        # metadatas update
         metadata['fields'] = ' '.join(data.columns)
-        metadata["units_multiplier"] = len(metadata['fields'].split())*"1 "
+        metadata["units_multiplier"] = len(metadata['fields'].split()) * "1 "
 
-        #writing data
-        #metadata
+        # writing data
+        # metadata
         f.write('SMET 1.1 ASCII\n')
         f.write('[HEADER]\n')
 
         for k, v in metadata.items():
             f.write('{} = {}\n'.format(k, v))
 
-        #data
+        # data
         f.write('[DATA]\n')
 
         data_str = data.fillna(nodata_value).to_string(
             header=False,
             index=False,
             float_format=lambda x: '{:.2f}'.format(x),
         )
@@ -330,18 +317,17 @@
 
     Returns:
         pandas data frame including time series
     """
     hourly_data_obs_raw = pd.read_csv(
         filename,
         parse_dates=[['YYYYMMDD', 'HH']],
-        date_parser=lambda yyyymmdd, hh: pd.datetime(int(str(yyyymmdd)[0:4]),
-                                                     int(str(yyyymmdd)[4:6]),
-                                                     int(str(yyyymmdd)[6:8]),
-                                                     int(hh) - 1),
+        date_parser=lambda yyyymmdd, hh: pd.datetime(
+            int(str(yyyymmdd)[0:4]), int(str(yyyymmdd)[4:6]), int(str(yyyymmdd)[6:8]), int(hh) - 1
+        ),
         skiprows=31,
         skipinitialspace=True,
         na_values='',
         keep_date_col=True,
     )
 
     hourly_data_obs_raw.index = hourly_data_obs_raw['YYYYMMDD_HH']
@@ -351,15 +337,15 @@
 
     hourly_data_obs = pd.DataFrame(
         index=hourly_data_obs_raw.index,
         columns=columns_hourly,
         data=dict(
             temp=hourly_data_obs_raw['T'] / 10 + 273.15,
             precip=hourly_data_obs_raw['RH'] / 10,
-            glob=hourly_data_obs_raw['Q'] * 10000 / 3600.,
+            glob=hourly_data_obs_raw['Q'] * 10000 / 3600.0,
             hum=hourly_data_obs_raw['U'],
             wind=hourly_data_obs_raw['FH'] / 10,
             ssd=hourly_data_obs_raw['SQ'] * 6,
         ),
     )
     # remove negative values
     negative_values = hourly_data_obs['precip'] < 0.0
@@ -385,13 +371,13 @@
     columns_hourly = ['temp', 'precip', 'glob', 'hum', 'wind', 'ssd']
     ts = pd.DataFrame(columns=columns_hourly)
 
     first_call = True
     for file_i in filelist:
         print(file_i)
         current = read_single_knmi_file(file_i)
-        if(first_call):
+        if first_call:
             ts = current
             first_call = False
         else:
             ts = pd.concat([ts, current])
     return ts
```

### Comparing `melodist-0.1.4/melodist/humidity.py` & `melodist-0.1.5/melodist/humidity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,66 @@
-# -*- coding: utf-8 -*-
-###############################################################################################################
-# This file is part of MELODIST - MEteoroLOgical observation time series DISaggregation Tool                  #
-# a program to disaggregate daily values of meteorological variables to hourly values                         #
-#                                                                                                             #
-# Copyright (C) 2016  Florian Hanzer (1,2), Kristian Förster (1,2), Benjamin Winter (1,2), Thomas Marke (1)   #
-#                                                                                                             #
-# (1) Institute of Geography, University of Innsbruck, Austria                                                #
-# (2) alpS - Centre for Climate Change Adaptation, Innsbruck, Austria                                         #
-#                                                                                                             #
-# MELODIST is free software: you can redistribute it and/or modify                                            #
-# it under the terms of the GNU General Public License as published by                                        #
-# the Free Software Foundation, either version 3 of the License, or                                           #
-# (at your option) any later version.                                                                         #
-#                                                                                                             #
-# MELODIST is distributed in the hope that it will be useful,                                                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                                              #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the                                                #
-# GNU General Public License for more details.                                                                #
-#                                                                                                             #
-# You should have received a copy of the GNU General Public License                                           #
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.                                       #
-#                                                                                                             #
-###############################################################################################################
+################################################################################
+# This file is part of MELODIST - MEteoroLOgical observation time series       #
+# DISaggregation Tool.                                                         #
+#                                                                              #
+# Copyright (C) 2016-2023 Florian Hanzer, Kristian Förster, Benjamin Winter,   #
+# Thomas Marke                                                                 #
+#                                                                              #
+# MELODIST is free software: you can redistribute it and/or modify it under    #
+# the terms of the GNU General Public License as published by the Free         #
+# Software Foundation, either version 3 of the License, or (at your option)    #
+# any later version.                                                           #
+#                                                                              #
+# MELODIST is distributed in the hope that it will be useful, but WITHOUT ANY  #
+# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS    #
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more        #
+# details.                                                                     #
+#                                                                              #
+# You should have received a copy of the GNU General Public License along with #
+# this program.  If not, see <http://www.gnu.org/licenses/>.                   #
+################################################################################
+import numpy as np
+import pandas as pd
 
-from __future__ import print_function, division, absolute_import
 import melodist
 import melodist.util.util as util
-import numpy as np
-import pandas as pd
 
 
-def disaggregate_humidity(data_daily, method='equal', temp=None,
-                          a0=None, a1=None, kr=None,
-                          month_hour_precip_mean=None, preserve_daily_mean=False):
+def disaggregate_humidity(
+    data_daily,
+    method='equal',
+    temp=None,
+    a0=None,
+    a1=None,
+    kr=None,
+    month_hour_precip_mean=None,
+    preserve_daily_mean=False,
+):
     """general function for humidity disaggregation
 
     Args:
         daily_data: daily values
         method: keyword specifying the disaggregation method to be used
         temp: hourly temperature time series (necessary for some methods)
         kr: parameter for linear_dewpoint_variation method (6 or 12)
         month_hour_precip_mean: [month, hour, precip(y/n)] categorical mean values
         preserve_daily_mean: if True, correct the daily mean values of the disaggregated
             data with the observed daily means.
 
     Returns:
         Disaggregated hourly values of relative humidity.
     """
-    assert method in ('equal',
-                      'minimal',
-                      'dewpoint_regression',
-                      'min_max',
-                      'linear_dewpoint_variation',
-                      'month_hour_precip_mean'), 'Invalid option'
+    assert method in (
+        'equal',
+        'minimal',
+        'dewpoint_regression',
+        'min_max',
+        'linear_dewpoint_variation',
+        'month_hour_precip_mean',
+    ), 'Invalid option'
 
     if method == 'equal':
         hum_disagg = melodist.distribute_equally(data_daily.hum)
     elif method in ('minimal', 'dewpoint_regression', 'linear_dewpoint_variation'):
         if method == 'minimal':
             a0 = 0
             a1 = 1
@@ -65,66 +69,73 @@
         tdew_daily = a0 + a1 * data_daily.tmin
 
         tdew = melodist.distribute_equally(tdew_daily)
 
         if method == 'linear_dewpoint_variation':
             assert kr is not None, 'kr must be specified'
             assert kr in (6, 12), 'kr must be 6 or 12'
-            tdew_delta = 0.5 * np.sin((temp.index.hour + 1) * np.pi / kr - 3. * np.pi / 4.)  # eq. (21) from Debele et al. (2007)
+            tdew_delta = 0.5 * np.sin(
+                (temp.index.hour + 1) * np.pi / kr - 3.0 * np.pi / 4.0
+            )  # eq. (21) from Debele et al. (2007)
 
             tdew_nextday = tdew.shift(-24)
             tdew_nextday.iloc[-24:] = tdew.iloc[-24:]  # copy the last day
 
             # eq. (20) from Debele et al. (2007):
-            # (corrected - the equation is wrong both in Debele et al. (2007) and Bregaglio et al. (2010) - it should
-            # be (T_dp,day)_(d+1) - (T_dp,day)_d instead of the other way around)
-            tdew += temp.index.hour / 24. * (tdew_nextday - tdew) + tdew_delta
+            # (corrected - the equation is wrong both in Debele et al. (2007) and Bregaglio et al.
+            # (2010) - it should be (T_dp,day)_(d+1) - (T_dp,day)_d instead of the other way around)
+            tdew += temp.index.hour / 24.0 * (tdew_nextday - tdew) + tdew_delta
 
         sat_vap_press_tdew = util.vapor_pressure(tdew, 100)
         sat_vap_press_t = util.vapor_pressure(temp, 100)
         hum_disagg = pd.Series(index=temp.index, data=100 * sat_vap_press_tdew / sat_vap_press_t)
     elif method == 'min_max':
-        assert 'hum_min' in data_daily.columns and 'hum_max' in data_daily.columns, \
-            'Minimum and maximum humidity must be present in data frame'
+        assert (
+            'hum_min' in data_daily.columns and 'hum_max' in data_daily.columns
+        ), 'Minimum and maximum humidity must be present in data frame'
 
         hmin = melodist.distribute_equally(data_daily.hum_min)
         hmax = melodist.distribute_equally(data_daily.hum_max)
         tmin = melodist.distribute_equally(data_daily.tmin)
         tmax = melodist.distribute_equally(data_daily.tmax)
 
         hum_disagg = hmax + (temp - tmin) / (tmax - tmin) * (hmin - hmax)
     elif method == 'month_hour_precip_mean':
         assert month_hour_precip_mean is not None
 
-        precip_equal = melodist.distribute_equally(data_daily.precip)  # daily precipitation equally distributed to hourly values
+        precip_equal = melodist.distribute_equally(
+            data_daily.precip
+        )  # daily precipitation equally distributed to hourly values
         hum_disagg = pd.Series(index=precip_equal.index, dtype=float)
         locs = list(zip(hum_disagg.index.month, hum_disagg.index.hour, precip_equal > 0))
         hum_disagg[:] = month_hour_precip_mean.loc[locs].values
 
     if preserve_daily_mean:
-        daily_mean_df = pd.DataFrame(data=dict(obs=data_daily.hum, disagg=hum_disagg.resample('D').mean()))
+        daily_mean_df = pd.DataFrame(
+            data=dict(obs=data_daily.hum, disagg=hum_disagg.resample('D').mean())
+        )
         bias = melodist.util.distribute_equally(daily_mean_df.disagg - daily_mean_df.obs)
         bias = bias.fillna(0)
         hum_disagg -= bias
 
     return hum_disagg.clip(0, 100)
 
 
 def calculate_dewpoint_regression(hourly_data_obs, return_stats=False):
     temphum = hourly_data_obs[['temp', 'hum']]
 
     tdew = melodist.util.dewpoint_temperature(temphum.temp, temphum.hum).resample('D').mean()
-    tmin = temphum.temp.groupby(temphum.index.date).min()
+    tmin = temphum.temp.groupby(temphum.index.normalize()).min()
     df = pd.DataFrame(data=dict(tmin=tmin, tdew=tdew)).dropna(how='any')
 
     return util.linregress(df.tmin, df.tdew, return_stats=return_stats)
 
 
 def calculate_month_hour_precip_mean(hourly_data_obs):
-    daily_precip_yesno = (hourly_data_obs.precip.resample('D').sum() > 0)
+    daily_precip_yesno = hourly_data_obs.precip.resample('D').sum() > 0
     daily_precip_yesno.index.name = None
     hum = hourly_data_obs.hum
     hum.index.name = None
     wet = daily_precip_yesno.loc[hum.index.date].values
     mhp_mean = hum.groupby([hum.index.month, hum.index.hour, wet]).mean()
 
     return mhp_mean
```

### Comparing `melodist-0.1.4/melodist/precipitation.py` & `melodist-0.1.5/melodist/precipitation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,46 @@
-# -*- coding: utf-8 -*-
-########################################################################
-# This file is part of MELODIST - MEteoroLOgical observation time      #
-# series DISaggregation Tool a program to disaggregate daily values    #
-# of meteorological variables to hourly values                         #
-#                                                                      #
-#                                                                      #
-# Copyright (C) 2016  Florian Hanzer (1, 2), Kristian Förster (1, 2),  #
-# Benjamin Winter (1, 2), Thomas Marke (1)                             #
-#                                                                      #
-# (1) Institute of Geography, University of Innsbruck, Austria         #
-# (2) alpS - Centre for Climate Change Adaptation, Innsbruck, Austria  #
-#                                                                      #
-# MELODIST is free software: you can redistribute it and/or modify     #
-# it under the terms of the GNU General Public License as published by #
-# the Free Software Foundation, either version 3 of the License, or    #
-# (at your option) any later version.                                  #
-#                                                                      #
-# MELODIST is distributed in the hope that it will be useful,          #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of       #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the         #
-# GNU General Public License for more details.                         #
-#                                                                      #
-# You should have received a copy of the GNU General Public License    #
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.#
-#                                                                      #
-########################################################################
-
-# Update 2018: Allow cascade-based disaggregation from daily data
-# to 5 minutes data (9, 10, or 11 levels of branching)
-# Author: Siling Chen
-
-from __future__ import print_function, division, absolute_import
+################################################################################
+# This file is part of MELODIST - MEteoroLOgical observation time series       #
+# DISaggregation Tool.                                                         #
+#                                                                              #
+# Copyright (C) 2016-2023 Florian Hanzer, Kristian Förster, Benjamin Winter,   #
+# Thomas Marke, Siling Chen                                                    #
+#                                                                              #
+# MELODIST is free software: you can redistribute it and/or modify it under    #
+# the terms of the GNU General Public License as published by the Free         #
+# Software Foundation, either version 3 of the License, or (at your option)    #
+# any later version.                                                           #
+#                                                                              #
+# MELODIST is distributed in the hope that it will be useful, but WITHOUT ANY  #
+# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS    #
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more        #
+# details.                                                                     #
+#                                                                              #
+# You should have received a copy of the GNU General Public License along with #
+# this program.  If not, see <http://www.gnu.org/licenses/>.                   #
+################################################################################
+import copy
 
 import numpy as np
 import pandas as pd
 
-import copy
 import melodist
 import melodist.util
 
 from . import cascade
 
 
-def disagg_prec(dailyData,
-                method='equal',
-                cascade_options=None,
-                hourly_data_obs=None,
-                zerodiv="uniform",
-                shift=0):
+def disagg_prec(
+    dailyData,
+    method='equal',
+    cascade_options=None,
+    hourly_data_obs=None,
+    zerodiv="uniform",
+    shift=0,
+):
     """The disaggregation function for precipitation.
 
     Parameters
     ----------
     dailyData : pd.Series
         daily data
     method : str
@@ -68,41 +57,33 @@
         7:00 to 6:00)
     """
 
     if method not in ('equal', 'cascade', 'masterstation'):
         raise ValueError('Invalid option')
 
     if method == 'equal':
-        precip_disagg = melodist.distribute_equally(dailyData.precip,
-                                                    divide=True)
+        precip_disagg = melodist.distribute_equally(dailyData.precip, divide=True)
     elif method == 'masterstation':
-        precip_disagg = precip_master_station(dailyData,
-                                              hourly_data_obs,
-                                              zerodiv)
+        precip_disagg = precip_master_station(dailyData, hourly_data_obs, zerodiv)
     elif method == 'cascade':
         assert cascade_options is not None
-        precip_disagg = disagg_prec_cascade(dailyData,
-                                            cascade_options,
-                                            shift=shift)
+        precip_disagg = disagg_prec_cascade(dailyData, cascade_options, shift=shift)
 
     return precip_disagg
 
 
-def disagg_prec_cascade(precip_daily, 
-                        cascade_options, hourly=True,level=9,
-                        shift=0,
-                        test=False):
+def disagg_prec_cascade(precip_daily, cascade_options, hourly=True, level=9, shift=0, test=False):
     """Precipitation disaggregation with cascade model (Olsson, 1998)
 
     Parameters
     ----------
     precip_daily : pd.Series
         daily data
     hourly: Boolean (for an hourly resolution disaggregation)
-        if False, then returns 5-min disaggregated precipitation 
+        if False, then returns 5-min disaggregated precipitation
         (disaggregation level depending on the "level" variable)
     cascade_options : cascade object
         including statistical parameters for the cascade model
     shift : int
         shifts the precipitation data by shift steps (eg +7 for 7:00 to
         6:00)
     test : bool
@@ -127,53 +108,46 @@
     if isinstance(cascade_options, melodist.cascade.CascadeStatistics):
         # this is the standard case considering one data set for all levels
         # get cumulative probabilities for branching
         overwrite_stats = False
         for k in range(0, 7):
             wxxcum[k, :, :] = cascade_options.wxx[k, :, :]
             if k > 0:
-                wxxcum[k, :, :] = wxxcum[k-1, :, :] + wxxcum[k, :, :]
+                wxxcum[k, :, :] = wxxcum[k - 1, :, :] + wxxcum[k, :, :]
     elif isinstance(cascade_options, list):
-        if len(cascade_options) == si:#5
+        if len(cascade_options) == si:  # 5
             overwrite_stats = True
             list_casc = cascade_options
         else:
             raise ValueError('Cascade statistics list must have %s elements!' % si)
     else:
         raise TypeError('cascade_options has invalid type')
 
     # arrays for each level
     n = len(precip_daily)
-    vdn1 = np.zeros(n*2)
-    vdn2 = np.zeros(n*4)
-    vdn3 = np.zeros(n*8)
-    vdn4 = np.zeros(n*16)
-    vdn5 = np.zeros(n*32)
+    vdn1 = np.zeros(n * 2)
+    vdn2 = np.zeros(n * 4)
+    vdn3 = np.zeros(n * 8)
+    vdn4 = np.zeros(n * 16)
+    vdn5 = np.zeros(n * 32)
     if not hourly:
-        vdn6 = np.zeros(n*64)
-        vdn7 = np.zeros(n*128)
-        vdn8 = np.zeros(n*256)
-        vdn9 = np.zeros(n*512)
+        vdn6 = np.zeros(n * 64)
+        vdn7 = np.zeros(n * 128)
+        vdn8 = np.zeros(n * 256)
+        vdn9 = np.zeros(n * 512)
     if level == 10 or level == 11:
-        vdn10 = np.zeros(n*1024)
+        vdn10 = np.zeros(n * 1024)
         if level == 11:
-            vdn11 = np.zeros(n*2048)
-            
+            vdn11 = np.zeros(n * 2048)
+
     # class boundaries for histograms
-    wclassbounds = np.array([0.0,
-                             0.1429,
-                             0.2857,
-                             0.4286,
-                             0.5714,
-                             0.7143,
-                             0.8571,
-                             1.0])
+    wclassbounds = np.array([0.0, 0.1429, 0.2857, 0.4286, 0.5714, 0.7143, 0.8571, 1.0])
 
     # disaggregation for each level
-    for l in range(1, si+1):
+    for l in range(1, si + 1):
         if l == 1:
             vdn_in = precip_daily
             vdn_out = vdn1
         elif l == 2:
             vdn_in = vdn_out
             vdn_out = vdn2
         elif l == 3:
@@ -181,15 +155,15 @@
             vdn_out = vdn3
         elif l == 4:
             vdn_in = vdn_out
             vdn_out = vdn4
         elif l == 5:
             vdn_in = vdn_out
             vdn_out = vdn5
-       
+
         elif l == 6:
             vdn_in = vdn_out
             vdn_out = vdn6
         elif l == 7:
             vdn_in = vdn_out
             vdn_out = vdn7
         elif l == 8:
@@ -200,22 +174,22 @@
             vdn_out = vdn9
         elif l == 10:
             vdn_in = vdn_out
             vdn_out = vdn10
         elif l == 11:
             vdn_in = vdn_out
             vdn_out = vdn11
-                
+
         si -= 1
         if overwrite_stats:
             cascade_options = list_casc[si]
             for k in range(0, 7):
                 wxxcum[k, :, :] = cascade_options.wxx[k, :, :]
                 if k > 0:
-                    wxxcum[k, :, :] = wxxcum[k-1, :, :] + wxxcum[k, :, :]
+                    wxxcum[k, :, :] = wxxcum[k - 1, :, :] + wxxcum[k, :, :]
             meanvol = cascade_options.threshold[0]
         else:
             meanvol = cascade_options.threshold[si]
 
         # evaluate mean rainfall intensity for wet boxes
         # these values should be determined during the aggregation phase!!!!!
         # mean volume threshold
@@ -226,47 +200,47 @@
 
         j = 0
         for i in range(0, len(vdn_in)):
             # it's raining now?
             if vdn_in[i] > 0:
                 # determine type of box
                 if i == 0:  # only starting or isolated
-                    if vdn_in[i+1] > 0:
+                    if vdn_in[i + 1] > 0:
                         vbtype = cascade.BoxTypes.starting
                     else:
                         vbtype = cascade.BoxTypes.isolated
-                elif i == len(vdn_in)-1:  # only ending or isolated
-                    if vdn_in[i-1] > 0:
+                elif i == len(vdn_in) - 1:  # only ending or isolated
+                    if vdn_in[i - 1] > 0:
                         vbtype = cascade.BoxTypes.ending
                     else:
                         vbtype = cascade.BoxTypes.isolated
                 else:  # neither at at the end nor at the beginning
-                    if vdn_in[i-1] == 0 and vdn_in[i+1] == 0:
+                    if vdn_in[i - 1] == 0 and vdn_in[i + 1] == 0:
                         vbtype = cascade.BoxTypes.isolated
 
-                    if vdn_in[i-1] == 0 and vdn_in[i+1] > 0:
+                    if vdn_in[i - 1] == 0 and vdn_in[i + 1] > 0:
                         vbtype = cascade.BoxTypes.starting
 
-                    if vdn_in[i-1] > 0 and vdn_in[i+1] > 0:
+                    if vdn_in[i - 1] > 0 and vdn_in[i + 1] > 0:
                         vbtype = cascade.BoxTypes.enclosed
 
-                    if vdn_in[i-1] > 0 and vdn_in[i+1] == 0:
+                    if vdn_in[i - 1] > 0 and vdn_in[i + 1] == 0:
                         vbtype = cascade.BoxTypes.ending
 
                 # above or below mean?
                 if vdn_in[i] > meanvol:
                     belowabove = 1  # above mean
                 else:
                     belowabove = 0  # below mean
 
                 #
                 p = np.zeros((3, 1))
-                p[0] = cascade_options.p01[belowabove, vbtype-1]  # index changed!
-                p[1] = cascade_options.p10[belowabove, vbtype-1]
-                p[2] = cascade_options.pxx[belowabove, vbtype-1]
+                p[0] = cascade_options.p01[belowabove, vbtype - 1]  # index changed!
+                p[1] = cascade_options.p10[belowabove, vbtype - 1]
+                p[2] = cascade_options.pxx[belowabove, vbtype - 1]
 
                 # draw a random number to determine the braching type
                 rndp = np.random.random()
 
                 if rndp <= p[0]:
                     # first box 0, second box: 1 P(0/1)
                     vdn_out[j] = 0.0
@@ -282,87 +256,127 @@
                 else:
                     # both boxes wet
                     # we need a new random number
                     rndw = np.random.random()
 
                     # guess w1:
                     for k in range(0, 7):
-                        if rndw <= wxxcum[k, belowabove, vbtype-1]:
-                            w1 = wclassbounds[k+1] - 1./14.  # class center
+                        if rndw <= wxxcum[k, belowabove, vbtype - 1]:
+                            w1 = wclassbounds[k + 1] - 1.0 / 14.0  # class center
                             break
 
                     vdn_out[j] = w1 * vdn_in[i]
                     j = j + 1
-                    vdn_out[j] = (1. - w1) * vdn_in[i]
+                    vdn_out[j] = (1.0 - w1) * vdn_in[i]
                     j = j + 1
 
                     # check results (in the previous version this error has never been observed)
                     if w1 < 0 or w1 > 1:
                         print('error')
                         return
             else:
                 # add two dry boxes
                 vdn_out[j] = 0.0
                 j = j + 1
                 vdn_out[j] = 0.0
                 j = j + 1
-    
+
     if hourly:
         # uniformly disaggregate 0.75 h values to 0.25 h values
-        vdn_025 = np.zeros(len(vdn_out)*3)
+        vdn_025 = np.zeros(len(vdn_out) * 3)
         j = 0
         for i in range(0, len(vdn_out)):
             for m in range(0, 3):
-                vdn_025[j+m] = vdn_out[i] / 3.
+                vdn_025[j + m] = vdn_out[i] / 3.0
             j = j + 3
-    
+
         # aggregate to hourly time steps
         vdn_025cs = np.cumsum(vdn_025)
-        vdn = np.zeros(int(len(vdn_025)/4))
-        for i in range(0, len(vdn)+1):
+        vdn = np.zeros(int(len(vdn_025) / 4))
+        for i in range(0, len(vdn) + 1):
             # for first hour take 4th item
             if i == 0:
                 vdn[i] = vdn_025cs[3]
             elif i == 1:
                 pass
             else:
                 # >1 (starting with 2-1 = 1 item)
-                vdn[i-1] = vdn_025cs[(i*4)-1] - vdn_025cs[(i*4)-5]
-    
+                vdn[i - 1] = vdn_025cs[(i * 4) - 1] - vdn_025cs[(i * 4) - 5]
+
         disagg_precip = pd.Series(index=melodist.util.hourly_index(precip_daily.index), data=vdn)
-    
+
     else:
-        precip_sn = pd.Series(index= sub_level_index(precip_daily.index, level=level, fill_gaps=False), data=vdn_out)
+        precip_sn = pd.Series(
+            index=sub_level_index(precip_daily.index, level=level, fill_gaps=False), data=vdn_out
+        )
         disagg_precip = precip_sn.resample('5min').sum()
-    
+
     # set missing days to nan again:
     for date in missing_days:
-         disagg_precip[ disagg_precip.index.date == date.date()] = np.nan
+        disagg_precip[disagg_precip.index.date == date.date()] = np.nan
 
     # shifts the data by shift steps (fills with nan/cuts edge data )
     if shift != 0:
-         disagg_precip =  disagg_precip.shift(shift) #? freq='1U')
+        disagg_precip = disagg_precip.shift(shift)  # ? freq='1U')
 
     # return time series
     if test:
         if hourly:
             return vdn1, vdn2, vdn3, vdn4, vdn5, vdn_025, disagg_precip
         else:
             if level == 9:
-                return vdn1, vdn2, vdn3, vdn4, vdn5, vdn6, vdn7, vdn8, vdn9, precip_sn, disagg_precip
+                return (
+                    vdn1,
+                    vdn2,
+                    vdn3,
+                    vdn4,
+                    vdn5,
+                    vdn6,
+                    vdn7,
+                    vdn8,
+                    vdn9,
+                    precip_sn,
+                    disagg_precip,
+                )
             elif level == 10:
-                return vdn1, vdn2, vdn3, vdn4, vdn5, vdn6, vdn7, vdn8, vdn9, vdn10, precip_sn, disagg_precip
+                return (
+                    vdn1,
+                    vdn2,
+                    vdn3,
+                    vdn4,
+                    vdn5,
+                    vdn6,
+                    vdn7,
+                    vdn8,
+                    vdn9,
+                    vdn10,
+                    precip_sn,
+                    disagg_precip,
+                )
             else:
-                return vdn1, vdn2, vdn3, vdn4, vdn5, vdn6, vdn7, vdn8, vdn9, vdn10, vdn11, precip_sn, disagg_precip
+                return (
+                    vdn1,
+                    vdn2,
+                    vdn3,
+                    vdn4,
+                    vdn5,
+                    vdn6,
+                    vdn7,
+                    vdn8,
+                    vdn9,
+                    vdn10,
+                    vdn11,
+                    precip_sn,
+                    disagg_precip,
+                )
     else:
-        return  disagg_precip
+        return disagg_precip
+
 
-def precip_master_station(precip_daily,
-                          master_precip_hourly,
-                          zerodiv):
+def precip_master_station(precip_daily, master_precip_hourly, zerodiv):
     """Disaggregate precipitation based on the patterns of a master station
 
     Parameters
     -----------
     precip_daily : pd.Series
         daily data
     master_precip_hourly :  pd.Series
@@ -372,226 +386,229 @@
         distribution
     """
 
     precip_hourly = pd.Series(index=melodist.util.hourly_index(precip_daily.index))
 
     # set some parameters for cosine function
     for index_d, precip in precip_daily.iteritems():
-
         # get hourly data of the day
         index = index_d.date().isoformat()
         precip_h = master_precip_hourly[index]
 
         # calc rel values and multiply by daily sums
         # check for zero division
         if precip_h.sum() != 0 and precip_h.sum() != np.isnan(precip_h.sum()):
             precip_h_rel = (precip_h / precip_h.sum()) * precip
 
         else:
             # uniform option will preserve daily data by uniform distr
             if zerodiv == 'uniform':
-                precip_h_rel = (1/24) * precip
+                precip_h_rel = (1 / 24) * precip
 
             else:
                 precip_h_rel = 0
 
         # write the disaggregated day to data
         precip_hourly[index] = precip_h_rel
 
     return precip_hourly
 
 
-def aggregate_precipitation(vec_data,hourly=True, percentile=50):
+def aggregate_precipitation(vec_data, hourly=True, percentile=50):
     """Aggregates highly resolved precipitation data and creates statistics
 
     Parameters
     ----------
     vec_data : pd.Series
-        hourly (hourly=True) OR 5-min values 
+        hourly (hourly=True) OR 5-min values
 
     Returns
     -------
     output : cascade object
         representing statistics of the cascade model
     """
     cascade_opt = cascade.CascadeStatistics()
     cascade_opt.percentile = percentile
 
     # length of input time series
     n_in = len(vec_data)
-    n_out = np.floor(n_in/2)
+    n_out = np.floor(n_in / 2)
 
     # alternative:
     # 1st step: new time series
     vec_time = vec_data.index
     vdn0 = []
     vtn0 = []
     j = 0
     for i in range(0, n_in):
         if np.mod(i, 2) != 0:
-            vdn0.append(vec_data.precip.values[i-1] + vec_data.precip.values[i])
+            vdn0.append(vec_data.precip.values[i - 1] + vec_data.precip.values[i])
             vtn0.append(vec_time[i])
-            j = j+1
+            j = j + 1
 
     vdn = pd.DataFrame(index=vtn0, data={'precip': vdn0})
 
     # length of new time series
     n_out = len(vdn)
 
     # series of box types:
-    vbtype = np.zeros((n_out, ), dtype=np.int)
+    vbtype = np.zeros((n_out,), dtype=int)
 
     # fields for empirical probabilities
     # counts
     nb = np.zeros((2, 4))
     nbxx = np.zeros((2, 4))
 
     # class boundaries for histograms
     # wclassbounds = np.linspace(0, 1, num=8)
-    wlower = np.array([0,
-                       0.1429,
-                       0.2857,
-                       0.4286,
-                       0.5714,
-                       0.7143,
-                       0.8571])  # wclassbounds[0:7]
-    wupper = np.array([0.1429,
-                       0.2857,
-                       0.4286,
-                       0.5714,
-                       0.7143,
-                       0.8571,
-                       1.0])  # wclassbounds[1:8]
+    wlower = np.array([0, 0.1429, 0.2857, 0.4286, 0.5714, 0.7143, 0.8571])  # wclassbounds[0:7]
+    wupper = np.array([0.1429, 0.2857, 0.4286, 0.5714, 0.7143, 0.8571, 1.0])  # wclassbounds[1:8]
 
     # evaluate mean rainfall intensity for wet boxes
     # these values should be determined during the aggregation phase!!!!!
     # mean volume threshold
-    meanvol = np.percentile(vdn.precip[vdn.precip > 0.],
-                            cascade_opt.percentile)  # np.mean(vdn.precip[vdn.precip>0.])
+    meanvol = np.percentile(
+        vdn.precip[vdn.precip > 0.0], cascade_opt.percentile
+    )  # np.mean(vdn.precip[vdn.precip>0.])
     cascade_opt.threshold = np.array([meanvol])
 
     # 2nd step: classify boxes at the upper level
     for i in range(0, n_out):
-        if vdn.precip.values[i] > 0.:  # rain?
+        if vdn.precip.values[i] > 0.0:  # rain?
             if i == 0:  # only starting or isolated
-                if vdn.precip.values[i+1] > 0.:
+                if vdn.precip.values[i + 1] > 0.0:
                     vbtype[i] = cascade.BoxTypes.starting
                 else:
                     vbtype[i] = cascade.BoxTypes.isolated
-            elif i == n_out-1:  # only ending or isolated
-                if vdn.precip.values[i-1] > 0.:
+            elif i == n_out - 1:  # only ending or isolated
+                if vdn.precip.values[i - 1] > 0.0:
                     vbtype[i] = cascade.BoxTypes.ending
                 else:
                     vbtype[i] = cascade.BoxTypes.isolated
             else:  # neither at at the end nor at the beginning
-                if vdn.precip.values[i-1] == 0. and vdn.precip.values[i+1] == 0.:
+                if vdn.precip.values[i - 1] == 0.0 and vdn.precip.values[i + 1] == 0.0:
                     vbtype[i] = cascade.BoxTypes.isolated
-                if vdn.precip.values[i-1] == 0. and vdn.precip.values[i+1] > 0.:
+                if vdn.precip.values[i - 1] == 0.0 and vdn.precip.values[i + 1] > 0.0:
                     vbtype[i] = cascade.BoxTypes.starting
-                if vdn.precip.values[i-1] > 0. and vdn.precip.values[i+1] > 0.:
+                if vdn.precip.values[i - 1] > 0.0 and vdn.precip.values[i + 1] > 0.0:
                     vbtype[i] = cascade.BoxTypes.enclosed
-                if vdn.precip.values[i-1] > 0. and vdn.precip.values[i+1] == 0.:
+                if vdn.precip.values[i - 1] > 0.0 and vdn.precip.values[i + 1] == 0.0:
                     vbtype[i] = cascade.BoxTypes.ending
         else:
             vbtype[i] = cascade.BoxTypes.dry  # no rain
 
     # 3rd step: examine branching
     j = 0
     for i in range(0, n_in):
         if np.mod(i, 2) != 0:
             if vdn.precip.values[j] > 0:
                 if vdn.precip.values[j] > meanvol:
                     belowabove = 1  # above mean
                 else:
                     belowabove = 0  # below mean
 
-                nb[belowabove, vbtype[j]-1] += 1
+                nb[belowabove, vbtype[j] - 1] += 1
 
-                if vec_data.precip.values[i-1] > 0 and vec_data.precip.values[i] == 0:
+                if vec_data.precip.values[i - 1] > 0 and vec_data.precip.values[i] == 0:
                     # P(1/0)
-                    cascade_opt.p10[belowabove, vbtype[j]-1] += 1
+                    cascade_opt.p10[belowabove, vbtype[j] - 1] += 1
 
-                if vec_data.precip.values[i-1] == 0 and vec_data.precip.values[i] > 0:
+                if vec_data.precip.values[i - 1] == 0 and vec_data.precip.values[i] > 0:
                     # P(0/1)
-                    cascade_opt.p01[belowabove, vbtype[j]-1] += 1
+                    cascade_opt.p01[belowabove, vbtype[j] - 1] += 1
 
-                if vec_data.precip.values[i-1] > 0 and vec_data.precip.values[i] > 0:
+                if vec_data.precip.values[i - 1] > 0 and vec_data.precip.values[i] > 0:
                     # P(x/x)
-                    cascade_opt.pxx[belowabove, vbtype[j]-1] += 1
+                    cascade_opt.pxx[belowabove, vbtype[j] - 1] += 1
 
-                    nbxx[belowabove, vbtype[j]-1] += 1
+                    nbxx[belowabove, vbtype[j] - 1] += 1
 
                     # weights
-                    r1 = vec_data.precip.values[i-1]
+                    r1 = vec_data.precip.values[i - 1]
                     r2 = vec_data.precip.values[i]
                     wxxval = r1 / (r1 + r2)
 
                     # Test
-                    if abs(r1+r2-vdn.precip.values[j]) > 1.E-3:
-                        print('i=' + str(i) + ', j=' + str(j) +
-                              ', r1=' + str(r1) + ", r2=" + str(r2) +
-                              ", Summe=" + str(vdn.precip.values[j]))
+                    if abs(r1 + r2 - vdn.precip.values[j]) > 1.0e-3:
+                        print(
+                            'i='
+                            + str(i)
+                            + ', j='
+                            + str(j)
+                            + ', r1='
+                            + str(r1)
+                            + ", r2="
+                            + str(r2)
+                            + ", Summe="
+                            + str(vdn.precip.values[j])
+                        )
                         print(vec_data.index[i])
                         print(vdn.index[j])
                         print('error')
                         return cascade_opt, vdn
 
                     for k in range(0, 7):
                         if wxxval > wlower[k] and wxxval <= wupper[k]:
-                            cascade_opt.wxx[k, belowabove, vbtype[j]-1] += 1
+                            cascade_opt.wxx[k, belowabove, vbtype[j] - 1] += 1
                             break
             j = j + 1
 
     # 4th step: transform counts to percentages
     cascade_opt.p01 = cascade_opt.p01 / nb
     cascade_opt.p10 = cascade_opt.p10 / nb
     cascade_opt.pxx = cascade_opt.pxx / nb
 
-    with np.errstate(divide='ignore', invalid='ignore'):  # do not issue warnings here when dividing by zero, this is handled below
+    with np.errstate(
+        divide='ignore', invalid='ignore'
+    ):  # do not issue warnings here when dividing by zero, this is handled below
         for k in range(0, 7):
             cascade_opt.wxx[k, :, :] = cascade_opt.wxx[k, :, :] / nbxx[:, :]
 
     # In some cases, the time series are too short for deriving statistics.
 
-    if (np.isnan(cascade_opt.p01).any() or
-            np.isnan(cascade_opt.p10).any() or
-            np.isnan(cascade_opt.pxx).any()):
+    if (
+        np.isnan(cascade_opt.p01).any()
+        or np.isnan(cascade_opt.p10).any()
+        or np.isnan(cascade_opt.pxx).any()
+    ):
         print("ERROR (branching probabilities):")
-        print("Invalid statistics. Default values will be returned. "
-              "Try to use longer time series or apply statistics "
-              "derived for another station.")
+        print(
+            "Invalid statistics. Default values will be returned. "
+            "Try to use longer time series or apply statistics "
+            "derived for another station."
+        )
         cascade_opt.fill_with_sample_data()
 
     # For some box types, the corresponding probabilities might yield nan.
     # If this happens, nan values will be replaced by 1/7 in order to provide
     # valid values for disaggregation.
     if np.isnan(cascade_opt.wxx).any():
         print("Warning (weighting probabilities):")
-        print("The derived cascade statistics are not valid as some "
-              "probabilities are undefined! ", end="")
-        print("Try to use longer time series that might be more "
-              "appropriate for deriving statistics. ", end="")
-        print("As a workaround, default values according to equally "
-              "distributed probabilities ", end="")
-        print("will be applied...", end="")
+        print(
+            "The derived cascade statistics are not valid as some probabilities are undefined! ",
+            "Try to use longer time series that might be more "
+            "appropriate for deriving statistics. "
+            "As a workaround, default values according to equally distributed probabilities "
+            "will be applied... ",
+            end='',
+        )
         cascade_opt.wxx[np.isnan(cascade_opt.wxx)] = 1.0 / 7.0
         wxx = np.zeros((2, 4))
         for k in range(0, 7):
             wxx[:, :] += cascade_opt.wxx[k, :, :]
         if wxx.any() > 1.001 or wxx.any() < 0.999:
             print("failed! Using default values!")
             cascade_opt.fill_with_sample_data()
         else:
             print("OK!")
 
     return cascade_opt, vdn
 
 
-def seasonal_subset(dataframe,
-                    months='all'):
+def seasonal_subset(dataframe, months='all'):
     '''Get the seasonal data.
 
     Parameters
     ----------
     dataframe : pd.DataFrame
     months: int, str
         Months to use for statistics, or 'all' for 1-12 (default='all')
@@ -602,31 +619,28 @@
 
     for month_num, month in enumerate(months):
         df_cur = dataframe[dataframe.index.month == month]
 
         if month_num == 0:
             df = df_cur
         else:
-            df = df.append(df_cur)
+            df = pd.concat([df, df_cur])
 
     return df.sort_index()
 
 
-def build_casc(ObsData, hourly=True,level=9,
-               months=None,
-               avg_stats=True,
-               percentile=50):
+def build_casc(ObsData, hourly=True, level=9, months=None, avg_stats=True, percentile=50):
     '''Builds the cascade statistics of observed data for disaggregation
 
     Parameters
     -----------
     ObsData : pd.Series
         hourly=True -> hourly obs data
         else -> 5min data (disaggregation level=9 (default), 10, 11)
-    
+
     months : numpy array of ints
         Months for each seasons to be used for statistics (array of
         numpy array, default=1-12, e.g., [np.arange(12) + 1])
     avg_stats : bool
         average statistics for all levels True/False (default=True)
     percentile : int, float
         percentile for splitting the dataset in small and high
@@ -648,79 +662,107 @@
         vdn = seasonal_subset(ObsData, cur_months)
         if len(ObsData.precip[np.isnan(ObsData.precip)]) > 0:
             ObsData.precip[np.isnan(ObsData.precip)] = 0
 
         casc_opt = melodist.cascade.CascadeStatistics()
         casc_opt.percentile = percentile
         list_casc_opt = list()
-        
+
         count = 0
-        
+
         if hourly:
             aggre_level = 5
         else:
-            aggre_level =  level
-        
-        thresholds = np.zeros(aggre_level) #np.array([0., 0., 0., 0., 0.])
-        
+            aggre_level = level
+
+        thresholds = np.zeros(aggre_level)  # np.array([0., 0., 0., 0., 0.])
+
         for i in range(0, aggre_level):
             # aggregate the data
-            casc_opt_i, vdn = aggregate_precipitation(vdn, hourly, \
-                                percentile=percentile)
-            thresholds[i] = casc_opt_i.threshold
+            casc_opt_i, vdn = aggregate_precipitation(vdn, hourly, percentile=percentile)
+            thresholds[i] = casc_opt_i.threshold[0]
             copy_of_casc_opt_i = copy.copy(casc_opt_i)
             list_casc_opt.append(copy_of_casc_opt_i)
             n_vdn = len(vdn)
             casc_opt_i * n_vdn  # level related weighting
             casc_opt + casc_opt_i  # add to total statistics
             count = count + n_vdn
-        casc_opt * (1. / count)  # transfer weighted matrices to probabilities
+        casc_opt * (1.0 / count)  # transfer weighted matrices to probabilities
         casc_opt.threshold = thresholds
-        
+
         # statistics object
         if avg_stats:
             # in this case, the average statistics will be applied for all levels likewise
             stat_obj = casc_opt
         else:
             # for longer time series, separate statistics might be more appropriate
             # level dependent statistics will be assumed
             stat_obj = list_casc_opt
 
         list_seasonal_casc.append(stat_obj)
 
     return list_seasonal_casc
 
+
 def sub_level_index(daily_index, level=9, fill_gaps=False):
-    frequency = 42187500 * (2**(11-level))
-    sublevel_index = pd.date_range(start=daily_index.min(), end=daily_index.max().replace(hour=23,minute=59,second=59), freq= '%sU'% frequency)
+    frequency = 42187500 * (2 ** (11 - level))
+    sublevel_index = pd.date_range(
+        start=daily_index.min(),
+        end=daily_index.max().replace(hour=23, minute=59, second=59),
+        freq='%sU' % frequency,
+    )
     # remove days that are not in the daily index:
     time_steps = 2**level
     if not fill_gaps and len(sublevel_index) > len(daily_index) * time_steps:
-        df = pd.DataFrame(index=sublevel_index.date, data=dict(hour=sublevel_index.hour,\
-                                                               minute=sublevel_index.minute,second=sublevel_index.second, keep=True))
-        df.index = pd.to_datetime(df.index) #got a warning at firsr: "to_datetime"is depreciated
+        df = pd.DataFrame(
+            index=sublevel_index.date,
+            data=dict(
+                hour=sublevel_index.hour,
+                minute=sublevel_index.minute,
+                second=sublevel_index.second,
+                keep=True,
+            ),
+        )
+        df.index = pd.to_datetime(df.index)  # got a warning at firsr: "to_datetime"is depreciated
         dropdates = list(set(sublevel_index.date) - set(daily_index.date))
         df.loc[dropdates, 'keep'] = False
         df = df[df.keep]
-        sublevel_index = pd.DatetimeIndex([pd.datetime(y, m, d, h,minute,second) for y, m, d, h,minute,second in zip(df.index.year,
-                                                                                df.index.month,
-                                                                                df.index.day,
-                                                                                df.hour,df.minute,df.second)])
+        sublevel_index = pd.DatetimeIndex(
+            [
+                pd.datetime(y, m, d, h, minute, second)
+                for y, m, d, h, minute, second in zip(
+                    df.index.year, df.index.month, df.index.day, df.hour, df.minute, df.second
+                )
+            ]
+        )
 
     return sublevel_index
 
+
 def fmin_index(daily_index, fill_gaps=False):
-    fminindex = pd.date_range(start=daily_index.min(), end=daily_index.max().replace(hour=23,minute=59,second=59), freq='300000L')
+    fminindex = pd.date_range(
+        start=daily_index.min(),
+        end=daily_index.max().replace(hour=23, minute=59, second=59),
+        freq='300000L',
+    )
     # remove days that are not in the daily index:
     if not fill_gaps and len(fminindex) > len(daily_index) * 288:
-        df = pd.DataFrame(index=fminindex.date, data=dict(hour=fminindex.hour,minute=fminindex.minute,second=fminindex.second, keep=True))
-        df.index = pd.to_datetime(df.index) #got a warning at firsr: "to_datetime"is depreciated
+        df = pd.DataFrame(
+            index=fminindex.date,
+            data=dict(
+                hour=fminindex.hour, minute=fminindex.minute, second=fminindex.second, keep=True
+            ),
+        )
+        df.index = pd.to_datetime(df.index)  # got a warning at firsr: "to_datetime"is depreciated
         dropdates = list(set(fminindex.date) - set(daily_index.date))
         df.loc[dropdates, 'keep'] = False
         df = df[df.keep]
-        fminindex = pd.DatetimeIndex([pd.datetime(y, m, d, h,minute,second) for y, m, d, h,minute,second in zip(df.index.year,
-                                                                                df.index.month,
-                                                                                df.index.day,
-                                                                                df.hour,df.minute,df.second)])
+        fminindex = pd.DatetimeIndex(
+            [
+                pd.datetime(y, m, d, h, minute, second)
+                for y, m, d, h, minute, second in zip(
+                    df.index.year, df.index.month, df.index.day, df.hour, df.minute, df.second
+                )
+            ]
+        )
 
     return fminindex
-
```

### Comparing `melodist-0.1.4/melodist/radiation.py` & `melodist-0.1.5/melodist/radiation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,104 +1,120 @@
-# -*- coding: utf-8 -*-
-###############################################################################################################
-# This file is part of MELODIST - MEteoroLOgical observation time series DISaggregation Tool                  #
-# a program to disaggregate daily values of meteorological variables to hourly values                         #
-#                                                                                                             #
-# Copyright (C) 2016  Florian Hanzer (1,2), Kristian Förster (1,2), Benjamin Winter (1,2), Thomas Marke (1)   #
-#                                                                                                             #
-# (1) Institute of Geography, University of Innsbruck, Austria                                                #
-# (2) alpS - Centre for Climate Change Adaptation, Innsbruck, Austria                                         #
-#                                                                                                             #
-# MELODIST is free software: you can redistribute it and/or modify                                            #
-# it under the terms of the GNU General Public License as published by                                        #
-# the Free Software Foundation, either version 3 of the License, or                                           #
-# (at your option) any later version.                                                                         #
-#                                                                                                             #
-# MELODIST is distributed in the hope that it will be useful,                                                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                                              #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the                                                #
-# GNU General Public License for more details.                                                                #
-#                                                                                                             #
-# You should have received a copy of the GNU General Public License                                           #
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.                                       #
-#                                                                                                             #
-###############################################################################################################
-
-from __future__ import print_function, division, absolute_import
-import melodist.util
-import pandas as pd
+################################################################################
+# This file is part of MELODIST - MEteoroLOgical observation time series       #
+# DISaggregation Tool.                                                         #
+#                                                                              #
+# Copyright (C) 2016-2023 Florian Hanzer, Kristian Förster, Benjamin Winter,   #
+# Thomas Marke                                                                 #
+#                                                                              #
+# MELODIST is free software: you can redistribute it and/or modify it under    #
+# the terms of the GNU General Public License as published by the Free         #
+# Software Foundation, either version 3 of the License, or (at your option)    #
+# any later version.                                                           #
+#                                                                              #
+# MELODIST is distributed in the hope that it will be useful, but WITHOUT ANY  #
+# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS    #
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more        #
+# details.                                                                     #
+#                                                                              #
+# You should have received a copy of the GNU General Public License along with #
+# this program.  If not, see <http://www.gnu.org/licenses/>.                   #
+################################################################################
 import numpy as np
+import pandas as pd
 import scipy.optimize
 
+import melodist.util
+
 """
 This routine diaggregates daily values of global radiation data to hourly values
 """
 
 
-def disaggregate_radiation(data_daily,
-                           sun_times=None,
-                           pot_rad=None,
-                           method='pot_rad',
-                           angstr_a=0.25,
-                           angstr_b=0.5,
-                           bristcamp_a=0.75,
-                           bristcamp_c=2.4,
-                           mean_course=None):
+def disaggregate_radiation(
+    data_daily,
+    sun_times=None,
+    pot_rad=None,
+    method='pot_rad',
+    angstr_a=0.25,
+    angstr_b=0.5,
+    bristcamp_a=0.75,
+    bristcamp_c=2.4,
+    mean_course=None,
+):
     """general function for radiation disaggregation
 
     Args:
         daily_data: daily values
         sun_times: daily dataframe including results of the util.sun_times function
         pot_rad: hourly dataframe including potential radiation
         method: keyword specifying the disaggregation method to be used
         angstr_a: parameter a of the Angstrom model (intercept)
         angstr_b: parameter b of the Angstrom model (slope)
         mean_course: monthly values of the mean hourly radiation course
-        
+
     Returns:
         Disaggregated hourly values of shortwave radiation.
     """
     # check if disaggregation method has a valid value
     if method not in ('pot_rad', 'pot_rad_via_ssd', 'pot_rad_via_bc', 'mean_course'):
         raise ValueError('Invalid option')
 
     glob_disagg = pd.Series(index=melodist.util.hourly_index(data_daily.index), dtype=float)
 
     if method == 'mean_course':
         assert mean_course is not None
 
         pot_rad = pd.Series(index=glob_disagg.index, dtype=float)
-        pot_rad[:] = mean_course.unstack().loc[list(zip(pot_rad.index.month, pot_rad.index.hour))].values
+        pot_rad[:] = (
+            mean_course.unstack().loc[list(zip(pot_rad.index.month, pot_rad.index.hour))].values
+        )
     else:
         assert pot_rad is not None
 
     pot_rad_daily = pot_rad.resample('D').mean()
 
     if method in ('pot_rad', 'mean_course'):
         globalrad = data_daily.glob
     elif method == 'pot_rad_via_ssd':
         # in this case use the Angstrom model
-        globalrad = pd.Series(index=data_daily.index, data=0.)
+        globalrad = pd.Series(index=data_daily.index, data=0.0)
         dates = sun_times.index[sun_times.daylength > 0]  # account for polar nights
-        globalrad[dates] = angstroem(data_daily.ssd[dates], sun_times.daylength[dates],
-                                     pot_rad_daily[dates], angstr_a, angstr_b)
+        globalrad[dates] = angstroem(
+            data_daily.ssd[dates],
+            sun_times.daylength[dates],
+            pot_rad_daily[dates],
+            angstr_a,
+            angstr_b,
+        )
     elif method == 'pot_rad_via_bc':
         # using data from Bristow-Campbell model
-        globalrad = bristow_campbell(data_daily.tmin, data_daily.tmax, pot_rad_daily, bristcamp_a, bristcamp_c)
-
-    globalrad_equal = globalrad.reindex(pot_rad.index, method='ffill')  # hourly values (replicate daily mean value for each hour)
+        globalrad = bristow_campbell(
+            data_daily.tmin, data_daily.tmax, pot_rad_daily, bristcamp_a, bristcamp_c
+        )
+
+    globalrad_equal = globalrad.reindex(
+        pot_rad.index, method='ffill'
+    )  # hourly values (replicate daily mean value for each hour)
     pot_rad_daily_equal = pot_rad_daily.reindex(pot_rad.index, method='ffill')
     glob_disagg = pot_rad / pot_rad_daily_equal * globalrad_equal
-    glob_disagg[glob_disagg < 1e-2] = 0.
+    glob_disagg[glob_disagg < 1e-2] = 0.0
 
     return glob_disagg
 
 
-def potential_radiation(dates, lon, lat, timezone, terrain_slope=0, terrain_slope_azimuth=0,
-                        cloud_fraction=0, split=False):
+def potential_radiation(
+    dates,
+    lon,
+    lat,
+    timezone,
+    terrain_slope=0,
+    terrain_slope_azimuth=0,
+    cloud_fraction=0,
+    split=False,
+):
     """
     Calculate potential shortwave radiation for a specific location and time.
 
     This routine calculates global radiation as described in:
     Liston, G. E. and Elder, K. (2006): A Meteorological Distribution System for
     High-Resolution Terrestrial Modeling (MicroMet), J. Hydrometeorol., 7, 217–234.
 
@@ -122,55 +138,66 @@
         Terrain slope azimuth as defined in Liston & Elder (2006) (eq. 13)
     cloud_fraction : float, default 0
         Cloud fraction between 0 and 1
     split : boolean, default False
         If True, return a DataFrame containing direct and diffuse radiation,
         otherwise return a Series containing total radiation
     """
-    solar_constant = 1367.
+    solar_constant = 1367.0
     days_per_year = 365.25
     tropic_of_cancer = np.deg2rad(23.43697)
     solstice = 173.0
 
     dates = pd.DatetimeIndex(dates)
     dates_hour = np.array(dates.hour)
     dates_minute = np.array(dates.minute)
     day_of_year = np.array(dates.dayofyear)
 
     # compute solar decline in rad
-    solar_decline = tropic_of_cancer * np.cos(2.0 * np.pi * (day_of_year - solstice) / days_per_year)
+    solar_decline = tropic_of_cancer * np.cos(
+        2.0 * np.pi * (day_of_year - solstice) / days_per_year
+    )
 
     # compute the sun hour angle in rad
-    standard_meridian = timezone * 15.
-    delta_lat_time = (lon - standard_meridian) * 24. / 360.
-    hour_angle = np.pi * (((dates_hour + dates_minute / 60. + delta_lat_time) / 12.) - 1.)
+    standard_meridian = timezone * 15.0
+    delta_lat_time = (lon - standard_meridian) * 24.0 / 360.0
+    hour_angle = np.pi * (((dates_hour + dates_minute / 60.0 + delta_lat_time) / 12.0) - 1.0)
 
     # get solar zenith angle
-    cos_solar_zenith = (np.sin(solar_decline) * np.sin(np.deg2rad(lat))
-                        + np.cos(solar_decline) * np.cos(np.deg2rad(lat)) * np.cos(hour_angle))
+    cos_solar_zenith = np.sin(solar_decline) * np.sin(np.deg2rad(lat)) + np.cos(
+        solar_decline
+    ) * np.cos(np.deg2rad(lat)) * np.cos(hour_angle)
     cos_solar_zenith = cos_solar_zenith.clip(min=0)
     solar_zenith_angle = np.arccos(cos_solar_zenith)
 
     # compute transmissivities for direct and diffus radiation using cloud fraction
     transmissivity_direct = (0.6 + 0.2 * cos_solar_zenith) * (1.0 - cloud_fraction)
     transmissivity_diffuse = (0.3 + 0.1 * cos_solar_zenith) * cloud_fraction
 
     # modify solar constant for eccentricity
-    beta = 2. * np.pi * (day_of_year / days_per_year)
-    radius_ratio = (1.00011 + 0.034221 * np.cos(beta) + 0.00128 * np.sin(beta)
-                    + 0.000719 * np.cos(2. * beta) + 0.000077 * np.sin(2 * beta))
+    beta = 2.0 * np.pi * (day_of_year / days_per_year)
+    radius_ratio = (
+        1.00011
+        + 0.034221 * np.cos(beta)
+        + 0.00128 * np.sin(beta)
+        + 0.000719 * np.cos(2.0 * beta)
+        + 0.000077 * np.sin(2 * beta)
+    )
     solar_constant_times_radius_ratio = solar_constant * radius_ratio
 
     mu = np.arcsin(np.cos(solar_decline) * np.sin(hour_angle) / np.sin(solar_zenith_angle))
-    cosi = (np.cos(terrain_slope) * cos_solar_zenith
-            + np.sin(terrain_slope) * np.sin(solar_zenith_angle) * np.cos(mu - terrain_slope_azimuth))
+    cosi = np.cos(terrain_slope) * cos_solar_zenith + np.sin(terrain_slope) * np.sin(
+        solar_zenith_angle
+    ) * np.cos(mu - terrain_slope_azimuth)
 
     # get total shortwave radiation
     direct_radiation = solar_constant_times_radius_ratio * transmissivity_direct * cosi
-    diffuse_radiation = solar_constant_times_radius_ratio * transmissivity_diffuse * cos_solar_zenith
+    diffuse_radiation = (
+        solar_constant_times_radius_ratio * transmissivity_diffuse * cos_solar_zenith
+    )
     direct_radiation = direct_radiation.clip(min=0)
 
     df = pd.DataFrame(index=dates, data=dict(direct=direct_radiation, diffuse=diffuse_radiation))
 
     if split:
         return df
     else:
@@ -237,18 +264,21 @@
 
     pot_rad_daily : Series
         Mean potential daily solar radiation.
 
     obs_rad_daily : Series
         Mean observed daily solar radiation.
     """
+
     def bc_absbias(ac):
         return np.abs(np.mean(bristow_campbell(df.tmin, df.tmax, df.pot, ac[0], ac[1]) - df.obs))
 
-    df = pd.DataFrame(data=dict(tmin=tmin, tmax=tmax, pot=pot_rad_daily, obs=obs_rad_daily)).dropna(how='any')
+    df = pd.DataFrame(data=dict(tmin=tmin, tmax=tmax, pot=pot_rad_daily, obs=obs_rad_daily)).dropna(
+        how='any'
+    )
     res = scipy.optimize.minimize(bc_absbias, [0.75, 2.4])  # i.e. we minimize the absolute bias
 
     return res.x
 
 
 def angstroem(ssd, day_length, pot_rad_daily, a, b):
     """
@@ -297,15 +327,17 @@
 
     pot_rad_daily : Series
         Mean potential daily solar radiation.
 
     obs_rad_daily : Series
         Mean observed daily solar radiation.
     """
-    df = pd.DataFrame(data=dict(ssd=ssd, day_length=day_length, pot=pot_rad_daily, obs=obs_rad_daily)).dropna(how='any')
+    df = pd.DataFrame(
+        data=dict(ssd=ssd, day_length=day_length, pot=pot_rad_daily, obs=obs_rad_daily)
+    ).dropna(how='any')
 
     def angstroem_opt(x, a, b):
         return angstroem(x[0], x[1], x[2], a, b)
 
     x = np.array([df.ssd, df.day_length, df.pot])
     popt, pcov = scipy.optimize.curve_fit(angstroem_opt, x, df.obs, p0=[0.25, 0.75])
```

### Comparing `melodist-0.1.4/melodist/station.py` & `melodist-0.1.5/melodist/station.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,40 @@
-# -*- coding: utf-8 -*-
-###############################################################################################################
-# This file is part of MELODIST - MEteoroLOgical observation time series DISaggregation Tool                  #
-# a program to disaggregate daily values of meteorological variables to hourly values                         #
-#                                                                                                             #
-# Copyright (C) 2016  Florian Hanzer (1,2), Kristian Förster (1,2), Benjamin Winter (1,2), Thomas Marke (1)   #
-#                                                                                                             #
-# (1) Institute of Geography, University of Innsbruck, Austria                                                #
-# (2) alpS - Centre for Climate Change Adaptation, Innsbruck, Austria                                         #
-#                                                                                                             #
-# MELODIST is free software: you can redistribute it and/or modify                                            #
-# it under the terms of the GNU General Public License as published by                                        #
-# the Free Software Foundation, either version 3 of the License, or                                           #
-# (at your option) any later version.                                                                         #
-#                                                                                                             #
-# MELODIST is distributed in the hope that it will be useful,                                                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                                              #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the                                                #
-# GNU General Public License for more details.                                                                #
-#                                                                                                             #
-# You should have received a copy of the GNU General Public License                                           #
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.                                       #
-#                                                                                                             #
-###############################################################################################################
+################################################################################
+# This file is part of MELODIST - MEteoroLOgical observation time series       #
+# DISaggregation Tool.                                                         #
+#                                                                              #
+# Copyright (C) 2016-2023 Florian Hanzer, Kristian Förster, Benjamin Winter,   #
+# Thomas Marke                                                                 #
+#                                                                              #
+# MELODIST is free software: you can redistribute it and/or modify it under    #
+# the terms of the GNU General Public License as published by the Free         #
+# Software Foundation, either version 3 of the License, or (at your option)    #
+# any later version.                                                           #
+#                                                                              #
+# MELODIST is distributed in the hope that it will be useful, but WITHOUT ANY  #
+# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS    #
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more        #
+# details.                                                                     #
+#                                                                              #
+# You should have received a copy of the GNU General Public License along with #
+# this program.  If not, see <http://www.gnu.org/licenses/>.                   #
+################################################################################
+import pandas as pd
 
-from __future__ import print_function, division, absolute_import
 import melodist
 import melodist.util
-import pandas as pd
 
 
 class Station(object):
     """
-    Class representing meteorological stations including all relevant 
+    Class representing meteorological stations including all relevant
     information such as metadata and meteorological time series (observed
     and disaggregated)
     """
+
     _columns_daily = [
         'tmean',
         'tmin',
         'tmax',
         'precip',
         'glob',
         'ssd',
@@ -80,26 +76,28 @@
         or aggregation of hourly data for testing purposes.
         """
         return self._data_daily
 
     @data_daily.setter
     def data_daily(self, df):
         assert isinstance(df, pd.DataFrame)
-        assert df.index.is_all_dates
+        assert isinstance(df.index, pd.DatetimeIndex)
         # for col in df:
         #     assert col in Station._columns_daily
         assert df.index.resolution == 'day'
         assert df.index.is_monotonic_increasing
 
         if df.index.freq is None:  # likely some days are missing
             df = df.reindex(pd.date_range(start=df.index[0], end=df.index[-1], freq='D'))
 
         for var in 'tmin', 'tmax', 'tmean':
             if var in df:
-                assert not any(df[var] < 200), 'Implausible temperature values detected - temperatures must be in K'
+                assert not any(
+                    df[var] < 200
+                ), 'Implausible temperature values detected - temperatures must be in K'
 
         self._data_daily = df.copy()
 
         # create data frame for disaggregated data:
         index = melodist.util.hourly_index(df.index)
         df = pd.DataFrame(index=index, columns=Station._columns_hourly, dtype=float)
         self._data_disagg = df
@@ -131,15 +129,15 @@
         self._lat = lat
         self.statistics._lat = lat
 
     @property
     def timezone(self):
         """
         Timezone indicates the differnce in hours calculated from UTC
-        
+
         Negative values indicate timezones later than UTC, i.e. west of 0 deg
         long. Positive values indicate the reverse.
         """
         return self._timezone
 
     @timezone.setter
     def timezone(self, timezone):
@@ -172,15 +170,17 @@
         return self._data_disagg
 
     def calc_sun_times(self):
         """
         Computes the times of sunrise, solar noon, and sunset for each day.
         """
 
-        self.sun_times = melodist.util.get_sun_times(self.data_daily.index, self.lon, self.lat, self.timezone)
+        self.sun_times = melodist.util.get_sun_times(
+            self.data_daily.index, self.lon, self.lat, self.timezone
+        )
 
     def disaggregate_wind(self, method='equal'):
         """
         Disaggregate wind speed.
 
         Parameters
         ----------
@@ -194,59 +194,65 @@
                 Distributes daily mean wind speed using a cosine function derived from hourly
                 observations.
 
             ``random``
                 Draws random numbers to distribute wind speed (usually not conserving the
                 daily average).
         """
-        self.data_disagg.wind = melodist.disaggregate_wind(self.data_daily.wind, method=method, **self.statistics.wind)
+        self.data_disagg.wind = melodist.disaggregate_wind(
+            self.data_daily.wind, method=method, **self.statistics.wind
+        )
 
     def disaggregate_humidity(self, method='equal', preserve_daily_mean=False):
         """
         Disaggregate relative humidity.
 
         Parameters
         ----------
         method : str, optional
             Disaggregation method.
 
             ``equal``
                 Mean daily humidity is duplicated for the 24 hours of the day. (Default)
 
             ``minimal``:
-                Calculates humidity from daily dew point temperature by setting the dew point temperature
-                equal to the daily minimum temperature.
+                Calculates humidity from daily dew point temperature by setting the dew point
+                temperature equal to the daily minimum temperature.
 
             ``dewpoint_regression``:
-                Calculates humidity from daily dew point temperature by calculating dew point temperature
-                using ``Tdew = a * Tmin + b``, where ``a`` and ``b`` are determined by calibration.
+                Calculates humidity from daily dew point temperature by calculating dew point
+                temperature using ``Tdew = a * Tmin + b``, where ``a`` and ``b`` are determined by
+                calibration.
 
             ``linear_dewpoint_variation``:
                 Calculates humidity from hourly dew point temperature by assuming a linear dew point
                 temperature variation between consecutive days.
 
             ``min_max``:
                 Calculates hourly humidity from observations of daily minimum and maximum humidity.
 
             ``month_hour_precip_mean``:
                 Calculates hourly humidity from categorical [month, hour, precip(y/n)] mean values
                 derived from observations.
 
         preserve_daily_mean : bool, optional
-            If True, correct the daily mean values of the disaggregated data with the observed daily means.
+            If True, correct the daily mean values of the disaggregated data with the observed daily
+            means.
         """
         self.data_disagg.hum = melodist.disaggregate_humidity(
             self.data_daily,
             temp=self.data_disagg.temp,
             method=method,
             preserve_daily_mean=preserve_daily_mean,
-            **self.statistics.hum
+            **self.statistics.hum,
         )
 
-    def disaggregate_temperature(self, method='sine_min_max', min_max_time='fix', mod_nighttime=False):
+    def disaggregate_temperature(
+        self, method='sine_min_max', min_max_time='fix', mod_nighttime=False
+    ):
         """
         Disaggregate air temperature.
 
         Parameters
         ----------
         method : str, optional
             Disaggregation method.
@@ -276,30 +282,33 @@
             ``fix``:
                 Minimum/maximum temperature are assumed to occur at 07:00/14:00 local time.
 
             ``sun_loc``:
                 Minimum/maximum temperature are assumed to occur at sunrise / solar noon + 2 h.
 
             ``sun_loc_shift``:
-                Minimum/maximum temperature are assumed to occur at sunrise / solar noon + monthly mean shift.
+                Minimum/maximum temperature are assumed to occur at sunrise / solar noon + monthly
+                mean shift.
 
         mod_nighttime : bool, optional
             Use linear interpolation between minimum and maximum temperature.
         """
         self.data_disagg.temp = melodist.disaggregate_temperature(
             self.data_daily,
             method=method,
             min_max_time=min_max_time,
             max_delta=self.statistics.temp.max_delta,
             mean_course=self.statistics.temp.mean_course,
             sun_times=self.sun_times,
-            mod_nighttime=mod_nighttime
+            mod_nighttime=mod_nighttime,
         )
 
-    def disaggregate_precipitation(self, method='equal', zerodiv='uniform', shift=0, master_precip=None):
+    def disaggregate_precipitation(
+        self, method='equal', zerodiv='uniform', shift=0, master_precip=None
+    ):
         """
         Disaggregate precipitation.
 
         Parameters
         ----------
         method : str, optional
             Disaggregation method.
@@ -325,19 +334,26 @@
             precip_disagg = melodist.disagg_prec(self.data_daily, method=method, shift=shift)
         elif method == 'cascade':
             precip_disagg = pd.Series(index=self.data_disagg.index, dtype=float)
 
             for months, stats in zip(self.statistics.precip.months, self.statistics.precip.stats):
                 precip_daily = melodist.seasonal_subset(self.data_daily.precip, months=months)
                 if len(precip_daily) > 1:
-                    data = melodist.disagg_prec(precip_daily, method=method, cascade_options=stats,
-                                                shift=shift, zerodiv=zerodiv)
+                    data = melodist.disagg_prec(
+                        precip_daily,
+                        method=method,
+                        cascade_options=stats,
+                        shift=shift,
+                        zerodiv=zerodiv,
+                    )
                     precip_disagg.loc[data.index] = data
         elif method == 'masterstation':
-            precip_disagg = melodist.precip_master_station(self.data_daily.precip, master_precip, zerodiv)
+            precip_disagg = melodist.precip_master_station(
+                self.data_daily.precip, master_precip, zerodiv
+            )
 
         self.data_disagg.precip = precip_disagg
 
     def disaggregate_radiation(self, method='pot_rad', pot_rad=None):
         """
         Disaggregate solar radiation.
 
@@ -364,29 +380,33 @@
         pot_rad : Series, optional
             Hourly values of potential solar radiation. If ``None``, calculated internally.
         """
         if self.sun_times is None:
             self.calc_sun_times()
 
         if pot_rad is None and method != 'mean_course':
-            pot_rad = melodist.potential_radiation(self.data_disagg.index, self.lon, self.lat, self.timezone)
+            pot_rad = melodist.potential_radiation(
+                self.data_disagg.index, self.lon, self.lat, self.timezone
+            )
 
         self.data_disagg.glob = melodist.disaggregate_radiation(
             self.data_daily,
             sun_times=self.sun_times,
             pot_rad=pot_rad,
             method=method,
             angstr_a=self.statistics.glob.angstroem.a,
             angstr_b=self.statistics.glob.angstroem.b,
             bristcamp_a=self.statistics.glob.bristcamp.a,
             bristcamp_c=self.statistics.glob.bristcamp.c,
-            mean_course=self.statistics.glob.mean_course
+            mean_course=self.statistics.glob.mean_course,
         )
 
-    def interpolate(self, column_hours, method='linear', limit=24, limit_direction='both', **kwargs):
+    def interpolate(
+        self, column_hours, method='linear', limit=24, limit_direction='both', **kwargs
+    ):
         """
         Wrapper function for ``pandas.Series.interpolate`` that can be used to
         "disaggregate" values using various interpolation methods.
 
         Parameters
         ----------
         column_hours : dict
@@ -400,13 +420,18 @@
         --------
         Assume that ``mystation.data_daily.T7``, ``mystation.data_daily.T14``,
         and ``mystation.data_daily.T19`` contain air temperature measurements
         taken at 07:00, 14:00, and 19:00.
         We can use the interpolation functions provided by pandas/scipy to derive
         hourly values:
 
-        >>> mystation.data_hourly.temp = mystation.interpolate({'T7': 7, 'T14': 14, 'T19': 19}) # linear interpolation (default)
-        >>> mystation.data_hourly.temp = mystation.interpolate({'T7': 7, 'T14': 14, 'T19': 19}, method='cubic') # cubic spline
+        >>> # Linear interpolation (default)
+        >>> mystation.data_hourly.temp = mystation.interpolate({'T7': 7, 'T14': 14, 'T19': 19})
+        >>> # Cubic spline interpolation
+        >>> mystation.data_hourly.temp = mystation.interpolate(
+        >>>     {'T7': 7, 'T14': 14, 'T19': 19},
+        >>>     method='cubic',
+        >>> )
         """
         kwargs = dict(kwargs, method=method, limit=limit, limit_direction=limit_direction)
         data = melodist.util.prepare_interpolation_data(self.data_daily, column_hours)
         return data.interpolate(**kwargs)
```

### Comparing `melodist-0.1.4/melodist/stationstatistics.py` & `melodist-0.1.5/melodist/stationstatistics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,44 @@
-# -*- coding: utf-8 -*-
-###############################################################################################################
-# This file is part of MELODIST - MEteoroLOgical observation time series DISaggregation Tool                  #
-# a program to disaggregate daily values of meteorological variables to hourly values                         #
-#                                                                                                             #
-# Copyright (C) 2016  Florian Hanzer (1,2), Kristian Förster (1,2), Benjamin Winter (1,2), Thomas Marke (1)   #
-#                                                                                                             #
-# (1) Institute of Geography, University of Innsbruck, Austria                                                #
-# (2) alpS - Centre for Climate Change Adaptation, Innsbruck, Austria                                         #
-#                                                                                                             #
-# MELODIST is free software: you can redistribute it and/or modify                                            #
-# it under the terms of the GNU General Public License as published by                                        #
-# the Free Software Foundation, either version 3 of the License, or                                           #
-# (at your option) any later version.                                                                         #
-#                                                                                                             #
-# MELODIST is distributed in the hope that it will be useful,                                                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                                              #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the                                                #
-# GNU General Public License for more details.                                                                #
-#                                                                                                             #
-# You should have received a copy of the GNU General Public License                                           #
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.                                       #
-#                                                                                                             #
-###############################################################################################################
-
-from __future__ import print_function, division, absolute_import
-import melodist
-from melodist.util.bunch import Bunch
+################################################################################
+# This file is part of MELODIST - MEteoroLOgical observation time series       #
+# DISaggregation Tool.                                                         #
+#                                                                              #
+# Copyright (C) 2016-2023 Florian Hanzer, Kristian Förster, Benjamin Winter,   #
+# Thomas Marke                                                                 #
+#                                                                              #
+# MELODIST is free software: you can redistribute it and/or modify it under    #
+# the terms of the GNU General Public License as published by the Free         #
+# Software Foundation, either version 3 of the License, or (at your option)    #
+# any later version.                                                           #
+#                                                                              #
+# MELODIST is distributed in the hope that it will be useful, but WITHOUT ANY  #
+# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS    #
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more        #
+# details.                                                                     #
+#                                                                              #
+# You should have received a copy of the GNU General Public License along with #
+# this program.  If not, see <http://www.gnu.org/licenses/>.                   #
+################################################################################
 import json
+
 import numpy as np
 import pandas as pd
 
+import melodist
+from melodist.util.bunch import Bunch
+
 
 class StationStatistics(object):
     """
     Class representing objects that include statistical information about
     diurnal features of selected variables. A StationStatistics object is
     generally associated to a Station object for which this infomration
     is valid.
     """
+
     def __init__(self, data=None, lon=None, lat=None, timezone=None):
         self._data = None
         self._lon = lon
         self._lat = lat
         self._timezone = timezone
 
         if data is not None:
@@ -65,35 +62,39 @@
     @property
     def data(self):
         return self._data
 
     @data.setter
     def data(self, df):
         assert isinstance(df, pd.DataFrame)
-        assert df.index.is_all_dates
+        assert isinstance(df.index, pd.DatetimeIndex)
         assert df.index.resolution == 'hour'
 
         self._data = df.copy()
 
     def calc_precipitation_stats(self, months=None, avg_stats=True, percentile=50):
         """
-        Calculates precipitation statistics for the cascade model while aggregating hourly observations
+        Calculates precipitation statistics for the cascade model while aggregating hourly
+        observations
 
         Parameters
         ----------
-        months :        Months for each seasons to be used for statistics (array of numpy array, default=1-12, e.g., [np.arange(12) + 1])
+        months :        Months for each seasons to be used for statistics
+                        (array of numpy array, default=1-12, e.g., [np.arange(12) + 1])
         avg_stats :     average statistics for all levels True/False (default=True)
-        percentile :    percentil for splitting the dataset in small and high intensities (default=50)
-        
+        percentile :    percentile for splitting the dataset in small and high intensities
+                        (default=50)
         """
         if months is None:
             months = [np.arange(12) + 1]
 
         self.precip.months = months
-        self.precip.stats = melodist.build_casc(self.data, months=months, avg_stats=avg_stats, percentile=percentile)
+        self.precip.stats = melodist.build_casc(
+            self.data, months=months, avg_stats=avg_stats, percentile=percentile
+        )
 
     def calc_wind_stats(self):
         """
         Calculates statistics in order to derive diurnal patterns of wind speed
         """
         a, b, t_shift = melodist.fit_cosine_function(self.data.wind)
         self.wind.update(a=a, b=b, t_shift=t_shift)
@@ -108,16 +109,20 @@
 
         self.hum.month_hour_precip_mean = melodist.calculate_month_hour_precip_mean(self.data)
 
     def calc_temperature_stats(self):
         """
         Calculates statistics in order to derive diurnal patterns of temperature
         """
-        self.temp.max_delta = melodist.get_shift_by_data(self.data.temp, self._lon, self._lat, self._timezone)
-        self.temp.mean_course = melodist.util.calculate_mean_daily_course_by_month(self.data.temp, normalize=True)
+        self.temp.max_delta = melodist.get_shift_by_data(
+            self.data.temp, self._lon, self._lat, self._timezone
+        )
+        self.temp.mean_course = melodist.util.calculate_mean_daily_course_by_month(
+            self.data.temp, normalize=True
+        )
 
     def calc_radiation_stats(self, data_daily=None, day_length=None, how='all'):
         """
         Calculates statistics in order to derive solar radiation from sunshine duration or
         minimum/maximum temperature.
 
         Parameters
@@ -130,16 +135,16 @@
         """
         assert how in ('all', 'seasonal', 'monthly')
 
         self.glob.mean_course = melodist.util.calculate_mean_daily_course_by_month(self.data.glob)
 
         if data_daily is not None:
             pot_rad = melodist.potential_radiation(
-                melodist.util.hourly_index(data_daily.index),
-                self._lon, self._lat, self._timezone)
+                melodist.util.hourly_index(data_daily.index), self._lon, self._lat, self._timezone
+            )
             pot_rad_daily = pot_rad.resample('D').mean()
             obs_rad_daily = self.data.glob.resample('D').mean()
 
             if how == 'all':
                 month_ranges = [np.arange(12) + 1]
             elif how == 'seasonal':
                 month_ranges = [[3, 4, 5], [6, 7, 8], [9, 10, 11], [12, 1, 2]]
@@ -189,34 +194,29 @@
         """
         Exports statistical data to a JSON formatted file
 
         Parameters
         ----------
         filename:    output file that holds statistics data
         """
+
         def json_encoder(obj):
             if isinstance(obj, pd.DataFrame) or isinstance(obj, pd.Series):
                 if isinstance(obj.index, pd.MultiIndex):
                     obj = obj.reset_index()  # convert MultiIndex to columns
 
                 return json.loads(obj.to_json(date_format='iso'))
             elif isinstance(obj, melodist.cascade.CascadeStatistics):
                 return obj.__dict__
             elif isinstance(obj, np.ndarray):
                 return obj.tolist()
             else:
                 raise TypeError('%s not supported' % type(obj))
 
-        d = dict(
-            temp=self.temp,
-            wind=self.wind,
-            precip=self.precip,
-            hum=self.hum,
-            glob=self.glob
-        )
+        d = dict(temp=self.temp, wind=self.wind, precip=self.precip, hum=self.hum, glob=self.glob)
 
         j = json.dumps(d, default=json_encoder, indent=4)
 
         if filename is None:
             return j
         else:
             with open(filename, 'w') as f:
@@ -227,14 +227,15 @@
         """
         Imports statistical data from a JSON formatted file
 
         Parameters
         ----------
         filename:    input file that holds statistics data
         """
+
         def json_decoder(d):
             if 'p01' in d and 'pxx' in d:  # we assume this is a CascadeStatistics object
                 return melodist.cascade.CascadeStatistics.from_dict(d)
 
             return d
 
         with open(filename) as f:
@@ -245,22 +246,28 @@
         stats.temp.update(d['temp'])
         stats.hum.update(d['hum'])
         stats.precip.update(d['precip'])
         stats.wind.update(d['wind'])
         stats.glob.update(d['glob'])
 
         if stats.temp.max_delta is not None:
-            stats.temp.max_delta = pd.read_json(json.dumps(stats.temp.max_delta), typ='series').sort_index()
+            stats.temp.max_delta = pd.read_json(
+                json.dumps(stats.temp.max_delta), typ='series'
+            ).sort_index()
 
         if stats.temp.mean_course is not None:
-            mc = pd.read_json(json.dumps(stats.temp.mean_course), typ='frame').sort_index()[np.arange(1, 12 + 1)]
+            mc = pd.read_json(json.dumps(stats.temp.mean_course), typ='frame').sort_index()[
+                np.arange(1, 12 + 1)
+            ]
             stats.temp.mean_course = mc.sort_index()[np.arange(1, 12 + 1)]
 
         if stats.hum.month_hour_precip_mean is not None:
-            mhpm = pd.read_json(json.dumps(stats.hum.month_hour_precip_mean), typ='frame').sort_index()
+            mhpm = pd.read_json(
+                json.dumps(stats.hum.month_hour_precip_mean), typ='frame'
+            ).sort_index()
             mhpm = mhpm.set_index(['level_0', 'level_1', 'level_2'])  # convert to MultiIndex
             mhpm = mhpm.squeeze()  # convert to Series
             mhpm = mhpm.rename_axis([None, None, None])  # remove index labels
             stats.hum.month_hour_precip_mean = mhpm
 
         for var in ('angstroem', 'bristcamp', 'mean_course'):
             if stats.glob[var] is not None:
```

### Comparing `melodist-0.1.4/melodist/temperature.py` & `melodist-0.1.5/melodist/temperature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-# -*- coding: utf-8 -*-
-###############################################################################################################
-# This file is part of MELODIST - MEteoroLOgical observation time series DISaggregation Tool                  #
-# a program to disaggregate daily values of meteorological variables to hourly values                         #
-#                                                                                                             #
-# Copyright (C) 2016  Florian Hanzer (1,2), Kristian Förster (1,2), Benjamin Winter (1,2), Thomas Marke (1)   #
-#                                                                                                             #
-# (1) Institute of Geography, University of Innsbruck, Austria                                                #
-# (2) alpS - Centre for Climate Change Adaptation, Innsbruck, Austria                                         #
-#                                                                                                             #
-# MELODIST is free software: you can redistribute it and/or modify                                            #
-# it under the terms of the GNU General Public License as published by                                        #
-# the Free Software Foundation, either version 3 of the License, or                                           #
-# (at your option) any later version.                                                                         #
-#                                                                                                             #
-# MELODIST is distributed in the hope that it will be useful,                                                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                                              #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the                                                #
-# GNU General Public License for more details.                                                                #
-#                                                                                                             #
-# You should have received a copy of the GNU General Public License                                           #
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.                                       #
-#                                                                                                             #
-###############################################################################################################
+################################################################################
+# This file is part of MELODIST - MEteoroLOgical observation time series       #
+# DISaggregation Tool.                                                         #
+#                                                                              #
+# Copyright (C) 2016-2023 Florian Hanzer, Kristian Förster, Benjamin Winter,   #
+# Thomas Marke                                                                 #
+#                                                                              #
+# MELODIST is free software: you can redistribute it and/or modify it under    #
+# the terms of the GNU General Public License as published by the Free         #
+# Software Foundation, either version 3 of the License, or (at your option)    #
+# any later version.                                                           #
+#                                                                              #
+# MELODIST is distributed in the hope that it will be useful, but WITHOUT ANY  #
+# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS    #
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more        #
+# details.                                                                     #
+#                                                                              #
+# You should have received a copy of the GNU General Public License along with #
+# this program.  If not, see <http://www.gnu.org/licenses/>.                   #
+################################################################################
+import numpy as np
+import pandas as pd
 
-from __future__ import print_function, division, absolute_import
 import melodist
 import melodist.util
-import numpy as np
-import pandas as pd
 
 
-def disaggregate_temperature(data_daily,
-                             method='sine_min_max',
-                             min_max_time='fix',
-                             mod_nighttime=False,
-                             max_delta=None,
-                             mean_course=None,
-                             sun_times=None):
+def disaggregate_temperature(
+    data_daily,
+    method='sine_min_max',
+    min_max_time='fix',
+    mod_nighttime=False,
+    max_delta=None,
+    mean_course=None,
+    sun_times=None,
+):
     """The disaggregation function for temperature
 
     Parameters
     ----
     data_daily :      daily data
     method :          method to disaggregate
     min_max_time:     "fix" - min/max temperature at fixed times 7h/14h,
@@ -58,15 +55,16 @@
         'mean_course_mean',
     ):
         raise ValueError('Invalid option')
 
     temp_disagg = pd.Series(index=melodist.util.hourly_index(data_daily.index), dtype=float)
 
     if method in ('sine_min_max', 'sine_mean', 'sine'):
-        # for this option assume time of minimum and maximum and fit cosine function through minimum and maximum temperatures
+        # for this option assume time of minimum and maximum and fit cosine function through minimum
+        # and maximum temperatures
         hours_per_day = 24
         default_shift_hours = 2
 
         daylength_thres = 3
         # min / max hour during polar night assumption
         min_loc_polar = 6
         max_loc_polar = 18
@@ -79,32 +77,38 @@
                 'min_val_before',
                 'min_val_cur',
                 'min_val_next',
                 'max_val_before',
                 'max_val_cur',
                 'max_val_next',
                 'mean_val_cur',
-            ]
+            ],
         )
 
         if min_max_time == 'fix':
             # take fixed location for minimum and maximum
             locdf.min_loc = 7
             locdf.max_loc = 14
         elif min_max_time == 'sun_loc':
             # take location for minimum and maximum by sunrise / sunnoon + 2h
             locdf.min_loc = sun_times.sunrise.round()  # sun rise round to full hour
-            locdf.max_loc = sun_times.sunnoon.round() + default_shift_hours  # sun noon round to full hour + fix 2h
+            locdf.max_loc = (
+                sun_times.sunnoon.round() + default_shift_hours
+            )  # sun noon round to full hour + fix 2h
         elif min_max_time == 'sun_loc_shift':
             # take location for minimum and maximum by sunrise / sunnoon + monthly delta
             locdf.min_loc = sun_times.sunrise.round()  # sun rise round to full hour
-            locdf.max_loc = (sun_times.sunnoon + max_delta[locdf.index.month].values).round()  # sun noon + shift derived from observed hourly data, round to full hour
+            locdf.max_loc = (
+                sun_times.sunnoon + max_delta[locdf.index.month].values
+            ).round()  # sun noon + shift derived from observed hourly data, round to full hour
 
             pos = locdf.min_loc > locdf.max_loc
-            locdf.loc[pos, 'max_loc'] = sun_times.sunnoon[pos].round() + default_shift_hours  # standard shift in this case
+            locdf.loc[pos, 'max_loc'] = (
+                sun_times.sunnoon[pos].round() + default_shift_hours
+            )  # standard shift in this case
 
         locdf.min_loc = locdf.min_loc.astype(int)
         locdf.max_loc = locdf.max_loc.astype(int)
 
         locdf.min_val_cur = data_daily.tmin
         locdf.max_val_cur = data_daily.tmax
         locdf.mean_val_cur = data_daily.temp
@@ -116,83 +120,125 @@
         locdf.max_val_before = data_daily.tmax.shift(1, 'D')
         locdf.loc[locdf.index[0], 'min_val_before'] = locdf.min_val_cur.iloc[0]
         locdf.loc[locdf.index[0], 'max_val_before'] = locdf.max_val_cur.iloc[0]
 
         locdf_day = locdf
         locdf = locdf.reindex(temp_disagg.index, method='ffill')
 
-        # whenever we are before the maximum for the current day, use minimum value of current day for cosine function fitting
-        # once we have passed the maximum value use the minimum for next day to ensure smooth transitions
+        # whenever we are before the maximum for the current day, use minimum value of current day
+        # for cosine function fitting once we have passed the maximum value use the minimum for next
+        # day to ensure smooth transitions
         min_val = locdf.min_val_next.copy()
         min_val[min_val.index.hour < locdf.max_loc] = locdf.min_val_cur
 
-        # whenever we are before the minimum for the current day, use maximum value of day before for cosine function fitting
-        # once we have passed the minimum value use the maximum for the current day to ensure smooth transitions
+        # whenever we are before the minimum for the current day, use maximum value of day before
+        # for cosine function fitting once we have passed the minimum value use the maximum for the
+        # current day to ensure smooth transitions
         max_val = locdf.max_val_cur.copy()
         max_val[max_val.index.hour < locdf.min_loc] = locdf.max_val_before
 
         temp_disagg = pd.Series(index=min_val.index, dtype=float)
 
         if method in ('sine_min_max', 'sine'):
             delta_val = max_val - min_val
-            v_trans = min_val + delta_val / 2.
+            v_trans = min_val + delta_val / 2.0
 
             if mod_nighttime:
                 before_min = locdf.index.hour <= locdf.min_loc
-                between_min_max = (locdf.index.hour > locdf.min_loc) & (locdf.index.hour < locdf.max_loc)
+                between_min_max = (locdf.index.hour > locdf.min_loc) & (
+                    locdf.index.hour < locdf.max_loc
+                )
                 after_max = locdf.index.hour >= locdf.max_loc
-                temp_disagg[before_min]      = v_trans + delta_val / 2. * np.cos(np.pi / (hours_per_day - (locdf.max_loc - locdf.min_loc)) * (hours_per_day - locdf.max_loc + locdf.index.hour))
-                temp_disagg[between_min_max] = v_trans + delta_val / 2. * np.cos(1.25 * np.pi + 0.75 * np.pi / (locdf.max_loc - locdf.min_loc) * (locdf.index.hour - locdf.min_loc))
-                temp_disagg[after_max]       = v_trans + delta_val / 2. * np.cos(np.pi / (hours_per_day - (locdf.max_loc - locdf.min_loc)) * (locdf.index.hour - locdf.max_loc))
+                temp_disagg[before_min] = v_trans + delta_val / 2.0 * np.cos(
+                    np.pi
+                    / (hours_per_day - (locdf.max_loc - locdf.min_loc))
+                    * (hours_per_day - locdf.max_loc + locdf.index.hour)
+                )
+                temp_disagg[between_min_max] = v_trans + delta_val / 2.0 * np.cos(
+                    1.25 * np.pi
+                    + 0.75
+                    * np.pi
+                    / (locdf.max_loc - locdf.min_loc)
+                    * (locdf.index.hour - locdf.min_loc)
+                )
+                temp_disagg[after_max] = v_trans + delta_val / 2.0 * np.cos(
+                    np.pi
+                    / (hours_per_day - (locdf.max_loc - locdf.min_loc))
+                    * (locdf.index.hour - locdf.max_loc)
+                )
             else:
-                temp_disagg[:] = v_trans + (delta_val / 2.) * np.cos(2 * np.pi / hours_per_day * (locdf.index.hour - locdf.max_loc))
+                temp_disagg[:] = v_trans + (delta_val / 2.0) * np.cos(
+                    2 * np.pi / hours_per_day * (locdf.index.hour - locdf.max_loc)
+                )
         elif method == 'sine_mean':
             dtr = locdf.max_val_cur - locdf.min_val_cur
-            temp_disagg[:] = locdf.mean_val_cur + dtr / 2. * np.cos(2 * np.pi / hours_per_day * (locdf.index.hour - locdf.max_loc))
+            temp_disagg[:] = locdf.mean_val_cur + dtr / 2.0 * np.cos(
+                2 * np.pi / hours_per_day * (locdf.index.hour - locdf.max_loc)
+            )
 
         polars = sun_times.daylength < daylength_thres
         if polars.sum() > 0:
             # during polar night, no diurnal variation of temperature is applied
             # instead the daily average calculated using tmin and tmax is applied
             polars_index_hourly = melodist.util.hourly_index(polars[polars].index)
             temp_disagg.loc[polars_index_hourly] = np.nan
 
-            avg_before = (locdf_day.min_val_before + locdf_day.max_val_before) / 2.
-            avg_cur = (locdf_day.min_val_cur + locdf_day.max_val_cur) / 2.
-            getting_warmers = polars &  (avg_before <= avg_cur)
+            avg_before = (locdf_day.min_val_before + locdf_day.max_val_before) / 2.0
+            avg_cur = (locdf_day.min_val_cur + locdf_day.max_val_cur) / 2.0
+            getting_warmers = polars & (avg_before <= avg_cur)
             getting_colders = polars & ~(avg_before <= avg_cur)
 
-            getting_warmers_min_loc = pd.DatetimeIndex([ts.replace(hour=min_loc_polar) for ts in getting_warmers[getting_warmers].index])
-            getting_warmers_max_loc = pd.DatetimeIndex([ts.replace(hour=max_loc_polar) for ts in getting_warmers[getting_warmers].index])
+            getting_warmers_min_loc = pd.DatetimeIndex(
+                [ts.replace(hour=min_loc_polar) for ts in getting_warmers[getting_warmers].index]
+            )
+            getting_warmers_max_loc = pd.DatetimeIndex(
+                [ts.replace(hour=max_loc_polar) for ts in getting_warmers[getting_warmers].index]
+            )
             temp_disagg[getting_warmers_min_loc] = locdf_day.min_val_cur[getting_warmers].values
             temp_disagg[getting_warmers_max_loc] = locdf_day.max_val_cur[getting_warmers].values
 
-            getting_colders_min_loc = pd.DatetimeIndex([ts.replace(hour=min_loc_polar) for ts in getting_colders[getting_colders].index])
-            getting_colders_max_loc = pd.DatetimeIndex([ts.replace(hour=max_loc_polar) for ts in getting_colders[getting_colders].index])
+            getting_colders_min_loc = pd.DatetimeIndex(
+                [ts.replace(hour=min_loc_polar) for ts in getting_colders[getting_colders].index]
+            )
+            getting_colders_max_loc = pd.DatetimeIndex(
+                [ts.replace(hour=max_loc_polar) for ts in getting_colders[getting_colders].index]
+            )
             temp_disagg[getting_colders_min_loc] = locdf_day.max_val_cur[getting_colders].values
             temp_disagg[getting_colders_max_loc] = locdf_day.min_val_cur[getting_colders].values
 
             temp_polars = temp_disagg.loc[polars_index_hourly].copy()
-            transition_days = polars[polars.diff() == True].astype(int) # 0 where transition from polar to "normal" mode, 1 where transition from normal to polar
+            transition_days = polars[polars.diff()].astype(
+                int
+            )
+            # (0 where transition from polar to "normal" mode, 1 where transition from normal to
+            # polar)
 
             if len(transition_days) > 0:
                 polar_to_normal_days = transition_days.index[transition_days == 0]
-                normal_to_polar_days = transition_days.index[transition_days == 1] - pd.Timedelta(days=1)
+                normal_to_polar_days = transition_days.index[transition_days == 1] - pd.Timedelta(
+                    days=1
+                )
                 add_days = polar_to_normal_days.union(normal_to_polar_days)
 
-                temp_polars = temp_polars.append(temp_disagg[melodist.util.hourly_index(add_days)]).sort_index()
+                temp_polars = temp_polars.append(
+                    temp_disagg[melodist.util.hourly_index(add_days)]
+                ).sort_index()
 
                 for day in polar_to_normal_days:
                     min_loc = int(locdf.loc[day].min_loc)
-                    temp_polars[day.replace(hour=0):day.replace(hour=min_loc) - pd.Timedelta(hours=1)] = np.nan
+                    temp_polars[
+                        day.replace(hour=0) : day.replace(hour=min_loc) - pd.Timedelta(hours=1)
+                    ] = np.nan
                     temp_polars[day.replace(hour=min_loc)] = locdf.min_val_cur[day]
 
                 for day in normal_to_polar_days:
                     max_loc = int(locdf.loc[day].max_loc)
-                    temp_polars[day.replace(hour=max_loc) + pd.Timedelta(hours=1):day.replace(hour=23)] = np.nan
+                    temp_polars[
+                        day.replace(hour=max_loc) + pd.Timedelta(hours=1) : day.replace(hour=23)
+                    ] = np.nan
 
             temp_interp = temp_polars.interpolate(method='linear', limit=23)
             temp_disagg[temp_interp.index] = temp_interp
     elif method == 'mean_course_min_max':
         data_daily_as_hourly = data_daily.reindex(temp_disagg.index, method='ffill', limit=23)
 
         df = pd.DataFrame(index=temp_disagg.index)
@@ -201,29 +247,35 @@
         df['tmax'] = data_daily_as_hourly.tmax
 
         temp_disagg[:] = df.normval * (df.tmax - df.tmin) + df.tmin
     elif method == 'mean_course_mean':
         data_daily_as_hourly = data_daily.reindex(temp_disagg.index, method='ffill', limit=23)
         dtr = data_daily_as_hourly.tmax - data_daily_as_hourly.tmin
         mc = pd.Series(index=temp_disagg.index, dtype=float)
-        mean_course_zeromean = mean_course - mean_course.mean()  # shift mean course so that the daily mean is 0
-        mc[:] = mean_course_zeromean.unstack().loc[list(zip(temp_disagg.index.month, temp_disagg.index.hour))].values
+        mean_course_zeromean = (
+            mean_course - mean_course.mean()
+        )  # shift mean course so that the daily mean is 0
+        mc[:] = (
+            mean_course_zeromean.unstack()
+            .loc[list(zip(temp_disagg.index.month, temp_disagg.index.hour))]
+            .values
+        )
         temp_disagg[:] = data_daily_as_hourly.temp + dtr * mc
 
     return temp_disagg
 
 
 def get_shift_by_data(temp_hourly, lon, lat, time_zone):
-    '''function to get max temp shift (monthly) by hourly data
-    
+    '''Get maximum temperature shift (monthly) from hourly data
+
     Parameters
     ----
-    hourly_data_obs : observed hourly data 
-    lat :             latitude in DezDeg
-    lon :             longitude in DezDeg
+    hourly_data_obs : observed hourly data
+    lat :             latitude (degrees)
+    lon :             longitude (degrees)
     time_zone:        timezone
     '''
     daily_index = temp_hourly.resample('D').mean().index
     sun_times = melodist.util.get_sun_times(daily_index, lon, lat, time_zone)
 
     idxmax = temp_hourly.groupby(temp_hourly.index.date).idxmax()
     idxmax.index = pd.to_datetime(idxmax.index)
```

### Comparing `melodist-0.1.4/melodist/util/util.py` & `melodist-0.1.5/melodist/util/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,27 @@
-# -*- coding: utf-8 -*-
-###############################################################################################################
-# This file is part of MELODIST - MEteoroLOgical observation time series DISaggregation Tool                  #
-# a program to disaggregate daily values of meteorological variables to hourly values                         #
-#                                                                                                             #
-# Copyright (C) 2016  Florian Hanzer (1,2), Kristian Förster (1,2), Benjamin Winter (1,2), Thomas Marke (1)   #
-#                                                                                                             #
-# (1) Institute of Geography, University of Innsbruck, Austria                                                #
-# (2) alpS - Centre for Climate Change Adaptation, Innsbruck, Austria                                         #
-#                                                                                                             #
-# MELODIST is free software: you can redistribute it and/or modify                                            #
-# it under the terms of the GNU General Public License as published by                                        #
-# the Free Software Foundation, either version 3 of the License, or                                           #
-# (at your option) any later version.                                                                         #
-#                                                                                                             #
-# MELODIST is distributed in the hope that it will be useful,                                                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                                              #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the                                                #
-# GNU General Public License for more details.                                                                #
-#                                                                                                             #
-# You should have received a copy of the GNU General Public License                                           #
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.                                       #
-#                                                                                                             #
-###############################################################################################################
-
-from __future__ import print_function, division, absolute_import
+################################################################################
+# This file is part of MELODIST - MEteoroLOgical observation time series       #
+# DISaggregation Tool.                                                         #
+#                                                                              #
+# Copyright (C) 2016-2023 Florian Hanzer, Kristian Förster, Benjamin Winter,   #
+# Thomas Marke                                                                 #
+#                                                                              #
+# MELODIST is free software: you can redistribute it and/or modify it under    #
+# the terms of the GNU General Public License as published by the Free         #
+# Software Foundation, either version 3 of the License, or (at your option)    #
+# any later version.                                                           #
+#                                                                              #
+# MELODIST is distributed in the hope that it will be useful, but WITHOUT ANY  #
+# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS    #
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more        #
+# details.                                                                     #
+#                                                                              #
+# You should have received a copy of the GNU General Public License along with #
+# this program.  If not, see <http://www.gnu.org/licenses/>.                   #
+################################################################################
 import numpy as np
 import pandas as pd
 import scipy.stats
 
 
 def hourly_index(daily_index, fill_gaps=False):
     index = pd.date_range(start=daily_index.min(), end=daily_index.max().replace(hour=23), freq='H')
@@ -35,18 +29,20 @@
     # remove days that are not in the daily index:
     if not fill_gaps and len(index) > len(daily_index) * 24:
         df = pd.DataFrame(index=index.date, data=dict(hour=index.hour, keep=True))
         df.index = df.index.to_datetime()
         dropdates = list(set(index.date) - set(daily_index.date))
         df.loc[dropdates, 'keep'] = False
         df = df[df.keep]
-        index = pd.DatetimeIndex([pd.datetime(y, m, d, h) for y, m, d, h in zip(df.index.year,
-                                                                                df.index.month,
-                                                                                df.index.day,
-                                                                                df.hour)])
+        index = pd.DatetimeIndex(
+            [
+                pd.datetime(y, m, d, h)
+                for y, m, d, h in zip(df.index.year, df.index.month, df.index.day, df.hour)
+            ]
+        )
 
     return index
 
 
 def distribute_equally(daily_data, divide=False):
     """Obtains hourly values by equally distributing the daily values.
 
@@ -58,15 +54,16 @@
     Returns:
         Equally distributed hourly values.
     """
 
     index = hourly_index(daily_data.index)
     hourly_data = daily_data.reindex(index)
     hourly_data = hourly_data.groupby(hourly_data.index.day).transform(
-        lambda x: x.fillna(method='ffill', limit=23))
+        lambda x: x.fillna(method='ffill', limit=23)
+    )
 
     if divide:
         hourly_data /= 24
 
     return hourly_data
 
 
@@ -81,57 +78,75 @@
     Returns:
         Vapor pressure in hPa.
     """
 
     if np.isscalar(hum):
         hum = np.zeros(temp.shape) + hum
 
-    assert(temp.shape == hum.shape)
+    assert temp.shape == hum.shape
 
     positives = np.array(temp >= 273.15)
     vap_press = np.zeros(temp.shape) * np.nan
-    vap_press[positives] = 6.112 * np.exp((17.62 * (temp[positives] - 273.15)) / (243.12 + (temp[positives] - 273.15))) * hum[positives] / 100.
-    vap_press[~positives] = 6.112 * np.exp((22.46 * (temp[~positives] - 273.15)) / (272.62  + (temp[~positives] - 273.15))) * hum[~positives] / 100.
+    vap_press[positives] = (
+        6.112
+        * np.exp((17.62 * (temp[positives] - 273.15)) / (243.12 + (temp[positives] - 273.15)))
+        * hum[positives]
+        / 100.0
+    )
+    vap_press[~positives] = (
+        6.112
+        * np.exp((22.46 * (temp[~positives] - 273.15)) / (272.62 + (temp[~positives] - 273.15)))
+        * hum[~positives]
+        / 100.0
+    )
 
     return vap_press
 
 
 def dewpoint_temperature(temp, hum):
     """computes the dewpoint temperature
 
     Parameters
     ----
     temp :      temperature [K]
     hum :       relative humidity
-    
+
 
     Returns
         dewpoint temperature in K
     """
-    assert(temp.shape == hum.shape)
+    assert temp.shape == hum.shape
 
     vap_press = vapor_pressure(temp, hum)
 
     positives = np.array(temp >= 273.15)
     dewpoint_temp = temp.copy() * np.nan
-    dewpoint_temp[positives] = 243.12 * np.log(vap_press[positives] / 6.112) / (17.62 - np.log(vap_press[positives] / 6.112))
-    dewpoint_temp[~positives] = 272.62 * np.log(vap_press[~positives] / 6.112) / (22.46 - np.log(vap_press[~positives] / 6.112))
+    dewpoint_temp[positives] = (
+        243.12
+        * np.log(vap_press[positives] / 6.112)
+        / (17.62 - np.log(vap_press[positives] / 6.112))
+    )
+    dewpoint_temp[~positives] = (
+        272.62
+        * np.log(vap_press[~positives] / 6.112)
+        / (22.46 - np.log(vap_press[~positives] / 6.112))
+    )
 
     return dewpoint_temp + 273.15
 
 
 def linregress(x, y, return_stats=False):
     """linear regression calculation
 
     Parameters
     ----
     x :         independent variable (series)
     y :         dependent variable (series)
     return_stats : returns statistical values as well if required (bool)
-    
+
 
     Returns
     ----
     list of parameters (and statistics)
     """
     a1, a0, r_value, p_value, stderr = scipy.stats.linregress(x, y)
 
@@ -147,72 +162,82 @@
 
     Parameters
     ----
     dates:      datetime
     lat :       latitude in DecDeg
     lon :       longitude in DecDeg
     time_zone : timezone
-    
+
 
     Returns
     ----
     DataFrame:  [sunrise, sunnoon, sunset, day length] in dec hours
     """
 
     df = pd.DataFrame(index=dates, columns=['sunrise', 'sunnoon', 'sunset', 'daylength'])
 
     doy = np.array([(d - d.replace(day=1, month=1)).days + 1 for d in df.index])  # day of year
 
     # Day angle and declination after Bourges (1985):
-    day_angle_b = np.deg2rad((360. / 365.25) * (doy - 79.346))
-    
+    day_angle_b = np.deg2rad((360.0 / 365.25) * (doy - 79.346))
+
     declination = np.deg2rad(
-        0.3723 + 23.2567 * np.sin(day_angle_b) - 0.7580 * np.cos(day_angle_b)
-        + 0.1149 * np.sin(2*day_angle_b) + 0.3656 * np.cos(2*day_angle_b)
-        - 0.1712 * np.sin(3*day_angle_b) + 0.0201 * np.cos(3*day_angle_b)
+        0.3723
+        + 23.2567 * np.sin(day_angle_b)
+        - 0.7580 * np.cos(day_angle_b)
+        + 0.1149 * np.sin(2 * day_angle_b)
+        + 0.3656 * np.cos(2 * day_angle_b)
+        - 0.1712 * np.sin(3 * day_angle_b)
+        + 0.0201 * np.cos(3 * day_angle_b)
     )
-    
+
     # Equation of time with day angle after Spencer (1971):
-    day_angle_s = 2 * np.pi * (doy - 1) / 365.
-    eq_time = 12. / np.pi * (
-        0.000075 +
-        0.001868 * np.cos(  day_angle_s) - 0.032077 * np.sin(  day_angle_s) -
-        0.014615 * np.cos(2*day_angle_s) - 0.040849 * np.sin(2*day_angle_s)
+    day_angle_s = 2 * np.pi * (doy - 1) / 365.0
+    eq_time = (
+        12.0
+        / np.pi
+        * (
+            0.000075
+            + 0.001868 * np.cos(day_angle_s)
+            - 0.032077 * np.sin(day_angle_s)
+            - 0.014615 * np.cos(2 * day_angle_s)
+            - 0.040849 * np.sin(2 * day_angle_s)
         )
-    
+    )
+
     #
-    standard_meridian = time_zone * 15.
-    delta_lat_time = (lon - standard_meridian) * 24. / 360.
-    
+    standard_meridian = time_zone * 15.0
+    delta_lat_time = (lon - standard_meridian) * 24.0 / 360.0
+
     omega_nul_arg = -np.tan(np.deg2rad(lat)) * np.tan(declination)
     omega_nul = np.arccos(omega_nul_arg)
-    sunrise = 12. * (1. - (omega_nul) / np.pi) - delta_lat_time - eq_time
-    sunset  = 12. * (1. + (omega_nul) / np.pi) - delta_lat_time - eq_time
+    sunrise = 12.0 * (1.0 - (omega_nul) / np.pi) - delta_lat_time - eq_time
+    sunset = 12.0 * (1.0 + (omega_nul) / np.pi) - delta_lat_time - eq_time
 
     # as an approximation, solar noon is independent of the below mentioned
     # cases:
-    sunnoon  = 12. * (1.) - delta_lat_time - eq_time
-    
+    sunnoon = 12.0 * (1.0) - delta_lat_time - eq_time
+
     # $kf 2015-11-13: special case midnight sun and polar night
     # CASE 1: MIDNIGHT SUN
     # set sunrise and sunset to values that would yield the maximum day
     # length even though this a crude assumption
     pos = omega_nul_arg < -1
     sunrise[pos] = sunnoon[pos] - 12
-    sunset[pos]  = sunnoon[pos] + 12
+    sunset[pos] = sunnoon[pos] + 12
 
     # CASE 2: POLAR NIGHT
     # set sunrise and sunset to values that would yield the minmum day
     # length even though this a crude assumption
     pos = omega_nul_arg > 1
     sunrise[pos] = sunnoon[pos]
-    sunset[pos]  = sunnoon[pos]
+    sunset[pos] = sunnoon[pos]
 
     daylength = sunset - sunrise
-        
+
     # adjust if required
     sunrise[sunrise < 0] += 24
     sunset[sunset > 24] -= 24
 
     df.sunrise = sunrise
     df.sunnoon = sunnoon
     df.sunset = sunset
@@ -220,15 +245,15 @@
 
     return df
 
 
 def detect_gaps(dataframe, timestep, print_all=False, print_max=5, verbose=True):
     """checks if a given dataframe contains gaps and returns the number of gaps
 
-    This funtion checks if a dataframe contains any gaps for a given temporal
+    This function checks if a dataframe contains any gaps for a given temporal
     resolution that needs to be specified in seconds. The number of gaps
     detected in the dataframe is returned.
 
     Args:
         dataframe: A pandas dataframe object with index defined as datetime
         timestep (int): The temporal resolution of the time series in seconds
             (e.g., 86400 for daily values)
@@ -245,34 +270,41 @@
     warning_printed = False
     try:
         n = len(dataframe.index)
     except:
         print('Error: Invalid dataframe.')
         return -1
     for i in range(0, n):
-        if(i > 0):
-            time_diff = dataframe.index[i] - dataframe.index[i-1]
-            if(time_diff.delta/1E9 != timestep):
+        if i > 0:
+            time_diff = dataframe.index[i] - dataframe.index[i - 1]
+            if time_diff.delta / 1e9 != timestep:
                 gcount += 1
                 if print_all or (msg_counter <= print_max - 1):
                     if verbose:
-                        print('Warning: Gap in time series found between %s and %s' % (dataframe.index[i-1], dataframe.index[i]))
+                        print(
+                            'Warning: Gap in time series found between %s and %s'
+                            % (dataframe.index[i - 1], dataframe.index[i])
+                        )
                     msg_counter += 1
                 if msg_counter == print_max and verbose and not warning_printed:
-                    print('Waring: Only the first %i gaps have been listed. Try to increase print_max parameter to show more details.' % msg_counter)
+                    print(
+                        'Warning: Only the first %i gaps have been listed. Try to increase '
+                        'print_max parameter to show more details.'
+                        % msg_counter
+                    )
                     warning_printed = True
     if verbose:
         print('%i gaps found in total.' % (gcount))
     return gcount
 
 
 def drop_incomplete_days(dataframe, shift=0):
     """truncates a given dataframe to full days only
 
-    This funtion truncates a given pandas dataframe (time series) to full days
+    This function truncates a given pandas dataframe (time series) to full days
     only, thus dropping leading and tailing hours of incomplete days. Please
     note that this methodology only applies to hourly time series.
 
     Args:
         dataframe: A pandas dataframe object with index defined as datetime
         shift (unsigned int, opt): First hour of daily recordings. For daily
             recordings of precipitation gages, 8 would be the first hour of
@@ -293,45 +325,47 @@
         last += 24
     try:
         # todo: move this checks to a separate function
         n = len(dataframe.index)
     except:
         print('Error: Invalid dataframe.')
         return dataframe
-    
-    delete = list()  
-    
+
+    delete = list()
+
     # drop heading lines if required
     for i in range(0, n):
         if dataframe.index.hour[i] == first and dataframe.index.minute[i] == 0:
             break
         else:
             delete.append(i)
             dropped += 1
 
     # drop tailing lines if required
-    for i in range(n-1, 0, -1):
+    for i in range(n - 1, 0, -1):
         if dataframe.index.hour[i] == last and dataframe.index.minute[i] == 0:
             break
         else:
             delete.append(i)
             dropped += 1
     # print("The following rows have been dropped (%i in total):" % dropped)
     # print(delete)
-    return dataframe.drop(dataframe.index[[delete]])
+    return dataframe.drop(index=dataframe.index[delete])
 
 
 def prepare_interpolation_data(data_daily, column_hours):
     start_date = data_daily.index[0]
     end_date = data_daily.index[-1]
 
     data = pd.Series()
 
     for column, hour in column_hours.items():
-        index = pd.date_range(start=start_date.replace(hour=hour), end=end_date.replace(hour=hour), freq='D')
+        index = pd.date_range(
+            start=start_date.replace(hour=hour), end=end_date.replace(hour=hour), freq='D'
+        )
         s = pd.Series(index=index, data=data_daily[column].values)
         data = data.append(s)
 
     data = data.sort_index()
     data = data.reindex(hourly_index(data_daily.index))
 
     return data
@@ -381,15 +415,15 @@
 
 
 def calculate_mean_daily_course_by_month(data_hourly, normalize=False):
     data_hourly = data_hourly.copy()
     data_hourly.index.name = None
 
     df = data_hourly.groupby([data_hourly.index.month, data_hourly.index.hour]).mean()
-    df = df.reset_index().pivot('level_1', 'level_0')
+    df = df.reset_index().pivot(columns='level_0', index='level_1')
     df.columns = df.columns.droplevel()  # remove MultiIndex
     df.columns.name = None
     df.index.name = None
 
     if normalize:
         df = (df - df.min()) / (df.max() - df.min())  # normalize values to 0-1 range
```

### Comparing `melodist-0.1.4/melodist/wind.py` & `melodist-0.1.5/melodist/wind.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,94 +1,93 @@
-# -*- coding: utf-8 -*-
-###############################################################################################################
-# This file is part of MELODIST - MEteoroLOgical observation time series DISaggregation Tool                  #
-# a program to disaggregate daily values of meteorological variables to hourly values                         #
-#                                                                                                             #
-# Copyright (C) 2016  Florian Hanzer (1,2), Kristian Förster (1,2), Benjamin Winter (1,2), Thomas Marke (1)   #
-#                                                                                                             #
-# (1) Institute of Geography, University of Innsbruck, Austria                                                #
-# (2) alpS - Centre for Climate Change Adaptation, Innsbruck, Austria                                         #
-#                                                                                                             #
-# MELODIST is free software: you can redistribute it and/or modify                                            #
-# it under the terms of the GNU General Public License as published by                                        #
-# the Free Software Foundation, either version 3 of the License, or                                           #
-# (at your option) any later version.                                                                         #
-#                                                                                                             #
-# MELODIST is distributed in the hope that it will be useful,                                                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                                              #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the                                                #
-# GNU General Public License for more details.                                                                #
-#                                                                                                             #
-# You should have received a copy of the GNU General Public License                                           #
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.                                       #
-#                                                                                                             #
-###############################################################################################################
-
-from __future__ import print_function, division, absolute_import
-import melodist
+################################################################################
+# This file is part of MELODIST - MEteoroLOgical observation time series       #
+# DISaggregation Tool.                                                         #
+#                                                                              #
+# Copyright (C) 2016-2023 Florian Hanzer, Kristian Förster, Benjamin Winter,   #
+# Thomas Marke                                                                 #
+#                                                                              #
+# MELODIST is free software: you can redistribute it and/or modify it under    #
+# the terms of the GNU General Public License as published by the Free         #
+# Software Foundation, either version 3 of the License, or (at your option)    #
+# any later version.                                                           #
+#                                                                              #
+# MELODIST is distributed in the hope that it will be useful, but WITHOUT ANY  #
+# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS    #
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more        #
+# details.                                                                     #
+#                                                                              #
+# You should have received a copy of the GNU General Public License along with #
+# this program.  If not, see <http://www.gnu.org/licenses/>.                   #
+################################################################################
 import numpy as np
 import pandas as pd
 import scipy.optimize
 
+import melodist
+
 
 def _cosine_function(x, a, b, t_shift):
-    """genrates a diurnal course of windspeed accroding to the cosine function
+    """Generate a diurnal course of windspeed according to the cosine function
 
     Args:
         x: series of euqally distributed windspeed values
         a: parameter a for the cosine function
         b: parameter b for the cosine function
         t_shift: parameter t_shift for the cosine function
-        
+
     Returns:
         series including diurnal course of windspeed.
     """
 
     mean_wind, t = x
     return a * mean_wind * np.cos(np.pi * (t - t_shift) / 12) + b * mean_wind
 
 
 def disaggregate_wind(wind_daily, method='equal', a=None, b=None, t_shift=None):
-    """general function for windspeed disaggregation
+    """General function for windspeed disaggregation
 
     Args:
         wind_daily: daily values
         method: keyword specifying the disaggregation method to be used
         a: parameter a for the cosine function
         b: parameter b for the cosine function
         t_shift: parameter t_shift for the cosine function
-        
+
     Returns:
         Disaggregated hourly values of windspeed.
     """
     assert method in ('equal', 'cosine', 'random'), 'Invalid method'
 
     wind_eq = melodist.distribute_equally(wind_daily)
 
     if method == 'equal':
         wind_disagg = wind_eq
     elif method == 'cosine':
         assert None not in (a, b, t_shift)
-        wind_disagg = _cosine_function(np.array([wind_eq.values, wind_eq.index.hour]), a, b, t_shift)
+        wind_disagg = _cosine_function(
+            np.array([wind_eq.values, wind_eq.index.hour]), a, b, t_shift
+        )
     elif method == 'random':
-        wind_disagg = wind_eq * (-np.log(np.random.rand(len(wind_eq))))**0.3
+        wind_disagg = wind_eq * (-np.log(np.random.rand(len(wind_eq)))) ** 0.3
 
     return wind_disagg
 
 
 def fit_cosine_function(wind):
-    """fits a cosine function to observed hourly windspeed data
+    """Fit a cosine function to observed hourly windspeed data
 
     Args:
         wind: observed hourly windspeed data
-        
+
     Returns:
         parameters needed to generate diurnal features of windspeed using a cosine function
     """
     wind_daily = wind.groupby(wind.index.date).mean()
-    wind_daily_hourly = pd.Series(index=wind.index, data=wind_daily.loc[wind.index.date].values)  # daily values evenly distributed over the hours
+    wind_daily_hourly = pd.Series(
+        index=wind.index, data=wind_daily.loc[wind.index.date].values
+    )  # daily values evenly distributed over the hours
 
     df = pd.DataFrame(data=dict(daily=wind_daily_hourly, hourly=wind)).dropna(how='any')
     x = np.array([df.daily, df.index.hour])
     popt, pcov = scipy.optimize.curve_fit(_cosine_function, x, df.hourly)
 
     return popt
```

