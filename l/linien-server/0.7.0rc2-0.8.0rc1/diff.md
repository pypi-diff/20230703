# Comparing `tmp/linien-server-0.7.0rc2.tar.gz` & `tmp/linien-server-0.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-server-0.7.0rc2.tar", last modified: Tue Mar 21 15:47:42 2023, max compression
+gzip compressed data, was "linien-server-0.8.0rc1.tar", last modified: Mon Jul  3 12:17:06 2023, max compression
```

## Comparing `linien-server-0.7.0rc2.tar` & `linien-server-0.8.0rc1.tar`

### file list

```diff
@@ -1,45 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:42.093094 linien-server-0.7.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-21 15:47:42.093094 linien-server-0.7.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:42.093094 linien-server-0.7.0rc2/linien_server/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/acquisition_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/approach_line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:42.093094 linien-server-0.7.0rc2/linien_server/autolock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/autolock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/autolock/algorithm_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/autolock/autolock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/autolock/fast.py
--rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/autolock/robust.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/autolock/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/csr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/csrmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/iir_coeffs.py
--rw-r--r--   0 runner    (1001) docker     (123)  2083740 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/linien.bin
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/linien_install_requirements.sh
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/linien_start_server.sh
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/linien_stop_server.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:42.093094 linien-server-0.7.0rc2/linien_server/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/optimization/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/optimization/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/optimization/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    21500 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/parameters_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:42.093094 linien-server-0.7.0rc2/linien_server/pid_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/pid_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/pid_optimization/pid_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15495 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/registers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/linien_server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:42.093094 linien-server-0.7.0rc2/linien_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-21 15:47:42.000000 linien-server-0.7.0rc2/linien_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-21 15:47:42.000000 linien-server-0.7.0rc2/linien_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:47:42.000000 linien-server-0.7.0rc2/linien_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-21 15:47:42.000000 linien-server-0.7.0rc2/linien_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-21 15:47:42.000000 linien-server-0.7.0rc2/linien_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-21 15:47:42.000000 linien-server-0.7.0rc2/linien_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 15:47:42.093094 linien-server-0.7.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-03-21 15:47:14.000000 linien-server-0.7.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:17:06.721103 linien-server-0.8.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 12:17:06.721103 linien-server-0.8.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:17:06.717103 linien-server-0.8.0rc1/linien_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/acquisition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:17:06.717103 linien-server-0.8.0rc1/linien_server/autolock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/autolock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/autolock/algorithm_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/autolock/autolock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/autolock/fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/autolock/robust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/autolock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/csr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/csrmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/iir_coeffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2083740 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/linien.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/linien_install_requirements.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/linien_start_server.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/linien_stop_server.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:17:06.721103 linien-server-0.8.0rc1/linien_server/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/optimization/approach_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/optimization/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/optimization/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/optimization/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29123 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:17:06.721103 linien-server-0.8.0rc1/linien_server/pid_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/pid_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/pid_optimization/pid_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15489 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/linien_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:17:06.717103 linien-server-0.8.0rc1/linien_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 12:17:06.000000 linien-server-0.8.0rc1/linien_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-03 12:17:06.000000 linien-server-0.8.0rc1/linien_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:17:06.000000 linien-server-0.8.0rc1/linien_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-03 12:17:06.000000 linien-server-0.8.0rc1/linien_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-03 12:17:06.000000 linien-server-0.8.0rc1/linien_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 12:17:06.000000 linien-server-0.8.0rc1/linien_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:17:06.721103 linien-server-0.8.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-03 12:16:37.000000 linien-server-0.8.0rc1/setup.py
```

### Comparing `linien-server-0.7.0rc2/PKG-INFO` & `linien-server-0.8.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-server
-Version: 0.7.0rc2
+Version: 0.8.0rc1
 Summary: Server components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-server-0.7.0rc2/linien_server/acquisition_process.py` & `linien-server-0.8.0rc1/linien_server/acquisition.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright 2018-2022 Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>
-# Copyright 2021-2022 Bastian Leykauf <leykauf@physik.hu-berlin.de>
+# Copyright 2021-2023 Bastian Leykauf <leykauf@physik.hu-berlin.de>
 #
 # This file is part of Linien and based on redpid.
 #
 # Linien is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,50 +12,49 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
-import _thread
-import os
 import pickle
-import threading
+import shutil
+import subprocess
+from pathlib import Path
 from random import random
+from threading import Event, Thread
 from time import sleep
+from typing import Any, Dict, Optional, Tuple, Union
 
 import numpy as np
 from linien_common.common import DECIMATION, MAX_N_POINTS, N_POINTS
 from linien_common.config import ACQUISITION_PORT
-from pyrp3.board import RedPitaya
+from linien_server.csr import PythonCSR
+from pyrp3.board import RedPitaya  # type: ignore
+from pyrp3.instrument import TriggerSource  # type: ignore
 from rpyc import Service
-from rpyc.utils.server import OneShotServer
+from rpyc.utils.server import ThreadedServer
 
-from .csr import PythonCSR
 
-
-def shutdown():
-    _thread.interrupt_main()
-    os._exit(0)
-
-
-class DataAcquisitionService(Service):
+class AcquisitionService(Service):
     def __init__(self):
+        super(AcquisitionService, self).__init__()
+        stop_nginx()
+        flash_fpga()
+
         self.red_pitaya = RedPitaya()
         self.csr = PythonCSR(self.red_pitaya)
         self.csr_queue = []
         self.csr_iir_queue = []
 
         self.data = pickle.dumps(None)
         self.data_was_raw = False
         self.data_hash = None
         self.data_uuid = None
 
-        super(DataAcquisitionService, self).__init__()
-
         self.locked = False
         self.exposed_set_sweep_speed(9)
         # when self.locked is set to True, this doesn't mean that the lock is really on.
         # It just means that the lock is requested and that the gateware waits until the
         # sweep is at the correct position for the lock. Therefore, when self.locked is
         # set, the acquisition process waits for confirmation from the gateware that the
         # lock is actually running.
@@ -63,220 +62,264 @@
 
         self.fetch_additional_signals = True
         self.raw_acquisition_enabled = False
         self.raw_acquisition_decimation = 0
 
         self.dual_channel = False
 
-        self.acquisition_paused = False
-        self.skip_next_data = False
-
-        self.run()
-
-    def run(self):
-        def run_acquiry_loop():
-            while True:
-                while self.csr_queue:
-                    key, value = self.csr_queue.pop(0)
-                    self.csr.set(key, value)
-
-                while self.csr_iir_queue:
-                    args = self.csr_iir_queue.pop(0)
-                    self.csr.set_iir(*args)
-
-                if self.locked and not self.confirmed_that_in_lock:
-                    self.confirmed_that_in_lock = self.csr.get(
-                        "logic_autolock_lock_running"
-                    )
-                    if not self.confirmed_that_in_lock:
-                        sleep(0.05)
-                        continue
+        self.stop_event = Event()
+        self.pause_event = Event()
+        self.skip_next_data_event = Event()
+
+        self.thread = Thread(
+            target=self._acquisition_loop,
+            args=(
+                self.stop_event,
+                self.pause_event,
+                self.skip_next_data_event,
+            ),
+            daemon=True,
+        )
+        self.thread.start()
 
-                if self.acquisition_paused:
+    def _acquisition_loop(
+        self, stop_event: Event, pause_event: Event, skip_next_data_event: Event
+    ) -> None:
+        while not stop_event.is_set():
+            while self.csr_queue:
+                key, value = self.csr_queue.pop(0)
+                self.csr.set(key, value)
+
+            while self.csr_iir_queue:
+                args = self.csr_iir_queue.pop(0)
+                self.csr.set_iir(*args)
+
+            if self.locked and not self.confirmed_that_in_lock:
+                self.confirmed_that_in_lock = self.csr.get(
+                    "logic_autolock_lock_running"
+                )
+                if not self.confirmed_that_in_lock:
                     sleep(0.05)
                     continue
 
-                # copied from https://github.com/RedPitaya/RedPitaya/blob/14cca62dd58f29826ee89f4b28901602f5cdb1d8/api/src/oscilloscope.c#L115  # noqa: E501
-                # check whether scope was triggered
-                not_triggered = (self.red_pitaya.scope.read(0x1 << 2) & 0x4) > 0
-                if not_triggered:
-                    sleep(0.05)
-                    continue
+            if pause_event.is_set():
+                sleep(0.05)
+                continue
+
+            # check that scope is triggered; copied from
+            # https://github.com/RedPitaya/RedPitaya/blob/14cca62dd58f29826ee89f4b28901602f5cdb1d8/api/src/oscilloscope.c#L115  # noqa: E501
+            if not (self.red_pitaya.scope.read(0x1 << 2) & 0x4) <= 0:
+                sleep(0.05)
+                continue
+
+            if self.raw_acquisition_enabled:
+                data_raw = self.read_data_raw(
+                    0x10000, self.red_pitaya.scope.write_pointer_trigger, MAX_N_POINTS
+                )
+                is_raw = True
+            else:
+                data = self.read_data()
+                is_raw = False
 
-                data, is_raw = self.read_data()
+            if pause_event.is_set():
+                # it may seem strange that we check this here a second time. Reason:
+                # `read_data` takes some time and if in the mean time acquisition
+                # was paused, we do not want to send the data
+                continue
 
-                if self.acquisition_paused:
-                    # it may seem strange that we check this here a second time. Reason:
-                    # `read_data` takes some time and if in the mean time acquisition
-                    # was paused, we do not want to send the data
-                    continue
-
-                if self.skip_next_data:
-                    self.skip_next_data = False
+            if skip_next_data_event.is_set():
+                skip_next_data_event.clear()
+            else:
+                if self.raw_acquisition_enabled:
+                    self.data = pickle.dumps(data_raw)
                 else:
                     self.data = pickle.dumps(data)
-                    self.data_was_raw = is_raw
-                    self.data_hash = random()
+                self.data_was_raw = is_raw
+                self.data_hash = random()
 
-                self.program_acquisition_and_rearm()
+            self.program_acquisition_and_rearm()
 
-        self.thread = threading.Thread(target=run_acquiry_loop, args=())
-        self.thread.daemon = True
-        self.thread.start()
+    def read_data(self) -> Dict[str, np.ndarray]:
+        signals = []
+
+        channel_offsets = [0x10000]
+        if self.fetch_additional_signals or self.locked:
+            channel_offsets.append(0x20000)
+
+        for channel_offset in channel_offsets:
+            channel_data = self.read_data_raw(
+                channel_offset,
+                self.red_pitaya.scope.write_pointer_trigger,
+                N_POINTS,
+            )
+
+            for sub_channel_idx in (0, 1):
+                signals.append(channel_data[sub_channel_idx])
+
+        signals_named = {}
+
+        if not self.locked:
+            signals_named["error_signal_1"] = signals[0]
+
+            if self.fetch_additional_signals and len(signals) >= 3:
+                signals_named["error_signal_1_quadrature"] = signals[2]
+
+            if self.dual_channel:
+                signals_named["error_signal_2"] = signals[1]
+                if self.fetch_additional_signals and len(signals) >= 3:
+                    signals_named["error_signal_2_quadrature"] = signals[3]
+            else:
+                signals_named["monitor_signal"] = signals[1]
+
+        else:
+            signals_named["error_signal"] = signals[0]
+            signals_named["control_signal"] = signals[1]
+
+            if not self.dual_channel and len(signals) >= 3:
+                signals_named["monitor_signal"] = signals[2]
+
+        slow_out = self.csr.get("logic_slow_value")
+        slow_out = slow_out if slow_out <= 8191 else slow_out - 16384
+        signals_named["slow_control_signal"] = slow_out
+
+        return signals_named
+
+    def read_data_raw(
+        self, offset: int, addr: int, data_length: int
+    ) -> Tuple[Any, ...]:
+        max_data_length = 16383
+        if data_length + addr > max_data_length:
+            to_read_later = data_length + addr - max_data_length
+            data_length -= to_read_later
+        else:
+            to_read_later = 0
+
+        # raw data contains two signals:
+        #   2'h0,adc_b_rd,2'h0,adc_a_rd
+        #   i.e.: 2 zero bits, channel b (14 bit), 2 zero bits, channel a (14 bit)
+        # .copy() is required, because np.frombuffer returns a readonly array
+        raw_data = self.red_pitaya.scope.reads(offset + (4 * addr), data_length).copy()
+
+        # raw_data is an array of 32-bit ints. We cast it to 16 bit --> each original
+        # int is split into two ints
+        raw_data.dtype = np.int16
+
+        # sign bit is at position 14, but we have 16 bit ints
+        raw_data[raw_data >= 2**13] -= 2**14
+
+        # order is such that we have first the signal a then signal b
+        signals = tuple(raw_data[signal_idx::2] for signal_idx in (0, 1))
+
+        if to_read_later > 0:
+            additional_raw_data = self.read_data_raw(offset, 0, to_read_later)
+            signals = tuple(
+                np.append(signals[signal_idx], additional_raw_data[signal_idx])
+                for signal_idx in (0, 1)
+            )
+
+        return signals
 
     def program_acquisition_and_rearm(self, trigger_delay=16384):
-        """Programs the acquisition settings and rearms acquisition."""
+        """Program the acquisition settings and rearm acquisition."""
         if not self.locked:
             target_decimation = 2 ** (self.sweep_speed + int(np.log2(DECIMATION)))
 
             self.red_pitaya.scope.data_decimation = target_decimation
             self.red_pitaya.scope.trigger_delay = int(trigger_delay / DECIMATION) - 1
 
         elif self.raw_acquisition_enabled:
             self.red_pitaya.scope.data_decimation = 2**self.raw_acquisition_decimation
             self.red_pitaya.scope.trigger_delay = trigger_delay
 
         else:
             self.red_pitaya.scope.data_decimation = 1
             self.red_pitaya.scope.trigger_delay = int(trigger_delay / DECIMATION) - 1
 
-        # trigger_source=6 means external trigger positive edge
-        self.red_pitaya.scope.rearm(trigger_source=6)
+        self.red_pitaya.scope.rearm(trigger_source=TriggerSource.ext_posedge)
 
-    def exposed_return_data(self, last_hash):
+    def exposed_return_data(
+        self, last_hash: Optional[float]
+    ) -> Tuple[
+        bool,
+        Union[float, None],
+        Union[bool, None],
+        Union[bytes, None],
+        Union[float, None],
+    ]:
         no_data_available = self.data_hash is None
         data_not_changed = self.data_hash == last_hash
-        if data_not_changed or no_data_available or self.acquisition_paused:
+        if data_not_changed or no_data_available or self.pause_event.is_set():
             return False, None, None, None, None
         else:
             return True, self.data_hash, self.data_was_raw, self.data, self.data_uuid
 
     def exposed_set_sweep_speed(self, speed):
         self.sweep_speed = speed
         # if a slow acqisition is currently running and we change the sweep speed we
         # don't want to wait until it finishes
         self.program_acquisition_and_rearm()
 
-    def exposed_set_lock_status(self, locked):
+    def exposed_set_lock_status(self, locked: bool) -> None:
         self.locked = locked
         self.confirmed_that_in_lock = False
 
-    def exposed_set_fetch_additional_signals(self, fetch):
+    def exposed_set_fetch_additional_signals(self, fetch: bool) -> None:
         self.fetch_additional_signals = fetch
 
-    def exposed_set_raw_acquisition(self, data):
-        self.raw_acquisition_enabled = data[0]
-        self.raw_acquisition_decimation = data[1]
+    def exposed_set_raw_acquisition(self, enabled: bool, decimation: int) -> None:
+        self.raw_acquisition_enabled = enabled
+        self.raw_acquisition_decimation = decimation
 
     def exposed_set_dual_channel(self, dual_channel):
         self.dual_channel = dual_channel
 
-    def exposed_set_csr(self, key, value):
+    def exposed_set_csr(self, key: str, value: int) -> None:
         self.csr_queue.append((key, value))
 
     def exposed_set_iir_csr(self, *args):
         self.csr_iir_queue.append(args)
 
+    def exposed_stop_acquisition(self) -> None:
+        self.stop_event.set()
+        self.thread.join()
+        start_nginx()
+
     def exposed_pause_acquisition(self):
-        self.acquisition_paused = True
+        self.pause_event.set()
         self.data_hash = None
         self.data = None
 
-    def exposed_continue_acquisition(self, uuid):
+    def exposed_continue_acquisition(self, uuid: Optional[float]) -> None:
         self.program_acquisition_and_rearm()
         sleep(0.01)
         # resetting data here is not strictly required but we want to be on the safe
         # side
         self.data_hash = None
         self.data = None
-        self.acquisition_paused = False
+        self.pause_event.clear()
         self.data_uuid = uuid
         # if we are sweeping, we have to skip one data set because an incomplete sweep
         # may have been recorded. When locked, this does not matter
-        self.skip_next_data = not self.confirmed_that_in_lock
-
-    def read_data(self):
-        write_pointer = self.red_pitaya.scope.write_pointer_trigger
-
-        if self.raw_acquisition_enabled:
-            return self.read_data_raw(0x10000, write_pointer, MAX_N_POINTS), True
-
-        else:
-            signals = []
-
-            channel_offsets = [0x10000]
-            if self.fetch_additional_signals or self.locked:
-                channel_offsets.append(0x20000)
-
-            for channel_offset in channel_offsets:
-                channel_data = self.read_data_raw(
-                    channel_offset, write_pointer, N_POINTS
-                )
-
-                for sub_channel_idx in (0, 1):
-                    signals.append(channel_data[sub_channel_idx])
-
-            signals_named = {}
-
-            if not self.locked:
-                signals_named["error_signal_1"] = signals[0]
-
-                if self.fetch_additional_signals and len(signals) >= 3:
-                    signals_named["error_signal_1_quadrature"] = signals[2]
-
-                if self.dual_channel:
-                    signals_named["error_signal_2"] = signals[1]
-                    if self.fetch_additional_signals and len(signals) >= 3:
-                        signals_named["error_signal_2_quadrature"] = signals[3]
-                else:
-                    signals_named["monitor_signal"] = signals[1]
-
-            else:
-                signals_named["error_signal"] = signals[0]
-                signals_named["control_signal"] = signals[1]
-
-                if not self.dual_channel and len(signals) >= 3:
-                    signals_named["monitor_signal"] = signals[2]
-
-            slow_out = self.csr.get("logic_slow_value")
-            slow_out = slow_out if slow_out <= 8191 else slow_out - 16384
-            signals_named["slow_control_signal"] = slow_out
-
-            return signals_named, False
-
-    def read_data_raw(self, offset, addr, data_length):
-        max_data_length = 16383
-        if data_length + addr > max_data_length:
-            to_read_later = data_length + addr - max_data_length
-            data_length -= to_read_later
+        if self.confirmed_that_in_lock:
+            self.skip_next_data_event.clear()
         else:
-            to_read_later = 0
+            self.skip_next_data_event.set()
 
-        # raw data contains two signals:
-        #   2'h0,adc_b_rd,2'h0,adc_a_rd
-        #   i.e.: 2 zero bits, channel b (14 bit), 2 zero bits, channel a (14 bit)
-        # .copy() is required, because np.frombuffer returns a readonly array
-        raw_data = self.red_pitaya.scope.reads(offset + (4 * addr), data_length).copy()
 
-        # raw_data is an array of 32-bit ints. We cast it to 16 bit --> each original
-        # int is split into two ints
-        raw_data.dtype = np.int16
+def flash_fpga():
+    filepath = Path(__file__).resolve().parent / "linien.bin"
+    shutil.copy(str(filepath), "/dev/xdevcfg")
 
-        # sign bit is at position 14, but we have 16 bit ints
-        raw_data[raw_data >= 2**13] -= 2**14
 
-        # order is such that we have first the signal a then signal b
-        signals = tuple(raw_data[signal_idx::2] for signal_idx in (0, 1))
+def start_nginx():
+    subprocess.Popen(["systemctl", "start", "redpitaya_nginx.service"])
 
-        if to_read_later > 0:
-            additional_raw_data = self.read_data_raw(offset, 0, to_read_later)
-            signals = tuple(
-                np.append(signals[signal_idx], additional_raw_data[signal_idx])
-                for signal_idx in (0, 1)
-            )
 
-        return signals
+def stop_nginx():
+    subprocess.Popen(["systemctl", "stop", "redpitaya_nginx.service"]).wait()
+    subprocess.Popen(["systemctl", "stop", "redpitaya_scpi.service"]).wait()
 
 
 if __name__ == "__main__":
-    t = OneShotServer(DataAcquisitionService(), port=ACQUISITION_PORT)
-    t.start()
+    threaded_server = ThreadedServer(AcquisitionService(), port=ACQUISITION_PORT)
+    print("Starting AcquisitionService on port ", ACQUISITION_PORT)
+    threaded_server.start()
```

### Comparing `linien-server-0.7.0rc2/linien_server/approach_line.py` & `linien-server-0.8.0rc1/linien_server/optimization/approach_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,28 +134,28 @@
     def _decrease_scan_range(self):
         self.N_at_this_zoom = 0
         self.last_shifts_at_this_zoom = None
 
         self.zoom_factor *= ZOOM_STEP
         self.time_last_zoom = time()
 
-        self.control.pause_acquisition()
+        self.control.exposed_pause_acquisition()
 
         self.parameters.sweep_amplitude.value /= ZOOM_STEP
         if self.allow_sweep_speed_change:
             new_sweep_speed = (
                 self.parameters.sweep_speed.value - 1
                 if self.parameters.sweep_speed.value > 5
                 else self.parameters.sweep_speed.value
             )
             self.parameters.sweep_speed.value = new_sweep_speed
         self.control.exposed_write_registers()
-        self.control.continue_acquisition()
+        self.control.exposed_continue_acquisition()
 
     def _correct_current(self, shift):
-        self.control.pause_acquisition()
+        self.control.exposed_pause_acquisition()
         self.time_last_current_correction = time()
 
         self.parameters.sweep_center.value -= shift
 
         self.control.exposed_write_registers()
-        self.control.continue_acquisition()
+        self.control.exposed_continue_acquisition()
```

### Comparing `linien-server-0.7.0rc2/linien_server/autolock/algorithm_selection.py` & `linien-server-0.8.0rc1/linien_server/autolock/algorithm_selection.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.7.0rc2/linien_server/autolock/autolock.py` & `linien-server-0.8.0rc1/linien_server/autolock/autolock.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,21 +124,21 @@
             self.peak_idxs[1],
             additional_spectra=self.additional_spectra,
         )
 
     def add_data_listener(self):
         if not self._data_listener_added:
             self._data_listener_added = True
-            self.parameters.to_plot.on_change(
-                self.react_to_new_spectrum, call_listener_with_first_value=False
+            self.parameters.to_plot.add_callback(
+                self.react_to_new_spectrum, call_with_first_value=False
             )
 
     def remove_data_listener(self):
         self._data_listener_added = False
-        self.parameters.to_plot.remove_listener(self.react_to_new_spectrum)
+        self.parameters.to_plot.remove_callback(self.react_to_new_spectrum)
 
     def react_to_new_spectrum(self, plot_data):
         """React to new spectrum data.
 
         If this is executed for the first time, a reference spectrum is
         recorded.
 
@@ -216,23 +216,23 @@
             line_width,
             peak_idxs,
         ) = get_lock_point(error_signal, self.x0, self.x1)
 
         self.central_y = int(mean_signal)
 
         if auto_offset:
-            self.control.pause_acquisition()
+            self.control.exposed_pause_acquisition()
             self.parameters.combined_offset.value = -1 * self.central_y
             error_signal -= self.central_y
             error_signal_rolled -= self.central_y
             self.additional_spectra = [
                 s - self.central_y for s in self.additional_spectra
             ]
             self.control.exposed_write_registers()
-            self.control.continue_acquisition()
+            self.control.exposed_continue_acquisition()
 
         self.parameters.target_slope_rising.value = target_slope_rising
         self.control.exposed_write_registers()
 
         return error_signal, error_signal_rolled, line_width, peak_idxs
 
     def after_lock(self, error_signal, control_signal, slow_out):
@@ -274,15 +274,15 @@
         self.parameters.fetch_additional_signals.value = True
         self.remove_data_listener()
 
         self._reset_scan()
         self.parameters.task.value = None
 
     def _reset_scan(self):
-        self.control.pause_acquisition()
+        self.control.exposed_pause_acquisition()
 
         self.parameters.sweep_amplitude.value = (
             self.parameters.autolock_initial_sweep_amplitude.value
         )
         self.control.exposed_start_sweep()
 
-        self.control.continue_acquisition()
+        self.control.exposed_continue_acquisition()
```

### Comparing `linien-server-0.7.0rc2/linien_server/autolock/fast.py` & `linien-server-0.8.0rc1/linien_server/autolock/fast.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.7.0rc2/linien_server/autolock/robust.py` & `linien-server-0.8.0rc1/linien_server/autolock/robust.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     get_diff_at_time_scale,
     get_lock_region,
     get_target_peak,
     get_time_scale,
     sign,
     sum_up_spectrum,
 )
-from linien_server.utils import sweep_speed_to_time
 
 
 class LockPositionNotFound(Exception):
     pass
 
 
 class UnableToFindDescription(Exception):
@@ -145,28 +144,28 @@
         self._timeout_start_time = time()
         self._timeout_time_to_wait = (
             N_acquisitions_to_wait
             * 2
             * sweep_speed_to_time(self.parameters.sweep_speed.value)
         )
 
-        self.parameters.ping.on_change(self.check_for_timeout)
+        self.parameters.ping.add_callback(self.check_for_timeout)
 
     def check_for_timeout(self, ping):
         min_time_to_wait = 5
 
         if time() - self._timeout_start_time > max(
             self._timeout_time_to_wait, min_time_to_wait
         ):
             print("Waited too long for autolock! Aborting")
             self.stop_timeout()
             self.parameters.task.value.exposed_stop()
 
     def stop_timeout(self):
-        self.parameters.ping.remove_listener(self.check_for_timeout)
+        self.parameters.ping.remove_callback(self.check_for_timeout)
 
     def after_lock(self):
         self.stop_timeout()
 
 
 def calculate_autolock_instructions(spectra_with_jitter, target_idxs):
     spectra, crop_left = crop_spectra_to_same_view(spectra_with_jitter)
@@ -271,7 +270,16 @@
             last_detected_peak = idx
 
             if description_idx == len(description):
                 # this was the last peak!
                 return idx + final_wait_time
 
     raise LockPositionNotFound()
+
+
+def sweep_speed_to_time(sweep_speed):
+    """Sweep speed is an arbitrary unit (cf. `parameters.py`).
+    This function converts it to the duration of the sweep in seconds.
+    """
+    f_real = 3.8e3 / (2**sweep_speed)
+    duration = 1 / f_real
+    return duration
```

### Comparing `linien-server-0.7.0rc2/linien_server/autolock/utils.py` & `linien-server-0.8.0rc1/linien_server/autolock/utils.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.7.0rc2/linien_server/csr.py` & `linien-server-0.8.0rc1/linien_server/csr.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,19 +18,28 @@
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 
 from . import csrmap
 from .iir_coeffs import get_params
 
 
-class PitayaCSR:
+class PythonCSR:
     map = csrmap.csr
     constants = csrmap.csr_constants
     offset = 0x40300000
 
+    def __init__(self, rp):
+        self.rp = rp
+
+    def set_one(self, addr: str, value: int) -> None:
+        self.rp.write(addr, value)
+
+    def get_one(self, addr):
+        return int(self.rp.read(addr))
+
     def set(self, name, value):
         map, addr, width, wr = self.map[name]
         assert wr, name
 
         ma = 1 << width
         bit_mask = ma - 1
         val = value & bit_mask
@@ -40,15 +49,15 @@
         )
 
         b = (width + 8 - 1) // 8
         for i in range(b):
             v = (val >> (8 * (b - i - 1))) & 0xFF
             self.set_one(self.offset + (map << 11) + ((addr + i) << 2), v)
 
-    def get(self, name):
+    def get(self, name: str) -> int:
         if name in self.constants:
             return self.constants[name]
 
         map, addr, nr, wr = self.map[name]
         v = 0
         b = (nr + 8 - 1) // 8
         for i in range(b):
@@ -68,23 +77,9 @@
         self.set(prefix + "_z0", z)
         for i in range(len(b), 3):
             n = prefix + "_b%i" % i
             if n in self.map:
                 self.set(n, 0)
                 self.set(prefix + "_a%i" % i, 0)
 
-    def signal(self, name):
-        return csrmap.signals.index(name)
-
     def states(self, *names):
         return sum(1 << csrmap.states.index(name) for name in names)
-
-
-class PythonCSR(PitayaCSR):
-    def __init__(self, rp):
-        self.rp = rp
-
-    def set_one(self, addr, value):
-        self.rp.write(addr, value)
-
-    def get_one(self, addr):
-        return int(self.rp.read(addr))
```

### Comparing `linien-server-0.7.0rc2/linien_server/csrmap.py` & `linien-server-0.8.0rc1/linien_server/csrmap.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.7.0rc2/linien_server/iir_coeffs.py` & `linien-server-0.8.0rc1/linien_server/iir_coeffs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # Copyright 2014-2015 Robert Jordens <jordens@gmail.com>
 # Copyright 2018-2022 Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>
 # Copyright 2021-2022 Bastian Leykauf <leykauf@physik.hu-berlin.de>
 #
-# This file is part of redpid.
+# This file is part of Linien.
 #
-# redpid is free software: you can redistribute it and/or modify
+# Linien is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # Linien is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with Linien.  If not, see <http://www.gnu.org/licenses/>.
+# along with Linien. If not, see <http://www.gnu.org/licenses/>.
 
 import warnings
 from math import ceil, log2, pi
 
-import scipy.signal
+from scipy import signal
 
 
 def make_filter(name, k=1.0, f=0.0, g=1e20, q=0.5):
     f *= pi
 
     if name == "LP":  # k/(s + 1)
         b = [f * k / (f + 2), f * k / (f + 2)]
@@ -124,15 +124,18 @@
     b = [int(round(i * s)) for i in b]
     a = [int(round(i * s)) for i in a]
 
     m = 1 << (width - 1)
     for i in b + a:
         assert -m <= i < m, (hex(i), hex(m))
 
-    z, p, k = scipy.signal.tf2zpk(b, a)
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", category=signal.BadCoefficients)
+        warnings.simplefilter("ignore", category=RuntimeWarning)
+        z, p, k = signal.tf2zpk(b, a)
     if any(abs(_) > 1 for _ in p):
         warnings.warn(
             "unstable filter: z={}, p={}, k={}".format(z, p, k), RuntimeWarning
         )
 
     return b, a, shift
```

### Comparing `linien-server-0.7.0rc2/linien_server/linien.bin` & `linien-server-0.8.0rc1/linien_server/linien.bin`

 * *Files identical despite different names*

### Comparing `linien-server-0.7.0rc2/linien_server/linien_start_server.sh` & `linien-server-0.8.0rc1/linien_server/linien_start_server.sh`

 * *Files identical despite different names*

### Comparing `linien-server-0.7.0rc2/linien_server/optimization/engine.py` & `linien-server-0.8.0rc1/linien_server/optimization/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,20 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import math
+import warnings
+
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore")
+    import cma
 
-import cma
 from linien_common.common import MHz, Vpp
 from linien_server.optimization.utils import (
     FINAL_ZOOM_FACTOR,
     get_max_slope,
     optimize_phase_from_iq,
 )
 
@@ -169,15 +173,15 @@
         self.opt = [
             NoOptimizationEngine,
             OneDimensionalOptimizationEngine,
             MultiDimensionalOptimizationEngine,
         ][len(self.bounds)]([[0, 1]] * len(self.bounds))
 
     def request_and_set_new_parameters(self, use_initial_parameters=False):
-        self.control.pause_acquisition()
+        self.control.exposed_pause_acquisition()
 
         if use_initial_parameters:
             for param, initial in zip(self.all_params, self.params_before_start):
                 param.value = initial
         else:
             new_params = self.opt.ask()
             new_params_converted = [
@@ -188,15 +192,15 @@
             for param, value in zip(self.to_optimize, new_params_converted):
                 param.value = value
 
             self.last_parameters = list(new_params_converted)
             self.last_parameters_internal = list(new_params)
 
         self.control.exposed_write_registers()
-        self.control.continue_acquisition()
+        self.control.exposed_continue_acquisition()
 
     def finished(self):
         return self.opt.finished()
 
     def get_demod_phase_param(self):
         params = self.parameters
         dual_channel = params.dual_channel.value
```

### Comparing `linien-server-0.7.0rc2/linien_server/optimization/general.py` & `linien-server-0.8.0rc1/linien_server/optimization/general.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.7.0rc2/linien_server/optimization/optimization.py` & `linien-server-0.8.0rc1/linien_server/optimization/optimization.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import pickle
 import traceback
 
 import numpy as np
 from linien_common.common import determine_shift_by_correlation, get_lock_point
-from linien_server.approach_line import Approacher
-from linien_server.optimization.engine import OptimizerEngine
-from linien_server.optimization.utils import FINAL_ZOOM_FACTOR
+
+from .approach_line import Approacher
+from .engine import OptimizerEngine
+from .utils import FINAL_ZOOM_FACTOR
 
 
 class OptimizeSpectroscopy:
     def __init__(self, control, parameters):
         self.control = control
         self.parameters = parameters
 
@@ -54,15 +55,15 @@
         max_idx = np.argmax(cropped)
         self.x0, self.x1 = x0 + min_idx, x0 + max_idx
 
         self.record_first_error_signal(spectrum)
 
         params = self.parameters
         self.engine = OptimizerEngine(self.control, params)
-        params.to_plot.on_change(self.react_to_new_spectrum)
+        params.to_plot.add_callback(self.react_to_new_spectrum)
         params.optimization_running.value = True
         params.optimization_improvement.value = 0
 
     def record_first_error_signal(self, error_signal):
         (
             mean_signal,
             _2,
@@ -160,21 +161,21 @@
     def exposed_stop(self, use_new_parameters):
         if use_new_parameters and self.parameters.optimization_improvement.value > 0:
             self.engine.use_best_parameters()
         else:
             self.engine.request_and_set_new_parameters(use_initial_parameters=True)
 
         self.parameters.optimization_running.value = False
-        self.parameters.to_plot.remove_listener(self.react_to_new_spectrum)
+        self.parameters.to_plot.remove_callback(self.react_to_new_spectrum)
         self.parameters.task.value = None
 
         self.reset_scan()
 
     def reset_scan(self):
-        self.control.pause_acquisition()
+        self.control.exposed_pause_acquisition()
 
         self.parameters.sweep_speed.value = self.initial_sweep_speed
         self.parameters.sweep_amplitude.value = self.initial_sweep_amplitude
         self.parameters.sweep_center.value = self.initial_sweep_center
         self.control.exposed_write_registers()
 
-        self.control.continue_acquisition()
+        self.control.exposed_continue_acquisition()
```

### Comparing `linien-server-0.7.0rc2/linien_server/optimization/utils.py` & `linien-server-0.8.0rc1/linien_server/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.7.0rc2/linien_server/pid_optimization/pid_optimization.py` & `linien-server-0.8.0rc1/linien_server/pid_optimization/pid_optimization.py`

 * *Files 9% similar despite different names*

```diff
@@ -108,38 +108,38 @@
 
         self.is_child = is_child
 
     def run(self):
         try:
             self.uuid = generate_curve_uuid()
             self.set_decimation(ALL_DECIMATIONS[0])
-            self.add_listeners()
+            self.add_callbacks()
             self.parameters.psd_acquisition_running.value = True
-        except:
+        except Exception as e:
             self.cleanup()
-            raise
+            raise e
 
-    def add_listeners(self):
-        self.parameters.acquisition_raw_data.on_change(
-            self.react_to_new_signal, call_listener_with_first_value=False
+    def add_callbacks(self):
+        self.parameters.acquisition_raw_data.add_callback(
+            self.react_to_new_signal, call_with_first_value=False
         )
 
     def cleanup(self):
         self.running = False
         self.parameters.psd_acquisition_running.value = False
 
-        self.parameters.acquisition_raw_data.remove_listener(self.react_to_new_signal)
+        self.parameters.acquisition_raw_data.remove_callback(self.react_to_new_signal)
 
         if not self.is_child:
-            self.control.pause_acquisition()
+            self.control.exposed_pause_acquisition()
             self.parameters.acquisition_raw_enabled.value = False
             self.parameters.acquisition_raw_filter_enabled.value = False
 
             self.control.exposed_write_registers()
-            self.control.continue_acquisition()
+            self.control.exposed_continue_acquisition()
 
     def react_to_new_signal(self, data_pickled):
         try:
             if not self.running or self.parameters.pause_acquisition.value:
                 return
 
             data = pickle.loads(data_pickled)
@@ -168,17 +168,17 @@
             if not complete:
                 new_decimation = self.decimation_index
                 print("set new decimation", new_decimation)
                 self.set_decimation(new_decimation)
             else:
                 self.cleanup()
 
-        except:
+        except Exception as e:
             self.cleanup()
-            raise
+            raise e
 
     def publish_psd_data(self, complete):
         data_pickled = pickle.dumps(
             {
                 "uuid": self.uuid,
                 "time": time(),
                 "p": self.parameters.p.value,
@@ -196,28 +196,28 @@
             # psd data may change quickly. This makes it possible that someone
             # listening to partial psd data may miss the complete data set because
             # a new partial trace is being recorded.
             self.parameters.psd_data_complete.value = data_pickled
 
     def set_decimation(self, decimation):
         self.time_decimation_set = time()
-        self.control.pause_acquisition()
+        self.control.exposed_pause_acquisition()
         self.parameters.acquisition_raw_decimation.value = decimation
         self.parameters.acquisition_raw_enabled.value = True
 
         # lowpass filter for preventing alias effects
         self.parameters.acquisition_raw_filter_enabled.value = True
         self.parameters.acquisition_raw_filter_frequency.value = int(
             125e6 / (2**decimation) / 2
         )
 
         self.control.exposed_write_registers()
         # take care that new decimation was actually written to FPGA
         sleep(0.1)
-        self.control.continue_acquisition()
+        self.control.exposed_continue_acquisition()
 
     def exposed_stop(self):
         self.cleanup()
 
 
 class PIDOptimization:
     def __init__(self, control, parameters):
@@ -226,36 +226,36 @@
 
         self.engine = MultiDimensionalOptimizationEngine(
             [[100, 4000], [100, 4000]], x0=[2000, 2000]
         )
 
     def run(self):
         try:
-            self.parameters.psd_data_complete.on_change(
-                self.psd_data_received, call_listener_with_first_value=False
+            self.parameters.psd_data_complete.add_callback(
+                self.psd_data_received, call_with_first_value=False
             )
             self.parameters.psd_optimization_running.value = True
             self.start_single_psd_measurement()
-        except:
+        except Exception as e:
             self.cleanup()
-            raise
+            raise e
 
     def start_single_psd_measurement(self):
         new_params = self.engine.ask()
         self.parameters.p.value = int(new_params[0])
         self.parameters.i.value = int(new_params[1])
 
         self.psd_acquisition = PSDAcquisition(
             self.control, self.parameters, is_child=True
         )
         self.psd_acquisition.run()
 
     def cleanup(self):
         self.parameters.psd_optimization_running.value = False
-        self.parameters.psd_data_complete.remove_listener(self.psd_data_received)
+        self.parameters.psd_data_complete.remove_callback(self.psd_data_received)
 
     def psd_data_received(self, psd_data_pickled):
         try:
             # psd data doesn't have to be stored here as a client that is interested
             # in it may listen to parameters.psd_data change events
             psd_data = pickle.loads(psd_data_pickled)
 
@@ -267,13 +267,13 @@
             self.start_single_psd_measurement()
 
             done = self.engine.finished()
             if done:
                 # FIXME: implement use of optimized pid parameters
                 self.cleanup()
 
-        except:
+        except Exception as e:
             self.cleanup()
-            raise
+            raise e
 
     def exposed_stop(self):
         self.cleanup()
```

### Comparing `linien-server-0.7.0rc2/linien_server/server.py` & `linien-server-0.8.0rc1/linien_server/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,415 +13,401 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import _thread
-import os
+import atexit
 import pickle
-import sys
-import threading
-from random import random
+from copy import copy
+from random import randint, random
+from threading import Event, Thread
 from time import sleep
+from typing import List, Tuple
 
 import click
 import numpy as np
 import rpyc
-from linien_common.common import (
-    N_POINTS,
-    check_plot_data,
-    pack,
-    unpack,
-    update_signal_history,
-)
+from linien_common.common import N_POINTS, check_plot_data, update_signal_history
 from linien_common.config import DEFAULT_SERVER_PORT
+from linien_common.influxdb import InfluxDBCredentials, restore_credentials
 from linien_server import __version__
 from linien_server.autolock.autolock import Autolock
+from linien_server.influxdb import InfluxDBLogger
 from linien_server.optimization.optimization import OptimizeSpectroscopy
-from linien_server.parameter_store import ParameterStore
-from linien_server.parameters import Parameters
+from linien_server.parameters import Parameters, restore_parameters, save_parameters
 from linien_server.pid_optimization.pid_optimization import (
     PIDOptimization,
     PSDAcquisition,
 )
-from rpyc.utils.authenticators import AuthenticationError
+from linien_server.registers import Registers
 from rpyc.utils.server import ThreadedServer
 
 
 class BaseService(rpyc.Service):
     """
     A service that provides functionality for seamless integration of parameter access
     on the client.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.parameters = Parameters()
-        self.parameter_store = ParameterStore(self.parameters)
-        self._uuid_mapping = {}
+        self.parameters = restore_parameters(self.parameters)
+        atexit.register(save_parameters, self.parameters)
+        self._uuid_mapping = {}  # type: ignore[var-annotated]
+
+        influxdb_credentials = restore_credentials()
+        self.influxdb_logger = InfluxDBLogger(influxdb_credentials, self.parameters)
 
-    def on_connect(self, client):
+        self.stop_event = Event()
+        self.stop_log_event = Event()
+
+    def on_connect(self, client) -> None:
         self._uuid_mapping[client] = client.root.uuid
 
-    def on_disconnect(self, client):
+    def on_disconnect(self, client) -> None:
         uuid = self._uuid_mapping[client]
         self.parameters.unregister_remote_listeners(uuid)
 
-    def exposed_get_param(self, param_name):
-        return pack(self.parameters._get_param(param_name).value)
+    def exposed_get_server_version(self) -> str:
+        return __version__
+
+    def exposed_get_param(self, param_name: str) -> bytes:
+        return pickle.dumps(getattr(self.parameters, param_name).value)
 
-    def exposed_set_param(self, param_name, value):
-        self.parameters._get_param(param_name).value = unpack(value)
+    def exposed_set_param(self, param_name: str, value: bytes) -> None:
+        getattr(self.parameters, param_name).value = pickle.loads(value)
 
-    def exposed_init_parameter_sync(self, uuid):
-        return pack(list(self.parameters.init_parameter_sync(uuid)))
+    def exposed_reset_param(self, param_name: str) -> None:
+        getattr(self.parameters, param_name).reset()
 
-    def exposed_register_remote_listener(self, uuid, param_name):
-        return self.parameters.register_remote_listener(uuid, param_name)
+    def exposed_init_parameter_sync(self, uuid: str) -> bytes:
+        return pickle.dumps(list(self.parameters.init_parameter_sync(uuid)))
 
-    def exposed_register_remote_listeners(self, uuid, param_names):
+    def exposed_register_remote_listener(self, uuid: str, param_name: str) -> None:
+        self.parameters.register_remote_listener(uuid, param_name)
+
+    def exposed_register_remote_listeners(
+        self, uuid: str, param_names: List[str]
+    ) -> None:
         for param_name in param_names:
             self.exposed_register_remote_listener(uuid, param_name)
 
-    def exposed_get_listener_queue(self, uuid):
-        return self.parameters.get_listener_queue(uuid)
+    def exposed_get_changed_parameters_queue(self, uuid: str) -> bytes:
+        return pickle.dumps(self.parameters.get_changed_parameters_queue(uuid))
+
+    def exposed_set_parameter_log(self, param_name: str, value: bool) -> None:
+        if getattr(self.parameters, param_name).log != value:
+            print("Setting log for %s to %s" % (param_name, value))
+            getattr(self.parameters, param_name).log = value
+
+    def exposed_get_parameter_log(self, param_name: str) -> bool:
+        return getattr(self.parameters, param_name).log
+
+    def exposed_update_influxdb_credentials(
+        self, credentials: InfluxDBCredentials
+    ) -> Tuple[bool, int, str]:
+        credentials = copy(credentials)
+        (
+            connection_succesful,
+            status_code,
+            message,
+        ) = self.influxdb_logger.test_connection(credentials)
+        if connection_succesful:
+            self.influxdb_logger.credentials = credentials
+            print("InfluxDB credentials updated successfully")
+        else:
+            print(
+                "InfluxDB credentials update failed. Error message: %s (Status Code %s)"
+                % (message, status_code)
+            )
+        return connection_succesful, status_code, message
+
+    def exposed_get_influxdb_credentials(self) -> bytes:
+        return pickle.dumps(self.influxdb_logger.credentials)
+
+    def exposed_start_logging(self, interval: float) -> None:
+        print("Starting logging")
+        self.influxdb_logger.start_logging(interval)
+
+    def exposed_stop_logging(self) -> None:
+        print("Stopping logging")
+        self.influxdb_logger.stop_logging()
+
+    def exposed_get_logging_status(self) -> bool:
+        return not self.influxdb_logger.stop_event.is_set()
 
 
 class RedPitayaControlService(BaseService):
     """Control server that runs on the RP that provides high-level methods."""
 
-    def __init__(self, **kwargs):
+    def __init__(self, host=None):
         self._cached_data = {}
         self.exposed_is_locked = None
 
-        super().__init__()
+        super(RedPitayaControlService, self).__init__()
 
-        from linien_server.registers import Registers
+        self.registers = Registers(control=self, parameters=self.parameters, host=host)
+        # Connect the acquisition loop to the parameters: Every received value is pushed
+        # to `parameters.to_plot`.
+        self.exposed_pause_acquisition()
+        self.exposed_continue_acquisition()
+
+        # Start a timer that increases the `ping` parameter once per second. Its purpose
+        # is to allow for periodic tasks on the server: just register an `on_change`
+        # listener for this parameter.
 
-        self.registers = Registers(**kwargs)
-        self.registers.connect(self, self.parameters)
+        self.ping_thread = Thread(
+            target=self._send_ping_loop, args=(self.stop_event,), daemon=True
+        )
+        self.data_pusher_thread = Thread(
+            target=self._push_acquired_data_to_parameters,
+            args=(self.stop_event,),
+            daemon=True,
+        )
+
+        self.ping_thread.start()
+        self.data_pusher_thread.start()
+
+        self.exposed_write_registers()
 
-    def run_acquiry_loop(self):
-        """Starts a background process that keeps polling control and error
-        signal. Every received value is pushed to `parameters.to_plot`."""
-
-        def on_new_data_received(is_raw, plot_data, data_uuid):
-            # When a parameter is changed, `pause_acquisition` is set.
-            # This means that the we should skip new data until we are sure that
-            # it was recorded with the new settings.
+    def _send_ping_loop(self, stop_event: Event):
+        while not stop_event.is_set():
+            self.parameters.ping.value += 1
+            if self.parameters.ping.value < 10:
+                print("ping", self.parameters.ping.value)
+                if self.parameters.ping.value == 9:
+                    print("further pings will be suppressed")
+            sleep(1)
+
+    def _push_acquired_data_to_parameters(self, stop_event: Event):
+        last_hash = None
+        while not stop_event.is_set():
+            (
+                new_data_returned,
+                new_hash,
+                data_was_raw,
+                new_data,
+                data_uuid,
+            ) = self.registers.acquisition.exposed_return_data(last_hash)
+            if new_data_returned:
+                last_hash = new_hash
+            # When a parameter is changed, `pause_acquisition` is set. This means that
+            # the we should skip new data until we are sure that it was recorded with
+            # the new settings.
             if not self.parameters.pause_acquisition.value:
                 if data_uuid != self.data_uuid:
-                    return
+                    continue
 
-                data_loaded = pickle.loads(plot_data)
+                data_loaded = pickle.loads(new_data)
 
-                if not is_raw:
+                if not data_was_raw:
                     is_locked = self.parameters.lock.value
 
                     if not check_plot_data(is_locked, data_loaded):
-                        print(
-                            "warning: incorrect data received for lock state, ignoring!"
-                        )
-                        return
+                        print("incorrect data received for lock state, ignoring!")
+                        continue
 
-                    self.parameters.to_plot.value = plot_data
-                    self._generate_signal_stats(data_loaded)
+                    self.parameters.to_plot.value = new_data
 
+                    # generate signal stats
+                    stats = {}
+                    for signal_name, signal in data_loaded.items():
+                        stats["%s_mean" % signal_name] = np.mean(signal)
+                        stats["%s_std" % signal_name] = np.std(signal)
+                        stats["%s_max" % signal_name] = np.max(signal)
+                        stats["%s_min" % signal_name] = np.min(signal)
+                    self.parameters.signal_stats.value = stats
                     # update signal history (if in locked state)
                     (
                         self.parameters.control_signal_history.value,
                         self.parameters.monitor_signal_history.value,
                     ) = update_signal_history(
                         self.parameters.control_signal_history.value,
                         self.parameters.monitor_signal_history.value,
                         data_loaded,
                         is_locked,
                         self.parameters.control_signal_history_length.value,
                     )
                 else:
-                    self.parameters.acquisition_raw_data.value = plot_data
-
-        # each time new data is acquired, this function is called
-        self.registers.acquisition.on_new_data_received = on_new_data_received
-        self.pause_acquisition()
-        self.continue_acquisition()
-
-    def run_periodic_timer(self):
-        """
-        Start a timer that increases the `ping` parameter once per second. Its purpose
-        is to allow for periodic tasks on the server: just register an `on_change`
-        listener for this parameter.
-        """
+                    self.parameters.acquisition_raw_data.value = new_data
+            sleep(0.05)
 
-        def send_ping():
-            while True:
-                self.parameters.ping.value = self.parameters.ping.value + 1
-                print("ping", self.parameters.ping.value)
-                sleep(1)
-
-        thread = threading.Thread(target=send_ping)
-        thread.daemon = True
-        thread.start()
-        self._periodic_timer = thread
-
-    def _generate_signal_stats(self, to_plot):
-        stats = {}
-
-        for signal_name, signal in to_plot.items():
-            stats["%s_mean" % signal_name] = np.mean(signal)
-            stats["%s_std" % signal_name] = np.std(signal)
-            stats["%s_max" % signal_name] = np.max(signal)
-            stats["%s_min" % signal_name] = np.min(signal)
-
-        self.parameters.signal_stats.value = stats
-
-    def exposed_write_registers(self):
-        """Sync the parameters with the FPGA registers."""
-        self.registers.write_registers()
-
-    def task_running(self):
+    def _task_running(self):
         return (
             self.parameters.autolock_running.value
             or self.parameters.optimization_running.value
             or self.parameters.psd_acquisition_running.value
             or self.parameters.psd_optimization_running.value
         )
 
+    def exposed_write_registers(self) -> None:
+        """Sync the parameters with the FPGA registers."""
+        self.registers.write_registers()
+
     def exposed_start_autolock(self, x0, x1, spectrum, additional_spectra=None):
         spectrum = pickle.loads(spectrum)
         # start_watching = self.parameters.watch_lock.value
         start_watching = False
         auto_offset = self.parameters.autolock_determine_offset.value
 
-        if not self.task_running():
+        if not self._task_running():
             autolock = Autolock(self, self.parameters)
             self.parameters.task.value = autolock
             autolock.run(
                 x0,
                 x1,
                 spectrum,
                 should_watch_lock=start_watching,
                 auto_offset=auto_offset,
                 additional_spectra=pickle.loads(additional_spectra)
                 if additional_spectra is not None
                 else None,
             )
 
     def exposed_start_optimization(self, x0, x1, spectrum):
-        if not self.task_running():
+        if not self._task_running():
             optim = OptimizeSpectroscopy(self, self.parameters)
             self.parameters.task.value = optim
             optim.run(x0, x1, spectrum)
 
     def exposed_start_psd_acquisition(self):
-        if not self.task_running():
+        if not self._task_running():
             self.parameters.task.value = PSDAcquisition(self, self.parameters)
             self.parameters.task.value.run()
 
+        print("Logging thread stopped.")
+
     def exposed_start_pid_optimization(self):
-        if not self.task_running():
+        if not self._task_running():
             self.parameters.task.value = PIDOptimization(self, self.parameters)
             self.parameters.task.value.run()
 
     def exposed_start_sweep(self):
-        self.pause_acquisition()
-
+        self.exposed_pause_acquisition()
         self.parameters.combined_offset.value = 0
         self.parameters.lock.value = False
         self.exposed_write_registers()
-
-        self.continue_acquisition()
+        self.exposed_continue_acquisition()
 
     def exposed_start_lock(self):
-        self.pause_acquisition()
-
+        self.exposed_pause_acquisition()
         self.parameters.lock.value = True
         self.exposed_write_registers()
-
-        self.continue_acquisition()
+        self.exposed_continue_acquisition()
 
     def exposed_shutdown(self):
-        """Kills the server."""
-        self.registers.acquisition.shutdown()
+        self.stop_event.set()
+        self.ping_thread.join()
+        self.data_pusher_thread.join()
+        self.registers.acquisition.exposed_stop_acquisition()
+        # FIXME: hacky way to trigger atexit handlers for saving parameters
         _thread.interrupt_main()
-        # we use SystemExit instead of os._exit because we want to call atexit
-        # handlers
-        raise SystemExit
-
-    def exposed_get_server_version(self):
-        import linien_server
-
-        return linien_server.__version__
-
-    def exposed_get_restorable_parameters(self):
-        return self.parameters._restorable_parameters
+        raise SystemExit()
 
     def exposed_pause_acquisition(self):
-        self.pause_acquisition()
-
-    def exposed_continue_acquisition(self):
-        self.continue_acquisition()
-
-    def exposed_set_csr_direct(self, k, v):
-        """Directly sets a CSR register. This method is intended for debugging.
-        Normally, the FPGA should be controlled via manipulation of parameters."""
-        self.registers.set(k, v)
-
-    def pause_acquisition(self):
-        """Pause continuous acquisition. Call this before changing a parameter
-        that alters the error / control signal. This way, no inconsistent signals
-        reach the application. After setting the new parameter values, call
-        `continue_acquisition`."""
+        """
+        Pause continuous acquisition. Call this before changing a parameter that alters
+        the error / control signal. This way, no inconsistent signals reach the
+        application. After setting the new parameter values, call
+        `continue_acquisition`.
+        """
         self.parameters.pause_acquisition.value = True
         self.data_uuid = random()
-        self.registers.acquisition.pause_acquisition()
+        self.registers.acquisition.exposed_pause_acquisition()
 
-    def continue_acquisition(self):
-        """Continue acquisition after a short delay, when we are sure that the
-        new parameters values have been written to the FPGA and that data that
-        is now recorded is recorded with the correct parameters."""
+    def exposed_continue_acquisition(self):
+        """
+        Continue acquisition after a short delay, when we are sure that the new
+        parameters values have been written to the FPGA and that data that is now
+        recorded is recorded with the correct parameters.
+        """
         self.parameters.pause_acquisition.value = False
-        self.registers.acquisition.continue_acquisition(self.data_uuid)
+        self.registers.acquisition.exposed_continue_acquisition(self.data_uuid)
 
+    def exposed_set_csr_direct(self, key: str, value: int) -> None:
+        """
+        Directly sets a CSR register. This method is intended for debugging. Normally,
+        the FPGA should be controlled via manipulation of parameters.
+        """
+        self.registers.set(key, value)
 
-class FakeRedPitayaControl(BaseService):
+
+class FakeRedPitayaControlService(BaseService):
     def __init__(self):
         super().__init__()
         self.exposed_is_locked = None
 
-    def exposed_write_registers(self):
-        pass
+        self.random_data_thread = Thread(
+            target=self._write_random_data_to_parameters_loop,
+            args=(self.stop_event,),
+            daemon=True,
+        )
+        self.random_data_thread.start()
 
-    def run_acquiry_loop(self):
-        import threading
-        from random import randint
-        from time import sleep
-
-        def run():
-            while True:
-                max_ = randint(0, 8191)
-                gen = lambda: np.array([randint(-max_, max_) for _ in range(N_POINTS)])
-                self.parameters.to_plot.value = pickle.dumps(
-                    {
-                        "error_signal_1": gen(),
-                        "error_signal_1_quadrature": gen(),
-                        "error_signal_2": gen(),
-                        "error_signal_2_quadrature": gen(),
-                    }
-                )
-                sleep(0.1)
-
-        t = threading.Thread(target=run)
-        t.daemon = True
-        t.start()
+    def _write_random_data_to_parameters_loop(self, stop_event: Event):
+        while not stop_event.is_set():
+            max_ = randint(0, 8191)
+            gen = lambda: np.array([randint(-max_, max_) for _ in range(N_POINTS)])
+            self.parameters.to_plot.value = pickle.dumps(
+                {
+                    "error_signal_1": gen(),
+                    "error_signal_1_quadrature": gen(),
+                    "error_signal_2": gen(),
+                    "error_signal_2_quadrature": gen(),
+                }
+            )
+            sleep(0.1)
 
-    def run_periodic_timer(self):
+    def exposed_write_registers(self):
         pass
 
-    def exposed_shutdown(self):
-        _thread.interrupt_main()
-        os._exit(0)
-
     def exposed_start_autolock(self, x0, x1, spectrum):
         print("start autolock", x0, x1)
 
     def exposed_start_optimization(self, x0, x1, spectrum):
         print("start optimization")
         self.parameters.optimization_running.value = True
 
-    def exposed_get_restorable_parameters(self):
-        return self.parameters._restorable_parameters
-
-    def exposed_get_server_version(self):
-        import linien_server
-
-        return linien_server.__version__
+    def exposed_shutdown(self):
+        raise SystemExit()
 
-    def pause_acquisition(self):
+    def exposed_pause_acquisition(self):
         pass
 
-    def continue_acquisition(self):
+    def exposed_continue_acquisition(self):
         pass
 
 
 @click.command()
 @click.version_option(__version__)
 @click.argument("port", default=DEFAULT_SERVER_PORT, type=int, required=False)
 @click.option(
     "--fake", is_flag=True, help="Runs a fake server that just returns random data"
 )
 @click.option(
-    "--remote-rp",
+    "--host",
     help=(
         "Allows to run the server locally for development and connects to a RedPitaya. "
-        "Specify the RP's credentials as follows: "
-        "--remote-rp=root:myPassword@rp-f0xxxx.local"
+        "Specify the RP's host as follows: --host=rp-f0xxxx.local"
     ),
 )
-def run_server(port, fake=False, remote_rp=False):
+def run_server(port, fake=False, host=None):
     print("Start server on port", port)
 
     if fake:
         print("starting fake server")
-        control = FakeRedPitayaControl()
+        control = FakeRedPitayaControlService()
     else:
-        if remote_rp is not None:
-            assert (
-                "@" in remote_rp and ":" in remote_rp
-            ), "invalid format, should be root:myPassword@rp-f0xxxx.local"
-
-            username, tmp = remote_rp.split(":", 1)
-            r_host, r_password = "".join(reversed(tmp)).split("@", 1)
-            host = "".join(reversed(r_host))
-            password = "".join(reversed(r_password))
-            control = RedPitayaControlService(
-                host=host, user=username, password=password
-            )
-        else:
-            control = RedPitayaControlService()
-
-    control.run_acquiry_loop()
-    control.run_periodic_timer()
-    control.exposed_write_registers()
-
-    failed_auth_counter = {"c": 0}
-
-    def username_and_password_authenticator(sock):
-        # when a client starts the server, it supplies this hash via an environment
-        # variable
-        secret = os.environ.get("LINIEN_AUTH_HASH")
-
-        # client always sends auth hash, even if we run in non-auth mode
-        # --> always read 64 bytes, otherwise rpyc connection can't be established
-        received = sock.recv(64)
-
-        # as a protection against brute force, we don't accept requests after
-        # too many failed auth requests
-        if failed_auth_counter["c"] > 1000:
-            print("received too many failed auth requests!")
-            sys.exit(1)
-
-        if secret is None:
-            print("warning: no authentication set up")
-        else:
-            if received != secret.encode():
-                print("received invalid credentials: ", received)
-
-                failed_auth_counter["c"] += 1
-
-                raise AuthenticationError("invalid username / password")
-
-            print("authentication successful")
-
-        return sock, None
+        control = RedPitayaControlService(host=host)
 
-    t = ThreadedServer(
+    thread = ThreadedServer(
         control,
         port=port,
-        authenticator=username_and_password_authenticator,
         protocol_config={"allow_pickle": True},
     )
-    t.start()
+    thread.start()
 
 
 if __name__ == "__main__":
     run_server()
```

### Comparing `linien-server-0.7.0rc2/linien_server.egg-info/PKG-INFO` & `linien-server-0.8.0rc1/linien_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-server
-Version: 0.7.0rc2
+Version: 0.8.0rc1
 Summary: Server components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-server-0.7.0rc2/linien_server.egg-info/SOURCES.txt` & `linien-server-0.8.0rc1/linien_server.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 setup.py
 linien_server/__init__.py
 linien_server/acquisition.py
-linien_server/acquisition_process.py
-linien_server/approach_line.py
 linien_server/csr.py
 linien_server/csrmap.py
 linien_server/iir_coeffs.py
+linien_server/influxdb.py
 linien_server/linien.bin
 linien_server/linien_install_requirements.sh
 linien_server/linien_start_server.sh
 linien_server/linien_stop_server.sh
-linien_server/parameter_store.py
 linien_server/parameters.py
-linien_server/parameters_base.py
 linien_server/registers.py
 linien_server/server.py
-linien_server/utils.py
 linien_server.egg-info/PKG-INFO
 linien_server.egg-info/SOURCES.txt
 linien_server.egg-info/dependency_links.txt
 linien_server.egg-info/entry_points.txt
 linien_server.egg-info/requires.txt
 linien_server.egg-info/top_level.txt
 linien_server/autolock/__init__.py
 linien_server/autolock/algorithm_selection.py
 linien_server/autolock/autolock.py
 linien_server/autolock/fast.py
 linien_server/autolock/robust.py
 linien_server/autolock/utils.py
 linien_server/optimization/__init__.py
+linien_server/optimization/approach_line.py
 linien_server/optimization/engine.py
 linien_server/optimization/general.py
 linien_server/optimization/optimization.py
 linien_server/optimization/utils.py
 linien_server/pid_optimization/__init__.py
 linien_server/pid_optimization/pid_optimization.py
```

### Comparing `linien-server-0.7.0rc2/setup.py` & `linien-server-0.8.0rc1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
-version = "0.7.0rc2"
+version = "0.8.0rc1"
 
 setup(
     name="linien-server",
     version=version,
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
@@ -36,19 +36,22 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     entry_points={"console_scripts": ["linien-server=linien_server.server:run_server"]},
     python_requires=">=3.5",
     install_requires=[
+        "appdirs>=1.4.4",
+        "certifi==2021.10.8",  # pinned because of bug in default pip 9.0.1, see #339
         "click>=7.1.2",
         "cma>=3.0.3",
+        "pip>=20.3.4",
         "pylpsd>=0.1.4",
         "pyrp3>=1.1.0;platform_machine=='armv7l'",  # only install on RedPitaya
-        "rpyc>=4.0,<5.0",
+        "requests<=2.25.1",
         "linien-common=={}".format(version),
     ],
     scripts=[
         "linien_server/linien_start_server.sh",
         "linien_server/linien_stop_server.sh",
         "linien_server/linien_install_requirements.sh",
     ],
```

