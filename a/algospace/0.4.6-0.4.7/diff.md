# Comparing `tmp/algospace-0.4.6.tar.gz` & `tmp/algospace-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algospace-0.4.6.tar", last modified: Fri May 12 09:46:12 2023, max compression
+gzip compressed data, was "algospace-0.4.7.tar", last modified: Mon Jul  3 18:20:22 2023, max compression
```

## Comparing `algospace-0.4.6.tar` & `algospace-0.4.7.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.420284 algospace-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-12 09:46:03.000000 algospace-0.4.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-12 09:46:03.000000 algospace-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-12 09:46:12.420284 algospace-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-12 09:46:03.000000 algospace-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.412284 algospace-0.4.6/algospace/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.416284 algospace-0.4.6/algospace/customer/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/customer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/customer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/customer/fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/customer/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.416284 algospace-0.4.6/algospace/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.416284 algospace-0.4.6/algospace/provider/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/docker_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/enroll.py
--rw-r--r--   0 runner    (1001) docker     (123)    41308 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/stdio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.416284 algospace-0.4.6/algospace/provider/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/templates/algospace-config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.420284 algospace-0.4.6/algospace/provider/templates/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/templates/docker/algospace-docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/templates/docker/algospace-docker-logs.sh
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/templates/docker/algospace-docker-start.sh
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/templates/docker/algospace-docker-stop.sh
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/templates/docker/algospace-dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/util.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.412284 algospace-0.4.6/algospace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-12 09:46:12.000000 algospace-0.4.6/algospace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-12 09:46:12.000000 algospace-0.4.6/algospace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:46:12.000000 algospace-0.4.6/algospace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-12 09:46:12.000000 algospace-0.4.6/algospace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-12 09:46:12.000000 algospace-0.4.6/algospace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 09:46:12.000000 algospace-0.4.6/algospace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:46:12.420284 algospace-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-12 09:46:03.000000 algospace-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.813934 algospace-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-03 18:20:13.000000 algospace-0.4.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-03 18:20:13.000000 algospace-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-03 18:20:22.813934 algospace-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-03 18:20:13.000000 algospace-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.809934 algospace-0.4.7/algospace/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.809934 algospace-0.4.7/algospace/customer/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/customer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/customer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/customer/fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/customer/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.809934 algospace-0.4.7/algospace/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.809934 algospace-0.4.7/algospace/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/docker_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/enroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/param_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41688 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/stdio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.813934 algospace-0.4.7/algospace/provider/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/templates/algospace-config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.813934 algospace-0.4.7/algospace/provider/templates/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/templates/docker/algospace-docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/templates/docker/algospace-docker-logs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/templates/docker/algospace-docker-start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/templates/docker/algospace-docker-stop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/provider/templates/docker/algospace-dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 18:20:13.000000 algospace-0.4.7/algospace/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:20:22.809934 algospace-0.4.7/algospace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-03 18:20:22.000000 algospace-0.4.7/algospace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-03 18:20:22.000000 algospace-0.4.7/algospace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:20:22.000000 algospace-0.4.7/algospace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-03 18:20:22.000000 algospace-0.4.7/algospace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-03 18:20:22.000000 algospace-0.4.7/algospace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 18:20:22.000000 algospace-0.4.7/algospace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 18:20:22.813934 algospace-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-03 18:20:13.000000 algospace-0.4.7/setup.py
```

### Comparing `algospace-0.4.6/PKG-INFO` & `algospace-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algospace
-Version: 0.4.6
+Version: 0.4.7
 Summary: AlgoSpace: A platform for displaying and using algorithm achievements
 Home-page: https://github.com/Algo-Space/algospace-pypi
 Author: DBIIR
 Author-email: ckeming@outlook.com
 Maintainer: DBIIR
 Maintainer-email: ckeming@outlook.com
 License: BSD License
```

### Comparing `algospace-0.4.6/README.md` & `algospace-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `algospace-0.4.6/algospace/__init__.py` & `algospace-0.4.7/algospace/__init__.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.6/algospace/__main__.py` & `algospace-0.4.7/algospace/__main__.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.6/algospace/customer/fn.py` & `algospace-0.4.7/algospace/customer/fn.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.6/algospace/customer/service.py` & `algospace-0.4.7/algospace/customer/service.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.6/algospace/exceptions/__init__.py` & `algospace-0.4.7/algospace/exceptions/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 '''
 @Description: 异常
 @Author: Kermit
 @Date: 2022-10-06 12:30:47
 @LastEditors: Kermit
-@LastEditTime: 2022-11-11 18:50:46
+@LastEditTime: 2023-05-22 17:17:56
 '''
 
 class ConfigError(Exception):
     def __init__(self, err_msg):
         Exception.__init__(self, err_msg)
 
 class FileExtNotValid(Exception):
@@ -30,8 +30,13 @@
 class LoginError(Exception):
     def __init__(self, err_msg):
         Exception.__init__(self, err_msg)
 
 
 class InvalidAlgorithmVersion(Exception):
     def __init__(self, err_msg):
+        Exception.__init__(self, err_msg)
+
+
+class InvalidCallParamException(Exception):
+    def __init__(self, err_msg):
         Exception.__init__(self, err_msg)
```

### Comparing `algospace-0.4.6/algospace/logger.py` & `algospace-0.4.7/algospace/logger.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.6/algospace/login.py` & `algospace-0.4.7/algospace/login.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.6/algospace/provider/cloud.py` & `algospace-0.4.7/algospace/provider/cloud.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.6/algospace/provider/config_generator.py` & `algospace-0.4.7/algospace/provider/config_generator.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.6/algospace/provider/config_loader.py` & `algospace-0.4.7/algospace/provider/config_loader.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.6/algospace/provider/docker_generator.py` & `algospace-0.4.7/algospace/provider/docker_generator.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.6/algospace/provider/enroll.py` & `algospace-0.4.7/algospace/provider/enroll.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.6/algospace/provider/service.py` & `algospace-0.4.7/algospace/provider/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 '''
 @Description: 算法提供者核心服务
 @Author: Kermit
 @Date: 2022-11-05 16:46:46
-@LastEditors: Kermit
-@LastEditTime: 2023-05-12 17:10:35
 '''
 
 from typing import Any, Callable, Optional, List, Tuple, Union
 from algospace.logger import Logger, algospace_logger
 from algospace.util import create_timestamp_filename
 from . import config
 from .config import Algoinfo
@@ -23,43 +21,49 @@
 import concurrent.futures
 import socket
 import traceback
 import requests
 import websocket
 from algospace.login import login, login_instance
 from .config_loader import ConfigLoader, InputType, OutputType, valid_input_type, valid_output_type
+from .param_validator import ParamValidator
 from .enroll import enroll, verify_config, is_component_normal
 from .stdio import GradioPrint, QueueStdIO, QueueStdIOExec
+from algospace.exceptions import InvalidCallParamException
 import json
 import time
 import datetime
 import os
 import re
 import base64
 
 
 class FnService:
     ''' 模型函数 Service '''
 
     def __init__(self, algorithm_config: ConfigLoader) -> None:
         self.algorithm_config = algorithm_config
+        self.param_validator = ParamValidator(algorithm_config)
         self.logger = Logger('Fn Service', is_show_time=True)
 
     async def handle(self, *args, **kwargs):
         ''' 处理函数请求 '''
         future = asyncio.get_event_loop().run_in_executor(None, lambda: self.algorithm_config.fn(*args, **kwargs))
         out = await asyncio.wait_for(future, timeout=self.algorithm_config.service_timeout)
         return out
 
     def launch_thread(self, fn_index: int, fn_req_queue: multiprocessing.Queue, fn_res_queue: multiprocessing.Queue) -> None:
         ''' 启动函数服务线程 '''
         while True:
             try:
                 args, kwargs = fn_req_queue.get()
                 self.logger.info(f'[{fn_index}] Begin to calculate.')
+                param_result, param_err_msg = self.param_validator.validate(*args, **kwargs)
+                if not param_result:
+                    raise InvalidCallParamException(param_err_msg)
                 out = asyncio.run(self.handle(*args, **kwargs))
                 self.logger.info(f'[{fn_index}] Complete.')
                 fn_res_queue.put((out, None))
             except Exception as e:
                 fn_res_queue.put((None, e))
 
     def launch(self,
@@ -837,14 +841,16 @@
         fn_process = create_fn_process()
         service_process = create_service_process()
         gradio_process = create_gradio_process()
         process_exit_code = None
 
         self.algo_logger.info(f'Waiting for service launched...')
 
+        after_cancel_tasks = []
+
         async def join_task(process: multiprocessing.Process):
             nonlocal process_exit_code
             try:
                 await asyncio.get_event_loop().run_in_executor(None, process.join)
                 process_exit_code = process.exitcode
             except:
                 if process.is_alive():
@@ -869,39 +875,40 @@
                     traceback.print_exc()
                     self.algo_logger.error(f'Heartbeat error: {str(e)}')
 
         async def subprocess_stdio_task():
             queue_stdio_exec = QueueStdIOExec(stdio_queue)
             stdio_exec = queue_stdio_exec.exec
             stdio_exec_all = queue_stdio_exec.exec_all
+            after_cancel_tasks.append(stdio_exec_all)
             is_execed = True
             while True:
                 try:
                     if not is_execed:
                         await asyncio.sleep(0.1)
                     is_execed = await asyncio.get_event_loop().run_in_executor(None, stdio_exec)
                 except concurrent.futures._base.CancelledError:
-                    stdio_exec_all()
                     break
                 except asyncio.CancelledError:
-                    stdio_exec_all()
                     break
                 except Exception as e:
                     traceback.print_exc()
                     self.algo_logger.error(f'Handle subprocess stdio error: {str(e)}')
 
         # 当有任务抛出异常时，停止所有任务
         tasks = [join_task(fn_process),
                  join_task(service_process),
                  join_task(gradio_process),
                  heartbeat_task(),
                  subprocess_stdio_task()]
         done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
         for task in pending:
             task.cancel()
+        for task in after_cancel_tasks:
+            task()
         for task in done:
             task.result()
         return process_exit_code
 
 
 def run_service(config_path: str, fetch_mode: str = 'listen') -> None:
     loop = asyncio.get_event_loop()
```

### Comparing `algospace-0.4.6/algospace/provider/stdio.py` & `algospace-0.4.7/algospace/provider/stdio.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.6/algospace/provider/templates/algospace-config.py` & `algospace-0.4.7/algospace/provider/templates/algospace-config.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.6/algospace.egg-info/PKG-INFO` & `algospace-0.4.7/algospace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algospace
-Version: 0.4.6
+Version: 0.4.7
 Summary: AlgoSpace: A platform for displaying and using algorithm achievements
 Home-page: https://github.com/Algo-Space/algospace-pypi
 Author: DBIIR
 Author-email: ckeming@outlook.com
 Maintainer: DBIIR
 Maintainer-email: ckeming@outlook.com
 License: BSD License
```

### Comparing `algospace-0.4.6/algospace.egg-info/SOURCES.txt` & `algospace-0.4.7/algospace.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 algospace/provider/__init__.py
 algospace/provider/cloud.py
 algospace/provider/config.py
 algospace/provider/config_generator.py
 algospace/provider/config_loader.py
 algospace/provider/docker_generator.py
 algospace/provider/enroll.py
+algospace/provider/param_validator.py
 algospace/provider/service.py
 algospace/provider/stdio.py
 algospace/provider/templates/algospace-config.py
 algospace/provider/templates/docker/algospace-docker-compose.yml
 algospace/provider/templates/docker/algospace-docker-logs.sh
 algospace/provider/templates/docker/algospace-docker-start.sh
 algospace/provider/templates/docker/algospace-docker-stop.sh
```

### Comparing `algospace-0.4.6/setup.py` & `algospace-0.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 '''
 @Description: Setuptools
 @Author: Kermit
 @Date: 2022-10-06 12:30:47
 @LastEditors: Kermit
-@LastEditTime: 2023-03-30 05:11:30
+@LastEditTime: 2023-07-04 01:54:08
 '''
 
 from setuptools import setup, find_packages
 from os import path
 
 name = 'algospace'
 with open(path.join(name, 'version.txt'), 'r', encoding='utf-8') as f:
@@ -36,15 +36,15 @@
         'Homepage': 'https://algospace.top',
     },
     install_requires=[
         'setuptools>=3.0',
         'requests',
         'requests-toolbelt>=0.9.1',
         'websocket-client',
-        'gradio>=3.0'
+        'gradio>=3.0, <4.0',
     ],
     python_requires='>=3.7',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
```

