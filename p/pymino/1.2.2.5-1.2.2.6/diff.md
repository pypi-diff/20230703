# Comparing `tmp/pymino-1.2.2.5.tar.gz` & `tmp/pymino-1.2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\pymino push\dist\.tmp-zf55okvu\pymino-1.2.2.5.tar", last modified: Sun Jul  2 21:06:08 2023, max compression
+gzip compressed data, was "pymino-1.2.2.6.tar", last modified: Sun Jul  2 23:12:28 2023, max compression
```

## Comparing `pymino-1.2.2.5.tar` & `pymino-1.2.2.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 21:06:08.376103 pymino-1.2.2.5/
--rw-rw-rw-   0        0        0     1085 2023-06-28 09:49:18.000000 pymino-1.2.2.5/LICENSE
--rw-rw-rw-   0        0        0     7424 2023-07-02 21:06:08.376599 pymino-1.2.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     6706 2023-06-28 10:21:17.000000 pymino-1.2.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 21:06:08.281367 pymino-1.2.2.5/pymino/
--rw-rw-rw-   0        0        0      721 2023-07-01 20:52:00.000000 pymino-1.2.2.5/pymino/__init__.py
--rw-rw-rw-   0        0        0    11727 2023-07-02 15:44:24.000000 pymino-1.2.2.5/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30988 2023-07-02 15:43:21.000000 pymino-1.2.2.5/pymino/bot.py
--rw-rw-rw-   0        0        0    36824 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-07-02 21:06:08.321047 pymino-1.2.2.5/pymino/ext/
--rw-rw-rw-   0        0        0      528 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0      192 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/_global.py
--rw-rw-rw-   0        0        0    11196 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/account.py
--rw-rw-rw-   0        0        0   343766 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    21408 2023-07-02 15:57:37.000000 pymino-1.2.2.5/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    25886 2023-07-02 15:58:45.000000 pymino-1.2.2.5/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   342679 2023-07-02 15:30:17.000000 pymino-1.2.2.5/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/console.py
--rw-rw-rw-   0        0        0    45528 2023-07-02 20:56:56.000000 pymino-1.2.2.5/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1856 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-07-02 21:06:08.349815 pymino-1.2.2.5/pymino/ext/entities/
--rw-rw-rw-   0        0        0      428 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     9014 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/admin_log.py
--rw-rw-rw-   0        0        0     1670 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    17769 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/bubble.py
--rw-rw-rw-   0        0        0    20322 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    15825 2023-07-02 15:04:30.000000 pymino-1.2.2.5/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1839 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31711 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/sticker.py
--rw-rw-rw-   0        0        0     6185 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0    70299 2023-07-02 15:19:03.000000 pymino-1.2.2.5/pymino/ext/global_client.py
--rw-rw-rw-   0        0        0      543 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6657 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-07-02 21:06:08.375111 pymino-1.2.2.5/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11357 2023-07-02 15:09:23.000000 pymino-1.2.2.5/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6280 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10322 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-02 21:06:08.299223 pymino-1.2.2.5/pymino.egg-info/
--rw-rw-rw-   0        0        0     7424 2023-07-02 21:06:08.000000 pymino-1.2.2.5/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1555 2023-07-02 21:06:08.000000 pymino-1.2.2.5/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 21:06:08.000000 pymino-1.2.2.5/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-07-02 21:06:08.000000 pymino-1.2.2.5/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-02 21:06:08.000000 pymino-1.2.2.5/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-07-02 21:06:08.379574 pymino-1.2.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1394 2023-06-28 09:49:18.000000 pymino-1.2.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 23:12:28.399698 pymino-1.2.2.6/
+-rw-rw-rw-   0        0        0     1085 2023-06-27 02:23:25.000000 pymino-1.2.2.6/LICENSE
+-rw-rw-rw-   0        0        0     7424 2023-07-02 23:12:28.399698 pymino-1.2.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6706 2023-07-02 23:10:10.000000 pymino-1.2.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 23:12:28.019991 pymino-1.2.2.6/pymino/
+-rw-rw-rw-   0        0        0      721 2023-07-02 22:29:02.000000 pymino-1.2.2.6/pymino/__init__.py
+-rw-rw-rw-   0        0        0    11727 2023-07-02 22:27:27.000000 pymino-1.2.2.6/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30988 2023-07-02 22:27:27.000000 pymino-1.2.2.6/pymino/bot.py
+-rw-rw-rw-   0        0        0    36824 2023-06-28 06:25:49.000000 pymino-1.2.2.6/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-07-02 23:12:28.188642 pymino-1.2.2.6/pymino/ext/
+-rw-rw-rw-   0        0        0      528 2023-06-27 04:04:07.000000 pymino-1.2.2.6/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-06-17 07:35:45.000000 pymino-1.2.2.6/pymino/ext/_global.py
+-rw-rw-rw-   0        0        0    11196 2023-06-28 06:25:45.000000 pymino-1.2.2.6/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   345265 2023-07-02 22:55:58.000000 pymino-1.2.2.6/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    21408 2023-07-02 22:27:27.000000 pymino-1.2.2.6/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    25886 2023-07-02 22:27:27.000000 pymino-1.2.2.6/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   344166 2023-07-02 22:55:07.000000 pymino-1.2.2.6/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    45526 2023-07-02 22:27:53.000000 pymino-1.2.2.6/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1856 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-07-02 23:12:28.316653 pymino-1.2.2.6/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      428 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     9014 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/admin_log.py
+-rw-rw-rw-   0        0        0     1670 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    15825 2023-07-02 22:27:27.000000 pymino-1.2.2.6/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1839 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0    70299 2023-07-02 22:27:27.000000 pymino-1.2.2.6/pymino/ext/global_client.py
+-rw-rw-rw-   0        0        0      543 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6657 2023-06-27 07:21:56.000000 pymino-1.2.2.6/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-07-02 23:12:28.398700 pymino-1.2.2.6/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11357 2023-07-02 22:27:27.000000 pymino-1.2.2.6/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6280 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10322 2023-06-27 02:23:25.000000 pymino-1.2.2.6/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-02 23:12:28.035118 pymino-1.2.2.6/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7424 2023-07-02 23:12:27.000000 pymino-1.2.2.6/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1555 2023-07-02 23:12:27.000000 pymino-1.2.2.6/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 23:12:27.000000 pymino-1.2.2.6/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-07-02 23:12:27.000000 pymino-1.2.2.6/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-02 23:12:27.000000 pymino-1.2.2.6/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-07-02 23:12:28.401692 pymino-1.2.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1394 2023-06-27 04:33:02.000000 pymino-1.2.2.6/setup.py
```

### Comparing `pymino-1.2.2.5/LICENSE` & `pymino-1.2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/PKG-INFO` & `pymino-1.2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.2.5
+Version: 1.2.2.6
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.2.5 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.2.6 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.2.5/README.md` & `pymino-1.2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/__init__.py` & `pymino-1.2.2.6/pymino/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.2.2.5'
+__version__ = '1.2.2.6'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.2.2.5/pymino/async_bot.py` & `pymino-1.2.2.6/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/bot.py` & `pymino-1.2.2.6/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/client.py` & `pymino-1.2.2.6/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/__init__.py` & `pymino-1.2.2.6/pymino/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/account.py` & `pymino-1.2.2.6/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/async_community.py` & `pymino-1.2.2.6/pymino/ext/async_community.py`

 * *Files 0% similar despite different names*

```diff
@@ -5195,14 +5195,52 @@
                 } if reason is None else {
                     "adminOpNote": {"content": reason},
                     "adminOpName": 110,
                     "adminOpValue": 9,
                     "timestamp": int(time() * 1000)
                 }))
 
+    @community
+    async def enable_chat(self, chatId: str, reason: str = None, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Enables a chat in the community.
+
+        :param chatId: The ID of the chat to enable.
+        :type chatId: str
+        :param reason: The reason for enabling the chat. (Optional)
+        :type reason: str, optional
+        :param comId: The ID of the community where the chat is located. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: An `ApiResponse` object representing the response from the API.
+        :rtype: ApiResponse
+
+        This function enables a chat in the specified community.
+
+        `ApiResponse` represents a response from the API.
+
+        **Example usage:**
+
+        >>> response = client.community.enable_chat("chat123")
+        ... print(response.status_code)
+        ... print(response.json())
+        """
+        return ApiResponse(await self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/chat/thread/{chatId}/admin",
+            data = {
+            "adminOpName": 110,
+            "adminOpValue": 0,
+            "timestamp": int(time() * 1000)
+            } if reason is None else {
+            "adminOpNote": {"content": reason},
+            "adminOpName": 110,
+            "adminOpValue": 0,
+            "timestamp": int(time() * 1000)
+            }
+        ))
 
     @community
     async def disable_blog(self, blogId: str, reason: str = None, comId: Union[str, int] = None) -> ApiResponse:
         """
         Disables a blog in the current or specified community.
 
         :param blogId: The ID of the blog to disable.
```

### Comparing `pymino-1.2.2.5/pymino/ext/async_context.py` & `pymino-1.2.2.6/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/async_event_handler.py` & `pymino-1.2.2.6/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/async_socket.py` & `pymino-1.2.2.6/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/community.py` & `pymino-1.2.2.6/pymino/ext/community.py`

 * *Files 1% similar despite different names*

```diff
@@ -5128,14 +5128,52 @@
             } if reason is None else {
             "adminOpNote": {"content": reason},
             "adminOpName": 110,
             "adminOpValue": 9,
             "timestamp": int(time() * 1000)
             }))
 
+    @community
+    def enable_chat(self, chatId: str, reason: str = None, comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Enables a chat in the community.
+
+        :param chatId: The ID of the chat to enable.
+        :type chatId: str
+        :param reason: The reason for enabling the chat. (Optional)
+        :type reason: str, optional
+        :param comId: The ID of the community where the chat is located. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: An `ApiResponse` object representing the response from the API.
+        :rtype: ApiResponse
+
+        This function enables a chat in the specified community.
+
+        `ApiResponse` represents a response from the API.
+
+        **Example usage:**
+
+        >>> response = client.community.enable_chat("chat123")
+        ... print(response.status_code)
+        ... print(response.json())
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/chat/thread/{chatId}/admin",
+            data = {
+            "adminOpName": 110,
+            "adminOpValue": 0,
+            "timestamp": int(time() * 1000)
+            } if reason is None else {
+            "adminOpNote": {"content": reason},
+            "adminOpName": 110,
+            "adminOpValue": 0,
+            "timestamp": int(time() * 1000)
+            }
+        ))
 
     @community
     def disable_blog(self, blogId: str, reason: str = None, comId: Union[str, int] = None) -> ApiResponse:
         """
         Disables a blog in the current or specified community.
 
         :param blogId: The ID of the blog to disable.
```

### Comparing `pymino-1.2.2.5/pymino/ext/console.py` & `pymino-1.2.2.6/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/context.py` & `pymino-1.2.2.6/pymino/ext/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -867,15 +867,15 @@
 
         return 200
 
 
     def _add_cache(self, chatId: str, userId: str, content: str):
         with self.cache as cache:
             if cache.get(f"{chatId}_{userId}") is not None:
-                self.cache.clear(f"{chatId}_{userId}")
+                self.cache.pop(f"{chatId}_{userId}")
 
             cache.add(
                 key=f"{chatId}_{userId}",
                 value=content,
                 expire=90
                 )
```

### Comparing `pymino-1.2.2.5/pymino/ext/dispatcher.py` & `pymino-1.2.2.6/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/acm.py` & `pymino-1.2.2.6/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/admin_log.py` & `pymino-1.2.2.6/pymino/ext/entities/admin_log.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/api_response.py` & `pymino-1.2.2.6/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/bubble.py` & `pymino-1.2.2.6/pymino/ext/entities/bubble.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/chat_threads.py` & `pymino-1.2.2.6/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/comments.py` & `pymino-1.2.2.6/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/enums.py` & `pymino-1.2.2.6/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/exceptions.py` & `pymino-1.2.2.6/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/general.py` & `pymino-1.2.2.6/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/handlers.py` & `pymino-1.2.2.6/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/link_info.py` & `pymino-1.2.2.6/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/member.py` & `pymino-1.2.2.6/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/messages.py` & `pymino-1.2.2.6/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/notification.py` & `pymino-1.2.2.6/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/sticker.py` & `pymino-1.2.2.6/pymino/ext/entities/sticker.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/threads.py` & `pymino-1.2.2.6/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/userprofile.py` & `pymino-1.2.2.6/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/entities/wsevents.py` & `pymino-1.2.2.6/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/global_client.py` & `pymino-1.2.2.6/pymino/ext/global_client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/handle_queue.py` & `pymino-1.2.2.6/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/socket.py` & `pymino-1.2.2.6/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.2.6/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/utilities/chat_console.py` & `pymino-1.2.2.6/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/utilities/commands.py` & `pymino-1.2.2.6/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/utilities/community_console.py` & `pymino-1.2.2.6/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/utilities/generate.py` & `pymino-1.2.2.6/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/utilities/menu.py` & `pymino-1.2.2.6/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/utilities/profile_console.py` & `pymino-1.2.2.6/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino/ext/utilities/request_handler.py` & `pymino-1.2.2.6/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/pymino.egg-info/PKG-INFO` & `pymino-1.2.2.6/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.2.5
+Version: 1.2.2.6
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.2.5 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.2.6 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.2.5/pymino.egg-info/SOURCES.txt` & `pymino-1.2.2.6/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.5/setup.cfg` & `pymino-1.2.2.6/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e32 2e35 0d0a 6175  on = 1.2.2.5..au
+00000020: 6f6e 203d 2031 2e32 2e32 2e36 0d0a 6175  on = 1.2.2.6..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.2.2.5/setup.py` & `pymino-1.2.2.6/setup.py`

 * *Files identical despite different names*

