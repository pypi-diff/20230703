# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.925.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.925.tar", last modified: Fri Jun 30 02:03:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.926.tar", last modified: Mon Jul  3 00:22:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.925.tar` & `tencentcloud-sdk-python-ckafka-3.0.926.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)   486893 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)    71620 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/README.rst
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-30 02:03:31.000000 tencentcloud-sdk-python-ckafka-3.0.925/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud/ckafka/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud/ckafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)   487706 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)    71620 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:22:22.000000 tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud/ckafka/v20190819/__init__.py
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2300,25 +2300,25 @@
         :type InstanceName: str
         :param BandWidth: 实例内网峰值带宽。单位 MB/s。标准版需传入当前实例规格所对应的峰值带宽。注意如果创建的实例为专业版实例，峰值带宽，分区数等参数配置需要满足专业版的计费规格。
         :type BandWidth: int
         :param VpcId: 创建的实例默认接入点所在的 vpc 对应 vpcId。目前不支持创建基础网络实例，因此该参数必填
         :type VpcId: str
         :param SubnetId: 子网id。创建实例默认接入点所在的子网对应的子网 id
         :type SubnetId: str
-        :param InstanceType: 实例规格。当创建标准版实例时必填，创建专业版实例时不需要填写。1：入门型；2：标准型；3：进阶型；4：容量型；5：高阶型1；6：高阶性2；7：高阶型3；8：高阶型4；9 ：独占型
+        :param InstanceType: 国际站标准版实例规格。目前只有国际站标准版使用当前字段区分规格，国内站标准版使用峰值带宽区分规格。除了国际站标准版外的所有实例填写 1 即可。国际站标准版实例：入门型(general)]填写1；[标准型(standard)]填写2；[进阶型(advanced)]填写3；[容量型(capacity)]填写4；[高阶型1(specialized-1)]填写5；[高阶型2(specialized-2)]填写6；[高阶型3(specialized-3)]填写7；[高阶型4(specialized-4)]填写8。
         :type InstanceType: int
         :param MsgRetentionTime: 实例日志的默认最长保留时间，单位分钟。不传入该参数时默认为 1440 分钟（1天），最大30天。当 topic 显式设置消息保留时间时，以 topic 保留时间为准
         :type MsgRetentionTime: int
         :param ClusterId: 创建实例时可以选择集群Id, 该入参表示集群Id。不指定实例所在集群则不传入该参数
         :type ClusterId: int
         :param KafkaVersion: 实例版本。目前支持 "0.10.2","1.1.1","2.4.1","2.4.2","2.8.1"。"2.4.1" 与 "2.4.2" 属于同一个版本，传任意一个均可。
         :type KafkaVersion: str
         :param SpecificationsType: 实例类型。"standard"：标准版，"profession"：专业版
         :type SpecificationsType: str
-        :param DiskType: 实例硬盘类型，"CLOUD_BASIC"：云硬盘，"CLOUD_SSD"：高速云硬盘。不传默认为 "CLOUD_BASIC"
+        :param DiskType: 专业版实例磁盘类型，标准版实例不需要填写。"CLOUD_SSD"：SSD云硬盘；"CLOUD_BASIC"：高性能云硬盘。不传默认值为 "CLOUD_BASIC"
         :type DiskType: str
         :param DiskSize: 实例硬盘大小，需要满足当前实例的计费规格
         :type DiskSize: int
         :param Partition: 实例最大分区数量，需要满足当前实例的计费规格
         :type Partition: int
         :param TopicNum: 实例最大 topic 数量，需要满足当前实例的计费规格
         :type TopicNum: int
@@ -2489,46 +2489,45 @@
 
     """
 
     def __init__(self):
         r"""
         :param InstanceName: 实例名称，是一个不超过 64 个字符的字符串，必须以字母为首字符，剩余部分可以包含字母、数字和横划线(-)
         :type InstanceName: str
-        :param ZoneId: 可用区，购买多可用区实例时，填写ZoneIds.N字段中的任意一个值
+        :param ZoneId: 可用区。当购买多可用区实例时，当前参数为主可用区。需要保证传入的参数和 SubnetId 所在子网属于同一个可用区
         :type ZoneId: int
         :param Period: 预付费购买时长，例如 "1m",就是一个月
         :type Period: str
-        :param InstanceType: 实例规格说明 专业版实例[所有规格]填写1.
-标准版实例 ([入门型(general)]填写1，[标准型(standard)]填写2，[进阶型(advanced)]填写3，[容量型(capacity)]填写4，[高阶型1(specialized-1)]填写5，[高阶型2(specialized-2)]填写6,[高阶型3(specialized-3)]填写7,[高阶型4(specialized-4)]填写8，[独占型(exclusive)]填写9。
+        :param InstanceType: 国际站标准版实例规格。目前只有国际站标准版使用当前字段区分规格，国内站标准版使用峰值带宽区分规格。除了国际站标准版外的所有实例填写 1 即可。国际站标准版实例：入门型(general)]填写1；[标准型(standard)]填写2；[进阶型(advanced)]填写3；[容量型(capacity)]填写4；[高阶型1(specialized-1)]填写5；[高阶型2(specialized-2)]填写6；[高阶型3(specialized-3)]填写7；[高阶型4(specialized-4)]填写8。
         :type InstanceType: int
-        :param VpcId: vpcId必填
+        :param VpcId: vpcId，必填
         :type VpcId: str
-        :param SubnetId: 子网id，vpc网络需要传该参数，基础网络可以不传
+        :param SubnetId: 子网id，必填
         :type SubnetId: str
         :param MsgRetentionTime: 可选。实例日志的最长保留时间，单位分钟，默认为10080（7天），最大30天，不填默认0，代表不开启日志保留时间回收策略
         :type MsgRetentionTime: int
         :param ClusterId: 创建实例时可以选择集群Id, 该入参表示集群Id
         :type ClusterId: int
         :param RenewFlag: 预付费自动续费标记，0表示默认状态(用户未设置，即初始状态)， 1表示自动续费，2表示明确不自动续费(用户设置)
         :type RenewFlag: int
         :param KafkaVersion: CKafka版本号[0.10.2、1.1.1、2.4.1、2.4.2、2.8.1], 默认是1.1.1。2.4.1 与 2.4.2 属于同一个版本，传任意一个均可。
         :type KafkaVersion: str
-        :param SpecificationsType: 实例类型: [标准版实例]填写 standard(默认), [专业版实例]填写 profession
+        :param SpecificationsType: 实例类型: [标准版实例]填写 "standard" (默认), [专业版实例]填写 "profession"
         :type SpecificationsType: str
-        :param DiskSize: 磁盘大小，专业版不填写默认最小磁盘，如果跟控制台规格配比不相符，则无法创建成功
+        :param DiskSize: 磁盘大小，如果跟控制台规格配比不相符，则无法创建成功
         :type DiskSize: int
-        :param BandWidth: 带宽，专业版不填写默认最小带宽，如果跟控制台规格配比不相符，则无法创建成功
+        :param BandWidth: 带宽，如果跟控制台规格配比不相符，则无法创建成功
         :type BandWidth: int
-        :param Partition: 分区大小，专业版不填写默认最小分区数，如果跟控制台规格配比不相符，则无法创建成功
+        :param Partition: 分区大小，如果跟控制台规格配比不相符，则无法创建成功
         :type Partition: int
         :param Tags: 标签
         :type Tags: list of Tag
-        :param DiskType: 磁盘类型（ssd填写CLOUD_SSD，sata填写CLOUD_BASIC）
+        :param DiskType: 专业版实例磁盘类型，标准版实例不需要填写。"CLOUD_SSD"：SSD云硬盘；"CLOUD_BASIC"：高性能云硬盘。不传默认为 "CLOUD_BASIC"
         :type DiskType: str
-        :param MultiZoneFlag: 跨可用区，zoneIds必填
+        :param MultiZoneFlag: 是否创建跨可用区实例，当前参数为 true 时，zoneIds必填
         :type MultiZoneFlag: bool
         :param ZoneIds: 可用区列表，购买多可用区实例时为必填项
         :type ZoneIds: list of int
         :param PublicNetworkMonthly: 公网带宽大小，单位 Mbps。默认是没有加上免费 3Mbps 带宽。例如总共需要 3Mbps 公网带宽，此处传 0；总共需要 6Mbps 公网带宽，此处传 3。默认值为 0。需要保证传入参数为 3 的整数倍
         :type PublicNetworkMonthly: int
         :param InstanceNum: 购买实例数量。非必填，默认值为 1。当传入该参数时，会创建多个 instanceName 加后缀区分的实例
         :type InstanceNum: int
@@ -2717,25 +2716,25 @@
         r"""
         :param InstanceName: 实例名称，是一个不超过 64 个字符的字符串，必须以字母为首字符，剩余部分可以包含字母、数字和横划线(-)
         :type InstanceName: str
         :param VpcId: 创建的实例默认接入点所在的 vpc 对应 vpcId。目前不支持创建基础网络实例，因此该参数必填
         :type VpcId: str
         :param SubnetId: 子网id。创建实例默认接入点所在的子网对应的子网 id
         :type SubnetId: str
-        :param InstanceType: 实例规格。当创建标准版实例时必填，创建专业版实例时不需要填写。1：入门型；2：标准型；3：进阶型；4：容量型；5：高阶型1；6：高阶性2；7：高阶型3；8：高阶型4；9 ：独占型
+        :param InstanceType: 国际站标准版实例规格。目前只有国际站标准版使用当前字段区分规格，国内站标准版使用峰值带宽区分规格。除了国际站标准版外的所有实例填写 1 即可。国际站标准版实例：入门型(general)]填写1；[标准型(standard)]填写2；[进阶型(advanced)]填写3；[容量型(capacity)]填写4；[高阶型1(specialized-1)]填写5；[高阶型2(specialized-2)]填写6；[高阶型3(specialized-3)]填写7；[高阶型4(specialized-4)]填写8。
         :type InstanceType: int
         :param MsgRetentionTime: 实例日志的默认最长保留时间，单位分钟。不传入该参数时默认为 1440 分钟（1天），最大30天。当 topic 显式设置消息保留时间时，以 topic 保留时间为准
         :type MsgRetentionTime: int
         :param ClusterId: 创建实例时可以选择集群Id, 该入参表示集群Id。不指定实例所在集群则不传入该参数
         :type ClusterId: int
         :param KafkaVersion: 实例版本。目前支持 "0.10.2","1.1.1","2.4.1","2.4.2","2.8.1"。"2.4.1" 与 "2.4.2" 属于同一个版本，传任意一个均可。
         :type KafkaVersion: str
         :param SpecificationsType: 实例类型。"standard"：标准版，"profession"：专业版
         :type SpecificationsType: str
-        :param DiskType: 实例硬盘类型，"CLOUD_BASIC"：云硬盘，"CLOUD_SSD"：高速云硬盘。不传默认为 "CLOUD_BASIC"
+        :param DiskType: 专业版实例磁盘类型，标准版实例不需要填写。"CLOUD_SSD"：SSD云硬盘；"CLOUD_BASIC"：高性能云硬盘。不传默认值为 "CLOUD_BASIC"
         :type DiskType: str
         :param BandWidth: 实例内网峰值带宽。单位 MB/s。标准版需传入当前实例规格所对应的峰值带宽。注意如果创建的实例为专业版实例，峰值带宽，分区数等参数配置需要满足专业版的计费规格。
         :type BandWidth: int
         :param DiskSize: 实例硬盘大小，需要满足当前实例的计费规格
         :type DiskSize: int
         :param Partition: 实例最大分区数量，需要满足当前实例的计费规格
         :type Partition: int
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.925/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.926/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.925/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.926/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.925/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.926/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.925/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.926/setup.py`

 * *Files identical despite different names*

