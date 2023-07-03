# Comparing `tmp/pydatawork-0.17.3.0.tar.gz` & `tmp/pydatawork-0.17.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.3.0.tar", last modified: Mon Jul  3 13:31:07 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.3.1.tar", last modified: Mon Jul  3 14:06:18 2023, max compression
```

## Comparing `pydatawork-0.17.3.0.tar` & `pydatawork-0.17.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    16837 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    12974 2023-07-03 13:26:40.000000 pydatawork-0.17.3.0/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    16837 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    38814 2023-07-03 13:26:02.000000 pydatawork-0.17.3.0/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-03 13:31:07.000000 pydatawork-0.17.3.0/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-03 13:19:13.000000 pydatawork-0.17.3.0/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    18555 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    13980 2023-07-03 13:54:13.000000 pydatawork-0.17.3.1/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    18555 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    39093 2023-07-03 14:05:45.000000 pydatawork-0.17.3.1/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-03 14:06:18.000000 pydatawork-0.17.3.1/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-03 13:54:41.000000 pydatawork-0.17.3.1/setup.py
```

### Comparing `pydatawork-0.17.3.0/PKG-INFO` & `pydatawork-0.17.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,55 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.3.0
+Version: 0.17.3.1
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
         https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ
         
         
         
-        pydatawork content summary：Sun Jul 2 02:01:46 CST 2023
+        pydatawork content summary：Mon Jul 3 21:52:47 CST 2023
         - basic functions
         - data processing
         - data analysis
         
         
         
+        # pydatawork测试环境：python 3.7.2
+        
+        pydatawork中所用到的库：
+        
+        ```python
+        import os
+        import shutil
+        import re
+        import datetime
+        import random
+        import time
+        import math
+        import json
+        import requests # 需要单独安装
+        import urllib.request
+        ```
+        
+        requests非python自带的库，需要单独安装，否则无法正常运行pydatawork：
+        
+        ```shell
+        pip install requests 
+        或 
+        pip3 install requests
+        ```
+        
+        
+        
         # Basic Functions
         
         
         ## file_split() 文件分割：按指定数量对文件夹中的文件进行拆分 （v 0.17.3.0）
         
         ###### Mon Jul 3 21:21:23 CST 2023
         
@@ -46,34 +73,44 @@
         ## move_files_by_keyword() 按文件名中关键词移动文件，灵活提取文件 (v 0.17.1.2)
         
         ###### Sun Jul 2 24:35:12 CST 2023
         
         ```python
         def move_files_by_keyword(raw_data_path,working_path):
             """
-            raw_data_path：原始数据所在路径。（不会移动子文件夹，也不会遍历子文件夹）
+            功能：根据文件名中的关键词移动文件。
+        
+            参数：
+        
+            raw_data_path：原始数据所在路径。（不会移动子文件夹，也不会遍历子文件夹）。
+        
             working_path：工作路径，提取出来的文件将存放到该路径。
+        
             keyword（不是参数）：指文件名中包含的关键词，不是参数，程序运行后，在命令行中根据提示按需输入。
-            目标：根据文件名中的关键词移动文件。
             """
         ```
         
         
         
         ## copy_files_by_keyword() 按文件名中关键词复制文件，灵活提取文件 (v 0.17.1.2)
         
         ###### Sun Jul 2 24:28:40 CST 2023
         
         ```python
         def copy_files_by_keyword(raw_data_path,working_path):
             """
-            raw_data_path：原始数据所在路径。（不会复制子文件夹，也不会遍历子文件夹）
+            功能：根据文件名中的关键词复制文件。
+        
+            参数：
+        
+            raw_data_path：原始数据所在路径。（不会复制子文件夹，也不会遍历子文件夹）。
+            
             working_path：工作路径，提取出来的文件将存放到该路径。
+        
             keyword（不是参数）：指文件名中包含的关键词，不是参数，程序运行后，在命令行中根据提示按需输入。
-            目标：根据文件名中的关键词复制文件。
             """
         ```
         
         使用示例：
         
         ```python
         import pydatawork as dw
@@ -97,93 +134,119 @@
         
         ## get_current_folder_name() 给定一个路径，返回当前文件夹名 (v 0.1.26)
         
         ###### Mon Jun 26 24:23:48 CST 2023
         ```python
         def get_current_folder_name(path):
             """
-            path:一个路径，可以是文件夹路径，也可以是文件路径
-            结果：返回current_folder_name
+            功能：输入一个路径，返回当前文件夹名。
+        
+            参数：
+        
+            path：一个路径，可以是文件夹路径，也可以是文件路径。
             """
         ```
         
         
         
         ## get_file_name() 给定一个路径，返回文件名  (v 0.1.32)
         
         ###### Mon Jun 26 24:24:45 CST 2023
         ```python
         def get_file_name(path):
             """
-            path:一个路径，可以是文件夹路径，也可以是文件路径
-            结果：返回file_name,当path为文件夹路径值，返回的值为空值
+            功能：输入一个路径，返回文件名。（当path为文件夹路径，返回的值为空值。）
+        
+            参数：
+        
+            path：一个路径，可以是文件夹路径，也可以是文件路径。
             """
         ```
         
         
         
         ## copy_files() 复制当前文件夹中（不包括子文件夹）指定类型的文件 （v 0.1.23） 
         
         ###### Sun Jun 25 06:19:50 CST 2023
         
         ```python
         def copy_files(folder_path, target_folder, file_type_list):
             """
-            folder_path:待整理文件夹
-            target_folder:目标文件夹
-            file_type_list:一个列表，里面存放需要复制的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类
-            实现效果：将待整理文件夹中(注：不包括子文件夹)指定类型的文件复制到目标文件夹
+            功能：将待整理文件夹中(不包括子文件夹)指定类型的文件复制到目标文件夹。
+        
+            参数：
+        
+            folder_path：待整理文件夹。
+        
+            target_folder：目标文件夹。
+        
+            file_type_list：一个列表，里面存放需要复制的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类。
             """
         ```
         
         
         
         ## move_files() 移动当前文件夹中（不包括子文件夹）指定类型的文件 （v 0.1.23） 
         
         ###### Sun Jun 25 06:17:26 CST 2023
         
         ```python
         def move_files(folder_path, target_folder, file_type_list):
             """
-            folder_path:待整理文件夹
-            target_folder:目标文件夹
-            file_type_list:一个列表，里面存放需要移动的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类
-            实现效果：将待整理文件夹中(注：不包括子文件夹)指定类型的文件移动到目标文件夹
+            功能：将待整理文件夹中（不包括子文件夹)指定类型的文件移动到目标文件夹。
+        
+            参数：
+        
+            folder_path：待整理文件夹。
+        
+            target_folder：目标文件夹。
+        
+            file_type_list：一个列表，里面存放需要移动的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类。
             """
         ```
         
         
         
         ## copy_all_files() 复制文件夹及子文件夹下指定类型的全部文件 （v 0.1.22）
         
         ###### Sun Jun 25 06:05:29 CST 2023
         
         ```python
         def copy_all_files(folder_path, target_folder, file_type_list):
             """
-            folder_path:待整理文件夹，可包含多层级子文件夹
-            target_folder:目标文件夹
-            file_type_list:一个列表，里面存放需要复制的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类
-            实现效果：将待整理文件夹及其子文件夹中指定类型的全部文件复制到目标文件夹
+            功能：将待整理文件夹及其子文件夹中指定类型的全部文件复制到目标文件夹。
+        
+            参数：
+        
+            folder_path：待整理文件夹，可包含多层级子文件夹。
+        
+            target_folder：目标文件夹。
+        
+            file_type_list：一个列表，里面存放需要复制的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类。
             """
         ```
         
         
         
         ## move_all_files() 移动文件夹及子文件夹下指定类型的全部文件 （v 0.1.22）
         
         ###### Sun Jun 25 05:01:22 CST 2023
         
         ```python
         def move_all_files(folder_path, target_folder, file_type_list):
             """
-            folder_path:待整理文件夹，可包含多层级子文件夹
-            target_folder:目标文件夹
-            file_type_list:一个列表，里面存放需要移动的文件类别的后缀类型，如.ipg|.png|.gif|.zip|.rar|.md|.mp4|.xml|.gz(表示.tar.gz)|等，注意，要带点“.”
-            实现效果：将待整理文件夹及其子文件夹中指定类型的全部文件移动到目标文件夹
+            功能：将待整理文件夹及其子文件夹中指定类型的全部文件移动到目标文件夹。
+        
+            参数：
+        
+            folder_path：待整理文件夹，可包含多层级子文件夹。
+        
+            target_folder：目标文件夹。
+        
+            file_type_list：一个列表，里面存放需要移动的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类。
             """
         ```
         
         示例：
         ```Python
         import pydatawork as dw 
         
@@ -199,15 +262,19 @@
         ## rename_folder_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.6）
         
         ###### Sun Jun 18 22:37:01 CST 2023
         
         ```python
         def rename_folder_numeric_serialize(path):
             """
-            path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
+            功能：给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
+        
+            参数：
+        
+            path：文件夹路径。
             """
         ```
         
         
         
         # Data Processing
         
@@ -215,16 +282,21 @@
         
         ###### Sat Jul 1 01:42:58 CST 2023
         
         ```python
         def game_number_guessing(number=100):
             """
             游戏规则：指定一个整数，确定数字的范围；根据提示猜数字，直到猜中。
-            number:大于1的整数，用于指定数字的范围，默认100，说明要猜的数字在100以内。
+        
+            参数：
+        
+            number：大于1的整数，默认为100，指要猜的数字在100以内。
+        
             用法1：若不设定参数，可以写成 game_number_guessing() ，这时默认值为100。
+        
             用法2：自定义参数，可以写成 game_number_guessing(number=200)，这时，数字范围设定为在200以内。
             """
         ```
         
         使用示例1：
         
         ```python
@@ -246,35 +318,42 @@
         ## obsidian_bookmarks_merge_and_deduplicate() obsidian中surfing插件产生的书签整理：先合并，再去重 （v 0.1.31）
         
         ###### Mon Jun 26 22:50:45 CST 2023
         
         ```python
         def obsidian_bookmarks_merge_and_deduplicate(original_bookmarks_path,result_path):
             """
-            函数设计：用于处理surfing插件产生的bookmarks。先合并多个bookmarks（只有1个也能正常使用），再对合并后的bookmarks去重，最后得到一个最全、不重复的bookmarks。
-            original_bookmarks_path:一个路径，路径下存放bookmarks文件，json格式，可以是1个或多个json文件。
-            result_path:一个路径，用于存放最终结果。
+            功能：用于处理surfing插件产生的bookmarks。先合并多个bookmarks（只有1个也能正常使用），再对合并后的bookmarks去重，最后得到一个最全、不重复的bookmarks。
+        
+            参数：
+        
+            original_bookmarks_path：一个路径，路径下存放bookmarks文件，json格式，可以是1个或多个json文件。
+        
+            result_path：一个路径，用于存放最终结果。
             """
         ```
         
         
         
         ## obsidian_move_md_or_canvas_linked_images() 提取obsidian中.md文档、.canvas文档中链接的图片，实现附件管理、库空间管理、笔记归档 (v 0.1.24)
         
         ###### Sat Jun 24 18:37:16 CST 2023
         
         ```python
         def obsidian_move_md_or_canvas_linked_images(images_path,folder_path,target_folder):
             """
-            提取obsidian中.md文档、.canvas文档中链接的图片，实现附件管理、库空间管理、笔记归档。
-            需要指定三个路径：
-            images_path:图片附件所在的文件夹。通常是笔记库的附件文件夹
-            folder_path:待整理的md、canvas文档所在文件夹（可包括多层级子文件夹，会遍历）。通常临时建立一个文件夹,将待整理的笔记存进去
-            target_folder:提前准备的文件夹，可以建在任意位置，用于存放提取出来的图片
-            执行结束后，可以将文档和对应的图片一起进行归档，实现笔记管理的目的。
+            功能：指定相关路径，提取obsidian中.md文档、.canvas文档中链接的图片，实现附件管理、库空间管理、笔记归档。
+        
+            参数：
+        
+            images_path：图片附件所在的文件夹。通常是笔记库的附件文件夹。
+        
+            folder_path：待整理的md、canvas文档所在文件夹（可包括多层级子文件夹，会遍历）。通常临时建立一个文件夹,将待整理的笔记存进去。
+        
+            target_folder：提前准备的文件夹，可以建在任意位置，用于存放提取出来的图片。
             """
         ```
         
         示例及说明：在自己的代码中提前准备好三个路径，然后调用函数
         
         ```python
         import pydatawork as dw 
@@ -291,17 +370,23 @@
         ## get_weibo() 微博图片获取（v 0.1.2）
         
         ###### Sun Jun 18 17:10:46 CST 2023
         
         ```python
         def get_weibo(path,id,weibo_name):
             """
-            path: 内容存放路径；
-            id: 微博id；
-            weibo_name: 内容存放路径下文件夹的名字。
+            功能：获取某个微博的全部图片及正文。
+        
+            参数：
+        
+            path: 内容存放路径。
+        
+            id: 微博id。（id获取方法：以梅西的微博id为例。在网页版微博上找到梅西的微博，查看链接，链接为 https://weibo.com/u/5934019851 ，链接中u后面的数字即为id ,梅西微博的id为 5934019851。）
+        
+            weibo_name: 内容存放路径下一个自定义的文件夹名。
             """
         ```
         
         示例：获取梅西的微博id，获取其微博内容
         
         ```python
         import pydatawork as dw 
@@ -325,17 +410,21 @@
         ## get_BMI() 输入身高（m）、体重(kg)，进行身体质量指数（BMI）测量，了解当前身体健康状态，获得体重管理建议 （V 0.1.36）
         
         ###### Fri Jun 30 19:50:03 CST 2023
         
         ```python
         def get_BMI(height,weight):
             """
-            height：身高（m）（注意，单位为米）
-            weight：体重（kg）（注意，单位为千克）
-            BMI（身体质量指数）是一种计算一个人体重是否健康的方法，基于身高和体重的比例来计算。如果 bmi 小于 18.5，说明体重过轻；如果 bmi 在 18.5 和 24.9 之间说明体重在正常范围；如果 bmi 在 24.9 和 29.9 之间说明体重过重；如果大于 29.9 说明肥胖。
+            功能：用于BMI测量。BMI（身体质量指数）是一种计算一个人体重是否健康的方法，基于身高和体重的比例来计算。如果 bmi 小于 18.5，说明体重过轻；如果 bmi 在 18.5 和 24.9 之间说明体重在正常范围；如果 bmi 在 24.9 和 29.9 之间说明体重过重；如果大于 29.9 说明肥胖。
+        
+            参数：
+        
+            height：身高（m）（注意，单位为米）。
+        
+            weight：体重（kg）（注意，单位为千克）。
             """
         ```
         
         使用示例1：
         
         ```python
         import pydatawork as dw
```

### Comparing `pydatawork-0.17.3.0/README.md` & `pydatawork-0.17.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,47 @@
 
 pydatawork功能建议收集表：
 https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ
 
 
 
-pydatawork content summary：Sun Jul 2 02:01:46 CST 2023
+pydatawork content summary：Mon Jul 3 21:52:47 CST 2023
 - basic functions
 - data processing
 - data analysis
 
 
 
+# pydatawork测试环境：python 3.7.2
+
+pydatawork中所用到的库：
+
+```python
+import os
+import shutil
+import re
+import datetime
+import random
+import time
+import math
+import json
+import requests # 需要单独安装
+import urllib.request
+```
+
+requests非python自带的库，需要单独安装，否则无法正常运行pydatawork：
+
+```shell
+pip install requests 
+或 
+pip3 install requests
+```
+
+
+
 # Basic Functions
 
 
 ## file_split() 文件分割：按指定数量对文件夹中的文件进行拆分 （v 0.17.3.0）
 
 ###### Mon Jul 3 21:21:23 CST 2023
 
@@ -38,34 +65,44 @@
 ## move_files_by_keyword() 按文件名中关键词移动文件，灵活提取文件 (v 0.17.1.2)
 
 ###### Sun Jul 2 24:35:12 CST 2023
 
 ```python
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
 ```
 
 
 
 ## copy_files_by_keyword() 按文件名中关键词复制文件，灵活提取文件 (v 0.17.1.2)
 
 ###### Sun Jul 2 24:28:40 CST 2023
 
 ```python
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
 ```
 
 使用示例：
 
 ```python
 import pydatawork as dw
@@ -89,93 +126,119 @@
 
 ## get_current_folder_name() 给定一个路径，返回当前文件夹名 (v 0.1.26)
 
 ###### Mon Jun 26 24:23:48 CST 2023
 ```python
 def get_current_folder_name(path):
     """
-    path:一个路径，可以是文件夹路径，也可以是文件路径
-    结果：返回current_folder_name
+    功能：输入一个路径，返回当前文件夹名。
+
+    参数：
+
+    path：一个路径，可以是文件夹路径，也可以是文件路径。
     """
 ```
 
 
 
 ## get_file_name() 给定一个路径，返回文件名  (v 0.1.32)
 
 ###### Mon Jun 26 24:24:45 CST 2023
 ```python
 def get_file_name(path):
     """
-    path:一个路径，可以是文件夹路径，也可以是文件路径
-    结果：返回file_name,当path为文件夹路径值，返回的值为空值
+    功能：输入一个路径，返回文件名。（当path为文件夹路径，返回的值为空值。）
+
+    参数：
+
+    path：一个路径，可以是文件夹路径，也可以是文件路径。
     """
 ```
 
 
 
 ## copy_files() 复制当前文件夹中（不包括子文件夹）指定类型的文件 （v 0.1.23） 
 
 ###### Sun Jun 25 06:19:50 CST 2023
 
 ```python
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
 ```
 
 
 
 ## move_files() 移动当前文件夹中（不包括子文件夹）指定类型的文件 （v 0.1.23） 
 
 ###### Sun Jun 25 06:17:26 CST 2023
 
 ```python
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
 ```
 
 
 
 ## copy_all_files() 复制文件夹及子文件夹下指定类型的全部文件 （v 0.1.22）
 
 ###### Sun Jun 25 06:05:29 CST 2023
 
 ```python
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
 ```
 
 
 
 ## move_all_files() 移动文件夹及子文件夹下指定类型的全部文件 （v 0.1.22）
 
 ###### Sun Jun 25 05:01:22 CST 2023
 
 ```python
 def move_all_files(folder_path, target_folder, file_type_list):
     """
-    folder_path:待整理文件夹，可包含多层级子文件夹
-    target_folder:目标文件夹
-    file_type_list:一个列表，里面存放需要移动的文件类别的后缀类型，如.ipg|.png|.gif|.zip|.rar|.md|.mp4|.xml|.gz(表示.tar.gz)|等，注意，要带点“.”
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
 ```
 
 示例：
 ```Python
 import pydatawork as dw 
 
@@ -191,15 +254,19 @@
 ## rename_folder_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.6）
 
 ###### Sun Jun 18 22:37:01 CST 2023
 
 ```python
 def rename_folder_numeric_serialize(path):
     """
-    path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
+    功能：给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
+
+    参数：
+
+    path：文件夹路径。
     """
 ```
 
 
 
 # Data Processing
 
@@ -207,16 +274,21 @@
 
 ###### Sat Jul 1 01:42:58 CST 2023
 
 ```python
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
 ```
 
 使用示例1：
 
 ```python
@@ -238,35 +310,42 @@
 ## obsidian_bookmarks_merge_and_deduplicate() obsidian中surfing插件产生的书签整理：先合并，再去重 （v 0.1.31）
 
 ###### Mon Jun 26 22:50:45 CST 2023
 
 ```python
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
 ```
 
 
 
 ## obsidian_move_md_or_canvas_linked_images() 提取obsidian中.md文档、.canvas文档中链接的图片，实现附件管理、库空间管理、笔记归档 (v 0.1.24)
 
 ###### Sat Jun 24 18:37:16 CST 2023
 
 ```python
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
 ```
 
 示例及说明：在自己的代码中提前准备好三个路径，然后调用函数
 
 ```python
 import pydatawork as dw 
@@ -283,17 +362,23 @@
 ## get_weibo() 微博图片获取（v 0.1.2）
 
 ###### Sun Jun 18 17:10:46 CST 2023
 
 ```python
 def get_weibo(path,id,weibo_name):
     """
-    path: 内容存放路径；
-    id: 微博id；
-    weibo_name: 内容存放路径下文件夹的名字。
+    功能：获取某个微博的全部图片及正文。
+
+    参数：
+
+    path: 内容存放路径。
+
+    id: 微博id。（id获取方法：以梅西的微博id为例。在网页版微博上找到梅西的微博，查看链接，链接为 https://weibo.com/u/5934019851 ，链接中u后面的数字即为id ,梅西微博的id为 5934019851。）
+
+    weibo_name: 内容存放路径下一个自定义的文件夹名。
     """
 ```
 
 示例：获取梅西的微博id，获取其微博内容
 
 ```python
 import pydatawork as dw 
@@ -317,17 +402,21 @@
 ## get_BMI() 输入身高（m）、体重(kg)，进行身体质量指数（BMI）测量，了解当前身体健康状态，获得体重管理建议 （V 0.1.36）
 
 ###### Fri Jun 30 19:50:03 CST 2023
 
 ```python
 def get_BMI(height,weight):
     """
-    height：身高（m）（注意，单位为米）
-    weight：体重（kg）（注意，单位为千克）
-    BMI（身体质量指数）是一种计算一个人体重是否健康的方法，基于身高和体重的比例来计算。如果 bmi 小于 18.5，说明体重过轻；如果 bmi 在 18.5 和 24.9 之间说明体重在正常范围；如果 bmi 在 24.9 和 29.9 之间说明体重过重；如果大于 29.9 说明肥胖。
+    功能：用于BMI测量。BMI（身体质量指数）是一种计算一个人体重是否健康的方法，基于身高和体重的比例来计算。如果 bmi 小于 18.5，说明体重过轻；如果 bmi 在 18.5 和 24.9 之间说明体重在正常范围；如果 bmi 在 24.9 和 29.9 之间说明体重过重；如果大于 29.9 说明肥胖。
+
+    参数：
+
+    height：身高（m）（注意，单位为米）。
+
+    weight：体重（kg）（注意，单位为千克）。
     """
 ```
 
 使用示例1：
 
 ```python
 import pydatawork as dw
```

### Comparing `pydatawork-0.17.3.0/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.3.1/pydatawork.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,55 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.3.0
+Version: 0.17.3.1
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
         https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ
         
         
         
-        pydatawork content summary：Sun Jul 2 02:01:46 CST 2023
+        pydatawork content summary：Mon Jul 3 21:52:47 CST 2023
         - basic functions
         - data processing
         - data analysis
         
         
         
+        # pydatawork测试环境：python 3.7.2
+        
+        pydatawork中所用到的库：
+        
+        ```python
+        import os
+        import shutil
+        import re
+        import datetime
+        import random
+        import time
+        import math
+        import json
+        import requests # 需要单独安装
+        import urllib.request
+        ```
+        
+        requests非python自带的库，需要单独安装，否则无法正常运行pydatawork：
+        
+        ```shell
+        pip install requests 
+        或 
+        pip3 install requests
+        ```
+        
+        
+        
         # Basic Functions
         
         
         ## file_split() 文件分割：按指定数量对文件夹中的文件进行拆分 （v 0.17.3.0）
         
         ###### Mon Jul 3 21:21:23 CST 2023
         
@@ -46,34 +73,44 @@
         ## move_files_by_keyword() 按文件名中关键词移动文件，灵活提取文件 (v 0.17.1.2)
         
         ###### Sun Jul 2 24:35:12 CST 2023
         
         ```python
         def move_files_by_keyword(raw_data_path,working_path):
             """
-            raw_data_path：原始数据所在路径。（不会移动子文件夹，也不会遍历子文件夹）
+            功能：根据文件名中的关键词移动文件。
+        
+            参数：
+        
+            raw_data_path：原始数据所在路径。（不会移动子文件夹，也不会遍历子文件夹）。
+        
             working_path：工作路径，提取出来的文件将存放到该路径。
+        
             keyword（不是参数）：指文件名中包含的关键词，不是参数，程序运行后，在命令行中根据提示按需输入。
-            目标：根据文件名中的关键词移动文件。
             """
         ```
         
         
         
         ## copy_files_by_keyword() 按文件名中关键词复制文件，灵活提取文件 (v 0.17.1.2)
         
         ###### Sun Jul 2 24:28:40 CST 2023
         
         ```python
         def copy_files_by_keyword(raw_data_path,working_path):
             """
-            raw_data_path：原始数据所在路径。（不会复制子文件夹，也不会遍历子文件夹）
+            功能：根据文件名中的关键词复制文件。
+        
+            参数：
+        
+            raw_data_path：原始数据所在路径。（不会复制子文件夹，也不会遍历子文件夹）。
+            
             working_path：工作路径，提取出来的文件将存放到该路径。
+        
             keyword（不是参数）：指文件名中包含的关键词，不是参数，程序运行后，在命令行中根据提示按需输入。
-            目标：根据文件名中的关键词复制文件。
             """
         ```
         
         使用示例：
         
         ```python
         import pydatawork as dw
@@ -97,93 +134,119 @@
         
         ## get_current_folder_name() 给定一个路径，返回当前文件夹名 (v 0.1.26)
         
         ###### Mon Jun 26 24:23:48 CST 2023
         ```python
         def get_current_folder_name(path):
             """
-            path:一个路径，可以是文件夹路径，也可以是文件路径
-            结果：返回current_folder_name
+            功能：输入一个路径，返回当前文件夹名。
+        
+            参数：
+        
+            path：一个路径，可以是文件夹路径，也可以是文件路径。
             """
         ```
         
         
         
         ## get_file_name() 给定一个路径，返回文件名  (v 0.1.32)
         
         ###### Mon Jun 26 24:24:45 CST 2023
         ```python
         def get_file_name(path):
             """
-            path:一个路径，可以是文件夹路径，也可以是文件路径
-            结果：返回file_name,当path为文件夹路径值，返回的值为空值
+            功能：输入一个路径，返回文件名。（当path为文件夹路径，返回的值为空值。）
+        
+            参数：
+        
+            path：一个路径，可以是文件夹路径，也可以是文件路径。
             """
         ```
         
         
         
         ## copy_files() 复制当前文件夹中（不包括子文件夹）指定类型的文件 （v 0.1.23） 
         
         ###### Sun Jun 25 06:19:50 CST 2023
         
         ```python
         def copy_files(folder_path, target_folder, file_type_list):
             """
-            folder_path:待整理文件夹
-            target_folder:目标文件夹
-            file_type_list:一个列表，里面存放需要复制的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类
-            实现效果：将待整理文件夹中(注：不包括子文件夹)指定类型的文件复制到目标文件夹
+            功能：将待整理文件夹中(不包括子文件夹)指定类型的文件复制到目标文件夹。
+        
+            参数：
+        
+            folder_path：待整理文件夹。
+        
+            target_folder：目标文件夹。
+        
+            file_type_list：一个列表，里面存放需要复制的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类。
             """
         ```
         
         
         
         ## move_files() 移动当前文件夹中（不包括子文件夹）指定类型的文件 （v 0.1.23） 
         
         ###### Sun Jun 25 06:17:26 CST 2023
         
         ```python
         def move_files(folder_path, target_folder, file_type_list):
             """
-            folder_path:待整理文件夹
-            target_folder:目标文件夹
-            file_type_list:一个列表，里面存放需要移动的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类
-            实现效果：将待整理文件夹中(注：不包括子文件夹)指定类型的文件移动到目标文件夹
+            功能：将待整理文件夹中（不包括子文件夹)指定类型的文件移动到目标文件夹。
+        
+            参数：
+        
+            folder_path：待整理文件夹。
+        
+            target_folder：目标文件夹。
+        
+            file_type_list：一个列表，里面存放需要移动的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类。
             """
         ```
         
         
         
         ## copy_all_files() 复制文件夹及子文件夹下指定类型的全部文件 （v 0.1.22）
         
         ###### Sun Jun 25 06:05:29 CST 2023
         
         ```python
         def copy_all_files(folder_path, target_folder, file_type_list):
             """
-            folder_path:待整理文件夹，可包含多层级子文件夹
-            target_folder:目标文件夹
-            file_type_list:一个列表，里面存放需要复制的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类
-            实现效果：将待整理文件夹及其子文件夹中指定类型的全部文件复制到目标文件夹
+            功能：将待整理文件夹及其子文件夹中指定类型的全部文件复制到目标文件夹。
+        
+            参数：
+        
+            folder_path：待整理文件夹，可包含多层级子文件夹。
+        
+            target_folder：目标文件夹。
+        
+            file_type_list：一个列表，里面存放需要复制的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类。
             """
         ```
         
         
         
         ## move_all_files() 移动文件夹及子文件夹下指定类型的全部文件 （v 0.1.22）
         
         ###### Sun Jun 25 05:01:22 CST 2023
         
         ```python
         def move_all_files(folder_path, target_folder, file_type_list):
             """
-            folder_path:待整理文件夹，可包含多层级子文件夹
-            target_folder:目标文件夹
-            file_type_list:一个列表，里面存放需要移动的文件类别的后缀类型，如.ipg|.png|.gif|.zip|.rar|.md|.mp4|.xml|.gz(表示.tar.gz)|等，注意，要带点“.”
-            实现效果：将待整理文件夹及其子文件夹中指定类型的全部文件移动到目标文件夹
+            功能：将待整理文件夹及其子文件夹中指定类型的全部文件移动到目标文件夹。
+        
+            参数：
+        
+            folder_path：待整理文件夹，可包含多层级子文件夹。
+        
+            target_folder：目标文件夹。
+        
+            file_type_list：一个列表，里面存放需要移动的文件类别的后缀类型，如[".jpg",".zip",".png",".gz",".whl",".md"]，注意，要带点“.”。其中“.gz”表示“.tar.gz”这一类。
             """
         ```
         
         示例：
         ```Python
         import pydatawork as dw 
         
@@ -199,15 +262,19 @@
         ## rename_folder_numeric_serialize() 文件夹从左到右比较，按数值从小到大排序，再从1开始进行序列化重命名（v 0.1.6）
         
         ###### Sun Jun 18 22:37:01 CST 2023
         
         ```python
         def rename_folder_numeric_serialize(path):
             """
-            path:文件夹路径。给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
+            功能：给定一个文件夹路径，获取其中子文件夹的名字，根据子文件夹的名字，从左到右进行比较，按数值从小到大对子文件夹排序，再从1开始对子文件夹进行序列化重命名。
+        
+            参数：
+        
+            path：文件夹路径。
             """
         ```
         
         
         
         # Data Processing
         
@@ -215,16 +282,21 @@
         
         ###### Sat Jul 1 01:42:58 CST 2023
         
         ```python
         def game_number_guessing(number=100):
             """
             游戏规则：指定一个整数，确定数字的范围；根据提示猜数字，直到猜中。
-            number:大于1的整数，用于指定数字的范围，默认100，说明要猜的数字在100以内。
+        
+            参数：
+        
+            number：大于1的整数，默认为100，指要猜的数字在100以内。
+        
             用法1：若不设定参数，可以写成 game_number_guessing() ，这时默认值为100。
+        
             用法2：自定义参数，可以写成 game_number_guessing(number=200)，这时，数字范围设定为在200以内。
             """
         ```
         
         使用示例1：
         
         ```python
@@ -246,35 +318,42 @@
         ## obsidian_bookmarks_merge_and_deduplicate() obsidian中surfing插件产生的书签整理：先合并，再去重 （v 0.1.31）
         
         ###### Mon Jun 26 22:50:45 CST 2023
         
         ```python
         def obsidian_bookmarks_merge_and_deduplicate(original_bookmarks_path,result_path):
             """
-            函数设计：用于处理surfing插件产生的bookmarks。先合并多个bookmarks（只有1个也能正常使用），再对合并后的bookmarks去重，最后得到一个最全、不重复的bookmarks。
-            original_bookmarks_path:一个路径，路径下存放bookmarks文件，json格式，可以是1个或多个json文件。
-            result_path:一个路径，用于存放最终结果。
+            功能：用于处理surfing插件产生的bookmarks。先合并多个bookmarks（只有1个也能正常使用），再对合并后的bookmarks去重，最后得到一个最全、不重复的bookmarks。
+        
+            参数：
+        
+            original_bookmarks_path：一个路径，路径下存放bookmarks文件，json格式，可以是1个或多个json文件。
+        
+            result_path：一个路径，用于存放最终结果。
             """
         ```
         
         
         
         ## obsidian_move_md_or_canvas_linked_images() 提取obsidian中.md文档、.canvas文档中链接的图片，实现附件管理、库空间管理、笔记归档 (v 0.1.24)
         
         ###### Sat Jun 24 18:37:16 CST 2023
         
         ```python
         def obsidian_move_md_or_canvas_linked_images(images_path,folder_path,target_folder):
             """
-            提取obsidian中.md文档、.canvas文档中链接的图片，实现附件管理、库空间管理、笔记归档。
-            需要指定三个路径：
-            images_path:图片附件所在的文件夹。通常是笔记库的附件文件夹
-            folder_path:待整理的md、canvas文档所在文件夹（可包括多层级子文件夹，会遍历）。通常临时建立一个文件夹,将待整理的笔记存进去
-            target_folder:提前准备的文件夹，可以建在任意位置，用于存放提取出来的图片
-            执行结束后，可以将文档和对应的图片一起进行归档，实现笔记管理的目的。
+            功能：指定相关路径，提取obsidian中.md文档、.canvas文档中链接的图片，实现附件管理、库空间管理、笔记归档。
+        
+            参数：
+        
+            images_path：图片附件所在的文件夹。通常是笔记库的附件文件夹。
+        
+            folder_path：待整理的md、canvas文档所在文件夹（可包括多层级子文件夹，会遍历）。通常临时建立一个文件夹,将待整理的笔记存进去。
+        
+            target_folder：提前准备的文件夹，可以建在任意位置，用于存放提取出来的图片。
             """
         ```
         
         示例及说明：在自己的代码中提前准备好三个路径，然后调用函数
         
         ```python
         import pydatawork as dw 
@@ -291,17 +370,23 @@
         ## get_weibo() 微博图片获取（v 0.1.2）
         
         ###### Sun Jun 18 17:10:46 CST 2023
         
         ```python
         def get_weibo(path,id,weibo_name):
             """
-            path: 内容存放路径；
-            id: 微博id；
-            weibo_name: 内容存放路径下文件夹的名字。
+            功能：获取某个微博的全部图片及正文。
+        
+            参数：
+        
+            path: 内容存放路径。
+        
+            id: 微博id。（id获取方法：以梅西的微博id为例。在网页版微博上找到梅西的微博，查看链接，链接为 https://weibo.com/u/5934019851 ，链接中u后面的数字即为id ,梅西微博的id为 5934019851。）
+        
+            weibo_name: 内容存放路径下一个自定义的文件夹名。
             """
         ```
         
         示例：获取梅西的微博id，获取其微博内容
         
         ```python
         import pydatawork as dw 
@@ -325,17 +410,21 @@
         ## get_BMI() 输入身高（m）、体重(kg)，进行身体质量指数（BMI）测量，了解当前身体健康状态，获得体重管理建议 （V 0.1.36）
         
         ###### Fri Jun 30 19:50:03 CST 2023
         
         ```python
         def get_BMI(height,weight):
             """
-            height：身高（m）（注意，单位为米）
-            weight：体重（kg）（注意，单位为千克）
-            BMI（身体质量指数）是一种计算一个人体重是否健康的方法，基于身高和体重的比例来计算。如果 bmi 小于 18.5，说明体重过轻；如果 bmi 在 18.5 和 24.9 之间说明体重在正常范围；如果 bmi 在 24.9 和 29.9 之间说明体重过重；如果大于 29.9 说明肥胖。
+            功能：用于BMI测量。BMI（身体质量指数）是一种计算一个人体重是否健康的方法，基于身高和体重的比例来计算。如果 bmi 小于 18.5，说明体重过轻；如果 bmi 在 18.5 和 24.9 之间说明体重在正常范围；如果 bmi 在 24.9 和 29.9 之间说明体重过重；如果大于 29.9 说明肥胖。
+        
+            参数：
+        
+            height：身高（m）（注意，单位为米）。
+        
+            weight：体重（kg）（注意，单位为千克）。
             """
         ```
         
         使用示例1：
         
         ```python
         import pydatawork as dw
```

### Comparing `pydatawork-0.17.3.0/pydatawork.py` & `pydatawork-0.17.3.1/pydatawork.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 
 # -*- coding: utf-8 -*-
-import urllib.request
-import json
-import requests # 新电脑刚装上python时，不带这个库，需要自己安装
+
 import os
 import shutil
 import re
 import datetime
 import random
 import time
 import math
+import json
+import requests # 新电脑刚装上python时，不带这个库，需要自己安装
+import urllib.request
+
 
 
 # others
 
 # def break_words(stuff):
 #     """This function will break up words for us."""
 #     words = stuff.split(' ')
@@ -56,18 +58,21 @@
 # 折叠：ctrl + k , ctrl + 1
 # 展开：ctrl + k , ctrl + j
 
 
 # get help
 def hello_jkzhou():
     """
-    功能：获取pydatawork的使用教程。
+    功能：获取pydatawork的使用帮助。
     """
-    print("如果需要帮助，可以给我发邮件: zhouqiling.bjfu@foxmail.com")
-    print("也可以描述你的需求，给pydatawork提一个功能建议：\npydatawork功能建议收集表：https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ")
+    print("\nHi, 感谢你使用pydatawork～")    
+    print("\n1.pydatawork的官方文档中提供了函数说明和一些示例，或许对你有用。\npydatawork官方文档：https://pypi.org/project/pydatawork/")
+    print("\n2.如果你有好的想法或建议，欢迎给我反馈。\n我的邮箱是: zhouqiling.bjfu@foxmail.com")
+    print("\n3.也可以描述你的需求，给pydatawork提出功能建议。\npydatawork功能建议收集表：https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ")
+    print("\n")
 
 
 
 
 
 
 # Basic Functions
@@ -244,14 +249,15 @@
     """
     功能：输入一个路径，返回当前文件夹名。
 
     参数：
 
     path：一个路径，可以是文件夹路径，也可以是文件路径。
     """
+
     # 判断路径是文件夹路径还是文件路径
     if os.path.isdir(path):
         # 如果是文件夹路径
         current_folder_name = os.path.basename(path)
     else:
         # 如果是文件路径
         current_folder_name = os.path.basename(os.path.dirname(path))
@@ -264,14 +270,15 @@
     """
     功能：输入一个路径，返回文件名。（当path为文件夹路径，返回的值为空值。）
 
     参数：
 
     path：一个路径，可以是文件夹路径，也可以是文件路径。
     """
+
     # 判断路径是文件夹路径还是文件路径
     if os.path.isdir(path):
         # 如果是文件夹路径
         file_name = None
     else:
         # 如果是文件路径
         file_name = os.path.basename(path)
@@ -861,14 +868,15 @@
 
     height：身高（m）（注意，单位为米）。
 
     weight：体重（kg）（注意，单位为千克）。
 
     调用示例：dw.get_BMI(height=1.75,weight=73)。
     """
+
     # height = float(input("输入身高（米）："))
     # weight = float(input("输入体重（千克）："))
 
     height = float(height) 
     weight = float(weight)
     bmi = weight / (height * height)  #计算BMI指数
     suggested_weight_lower =  (height * height) * 18.5
```

### Comparing `pydatawork-0.17.3.0/setup.py` & `pydatawork-0.17.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.3.0',
+    version='0.17.3.1',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

