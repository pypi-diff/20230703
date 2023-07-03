# Comparing `tmp/spice_agent-0.1.4.tar.gz` & `tmp/spice_agent-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spice_agent-0.1.4.tar", max compression
+gzip compressed data, was "spice_agent-0.1.5.tar", max compression
```

## Comparing `spice_agent-0.1.4.tar` & `spice_agent-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1921 2023-07-03 00:07:24.260204 spice_agent-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/__init__.py
--rw-r--r--   0        0        0       22 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/__version__.py
--rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/auth/__init__.py
--rw-r--r--   0        0        0     1024 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/auth/actions.py
--rw-r--r--   0        0        0     2761 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/auth/commands.py
--rw-r--r--   0        0        0     1869 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/cli.py
--rw-r--r--   0        0        0     5039 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/client.py
--rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/daemons/__init__.py
--rw-r--r--   0        0        0     2500 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/daemons/actions.py
--rw-r--r--   0        0        0     1508 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/daemons/commands.py
--rw-r--r--   0        0        0     4302 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/daemons/launch_agents.py
--rw-r--r--   0        0        0     4982 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/daemons/launch_service.py
--rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/graphql/documents/__init__.py
--rw-r--r--   0        0        0     1196 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/graphql/documents/authentication.gql
--rw-r--r--   0        0        0     1504 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/graphql/sdk.py
--rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/hardware/__init__.py
--rw-r--r--   0        0        0     7844 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/hardware/actions.py
--rw-r--r--   0        0        0     1070 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/hardware/commands.py
--rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/inference/__init__.py
--rw-r--r--   0        0        0     6414 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/inference/actions.py
--rw-r--r--   0        0        0     1055 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/inference/commands.py
--rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/tests/__init__.py
--rw-r--r--   0        0        0      555 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/tests/test_version.py
--rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/training/__init__.py
--rw-r--r--   0        0        0    42091 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/training/actions.py
--rw-r--r--   0        0        0       97 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/training/commands.py
--rw-r--r--   0        0        0     7269 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/uploader/actions.py
--rw-r--r--   0        0        0     1907 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/utils/config.py
--rw-r--r--   0        0        0      252 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/utils/printer.py
--rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/utils/updates.py
--rw-r--r--   0        0        0     1437 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/utils/version.py
--rw-r--r--   0        0        0        0 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/worker/__init__.py
--rw-r--r--   0        0        0     9335 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/worker/actions.py
--rw-r--r--   0        0        0      397 2023-07-03 00:07:24.260204 spice_agent-0.1.4/spice_agent/worker/commands.py
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 spice_agent-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1921 2023-07-03 19:35:59.093040 spice_agent-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-03 19:35:59.093040 spice_agent-0.1.5/spice_agent/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-03 19:35:59.093040 spice_agent-0.1.5/spice_agent/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:35:59.093040 spice_agent-0.1.5/spice_agent/auth/__init__.py
+-rw-r--r--   0        0        0     1024 2023-07-03 19:35:59.093040 spice_agent-0.1.5/spice_agent/auth/actions.py
+-rw-r--r--   0        0        0     2761 2023-07-03 19:35:59.093040 spice_agent-0.1.5/spice_agent/auth/commands.py
+-rw-r--r--   0        0        0     1869 2023-07-03 19:35:59.093040 spice_agent-0.1.5/spice_agent/cli.py
+-rw-r--r--   0        0        0     5039 2023-07-03 19:35:59.093040 spice_agent-0.1.5/spice_agent/client.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:35:59.093040 spice_agent-0.1.5/spice_agent/daemons/__init__.py
+-rw-r--r--   0        0        0     2500 2023-07-03 19:35:59.093040 spice_agent-0.1.5/spice_agent/daemons/actions.py
+-rw-r--r--   0        0        0     1508 2023-07-03 19:35:59.093040 spice_agent-0.1.5/spice_agent/daemons/commands.py
+-rw-r--r--   0        0        0     4302 2023-07-03 19:35:59.093040 spice_agent-0.1.5/spice_agent/daemons/launch_agents.py
+-rw-r--r--   0        0        0     4982 2023-07-03 19:35:59.093040 spice_agent-0.1.5/spice_agent/daemons/launch_service.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:35:59.093040 spice_agent-0.1.5/spice_agent/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:35:59.093040 spice_agent-0.1.5/spice_agent/graphql/documents/__init__.py
+-rw-r--r--   0        0        0     1196 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/graphql/documents/authentication.gql
+-rw-r--r--   0        0        0     1504 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/graphql/sdk.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/hardware/__init__.py
+-rw-r--r--   0        0        0     7844 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/hardware/actions.py
+-rw-r--r--   0        0        0     1070 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/hardware/commands.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/inference/__init__.py
+-rw-r--r--   0        0        0     6417 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/inference/actions.py
+-rw-r--r--   0        0        0     1055 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/inference/commands.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/tests/__init__.py
+-rw-r--r--   0        0        0      555 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/tests/test_version.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/training/__init__.py
+-rw-r--r--   0        0        0    42091 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/training/actions.py
+-rw-r--r--   0        0        0       97 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/training/commands.py
+-rw-r--r--   0        0        0     7269 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/uploader/actions.py
+-rw-r--r--   0        0        0     1907 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/utils/config.py
+-rw-r--r--   0        0        0      252 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/utils/printer.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/utils/updates.py
+-rw-r--r--   0        0        0     1437 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/utils/version.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/worker/__init__.py
+-rw-r--r--   0        0        0     9335 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/worker/actions.py
+-rw-r--r--   0        0        0      397 2023-07-03 19:35:59.097041 spice_agent-0.1.5/spice_agent/worker/commands.py
+-rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 spice_agent-0.1.5/PKG-INFO
```

### Comparing `spice_agent-0.1.4/pyproject.toml` & `spice_agent-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spice_agent"
-version = "0.1.4"
+version = "0.1.5"
 description = "spice agent"
 authors = ["Dylan Stein <dylan@spice.cloud>", "Ankush Patel <ankush@spice.cloud>"]
 license = ""
 
 [tool.poetry.dependencies]
 python = "^3.11.3"
 gql = "^3.4.1"
```

### Comparing `spice_agent-0.1.4/spice_agent/auth/actions.py` & `spice_agent-0.1.5/spice_agent/auth/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/auth/commands.py` & `spice_agent-0.1.5/spice_agent/auth/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/cli.py` & `spice_agent-0.1.5/spice_agent/cli.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/client.py` & `spice_agent-0.1.5/spice_agent/client.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/daemons/actions.py` & `spice_agent-0.1.5/spice_agent/daemons/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/daemons/commands.py` & `spice_agent-0.1.5/spice_agent/daemons/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/daemons/launch_agents.py` & `spice_agent-0.1.5/spice_agent/daemons/launch_agents.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/daemons/launch_service.py` & `spice_agent-0.1.5/spice_agent/daemons/launch_service.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/graphql/documents/authentication.gql` & `spice_agent-0.1.5/spice_agent/graphql/documents/authentication.gql`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/graphql/sdk.py` & `spice_agent-0.1.5/spice_agent/graphql/sdk.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/hardware/actions.py` & `spice_agent-0.1.5/spice_agent/hardware/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/hardware/commands.py` & `spice_agent-0.1.5/spice_agent/hardware/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/inference/actions.py` & `spice_agent-0.1.5/spice_agent/inference/actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             if is_text_input and is_text_output:
                 result = None
                 pipe = pipeline(model=hf_model_repo_id, device=self.device)
                 result = pipe(text_input)
 
                 response = self._update_inference_job(
                     inference_job_id=inference_job_id,
-                    status="SUCCESS",
+                    status="COMPLETE",
                     text_output=json.dumps(result),
                 )
             elif is_text_input and is_file_output:
                 SPICE_INFERENCE_DIRECTORY.mkdir(parents=True, exist_ok=True)
                 save_at = Path(SPICE_INFERENCE_DIRECTORY / f"{inference_job_id}.png")
                 if not save_at.exists():
                     pipe = StableDiffusionPipeline.from_pretrained(
@@ -153,18 +153,18 @@
 
                 upload_file_response = self.spice.uploader.upload_file_via_api(
                     path=save_at
                 )
                 file_id = upload_file_response.json()["data"]["uploadFile"]["id"]
                 response = self._update_inference_job(
                     inference_job_id=inference_job_id,
-                    status="SUCCESS",
+                    status="COMPLETE",
                     file_outputs_ids=file_id,
                 )
-            LOGGER.info(f""" [*] SUCCESS. Result: " {result}""")
+            LOGGER.info(f""" [*] COMPLETE. Result: " {result}""")
             return response
         except PipelineException as exception:
             message = f"""Input: "{input}" threw exception: {exception}"""
             LOGGER.error(message)
             self._update_inference_job(
                 inference_job_id=inference_job_id,
                 status="ERROR",
```

### Comparing `spice_agent-0.1.4/spice_agent/inference/commands.py` & `spice_agent-0.1.5/spice_agent/inference/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/tests/test_version.py` & `spice_agent-0.1.5/spice_agent/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/training/actions.py` & `spice_agent-0.1.5/spice_agent/training/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/uploader/actions.py` & `spice_agent-0.1.5/spice_agent/uploader/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/utils/config.py` & `spice_agent-0.1.5/spice_agent/utils/config.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/utils/version.py` & `spice_agent-0.1.5/spice_agent/utils/version.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/spice_agent/worker/actions.py` & `spice_agent-0.1.5/spice_agent/worker/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.4/PKG-INFO` & `spice_agent-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spice-agent
-Version: 0.1.4
+Version: 0.1.5
 Summary: spice agent
 Author: Dylan Stein
 Author-email: dylan@spice.cloud
 Requires-Python: >=3.11.3,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: accelerate (>=0.20.3,<0.21.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
```

