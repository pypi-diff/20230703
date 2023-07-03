# Comparing `tmp/threemystic_cloud_client-0.1.3.tar.gz` & `tmp/threemystic_cloud_client-0.1.4.tar.gz`

## Comparing `threemystic_cloud_client-0.1.3.tar` & `threemystic_cloud_client-0.1.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/test/__init__.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/token/__init__.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0    21250 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/test/step_1.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0    13846 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/test/step_1.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/LICENSE
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/hatch.toml
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cli/actions/test/__init__.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cli/actions/token/__init__.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0    21260 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/test/step_1.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0    13856 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/test/step_1.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/hatch.toml
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.4/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/test/__init__.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cli/actions/test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/token/__init__.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cli/actions/token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from threemystic_cloud_client.cloud_providers.aws.client.base_class.base import cloud_client_aws_client_base as base
 import sys
 import os
 import boto3
-from polling2 import TimeoutException, poll
+from polling2 import TimeoutException, poll as poll2
     
 class cloud_client_aws_client_sso(base):
   def __init__(self, *args, **kwargs):
     super().__init__(logger_name= "cloud_client_aws_client_sso", *args, **kwargs)
 
     if(self.get_common().helper_type().string().set_case(string_value= self.get_profile()["profile_data"]["auth_method"], case= "lower") != "sso"):
       raise self.get_common().exception().exception(
@@ -150,15 +150,15 @@
       ).type_error(
         logger = self.get_common().get_logger(),
         name = f"NOT AUTHENTICATED",
         message = f"Cloud Client Profile could not authenticate SSO Profile"
       )
 
     try:
-      logged_in = poll(
+      logged_in = poll2(
         lambda: not self.session_expired(refresh = True),
         ignore_exceptions=(Exception,),
         timeout=self.get_aws_poll_login(),
         step=0.1
       )
       if logged_in is not None:      
         return logged_in
```

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from abc import abstractmethod
 from threemystic_cloud_client.cloud_providers.aws.base_class.base import cloud_client_provider_aws_base as base
 from botocore import session as botocore_session, credentials as botocore_credentials
 from botocore.config import Config as botocore_config_config
 from boto3 import Session as boto_session
 from botocore.exceptions import ClientError
-from polling2 import TimeoutException, poll
+from polling2 import TimeoutException, poll as poll2
 import time
 from random import randint
 
 class cloud_client_aws_client_base(base):
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
 
@@ -279,15 +279,15 @@
       ).type_error(
         logger = self.get_common().get_logger(),
         name = "NOT AUTHENTICATED",
         message = f"Error waiting for authentication"
       )
     
     if(self.is_authenticating_session()):
-      poll(
+      poll2(
         lambda: self.is_authenticating_session(),
         ignore_exceptions=(Exception,),
         timeout=self.get_aws_poll_authenticate(),
         step=0.1
       )
       return self.ensure_session(count= count+1)
```

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/test/step_1.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/test/step_2.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from threemystic_cloud_client.cloud_providers.base_class.base import cloud_client_provider_base as base
 from azure.mgmt.costmanagement.models import TimeframeType, OperatorType, QueryColumnType, QueryDefinition, QueryTimePeriod, QueryDataset, QueryAggregation, QueryGrouping, QueryFilter, QueryComparisonExpression
 from azure.core.exceptions import HttpResponseError, ClientAuthenticationError
 import time
 import math
 from abc import abstractmethod
-from polling2 import TimeoutException, poll
+from polling2 import TimeoutException, poll as poll2
 
 
 class cloud_client_provider_azure_base(base):
   def __init__(self, *args, **kwargs):
     self._stop_process_login()
     super().__init__(provider= "azure", *args, **kwargs)
     
@@ -31,15 +31,15 @@
     self.__is_processing_login = False
 
   def _start_process_login(self, *args, **kwargs):
     self.__is_processing_login = True
      
   def login(self, *args, **kwargs):
     if self.is_login_processing():
-      poll(
+      poll2(
         lambda: self.is_login_processing(),
         ignore_exceptions=(Exception,),
         timeout=240,
         step=0.1
       )
 
     self._start_process_login()
```

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/test/step_1.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.4/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/.gitignore` & `threemystic_cloud_client-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/LICENSE` & `threemystic_cloud_client-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/README.md` & `threemystic_cloud_client-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/hatch.toml` & `threemystic_cloud_client-0.1.4/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/pyproject.toml` & `threemystic_cloud_client-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.3/PKG-INFO` & `threemystic_cloud_client-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

