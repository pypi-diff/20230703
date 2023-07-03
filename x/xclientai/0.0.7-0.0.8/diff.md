# Comparing `tmp/xclientai-0.0.7.tar.gz` & `tmp/xclientai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xclientai-0.0.7.tar", last modified: Tue Apr  4 09:17:40 2023, max compression
+gzip compressed data, was "xclientai-0.0.8.tar", last modified: Mon Jul  3 10:04:27 2023, max compression
```

## Comparing `xclientai-0.0.7.tar` & `xclientai-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,40 @@
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-04-04 09:17:40.022897 xclientai-0.0.7/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      493 2023-04-04 09:17:40.018897 xclientai-0.0.7/PKG-INFO
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       38 2023-04-04 09:17:40.022897 xclientai-0.0.7/setup.cfg
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1482 2023-03-10 11:15:42.000000 xclientai-0.0.7/setup.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-04-04 09:17:40.018897 xclientai-0.0.7/src/
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-04-04 09:17:40.018897 xclientai-0.0.7/src/xclientai/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       21 2023-04-04 09:17:38.000000 xclientai-0.0.7/src/xclientai/__about__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      762 2023-04-03 12:15:57.000000 xclientai-0.0.7/src/xclientai/__init__.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-04-04 09:17:40.018897 xclientai-0.0.7/src/xclientai/clients/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-31 10:27:39.000000 xclientai-0.0.7/src/xclientai/clients/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2847 2023-03-31 11:15:41.000000 xclientai-0.0.7/src/xclientai/clients/acceleration_jobs.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3635 2023-04-03 12:47:58.000000 xclientai-0.0.7/src/xclientai/clients/deployments.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2525 2023-03-31 18:56:22.000000 xclientai-0.0.7/src/xclientai/clients/executor_jobs.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      741 2023-04-03 12:27:23.000000 xclientai-0.0.7/src/xclientai/config.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-04-04 09:17:40.018897 xclientai-0.0.7/src/xclientai/dtypes/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-31 10:26:50.000000 xclientai-0.0.7/src/xclientai/dtypes/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1862 2023-04-04 09:17:00.000000 xclientai-0.0.7/src/xclientai/dtypes/deployments.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3136 2023-04-01 08:10:51.000000 xclientai-0.0.7/src/xclientai/dtypes/executor.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6207 2023-03-31 10:22:38.000000 xclientai-0.0.7/src/xclientai/dtypes/optimization.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1471 2023-04-04 09:17:23.000000 xclientai-0.0.7/src/xclientai/dtypes/shared.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-04-04 09:17:40.018897 xclientai-0.0.7/src/xclientai/utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-02 11:06:10.000000 xclientai-0.0.7/src/xclientai/utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1769 2023-03-31 10:27:00.000000 xclientai-0.0.7/src/xclientai/utils/logging.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1232 2023-03-31 10:27:08.000000 xclientai-0.0.7/src/xclientai/utils/requests_utils.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-04-04 09:17:40.018897 xclientai-0.0.7/src/xclientai.egg-info/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      493 2023-04-04 09:17:39.000000 xclientai-0.0.7/src/xclientai.egg-info/PKG-INFO
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      693 2023-04-04 09:17:39.000000 xclientai-0.0.7/src/xclientai.egg-info/SOURCES.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        1 2023-04-04 09:17:39.000000 xclientai-0.0.7/src/xclientai.egg-info/dependency_links.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       49 2023-04-04 09:17:39.000000 xclientai-0.0.7/src/xclientai.egg-info/requires.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       10 2023-04-04 09:17:39.000000 xclientai-0.0.7/src/xclientai.egg-info/top_level.txt
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-03 10:04:27.881006 xclientai-0.0.8/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      493 2023-07-03 10:04:27.881006 xclientai-0.0.8/PKG-INFO
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       38 2023-07-03 10:04:27.881006 xclientai-0.0.8/setup.cfg
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1605 2023-06-02 13:05:15.000000 xclientai-0.0.8/setup.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-03 10:04:27.877006 xclientai-0.0.8/src/
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-03 10:04:27.877006 xclientai-0.0.8/src/xclientai/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       21 2023-07-03 10:04:26.000000 xclientai-0.0.8/src/xclientai/__about__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      857 2023-05-19 16:17:02.000000 xclientai-0.0.8/src/xclientai/__init__.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-03 10:04:27.877006 xclientai-0.0.8/src/xclientai/cli/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      388 2023-06-01 16:15:01.000000 xclientai-0.0.8/src/xclientai/cli/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1170 2023-06-02 14:11:10.000000 xclientai-0.0.8/src/xclientai/cli/configure.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-03 10:04:27.877006 xclientai-0.0.8/src/xclientai/clients/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-31 10:27:39.000000 xclientai-0.0.8/src/xclientai/clients/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2847 2023-04-06 11:29:37.000000 xclientai-0.0.8/src/xclientai/clients/acceleration_jobs.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4888 2023-06-02 14:16:58.000000 xclientai-0.0.8/src/xclientai/clients/deployments.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3591 2023-06-02 14:17:25.000000 xclientai-0.0.8/src/xclientai/clients/executor_jobs.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1030 2023-07-03 09:23:48.000000 xclientai-0.0.8/src/xclientai/config.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-03 10:04:27.881006 xclientai-0.0.8/src/xclientai/dtypes/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-31 10:26:50.000000 xclientai-0.0.8/src/xclientai/dtypes/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3663 2023-06-23 13:11:38.000000 xclientai-0.0.8/src/xclientai/dtypes/deployments.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1458 2023-05-24 16:27:54.000000 xclientai-0.0.8/src/xclientai/dtypes/executor.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6398 2023-05-19 12:29:40.000000 xclientai-0.0.8/src/xclientai/dtypes/optimization.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3531 2023-05-24 16:14:21.000000 xclientai-0.0.8/src/xclientai/dtypes/shared.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-03 10:04:27.881006 xclientai-0.0.8/src/xclientai/inference_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-05-19 12:29:40.000000 xclientai-0.0.8/src/xclientai/inference_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      104 2023-05-19 12:29:40.000000 xclientai-0.0.8/src/xclientai/inference_utils/inference_utils.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-03 10:04:27.881006 xclientai-0.0.8/src/xclientai/utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-03-02 11:06:10.000000 xclientai-0.0.8/src/xclientai/utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1029 2023-06-02 13:13:29.000000 xclientai-0.0.8/src/xclientai/utils/config_utils.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1769 2023-03-31 10:27:00.000000 xclientai-0.0.8/src/xclientai/utils/logging.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2655 2023-06-08 12:32:20.000000 xclientai-0.0.8/src/xclientai/utils/requests_utils.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      794 2023-06-02 14:09:40.000000 xclientai-0.0.8/src/xclientai/utils/validations.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      863 2023-05-19 14:31:28.000000 xclientai-0.0.8/src/xclientai/utils/zip_files.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-03 10:04:27.877006 xclientai-0.0.8/src/xclientai.egg-info/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      493 2023-07-03 10:04:27.000000 xclientai-0.0.8/src/xclientai.egg-info/PKG-INFO
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      989 2023-07-03 10:04:27.000000 xclientai-0.0.8/src/xclientai.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        1 2023-07-03 10:04:27.000000 xclientai-0.0.8/src/xclientai.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       48 2023-07-03 10:04:27.000000 xclientai-0.0.8/src/xclientai.egg-info/entry_points.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       62 2023-07-03 10:04:27.000000 xclientai-0.0.8/src/xclientai.egg-info/requires.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       10 2023-07-03 10:04:27.000000 xclientai-0.0.8/src/xclientai.egg-info/top_level.txt
```

### Comparing `xclientai-0.0.7/setup.py` & `xclientai-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,28 +31,35 @@
 print("NEW VERSION: {}".format(str(version)))
 
 install_requires = [
    "setuptools",
    "pydantic",
    "numpy",
    "requests",
-   "python-dotenv"
+   "python-dotenv",
+   "kserve",
+   "click"
 ]
 
 
 setuptools.setup(
    name='xclientai',
    version=str(version),
    author='Marcos Rivera Martínez, Sarthak Langde, Glenn Ko, Subhash G N, Toan Do, Roman Ageev',
    author_email='marcos.rm@stochastic.ai, sarthak.langde@stochastic.ai, glenn@stochastic.ai, subhash.gn@stochastic.ai',
    description='',
    long_description_content_type="text/markdown",
    url="",
    classifiers=[
-        "Programming Language :: Python :: 3",
-        "Operating System :: OS Independent"
+      "Programming Language :: Python :: 3",
+      "Operating System :: OS Independent"
    ],
    package_dir={"": "src"},
    packages=setuptools.find_packages(where="src"),
    python_requires=">=3.6",
-   install_requires=install_requires
+   install_requires=install_requires,
+   entry_points={
+      "console_scripts": [
+         "xcloud = xclientai.cli:xcloud"
+      ]
+   }  
 )
```

### Comparing `xclientai-0.0.7/src/xclientai/__init__.py` & `xclientai-0.0.8/src/xclientai/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from xclientai.__about__ import __version__
 
 from xclientai.dtypes.shared import (
     Status,
     Credentials,
-    Instance
+    MachineType
 )
 
 from xclientai.dtypes.optimization import (
     Signature,
     BenchmarkConfig,
     Accelerator,
     BenchmarkResults,
@@ -15,22 +15,26 @@
     AccelerationInfo,
     Notification,
     AccelerationJob
 )
 
 from xclientai.dtypes.executor import (
     ExecutionJob,
-    ContainerExecutionSpecs,
-    PythonExecutionSpecs
+    ExecutionContainerSpecs,
+    CodeSpecs
 )
 
 from xclientai.dtypes.deployments import (
     ModelSpecs,
     Batcher,
     Scaling,
+    SCALE_METRIC,
     DeploymentSpecs,
-    Deployment
+    Deployment,
+    DeploymentContainerSpecs
 )
 
+from xclientai.inference_utils import inference_utils
+
 from xclientai.clients.acceleration_jobs import AccelerationJobsClient
 from xclientai.clients.executor_jobs import ExecutionJobsClient
 from xclientai.clients.deployments import DeploymentsClient
```

### Comparing `xclientai-0.0.7/src/xclientai/clients/acceleration_jobs.py` & `xclientai-0.0.8/src/xclientai/clients/acceleration_jobs.py`

 * *Files identical despite different names*

### Comparing `xclientai-0.0.7/src/xclientai/config.py` & `xclientai-0.0.8/src/xclientai/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,26 @@
 # IMPORTANT: dont import logger here (circular import)
 
 env_path = find_dotenv()
 load_dotenv(env_path)
 
 
 class Config:
+    DEBUG = os.getenv("DEBUG", "false").lower() in ('true', '1', 't')
     ACCELERATION_BASE_URL_X_BACKEND = os.environ.get(
         "ACCELERATION_BASE_URL_X_BACKEND", 
-        "https://xcloud-api.stochastic.ai/backend"
+        "https://xcloud-api.stochastic.ai/acceleron/backend"
     )
     EXECUTION_BASE_URL_X_BACKEND = os.environ.get(
         "EXECUTION_BASE_URL_X_BACKEND", 
         "https://xcloud-api.stochastic.ai/executor/backend"
     )
     DEPLOYMENTS_BASE_URL_X_BACKEND = os.environ.get(
         "DEPLOYMENTS_BASE_URL_X_BACKEND", 
-        "https://xcloud-api.stochastic.ai/xinference/backend"
+        "https://xcloud-api.stochastic.ai/inference/backend"
     )
-    PANEL_DOMAIN = "https://xcloud.stochastic.ai"
+    PANEL_DOMAIN = "https://xcloud.stochastic.ai"
+    AUTH_BASE_URL_X_BACKEND = os.environ.get(
+        "AUTH_BASE_URL_X_BACKEND", 
+        "https://xcloud-api.stochastic.ai/auth/backend"
+    )
+    XCLOUD_CONFIG_PATH: Path = Path.home() / ".xcloud" / "config"
```

### Comparing `xclientai-0.0.7/src/xclientai/dtypes/optimization.py` & `xclientai-0.0.8/src/xclientai/dtypes/optimization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Any, Dict, Optional
 from pydantic import BaseModel, validator
 import numpy as np
 import re
-from xclientai.dtypes.shared import Status, Credentials
+from xclientai.dtypes.shared import Status, Credentials, MachineType
 from xclientai.utils.logging import configure_logger
 from xclientai.config import Config
 from urllib.parse import urlparse
 
 
 logger = configure_logger(__name__)
 
@@ -153,21 +153,25 @@
 
 
 class NotificationResult(BaseModel):
     type: str
     message: str
     status_code: int
 
+class AccelerationContainerSpecs(BaseModel):
+    machine_type: MachineType = MachineType.GPU_T4_1
+    spot: Optional[bool] = True
 
 class AccelerationJob(BaseModel):
     job_name: str
     status: Status = Status.NOT_STARTED
     panel_url: Optional[str]
     error: Optional[str]
     notification_result: Optional[NotificationResult]
+    container_specs: AccelerationContainerSpecs
     credentials: Credentials
     acceleration: AccelerationInfo
     benchmark: BenchmarkInfo = None
     notification: Notification = None
     started: Optional[int]
     ended: Optional[int]
```

### Comparing `xclientai-0.0.7/src/xclientai/utils/logging.py` & `xclientai-0.0.8/src/xclientai/utils/logging.py`

 * *Files identical despite different names*

### Comparing `xclientai-0.0.7/src/xclientai.egg-info/SOURCES.txt` & `xclientai-0.0.8/src/xclientai.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 setup.py
 src/xclientai/__about__.py
 src/xclientai/__init__.py
 src/xclientai/config.py
 src/xclientai.egg-info/PKG-INFO
 src/xclientai.egg-info/SOURCES.txt
 src/xclientai.egg-info/dependency_links.txt
+src/xclientai.egg-info/entry_points.txt
 src/xclientai.egg-info/requires.txt
 src/xclientai.egg-info/top_level.txt
+src/xclientai/cli/__init__.py
+src/xclientai/cli/configure.py
 src/xclientai/clients/__init__.py
 src/xclientai/clients/acceleration_jobs.py
 src/xclientai/clients/deployments.py
 src/xclientai/clients/executor_jobs.py
 src/xclientai/dtypes/__init__.py
 src/xclientai/dtypes/deployments.py
 src/xclientai/dtypes/executor.py
 src/xclientai/dtypes/optimization.py
 src/xclientai/dtypes/shared.py
+src/xclientai/inference_utils/__init__.py
+src/xclientai/inference_utils/inference_utils.py
 src/xclientai/utils/__init__.py
+src/xclientai/utils/config_utils.py
 src/xclientai/utils/logging.py
-src/xclientai/utils/requests_utils.py
+src/xclientai/utils/requests_utils.py
+src/xclientai/utils/validations.py
+src/xclientai/utils/zip_files.py
```

