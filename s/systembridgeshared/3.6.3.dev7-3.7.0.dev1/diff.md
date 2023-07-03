# Comparing `tmp/systembridgeshared-3.6.3.dev7.tar.gz` & `tmp/systembridgeshared-3.7.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgeshared-3.6.3.dev7.tar", last modified: Thu Apr 13 20:19:08 2023, max compression
+gzip compressed data, was "systembridgeshared-3.7.0.dev1.tar", last modified: Mon Jul  3 08:33:15 2023, max compression
```

## Comparing `systembridgeshared-3.6.3.dev7.tar` & `systembridgeshared-3.7.0.dev1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:08.163660 systembridgeshared-3.6.3.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-13 20:19:08.163660 systembridgeshared-3.6.3.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:19:08.163660 systembridgeshared-3.6.3.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:08.143660 systembridgeshared-3.6.3.dev7/systembridgeshared/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 20:19:05.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:08.159660 systembridgeshared-3.6.3.dev7/systembridgeshared/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/database_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/database_data_remote_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/database_data_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/display.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/get_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/keyboard_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/keyboard_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/media_directories.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/media_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/media_get_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/media_get_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/media_play.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/open_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/open_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/register_data_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/models/update_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    17315 2023-04-13 20:18:47.000000 systembridgeshared-3.6.3.dev7/systembridgeshared/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:08.143660 systembridgeshared-3.6.3.dev7/systembridgeshared.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-13 20:19:08.000000 systembridgeshared-3.6.3.dev7/systembridgeshared.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-13 20:19:08.000000 systembridgeshared-3.6.3.dev7/systembridgeshared.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:19:08.000000 systembridgeshared-3.6.3.dev7/systembridgeshared.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-13 20:19:08.000000 systembridgeshared-3.6.3.dev7/systembridgeshared.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 20:19:08.000000 systembridgeshared-3.6.3.dev7/systembridgeshared.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:15.401466 systembridgeshared-3.7.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-03 08:33:15.401466 systembridgeshared-3.7.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 08:33:15.401466 systembridgeshared-3.7.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:15.393466 systembridgeshared-3.7.0.dev1/systembridgeshared/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-03 08:33:13.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:15.397466 systembridgeshared-3.7.0.dev1/systembridgeshared/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/database_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/database_data_remote_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/database_data_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/get_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/keyboard_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/keyboard_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/media_directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/media_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/media_get_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/media_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/media_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/open_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/open_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/register_data_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/update_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17315 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:15.393466 systembridgeshared-3.7.0.dev1/systembridgeshared.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-03 08:33:15.000000 systembridgeshared-3.7.0.dev1/systembridgeshared.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-03 08:33:15.000000 systembridgeshared-3.7.0.dev1/systembridgeshared.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:33:15.000000 systembridgeshared-3.7.0.dev1/systembridgeshared.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-03 08:33:15.000000 systembridgeshared-3.7.0.dev1/systembridgeshared.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 08:33:15.000000 systembridgeshared-3.7.0.dev1/systembridgeshared.egg-info/top_level.txt
```

### Comparing `systembridgeshared-3.6.3.dev7/pyproject.toml` & `systembridgeshared-3.7.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.6.3.dev7/setup.py` & `systembridgeshared-3.7.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/common.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/common.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/const.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .models.data import Data
 from .models.disk import Disk
 from .models.display import Display
 from .models.generic import Generic
 from .models.gpu import Gpu
 from .models.keyboard_key import KeyboardKey
 from .models.keyboard_text import KeyboardText
+from .models.media import Media
 from .models.media_directories import MediaDirectories
 from .models.media_files import File, MediaFiles
 from .models.memory import Memory
 from .models.network import Network
 from .models.notification import Notification
 from .models.open_path import OpenPath
 from .models.open_url import OpenUrl
@@ -167,14 +168,15 @@
 MODEL_GENERIC = "generic"
 MODEL_GPU = "gpu"
 MODEL_KEYBOARD_KEY = "keyboard_key"
 MODEL_KEYBOARD_TEXT = "keyboard_text"
 MODEL_MEDIA_DIRECTORIES = "media_directories"
 MODEL_MEDIA_FILE = "media_file"
 MODEL_MEDIA_FILES = "media_files"
+MODEL_MEDIA = "media"
 MODEL_MEMORY = "memory"
 MODEL_NETWORK = "network"
 MODEL_NOTIFICATION = "notification"
 MODEL_OPEN_PATH = "open_path"
 MODEL_OPEN_URL = "open_url"
 MODEL_RESPONSE = "response"
 MODEL_SECRETS = "secrets"
@@ -191,14 +193,15 @@
     MODEL_GENERIC: Generic,
     MODEL_GPU: Gpu,
     MODEL_KEYBOARD_KEY: KeyboardKey,
     MODEL_KEYBOARD_TEXT: KeyboardText,
     MODEL_MEDIA_DIRECTORIES: MediaDirectories,
     MODEL_MEDIA_FILE: File,
     MODEL_MEDIA_FILES: MediaFiles,
+    MODEL_MEDIA: Media,
     MODEL_MEMORY: Memory,
     MODEL_NETWORK: Network,
     MODEL_NOTIFICATION: Notification,
     MODEL_OPEN_PATH: OpenPath,
     MODEL_OPEN_URL: OpenUrl,
     MODEL_RESPONSE: Response,
     MODEL_SENSORS: Sensors,
```

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/database.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .common import convert_string_to_correct_type, get_user_data_directory
 from .const import (
     MODEL_BATTERY,
     MODEL_CPU,
     MODEL_DISK,
     MODEL_DISPLAY,
     MODEL_GPU,
+    MODEL_MEDIA,
     MODEL_MEMORY,
     MODEL_NETWORK,
     MODEL_SECRETS,
     MODEL_SENSORS,
     MODEL_SETTINGS,
     MODEL_SYSTEM,
 )
@@ -28,14 +29,15 @@
 from .models.database_data import (
     CPU,
     GPU,
     Battery,
     Data,
     Disk,
     Display,
+    Media,
     Memory,
     Network,
     Secrets,
     Settings,
     System,
 )
 from .models.database_data_remote_bridge import RemoteBridge
@@ -43,14 +45,15 @@
 
 TABLE_MAP: Mapping[str, Any] = {
     MODEL_BATTERY: Battery,
     MODEL_CPU: CPU,
     MODEL_DISK: Disk,
     MODEL_DISPLAY: Display,
     MODEL_GPU: GPU,
+    MODEL_MEDIA: Media,
     MODEL_MEMORY: Memory,
     MODEL_NETWORK: Network,
     MODEL_SECRETS: Secrets,
     MODEL_SENSORS: Sensors,
     MODEL_SETTINGS: Settings,
     MODEL_SYSTEM: System,
 }
@@ -58,14 +61,15 @@
 
 TableDataType = Union[
     Battery,
     CPU,
     Disk,
     Display,
     GPU,
+    Media,
     Memory,
     Network,
     RemoteBridge,
     Secrets,
     Sensors,
     Settings,
     System,
```

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/exceptions.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/exceptions.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/http_client.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/http_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/logger.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/logger.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/models/battery.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/models/media.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # generated by datamodel-codegen:
-#   filename:  battery.json
+#   filename:  media.json
 
 from __future__ import annotations
 
 from typing import Optional
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel
 
 
-class LastUpdated(BaseModel):
+class Media(BaseModel):
     """
-    Last updated
+    Media Info
     """
 
-    class Config:
-        extra = Extra.allow
-
-    is_charging: Optional[float] = None
-    percentage: Optional[float] = None
-
-
-class Battery(BaseModel):
-    """
-    Battery
-    """
-
-    class Config:
-        extra = Extra.allow
-
-    id: Optional[str] = Field(None, description="Event ID")
-    is_charging: Optional[bool] = None
-    percentage: Optional[float] = None
-    last_updated: Optional[LastUpdated] = Field(None, description="Last updated")
+    album_artist: Optional[str] = None
+    album_title: Optional[str] = None
+    artist: Optional[str] = None
+    duration: Optional[float] = None
+    is_fast_forward_enabled: Optional[bool] = None
+    is_next_enabled: Optional[bool] = None
+    is_pause_enabled: Optional[bool] = None
+    is_play_enabled: Optional[bool] = None
+    is_previous_enabled: Optional[bool] = None
+    is_rewind_enabled: Optional[bool] = None
+    is_stop_enabled: Optional[bool] = None
+    playback_rate: Optional[float] = None
+    position: Optional[float] = None
+    repeat: Optional[str] = None
+    shuffle: Optional[bool] = None
+    status: Optional[str] = None
+    subtitle: Optional[str] = None
+    thumbnail: Optional[str] = None
+    title: Optional[str] = None
+    track_number: Optional[int] = None
+    type: Optional[str] = None
```

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/models/cpu.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/models/cpu.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # generated by datamodel-codegen:
 #   filename:  cpu.json
 
 from __future__ import annotations
 
 from typing import Optional
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
 
 
 class LastUpdated(BaseModel):
     """
     Last updated
     """
 
-    class Config:
-        extra = Extra.allow
-
     count: Optional[float] = None
     frequency_current: Optional[float] = None
     frequency_min: Optional[float] = None
     frequency_max: Optional[float] = None
     load_average: Optional[float] = None
     power_package: Optional[float] = None
     stats_ctx_switches: Optional[float] = None
@@ -42,17 +39,14 @@
 
 
 class Cpu(BaseModel):
     """
     CPU
     """
 
-    class Config:
-        extra = Extra.allow
-
     id: Optional[str] = Field(None, description="Event ID")
     count: Optional[int] = None
     frequency_current: Optional[float] = None
     frequency_min: Optional[float] = None
     frequency_max: Optional[float] = None
     load_average: Optional[float] = None
     power_package: Optional[float] = None
```

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/models/data.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/models/data.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/models/database_data.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/models/database_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,18 @@
     """Database Data Display"""
 
 
 class GPU(Data, table=True):
     """Database Data GPU"""
 
 
+class Media(Data, table=True):
+    """Media Data Memory"""
+
+
 class Memory(Data, table=True):
     """Database Data Memory"""
 
 
 class Network(Data, table=True):
     """Database Data Network"""
```

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/models/database_data_remote_bridge.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/models/database_data_remote_bridge.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/models/disk.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/models/disk.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # generated by datamodel-codegen:
 #   filename:  disk.json
 
 from __future__ import annotations
 
 from typing import Optional
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
 
 
 class LastUpdated(BaseModel):
     """
     Last updated
     """
 
-    class Config:
-        extra = Extra.allow
-
     devices: float
     io_counters_read_count: Optional[float] = None
     io_counters_write_count: Optional[float] = None
     io_counters_read_bytes: Optional[float] = None
     io_counters_write_bytes: Optional[float] = None
     io_counters_read_time: Optional[float] = None
     io_counters_write_time: Optional[float] = None
@@ -27,17 +24,14 @@
 
 
 class Disk(BaseModel):
     """
     Disk
     """
 
-    class Config:
-        extra = Extra.allow
-
     id: Optional[str] = Field(None, description="Event ID")
     devices: list
     io_counters_read_count: Optional[int] = None
     io_counters_write_count: Optional[int] = None
     io_counters_read_bytes: Optional[int] = None
     io_counters_write_bytes: Optional[int] = None
     io_counters_read_time: Optional[int] = None
```

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/models/gpu.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/models/battery.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 # generated by datamodel-codegen:
-#   filename:  gpu.json
+#   filename:  battery.json
 
 from __future__ import annotations
 
 from typing import Optional
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
 
 
 class LastUpdated(BaseModel):
     """
     Last updated
     """
 
-    class Config:
-        extra = Extra.allow
+    is_charging: Optional[float] = None
+    percentage: Optional[float] = None
 
-    gpus: Optional[float] = None
 
-
-class Gpu(BaseModel):
+class Battery(BaseModel):
     """
-    GPU
+    Battery
     """
 
-    class Config:
-        extra = Extra.allow
-
     id: Optional[str] = Field(None, description="Event ID")
-    gpus: Optional[list] = None
+    is_charging: Optional[bool] = None
+    percentage: Optional[float] = None
     last_updated: Optional[LastUpdated] = Field(None, description="Last updated")
```

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/models/media_files.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/models/media_files.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/models/memory.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/models/memory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # generated by datamodel-codegen:
 #   filename:  memory.json
 
 from __future__ import annotations
 
 from typing import Optional
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
 
 
 class LastUpdated(BaseModel):
     """
     Last updated
     """
 
-    class Config:
-        extra = Extra.allow
-
     swap_total: Optional[float] = None
     swap_used: Optional[float] = None
     swap_free: Optional[float] = None
     swap_percent: Optional[float] = None
     swap_sin: Optional[float] = None
     swap_sout: Optional[float] = None
     virtual_total: Optional[float] = None
@@ -30,17 +27,14 @@
 
 
 class Memory(BaseModel):
     """
     Memory
     """
 
-    class Config:
-        extra = Extra.allow
-
     id: Optional[str] = Field(None, description="Event ID")
     swap_total: Optional[int] = None
     swap_used: Optional[int] = None
     swap_free: Optional[float] = None
     swap_percent: Optional[float] = None
     swap_sin: Optional[int] = None
     swap_sout: Optional[int] = None
```

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/models/network.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/models/network.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # generated by datamodel-codegen:
 #   filename:  network.json
 
 from __future__ import annotations
 
 from typing import Optional
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
 
 
 class LastUpdated(BaseModel):
     """
     Last updated
     """
 
-    class Config:
-        extra = Extra.allow
-
     io_counters_bytes_sent: Optional[float] = None
     io_counters_bytes_recv: Optional[float] = None
     io_counters_packets_sent: Optional[float] = None
     io_counters_packets_recv: Optional[float] = None
     io_counters_errin: Optional[float] = None
     io_counters_errout: Optional[float] = None
     io_counters_dropin: Optional[float] = None
@@ -27,17 +24,14 @@
 
 
 class Network(BaseModel):
     """
     Network
     """
 
-    class Config:
-        extra = Extra.allow
-
     id: Optional[str] = Field(None, description="Event ID")
     io_counters_bytes_sent: Optional[int] = None
     io_counters_bytes_recv: Optional[int] = None
     io_counters_packets_sent: Optional[int] = None
     io_counters_packets_recv: Optional[int] = None
     io_counters_errin: Optional[int] = None
     io_counters_errout: Optional[int] = None
```

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/models/notification.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/models/notification.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/models/response.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/models/response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # generated by datamodel-codegen:
 #   filename:  response.json
 
 from __future__ import annotations
 
 from typing import Any, Optional
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Field
 
 
 class Response(BaseModel):
     """
     Response
     """
 
-    class Config:
-        extra = Extra.allow
-
     id: Optional[str] = Field(None, description="Message ID")
     type: str = Field(..., description="Type")
     subtype: Optional[str] = Field(None, description="Subtype")
     message: Optional[str] = Field(None, description="Message")
     module: Optional[str] = Field(None, description="Module")
     data: Optional[Any] = Field(None, description="Data")
```

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/models/system.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/models/system.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/settings.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/settings.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/update.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/update.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared/websocket_client.py` & `systembridgeshared-3.7.0.dev1/systembridgeshared/websocket_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.6.3.dev7/systembridgeshared.egg-info/SOURCES.txt` & `systembridgeshared-3.7.0.dev1/systembridgeshared.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 systembridgeshared/models/display.py
 systembridgeshared/models/generic.py
 systembridgeshared/models/get_data.py
 systembridgeshared/models/get_setting.py
 systembridgeshared/models/gpu.py
 systembridgeshared/models/keyboard_key.py
 systembridgeshared/models/keyboard_text.py
+systembridgeshared/models/media.py
 systembridgeshared/models/media_directories.py
 systembridgeshared/models/media_files.py
 systembridgeshared/models/media_get_file.py
 systembridgeshared/models/media_get_files.py
 systembridgeshared/models/media_play.py
 systembridgeshared/models/memory.py
 systembridgeshared/models/network.py
```

