# Comparing `tmp/tencentcloud-sdk-python-cme-3.0.925.tar.gz` & `tmp/tencentcloud-sdk-python-cme-3.0.926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cme-3.0.925.tar", last modified: Fri Jun 30 02:04:05 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cme-3.0.926.tar", last modified: Mon Jul  3 00:22:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cme-3.0.925.tar` & `tencentcloud-sdk-python-cme-3.0.926.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/tencentcloud/cme/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/tencentcloud/cme/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/tencentcloud/cme/v20191029/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/tencentcloud/cme/v20191029/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55291 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/tencentcloud/cme/v20191029/cme_client.py
--rw-r--r--   0 root         (0) root         (0)   298970 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/tencentcloud/cme/v20191029/models.py
--rw-r--r--   0 root         (0) root         (0)     8415 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/tencentcloud/cme/v20191029/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/tencentcloud_sdk_python_cme.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/tencentcloud_sdk_python_cme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/tencentcloud_sdk_python_cme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/tencentcloud_sdk_python_cme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:04:05.000000 tencentcloud-sdk-python-cme-3.0.925/tencentcloud_sdk_python_cme.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/tencentcloud_sdk_python_cme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/tencentcloud_sdk_python_cme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/tencentcloud_sdk_python_cme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/tencentcloud_sdk_python_cme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/tencentcloud_sdk_python_cme.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/tencentcloud/cme/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/tencentcloud/cme/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/tencentcloud/cme/v20191029/
+-rw-r--r--   0 root         (0) root         (0)   298964 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/tencentcloud/cme/v20191029/models.py
+-rw-r--r--   0 root         (0) root         (0)    55254 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/tencentcloud/cme/v20191029/cme_client.py
+-rw-r--r--   0 root         (0) root         (0)     8415 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/tencentcloud/cme/v20191029/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/tencentcloud/cme/v20191029/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:22:54.000000 tencentcloud-sdk-python-cme-3.0.926/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-cme-3.0.925/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cme-3.0.926/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cme-3.0.925/tencentcloud/cme/v20191029/cme_client.py` & `tencentcloud-sdk-python-cme-3.0.926/tencentcloud/cme/v20191029/cme_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -849,28 +849,28 @@
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def HandleMediaCastProject(self, request):
         """对媒体转推项目进行操作。
         ### 操作类型<a id="Operation"></a>
-        - `AddSource`（添加输入源），项目状态为 Idle、Working 时均可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B12-.E6.B7.BB.E5.8A.A0.E8.BE.93.E5.85.A5.E6.BA.90)；
-        - `DeleteSource`（删除输入源），项目状态为 Idle、Working 时均可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B7-.E5.88.A0.E9.99.A4.E8.BE.93.E5.85.A5.E6.BA.90)；
-        - `SwitchSource`（切换当前播放的输入源），项目状态为 Working 时可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B6-.E5.88.87.E6.8D.A2.E5.BD.93.E5.89.8D.E6.92.AD.E6.94.BE.E7.9A.84.E8.BE.93.E5.85.A5.E6.BA.90)
-        - `AddDestination`（ 添加输出源），项目状态为 Idle、Working 时均可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B13-.E6.B7.BB.E5.8A.A0.E8.BE.93.E5.87.BA.E6.BA.90)；
-        - `DeleteDestination`（删除输出源），项目状态为 Idle、Working 时均可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B8-.E5.88.A0.E9.99.A4.E8.BE.93.E5.87.BA.E6.BA.90)；
-        - `EnableDestination`（启动输出源），项目状态为 Working 时可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B10-.E5.90.AF.E5.8A.A8.E8.BE.93.E5.87.BA.E6.BA.90)；
-        - `DisableDestination`（停止输出源），项目状态为 Working 时可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B5-.E5.81.9C.E6.AD.A2.E8.BE.93.E5.87.BA.E6.BA.90)；
+        - `AddSource`（添加输入源），项目状态为 Idle、Working 时均可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B9-.E6.B7.BB.E5.8A.A0.E8.BE.93.E5.85.A5.E6.BA.90)；
+        - `DeleteSource`（删除输入源），项目状态为 Idle、Working 时均可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B6-.E5.88.A0.E9.99.A4.E8.BE.93.E5.85.A5.E6.BA.90)；
+        - `SwitchSource`（切换当前播放的输入源），项目状态为 Working 时可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B5-.E5.88.87.E6.8D.A2.E5.BD.93.E5.89.8D.E6.92.AD.E6.94.BE.E7.9A.84.E8.BE.93.E5.85.A5.E6.BA.90)
+        - `AddDestination`（ 添加输出源），项目状态为 Idle、Working 时均可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B8-.E5.90.AF.E5.8A.A8.E8.BE.93.E5.87.BA.E6.BA.90)；
+        - `DeleteDestination`（删除输出源），项目状态为 Idle、Working 时均可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B7-.E5.88.A0.E9.99.A4.E8.BE.93.E5.87.BA.E6.BA.90)；
+        - `EnableDestination`（启动输出源），项目状态为 Working 时可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B8-.E5.90.AF.E5.8A.A8.E8.BE.93.E5.87.BA.E6.BA.90)；
+        - `DisableDestination`（停止输出源），项目状态为 Working 时可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B4-.E5.81.9C.E6.AD.A2.E8.BE.93.E5.87.BA.E6.BA.90)；
         - `ModifyDestination`（修改输出源），项目状态为 Idle、Working 时均可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B2-.E4.BF.AE.E6.94.B9.E8.BE.93.E5.87.BA.E6.BA.90)；
-        - `Start`（启动媒体转推），项目状态为 Idle 时可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B9-.E5.90.AF.E5.8A.A8.E7.82.B9.E6.92.AD.E8.BD.AC.E7.9B.B4.E6.92.AD)。发起 Start 请求成功后，媒体转推项目开始启动，30秒内还需要再进行一次 Confirm操作进行确认；
-        - `Confirm`（确认媒体转推项目启动），项目状态为 Working 时可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B14-.E7.A1.AE.E8.AE.A4.E7.82.B9.E6.92.AD.E8.BD.AC.E7.9B.B4.E6.92.AD.E9.A1.B9.E7.9B.AE.E5.90.AF.E5.8A.A8)；
-        - `Stop`（停止媒体转推），项目状态为 Working 时可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B4-.E5.81.9C.E6.AD.A2.E7.82.B9.E6.92.AD.E8.BD.AC.E7.9B.B4.E6.92.AD)；
+        - `Start`（启动媒体转推），项目状态为 Idle 时可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B12-.E5.90.AF.E5.8A.A8.E5.AA.92.E4.BD.93.E8.BD.AC.E6.8E.A8)。发起 Start 请求成功后，媒体转推项目开始启动，30秒内还需要再进行一次 Confirm操作进行确认；
+        - `Confirm`（确认媒体转推项目启动），项目状态为 Working 时可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B14-.E7.A1.AE.E8.AE.A4.E5.AA.92.E4.BD.93.E8.BD.AC.E6.8E.A8.E9.A1.B9.E7.9B.AE.E5.90.AF.E5.8A.A8)；
+        - `Stop`（停止媒体转推），项目状态为 Working 时可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B11-.E5.81.9C.E6.AD.A2.E5.AA.92.E4.BD.93.E8.BD.AC.E6.8E.A8)；
         - `ModifyOutputMediaSetting`（修改媒体输出配置），项目状态为 Idle 时可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B3-.E4.BF.AE.E6.94.B9.E8.BE.93.E5.87.BA.E7.9A.84.E5.AA.92.E4.BD.93.E9.85.8D.E7.BD.AE)；
         - `ModifyPlaySetting`（修改播放结束时间），项目状态为 Idle、Working 时均可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B1-.E4.BF.AE.E6.94.B9.E7.BB.93.E6.9D.9F.E6.97.B6.E9.97.B4);
-        - `DescribePlayInfo`（查询播放信息），项目状态为 Idle、Working 时均可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B11-.E6.9F.A5.E8.AF.A2.E7.82.B9.E6.92.AD.E8.BD.AC.E7.9B.B4.E6.92.AD.E9.A1.B9.E7.9B.AE.E7.9A.84.E6.92.AD.E6.94.BE.E4.BF.A1.E6.81.AF)。
+        - `DescribePlayInfo`（查询播放信息），项目状态为 Idle、Working 时均可以操作。参见 [示例](#.E7.A4.BA.E4.BE.8B13-.E6.9F.A5.E8.AF.A2.E5.AA.92.E4.BD.93.E8.BD.AC.E6.8E.A8.E9.A1.B9.E7.9B.AE.E7.9A.84.E6.92.AD.E6.94.BE.E4.BF.A1.E6.81.AF)。
 
         :param request: Request instance for HandleMediaCastProject.
         :type request: :class:`tencentcloud.cme.v20191029.models.HandleMediaCastProjectRequest`
         :rtype: :class:`tencentcloud.cme.v20191029.models.HandleMediaCastProjectResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-cme-3.0.925/tencentcloud/cme/v20191029/models.py` & `tencentcloud-sdk-python-cme-3.0.926/tencentcloud/cme/v20191029/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -776,15 +776,15 @@
         :type Owner: :class:`tencentcloud.cme.v20191029.models.Entity`
         :param Category: 项目类别，取值有：
 <li>VIDEO_EDIT：视频编辑。</li>
 <li>SWITCHER：导播台。</li>
 <li>VIDEO_SEGMENTATION：视频拆条。</li>
 <li>STREAM_CONNECT：云转推。</li>
 <li>RECORD_REPLAY：录制回放。</li>
-<li>MEDIA_CAST：点播转直播。</li>
+<li>MEDIA_CAST：媒体转推。</li>
         :type Category: str
         :param Mode: 项目模式，一个项目可以有多种模式并相互切换。
 当 Category 为 VIDEO_EDIT 时，可选模式有：
 <li>Default：默认模式，即普通视频编辑项目。</li>
 <li>VideoEditTemplate：剪辑模板制作模式，用于制作剪辑模板。</li>
 
 注：不填则为默认模式。
@@ -4685,15 +4685,15 @@
 <li>VOD：云点播的媒资文件。</li>
 <li>EXTERNAL：非多媒体创建引擎或者云点播的媒资文件。</li>
         :type Type: str
         :param FileId: 云点播媒体文件 ID。当 Type = VOD 时必填。
         :type FileId: str
         :param MaterialId: 多媒体创作引擎的媒体 ID。当 Type = CME  时必填。
         :type MaterialId: str
-        :param Offset: 文件播放的的起始位置，单位：秒。默认为0，从文件头开始播放。当 Type = CME  或者 VOD 时有效。
+        :param Offset: 文件播放的起始位置，单位：秒。默认为0，从文件头开始播放。当 Type = CME  或者 VOD 时有效。
         :type Offset: float
         :param Duration: 播放时长，单位：秒。默认播放整个文件。当 Type = CME  或者 VOD 时有效。
         :type Duration: float
         :param Url: 外部文件的 Url， Type=EXTERNAL 时必填，可以是点播文件或者直播文件，支持的 Scheme 包括HTTP、HTTPS、RTMP。
         :type Url: str
         """
         self.Id = None
```

### Comparing `tencentcloud-sdk-python-cme-3.0.925/tencentcloud/cme/v20191029/errorcodes.py` & `tencentcloud-sdk-python-cme-3.0.926/tencentcloud/cme/v20191029/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cme-3.0.925/README.rst` & `tencentcloud-sdk-python-cme-3.0.926/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cme-3.0.925/PKG-INFO` & `tencentcloud-sdk-python-cme-3.0.926/tencentcloud_sdk_python_cme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cme
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Cme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cme-3.0.925/setup.py` & `tencentcloud-sdk-python-cme-3.0.926/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cme-3.0.925/tencentcloud_sdk_python_cme.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cme-3.0.926/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cme
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Cme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

