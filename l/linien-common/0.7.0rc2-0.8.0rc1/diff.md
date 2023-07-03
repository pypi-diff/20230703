# Comparing `tmp/linien-common-0.7.0rc2.tar.gz` & `tmp/linien-common-0.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-common-0.7.0rc2.tar", last modified: Tue Mar 21 15:47:28 2023, max compression
+gzip compressed data, was "linien-common-0.8.0rc1.tar", last modified: Mon Jul  3 12:16:52 2023, max compression
```

## Comparing `linien-common-0.7.0rc2.tar` & `linien-common-0.8.0rc1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:28.289105 linien-common-0.7.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-21 15:47:28.289105 linien-common-0.7.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:28.289105 linien-common-0.7.0rc2/linien_common/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-21 15:47:14.000000 linien-common-0.7.0rc2/linien_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-03-21 15:47:14.000000 linien-common-0.7.0rc2/linien_common/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-21 15:47:14.000000 linien-common-0.7.0rc2/linien_common/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:28.289105 linien-common-0.7.0rc2/linien_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-21 15:47:28.000000 linien-common-0.7.0rc2/linien_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-21 15:47:28.000000 linien-common-0.7.0rc2/linien_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:47:28.000000 linien-common-0.7.0rc2/linien_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-21 15:47:28.000000 linien-common-0.7.0rc2/linien_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-21 15:47:28.000000 linien-common-0.7.0rc2/linien_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 15:47:28.289105 linien-common-0.7.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-21 15:47:14.000000 linien-common-0.7.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:16:52.296916 linien-common-0.8.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 12:16:52.296916 linien-common-0.8.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:16:52.296916 linien-common-0.8.0rc1/linien_common/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 12:16:37.000000 linien-common-0.8.0rc1/linien_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-07-03 12:16:37.000000 linien-common-0.8.0rc1/linien_common/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-03 12:16:37.000000 linien-common-0.8.0rc1/linien_common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-03 12:16:37.000000 linien-common-0.8.0rc1/linien_common/influxdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:16:52.296916 linien-common-0.8.0rc1/linien_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 12:16:52.000000 linien-common-0.8.0rc1/linien_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-03 12:16:52.000000 linien-common-0.8.0rc1/linien_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:16:52.000000 linien-common-0.8.0rc1/linien_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 12:16:52.000000 linien-common-0.8.0rc1/linien_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 12:16:52.000000 linien-common-0.8.0rc1/linien_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:16:52.296916 linien-common-0.8.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-03 12:16:37.000000 linien-common-0.8.0rc1/setup.py
```

### Comparing `linien-common-0.7.0rc2/PKG-INFO` & `linien-common-0.8.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 0.7.0rc2
+Version: 0.8.0rc1
 Summary: Shared components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-common-0.7.0rc2/linien_common/common.py` & `linien-common-0.8.0rc1/linien_common/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,16 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 
 """This file contains stuff that is required by the server as well as the client."""
 
-import hashlib
-import pickle
 from time import time
+from typing import Tuple
 
 import numpy as np
 from scipy.signal import correlate, resample
 
 MHz = 0x10000000 / 8
 Vpp = ((1 << 14) - 1) / 4
 # conversion of bits to V
@@ -34,15 +33,14 @@
 HIGH_PASS_FILTER = 1
 
 FAST_OUT1 = 0
 FAST_OUT2 = 1
 ANALOG_OUT0 = 2
 
 DECIMATION = 8
-assert DECIMATION % 2 == 0 or DECIMATION == 1
 MAX_N_POINTS = 16384
 N_POINTS = int(MAX_N_POINTS / DECIMATION)
 
 AUTOLOCK_MAX_N_INSTRUCTIONS = 32
 
 AUTO_DETECT_AUTOLOCK_MODE = 0
 ROBUST_AUTOLOCK = 1
@@ -247,15 +245,15 @@
         target_zoom,
         rolled_error_signal,
         line_width,
         peak_idxs,
     )
 
 
-def convert_channel_mixing_value(value):
+def convert_channel_mixing_value(value: int) -> Tuple[int, int]:
     if value <= 0:
         a_value = 128
         b_value = 128 + value
     else:
         a_value = 127 - value
         b_value = 128
 
@@ -274,46 +272,24 @@
             (a_factor * a + b_factor * b) >> chain_factor_width
             for a, b in zip(*error_signals)
         ]
 
     return np.array([v + combined_offset for v in signal])
 
 
-def check_plot_data(is_locked, plot_data):
+def check_plot_data(is_locked: bool, plot_data) -> bool:
     if is_locked:
         if "error_signal" not in plot_data or "control_signal" not in plot_data:
             return False
     else:
         if "error_signal_1" not in plot_data:
             return False
     return True
 
 
-def pack(value):
-    try:
-        return pickle.dumps(value)
-    except Exception:
-        # this happens when un-pickleable objects (e.g. functions) are assigned
-        # to a parameter. In this case, we don't pickle it but transfer a netref
-        # instead
-        return value
-
-
-def unpack(value):
-    try:
-        return pickle.loads(value)
-    except Exception:
-        return value
-
-
 def get_signal_strength_from_i_q(i, q):
     i = i.astype(np.int64)
     q = q.astype(np.int64)
     i_squared = i**2
     q_squared = q**2
     signal_strength = np.sqrt(i_squared + q_squared)
     return signal_strength
-
-
-def hash_username_and_password(username, password):
-    secret = hashlib.sha256((username + "/" + password).encode()).hexdigest()
-    return secret
```

### Comparing `linien-common-0.7.0rc2/linien_common.egg-info/PKG-INFO` & `linien-common-0.8.0rc1/linien_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 0.7.0rc2
+Version: 0.8.0rc1
 Summary: Shared components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-common-0.7.0rc2/setup.py` & `linien-common-0.8.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
 setup(
     name="linien-common",
-    version="0.7.0rc2",
+    version="0.8.0rc1",
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
     maintainer_email="leykauf@physik.hu-berlin.de",
     description="Shared components of the Linien spectroscopy lock application.",
     long_description="Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.",  # noqa: E501
     long_description_content_type="text/markdown",
@@ -32,12 +32,13 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.5",
     install_requires=[
+        "importlib_metadata>=2.1.3",
         "numpy>=1.11.0",
+        "rpyc>=4.0,<5.0",
         "scipy>=0.17.0",
-        "importlib_metadata>=2.1.3",
     ],
 )
```

