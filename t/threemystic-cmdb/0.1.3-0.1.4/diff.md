# Comparing `tmp/threemystic_cmdb-0.1.3.tar.gz` & `tmp/threemystic_cmdb-0.1.4.tar.gz`

## Comparing `threemystic_cmdb-0.1.3.tar` & `threemystic_cmdb-0.1.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/__version__.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_cmdb_client.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cli/__init__.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    21346 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    20199 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py
--rw-r--r--   0        0        0    30767 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py
--rw-r--r--   0        0        0    13381 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0    18353 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/LICENSE
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/README.md
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/__version__.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_cmdb_client.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    21346 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    20694 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py
+-rw-r--r--   0        0        0    31108 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py
+-rw-r--r--   0        0        0    13381 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0    18353 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/README.md
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.4/PKG-INFO
```

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_cmdb_client.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_cmdb_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cli/__init__.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cli/actions/base_class/base.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cli/actions/config/__init__.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/base_class/base.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from threemystic_common.base_class.base_provider import base
 import asyncio, concurrent.futures
 from abc import abstractmethod
 from openpyxl import Workbook,worksheet
+from polling2 import TimeoutException, poll as poll2
 
 class cloud_cmdb_provider_base_cmdb(base):
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
     
     self._set_max_process_pool(*args, **kwargs)
     self._set_max_thread_pool(*args, **kwargs)
@@ -81,16 +82,32 @@
     self._excel_report_path_save = self.get_cloud_cmdb().get_cmdb_report_path().joinpath(f'{self._get_cloud_cmdb_raw().get_provider()}/{report_name}')
     if not self._excel_report_path_save.parent.exists():
       self._excel_report_path_save.parent.mkdir(parents= True)
     
     return self.save_excel_report_path()
   
   async def save_excel_report_only(self, close_connection = False, *args, **kwargs):
-    self._get_excel().save(self._excel_report_path_save)
+    if hasattr(self, "_saving_excel_report_data"):
+      if self._saving_excel_report_data is True and not close_connection:
+        return
+      
+      if self._saving_excel_report_data is True and not close_connection:
+        poll2(
+          lambda: self._saving_excel_report_data,
+          ignore_exceptions=(Exception,),
+          timeout= 240,
+          step=0.1
+        )
     
+    self._saving_excel_report_data = True
+
+    # When in write mode you can only save onces
+    self._get_excel().save(self.save_excel_report_path())
+    self._saving_excel_report_data = False
+
     if close_connection is True:
       self._excel_close()
 
   async def save_report(self, *args, **kwargs):
     
     
     if len(self._get_excel().sheetnames) < 1:
@@ -165,23 +182,33 @@
   
   def _get_data_action_by_key(self, *args, **kwargs):
     return {
       action: self._get_cloud_cmdb_raw().get_cloud_data_client().get_data_action(action= action) for action in list(self.get_workbook_general_data().keys())
     }
   
   async def _generate_report_data(self, pool, loop= None, *args, **kwargs):  
-    await self._process_report_data(
-      data= {
-        sheet_key: await data.main(pool= pool, loop= loop) for sheet_key, data in self._get_data_action_by_key().items()
-      }
-    )
+    
+    # await self._process_report_data(
+    #   data= {
+    #     sheet_key: await data.main(pool= pool, loop= loop,) for sheet_key, data in self._get_data_action_by_key().items()
+    #   }
+    # )
+    for sheet_key, data in self._get_data_action_by_key().items():
+      await data.main(
+          run_params = {
+            "send_account_data_lambda": {
+              "handler": self._process_report_data,
+              "sheet_key": sheet_key
+            },
+          },
+          pool= pool,
+          loop= loop)
 
   async def _process_report_data(self, data, *args, **kwargs):
     
-    save_task = None
     for sheet_key, main_report_data in data.items():
       for _, report_data in main_report_data.items():
         if report_data is None:
           continue
         
         while len(report_data) > 0:
           report_data_item=report_data.pop(0)
@@ -197,24 +224,17 @@
             [self.get_handler_column_data(column_data= column_data, is_cmdb= False)(report_data_item) for _, column_data in self.get_workbook_columns()[sheet_key].items()] +
             self.generate_tag_columns(
               account=report_data_item.get("extra_account"),
               resource= report_data_item,
               is_cmdb= False)
           )
           self.save_cmdb_workbook_item(sheet_key= sheet_key, account= report_data_item.get("extra_account"), report_data_item= report_data_item)
-          
-          report_data_len = len(report_data)
-          if ( report_data_len % 1000) == 0 and report_data_len > 0:
-            if save_task is not None:
-              await asyncio.wait([save_task])
 
-            save_task = asyncio.get_event_loop().create_task(self.save_excel_report_only(close_connection= False))
-    
-    if save_task is not None:
-      await asyncio.wait([save_task])
+
+      
 
   def _excel_close(self, *args, **kwargs):    
     self._get_excel().close()
     self.get_excel_workbook(unset= True)
     self._get_excel(unset= True)
 
   def _get_excel(self, unset = False, *args, **kwargs):
```

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/__init__.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,14 +518,18 @@
     for sheet_key, processed_data in self._processed_report_data.items():
       existing_data = self.__sync_data_get_existing(sheet_key= sheet_key)
       if len(existing_data) < 1:
         self.__sync_data_add_data(sheet_key= sheet_key, insert_data= processed_data)
         continue
       
       cmdb_id_index = self.get_existing_columns_sorted_by_index()[sheet_key].index(self.get_cmdb_data_containers_columns_raw_byid_display()[sheet_key]["cmdb_id"])
+      delete_index= -1
+      if self.get_cmdb_data_containers_columns_raw_byid_display()[sheet_key].get("deleted") is not None:
+        delete_index = self.get_existing_columns_sorted_by_index()[sheet_key].index(self.get_cmdb_data_containers_columns_raw_byid_display()[sheet_key]["deleted"])
+
       insert_data = []
       update_data = []
 
       while len(processed_data) > 0:
         row_cmdb_id = self.get_common().helper_type().string().set_case(
           string_value= processed_data[-1][cmdb_id_index],
           case= "lower"
@@ -551,20 +555,24 @@
             
             if(self.get_common().helper_type().string().is_null_or_whitespace(string_value= existing_row.get("values")[0][col_index]) and 
               self.get_common().helper_type().string().is_null_or_whitespace(string_value= check_row[col_index])):
               continue
 
             existing_row.get("values")[0][col_index] = check_row[col_index]
             has_update_data = True
-
+        
+        if delete_index > -1:
+          if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= existing_row.get("values")[0][delete_index]):
+            existing_row.get("values")[0][delete_index] = None
+            has_update_data = True
+            
         if has_update_data:
           update_data.append(existing_row)
       
-      if self.get_cmdb_data_containers_columns_raw_byid_display()[sheet_key].get("deleted") is not None:
-        delete_index = self.get_existing_columns_sorted_by_index()[sheet_key].index(self.get_cmdb_data_containers_columns_raw_byid_display()[sheet_key]["deleted"])
+      if delete_index > -1:
         while len(existing_data) > 0:
           _, deleted_data = existing_data.popitem()
           
           if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= deleted_data.get("values")[0][delete_index]):
             continue
 
           deleted_data.get("values")[0][delete_index] = self._get_delete_time()
```

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py` & `threemystic_cmdb-0.1.4/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/.gitignore` & `threemystic_cmdb-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/LICENSE` & `threemystic_cmdb-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/README.md` & `threemystic_cmdb-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.3/pyproject.toml` & `threemystic_cmdb-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,21 +24,22 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
   "threemystic-common >= 0.1.2",
-  "threemystic-cloud-data-client >= 0.1.3",
+  "threemystic-cloud-data-client >= 0.1.4",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
   "openpyxl >= 3.1.2",
-  "msgraph-sdk >= 1.0.0a12",
-  "lxml >= 4.9.2"
+  "lxml >= 4.9.2",
+  "msgraph-sdk >= 1.0.0a12",  
+  "polling2 >= 0.5.0",
 
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/3MysticApes/3mystic_cloud_cmdb"
 "Bug Tracker" = "https://github.com/3MysticApes/3mystic_cloud_cmdb/issues"
```

### Comparing `threemystic_cmdb-0.1.3/PKG-INFO` & `threemystic_cmdb-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cmdb
-Version: 0.1.3
+Version: 0.1.4
 Summary: A lightweight CMDB to help you track your cloud resources from various providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_cmdb
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_cmdb/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,16 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: asyncio>=3.4.3
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: msgraph-sdk>=1.0.0a12
 Requires-Dist: openpyxl>=3.1.2
-Requires-Dist: threemystic-cloud-data-client>=0.1.3
+Requires-Dist: polling2>=0.5.0
+Requires-Dist: threemystic-cloud-data-client>=0.1.4
 Requires-Dist: threemystic-common>=0.1.2
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cmdb
 A Lightweight Multi Cloud CMDB (Configuration management database)
```

