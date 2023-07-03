# Comparing `tmp/metafora-1.0.2.tar.gz` & `tmp/metafora-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metafora-1.0.2.tar", last modified: Wed Mar 15 14:56:45 2023, max compression
+gzip compressed data, was "dist/metafora-1.1.0.tar", last modified: Mon Jul  3 07:44:42 2023, max compression
```

## Comparing `metafora-1.0.2.tar` & `metafora-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 dalmau    (1000) dalmau    (1000)        0 2023-03-15 14:56:45.707294 metafora-1.0.2/
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)      273 2023-03-15 14:56:45.707294 metafora-1.0.2/PKG-INFO
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)     1357 2023-02-06 18:00:18.000000 metafora-1.0.2/README.rst
-drwxrwxr-x   0 dalmau    (1000) dalmau    (1000)        0 2023-03-15 14:56:45.707294 metafora-1.0.2/metafora/
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)      184 2023-03-15 14:54:23.000000 metafora-1.0.2/metafora/__init__.py
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)    11044 2023-02-19 10:04:43.000000 metafora-1.0.2/metafora/common.py
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)     2403 2023-02-19 10:04:43.000000 metafora-1.0.2/metafora/enums.py
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)     7228 2023-02-19 10:04:43.000000 metafora-1.0.2/metafora/metar.py
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)     1027 2023-02-19 10:04:43.000000 metafora-1.0.2/metafora/ml.py
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)     2500 2023-02-05 17:49:41.000000 metafora-1.0.2/metafora/parser.py
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)     7504 2023-02-08 06:44:06.000000 metafora-1.0.2/metafora/taf.py
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)     2423 2023-02-19 10:04:43.000000 metafora-1.0.2/metafora/utils.py
-drwxrwxr-x   0 dalmau    (1000) dalmau    (1000)        0 2023-03-15 14:56:45.707294 metafora-1.0.2/metafora.egg-info/
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)      273 2023-03-15 14:56:45.000000 metafora-1.0.2/metafora.egg-info/PKG-INFO
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)      322 2023-03-15 14:56:45.000000 metafora-1.0.2/metafora.egg-info/SOURCES.txt
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)        1 2023-03-15 14:56:45.000000 metafora-1.0.2/metafora.egg-info/dependency_links.txt
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)       61 2023-03-15 14:56:45.000000 metafora-1.0.2/metafora.egg-info/requires.txt
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)        9 2023-03-15 14:56:45.000000 metafora-1.0.2/metafora.egg-info/top_level.txt
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)       38 2023-03-15 14:56:45.707294 metafora-1.0.2/setup.cfg
--rw-rw-r--   0 dalmau    (1000) dalmau    (1000)      519 2023-03-15 14:54:15.000000 metafora-1.0.2/setup.py
+drwxrwxr-x   0 dalmau    (1000) dalmau    (1000)        0 2023-07-03 07:44:42.000000 metafora-1.1.0/
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)      318 2023-07-03 07:44:42.000000 metafora-1.1.0/PKG-INFO
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)     1357 2023-02-06 18:00:18.000000 metafora-1.1.0/README.rst
+drwxrwxr-x   0 dalmau    (1000) dalmau    (1000)        0 2023-07-03 07:44:42.000000 metafora-1.1.0/metafora/
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)      184 2023-07-03 07:32:32.000000 metafora-1.1.0/metafora/__init__.py
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)    10481 2023-07-03 07:31:01.000000 metafora-1.1.0/metafora/common.py
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)     2403 2023-02-19 10:04:43.000000 metafora-1.1.0/metafora/enums.py
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)     7218 2023-07-03 07:28:40.000000 metafora-1.1.0/metafora/metar.py
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)     1027 2023-02-19 10:04:43.000000 metafora-1.1.0/metafora/ml.py
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)     2500 2023-02-05 17:49:41.000000 metafora-1.1.0/metafora/parser.py
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)     7504 2023-02-08 06:44:06.000000 metafora-1.1.0/metafora/taf.py
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)     2423 2023-02-19 10:04:43.000000 metafora-1.1.0/metafora/utils.py
+drwxrwxr-x   0 dalmau    (1000) dalmau    (1000)        0 2023-07-03 07:44:42.000000 metafora-1.1.0/metafora.egg-info/
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)      318 2023-07-03 07:44:42.000000 metafora-1.1.0/metafora.egg-info/PKG-INFO
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)      322 2023-07-03 07:44:42.000000 metafora-1.1.0/metafora.egg-info/SOURCES.txt
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)        1 2023-07-03 07:44:42.000000 metafora-1.1.0/metafora.egg-info/dependency_links.txt
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)       61 2023-07-03 07:44:42.000000 metafora-1.1.0/metafora.egg-info/requires.txt
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)        9 2023-07-03 07:44:42.000000 metafora-1.1.0/metafora.egg-info/top_level.txt
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)       38 2023-07-03 07:44:42.000000 metafora-1.1.0/setup.cfg
+-rw-rw-r--   0 dalmau    (1000) dalmau    (1000)      519 2023-07-03 07:32:21.000000 metafora-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `metafora-1.0.2/README.rst` & `metafora-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `metafora-1.0.2/metafora/common.py` & `metafora-1.1.0/metafora/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,20 +12,16 @@
     convert_distance,
     convert_speed,
     convert_direction,
     Number,
 )
 from metafora.enums import *
 
-WEATHER_MEMBERS = "|".join(
-    WeatherDescriptor.set()
-    .union(WeatherPrecipitation.set())
-    .union(WeatherObscuration.set())
-    .union(OtherWeather.set())
-)
+WEATHER_DESCRIPTOR = "|".join(WeatherDescriptor.set())
+WEATHER_PHENOMENA = "|".join(WeatherPrecipitation.set().union(WeatherObscuration.set()).union(OtherWeather.set()))
 
 TIME_FORMAT = "(0[0-9]|1[0-9]|2[0-9]|3[0-1])(0[0-9]|1[0-9]|2[0-4])([0-5][0-9])"
 DIRECTION_FMT = "0[0-9][0-9]|1[0-9][0-9]|2[0-9][0-9]|3[0-5][0-9]|360"
 
 
 class Station(str):
     """
@@ -234,75 +230,65 @@
 
     intensity: Optional[str] = field(
         default=None, metadata=config(exclude=lambda x: x is None)
     )
     descriptor: Optional[str] = field(
         default=None, metadata=config(exclude=lambda x: x is None)
     )
-    precipitation: Optional[str] = field(
-        default=None, metadata=config(exclude=lambda x: x is None)
-    )
-    obscuration: Optional[str] = field(
-        default=None, metadata=config(exclude=lambda x: x is None)
-    )
-    other: Optional[str] = field(
+    phenomena: Optional[str] = field(
         default=None, metadata=config(exclude=lambda x: x is None)
     )
 
     @classmethod
     def from_text(cls, token: str):
         """
         Attempts to parse the weather conditions from a token
 
         :param token: token
         :return: weather conditions instance or None if not successful
         """
         expression = (
                 "^([-+]|VC)?("
-                + WEATHER_MEMBERS
+                + WEATHER_DESCRIPTOR
                 + ")?("
-                + WEATHER_MEMBERS
+                + WEATHER_PHENOMENA
                 + ")?("
-                + WEATHER_MEMBERS
+                + WEATHER_PHENOMENA
                 + ")?("
-                + WEATHER_MEMBERS
+                + WEATHER_PHENOMENA
                 + ")?(NSW)?$"
         )
         found = re.search(expression, token)
 
         if not found:
             return None
 
         intensity = None
         descriptor = None
-        precipitation = None
-        obscuration = None
-        other = None
+        phenomena = None
 
         # intensity
         if found[1]:
             intensity = found[1]
 
+        # descriptor
+        if found[2]:
+            descriptor = found[2]
+
         # for all codes after intensity ...
-        for code in found.groups()[1:]:
-            if code in WeatherDescriptor.set() and descriptor is None:
-                descriptor = code
-            elif code in WeatherPrecipitation.set() and precipitation is None:
-                precipitation = code
-            elif code in WeatherObscuration.set() and obscuration is None:
-                obscuration = code
-            elif code in OtherWeather.set() and other is None:
-                other = code
+        if found[3]:
+            phenomena = ""
+            for code in found.groups()[2:]:
+                if code:
+                    phenomena += code
 
         return cls(
             intensity=intensity,
             descriptor=descriptor,
-            precipitation=precipitation,
-            obscuration=obscuration,
-            other=other,
+            phenomena=phenomena,
         )
 
 
 @dataclass_json
 @dataclass
 class Clouds:
     """
```

### Comparing `metafora-1.0.2/metafora/enums.py` & `metafora-1.1.0/metafora/enums.py`

 * *Files identical despite different names*

### Comparing `metafora-1.0.2/metafora/metar.py` & `metafora-1.1.0/metafora/metar.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding: utf-8
 """
 metafora - metar
 """
 import re
 from dataclasses import field, dataclass
 from dataclasses_json import dataclass_json, config
-from typing import List, Optional, Tuple
+from typing import List, Optional
 import warnings
 
 warnings.filterwarnings(action="ignore", category=UserWarning)
 
 from metafora.common import (
     Station,
     Timestamp,
@@ -254,10 +254,7 @@
                     compass = convert_direction(int(r.runway[:2]))
             elif r.distance_max is not None:
                 if distance is None or r.distance_max > distance:
                     distance = r.distance_max
                     compass = convert_direction(int(r.runway[:2]))
                 
     return RunwayVisualRange(runway=compass, distance=distance)
-
-
-
```

### Comparing `metafora-1.0.2/metafora/ml.py` & `metafora-1.1.0/metafora/ml.py`

 * *Files identical despite different names*

### Comparing `metafora-1.0.2/metafora/parser.py` & `metafora-1.1.0/metafora/parser.py`

 * *Files identical despite different names*

### Comparing `metafora-1.0.2/metafora/taf.py` & `metafora-1.1.0/metafora/taf.py`

 * *Files identical despite different names*

### Comparing `metafora-1.0.2/metafora/utils.py` & `metafora-1.1.0/metafora/utils.py`

 * *Files identical despite different names*

### Comparing `metafora-1.0.2/setup.py` & `metafora-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(name='metafora',
-      version="1.0.2",
+      version="1.1.0",
       description='METAR and TAF parser with dataclasses and regular expressions',
       author='Ramon Dalmau-Codina',
       author_email='ramon.dalmau.codina@gmail.com',
       url='https://github.com/ramondalmau/metafora.git',
       packages=["metafora"],
       python_requires='>=3.7',
       install_requires=[
```

