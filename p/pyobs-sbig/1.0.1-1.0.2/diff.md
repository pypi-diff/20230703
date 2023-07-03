# Comparing `tmp/pyobs_sbig-1.0.1.tar.gz` & `tmp/pyobs_sbig-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_sbig-1.0.1.tar", max compression
+gzip compressed data, was "pyobs_sbig-1.0.2.tar", max compression
```

## Comparing `pyobs_sbig-1.0.1.tar` & `pyobs_sbig-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1099 2023-03-22 08:12:32.652808 pyobs_sbig-1.0.1/LICENSE
--rw-r--r--   0        0        0     1219 2023-03-22 08:12:32.652808 pyobs_sbig-1.0.1/build.py
--rw-r--r--   0        0        0      121 2023-03-22 08:12:32.652808 pyobs_sbig-1.0.1/pyobs_sbig/__init__.py
--rw-r--r--   0        0        0     1592 2023-03-22 08:12:32.652808 pyobs_sbig-1.0.1/pyobs_sbig/sbig6303e.py
--rw-r--r--   0        0        0    10011 2023-03-22 08:12:32.652808 pyobs_sbig-1.0.1/pyobs_sbig/sbigcamera.py
--rw-r--r--   0        0        0     7661 2023-03-22 08:12:32.652808 pyobs_sbig-1.0.1/pyobs_sbig/sbigfiltercamera.py
--rw-r--r--   0        0        0     9399 2023-03-22 08:12:32.652808 pyobs_sbig-1.0.1/pyobs_sbig/sbigudrv.pxd
--rw-r--r--   0        0        0    11096 2023-03-22 08:12:32.652808 pyobs_sbig-1.0.1/pyobs_sbig/sbigudrv.pyx
--rw-r--r--   0        0        0      715 2023-03-22 08:12:32.652808 pyobs_sbig-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    46914 2023-03-22 08:12:32.652808 pyobs_sbig-1.0.1/src/csbigcam.cpp
--rw-r--r--   0        0        0     6041 2023-03-22 08:12:32.652808 pyobs_sbig-1.0.1/src/csbigcam.h
--rw-r--r--   0        0        0    60914 2023-03-22 08:12:32.656808 pyobs_sbig-1.0.1/src/csbigimg.cpp
--rw-r--r--   0        0        0    10777 2023-03-22 08:12:32.656808 pyobs_sbig-1.0.1/src/csbigimg.h
--rw-r--r--   0        0        0      850 2023-03-22 08:12:32.656808 pyobs_sbig-1.0.1/src/lpardrv.h
--rw-r--r--   0        0        0    28066 2023-03-22 08:12:32.656808 pyobs_sbig-1.0.1/src/sbigudrv.h
--rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 pyobs_sbig-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1219 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/build.py
+-rw-r--r--   0        0        0      121 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/pyobs_sbig/__init__.py
+-rw-r--r--   0        0        0     1592 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/pyobs_sbig/sbig6303e.py
+-rw-r--r--   0        0        0    10011 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/pyobs_sbig/sbigcamera.py
+-rw-r--r--   0        0        0     7661 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/pyobs_sbig/sbigfiltercamera.py
+-rw-r--r--   0        0        0     9399 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/pyobs_sbig/sbigudrv.pxd
+-rw-r--r--   0        0        0    11096 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/pyobs_sbig/sbigudrv.pyx
+-rw-r--r--   0        0        0      715 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    46914 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/src/csbigcam.cpp
+-rw-r--r--   0        0        0     6041 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/src/csbigcam.h
+-rw-r--r--   0        0        0    60914 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/src/csbigimg.cpp
+-rw-r--r--   0        0        0    10777 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/src/csbigimg.h
+-rw-r--r--   0        0        0      850 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/src/lpardrv.h
+-rw-r--r--   0        0        0    28066 2023-07-03 09:52:24.994693 pyobs_sbig-1.0.2/src/sbigudrv.h
+-rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 pyobs_sbig-1.0.2/PKG-INFO
```

### Comparing `pyobs_sbig-1.0.1/LICENSE` & `pyobs_sbig-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.1/build.py` & `pyobs_sbig-1.0.2/build.py`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.1/pyobs_sbig/sbig6303e.py` & `pyobs_sbig-1.0.2/pyobs_sbig/sbig6303e.py`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.1/pyobs_sbig/sbigcamera.py` & `pyobs_sbig-1.0.2/pyobs_sbig/sbigcamera.py`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.1/pyobs_sbig/sbigfiltercamera.py` & `pyobs_sbig-1.0.2/pyobs_sbig/sbigfiltercamera.py`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.1/pyobs_sbig/sbigudrv.pxd` & `pyobs_sbig-1.0.2/pyobs_sbig/sbigudrv.pxd`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.1/pyobs_sbig/sbigudrv.pyx` & `pyobs_sbig-1.0.2/pyobs_sbig/sbigudrv.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 np.import_array()
 
 from .sbigudrv cimport *
 
 
 @contextmanager
 def acquire_lock(lock):
-    if not lock.acquire(timeout=1):
+    if not lock.acquire(timeout=5):
         raise ValueError('Could not acquire exclusive lock on camera.')
     yield
     lock.release()
 
 
 class FilterWheelModel(Enum):
     UNKNOWN = CFW_MODEL_SELECT.CFWSEL_UNKNOWN
```

### Comparing `pyobs_sbig-1.0.1/pyproject.toml` & `pyobs_sbig-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyobs-sbig"
-version = "1.0.1"
+version = "1.0.2"
 description = "pyobs module for SBIG cameras"
 authors = ["Tim-Oliver Husser <thusser@uni-goettingen.de>"]
 license = "MIT"
 include = ['src']
 #build = 'build.py'
 
 [tool.poetry.build]
```

### Comparing `pyobs_sbig-1.0.1/src/csbigcam.cpp` & `pyobs_sbig-1.0.2/src/csbigcam.cpp`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.1/src/csbigcam.h` & `pyobs_sbig-1.0.2/src/csbigcam.h`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.1/src/csbigimg.cpp` & `pyobs_sbig-1.0.2/src/csbigimg.cpp`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.1/src/csbigimg.h` & `pyobs_sbig-1.0.2/src/csbigimg.h`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.1/src/lpardrv.h` & `pyobs_sbig-1.0.2/src/lpardrv.h`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.1/src/sbigudrv.h` & `pyobs_sbig-1.0.2/src/sbigudrv.h`

 * *Files identical despite different names*

