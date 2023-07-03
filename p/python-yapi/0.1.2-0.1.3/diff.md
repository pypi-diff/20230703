# Comparing `tmp/python_yapi-0.1.2.tar.gz` & `tmp/python_yapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_yapi-0.1.2.tar", last modified: Sun Jul  2 09:17:45 2023, max compression
+gzip compressed data, was "python_yapi-0.1.3.tar", last modified: Mon Jul  3 08:35:41 2023, max compression
```

## Comparing `python_yapi-0.1.2.tar` & `python_yapi-0.1.3.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-02 09:17:45.784664 python_yapi-0.1.2/
--rw-r--r--   0 superhin   (502) staff       (20)      153 2023-06-28 07:02:56.000000 python_yapi-0.1.2/AUTHORS.rst
--rw-r--r--   0 superhin   (502) staff       (20)     3562 2023-06-28 08:12:06.000000 python_yapi-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 superhin   (502) staff       (20)       89 2023-06-28 07:02:56.000000 python_yapi-0.1.2/HISTORY.rst
--rw-r--r--   0 superhin   (502) staff       (20)     1068 2023-06-10 12:41:28.000000 python_yapi-0.1.2/LICENSE
--rw-r--r--   0 superhin   (502) staff       (20)      137 2023-06-10 12:41:28.000000 python_yapi-0.1.2/MANIFEST.in
--rw-r--r--   0 superhin   (502) staff       (20)     1476 2023-07-02 09:17:45.784906 python_yapi-0.1.2/PKG-INFO
--rw-r--r--   0 superhin   (502) staff       (20)     1005 2023-07-02 08:53:16.000000 python_yapi-0.1.2/README.md
--rw-r--r--   0 superhin   (502) staff       (20)     2761 2023-06-28 06:53:34.000000 python_yapi-0.1.2/README.rst
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-02 09:17:45.773514 python_yapi-0.1.2/python_yapi/
--rw-r--r--   0 superhin   (502) staff       (20)       42 2023-06-28 03:57:06.000000 python_yapi-0.1.2/python_yapi/__init__.py
--rw-r--r--   0 superhin   (502) staff       (20)     3546 2023-06-30 12:47:33.000000 python_yapi-0.1.2/python_yapi/base.py
--rw-r--r--   0 superhin   (502) staff       (20)      448 2023-06-28 07:02:56.000000 python_yapi-0.1.2/python_yapi/cli.py
--rw-r--r--   0 superhin   (502) staff       (20)      295 2023-06-28 03:56:07.000000 python_yapi-0.1.2/python_yapi/collection.py
--rw-r--r--   0 superhin   (502) staff       (20)      202 2023-06-30 11:36:46.000000 python_yapi-0.1.2/python_yapi/constants.py
--rw-r--r--   0 superhin   (502) staff       (20)      347 2023-06-30 12:24:32.000000 python_yapi-0.1.2/python_yapi/exceptions.py
--rw-r--r--   0 superhin   (502) staff       (20)      336 2023-06-28 09:01:36.000000 python_yapi-0.1.2/python_yapi/follow.py
--rw-r--r--   0 superhin   (502) staff       (20)     1361 2023-06-30 11:59:22.000000 python_yapi-0.1.2/python_yapi/group.py
--rw-r--r--   0 superhin   (502) staff       (20)     2224 2023-07-02 08:54:14.000000 python_yapi-0.1.2/python_yapi/interface.py
--rw-r--r--   0 superhin   (502) staff       (20)      307 2023-06-28 08:57:31.000000 python_yapi-0.1.2/python_yapi/log.py
--rw-r--r--   0 superhin   (502) staff       (20)     1286 2023-06-28 09:45:42.000000 python_yapi-0.1.2/python_yapi/models.py
--rw-r--r--   0 superhin   (502) staff       (20)    14308 2023-06-30 13:00:29.000000 python_yapi-0.1.2/python_yapi/project.py
--rw-r--r--   0 superhin   (502) staff       (20)     3409 2023-06-30 12:51:34.000000 python_yapi-0.1.2/python_yapi/user.py
--rw-r--r--   0 superhin   (502) staff       (20)      993 2023-06-28 04:36:56.000000 python_yapi-0.1.2/python_yapi/utils.py
--rw-r--r--   0 superhin   (502) staff       (20)      260 2023-06-30 09:01:05.000000 python_yapi-0.1.2/python_yapi/yapi.py
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-02 09:17:45.778959 python_yapi-0.1.2/python_yapi.egg-info/
--rw-r--r--   0 superhin   (502) staff       (20)     1476 2023-07-02 09:17:45.000000 python_yapi-0.1.2/python_yapi.egg-info/PKG-INFO
--rw-r--r--   0 superhin   (502) staff       (20)      732 2023-07-02 09:17:45.000000 python_yapi-0.1.2/python_yapi.egg-info/SOURCES.txt
--rw-r--r--   0 superhin   (502) staff       (20)        1 2023-07-02 09:17:45.000000 python_yapi-0.1.2/python_yapi.egg-info/dependency_links.txt
--rw-r--r--   0 superhin   (502) staff       (20)       12 2023-07-02 09:17:45.000000 python_yapi-0.1.2/python_yapi.egg-info/top_level.txt
--rw-r--r--   0 superhin   (502) staff       (20)        1 2023-06-10 12:41:40.000000 python_yapi-0.1.2/python_yapi.egg-info/zip-safe
--rw-r--r--   0 superhin   (502) staff       (20)      216 2023-06-30 11:38:00.000000 python_yapi-0.1.2/requirements_dev.txt
--rw-r--r--   0 superhin   (502) staff       (20)       24 2023-06-30 10:48:01.000000 python_yapi-0.1.2/requirments.txt
--rw-r--r--   0 superhin   (502) staff       (20)      428 2023-07-02 09:17:45.785935 python_yapi-0.1.2/setup.cfg
--rw-r--r--   0 superhin   (502) staff       (20)     1183 2023-07-02 09:17:36.000000 python_yapi-0.1.2/setup.py
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-02 09:17:45.783845 python_yapi-0.1.2/tests/
--rw-r--r--   0 superhin   (502) staff       (20)        0 2023-06-10 13:10:56.000000 python_yapi-0.1.2/tests/test_base_api.py
--rw-r--r--   0 superhin   (502) staff       (20)      491 2023-06-30 11:59:56.000000 python_yapi-0.1.2/tests/test_group.py
--rw-r--r--   0 superhin   (502) staff       (20)     2650 2023-06-30 12:49:41.000000 python_yapi-0.1.2/tests/test_project.py
--rw-r--r--   0 superhin   (502) staff       (20)      275 2023-06-30 09:09:18.000000 python_yapi-0.1.2/tests/test_user.py
--rw-r--r--   0 superhin   (502) staff       (20)      542 2023-06-28 07:02:56.000000 python_yapi-0.1.2/tox.ini
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-03 08:35:41.875370 python_yapi-0.1.3/
+-rw-r--r--   0 superhin   (502) staff       (20)      153 2023-06-28 07:02:56.000000 python_yapi-0.1.3/AUTHORS.rst
+-rw-r--r--   0 superhin   (502) staff       (20)     3562 2023-06-28 08:12:06.000000 python_yapi-0.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 superhin   (502) staff       (20)       89 2023-06-28 07:02:56.000000 python_yapi-0.1.3/HISTORY.rst
+-rw-r--r--   0 superhin   (502) staff       (20)     1068 2023-06-10 12:41:28.000000 python_yapi-0.1.3/LICENSE
+-rw-r--r--   0 superhin   (502) staff       (20)      137 2023-06-10 12:41:28.000000 python_yapi-0.1.3/MANIFEST.in
+-rw-r--r--   0 superhin   (502) staff       (20)     2965 2023-07-03 08:35:41.875618 python_yapi-0.1.3/PKG-INFO
+-rw-r--r--   0 superhin   (502) staff       (20)     2482 2023-07-03 08:34:46.000000 python_yapi-0.1.3/README.md
+-rw-r--r--   0 superhin   (502) staff       (20)     2761 2023-06-28 06:53:34.000000 python_yapi-0.1.3/README.rst
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-03 08:35:41.867350 python_yapi-0.1.3/python_yapi/
+-rw-r--r--   0 superhin   (502) staff       (20)       45 2023-07-03 02:27:56.000000 python_yapi-0.1.3/python_yapi/__init__.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3546 2023-06-30 12:47:33.000000 python_yapi-0.1.3/python_yapi/base.py
+-rw-r--r--   0 superhin   (502) staff       (20)      448 2023-06-28 07:02:56.000000 python_yapi-0.1.3/python_yapi/cli.py
+-rw-r--r--   0 superhin   (502) staff       (20)      295 2023-06-28 03:56:07.000000 python_yapi-0.1.3/python_yapi/collection.py
+-rw-r--r--   0 superhin   (502) staff       (20)      202 2023-06-30 11:36:46.000000 python_yapi-0.1.3/python_yapi/constants.py
+-rw-r--r--   0 superhin   (502) staff       (20)      347 2023-06-30 12:24:32.000000 python_yapi-0.1.3/python_yapi/exceptions.py
+-rw-r--r--   0 superhin   (502) staff       (20)      336 2023-06-28 09:01:36.000000 python_yapi-0.1.3/python_yapi/follow.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1361 2023-06-30 11:59:22.000000 python_yapi-0.1.3/python_yapi/group.py
+-rw-r--r--   0 superhin   (502) staff       (20)    12583 2023-07-03 08:12:29.000000 python_yapi-0.1.3/python_yapi/interface.py
+-rw-r--r--   0 superhin   (502) staff       (20)      307 2023-06-28 08:57:31.000000 python_yapi-0.1.3/python_yapi/log.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1286 2023-06-28 09:45:42.000000 python_yapi-0.1.3/python_yapi/models.py
+-rw-r--r--   0 superhin   (502) staff       (20)    14594 2023-07-03 02:40:58.000000 python_yapi-0.1.3/python_yapi/project.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3409 2023-06-30 12:51:34.000000 python_yapi-0.1.3/python_yapi/user.py
+-rw-r--r--   0 superhin   (502) staff       (20)      993 2023-06-28 04:36:56.000000 python_yapi-0.1.3/python_yapi/utils.py
+-rw-r--r--   0 superhin   (502) staff       (20)      260 2023-06-30 09:01:05.000000 python_yapi-0.1.3/python_yapi/yapi.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-03 08:35:41.871044 python_yapi-0.1.3/python_yapi.egg-info/
+-rw-r--r--   0 superhin   (502) staff       (20)     2965 2023-07-03 08:35:41.000000 python_yapi-0.1.3/python_yapi.egg-info/PKG-INFO
+-rw-r--r--   0 superhin   (502) staff       (20)      790 2023-07-03 08:35:41.000000 python_yapi-0.1.3/python_yapi.egg-info/SOURCES.txt
+-rw-r--r--   0 superhin   (502) staff       (20)        1 2023-07-03 08:35:41.000000 python_yapi-0.1.3/python_yapi.egg-info/dependency_links.txt
+-rw-r--r--   0 superhin   (502) staff       (20)       40 2023-07-03 08:35:41.000000 python_yapi-0.1.3/python_yapi.egg-info/requires.txt
+-rw-r--r--   0 superhin   (502) staff       (20)       12 2023-07-03 08:35:41.000000 python_yapi-0.1.3/python_yapi.egg-info/top_level.txt
+-rw-r--r--   0 superhin   (502) staff       (20)        1 2023-06-10 12:41:40.000000 python_yapi-0.1.3/python_yapi.egg-info/zip-safe
+-rw-r--r--   0 superhin   (502) staff       (20)      216 2023-06-30 11:38:00.000000 python_yapi-0.1.3/requirements_dev.txt
+-rw-r--r--   0 superhin   (502) staff       (20)       24 2023-06-30 10:48:01.000000 python_yapi-0.1.3/requirments.txt
+-rw-r--r--   0 superhin   (502) staff       (20)      428 2023-07-03 08:35:41.876367 python_yapi-0.1.3/setup.cfg
+-rw-r--r--   0 superhin   (502) staff       (20)     1241 2023-07-03 08:34:46.000000 python_yapi-0.1.3/setup.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-03 08:35:41.874621 python_yapi-0.1.3/tests/
+-rw-r--r--   0 superhin   (502) staff       (20)        0 2023-06-10 13:10:56.000000 python_yapi-0.1.3/tests/test_base_api.py
+-rw-r--r--   0 superhin   (502) staff       (20)      491 2023-06-30 11:59:56.000000 python_yapi-0.1.3/tests/test_group.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3301 2023-07-03 08:26:57.000000 python_yapi-0.1.3/tests/test_interface.py
+-rw-r--r--   0 superhin   (502) staff       (20)     2650 2023-07-03 08:15:29.000000 python_yapi-0.1.3/tests/test_project.py
+-rw-r--r--   0 superhin   (502) staff       (20)      275 2023-06-30 09:09:18.000000 python_yapi-0.1.3/tests/test_user.py
+-rw-r--r--   0 superhin   (502) staff       (20)      542 2023-06-28 07:02:56.000000 python_yapi-0.1.3/tox.ini
```

### Comparing `python_yapi-0.1.2/CONTRIBUTING.rst` & `python_yapi-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python_yapi-0.1.2/LICENSE` & `python_yapi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_yapi-0.1.2/README.rst` & `python_yapi-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `python_yapi-0.1.2/python_yapi/base.py` & `python_yapi-0.1.3/python_yapi/base.py`

 * *Files identical despite different names*

### Comparing `python_yapi-0.1.2/python_yapi/group.py` & `python_yapi-0.1.3/python_yapi/group.py`

 * *Files identical despite different names*

### Comparing `python_yapi-0.1.2/python_yapi/models.py` & `python_yapi-0.1.3/python_yapi/models.py`

 * *Files identical despite different names*

### Comparing `python_yapi-0.1.2/python_yapi/project.py` & `python_yapi-0.1.3/python_yapi/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         params = {
             'group_id': group_id,
             'page': page,
             'limit': limit
         }
         return self.get(url, params=params)
 
-    def get_project(self, project_id: int):
+    def get_project(self, project_id: int) -> dict:
         """
         Get a project.
         :param project_id:
         :return:
             eg: {'_id': 55,
                  'add_time': 1688125162,
                  'basepath': '/leslie-medina',
@@ -131,14 +131,22 @@
                  'uid': 15,
                  'up_time': 1688126042}
         """
         url = 'api/project/get'
         params = {'id': project_id}
         return self.get(url, params=params)
 
+    def get_project_cat(self, project_id: int) -> list:
+        data = self.get_project(project_id)
+        return data['cat']
+
+    def get_project_default_category_id(self, project_id: int) -> int:
+        data = self.get_project_cat(project_id)
+        return data[0]['_id']
+
     def get_project_tag(self, project_id: int) -> List[dict]:
         return self.get_project(project_id)['tag']
 
     def search_project(self, keyword: str):
         """
         Search project by keyword
         :param keyword:
```

### Comparing `python_yapi-0.1.2/python_yapi/user.py` & `python_yapi-0.1.3/python_yapi/user.py`

 * *Files identical despite different names*

### Comparing `python_yapi-0.1.2/python_yapi/utils.py` & `python_yapi-0.1.3/python_yapi/utils.py`

 * *Files identical despite different names*

### Comparing `python_yapi-0.1.2/python_yapi.egg-info/SOURCES.txt` & `python_yapi-0.1.3/python_yapi.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -24,13 +24,15 @@
 python_yapi/project.py
 python_yapi/user.py
 python_yapi/utils.py
 python_yapi/yapi.py
 python_yapi.egg-info/PKG-INFO
 python_yapi.egg-info/SOURCES.txt
 python_yapi.egg-info/dependency_links.txt
+python_yapi.egg-info/requires.txt
 python_yapi.egg-info/top_level.txt
 python_yapi.egg-info/zip-safe
 tests/test_base_api.py
 tests/test_group.py
+tests/test_interface.py
 tests/test_project.py
 tests/test_user.py
```

### Comparing `python_yapi-0.1.2/setup.py` & `python_yapi-0.1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """The setup script."""
 import os
-from setuptools import setup, find_packages
 
-version = '0.1.2'
+from setuptools import setup, find_packages
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
-setup_requirements = ['requests',
-                      'python-slugify']
+
+__author__ = """Han Zhichao"""
+__email__ = 'superhin@126.com'
+__version__ = '0.1.3'
+
+setup_requirements = []
+install_requires = [
+    'requests',
+    'python-slugify',
+    'urllib3==1.26.6',
+]
+
 
 def read_file(filename):
     with open(os.path.join(this_directory, filename), encoding='utf-8') as f:
-        long_description = f.read()
-    return long_description
+        return f.read()
 
 
 setup(
-    author="Han Zhichao",
-    author_email='superhin@126.com',
+    name='python_yapi',
+    version=__version__,
+    author=__author__,
+    author_email=__email__,
+    license="MIT license",
     description='python yapi sdk',
     long_description=read_file('README.md'),
-    long_description_content_type="text/markdown",  # 新参数
+    long_description_content_type="text/markdown",
+    url='https://github.com/hanzhichao/python-yapi',
+
+    include_package_data=True,
+    packages=find_packages(include=['python_yapi']),
+    zip_safe=True,
+    setup_requires=setup_requirements,
+    install_requires=install_requires,
+    keywords=['yapi', 'python-yapi', 'pyyapi', 'yapi-client'],
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.7',
     ],
-    license="MIT license",
-    include_package_data=True,
-    keywords=[
-        'yapi', 'python-yapi', 'pyyapi',
-    ],
-    name='python_yapi',
-    packages=find_packages(include=['python_yapi']),
-    setup_requires=setup_requirements,
-    url='https://github.com/hanzhichao/python-yapi',
-    version=version,
-    zip_safe=True,
-    install_requires=[]
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python_yapi-0.1.2/tests/test_project.py` & `python_yapi-0.1.3/tests/test_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from pprint import pprint
 
 
 class TestProject:
 
-    def test_get_project_list(self, yapi_admin):
-        print(yapi_admin.get_project_list())
+    def test_get_project_list(self, yapi_login):
+        print(yapi_login.get_project_list())
 
-    def test_get_project(self, yapi_admin):
-        print(yapi_admin.get_project(project_id=55))
+    def test_get_project(self, yapi_login):
+        print(yapi_login.get_project(project_id=55))
 
-    def test_add_project(self, yapi_admin):
-        print(yapi_admin.add_project(name='测试项目3'))
+    def test_add_project(self, yapi_login):
+        print(yapi_login.add_project(name='测试项目3'))
 
-    def test_delete_project(self, yapi_admin):
-        data = yapi_admin.delete_project(project_id=56)
+    def test_delete_project(self, yapi_login):
+        data = yapi_login.delete_project(project_id=56)
         pprint(data)
         # print(yapi_admin.get_project(project_id=33))
 
     def test_add_project_with_random_name(self, yapi, faker):
         yapi.login('zhangsan@126.com', 'abc123456')
         # data = yapi.get_my_group()
         # group_id = data['_id']
```

### Comparing `python_yapi-0.1.2/tox.ini` & `python_yapi-0.1.3/tox.ini`

 * *Files identical despite different names*

