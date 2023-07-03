# Comparing `tmp/opensesame-plugin-radboudbox-2.3.0.tar.gz` & `tmp/opensesame-plugin-radboudbox-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensesame-plugin-radboudbox-2.3.0.tar", last modified: Fri Nov 25 15:27:26 2022, max compression
+gzip compressed data, was "opensesame-plugin-radboudbox-2.4.0.tar", last modified: Mon Jul  3 19:07:44 2023, max compression
```

## Comparing `opensesame-plugin-radboudbox-2.3.0.tar` & `opensesame-plugin-radboudbox-2.4.0.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2022-11-25 15:27:26.665639 opensesame-plugin-radboudbox-2.3.0/
--rw-r--r--   0 bob       (1000) bob       (1000)     2772 2022-11-25 14:26:22.000000 opensesame-plugin-radboudbox-2.3.0/.gitignore
--rw-r--r--   0 bob       (1000) bob       (1000)    35147 2017-10-13 14:38:12.000000 opensesame-plugin-radboudbox-2.3.0/COPYING
--rw-r--r--   0 bob       (1000) bob       (1000)      349 2017-11-24 23:59:08.000000 opensesame-plugin-radboudbox-2.3.0/LICENSE.md
--rw-r--r--   0 bob       (1000) bob       (1000)      106 2017-11-24 23:04:58.000000 opensesame-plugin-radboudbox-2.3.0/MANIFEST.in
--rw-r--r--   0 bob       (1000) bob       (1000)     3918 2022-11-25 15:27:26.665639 opensesame-plugin-radboudbox-2.3.0/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1000)     3091 2022-11-25 14:29:09.000000 opensesame-plugin-radboudbox-2.3.0/README.md
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2022-11-25 15:27:26.662639 opensesame-plugin-radboudbox-2.3.0/opensesame_plugin_radboudbox.egg-info/
--rw-r--r--   0 bob       (1000) bob       (1000)     3918 2022-11-25 15:27:26.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugin_radboudbox.egg-info/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1000)     2323 2022-11-25 15:27:26.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugin_radboudbox.egg-info/SOURCES.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        1 2022-11-25 15:27:26.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugin_radboudbox.egg-info/dependency_links.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        1 2022-11-25 15:27:26.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugin_radboudbox.egg-info/top_level.txt
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2022-11-25 15:27:26.661640 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2022-11-25 15:27:26.662639 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_start/
--rw-r--r--   0 bob       (1000) bob       (1000)     1236 2022-11-25 15:10:12.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_start/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)     1665 2021-04-12 13:10:41.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start.md
--rw-r--r--   0 bob       (1000) bob       (1000)      762 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start.png
--rw-r--r--   0 bob       (1000) bob       (1000)     6763 2022-11-25 14:50:22.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1716 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start_large.png
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2022-11-25 15:27:26.663640 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_wait/
--rw-r--r--   0 bob       (1000) bob       (1000)      455 2022-11-25 15:10:12.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_wait/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)     1236 2021-04-12 13:10:38.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.md
--rw-r--r--   0 bob       (1000) bob       (1000)      755 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.png
--rw-r--r--   0 bob       (1000) bob       (1000)     3220 2022-11-25 14:50:47.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1687 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait_large.png
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2022-11-25 15:27:26.663640 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_init/
--rw-r--r--   0 bob       (1000) bob       (1000)      960 2022-11-25 15:10:12.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_init/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)     1935 2021-04-12 13:07:28.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_init/radboudbox_init.md
--rw-r--r--   0 bob       (1000) bob       (1000)      705 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_init/radboudbox_init.png
--rw-r--r--   0 bob       (1000) bob       (1000)     4122 2022-11-25 14:50:42.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_init/radboudbox_init.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1709 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_init/radboudbox_init_large.png
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2022-11-25 15:27:26.664640 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_control/
--rw-r--r--   0 bob       (1000) bob       (1000)     1056 2022-11-25 15:10:12.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_control/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)     1299 2021-04-12 13:10:32.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control.md
--rw-r--r--   0 bob       (1000) bob       (1000)      719 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control.png
--rw-r--r--   0 bob       (1000) bob       (1000)     3799 2022-11-25 14:50:37.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1678 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control_large.png
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2022-11-25 15:27:26.664640 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_trigger/
--rw-r--r--   0 bob       (1000) bob       (1000)      529 2022-11-25 15:10:12.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_trigger/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)     1630 2021-04-12 13:10:28.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger.md
--rw-r--r--   0 bob       (1000) bob       (1000)      725 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger.png
--rw-r--r--   0 bob       (1000) bob       (1000)     2623 2022-11-25 14:50:34.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1692 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger_large.png
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2022-11-25 15:27:26.665639 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_wait_buttons/
--rw-r--r--   0 bob       (1000) bob       (1000)     1206 2022-11-25 15:10:12.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_wait_buttons/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)     1622 2021-04-12 13:10:24.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons.md
--rw-r--r--   0 bob       (1000) bob       (1000)      723 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons.png
--rw-r--r--   0 bob       (1000) bob       (1000)     5578 2022-11-25 14:50:30.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1691 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)       38 2022-11-25 15:27:26.665639 opensesame-plugin-radboudbox-2.3.0/setup.cfg
--rw-r--r--   0 bob       (1000) bob       (1000)     5081 2022-11-25 15:25:19.000000 opensesame-plugin-radboudbox-2.3.0/setup.py
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-03 19:07:44.449342 opensesame-plugin-radboudbox-2.4.0/
+-rw-r--r--   0 bob       (1000) bob       (1000)    35147 2017-10-13 14:38:12.000000 opensesame-plugin-radboudbox-2.4.0/COPYING
+-rw-r--r--   0 bob       (1000) bob       (1000)      349 2017-11-24 23:59:08.000000 opensesame-plugin-radboudbox-2.4.0/LICENSE.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      106 2017-11-24 23:04:58.000000 opensesame-plugin-radboudbox-2.4.0/MANIFEST.in
+-rw-r--r--   0 bob       (1000) bob       (1000)     3918 2023-07-03 19:07:44.449342 opensesame-plugin-radboudbox-2.4.0/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)     3091 2022-11-25 14:29:09.000000 opensesame-plugin-radboudbox-2.4.0/README.md
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-03 19:07:44.445342 opensesame-plugin-radboudbox-2.4.0/opensesame_plugin_radboudbox.egg-info/
+-rw-r--r--   0 bob       (1000) bob       (1000)     3918 2023-07-03 19:07:44.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugin_radboudbox.egg-info/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)     2322 2023-07-03 19:07:44.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugin_radboudbox.egg-info/SOURCES.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-07-03 19:07:44.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugin_radboudbox.egg-info/dependency_links.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-07-03 19:07:44.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugin_radboudbox.egg-info/top_level.txt
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-03 19:07:44.444342 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-03 19:07:44.446342 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_start/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1236 2023-07-03 19:04:18.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_start/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)     1665 2021-04-12 13:10:41.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      762 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     6763 2023-07-03 19:04:18.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1716 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start_large.png
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-03 19:07:44.447342 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_wait/
+-rw-r--r--   0 bob       (1000) bob       (1000)      455 2023-07-03 19:04:18.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_wait/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)     1236 2021-04-12 13:10:38.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      755 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     3220 2023-07-03 19:04:18.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1687 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait_large.png
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-03 19:07:44.447342 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_init/
+-rw-r--r--   0 bob       (1000) bob       (1000)      960 2023-07-03 19:04:18.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_init/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)     1935 2021-04-12 13:07:28.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_init/radboudbox_init.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      705 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_init/radboudbox_init.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     4040 2023-07-03 19:04:18.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_init/radboudbox_init.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1709 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_init/radboudbox_init_large.png
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-03 19:07:44.448342 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_control/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1056 2023-07-03 19:04:18.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_control/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)     1299 2021-04-12 13:10:32.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      719 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     3799 2023-07-03 19:04:18.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1678 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control_large.png
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-03 19:07:44.448342 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_trigger/
+-rw-r--r--   0 bob       (1000) bob       (1000)      529 2023-07-03 19:04:18.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_trigger/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)     1630 2021-04-12 13:10:28.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      725 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     2623 2023-07-03 19:04:18.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1692 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger_large.png
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-03 19:07:44.449342 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_wait_buttons/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1206 2023-07-03 19:04:18.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_wait_buttons/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)     1622 2021-04-12 13:10:24.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      723 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     5578 2023-07-03 19:04:18.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1691 2017-11-15 19:24:34.000000 opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)      121 2023-07-03 19:07:44.449342 opensesame-plugin-radboudbox-2.4.0/setup.cfg
+-rw-r--r--   0 bob       (1000) bob       (1000)     5081 2023-07-03 19:04:18.000000 opensesame-plugin-radboudbox-2.4.0/setup.py
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/COPYING` & `opensesame-plugin-radboudbox-2.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/PKG-INFO` & `opensesame-plugin-radboudbox-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensesame-plugin-radboudbox
-Version: 2.3.0
+Version: 2.4.0
 Summary: An OpenSesame Plug-in for collecting button responses, audio detection, voice key and sending stimulus synchronization triggers with the Radboud Buttonbox to data acquisition systems.
 Home-page: https://github.com/dev-jam/opensesame-plugin-radboudbox
 Author: Bob Rosbag
 Author-email: debian@bobrosbag.nl
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: MacOS X
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/README.md` & `opensesame-plugin-radboudbox-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugin_radboudbox.egg-info/PKG-INFO` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugin_radboudbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensesame-plugin-radboudbox
-Version: 2.3.0
+Version: 2.4.0
 Summary: An OpenSesame Plug-in for collecting button responses, audio detection, voice key and sending stimulus synchronization triggers with the Radboud Buttonbox to data acquisition systems.
 Home-page: https://github.com/dev-jam/opensesame-plugin-radboudbox
 Author: Bob Rosbag
 Author-email: debian@bobrosbag.nl
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: MacOS X
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugin_radboudbox.egg-info/SOURCES.txt` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugin_radboudbox.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.gitignore
 COPYING
 LICENSE.md
 MANIFEST.in
 README.md
+setup.cfg
 setup.py
 opensesame_plugin_radboudbox.egg-info/PKG-INFO
 opensesame_plugin_radboudbox.egg-info/SOURCES.txt
 opensesame_plugin_radboudbox.egg-info/dependency_links.txt
 opensesame_plugin_radboudbox.egg-info/top_level.txt
 opensesame_plugins/radboudbox_get_buttons_start/info.yaml
 opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start.md
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_start/info.yaml` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_start/info.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 description: Radboud Buttonbox - starts button registration in the background.
-version: 2.3.0
+version: 2.4.0
 author: "Bob Rosbag"
 url: "http://osdoc.cogsci.nl/"
 category: "RadboudBox"
 date: "2020"
 controls:
 -
     label: Allowed responses
@@ -29,9 +29,9 @@
     type: "text"
 -
     label: |
       <small><b>Note:</b> Radboudbox init item at the begin of the experiment is needed for initialization of the buttonbox</small>
     type: text
 -
     label:  |
-      <small>Radboud Buttonbox version 2.3.0</small>
+      <small>Radboud Buttonbox version 2.4.0</small>
     type: "text"
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start.md` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start.png` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start.py` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import openexp.keyboard
 from libopensesame.py3compat import *
 from libopensesame.item import item
 from libopensesame.generic_response import generic_response
 import threading
 
 
-VERSION = u'2.3.0'
+VERSION = u'2.4.0'
 
 class radboudbox_get_buttons_start(item, generic_response):
 
     description = u'Radboud Buttonbox: starts button registration in the background.'
 
     def __init__(self, name, experiment, string=None):
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start_large.png` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_start/radboudbox_get_buttons_start_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.md` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.png` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.py` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from libopensesame import debug
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from openexp.keyboard import keyboard
 from libopensesame.py3compat import *
 from libopensesame.item import item
 
 
-VERSION = u'2.3.0'
+VERSION = u'2.4.0'
 
 class radboudbox_get_buttons_wait(item):
 
     description = u'Radboud Buttonbox: waits until the background button registration has finished.'
 
     def __init__(self, name, experiment, string=None):
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait_large.png` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_init/info.yaml` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_init/info.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 description: Radboud Buttonbox - initializes the buttonbox.
-version: 2.3.0
+version: 2.4.0
 author: "Bob Rosbag"
 url: "http://osdoc.cogsci.nl/"
 category: "RadboudBox"
 date: "2020"
 controls:
 -
     label: "Dummy Mode"
@@ -31,9 +31,9 @@
     var: port
 -
     label: |
       <small><b>Note:</b> Radboudbox init item at the begin of the experiment is needed for initialization of the buttonbox</small>
     type: text
 -
     label:  |
-      <small>Radboud Buttonbox version 2.3.0</small>
+      <small>Radboud Buttonbox version 2.4.0</small>
     type: "text"
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_init/radboudbox_init.md` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_init/radboudbox_init.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_init/radboudbox_init.png` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_init/radboudbox_init.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_init/radboudbox_init.py` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_init/radboudbox_init.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from libopensesame.py3compat import *
 from libopensesame import debug
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 
-VERSION = u'2.3.0'
+VERSION = u'2.4.0'
 
 class radboudbox_init(item):
 
     description = u'Radboud Buttonbox - initializes the buttonbox.'
 
     def __init__(self, name, experiment, string=None):
 
@@ -83,15 +83,14 @@
                 from rusocsci import buttonbox
             except ImportError:
                 self.show_message(u'The RuSocSci package could not be imported. Please install package.')
             try:
                 self.experiment.radboudbox = buttonbox.Buttonbox(id=self.id, port=self.port)
                 self.clock.sleep(4000)
                 self.experiment.cleanup_functions.append(self.close)
-                self.python_workspace[u'radboudbox'] = self.experiment.radboudbox
             except OSError:
                     debug.msg(u'Could not access the Radboud Buttonbox')
         elif self.dummy_mode == u'yes':
             self.show_message(u'Dummy mode enabled, prepare phase')
         else:
             self.show_message(u'Error with dummy mode, dummy mode: %s' % self.dummy_mode)
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_init/radboudbox_init_large.png` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_init/radboudbox_init_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_control/info.yaml` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_control/info.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 description: Radboud Buttonbox - sends a control command to the buttonbox.
-version: 2.3.0
+version: 2.4.0
 author: "Bob Rosbag"
 url: "http://osdoc.cogsci.nl/"
 category: "RadboudBox"
 date: "2018"
 controls:
 -
     label: "Send Command"
@@ -37,9 +37,9 @@
     var: command_value
 -
     label: |
       <small><b>Note:</b> Radboudbox init item at the begin of the experiment is needed for initialization of the buttonbox</small>
     type: text
 -
     label:  |
-      <small>Radboud Buttonbox version 2.3.0</small>
+      <small>Radboud Buttonbox version 2.4.0</small>
     type: "text"
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control.md` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control.png` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control.py` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from libopensesame.py3compat import *
 from libopensesame import debug
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 
-VERSION = u'2.3.0'
+VERSION = u'2.4.0'
 
 CMD_DICT = {u'Calibrate Sound': [u'C',u'S'],
             u'Calibrate Voice': [u'C',u'V'],
             u'Detect Sound': [u'D',u'S'],
             u'Detect Voice': [u'D',u'V'],
             u'Marker Out': u'M',
             u'Pulse Out': u'P',
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control_large.png` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_control/radboudbox_send_control_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_trigger/info.yaml` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_trigger/info.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 description: Radboud Buttonbox - sends a trigger.
-version: 2.3.0
+version: 2.4.0
 author: "Bob Rosbag"
 url: "http://osdoc.cogsci.nl/"
 category: "RadboudBox"
 date: "2020"
 controls:
 -
     label: "Value"
@@ -13,9 +13,9 @@
     var: "value"
 -
     label: |
       <small><b>Note:</b> Radboudbox init item at the begin of the experiment is needed for initialization of the buttonbox</small>
     type: text
 -
     label:  |
-      <small>Radboud Buttonbox version 2.3.0</small>
+      <small>Radboud Buttonbox version 2.4.0</small>
     type: "text"
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger.md` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger.png` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger.py` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from libopensesame.py3compat import *
 from libopensesame import debug
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 
-VERSION = u'2.3.0'
+VERSION = u'2.4.0'
 
 class radboudbox_send_trigger(item):
 
     description = u'Radboud Buttonbox: sends a trigger.'
 
     def __init__(self, name, experiment, string=None):
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger_large.png` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_send_trigger/radboudbox_send_trigger_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_wait_buttons/info.yaml` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_wait_buttons/info.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 description: Radboud Buttonbox - starts button registration on the foreground.
-version: 2.3.0
+version: 2.4.0
 author: "Bob Rosbag"
 url: "http://osdoc.cogsci.nl/"
 category: "RadboudBox"
 date: "2020"
 controls:
 -
     label: Allowed responses
@@ -29,9 +29,9 @@
     type: "text"
 -
     label: |
       <small><b>Note:</b> Radboudbox init item at the begin of the experiment is needed for initialization of the buttonbox</small>
     type: text
 -
     label:  |
-      <small>Radboud Buttonbox version 2.3.0</small>
+      <small>Radboud Buttonbox version 2.4.0</small>
     type: "text"
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons.md` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons.png` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons.py` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from libopensesame import debug
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 import openexp.keyboard
 from libopensesame.py3compat import *
 from libopensesame.item import item
 from libopensesame.generic_response import generic_response
 
-VERSION = u'2.3.0'
+VERSION = u'2.4.0'
 
 class radboudbox_wait_buttons(item, generic_response):
 
     description = u'Radboud Buttonbox: starts button registration on the foreground.'
 
     def __init__(self, name, experiment, string=None):
```

### Comparing `opensesame-plugin-radboudbox-2.3.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons_large.png` & `opensesame-plugin-radboudbox-2.4.0/opensesame_plugins/radboudbox_wait_buttons/radboudbox_wait_buttons_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-radboudbox-2.3.0/setup.py` & `opensesame-plugin-radboudbox-2.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         with open('README.md') as fd:
             return fd.read()
     return 'No readme information'
 
 
 setup(
     name='opensesame-plugin-radboudbox',
-    version='2.3.0',
+    version='2.4.0',
     description='An OpenSesame Plug-in for collecting button responses, audio detection, voice key and sending stimulus synchronization triggers with the Radboud Buttonbox to data acquisition systems.',
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     author='Bob Rosbag',
     author_email='debian@bobrosbag.nl',
     url='https://github.com/dev-jam/opensesame-plugin-radboudbox',
     # Classifiers used by PyPi if you upload the plugin there
```

