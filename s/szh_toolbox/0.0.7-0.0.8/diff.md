# Comparing `tmp/szh_toolbox-0.0.7.tar.gz` & `tmp/szh_toolbox-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "szh_toolbox-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "szh_toolbox-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `szh_toolbox-0.0.7.tar` & `szh_toolbox-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1202 2023-06-30 05:00:52.117540 szh_toolbox-0.0.7/README.md
--rw-r--r--   0        0        0      691 2023-06-30 15:09:37.467679 szh_toolbox-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3509 2023-06-30 04:38:54.950176 szh_toolbox-0.0.7/src/szh_toolbox/__init__.py
--rw-r--r--   0        0        0      349 2023-06-29 02:31:19.795188 szh_toolbox-0.0.7/src/szh_toolbox/commond.py
--rw-r--r--   0        0        0     4563 2023-05-15 06:26:45.362456 szh_toolbox-0.0.7/src/szh_toolbox/namelist.py
--rw-r--r--   0        0        0     2793 2023-06-29 06:39:39.421182 szh_toolbox-0.0.7/src/szh_toolbox/namelistwps.py
--rw-r--r--   0        0        0     4028 2023-06-30 15:06:38.250074 szh_toolbox-0.0.7/src/szh_toolbox/noaa_download.py
--rw-r--r--   0        0        0       67 2023-06-28 07:18:07.747348 szh_toolbox-0.0.7/src/szh_toolbox/test.py
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 szh_toolbox-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1290 2023-07-01 06:49:22.545897 szh_toolbox-0.0.8/README.md
+-rw-r--r--   0        0        0      692 2023-07-03 05:38:45.662333 szh_toolbox-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4875 2023-07-01 06:45:47.550013 szh_toolbox-0.0.8/src/szh_toolbox/__init__.py
+-rw-r--r--   0        0        0      349 2023-06-29 02:31:19.795188 szh_toolbox-0.0.8/src/szh_toolbox/commond.py
+-rw-r--r--   0        0        0     2951 2023-07-02 06:38:49.985918 szh_toolbox-0.0.8/src/szh_toolbox/mylogger.py
+-rw-r--r--   0        0        0     4563 2023-05-15 06:26:45.362456 szh_toolbox-0.0.8/src/szh_toolbox/namelist.py
+-rw-r--r--   0        0        0     2793 2023-06-29 06:39:39.421182 szh_toolbox-0.0.8/src/szh_toolbox/namelistwps.py
+-rw-r--r--   0        0        0     4237 2023-07-03 05:29:43.330397 szh_toolbox-0.0.8/src/szh_toolbox/noaa_download.py
+-rw-r--r--   0        0        0       67 2023-06-28 07:18:07.747348 szh_toolbox-0.0.8/src/szh_toolbox/test.py
+-rw-r--r--   0        0        0     1753 1970-01-01 00:00:00.000000 szh_toolbox-0.0.8/PKG-INFO
```

### Comparing `szh_toolbox-0.0.7/README.md` & `szh_toolbox-0.0.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -29,10 +29,15 @@
 # 一行代码替换变量
 ShellScriptVariable.modify('data/myshell.sh', 'a', '这是A', 'data/myshell3.sh')
 ```
 # 命令行工具
 也就是可以直接在命令行里执行的代码
 ```bash
 # 直接打印namelist.wps文件定义的区域的范围
-stwps
-stwps namelist.wps
+st-wps
+st-wps namelist.wps
+```
+```bash
+# 下载noaa的数据比如ATMS L1
+st-noaa -h
+st-noaa orderId -o savepath
 ```
```

### Comparing `szh_toolbox-0.0.7/pyproject.toml` & `szh_toolbox-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["flit_core>=3.9"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "szh_toolbox"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="szh", email="suo.zh@qq.com"},
 ]
-description = "A small example package"
+description = "我自己的工具箱"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
 greetc = "szh_toolbox.commond:main"
 st-wps = "szh_toolbox.namelistwps:main"
-st-noaa = "szh_toolbox.noaa_download:main"
+st-noaa = "szh_toolbox.noaa_download:commond"
 
 [project.urls]
 "Homepage" = "https://github.com/pypa/sampleproject"
 "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `szh_toolbox-0.0.7/src/szh_toolbox/namelist.py` & `szh_toolbox-0.0.8/src/szh_toolbox/namelist.py`

 * *Files identical despite different names*

### Comparing `szh_toolbox-0.0.7/src/szh_toolbox/namelistwps.py` & `szh_toolbox-0.0.8/src/szh_toolbox/namelistwps.py`

 * *Files identical despite different names*

### Comparing `szh_toolbox-0.0.7/src/szh_toolbox/noaa_download.py` & `szh_toolbox-0.0.8/src/szh_toolbox/noaa_download.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,27 +78,20 @@
             t.join()
 
     def quit(self):
         for f in self.ftps:
             f.quit()
 
 
-def main():
-    parser = argparse.ArgumentParser(description='这是一个计算namelist.wps经纬度范围的程序')
-    parser.add_argument('order', type=str, help='订单编号')
-    parser.add_argument('--nftp', '-n', default=30,
-                        type=int, help='ftp最大数量，默认为%(default)s')
-    parser.add_argument('-o', dest='save_path', metavar='PATH',
-                        default='./', type=str, help='保存路径，默认为当前路径')
-    args = parser.parse_args()
-
-    order_id = args.order
-    num_ftp = args.nftp
-    save_path = args.save_path
-
+def main(order_id, num_ftp, save_path):
+    '''
+    order_id: 订单号
+    num_ftp: ftp最大数量
+    save_path: 保存路径
+    '''
     # 测试FTP可用性，以及获取对应订单的文件
     print(f'订单号为：{order_id}')
     print('-------------------')
     fi = LinkFTP('ftp测试用例')
     filepath = f'/{order_id}/001'  # 对面FTP服务上的文件夹路径
     filenames = fi.get_filenames(filepath)
     print(f'订单{order_id}有{len(filenames)}个文件')
@@ -114,9 +107,27 @@
     ftp_pool.set_save_path(save_path)
     ftp_pool.download()
     ftp_pool.close()
 
     print("全部下载完成")
 
 
+def commond():
+    '''
+    命令行调用
+    '''
+    parser = argparse.ArgumentParser(description='下载NOAA数据，比如ATMS L1 L2的数据')
+    parser.add_argument('order', type=str, help='订单编号')
+    parser.add_argument('--nftp', '-n', default=30,
+                        type=int, help='ftp最大数量，默认为%(default)s')
+    parser.add_argument('-o', dest='save_path', metavar='PATH',
+                        default='./', type=str, help='保存路径，默认为当前路径')
+    args = parser.parse_args()
+
+    order_id = args.order
+    num_ftp = args.nftp
+    save_path = args.save_path
+    main(order_id, num_ftp, save_path)
+
+
 if __name__ == '__main__':
-    main()
+    commond()
```

### Comparing `szh_toolbox-0.0.7/PKG-INFO` & `szh_toolbox-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: szh_toolbox
-Version: 0.0.7
-Summary: A small example package
+Version: 0.0.8
+Summary: 我自己的工具箱
 Author-email: szh <suo.zh@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
@@ -42,10 +42,15 @@
 # 一行代码替换变量
 ShellScriptVariable.modify('data/myshell.sh', 'a', '这是A', 'data/myshell3.sh')
 ```
 # 命令行工具
 也就是可以直接在命令行里执行的代码
 ```bash
 # 直接打印namelist.wps文件定义的区域的范围
-stwps
-stwps namelist.wps
+st-wps
+st-wps namelist.wps
+```
+```bash
+# 下载noaa的数据比如ATMS L1
+st-noaa -h
+st-noaa orderId -o savepath
 ```
```

