# Comparing `tmp/threemystic_cloud_data_client-0.1.3.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.4.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.3.tar` & `threemystic_cloud_data_client-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    19682 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/LICENSE
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/hatch.toml
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/hatch.toml
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,16 +131,19 @@
           **kwargs
         )
   
   def get_runparam_key(self, data_key = None, default_value = {}, *args, **kwargs):
     if data_key is None:
       return self.__run_params
     
+    if data_key == "send_account_data_lambda":
+      return self.__run_params_send_account_data_lambda
+    
     if data_key is not None and data_key in self.__run_params:
-      if self.get_common().helper_type().general().is_type(obj= self.__run_params.get(data_key), type_check= type(default_value)):
+      if default_value is None or self.get_common().helper_type().general().is_type(obj= self.__run_params.get(data_key), type_check= type(default_value)):
         return self.__run_params.get(data_key)
     
     return default_value
   
   def _set_run_params(self, run_params = None, *args, **kwargs):
     if run_params is None:
       self.__run_params = {}
@@ -162,23 +165,28 @@
         run_params["data_accounts"] = self.get_common().helper_type().string().split(
           string_value= run_params["data_accounts"],
           separator= r"[,;\s]"
         )
       if not self.get_common().helper_type().general().is_type(obj= run_params.get("data_accounts"), type_check= list):
         run_params["data_accounts"] = []
     
+    self.__run_params_send_account_data_lambda = None
+    if "send_account_data_lambda" in run_params:
+      self.__run_params_send_account_data_lambda = run_params.pop("send_account_data_lambda")
+
     self.__run_params = self.get_common().helper_type().dictionary().merge_dictionary([
       {},
       {
         "data_filter": {},
         "data_hideempty": False,
-        "data_accounts": None
+        "data_accounts": None,
       },
       run_params
     ])
+    
   
   
   def _process_data_filter_condition_in(self, condition, condition_value, data_value, *args, **kwargs):
     condition_settings = self._process_data_filter_condition_settings("in", condition)
 
     if condition_settings.get("case_insensitive") is True:
       data_value = self.get_common().helper_type().string().set_case(string_value= data_value, case= "lower")
@@ -422,15 +430,27 @@
     return {
         "tasks": done_results["tasks"],
         "tasks_processed": done_results["done"],
         "done_count": done_count,
     }
   
   async def _process_account(self, *args, **kwargs):
-    return await self._process_account_data(*args, **kwargs)
+    return_data = await self._process_account_data(*args, **kwargs)
+    if self.get_runparam_key(data_key= "send_account_data_lambda", default_value= None) is None:
+      return return_data
+    
+    await self.get_runparam_key(data_key= "send_account_data_lambda", default_value= None)["handler"](data= {
+      (self.get_runparam_key(data_key= "send_account_data_lambda", default_value= None)["sheet_key"]): {
+        self.get_cloud_client().get_account_id(account= return_data["account"]): return_data.pop("data")
+      }
+    })
+    
+
+    return_data["data"] = []
+    return return_data
   
   async def process_account(self, *args, **kwargs):
     return await self._process_account(*args, **kwargs)
   
   def process_account_sync(self, *args, **kwargs):
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
```

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/.gitignore` & `threemystic_cloud_data_client-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/LICENSE` & `threemystic_cloud_data_client-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/README.md` & `threemystic_cloud_data_client-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/hatch.toml` & `threemystic_cloud_data_client-0.1.4/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.3/pyproject.toml` & `threemystic_cloud_data_client-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
   "threemystic-common >= 0.1.2",
-  "threemystic-cloud-client >= 0.1.3",
+  "threemystic-cloud-client >= 0.1.4",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
   "azure-mgmt-subscription >= 3.1.1",
   "azure-mgmt-managementgroups >= 1.0.0",
   "azure-mgmt-resourcegraph >= 8.0.0",
   "azure-mgmt-costmanagement >= 4.0.0",
```

### Comparing `threemystic_cloud_data_client-0.1.3/PKG-INFO` & `threemystic_cloud_data_client-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 Requires-Dist: asyncio>=3.4.3
 Requires-Dist: azure-mgmt-costmanagement>=4.0.0
 Requires-Dist: azure-mgmt-managementgroups>=1.0.0
 Requires-Dist: azure-mgmt-network>=23.1.0
 Requires-Dist: azure-mgmt-resourcegraph>=8.0.0
 Requires-Dist: azure-mgmt-subscription>=3.1.1
 Requires-Dist: colorama; platform_system == 'Windows'
-Requires-Dist: threemystic-cloud-client>=0.1.3
+Requires-Dist: threemystic-cloud-client>=0.1.4
 Requires-Dist: threemystic-common>=0.1.2
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_data_client
 A set of scripts to help uniformly pull data from the cloud providers for various resources.
```

