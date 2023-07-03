# Comparing `tmp/spice_agent-0.1.3.tar.gz` & `tmp/spice_agent-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spice_agent-0.1.3.tar", max compression
+gzip compressed data, was "spice_agent-0.1.4.tar", max compression
```

## Comparing `spice_agent-0.1.3.tar` & `spice_agent-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1921 2023-07-02 23:55:30.254863 spice_agent-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/__init__.py
--rw-r--r--   0        0        0       22 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/__version__.py
--rw-r--r--   0        0        0        0 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/auth/__init__.py
--rw-r--r--   0        0        0     1024 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/auth/actions.py
--rw-r--r--   0        0        0     2761 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/auth/commands.py
--rw-r--r--   0        0        0     1869 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/cli.py
--rw-r--r--   0        0        0     5039 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/client.py
--rw-r--r--   0        0        0        0 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/daemons/__init__.py
--rw-r--r--   0        0        0     2500 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/daemons/actions.py
--rw-r--r--   0        0        0     1508 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/daemons/commands.py
--rw-r--r--   0        0        0     4302 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/daemons/launch_agents.py
--rw-r--r--   0        0        0     4982 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/daemons/launch_service.py
--rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/graphql/documents/__init__.py
--rw-r--r--   0        0        0     1196 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/graphql/documents/authentication.gql
--rw-r--r--   0        0        0     1504 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/graphql/sdk.py
--rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/hardware/__init__.py
--rw-r--r--   0        0        0     7844 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/hardware/actions.py
--rw-r--r--   0        0        0     1070 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/hardware/commands.py
--rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/inference/__init__.py
--rw-r--r--   0        0        0     6273 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/inference/actions.py
--rw-r--r--   0        0        0     1055 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/inference/commands.py
--rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/tests/__init__.py
--rw-r--r--   0        0        0      555 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/tests/test_version.py
--rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/training/__init__.py
--rw-r--r--   0        0        0    42091 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/training/actions.py
--rw-r--r--   0        0        0       97 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/training/commands.py
--rw-r--r--   0        0        0     7269 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/uploader/actions.py
--rw-r--r--   0        0        0     1823 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/utils/config.py
--rw-r--r--   0        0        0      252 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/utils/printer.py
--rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/utils/updates.py
--rw-r--r--   0        0        0     1437 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/utils/version.py
--rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/worker/__init__.py
--rw-r--r--   0        0        0     9335 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/worker/actions.py
--rw-r--r--   0        0        0      397 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/worker/commands.py
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 spice_agent-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1921 2023-07-03 00:07:24.260204 spice_agent-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/auth/__init__.py
+-rw-r--r--   0        0        0     1024 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/auth/actions.py
+-rw-r--r--   0        0        0     2761 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/auth/commands.py
+-rw-r--r--   0        0        0     1869 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/cli.py
+-rw-r--r--   0        0        0     5039 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/client.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/daemons/__init__.py
+-rw-r--r--   0        0        0     2500 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/daemons/actions.py
+-rw-r--r--   0        0        0     1508 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/daemons/commands.py
+-rw-r--r--   0        0        0     4302 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/daemons/launch_agents.py
+-rw-r--r--   0        0        0     4982 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/daemons/launch_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/graphql/documents/__init__.py
+-rw-r--r--   0        0        0     1196 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/graphql/documents/authentication.gql
+-rw-r--r--   0        0        0     1504 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/graphql/sdk.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/hardware/__init__.py
+-rw-r--r--   0        0        0     7844 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/hardware/actions.py
+-rw-r--r--   0        0        0     1070 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/hardware/commands.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/inference/__init__.py
+-rw-r--r--   0        0        0     6414 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/inference/actions.py
+-rw-r--r--   0        0        0     1055 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/inference/commands.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/tests/__init__.py
+-rw-r--r--   0        0        0      555 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/tests/test_version.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/training/__init__.py
+-rw-r--r--   0        0        0    42091 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/training/actions.py
+-rw-r--r--   0        0        0       97 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/training/commands.py
+-rw-r--r--   0        0        0     7269 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/uploader/actions.py
+-rw-r--r--   0        0        0     1907 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/utils/config.py
+-rw-r--r--   0        0        0      252 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/utils/printer.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/utils/updates.py
+-rw-r--r--   0        0        0     1437 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/utils/version.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/worker/__init__.py
+-rw-r--r--   0        0        0     9335 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/worker/actions.py
+-rw-r--r--   0        0        0      397 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/worker/commands.py
+-rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 spice_agent-0.1.4/PKG-INFO
```

### Comparing `spice_agent-0.1.3/pyproject.toml` & `spice_agent-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spice_agent"
-version = "0.1.3"
+version = "0.1.4"
 description = "spice agent"
 authors = ["Dylan Stein <dylan@spice.cloud>", "Ankush Patel <ankush@spice.cloud>"]
 license = ""
 
 [tool.poetry.dependencies]
 python = "^3.11.3"
 gql = "^3.4.1"
```

### Comparing `spice_agent-0.1.3/spice_agent/auth/actions.py` & `spice_agent-0.1.4/spice_agent/auth/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/auth/commands.py` & `spice_agent-0.1.4/spice_agent/auth/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/cli.py` & `spice_agent-0.1.4/spice_agent/cli.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/client.py` & `spice_agent-0.1.4/spice_agent/client.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/daemons/actions.py` & `spice_agent-0.1.4/spice_agent/daemons/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/daemons/commands.py` & `spice_agent-0.1.4/spice_agent/daemons/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/daemons/launch_agents.py` & `spice_agent-0.1.4/spice_agent/daemons/launch_agents.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/daemons/launch_service.py` & `spice_agent-0.1.4/spice_agent/daemons/launch_service.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/graphql/documents/authentication.gql` & `spice_agent-0.1.4/spice_agent/graphql/documents/authentication.gql`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/graphql/sdk.py` & `spice_agent-0.1.4/spice_agent/graphql/sdk.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/hardware/actions.py` & `spice_agent-0.1.4/spice_agent/hardware/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/hardware/commands.py` & `spice_agent-0.1.4/spice_agent/hardware/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/inference/actions.py` & `spice_agent-0.1.4/spice_agent/inference/actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from typing import Dict, Optional
 
 from diffusers import StableDiffusionPipeline
 from gql import gql
 from gql.transport.exceptions import TransportQueryError
 from torch.mps import empty_cache as mps_empty_cache
 
+from spice_agent.utils.config import SPICE_INFERENCE_DIRECTORY
+
 os.environ["PYTORCH_ENABLE_MPS_FALLBACK"] = "1"
 
 import torch  # noqa
 import transformers  # noqa
 from transformers import pipeline  # noqa
 from transformers.pipelines.base import PipelineException  # noqa
 
@@ -133,15 +135,16 @@
 
                 response = self._update_inference_job(
                     inference_job_id=inference_job_id,
                     status="SUCCESS",
                     text_output=json.dumps(result),
                 )
             elif is_text_input and is_file_output:
-                save_at = Path(Path.home() / "Downloads" / f"{inference_job_id}.png")
+                SPICE_INFERENCE_DIRECTORY.mkdir(parents=True, exist_ok=True)
+                save_at = Path(SPICE_INFERENCE_DIRECTORY / f"{inference_job_id}.png")
                 if not save_at.exists():
                     pipe = StableDiffusionPipeline.from_pretrained(
                         hf_model_repo_id, torch_dtype=torch.float32
                     )
                     pipe = pipe.to(self.device)  # type: ignore
                     result = pipe(text_input).images[0]  # type: ignore
                     result.save(save_at)
```

### Comparing `spice_agent-0.1.3/spice_agent/inference/commands.py` & `spice_agent-0.1.4/spice_agent/inference/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/tests/test_version.py` & `spice_agent-0.1.4/spice_agent/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/training/actions.py` & `spice_agent-0.1.4/spice_agent/training/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/uploader/actions.py` & `spice_agent-0.1.4/spice_agent/uploader/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/utils/config.py` & `spice_agent-0.1.4/spice_agent/utils/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import os
 from pathlib import Path
 import shutil
 from typing import Dict
 
 HOME_DIRECTORY = Path.home()
+SPICE_INFERENCE_DIRECTORY = Path(HOME_DIRECTORY / ".cache" / "spice" / "inference")
 SPICE_HOSTS_FILEPATH = Path(HOME_DIRECTORY / ".config" / "spice" / "hosts.json")
 SPICE_TRAINING_FILEPATH = Path(HOME_DIRECTORY / ".config" / "spice" / "training.json")
 SPICE_ROUND_VERIFICATION_FILEPATH = Path(
     HOME_DIRECTORY / ".config" / "spice" / "training-verification.json"
 )
 SPICE_MODEL_CACHE_FILEPATH = Path(HOME_DIRECTORY / ".cache" / "spice" / "models")
 HF_HUB_DIRECTORY = Path(HOME_DIRECTORY / ".cache" / "huggingface" / "hub")
```

### Comparing `spice_agent-0.1.3/spice_agent/utils/version.py` & `spice_agent-0.1.4/spice_agent/utils/version.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/spice_agent/worker/actions.py` & `spice_agent-0.1.4/spice_agent/worker/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.3/PKG-INFO` & `spice_agent-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spice-agent
-Version: 0.1.3
+Version: 0.1.4
 Summary: spice agent
 Author: Dylan Stein
 Author-email: dylan@spice.cloud
 Requires-Python: >=3.11.3,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: accelerate (>=0.20.3,<0.21.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
```

