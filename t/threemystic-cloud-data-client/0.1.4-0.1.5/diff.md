# Comparing `tmp/threemystic_cloud_data_client-0.1.4.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.5.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.4.tar` & `threemystic_cloud_data_client-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/LICENSE
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/hatch.toml
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
+-rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/hatch.toml
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.5/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,56 @@
 from threemystic_cloud_data_client.cloud_providers.azure.client.actions.base_class.base import cloud_data_client_azure_client_action_base as base
 import asyncio
-from azure.mgmt.storage import StorageManagementClient
+from azure.mgmt.compute import ComputeManagementClient
+from azure.mgmt.resource import ResourceManagementClient
+
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
-      data_action="cloudstorage", 
-      logger_name= "cloud_data_client_azure_client_action_cloudstorage", 
-      uniqueid_lambda = lambda: True,
+      data_action="vmss", 
+      logger_name= "cloud_data_client_azure_client_action_vmss", 
+      uniqueid_lambda = lambda: True, 
       *args, **kwargs)
   
   
     
-  async def _process_account_data_blob_containers(self, client:StorageManagementClient, account, storage_account, **kwargs):
-      try:
-        resource_group= self.get_cloud_client().get_resource_group_from_resource(resource= storage_account)
-        storage_account_name= self.get_cloud_client().get_resource_name_from_resource(resource= storage_account)
-        return [self.get_cloud_client().serialize_azresource(resource= item) for item in self.get_cloud_client().sdk_request(
-          tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
-          lambda_sdk_command=lambda: client.blob_containers.list(resource_group_name= resource_group, account_name= storage_account_name)
-        )]
-      except:
-        return []
-      
-  async def _process_storage_account_by_page(self, client:StorageManagementClient, account, **kwargs):
-      
-      process_object = []
-      for _, page in self.get_cloud_client().sdk_request(
+  async def __process_get_resources_vmss(self, account, *args, **kwargs):
+    resource_client = ResourceManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
+    try:
+      return { self.get_cloud_client().get_resource_id_from_resource(resource= resource): resource for resource in self.get_cloud_client().sdk_request(
           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
-          lambda_sdk_command=lambda: enumerate(client.storage_accounts.list().by_page())
-        ):
-        for storage_account in page:
-          for blob_container in await self._process_account_data_blob_containers(client= client, account= account, storage_account= storage_account):
-            process_object.append({
-              "container": blob_container,
-              "storage_account": storage_account
-            })
-          process_object.append({
-            "container": None,
-            "storage_account": storage_account
-          })
-      
-      return process_object
+          lambda_sdk_command=lambda: resource_client.resources.list(filter="resourceType eq 'Microsoft.Compute/virtualMachineScaleSets'", expand="createdTime,changedTime,provisioningState")
+        )
+      }
+    except:
+      return []
+        
+  async def _process_account_data(self, account, loop, *args, **kwargs):
+    client = ComputeManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
+    tasks = {
+      "resource": loop.create_task(self.__process_get_resources_vmss(account= account))
+    }
 
-  async def _process_account_data(self, account, loop, **kwargs):
+    await asyncio.wait(tasks.values())
 
-    client = StorageManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
-    process_object = await self._process_storage_account_by_page(client= client, account= account)
-      
     return {
-        "account": account,
-        "data": [ self.get_common().helper_type().dictionary().merge_dictionary([
+      "account": account,
+      "data": [ self.get_common().helper_type().dictionary().merge_dictionary([
           {},
           self.get_base_return_data(
             account= self.get_cloud_client().serialize_azresource(resource= account),
-            resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item.get("container") if item.get("container") is not None else item.get("storage_account")),
-            resource = item.get("container"),
-            region= self.get_cloud_client().get_azresource_location(resource= item.get("storage_account")),
-            resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item.get("storage_account"))],
+            resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
+            resource= item,
+            region= self.get_cloud_client().get_azresource_location(resource= item),
+            resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
           ),
           {
-            "extra_storage_account": item.get("storage_account")
-          }
-        ]) for item in process_object]
+            "extra_resource": self.get_cloud_client().serialize_azresource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item))),
+            "extra_vmss_vms": [ self.get_cloud_client().serialize_azresource(vm) for vm in client.virtual_machine_scale_set_vms.list(resource_group_name= self.get_cloud_client().get_resource_group_from_resource(item), virtual_machine_scale_set_name= item.name) ]
+          },
+          ]) for item in self.get_cloud_client().sdk_request(
+          tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
+          lambda_sdk_command=lambda: client.virtual_machine_scale_sets.list_all()
+        )
+      ]
     }
```

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,21 @@
       "--budget": {
         "default": None, 
         "const": "budget",
         "dest": "data_action",
         "help": "Data Action: This pulls a general budget to provide you insights in your accounts/subscriptions",
         "action": 'store_const'
       },
+      # "--secrets": {
+      #   "default": None, 
+      #   "const": "secrets",
+      #   "dest": "data_action",
+      #   "help": "Data Action: Pulls Key Vaults Secrets and Keys / Paramater Store",
+      #   "action": 'store_const'
+      # },
       "--storage": {
         "default": None, 
         "const": "storage",
         "dest": "data_action",
         "help": "Data Action: This pulls either VM Disks or EC2 Storage depending on the provider",
         "action": 'store_const'
       },
```

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.5/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/.gitignore` & `threemystic_cloud_data_client-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/LICENSE` & `threemystic_cloud_data_client-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/README.md` & `threemystic_cloud_data_client-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/hatch.toml` & `threemystic_cloud_data_client-0.1.5/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.4/pyproject.toml` & `threemystic_cloud_data_client-0.1.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -23,24 +23,30 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.2",
-  "threemystic-cloud-client >= 0.1.4",
+  "threemystic-common >= 0.1.3",
+  "threemystic-cloud-client >= 0.1.5",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
   "azure-mgmt-subscription >= 3.1.1",
   "azure-mgmt-managementgroups >= 1.0.0",
   "azure-mgmt-resourcegraph >= 8.0.0",
   "azure-mgmt-costmanagement >= 4.0.0",
-  "azure-mgmt-network >= 23.1.0"
+  "azure-mgmt-network >= 23.1.0",
+  "azure-mgmt-keyvault >= 10.2.2",
+  "azure-mgmt-monitor >= 6.0.1",
+  "azure-keyvault-administration >= 4.3.0",
+  "azure-keyvault-certificates >= 4.7.0",
+  "azure-keyvault-keys >= 4.8.0",
+  "azure-keyvault-secrets >= 4.7.0",
 
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/3MysticApes/3mystic_cloud_data_client"
 "Bug Tracker" = "https://github.com/3MysticApes/3mystic_cloud_data_client/issues"
```

### Comparing `threemystic_cloud_data_client-0.1.4/PKG-INFO` & `threemystic_cloud_data_client-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -14,22 +14,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: asyncio>=3.4.3
+Requires-Dist: azure-keyvault-administration>=4.3.0
+Requires-Dist: azure-keyvault-certificates>=4.7.0
+Requires-Dist: azure-keyvault-keys>=4.8.0
+Requires-Dist: azure-keyvault-secrets>=4.7.0
 Requires-Dist: azure-mgmt-costmanagement>=4.0.0
+Requires-Dist: azure-mgmt-keyvault>=10.2.2
 Requires-Dist: azure-mgmt-managementgroups>=1.0.0
+Requires-Dist: azure-mgmt-monitor>=6.0.1
 Requires-Dist: azure-mgmt-network>=23.1.0
 Requires-Dist: azure-mgmt-resourcegraph>=8.0.0
 Requires-Dist: azure-mgmt-subscription>=3.1.1
 Requires-Dist: colorama; platform_system == 'Windows'
-Requires-Dist: threemystic-cloud-client>=0.1.4
-Requires-Dist: threemystic-common>=0.1.2
+Requires-Dist: threemystic-cloud-client>=0.1.5
+Requires-Dist: threemystic-common>=0.1.3
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_data_client
 A set of scripts to help uniformly pull data from the cloud providers for various resources.
 Currently supports AWS/Azure
```

