# Comparing `tmp/tencentcloud-sdk-python-mgobe-3.0.925.tar.gz` & `tmp/tencentcloud-sdk-python-mgobe-3.0.926.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mgobe-3.0.925.tar", last modified: Fri Jun 30 02:17:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mgobe-3.0.926.tar", last modified: Mon Jul  3 00:30:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mgobe-3.0.925.tar` & `tencentcloud-sdk-python-mgobe-3.0.926.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20201014/
--rw-r--r--   0 root         (0) root         (0)     8244 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20201014/mgobe_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20201014/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20430 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20201014/models.py
--rw-r--r--   0 root         (0) root         (0)    34111 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20201014/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20190929/
--rw-r--r--   0 root         (0) root         (0)     1855 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20190929/mgobe_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20190929/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20190929/models.py
--rw-r--r--   0 root         (0) root         (0)    34005 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20190929/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/README.rst
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud_sdk_python_mgobe.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud_sdk_python_mgobe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud_sdk_python_mgobe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-30 02:17:40.000000 tencentcloud-sdk-python-mgobe-3.0.925/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/setup.py
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud_sdk_python_mgobe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud_sdk_python_mgobe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud_sdk_python_mgobe.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20201014/
+-rw-r--r--   0 root         (0) root         (0)    20430 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20201014/models.py
+-rw-r--r--   0 root         (0) root         (0)     8244 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20201014/mgobe_client.py
+-rw-r--r--   0 root         (0) root         (0)    34111 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20201014/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20201014/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20190929/
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20190929/models.py
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20190929/mgobe_client.py
+-rw-r--r--   0 root         (0) root         (0)    34005 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20190929/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20190929/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 00:30:22.000000 tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/__init__.py
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20201014/mgobe_client.py` & `tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20201014/mgobe_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20201014/models.py` & `tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20201014/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20201014/errorcodes.py` & `tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20201014/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20190929/mgobe_client.py` & `tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20190929/mgobe_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20190929/models.py` & `tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20190929/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud/mgobe/v20190929/errorcodes.py` & `tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud/mgobe/v20190929/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.925/README.rst` & `tencentcloud-sdk-python-mgobe-3.0.926/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.925/PKG-INFO` & `tencentcloud-sdk-python-mgobe-3.0.926/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mgobe
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Mgobe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud_sdk_python_mgobe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mgobe-3.0.925/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mgobe-3.0.926/tencentcloud_sdk_python_mgobe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mgobe
-Version: 3.0.925
+Version: 3.0.926
 Summary: Tencent Cloud Mgobe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mgobe-3.0.925/setup.py` & `tencentcloud-sdk-python-mgobe-3.0.926/setup.py`

 * *Files identical despite different names*

