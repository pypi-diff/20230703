# Comparing `tmp/sbot-0.9.0.tar.gz` & `tmp/sbot-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbot-0.9.0.tar", max compression
+gzip compressed data, was "sbot-1.0.0rc1.tar", last modified: Mon Jul  3 20:11:02 2023, max compression
```

## Comparing `sbot-0.9.0.tar` & `sbot-1.0.0rc1.tar`

### file list

```diff
@@ -1,17 +1,61 @@
--rw-r--r--   0        0        0     1072 2022-07-30 17:13:38.716637 sbot-0.9.0/LICENSE
--rw-r--r--   0        0        0     1860 2022-07-30 17:13:38.716637 sbot-0.9.0/README.md
--rw-r--r--   0        0        0     1055 2022-07-30 17:13:38.776637 sbot-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      611 2022-07-30 17:13:38.776637 sbot-0.9.0/sbot/__init__.py
--rw-r--r--   0        0        0     1832 2022-07-30 17:13:38.776637 sbot-0.9.0/sbot/env.py
--rw-r--r--   0        0        0      343 2022-07-30 17:13:38.776637 sbot-0.9.0/sbot/logging.py
--rw-r--r--   0        0        0     2615 2022-07-30 17:13:38.776637 sbot-0.9.0/sbot/metadata.py
--rw-r--r--   0        0        0       89 2022-07-30 17:13:38.776637 sbot-0.9.0/sbot/py.typed
--rw-r--r--   0        0        0     5445 2022-07-30 17:13:38.776637 sbot-0.9.0/sbot/robot.py
--rw-r--r--   0        0        0      616 2022-07-30 17:13:38.776637 sbot-0.9.0/sbot/timeout.py
--rw-r--r--   0        0        0      129 2022-07-30 17:13:38.776637 sbot-0.9.0/sbot/vision/__init__.py
--rw-r--r--   0        0        0     1607 2022-07-30 17:13:38.776637 sbot-0.9.0/sbot/vision/backend.py
--rw-r--r--   0        0        0     1254 2022-07-30 17:13:38.776637 sbot-0.9.0/sbot/vision/calibrations/Logitech C270.xml
--rw-r--r--   0        0        0       59 2022-07-30 17:13:38.776637 sbot-0.9.0/sbot/vision/calibrations/__init__.py
--rw-r--r--   0        0        0      361 2022-07-30 17:13:38.776637 sbot-0.9.0/sbot/vision/game.py
--rw-r--r--   0        0        0     2600 2022-07-30 17:14:22.555791 sbot-0.9.0/setup.py
--rw-r--r--   0        0        0     2812 2022-07-30 17:14:22.556161 sbot-0.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.747489 sbot-1.0.0rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.747489 sbot-1.0.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/.github/workflows/test_build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.747489 sbot-1.0.0rc1/sbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-03 20:11:02.000000 sbot-1.0.0rc1/sbot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/arduino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/game_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/motor_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/power_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/serial_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/servo_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/sbot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.747489 sbot-1.0.0rc1/sbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-03 20:11:02.000000 sbot-1.0.0rc1/sbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-03 20:11:02.000000 sbot-1.0.0rc1/sbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:11:02.000000 sbot-1.0.0rc1/sbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-03 20:11:02.000000 sbot-1.0.0rc1/sbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 20:11:02.000000 sbot-1.0.0rc1/sbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9535 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_arduino.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.743489 sbot-1.0.0rc1/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/tests/test_data/bad/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_data/bad/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/tests/test_data/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_data/empty/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/tests/test_data/missing_key/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_data/missing_key/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.743489 sbot-1.0.0rc1/tests/test_data/nested/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/tests/test_data/nested/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_data/nested/valid/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/tests/test_data/not_object/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_data/not_object/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:11:02.751489 sbot-1.0.0rc1/tests/test_data/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_data/valid/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_motor_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_power_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_sbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_serial_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_servo_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-03 20:10:45.000000 sbot-1.0.0rc1/tests/test_timeout.py
```

### Comparing `sbot-0.9.0/LICENSE` & `sbot-1.0.0rc1/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MIT License
 
-Copyright (c) 2019-21 Dan Trickey 
+Copyright (c) 2019-21 Dan Trickey
+Copyright (c) 2023 SourceBots
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

