# Comparing `tmp/spice_agent-0.1.6.tar.gz` & `tmp/spice_agent-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spice_agent-0.1.6.tar", max compression
+gzip compressed data, was "spice_agent-0.1.7.tar", max compression
```

## Comparing `spice_agent-0.1.6.tar` & `spice_agent-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1921 2023-07-03 19:56:20.522660 spice_agent-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/__init__.py
--rw-r--r--   0        0        0       22 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/__version__.py
--rw-r--r--   0        0        0        0 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/auth/__init__.py
--rw-r--r--   0        0        0     1024 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/auth/actions.py
--rw-r--r--   0        0        0     2761 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/auth/commands.py
--rw-r--r--   0        0        0     1869 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/cli.py
--rw-r--r--   0        0        0     5039 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/client.py
--rw-r--r--   0        0        0        0 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/daemons/__init__.py
--rw-r--r--   0        0        0     2500 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/daemons/actions.py
--rw-r--r--   0        0        0     1508 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/daemons/commands.py
--rw-r--r--   0        0        0     4302 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/daemons/launch_agents.py
--rw-r--r--   0        0        0     4982 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/daemons/launch_service.py
--rw-r--r--   0        0        0        0 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/graphql/documents/__init__.py
--rw-r--r--   0        0        0     1196 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/graphql/documents/authentication.gql
--rw-r--r--   0        0        0     1504 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/graphql/sdk.py
--rw-r--r--   0        0        0        0 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/hardware/__init__.py
--rw-r--r--   0        0        0     7844 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/hardware/actions.py
--rw-r--r--   0        0        0     1070 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/hardware/commands.py
--rw-r--r--   0        0        0        0 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/inference/__init__.py
--rw-r--r--   0        0        0     6417 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/inference/actions.py
--rw-r--r--   0        0        0     1055 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/inference/commands.py
--rw-r--r--   0        0        0        0 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/tests/__init__.py
--rw-r--r--   0        0        0      555 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/tests/test_version.py
--rw-r--r--   0        0        0        0 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/training/__init__.py
--rw-r--r--   0        0        0    42091 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/training/actions.py
--rw-r--r--   0        0        0       97 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/training/commands.py
--rw-r--r--   0        0        0     7269 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/uploader/actions.py
--rw-r--r--   0        0        0     1907 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/utils/config.py
--rw-r--r--   0        0        0      252 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/utils/printer.py
--rw-r--r--   0        0        0        0 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/utils/updates.py
--rw-r--r--   0        0        0     1437 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/utils/version.py
--rw-r--r--   0        0        0        0 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/worker/__init__.py
--rw-r--r--   0        0        0     9389 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/worker/actions.py
--rw-r--r--   0        0        0      397 2023-07-03 19:56:20.522660 spice_agent-0.1.6/spice_agent/worker/commands.py
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 spice_agent-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1921 2023-07-03 20:15:53.366214 spice_agent-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/auth/__init__.py
+-rw-r--r--   0        0        0     1024 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/auth/actions.py
+-rw-r--r--   0        0        0     2761 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/auth/commands.py
+-rw-r--r--   0        0        0     1869 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/cli.py
+-rw-r--r--   0        0        0     5039 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/client.py
+-rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/daemons/__init__.py
+-rw-r--r--   0        0        0     2500 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/daemons/actions.py
+-rw-r--r--   0        0        0     1508 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/daemons/commands.py
+-rw-r--r--   0        0        0     4302 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/daemons/launch_agents.py
+-rw-r--r--   0        0        0     4982 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/daemons/launch_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/graphql/documents/__init__.py
+-rw-r--r--   0        0        0     1196 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/graphql/documents/authentication.gql
+-rw-r--r--   0        0        0     1504 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/graphql/sdk.py
+-rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/hardware/__init__.py
+-rw-r--r--   0        0        0     7954 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/hardware/actions.py
+-rw-r--r--   0        0        0     1070 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/hardware/commands.py
+-rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/inference/__init__.py
+-rw-r--r--   0        0        0     6417 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/inference/actions.py
+-rw-r--r--   0        0        0     1055 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/inference/commands.py
+-rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/tests/__init__.py
+-rw-r--r--   0        0        0      555 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/tests/test_version.py
+-rw-r--r--   0        0        0        0 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/training/__init__.py
+-rw-r--r--   0        0        0    42091 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/training/actions.py
+-rw-r--r--   0        0        0       97 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/training/commands.py
+-rw-r--r--   0        0        0     7269 2023-07-03 20:15:53.366214 spice_agent-0.1.7/spice_agent/uploader/actions.py
+-rw-r--r--   0        0        0     1907 2023-07-03 20:15:53.370214 spice_agent-0.1.7/spice_agent/utils/config.py
+-rw-r--r--   0        0        0      252 2023-07-03 20:15:53.370214 spice_agent-0.1.7/spice_agent/utils/printer.py
+-rw-r--r--   0        0        0        0 2023-07-03 20:15:53.370214 spice_agent-0.1.7/spice_agent/utils/updates.py
+-rw-r--r--   0        0        0     1437 2023-07-03 20:15:53.370214 spice_agent-0.1.7/spice_agent/utils/version.py
+-rw-r--r--   0        0        0        0 2023-07-03 20:15:53.370214 spice_agent-0.1.7/spice_agent/worker/__init__.py
+-rw-r--r--   0        0        0     9500 2023-07-03 20:15:53.370214 spice_agent-0.1.7/spice_agent/worker/actions.py
+-rw-r--r--   0        0        0      397 2023-07-03 20:15:53.370214 spice_agent-0.1.7/spice_agent/worker/commands.py
+-rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 spice_agent-0.1.7/PKG-INFO
```

### Comparing `spice_agent-0.1.6/pyproject.toml` & `spice_agent-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spice_agent"
-version = "0.1.6"
+version = "0.1.7"
 description = "spice agent"
 authors = ["Dylan Stein <dylan@spice.cloud>", "Ankush Patel <ankush@spice.cloud>"]
 license = ""
 
 [tool.poetry.dependencies]
 python = "^3.11.3"
 gql = "^3.4.1"
```

### Comparing `spice_agent-0.1.6/spice_agent/auth/actions.py` & `spice_agent-0.1.7/spice_agent/auth/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/auth/commands.py` & `spice_agent-0.1.7/spice_agent/auth/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/cli.py` & `spice_agent-0.1.7/spice_agent/cli.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/client.py` & `spice_agent-0.1.7/spice_agent/client.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/daemons/actions.py` & `spice_agent-0.1.7/spice_agent/daemons/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/daemons/commands.py` & `spice_agent-0.1.7/spice_agent/daemons/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/daemons/launch_agents.py` & `spice_agent-0.1.7/spice_agent/daemons/launch_agents.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/daemons/launch_service.py` & `spice_agent-0.1.7/spice_agent/daemons/launch_service.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/graphql/documents/authentication.gql` & `spice_agent-0.1.7/spice_agent/graphql/documents/authentication.gql`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/graphql/sdk.py` & `spice_agent-0.1.7/spice_agent/graphql/sdk.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/hardware/actions.py` & `spice_agent-0.1.7/spice_agent/hardware/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import csv
 import io
 import json
+import logging
 import platform
 import subprocess
 from typing import Dict
 
 from aiohttp import client_exceptions
 from gql import gql
 
 from spice_agent.utils.config import (
     SPICE_TRAINING_FILEPATH,
     read_config_file,
     update_config_file,
 )
 
+LOGGER = logging.getLogger(__name__)
+
 
 class Hardware:
     def __init__(self, spice) -> None:
         self.spice = spice
 
     def get_darwin_system_profiler_values(self) -> Dict[str, str]:
         system_profiler_hardware_data_type = subprocess.check_output(
@@ -189,12 +192,13 @@
             "isHealthy": is_healthy,
             "isQuarantined": is_quarantined,
             "isAvailable": is_available,
         }
         variables = {"input": input}
         try:
             result = self.spice.session.execute(mutation, variable_values=variables)
+            LOGGER.info(" [*] Checked in successfully.")
             return result
         except client_exceptions.ClientConnectorError:
             config = read_config_file(filepath=SPICE_TRAINING_FILEPATH)
             if config.get("status") in self.spice.worker.ACTIVE_STATUSES:
                 return None
```

### Comparing `spice_agent-0.1.6/spice_agent/hardware/commands.py` & `spice_agent-0.1.7/spice_agent/hardware/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/inference/actions.py` & `spice_agent-0.1.7/spice_agent/inference/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/inference/commands.py` & `spice_agent-0.1.7/spice_agent/inference/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/tests/test_version.py` & `spice_agent-0.1.7/spice_agent/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/training/actions.py` & `spice_agent-0.1.7/spice_agent/training/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/uploader/actions.py` & `spice_agent-0.1.7/spice_agent/uploader/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/utils/config.py` & `spice_agent-0.1.7/spice_agent/utils/config.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/utils/version.py` & `spice_agent-0.1.7/spice_agent/utils/version.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.6/spice_agent/worker/actions.py` & `spice_agent-0.1.7/spice_agent/worker/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from retry import retry
 
 from spice_agent.utils.config import (
     SPICE_ROUND_VERIFICATION_FILEPATH,
     SPICE_TRAINING_FILEPATH,
     read_config_file,
 )
+from spice_agent.utils.version import get_current_version
 
 os.environ["PYTORCH_ENABLE_MPS_FALLBACK"] = "1"
 
 import transformers  # noqa
 
 LOGGER = logging.getLogger(__name__)
 
@@ -186,15 +187,16 @@
                 self.channel.stop_consuming()
                 self.channel.close()
                 self.channel = None
             self.spice.hardware.check_in_http(is_available=False)
             raise exception
 
     def start(self):
-        LOGGER.info(" [*] ✨ Starting Spice Worker")
+        LOGGER.info(" [*] ✨ spice worker")
+        LOGGER.info(f" [*] Version: {get_current_version()}")
         try:
             while True:
                 self.spice.hardware.check_in_http(is_available=True)
 
                 # check if this machine picked up a training round already
                 training_config = read_config_file(filepath=SPICE_TRAINING_FILEPATH)
```

### Comparing `spice_agent-0.1.6/PKG-INFO` & `spice_agent-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spice-agent
-Version: 0.1.6
+Version: 0.1.7
 Summary: spice agent
 Author: Dylan Stein
 Author-email: dylan@spice.cloud
 Requires-Python: >=3.11.3,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: accelerate (>=0.20.3,<0.21.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
```

