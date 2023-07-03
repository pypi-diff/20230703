# Comparing `tmp/huhangkai-1.2.2.tar.gz` & `tmp/huhangkai-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.2.2.tar", last modified: Tue Jun  6 08:37:54 2023, max compression
+gzip compressed data, was "huhangkai-1.2.3.tar", last modified: Mon Jul  3 03:02:41 2023, max compression
```

## Comparing `huhangkai-1.2.2.tar` & `huhangkai-1.2.3.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 08:37:54.897881 huhangkai-1.2.2/
--rw-rw-rw-   0        0        0      228 2023-06-06 08:37:54.896884 huhangkai-1.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 08:37:54.884765 huhangkai-1.2.2/commen/
--rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.2.2/commen/__init__.py
--rw-rw-rw-   0        0        0    31571 2023-06-02 07:34:45.000000 huhangkai-1.2.2/commen/init_project.py
--rw-rw-rw-   0        0        0     4508 2023-05-25 08:37:49.000000 huhangkai-1.2.2/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-05-25 08:46:34.000000 huhangkai-1.2.2/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    22834 2023-06-06 08:37:33.000000 huhangkai-1.2.2/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-05-25 08:37:49.000000 huhangkai-1.2.2/commen/unit_logger.py
--rw-rw-rw-   0        0        0     9218 2023-06-02 10:02:56.000000 huhangkai-1.2.2/commen/unit_request.py
--rw-rw-rw-   0        0        0     2461 2023-05-25 08:37:49.000000 huhangkai-1.2.2/commen/unit_tasks.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:37:54.895887 huhangkai-1.2.2/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-06-06 08:37:54.000000 huhangkai-1.2.2/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-06-06 08:37:54.000000 huhangkai-1.2.2/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 08:37:54.000000 huhangkai-1.2.2/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-06-06 08:37:54.000000 huhangkai-1.2.2/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 08:37:54.000000 huhangkai-1.2.2/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 08:37:54.897881 huhangkai-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      600 2023-06-06 08:37:40.000000 huhangkai-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:02:41.244668 huhangkai-1.2.3/
+-rw-rw-rw-   0        0        0      228 2023-07-03 03:02:41.243671 huhangkai-1.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 03:02:41.228689 huhangkai-1.2.3/commen/
+-rw-rw-rw-   0        0        0      933 2023-06-20 02:22:12.000000 huhangkai-1.2.3/commen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:02:41.232700 huhangkai-1.2.3/commen/case_project/
+-rw-rw-rw-   0        0        0        0 2023-06-20 03:37:01.000000 huhangkai-1.2.3/commen/case_project/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-06-20 09:33:09.000000 huhangkai-1.2.3/commen/case_project/base_project.py
+-rw-rw-rw-   0        0        0    29301 2023-06-20 08:10:42.000000 huhangkai-1.2.3/commen/init_project.py
+-rw-rw-rw-   0        0        0    12278 2023-07-03 02:53:24.000000 huhangkai-1.2.3/commen/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-05-25 08:37:49.000000 huhangkai-1.2.3/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-05-25 08:46:34.000000 huhangkai-1.2.3/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    23116 2023-06-20 08:00:58.000000 huhangkai-1.2.3/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-05-25 08:37:49.000000 huhangkai-1.2.3/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     9218 2023-06-02 10:02:56.000000 huhangkai-1.2.3/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-06-29 01:27:06.000000 huhangkai-1.2.3/commen/unit_tasks.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:02:41.241677 huhangkai-1.2.3/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-07-03 03:02:41.000000 huhangkai-1.2.3/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-07-03 03:02:41.000000 huhangkai-1.2.3/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 03:02:41.000000 huhangkai-1.2.3/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-03 03:02:41.000000 huhangkai-1.2.3/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-03 03:02:41.000000 huhangkai-1.2.3/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 03:02:41.244668 huhangkai-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      643 2023-07-03 03:02:39.000000 huhangkai-1.2.3/setup.py
```

### Comparing `huhangkai-1.2.2/commen/__init__.py` & `huhangkai-1.2.3/commen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sys
 admin_host = "http://47.96.124.102/api"
-# admin_host = "http://127.0.0.1:8000"
+# admin_host = "http://127.0.0.1:8000/api"
 
 projects_path = os.getcwd()
 projects_path_list = projects_path.split(os.path.sep)
 if "site-packages" in projects_path_list and "commen" in projects_path_list:
     projects_path = os.path.join(*projects_path_list[:projects_path_list.index("site-packages") - 2])
 elif "service" in projects_path_list:
     projects_path = os.path.join(*projects_path_list[:projects_path_list.index("service")])
```

### Comparing `huhangkai-1.2.2/commen/init_project.py` & `huhangkai-1.2.3/commen/init_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,111 +1,84 @@
 import json
 import os.path
 import re
 import sys
 import requests
 import time
 
-from commen import admin_host, projects_path, service_path, testcase_path, files_path
+from commen.case_project.base_project import BaseProject
+from commen.unit_fun import FunBase
+from commen import service_path, testcase_path
 
 
-class GetApi:
+class GetApi(BaseProject):
     def __init__(self, api_type=1, value="", name="", yapi_url="", app_key=""):
         """api_type: 0时，value是swagger的api，json的url
                      1时，value值为yapi项目token,
                      2时，value是yapi下载的json文件名，文件放在file目录下,
                      3时，value是yapi的yapi-swagger.json
            name:项目名称，空时默认当前py文件所在文件名上级目录
         """
-        self.dir = projects_path
-        self.url = admin_host
-        self.api_testcase_list = []
-        self.api_testcase_file_str = ""
-        self.api_testcase_file_path = ""
-        self.sql_fun_list = None
-        self.name2 = None
-        self.api_fun_fun_list = None
-        self.api_fun_file_str = None
-        self.api_fun_file_path = None
-        self.assert_fun_list = None
-        self.assert_file_str = None
-        self.assert_file_path = None
-        self.sql_file_str = None
-        self.sql_file_str = None
-        self.sql_file_path = None
-        self.fun_init_list = None
-        self.fun_init_str = None
-        self.fun_file_path = None
-        self.fun_file_str = None
-        self.testcase_dir = ""
-        self.api_file_path = ""
-        self.service_dir = ""
-        self.api_file_str = ""
-        self.size_names = ("pageSize", "size")
-        self.page_names = ("pageNum", "current")
-        self.page_and_size = self.size_names + self.page_names
-        self.yapi_url = yapi_url
-        self.value = value
-        self.api_type = api_type
-        self.app_key = app_key
-        self.name = name
-        self.api_list_old = []
-        self.api_list = []
+        super().__init__(api_type, value, name, yapi_url, app_key)
         self.get_project()
         self.run()
 
     def get_project(self):
         if self.app_key:
             project = requests.post(self.url + '/variable/variable/',
                                     json={"app_key": self.app_key, "environment": "sit"}).json()
             if project.get('project'):
                 self.name = project.get('project')[0].get('code')
+                if project.get('api_settings'):
+                    self.api_type = project.get('api_settings')[0].get('api_type')
+                    if self.api_type == 2:
+                        self.yapi_file_str = requests.get(self.url + "/media/" +
+                                                          project.get('api_settings')[0].get('file')).text
+                    elif self.api_type in (0, 3):
+                        self.value = project.get('api_settings')[0].get('url')
+                    elif self.api_type == 1:
+                        self.yapi_url = project.get('api_settings')[0].get('url').strip()
+                        if self.yapi_url[-1] == "/":
+                            self.yapi_url = self.yapi_url[:-1]
+                        self.value = project.get('api_settings')[0].get('token')
             else:
-                self.name = "demo"
+                self.error = project.get('non_field_errors')[0]
+        self.name = self.name if self.name else "demo"
+        self.name2 = self.name.title()
 
-            if project.get('api_settings'):
-                self.api_type = project.get('api_settings')[0].get('api_type')
-                if self.api_type == 2:
-                    self.yapi_file_str = requests.get(self.url + "/media/" +
-                                                      project.get('api_settings')[0].get('file')).text
-                elif self.api_type in (0, 3):
-                    self.value = project.get('api_settings')[0].get('url')
-                elif self.api_type == 1:
-                    self.yapi_url = project.get('api_settings')[0].get('url').strip()
-                    if self.yapi_url[-1] == "/":
-                        self.yapi_url = self.yapi_url[:-1]
-                    self.value = project.get('api_settings')[0].get('token')
     def run(self):
         """
         创建项目
         """
+        if self.error:
+            print(self.error)
+            return False
         # 创建项目目录
         self.set_file_path()
         # 获取已维护api方法接口列表
         self.get_api_fun_list()
         # 获取全量api接口列表
         self.get_api_list()
         # 添加api封装方法
         self.write_api_fun()
 
     def get_api_fun_list(self):
-        """获取已维护方法列表，无则创建文件标题"""
-        self.name2 = self.name.title()
+        """获取已维护方法列表，无则创建demo文件"""
         self.api_file_path = os.path.join(self.service_dir, self.name + "_api.py")
         if os.path.exists(self.api_file_path):
-            self.api_file_str = self.read_file(self.api_file_path)
+            self.api_file_str = FunBase.read_file(self.api_file_path)
         else:
             self.api_file_str = "import allure\n\nfrom service.%s import http_requester\n" \
                                 "from commen.unit_request import get_url\n\n\n" % self.name
         tmp = re.findall("def +(.*)?\([\d\D]*?_method = [\"'](.*)?[\"']", self.api_file_str)
         self.api_list_old = re.findall("def +(.*)?\(", self.api_file_str)
 
         self.fun_file_path = os.path.join(self.service_dir, self.name + "_fun.py")
         if os.path.exists(self.fun_file_path):
-            self.fun_file_str = self.read_file(self.fun_file_path)
+            self.fun_file_str = FunBase.read_file(self.fun_file_path)
         else:
             self.fun_file_str = "import requests\n\nfrom commen.unit_fun import FunBase\n" \
                                 "from commen import admin_host\n\n\nclass %sFun(FunBase):\n" \
                                 "    def __init__(self):\n        super().__init__()\n        self.res = None\n\n" \
                                 "    def run_mysql(self, sql_str):\n" \
                                 "        # id是后台http://47.96.124.102/admin 项目数据库链接的id\n" \
                                 '        out = requests.post(admin_host + "/sql/running_sql/", ' \
@@ -117,115 +90,79 @@
                                 '    out = f.run_mysql("SELECT * FROM `t_accept_log`  LIMIT 1;")\n' \
                                 '    print(out)\n\n' % (self.name2, self.name2)
         self.fun_init_str = re.findall(r"(def +[\d\D]*?\n)\s*def", self.fun_file_str)[0]
         self.fun_init_list = [i.split('=')[0].strip()[5:] for i in self.fun_init_str.split('\n') if "=" in i]
 
         self.sql_file_path = os.path.join(self.service_dir, self.name + "_sql.py")
         if os.path.exists(self.sql_file_path):
-            self.sql_file_str = self.read_file(self.sql_file_path)
+            self.sql_file_str = FunBase.read_file(self.sql_file_path)
         else:
             self.sql_file_str = "from service.%s.%s_fun import %sFun\n\n\n" % (self.name, self.name, self.name2)
             self.sql_file_str += "class %sSql(%sFun):\n\n\n" \
                                  "if __name__ == '__main__':\n    s = %sSql()\n\n" % (
-                self.name2, self.name2, self.name2)
+                                     self.name2, self.name2, self.name2)
         self.sql_fun_list = re.findall("    def +(.*)?\(", self.sql_file_str)
 
         self.assert_file_path = os.path.join(self.service_dir, self.name + "_assert.py")
         if os.path.exists(self.assert_file_path):
-            self.assert_file_str = self.read_file(self.assert_file_path)
+            self.assert_file_str = FunBase.read_file(self.assert_file_path)
         else:
-            self.assert_file_str = "import allure\n\nfrom service.%s.%s_sql import %sSql\n\n\n" % (self.name, self.name, self.name2)
+            self.assert_file_str = "import allure\n\nfrom service.%s.%s_sql import %sSql\n\n\n" % (
+            self.name, self.name, self.name2)
             self.assert_file_str += "class %sAssert(%sSql):\n\n\n" \
                                     "if __name__ == '__main__':\n    s = %sAssert()\n\n" % (
-                self.name2, self.name2, self.name2)
+                                        self.name2, self.name2, self.name2)
         self.assert_fun_list = re.findall("    def +(.*)?\(", self.assert_file_str)
 
         self.api_fun_file_path = os.path.join(self.service_dir, self.name + "_api_fun.py")
         if os.path.exists(self.api_fun_file_path):
-            self.api_fun_file_str = self.read_file(self.api_fun_file_path)
+            self.api_fun_file_str = FunBase.read_file(self.api_fun_file_path)
         else:
             self.api_fun_file_str = "from service.%s.%s_assert import %sAssert\n" % (self.name, self.name, self.name2)
             self.api_fun_file_str += "from service.%s import %s_api\n\nimport allure\n" % (self.name, self.name)
             self.api_fun_file_str += "\n\nclass %sApiFun(%sAssert):\n\n" \
-                                    "if __name__ == '__main__':\n    s = %sApiFun()\n\n" % (
-                                        self.name2, self.name2, self.name2)
+                                     "if __name__ == '__main__':\n    s = %sApiFun()\n\n" % (
+                                         self.name2, self.name2, self.name2)
         self.api_fun_fun_list = re.findall("    def +(.*)?\(", self.api_fun_file_str)
 
         self.api_testcase_file_path = os.path.join(self.testcase_dir, "test_api.py")
         if os.path.exists(self.api_testcase_file_path):
-            self.api_testcase_file_str = self.read_file(self.api_testcase_file_path)
+            self.api_testcase_file_str = FunBase.read_file(self.api_testcase_file_path)
         else:
             self.api_testcase_file_str = "import pytest\nimport allure\n\n" \
                                          "from service.%s.%s_api_fun import %sApiFun\n\n\n" % (
-                self.name, self.name, self.name2)
+                                             self.name, self.name, self.name2)
             self.api_testcase_file_str += '@allure.epic("针对单api的测试")\n@allure.feature("场景：")\nclass TestApi:\n' \
                                           '    def setup(self):\n        self.f = %sApiFun()\n\n' % self.name2
         self.api_testcase_list = re.findall("    def +test_(.*)?\(", self.api_testcase_file_str)
 
     def set_file_path(self):
         """创建项目目录"""
         if not self.name:
             self.name = os.path.basename(sys.argv[0])
-        for path in [service_path, os.path.join(service_path, self.name), 
-                     testcase_path, os.path.join(testcase_path,self.name)]:
-            if not os.path.exists(path):
-                os.makedirs(path)
-
         self.service_dir = os.path.join(service_path, self.name)
-        if not os.path.exists(os.path.join(self.service_dir, "__init__.py")):
-            self.write_file(os.path.join(self.service_dir, "__init__.py"), value=self.get_init_value())
         self.testcase_dir = os.path.join(testcase_path, self.name)
-
-    def get_init_value(self):
-        """生成项目__init__.py文件"""
-        value = 'from commen.init_project import GetApi\n' \
-                'from commen.unit_request import UnitRequest\n\n\n' \
-                'class Request(UnitRequest):\n    pass\n\n\n' \
-                'unit_request = UnitRequest("SIT", "%s")\n' \
-                '# 环境变量\nvariable = unit_request.variable\n' \
-                'http_requester = unit_request.http_requester\n\n\n' \
-                'if __name__ == "__main__":\n' % (self.app_key)
-        if self.app_key:
-            value += "    GetApi(app_key=APP_KEY)\n"
-        else:
-            value += "    GetApi("
-            value += "api_type=%s, " % self.api_type if self.api_type else ""
-            value += "value='%s', " % self.value if self.value else ""
-            value += "name='%s', " % self.name if self.name else ""
-            value += "yapi_url='%s', " % self.yapi_url if self.yapi_url else ""
-            value = value[:-2] + ")"
-        return value
-
-    @staticmethod
-    def write_file(file_path, value=""):
-        """写文件"""
-        with open(file_path, 'w', encoding='utf-8') as f:
-            f.write(value)
-
-    @staticmethod
-    def read_file(file_path):
-        """读文件"""
-        with open(file_path, 'r', encoding='utf-8') as f:
-            value = f.read()
-        return value
+        FunBase.mkdir_file([self.service_dir, self.testcase_dir], is_py=False)
+        if not os.path.exists(os.path.join(self.service_dir, "__init__.py")):
+            FunBase.write_file(os.path.join(self.service_dir, "__init__.py"), value=self.get_init_value())
 
     def get_api_list(self):
         """根据api文档不同方式生成api文件"""
         if self.api_type == 1:
             self.get_list_menu()
         elif self.api_type == 2:
             self.get_list_json()
         elif self.api_type == 0:
             self.get_list_menu_swagger()
 
     def get_list_json(self):
         if self.value:
             file_path = os.path.join(self.dir, 'file', self.value)
             if os.path.exists(file_path):
-                value = self.read_file(file_path)
+                value = FunBase.read_file(file_path)
                 value = json.loads(value)
                 self.api_list = []
                 for v in value:
                     self.api_list.extend(v.get('list'))
             else:
                 assert not "Yapi的json文件在file中不存在"
         elif self.app_key:
@@ -239,15 +176,15 @@
             try:
                 data = requests.get(self.value)
                 data = data.json()
                 self.api_list = []
                 for k, v in data.get("paths", {}).items():
                     api = {}
                     api["path"] = data.get("basePath", "") + k
-                    
+
                     for k2, v2 in v.items():
                         api["method"] = k2
                         api["title"] = v2.get('summary', "")
                         api["up_time"] = int(time.time())
                         api["req_headers"] = []
                         if v2.get('consumes'):
                             api["req_headers"].append(
@@ -266,20 +203,20 @@
                                         tmp = parameter.get("schema").get("$ref").split("/")
                                         if len(tmp) > 2:
                                             tmp2 = data.get(tmp[1], {}).get(tmp[2], {})
                                             for k3, v3 in tmp2.get('properties', {}).items():
                                                 api["res_body"].append({'name': k3, 'desc': v3.get('description', "")})
                                     else:
                                         api["res_body"].append({'name': parameter.get("name"),
-                                                                 'desc': parameter.get('description')})
+                                                                'desc': parameter.get('description')})
                             elif parameter.get('in') in ("params", "path"):
                                 api["req_params"].append({'name': parameter.get("name"),
-                                                         'desc': parameter.get('description')})
+                                                          'desc': parameter.get('description')})
                             elif parameter.get('in') == "query":
-                                if parameter.get('name') not in  ("params", ):
+                                if parameter.get('name') not in ("params",):
                                     api["req_query"].append({'name': parameter.get("name"),
                                                              'desc': parameter.get('description')})
                             else:
                                 print()
                         self.api_list.append(api)
             except:
                 assert False, "swagger路径错误"
@@ -328,15 +265,15 @@
         _list4 = ["Content-Type"]
         for i in _list:
             name = i.get("name").split("[")[0]
             if name not in _list4:
                 _list4.append(name)
                 i["name"] = name
                 _list3.append(i)
-        
+
         return _list3
 
     def get_description(self, req_body_other):
         try:
             if not req_body_other:
                 return []
             elif isinstance(req_body_other, str):
@@ -364,22 +301,24 @@
                 _list.append(_row)
         except Exception as e:
             print(e)
         return _list
 
     def get_params_string(self, req_all, res_body):
         """方法描述生成"""
+
         def get_str(l):
             _str = ""
             for p in l:
                 _str += f'    params: {p.get("name", "")} : {p.get("type", "")} : {p.get("desc", "")}\n'
                 if p.get('properties') or p.get('items'):
                     for p2 in p.get('properties') or p.get('items'):
                         _str += f'              {p2.get("name", "")} : {p2.get("type", "")} : {p2.get("desc", "")}\n'
             return _str
+
         try:
             api_str = get_str(req_all)
             api_str += "    params: headers : 请求头\n    ====================返回======================\n"
             api_str += get_str(res_body)
             return api_str
         except Exception as e:
             print(e)
@@ -406,17 +345,16 @@
             api_str += f'    _url = get_url(_url, locals())\n'
         api_str += '\n    _headers = ' + self.get_req_json(req_headers, True)
         api_str += '\n    _headers.update({"headers": headers})\n\n'
         api_str += '    _data = ' + self.get_req_json(req_all_data)
         api_str += '\n\n    _params = ' + self.get_req_json(req_params)
         api_str += '\n\n    return http_requester(_method, _url, params=_params, data=_data, ' \
                    'headers=_headers, **kwargs)\n\n\n'
-    
+
         return api_str
-            
 
     @staticmethod
     def get_fun_name(name):
         name = name.strip()
         if name.startswith('/'):
             name = name[1:]
         if "/{" in name:
@@ -462,20 +400,20 @@
                 self.sql_fun_list.append("sql_" + fun_name)
                 self.get_sql_fun_str(fun_name)
         for fun_name in self.api_fun_fun_list:
             if fun_name not in self.api_testcase_list:
                 self.api_testcase_list.append("test_" + fun_name)
                 self.get_api_testcase_str(fun_name)
 
-        self.write_file(self.api_file_path, self.api_file_str)
-        self.write_file(self.fun_file_path, self.fun_file_str)
-        self.write_file(self.sql_file_path, self.sql_file_str)
-        self.write_file(self.assert_file_path, self.assert_file_str)
-        self.write_file(self.api_fun_file_path, self.api_fun_file_str)
-        self.write_file(self.api_testcase_file_path, self.api_testcase_file_str)
+        FunBase.write_file(self.api_file_path, self.api_file_str)
+        FunBase.write_file(self.fun_file_path, self.fun_file_str)
+        FunBase.write_file(self.sql_file_path, self.sql_file_str)
+        FunBase.write_file(self.assert_file_path, self.assert_file_str)
+        FunBase.write_file(self.api_fun_file_path, self.api_fun_file_str)
+        FunBase.write_file(self.api_testcase_file_path, self.api_testcase_file_str)
 
     def get_sql_fun_str(self, api_fun_name):
         sql_fun_str = "    def sql_%s(self, **kwargs):\n" % api_fun_name
         sql_fun_str += "        # name = self.kwargs_pop(kwargs, 'name')  # 单独处理字段\n" \
                        "        # self.kwargs_replace(kwargs, likes=[], ins=[], before_end=[])  # 模糊查询字段，数组包含查询字段，区间字段处理\n" \
                        '        # kwargs["order_by"] = None  # 排序\n' \
                        '        sql_str = self.get_sql_str("table", **kwargs)  # 生成sql语句\n' \
@@ -537,15 +475,15 @@
 
         if api_fun_name.lower()[-4:] in ('page', 'list', 'ages'):
             for n in data_list:
                 api_fun_fun_str += "        self._list_%s = self.get_res_value_list('%s')\n" % (n, n)
                 if "_list_%s" % n not in self.fun_init_list:
                     self.fun_init_list.append("_list_%s" % n)
                     self.fun_file_str = self.fun_file_str.replace(self.fun_init_str,
-                                                              self.fun_init_str + "        self._list_%s = []\n" % n)
+                                                                  self.fun_init_str + "        self._list_%s = []\n" % n)
         for n in data_list:
             api_fun_fun_str += "        self._v_%s = %s\n" % (n, n)
             if "_v_%s" % n not in self.fun_init_list:
                 self.fun_init_list.append("_v_%s" % n)
                 self.fun_file_str = self.fun_file_str.replace(self.fun_init_str,
                                                               self.fun_init_str + "        self._v_%s = None\n" % n)
         api_fun_fun_str += '\n' if data_list else ''
```

### Comparing `huhangkai-1.2.2/commen/unit_dict.py` & `huhangkai-1.2.3/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.2/commen/unit_encryption.py` & `huhangkai-1.2.3/commen/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.2/commen/unit_fun.py` & `huhangkai-1.2.3/commen/unit_fun.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import re
 import random
 import time
 import requests
 import datetime
 # import pymysql
 
@@ -74,28 +75,26 @@
             code += random.choice(char3)
             return code
             test = re.match('^.\w.[A-Z]\d{4}$|^.\w.\d[A-Z]\d{3}$|^.\w.\d{2}[A-Z]\d{2}$|^.\w.\d{3}[A-Z]\d$|^.\w.\d{5}$',
                             code)
             if test:
                 return code
 
-    # # mock方法，国家locale_list随机，也可根据数字获取第几个国家，超出时随机
-    # def faker_random_country(self, locale=None):
-    #     country = None
-    #     if locale:
-    #         try:
-    #             if self.locale_list.get(locale):
-    #                 country = locale
-    #             else:
-    #                 country = list(self.locale_list.keys())[int(locale)]
-    #         except:
-    #             pass
-    #     if not country:
-    #         country = random.choice(list(self.locale_list.keys()))
-    #     return self.faker(locale=country)
+    @staticmethod
+    def write_file(file_path, value=""):
+        """写文件"""
+        with open(file_path, 'w', encoding='utf-8') as f:
+            f.write(value)
+
+    @staticmethod
+    def read_file(file_path):
+        """读文件"""
+        with open(file_path, 'r', encoding='utf-8') as f:
+            value = f.read()
+        return value
 
     @staticmethod
     def log_info(msg):
         logger.info(str(msg))
 
     def sleep(self, t=1, debug=False):
         self.log_info("sleep %s 秒" % t)
@@ -119,14 +118,27 @@
     def time_ms(self, string=None, fmt="%Y-%m-%d"):
         time_array = self.time(string=string, fmt=fmt)
         return time_array * 1000
 
     def data_str(self):
         return datetime.datetime.now().strftime("%Y-%m-%d")
 
+    @staticmethod
+    def mkdir_file(path, is_py=True):
+        if isinstance(path, (list, tuple)):
+            for i in path:
+                FunBase.mkdir_file(path=i, is_py=is_py)
+        else:
+            if not os.path.lexists(path):
+                if not os.path.lexists(os.path.dirname(path)):
+                    FunBase.mkdir_file(path=os.path.dirname(path), is_py=is_py)
+                os.makedirs(path)
+                if is_py:
+                    FunBase.write_file(os.path.join(path, "__init__.py"))
+
     # # 根据sql语句执行sql
     # def run_mysql(self, sql_str="", host="", user="", password="", database=""):
     #     sql_str = sql_str or self.sql_str
     #     if self._db.get(host+database):
     #         cursor = self._db.get(host+database)
     #     else:
     #         try:
```

### Comparing `huhangkai-1.2.2/commen/unit_logger.py` & `huhangkai-1.2.3/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.2/commen/unit_request.py` & `huhangkai-1.2.3/commen/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.2/commen/unit_tasks.py` & `huhangkai-1.2.3/commen/unit_tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         day_of_week = '*' if cron_list[5] in ('?', '？') else cron_list[5]
         year = cron_list[6]
         return second, minute, hour, day, month, day_of_week, year
 
     def add_jobs(self, fun, schedules=None, cron=None):
         if cron:
             second, minute, hour, day, month, day_of_week, year = self.get_cron(cron)
-            if schedules:
+            if schedules is not None:
                 Scheduler.scheduler.add_job(fun, 'cron', year=year, day_of_week=day_of_week, month=month, day=day,
                                             hour=hour, minute=minute, second=second, args=(schedules,))
             else:
                 Scheduler.scheduler.add_job(fun, 'cron', year=year, day_of_week=day_of_week, month=month, day=day,
                                             hour=hour, minute=minute, second=second)
             return True
         elif schedules:
```

### Comparing `huhangkai-1.2.2/setup.py` & `huhangkai-1.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='huhangkai',  # 对外模块的名字
-    version='1.2.2',  # 版本号
+    version='1.2.3',  # 版本号
     description='接口自动化',  # 描述
     author='胡杭凯',  # 作者
     author_email='3173825608@qq.com',
     # package_dir={"": "commen"},
     packages=find_packages(),
     package_data={'by': ['常用命令.bat'],},
     python_requires=">=3.0",
@@ -15,9 +15,11 @@
         "openpyxl",
         "apscheduler",
         "rsa",
         "pyDes",
         "pycryptodome",
         "xlsxwriter",
         "pandas",
+        "apache-beam",
+        "pytest",
     ],
 )
```

