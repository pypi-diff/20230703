# Comparing `tmp/ctapipe_io_magic-0.5.1.tar.gz` & `tmp/ctapipe_io_magic-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctapipe_io_magic-0.5.1.tar", last modified: Thu May  4 09:02:18 2023, max compression
+gzip compressed data, was "ctapipe_io_magic-0.5.2.tar", last modified: Mon Jul  3 19:49:31 2023, max compression
```

## Comparing `ctapipe_io_magic-0.5.1.tar` & `ctapipe_io_magic-0.5.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-05-04 09:02:18.179339 ctapipe_io_magic-0.5.1/
--rw-r--r--   0 shari90   (1000) shari90   (1000)     1090 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.1/LICENSE
--rw-r--r--   0 shari90   (1000) shari90   (1000)      159 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.1/MANIFEST.in
--rw-r--r--   0 shari90   (1000) shari90   (1000)     6914 2023-05-04 09:02:18.179339 ctapipe_io_magic-0.5.1/PKG-INFO
--rw-r--r--   0 shari90   (1000) shari90   (1000)     6645 2023-05-04 08:57:20.000000 ctapipe_io_magic-0.5.1/README.md
-drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-05-04 09:02:18.179339 ctapipe_io_magic-0.5.1/ctapipe_io_magic/
--rw-r--r--   0 shari90   (1000) shari90   (1000)    74479 2023-05-04 07:53:54.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/__init__.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)      160 2023-05-04 09:02:18.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/_version.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)      420 2023-04-19 10:27:57.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/constants.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)     1069 2023-04-17 09:32:56.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/mars_datalevels.py
-drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-05-04 09:02:18.179339 ctapipe_io_magic-0.5.1/ctapipe_io_magic/resources/
--rw-r--r--   0 shari90   (1000) shari90   (1000)     7189 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/resources/MAGICCam.camgeom.fits.gz
-drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-05-04 09:02:18.179339 ctapipe_io_magic-0.5.1/ctapipe_io_magic/tests/
--rw-r--r--   0 shari90   (1000) shari90   (1000)    13436 2023-05-04 07:53:54.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/tests/test_magic_event_source.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)      193 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/tests/test_mars_datalevels.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)     2685 2023-05-04 07:53:54.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/tests/test_stage1.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)      106 2023-05-04 07:53:54.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/tests/test_version.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)      844 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/version.py
-drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-05-04 09:02:18.179339 ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/
--rw-r--r--   0 shari90   (1000) shari90   (1000)     6914 2023-05-04 09:02:18.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/PKG-INFO
--rw-r--r--   0 shari90   (1000) shari90   (1000)      774 2023-05-04 09:02:18.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/SOURCES.txt
--rw-r--r--   0 shari90   (1000) shari90   (1000)        1 2023-05-04 09:02:18.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/dependency_links.txt
--rw-r--r--   0 shari90   (1000) shari90   (1000)       66 2023-05-04 09:02:18.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/entry_points.txt
--rw-r--r--   0 shari90   (1000) shari90   (1000)      251 2023-05-04 09:02:18.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/requires.txt
--rw-r--r--   0 shari90   (1000) shari90   (1000)       17 2023-05-04 09:02:18.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/top_level.txt
--rw-r--r--   0 shari90   (1000) shari90   (1000)     2232 2023-04-28 12:47:55.000000 ctapipe_io_magic-0.5.1/download_test_data.sh
--rw-r--r--   0 shari90   (1000) shari90   (1000)      335 2023-05-04 07:53:54.000000 ctapipe_io_magic-0.5.1/environment.yml
--rw-r--r--   0 shari90   (1000) shari90   (1000)      123 2023-05-04 08:57:20.000000 ctapipe_io_magic-0.5.1/eventsource_subclasses.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)     1153 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.1/example_stage1_config.json
--rw-r--r--   0 shari90   (1000) shari90   (1000)      130 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.1/pyproject.toml
--rw-r--r--   0 shari90   (1000) shari90   (1000)      357 2023-05-04 09:02:18.189339 ctapipe_io_magic-0.5.1/setup.cfg
--rw-r--r--   0 shari90   (1000) shari90   (1000)      846 2023-05-04 07:53:54.000000 ctapipe_io_magic-0.5.1/setup.py
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-07-03 19:49:31.835818 ctapipe_io_magic-0.5.2/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     1090 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.2/LICENSE
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      159 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.2/MANIFEST.in
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     7904 2023-07-03 19:49:31.835818 ctapipe_io_magic-0.5.2/PKG-INFO
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     7059 2023-07-03 19:45:33.000000 ctapipe_io_magic-0.5.2/README.md
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-07-03 19:49:31.835818 ctapipe_io_magic-0.5.2/ctapipe_io_magic/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)    78966 2023-07-03 19:39:53.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic/__init__.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      160 2023-07-03 19:49:31.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic/_version.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      628 2023-07-03 19:39:53.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic/constants.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     1069 2023-04-17 09:32:56.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic/mars_datalevels.py
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-07-03 19:49:31.835818 ctapipe_io_magic-0.5.2/ctapipe_io_magic/resources/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     7189 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic/resources/MAGICCam.camgeom.fits.gz
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-07-03 19:49:31.835818 ctapipe_io_magic-0.5.2/ctapipe_io_magic/tests/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)    19055 2023-07-03 19:39:53.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic/tests/test_magic_event_source.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      193 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic/tests/test_mars_datalevels.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     2652 2023-07-03 19:39:53.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic/tests/test_stage1.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      106 2023-05-04 07:53:54.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic/tests/test_version.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      844 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic/version.py
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-07-03 19:49:31.835818 ctapipe_io_magic-0.5.2/ctapipe_io_magic.egg-info/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     7904 2023-07-03 19:49:31.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic.egg-info/PKG-INFO
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      813 2023-07-03 19:49:31.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic.egg-info/SOURCES.txt
+-rw-r--r--   0 shari90   (1000) shari90   (1000)        1 2023-07-03 19:49:31.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic.egg-info/dependency_links.txt
+-rw-r--r--   0 shari90   (1000) shari90   (1000)       66 2023-07-03 19:49:31.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic.egg-info/entry_points.txt
+-rw-r--r--   0 shari90   (1000) shari90   (1000)        1 2023-07-03 19:49:31.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic.egg-info/not-zip-safe
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      139 2023-07-03 19:49:31.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic.egg-info/requires.txt
+-rw-r--r--   0 shari90   (1000) shari90   (1000)       17 2023-07-03 19:49:31.000000 ctapipe_io_magic-0.5.2/ctapipe_io_magic.egg-info/top_level.txt
+-rwxr-xr-x   0 shari90   (1000) shari90   (1000)     2684 2023-07-03 19:39:53.000000 ctapipe_io_magic-0.5.2/download_test_data.sh
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      335 2023-05-05 13:06:18.000000 ctapipe_io_magic-0.5.2/environment.yml
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      123 2023-05-04 08:57:20.000000 ctapipe_io_magic-0.5.2/eventsource_subclasses.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     1153 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.2/example_stage1_config.json
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      200 2023-05-05 13:17:27.000000 ctapipe_io_magic-0.5.2/pyproject.toml
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     1387 2023-07-03 19:49:31.835818 ctapipe_io_magic-0.5.2/setup.cfg
+-rw-r--r--   0 shari90   (1000) shari90   (1000)       39 2023-05-05 13:17:27.000000 ctapipe_io_magic-0.5.2/setup.py
```

### Comparing `ctapipe_io_magic-0.5.1/LICENSE` & `ctapipe_io_magic-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctapipe_io_magic-0.5.1/PKG-INFO` & `ctapipe_io_magic-0.5.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 Metadata-Version: 2.1
 Name: ctapipe_io_magic
-Version: 0.5.1
+Version: 0.5.2
 Summary: ctapipe plugin for reading calibrated MAGIC files
-Home-page: https://github.com/cta-observatory/ctapipe_io_magic
 Author: Ievgen Vovk et al.
 Author-email: Ievgen.Vovk@mpp.mpg.de
 License: MIT
+Project-URL: Bug Tracker, https://github.com/cta-observatory/ctapipe_io_magic/issues
+Project-URL: Source Code, https://github.com/cta-observatory/ctapipe_io_magic
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: all
 Provides-Extra: tests
-Provides-Extra: docs
+Provides-Extra: dev
+Provides-Extra: all
 License-File: LICENSE
 
 ## *ctapipe* MAGIC event source
 
 EventSource plugin for *ctapipe*, needed to read the calibrated data of the MAGIC telescope system. It requires the [*ctapipe*](https://github.com/cta-observatory/ctapipe) (v0.19.0) and [*uproot*](https://github.com/scikit-hep/uproot4) (>=5) packages to run.
 
 #### Installation
@@ -30,14 +41,22 @@
 git clone https://github.com/cta-observatory/ctapipe_io_magic.git
 cd ctapipe_io_magic
 conda env create -n ctapipe-io_magic -f environment.yml
 conda activate ctapipe-io_magic
 pip install .
 ```
 
+#### Test Data
+
+To run the tests, a set of non-public files is needed. If you are a member of MAGIC, ask one of the project maintainers for the credentials and then run:
+
+```bash
+./download_test_data.sh
+```
+
 #### Usage
 
 ```python
 import ctapipe
 from ctapipe_io_magic import MAGICEventSource
 
 with MAGICEventSource(input_url=file_name) as event_source:
@@ -124,7 +143,8 @@
 -   v0.4.4: changed units of peak_time from time slices (as stored in MARS) to nanoseconds
 -   v0.4.5: fixed automatic tests, add possibility to choose between effective and nominal focal length
 -   v0.4.6: add support to read in data taken in mono mode (full for real data, partial for MCs). Fixed bug in recognition of mono/stereo or standard trigger/SumT data (added also for MC)
 -   v0.4.7: add full support to read in real and MC data taken in mono mode, and with SumT. Added treatment of unsuitable pixels for MC data. Added readout of true XMax value from MC data (usually not available, filled with 0 otherwise)
 -   v0.5.0: release compatible with ctapipe 0.17. Also, the equivalent focal length is set to the
     correct value used in MAGIC simulations (i.e. 16.97 meters)
 -   v0.5.1: release compatible with ctapipe 0.19
+-   v0.5.2: introduce capbility of reading data taken with the Hardware Stereo Trigger (HaST) between MAGIC and LST-1. Also, fixed bug when getting the time difference between events for mono data
```

### Comparing `ctapipe_io_magic-0.5.1/README.md` & `ctapipe_io_magic-0.5.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 git clone https://github.com/cta-observatory/ctapipe_io_magic.git
 cd ctapipe_io_magic
 conda env create -n ctapipe-io_magic -f environment.yml
 conda activate ctapipe-io_magic
 pip install .
 ```
 
+#### Test Data
+
+To run the tests, a set of non-public files is needed. If you are a member of MAGIC, ask one of the project maintainers for the credentials and then run:
+
+```bash
+./download_test_data.sh
+```
+
 #### Usage
 
 ```python
 import ctapipe
 from ctapipe_io_magic import MAGICEventSource
 
 with MAGICEventSource(input_url=file_name) as event_source:
@@ -110,7 +118,8 @@
 -   v0.4.4: changed units of peak_time from time slices (as stored in MARS) to nanoseconds
 -   v0.4.5: fixed automatic tests, add possibility to choose between effective and nominal focal length
 -   v0.4.6: add support to read in data taken in mono mode (full for real data, partial for MCs). Fixed bug in recognition of mono/stereo or standard trigger/SumT data (added also for MC)
 -   v0.4.7: add full support to read in real and MC data taken in mono mode, and with SumT. Added treatment of unsuitable pixels for MC data. Added readout of true XMax value from MC data (usually not available, filled with 0 otherwise)
 -   v0.5.0: release compatible with ctapipe 0.17. Also, the equivalent focal length is set to the
     correct value used in MAGIC simulations (i.e. 16.97 meters)
 -   v0.5.1: release compatible with ctapipe 0.19
+-   v0.5.2: introduce capbility of reading data taken with the Hardware Stereo Trigger (HaST) between MAGIC and LST-1. Also, fixed bug when getting the time difference between events for mono data
```

### Comparing `ctapipe_io_magic-0.5.1/ctapipe_io_magic/__init__.py` & `ctapipe_io_magic-0.5.2/ctapipe_io_magic/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 from .constants import (
     DATA_MONO_TRIGGER_PATTERN,
     MC_STEREO_AND_MONO_TRIGGER_PATTERN,
     MC_SUMT_TRIGGER_PATTERN,
     DATA_MONO_SUMT_TRIGGER_PATTERN,
     PEDESTAL_TRIGGER_PATTERN,
     DATA_STEREO_TRIGGER_PATTERN,
+    DATA_TOPOLOGICAL_TRIGGER,
+    DATA_MAGIC_LST_TRIGGER,
 )
 
 __all__ = ["MAGICEventSource", "MARSDataLevel", "__version__"]
 
 logger = logging.getLogger(__name__)
 
 degrees_per_hour = 15.0
@@ -70,14 +72,16 @@
 MAGIC_TO_CTA_EVENT_TYPE = {
     DATA_MONO_TRIGGER_PATTERN: EventType.SUBARRAY,
     MC_STEREO_AND_MONO_TRIGGER_PATTERN: EventType.SUBARRAY,
     MC_SUMT_TRIGGER_PATTERN: EventType.SUBARRAY,
     DATA_STEREO_TRIGGER_PATTERN: EventType.SUBARRAY,
     DATA_MONO_SUMT_TRIGGER_PATTERN: EventType.SUBARRAY,
     PEDESTAL_TRIGGER_PATTERN: EventType.SKY_PEDESTAL,
+    DATA_TOPOLOGICAL_TRIGGER: EventType.SUBARRAY,
+    DATA_MAGIC_LST_TRIGGER: EventType.SUBARRAY,
 }
 
 
 def load_camera_geometry():
     """Load camera geometry from bundled resources of this repo"""
     f = resource_filename("ctapipe_io_magic", "resources/MAGICCam.camgeom.fits.gz")
     Provenance().add_input_file(f, role="CameraGeometry")
@@ -204,15 +208,15 @@
 
         # Retrieving the data level (so far HARDCODED Sorcerer)
         self.datalevel = DataLevel.DL0
 
         if self.is_simulation:
             self._simulation_config = self.parse_simulation_header()
 
-        self.is_stereo, self.is_sumt = self.parse_data_info()
+        self.is_stereo, self.is_sumt, self.is_hast = self.parse_data_info()
 
         if self.is_simulation and self.use_mc_mono_events and not self.is_stereo:
             logger.warning(
                 "Processing mono simulation data with"
                 " use_mc_mono_events=True. use_mc_mono_events will be ignored."
             )
 
@@ -511,19 +515,21 @@
             True if stereo data, False if mono
         is_sumt: Bool
             True if SUMT data, False if std trigger
         """
 
         is_stereo = []
         is_sumt = []
+        is_hast = []
 
         if not self.is_simulation:
             prescaler_mono_nosumt = [1, 1, 0, 1, 0, 0, 0, 0]
             prescaler_mono_sumt = [0, 1, 0, 1, 0, 1, 0, 0]
             prescaler_stereo = [0, 1, 0, 1, 0, 0, 0, 1]
+            prescaler_hast = [0, 1, 1, 1, 0, 0, 0, 1]
 
             # L1_table_mono = "L1_4NN"
             # L1_table_stereo = "L1_3NN"
 
             L3_table_nosumt = "L3T_L1L1_100_SYNC"
             L3_table_sumt = "L3T_SUMSUM_100_SYNC"
 
@@ -539,31 +545,38 @@
                     ].array(library="np")
                 except AssertionError:
                     logger.warning(
                         "No prescaler info found. Will assume standard stereo data."
                     )
                     stereo = True
                     sumt = False
-                    return stereo, sumt
+                    hast = False
+                    return stereo, sumt, hast
 
                 prescaler_size = prescaler_array.size
                 if prescaler_size > 1:
                     prescaler = list(prescaler_array[1])
                 else:
                     prescaler = list(prescaler_array[0])
 
                 if (
                     prescaler == prescaler_mono_nosumt
                     or prescaler == prescaler_mono_sumt
                 ):
                     stereo = False
+                    hast = False
                 elif prescaler == prescaler_stereo:
                     stereo = True
+                    hast = False
+                elif prescaler == prescaler_hast:
+                    stereo = True
+                    hast = True
                 else:
                     stereo = True
+                    hast = False
 
                 sumt = False
                 if stereo:
                     # here we take the 2nd element for the same reason as above
                     # L3Table is empty for mono data i.e. taken with one telescope only
                     # if both telescopes take data with no L3, L3Table is filled anyway
                     L3Table_array = L3T_tree["MReportL3T.fTablename"].array(
@@ -583,14 +596,15 @@
                         sumt = False
                 else:
                     if prescaler == prescaler_mono_sumt:
                         sumt = True
 
                 is_stereo.append(stereo)
                 is_sumt.append(sumt)
+                is_hast.append(hast)
 
         else:
             for rootf in self.files_:
                 # looking into MC data, when SumT is simulated, trigger pattern of all events is set to 32 (bit 5), except the first (set to 0)
                 trigger_pattern_array_unique = np.unique(
                     rootf["Events"]["MTriggerPattern.fPrescaled"].array(library="np")[
                         1:
@@ -611,31 +625,39 @@
                 ].array(library="np")[0]
                 if num_telescopes == 1:
                     stereo = False
                 else:
                     stereo = True
 
                 is_stereo.append(stereo)
+                is_hast.append(False)
 
         is_stereo = np.unique(is_stereo).tolist()
         is_sumt = np.unique(is_sumt).tolist()
+        is_hast = np.unique(is_hast).tolist()
 
         if len(is_stereo) > 1:
             raise ValueError(
                 "Loaded files contain both stereo and mono data. \
                  Please load only stereo or mono."
             )
 
         if len(is_sumt) > 1:
             logger.warning(
                 "Found data with both standard and Sum trigger. While this is \
                 not an issue, check that this is what you really want to do."
             )
 
-        return is_stereo[0], is_sumt[0]
+        if len(is_hast) > 1:
+            logger.warning(
+                "Found data with both stereo and hardware stereo trigger. While this is \
+                not an issue, check that this is what you really want to do."
+            )
+
+        return is_stereo[0], is_sumt[0], is_hast[0]
 
     def prepare_subarray_info(self):
         """
         Fill SubarrayDescription container
 
         Returns
         -------
@@ -1081,18 +1103,35 @@
         -------
         time_diffs: astropy.units.quantity.Quantity
             Trigger time differences of consecutive events
         """
 
         time_diffs = np.array([])
 
+        data_trigger_pattern = DATA_STEREO_TRIGGER_PATTERN
+        if not self.is_stereo:
+            if self.is_sumt:
+                data_trigger_pattern = DATA_MONO_SUMT_TRIGGER_PATTERN
+            else:
+                data_trigger_pattern = DATA_MONO_TRIGGER_PATTERN
+        if self.is_hast:
+            event_cut = (
+                f"(MTriggerPattern.fPrescaled == {data_trigger_pattern})"
+            f" | (MTriggerPattern.fPrescaled == {DATA_TOPOLOGICAL_TRIGGER})"
+            f" | (MTriggerPattern.fPrescaled == {DATA_MAGIC_LST_TRIGGER})"
+            )
+        else:
+            event_cut = (
+                f"(MTriggerPattern.fPrescaled == {data_trigger_pattern})",
+            )
+
         for uproot_file in self.files_:
             event_info = uproot_file["Events"].arrays(
                 expressions=["MRawEvtHeader.fTimeDiff"],
-                cut=f"(MTriggerPattern.fPrescaled == {DATA_STEREO_TRIGGER_PATTERN})",
+                cut=event_cut,
                 library="np",
             )
 
             time_diffs = np.append(time_diffs, event_info["MRawEvtHeader.fTimeDiff"])
 
         time_diffs *= u.s
 
@@ -1122,15 +1161,15 @@
     def datalevels(self):
         return (self.datalevel,)
 
     @property
     def obs_ids(self):
         # ToCheck: will this be compatible in the future, e.g. with merged MC files
         return list(self.observation_blocks)
-        
+
     def _get_badrmspixel_mask(self, event):
         """
         Fetch bad RMS pixel mask for a given event.
 
         Parameters
         ----------
         event: ctapipe.containers.ArrayEventContainer
@@ -1235,14 +1274,15 @@
         run["input_file"] = uproot_file.file_path
 
         if self.mars_datalevel == MARSDataLevel.CALIBRATED:
             run["data"] = MarsCalibratedRun(
                 uproot_file,
                 self.is_simulation,
                 self.is_stereo,
+                self.is_hast,
                 self.use_mc_mono_events,
                 self.is_sumt,
             )
 
         return run
 
     def _generator(self):
@@ -1273,15 +1313,14 @@
         event = ArrayEventContainer()
 
         event.meta["origin"] = "MAGIC"
         event.meta["max_events"] = self.max_events
         event.index.obs_id = self.obs_ids[0]
 
         tel_id = self.telescope
-        event.trigger.tels_with_trigger = np.array([tel_id])
 
         counter = 0
 
         # Read the input files subrun-wise:
         for uproot_file in self.files_:
             event.meta["input_file"] = uproot_file.file_path
 
@@ -1376,14 +1415,47 @@
                 event_data["pointing_alt"] = u.Quantity(90 - pointing_zd, u.deg)
                 event_data["pointing_ra"] = u.Quantity(pointing_ra, u.deg)
                 event_data["pointing_dec"] = u.Quantity(pointing_dec, u.deg)
 
             # Loop over the events:
             for i_event in range(n_events):
                 event.count = counter
+
+                if not self.is_simulation:
+                    if (
+                        event_data["trigger_pattern"][i_event]
+                        == DATA_STEREO_TRIGGER_PATTERN
+                    ):
+                        event.trigger.tels_with_trigger = [1, 2]
+                    elif (
+                        event_data["trigger_pattern"][i_event]
+                        == DATA_TOPOLOGICAL_TRIGGER
+                    ):
+                        event.trigger.tels_with_trigger = [tel_id, 3]
+                    elif (
+                        event_data["trigger_pattern"][i_event] == DATA_MAGIC_LST_TRIGGER
+                    ):
+                        event.trigger.tels_with_trigger = [1, 2, 3]
+                    else:
+                        event.trigger.tels_with_trigger = [tel_id]
+                else:
+                    if self.is_stereo and not self.use_mc_mono_events:
+                        event.trigger.tels_with_trigger = [1, 2]
+                    else:
+                        event.trigger.tels_with_trigger = [tel_id]
+
+                if self.allowed_tels:
+                    tels_with_trigger = np.intersect1d(
+                        event.trigger.tels_with_trigger,
+                        self.subarray.tel_ids,
+                        assume_unique=True,
+                    )
+
+                    event.trigger.tels_with_trigger = tels_with_trigger.tolist()
+
                 event.index.event_id = event_data["event_number"][i_event]
 
                 event.trigger.event_type = MAGIC_TO_CTA_EVENT_TYPE.get(
                     event_data["trigger_pattern"][i_event]
                 )
 
                 if not self.is_simulation:
@@ -1485,14 +1557,15 @@
     """
 
     def __init__(
         self,
         uproot_file,
         is_mc,
         is_stereo,
+        is_hast,
         use_mc_mono_events,
         use_sumt_events,
         n_cam_pixels=1039,
     ):
         """
         Constructor of the class. Loads an input uproot file
         and store the informaiton to constructor variables.
@@ -1511,14 +1584,15 @@
 
         self.uproot_file = uproot_file
         self.is_mc = is_mc
         self.is_stereo = is_stereo
         self.use_mc_mono_events = use_mc_mono_events
         self.use_sumt_events = use_sumt_events
         self.n_cam_pixels = n_cam_pixels
+        self.is_hast = is_hast
 
         # Load the input data:
         calib_data = self._load_data()
 
         self.cosmic_events = calib_data["cosmic_events"]
         self.pedestal_events = calib_data["pedestal_events"]
         self.monitoring_data = calib_data["monitoring_data"]
@@ -1623,17 +1697,24 @@
         else:
             data_trigger_pattern = DATA_STEREO_TRIGGER_PATTERN
             if not self.is_stereo:
                 if self.use_sumt_events:
                     data_trigger_pattern = DATA_MONO_SUMT_TRIGGER_PATTERN
                 else:
                     data_trigger_pattern = DATA_MONO_TRIGGER_PATTERN
-            events_cut[
-                "cosmic_events"
-            ] = f"(MTriggerPattern.fPrescaled == {data_trigger_pattern})"
+            if self.is_hast:
+                events_cut["cosmic_events"] = (
+                    f"(MTriggerPattern.fPrescaled == {data_trigger_pattern})"
+                    f" | (MTriggerPattern.fPrescaled == {DATA_TOPOLOGICAL_TRIGGER})"
+                    f" | (MTriggerPattern.fPrescaled == {DATA_MAGIC_LST_TRIGGER})"
+                )
+            else:
+                events_cut[
+                    "cosmic_events"
+                ] = f"(MTriggerPattern.fPrescaled == {data_trigger_pattern})"
             # Only for cosmic events because MC data do not have pedestal events:
             events_cut[
                 "pedestal_events"
             ] = f"(MTriggerPattern.fPrescaled == {PEDESTAL_TRIGGER_PATTERN})"
 
         logger.info(f"Cosmic events selection: {events_cut['cosmic_events']}")
 
@@ -1682,18 +1763,37 @@
                         f"{subrun_id}{daq_id:05}"
                         for daq_id in common_info["MRawEvtHeader.fDAQEvtNumber"]
                     ],
                     dtype=int,
                 )
                 logger.info("Using fDAQEvtNumber to generate event IDs.")
             else:
-                calib_data[event_type]["event_number"] = np.array(
-                    common_info["MRawEvtHeader.fStereoEvtNumber"], dtype=int
-                )
-                logger.info("Using fStereoEvtNumber to generate event IDs.")
+                if self.is_hast:
+                    subrun_id = self.uproot_file["RunHeaders"][
+                        "MRawRunHeader.fSubRunIndex"
+                    ].array(library="np")[0]
+                    stereo_ids = common_info["MRawEvtHeader.fStereoEvtNumber"]
+                    daq_ids = common_info["MRawEvtHeader.fDAQEvtNumber"]
+                    calib_data[event_type]["event_number"] = np.array(
+                        [
+                            f"{subrun_id}{daq_ids[event_idx]:07}"
+                            if common_info["MTriggerPattern.fPrescaled"][event_idx]
+                            == DATA_TOPOLOGICAL_TRIGGER
+                            else stereo_ids[event_idx]
+                            for event_idx in range(
+                                common_info["MTriggerPattern.fPrescaled"].size
+                            )
+                        ],
+                        dtype=int,
+                    )
+                else:
+                    calib_data[event_type]["event_number"] = np.array(
+                        common_info["MRawEvtHeader.fStereoEvtNumber"], dtype=int
+                    )
+                    logger.info("Using fStereoEvtNumber to generate event IDs.")
 
             # Set pixel-wise charge and peak time information.
             # The length of the pixel array is 1183, but here only the first part of the pixel
             # information are extracted (i.e., for the current MAGIC camera geometry, the pixels
             # between 0 and 1039 are extracted, since the other part of pixels has only zeros):
             calib_data[event_type]["image"] = np.array(
                 common_info["MCerPhotEvt.fPixels.fPhot"].tolist()
@@ -1907,16 +2007,17 @@
             )
 
         if not self.is_mc:
             if self.is_stereo:
                 # Check for bit flips in the stereo event IDs:
                 uplim_total_jumps = 100
 
-                stereo_event_number = calib_data["cosmic_events"][
-                    "event_number"
+                stereo_event_number = calib_data["cosmic_events"]["event_number"][
+                    calib_data["cosmic_events"]["trigger_pattern"]
+                    == DATA_STEREO_TRIGGER_PATTERN
                 ].astype(int)
                 number_difference = np.diff(stereo_event_number)
 
                 indices_flip = np.where(number_difference < 0)[0]
                 n_flips = len(indices_flip)
 
                 if n_flips > 0:
```

### Comparing `ctapipe_io_magic-0.5.1/ctapipe_io_magic/mars_datalevels.py` & `ctapipe_io_magic-0.5.2/ctapipe_io_magic/mars_datalevels.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_magic-0.5.1/ctapipe_io_magic/resources/MAGICCam.camgeom.fits.gz` & `ctapipe_io_magic-0.5.2/ctapipe_io_magic/resources/MAGICCam.camgeom.fits.gz`

 * *Files identical despite different names*

### Comparing `ctapipe_io_magic-0.5.1/ctapipe_io_magic/tests/test_stage1.py` & `ctapipe_io_magic-0.5.2/ctapipe_io_magic/tests/test_stage1.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     ret = run_tool(
         tool,
         argv=[
             f"--input={test_cal_path}",
             f"--output={output}",
             f"--config={str(config)}",
             "--MAGICEventSource.process_run=false",
-            "--allowed-tels=1",
             "--camera-frame",
         ],
     )
     assert ret == 0
 
     parameters = read_table(output, "/dl1/event/telescope/parameters/tel_001")
     assert len(parameters) == 458
```

### Comparing `ctapipe_io_magic-0.5.1/ctapipe_io_magic/version.py` & `ctapipe_io_magic-0.5.2/ctapipe_io_magic/version.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/PKG-INFO` & `ctapipe_io_magic-0.5.2/ctapipe_io_magic.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 Metadata-Version: 2.1
 Name: ctapipe-io-magic
-Version: 0.5.1
+Version: 0.5.2
 Summary: ctapipe plugin for reading calibrated MAGIC files
-Home-page: https://github.com/cta-observatory/ctapipe_io_magic
 Author: Ievgen Vovk et al.
 Author-email: Ievgen.Vovk@mpp.mpg.de
 License: MIT
+Project-URL: Bug Tracker, https://github.com/cta-observatory/ctapipe_io_magic/issues
+Project-URL: Source Code, https://github.com/cta-observatory/ctapipe_io_magic
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: all
 Provides-Extra: tests
-Provides-Extra: docs
+Provides-Extra: dev
+Provides-Extra: all
 License-File: LICENSE
 
 ## *ctapipe* MAGIC event source
 
 EventSource plugin for *ctapipe*, needed to read the calibrated data of the MAGIC telescope system. It requires the [*ctapipe*](https://github.com/cta-observatory/ctapipe) (v0.19.0) and [*uproot*](https://github.com/scikit-hep/uproot4) (>=5) packages to run.
 
 #### Installation
@@ -30,14 +41,22 @@
 git clone https://github.com/cta-observatory/ctapipe_io_magic.git
 cd ctapipe_io_magic
 conda env create -n ctapipe-io_magic -f environment.yml
 conda activate ctapipe-io_magic
 pip install .
 ```
 
+#### Test Data
+
+To run the tests, a set of non-public files is needed. If you are a member of MAGIC, ask one of the project maintainers for the credentials and then run:
+
+```bash
+./download_test_data.sh
+```
+
 #### Usage
 
 ```python
 import ctapipe
 from ctapipe_io_magic import MAGICEventSource
 
 with MAGICEventSource(input_url=file_name) as event_source:
@@ -124,7 +143,8 @@
 -   v0.4.4: changed units of peak_time from time slices (as stored in MARS) to nanoseconds
 -   v0.4.5: fixed automatic tests, add possibility to choose between effective and nominal focal length
 -   v0.4.6: add support to read in data taken in mono mode (full for real data, partial for MCs). Fixed bug in recognition of mono/stereo or standard trigger/SumT data (added also for MC)
 -   v0.4.7: add full support to read in real and MC data taken in mono mode, and with SumT. Added treatment of unsuitable pixels for MC data. Added readout of true XMax value from MC data (usually not available, filled with 0 otherwise)
 -   v0.5.0: release compatible with ctapipe 0.17. Also, the equivalent focal length is set to the
     correct value used in MAGIC simulations (i.e. 16.97 meters)
 -   v0.5.1: release compatible with ctapipe 0.19
+-   v0.5.2: introduce capbility of reading data taken with the Hardware Stereo Trigger (HaST) between MAGIC and LST-1. Also, fixed bug when getting the time difference between events for mono data
```

### Comparing `ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/SOURCES.txt` & `ctapipe_io_magic-0.5.2/ctapipe_io_magic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ctapipe_io_magic/constants.py
 ctapipe_io_magic/mars_datalevels.py
 ctapipe_io_magic/version.py
 ctapipe_io_magic.egg-info/PKG-INFO
 ctapipe_io_magic.egg-info/SOURCES.txt
 ctapipe_io_magic.egg-info/dependency_links.txt
 ctapipe_io_magic.egg-info/entry_points.txt
+ctapipe_io_magic.egg-info/not-zip-safe
 ctapipe_io_magic.egg-info/requires.txt
 ctapipe_io_magic.egg-info/top_level.txt
 ctapipe_io_magic/resources/MAGICCam.camgeom.fits.gz
 ctapipe_io_magic/tests/test_magic_event_source.py
 ctapipe_io_magic/tests/test_mars_datalevels.py
 ctapipe_io_magic/tests/test_stage1.py
 ctapipe_io_magic/tests/test_version.py
```

### Comparing `ctapipe_io_magic-0.5.1/download_test_data.sh` & `ctapipe_io_magic-0.5.2/download_test_data.sh`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 #!/bin/bash
 
 set -e
 
-echo "https://webdav-magic.pic.es:8451/Users/ctapipe_io_magic/test_data/real/calibrated/20210314_M1_05095172.001_Y_CrabNebula-W0.40+035.root" >  test_data_real.txt
-echo "https://webdav-magic.pic.es:8451/Users/ctapipe_io_magic/test_data/real/calibrated/20210314_M1_05095172.002_Y_CrabNebula-W0.40+035.root" >> test_data_real.txt
-echo "https://webdav-magic.pic.es:8451/Users/ctapipe_io_magic/test_data/real/calibrated/20210314_M2_05095172.001_Y_CrabNebula-W0.40+035.root" >> test_data_real.txt
-echo "https://webdav-magic.pic.es:8451/Users/ctapipe_io_magic/test_data/real/calibrated/20210314_M2_05095172.002_Y_CrabNebula-W0.40+035.root" >> test_data_real.txt
+echo "https://www.magic.iac.es/mcp-testdata/test_data/real/calibrated/20210314_M1_05095172.001_Y_CrabNebula-W0.40+035.root" >  test_data_real.txt
+echo "https://www.magic.iac.es/mcp-testdata/test_data/real/calibrated/20210314_M1_05095172.002_Y_CrabNebula-W0.40+035.root" >> test_data_real.txt
+echo "https://www.magic.iac.es/mcp-testdata/test_data/real/calibrated/20210314_M2_05095172.001_Y_CrabNebula-W0.40+035.root" >> test_data_real.txt
+echo "https://www.magic.iac.es/mcp-testdata/test_data/real/calibrated/20210314_M2_05095172.002_Y_CrabNebula-W0.40+035.root" >> test_data_real.txt
+echo "https://www.magic.iac.es/mcp-testdata/test_data/real/calibrated/20230324_M1_05106879.001_Y_1ES0806+524-W0.40+000.root" >>  test_data_real.txt
+echo "https://www.magic.iac.es/mcp-testdata/test_data/real/calibrated/20230324_M1_05106879.002_Y_1ES0806+524-W0.40+000.root" >>  test_data_real.txt
+echo "https://www.magic.iac.es/mcp-testdata/test_data/real/calibrated/20230324_M2_05106879.001_Y_1ES0806+524-W0.40+000.root" >>  test_data_real.txt
+echo "https://www.magic.iac.es/mcp-testdata/test_data/real/calibrated/20230324_M2_05106879.002_Y_1ES0806+524-W0.40+000.root" >>  test_data_real.txt
 
-echo "https://webdav-magic.pic.es:8451/Users/ctapipe_io_magic/test_data/simulated/calibrated/GA_M1_za35to50_8_824318_Y_w0.root" >  test_data_simulated.txt
-echo "https://webdav-magic.pic.es:8451/Users/ctapipe_io_magic/test_data/simulated/calibrated/GA_M1_za35to50_8_824319_Y_w0.root" >> test_data_simulated.txt
-echo "https://webdav-magic.pic.es:8451/Users/ctapipe_io_magic/test_data/simulated/calibrated/GA_M2_za35to50_8_824318_Y_w0.root" >> test_data_simulated.txt
-echo "https://webdav-magic.pic.es:8451/Users/ctapipe_io_magic/test_data/simulated/calibrated/GA_M2_za35to50_8_824319_Y_w0.root" >> test_data_simulated.txt
+echo "https://www.magic.iac.es/mcp-testdata/test_data/simulated/calibrated/GA_M1_za35to50_8_824318_Y_w0.root" >  test_data_simulated.txt
+echo "https://www.magic.iac.es/mcp-testdata/test_data/simulated/calibrated/GA_M1_za35to50_8_824319_Y_w0.root" >> test_data_simulated.txt
+echo "https://www.magic.iac.es/mcp-testdata/test_data/simulated/calibrated/GA_M2_za35to50_8_824318_Y_w0.root" >> test_data_simulated.txt
+echo "https://www.magic.iac.es/mcp-testdata/test_data/simulated/calibrated/GA_M2_za35to50_8_824319_Y_w0.root" >> test_data_simulated.txt
 
 if [ -z "$TEST_DATA_USER" ]; then
     read -p "Username: " TEST_DATA_USER
     echo
 fi
 
 if [ -z "$TEST_DATA_PASSWORD" ]; then
```

### Comparing `ctapipe_io_magic-0.5.1/example_stage1_config.json` & `ctapipe_io_magic-0.5.2/example_stage1_config.json`

 * *Files identical despite different names*

