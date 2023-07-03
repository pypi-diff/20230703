# Comparing `tmp/qinglan-bot-0.1.4.tar.gz` & `tmp/qinglan-bot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qinglan-bot-0.1.4.tar", last modified: Mon Jun 26 07:20:53 2023, max compression
+gzip compressed data, was "qinglan-bot-0.1.5.tar", last modified: Mon Jul  3 03:48:49 2023, max compression
```

## Comparing `qinglan-bot-0.1.4.tar` & `qinglan-bot-0.1.5.tar`

### file list

```diff
@@ -1,62 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.792714 qinglan-bot-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-26 07:20:53.792714 qinglan-bot-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/cli/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/database/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/database/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/database/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/auto_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/connected_servers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/plugins/display_server_name/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/display_server_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/display_server_name/display_off.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/display_server_name/display_on.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/plugins/on_msg/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/on_msg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/on_msg/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon/change_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon/change_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon/change_port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_cmd/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_cmd/rcon_cmd_off.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_cmd/rcon_cmd_on.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.792714 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_msg/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_msg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_msg/rcon_msg_off.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_msg/rcon_msg_on.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.792714 qinglan-bot-0.1.4/qinglan_bot/plugins/send_group_name/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/send_group_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/send_group_name/send_off.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/send_group_name/send_on.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/servers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.792714 qinglan-bot-0.1.4/qinglan_bot/plugins/sub/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/sub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/sub/add_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/sub/delete_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/plugins/sub/sub_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/qinglan_bot/ws_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:20:53.788714 qinglan-bot-0.1.4/qinglan_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-26 07:20:53.000000 qinglan-bot-0.1.4/qinglan_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-26 07:20:53.000000 qinglan-bot-0.1.4/qinglan_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:20:53.000000 qinglan-bot-0.1.4/qinglan_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 07:20:53.000000 qinglan-bot-0.1.4/qinglan_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-26 07:20:53.000000 qinglan-bot-0.1.4/qinglan_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 07:20:53.000000 qinglan-bot-0.1.4/qinglan_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 07:20:53.792714 qinglan-bot-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-26 07:20:48.000000 qinglan-bot-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:48:49.414570 qinglan-bot-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-03 03:48:49.414570 qinglan-bot-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:48:49.406570 qinglan-bot-0.1.5/qinglan_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:48:49.406570 qinglan-bot-0.1.5/qinglan_bot/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/cli/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:48:49.410570 qinglan-bot-0.1.5/qinglan_bot/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/database/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/database/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:48:49.410570 qinglan-bot-0.1.5/qinglan_bot/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/auto_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/connected_servers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:48:49.410570 qinglan-bot-0.1.5/qinglan_bot/plugins/display_server_name/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/display_server_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/display_server_name/display_off.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/display_server_name/display_on.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/on_msg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:48:49.410570 qinglan-bot-0.1.5/qinglan_bot/plugins/rcon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/rcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/rcon/change_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/rcon/change_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/rcon/change_port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:48:49.410570 qinglan-bot-0.1.5/qinglan_bot/plugins/rcon_cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/rcon_cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/rcon_cmd/rcon_cmd_off.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/rcon_cmd/rcon_cmd_on.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:48:49.410570 qinglan-bot-0.1.5/qinglan_bot/plugins/rcon_msg/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/rcon_msg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/rcon_msg/rcon_msg_off.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/rcon_msg/rcon_msg_on.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:48:49.410570 qinglan-bot-0.1.5/qinglan_bot/plugins/send_group_name/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/send_group_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/send_group_name/send_off.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/send_group_name/send_on.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/servers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:48:49.414570 qinglan-bot-0.1.5/qinglan_bot/plugins/sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/sub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/sub/add_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/sub/delete_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/plugins/sub/sub_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/qinglan_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:48:49.406570 qinglan-bot-0.1.5/qinglan_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-03 03:48:49.000000 qinglan-bot-0.1.5/qinglan_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-03 03:48:49.000000 qinglan-bot-0.1.5/qinglan_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 03:48:49.000000 qinglan-bot-0.1.5/qinglan_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 03:48:49.000000 qinglan-bot-0.1.5/qinglan_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 03:48:49.000000 qinglan-bot-0.1.5/qinglan_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 03:48:49.000000 qinglan-bot-0.1.5/qinglan_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 03:48:49.414570 qinglan-bot-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-03 03:48:41.000000 qinglan-bot-0.1.5/setup.py
```

### Comparing `qinglan-bot-0.1.4/LICENSE` & `qinglan-bot-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/PKG-INFO` & `qinglan-bot-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qinglan-bot
-Version: 0.1.4
+Version: 0.1.5
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通机器人
 Home-page: https://github.com/17TheWord/qinglan_bot
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -25,15 +25,14 @@
 
 ## 安装
 
 - 文档：[仍在更新的青岚Bot文档](https://17theword.github.io/qinglan_bot/)
 
 - NoneBot2
     - `pip install qinglan-bot`
-
     - 空目录下使用命令 `ql run`
 
 - MineCraft Server
   - 前往 [插件Releases](https://github.com/17TheWord/nonebot-plugin-mcqq/releases) 下载对应服务端的 `jar` 文件并安装
   - `jar` 安装文档可参考 [MC_QQ](https://17theword.github.io/mc_qq/)
 
 ## 命令
```

### Comparing `qinglan-bot-0.1.4/README.md` & `qinglan-bot-0.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 ## 安装
 
 - 文档：[仍在更新的青岚Bot文档](https://17theword.github.io/qinglan_bot/)
 
 - NoneBot2
     - `pip install qinglan-bot`
-
     - 空目录下使用命令 `ql run`
 
 - MineCraft Server
   - 前往 [插件Releases](https://github.com/17TheWord/nonebot-plugin-mcqq/releases) 下载对应服务端的 `jar` 文件并安装
   - `jar` 安装文档可参考 [MC_QQ](https://17theword.github.io/mc_qq/)
 
 ## 命令
```

### Comparing `qinglan-bot-0.1.4/qinglan_bot/__init__.py` & `qinglan-bot-0.1.5/qinglan_bot/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,31 @@
-from nonebot import get_driver, require
+from nonebot import get_driver, ReverseDriver
 from nonebot.plugin import PluginMetadata
 from nonebot.plugin.manager import PluginLoader
+from .config import Config
 
-if isinstance(globals()["__loader__"], PluginLoader):
-    require("nonebot_plugin_guild_patch")
-    from .config import Config
+__plugin_meta__ = PluginMetadata(
+    name="青岚Bot",
+    description="基于NoneBot的与Minecraft Server互通消息的机器人",
+    homepage="https://github.com/17TheWord/qinglan_bot",
+    usage="配置完成后在群聊发送消息即可同步至 Minecraft 服务器",
+    config=Config,
+    type="application",
+    supported_adapters={
+        "nonebot.adapters.onebot.v11"
+    }
+)
 
-    __plugin_meta__ = PluginMetadata(
-        name="青岚Bot",
-        description="基于NoneBot的与Minecraft Server互通消息的机器人",
-        homepage="https://github.com/17TheWord/qinglan_bot",
-        usage="配置完成后在群聊发送消息即可同步至 Minecraft 服务器",
-        config=Config,
-        type="application",
-        supported_adapters={
-            "nonebot.adapters.onebot.v11"
-        }
-    )
+if isinstance(globals()["__loader__"], PluginLoader):
     driver = get_driver()
 
     plugin_config: Config = Config.parse_obj(get_driver().config)
 
-    from .ws_server import start_ws_server, stop_ws_server
+    from .router import set_route
     from . import plugins
 
-
     # Bot 连接时
-    @driver.on_bot_connect
+    @driver.on_startup
     async def on_start():
         # 启动 WebSocket 服务器
-        await start_ws_server()
-
-
-    # Bot 断开时
-    @driver.on_bot_disconnect
-    async def on_close():
-        # 关闭 WebSocket 服务器
-        await stop_ws_server()
+        if isinstance(driver, ReverseDriver):
+            await set_route(driver=driver)
```

### Comparing `qinglan-bot-0.1.4/qinglan_bot/cli/bot.py` & `qinglan-bot-0.1.5/qinglan_bot/cli/bot.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/cli/utils.py` & `qinglan-bot-0.1.5/qinglan_bot/cli/utils.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/database/db.py` & `qinglan-bot-0.1.5/qinglan_bot/database/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,28 +159,30 @@
     # 列表 相关操作
     @classmethod
     async def get_sub(cls, **kwargs):
         """获取指定位置的 互通列表"""
         return await Sub.get(**kwargs).first()
 
     @classmethod
-    async def add_sub(cls, *, server_name, **kwargs) -> bool:
+    async def add_sub(cls, *, server_name: str, bot_self_id: int, **kwargs) -> bool:
         """添加互通服务器"""
+
         if not await Sub.add(server_name=server_name, **kwargs):
             return False
         if kwargs["type"] == "group":
             await cls.add_group(group_id=kwargs["type_id"], send_group_name=False)
         if not await Server.get(server_name=server_name):
             await cls.add_server(
                 server_name=server_name,
                 rcon_ip="127.0.0.1",
                 rcon_port=25575,
                 rcon_password="change_password",
                 rcon_msg=False,
-                rcon_cmd=False
+                rcon_cmd=False,
+                bot_self_id=bot_self_id
             )
         await cls.update_server_list()
         return True
 
     @classmethod
     async def set_sub(cls, conf, switch, **kwargs):
         """开关互通设置"""
```

### Comparing `qinglan-bot-0.1.4/qinglan_bot/database/models.py` & `qinglan-bot-0.1.5/qinglan_bot/database/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from tortoise.fields.data import CharField, IntField, TextField, BooleanField
 from tortoise.models import Model
+from tortoise.fields.data import CharField, IntField, TextField, BooleanField
 
 
 class BaseModel(Model):
     @classmethod
     def get_(cls, *args, **kwargs):
         super().get(*args, **kwargs)
 
@@ -53,14 +53,15 @@
 class Server(BaseModel):
     server_name = TextField()
     rcon_ip = CharField(max_length=20)
     rcon_port = IntField()
     rcon_password = CharField(max_length=18)
     rcon_msg = BooleanField()
     rcon_cmd = BooleanField()
+    bot_self_id = IntField()
 
 
 class Group(BaseModel):
     group_id = IntField()
     send_group_name = BooleanField()
```

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/auto_delete.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/auto_delete.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/connected_servers.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/connected_servers.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/display_server_name/display_off.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/display_server_name/display_off.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/display_server_name/display_on.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/display_server_name/display_on.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/help.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/help.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from nonebot import on_command
 from nonebot.matcher import matchers
 
 from ..utils import to_me
 
-help = on_command("ql帮助", rule=to_me(), priority=3)
+help = on_command("ql帮助", rule=to_me(), priority=1)
 
 
 @help.handle()
 async def _():
     message = "青岚 目前支持的功能：\n（请将Server替换为需要操作的服务器名）\n"
     for matchers_list in matchers.values():
         for matcher in matchers_list:
```

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/on_msg/__init__.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/on_msg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from nonebot import on_message, on_command
 from nonebot.adapters import Message
 from nonebot.params import CommandArg
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent
 from nonebot_plugin_guild_patch import GuildMessageEvent
 from typing import Union
 
-from .data_source import send_msg_to_mc, send_cmd_to_mc
-from ...utils import msg_rule, permission_check
+from mcqq_tool.utils import send_msg_to_mc, send_cmd_to_mc
+from ..utils import msg_rule, permission_check
 
 mc_qq = on_message(priority=2, rule=msg_rule)
 
 mc_qq_cmd = on_command("minecraft_command", aliases={"mcc"}, priority=1, rule=msg_rule, block=True)
 
 mc_qq_cmd.handle()(permission_check)
```

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/rcon/__init__.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/rcon/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import aiomcrcon
 from nonebot import logger
-from mcqq_tool.utils import get_client, rcon_connect
+from mcqq_tool.utils import rcon_connect, CLIENTS
 
 from . import change_ip, change_port, change_password
 from ...database.db import DB as db, server_list
 
 
 async def change_rcon_status(server_name):
     """更新Rcon状态"""
     for server in server_list:
-        if (client := get_client(server_name=server_name)) and server.server_name == server_name:
+        if (client := CLIENTS.get(server_name)) and server.server_name == server_name:
             # 获取该服务器的信息
             server = await db.get_server(server_name=server_name)
             # 开
             if server.rcon_msg or server.rcon_cmd and not client.rcon:
                 client.rcon = aiomcrcon.Client(
                     server.rcon_ip,
                     server.rcon_port,
```

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/rcon/change_ip.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/rcon/change_ip.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/rcon/change_password.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/rcon/change_password.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/rcon/change_port.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/rcon/change_port.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_cmd/rcon_cmd_off.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/rcon_cmd/rcon_cmd_off.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_cmd/rcon_cmd_on.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/rcon_cmd/rcon_cmd_on.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_msg/rcon_msg_off.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/rcon_msg/rcon_msg_off.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/rcon_msg/rcon_msg_on.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/rcon_msg/rcon_msg_on.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/send_group_name/send_off.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/send_group_name/send_off.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/send_group_name/send_on.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/send_group_name/send_on.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/servers.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/servers.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/sub/add_sub.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/sub/add_sub.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,13 +34,14 @@
             guild_id=event.guild_id, channel_id=event.channel_id, send_group_name=False
         )
 
     result = await db.add_sub(
         type=event.message_type,
         type_id=await get_type_id(event),
         server_name=server_name,
-        display_server_name=False
+        display_server_name=False,
+        bot_self_id=event.self_id
     )
 
     if result:
         await add_sub.finish(message=f"已开启与服务器 {server_name} 的互通")
     await add_sub.finish(message=f"服务器 {server_name} 的互通已经开启过了")
```

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/sub/delete_sub.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/sub/delete_sub.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/plugins/sub/sub_list.py` & `qinglan-bot-0.1.5/qinglan_bot/plugins/sub/sub_list.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot/utils.py` & `qinglan-bot-0.1.5/qinglan_bot/utils.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.1.4/qinglan_bot.egg-info/PKG-INFO` & `qinglan-bot-0.1.5/qinglan_bot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qinglan-bot
-Version: 0.1.4
+Version: 0.1.5
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通机器人
 Home-page: https://github.com/17TheWord/qinglan_bot
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -25,15 +25,14 @@
 
 ## 安装
 
 - 文档：[仍在更新的青岚Bot文档](https://17theword.github.io/qinglan_bot/)
 
 - NoneBot2
     - `pip install qinglan-bot`
-
     - 空目录下使用命令 `ql run`
 
 - MineCraft Server
   - 前往 [插件Releases](https://github.com/17TheWord/nonebot-plugin-mcqq/releases) 下载对应服务端的 `jar` 文件并安装
   - `jar` 安装文档可参考 [MC_QQ](https://17theword.github.io/mc_qq/)
 
 ## 命令
```

### Comparing `qinglan-bot-0.1.4/qinglan_bot.egg-info/SOURCES.txt` & `qinglan-bot-0.1.5/qinglan_bot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 README.md
 setup.py
 qinglan_bot/__init__.py
 qinglan_bot/cli_start.py
 qinglan_bot/config.py
+qinglan_bot/router.py
 qinglan_bot/utils.py
-qinglan_bot/ws_server.py
 qinglan_bot.egg-info/PKG-INFO
 qinglan_bot.egg-info/SOURCES.txt
 qinglan_bot.egg-info/dependency_links.txt
 qinglan_bot.egg-info/entry_points.txt
 qinglan_bot.egg-info/requires.txt
 qinglan_bot.egg-info/top_level.txt
 qinglan_bot/cli/__init__.py
@@ -18,20 +18,19 @@
 qinglan_bot/database/__init__.py
 qinglan_bot/database/db.py
 qinglan_bot/database/models.py
 qinglan_bot/plugins/__init__.py
 qinglan_bot/plugins/auto_delete.py
 qinglan_bot/plugins/connected_servers.py
 qinglan_bot/plugins/help.py
+qinglan_bot/plugins/on_msg.py
 qinglan_bot/plugins/servers.py
 qinglan_bot/plugins/display_server_name/__init__.py
 qinglan_bot/plugins/display_server_name/display_off.py
 qinglan_bot/plugins/display_server_name/display_on.py
-qinglan_bot/plugins/on_msg/__init__.py
-qinglan_bot/plugins/on_msg/data_source.py
 qinglan_bot/plugins/rcon/__init__.py
 qinglan_bot/plugins/rcon/change_ip.py
 qinglan_bot/plugins/rcon/change_password.py
 qinglan_bot/plugins/rcon/change_port.py
 qinglan_bot/plugins/rcon_cmd/__init__.py
 qinglan_bot/plugins/rcon_cmd/rcon_cmd_off.py
 qinglan_bot/plugins/rcon_cmd/rcon_cmd_on.py
```

