# Comparing `tmp/systembridgeconnector-3.6.3.dev7.tar.gz` & `tmp/systembridgeconnector-3.7.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgeconnector-3.6.3.dev7.tar", last modified: Thu Apr 13 20:18:27 2023, max compression
+gzip compressed data, was "systembridgeconnector-3.7.0.dev1.tar", last modified: Mon Jul  3 08:32:40 2023, max compression
```

## Comparing `systembridgeconnector-3.6.3.dev7.tar` & `systembridgeconnector-3.7.0.dev1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:18:27.644997 systembridgeconnector-3.6.3.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-13 20:18:27.644997 systembridgeconnector-3.6.3.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:18:27.644997 systembridgeconnector-3.6.3.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:18:27.636996 systembridgeconnector-3.6.3.dev7/systembridgeconnector/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-13 20:18:25.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:18:27.644997 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/database_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/database_data_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/database_data_remote_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/database_data_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/display.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/get_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/keyboard_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/keyboard_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/media_directories.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/media_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/media_get_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/media_get_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/media_play.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/open_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/open_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/register_data_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/update_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17270 2023-04-13 20:18:07.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:18:27.636996 systembridgeconnector-3.6.3.dev7/systembridgeconnector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-13 20:18:27.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-13 20:18:27.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:18:27.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 20:18:27.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 20:18:27.000000 systembridgeconnector-3.6.3.dev7/systembridgeconnector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:32:40.325950 systembridgeconnector-3.7.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-03 08:32:40.325950 systembridgeconnector-3.7.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 08:32:40.325950 systembridgeconnector-3.7.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:32:40.321951 systembridgeconnector-3.7.0.dev1/systembridgeconnector/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-03 08:32:38.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:32:40.325950 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/database_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/database_data_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/database_data_remote_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/database_data_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/get_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/keyboard_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/keyboard_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/media_directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/media_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/media_get_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/media_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/media_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/open_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/open_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/register_data_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/update_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17270 2023-07-03 08:32:24.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:32:40.321951 systembridgeconnector-3.7.0.dev1/systembridgeconnector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-03 08:32:40.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-03 08:32:40.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:32:40.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 08:32:40.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 08:32:40.000000 systembridgeconnector-3.7.0.dev1/systembridgeconnector.egg-info/top_level.txt
```

### Comparing `systembridgeconnector-3.6.3.dev7/pyproject.toml` & `systembridgeconnector-3.7.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.6.3.dev7/setup.py` & `systembridgeconnector-3.7.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/const.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/const.py`

 * *Files 7% similar despite different names*

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
@@ -38,15 +39,14 @@
 QUERY_BASE = "base"
 QUERY_FILENAME = "filename"
 QUERY_PATH = "path"
 QUERY_TITLE = "title"
 QUERY_URL = "url"
 QUERY_VOLUME = "volume"
 
-
 # Event Keys
 EVENT_API_KEY = "api-key"
 EVENT_APP_ICON = "app_icon"
 EVENT_APP_NAME = "app_name"
 EVENT_BASE = "base"
 EVENT_DATA = "data"
 EVENT_DIRECTORIES = "directories"
@@ -103,14 +103,16 @@
 TYPE_EXIT_APPLICATION = "EXIT_APPLICATION"
 TYPE_FILE = "FILE"
 TYPE_FILES = "FILES"
 TYPE_GET_DATA = "GET_DATA"
 TYPE_GET_DIRECTORIES = "GET_DIRECTORIES"
 TYPE_GET_FILE = "GET_FILE"
 TYPE_GET_FILES = "GET_FILES"
+TYPE_GET_REMOTE_BRIDGES = "GET_REMOTE_BRIDGES"
+TYPE_GET_REMOTE_BRIDGES_RESULT = "GET_REMOTE_BRIDGES_RESULT"
 TYPE_GET_SETTING = "GET_SETTING"
 TYPE_GET_SETTINGS = "GET_SETTINGS"
 TYPE_KEYBOARD_KEY_PRESSED = "KEYBOARD_KEY_PRESSED"
 TYPE_KEYBOARD_KEYPRESS = "KEYBOARD_KEYPRESS"
 TYPE_KEYBOARD_TEXT = "KEYBOARD_TEXT"
 TYPE_KEYBOARD_TEXT_SENT = "KEYBOARD_TEXT_SENT"
 TYPE_NOTIFICATION = "NOTIFICATION"
@@ -130,14 +132,16 @@
 TYPE_POWER_SLEEP = "POWER_SLEEP"
 TYPE_POWER_SLEEPING = "POWER_SLEEPING"
 TYPE_REGISTER_DATA_LISTENER = "REGISTER_DATA_LISTENER"
 TYPE_SETTING_RESULT = "SETTING_RESULT"
 TYPE_SETTING_UPDATED = "SETTING_UPDATED"
 TYPE_SETTINGS_RESULT = "SETTINGS_RESULT"
 TYPE_UNREGISTER_DATA_LISTENER = "UNREGISTER_DATA_LISTENER"
+TYPE_UPDATE_REMOTE_BRIDGE = "UPDATE_REMOTE_BRIDGE"
+TYPE_UPDATE_REMOTE_BRIDGE_RESULT = "UPDATE_REMOTE_BRIDGE_RESULT"
 TYPE_UPDATE_SETTING = "UPDATE_SETTING"
 
 # Model
 MODEL_BATTERY = "battery"
 MODEL_CPU = "cpu"
 MODEL_DATA = "data"
 MODEL_DISK = "disk"
@@ -145,14 +149,15 @@
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
@@ -169,14 +174,15 @@
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

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/http_client.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/http_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/battery.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/media.py`

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

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/cpu.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/cpu.py`

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

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/data.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/data.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/database_data.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/database_data.py`

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

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/database_data_bridge.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/database_data_bridge.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/database_data_remote_bridge.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/database_data_remote_bridge.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/disk.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/disk.py`

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

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/gpu.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/battery.py`

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

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/media_files.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/media_files.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/memory.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/memory.py`

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

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/network.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/network.py`

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

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/notification.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/notification.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/response.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/response.py`

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

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/models/system.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/models/system.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/version.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/version.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector/websocket_client.py` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector/websocket_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.6.3.dev7/systembridgeconnector.egg-info/SOURCES.txt` & `systembridgeconnector-3.7.0.dev1/systembridgeconnector.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 systembridgeconnector/models/display.py
 systembridgeconnector/models/generic.py
 systembridgeconnector/models/get_data.py
 systembridgeconnector/models/get_setting.py
 systembridgeconnector/models/gpu.py
 systembridgeconnector/models/keyboard_key.py
 systembridgeconnector/models/keyboard_text.py
+systembridgeconnector/models/media.py
 systembridgeconnector/models/media_directories.py
 systembridgeconnector/models/media_files.py
 systembridgeconnector/models/media_get_file.py
 systembridgeconnector/models/media_get_files.py
 systembridgeconnector/models/media_play.py
 systembridgeconnector/models/memory.py
 systembridgeconnector/models/network.py
```

