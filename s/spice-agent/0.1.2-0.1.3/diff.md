# Comparing `tmp/spice_agent-0.1.2.tar.gz` & `tmp/spice_agent-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spice_agent-0.1.2.tar", max compression
+gzip compressed data, was "spice_agent-0.1.3.tar", max compression
```

## Comparing `spice_agent-0.1.2.tar` & `spice_agent-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1921 2023-07-02 23:21:31.164811 spice_agent-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/__init__.py
--rw-r--r--   0        0        0       22 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/__version__.py
--rw-r--r--   0        0        0        0 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/auth/__init__.py
--rw-r--r--   0        0        0     1024 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/auth/actions.py
--rw-r--r--   0        0        0     2761 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/auth/commands.py
--rw-r--r--   0        0        0     1869 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/cli.py
--rw-r--r--   0        0        0     5039 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/client.py
--rw-r--r--   0        0        0        0 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/daemons/__init__.py
--rw-r--r--   0        0        0     2500 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/daemons/actions.py
--rw-r--r--   0        0        0     1508 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/daemons/commands.py
--rw-r--r--   0        0        0     4302 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/daemons/launch_agents.py
--rw-r--r--   0        0        0     4982 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/daemons/launch_service.py
--rw-r--r--   0        0        0        0 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/graphql/documents/__init__.py
--rw-r--r--   0        0        0     1196 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/graphql/documents/authentication.gql
--rw-r--r--   0        0        0     1504 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/graphql/sdk.py
--rw-r--r--   0        0        0        0 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/hardware/__init__.py
--rw-r--r--   0        0        0     7844 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/hardware/actions.py
--rw-r--r--   0        0        0     1070 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/hardware/commands.py
--rw-r--r--   0        0        0        0 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/inference/__init__.py
--rw-r--r--   0        0        0     6273 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/inference/actions.py
--rw-r--r--   0        0        0     1055 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/inference/commands.py
--rw-r--r--   0        0        0        0 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/tests/__init__.py
--rw-r--r--   0        0        0      555 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/tests/test_version.py
--rw-r--r--   0        0        0        0 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/training/__init__.py
--rw-r--r--   0        0        0    42091 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/training/actions.py
--rw-r--r--   0        0        0       97 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/training/commands.py
--rw-r--r--   0        0        0     7269 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/uploader/actions.py
--rw-r--r--   0        0        0     1823 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/utils/config.py
--rw-r--r--   0        0        0      252 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/utils/printer.py
--rw-r--r--   0        0        0        0 2023-07-02 23:21:31.164811 spice_agent-0.1.2/spice_agent/utils/updates.py
--rw-r--r--   0        0        0     1437 2023-07-02 23:21:31.168811 spice_agent-0.1.2/spice_agent/utils/version.py
--rw-r--r--   0        0        0        0 2023-07-02 23:21:31.168811 spice_agent-0.1.2/spice_agent/worker/__init__.py
--rw-r--r--   0        0        0     9054 2023-07-02 23:21:31.168811 spice_agent-0.1.2/spice_agent/worker/actions.py
--rw-r--r--   0        0        0      397 2023-07-02 23:21:31.168811 spice_agent-0.1.2/spice_agent/worker/commands.py
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 spice_agent-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1921 2023-07-02 23:55:30.254863 spice_agent-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/auth/__init__.py
+-rw-r--r--   0        0        0     1024 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/auth/actions.py
+-rw-r--r--   0        0        0     2761 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/auth/commands.py
+-rw-r--r--   0        0        0     1869 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/cli.py
+-rw-r--r--   0        0        0     5039 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/client.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:55:30.254863 spice_agent-0.1.3/spice_agent/daemons/__init__.py
+-rw-r--r--   0        0        0     2500 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/daemons/actions.py
+-rw-r--r--   0        0        0     1508 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/daemons/commands.py
+-rw-r--r--   0        0        0     4302 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/daemons/launch_agents.py
+-rw-r--r--   0        0        0     4982 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/daemons/launch_service.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/graphql/documents/__init__.py
+-rw-r--r--   0        0        0     1196 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/graphql/documents/authentication.gql
+-rw-r--r--   0        0        0     1504 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/graphql/sdk.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/hardware/__init__.py
+-rw-r--r--   0        0        0     7844 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/hardware/actions.py
+-rw-r--r--   0        0        0     1070 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/hardware/commands.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/inference/__init__.py
+-rw-r--r--   0        0        0     6273 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/inference/actions.py
+-rw-r--r--   0        0        0     1055 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/inference/commands.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/tests/__init__.py
+-rw-r--r--   0        0        0      555 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/tests/test_version.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/training/__init__.py
+-rw-r--r--   0        0        0    42091 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/training/actions.py
+-rw-r--r--   0        0        0       97 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/training/commands.py
+-rw-r--r--   0        0        0     7269 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/uploader/actions.py
+-rw-r--r--   0        0        0     1823 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/utils/config.py
+-rw-r--r--   0        0        0      252 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/utils/printer.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/utils/updates.py
+-rw-r--r--   0        0        0     1437 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/utils/version.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/worker/__init__.py
+-rw-r--r--   0        0        0     9335 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/worker/actions.py
+-rw-r--r--   0        0        0      397 2023-07-02 23:55:30.258863 spice_agent-0.1.3/spice_agent/worker/commands.py
+-rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 spice_agent-0.1.3/PKG-INFO
```

### Comparing `spice_agent-0.1.2/pyproject.toml` & `spice_agent-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spice_agent"
-version = "0.1.2"
+version = "0.1.3"
 description = "spice agent"
 authors = ["Dylan Stein <dylan@spice.cloud>", "Ankush Patel <ankush@spice.cloud>"]
 license = ""
 
 [tool.poetry.dependencies]
 python = "^3.11.3"
 gql = "^3.4.1"
```

### Comparing `spice_agent-0.1.2/spice_agent/auth/actions.py` & `spice_agent-0.1.3/spice_agent/auth/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/auth/commands.py` & `spice_agent-0.1.3/spice_agent/auth/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/cli.py` & `spice_agent-0.1.3/spice_agent/cli.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/client.py` & `spice_agent-0.1.3/spice_agent/client.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/daemons/actions.py` & `spice_agent-0.1.3/spice_agent/daemons/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/daemons/commands.py` & `spice_agent-0.1.3/spice_agent/daemons/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/daemons/launch_agents.py` & `spice_agent-0.1.3/spice_agent/daemons/launch_agents.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/daemons/launch_service.py` & `spice_agent-0.1.3/spice_agent/daemons/launch_service.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/graphql/documents/authentication.gql` & `spice_agent-0.1.3/spice_agent/graphql/documents/authentication.gql`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/graphql/sdk.py` & `spice_agent-0.1.3/spice_agent/graphql/sdk.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/hardware/actions.py` & `spice_agent-0.1.3/spice_agent/hardware/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/hardware/commands.py` & `spice_agent-0.1.3/spice_agent/hardware/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/inference/actions.py` & `spice_agent-0.1.3/spice_agent/inference/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/inference/commands.py` & `spice_agent-0.1.3/spice_agent/inference/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/tests/test_version.py` & `spice_agent-0.1.3/spice_agent/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/training/actions.py` & `spice_agent-0.1.3/spice_agent/training/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/uploader/actions.py` & `spice_agent-0.1.3/spice_agent/uploader/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/utils/config.py` & `spice_agent-0.1.3/spice_agent/utils/config.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/utils/version.py` & `spice_agent-0.1.3/spice_agent/utils/version.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.2/spice_agent/worker/actions.py` & `spice_agent-0.1.3/spice_agent/worker/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,23 @@
             and not training_round_step_id
             and not training_round_id
         ):
             raise Exception(
                 f'No inference_job_id or training_round_step_id or training_round_id found in message body: {body.decode("utf-8")}'  # noqa
             )
 
+        message_acked = False
         if inference_job_id:
             result = self.spice.inference._update_inference_job(
                 inference_job_id=inference_job_id, status="CLAIMED"
             )
+            # ack message at inference level so another machine does not steal the
+            # message while inference is running
+            channel.basic_ack(delivery_tag=method.delivery_tag)
+            message_acked = True
             self.spice.inference.run_pipeline(inference_job_id=inference_job_id)
             LOGGER.info(" [*] Completed inference job.")
 
         if training_round_id:
             result = self.spice.training._update_training_round(
                 training_round_id=training_round_id, status="CLAIMED"
             )
@@ -104,15 +109,15 @@
         if training_round_step_id:
             result = self.spice.training._update_training_round_step(
                 training_round_step_id=training_round_step_id, status="CLAIMED"
             )
             if result is not None:
                 LOGGER.info(" [*] Obtained training round step.")
 
-        if channel.is_open:
+        if not message_acked and channel.is_open:
             channel.basic_ack(delivery_tag=method.delivery_tag)
         else:
             LOGGER.info(" [*] Channel closed already. Cannot ack message.")
 
         LOGGER.info(" [*] Stopping worker...")
         if self.channel:
             self.channel.stop_consuming()
```

### Comparing `spice_agent-0.1.2/PKG-INFO` & `spice_agent-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spice-agent
-Version: 0.1.2
+Version: 0.1.3
 Summary: spice agent
 Author: Dylan Stein
 Author-email: dylan@spice.cloud
 Requires-Python: >=3.11.3,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: accelerate (>=0.20.3,<0.21.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
```

