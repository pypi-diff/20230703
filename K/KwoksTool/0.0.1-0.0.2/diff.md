# Comparing `tmp/KwoksTool-0.0.1.tar.gz` & `tmp/KwoksTool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KwoksTool-0.0.1.tar", last modified: Mon Jul  3 08:14:25 2023, max compression
+gzip compressed data, was "KwoksTool-0.0.2.tar", last modified: Mon Jul  3 08:23:23 2023, max compression
```

## Comparing `KwoksTool-0.0.1.tar` & `KwoksTool-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 08:14:25.196029 KwoksTool-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-03 08:14:25.180435 KwoksTool-0.0.1/KwoksTool/
--rw-rw-rw-   0        0        0     1069 2023-07-03 07:58:24.000000 KwoksTool-0.0.1/KwoksTool/__init__.py
--rw-rw-rw-   0        0        0       22 2023-07-03 08:11:10.000000 KwoksTool-0.0.1/KwoksTool/_version.py
--rw-rw-rw-   0        0        0    15838 2023-07-03 07:54:38.000000 KwoksTool-0.0.1/KwoksTool/function.py
--rw-rw-rw-   0        0        0      122 2023-07-03 07:43:06.000000 KwoksTool-0.0.1/KwoksTool/info.py
--rw-rw-rw-   0        0        0     1806 2023-07-03 07:56:39.000000 KwoksTool-0.0.1/KwoksTool/model.py
--rw-rw-rw-   0        0        0      734 2023-07-03 07:50:23.000000 KwoksTool-0.0.1/KwoksTool/spider.py
-drwxrwxrwx   0        0        0        0 2023-07-03 08:14:25.196029 KwoksTool-0.0.1/KwoksTool.egg-info/
--rw-rw-rw-   0        0        0       56 2023-07-03 08:14:25.000000 KwoksTool-0.0.1/KwoksTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-07-03 08:14:25.000000 KwoksTool-0.0.1/KwoksTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 08:14:25.000000 KwoksTool-0.0.1/KwoksTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-03 08:14:25.000000 KwoksTool-0.0.1/KwoksTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-07-03 08:14:25.196029 KwoksTool-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-07-03 08:13:49.000000 KwoksTool-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 08:14:25.196029 KwoksTool-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 08:23:23.181223 KwoksTool-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-03 08:23:23.165601 KwoksTool-0.0.2/KwoksTool/
+-rw-rw-rw-   0        0        0     1069 2023-07-03 08:22:49.000000 KwoksTool-0.0.2/KwoksTool/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-07-03 08:23:08.000000 KwoksTool-0.0.2/KwoksTool/_version.py
+-rw-rw-rw-   0        0        0    15838 2023-07-03 07:54:38.000000 KwoksTool-0.0.2/KwoksTool/function.py
+-rw-rw-rw-   0        0        0      122 2023-07-03 07:43:06.000000 KwoksTool-0.0.2/KwoksTool/info.py
+-rw-rw-rw-   0        0        0     1806 2023-07-03 07:56:39.000000 KwoksTool-0.0.2/KwoksTool/model.py
+-rw-rw-rw-   0        0        0      734 2023-07-03 07:50:23.000000 KwoksTool-0.0.2/KwoksTool/spider.py
+drwxrwxrwx   0        0        0        0 2023-07-03 08:23:23.165601 KwoksTool-0.0.2/KwoksTool.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-07-03 08:23:23.000000 KwoksTool-0.0.2/KwoksTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-07-03 08:23:23.000000 KwoksTool-0.0.2/KwoksTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 08:23:23.000000 KwoksTool-0.0.2/KwoksTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-03 08:23:23.000000 KwoksTool-0.0.2/KwoksTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-07-03 08:23:23.181223 KwoksTool-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-07-03 08:23:02.000000 KwoksTool-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 08:23:23.181223 KwoksTool-0.0.2/setup.cfg
```

### Comparing `KwoksTool-0.0.1/KwoksTool/__init__.py` & `KwoksTool-0.0.2/KwoksTool/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
-from KwoksNote.info import (welcome,how)
-from KwoksNote.spider import (Browser)
-from KwoksNote.function import (GetCityNumFromLiepin,
+from KwoksTool.info import (welcome,how)
+from KwoksTool.spider import (Browser)
+from KwoksTool.function import (GetCityNumFromLiepin,
                                 GetIpPool,
                                 GetCityNumFromBossZhiPing,
                                 GetCityNameFromLiepin,
                                 YesOrNot,
                                 CheckIp,
                                 IntoZip,
                                 ZipOut,
                                 SendEmail,
                                 GetEmail,
                                 ProgressBar,
                                 GetPlateSon,
                                 GetPlateInfo,
                                 MergeTable,
                                 ChoiceColumn)
-from KwoksNote.model import (GetProbMatrix,ToMat)
+from KwoksTool.model import (GetProbMatrix,ToMat)
 if not os.path.exists(
         r'C:\Windows\AgentPool.xlsx'):
     print('注意注意！\n请确保存在\'C:\Windows\AgentPool.xlsx\'的ip代理文件\n否则，ip池功能将无法使用\n继续使用请敲击回车键')
```

### Comparing `KwoksTool-0.0.1/KwoksTool/function.py` & `KwoksTool-0.0.2/KwoksTool/function.py`

 * *Files identical despite different names*

### Comparing `KwoksTool-0.0.1/KwoksTool/model.py` & `KwoksTool-0.0.2/KwoksTool/model.py`

 * *Files identical despite different names*

### Comparing `KwoksTool-0.0.1/KwoksTool/spider.py` & `KwoksTool-0.0.2/KwoksTool/spider.py`

 * *Files identical despite different names*

