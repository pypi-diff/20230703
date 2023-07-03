# Comparing `tmp/threemystic_cmdb-0.1.4.tar.gz` & `tmp/threemystic_cmdb-0.1.5.tar.gz`

## Comparing `threemystic_cmdb-0.1.4.tar` & `threemystic_cmdb-0.1.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/__version__.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_cmdb_client.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cli/__init__.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    21346 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    20694 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py
--rw-r--r--   0        0        0    31108 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py
--rw-r--r--   0        0        0    13381 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0    18353 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/LICENSE
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/README.md
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/__version__.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_cmdb_client.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    21346 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    21382 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py
+-rw-r--r--   0        0        0    31108 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py
+-rw-r--r--   0        0        0    13381 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0    18353 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/README.md
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.5/PKG-INFO
```

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_cmdb_client.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_cmdb_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cli/__init__.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cli/actions/base_class/base.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cli/actions/config/__init__.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from threemystic_cloud_cmdb.cloud_providers.azure.client.actions.base_class.base import cloud_cmdb_azure_client_action_base as base
 import asyncio
 from azure.mgmt.storage import StorageManagementClient
+from decimal import Decimal, ROUND_HALF_UP
 
 class cloud_cmdb_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="cloudstorage", 
       logger_name= "cloud_cmdb_azure_client_action_cloudstorage", 
       uniqueid_lambda = lambda: True
@@ -37,15 +38,15 @@
         },
         "BucketName":{
           "display": "BucketName",
           "handler": lambda item: self.get_item_data_value(item_data= item, value_key=["name"])
         },
         "AvgSizeLast24HR_Bytes":{
           "display": "AvgSizeLast24HR_Bytes",
-          "handler": lambda item:  None
+          "handler": lambda item:  self.get_item_data_value(item_data= item, value_key=["extra_storageaccount_bytes_24hours"])
         },
         "SampleObjectClass":{
           "display": "SampleObjectClass",
           "handler": lambda item: None
         },
         "SampleObjectRetention":{
           "display": "SampleObjectRetention",
```

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/base_class/base.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from threemystic_common.base_class.base_provider import base
 import asyncio, concurrent.futures
 from abc import abstractmethod
 from openpyxl import Workbook,worksheet
 from polling2 import TimeoutException, poll as poll2
+from random import Random
 
 class cloud_cmdb_provider_base_cmdb(base):
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
     
     self._set_max_process_pool(*args, **kwargs)
     self._set_max_thread_pool(*args, **kwargs)
@@ -103,14 +104,25 @@
     # When in write mode you can only save onces
     self._get_excel().save(self.save_excel_report_path())
     self._saving_excel_report_data = False
 
     if close_connection is True:
       self._excel_close()
 
+  def _stop_is_processing_sheet_data_or_set_processing(self, sheet_key, *args, **kwargs):
+    setattr(self, f"_is_processing_sheet_data_{sheet_key}", False)
+
+  def _is_processing_sheet_data_or_set_processing(self, sheet_key, *args, **kwargs):
+    if getattr(self, f"_is_processing_sheet_data_{sheet_key}", False) is True:
+      return True
+        
+      
+    setattr(self, f"_is_processing_sheet_data_{sheet_key}", True)
+    return False
+
   async def save_report(self, *args, **kwargs):
     
     
     if len(self._get_excel().sheetnames) < 1:
       print(f'No Report Saved - No Data')
       return  
     print(f'Report saved at: {self.save_excel_report_path()}')
@@ -202,14 +214,16 @@
           },
           pool= pool,
           loop= loop)
 
   async def _process_report_data(self, data, *args, **kwargs):
     
     for sheet_key, main_report_data in data.items():
+      while self._is_processing_sheet_data_or_set_processing(sheet_key= sheet_key):
+        await asyncio.sleep(Random().random()*2)
       for _, report_data in main_report_data.items():
         if report_data is None:
           continue
         
         while len(report_data) > 0:
           report_data_item=report_data.pop(0)
           self.get_excel_workbook(sheet_key= sheet_key).append(
@@ -224,14 +238,16 @@
             [self.get_handler_column_data(column_data= column_data, is_cmdb= False)(report_data_item) for _, column_data in self.get_workbook_columns()[sheet_key].items()] +
             self.generate_tag_columns(
               account=report_data_item.get("extra_account"),
               resource= report_data_item,
               is_cmdb= False)
           )
           self.save_cmdb_workbook_item(sheet_key= sheet_key, account= report_data_item.get("extra_account"), report_data_item= report_data_item)
+      
+      self._stop_is_processing_sheet_data_or_set_processing(sheet_key= sheet_key)
 
 
       
 
   def _excel_close(self, *args, **kwargs):    
     self._get_excel().close()
     self.get_excel_workbook(unset= True)
```

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/__init__.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py` & `threemystic_cmdb-0.1.5/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/.gitignore` & `threemystic_cmdb-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/LICENSE` & `threemystic_cmdb-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/README.md` & `threemystic_cmdb-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.4/pyproject.toml` & `threemystic_cmdb-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.2",
-  "threemystic-cloud-data-client >= 0.1.4",
+  "threemystic-common >= 0.1.3",
+  "threemystic-cloud-data-client >= 0.1.5",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
   "openpyxl >= 3.1.2",
   "lxml >= 4.9.2",
   "msgraph-sdk >= 1.0.0a12",  
   "polling2 >= 0.5.0",
```

### Comparing `threemystic_cmdb-0.1.4/PKG-INFO` & `threemystic_cmdb-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cmdb
-Version: 0.1.4
+Version: 0.1.5
 Summary: A lightweight CMDB to help you track your cloud resources from various providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_cmdb
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_cmdb/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -19,16 +19,16 @@
 Requires-Python: >=3.8
 Requires-Dist: asyncio>=3.4.3
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: msgraph-sdk>=1.0.0a12
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: polling2>=0.5.0
-Requires-Dist: threemystic-cloud-data-client>=0.1.4
-Requires-Dist: threemystic-common>=0.1.2
+Requires-Dist: threemystic-cloud-data-client>=0.1.5
+Requires-Dist: threemystic-common>=0.1.3
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cmdb
 A Lightweight Multi Cloud CMDB (Configuration management database)
 Currently supports AWS/Azure
```

