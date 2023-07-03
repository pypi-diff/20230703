# Comparing `tmp/pydatawork-0.17.3.2.tar.gz` & `tmp/pydatawork-0.17.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.3.2.tar", last modified: Mon Jul  3 14:13:25 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.3.3.tar", last modified: Mon Jul  3 21:13:53 2023, max compression
```

## Comparing `pydatawork-0.17.3.2.tar` & `pydatawork-0.17.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    18739 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    14084 2023-07-03 14:12:21.000000 pydatawork-0.17.3.2/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    18739 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    39093 2023-07-03 14:05:45.000000 pydatawork-0.17.3.2/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-03 14:13:25.000000 pydatawork-0.17.3.2/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-03 14:13:06.000000 pydatawork-0.17.3.2/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 21:13:53.000000 pydatawork-0.17.3.3/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    18739 2023-07-03 21:13:53.000000 pydatawork-0.17.3.3/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    14084 2023-07-03 14:12:21.000000 pydatawork-0.17.3.3/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-03 21:13:53.000000 pydatawork-0.17.3.3/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    18739 2023-07-03 21:13:53.000000 pydatawork-0.17.3.3/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-03 21:13:53.000000 pydatawork-0.17.3.3/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-03 21:13:53.000000 pydatawork-0.17.3.3/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-03 21:13:53.000000 pydatawork-0.17.3.3/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    43448 2023-07-03 21:13:29.000000 pydatawork-0.17.3.3/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-03 21:13:53.000000 pydatawork-0.17.3.3/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-03 21:12:47.000000 pydatawork-0.17.3.3/setup.py
```

### Comparing `pydatawork-0.17.3.2/PKG-INFO` & `pydatawork-0.17.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.3.2
+Version: 0.17.3.3
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
```

### Comparing `pydatawork-0.17.3.2/README.md` & `pydatawork-0.17.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pydatawork-0.17.3.2/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.3.3/pydatawork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.3.2
+Version: 0.17.3.3
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
```

### Comparing `pydatawork-0.17.3.2/pydatawork.py` & `pydatawork-0.17.3.3/pydatawork.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,23 +56,117 @@
 # 维护
 
 # 折叠：ctrl + k , ctrl + 1
 # 展开：ctrl + k , ctrl + j
 
 
 # get help
-def hello_jkzhou():
-    """
-    功能：获取pydatawork的使用帮助。
-    """
-    print("\nHi, 感谢你使用pydatawork～")    
-    print("\n1.pydatawork的官方文档中提供了函数说明和一些示例，或许对你有用。\npydatawork官方文档：https://pypi.org/project/pydatawork/")
-    print("\n2.如果你有好的想法或建议，欢迎给我反馈。\n我的邮箱是: zhouqiling.bjfu@foxmail.com")
-    print("\n3.也可以描述你的需求，给pydatawork提出功能建议。\npydatawork功能建议收集表：https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ")
-    print("\n")
+# def hello_jkzhou():
+#     """
+#     功能：获取pydatawork的使用帮助。
+#     """
+#     print("\nHi, 感谢你使用pydatawork～")    
+#     print("\n1.pydatawork的官方文档中提供了函数说明和一些示例，或许对你有用。\npydatawork官方文档：https://pypi.org/project/pydatawork/")
+#     print("\n2.如果你有好的想法或建议，欢迎给我反馈。\n我的邮箱是: zhouqiling.bjfu@foxmail.com")
+#     print("\n3.也可以描述你的需求，给pydatawork提出功能建议。\npydatawork功能建议收集表：https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ")
+#     print("\n")
+
+
+def hello_jkzhou(): # 为什么要定义主函数？ @知识卡片
+    # 先定义需要用到的函数
+    def menu():
+        print("====================pydatawork官方文档====================")
+        print("------------------------功能菜单--------------------------")
+        print("\t\t1.basic functions")
+        print("\t\t2.data processing")
+        print("\t\t3.data analysis")
+        print("\t\t4.查找")
+        print("\t\t5.工作台")
+        print("\t\t6.知识库")
+        print("\t\t7.数据库")
+        print("\t\t8.联系与帮助")
+        print("\t\t0.退出")
+        print("-----------------------------------------------------------")
+
+    def basic_functions():
+        while True:
+            print("""basic functions:
+            file_split
+            get_current_folder_name
+            get_file_name
+            copy_files, copy_all_files, copy_files_by_keyword
+            move_files, move_all_files, move_files_by_keyword
+            renamer_folder_numeric_serialize
+            """)
+            answer = input("输入 n/N 退出，按 回车 继续...\n") # @知识卡片 输入时没有指定input的值的类型，所以，当输入的值为空值时，不会报错。如果指定了int，输入空值就会直接报错，无法进入下一步判断。
+            if answer == "n" or answer == "N": # 仅当输入n/N直接退出。要继续，直接回车就行
+                exit()
+            else:
+                break # @知识卡片 在这里要继续使用，本质上就是退出当前的循环，所以，直接break
+
+    def data_processing():
+        pass
+
+    def data_analysis():
+        pass
+
+    def search():
+        pass
+
+    def workspaces():
+        pass
+
+    def wiki():
+        pass
+
+    def database():
+        pass
+
+    def get_help():
+        print("\nHi, 感谢你使用pydatawork，下面的信息可能对你有用，试试看：")    
+        print("1.pydatawork的官方文档中提供了函数说明和一些示例。\npydatawork官方文档：https://pypi.org/project/pydatawork/")
+        print("2.如果你有好的想法或建议，欢迎给我反馈。\n我的邮箱是: zhouqiling.bjfu@foxmail.com")
+        print("3.也可以描述你的需求，给pydatawork提出功能建议。\npydatawork功能建议收集表：https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ")
+        print("\n")
+
+    while True: # 为什么选择使用while循环。布尔值和while循环用在一起，通常为了实现什么目的。每个对象都有一个布尔值。 @知识卡片
+        menu()
+        try:
+            choice = int(input("请选择：")) 
+            if choice in [0,1,2,3,4,5,6,7,8]: # @知识卡片 注意，这里需要提前指定输入数值的范围，别忘了
+                if choice == 0:
+                    answer=input("确认要退出吗？(y/n)") # 括号里面是提示信息
+                    if answer == "y" or answer == "Y": # 兼顾大小写。不能写成"y" or "Y"，这是错误的写法
+                        print("谢谢使用！")
+                        break # 退出系统。退出循环。
+                    else:
+                        continue
+                elif choice == 1:
+                    basic_functions() # 基本功能函数
+                elif choice == 2:
+                    data_processing() # 数据处理函数
+                elif choice == 3:
+                    data_analysis() # 数据分析函数
+                elif choice == 4:
+                    search() # 函数查询
+                elif choice == 5:
+                    workspaces() # 工作台
+                elif choice == 6: 
+                    wiki() # 知识库             
+                elif choice == 7:
+                    database() # 数据库
+                elif choice == 8:
+                    get_help() # 联系与帮助信息
+            else:
+                print("输入的数值超出范围...") # @知识卡片 注意与对应的模块对齐
+
+        except ValueError:
+            print("输入无效，请重新输入！") # 在选择界面直接回车时，弹出这条，然后重新选择——因为是在无限循环中，所以会直接重新回到 menu()函数，而不用在下方再写一个menu()
+            # menu() # 此处不用再写，因为本身就在无限循环的函数中
+
 
 
 
 
 
 
 # Basic Functions
```

### Comparing `pydatawork-0.17.3.2/setup.py` & `pydatawork-0.17.3.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.3.2',
+    version='0.17.3.3',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

