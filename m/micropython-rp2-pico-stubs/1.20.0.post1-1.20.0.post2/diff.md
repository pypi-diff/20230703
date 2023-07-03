# Comparing `tmp/micropython_rp2_pico_stubs-1.20.0.post1.tar.gz` & `tmp/micropython_rp2_pico_stubs-1.20.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_rp2_pico_stubs-1.20.0.post1.tar", max compression
+gzip compressed data, was "micropython_rp2_pico_stubs-1.20.0.post2.tar", max compression
```

## Comparing `micropython_rp2_pico_stubs-1.20.0.post1.tar` & `micropython_rp2_pico_stubs-1.20.0.post2.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0       71 2023-04-30 14:05:00.188832 micropython_rp2_pico_stubs-1.20.0.post1/_boot.pyi
--rw-r--r--   0        0        0       71 2023-04-30 14:05:00.189851 micropython_rp2_pico_stubs-1.20.0.post1/_boot_fat.pyi
--rw-r--r--   0        0        0      277 2023-05-04 20:38:22.139418 micropython_rp2_pico_stubs-1.20.0.post1/_onewire.pyi
--rw-r--r--   0        0        0     1364 2023-05-04 20:38:22.142263 micropython_rp2_pico_stubs-1.20.0.post1/_rp2.pyi
--rw-r--r--   0        0        0      846 2023-05-04 20:40:12.524123 micropython_rp2_pico_stubs-1.20.0.post1/_thread.pyi
--rw-r--r--   0        0        0      364 2023-05-04 20:38:22.145609 micropython_rp2_pico_stubs-1.20.0.post1/_uasyncio.pyi
--rw-r--r--   0        0        0     1001 2023-05-04 20:40:27.521042 micropython_rp2_pico_stubs-1.20.0.post1/array.pyi
--rw-r--r--   0        0        0     1406 2023-05-04 20:40:27.716052 micropython_rp2_pico_stubs-1.20.0.post1/binascii.pyi
--rw-r--r--   0        0        0     1452 2023-05-04 20:40:27.668966 micropython_rp2_pico_stubs-1.20.0.post1/cmath.pyi
--rw-r--r--   0        0        0     3638 2023-05-04 20:40:27.548661 micropython_rp2_pico_stubs-1.20.0.post1/collections.pyi
--rw-r--r--   0        0        0     1645 2023-05-04 20:40:13.769245 micropython_rp2_pico_stubs-1.20.0.post1/cryptolib.pyi
--rw-r--r--   0        0        0      344 2023-04-30 14:05:00.193359 micropython_rp2_pico_stubs-1.20.0.post1/dht.pyi
--rw-r--r--   0        0        0      404 2023-04-30 14:05:00.193359 micropython_rp2_pico_stubs-1.20.0.post1/ds18x20.pyi
--rw-r--r--   0        0        0      707 2023-05-04 20:40:13.944851 micropython_rp2_pico_stubs-1.20.0.post1/errno.pyi
--rw-r--r--   0        0        0     6347 2023-05-04 20:40:27.602532 micropython_rp2_pico_stubs-1.20.0.post1/framebuf.pyi
--rw-r--r--   0        0        0     1991 2023-05-04 20:40:27.602532 micropython_rp2_pico_stubs-1.20.0.post1/gc.pyi
--rw-r--r--   0        0        0     1640 2023-05-04 20:40:27.625948 micropython_rp2_pico_stubs-1.20.0.post1/hashlib.pyi
--rw-r--r--   0        0        0      928 2023-05-04 20:40:27.644871 micropython_rp2_pico_stubs-1.20.0.post1/heapq.pyi
--rw-r--r--   0        0        0     2469 2023-05-04 20:40:27.691392 micropython_rp2_pico_stubs-1.20.0.post1/io.pyi
--rw-r--r--   0        0        0     1382 2023-05-04 20:40:27.675380 micropython_rp2_pico_stubs-1.20.0.post1/json.pyi
--rw-r--r--   0        0        0     1092 2023-05-04 20:46:09.641328 micropython_rp2_pico_stubs-1.20.0.post1/LICENSE.md
--rw-r--r--   0        0        0      827 2023-05-04 20:38:22.175385 micropython_rp2_pico_stubs-1.20.0.post1/logging.pyi
--rw-r--r--   0        0        0    49173 2023-05-04 20:40:30.663227 micropython_rp2_pico_stubs-1.20.0.post1/machine.pyi
--rw-r--r--   0        0        0     4652 2023-05-04 20:40:27.976002 micropython_rp2_pico_stubs-1.20.0.post1/math.pyi
--rw-r--r--   0        0        0     7213 2023-04-05 11:07:45.360315 micropython_rp2_pico_stubs-1.20.0.post1/micropython.pyi
--rw-r--r--   0        0        0      448 2023-04-30 14:05:00.199241 micropython_rp2_pico_stubs-1.20.0.post1/neopixel.pyi
--rw-r--r--   0        0        0      617 2023-04-30 14:05:00.201127 micropython_rp2_pico_stubs-1.20.0.post1/onewire.pyi
--rw-r--r--   0        0        0     9305 2023-05-04 20:40:27.968001 micropython_rp2_pico_stubs-1.20.0.post1/os.pyi
--rw-r--r--   0        0        0     3185 2023-05-04 20:46:11.485189 micropython_rp2_pico_stubs-1.20.0.post1/pyproject.toml
--rw-r--r--   0        0        0     2636 2023-05-04 20:40:27.984002 micropython_rp2_pico_stubs-1.20.0.post1/random.pyi
--rw-r--r--   0        0        0     2011 2023-05-04 20:46:09.641328 micropython_rp2_pico_stubs-1.20.0.post1/README.md
--rw-r--r--   0        0        0     1918 2023-04-30 14:05:00.202944 micropython_rp2_pico_stubs-1.20.0.post1/rp2.pyi
--rw-r--r--   0        0        0     3851 2023-05-04 20:40:19.371166 micropython_rp2_pico_stubs-1.20.0.post1/select.pyi
--rw-r--r--   0        0        0     4239 2023-05-04 20:40:28.023954 micropython_rp2_pico_stubs-1.20.0.post1/struct.pyi
--rw-r--r--   0        0        0      873 2023-05-04 20:40:28.047972 micropython_rp2_pico_stubs-1.20.0.post1/sys.pyi
--rw-r--r--   0        0        0    12513 2023-05-04 20:40:28.116421 micropython_rp2_pico_stubs-1.20.0.post1/time.pyi
--rw-r--r--   0        0        0     1001 2023-05-04 20:40:28.059226 micropython_rp2_pico_stubs-1.20.0.post1/uarray.pyi
--rw-r--r--   0        0        0      132 2023-04-30 14:05:00.203475 micropython_rp2_pico_stubs-1.20.0.post1/uasyncio/__init__.pyi
--rw-r--r--   0        0        0     1530 2023-04-30 14:05:00.207637 micropython_rp2_pico_stubs-1.20.0.post1/uasyncio/core.pyi
--rw-r--r--   0        0        0      625 2023-04-30 14:05:00.210009 micropython_rp2_pico_stubs-1.20.0.post1/uasyncio/event.pyi
--rw-r--r--   0        0        0      390 2023-04-30 14:05:00.211770 micropython_rp2_pico_stubs-1.20.0.post1/uasyncio/funcs.pyi
--rw-r--r--   0        0        0      414 2023-04-30 14:05:00.211770 micropython_rp2_pico_stubs-1.20.0.post1/uasyncio/lock.pyi
--rw-r--r--   0        0        0     1410 2023-04-30 14:05:00.211770 micropython_rp2_pico_stubs-1.20.0.post1/uasyncio/stream.pyi
--rw-r--r--   0        0        0      789 2023-04-30 14:05:00.217879 micropython_rp2_pico_stubs-1.20.0.post1/uasyncio/task.pyi
--rw-r--r--   0        0        0     1406 2023-05-04 20:40:28.102698 micropython_rp2_pico_stubs-1.20.0.post1/ubinascii.pyi
--rw-r--r--   0        0        0     3638 2023-05-04 20:40:28.185108 micropython_rp2_pico_stubs-1.20.0.post1/ucollections.pyi
--rw-r--r--   0        0        0     1645 2023-05-04 20:40:20.980480 micropython_rp2_pico_stubs-1.20.0.post1/ucryptolib.pyi
--rw-r--r--   0        0        0     2361 2023-05-04 20:40:28.156241 micropython_rp2_pico_stubs-1.20.0.post1/uctypes.pyi
--rw-r--r--   0        0        0      707 2023-05-04 20:40:21.394080 micropython_rp2_pico_stubs-1.20.0.post1/uerrno.pyi
--rw-r--r--   0        0        0     1640 2023-05-04 20:40:28.207079 micropython_rp2_pico_stubs-1.20.0.post1/uhashlib.pyi
--rw-r--r--   0        0        0      928 2023-05-04 20:40:28.213591 micropython_rp2_pico_stubs-1.20.0.post1/uheapq.pyi
--rw-r--r--   0        0        0     2469 2023-05-04 20:40:28.286266 micropython_rp2_pico_stubs-1.20.0.post1/uio.pyi
--rw-r--r--   0        0        0     1382 2023-05-04 20:40:28.229637 micropython_rp2_pico_stubs-1.20.0.post1/ujson.pyi
--rw-r--r--   0        0        0    49173 2023-05-04 20:40:32.735426 micropython_rp2_pico_stubs-1.20.0.post1/umachine.pyi
--rw-r--r--   0        0        0     9305 2023-05-04 20:40:28.399776 micropython_rp2_pico_stubs-1.20.0.post1/uos.pyi
--rw-r--r--   0        0        0     2636 2023-05-04 20:40:28.358338 micropython_rp2_pico_stubs-1.20.0.post1/urandom.pyi
--rw-r--r--   0        0        0      187 2023-05-04 20:38:22.241008 micropython_rp2_pico_stubs-1.20.0.post1/ure.pyi
--rw-r--r--   0        0        0     3851 2023-05-04 20:40:24.875988 micropython_rp2_pico_stubs-1.20.0.post1/uselect.pyi
--rw-r--r--   0        0        0     4239 2023-05-04 20:40:28.407314 micropython_rp2_pico_stubs-1.20.0.post1/ustruct.pyi
--rw-r--r--   0        0        0      873 2023-05-04 20:40:28.407314 micropython_rp2_pico_stubs-1.20.0.post1/usys.pyi
--rw-r--r--   0        0        0    12513 2023-05-04 20:40:28.482651 micropython_rp2_pico_stubs-1.20.0.post1/utime.pyi
--rw-r--r--   0        0        0     1533 2023-05-04 20:40:28.439119 micropython_rp2_pico_stubs-1.20.0.post1/uzlib.pyi
--rw-r--r--   0        0        0     1533 2023-05-04 20:40:28.457333 micropython_rp2_pico_stubs-1.20.0.post1/zlib.pyi
--rw-r--r--   0        0        0     3299 1970-01-01 00:00:00.000000 micropython_rp2_pico_stubs-1.20.0.post1/setup.py
--rw-r--r--   0        0        0     3265 1970-01-01 00:00:00.000000 micropython_rp2_pico_stubs-1.20.0.post1/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-06-07 16:29:09.755582 micropython_rp2_pico_stubs-1.20.0.post2/_boot.pyi
+-rw-r--r--   0        0        0       71 2023-06-07 16:29:09.756991 micropython_rp2_pico_stubs-1.20.0.post2/_boot_fat.pyi
+-rw-r--r--   0        0        0      277 2023-06-07 16:29:10.351310 micropython_rp2_pico_stubs-1.20.0.post2/_onewire.pyi
+-rw-r--r--   0        0        0     1364 2023-06-07 16:29:10.352305 micropython_rp2_pico_stubs-1.20.0.post2/_rp2.pyi
+-rw-r--r--   0        0        0      846 2023-06-07 16:29:10.353306 micropython_rp2_pico_stubs-1.20.0.post2/_thread.pyi
+-rw-r--r--   0        0        0      364 2023-06-07 16:29:10.354787 micropython_rp2_pico_stubs-1.20.0.post2/_uasyncio.pyi
+-rw-r--r--   0        0        0     1001 2023-06-07 16:29:10.355995 micropython_rp2_pico_stubs-1.20.0.post2/array.pyi
+-rw-r--r--   0        0        0     1406 2023-06-07 16:29:10.357337 micropython_rp2_pico_stubs-1.20.0.post2/binascii.pyi
+-rw-r--r--   0        0        0     1452 2023-06-07 16:29:10.357337 micropython_rp2_pico_stubs-1.20.0.post2/cmath.pyi
+-rw-r--r--   0        0        0     3638 2023-06-07 16:29:10.358497 micropython_rp2_pico_stubs-1.20.0.post2/collections.pyi
+-rw-r--r--   0        0        0     1645 2023-06-07 16:29:10.360502 micropython_rp2_pico_stubs-1.20.0.post2/cryptolib.pyi
+-rw-r--r--   0        0        0      344 2023-06-07 16:29:09.758150 micropython_rp2_pico_stubs-1.20.0.post2/dht.pyi
+-rw-r--r--   0        0        0      404 2023-06-07 16:29:09.759157 micropython_rp2_pico_stubs-1.20.0.post2/ds18x20.pyi
+-rw-r--r--   0        0        0      707 2023-06-07 16:29:10.364502 micropython_rp2_pico_stubs-1.20.0.post2/errno.pyi
+-rw-r--r--   0        0        0     6347 2023-06-07 16:29:10.366504 micropython_rp2_pico_stubs-1.20.0.post2/framebuf.pyi
+-rw-r--r--   0        0        0     1991 2023-06-07 16:29:10.367507 micropython_rp2_pico_stubs-1.20.0.post2/gc.pyi
+-rw-r--r--   0        0        0     1640 2023-06-07 16:29:10.369505 micropython_rp2_pico_stubs-1.20.0.post2/hashlib.pyi
+-rw-r--r--   0        0        0      928 2023-06-07 16:29:10.370502 micropython_rp2_pico_stubs-1.20.0.post2/heapq.pyi
+-rw-r--r--   0        0        0     2469 2023-06-07 16:29:10.371509 micropython_rp2_pico_stubs-1.20.0.post2/io.pyi
+-rw-r--r--   0        0        0     1382 2023-06-07 16:29:10.372505 micropython_rp2_pico_stubs-1.20.0.post2/json.pyi
+-rw-r--r--   0        0        0     1092 2023-07-03 13:38:27.694533 micropython_rp2_pico_stubs-1.20.0.post2/LICENSE.md
+-rw-r--r--   0        0        0      827 2023-06-07 16:29:10.373502 micropython_rp2_pico_stubs-1.20.0.post2/logging.pyi
+-rw-r--r--   0        0        0    49173 2023-06-07 16:29:10.375502 micropython_rp2_pico_stubs-1.20.0.post2/machine.pyi
+-rw-r--r--   0        0        0     4652 2023-06-07 16:29:10.376504 micropython_rp2_pico_stubs-1.20.0.post2/math.pyi
+-rw-r--r--   0        0        0     8274 2023-07-03 11:26:14.336969 micropython_rp2_pico_stubs-1.20.0.post2/micropython.pyi
+-rw-r--r--   0        0        0     7213 2023-07-03 11:19:19.390108 micropython_rp2_pico_stubs-1.20.0.post2/micropython_.pyi
+-rw-r--r--   0        0        0      448 2023-06-07 16:29:09.760540 micropython_rp2_pico_stubs-1.20.0.post2/neopixel.pyi
+-rw-r--r--   0        0        0      617 2023-06-07 16:29:09.761978 micropython_rp2_pico_stubs-1.20.0.post2/onewire.pyi
+-rw-r--r--   0        0        0     9305 2023-06-07 16:29:10.395427 micropython_rp2_pico_stubs-1.20.0.post2/os.pyi
+-rw-r--r--   0        0        0     3223 2023-07-03 13:38:28.863451 micropython_rp2_pico_stubs-1.20.0.post2/pyproject.toml
+-rw-r--r--   0        0        0     2636 2023-06-07 16:29:10.396857 micropython_rp2_pico_stubs-1.20.0.post2/random.pyi
+-rw-r--r--   0        0        0     1996 2023-07-03 13:38:27.694021 micropython_rp2_pico_stubs-1.20.0.post2/README.md
+-rw-r--r--   0        0        0     1918 2023-06-07 16:29:09.762992 micropython_rp2_pico_stubs-1.20.0.post2/rp2.pyi
+-rw-r--r--   0        0        0     3851 2023-06-07 16:29:10.399967 micropython_rp2_pico_stubs-1.20.0.post2/select.pyi
+-rw-r--r--   0        0        0     4239 2023-06-07 16:29:10.402352 micropython_rp2_pico_stubs-1.20.0.post2/struct.pyi
+-rw-r--r--   0        0        0      873 2023-06-07 16:29:10.404357 micropython_rp2_pico_stubs-1.20.0.post2/sys.pyi
+-rw-r--r--   0        0        0    12513 2023-06-07 16:29:10.405825 micropython_rp2_pico_stubs-1.20.0.post2/time.pyi
+-rw-r--r--   0        0        0     1001 2023-06-07 16:29:10.407456 micropython_rp2_pico_stubs-1.20.0.post2/uarray.pyi
+-rw-r--r--   0        0        0      132 2023-06-07 16:29:09.765033 micropython_rp2_pico_stubs-1.20.0.post2/uasyncio/__init__.pyi
+-rw-r--r--   0        0        0     1530 2023-06-07 16:29:09.766515 micropython_rp2_pico_stubs-1.20.0.post2/uasyncio/core.pyi
+-rw-r--r--   0        0        0      625 2023-06-07 16:29:09.767702 micropython_rp2_pico_stubs-1.20.0.post2/uasyncio/event.pyi
+-rw-r--r--   0        0        0      390 2023-06-07 16:29:09.767702 micropython_rp2_pico_stubs-1.20.0.post2/uasyncio/funcs.pyi
+-rw-r--r--   0        0        0      414 2023-06-07 16:29:09.769186 micropython_rp2_pico_stubs-1.20.0.post2/uasyncio/lock.pyi
+-rw-r--r--   0        0        0     1410 2023-06-07 16:29:09.770631 micropython_rp2_pico_stubs-1.20.0.post2/uasyncio/stream.pyi
+-rw-r--r--   0        0        0      789 2023-06-07 16:29:09.771838 micropython_rp2_pico_stubs-1.20.0.post2/uasyncio/task.pyi
+-rw-r--r--   0        0        0     1406 2023-06-07 16:29:10.421473 micropython_rp2_pico_stubs-1.20.0.post2/ubinascii.pyi
+-rw-r--r--   0        0        0     3638 2023-06-07 16:29:10.424398 micropython_rp2_pico_stubs-1.20.0.post2/ucollections.pyi
+-rw-r--r--   0        0        0     1645 2023-06-07 16:29:10.430922 micropython_rp2_pico_stubs-1.20.0.post2/ucryptolib.pyi
+-rw-r--r--   0        0        0     2361 2023-06-07 16:29:10.433730 micropython_rp2_pico_stubs-1.20.0.post2/uctypes.pyi
+-rw-r--r--   0        0        0      707 2023-06-07 16:29:10.435946 micropython_rp2_pico_stubs-1.20.0.post2/uerrno.pyi
+-rw-r--r--   0        0        0     1640 2023-06-07 16:29:10.438548 micropython_rp2_pico_stubs-1.20.0.post2/uhashlib.pyi
+-rw-r--r--   0        0        0      928 2023-06-07 16:29:10.440048 micropython_rp2_pico_stubs-1.20.0.post2/uheapq.pyi
+-rw-r--r--   0        0        0     2469 2023-06-07 16:29:10.441418 micropython_rp2_pico_stubs-1.20.0.post2/uio.pyi
+-rw-r--r--   0        0        0     1382 2023-06-07 16:29:10.442762 micropython_rp2_pico_stubs-1.20.0.post2/ujson.pyi
+-rw-r--r--   0        0        0    49173 2023-06-07 16:29:10.446164 micropython_rp2_pico_stubs-1.20.0.post2/umachine.pyi
+-rw-r--r--   0        0        0     9305 2023-06-07 16:29:10.447162 micropython_rp2_pico_stubs-1.20.0.post2/uos.pyi
+-rw-r--r--   0        0        0     2636 2023-06-07 16:29:10.449414 micropython_rp2_pico_stubs-1.20.0.post2/urandom.pyi
+-rw-r--r--   0        0        0      187 2023-06-07 16:29:10.451147 micropython_rp2_pico_stubs-1.20.0.post2/ure.pyi
+-rw-r--r--   0        0        0     3851 2023-06-07 16:29:10.452164 micropython_rp2_pico_stubs-1.20.0.post2/uselect.pyi
+-rw-r--r--   0        0        0     4239 2023-06-07 16:29:10.453276 micropython_rp2_pico_stubs-1.20.0.post2/ustruct.pyi
+-rw-r--r--   0        0        0      873 2023-06-07 16:29:10.454780 micropython_rp2_pico_stubs-1.20.0.post2/usys.pyi
+-rw-r--r--   0        0        0    12513 2023-06-07 16:29:10.455795 micropython_rp2_pico_stubs-1.20.0.post2/utime.pyi
+-rw-r--r--   0        0        0     1533 2023-06-07 16:29:10.456802 micropython_rp2_pico_stubs-1.20.0.post2/uzlib.pyi
+-rw-r--r--   0        0        0     1533 2023-06-07 16:29:10.457815 micropython_rp2_pico_stubs-1.20.0.post2/zlib.pyi
+-rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 micropython_rp2_pico_stubs-1.20.0.post2/setup.py
+-rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 micropython_rp2_pico_stubs-1.20.0.post2/PKG-INFO
```

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/_rp2.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/_rp2.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/_thread.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/_thread.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/array.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/array.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/binascii.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/binascii.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/cmath.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/cmath.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/collections.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/collections.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/cryptolib.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/cryptolib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/errno.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/errno.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/framebuf.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/framebuf.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/gc.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/gc.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/hashlib.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/hashlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/heapq.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/heapq.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/io.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/io.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/json.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/json.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/LICENSE.md` & `micropython_rp2_pico_stubs-1.20.0.post2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/logging.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/logging.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/machine.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/machine.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/math.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/math.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/micropython.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/micropython_.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/onewire.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/onewire.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/os.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/os.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/pyproject.toml` & `micropython_rp2_pico_stubs-1.20.0.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropython-rp2-pico-stubs"
-version = "1.20.0.post1"
+version = "1.20.0.post2"
 description = "MicroPython stubs"
 authors = [
     "josverl <josverl@users.noreply.github.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/josverl/micropython-stubs#micropython-stubs"
@@ -52,14 +52,15 @@
     { include = "heapq.pyi" },
     { include = "io.pyi" },
     { include = "json.pyi" },
     { include = "logging.pyi" },
     { include = "machine.pyi" },
     { include = "math.pyi" },
     { include = "micropython.pyi" },
+    { include = "micropython_.pyi" },
     { include = "neopixel.pyi" },
     { include = "onewire.pyi" },
     { include = "os.pyi" },
     { include = "random.pyi" },
     { include = "rp2.pyi" },
     { include = "select.pyi" },
     { include = "struct.pyi" },
```

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/random.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/random.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/README.md` & `micropython_rp2_pico_stubs-1.20.0.post2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
 
 For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
  * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
 
 Included stubs:
-* StubSource.MERGED from `stubs/micropython-v1_20_0-rp2-pico-merged`
-* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`
-* StubSource.CORE from `stubs/micropython-core`
+* Merged stubs from `stubs/micropython-v1_20_0-rp2-pico-merged`
+* Frozen stubs from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`
+* Core stubs from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
 Documentation | micropython | - | - | v1.20 
 Core | micropython | rp2 | - | v1.20.0
```

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/rp2.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/rp2.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/select.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/select.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/struct.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/struct.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/sys.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/sys.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/time.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/time.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/uarray.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/uarray.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/uasyncio/core.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/uasyncio/core.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/uasyncio/event.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/uasyncio/event.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/uasyncio/stream.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/uasyncio/stream.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/uasyncio/task.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/uasyncio/task.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/ubinascii.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/ubinascii.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/ucollections.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/ucollections.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/ucryptolib.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/ucryptolib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/uctypes.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/uctypes.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/uerrno.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/uerrno.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/uhashlib.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/uhashlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/uheapq.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/uheapq.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/uio.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/uio.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/ujson.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/ujson.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/umachine.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/umachine.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/uos.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/uos.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/urandom.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/urandom.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/uselect.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/uselect.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/ustruct.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/ustruct.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/usys.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/usys.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/utime.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/utime.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/uzlib.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/uzlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/zlib.pyi` & `micropython_rp2_pico_stubs-1.20.0.post2/zlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/setup.py` & `micropython_rp2_pico_stubs-1.20.0.post2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
  'heapq',
  'io',
  'json',
  'logging',
  'machine',
  'math',
  'micropython',
+ 'micropython_',
  'neopixel',
  'onewire',
  'os',
  'random',
  'rp2',
  'select',
  'struct',
@@ -63,17 +64,17 @@
  'uzlib',
  'zlib']
 install_requires = \
 ['micropython-stdlib-stubs>=0.9.0']
 
 setup_kwargs = {
     'name': 'micropython-rp2-pico-stubs',
-    'version': '1.20.0.post1',
+    'version': '1.20.0.post2',
     'description': 'MicroPython stubs',
-    'long_description': '# micropython-rp2-pico-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* StubSource.MERGED from `stubs/micropython-v1_20_0-rp2-pico-merged`\n* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`\n* StubSource.CORE from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nDocumentation | micropython | - | - | v1.20 \nCore | micropython | rp2 | - | v1.20.0 \n',
+    'long_description': '# micropython-rp2-pico-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* Merged stubs from `stubs/micropython-v1_20_0-rp2-pico-merged`\n* Frozen stubs from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`\n* Core stubs from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nDocumentation | micropython | - | - | v1.20 \nCore | micropython | rp2 | - | v1.20.0 \n',
     'author': 'josverl',
     'author_email': 'josverl@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josverl/micropython-stubs#micropython-stubs',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `micropython_rp2_pico_stubs-1.20.0.post1/PKG-INFO` & `micropython_rp2_pico_stubs-1.20.0.post2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-rp2-pico-stubs
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
-* StubSource.MERGED from `stubs/micropython-v1_20_0-rp2-pico-merged`
-* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`
-* StubSource.CORE from `stubs/micropython-core`
+* Merged stubs from `stubs/micropython-v1_20_0-rp2-pico-merged`
+* Frozen stubs from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`
+* Core stubs from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
 Documentation | micropython | - | - | v1.20 
 Core | micropython | rp2 | - | v1.20.0
```

