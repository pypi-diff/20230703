# Comparing `tmp/systembridgebackend-3.6.3.dev7.tar.gz` & `tmp/systembridgebackend-3.7.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgebackend-3.6.3.dev7.tar", last modified: Thu Apr 13 20:19:39 2023, max compression
+gzip compressed data, was "systembridgebackend-3.7.0.dev1.tar", last modified: Mon Jul  3 08:33:46 2023, max compression
```

## Comparing `systembridgebackend-3.6.3.dev7.tar` & `systembridgebackend-3.7.0.dev1.tar`

### file list

```diff
@@ -1,73 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.346843 systembridgebackend-3.6.3.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-13 20:19:39.346843 systembridgebackend-3.6.3.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:19:39.346843 systembridgebackend-3.6.3.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.338842 systembridgebackend-3.6.3.dev7/systembridgebackend/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-13 20:19:37.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)   102485 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.338842 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.338842 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/battery/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/battery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/battery/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.338842 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/cpu/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.338842 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/disk/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/disk/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.342842 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/display/
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/display/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.342842 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/gpu/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/listeners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.342842 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/memory/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/memory/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.342842 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/network/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/network/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.342842 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/sensors/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.342842 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/system/
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/system/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/modules/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.342842 systembridgebackend-3.6.3.dev7/systembridgebackend/server/
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/server/mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/server/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.342842 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/action.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.346843 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/autostart/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/autostart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/autostart/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/autostart/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/power.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/remote_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.346843 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/shortcuts/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/shortcuts/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 20:19:23.000000 systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:19:39.338842 systembridgebackend-3.6.3.dev7/systembridgebackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-13 20:19:39.000000 systembridgebackend-3.6.3.dev7/systembridgebackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-13 20:19:39.000000 systembridgebackend-3.6.3.dev7/systembridgebackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:19:39.000000 systembridgebackend-3.6.3.dev7/systembridgebackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-13 20:19:39.000000 systembridgebackend-3.6.3.dev7/systembridgebackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 20:19:39.000000 systembridgebackend-3.6.3.dev7/systembridgebackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.475296 systembridgebackend-3.7.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-03 08:33:46.475296 systembridgebackend-3.7.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 08:33:46.475296 systembridgebackend-3.7.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.471296 systembridgebackend-3.7.0.dev1/systembridgebackend/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-03 08:33:44.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102485 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.471296 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.471296 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/battery/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/battery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/battery/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.471296 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/cpu/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.471296 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/disk/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/disk/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.471296 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/display/
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/display/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.471296 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/gpu/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/listeners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.471296 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/media/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.471296 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/memory/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.471296 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/network/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.471296 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/sensors/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.471296 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/system/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/modules/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.475296 systembridgebackend-3.7.0.dev1/systembridgebackend/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/server/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/server/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.475296 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/action.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.475296 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/autostart/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/autostart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/autostart/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/autostart/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/remote_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.475296 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/shortcuts/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/shortcuts/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-03 08:33:28.000000 systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:46.471296 systembridgebackend-3.7.0.dev1/systembridgebackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-03 08:33:46.000000 systembridgebackend-3.7.0.dev1/systembridgebackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-03 08:33:46.000000 systembridgebackend-3.7.0.dev1/systembridgebackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:33:46.000000 systembridgebackend-3.7.0.dev1/systembridgebackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-03 08:33:46.000000 systembridgebackend-3.7.0.dev1/systembridgebackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 08:33:46.000000 systembridgebackend-3.7.0.dev1/systembridgebackend.egg-info/top_level.txt
```

### Comparing `systembridgebackend-3.6.3.dev7/pyproject.toml` & `systembridgebackend-3.7.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/setup.py` & `systembridgebackend-3.7.0.dev1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 """Setup"""
 import io
+import platform
 
 from setuptools import find_packages, setup
 
 # Get setup packages from requirements.txt
 with io.open("requirements_setup.txt", encoding="utf-8") as f:
     requirements_setup = f.read().splitlines()
 
 # Get packages from requirements.txt
 with io.open("requirements.txt", encoding="utf-8") as f:
     requirements = f.read().splitlines()
 
+# Add windows specific requirements if applicable
+if platform.system() == "Windows":
+    with io.open("requirements_windows.txt", encoding="utf-8") as f:
+        requirements.extend(f.read().splitlines())
+
+
 package_data = ["icon.png", "icon.ico"]
 
 setup(
     name="systembridgebackend",
     description="System Bridge Backend",
     keywords="system bridge backend",
     author="Aidan Timson (Timmo)",
```

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/__main__.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/__main__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/data.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/data.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/gui.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/gui.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/icon.ico` & `systembridgebackend-3.7.0.dev1/systembridgebackend/icon.ico`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/icon.png` & `systembridgebackend-3.7.0.dev1/systembridgebackend/icon.png`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/battery/__init__.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/battery/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/battery/update.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/battery/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/cpu/__init__.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/cpu/update.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/cpu/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/disk/__init__.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/disk/update.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/disk/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/display/__init__.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/display/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/display/update.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/display/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/gpu/__init__.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/gpu/update.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/gpu/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/listeners.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/listeners.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/memory/update.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/memory/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/network/__init__.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/network/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/network/update.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/network/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/sensors/__init__.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/sensors/update.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/sensors/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/system/__init__.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/system/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/system/update.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/system/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/modules/update.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/modules/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from systembridgeshared.database import Database
 
 from .battery.update import BatteryUpdate
 from .cpu.update import CPUUpdate
 from .disk.update import DiskUpdate
 from .display.update import DisplayUpdate
 from .gpu.update import GPUUpdate
+from .media.update import MediaUpdate
 from .memory.update import MemoryUpdate
 from .network.update import NetworkUpdate
 from .sensors.update import SensorsUpdate
 from .system.update import SystemUpdate
 
 
 class Update(Base):
@@ -32,14 +33,15 @@
             {"name": "disk", "cls": DiskUpdate(self._database)},
             {"name": "system", "cls": SystemUpdate(self._database)},
         ]
         self._classes_frequent = [
             {"name": "cpu", "cls": CPUUpdate(self._database)},
             {"name": "display", "cls": DisplayUpdate(self._database)},
             {"name": "gpu", "cls": GPUUpdate(self._database)},
+            {"name": "media", "cls": MediaUpdate(self._database)},
             {"name": "memory", "cls": MemoryUpdate(self._database)},
             {"name": "network", "cls": NetworkUpdate(self._database)},
         ]
 
     async def _update(
         self,
         class_obj: dict,
```

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/server/__init__.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/server/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/server/api.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/server/api.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/server/mdns.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/server/mdns.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/server/websocket.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/server/websocket.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/action.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/action.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/autostart/__init__.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/autostart/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/autostart/linux.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/autostart/linux.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/autostart/windows.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/autostart/windows.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/keyboard.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/keyboard.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/media.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/media.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/power.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/power.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/shortcuts/linux.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/shortcuts/linux.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend/utilities/shortcuts/windows.py` & `systembridgebackend-3.7.0.dev1/systembridgebackend/utilities/shortcuts/windows.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.6.3.dev7/systembridgebackend.egg-info/SOURCES.txt` & `systembridgebackend-3.7.0.dev1/systembridgebackend.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 systembridgebackend/modules/cpu/update.py
 systembridgebackend/modules/disk/__init__.py
 systembridgebackend/modules/disk/update.py
 systembridgebackend/modules/display/__init__.py
 systembridgebackend/modules/display/update.py
 systembridgebackend/modules/gpu/__init__.py
 systembridgebackend/modules/gpu/update.py
+systembridgebackend/modules/media/__init__.py
+systembridgebackend/modules/media/update.py
 systembridgebackend/modules/memory/__init__.py
 systembridgebackend/modules/memory/update.py
 systembridgebackend/modules/network/__init__.py
 systembridgebackend/modules/network/update.py
 systembridgebackend/modules/sensors/__init__.py
 systembridgebackend/modules/sensors/update.py
 systembridgebackend/modules/system/__init__.py
```

