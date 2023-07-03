# Comparing `tmp/gaitalytics-0.1.2b0.tar.gz` & `tmp/gaitalytics-0.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitalytics-0.1.2b0.tar", last modified: Mon Jul  3 07:46:49 2023, max compression
+gzip compressed data, was "gaitalytics-0.1.3b0.tar", last modified: Mon Jul  3 08:11:01 2023, max compression
```

## Comparing `gaitalytics-0.1.2b0.tar` & `gaitalytics-0.1.3b0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 07:46:49.463152 gaitalytics-0.1.2b0/
--rw-rw-rw-   0        0        0     1096 2023-04-25 17:34:59.000000 gaitalytics-0.1.2b0/LICENSE
--rw-rw-rw-   0        0        0     7033 2023-07-03 07:46:49.463152 gaitalytics-0.1.2b0/PKG-INFO
--rw-rw-rw-   0        0        0     6509 2023-07-01 10:26:24.000000 gaitalytics-0.1.2b0/README.md
--rw-rw-rw-   0        0        0       84 2023-06-21 07:51:06.000000 gaitalytics-0.1.2b0/pyproject.toml
--rw-rw-rw-   0        0        0      728 2023-07-03 07:46:49.463152 gaitalytics-0.1.2b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 07:46:49.415520 gaitalytics-0.1.2b0/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 07:46:49.456203 gaitalytics-0.1.2b0/src/gaitalytics/
--rw-rw-rw-   0        0        0        0 2023-06-21 08:57:09.000000 gaitalytics-0.1.2b0/src/gaitalytics/__init__.py
--rw-rw-rw-   0        0        0    27232 2023-07-01 08:08:36.000000 gaitalytics-0.1.2b0/src/gaitalytics/analysis.py
--rw-rw-rw-   0        0        0    14608 2023-07-01 11:36:32.000000 gaitalytics-0.1.2b0/src/gaitalytics/api.py
--rw-rw-rw-   0        0        0     3226 2023-06-28 07:52:44.000000 gaitalytics-0.1.2b0/src/gaitalytics/c3d.py
--rw-rw-rw-   0        0        0    13160 2023-07-01 08:19:58.000000 gaitalytics-0.1.2b0/src/gaitalytics/cycle.py
--rw-rw-rw-   0        0        0     3340 2023-06-20 15:51:04.000000 gaitalytics-0.1.2b0/src/gaitalytics/emg.py
--rw-rw-rw-   0        0        0    15989 2023-06-28 13:09:43.000000 gaitalytics-0.1.2b0/src/gaitalytics/events.py
--rw-rw-rw-   0        0        0     8635 2023-07-03 07:45:20.000000 gaitalytics-0.1.2b0/src/gaitalytics/modelling.py
--rw-rw-rw-   0        0        0     6139 2023-07-01 08:19:58.000000 gaitalytics-0.1.2b0/src/gaitalytics/plot.py
--rw-rw-rw-   0        0        0    14514 2023-07-01 08:19:58.000000 gaitalytics-0.1.2b0/src/gaitalytics/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 07:46:49.463152 gaitalytics-0.1.2b0/src/gaitalytics.egg-info/
--rw-rw-rw-   0        0        0     7033 2023-07-03 07:46:49.000000 gaitalytics-0.1.2b0/src/gaitalytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-07-03 07:46:49.000000 gaitalytics-0.1.2b0/src/gaitalytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 07:46:49.000000 gaitalytics-0.1.2b0/src/gaitalytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-03 07:46:49.000000 gaitalytics-0.1.2b0/src/gaitalytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-03 07:46:49.000000 gaitalytics-0.1.2b0/src/gaitalytics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 08:11:01.782161 gaitalytics-0.1.3b0/
+-rw-rw-rw-   0        0        0     1096 2023-04-25 17:34:59.000000 gaitalytics-0.1.3b0/LICENSE
+-rw-rw-rw-   0        0        0     7033 2023-07-03 08:11:01.782161 gaitalytics-0.1.3b0/PKG-INFO
+-rw-rw-rw-   0        0        0     6509 2023-07-01 10:26:24.000000 gaitalytics-0.1.3b0/README.md
+-rw-rw-rw-   0        0        0       84 2023-06-21 07:51:06.000000 gaitalytics-0.1.3b0/pyproject.toml
+-rw-rw-rw-   0        0        0      728 2023-07-03 08:11:01.782161 gaitalytics-0.1.3b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 08:11:01.735602 gaitalytics-0.1.3b0/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 08:11:01.767217 gaitalytics-0.1.3b0/src/gaitalytics/
+-rw-rw-rw-   0        0        0        0 2023-06-21 08:57:09.000000 gaitalytics-0.1.3b0/src/gaitalytics/__init__.py
+-rw-rw-rw-   0        0        0    27232 2023-07-01 08:08:36.000000 gaitalytics-0.1.3b0/src/gaitalytics/analysis.py
+-rw-rw-rw-   0        0        0    14608 2023-07-01 11:36:32.000000 gaitalytics-0.1.3b0/src/gaitalytics/api.py
+-rw-rw-rw-   0        0        0     3226 2023-06-28 07:52:44.000000 gaitalytics-0.1.3b0/src/gaitalytics/c3d.py
+-rw-rw-rw-   0        0        0    13160 2023-07-01 08:19:58.000000 gaitalytics-0.1.3b0/src/gaitalytics/cycle.py
+-rw-rw-rw-   0        0        0     3340 2023-06-20 15:51:04.000000 gaitalytics-0.1.3b0/src/gaitalytics/emg.py
+-rw-rw-rw-   0        0        0    15989 2023-06-28 13:09:43.000000 gaitalytics-0.1.3b0/src/gaitalytics/events.py
+-rw-rw-rw-   0        0        0     8634 2023-07-03 08:09:26.000000 gaitalytics-0.1.3b0/src/gaitalytics/modelling.py
+-rw-rw-rw-   0        0        0     6139 2023-07-01 08:19:58.000000 gaitalytics-0.1.3b0/src/gaitalytics/plot.py
+-rw-rw-rw-   0        0        0    14514 2023-07-01 08:19:58.000000 gaitalytics-0.1.3b0/src/gaitalytics/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:11:01.778033 gaitalytics-0.1.3b0/src/gaitalytics.egg-info/
+-rw-rw-rw-   0        0        0     7033 2023-07-03 08:11:01.000000 gaitalytics-0.1.3b0/src/gaitalytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-07-03 08:11:01.000000 gaitalytics-0.1.3b0/src/gaitalytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 08:11:01.000000 gaitalytics-0.1.3b0/src/gaitalytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-03 08:11:01.000000 gaitalytics-0.1.3b0/src/gaitalytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-03 08:11:01.000000 gaitalytics-0.1.3b0/src/gaitalytics.egg-info/top_level.txt
```

### Comparing `gaitalytics-0.1.2b0/LICENSE` & `gaitalytics-0.1.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.2b0/PKG-INFO` & `gaitalytics-0.1.3b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitalytics
-Version: 0.1.2b0
+Version: 0.1.3b0
 Summary: Library to analyse gait data captured with a mocap system
 Home-page: https://github.com/cereneo-foundation/gaitalytics
 Author: André Böni
 Author-email: andre.boeni@cereneo.foundation
 License: MIT
 Keywords: gait,analysis,c3d,mocap
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gaitalytics-0.1.2b0/README.md` & `gaitalytics-0.1.3b0/README.md`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.2b0/setup.cfg` & `gaitalytics-0.1.3b0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6169 7461 6c79 7469 6373 0d0a   = gaitalytics..
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 3262  version = 0.1.2b
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 3362  version = 0.1.3b
 00000030: 6574 610d 0a61 7574 686f 7220 3d20 416e  eta..author = An
 00000040: 6472 c3a9 2042 c3b6 6e69 0d0a 6175 7468  dr.. B..ni..auth
 00000050: 6f72 5f65 6d61 696c 203d 2061 6e64 7265  or_email = andre
 00000060: 2e62 6f65 6e69 4063 6572 656e 656f 2e66  .boeni@cereneo.f
 00000070: 6f75 6e64 6174 696f 6e0d 0a75 726c 203d  oundation..url =
 00000080: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000090: 636f 6d2f 6365 7265 6e65 6f2d 666f 756e  com/cereneo-foun
```

### Comparing `gaitalytics-0.1.2b0/src/gaitalytics/analysis.py` & `gaitalytics-0.1.3b0/src/gaitalytics/analysis.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.2b0/src/gaitalytics/api.py` & `gaitalytics-0.1.3b0/src/gaitalytics/api.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.2b0/src/gaitalytics/c3d.py` & `gaitalytics-0.1.3b0/src/gaitalytics/c3d.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.2b0/src/gaitalytics/cycle.py` & `gaitalytics-0.1.3b0/src/gaitalytics/cycle.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.2b0/src/gaitalytics/emg.py` & `gaitalytics-0.1.3b0/src/gaitalytics/emg.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.2b0/src/gaitalytics/events.py` & `gaitalytics-0.1.3b0/src/gaitalytics/events.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.2b0/src/gaitalytics/modelling.py` & `gaitalytics-0.1.3b0/src/gaitalytics/modelling.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class BaseOutputModeller(ABC):
 
     def __init__(self, label: str, point_type: gaitalytics.utils.PointDataType):
         self._label = label
         self._type = point_type
 
     def create_point(self, acq: btkAcquisition, **kwargs):
-        result = self._calculate_point(acq , **kwargs)
+        result = self._calculate_point(acq, **kwargs)
         point = btkPoint(self._type.value)
         point.SetValues(result)
         point.SetLabel(self._label)
         acq.AppendPoint(point)
 
     @abstractmethod
     def _calculate_point(self, acq: btkAcquisition, **kwargs) -> np.ndarray:
```

### Comparing `gaitalytics-0.1.2b0/src/gaitalytics/plot.py` & `gaitalytics-0.1.3b0/src/gaitalytics/plot.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.2b0/src/gaitalytics/utils.py` & `gaitalytics-0.1.3b0/src/gaitalytics/utils.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.2b0/src/gaitalytics.egg-info/PKG-INFO` & `gaitalytics-0.1.3b0/src/gaitalytics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitalytics
-Version: 0.1.2b0
+Version: 0.1.3b0
 Summary: Library to analyse gait data captured with a mocap system
 Home-page: https://github.com/cereneo-foundation/gaitalytics
 Author: André Böni
 Author-email: andre.boeni@cereneo.foundation
 License: MIT
 Keywords: gait,analysis,c3d,mocap
 Classifier: Programming Language :: Python :: 3
```

