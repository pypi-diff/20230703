# Comparing `tmp/nb_log-9.1.tar.gz` & `tmp/nb_log-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_log-9.1.tar", last modified: Sun Jul  2 10:34:52 2023, max compression
+gzip compressed data, was "dist\nb_log-9.2.tar", last modified: Mon Jul  3 06:49:24 2023, max compression
```

## Comparing `nb_log-9.1.tar` & `nb_log-9.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 10:34:52.572448 nb_log-9.1/
--rw-rw-rw-   0        0        0    27859 2023-07-02 10:34:52.570445 nb_log-9.1/PKG-INFO
--rw-rw-rw-   0        0        0    26926 2023-05-13 11:59:47.000000 nb_log-9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 10:34:52.549441 nb_log-9.1/nb_log/
--rw-rw-rw-   0        0        0     3192 2023-07-02 07:24:38.000000 nb_log-9.1/nb_log/__init__.py
--rw-rw-rw-   0        0        0     2679 2023-07-02 10:25:39.000000 nb_log-9.1/nb_log/file_write.py
--rw-rw-rw-   0        0        0    50691 2023-06-24 02:46:57.000000 nb_log-9.1/nb_log/handlers.py
--rw-rw-rw-   0        0        0    49868 2022-09-12 12:13:59.000000 nb_log-9.1/nb_log/handlers0000.py
--rw-rw-rw-   0        0        0    30839 2023-06-30 14:23:45.000000 nb_log-9.1/nb_log/log_manager.py
--rw-rw-rw-   0        0        0     6409 2023-07-02 07:15:56.000000 nb_log-9.1/nb_log/monkey_print.py
--rw-rw-rw-   0        0        0      853 2023-07-01 05:26:36.000000 nb_log-9.1/nb_log/monkey_std_filter_words.py
--rw-rw-rw-   0        0        0      819 2023-07-02 07:15:56.000000 nb_log-9.1/nb_log/monkey_sys_std.py
--rw-rw-rw-   0        0        0    10520 2023-07-02 08:12:50.000000 nb_log-9.1/nb_log/nb_log_config_default.py
--rw-rw-rw-   0        0        0     4328 2023-06-30 14:23:45.000000 nb_log-9.1/nb_log/nb_logger.py
--rw-rw-rw-   0        0        0     7710 2023-06-24 02:46:57.000000 nb_log-9.1/nb_log/set_nb_log_config.py
-drwxrwxrwx   0        0        0        0 2023-07-02 10:34:52.567445 nb_log-9.1/nb_log.egg-info/
--rw-rw-rw-   0        0        0    27859 2023-07-02 10:34:52.000000 nb_log-9.1/nb_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-07-02 10:34:52.000000 nb_log-9.1/nb_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 10:34:52.000000 nb_log-9.1/nb_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      210 2023-07-02 10:34:52.000000 nb_log-9.1/nb_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-02 10:34:52.000000 nb_log-9.1/nb_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 10:34:52.573446 nb_log-9.1/setup.cfg
--rw-rw-rw-   0        0        0     2376 2023-07-02 10:34:49.000000 nb_log-9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:49:24.000000 nb_log-9.2/
+-rw-rw-rw-   0        0        0    30397 2023-07-03 06:49:24.000000 nb_log-9.2/PKG-INFO
+-rw-rw-rw-   0        0        0    29460 2023-07-03 03:00:00.000000 nb_log-9.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 06:49:24.000000 nb_log-9.2/nb_log/
+-rw-rw-rw-   0        0        0     3192 2023-07-03 02:35:14.000000 nb_log-9.2/nb_log/__init__.py
+-rw-rw-rw-   0        0        0     2838 2023-07-03 06:48:38.000000 nb_log-9.2/nb_log/file_write.py
+-rw-rw-rw-   0        0        0    50691 2023-04-28 10:26:55.000000 nb_log-9.2/nb_log/handlers.py
+-rw-rw-rw-   0        0        0    49868 2022-09-17 07:28:19.000000 nb_log-9.2/nb_log/handlers0000.py
+-rw-rw-rw-   0        0        0    30839 2023-06-29 11:11:21.000000 nb_log-9.2/nb_log/log_manager.py
+-rw-rw-rw-   0        0        0     6409 2023-07-03 02:35:14.000000 nb_log-9.2/nb_log/monkey_print.py
+-rw-rw-rw-   0        0        0      853 2023-07-03 02:35:14.000000 nb_log-9.2/nb_log/monkey_std_filter_words.py
+-rw-rw-rw-   0        0        0      819 2023-07-03 02:35:14.000000 nb_log-9.2/nb_log/monkey_sys_std.py
+-rw-rw-rw-   0        0        0    10515 2023-07-03 03:00:00.000000 nb_log-9.2/nb_log/nb_log_config_default.py
+-rw-rw-rw-   0        0        0     4328 2023-06-30 01:44:40.000000 nb_log-9.2/nb_log/nb_logger.py
+-rw-rw-rw-   0        0        0     7710 2023-04-13 09:47:00.000000 nb_log-9.2/nb_log/set_nb_log_config.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:49:24.000000 nb_log-9.2/nb_log.egg-info/
+-rw-rw-rw-   0        0        0    30397 2023-07-03 06:49:23.000000 nb_log-9.2/nb_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-07-03 06:49:23.000000 nb_log-9.2/nb_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 06:49:23.000000 nb_log-9.2/nb_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-07-03 06:49:23.000000 nb_log-9.2/nb_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-03 06:49:23.000000 nb_log-9.2/nb_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 06:49:24.000000 nb_log-9.2/setup.cfg
+-rw-rw-rw-   0        0        0     2376 2023-07-03 06:49:18.000000 nb_log-9.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `nb_log-9.1/PKG-INFO` & `nb_log-9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_log
-Version: 9.1
+Version: 9.2
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -39,14 +39,22 @@
 
 
 
 ## 1.0 nb_log 安装
 
 pip install nb_log
 
+## 1.0.1 nb_log不仅是日志，还对print以及sys.stdout(sys.stderr) 打了强力的猴子补丁
+
+对代码里面的print打了猴子补丁，自动显示print所在地方的文件名和精确行号，不怕有人胡乱print，找不到在哪里print的了。
+
+对代码里面的 print 以及 streamHanlder日志调用的sys.stdout/stderr 打了猴子补丁，能支持所有标准输出自动写入到文件中,每天生成一个文件。
+(见1.1.d配置文件说明的 SYS_STD_FILE_NAME 和 PRINT_WRTIE_FILE_NAME)。
+
+
 ## 1.1 nb_log 简单使用例子
 
 ```python
 print('导入nb_log之前的print是普通的')
 
 from nb_log import get_logger
 
@@ -114,14 +122,23 @@
 
 [pythonpath作用介绍的文章](https://github.com/ydf0509/pythonpathdemo)
 
 
 ### 1.1.d nb_log配置文件的一些参数说明。
 
 ```doctest
+
+# 项目中的print是否自动写入到文件中。值为None则不重定向print到文件中。 自动每天一个文件， 2023-06-30.my_proj.print,生成的文件位置在定义的LOG_PATH
+# 如果你设置了环境变量，export PRINT_WRTIE_FILE_NAME="my_proj.print" (linux临时环境变量语法，windows语法自己百度这里不举例),那就优先使用环境变量中设置的文件名字，而不是nb_log_config.py中设置的名字
+PRINT_WRTIE_FILE_NAME = Path(sys.path[1]).name + '.print' 
+
+# 项目中的所有标准输出（不仅包括print，还包括了streamHandler日志）都写入到这个文件。自动每天一个文件， 2023-06-30.my_proj.std,生成的文件位置在定义的LOG_PATH
+# 如果你设置了环境变量，export SYS_STD_FILE_NAME="my_proj.std"  (linux临时环境变量语法，windows语法自己百度这里不举例),那就优先使用环境变量中设置的文件名字，，而不是nb_log_config.py中设置的名字
+SYS_STD_FILE_NAME = Path(sys.path[1]).name + '.std'   
+
 DEFAULUT_USE_COLOR_HANDLER = True  # 是否默认使用有彩的日志。
 DISPLAY_BACKGROUD_COLOR_IN_CONSOLE = True  # 在控制台是否显示彩色块状的日志。为False则不使用大块的背景颜色。
 AUTO_PATCH_PRINT = True  # 是否自动打print的猴子补丁，如果打了猴子补丁，print自动变色和可点击跳转。
 SHOW_PYCHARM_COLOR_SETINGS = True  # 有的人很反感启动代码时候提示教你怎么优化pycahrm控制台颜色，可以把这里设置为False
 
 DEFAULT_ADD_MULTIPROCESSING_SAFE_ROATING_FILE_HANDLER = False  # 是否默认同时将日志记录到记log文件记事本中，就是用户不指定 log_filename的值，会自动写入日志命名空间.log文件中。
 LOG_FILE_SIZE = 100  # 单位是M,每个文件的切片大小，超过多少后就自动切割
@@ -139,14 +156,16 @@
 1为使用多进程安全按日志文件大小切割的文件日志,这是本人实现的批量写入日志，减少操作文件锁次数，测试10进程快速写入文件，win上性能比第5种提高了100倍，linux提升5倍
 2为多进程安全按天自动切割的文件日志，同一个文件，每天生成一个新的日志文件。日志文件名字后缀自动加上日期。
 3为不自动切割的单个文件的日志(不切割文件就不会出现所谓进程安不安全的问题) 
 4为 WatchedFileHandler，这个是需要在linux下才能使用，需要借助lograte外力进行日志文件的切割，多进程安全。
 5 为第三方的concurrent_log_handler.ConcurrentRotatingFileHandler按日志文件大小切割的文件日志，
    这个是采用了文件锁，多进程安全切割，文件锁在linux上使用fcntl性能还行，win上使用win32con性能非常惨。按大小切割建议不要选第5个个filehandler而是选择第1个。
 """
+
+FILTER_WORDS_PRINT = []  # 例如， 你希望消息中包括阿弥陀佛 或者 包括善哉善哉 就不打印，那么可以设置  FILTER_WORDS_PRINT = ['阿弥陀佛','善哉善哉']
 ```
 
 以上只是部分配置的例子，其他配置在你项目根目录下的 nb_log_config.py中都有默认值，自己按需修改设置。
 其他例如日志模板定义，默认日志模板选择什么，都可以在 nb_log_config.py文件中设置。
 
 
 ### 1.1.1e  日志配置文件和get_logger传参的关系。
@@ -479,23 +498,38 @@
 
 print('logger1 id: ',id(logger1),'logger2 id: ',id(logger2),'logger3 id: ',id(logger3))
 ```
 
 运行上面可以发现 logger1和logger2对象是同一个id，logger3对象是另外一个id。
 通过不同的日志命名空间，可以设置不同级别的日志显示，设置不同类型的日志记录到不同的文件，是否打印控制台，是否发送邮件 钉钉消息。
 
+<pre style="font-size: large;color: #FFFF66;background-color: #0c1119">
 有的人到现在还是不知道日志命名空间的作用，对一个大项目的所有的日志只会处理成一种表现行为，悲了个剧。
+如果有人说某部分的日志打印啰嗦了，会说把日志级别调高，这是很外行的说法，请问你如何调高日志级别？有的人不懂日志命名空间，那是完全无法调日志界别，
+比如1.9中的代码，有的笨瓜把 logger3的 logger3.s
+
+你把日志界别调高了，另一个模块或类或函数里面的日志你希望需要显示debug日志呢，
+你只是要屏蔽某些debug日志，
+</pre>
 
 
 ## 1.10 nb_log比logurur有10胜
 
 [nb_log比logurur有10个优点方面](https://nb-log-doc.readthedocs.io/zh_CN/latest/articles/c6.html)
 
+## 1.11 关于nb_log日志级别设置，看文档9.5 章节。
+
+要精通python logging.getLogger第一个入参意义，非常非常重要。
+
+[关于nb_log日志级别设置](https://nb-log-doc.readthedocs.io/zh_CN/latest/articles/c9.html#id2)
+
 ## 1.20 完整readthedocs文档地址
 
 [nb_log readthedocs文档链接](https://nb-log-doc.readthedocs.io/zh_CN/latest)
 
 [nb_log 源码链接](https://github.com/ydf0509/nb_log)
 
 ![](https://visitor-badge.glitch.me/badge?page_id=nb_log)
 
 <div> </div>
+
+
```

### Comparing `nb_log-9.1/README.md` & `nb_log-9.2/nb_log.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: nb-log
+Version: 9.2
+Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
+Home-page: https://github.com/ydf0509/nb_log
+Author: bfzs
+Author-email: ydf0509@sohu.com
+Maintainer: ydf
+Maintainer-email: ydf0509@sohu.com
+License: BSD License
+Keywords: logging,logger,multiprocess file handler,color handler
+Platform: all
+Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: Implementation
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development :: Libraries
+Description-Content-Type: text/markdown
+
 
 # 1.nb_log 简介
 
 [nb_log readthedocs文档链接](https://nb-log-doc.readthedocs.io/zh_CN/latest)
 
 [nb_log 源码链接](https://github.com/ydf0509/nb_log)
 
@@ -17,14 +39,22 @@
 
 
 
 ## 1.0 nb_log 安装
 
 pip install nb_log
 
+## 1.0.1 nb_log不仅是日志，还对print以及sys.stdout(sys.stderr) 打了强力的猴子补丁
+
+对代码里面的print打了猴子补丁，自动显示print所在地方的文件名和精确行号，不怕有人胡乱print，找不到在哪里print的了。
+
+对代码里面的 print 以及 streamHanlder日志调用的sys.stdout/stderr 打了猴子补丁，能支持所有标准输出自动写入到文件中,每天生成一个文件。
+(见1.1.d配置文件说明的 SYS_STD_FILE_NAME 和 PRINT_WRTIE_FILE_NAME)。
+
+
 ## 1.1 nb_log 简单使用例子
 
 ```python
 print('导入nb_log之前的print是普通的')
 
 from nb_log import get_logger
 
@@ -92,14 +122,23 @@
 
 [pythonpath作用介绍的文章](https://github.com/ydf0509/pythonpathdemo)
 
 
 ### 1.1.d nb_log配置文件的一些参数说明。
 
 ```doctest
+
+# 项目中的print是否自动写入到文件中。值为None则不重定向print到文件中。 自动每天一个文件， 2023-06-30.my_proj.print,生成的文件位置在定义的LOG_PATH
+# 如果你设置了环境变量，export PRINT_WRTIE_FILE_NAME="my_proj.print" (linux临时环境变量语法，windows语法自己百度这里不举例),那就优先使用环境变量中设置的文件名字，而不是nb_log_config.py中设置的名字
+PRINT_WRTIE_FILE_NAME = Path(sys.path[1]).name + '.print' 
+
+# 项目中的所有标准输出（不仅包括print，还包括了streamHandler日志）都写入到这个文件。自动每天一个文件， 2023-06-30.my_proj.std,生成的文件位置在定义的LOG_PATH
+# 如果你设置了环境变量，export SYS_STD_FILE_NAME="my_proj.std"  (linux临时环境变量语法，windows语法自己百度这里不举例),那就优先使用环境变量中设置的文件名字，，而不是nb_log_config.py中设置的名字
+SYS_STD_FILE_NAME = Path(sys.path[1]).name + '.std'   
+
 DEFAULUT_USE_COLOR_HANDLER = True  # 是否默认使用有彩的日志。
 DISPLAY_BACKGROUD_COLOR_IN_CONSOLE = True  # 在控制台是否显示彩色块状的日志。为False则不使用大块的背景颜色。
 AUTO_PATCH_PRINT = True  # 是否自动打print的猴子补丁，如果打了猴子补丁，print自动变色和可点击跳转。
 SHOW_PYCHARM_COLOR_SETINGS = True  # 有的人很反感启动代码时候提示教你怎么优化pycahrm控制台颜色，可以把这里设置为False
 
 DEFAULT_ADD_MULTIPROCESSING_SAFE_ROATING_FILE_HANDLER = False  # 是否默认同时将日志记录到记log文件记事本中，就是用户不指定 log_filename的值，会自动写入日志命名空间.log文件中。
 LOG_FILE_SIZE = 100  # 单位是M,每个文件的切片大小，超过多少后就自动切割
@@ -117,14 +156,16 @@
 1为使用多进程安全按日志文件大小切割的文件日志,这是本人实现的批量写入日志，减少操作文件锁次数，测试10进程快速写入文件，win上性能比第5种提高了100倍，linux提升5倍
 2为多进程安全按天自动切割的文件日志，同一个文件，每天生成一个新的日志文件。日志文件名字后缀自动加上日期。
 3为不自动切割的单个文件的日志(不切割文件就不会出现所谓进程安不安全的问题) 
 4为 WatchedFileHandler，这个是需要在linux下才能使用，需要借助lograte外力进行日志文件的切割，多进程安全。
 5 为第三方的concurrent_log_handler.ConcurrentRotatingFileHandler按日志文件大小切割的文件日志，
    这个是采用了文件锁，多进程安全切割，文件锁在linux上使用fcntl性能还行，win上使用win32con性能非常惨。按大小切割建议不要选第5个个filehandler而是选择第1个。
 """
+
+FILTER_WORDS_PRINT = []  # 例如， 你希望消息中包括阿弥陀佛 或者 包括善哉善哉 就不打印，那么可以设置  FILTER_WORDS_PRINT = ['阿弥陀佛','善哉善哉']
 ```
 
 以上只是部分配置的例子，其他配置在你项目根目录下的 nb_log_config.py中都有默认值，自己按需修改设置。
 其他例如日志模板定义，默认日志模板选择什么，都可以在 nb_log_config.py文件中设置。
 
 
 ### 1.1.1e  日志配置文件和get_logger传参的关系。
@@ -457,23 +498,38 @@
 
 print('logger1 id: ',id(logger1),'logger2 id: ',id(logger2),'logger3 id: ',id(logger3))
 ```
 
 运行上面可以发现 logger1和logger2对象是同一个id，logger3对象是另外一个id。
 通过不同的日志命名空间，可以设置不同级别的日志显示，设置不同类型的日志记录到不同的文件，是否打印控制台，是否发送邮件 钉钉消息。
 
+<pre style="font-size: large;color: #FFFF66;background-color: #0c1119">
 有的人到现在还是不知道日志命名空间的作用，对一个大项目的所有的日志只会处理成一种表现行为，悲了个剧。
+如果有人说某部分的日志打印啰嗦了，会说把日志级别调高，这是很外行的说法，请问你如何调高日志级别？有的人不懂日志命名空间，那是完全无法调日志界别，
+比如1.9中的代码，有的笨瓜把 logger3的 logger3.s
+
+你把日志界别调高了，另一个模块或类或函数里面的日志你希望需要显示debug日志呢，
+你只是要屏蔽某些debug日志，
+</pre>
 
 
 ## 1.10 nb_log比logurur有10胜
 
 [nb_log比logurur有10个优点方面](https://nb-log-doc.readthedocs.io/zh_CN/latest/articles/c6.html)
 
+## 1.11 关于nb_log日志级别设置，看文档9.5 章节。
+
+要精通python logging.getLogger第一个入参意义，非常非常重要。
+
+[关于nb_log日志级别设置](https://nb-log-doc.readthedocs.io/zh_CN/latest/articles/c9.html#id2)
+
 ## 1.20 完整readthedocs文档地址
 
 [nb_log readthedocs文档链接](https://nb-log-doc.readthedocs.io/zh_CN/latest)
 
 [nb_log 源码链接](https://github.com/ydf0509/nb_log)
 
 ![](https://visitor-badge.glitch.me/badge?page_id=nb_log)
 
 <div> </div>
+
+
```

### Comparing `nb_log-9.1/nb_log/__init__.py` & `nb_log-9.2/nb_log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.1/nb_log/file_write.py` & `nb_log-9.2/nb_log/file_write.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,22 +55,28 @@
                 if now_ts - self._last_del_old_files_ts > 300:
                     self._last_del_old_files_ts = time.time()
                     self._delete_old_files()
 
     def _delete_old_files(self):
         for i in range(10, 100):
             file_path = Path(nb_log_config_default.LOG_PATH) / Path(DatetimeConverter(time.time() - 86400 * i).date_str + '.' + self._file_name)
-            file_path.unlink(missing_ok=True)
+            try:
+                file_path.unlink()  # 低版本python 没有missing_ok入参。
+            except FileNotFoundError:
+                pass
 
 
 class PrintFileWritter(FileWritter):
     _lock = threading.Lock()
     need_write_2_file = False if nb_log_config_default.PRINT_WRTIE_FILE_NAME in (None, '') else True
 
 
 class StdFileWritter(FileWritter):
     _lock = threading.Lock()
     need_write_2_file = False if nb_log_config_default.SYS_STD_FILE_NAME in (None, '') else True
 
 
+
 if __name__ == '__main__':
-    FileWritter(nb_log_config_default.PRINT_WRTIE_FILE_NAME).write_2_file('哈哈哈')
+    fw = StdFileWritter(nb_log_config_default.PRINT_WRTIE_FILE_NAME)
+    fw.write_2_file('哈哈哈')
+    fw._delete_old_files()
```

### Comparing `nb_log-9.1/nb_log/handlers.py` & `nb_log-9.2/nb_log/handlers.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.1/nb_log/handlers0000.py` & `nb_log-9.2/nb_log/handlers0000.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.1/nb_log/log_manager.py` & `nb_log-9.2/nb_log/log_manager.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.1/nb_log/monkey_print.py` & `nb_log-9.2/nb_log/monkey_print.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.1/nb_log/monkey_std_filter_words.py` & `nb_log-9.2/nb_log/monkey_std_filter_words.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.1/nb_log/monkey_sys_std.py` & `nb_log-9.2/nb_log/monkey_sys_std.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.1/nb_log/nb_log_config_default.py` & `nb_log-9.2/nb_log/nb_log_config_default.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 ELASTIC_PORT = 9200
 
 KAFKA_BOOTSTRAP_SERVERS = ['192.168.199.202:9092']
 ALWAYS_ADD_KAFKA_HANDLER_IN_TEST_ENVIRONENT = False
 
 MONGO_URL = 'mongodb://myUserAdmin:mimamiama@127.0.0.1:27016/admin'
 
-# 项目中的print是否自动写入到文件中。值为None则不重定向标准输出到文件中。 自动每天一个文件， 2023-06-30.my_proj.out,生成的文件位置在定义的LOG_PATH
+# 项目中的print是否自动写入到文件中。值为None则不重定向print到文件中。 自动每天一个文件， 2023-06-30.my_proj.print,生成的文件位置在定义的LOG_PATH
 # 如果你设置了环境变量，export PRINT_WRTIE_FILE_NAME="my_proj.print" (linux临时环境变量语法，windows语法自己百度这里不举例),那就优先使用环境变量中设置的文件名字，而不是nb_log_config.py中设置的名字
 PRINT_WRTIE_FILE_NAME = Path(sys.path[1]).name + '.print'
 
 # 项目中的所有标准输出（不仅包括print，还包括了streamHandler日志）都写入到这个文件。自动每天一个文件， 2023-06-30.my_proj.std,生成的文件位置在定义的LOG_PATH
 # 如果你设置了环境变量，export SYS_STD_FILE_NAME="my_proj.std"  (linux临时环境变量语法，windows语法自己百度这里不举例),那就优先使用环境变量中设置的文件名字，，而不是nb_log_config.py中设置的名字
 SYS_STD_FILE_NAME = Path(sys.path[1]).name + '.std'
```

### Comparing `nb_log-9.1/nb_log/nb_logger.py` & `nb_log-9.2/nb_log/nb_logger.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.1/nb_log/set_nb_log_config.py` & `nb_log-9.2/nb_log/set_nb_log_config.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.1/nb_log.egg-info/PKG-INFO` & `nb_log-9.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: nb-log
-Version: 9.1
-Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
-Home-page: https://github.com/ydf0509/nb_log
-Author: bfzs
-Author-email: ydf0509@sohu.com
-Maintainer: ydf
-Maintainer-email: ydf0509@sohu.com
-License: BSD License
-Keywords: logging,logger,multiprocess file handler,color handler
-Platform: all
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries
-Description-Content-Type: text/markdown
-
 
 # 1.nb_log 简介
 
 [nb_log readthedocs文档链接](https://nb-log-doc.readthedocs.io/zh_CN/latest)
 
 [nb_log 源码链接](https://github.com/ydf0509/nb_log)
 
@@ -39,14 +17,22 @@
 
 
 
 ## 1.0 nb_log 安装
 
 pip install nb_log
 
+## 1.0.1 nb_log不仅是日志，还对print以及sys.stdout(sys.stderr) 打了强力的猴子补丁
+
+对代码里面的print打了猴子补丁，自动显示print所在地方的文件名和精确行号，不怕有人胡乱print，找不到在哪里print的了。
+
+对代码里面的 print 以及 streamHanlder日志调用的sys.stdout/stderr 打了猴子补丁，能支持所有标准输出自动写入到文件中,每天生成一个文件。
+(见1.1.d配置文件说明的 SYS_STD_FILE_NAME 和 PRINT_WRTIE_FILE_NAME)。
+
+
 ## 1.1 nb_log 简单使用例子
 
 ```python
 print('导入nb_log之前的print是普通的')
 
 from nb_log import get_logger
 
@@ -114,14 +100,23 @@
 
 [pythonpath作用介绍的文章](https://github.com/ydf0509/pythonpathdemo)
 
 
 ### 1.1.d nb_log配置文件的一些参数说明。
 
 ```doctest
+
+# 项目中的print是否自动写入到文件中。值为None则不重定向print到文件中。 自动每天一个文件， 2023-06-30.my_proj.print,生成的文件位置在定义的LOG_PATH
+# 如果你设置了环境变量，export PRINT_WRTIE_FILE_NAME="my_proj.print" (linux临时环境变量语法，windows语法自己百度这里不举例),那就优先使用环境变量中设置的文件名字，而不是nb_log_config.py中设置的名字
+PRINT_WRTIE_FILE_NAME = Path(sys.path[1]).name + '.print' 
+
+# 项目中的所有标准输出（不仅包括print，还包括了streamHandler日志）都写入到这个文件。自动每天一个文件， 2023-06-30.my_proj.std,生成的文件位置在定义的LOG_PATH
+# 如果你设置了环境变量，export SYS_STD_FILE_NAME="my_proj.std"  (linux临时环境变量语法，windows语法自己百度这里不举例),那就优先使用环境变量中设置的文件名字，，而不是nb_log_config.py中设置的名字
+SYS_STD_FILE_NAME = Path(sys.path[1]).name + '.std'   
+
 DEFAULUT_USE_COLOR_HANDLER = True  # 是否默认使用有彩的日志。
 DISPLAY_BACKGROUD_COLOR_IN_CONSOLE = True  # 在控制台是否显示彩色块状的日志。为False则不使用大块的背景颜色。
 AUTO_PATCH_PRINT = True  # 是否自动打print的猴子补丁，如果打了猴子补丁，print自动变色和可点击跳转。
 SHOW_PYCHARM_COLOR_SETINGS = True  # 有的人很反感启动代码时候提示教你怎么优化pycahrm控制台颜色，可以把这里设置为False
 
 DEFAULT_ADD_MULTIPROCESSING_SAFE_ROATING_FILE_HANDLER = False  # 是否默认同时将日志记录到记log文件记事本中，就是用户不指定 log_filename的值，会自动写入日志命名空间.log文件中。
 LOG_FILE_SIZE = 100  # 单位是M,每个文件的切片大小，超过多少后就自动切割
@@ -139,14 +134,16 @@
 1为使用多进程安全按日志文件大小切割的文件日志,这是本人实现的批量写入日志，减少操作文件锁次数，测试10进程快速写入文件，win上性能比第5种提高了100倍，linux提升5倍
 2为多进程安全按天自动切割的文件日志，同一个文件，每天生成一个新的日志文件。日志文件名字后缀自动加上日期。
 3为不自动切割的单个文件的日志(不切割文件就不会出现所谓进程安不安全的问题) 
 4为 WatchedFileHandler，这个是需要在linux下才能使用，需要借助lograte外力进行日志文件的切割，多进程安全。
 5 为第三方的concurrent_log_handler.ConcurrentRotatingFileHandler按日志文件大小切割的文件日志，
    这个是采用了文件锁，多进程安全切割，文件锁在linux上使用fcntl性能还行，win上使用win32con性能非常惨。按大小切割建议不要选第5个个filehandler而是选择第1个。
 """
+
+FILTER_WORDS_PRINT = []  # 例如， 你希望消息中包括阿弥陀佛 或者 包括善哉善哉 就不打印，那么可以设置  FILTER_WORDS_PRINT = ['阿弥陀佛','善哉善哉']
 ```
 
 以上只是部分配置的例子，其他配置在你项目根目录下的 nb_log_config.py中都有默认值，自己按需修改设置。
 其他例如日志模板定义，默认日志模板选择什么，都可以在 nb_log_config.py文件中设置。
 
 
 ### 1.1.1e  日志配置文件和get_logger传参的关系。
@@ -479,21 +476,34 @@
 
 print('logger1 id: ',id(logger1),'logger2 id: ',id(logger2),'logger3 id: ',id(logger3))
 ```
 
 运行上面可以发现 logger1和logger2对象是同一个id，logger3对象是另外一个id。
 通过不同的日志命名空间，可以设置不同级别的日志显示，设置不同类型的日志记录到不同的文件，是否打印控制台，是否发送邮件 钉钉消息。
 
+<pre style="font-size: large;color: #FFFF66;background-color: #0c1119">
 有的人到现在还是不知道日志命名空间的作用，对一个大项目的所有的日志只会处理成一种表现行为，悲了个剧。
+如果有人说某部分的日志打印啰嗦了，会说把日志级别调高，这是很外行的说法，请问你如何调高日志级别？有的人不懂日志命名空间，那是完全无法调日志界别，
+比如1.9中的代码，有的笨瓜把 logger3的 logger3.s
+
+你把日志界别调高了，另一个模块或类或函数里面的日志你希望需要显示debug日志呢，
+你只是要屏蔽某些debug日志，
+</pre>
 
 
 ## 1.10 nb_log比logurur有10胜
 
 [nb_log比logurur有10个优点方面](https://nb-log-doc.readthedocs.io/zh_CN/latest/articles/c6.html)
 
+## 1.11 关于nb_log日志级别设置，看文档9.5 章节。
+
+要精通python logging.getLogger第一个入参意义，非常非常重要。
+
+[关于nb_log日志级别设置](https://nb-log-doc.readthedocs.io/zh_CN/latest/articles/c9.html#id2)
+
 ## 1.20 完整readthedocs文档地址
 
 [nb_log readthedocs文档链接](https://nb-log-doc.readthedocs.io/zh_CN/latest)
 
 [nb_log 源码链接](https://github.com/ydf0509/nb_log)
 
 ![](https://visitor-badge.glitch.me/badge?page_id=nb_log)
```

### Comparing `nb_log-9.1/setup.py` & `nb_log-9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ]
 
 if os.name == 'nt':
     install_requires.append('pywin32')
 
 setup(
     name='nb_log',  #
-    version="9.1",
+    version="9.2",
     description=(
         'very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on '
     ),
     keywords=["logging", "logger", "multiprocess file handler", "color handler"],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
@@ -63,14 +63,14 @@
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
 
 python setup.py sdist & twine upload dist/nb_log-6.0.tar.gz
-python setup.py sdist & python -m  twine upload dist/nb_log-9.1.tar.gz
+python setup.py sdist & python -m  twine upload dist/nb_log-9.2.tar.gz
 
 twine upload dist/*
 
 
 python -m pip install nb_log --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```

