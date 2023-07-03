# Comparing `tmp/chaostoolkit-terraform-0.0.7.tar.gz` & `tmp/chaostoolkit-terraform-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaostoolkit-terraform-0.0.7.tar", last modified: Fri Jun  2 18:16:50 2023, max compression
+gzip compressed data, was "chaostoolkit-terraform-0.0.8.tar", last modified: Mon Jul  3 12:57:10 2023, max compression
```

## Comparing `chaostoolkit-terraform-0.0.7.tar` & `chaostoolkit-terraform-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 18:16:50.943037 chaostoolkit-terraform-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (122)    34524 2023-06-02 18:16:32.000000 chaostoolkit-terraform-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4437 2023-06-02 18:16:50.943037 chaostoolkit-terraform-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-06-02 18:16:32.000000 chaostoolkit-terraform-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 18:16:50.939037 chaostoolkit-terraform-0.0.7/chaosterraform/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-02 18:16:45.000000 chaostoolkit-terraform-0.0.7/chaosterraform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3399 2023-06-02 18:16:32.000000 chaostoolkit-terraform-0.0.7/chaosterraform/control.py
--rw-r--r--   0 runner    (1001) docker     (122)     4606 2023-06-02 18:16:32.000000 chaostoolkit-terraform-0.0.7/chaosterraform/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 18:16:50.943037 chaostoolkit-terraform-0.0.7/chaostoolkit_terraform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4437 2023-06-02 18:16:50.000000 chaostoolkit-terraform-0.0.7/chaostoolkit_terraform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-02 18:16:50.000000 chaostoolkit-terraform-0.0.7/chaostoolkit_terraform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 18:16:50.000000 chaostoolkit-terraform-0.0.7/chaostoolkit_terraform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-02 18:16:50.000000 chaostoolkit-terraform-0.0.7/chaostoolkit_terraform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-02 18:16:50.000000 chaostoolkit-terraform-0.0.7/chaostoolkit_terraform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-02 18:16:45.000000 chaostoolkit-terraform-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 18:16:50.943037 chaostoolkit-terraform-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 18:16:50.943037 chaostoolkit-terraform-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-06-02 18:16:32.000000 chaostoolkit-terraform-0.0.7/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (122)     2715 2023-06-02 18:16:32.000000 chaostoolkit-terraform-0.0.7/tests/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-06-02 18:16:32.000000 chaostoolkit-terraform-0.0.7/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 12:57:10.596165 chaostoolkit-terraform-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (122)    34524 2023-07-03 12:56:47.000000 chaostoolkit-terraform-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4793 2023-07-03 12:57:10.596165 chaostoolkit-terraform-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4504 2023-07-03 12:56:47.000000 chaostoolkit-terraform-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 12:57:10.592165 chaostoolkit-terraform-0.0.8/chaosterraform/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-03 12:57:04.000000 chaostoolkit-terraform-0.0.8/chaosterraform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4183 2023-07-03 12:56:47.000000 chaostoolkit-terraform-0.0.8/chaosterraform/control.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4788 2023-07-03 12:56:47.000000 chaostoolkit-terraform-0.0.8/chaosterraform/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 12:57:10.592165 chaostoolkit-terraform-0.0.8/chaostoolkit_terraform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4793 2023-07-03 12:57:10.000000 chaostoolkit-terraform-0.0.8/chaostoolkit_terraform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-03 12:57:10.000000 chaostoolkit-terraform-0.0.8/chaostoolkit_terraform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 12:57:10.000000 chaostoolkit-terraform-0.0.8/chaostoolkit_terraform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 12:57:10.000000 chaostoolkit-terraform-0.0.8/chaostoolkit_terraform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-03 12:57:10.000000 chaostoolkit-terraform-0.0.8/chaostoolkit_terraform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-03 12:57:04.000000 chaostoolkit-terraform-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 12:57:10.596165 chaostoolkit-terraform-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 12:57:10.596165 chaostoolkit-terraform-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4243 2023-07-03 12:56:47.000000 chaostoolkit-terraform-0.0.8/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2715 2023-07-03 12:56:47.000000 chaostoolkit-terraform-0.0.8/tests/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-07-03 12:56:47.000000 chaostoolkit-terraform-0.0.8/tests/test_version.py
```

### Comparing `chaostoolkit-terraform-0.0.7/LICENSE` & `chaostoolkit-terraform-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chaostoolkit-terraform-0.0.7/PKG-INFO` & `chaostoolkit-terraform-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-terraform
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Chaos Toolkit module to deploy terraform stacks
 Author: Manuel Castellin
 Project-URL: homepage, https://github.com/mcastellin/chaostoolkit-terraform
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# chaostoolkit-terraform
+# ChaosToolkit Terraform
 
 A [Chaos Toolkit](https://chaostoolkit.org/) driver to extend chaos experiments with [Terraform](https://www.terraform.io/)
 
 ## Package Installation
 
 ### From Python package index
 
@@ -71,15 +71,15 @@
       type: python
       module: chaosterraform.control
       arguments:
         silent: false
         retain: true
 ```
 
-**Configuration using Ctk parameters**
+**Configuration using Chaos Toolkit parameters**
 ```yaml
 configuration:
 # parameters prefixed with `tf_conf__` will configure chaosterraform driver
   tf_conf__silent: false
   tf_conf__retain: true
 
 controls:
@@ -95,34 +95,50 @@
 
 | Parameter Name        | Usage |
 | --------------------- | ------- |
 | **silent** | Suppress Terraform console output to avoid verbose experiment logs, defaults to `true`|
 | **retain** | Do not run `terraform destroy` at the end of the experiment to retain resources, defaults to `false` |
 | **chdir** | Instruct Terraform to change its working directory before running subcommands |
 
-## Set Terraform Input Variables
+## Provide Input Variables for Terraform
 
-You can override input variables defined in the Terraform module from within the experiment using
-Chaos Toolkit configuration parameters prefixed by `tf__`:
+You can override input variables defined in the Terraform module from within the experiment using the `variables`
+argument for the control:
+
+```yaml
+controls:
+  - name: "Deploy Terraform module"
+    provider:
+      type: python
+      module: chaosterraform.control
+      arguments:
+        variables:
+          vpc_id: "vpc-0000000000"
+          number_of_azs: 2
+```
+
+Alternatively, you can supply input variables from Chaos Toolkit configuration by referencing a parameter name
+already defined in Chaos Toolkit configuration:
 
 ```yaml
 configuration:
-# parameters prefixed with `tf__` will set terraform input variables for the module
-  tf__vpc_id: "vpc-0000000000"
-  tf__number_of_azs: 2
+  env_name: "live"
   ...
 
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
       module: chaosterraform.control
+      arguments:
+        variables:
+          environment:
+            name: "env_name"
 ```
 
-
 ## Use Terraform Outputs In Chaos Experiments
 
 If your Terraform module exports some output variables you can use them in the Chaos Toolkit experiments
 as regular experiment parameters. Such variables are added to the configuration context with the `tf_out__` prefix.
 
 For example, this Terraform module exports a load balancer DNS name:
```

### Comparing `chaostoolkit-terraform-0.0.7/README.md` & `chaostoolkit-terraform-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# chaostoolkit-terraform
+# ChaosToolkit Terraform
 
 A [Chaos Toolkit](https://chaostoolkit.org/) driver to extend chaos experiments with [Terraform](https://www.terraform.io/)
 
 ## Package Installation
 
 ### From Python package index
 
@@ -62,15 +62,15 @@
       type: python
       module: chaosterraform.control
       arguments:
         silent: false
         retain: true
 ```
 
-**Configuration using Ctk parameters**
+**Configuration using Chaos Toolkit parameters**
 ```yaml
 configuration:
 # parameters prefixed with `tf_conf__` will configure chaosterraform driver
   tf_conf__silent: false
   tf_conf__retain: true
 
 controls:
@@ -86,34 +86,50 @@
 
 | Parameter Name        | Usage |
 | --------------------- | ------- |
 | **silent** | Suppress Terraform console output to avoid verbose experiment logs, defaults to `true`|
 | **retain** | Do not run `terraform destroy` at the end of the experiment to retain resources, defaults to `false` |
 | **chdir** | Instruct Terraform to change its working directory before running subcommands |
 
-## Set Terraform Input Variables
+## Provide Input Variables for Terraform
 
-You can override input variables defined in the Terraform module from within the experiment using
-Chaos Toolkit configuration parameters prefixed by `tf__`:
+You can override input variables defined in the Terraform module from within the experiment using the `variables`
+argument for the control:
+
+```yaml
+controls:
+  - name: "Deploy Terraform module"
+    provider:
+      type: python
+      module: chaosterraform.control
+      arguments:
+        variables:
+          vpc_id: "vpc-0000000000"
+          number_of_azs: 2
+```
+
+Alternatively, you can supply input variables from Chaos Toolkit configuration by referencing a parameter name
+already defined in Chaos Toolkit configuration:
 
 ```yaml
 configuration:
-# parameters prefixed with `tf__` will set terraform input variables for the module
-  tf__vpc_id: "vpc-0000000000"
-  tf__number_of_azs: 2
+  env_name: "live"
   ...
 
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
       module: chaosterraform.control
+      arguments:
+        variables:
+          environment:
+            name: "env_name"
 ```
 
-
 ## Use Terraform Outputs In Chaos Experiments
 
 If your Terraform module exports some output variables you can use them in the Chaos Toolkit experiments
 as regular experiment parameters. Such variables are added to the configuration context with the `tf_out__` prefix.
 
 For example, this Terraform module exports a load balancer DNS name:
```

### Comparing `chaostoolkit-terraform-0.0.7/chaosterraform/__init__.py` & `chaostoolkit-terraform-0.0.8/chaosterraform/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from chaoslib.discovery.discover import discover_actions, discover_activities, initialize_discovery_result
 from chaoslib.types import DiscoveredActivities, Discovery
 
 name = "chaosterraform"
 __author__ = """Manuel Castellin"""
 __email__ = "manuel@castellinconsulting.com"
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 __all__ = [
     "discover",
     "__version__",
 ]
 
 
 def discover(discover_system: bool = True) -> Discovery:
```

### Comparing `chaostoolkit-terraform-0.0.7/chaosterraform/control.py` & `chaostoolkit-terraform-0.0.8/chaosterraform/control.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """
 Terraform control module
 
 This module allows Chaos Toolkit users to create infrastructure resources using Terraform scripts
 for the experiment execution.
 """
+from typing import Any, Dict, List
+
+from chaoslib.exceptions import InterruptExecution
 from chaoslib.types import Configuration, Experiment, Journal, Secrets, Settings
 from logzero import logger
 
 from .driver import Terraform
 
-VAR_NAME_PREFIX = "tf__"
 CONFIG_PREFIX = "tf_conf__"
 EXPORT_VAR_PREFIX = "tf_out__"
 
 
 def configure_control(
     silent: bool = True,
     retain: bool = False,
     chdir: str = None,
+    variables: List = None,
+    outputs: Dict = None,
     configuration: Configuration = None,
     secrets: Secrets = None,
     settings: Settings = None,
     experiment: Experiment = None,
 ):
     """
     Configure terraform control for the experiment execution
@@ -30,42 +34,41 @@
     ----------
     silent: bool
         suppress Terraform logs in ChaosToolkit experiment logs
     retain: bool
         retain created resources at the end of the experiment
     chdir: str
         change the Terraform working directory
+    variables: List
+        input variables configuration for Terraform
+    outputs: Dict
+       configuration to map Terraform outputs to ChaosToolkit variables
 
     Raises
     ------
     InterruptExecution
         If terraform init fails we interrupt the experiment execution immediately
     """
     # pylint: disable=unused-argument
     tf_vars = {}
-    if configuration:
-        for key, value in configuration.items():
-            if key.startswith(VAR_NAME_PREFIX):
-                tf_key = key.replace(VAR_NAME_PREFIX, "")
-                tf_vars[tf_key] = value
-
-    for key, _ in tf_vars.items():
-        configuration.pop(f"{VAR_NAME_PREFIX}{key}")
+    if variables:
+        for key, value in variables.items():
+            tf_vars[key] = _resolve_variable(configuration, key, value)
 
     params = {
         "retain": bool(configuration.get(f"{CONFIG_PREFIX}retain", retain)),
         "silent": bool(configuration.get(f"{CONFIG_PREFIX}silent", silent)),
         "chdir": configuration.get(f"{CONFIG_PREFIX}chdir", chdir),
     }
     logger.info(
         "Terraform: retain stack after experiment completion: %s",
         str(params.get("retain")),
     )
 
-    driver = Terraform(**params, args=tf_vars)
+    driver = Terraform(**params, args=tf_vars, output_config=outputs)
     driver.terraform_init()
 
 
 def before_experiment_control(
     context: Experiment,
     configuration: Configuration = None,
     secrets: Secrets = None,
@@ -85,14 +88,17 @@
     # pylint: disable=unused-argument
     driver = Terraform()
     logger.info("Terraform: creating required resources for experiment")
     driver.apply()
     for key, value in driver.output().items():
         logger.info("Terraform: reading configuration value for [%s]", key)
         configuration[f"{EXPORT_VAR_PREFIX}{key}"] = value.get("value")
+        if key in driver.output_config:
+            export_name = driver.output_config[key]
+            configuration[export_name] = value.get("value")
 
 
 def after_experiment_control(
     context: Experiment,
     state: Journal,
     configuration: Configuration = None,
     secrets: Secrets = None,
@@ -107,7 +113,21 @@
     # pylint: disable=unused-argument
     driver = Terraform()
     if not driver.retain:
         logger.info("Terraform: removing experiment resources")
         driver.destroy()
     else:
         logger.info("Terraform: stack resources will be retained after experiment completion.")
+
+
+def _resolve_variable(configuration, key, value) -> Any:
+    if isinstance(value, dict):
+        if "name" not in value:
+            raise InterruptExecution(f"Terraform: parameter {key} should specify either a value or a 'name' key.")
+
+        parameter_name = value["name"]
+        if parameter_name not in configuration:
+            raise InterruptExecution(f"Terraform: could not resolve value for variable {key} in configuration")
+
+        return configuration[parameter_name]
+
+    return value
```

### Comparing `chaostoolkit-terraform-0.0.7/chaosterraform/driver.py` & `chaostoolkit-terraform-0.0.8/chaosterraform/driver.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,33 +42,37 @@
     silent: bool
         Suppress Terraform output in ChaosToolkit logs
     chdir: str
         A path to the terraform working directory. If the directory does not exists the experiment
         is interrupted with an InterruptExecution exception
     args: Dict
         Terraform variables overrides
+    output_config: Dict
+        Configuration to map Terraform output to configuration variables
 
     Raises
     ------
     InterruptExecution
         If the chdir path does not exists we interrupt the experiment execution immediately
     """
 
     def __init__(
         self,
         retain: bool = False,
         silent: bool = False,
         chdir: str = None,
         args: Dict = None,
+        output_config: Dict = None,
     ):
         super().__init__()
         self.retain = retain
         self.silent = silent
         self.chdir = chdir
         self.args = args or {}
+        self.output_config = output_config or {}
 
     @property
     def _terraform(self):
         if self.chdir:
             if not os.path.exists(self.chdir):
                 raise InterruptExecution(f"Terraform: chdir [{self.chdir}] does not exists")
             if not os.path.isdir(self.chdir):
```

### Comparing `chaostoolkit-terraform-0.0.7/chaostoolkit_terraform.egg-info/PKG-INFO` & `chaostoolkit-terraform-0.0.8/chaostoolkit_terraform.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-terraform
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Chaos Toolkit module to deploy terraform stacks
 Author: Manuel Castellin
 Project-URL: homepage, https://github.com/mcastellin/chaostoolkit-terraform
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# chaostoolkit-terraform
+# ChaosToolkit Terraform
 
 A [Chaos Toolkit](https://chaostoolkit.org/) driver to extend chaos experiments with [Terraform](https://www.terraform.io/)
 
 ## Package Installation
 
 ### From Python package index
 
@@ -71,15 +71,15 @@
       type: python
       module: chaosterraform.control
       arguments:
         silent: false
         retain: true
 ```
 
-**Configuration using Ctk parameters**
+**Configuration using Chaos Toolkit parameters**
 ```yaml
 configuration:
 # parameters prefixed with `tf_conf__` will configure chaosterraform driver
   tf_conf__silent: false
   tf_conf__retain: true
 
 controls:
@@ -95,34 +95,50 @@
 
 | Parameter Name        | Usage |
 | --------------------- | ------- |
 | **silent** | Suppress Terraform console output to avoid verbose experiment logs, defaults to `true`|
 | **retain** | Do not run `terraform destroy` at the end of the experiment to retain resources, defaults to `false` |
 | **chdir** | Instruct Terraform to change its working directory before running subcommands |
 
-## Set Terraform Input Variables
+## Provide Input Variables for Terraform
 
-You can override input variables defined in the Terraform module from within the experiment using
-Chaos Toolkit configuration parameters prefixed by `tf__`:
+You can override input variables defined in the Terraform module from within the experiment using the `variables`
+argument for the control:
+
+```yaml
+controls:
+  - name: "Deploy Terraform module"
+    provider:
+      type: python
+      module: chaosterraform.control
+      arguments:
+        variables:
+          vpc_id: "vpc-0000000000"
+          number_of_azs: 2
+```
+
+Alternatively, you can supply input variables from Chaos Toolkit configuration by referencing a parameter name
+already defined in Chaos Toolkit configuration:
 
 ```yaml
 configuration:
-# parameters prefixed with `tf__` will set terraform input variables for the module
-  tf__vpc_id: "vpc-0000000000"
-  tf__number_of_azs: 2
+  env_name: "live"
   ...
 
 controls:
   - name: "Deploy Terraform module"
     provider:
       type: python
       module: chaosterraform.control
+      arguments:
+        variables:
+          environment:
+            name: "env_name"
 ```
 
-
 ## Use Terraform Outputs In Chaos Experiments
 
 If your Terraform module exports some output variables you can use them in the Chaos Toolkit experiments
 as regular experiment parameters. Such variables are added to the configuration context with the `tf_out__` prefix.
 
 For example, this Terraform module exports a load balancer DNS name:
```

### Comparing `chaostoolkit-terraform-0.0.7/pyproject.toml` & `chaostoolkit-terraform-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "chaostoolkit-terraform"
 description = "A Chaos Toolkit module to deploy terraform stacks"
 readme = "README.md"
-version = "0.0.7"
+version = "0.0.8"
 authors = [ { name = "Manuel Castellin" } ]
 dependencies = [
     'chaostoolkit',
     'chaostoolkit-lib',
 ]
 
 [project.urls]
```

### Comparing `chaostoolkit-terraform-0.0.7/tests/test_control.py` & `chaostoolkit-terraform-0.0.8/tests/test_control.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,97 @@
+import pytest
 from unittest.mock import patch
+from chaoslib.exceptions import InterruptExecution
 from chaosterraform import control
 
 
 @patch("chaosterraform.control.Terraform", autospec=True)
 def test_configure_control_with_parameters(mocked_driver):
     control.configure_control(silent=False, retain=True, chdir="../testfolder/one", configuration={})
 
-    mocked_driver.assert_called_once_with(silent=False, retain=True, chdir="../testfolder/one", args={})
+    mocked_driver.assert_called_once_with(
+        silent=False, retain=True, chdir="../testfolder/one", args={}, output_config=None
+    )
     mock_instance = mocked_driver.return_value
     mock_instance.terraform_init.assert_called()
 
 
 @patch("chaosterraform.control.Terraform", autospec=True)
 def test_configure_control_with_terraform_variables(mocked_driver):
     configuration = {
-        "tf__variable_str": "sg-00001111",
-        "tf__one_more_bool_var": True,
-        "tf__numeric": 1.2,
+        "variable_str": "sg-00001111",
+        "one_more_bool_var": True,
+        "numeric": 1.2,
     }
 
-    control.configure_control(configuration=configuration)
+    variables = {
+        "one": {"name": "variable_str"},
+        "two": {"name": "one_more_bool_var"},
+        "three": {"name": "numeric"},
+        "four": "direct-value-assignment",
+    }
+
+    control.configure_control(variables=variables, configuration=configuration)
 
     expected_variables = {
-        "variable_str": "sg-00001111",
-        "one_more_bool_var": True,
+        "one": "sg-00001111",
+        "two": True,
+        "three": 1.2,
+        "four": "direct-value-assignment",
+    }
+
+    mocked_driver.assert_called_once_with(
+        silent=True, retain=False, chdir=None, args=expected_variables, output_config=None
+    )
+
+
+@patch("chaosterraform.control.Terraform", autospec=True)
+def test_configure_control_with_wrong_configuration(mocked_driver):
+    configuration = {
+        "numeric": 1.2,
+    }
+
+    variables = {
+        "three": {"__name": "numeric"},
+        "four": "direct-value-assignment",
+    }
+
+    with pytest.raises(InterruptExecution):
+        control.configure_control(variables=variables, configuration=configuration)
+
+
+@patch("chaosterraform.control.Terraform", autospec=True)
+def test_configure_control_with_missing_configuration(mocked_driver):
+    configuration = {
         "numeric": 1.2,
     }
 
-    mocked_driver.assert_called_once_with(silent=True, retain=False, chdir=None, args=expected_variables)
+    variables = {
+        "one": {"name": "missing"},
+        "three": {"name": "numeric"},
+        "four": "direct-value-assignment",
+    }
+
+    with pytest.raises(InterruptExecution):
+        control.configure_control(variables=variables, configuration=configuration)
 
 
 @patch("chaosterraform.control.Terraform", autospec=True)
 def test_configure_control_configuration_override(mocked_driver):
     configuration = {
         "tf_conf__silent": False,
         "tf_conf__retain": True,
         "tf_conf__chdir": "my/other/folder/path",
     }
 
     control.configure_control(silent=True, retain=False, chdir="some/folder", configuration=configuration)
 
-    mocked_driver.assert_called_once_with(silent=False, retain=True, chdir="my/other/folder/path", args={})
+    mocked_driver.assert_called_once_with(
+        silent=False, retain=True, chdir="my/other/folder/path", args={}, output_config=None
+    )
 
 
 @patch("chaosterraform.control.Terraform", autospec=True)
 def test_before_experiment_control_with_outputs(mocked_driver):
     outputs = {
         "dns_name": {"value": "example.com"},
         "desired_count": {"value": 1},
```

### Comparing `chaostoolkit-terraform-0.0.7/tests/test_driver.py` & `chaostoolkit-terraform-0.0.8/tests/test_driver.py`

 * *Files identical despite different names*

