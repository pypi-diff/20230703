# Comparing `tmp/tencentcloud-sdk-python-billing-3.0.925.tar.gz` & `tmp/tencentcloud-sdk-python-billing-3.0.926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.925.tar", last modified: Fri Jun 30 02:00:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.926.tar", last modified: Mon Jul  3 00:19:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-billing-3.0.925.tar` & `tencentcloud-sdk-python-billing-3.0.926.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:00:34.000000 tencentcloud-sdk-python-billing-3.0.925/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:00:34.000000 tencentcloud-sdk-python-billing-3.0.925/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:00:34.000000 tencentcloud-sdk-python-billing-3.0.925/tencentcloud_sdk_python_billing.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:00:33.000000 tencentcloud-sdk-python-billing-3.0.925/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-30 02:00:33.000000 tencentcloud-sdk-python-billing-3.0.925/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-30 02:00:33.000000 tencentcloud-sdk-python-billing-3.0.925/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:00:33.000000 tencentcloud-sdk-python-billing-3.0.925/tencentcloud_sdk_python_billing.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:00:34.000000 tencentcloud-sdk-python-billing-3.0.925/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:00:33.000000 tencentcloud-sdk-python-billing-3.0.925/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:00:34.000000 tencentcloud-sdk-python-billing-3.0.925/tencentcloud/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:00:33.000000 tencentcloud-sdk-python-billing-3.0.925/tencentcloud/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:00:34.000000 tencentcloud-sdk-python-billing-3.0.925/tencentcloud/billing/v20180709/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:00:33.000000 tencentcloud-sdk-python-billing-3.0.925/tencentcloud/billing/v20180709/__init__.py
--rw-r--r--   0 root         (0) root         (0)   167865 2023-06-30 02:00:33.000000 tencentcloud-sdk-python-billing-3.0.925/tencentcloud/billing/v20180709/models.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-06-30 02:00:33.000000 tencentcloud-sdk-python-billing-3.0.925/tencentcloud/billing/v20180709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    21124 2023-06-30 02:00:33.000000 tencentcloud-sdk-python-billing-3.0.925/tencentcloud/billing/v20180709/billing_client.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-30 02:00:33.000000 tencentcloud-sdk-python-billing-3.0.925/README.rst
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-30 02:00:34.000000 tencentcloud-sdk-python-billing-3.0.925/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-30 02:00:33.000000 tencentcloud-sdk-python-billing-3.0.925/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/setup.py
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/tencentcloud_sdk_python_billing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/tencentcloud_sdk_python_billing.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/tencentcloud/billing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/tencentcloud/billing/v20180709/
+-rw-r--r--   0 root         (0) root         (0)   168483 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/tencentcloud/billing/v20180709/models.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/tencentcloud/billing/v20180709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/tencentcloud/billing/v20180709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21124 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/tencentcloud/billing/v20180709/billing_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/tencentcloud/billing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:19:23.000000 tencentcloud-sdk-python-billing-3.0.926/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-billing-3.0.925/tencentcloud_sdk_python_billing.egg-info/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.926/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.925/tencentcloud/__init__.py` & `tencentcloud-sdk-python-billing-3.0.926/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.925'
+__version__ = '3.0.926'
```

### Comparing `tencentcloud-sdk-python-billing-3.0.925/tencentcloud/billing/v20180709/models.py` & `tencentcloud-sdk-python-billing-3.0.926/tencentcloud/billing/v20180709/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,14 +260,20 @@
         :type SpecifiedPrice: str
         :param PriceUnit: 组件价格单位：组件价格的单位，单位构成：元/用量单位/时长单位
         :type PriceUnit: str
         :param UsedAmount: 组件用量：该组件实际结算用量，组件用量 = 组件原始用量 - 抵扣用量（含资源包
         :type UsedAmount: str
         :param UsedAmountUnit: 组件用量单位：组件用量对应的单位
         :type UsedAmountUnit: str
+        :param RealTotalMeasure: 原始用量/时长：组件被资源包抵扣前的原始用量/时长
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RealTotalMeasure: str
+        :param DeductedMeasure: 抵扣用量/时长（含资源包）：组件被资源包抵扣的用量/时长
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeductedMeasure: str
         :param TimeSpan: 使用时长：资源使用的时长
         :type TimeSpan: str
         :param TimeUnitName: 时长单位：资源使用时长的单位
         :type TimeUnitName: str
         :param Cost: 组件原价：原价 = 组件刊例价 * 组件用量 * 使用时长（如果客户享受一口价/合同价则默认不展示，退费类场景也默认不展示）
         :type Cost: str
         :param Discount: 折扣率：本资源享受的折扣率（如果客户享受一口价/合同价则默认不展示，退费场景也默认不展示）
@@ -319,14 +325,16 @@
         self.ComponentCodeName = None
         self.ItemCodeName = None
         self.SinglePrice = None
         self.SpecifiedPrice = None
         self.PriceUnit = None
         self.UsedAmount = None
         self.UsedAmountUnit = None
+        self.RealTotalMeasure = None
+        self.DeductedMeasure = None
         self.TimeSpan = None
         self.TimeUnitName = None
         self.Cost = None
         self.Discount = None
         self.ReduceType = None
         self.RealCost = None
         self.VoucherPayAmount = None
@@ -349,14 +357,16 @@
         self.ComponentCodeName = params.get("ComponentCodeName")
         self.ItemCodeName = params.get("ItemCodeName")
         self.SinglePrice = params.get("SinglePrice")
         self.SpecifiedPrice = params.get("SpecifiedPrice")
         self.PriceUnit = params.get("PriceUnit")
         self.UsedAmount = params.get("UsedAmount")
         self.UsedAmountUnit = params.get("UsedAmountUnit")
+        self.RealTotalMeasure = params.get("RealTotalMeasure")
+        self.DeductedMeasure = params.get("DeductedMeasure")
         self.TimeSpan = params.get("TimeSpan")
         self.TimeUnitName = params.get("TimeUnitName")
         self.Cost = params.get("Cost")
         self.Discount = params.get("Discount")
         self.ReduceType = params.get("ReduceType")
         self.RealCost = params.get("RealCost")
         self.VoucherPayAmount = params.get("VoucherPayAmount")
```

### Comparing `tencentcloud-sdk-python-billing-3.0.925/tencentcloud/billing/v20180709/errorcodes.py` & `tencentcloud-sdk-python-billing-3.0.926/tencentcloud/billing/v20180709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.925/tencentcloud/billing/v20180709/billing_client.py` & `tencentcloud-sdk-python-billing-3.0.926/tencentcloud/billing/v20180709/billing_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.925/README.rst` & `tencentcloud-sdk-python-billing-3.0.926/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.925/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.926/tencentcloud_sdk_python_billing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.925/setup.py` & `tencentcloud-sdk-python-billing-3.0.926/setup.py`

 * *Files identical despite different names*

