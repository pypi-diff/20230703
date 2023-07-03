# Comparing `tmp/aomaker-2.3.0.tar.gz` & `tmp/aomaker-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aomaker-2.3.0.tar", last modified: Wed Jun 28 09:22:13 2023, max compression
+gzip compressed data, was "aomaker-2.3.1.tar", last modified: Mon Jul  3 04:51:51 2023, max compression
```

## Comparing `aomaker-2.3.0.tar` & `aomaker-2.3.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-06-28 09:22:13.737813 aomaker-2.3.0/
--rw-r-----   0 zhanglinsen   (501) staff       (20)    11509 2022-11-30 11:05:02.000000 aomaker-2.3.0/LICENSE
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       43 2023-05-20 11:36:28.000000 aomaker-2.3.0/MANIFEST.in
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-06-28 09:22:13.737670 aomaker-2.3.0/PKG-INFO
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      607 2022-11-03 10:41:01.000000 aomaker-2.3.0/README.md
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-06-28 09:22:13.732611 aomaker-2.3.0/aomaker/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1426 2023-06-27 14:54:19.000000 aomaker-2.3.0/aomaker/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9285 2023-04-12 10:30:39.000000 aomaker-2.3.0/aomaker/_aomaker.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      794 2023-04-10 14:08:17.000000 aomaker-2.3.0/aomaker/_constants.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2356 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/_log.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1245 2023-05-20 14:38:18.000000 aomaker-2.3.0/aomaker/_printer.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      237 2023-04-10 15:38:20.000000 aomaker-2.3.0/aomaker/aomaker.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-06-28 09:22:13.733749 aomaker-2.3.0/aomaker/base/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/base/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4395 2023-04-10 14:57:25.000000 aomaker-2.3.0/aomaker/base/base_api.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3296 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/base/base_testcase.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     6139 2023-05-29 14:52:36.000000 aomaker-2.3.0/aomaker/cache.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    11276 2023-06-28 09:19:16.000000 aomaker-2.3.0/aomaker/cli.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-06-28 09:22:13.734479 aomaker-2.3.0/aomaker/database/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/database/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1654 2023-03-24 06:30:20.000000 aomaker-2.3.0/aomaker/database/base_db.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1059 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/database/mysql.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2734 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/database/sqlite.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1685 2023-05-29 14:39:13.000000 aomaker-2.3.0/aomaker/exceptions.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-06-28 09:22:13.734605 aomaker-2.3.0/aomaker/extension/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        0 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/extension/__init__.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-06-28 09:22:13.734890 aomaker-2.3.0/aomaker/extension/har_parse/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2284 2023-03-22 14:18:38.000000 aomaker-2.3.0/aomaker/extension/har_parse/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    10792 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/extension/har_parse/har_parse.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-06-28 09:22:13.735456 aomaker-2.3.0/aomaker/extension/recording/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4517 2023-03-21 15:15:18.000000 aomaker-2.3.0/aomaker/extension/recording/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      170 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/extension/recording/addons.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     5679 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/extension/recording/recording.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1276 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/field.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2813 2023-05-20 14:38:18.000000 aomaker-2.3.0/aomaker/fixture.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      965 2023-03-22 10:18:59.000000 aomaker-2.3.0/aomaker/hook_manager.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-06-28 09:22:13.736116 aomaker-2.3.0/aomaker/html/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9937 2022-12-22 09:57:22.000000 aomaker-2.3.0/aomaker/html/heading.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4302 2022-12-22 09:57:22.000000 aomaker-2.3.0/aomaker/html/report.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    11555 2023-05-20 11:43:25.000000 aomaker-2.3.0/aomaker/html/template.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3816 2023-03-22 11:04:05.000000 aomaker-2.3.0/aomaker/log.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1476 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/make.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     7940 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/make_api.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1216 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/make_testcase.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2288 2023-06-28 07:54:12.000000 aomaker-2.3.0/aomaker/models.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      503 2023-06-13 10:28:50.000000 aomaker-2.3.0/aomaker/param_types.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      750 2023-06-19 04:14:35.000000 aomaker-2.3.0/aomaker/path.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2890 2023-05-20 14:38:18.000000 aomaker-2.3.0/aomaker/report.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8513 2023-06-28 06:57:49.000000 aomaker-2.3.0/aomaker/runner.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8639 2023-06-28 08:23:43.000000 aomaker-2.3.0/aomaker/scaffold.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-06-28 09:22:13.736670 aomaker-2.3.0/aomaker/send_msg/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/send_msg/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8329 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/send_msg/wechat.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     7672 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/swagger2yaml.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9148 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/template.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-06-28 09:22:13.737299 aomaker-2.3.0/aomaker/utils/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/utils/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9529 2023-05-22 08:33:10.000000 aomaker-2.3.0/aomaker/utils/gen_allure_report.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     5120 2023-02-02 04:06:40.000000 aomaker-2.3.0/aomaker/utils/utils.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    16987 2022-11-03 10:41:01.000000 aomaker-2.3.0/aomaker/yaml2case.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-06-28 09:22:13.733247 aomaker-2.3.0/aomaker.egg-info/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-06-28 09:22:13.000000 aomaker-2.3.0/aomaker.egg-info/PKG-INFO
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1349 2023-06-28 09:22:13.000000 aomaker-2.3.0/aomaker.egg-info/SOURCES.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        1 2023-06-28 09:22:13.000000 aomaker-2.3.0/aomaker.egg-info/dependency_links.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      154 2023-06-28 09:22:13.000000 aomaker-2.3.0/aomaker.egg-info/entry_points.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      173 2023-06-28 09:22:13.000000 aomaker-2.3.0/aomaker.egg-info/requires.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        8 2023-06-28 09:22:13.000000 aomaker-2.3.0/aomaker.egg-info/top_level.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       38 2023-06-28 09:22:13.737855 aomaker-2.3.0/setup.cfg
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1282 2023-06-27 14:54:19.000000 aomaker-2.3.0/setup.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-07-03 04:51:51.733001 aomaker-2.3.1/
+-rw-r-----   0 zhanglinsen   (501) staff       (20)    11509 2022-11-30 11:05:02.000000 aomaker-2.3.1/LICENSE
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       43 2023-05-20 11:36:28.000000 aomaker-2.3.1/MANIFEST.in
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-07-03 04:51:51.732864 aomaker-2.3.1/PKG-INFO
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      607 2022-11-03 10:41:01.000000 aomaker-2.3.1/README.md
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-07-03 04:51:51.728240 aomaker-2.3.1/aomaker/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1426 2023-07-03 04:51:29.000000 aomaker-2.3.1/aomaker/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9285 2023-04-12 10:30:39.000000 aomaker-2.3.1/aomaker/_aomaker.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      794 2023-04-10 14:08:17.000000 aomaker-2.3.1/aomaker/_constants.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2356 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/_log.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1245 2023-05-20 14:38:18.000000 aomaker-2.3.1/aomaker/_printer.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      237 2023-04-10 15:38:20.000000 aomaker-2.3.1/aomaker/aomaker.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-07-03 04:51:51.729431 aomaker-2.3.1/aomaker/base/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/base/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4395 2023-04-10 14:57:25.000000 aomaker-2.3.1/aomaker/base/base_api.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3296 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/base/base_testcase.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     6139 2023-05-29 14:52:36.000000 aomaker-2.3.1/aomaker/cache.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    11276 2023-06-28 09:19:16.000000 aomaker-2.3.1/aomaker/cli.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-07-03 04:51:51.730207 aomaker-2.3.1/aomaker/database/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/database/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1654 2023-03-24 06:30:20.000000 aomaker-2.3.1/aomaker/database/base_db.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1059 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/database/mysql.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2734 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/database/sqlite.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1685 2023-05-29 14:39:13.000000 aomaker-2.3.1/aomaker/exceptions.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-07-03 04:51:51.730333 aomaker-2.3.1/aomaker/extension/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        0 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/extension/__init__.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-07-03 04:51:51.730611 aomaker-2.3.1/aomaker/extension/har_parse/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2284 2023-03-22 14:18:38.000000 aomaker-2.3.1/aomaker/extension/har_parse/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    10792 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/extension/har_parse/har_parse.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-07-03 04:51:51.731052 aomaker-2.3.1/aomaker/extension/recording/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4517 2023-03-21 15:15:18.000000 aomaker-2.3.1/aomaker/extension/recording/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      170 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/extension/recording/addons.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     5679 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/extension/recording/recording.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1276 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/field.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2813 2023-05-20 14:38:18.000000 aomaker-2.3.1/aomaker/fixture.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      965 2023-03-22 10:18:59.000000 aomaker-2.3.1/aomaker/hook_manager.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-07-03 04:51:51.731621 aomaker-2.3.1/aomaker/html/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9937 2022-12-22 09:57:22.000000 aomaker-2.3.1/aomaker/html/heading.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4302 2022-12-22 09:57:22.000000 aomaker-2.3.1/aomaker/html/report.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    11555 2023-05-20 11:43:25.000000 aomaker-2.3.1/aomaker/html/template.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3816 2023-03-22 11:04:05.000000 aomaker-2.3.1/aomaker/log.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1476 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/make.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     7940 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/make_api.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1216 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/make_testcase.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2288 2023-06-28 07:54:12.000000 aomaker-2.3.1/aomaker/models.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      503 2023-06-13 10:28:50.000000 aomaker-2.3.1/aomaker/param_types.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      751 2023-07-03 04:37:49.000000 aomaker-2.3.1/aomaker/path.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2890 2023-05-20 14:38:18.000000 aomaker-2.3.1/aomaker/report.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8513 2023-06-28 06:57:49.000000 aomaker-2.3.1/aomaker/runner.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8639 2023-06-28 08:23:43.000000 aomaker-2.3.1/aomaker/scaffold.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-07-03 04:51:51.732029 aomaker-2.3.1/aomaker/send_msg/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/send_msg/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8329 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/send_msg/wechat.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     7672 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/swagger2yaml.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9148 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/template.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-07-03 04:51:51.732577 aomaker-2.3.1/aomaker/utils/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/utils/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9529 2023-05-22 08:33:10.000000 aomaker-2.3.1/aomaker/utils/gen_allure_report.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     5120 2023-02-02 04:06:40.000000 aomaker-2.3.1/aomaker/utils/utils.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    16987 2022-11-03 10:41:01.000000 aomaker-2.3.1/aomaker/yaml2case.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-07-03 04:51:51.728892 aomaker-2.3.1/aomaker.egg-info/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-07-03 04:51:51.000000 aomaker-2.3.1/aomaker.egg-info/PKG-INFO
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1349 2023-07-03 04:51:51.000000 aomaker-2.3.1/aomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        1 2023-07-03 04:51:51.000000 aomaker-2.3.1/aomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      154 2023-07-03 04:51:51.000000 aomaker-2.3.1/aomaker.egg-info/entry_points.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      173 2023-07-03 04:51:51.000000 aomaker-2.3.1/aomaker.egg-info/requires.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        8 2023-07-03 04:51:51.000000 aomaker-2.3.1/aomaker.egg-info/top_level.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       38 2023-07-03 04:51:51.733050 aomaker-2.3.1/setup.cfg
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1282 2023-07-03 04:51:29.000000 aomaker-2.3.1/setup.py
```

### Comparing `aomaker-2.3.0/LICENSE` & `aomaker-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/PKG-INFO` & `aomaker-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aomaker
-Version: 2.3.0
+Version: 2.3.1
 Summary: An api testing framework
 Home-page: https://github.com/ae86sen/aomaker
 Author: ancientone
 Author-email: listeningsss@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aomaker-2.3.0/README.md` & `aomaker-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/__init__.py` & `aomaker-2.3.1/aomaker/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from emoji import emojize
 
-__version__ = "2.3.0"
+__version__ = "2.3.1"
 __description__ = "Quickly Arrange,Quickly Test!"
 __image__ = emojize(fr"""
               :----.                                                             ::::
              .------            .:::::::::::::::::::::::::::::::::::::::::::::. :---:  ::::::::::::::::::::::::::
             .---::--:                                                           ----
             ----  :--:          ..::::.      :.:..::::  .::::     ..:::. .:::  :---: ...:.    .::::.     .:.:..::
            :---    :::        .---------:   :-----------------   :----------:  ----.:---:   :---::---:   -------:
```

### Comparing `aomaker-2.3.0/aomaker/_aomaker.py` & `aomaker-2.3.1/aomaker/_aomaker.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/_constants.py` & `aomaker-2.3.1/aomaker/_constants.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/_log.py` & `aomaker-2.3.1/aomaker/_log.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/_printer.py` & `aomaker-2.3.1/aomaker/_printer.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/base/base_api.py` & `aomaker-2.3.1/aomaker/base/base_api.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/base/base_testcase.py` & `aomaker-2.3.1/aomaker/base/base_testcase.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/cache.py` & `aomaker-2.3.1/aomaker/cache.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/cli.py` & `aomaker-2.3.1/aomaker/cli.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/database/base_db.py` & `aomaker-2.3.1/aomaker/database/base_db.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/database/mysql.py` & `aomaker-2.3.1/aomaker/database/mysql.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/database/sqlite.py` & `aomaker-2.3.1/aomaker/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/exceptions.py` & `aomaker-2.3.1/aomaker/exceptions.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/extension/har_parse/__init__.py` & `aomaker-2.3.1/aomaker/extension/har_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/extension/har_parse/har_parse.py` & `aomaker-2.3.1/aomaker/extension/har_parse/har_parse.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/extension/recording/__init__.py` & `aomaker-2.3.1/aomaker/extension/recording/__init__.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/extension/recording/recording.py` & `aomaker-2.3.1/aomaker/extension/recording/recording.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/field.py` & `aomaker-2.3.1/aomaker/field.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/fixture.py` & `aomaker-2.3.1/aomaker/fixture.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/hook_manager.py` & `aomaker-2.3.1/aomaker/hook_manager.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/html/heading.html` & `aomaker-2.3.1/aomaker/html/heading.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/html/report.html` & `aomaker-2.3.1/aomaker/html/report.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/html/template.html` & `aomaker-2.3.1/aomaker/html/template.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/log.py` & `aomaker-2.3.1/aomaker/log.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/make.py` & `aomaker-2.3.1/aomaker/make.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/make_api.py` & `aomaker-2.3.1/aomaker/make_api.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/make_testcase.py` & `aomaker-2.3.1/aomaker/make_testcase.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/models.py` & `aomaker-2.3.1/aomaker/models.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/path.py` & `aomaker-2.3.1/aomaker/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # DB目录
 DB_DIR = os.path.join(BASEDIR, "database")
 # pytest.ini文件路径
 PYTEST_INI_DIR = os.path.join(BASEDIR, "pytest.ini")
 # aomaker html路径
 AOMAKER_HTML = os.path.join(REPORT_DIR, "aomaker.html")
 
-AOMAKER_YAML_PATH = os.path.join(BASEDIR, "aomaker.yaml")
+AOMAKER_YAML_PATH = os.path.join(CONF_DIR, "aomaker.yaml")
```

### Comparing `aomaker-2.3.0/aomaker/report.py` & `aomaker-2.3.1/aomaker/report.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/runner.py` & `aomaker-2.3.1/aomaker/runner.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/scaffold.py` & `aomaker-2.3.1/aomaker/scaffold.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/send_msg/wechat.py` & `aomaker-2.3.1/aomaker/send_msg/wechat.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/swagger2yaml.py` & `aomaker-2.3.1/aomaker/swagger2yaml.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/template.py` & `aomaker-2.3.1/aomaker/template.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/utils/gen_allure_report.py` & `aomaker-2.3.1/aomaker/utils/gen_allure_report.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/utils/utils.py` & `aomaker-2.3.1/aomaker/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker/yaml2case.py` & `aomaker-2.3.1/aomaker/yaml2case.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/aomaker.egg-info/PKG-INFO` & `aomaker-2.3.1/aomaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aomaker
-Version: 2.3.0
+Version: 2.3.1
 Summary: An api testing framework
 Home-page: https://github.com/ae86sen/aomaker
 Author: ancientone
 Author-email: listeningsss@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aomaker-2.3.0/aomaker.egg-info/SOURCES.txt` & `aomaker-2.3.1/aomaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aomaker-2.3.0/setup.py` & `aomaker-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # --coding:utf-8--
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="aomaker",
-    version="2.3.0",
+    version="2.3.1",
     author="ancientone",
     author_email="listeningsss@163.com",
     description="An api testing framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ae86sen/aomaker",
     packages=setuptools.find_packages(),
```

