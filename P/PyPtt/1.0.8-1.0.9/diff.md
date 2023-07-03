# Comparing `tmp/PyPtt-1.0.8.tar.gz` & `tmp/PyPtt-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPtt-1.0.8.tar", last modified: Sun Jun 25 10:13:23 2023, max compression
+gzip compressed data, was "PyPtt-1.0.9.tar", last modified: Mon Jul  3 05:53:14 2023, max compression
```

## Comparing `PyPtt-1.0.8.tar` & `PyPtt-1.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:13:23.826362 PyPtt-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-25 10:13:11.000000 PyPtt-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-25 10:13:11.000000 PyPtt-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-25 10:13:23.826362 PyPtt-1.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:13:23.826362 PyPtt-1.0.8/PyPtt/
--rw-r--r--   0 runner    (1001) docker     (123)    30780 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/PTT.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_call_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_change_pw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_del_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_board_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_board_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_bottom_post_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_favourite_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_newest_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    22803 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_post_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_give_money.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_has_new_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_loginout.py
--rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_mark_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_reply_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_search_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_set_board_title.py
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/_api_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/check_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/connect_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    33897 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/lib_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    54737 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-06-25 10:13:11.000000 PyPtt-1.0.8/PyPtt/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 10:13:23.826362 PyPtt-1.0.8/PyPtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-25 10:13:23.000000 PyPtt-1.0.8/PyPtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-25 10:13:23.000000 PyPtt-1.0.8/PyPtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 10:13:23.000000 PyPtt-1.0.8/PyPtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-25 10:13:23.000000 PyPtt-1.0.8/PyPtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-25 10:13:23.000000 PyPtt-1.0.8/PyPtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-25 10:13:11.000000 PyPtt-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 10:13:23.826362 PyPtt-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-25 10:13:11.000000 PyPtt-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 05:53:14.944127 PyPtt-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-03 05:53:03.000000 PyPtt-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-03 05:53:03.000000 PyPtt-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-03 05:53:14.944127 PyPtt-1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 05:53:14.944127 PyPtt-1.0.9/PyPtt/
+-rw-r--r--   0 runner    (1001) docker     (123)    30780 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/PTT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_call_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_change_pw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_del_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_get_board_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_get_board_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_get_bottom_post_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_get_favourite_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_get_newest_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22803 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_get_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_get_post_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_get_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_give_money.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_has_new_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_loginout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_mark_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_reply_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_search_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_set_board_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17331 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/_api_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/check_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/connect_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33897 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/lib_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54787 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-03 05:53:03.000000 PyPtt-1.0.9/PyPtt/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 05:53:14.944127 PyPtt-1.0.9/PyPtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-03 05:53:14.000000 PyPtt-1.0.9/PyPtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-03 05:53:14.000000 PyPtt-1.0.9/PyPtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 05:53:14.000000 PyPtt-1.0.9/PyPtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-03 05:53:14.000000 PyPtt-1.0.9/PyPtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 05:53:14.000000 PyPtt-1.0.9/PyPtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-03 05:53:03.000000 PyPtt-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 05:53:14.944127 PyPtt-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-03 05:53:03.000000 PyPtt-1.0.9/setup.py
```

### Comparing `PyPtt-1.0.8/LICENSE` & `PyPtt-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PKG-INFO` & `PyPtt-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPtt
-Version: 1.0.8
+Version: 1.0.9
 Summary: PyPtt
 Home-page: https://github.com/PyPtt/PyPtt
 Author: CodingMan
 Author-email: pttcodingman@gmail.com
 Keywords: PTT,crawler,bot,library,websockets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![](https://raw.githubusercontent.com/PttCodingMan/PyPtt/master/logo/facebook_cover_photo_2.png)
 # PyPtt
 [![Package Version](https://img.shields.io/pypi/v/PyPtt.svg)](https://pypi.python.org/pypi/PyPtt)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/PyPtt)
-[![Codacy Badge](https://api.codacy.com/project/badge/Grade/940fe61df0a0443ba883307e11e7b22d)](https://www.codacy.com/manual/PttCodingMan/PyPtt?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=PttCodingMan/PyPtt&amp;utm_campaign=Badge_Grade)
+[![test](https://github.com/PyPtt/PyPtt/actions/workflows/flask8.yml/badge.svg)](https://github.com/PyPtt/PyPtt/actions/workflows/flask8.yml)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PyPtt)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 [![chatroom icon](https://patrolavia.github.io/telegram-badge/chat.png)](https://t.me/PyPtt)
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](http://paypal.me/CodingMan)
 
 #### PyPtt (PTT Library) 是一套 Pure Python PTT API。具備大部分常用功能，無論推文、發文、爬蟲、寄信、發 P 幣、丟水球或者追蹤帳號
 你都可以在這裡找到完整的使用範例
```

### Comparing `PyPtt-1.0.8/PyPtt/PTT.py` & `PyPtt-1.0.9/PyPtt/PTT.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_bucket.py` & `PyPtt-1.0.9/PyPtt/_api_bucket.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_call_status.py` & `PyPtt-1.0.9/PyPtt/_api_call_status.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_change_pw.py` & `PyPtt-1.0.9/PyPtt/_api_change_pw.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_comment.py` & `PyPtt-1.0.9/PyPtt/_api_comment.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_del_post.py` & `PyPtt-1.0.9/PyPtt/_api_del_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_get_board_info.py` & `PyPtt-1.0.9/PyPtt/_api_get_board_info.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_get_board_list.py` & `PyPtt-1.0.9/PyPtt/_api_get_board_list.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_get_bottom_post_list.py` & `PyPtt-1.0.9/PyPtt/_api_get_bottom_post_list.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_get_favourite_board.py` & `PyPtt-1.0.9/PyPtt/_api_get_favourite_board.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_get_newest_index.py` & `PyPtt-1.0.9/PyPtt/_api_get_newest_index.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_get_post.py` & `PyPtt-1.0.9/PyPtt/_api_get_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_get_post_index.py` & `PyPtt-1.0.9/PyPtt/_api_get_post_index.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_get_time.py` & `PyPtt-1.0.9/PyPtt/_api_get_time.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_get_user.py` & `PyPtt-1.0.9/PyPtt/_api_get_user.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_give_money.py` & `PyPtt-1.0.9/PyPtt/_api_give_money.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_has_new_mail.py` & `PyPtt-1.0.9/PyPtt/_api_has_new_mail.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_loginout.py` & `PyPtt-1.0.9/PyPtt/_api_loginout.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,14 @@
 
     index = api.connect_core.send(
         cmd,
         target_list,
         screen_timeout=api.config.screen_long_timeout,
         refresh=False,
         secret=True)
-    ori_screen = api.connect_core.get_screen_queue()[-1]
     if index == 0:
 
         current_capacity, max_capacity = _api_util.get_mailbox_capacity(api)
 
         api.logger.info(i18n.has_new_mail_goto_main_menu)
 
         if current_capacity > max_capacity:
@@ -193,26 +192,28 @@
 
     if not is_login:
         raise exceptions.LoginError()
 
     if '> (' in ori_screen:
         api.cursor = data_type.Cursor.NEW
         api.logger.debug(i18n.new_cursor)
-    else:
+    elif '●(' in ori_screen:
         api.cursor = data_type.Cursor.OLD
         api.logger.debug(i18n.old_cursor)
+    else:
+        raise exceptions.UnknownError()
 
-    if api.cursor not in screens.Target.InBoardWithCursor:
-        screens.Target.InBoardWithCursor.append('\n' + api.cursor)
+    screens.Target.InBoardWithCursor = screens.Target.InBoardWithCursor[:screens.Target.InBoardWithCursorLen]
+    screens.Target.InBoardWithCursor.append(api.cursor)
 
-    if len(screens.Target.MainMenu) == len(screens.Target.CursorToGoodbye):
-        if api.cursor == '>':
-            screens.Target.CursorToGoodbye.append('> (G)oodbye')
-        else:
-            screens.Target.CursorToGoodbye.append('●(G)oodbye')
+    screens.Target.CursorToGoodbye = screens.Target.CursorToGoodbye[:len(screens.Target.MainMenu)]
+    if api.cursor == '>':
+        screens.Target.CursorToGoodbye.append('> (G)oodbye')
+    else:
+        screens.Target.CursorToGoodbye.append('●(G)oodbye')
 
     unregistered_user = True
     if '(T)alk' in ori_screen:
         unregistered_user = False
     if '(P)lay' in ori_screen:
         unregistered_user = False
     if '(N)amelist' in ori_screen:
```

### Comparing `PyPtt-1.0.8/PyPtt/_api_mail.py` & `PyPtt-1.0.9/PyPtt/_api_mail.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_mark_post.py` & `PyPtt-1.0.9/PyPtt/_api_mark_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_post.py` & `PyPtt-1.0.9/PyPtt/_api_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_reply_post.py` & `PyPtt-1.0.9/PyPtt/_api_reply_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_search_user.py` & `PyPtt-1.0.9/PyPtt/_api_search_user.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_set_board_title.py` & `PyPtt-1.0.9/PyPtt/_api_set_board_title.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/_api_util.py` & `PyPtt-1.0.9/PyPtt/_api_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,20 +37,14 @@
         # 動畫文章
         connect_core.TargetUnit(screens.Target.Animation, response=command.go_main_menu_type_q,
                                 break_detect_after_send=True),
     ]
 
     line_from_pattern = re.compile('[\d]+~[\d]+')
 
-    content_start = '───────────────────────────────────────'
-    content_end = []
-    content_end.append('--\n※ 發信站: 批踢踢實業坊')
-    content_end.append('--\n※ 發信站: 批踢踢兔(ptt2.cc)')
-    content_end.append('--\n※ 發信站: 新批踢踢(ptt2.twbbs.org.tw)')
-
     has_control_code = False
     control_code_mode = False
     push_start = False
     content_start_exist = False
     content_start_jump = False
     content_start_jump_set = False
 
@@ -65,20 +59,20 @@
 
         last_screen = api.connect_core.get_screen_queue()[-1]
         lines = last_screen.split('\n')
         last_line = lines[-1]
         lines.pop()
         last_screen = '\n'.join(lines)
 
-        if content_start in last_screen and not content_start_exist:
+        if screens.Target.content_start in last_screen and not content_start_exist:
             content_start_exist = True
 
         if content_start_exist:
             if not content_start_jump_set:
-                if content_start not in last_screen:
+                if screens.Target.content_start not in last_screen:
                     content_start_jump = True
                     content_start_jump_set = True
             else:
                 content_start_jump = False
 
         pattern_result = line_from_pattern.search(last_line)
         if pattern_result is None:
@@ -93,14 +87,20 @@
                 last_read_line_b = last_read_line_b_temp - 1
             control_code_mode = False
 
         if first_page:
             first_page = False
             origin_post.append(last_screen)
         else:
+            # 這裡是根據觀察畫面行數的變化歸納出的神奇公式...
+            # 輸出的結果是要判斷出畫面的最後 x 行是新的文章內容
+            # 這裡的一切都太可怕，每除完一次錯誤，我的腦袋會選擇 flush 掉一次
+            # 所以這裡的變數名稱都是很亂的，請見諒
+            # but it works!
+
             # print(LastScreen)
             # print(f'last_read_line_a_temp [{last_read_line_a_temp}]')
             # print(f'last_read_line_b_temp [{last_read_line_b_temp}]')
             # print(f'last_read_line_a {last_read_line_a}')
             # print(f'last_read_line_b {last_read_line_b}')
             # print(f'GetLineB {last_read_line_a_temp - last_read_line_a}')
             # print(f'GetLineA {last_read_line_b_temp - last_read_line_b}')
@@ -111,31 +111,22 @@
                     new_content_part = '\n'.join(
                         lines[-stop_dict[last_read_line_a_temp]:])
                     stop_dict = dict()
                 else:
                     get_line_b = last_read_line_b_temp - last_read_line_b
                     if get_line_b > 0:
                         # print('Type 1')
-                        # print(f'Type 1 line_dis [{line_dis}]')
-                        # print(f'Type 1 get_line_b [{get_line_b}]')
-                        # print('index', index)
                         new_content_part = '\n'.join(lines[-get_line_b:])
                         if index == 1 and len(new_content_part) == get_line_b - 1:
-                            # print(1)
                             new_content_part = '\n'.join(lines[-(get_line_b * 2):])
                         elif origin_post:
-                            # print(2)
                             last_line_temp = origin_post[-1].strip()
                             try_line = lines[-(get_line_b + 1)].strip()
 
                             if not last_line_temp.endswith(try_line):
-                                # print(3)
-                                # print('=====' * 20)
-                                # print('== last line [', last_line_temp, ']')
-                                # print('== try_line [', try_line, ']')
                                 new_content_part = try_line + '\n' + new_content_part
                         stop_dict = dict()
                     else:
                         # 駐足現象，LastReadLineB跟上一次相比並沒有改變
                         if (last_read_line_b_temp + 1) not in stop_dict:
                             stop_dict[last_read_line_b_temp + 1] = 1
                         stop_dict[last_read_line_b_temp + 1] += 1
@@ -153,35 +144,34 @@
 
             origin_post.append(new_content_part)
 
             logger.debug('NewContentPart', new_content_part)
 
         if index == 1:
             if content_start_jump and len(new_content_part) == 0:
-                # print(f'!!!GetLineB {GetLineB}')
                 get_line_b += 1
                 new_content_part = '\n'.join(lines[-get_line_b:])
-                # print(f'!!!NewContentPart {NewContentPart}')
+
                 origin_post.pop()
                 origin_post.append(new_content_part)
             break
 
         if not control_code_mode:
             last_read_line_a = last_read_line_a_temp
             last_read_line_b = last_read_line_b_temp
 
-        for EC in content_end:
+        for EC in screens.Target.content_end_list:
             if EC in last_screen:
                 push_start = True
                 break
 
-        if not push_start:
-            cmd = command.down
-        else:
+        if push_start:
             cmd = command.right
+        else:
+            cmd = command.down
 
     # print(api.Unconfirmed)
     origin_post = '\n'.join(origin_post)
     # OriginPost = [line.strip() for line in OriginPost.split('\n')]
     # OriginPost = '\n'.join(OriginPost)
 
     logger.debug('OriginPost', origin_post)
@@ -299,49 +289,43 @@
 
     pattern = re.compile('[\d]+')
     pattern_result = pattern.search(cursor_line)
     if pattern_result is not None:
         post_index = int(pattern_result.group(0))
 
     push_number = cursor_line
-    # print(f'2>{push_number}<')
     push_number = push_number[7:11]
-    # print(push_number)
     push_number = push_number.split(' ')
-    # print(PushNumber)
     push_number = list(filter(None, push_number))
-    # print(push_number)
 
     if len(push_number) == 0:
         push_number = None
     else:
         push_number = push_number[-1]
         if push_number.startswith('爆') or push_number.startswith('~爆'):
             push_number = '爆'
 
         if push_number.startswith('+') or push_number.startswith('~'):
             push_number = push_number[1:]
-            # print(PushNumber)
+
         if push_number.lower().startswith('m'):
             push_number = push_number[1:]
-            # print(PushNumber)
+
         if push_number.lower().startswith('!'):
             push_number = push_number[1:]
 
         if push_number.lower().startswith('s'):
             push_number = push_number[1:]
 
         if push_number.lower().startswith('='):
             push_number = push_number[1:]
 
         if len(push_number) == 0:
             push_number = None
 
-    # print(PushNumber)
-
     logger.debug('PostAuthor', post_author)
     logger.debug('PostTitle', post_title)
     logger.debug('PostAID', post_aid)
     logger.debug('PostWeb', post_web)
     logger.debug('PostMoney', post_money)
     logger.debug('ListDate', list_date)
     logger.debug('PushNumber', push_number)
@@ -451,18 +435,16 @@
         ]
 
         api.connect_core.send(cmd, target_list)
 
 
 def one_thread(api):
     current_thread_id = threading.get_ident()
-    if current_thread_id == api._thread_id:
-        return
-
-    raise exceptions.MultiThreadOperated()
+    if current_thread_id != api._thread_id:
+        raise exceptions.MultiThreadOperated()
 
 
 def check_board(api, board: str, check_moderator: bool = False) -> Dict:
     if board.lower() not in api._exist_board_list:
         board_info = _api_get_board_info.get_board_info(api, board, get_post_kind=False, call_by_others=False)
         api._exist_board_list.append(board.lower())
         api._board_info_list[board.lower()] = board_info
```

### Comparing `PyPtt-1.0.8/PyPtt/check_value.py` & `PyPtt-1.0.9/PyPtt/check_value.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/command.py` & `PyPtt-1.0.9/PyPtt/command.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/config.py` & `PyPtt-1.0.9/PyPtt/config.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/connect_core.py` & `PyPtt-1.0.9/PyPtt/connect_core.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/data_type.py` & `PyPtt-1.0.9/PyPtt/data_type.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/exceptions.py` & `PyPtt-1.0.9/PyPtt/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/i18n.py` & `PyPtt-1.0.9/PyPtt/i18n.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/lib_util.py` & `PyPtt-1.0.9/PyPtt/lib_util.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt/screens.py` & `PyPtt-1.0.9/PyPtt/screens.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         '相關主題'
     ]
 
     InBoardWithCursor = [
         '【',
         '看板資訊/設定',
     ]
+    InBoardWithCursorLen = len(InBoardWithCursor)
 
     # (h)說明 (←/q)離開
     # (y)回應(X%)推文(h)說明(←)離開
     # (y)回應(X/%)推文 (←)離開
 
     InPost = [
         '瀏覽',
```

### Comparing `PyPtt-1.0.8/PyPtt/service.py` & `PyPtt-1.0.9/PyPtt/service.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/PyPtt.egg-info/PKG-INFO` & `PyPtt-1.0.9/PyPtt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPtt
-Version: 1.0.8
+Version: 1.0.9
 Summary: PyPtt
 Home-page: https://github.com/PyPtt/PyPtt
 Author: CodingMan
 Author-email: pttcodingman@gmail.com
 Keywords: PTT,crawler,bot,library,websockets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![](https://raw.githubusercontent.com/PttCodingMan/PyPtt/master/logo/facebook_cover_photo_2.png)
 # PyPtt
 [![Package Version](https://img.shields.io/pypi/v/PyPtt.svg)](https://pypi.python.org/pypi/PyPtt)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/PyPtt)
-[![Codacy Badge](https://api.codacy.com/project/badge/Grade/940fe61df0a0443ba883307e11e7b22d)](https://www.codacy.com/manual/PttCodingMan/PyPtt?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=PttCodingMan/PyPtt&amp;utm_campaign=Badge_Grade)
+[![test](https://github.com/PyPtt/PyPtt/actions/workflows/flask8.yml/badge.svg)](https://github.com/PyPtt/PyPtt/actions/workflows/flask8.yml)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PyPtt)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 [![chatroom icon](https://patrolavia.github.io/telegram-badge/chat.png)](https://t.me/PyPtt)
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](http://paypal.me/CodingMan)
 
 #### PyPtt (PTT Library) 是一套 Pure Python PTT API。具備大部分常用功能，無論推文、發文、爬蟲、寄信、發 P 幣、丟水球或者追蹤帳號
 你都可以在這裡找到完整的使用範例
```

### Comparing `PyPtt-1.0.8/PyPtt.egg-info/SOURCES.txt` & `PyPtt-1.0.9/PyPtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.8/README.md` & `PyPtt-1.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ![](https://raw.githubusercontent.com/PttCodingMan/PyPtt/master/logo/facebook_cover_photo_2.png)
 # PyPtt
 [![Package Version](https://img.shields.io/pypi/v/PyPtt.svg)](https://pypi.python.org/pypi/PyPtt)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/PyPtt)
-[![Codacy Badge](https://api.codacy.com/project/badge/Grade/940fe61df0a0443ba883307e11e7b22d)](https://www.codacy.com/manual/PttCodingMan/PyPtt?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=PttCodingMan/PyPtt&amp;utm_campaign=Badge_Grade)
+[![test](https://github.com/PyPtt/PyPtt/actions/workflows/flask8.yml/badge.svg)](https://github.com/PyPtt/PyPtt/actions/workflows/flask8.yml)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PyPtt)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 [![chatroom icon](https://patrolavia.github.io/telegram-badge/chat.png)](https://t.me/PyPtt)
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](http://paypal.me/CodingMan)
 
 #### PyPtt (PTT Library) 是一套 Pure Python PTT API。具備大部分常用功能，無論推文、發文、爬蟲、寄信、發 P 幣、丟水球或者追蹤帳號
 你都可以在這裡找到完整的使用範例
```

### Comparing `PyPtt-1.0.8/setup.py` & `PyPtt-1.0.9/setup.py`

 * *Files identical despite different names*

