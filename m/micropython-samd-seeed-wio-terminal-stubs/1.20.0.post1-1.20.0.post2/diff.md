# Comparing `tmp/micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1.tar.gz` & `tmp/micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1.tar", max compression
+gzip compressed data, was "micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2.tar", max compression
```

## Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1.tar` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0       92 2023-04-30 14:05:00.293142 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/_boot.pyi
--rw-r--r--   0        0        0      277 2023-05-05 18:32:00.223097 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/_onewire.pyi
--rw-r--r--   0        0        0      364 2023-05-05 18:32:00.223097 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/_uasyncio.pyi
--rw-r--r--   0        0        0     1001 2023-05-05 18:32:44.688510 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/array.pyi
--rw-r--r--   0        0        0     1406 2023-05-05 18:32:44.697439 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/binascii.pyi
--rw-r--r--   0        0        0     3638 2023-05-05 18:32:44.626052 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/collections.pyi
--rw-r--r--   0        0        0      344 2023-04-30 14:05:00.296076 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/dht.pyi
--rw-r--r--   0        0        0      404 2023-04-30 14:05:00.298292 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/ds18x20.pyi
--rw-r--r--   0        0        0      707 2023-05-05 18:32:08.219731 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/errno.pyi
--rw-r--r--   0        0        0     6347 2023-05-05 18:32:44.753963 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/framebuf.pyi
--rw-r--r--   0        0        0      927 2023-05-05 18:32:44.721216 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/gc.pyi
--rw-r--r--   0        0        0     1366 2023-05-05 18:32:44.715805 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/hashlib.pyi
--rw-r--r--   0        0        0      928 2023-05-05 18:32:44.730917 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/heapq.pyi
--rw-r--r--   0        0        0     2469 2023-05-05 18:32:44.810270 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/io.pyi
--rw-r--r--   0        0        0     1382 2023-05-05 18:32:44.776717 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/json.pyi
--rw-r--r--   0        0        0     1092 2023-05-05 18:44:57.883300 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/LICENSE.md
--rw-r--r--   0        0        0      827 2023-05-05 18:32:00.253025 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/logging.pyi
--rw-r--r--   0        0        0    47169 2023-05-05 18:32:49.839089 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/machine.pyi
--rw-r--r--   0        0        0     4652 2023-05-05 18:32:44.897671 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/math.pyi
--rw-r--r--   0        0        0     7213 2023-04-05 11:07:45.360315 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/micropython.pyi
--rw-r--r--   0        0        0      617 2023-04-30 14:05:00.301699 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/onewire.pyi
--rw-r--r--   0        0        0    10091 2023-05-05 18:32:45.034461 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/os.pyi
--rw-r--r--   0        0        0     2967 2023-05-05 18:45:00.472003 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/pyproject.toml
--rw-r--r--   0        0        0     2636 2023-05-05 18:32:44.914292 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/random.pyi
--rw-r--r--   0        0        0     2043 2023-05-05 18:44:57.857952 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/README.md
--rw-r--r--   0        0        0      467 2023-05-05 18:32:00.259541 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/samd.pyi
--rw-r--r--   0        0        0     3851 2023-05-05 18:32:23.838140 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/select.pyi
--rw-r--r--   0        0        0     4239 2023-05-05 18:32:44.966867 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/struct.pyi
--rw-r--r--   0        0        0      873 2023-05-05 18:32:45.027493 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/sys.pyi
--rw-r--r--   0        0        0    12321 2023-05-05 18:32:45.125463 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/time.pyi
--rw-r--r--   0        0        0     1001 2023-05-05 18:32:45.091848 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uarray.pyi
--rw-r--r--   0        0        0      132 2023-04-30 14:05:00.302557 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uasyncio/__init__.pyi
--rw-r--r--   0        0        0     1530 2023-04-30 14:05:00.302557 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uasyncio/core.pyi
--rw-r--r--   0        0        0      625 2023-04-30 14:05:00.302557 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uasyncio/event.pyi
--rw-r--r--   0        0        0      390 2023-04-30 14:05:00.308585 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uasyncio/funcs.pyi
--rw-r--r--   0        0        0      414 2023-04-30 14:05:00.312250 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uasyncio/lock.pyi
--rw-r--r--   0        0        0     1410 2023-04-30 14:05:00.312250 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uasyncio/stream.pyi
--rw-r--r--   0        0        0      789 2023-04-30 14:05:00.312250 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uasyncio/task.pyi
--rw-r--r--   0        0        0     1406 2023-05-05 18:32:45.178218 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/ubinascii.pyi
--rw-r--r--   0        0        0     3638 2023-05-05 18:32:45.178218 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/ucollections.pyi
--rw-r--r--   0        0        0     2361 2023-05-05 18:32:45.213190 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uctypes.pyi
--rw-r--r--   0        0        0      707 2023-05-05 18:32:29.048881 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uerrno.pyi
--rw-r--r--   0        0        0     1366 2023-05-05 18:32:45.195119 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uhashlib.pyi
--rw-r--r--   0        0        0      928 2023-05-05 18:32:45.215041 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uheapq.pyi
--rw-r--r--   0        0        0     2469 2023-05-05 18:32:45.261320 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uio.pyi
--rw-r--r--   0        0        0     1382 2023-05-05 18:32:45.229119 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/ujson.pyi
--rw-r--r--   0        0        0    47169 2023-05-05 18:32:53.367992 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/umachine.pyi
--rw-r--r--   0        0        0    10091 2023-05-05 18:32:45.459441 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uos.pyi
--rw-r--r--   0        0        0     2636 2023-05-05 18:32:45.368206 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/urandom.pyi
--rw-r--r--   0        0        0      187 2023-05-05 18:32:00.309599 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/ure.pyi
--rw-r--r--   0        0        0     3851 2023-05-05 18:32:40.339928 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uselect.pyi
--rw-r--r--   0        0        0     4239 2023-05-05 18:32:45.409598 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/ustruct.pyi
--rw-r--r--   0        0        0      873 2023-05-05 18:32:45.417486 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/usys.pyi
--rw-r--r--   0        0        0    12321 2023-05-05 18:32:45.475972 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/utime.pyi
--rw-r--r--   0        0        0     1533 2023-05-05 18:32:45.470262 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uzlib.pyi
--rw-r--r--   0        0        0     1533 2023-05-05 18:32:45.492055 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/zlib.pyi
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/setup.py
--rw-r--r--   0        0        0     3312 1970-01-01 00:00:00.000000 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/PKG-INFO
+-rw-r--r--   0        0        0       92 2023-06-07 16:29:09.875872 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/_boot.pyi
+-rw-r--r--   0        0        0      277 2023-06-07 16:29:11.338928 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/_onewire.pyi
+-rw-r--r--   0        0        0      364 2023-06-07 16:29:11.339933 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/_uasyncio.pyi
+-rw-r--r--   0        0        0     1003 2023-06-07 16:29:11.342932 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/array.pyi
+-rw-r--r--   0        0        0     1408 2023-06-07 16:29:11.343935 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/binascii.pyi
+-rw-r--r--   0        0        0     3640 2023-06-07 16:29:11.344942 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/collections.pyi
+-rw-r--r--   0        0        0      344 2023-07-03 11:19:25.001093 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/dht.pyi
+-rw-r--r--   0        0        0      404 2023-07-03 11:19:25.002094 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/ds18x20.pyi
+-rw-r--r--   0        0        0      709 2023-06-07 16:29:11.349759 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/errno.pyi
+-rw-r--r--   0        0        0     6349 2023-06-07 16:29:11.351239 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/framebuf.pyi
+-rw-r--r--   0        0        0      929 2023-06-07 16:29:11.352687 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/gc.pyi
+-rw-r--r--   0        0        0     1368 2023-06-07 16:29:11.353979 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/hashlib.pyi
+-rw-r--r--   0        0        0      930 2023-06-07 16:29:11.355185 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/heapq.pyi
+-rw-r--r--   0        0        0     2471 2023-06-07 16:29:11.356242 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/io.pyi
+-rw-r--r--   0        0        0     1384 2023-06-07 16:29:11.357520 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/json.pyi
+-rw-r--r--   0        0        0     1092 2023-07-03 13:39:27.768281 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/LICENSE.md
+-rw-r--r--   0        0        0      827 2023-06-07 16:29:11.358529 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/logging.pyi
+-rw-r--r--   0        0        0    47171 2023-06-07 16:29:11.361014 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/machine.pyi
+-rw-r--r--   0        0        0     4654 2023-06-07 16:29:11.362024 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/math.pyi
+-rw-r--r--   0        0        0     8274 2023-07-03 11:26:14.336969 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/micropython.pyi
+-rw-r--r--   0        0        0     7213 2023-07-03 11:19:19.390108 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/micropython_.pyi
+-rw-r--r--   0        0        0      617 2023-07-03 11:19:25.003514 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/onewire.pyi
+-rw-r--r--   0        0        0    10093 2023-06-07 16:29:11.365165 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/os.pyi
+-rw-r--r--   0        0        0     3005 2023-07-03 13:39:28.947704 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/pyproject.toml
+-rw-r--r--   0        0        0     2638 2023-06-07 16:29:11.367634 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/random.pyi
+-rw-r--r--   0        0        0     2030 2023-07-03 13:39:27.767289 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/README.md
+-rw-r--r--   0        0        0      467 2023-06-07 16:29:11.368636 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/samd.pyi
+-rw-r--r--   0        0        0     3853 2023-06-07 16:29:11.369683 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/select.pyi
+-rw-r--r--   0        0        0     4241 2023-06-07 16:29:11.370969 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/struct.pyi
+-rw-r--r--   0        0        0      875 2023-06-07 16:29:11.372002 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/sys.pyi
+-rw-r--r--   0        0        0    12323 2023-06-07 16:29:11.373002 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/time.pyi
+-rw-r--r--   0        0        0     1003 2023-06-07 16:29:11.373999 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uarray.pyi
+-rw-r--r--   0        0        0      132 2023-07-03 11:19:25.006521 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uasyncio/__init__.pyi
+-rw-r--r--   0        0        0     1530 2023-07-03 11:19:25.007522 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uasyncio/core.pyi
+-rw-r--r--   0        0        0      625 2023-07-03 11:19:25.008535 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uasyncio/event.pyi
+-rw-r--r--   0        0        0      390 2023-07-03 11:19:25.009520 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uasyncio/funcs.pyi
+-rw-r--r--   0        0        0      414 2023-07-03 11:19:25.011534 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uasyncio/lock.pyi
+-rw-r--r--   0        0        0     1410 2023-07-03 11:19:25.023714 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uasyncio/stream.pyi
+-rw-r--r--   0        0        0      789 2023-07-03 11:19:25.026224 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uasyncio/task.pyi
+-rw-r--r--   0        0        0     1408 2023-06-07 16:29:11.382519 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/ubinascii.pyi
+-rw-r--r--   0        0        0     3640 2023-06-07 16:29:11.384520 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/ucollections.pyi
+-rw-r--r--   0        0        0     2363 2023-06-07 16:29:11.385518 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uctypes.pyi
+-rw-r--r--   0        0        0      709 2023-06-07 16:29:11.386521 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uerrno.pyi
+-rw-r--r--   0        0        0     1368 2023-06-07 16:29:11.388522 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uhashlib.pyi
+-rw-r--r--   0        0        0      930 2023-06-07 16:29:11.389524 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uheapq.pyi
+-rw-r--r--   0        0        0     2471 2023-06-07 16:29:11.390526 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uio.pyi
+-rw-r--r--   0        0        0     1384 2023-06-07 16:29:11.391526 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/ujson.pyi
+-rw-r--r--   0        0        0    47171 2023-06-07 16:29:11.394701 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/umachine.pyi
+-rw-r--r--   0        0        0    10093 2023-06-07 16:29:11.395701 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uos.pyi
+-rw-r--r--   0        0        0     2638 2023-06-07 16:29:11.396700 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/urandom.pyi
+-rw-r--r--   0        0        0      187 2023-06-07 16:29:11.398007 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/ure.pyi
+-rw-r--r--   0        0        0     3853 2023-06-07 16:29:11.399047 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uselect.pyi
+-rw-r--r--   0        0        0     4241 2023-06-07 16:29:11.400225 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/ustruct.pyi
+-rw-r--r--   0        0        0      875 2023-06-07 16:29:11.402633 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/usys.pyi
+-rw-r--r--   0        0        0    12323 2023-06-07 16:29:11.403767 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/utime.pyi
+-rw-r--r--   0        0        0     1535 2023-06-07 16:29:11.404773 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uzlib.pyi
+-rw-r--r--   0        0        0     1535 2023-06-07 16:29:11.405827 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/zlib.pyi
+-rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/setup.py
+-rw-r--r--   0        0        0     3299 1970-01-01 00:00:00.000000 micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/PKG-INFO
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/array.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/array.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.20/library/array.html
+efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.20.0/library/array.html
 
 |see_cpython_module| :mod:`python:array` https://docs.python.org/3/library/array.html .
 
 Supported format codes: ``b``, ``B``, ``h``, ``H``, ``i``, ``I``, ``l``,
 ``L``, ``q``, ``Q``, ``f``, ``d`` (the latter 2 depending on the
 floating-point support).
 """
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/binascii.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/binascii.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-binary/ASCII conversions. See: https://docs.micropython.org/en/v1.20/library/binascii.html
+binary/ASCII conversions. See: https://docs.micropython.org/en/v1.20.0/library/binascii.html
 
 |see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
 
 This module implements conversions between binary data and various
 encodings of it in ASCII form (in both directions).
 """
 from typing import Optional, Any
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/collections.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/collections.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-collection and container types. See: https://docs.micropython.org/en/v1.20/library/collections.html
+collection and container types. See: https://docs.micropython.org/en/v1.20.0/library/collections.html
 
 |see_cpython_module| :mod:`python:collections` https://docs.python.org/3/library/collections.html .
 
 This module implements advanced collection and container types to
 hold/accumulate various objects.
 """
 from typing import Optional, Any
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/errno.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/errno.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-system error codes. See: https://docs.micropython.org/en/v1.20/library/errno.html
+system error codes. See: https://docs.micropython.org/en/v1.20.0/library/errno.html
 
 |see_cpython_module| :mod:`python:errno` https://docs.python.org/3/library/errno.html .
 
 This module provides access to symbolic error codes for `OSError` exception.
 A particular inventory of codes depends on :term:`MicroPython port`.
 """
 from typing import Any, Dict
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/framebuf.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/framebuf.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Frame buffer manipulation. See: https://docs.micropython.org/en/v1.20/library/framebuf.html
+Frame buffer manipulation. See: https://docs.micropython.org/en/v1.20.0/library/framebuf.html
 
 This module provides a general frame buffer which can be used to create
 bitmap images, which can then be sent to a display.
 """
 from typing import Optional, Any
 
 MONO_HMSB: int
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/gc.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/gc.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-control the garbage collector. See: https://docs.micropython.org/en/v1.20/library/gc.html
+control the garbage collector. See: https://docs.micropython.org/en/v1.20.0/library/gc.html
 
 |see_cpython_module| :mod:`python:gc` https://docs.python.org/3/library/gc.html .
 """
 from typing import Optional, Any
 
 def isenabled(*args, **kwargs) -> Any: ...
 def mem_free() -> int:
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/hashlib.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/hashlib.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-hashing algorithms. See: https://docs.micropython.org/en/v1.20/library/hashlib.html
+hashing algorithms. See: https://docs.micropython.org/en/v1.20.0/library/hashlib.html
 
 |see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
 
 This module implements binary data hashing algorithms. The exact inventory
 of available algorithms depends on a board. Among the algorithms which may
 be implemented:
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/heapq.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/heapq.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-heap queue algorithm. See: https://docs.micropython.org/en/v1.20/library/heapq.html
+heap queue algorithm. See: https://docs.micropython.org/en/v1.20.0/library/heapq.html
 
 |see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
 
 This module implements the
 `min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
 
 A heap queue is essentially a list that has its elements stored in such a way
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/io.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/io.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-input/output streams. See: https://docs.micropython.org/en/v1.20/library/io.html
+input/output streams. See: https://docs.micropython.org/en/v1.20.0/library/io.html
 
 |see_cpython_module| :mod:`python:io` https://docs.python.org/3/library/io.html .
 
 This module contains additional types of `stream` (file-like) objects
 and helper functions.
 """
 from typing import IO, Optional, Any
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/json.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/json.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-JSON encoding and decoding. See: https://docs.micropython.org/en/v1.20/library/json.html
+JSON encoding and decoding. See: https://docs.micropython.org/en/v1.20.0/library/json.html
 
 |see_cpython_module| :mod:`python:json` https://docs.python.org/3/library/json.html .
 
 This modules allows to convert between Python objects and the JSON
 data format.
 """
 from typing import Any
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/LICENSE.md` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/logging.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/logging.pyi`

 * *Files identical despite different names*

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/machine.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/machine.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-functions related to the hardware. See: https://docs.micropython.org/en/v1.20/library/machine.html
+functions related to the hardware. See: https://docs.micropython.org/en/v1.20.0/library/machine.html
 
 The ``machine`` module contains specific functions related to the hardware
 on a particular board. Most functions in this module allow to achieve direct
 and unrestricted access to and control of hardware blocks on a system
 (like CPU, timers, buses, etc.). Used incorrectly, this can lead to
 malfunction, lockups, crashes of your board, and in extreme cases, hardware
 damage.
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/math.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/math.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-mathematical functions. See: https://docs.micropython.org/en/v1.20/library/math.html
+mathematical functions. See: https://docs.micropython.org/en/v1.20.0/library/math.html
 
 |see_cpython_module| :mod:`python:math` https://docs.python.org/3/library/math.html .
 
 The ``math`` module provides some basic mathematical functions for
 working with floating-point numbers.
 
 *Note:* On the pyboard, floating-point numbers have 32-bit precision.
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/micropython.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/micropython_.pyi`

 * *Files identical despite different names*

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/onewire.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/onewire.pyi`

 * *Files identical despite different names*

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/os.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/os.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-basic "operating system" services. See: https://docs.micropython.org/en/v1.20/library/os.html
+basic "operating system" services. See: https://docs.micropython.org/en/v1.20.0/library/os.html
 
 |see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
 
 The ``os`` module contains functions for filesystem access and mounting,
 terminal redirection and duplication, and the ``uname`` and ``urandom``
 functions.
 """
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/pyproject.toml` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropython-samd-seeed_wio_terminal-stubs"
-version = "1.20.0.post1"
+version = "1.20.0.post2"
 description = "MicroPython stubs"
 authors = [
     "josverl <josverl@users.noreply.github.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/josverl/micropython-stubs#micropython-stubs"
@@ -47,14 +47,15 @@
     { include = "heapq.pyi" },
     { include = "io.pyi" },
     { include = "json.pyi" },
     { include = "logging.pyi" },
     { include = "machine.pyi" },
     { include = "math.pyi" },
     { include = "micropython.pyi" },
+    { include = "micropython_.pyi" },
     { include = "onewire.pyi" },
     { include = "os.pyi" },
     { include = "random.pyi" },
     { include = "samd.pyi" },
     { include = "select.pyi" },
     { include = "struct.pyi" },
     { include = "sys.pyi" },
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/random.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/random.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-random numbers. See: https://docs.micropython.org/en/v1.20/library/random.html
+random numbers. See: https://docs.micropython.org/en/v1.20.0/library/random.html
 
 This module implements a pseudo-random number generator (PRNG).
 
 |see_cpython_module| :mod:`python:random` https://docs.python.org/3/library/random.html . .
 
 .. note::
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/README.md` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
 
 For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
  * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
 
 Included stubs:
-* StubSource.MERGED from `stubs/micropython-v1_20_0-samd-seeed_wio_terminal-merged`
-* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/samd/GENERIC`
-* StubSource.CORE from `stubs/micropython-core`
+* Merged stubs from `stubs/micropython-v1_20_0-samd-seeed_wio_terminal-merged`
+* Frozen stubs from `stubs/micropython-v1_20_0-frozen/samd/GENERIC`
+* Core stubs from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
-Documentation | micropython | - | - | v1.20 
+Documentation | micropython | - | - | v1.20.0 
 Core | micropython | samd | - | v1.20.0
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/select.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/select.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-wait for events on a set of streams. See: https://docs.micropython.org/en/v1.20/library/select.html
+wait for events on a set of streams. See: https://docs.micropython.org/en/v1.20.0/library/select.html
 
 |see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
 
 This module provides functions to efficiently wait for events on multiple
 `streams <stream>` (select streams which are ready for operations).
 """
 from typing import Iterator, List, Optional, Tuple, Any
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/struct.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/struct.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-pack and unpack primitive data types. See: https://docs.micropython.org/en/v1.20/library/struct.html
+pack and unpack primitive data types. See: https://docs.micropython.org/en/v1.20.0/library/struct.html
 
 |see_cpython_module| :mod:`python:struct` https://docs.python.org/3/library/struct.html .
 
 The following byte orders are supported:
 
 +-----------+------------------------+----------+-----------+
 | Character | Byte order             | Size     | Alignment |
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/sys.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/sys.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-system specific functions. See: https://docs.micropython.org/en/v1.20/library/sys.html
+system specific functions. See: https://docs.micropython.org/en/v1.20.0/library/sys.html
 
 |see_cpython_module| :mod:`python:sys` https://docs.python.org/3/library/sys.html .
 """
 from typing import Dict, List, Tuple, Any
 
 platform: str
 version_info: tuple
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/time.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/time.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-time related functions. See: https://docs.micropython.org/en/v1.20/library/time.html
+time related functions. See: https://docs.micropython.org/en/v1.20.0/library/time.html
 
 |see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
 
 The ``time`` module provides functions for getting the current time and date,
 measuring time intervals, and for delays.
 
 **Time Epoch**: Unix port uses standard for POSIX systems epoch of
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uarray.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uarray.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.20/library/array.html
+efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.20.0/library/array.html
 
 |see_cpython_module| :mod:`python:array` https://docs.python.org/3/library/array.html .
 
 Supported format codes: ``b``, ``B``, ``h``, ``H``, ``i``, ``I``, ``l``,
 ``L``, ``q``, ``Q``, ``f``, ``d`` (the latter 2 depending on the
 floating-point support).
 """
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uasyncio/core.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uasyncio/core.pyi`

 * *Files identical despite different names*

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uasyncio/event.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uasyncio/event.pyi`

 * *Files identical despite different names*

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uasyncio/stream.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uasyncio/stream.pyi`

 * *Files identical despite different names*

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uasyncio/task.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uasyncio/task.pyi`

 * *Files identical despite different names*

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/ubinascii.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/ubinascii.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-binary/ASCII conversions. See: https://docs.micropython.org/en/v1.20/library/binascii.html
+binary/ASCII conversions. See: https://docs.micropython.org/en/v1.20.0/library/binascii.html
 
 |see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
 
 This module implements conversions between binary data and various
 encodings of it in ASCII form (in both directions).
 """
 from typing import Optional, Any
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/ucollections.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/ucollections.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-collection and container types. See: https://docs.micropython.org/en/v1.20/library/collections.html
+collection and container types. See: https://docs.micropython.org/en/v1.20.0/library/collections.html
 
 |see_cpython_module| :mod:`python:collections` https://docs.python.org/3/library/collections.html .
 
 This module implements advanced collection and container types to
 hold/accumulate various objects.
 """
 from typing import Optional, Any
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uctypes.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uctypes.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-access binary data in a structured way. See: https://docs.micropython.org/en/v1.20/library/uctypes.html
+access binary data in a structured way. See: https://docs.micropython.org/en/v1.20.0/library/uctypes.html
 
 This module implements "foreign data interface" for MicroPython. The idea
 behind it is similar to CPython's ``ctypes`` modules, but the actual API is
 different, streamlined and optimized for small size. The basic idea of the
 module is to define data structure layout with about the same power as the
 C language allows, and then access it using familiar dot-syntax to reference
 sub-fields.
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uerrno.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uerrno.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-system error codes. See: https://docs.micropython.org/en/v1.20/library/errno.html
+system error codes. See: https://docs.micropython.org/en/v1.20.0/library/errno.html
 
 |see_cpython_module| :mod:`python:errno` https://docs.python.org/3/library/errno.html .
 
 This module provides access to symbolic error codes for `OSError` exception.
 A particular inventory of codes depends on :term:`MicroPython port`.
 """
 from typing import Any, Dict
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uhashlib.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uhashlib.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-hashing algorithms. See: https://docs.micropython.org/en/v1.20/library/hashlib.html
+hashing algorithms. See: https://docs.micropython.org/en/v1.20.0/library/hashlib.html
 
 |see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
 
 This module implements binary data hashing algorithms. The exact inventory
 of available algorithms depends on a board. Among the algorithms which may
 be implemented:
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uheapq.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uheapq.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-heap queue algorithm. See: https://docs.micropython.org/en/v1.20/library/heapq.html
+heap queue algorithm. See: https://docs.micropython.org/en/v1.20.0/library/heapq.html
 
 |see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
 
 This module implements the
 `min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
 
 A heap queue is essentially a list that has its elements stored in such a way
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uio.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uio.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-input/output streams. See: https://docs.micropython.org/en/v1.20/library/io.html
+input/output streams. See: https://docs.micropython.org/en/v1.20.0/library/io.html
 
 |see_cpython_module| :mod:`python:io` https://docs.python.org/3/library/io.html .
 
 This module contains additional types of `stream` (file-like) objects
 and helper functions.
 """
 from typing import IO, Optional, Any
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/ujson.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/ujson.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-JSON encoding and decoding. See: https://docs.micropython.org/en/v1.20/library/json.html
+JSON encoding and decoding. See: https://docs.micropython.org/en/v1.20.0/library/json.html
 
 |see_cpython_module| :mod:`python:json` https://docs.python.org/3/library/json.html .
 
 This modules allows to convert between Python objects and the JSON
 data format.
 """
 from typing import Any
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/umachine.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/umachine.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-functions related to the hardware. See: https://docs.micropython.org/en/v1.20/library/machine.html
+functions related to the hardware. See: https://docs.micropython.org/en/v1.20.0/library/machine.html
 
 The ``machine`` module contains specific functions related to the hardware
 on a particular board. Most functions in this module allow to achieve direct
 and unrestricted access to and control of hardware blocks on a system
 (like CPU, timers, buses, etc.). Used incorrectly, this can lead to
 malfunction, lockups, crashes of your board, and in extreme cases, hardware
 damage.
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uos.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uos.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-basic "operating system" services. See: https://docs.micropython.org/en/v1.20/library/os.html
+basic "operating system" services. See: https://docs.micropython.org/en/v1.20.0/library/os.html
 
 |see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
 
 The ``os`` module contains functions for filesystem access and mounting,
 terminal redirection and duplication, and the ``uname`` and ``urandom``
 functions.
 """
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/urandom.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/urandom.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-random numbers. See: https://docs.micropython.org/en/v1.20/library/random.html
+random numbers. See: https://docs.micropython.org/en/v1.20.0/library/random.html
 
 This module implements a pseudo-random number generator (PRNG).
 
 |see_cpython_module| :mod:`python:random` https://docs.python.org/3/library/random.html . .
 
 .. note::
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uselect.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uselect.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-wait for events on a set of streams. See: https://docs.micropython.org/en/v1.20/library/select.html
+wait for events on a set of streams. See: https://docs.micropython.org/en/v1.20.0/library/select.html
 
 |see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
 
 This module provides functions to efficiently wait for events on multiple
 `streams <stream>` (select streams which are ready for operations).
 """
 from typing import Iterator, List, Optional, Tuple, Any
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/ustruct.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/ustruct.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-pack and unpack primitive data types. See: https://docs.micropython.org/en/v1.20/library/struct.html
+pack and unpack primitive data types. See: https://docs.micropython.org/en/v1.20.0/library/struct.html
 
 |see_cpython_module| :mod:`python:struct` https://docs.python.org/3/library/struct.html .
 
 The following byte orders are supported:
 
 +-----------+------------------------+----------+-----------+
 | Character | Byte order             | Size     | Alignment |
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/usys.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/usys.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-system specific functions. See: https://docs.micropython.org/en/v1.20/library/sys.html
+system specific functions. See: https://docs.micropython.org/en/v1.20.0/library/sys.html
 
 |see_cpython_module| :mod:`python:sys` https://docs.python.org/3/library/sys.html .
 """
 from typing import Dict, List, Tuple, Any
 
 platform: str
 version_info: tuple
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/utime.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/utime.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-time related functions. See: https://docs.micropython.org/en/v1.20/library/time.html
+time related functions. See: https://docs.micropython.org/en/v1.20.0/library/time.html
 
 |see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
 
 The ``time`` module provides functions for getting the current time and date,
 measuring time intervals, and for delays.
 
 **Time Epoch**: Unix port uses standard for POSIX systems epoch of
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/uzlib.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/uzlib.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-zlib decompression. See: https://docs.micropython.org/en/v1.20/library/zlib.html
+zlib decompression. See: https://docs.micropython.org/en/v1.20.0/library/zlib.html
 
 |see_cpython_module| :mod:`python:zlib` https://docs.python.org/3/library/zlib.html .
 
 This module allows to decompress binary data compressed with
 `DEFLATE algorithm <https://en.wikipedia.org/wiki/DEFLATE>`_
 (commonly used in zlib library and gzip archiver). Compression
 is not yet implemented.
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/zlib.pyi` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/zlib.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-zlib decompression. See: https://docs.micropython.org/en/v1.20/library/zlib.html
+zlib decompression. See: https://docs.micropython.org/en/v1.20.0/library/zlib.html
 
 |see_cpython_module| :mod:`python:zlib` https://docs.python.org/3/library/zlib.html .
 
 This module allows to decompress binary data compressed with
 `DEFLATE algorithm <https://en.wikipedia.org/wiki/DEFLATE>`_
 (commonly used in zlib library and gzip archiver). Compression
 is not yet implemented.
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/setup.py` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
  'heapq',
  'io',
  'json',
  'logging',
  'machine',
  'math',
  'micropython',
+ 'micropython_',
  'onewire',
  'os',
  'random',
  'samd',
  'select',
  'struct',
  'sys',
@@ -56,17 +57,17 @@
  'uzlib',
  'zlib']
 install_requires = \
 ['micropython-stdlib-stubs>=0.9.0']
 
 setup_kwargs = {
     'name': 'micropython-samd-seeed-wio-terminal-stubs',
-    'version': '1.20.0.post1',
+    'version': '1.20.0.post2',
     'description': 'MicroPython stubs',
-    'long_description': '# micropython-samd-seeed_wio_terminal-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* StubSource.MERGED from `stubs/micropython-v1_20_0-samd-seeed_wio_terminal-merged`\n* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/samd/GENERIC`\n* StubSource.CORE from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nDocumentation | micropython | - | - | v1.20 \nCore | micropython | samd | - | v1.20.0 \n',
+    'long_description': '# micropython-samd-seeed_wio_terminal-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* Merged stubs from `stubs/micropython-v1_20_0-samd-seeed_wio_terminal-merged`\n* Frozen stubs from `stubs/micropython-v1_20_0-frozen/samd/GENERIC`\n* Core stubs from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nDocumentation | micropython | - | - | v1.20.0 \nCore | micropython | samd | - | v1.20.0 \n',
     'author': 'josverl',
     'author_email': 'josverl@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josverl/micropython-stubs#micropython-stubs',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post1/PKG-INFO` & `micropython_samd_seeed_wio_terminal_stubs-1.20.0.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-samd-seeed-wio-terminal-stubs
-Version: 1.20.0.post1
+Version: 1.20.0.post2
 Summary: MicroPython stubs
 Home-page: https://github.com/josverl/micropython-stubs#micropython-stubs
 License: MIT
 Author: josverl
 Author-email: josverl@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -52,17 +52,17 @@
 
 If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
 
 For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
  * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
 
 Included stubs:
-* StubSource.MERGED from `stubs/micropython-v1_20_0-samd-seeed_wio_terminal-merged`
-* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/samd/GENERIC`
-* StubSource.CORE from `stubs/micropython-core`
+* Merged stubs from `stubs/micropython-v1_20_0-samd-seeed_wio_terminal-merged`
+* Frozen stubs from `stubs/micropython-v1_20_0-frozen/samd/GENERIC`
+* Core stubs from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
-Documentation | micropython | - | - | v1.20 
+Documentation | micropython | - | - | v1.20.0 
 Core | micropython | samd | - | v1.20.0
```

