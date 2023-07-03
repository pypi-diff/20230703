# Comparing `tmp/dynamic-links-0.0.3.tar.gz` & `tmp/dynamic-links-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-links-0.0.3.tar", last modified: Wed Jun 28 06:19:17 2023, max compression
+gzip compressed data, was "dynamic-links-0.0.4.tar", last modified: Mon Jul  3 09:46:18 2023, max compression
```

## Comparing `dynamic-links-0.0.3.tar` & `dynamic-links-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-06-28 06:19:17.729780 dynamic-links-0.0.3/
--rw-r--r--   0 pic        (501) staff       (20)     5342 2023-06-28 06:19:17.729632 dynamic-links-0.0.3/PKG-INFO
--rw-r--r--   0 pic        (501) staff       (20)     5069 2023-06-28 06:18:33.000000 dynamic-links-0.0.3/README.md
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-06-28 06:19:17.728721 dynamic-links-0.0.3/dlframe/
--rw-r--r--   0 pic        (501) staff       (20)     2630 2023-06-27 04:59:53.000000 dynamic-links-0.0.3/dlframe/CalculationNode.py
--rw-r--r--   0 pic        (501) staff       (20)     1924 2023-06-27 03:29:25.000000 dynamic-links-0.0.3/dlframe/CalculationNodeManager.py
--rw-r--r--   0 pic        (501) staff       (20)     2048 2023-06-27 04:00:46.000000 dynamic-links-0.0.3/dlframe/ExecutionNode.py
--rw-r--r--   0 pic        (501) staff       (20)      939 2023-06-27 05:19:42.000000 dynamic-links-0.0.3/dlframe/Logger.py
--rw-r--r--   0 pic        (501) staff       (20)     5170 2023-06-27 05:20:48.000000 dynamic-links-0.0.3/dlframe/WebManager.py
--rw-r--r--   0 pic        (501) staff       (20)      141 2023-06-26 17:09:16.000000 dynamic-links-0.0.3/dlframe/__init__.py
-drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-06-28 06:19:17.729429 dynamic-links-0.0.3/dynamic_links.egg-info/
--rw-r--r--   0 pic        (501) staff       (20)     5342 2023-06-28 06:19:17.000000 dynamic-links-0.0.3/dynamic_links.egg-info/PKG-INFO
--rw-r--r--   0 pic        (501) staff       (20)      348 2023-06-28 06:19:17.000000 dynamic-links-0.0.3/dynamic_links.egg-info/SOURCES.txt
--rw-r--r--   0 pic        (501) staff       (20)        1 2023-06-28 06:19:17.000000 dynamic-links-0.0.3/dynamic_links.egg-info/dependency_links.txt
--rw-r--r--   0 pic        (501) staff       (20)       30 2023-06-28 06:19:17.000000 dynamic-links-0.0.3/dynamic_links.egg-info/requires.txt
--rw-r--r--   0 pic        (501) staff       (20)        8 2023-06-28 06:19:17.000000 dynamic-links-0.0.3/dynamic_links.egg-info/top_level.txt
--rw-r--r--   0 pic        (501) staff       (20)       38 2023-06-28 06:19:17.729823 dynamic-links-0.0.3/setup.cfg
--rw-r--r--   0 pic        (501) staff       (20)      682 2023-06-28 06:18:12.000000 dynamic-links-0.0.3/setup.py
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-03 09:46:18.585344 dynamic-links-0.0.4/
+-rw-r--r--   0 pic        (501) staff       (20)     5443 2023-07-03 09:46:18.585104 dynamic-links-0.0.4/PKG-INFO
+-rw-r--r--   0 pic        (501) staff       (20)     5170 2023-07-03 09:44:30.000000 dynamic-links-0.0.4/README.md
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-03 09:46:18.583977 dynamic-links-0.0.4/dlframe/
+-rw-r--r--   0 pic        (501) staff       (20)     2630 2023-06-27 04:59:53.000000 dynamic-links-0.0.4/dlframe/CalculationNode.py
+-rw-r--r--   0 pic        (501) staff       (20)     1924 2023-06-27 03:29:25.000000 dynamic-links-0.0.4/dlframe/CalculationNodeManager.py
+-rw-r--r--   0 pic        (501) staff       (20)     2048 2023-06-27 04:00:46.000000 dynamic-links-0.0.4/dlframe/ExecutionNode.py
+-rw-r--r--   0 pic        (501) staff       (20)      939 2023-06-27 05:19:42.000000 dynamic-links-0.0.4/dlframe/Logger.py
+-rw-r--r--   0 pic        (501) staff       (20)     5174 2023-07-03 09:42:34.000000 dynamic-links-0.0.4/dlframe/WebManager.py
+-rw-r--r--   0 pic        (501) staff       (20)      141 2023-06-26 17:09:16.000000 dynamic-links-0.0.4/dlframe/__init__.py
+drwxr-xr-x   0 pic        (501) staff       (20)        0 2023-07-03 09:46:18.584667 dynamic-links-0.0.4/dynamic_links.egg-info/
+-rw-r--r--   0 pic        (501) staff       (20)     5443 2023-07-03 09:46:18.000000 dynamic-links-0.0.4/dynamic_links.egg-info/PKG-INFO
+-rw-r--r--   0 pic        (501) staff       (20)      348 2023-07-03 09:46:18.000000 dynamic-links-0.0.4/dynamic_links.egg-info/SOURCES.txt
+-rw-r--r--   0 pic        (501) staff       (20)        1 2023-07-03 09:46:18.000000 dynamic-links-0.0.4/dynamic_links.egg-info/dependency_links.txt
+-rw-r--r--   0 pic        (501) staff       (20)       30 2023-07-03 09:46:18.000000 dynamic-links-0.0.4/dynamic_links.egg-info/requires.txt
+-rw-r--r--   0 pic        (501) staff       (20)        8 2023-07-03 09:46:18.000000 dynamic-links-0.0.4/dynamic_links.egg-info/top_level.txt
+-rw-r--r--   0 pic        (501) staff       (20)       38 2023-07-03 09:46:18.585407 dynamic-links-0.0.4/setup.cfg
+-rw-r--r--   0 pic        (501) staff       (20)      682 2023-07-03 09:44:51.000000 dynamic-links-0.0.4/setup.py
```

### Comparing `dynamic-links-0.0.3/PKG-INFO` & `dynamic-links-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-links
-Version: 0.0.3
+Version: 0.0.4
 Summary: a calculation framework
 Home-page: https://github.com/picpic2013/dlframe-back
 Author: PIC
 Author-email: picpic2019@gmail.com
 License: MIT
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
@@ -179,14 +179,19 @@
 
 变量和方法可以混用。例如：
 
 ~~~python
 result1 > clsss.f2()
 ~~~
 
---- 
+### 指定运行 ip 与端口号
 
-### 前端
+~~~python
+with WebManager(host='0.0.0.0', port=8765):
+    pass
+~~~
+
+## 关于前端
 
 本框架仅提供 WebSocket 服务，不提供页面显示。需配合[前端](https://picpic2013.github.io/dlframe-front/)使用。前端代码开源在[仓库](https://github.com/picpic2013/dlframe-front.git)。
 
 注意！由于底层使用 `ws`，对于某些浏览器，可能无法通过安全检查，从而导致前后端无法连接。请禁用相关安全策略后重试。
```

### Comparing `dynamic-links-0.0.3/README.md` & `dynamic-links-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,19 @@
 
 变量和方法可以混用。例如：
 
 ~~~python
 result1 > clsss.f2()
 ~~~
 
---- 
+### 指定运行 ip 与端口号
 
-### 前端
+~~~python
+with WebManager(host='0.0.0.0', port=8765):
+    pass
+~~~
+
+## 关于前端
 
 本框架仅提供 WebSocket 服务，不提供页面显示。需配合[前端](https://picpic2013.github.io/dlframe-front/)使用。前端代码开源在[仓库](https://github.com/picpic2013/dlframe-front.git)。
 
 注意！由于底层使用 `ws`，对于某些浏览器，可能无法通过安全检查，从而导致前后端无法连接。请禁用相关安全策略后重试。
```

### Comparing `dynamic-links-0.0.3/dlframe/CalculationNode.py` & `dynamic-links-0.0.4/dlframe/CalculationNode.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.3/dlframe/CalculationNodeManager.py` & `dynamic-links-0.0.4/dlframe/CalculationNodeManager.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.3/dlframe/ExecutionNode.py` & `dynamic-links-0.0.4/dlframe/ExecutionNode.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.3/dlframe/Logger.py` & `dynamic-links-0.0.4/dlframe/Logger.py`

 * *Files identical despite different names*

### Comparing `dynamic-links-0.0.3/dlframe/WebManager.py` & `dynamic-links-0.0.4/dlframe/WebManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,12 +124,12 @@
                     else:
                         response = json.dumps({
                             'status': 500, 
                             'data': 'unknown type'
                         })
                         await socket.send(response)
 
-        print('Backend server is running at [{}:{}]...'.format(host, port))
-        print('To visit front end page: https://picpic2013.github.io/dlframe-front/')
+        print('The backend server is running on [{}:{}]...'.format(host, port))
+        print('The frontend page is at: https://picpic2013.github.io/dlframe-front/')
 
         event_loop.run_until_complete(websockets.serve(onRecv, host, port))
         event_loop.run_forever()
```

### Comparing `dynamic-links-0.0.3/dynamic_links.egg-info/PKG-INFO` & `dynamic-links-0.0.4/dynamic_links.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-links
-Version: 0.0.3
+Version: 0.0.4
 Summary: a calculation framework
 Home-page: https://github.com/picpic2013/dlframe-back
 Author: PIC
 Author-email: picpic2019@gmail.com
 License: MIT
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
@@ -179,14 +179,19 @@
 
 变量和方法可以混用。例如：
 
 ~~~python
 result1 > clsss.f2()
 ~~~
 
---- 
+### 指定运行 ip 与端口号
 
-### 前端
+~~~python
+with WebManager(host='0.0.0.0', port=8765):
+    pass
+~~~
+
+## 关于前端
 
 本框架仅提供 WebSocket 服务，不提供页面显示。需配合[前端](https://picpic2013.github.io/dlframe-front/)使用。前端代码开源在[仓库](https://github.com/picpic2013/dlframe-front.git)。
 
 注意！由于底层使用 `ws`，对于某些浏览器，可能无法通过安全检查，从而导致前后端无法连接。请禁用相关安全策略后重试。
```

### Comparing `dynamic-links-0.0.3/setup.py` & `dynamic-links-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 with open(os.path.join(here, 'README.md'), 'r',encoding='UTF-8') as mdFile:
     long_description = mdFile.read()
 
 setup(
     name='dynamic-links', 
-    version='0.0.3', 
+    version='0.0.4', 
     packages=['dlframe'], 
     url='https://github.com/picpic2013/dlframe-back', 
     license='MIT', 
     author='PIC', 
     author_email='picpic2019@gmail.com', 
     description='a calculation framework', 
     long_description=long_description,
```

