# Comparing `tmp/comet_mpm-0.3.2b0.tar.gz` & `tmp/comet_mpm-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comet_mpm-0.3.2b0.tar", last modified: Thu Jan 12 11:03:40 2023, max compression
+gzip compressed data, was "comet_mpm-0.4.1.tar", last modified: Mon Jul  3 14:16:00 2023, max compression
```

## Comparing `comet_mpm-0.3.2b0.tar` & `comet_mpm-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 11:03:40.655033 comet_mpm-0.3.2b0/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/PACKAGE.md
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-01-12 11:03:40.655033 comet_mpm-0.3.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 11:03:40.655033 comet_mpm-0.3.2b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 11:03:40.655033 comet_mpm-0.3.2b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 11:03:40.655033 comet_mpm-0.3.2b0/src/comet_mpm/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 11:03:40.655033 comet_mpm-0.3.2b0/src/comet_mpm/_json/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/_json/numpy_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/batch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/comet_mpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/data_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/events_from_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/logging_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/optional_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 11:03:40.655033 comet_mpm-0.3.2b0/src/comet_mpm/sender/
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/sender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/sender/asyncio_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/sender/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/sender/thread_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-01-12 11:03:31.000000 comet_mpm-0.3.2b0/src/comet_mpm/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 11:03:40.655033 comet_mpm-0.3.2b0/src/comet_mpm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-01-12 11:03:40.000000 comet_mpm-0.3.2b0/src/comet_mpm.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/PACKAGE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:00.606959 comet_mpm-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/src/comet_mpm/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/src/comet_mpm/_json/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/_json/numpy_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/batch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/comet_mpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/data_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/src/comet_mpm/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/events/base_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/events/events_from_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/events/label_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/events/prediction_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/logging_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/optional_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/src/comet_mpm/sender/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/sender/asyncio_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/sender/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/sender/thread_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/src/comet_mpm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-03 14:16:00.000000 comet_mpm-0.4.1/src/comet_mpm.egg-info/SOURCES.txt
```

### Comparing `comet_mpm-0.3.2b0/MANIFEST.in` & `comet_mpm-0.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.3.2b0/PKG-INFO` & `comet_mpm-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_mpm
-Version: 0.3.2b0
+Version: 0.4.1
 Summary: Comet MPM SDK
 Home-page: https://www.comet.ml
 Author: Comet ML Inc.
 Author-email: mail@comet.ml
 License: Proprietary
 Keywords: comet_mpm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `comet_mpm-0.3.2b0/setup.py` & `comet_mpm-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,21 @@
 #  permission of Comet ML Inc.
 # *******************************************************
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
-requirements = ["pandas", "typing_extensions>=3.7.4", "aiohttp", "pydantic", "requests"]
+requirements = [
+    "pandas",
+    "typing_extensions>=3.7.4",
+    "aiohttp",
+    "pydantic<2.0.0",
+    "requests",
+]
 
 # read the contents of your PACKAGE file
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "PACKAGE.md").read_text()
 
 
@@ -46,11 +52,11 @@
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="comet_mpm",
     name="comet_mpm",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://www.comet.ml",
-    version="0.3.2b0",
+    version="0.4.1",
     zip_safe=False,
     license="Proprietary",
 )
```

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/__init__.py` & `comet_mpm-0.4.1/src/comet_mpm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 #  Copyright (C) 2021 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
 __author__ = """Comet ML Inc."""
 __email__ = "mail@comet.ml"
-__version__ = "0.3.2b0"
+__version__ = "0.4.1"
 __all__ = ["CometMPM"]
 
 from ._logging import _setup_comet_mpm_logging
 from .comet_mpm import CometMPM
 
 _setup_comet_mpm_logging()
```

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/_json/__init__.py` & `comet_mpm-0.4.1/src/comet_mpm/_json/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/_json/numpy_encoder.py` & `comet_mpm-0.4.1/src/comet_mpm/_json/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/_logging.py` & `comet_mpm-0.4.1/src/comet_mpm/_logging.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/batch_utils.py` & `comet_mpm-0.4.1/src/comet_mpm/batch_utils.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/cli.py` & `comet_mpm-0.4.1/src/comet_mpm/cli.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/comet_mpm.py` & `comet_mpm-0.4.1/src/comet_mpm/comet_mpm.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,43 +10,26 @@
 #  Copyright (C) 2021 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
 import asyncio as asyncio_module
 import atexit
-import calendar
 import os
-from datetime import datetime
 from typing import Any, Awaitable, Dict, Iterable, List, Optional, Union
 
-import comet_mpm.event
-import comet_mpm.events_from_dataframe
-
 from . import optional_update
 from .connection import MPM_BASE_PATH, REST_API_BASE_PATH, sanitize_url, url_join
-from .constants import (
-    EVENT_FEATURES,
-    EVENT_PREDICTION,
-    EVENT_PREDICTION_ID,
-    EVENT_PREDICTION_PROBABILITY,
-    EVENT_PREDICTION_VALUE,
-    EVENT_TIMESTAMP,
-    EVENT_WORKSPACE_NAME,
-)
+from .events import events_from_dataframe
+from .events.label_event import LabelEvent
+from .events.prediction_event import PredictionEvent
 from .sender import get_sender
 from .settings import MPMSettings, get_model
 
-
-def local_timestamp() -> int:
-    """Return a timestamp in a format expected by the backend (milliseconds)"""
-    now = datetime.utcnow()
-    timestamp_in_seconds = calendar.timegm(now.timetuple()) + (now.microsecond / 1e6)
-    timestamp_in_milliseconds = int(timestamp_in_seconds * 1000)
-    return timestamp_in_milliseconds
+LogEventsResult = Union[List[Any], Awaitable[List[Any]]]
 
 
 class CometMPM:
     """
     The Comet MPM class is used to upload a model's input and output features to MPM
     """
 
@@ -100,41 +83,26 @@
         self._mpm_url = url_join(sanitize_url(self._settings.url), MPM_BASE_PATH)
         self._api_url = url_join(sanitize_url(self._settings.url), REST_API_BASE_PATH)
 
         if self.disabled:
             self._sender = None
         else:
             self._sender = get_sender(
-                self._settings.api_key,
-                self._mpm_url,
-                self._settings.mpm_model_name,
-                self._settings.mpm_model_version,
+                api_key=self._settings.api_key,
+                server_address=self._mpm_url,
                 max_batch_size=self._settings.mpm_max_batch_size,
                 max_batch_time=self._settings.mpm_max_batch_time,
                 asyncio=self._asyncio,
                 batch_sending_timeout=self._settings.mpm_batch_sending_timeout,
             )
 
             atexit.register(self._on_end)
 
         # TODO: Do handshake
 
-    LogEventsResult = Union[List[Any], Awaitable[List[Any]]]
-
-    def _log_events(self, events: Iterable[comet_mpm.event.Event]) -> LogEventsResult:
-        results = []
-        for event in events:
-            result = self.log_event(**event.to_dictionary())
-            results.append(result)
-
-        if self._asyncio:
-            return asyncio_module.gather(*results)  # type: ignore[arg-type]
-        else:
-            return results
-
     def log_event(
         self,
         prediction_id: str,
         input_features: Optional[Dict[str, Any]] = None,
         output_value: Optional[Any] = None,
         output_probability: Optional[Any] = None,
     ) -> Optional[Awaitable[None]]:
@@ -158,34 +126,49 @@
         """
         if self.disabled:
             if self._asyncio is False:
                 return None
             else:
                 return asyncio_module.sleep(0)
 
-        prediction: Dict[str, Any] = {}
-        if output_value is not None:
-            prediction[EVENT_PREDICTION_VALUE] = output_value
-        if output_probability is not None:
-            prediction[EVENT_PREDICTION_PROBABILITY] = output_probability
-
-        event = {
-            EVENT_WORKSPACE_NAME: self._settings.mpm_workspace_name,
-            EVENT_PREDICTION_ID: prediction_id,
-            EVENT_TIMESTAMP: local_timestamp(),
-        }
-
-        if input_features is not None:
-            event[EVENT_FEATURES] = input_features
+        event = PredictionEvent(
+            workspace=self._settings.mpm_workspace_name,
+            model_name=self._settings.mpm_model_name,
+            model_version=self._settings.mpm_model_version,
+            prediction_id=prediction_id,
+            input_features=input_features,
+            output_value=output_value,
+            output_probability=output_probability,
+        )
+        return self._log_event(event)
 
-        if prediction:
-            event[EVENT_PREDICTION] = prediction
+    def log_label(self, prediction_id: str, label: Any) -> Optional[Awaitable[None]]:
+        """
+        Send an MPM event containing the ground truth value for a prediction whose input and output
+        features are already stored in Comet.
+        Args:
+            prediction_id: The unique prediction ID, could be provided by the
+                framework, you or a random unique value could be provided like
+                str(uuid4())
+            label: the ground truth value for a prediction
+        """
+        if self.disabled:
+            if self._asyncio is False:
+                return None
+            else:
+                return asyncio_module.sleep(0)
 
-        assert self._sender is not None
-        return self._sender.put(event)
+        event = LabelEvent(
+            workspace=self._settings.mpm_workspace_name,
+            model_name=self._settings.mpm_model_name,
+            model_version=self._settings.mpm_model_version,
+            prediction_id=prediction_id,
+            label=label,
+        )
+        return self._log_event(event)
 
     def log_dataframe(  # type: ignore[no-untyped-def]
         self,
         dataframe,
         prediction_id_column: str,
         feature_columns: Optional[List[str]] = None,
         output_value_column: Optional[str] = None,
@@ -205,20 +188,23 @@
             feature_columns: if provided, this column will be used as the
                 input_features parameter for the events.
             output_value_column: if provided, this column will be used as the
                 output_value for the events.
             output_probability_column: if provided, this column will be used as
                 the output_probability for the events.
         """
-        events = comet_mpm.events_from_dataframe.generate(
-            dataframe,
-            prediction_id_column,
-            feature_columns,
-            output_value_column,
-            output_probability_column,
+        events = events_from_dataframe.generate(
+            workspace=self._settings.mpm_workspace_name,
+            model_name=self._settings.mpm_model_name,
+            model_version=self._settings.mpm_model_version,
+            dataframe=dataframe,
+            prediction_id_column=prediction_id_column,
+            feature_columns=feature_columns,
+            output_value_column=output_value_column,
+            output_probability_column=output_probability_column,
         )
 
         return self._log_events(events)
 
     def connect(self) -> None:
         """
         When using CometMPM in asyncio mode, this coroutine needs to be awaited
@@ -244,7 +230,25 @@
             else:
                 return asyncio_module.sleep(0)
 
     def _on_end(self) -> None:
         if not self.disabled:
             assert self._sender is not None
             self._sender.close()
+
+    def _log_events(self, events: Iterable[PredictionEvent]) -> LogEventsResult:
+        results = []
+        for event in events:
+            result = self._log_event(event)
+            if result is not None:
+                results.append(result)
+
+        if self._asyncio and len(results) > 0:
+            return asyncio_module.gather(*results)
+
+        return results
+
+    def _log_event(
+        self, event: Union[PredictionEvent, LabelEvent]
+    ) -> Optional[Awaitable[None]]:
+        assert self._sender is not None
+        return self._sender.put(event)
```

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/connection.py` & `comet_mpm-0.4.1/src/comet_mpm/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     # total = 3
     # s = lambda b, i: b * (2 ** (i - 1))
     # sleep = sum(s(backoff, i) for i in range(1, total + 1))
 
     return Retry(
         total=3,
         backoff_factor=2,
-        allowed_methods=None,  # Force retry on everything
+        allowed_methods=None,
     )  # Will wait up to 24s
 
 
 def get_http_session(retry_strategy: Optional[Retry] = None) -> Session:
     session = Session()
 
     # Setup retry strategy if asked
```

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/data_series.py` & `comet_mpm-0.4.1/src/comet_mpm/data_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,30 +79,32 @@
             The maximal allowed number of distinct values per series.
         sort : bool, default True
             Sort by frequencies.
     Raises:
         TypeError : if provided series has wrong data type. Only int, float, str, bool categorical values are supported.
         ValueError : if there are more than max_distinct_values distinct values per series
     """
-    if not (
-        types.is_numeric_dtype(series)
-        or types.is_bool_dtype(series)
-        or types.is_string_dtype(series)
-    ):
-        raise TypeError("Unsupported series data type: %s" % series.dtype)
+    # count all missing values
+    missing_values = series.isna().sum()
 
+    # check that maximal distinct values within range (including None)
     unique = series.nunique(dropna=False)
     if unique > max_distinct_values:
         raise ValueError(
             "The series has too many distinct values: %d. Max %d of distinct values are allowed."
             % (unique, max_distinct_values)
         )
 
-    # count all missing values
-    missing_values = series.isna().sum()
+    # drop missing values and check that dtype of remaining values are supported
+    series = series.dropna(axis="rows")
+    if not (
+        series.apply(lambda x: types.is_number(x) or types.is_bool(x)).all()
+        or types.is_string_dtype(series)
+    ):
+        raise TypeError("Unsupported series data type: %s" % series.dtype)
 
     # count all categories
     counts = series.value_counts(dropna=True, sort=sort)
     count_distribution = [(k, v) for k, v in counts.items()]
 
     return CategoricalSeriesSummary(
         missing_values=missing_values, count_distribution=count_distribution
@@ -130,15 +132,15 @@
     # count all missing values
     na_positions = series.isna()
     missing_values = na_positions.sum()
 
     # calculate statistics if appropriate
     if not na_positions.all():
         values_raw = series.dropna().quantile(quantiles)
-        values = [v for i, v in values_raw.iteritems()]
+        values = [v for i, v in values_raw.items()]
         stats = NumericalDistributionStats(
             quantiles=quantiles,
             values=values,
         )
 
         return NumericalSeriesSummary(
             missing_values=missing_values, numerical_distribution=stats
```

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/event.py` & `comet_mpm-0.4.1/src/comet_mpm/events/prediction_event.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,40 +8,76 @@
 #
 #  Sign up for free at http://www.comet.ml
 #  Copyright (C) 2021 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
-import copy
-import dataclasses
 from typing import Any, Dict, Optional
 
+from comet_mpm.constants import (
+    EVENT_FEATURES,
+    EVENT_PREDICTION,
+    EVENT_PREDICTION_PROBABILITY,
+    EVENT_PREDICTION_VALUE,
+)
+from comet_mpm.events.base_event import BaseEvent
 
-@dataclasses.dataclass
-class Event:
+
+class PredictionEvent(BaseEvent):
     """
-    This class represents a single event. Events are identified by the
+    This class represents a single prediction event. Events are identified by the
     mandatory prediction_id parameter. Many events can have the same
     prediction_id. The MPM backend merges events with the same prediction_id
     automatically.
     Args:
+        workspace: The project workspace.
+        model_name: The name of model
+        model_version: The version of model
         prediction_id: The unique prediction ID, could be provided by the
             framework, you or a random unique value could be provided like
             str(uuid4())
         input_features: If provided must be a flat Dictionary where the
             keys are the feature name and the value are native Python
             scalars, int, floats, booleans or strings. For example:
             `{“age”: 42, “income”: 42894.89}`
         output_value: The prediction as a native Python scalar, int,
             float, boolean or string.
         output_probability: If provided, must be a float between 0 and 1
             indicating the confidence of the model in the prediction
     """
 
-    prediction_id: str
-    input_features: Optional[Dict[str, Any]] = None
-    output_value: Any = None
-    output_probability: Any = None
+    def __init__(
+        self,
+        workspace: str,
+        model_name: str,
+        model_version: str,
+        prediction_id: str,
+        input_features: Optional[Dict[str, Any]] = None,
+        output_value: Any = None,
+        output_probability: Optional[float] = None,
+    ):
+        super(PredictionEvent, self).__init__(
+            workspace=workspace,
+            model_name=model_name,
+            model_version=model_version,
+            prediction_id=prediction_id,
+        )
+        self.input_features = input_features
+        self.output_value = output_value
+        self.output_probability = output_probability
+
+    def _get_event_dict(self) -> Dict[str, Any]:
+        prediction: Dict[str, Any] = {}
+        if self.output_value is not None:
+            prediction[EVENT_PREDICTION_VALUE] = self.output_value
+        if self.output_probability is not None:
+            prediction[EVENT_PREDICTION_PROBABILITY] = self.output_probability
+
+        event: Dict[str, Any] = {}
+        if self.input_features is not None:
+            event[EVENT_FEATURES] = self.input_features
+
+        if prediction:
+            event[EVENT_PREDICTION] = prediction
 
-    def to_dictionary(self) -> Dict[str, Any]:
-        return copy.deepcopy(self.__dict__)
+        return event
```

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/events_from_dataframe.py` & `comet_mpm-0.4.1/src/comet_mpm/events/events_from_dataframe.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,45 +9,59 @@
 #  Sign up for free at http://www.comet.ml
 #  Copyright (C) 2021 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 from typing import List, Optional
 
-import comet_mpm.event
+from .prediction_event import PredictionEvent
 
 
 def generate(  # type: ignore[no-untyped-def]
+    workspace: str,
+    model_name: str,
+    model_version: str,
     dataframe,
     prediction_id_column: str,
     feature_columns: Optional[List[str]] = None,
     output_value_column: Optional[str] = None,
     output_probability_column: Optional[str] = None,
 ):
     return (
         _event(
-            row,
-            prediction_id_column,
-            feature_columns,
-            output_value_column,
-            output_probability_column,
+            workspace=workspace,
+            model_name=model_name,
+            model_version=model_version,
+            row=row,
+            prediction_id_column=prediction_id_column,
+            feature_columns=feature_columns,
+            output_value_column=output_value_column,
+            output_probability_column=output_probability_column,
         )
         for row in dataframe.to_dict(orient="records")
     )
 
 
 def _event(  # type: ignore[no-untyped-def]
+    workspace: str,
+    model_name: str,
+    model_version: str,
     row,
     prediction_id_column,
     feature_columns,
     output_value_column,
     output_probability_column,
-) -> comet_mpm.event.Event:
+) -> PredictionEvent:
     prediction_id = str(row[prediction_id_column])
-    event = comet_mpm.event.Event(prediction_id=prediction_id)
+    event = PredictionEvent(
+        workspace=workspace,
+        model_name=model_name,
+        model_version=model_version,
+        prediction_id=prediction_id,
+    )
     if feature_columns is not None:
         event.input_features = {key: row[key] for key in feature_columns}
     if output_value_column is not None:
         event.output_value = row[output_value_column]
     if output_probability_column is not None:
         event.output_probability = row[output_probability_column]
```

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/exceptions.py` & `comet_mpm-0.4.1/src/comet_mpm/exceptions.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/logging_messages.py` & `comet_mpm-0.4.1/src/comet_mpm/logging_messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 #  permission of Comet ML Inc.
 # *******************************************************
 
 BATCH_SENDING_ERROR = "Error sending batch data to the backend"
 
 BATCH_SENDING_EXCEPTION = "Unknown exception happened when sending data to the backend"
 
+LABEL_EVENT_SEND_ERROR = "Error sending label to the backend"
+
 GEVENT_NOT_SUPPORTED = (
     "Using the MPM SDK with gevent is not officially supported, data loss might occurs"
 )
 
 ASYNCIO_SENDER_HARD_SHUTDOWN = "There are still some data in-flight and might be missing. Make sure to call CometMPM.join() manually to guarantee that all data has been sent to the Backend"
 
 ERROR_QUANTILES_LIST_EMPTY = (
@@ -30,7 +32,9 @@
 )
 
 LOGGING_DIRECTORY_CREATION_ERROR = "Cannot create path to log file %r"
 
 LOGGING_LOG_FILE_OPEN_ERROR = "Cannot open log file %r; file logging is disabled"
 
 INVALID_SETTING_DEFAULT_FALLBACK = "Some MPM settings values were invalid, default values were used instead, see below for the list"
+
+UNEXPECTED_EVENT_TYPE = "Unexpected event type %r"
```

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/optional_update.py` & `comet_mpm-0.4.1/src/comet_mpm/optional_update.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/sender/__init__.py` & `comet_mpm-0.4.1/src/comet_mpm/sender/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 
 LOGGER = logging.getLogger(__name__)
 
 
 def get_sender(
     api_key: str,
     server_address: str,
-    model_name: str,
-    model_version: str,
     max_batch_size: int,
     max_batch_time: int,
     batch_sending_timeout: int,
     asyncio: bool = False,
 ) -> "BaseSender":
 
     if "gevent" in sys.modules:
@@ -41,25 +39,21 @@
         is_gevent_active = bool(gevent.monkey.saved)
 
         if is_gevent_active:
             LOGGER.warning(GEVENT_NOT_SUPPORTED)
 
     if asyncio is True:
         return get_asyncio_sender(
-            api_key,
-            server_address,
-            model_name,
-            model_version,
-            max_batch_size,
-            max_batch_time,
-            batch_sending_timeout,
+            api_key=api_key,
+            server_address=server_address,
+            max_batch_size=max_batch_size,
+            max_batch_time=max_batch_time,
+            batch_sending_timeout=batch_sending_timeout,
         )
     else:
         return get_thread_sender(
-            api_key,
-            server_address,
-            model_name,
-            model_version,
-            max_batch_size,
-            max_batch_time,
-            batch_sending_timeout,
+            api_key=api_key,
+            server_address=server_address,
+            max_batch_size=max_batch_size,
+            max_batch_time=max_batch_time,
+            batch_sending_timeout=batch_sending_timeout,
         )
```

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/sender/asyncio_sender.py` & `comet_mpm-0.4.1/src/comet_mpm/sender/asyncio_sender.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,71 +16,72 @@
 import logging
 from typing import Any, Optional, Tuple
 
 import aiohttp
 
 from ..batch_utils import Batch
 from ..connection import send_asyncio_batch_requests
+from ..events.label_event import LabelEvent
+from ..events.prediction_event import PredictionEvent
 from ..exceptions import AsyncioSenderNoConnected
-from ..logging_messages import ASYNCIO_SENDER_HARD_SHUTDOWN, BATCH_SENDING_EXCEPTION
-from .base import CLOSE_MESSAGE, BaseSender, batch_endpoint_url, model_base_event
+from ..logging_messages import (
+    ASYNCIO_SENDER_HARD_SHUTDOWN,
+    BATCH_SENDING_EXCEPTION,
+    LABEL_EVENT_SEND_ERROR,
+    UNEXPECTED_EVENT_TYPE,
+)
+from .base import CLOSE_MESSAGE, BaseSender, batch_endpoint_url, labels_endpoint_url
 
 LOGGER = logging.getLogger(__name__)
 
 
 def get_asyncio_sender(
     api_key: str,
     server_address: str,
-    model_name: str,
-    model_version: str,
     max_batch_size: int,
     max_batch_time: int,
     batch_sending_timeout: int,
 ) -> "AsyncioSender":
     sender = AsyncioSender(
-        api_key,
-        server_address,
-        model_name,
-        model_version,
-        max_batch_size,
-        max_batch_time,
-        batch_sending_timeout,
+        api_key=api_key,
+        server_address=server_address,
+        max_batch_size=max_batch_size,
+        max_batch_time=max_batch_time,
+        batch_sending_timeout=batch_sending_timeout,
     )
 
     return sender
 
 
 class AsyncioBackgroundSender:
     def __init__(
         self,
         api_key: str,
         server_address: str,
-        model_name: str,
-        model_version: str,
         queue: "asyncio.Queue[Any]",
         max_batch_size: int,
         max_batch_time: int,
         batch_sending_timeout: int,
     ):
         """A background coroutine that reads from the queue, add the items to the batch and sends
         them whenever the batch is ready to be sent. Can only be created only when an event loop is running.
         """
         self.api_key = api_key
         self.server_address = server_address
-        self.base_event = model_base_event(model_name, model_version)
         self.session: aiohttp.ClientSession = aiohttp.ClientSession()
         self.queue: "asyncio.Queue[Any]" = queue
         self.max_batch_time = max_batch_time
         self.batch = Batch(max_batch_size, self.max_batch_time)
         self.batch_sending_timeout = batch_sending_timeout
 
         self.stop_processing = False
 
         # Pre-compute URLs
         self.batch_endpoint = batch_endpoint_url(self.server_address)
+        self.labels_endpoint = labels_endpoint_url(self.server_address)
 
     async def run(self) -> None:
         while True:
             stop = await self._loop()
 
             if stop is True:
                 break
@@ -88,53 +89,70 @@
         # We force stop the processing of the queue
         await self._check_batch_sending()
         return
 
     async def _loop(self) -> bool:
         try:
             data = await asyncio.wait_for(self.queue.get(), timeout=self.max_batch_time)
+            if data is None:
+                return False
 
-            if data:
-                if data is CLOSE_MESSAGE:
-                    self.stop_processing = True
-                    return True
-
-                self._process_single_event(data)
+            if data is CLOSE_MESSAGE:
+                self.stop_processing = True
+                return True
+
+            if isinstance(data, PredictionEvent):
+                self._process_prediction_event(data)
+            elif isinstance(data, LabelEvent):
+                await self._process_label_event(data)
+            else:
+                LOGGER.error(UNEXPECTED_EVENT_TYPE, data)
         except asyncio.TimeoutError:
             pass
 
         await self._check_batch_sending()
 
         return False
 
-    def _process_single_event(self, data: Any) -> None:
-        to_send = self.base_event.copy()
-        to_send.update(data)
+    async def _process_label_event(self, event: LabelEvent) -> None:
+        try:
+            await send_asyncio_batch_requests(
+                session=self.session,
+                url_endpoint=self.labels_endpoint,
+                api_key=self.api_key,
+                batch_sending_timeout=self.batch_sending_timeout,
+                batch=event.create_event_dict(),
+            )
+        except Exception:
+            LOGGER.error(LABEL_EVENT_SEND_ERROR, exc_info=True)
+
+    def _process_prediction_event(self, event: PredictionEvent) -> None:
+        to_send = event.create_event_dict()
         self.batch.append(to_send)
 
     async def _send_batch(self, batch: Any) -> None:
         async with aiohttp.ClientSession() as session:
             await send_asyncio_batch_requests(
-                session,
-                self.batch_endpoint,
+                session=session,
+                url_endpoint=self.batch_endpoint,
                 api_key=self.api_key,
                 batch_sending_timeout=self.batch_sending_timeout,
                 batch=batch,
             )
 
     async def _check_batch_sending(self) -> None:
         # This should only be called by the background sender coroutine, if not the batch could
         # become corrupted as its access not protected by a lock
         try:
             if self.batch.should_be_uploaded(self.stop_processing):
                 batch = self.batch.get_and_clear()
 
                 await send_asyncio_batch_requests(
-                    self.session,
-                    self.batch_endpoint,
+                    session=self.session,
+                    url_endpoint=self.batch_endpoint,
                     api_key=self.api_key,
                     batch_sending_timeout=self.batch_sending_timeout,
                     batch=batch,
                 )
         except Exception:
             LOGGER.error(BATCH_SENDING_EXCEPTION, exc_info=True)
 
@@ -143,60 +161,54 @@
         #
         self.stop_processing = True
 
         while True:
             try:
                 data = self.queue.get_nowait()
                 if data and data is not CLOSE_MESSAGE:
-                    self._process_single_event(data)
+                    self._process_prediction_event(data)
             except asyncio.QueueEmpty:
                 break
 
         asyncio.run(self._send_batch(self.batch.get_and_clear()))
 
 
 class AsyncioSender(BaseSender):
     def __init__(
         self,
         api_key: str,
         server_address: str,
-        model_name: str,
-        model_version: str,
         max_batch_size: int,
         max_batch_time: int,
         batch_sending_timeout: int,
     ) -> None:
         self.sender_queue: Optional["asyncio.Queue[Any]"] = None
         # We need to wait for the asyncio event loop to be created
         self.background_sender: Optional[AsyncioBackgroundSender] = None
         self.background_task: Optional[asyncio.Task[None]] = None
         self.lock: Optional[asyncio.Lock] = None
         self.drain = False
 
         self.api_key = api_key
         self.server_address = server_address
-        self.model_name = model_name
-        self.model_version = model_version
         self.max_batch_time = max_batch_time
         self.max_batch_size = max_batch_size
         self.batch_sending_timeout = batch_sending_timeout
 
     def connect(self) -> None:
         if self.sender_queue is None:
             sender_queue: "asyncio.Queue[Any]" = asyncio.Queue()
             self.sender_queue = sender_queue
             self.background_sender = AsyncioBackgroundSender(
-                self.api_key,
-                self.server_address,
-                self.model_name,
-                self.model_version,
-                self.sender_queue,
-                self.max_batch_size,
-                self.max_batch_time,
-                self.batch_sending_timeout,
+                api_key=self.api_key,
+                server_address=self.server_address,
+                queue=self.sender_queue,
+                max_batch_size=self.max_batch_size,
+                max_batch_time=self.max_batch_time,
+                batch_sending_timeout=self.batch_sending_timeout,
             )
             self.background_sender.queue = self.sender_queue
 
         if self.background_task is None:
             assert self.background_sender is not None
             self.background_task = asyncio.create_task(self.background_sender.run())
```

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/sender/base.py` & `comet_mpm-0.4.1/src/comet_mpm/sender/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,23 +9,27 @@
 #  Sign up for free at http://www.comet.ml
 #  Copyright (C) 2021 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
 from abc import ABCMeta
-from typing import Any, Awaitable, Dict, Optional
+from typing import Any, Awaitable, Optional
 from urllib.parse import urljoin
 
 
 def batch_endpoint_url(server_address: str) -> str:
     # TODO: Check that server_address finishes with a "/"
     return urljoin(server_address, "events/batch")
 
 
+def labels_endpoint_url(server_address: str) -> str:
+    return urljoin(server_address, "labels")
+
+
 CLOSE_MESSAGE = object()
 
 
 class BaseSender(metaclass=ABCMeta):
     def connect(self) -> None:
         ...  # pragma: no cover
 
@@ -33,11 +37,7 @@
         ...  # pragma: no cover
 
     def close(self) -> None:
         ...  # pragma: no cover
 
     def join(self, timeout: int) -> Optional[Awaitable[None]]:
         ...  # pragma: no cover
-
-
-def model_base_event(model_name: str, model_version: str) -> Dict[str, str]:
-    return {"modelName": model_name, "modelVersion": model_version}
```

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/sender/thread_sender.py` & `comet_mpm-0.4.1/src/comet_mpm/sender/thread_sender.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,45 +15,49 @@
 import logging
 import queue
 from threading import Lock, Thread
 from typing import Any, Optional, Tuple
 
 from ..batch_utils import ThreadSafeBatch
 from ..connection import get_http_session, get_retry_strategy, send_batch_requests
-from ..logging_messages import BATCH_SENDING_EXCEPTION
-from .base import CLOSE_MESSAGE, BaseSender, batch_endpoint_url, model_base_event
+from ..events.label_event import LabelEvent
+from ..events.prediction_event import PredictionEvent
+from ..logging_messages import (
+    BATCH_SENDING_EXCEPTION,
+    LABEL_EVENT_SEND_ERROR,
+    UNEXPECTED_EVENT_TYPE,
+)
+from .base import CLOSE_MESSAGE, BaseSender, batch_endpoint_url, labels_endpoint_url
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ThreadBackgroundSender:
     def __init__(
         self,
         api_key: str,
         server_address: str,
-        model_name: str,
-        model_version: str,
         sender_queue: "queue.Queue[Any]",
         max_batch_size: int,
         max_batch_time: int,
         batch_sending_timeout: int,
     ):
         self.api_key = api_key
         self.server_address = server_address
-        self.base_event = model_base_event(model_name, model_version)
         self.sender_queue = sender_queue
         self.max_batch_time = max_batch_time
         self.batch = ThreadSafeBatch(max_batch_size, self.max_batch_time)
         self.session = get_http_session(retry_strategy=get_retry_strategy())
         self.batch_sending_timeout = batch_sending_timeout
 
         self.stop_processing = False
 
         # Pre-compute URLs
         self.batch_endpoint = batch_endpoint_url(self.server_address)
+        self.labels_endpoint = labels_endpoint_url(self.server_address)
 
     def run(self) -> None:
         """This is meant to be run in an independent Thread"""
         while self.stop_processing is False:
             stop = self._loop()
 
             if stop is True:
@@ -62,30 +66,50 @@
         # We force stop the processing of the queue
         self._check_batch_sending()
         return
 
     def _loop(self) -> bool:
         try:
             data = self.sender_queue.get(block=True, timeout=self.max_batch_time)
+            if data is None:
+                return False
 
-            if data:
-                if data is CLOSE_MESSAGE:
-                    self.stop_processing = True
-                    return True
-
-                to_send = self.base_event.copy()
-                to_send.update(data)
-                self.batch.append(to_send)
+            if data is CLOSE_MESSAGE:
+                self.stop_processing = True
+                return True
+
+            if isinstance(data, PredictionEvent):
+                self._process_prediction_event(event=data)
+            elif isinstance(data, LabelEvent):
+                self._process_label_event(event=data)
+            else:
+                LOGGER.error(UNEXPECTED_EVENT_TYPE, data)
         except queue.Empty:
             pass
 
         self._check_batch_sending()
 
         return False
 
+    def _process_label_event(self, event: LabelEvent) -> None:
+        try:
+            send_batch_requests(
+                self.session,
+                self.labels_endpoint,
+                api_key=self.api_key,
+                batch=event.create_event_dict(),
+                batch_sending_timeout=self.batch_sending_timeout,
+            )
+        except Exception:
+            LOGGER.error(LABEL_EVENT_SEND_ERROR, exc_info=True)
+
+    def _process_prediction_event(self, event: PredictionEvent) -> None:
+        to_send = event.create_event_dict()
+        self.batch.append(to_send)
+
     def _check_batch_sending(self) -> None:
         try:
             if self.batch.should_be_uploaded(self.stop_processing):
                 batch = self.batch.get_and_clear()
 
                 send_batch_requests(
                     self.session,
@@ -107,50 +131,44 @@
 
 
 class ThreadSender(BaseSender):
     def __init__(
         self,
         api_key: str,
         server_address: str,
-        model_name: str,
-        model_version: str,
         max_batch_size: int,
         max_batch_time: int,
         batch_sending_timeout: int,
     ) -> None:
         self.lock = Lock()
         self.sender_queue: Optional["queue.Queue[Any]"] = None
         self.background_sender: Optional[ThreadBackgroundSender] = None
         self.background_thread: Optional[Thread] = None
         self.drain = False
 
         self.api_key = api_key
         self.server_address = server_address
-        self.model_name = model_name
-        self.model_version = model_version
         self.max_batch_time = max_batch_time
         self.max_batch_size = max_batch_size
         self.batch_sending_timeout = batch_sending_timeout
 
     def _prepare(self) -> "queue.Queue[Any]":
         """We need to create the background thread on the first request to support application
         pre-loading.
         """
         if self.sender_queue is None:
             sender_queue: "queue.Queue[Any]" = queue.Queue()
             self.sender_queue = sender_queue
             self.background_sender = ThreadBackgroundSender(
-                self.api_key,
-                self.server_address,
-                self.model_name,
-                self.model_version,
-                self.sender_queue,
-                self.max_batch_size,
-                self.max_batch_time,
-                self.batch_sending_timeout,
+                api_key=self.api_key,
+                server_address=self.server_address,
+                sender_queue=self.sender_queue,
+                max_batch_size=self.max_batch_size,
+                max_batch_time=self.max_batch_time,
+                batch_sending_timeout=self.batch_sending_timeout,
             )
 
         if self.background_thread is None:
             assert self.background_sender is not None
             self.background_thread = Thread(
                 target=self.background_sender.run, daemon=True, name="ThreadSender"
             )
@@ -193,48 +211,40 @@
         do the handshake during Python import"""
         return None
 
 
 def get_thread_sender(
     api_key: str,
     server_address: str,
-    model_name: str,
-    model_version: str,
     max_batch_size: int,
     max_batch_time: int,
     batch_sending_timeout: int,
 ) -> "ThreadSender":
     sender = ThreadSender(
-        api_key,
-        server_address,
-        model_name,
-        model_version,
-        max_batch_size,
-        max_batch_time,
-        batch_sending_timeout,
+        api_key=api_key,
+        server_address=server_address,
+        max_batch_size=max_batch_size,
+        max_batch_time=max_batch_time,
+        batch_sending_timeout=batch_sending_timeout,
     )
 
     return sender
 
 
 def _get_thread_background_sender(
     api_key: str,
     server_address: str,
-    model_name: str,
-    model_version: str,
     max_batch_size: int,
     max_batch_time: int,
     batch_sending_timeout: int,
 ) -> Tuple["queue.Queue[Any]", "ThreadBackgroundSender"]:
     sender_queue: queue.Queue[Any] = queue.Queue()
     background_sender = ThreadBackgroundSender(
-        api_key,
-        server_address,
-        model_name,
-        model_version,
-        sender_queue,
-        max_batch_size,
-        max_batch_time,
-        batch_sending_timeout,
+        api_key=api_key,
+        server_address=server_address,
+        sender_queue=sender_queue,
+        max_batch_size=max_batch_size,
+        max_batch_time=max_batch_time,
+        batch_sending_timeout=batch_sending_timeout,
     )
 
     return sender_queue, background_sender
```

### Comparing `comet_mpm-0.3.2b0/src/comet_mpm/settings.py` & `comet_mpm-0.4.1/src/comet_mpm/settings.py`

 * *Files identical despite different names*

