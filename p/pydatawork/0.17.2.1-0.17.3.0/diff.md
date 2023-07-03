# Comparing `tmp/pydatawork-0.17.2.1.tar.gz` & `tmp/pydatawork-0.17.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.2.1.tar", last modified: Sun Jul  2 07:21:16 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.3.0.tar", last modified: Mon Jul  3 13:31:07 2023, max compression
```

## Comparing `pydatawork-0.17.2.1.tar` & `pydatawork-0.17.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15838 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    12159 2023-07-01 18:02:42.000000 pydatawork-0.17.2.1/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15838 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    32701 2023-07-02 06:25:14.000000 pydatawork-0.17.2.1/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-02 07:21:16.000000 pydatawork-0.17.2.1/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-02 07:20:38.000000 pydatawork-0.17.2.1/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    16837 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    12974 2023-07-03 13:26:40.000000 pydatawork-0.17.3.0/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    16837 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    38814 2023-07-03 13:26:02.000000 pydatawork-0.17.3.0/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-03 13:19:13.000000 pydatawork-0.17.3.0/setup.py
```

### Comparing `pydatawork-0.17.2.1/PKG-INFO` & `pydatawork-0.17.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.2.1
+Version: 0.17.3.0
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -17,14 +17,36 @@
         - data processing
         - data analysis
         
         
         
         # Basic Functions
         
+        
+        ## file_split() 文件分割：按指定数量对文件夹中的文件进行拆分 （v 0.17.3.0）
+        
+        ###### Mon Jul 3 21:21:23 CST 2023
+        
+        ```python
+        def file_split():
+            """
+            功能：对文件夹中的文件按指定数量进行拆分。（会忽略文件夹，只处理文件）。如，文件夹中有1000张图片，可将其拆分为10个小文件夹，每个文件夹100张图片，文件夹编号为1-10。
+        
+            参数：无需提前输入参数，执行后，根据终端中的提示进行输入。
+        
+            path = input("请输入原始文件路径:")  # 输入待分割的原始文件所在路径。
+        
+            folderPath = input("请输入要输出的路径:")  # 输入分割后的结果存放路径。
+        
+            number = int(input("请输入每个文件夹中文件数:"))  # 每个文件夹中的文件数。
+            """
+        ```
+        
+        
+        
         ## move_files_by_keyword() 按文件名中关键词移动文件，灵活提取文件 (v 0.17.1.2)
         
         ###### Sun Jul 2 24:35:12 CST 2023
         
         ```python
         def move_files_by_keyword(raw_data_path,working_path):
             """
@@ -69,32 +91,32 @@
         找到名称中包括 11 的文件
         copying: 111.zip to /home/test_data/copy_files_by_keyword/working/11
         名称中包括 11 的文件已提取（复制）完毕
         ```
         
         
         
-        ## current_folder_name() 给定一个路径，返回当前文件夹名 (v 0.1.26)
+        ## get_current_folder_name() 给定一个路径，返回当前文件夹名 (v 0.1.26)
         
         ###### Mon Jun 26 24:23:48 CST 2023
         ```python
-        def current_folder_name(path):
+        def get_current_folder_name(path):
             """
             path:一个路径，可以是文件夹路径，也可以是文件路径
             结果：返回current_folder_name
             """
         ```
         
         
         
-        ## file_name() 给定一个路径，返回文件名  (v 0.1.32)
+        ## get_file_name() 给定一个路径，返回文件名  (v 0.1.32)
         
         ###### Mon Jun 26 24:24:45 CST 2023
         ```python
-        def file_name(path):
+        def get_file_name(path):
             """
             path:一个路径，可以是文件夹路径，也可以是文件路径
             结果：返回file_name,当path为文件夹路径值，返回的值为空值
             """
         ```
         
         
@@ -281,15 +303,15 @@
         
         示例：获取梅西的微博id，获取其微博内容
         
         ```python
         import pydatawork as dw 
         
         path="/home/Desktop/pydatawork"
-        id="5934019851" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 5934019851  https://weibo.com/u/5934019851
+        id="5934019851" # 梅西的微博id。在网页版微博上找到梅西的微博，查看链接，链接为 https://weibo.com/u/5934019851 ，链接中u后面的数字即为id ,梅西微博的id为 5934019851。
         weibo_name="mx"
         
         dw.get_weibo(path,id,weibo_name)
         ```
         
         来源：非原创
         原作者：XYJISAW
@@ -349,16 +371,17 @@
         
         ## hello_jkzhou() 获得帮助（v 0.1.7）
         
         ###### Sun Jun 18 23:34:45 CST 2023
         
         ```python
         def hello_jkzhou():
-            """If you need help or have a better idea, send me an e-mail."""
-            print("My e-mail is: zhouqiling.bjfu@foxmail.com")
+            """
+            获取pydatawork的使用教程。
+            """
         ```
         
         
         ## pypi维护指令
         
         ```shell
         cd 到pydatawork文件夹
```

### Comparing `pydatawork-0.17.2.1/README.md` & `pydatawork-0.17.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,36 @@
 - data processing
 - data analysis
 
 
 
 # Basic Functions
 
+
+## file_split() 文件分割：按指定数量对文件夹中的文件进行拆分 （v 0.17.3.0）
+
+###### Mon Jul 3 21:21:23 CST 2023
+
+```python
+def file_split():
+    """
+    功能：对文件夹中的文件按指定数量进行拆分。（会忽略文件夹，只处理文件）。如，文件夹中有1000张图片，可将其拆分为10个小文件夹，每个文件夹100张图片，文件夹编号为1-10。
+
+    参数：无需提前输入参数，执行后，根据终端中的提示进行输入。
+
+    path = input("请输入原始文件路径:")  # 输入待分割的原始文件所在路径。
+
+    folderPath = input("请输入要输出的路径:")  # 输入分割后的结果存放路径。
+
+    number = int(input("请输入每个文件夹中文件数:"))  # 每个文件夹中的文件数。
+    """
+```
+
+
+
 ## move_files_by_keyword() 按文件名中关键词移动文件，灵活提取文件 (v 0.17.1.2)
 
 ###### Sun Jul 2 24:35:12 CST 2023
 
 ```python
 def move_files_by_keyword(raw_data_path,working_path):
     """
@@ -61,32 +83,32 @@
 找到名称中包括 11 的文件
 copying: 111.zip to /home/test_data/copy_files_by_keyword/working/11
 名称中包括 11 的文件已提取（复制）完毕
 ```
 
 
 
-## current_folder_name() 给定一个路径，返回当前文件夹名 (v 0.1.26)
+## get_current_folder_name() 给定一个路径，返回当前文件夹名 (v 0.1.26)
 
 ###### Mon Jun 26 24:23:48 CST 2023
 ```python
-def current_folder_name(path):
+def get_current_folder_name(path):
     """
     path:一个路径，可以是文件夹路径，也可以是文件路径
     结果：返回current_folder_name
     """
 ```
 
 
 
-## file_name() 给定一个路径，返回文件名  (v 0.1.32)
+## get_file_name() 给定一个路径，返回文件名  (v 0.1.32)
 
 ###### Mon Jun 26 24:24:45 CST 2023
 ```python
-def file_name(path):
+def get_file_name(path):
     """
     path:一个路径，可以是文件夹路径，也可以是文件路径
     结果：返回file_name,当path为文件夹路径值，返回的值为空值
     """
 ```
 
 
@@ -273,15 +295,15 @@
 
 示例：获取梅西的微博id，获取其微博内容
 
 ```python
 import pydatawork as dw 
 
 path="/home/Desktop/pydatawork"
-id="5934019851" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 5934019851  https://weibo.com/u/5934019851
+id="5934019851" # 梅西的微博id。在网页版微博上找到梅西的微博，查看链接，链接为 https://weibo.com/u/5934019851 ，链接中u后面的数字即为id ,梅西微博的id为 5934019851。
 weibo_name="mx"
 
 dw.get_weibo(path,id,weibo_name)
 ```
 
 来源：非原创
 原作者：XYJISAW
@@ -341,16 +363,17 @@
 
 ## hello_jkzhou() 获得帮助（v 0.1.7）
 
 ###### Sun Jun 18 23:34:45 CST 2023
 
 ```python
 def hello_jkzhou():
-    """If you need help or have a better idea, send me an e-mail."""
-    print("My e-mail is: zhouqiling.bjfu@foxmail.com")
+    """
+    获取pydatawork的使用教程。
+    """
 ```
 
 
 ## pypi维护指令
 
 ```shell
 cd 到pydatawork文件夹
```

### Comparing `pydatawork-0.17.2.1/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.3.0/pydatawork.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.2.1
+Version: 0.17.3.0
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
@@ -17,14 +17,36 @@
         - data processing
         - data analysis
         
         
         
         # Basic Functions
         
+        
+        ## file_split() 文件分割：按指定数量对文件夹中的文件进行拆分 （v 0.17.3.0）
+        
+        ###### Mon Jul 3 21:21:23 CST 2023
+        
+        ```python
+        def file_split():
+            """
+            功能：对文件夹中的文件按指定数量进行拆分。（会忽略文件夹，只处理文件）。如，文件夹中有1000张图片，可将其拆分为10个小文件夹，每个文件夹100张图片，文件夹编号为1-10。
+        
+            参数：无需提前输入参数，执行后，根据终端中的提示进行输入。
+        
+            path = input("请输入原始文件路径:")  # 输入待分割的原始文件所在路径。
+        
+            folderPath = input("请输入要输出的路径:")  # 输入分割后的结果存放路径。
+        
+            number = int(input("请输入每个文件夹中文件数:"))  # 每个文件夹中的文件数。
+            """
+        ```
+        
+        
+        
         ## move_files_by_keyword() 按文件名中关键词移动文件，灵活提取文件 (v 0.17.1.2)
         
         ###### Sun Jul 2 24:35:12 CST 2023
         
         ```python
         def move_files_by_keyword(raw_data_path,working_path):
             """
@@ -69,32 +91,32 @@
         找到名称中包括 11 的文件
         copying: 111.zip to /home/test_data/copy_files_by_keyword/working/11
         名称中包括 11 的文件已提取（复制）完毕
         ```
         
         
         
-        ## current_folder_name() 给定一个路径，返回当前文件夹名 (v 0.1.26)
+        ## get_current_folder_name() 给定一个路径，返回当前文件夹名 (v 0.1.26)
         
         ###### Mon Jun 26 24:23:48 CST 2023
         ```python
-        def current_folder_name(path):
+        def get_current_folder_name(path):
             """
             path:一个路径，可以是文件夹路径，也可以是文件路径
             结果：返回current_folder_name
             """
         ```
         
         
         
-        ## file_name() 给定一个路径，返回文件名  (v 0.1.32)
+        ## get_file_name() 给定一个路径，返回文件名  (v 0.1.32)
         
         ###### Mon Jun 26 24:24:45 CST 2023
         ```python
-        def file_name(path):
+        def get_file_name(path):
             """
             path:一个路径，可以是文件夹路径，也可以是文件路径
             结果：返回file_name,当path为文件夹路径值，返回的值为空值
             """
         ```
         
         
@@ -281,15 +303,15 @@
         
         示例：获取梅西的微博id，获取其微博内容
         
         ```python
         import pydatawork as dw 
         
         path="/home/Desktop/pydatawork"
-        id="5934019851" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 5934019851  https://weibo.com/u/5934019851
+        id="5934019851" # 梅西的微博id。在网页版微博上找到梅西的微博，查看链接，链接为 https://weibo.com/u/5934019851 ，链接中u后面的数字即为id ,梅西微博的id为 5934019851。
         weibo_name="mx"
         
         dw.get_weibo(path,id,weibo_name)
         ```
         
         来源：非原创
         原作者：XYJISAW
@@ -349,16 +371,17 @@
         
         ## hello_jkzhou() 获得帮助（v 0.1.7）
         
         ###### Sun Jun 18 23:34:45 CST 2023
         
         ```python
         def hello_jkzhou():
-            """If you need help or have a better idea, send me an e-mail."""
-            print("My e-mail is: zhouqiling.bjfu@foxmail.com")
+            """
+            获取pydatawork的使用教程。
+            """
         ```
         
         
         ## pypi维护指令
         
         ```shell
         cd 到pydatawork文件夹
```

### Comparing `pydatawork-0.17.2.1/pydatawork.py` & `pydatawork-0.17.3.0/pydatawork.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 
 # -*- coding: utf-8 -*-
 import urllib.request
 import json
-import requests
+import requests # 新电脑刚装上python时，不带这个库，需要自己安装
 import os
 import shutil
 import re
 import datetime
 import random
 import time
+import math
 
 
 # others
 
 # def break_words(stuff):
 #     """This function will break up words for us."""
 #     words = stuff.split(' ')
@@ -54,32 +55,119 @@
 
 # 折叠：ctrl + k , ctrl + 1
 # 展开：ctrl + k , ctrl + j
 
 
 # get help
 def hello_jkzhou():
-    """If you need help or have a better idea, send me an e-mail."""
+    """
+    功能：获取pydatawork的使用教程。
+    """
     print("如果需要帮助，可以给我发邮件: zhouqiling.bjfu@foxmail.com")
     print("也可以描述你的需求，给pydatawork提一个功能建议：\npydatawork功能建议收集表：https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ")
 
 
 
 
 
 
 # Basic Functions
 
 
+# 分割
+
+def file_split():
+    """
+    功能：对文件夹中的文件按指定数量进行拆分。（会忽略文件夹，只处理文件）。如，文件夹中有1000张图片，可将其拆分为10个小文件夹，每个文件夹100张图片，文件夹编号为1-10。
+
+    参数：无需提前输入参数，执行后，根据终端中的提示进行输入。
+
+    path = input("请输入原始文件路径:")  # 输入待分割的原始文件所在路径。
+
+    folderPath = input("请输入要输出的路径:")  # 输入分割后的结果存放路径。
+
+    number = int(input("请输入每个文件夹中文件数:"))  # 每个文件夹中的文件数。
+    """
+
+    path = input("请输入原始文件路径:\n")  # 输入原始文件路径
+    folderPath = input("请输入要输出的路径:\n")  # 输入要输出的路径
+    path = path.strip("\"")  # 去除路径两端的引号
+    folderPath = folderPath.strip("\"")  # 去除路径两端的引号
+
+    number = int(input("请输入每个文件夹中文件数:\n"))  # 每个文件夹中的文件数
+    file_list = os.listdir(path)  # 原始文件名称列表
+    Number = math.ceil(len(file_list) / number)  # 目标文件夹数量
+
+    # 从0号文件夹开始，使用此处的设置
+    # folderNumber = -1 #起始文件夹id ，-1是因为0 % 任意数 = 0
+    # sort_folder_number = [x for x in range(0,Number)]
+
+    # 从1号文件夹开始，使用此处的设置
+    folderNumber = 0 # 起始文件夹id ，移动文件时，考虑到第一个文件的索引是0，由于将文件移动到哪个文件夹这个环节涉及到数学计算及判断（判断取余数的结果是否为0），索引，为保证第一个文件能存到1号文件夹，这里的初始id设置0，而不能直接设成1，在数学判断后，id会变成0+1=1。（0 % 任意数 = 0）
+    sort_folder_number = [x for x in range(1,Number+1)] # 这里可以是从1开始，不必从0开始，如果从0开始，会建立一个0号文件夹
+
+    # 创建文件夹
+    for foldernumber in sort_folder_number:
+        new_folder_path = os.path.join(folderPath, '%s' % foldernumber)  # 新文件夹路径为 'folderPath\number' 。
+        """
+        @知识卡片
+        这行代码的作用是将文件夹路径和文件夹编号拼接起来，形成新的文件夹路径。`os.path.join()` 函数用于拼接路径，它接受多个参数，并根据操作系统的不同使用适当的路径分隔符进行拼接。在这里，`folderPath` 是用户输入的输出路径，`'%s' % foldernumber` 是文件夹编号，通过字符串格式化将其转换为字符串。通过调用 `os.path.join(folderPath, '%s' % foldernumber)`，将输出路径和文件夹编号拼接在一起，得到新的文件夹路径 `new_folder_path`。例如，如果 `folderPath` 是 `/path/to/output`，`foldernumber` 是 `0`，那么 `new_folder_path` 将是 `/path/to/output/0`。这样就可以根据文件夹编号创建不同的文件夹路径。
+        """
+        if not os.path.exists(new_folder_path):
+            os.makedirs(new_folder_path)  # 创建新文件夹
+            print("新建了一个名为" + str(foldernumber) + "的文件夹，路径为" + new_folder_path)
+
+    # 分包
+    for i in range(0, len(file_list)):
+        old_file = os.path.join(path, file_list[i])  # 原始文件路径
+        if os.path.isdir(old_file):
+            '''如果路径是文件夹，程序将跳过它'''
+            print('图片不存在，路径为' + old_file + '，它是一个文件夹')
+            pass
+        elif not os.path.exists(old_file):
+            '''如果路径不存在，程序将跳过它'''
+            print('图片不存在，路径为' + old_file)
+            pass
+        else:
+            '''定义文件夹编号，与每个文件夹处理图片的数量相关'''
+            if (0 == (i % number)):  # @ 知识卡片 第一个i=0, 0 % 任意数 = 0,所以，folderNumber = 0，加1后为1，第一个文件会移动到1号文件夹中;如果每个文件夹中20个，索引0-19会存到1；上面虽然建立了0号文件夹，但0号文件夹不存东西。
+                folderNumber += 1  # 增加文件夹编号
+            """
+            @知识卡片
+            这段代码用于确定每个文件应该被移动到哪个文件夹中。
+            首先，`(i % number)` 是计算 `i` 除以 `number` 的余数。如果余数为 0，表示 `i` 是 `number` 的倍数。然后，`(0 == (i % number))` 是判断 `(i % number)` 是否等于 0。如果等于 0，表示 `i` 是 `number` 的倍数。
+            如果 `(i % number)` 等于 0，即 `i` 是 `number` 的倍数，那么 `folderNumber` 的值会加 1。这样，每当遍历到一个是 `number` 的倍数的文件时，`folderNumber` 的值就会增加，从而确定下一个文件应该被移动到的文件夹编号。
+            例如，如果 `number` 是 5，那么当 `i` 的值为 0、5、10、15 等时，`(i % number)` 的值都为 0，此时 `folderNumber` 的值会加 1。这样就可以确保每个文件夹中的文件数不超过 `number`，并且文件按照顺序被分配到不同的文件夹中。
+            """
+
+            new_file_path = os.path.join(folderPath, '%s' % (folderNumber))  # 新文件路径
+            if not os.path.exists(new_file_path):
+                break
+            shutil.move(old_file, new_file_path)  # 移动文件
+            print(old_file + '成功移动到' + new_file_path)
+
+    print(f"分割完毕：已将文件分到 {Number} 个文件夹，每个文件夹 {number} 个文件")
+
+
+
+
+# 文件对比
+
+
 def copy_files_by_keyword(raw_data_path,working_path):
     """
-    raw_data_path：原始数据所在路径。（不会复制子文件夹，也不会遍历子文件夹）
+    功能：根据文件名中的关键词复制文件。
+
+    参数：
+
+    raw_data_path：原始数据所在路径。（不会复制子文件夹，也不会遍历子文件夹）。
+    
     working_path：工作路径，提取出来的文件将存放到该路径。
+
     keyword（不是参数）：指文件名中包含的关键词，不是参数，程序运行后，在命令行中根据提示按需输入。
-    目标：根据文件名中的关键词复制文件。
     """
 
     # 原始数据文件夹
     raw_data_path = raw_data_path
     # 给定工作路径，或基础路径，用于制作结果文件夹路径
     working_path = working_path
 
@@ -106,18 +194,23 @@
     print(f"名称中包括 {keyword} 的文件已提取（复制）完毕") 
 
 
 
 
 def move_files_by_keyword(raw_data_path,working_path):
     """
-    raw_data_path：原始数据所在路径。（不会移动子文件夹，也不会遍历子文件夹）
+    功能：根据文件名中的关键词移动文件。
+
+    参数：
+
+    raw_data_path：原始数据所在路径。（不会移动子文件夹，也不会遍历子文件夹）。
+
     working_path：工作路径，提取出来的文件将存放到该路径。
+
     keyword（不是参数）：指文件名中包含的关键词，不是参数，程序运行后，在命令行中根据提示按需输入。
-    目标：根据文件名中的关键词移动文件。
     """
 
     # 原始数据文件夹
     raw_data_path = raw_data_path
     # 给定工作路径，或基础路径，用于制作结果文件夹路径
     working_path = working_path
 
@@ -143,35 +236,41 @@
                 continue 
 
     print(f"名称中包括 {keyword} 的文件已提取（移动）完毕") 
 
 
 
 
-def current_folder_name(path):
+def get_current_folder_name(path):
     """
-    path:一个路径，可以是文件夹路径，也可以是文件路径
-    结果：返回current_folder_name
+    功能：输入一个路径，返回当前文件夹名。
+
+    参数：
+
+    path：一个路径，可以是文件夹路径，也可以是文件路径。
     """
     # 判断路径是文件夹路径还是文件路径
     if os.path.isdir(path):
         # 如果是文件夹路径
         current_folder_name = os.path.basename(path)
     else:
         # 如果是文件路径
         current_folder_name = os.path.basename(os.path.dirname(path))
     return current_folder_name
 
 
 
 
-def file_name(path):
+def get_file_name(path):
     """
-    path:一个路径，可以是文件夹路径，也可以是文件路径
-    结果：返回file_name,当path为文件夹路径值，返回的值为空值
+    功能：输入一个路径，返回文件名。（当path为文件夹路径，返回的值为空值。）
+
+    参数：
+
+    path：一个路径，可以是文件夹路径，也可以是文件路径。
     """
     # 判断路径是文件夹路径还是文件路径
     if os.path.isdir(path):
         # 如果是文件夹路径
         file_name = None
     else:
         # 如果是文件路径
@@ -179,18 +278,23 @@
     return file_name
 
 
 
 
 def move_all_files(folder_path, target_folder, file_type_list):
     """
-    folder_path:待整理文件夹，可包含多层级子文件夹
-    target_folder:目标文件夹
-    file_type_list:一个列表，里面存放需要移动的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类
-    实现效果：将待整理文件夹及其子文件夹中指定类型的全部文件移动到目标文件夹
+    功能：将待整理文件夹及其子文件夹中指定类型的全部文件移动到目标文件夹。
+
+    参数：
+
+    folder_path：待整理文件夹，可包含多层级子文件夹。
+
+    target_folder：目标文件夹。
+
+    file_type_list：一个列表，里面存放需要移动的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类。
     """
 
     # 获取文件夹中的文件列表
     files = os.listdir(folder_path)
 
     # 遍历文件列表
     for file in files:
@@ -215,18 +319,23 @@
                 continue
 
 
 
 
 def copy_all_files(folder_path, target_folder, file_type_list):
     """
-    folder_path:待整理文件夹，可包含多层级子文件夹
-    target_folder:目标文件夹
-    file_type_list:一个列表，里面存放需要复制的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类
-    实现效果：将待整理文件夹及其子文件夹中指定类型的全部文件复制到目标文件夹
+    功能：将待整理文件夹及其子文件夹中指定类型的全部文件复制到目标文件夹。
+
+    参数：
+
+    folder_path：待整理文件夹，可包含多层级子文件夹。
+
+    target_folder：目标文件夹。
+
+    file_type_list：一个列表，里面存放需要复制的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类。
     """
 
     # 获取文件夹中的文件列表
     files = os.listdir(folder_path)
 
     # 遍历文件列表
     for file in files:
@@ -251,18 +360,23 @@
                 continue
 
 
 
 
 def move_files(folder_path, target_folder, file_type_list):
     """
-    folder_path:待整理文件夹
-    target_folder:目标文件夹
-    file_type_list:一个列表，里面存放需要移动的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类
-    实现效果：将待整理文件夹中(注：不包括子文件夹)指定类型的文件移动到目标文件夹
+    功能：将待整理文件夹中（不包括子文件夹)指定类型的文件移动到目标文件夹。
+
+    参数：
+
+    folder_path：待整理文件夹。
+
+    target_folder：目标文件夹。
+
+    file_type_list：一个列表，里面存放需要移动的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类。
     """
 
     # 获取文件夹中的文件列表
     files = os.listdir(folder_path)
 
     # 遍历文件列表
     for file in files:
@@ -287,18 +401,23 @@
                 continue
 
 
 
 
 def copy_files(folder_path, target_folder, file_type_list):
     """
-    folder_path:待整理文件夹
-    target_folder:目标文件夹
-    file_type_list:一个列表，里面存放需要复制的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类
-    实现效果：将待整理文件夹中(注：不包括子文件夹)指定类型的文件复制到目标文件夹
+    功能：将待整理文件夹中(不包括子文件夹)指定类型的文件复制到目标文件夹。
+
+    参数：
+
+    folder_path：待整理文件夹。
+
+    target_folder：目标文件夹。
+
+    file_type_list：一个列表，里面存放需要复制的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类。
     """
 
     # 获取文件夹中的文件列表
     files = os.listdir(folder_path)
 
     # 遍历文件列表
     for file in files:
@@ -322,15 +441,19 @@
             else:
                 continue
 
 
 
 def rename_folder_numeric_serialize(path):
     """
-    path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
+    功能：给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
+
+    参数：
+
+    path：文件夹路径。
     """
 
     # 定义一个函数，将输入的字符串按照数字和非数字的部分进行分割，并将数字部分转换为整数
     def split_key(s): # 【一个字符串一个字符串处理】
         parts = [] # 初始化一个空列表，用于存储分割后的字符串
         current_part = "" # 初始化一个空字符串，用于存储当前正在处理的部分
         for c in s: # 遍历字符串中的每个字符
@@ -374,16 +497,21 @@
 
 # Data Processing
 
 
 def game_number_guessing(number=100):
     """
     游戏规则：指定一个整数，确定数字的范围；根据提示猜数字，直到猜中。
-    number:大于1的整数，用于指定数字的范围，默认100，说明要猜的数字在100以内。
+
+    参数：
+
+    number：大于1的整数，默认为100，指要猜的数字在100以内。
+
     用法1：若不设定参数，可以写成 game_number_guessing() ，这时默认值为100。
+
     用法2：自定义参数，可以写成 game_number_guessing(number=200)，这时，数字范围设定为在200以内。
     """
 
     # 自定义数字的范围，不局限于100以内
     # x = int(input("输入一个数字，限定一个范围："))
     x = int(number)
 
@@ -434,20 +562,23 @@
     else:
         print(f"\nhi，无名氏，你一共猜了{num}次。")
 
 
 
 def obsidian_move_md_or_canvas_linked_images(images_path,folder_path,target_folder):
     """
-    提取obsidian中.md文档、.canvas文档中链接的图片，实现附件管理、库空间管理、笔记归档。
-    需要指定三个路径：
-    images_path:图片附件所在的文件夹。通常是笔记库的附件文件夹
-    folder_path:待整理的md、canvas文档所在文件夹（可包括多层级子文件夹，会遍历）。通常临时建立一个文件夹,将待整理的笔记存进去
-    target_folder:提前准备的文件夹，可以建在任意位置，用于存放提取出来的图片
-    执行结束后，可以将文档和对应的图片一起进行归档，实现笔记管理的目的。
+    功能：指定相关路径，提取obsidian中.md文档、.canvas文档中链接的图片，实现附件管理、库空间管理、笔记归档。
+
+    参数：
+
+    images_path：图片附件所在的文件夹。通常是笔记库的附件文件夹。
+
+    folder_path：待整理的md、canvas文档所在文件夹（可包括多层级子文件夹，会遍历）。通常临时建立一个文件夹,将待整理的笔记存进去。
+
+    target_folder：提前准备的文件夹，可以建在任意位置，用于存放提取出来的图片。
     """
 
     # 001-图片文件夹:原始库的附件文件夹路径
     images_path = images_path
     # 002-文件夹路径：准备移动归档的文件夹，里面包含.md和.canvas格式的文件
     folder_path = folder_path
     # 003-图片移动的目标文件夹：通常，在002中建立一个文件夹，用于存放图片即可
@@ -502,17 +633,21 @@
     print(f"\n已整理{num_images}个附件！")
 
 
 
 
 def obsidian_bookmarks_merge_and_deduplicate(original_bookmarks_path,result_path):
     """
-    函数设计：用于处理surfing插件产生的bookmarks。先合并多个bookmarks（只有1个也能正常使用），再对合并后的bookmarks去重，最后得到一个最全、不重复的bookmarks。
-    original_bookmarks_path:一个路径，路径下存放bookmarks文件，json格式，可以是1个或多个json文件。
-    result_path:一个路径，用于存放最终结果。
+    功能：用于处理surfing插件产生的bookmarks。先合并多个bookmarks（只有1个也能正常使用），再对合并后的bookmarks去重，最后得到一个最全、不重复的bookmarks。
+
+    参数：
+
+    original_bookmarks_path：一个路径，路径下存放bookmarks文件，json格式，可以是1个或多个json文件。
+
+    result_path：一个路径，用于存放最终结果。
     """
 
     # 当次处理结果文件夹
     result_path = result_path
     # 待处理书签文件夹：里面包括多个书签文件，仅包含1个也行
     original_bookmarks_path = original_bookmarks_path
 
@@ -578,28 +713,35 @@
     print("书签合并与去重完毕！")
 
 
 
 
 def get_weibo(path,id,weibo_name):
     """
-    path: 内容存放路径
-    id: 微博id
-    weibo_name: 内容存放路径下文件夹的名字
+    功能：获取某个微博的全部图片及正文。
+
+    参数：
+
+    path: 内容存放路径。
+
+    id: 微博id。
 
-    示例：获取梅西的微博id，获取其微博内容
+    weibo_name: 内容存放路径下一个自定义的文件夹名。
+
+    示例：获取梅西的微博id，获取其微博内容。
 
     import pydatawork as dw 
 
     path="/home/Desktop/pydatawork"
-    id="5934019851" # 梅西的微博id。在网页版上能获得链接，链接中u后面的内容即为id ,梅西微博的id为 5934019851  https://weibo.com/u/5934019851
+
+    id="5934019851" # 梅西的微博id。在网页版微博上找到梅西的微博，查看链接，链接为 https://weibo.com/u/5934019851 ，链接中u后面的数字即为id ,梅西微博的id为 5934019851。
+
     weibo_name="mx"
 
     dw.get_weibo(path,id,weibo_name)
-
     """
     path = path
     id = id # 在微博上获取
 
     proxy_addr = "122.241.72.191:808"
     weibo_name = weibo_name # 可以自定义名字
 
@@ -709,18 +851,23 @@
 
 
 
 # Data Analysis
 
 def get_BMI(height,weight):
     """
-    height：身高（m）（注意，单位为米）
-    weight：体重（kg）（注意，单位为千克）
-    调用示例：dw.get_BMI(height=1.75,weight=73)
-    BMI（身体质量指数）是一种计算一个人体重是否健康的方法，基于身高和体重的比例来计算。如果 bmi 小于 18.5，说明体重过轻；如果 bmi 在 18.5 和 24.9 之间说明体重在正常范围；如果 bmi 在 24.9 和 29.9 之间说明体重过重；如果大于 29.9 说明肥胖。
+    功能：用于BMI测量。BMI（身体质量指数）是一种计算一个人体重是否健康的方法，基于身高和体重的比例来计算。如果 bmi 小于 18.5，说明体重过轻；如果 bmi 在 18.5 和 24.9 之间说明体重在正常范围；如果 bmi 在 24.9 和 29.9 之间说明体重过重；如果大于 29.9 说明肥胖。
+
+    参数：
+
+    height：身高（m）（注意，单位为米）。
+
+    weight：体重（kg）（注意，单位为千克）。
+
+    调用示例：dw.get_BMI(height=1.75,weight=73)。
     """
     # height = float(input("输入身高（米）："))
     # weight = float(input("输入体重（千克）："))
 
     height = float(height) 
     weight = float(weight)
     bmi = weight / (height * height)  #计算BMI指数
```

### Comparing `pydatawork-0.17.2.1/setup.py` & `pydatawork-0.17.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.2.1',
+    version='0.17.3.0',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

