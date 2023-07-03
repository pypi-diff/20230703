# Comparing `tmp/micropython_stm32_stubs-1.20.0.post1.tar.gz` & `tmp/micropython_stm32_stubs-1.20.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_stm32_stubs-1.20.0.post1.tar", max compression
+gzip compressed data, was "micropython_stm32_stubs-1.20.0.post2.tar", max compression
```

## Comparing `micropython_stm32_stubs-1.20.0.post1.tar` & `micropython_stm32_stubs-1.20.0.post2.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0      277 2023-05-12 07:15:43.241810 micropython_stm32_stubs-1.20.0.post1/_onewire.pyi
--rw-r--r--   0        0        0      848 2023-05-12 07:15:46.137399 micropython_stm32_stubs-1.20.0.post1/_thread.pyi
--rw-r--r--   0        0        0      364 2023-05-12 07:15:43.243316 micropython_stm32_stubs-1.20.0.post1/_uasyncio.pyi
--rw-r--r--   0        0        0     1003 2023-05-12 07:15:58.913810 micropython_stm32_stubs-1.20.0.post1/array.pyi
--rw-r--r--   0        0        0     1408 2023-05-12 07:15:58.792096 micropython_stm32_stubs-1.20.0.post1/binascii.pyi
--rw-r--r--   0        0        0     1454 2023-05-12 07:15:58.813895 micropython_stm32_stubs-1.20.0.post1/cmath.pyi
--rw-r--r--   0        0        0     3640 2023-05-12 07:15:58.827952 micropython_stm32_stubs-1.20.0.post1/collections.pyi
--rw-r--r--   0        0        0      344 2023-05-05 19:51:02.978948 micropython_stm32_stubs-1.20.0.post1/dht.pyi
--rw-r--r--   0        0        0      709 2023-05-12 07:15:46.940344 micropython_stm32_stubs-1.20.0.post1/errno.pyi
--rw-r--r--   0        0        0     6349 2023-05-12 07:15:58.874726 micropython_stm32_stubs-1.20.0.post1/framebuf.pyi
--rw-r--r--   0        0        0     1993 2023-05-12 07:15:58.863196 micropython_stm32_stubs-1.20.0.post1/gc.pyi
--rw-r--r--   0        0        0     1368 2023-05-12 07:15:58.849147 micropython_stm32_stubs-1.20.0.post1/hashlib.pyi
--rw-r--r--   0        0        0      930 2023-05-12 07:15:58.866213 micropython_stm32_stubs-1.20.0.post1/heapq.pyi
--rw-r--r--   0        0        0     2471 2023-05-12 07:15:58.925863 micropython_stm32_stubs-1.20.0.post1/io.pyi
--rw-r--r--   0        0        0     1384 2023-05-12 07:15:58.879733 micropython_stm32_stubs-1.20.0.post1/json.pyi
--rw-r--r--   0        0        0    15648 2023-05-12 07:15:59.035817 micropython_stm32_stubs-1.20.0.post1/lcd160cr.pyi
--rw-r--r--   0        0        0     1092 2023-05-12 09:24:03.793899 micropython_stm32_stubs-1.20.0.post1/LICENSE.md
--rw-r--r--   0        0        0    51100 2023-05-12 07:16:01.476404 micropython_stm32_stubs-1.20.0.post1/machine.pyi
--rw-r--r--   0        0        0     4654 2023-05-12 07:15:59.023187 micropython_stm32_stubs-1.20.0.post1/math.pyi
--rw-r--r--   0        0        0     7213 2023-04-05 11:07:45.360315 micropython_stm32_stubs-1.20.0.post1/micropython.pyi
--rw-r--r--   0        0        0     1359 2023-05-12 07:15:50.462206 micropython_stm32_stubs-1.20.0.post1/network.pyi
--rw-r--r--   0        0        0      617 2023-05-05 19:51:02.981472 micropython_stm32_stubs-1.20.0.post1/onewire.pyi
--rw-r--r--   0        0        0     9396 2023-05-12 07:15:59.054853 micropython_stm32_stubs-1.20.0.post1/os.pyi
--rw-r--r--   0        0        0      162 2023-05-12 07:15:43.274041 micropython_stm32_stubs-1.20.0.post1/platform.pyi
--rw-r--r--   0        0        0    88587 2023-05-12 07:16:03.843741 micropython_stm32_stubs-1.20.0.post1/pyb.pyi
--rw-r--r--   0        0        0     3177 2023-05-12 09:24:04.932010 micropython_stm32_stubs-1.20.0.post1/pyproject.toml
--rw-r--r--   0        0        0     2638 2023-05-12 07:15:59.069379 micropython_stm32_stubs-1.20.0.post1/random.pyi
--rw-r--r--   0        0        0     2011 2023-05-12 09:24:03.793899 micropython_stm32_stubs-1.20.0.post1/README.md
--rw-r--r--   0        0        0     3853 2023-05-12 07:15:53.098617 micropython_stm32_stubs-1.20.0.post1/select.pyi
--rw-r--r--   0        0        0     9529 2023-05-12 07:15:59.160567 micropython_stm32_stubs-1.20.0.post1/socket.pyi
--rw-r--r--   0        0        0     4169 2023-05-12 07:15:53.724419 micropython_stm32_stubs-1.20.0.post1/stm.pyi
--rw-r--r--   0        0        0     4241 2023-05-12 07:15:59.172103 micropython_stm32_stubs-1.20.0.post1/struct.pyi
--rw-r--r--   0        0        0      875 2023-05-12 07:15:59.189143 micropython_stm32_stubs-1.20.0.post1/sys.pyi
--rw-r--r--   0        0        0    12515 2023-05-12 07:15:59.232246 micropython_stm32_stubs-1.20.0.post1/time.pyi
--rw-r--r--   0        0        0     1003 2023-05-12 07:15:59.199664 micropython_stm32_stubs-1.20.0.post1/uarray.pyi
--rw-r--r--   0        0        0      132 2023-05-05 19:51:02.935761 micropython_stm32_stubs-1.20.0.post1/uasyncio/__init__.pyi
--rw-r--r--   0        0        0     1530 2023-05-05 19:51:02.948379 micropython_stm32_stubs-1.20.0.post1/uasyncio/core.pyi
--rw-r--r--   0        0        0      625 2023-05-05 19:51:02.952597 micropython_stm32_stubs-1.20.0.post1/uasyncio/event.pyi
--rw-r--r--   0        0        0      390 2023-05-05 19:51:02.956666 micropython_stm32_stubs-1.20.0.post1/uasyncio/funcs.pyi
--rw-r--r--   0        0        0      414 2023-05-05 19:51:02.964713 micropython_stm32_stubs-1.20.0.post1/uasyncio/lock.pyi
--rw-r--r--   0        0        0     1410 2023-05-05 19:52:08.156723 micropython_stm32_stubs-1.20.0.post1/uasyncio/stream.pyi
--rw-r--r--   0        0        0      789 2023-05-05 19:51:02.973021 micropython_stm32_stubs-1.20.0.post1/uasyncio/task.pyi
--rw-r--r--   0        0        0     1408 2023-05-12 07:15:59.269519 micropython_stm32_stubs-1.20.0.post1/ubinascii.pyi
--rw-r--r--   0        0        0     3640 2023-05-12 07:15:59.306737 micropython_stm32_stubs-1.20.0.post1/ucollections.pyi
--rw-r--r--   0        0        0     2363 2023-05-12 07:15:59.314264 micropython_stm32_stubs-1.20.0.post1/uctypes.pyi
--rw-r--r--   0        0        0      709 2023-05-12 07:15:54.774402 micropython_stm32_stubs-1.20.0.post1/uerrno.pyi
--rw-r--r--   0        0        0     1368 2023-05-12 07:15:59.326324 micropython_stm32_stubs-1.20.0.post1/uhashlib.pyi
--rw-r--r--   0        0        0      930 2023-05-12 07:15:59.335227 micropython_stm32_stubs-1.20.0.post1/uheapq.pyi
--rw-r--r--   0        0        0     2471 2023-05-12 07:15:59.420836 micropython_stm32_stubs-1.20.0.post1/uio.pyi
--rw-r--r--   0        0        0     1384 2023-05-12 07:15:59.340235 micropython_stm32_stubs-1.20.0.post1/ujson.pyi
--rw-r--r--   0        0        0    51100 2023-05-12 07:16:05.691736 micropython_stm32_stubs-1.20.0.post1/umachine.pyi
--rw-r--r--   0        0        0     9396 2023-05-12 07:15:59.543674 micropython_stm32_stubs-1.20.0.post1/uos.pyi
--rw-r--r--   0        0        0      162 2023-05-12 07:15:43.303196 micropython_stm32_stubs-1.20.0.post1/uplatform.pyi
--rw-r--r--   0        0        0     2638 2023-05-12 07:15:59.484480 micropython_stm32_stubs-1.20.0.post1/urandom.pyi
--rw-r--r--   0        0        0      187 2023-05-12 07:15:43.305658 micropython_stm32_stubs-1.20.0.post1/ure.pyi
--rw-r--r--   0        0        0     3853 2023-05-12 07:15:57.203703 micropython_stm32_stubs-1.20.0.post1/uselect.pyi
--rw-r--r--   0        0        0     9529 2023-05-12 07:15:59.595730 micropython_stm32_stubs-1.20.0.post1/usocket.pyi
--rw-r--r--   0        0        0     4241 2023-05-12 07:15:59.556205 micropython_stm32_stubs-1.20.0.post1/ustruct.pyi
--rw-r--r--   0        0        0      875 2023-05-12 07:15:59.577684 micropython_stm32_stubs-1.20.0.post1/usys.pyi
--rw-r--r--   0        0        0    12515 2023-05-12 07:15:59.635636 micropython_stm32_stubs-1.20.0.post1/utime.pyi
--rw-r--r--   0        0        0      245 2023-05-12 07:15:43.313177 micropython_stm32_stubs-1.20.0.post1/utimeq.pyi
--rw-r--r--   0        0        0     1535 2023-05-12 07:15:59.615066 micropython_stm32_stubs-1.20.0.post1/uzlib.pyi
--rw-r--r--   0        0        0     1535 2023-05-12 07:15:59.632108 micropython_stm32_stubs-1.20.0.post1/zlib.pyi
--rw-r--r--   0        0        0     3291 1970-01-01 00:00:00.000000 micropython_stm32_stubs-1.20.0.post1/setup.py
--rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 micropython_stm32_stubs-1.20.0.post1/PKG-INFO
+-rw-r--r--   0        0        0      277 2023-06-07 16:29:11.643970 micropython_stm32_stubs-1.20.0.post2/_onewire.pyi
+-rw-r--r--   0        0        0      848 2023-06-07 16:29:11.644971 micropython_stm32_stubs-1.20.0.post2/_thread.pyi
+-rw-r--r--   0        0        0      364 2023-06-07 16:29:11.645977 micropython_stm32_stubs-1.20.0.post2/_uasyncio.pyi
+-rw-r--r--   0        0        0     1003 2023-06-07 16:29:11.646970 micropython_stm32_stubs-1.20.0.post2/array.pyi
+-rw-r--r--   0        0        0     1408 2023-06-07 16:29:11.647971 micropython_stm32_stubs-1.20.0.post2/binascii.pyi
+-rw-r--r--   0        0        0     1454 2023-06-07 16:29:11.649661 micropython_stm32_stubs-1.20.0.post2/cmath.pyi
+-rw-r--r--   0        0        0     3640 2023-06-07 16:29:11.650715 micropython_stm32_stubs-1.20.0.post2/collections.pyi
+-rw-r--r--   0        0        0      344 2023-06-07 16:29:10.010463 micropython_stm32_stubs-1.20.0.post2/dht.pyi
+-rw-r--r--   0        0        0      709 2023-06-07 16:29:11.653376 micropython_stm32_stubs-1.20.0.post2/errno.pyi
+-rw-r--r--   0        0        0     6349 2023-06-07 16:29:11.654411 micropython_stm32_stubs-1.20.0.post2/framebuf.pyi
+-rw-r--r--   0        0        0     1993 2023-06-07 16:29:11.655929 micropython_stm32_stubs-1.20.0.post2/gc.pyi
+-rw-r--r--   0        0        0     1368 2023-06-07 16:29:11.656952 micropython_stm32_stubs-1.20.0.post2/hashlib.pyi
+-rw-r--r--   0        0        0      930 2023-06-07 16:29:11.657952 micropython_stm32_stubs-1.20.0.post2/heapq.pyi
+-rw-r--r--   0        0        0     2471 2023-06-07 16:29:11.659948 micropython_stm32_stubs-1.20.0.post2/io.pyi
+-rw-r--r--   0        0        0     1384 2023-06-07 16:29:11.659948 micropython_stm32_stubs-1.20.0.post2/json.pyi
+-rw-r--r--   0        0        0    15648 2023-06-07 16:29:11.662659 micropython_stm32_stubs-1.20.0.post2/lcd160cr.pyi
+-rw-r--r--   0        0        0     1092 2023-07-03 13:39:37.235109 micropython_stm32_stubs-1.20.0.post2/LICENSE.md
+-rw-r--r--   0        0        0    51100 2023-06-07 16:29:11.665446 micropython_stm32_stubs-1.20.0.post2/machine.pyi
+-rw-r--r--   0        0        0     4654 2023-06-07 16:29:11.666532 micropython_stm32_stubs-1.20.0.post2/math.pyi
+-rw-r--r--   0        0        0     8274 2023-07-03 11:26:14.336969 micropython_stm32_stubs-1.20.0.post2/micropython.pyi
+-rw-r--r--   0        0        0     7213 2023-07-03 11:19:19.390108 micropython_stm32_stubs-1.20.0.post2/micropython_.pyi
+-rw-r--r--   0        0        0     1359 2023-06-07 16:29:11.668847 micropython_stm32_stubs-1.20.0.post2/network.pyi
+-rw-r--r--   0        0        0      617 2023-06-07 16:29:10.012863 micropython_stm32_stubs-1.20.0.post2/onewire.pyi
+-rw-r--r--   0        0        0     9396 2023-06-07 16:29:11.671054 micropython_stm32_stubs-1.20.0.post2/os.pyi
+-rw-r--r--   0        0        0      162 2023-06-07 16:29:11.672099 micropython_stm32_stubs-1.20.0.post2/platform.pyi
+-rw-r--r--   0        0        0    88587 2023-06-07 16:29:11.674278 micropython_stm32_stubs-1.20.0.post2/pyb.pyi
+-rw-r--r--   0        0        0     3215 2023-07-03 13:39:39.414678 micropython_stm32_stubs-1.20.0.post2/pyproject.toml
+-rw-r--r--   0        0        0     2638 2023-06-07 16:29:11.675356 micropython_stm32_stubs-1.20.0.post2/random.pyi
+-rw-r--r--   0        0        0     1996 2023-07-03 13:39:37.232938 micropython_stm32_stubs-1.20.0.post2/README.md
+-rw-r--r--   0        0        0     3853 2023-06-07 16:29:11.676455 micropython_stm32_stubs-1.20.0.post2/select.pyi
+-rw-r--r--   0        0        0     9529 2023-06-07 16:29:11.678096 micropython_stm32_stubs-1.20.0.post2/socket.pyi
+-rw-r--r--   0        0        0     4169 2023-06-07 16:29:11.679174 micropython_stm32_stubs-1.20.0.post2/stm.pyi
+-rw-r--r--   0        0        0     4241 2023-06-07 16:29:11.680209 micropython_stm32_stubs-1.20.0.post2/struct.pyi
+-rw-r--r--   0        0        0      875 2023-06-07 16:29:11.681286 micropython_stm32_stubs-1.20.0.post2/sys.pyi
+-rw-r--r--   0        0        0    12515 2023-06-07 16:29:11.682364 micropython_stm32_stubs-1.20.0.post2/time.pyi
+-rw-r--r--   0        0        0     1003 2023-06-07 16:29:11.683434 micropython_stm32_stubs-1.20.0.post2/uarray.pyi
+-rw-r--r--   0        0        0      132 2023-06-07 16:29:10.014039 micropython_stm32_stubs-1.20.0.post2/uasyncio/__init__.pyi
+-rw-r--r--   0        0        0     1530 2023-06-07 16:29:10.015101 micropython_stm32_stubs-1.20.0.post2/uasyncio/core.pyi
+-rw-r--r--   0        0        0      625 2023-06-07 16:29:10.016509 micropython_stm32_stubs-1.20.0.post2/uasyncio/event.pyi
+-rw-r--r--   0        0        0      390 2023-06-07 16:29:10.018024 micropython_stm32_stubs-1.20.0.post2/uasyncio/funcs.pyi
+-rw-r--r--   0        0        0      414 2023-06-07 16:29:10.020024 micropython_stm32_stubs-1.20.0.post2/uasyncio/lock.pyi
+-rw-r--r--   0        0        0     1410 2023-06-07 16:29:10.021026 micropython_stm32_stubs-1.20.0.post2/uasyncio/stream.pyi
+-rw-r--r--   0        0        0      789 2023-06-07 16:29:10.023025 micropython_stm32_stubs-1.20.0.post2/uasyncio/task.pyi
+-rw-r--r--   0        0        0     1408 2023-06-07 16:29:11.691467 micropython_stm32_stubs-1.20.0.post2/ubinascii.pyi
+-rw-r--r--   0        0        0     3640 2023-06-07 16:29:11.692497 micropython_stm32_stubs-1.20.0.post2/ucollections.pyi
+-rw-r--r--   0        0        0     2363 2023-06-07 16:29:11.693647 micropython_stm32_stubs-1.20.0.post2/uctypes.pyi
+-rw-r--r--   0        0        0      709 2023-06-07 16:29:11.695435 micropython_stm32_stubs-1.20.0.post2/uerrno.pyi
+-rw-r--r--   0        0        0     1368 2023-06-07 16:29:11.696663 micropython_stm32_stubs-1.20.0.post2/uhashlib.pyi
+-rw-r--r--   0        0        0      930 2023-06-07 16:29:11.697743 micropython_stm32_stubs-1.20.0.post2/uheapq.pyi
+-rw-r--r--   0        0        0     2471 2023-06-07 16:29:11.699334 micropython_stm32_stubs-1.20.0.post2/uio.pyi
+-rw-r--r--   0        0        0     1384 2023-06-07 16:29:11.701443 micropython_stm32_stubs-1.20.0.post2/ujson.pyi
+-rw-r--r--   0        0        0    51100 2023-06-07 16:29:11.704449 micropython_stm32_stubs-1.20.0.post2/umachine.pyi
+-rw-r--r--   0        0        0     9396 2023-06-07 16:29:11.707142 micropython_stm32_stubs-1.20.0.post2/uos.pyi
+-rw-r--r--   0        0        0      162 2023-06-07 16:29:11.708196 micropython_stm32_stubs-1.20.0.post2/uplatform.pyi
+-rw-r--r--   0        0        0     2638 2023-06-07 16:29:11.709278 micropython_stm32_stubs-1.20.0.post2/urandom.pyi
+-rw-r--r--   0        0        0      187 2023-06-07 16:29:11.710291 micropython_stm32_stubs-1.20.0.post2/ure.pyi
+-rw-r--r--   0        0        0     3853 2023-06-07 16:29:11.711304 micropython_stm32_stubs-1.20.0.post2/uselect.pyi
+-rw-r--r--   0        0        0     9529 2023-06-07 16:29:11.712311 micropython_stm32_stubs-1.20.0.post2/usocket.pyi
+-rw-r--r--   0        0        0     4241 2023-06-07 16:29:11.714316 micropython_stm32_stubs-1.20.0.post2/ustruct.pyi
+-rw-r--r--   0        0        0      875 2023-06-07 16:29:11.715450 micropython_stm32_stubs-1.20.0.post2/usys.pyi
+-rw-r--r--   0        0        0    12515 2023-06-07 16:29:11.717027 micropython_stm32_stubs-1.20.0.post2/utime.pyi
+-rw-r--r--   0        0        0      245 2023-06-07 16:29:11.718655 micropython_stm32_stubs-1.20.0.post2/utimeq.pyi
+-rw-r--r--   0        0        0     1535 2023-06-07 16:29:11.719765 micropython_stm32_stubs-1.20.0.post2/uzlib.pyi
+-rw-r--r--   0        0        0     1535 2023-06-07 16:29:11.720851 micropython_stm32_stubs-1.20.0.post2/zlib.pyi
+-rw-r--r--   0        0        0     3293 1970-01-01 00:00:00.000000 micropython_stm32_stubs-1.20.0.post2/setup.py
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 micropython_stm32_stubs-1.20.0.post2/PKG-INFO
```

### Comparing `micropython_stm32_stubs-1.20.0.post1/_thread.pyi` & `micropython_stm32_stubs-1.20.0.post2/_thread.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/array.pyi` & `micropython_stm32_stubs-1.20.0.post2/array.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/binascii.pyi` & `micropython_stm32_stubs-1.20.0.post2/binascii.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/cmath.pyi` & `micropython_stm32_stubs-1.20.0.post2/cmath.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/collections.pyi` & `micropython_stm32_stubs-1.20.0.post2/collections.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/errno.pyi` & `micropython_stm32_stubs-1.20.0.post2/errno.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/framebuf.pyi` & `micropython_stm32_stubs-1.20.0.post2/framebuf.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/gc.pyi` & `micropython_stm32_stubs-1.20.0.post2/gc.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/hashlib.pyi` & `micropython_stm32_stubs-1.20.0.post2/hashlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/heapq.pyi` & `micropython_stm32_stubs-1.20.0.post2/heapq.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/io.pyi` & `micropython_stm32_stubs-1.20.0.post2/io.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/json.pyi` & `micropython_stm32_stubs-1.20.0.post2/json.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/lcd160cr.pyi` & `micropython_stm32_stubs-1.20.0.post2/lcd160cr.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/LICENSE.md` & `micropython_stm32_stubs-1.20.0.post2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/machine.pyi` & `micropython_stm32_stubs-1.20.0.post2/machine.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/math.pyi` & `micropython_stm32_stubs-1.20.0.post2/math.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/micropython.pyi` & `micropython_stm32_stubs-1.20.0.post2/micropython_.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/network.pyi` & `micropython_stm32_stubs-1.20.0.post2/network.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/onewire.pyi` & `micropython_stm32_stubs-1.20.0.post2/onewire.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/os.pyi` & `micropython_stm32_stubs-1.20.0.post2/os.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/pyb.pyi` & `micropython_stm32_stubs-1.20.0.post2/pyb.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/pyproject.toml` & `micropython_stm32_stubs-1.20.0.post2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropython-stm32-stubs"
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
     { include = "lcd160cr.pyi" },
     { include = "machine.pyi" },
     { include = "math.pyi" },
     { include = "micropython.pyi" },
+    { include = "micropython_.pyi" },
     { include = "network.pyi" },
     { include = "onewire.pyi" },
     { include = "os.pyi" },
     { include = "platform.pyi" },
     { include = "pyb.pyi" },
     { include = "random.pyi" },
     { include = "select.pyi" },
```

### Comparing `micropython_stm32_stubs-1.20.0.post1/random.pyi` & `micropython_stm32_stubs-1.20.0.post2/random.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/README.md` & `micropython_stm32_stubs-1.20.0.post2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
 
 For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
  * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
 
 Included stubs:
-* StubSource.MERGED from `stubs/micropython-v1_20_0-stm32-merged`
-* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/stm32/GENERIC`
-* StubSource.CORE from `stubs/micropython-core`
+* Merged stubs from `stubs/micropython-v1_20_0-stm32-merged`
+* Frozen stubs from `stubs/micropython-v1_20_0-frozen/stm32/GENERIC`
+* Core stubs from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
 Documentation | micropython | - | - | v1.20.0 
 Core | micropython | stm32 | - | v1.20.0
```

### Comparing `micropython_stm32_stubs-1.20.0.post1/select.pyi` & `micropython_stm32_stubs-1.20.0.post2/select.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/socket.pyi` & `micropython_stm32_stubs-1.20.0.post2/socket.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/stm.pyi` & `micropython_stm32_stubs-1.20.0.post2/stm.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/struct.pyi` & `micropython_stm32_stubs-1.20.0.post2/struct.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/sys.pyi` & `micropython_stm32_stubs-1.20.0.post2/sys.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/time.pyi` & `micropython_stm32_stubs-1.20.0.post2/time.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/uarray.pyi` & `micropython_stm32_stubs-1.20.0.post2/uarray.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/uasyncio/core.pyi` & `micropython_stm32_stubs-1.20.0.post2/uasyncio/core.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/uasyncio/event.pyi` & `micropython_stm32_stubs-1.20.0.post2/uasyncio/event.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/uasyncio/stream.pyi` & `micropython_stm32_stubs-1.20.0.post2/uasyncio/stream.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/uasyncio/task.pyi` & `micropython_stm32_stubs-1.20.0.post2/uasyncio/task.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/ubinascii.pyi` & `micropython_stm32_stubs-1.20.0.post2/ubinascii.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/ucollections.pyi` & `micropython_stm32_stubs-1.20.0.post2/ucollections.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/uctypes.pyi` & `micropython_stm32_stubs-1.20.0.post2/uctypes.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/uerrno.pyi` & `micropython_stm32_stubs-1.20.0.post2/uerrno.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/uhashlib.pyi` & `micropython_stm32_stubs-1.20.0.post2/uhashlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/uheapq.pyi` & `micropython_stm32_stubs-1.20.0.post2/uheapq.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/uio.pyi` & `micropython_stm32_stubs-1.20.0.post2/uio.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/ujson.pyi` & `micropython_stm32_stubs-1.20.0.post2/ujson.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/umachine.pyi` & `micropython_stm32_stubs-1.20.0.post2/umachine.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/uos.pyi` & `micropython_stm32_stubs-1.20.0.post2/uos.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/urandom.pyi` & `micropython_stm32_stubs-1.20.0.post2/urandom.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/uselect.pyi` & `micropython_stm32_stubs-1.20.0.post2/uselect.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/usocket.pyi` & `micropython_stm32_stubs-1.20.0.post2/usocket.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/ustruct.pyi` & `micropython_stm32_stubs-1.20.0.post2/ustruct.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/usys.pyi` & `micropython_stm32_stubs-1.20.0.post2/usys.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/utime.pyi` & `micropython_stm32_stubs-1.20.0.post2/utime.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/uzlib.pyi` & `micropython_stm32_stubs-1.20.0.post2/uzlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/zlib.pyi` & `micropython_stm32_stubs-1.20.0.post2/zlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_stm32_stubs-1.20.0.post1/setup.py` & `micropython_stm32_stubs-1.20.0.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
  'heapq',
  'io',
  'json',
  'lcd160cr',
  'machine',
  'math',
  'micropython',
+ 'micropython_',
  'network',
  'onewire',
  'os',
  'platform',
  'pyb',
  'random',
  'select',
@@ -63,17 +64,17 @@
  'uzlib',
  'zlib']
 install_requires = \
 ['micropython-stdlib-stubs>=0.9.0']
 
 setup_kwargs = {
     'name': 'micropython-stm32-stubs',
-    'version': '1.20.0.post1',
+    'version': '1.20.0.post2',
     'description': 'MicroPython stubs',
-    'long_description': '# micropython-stm32-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* StubSource.MERGED from `stubs/micropython-v1_20_0-stm32-merged`\n* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/stm32/GENERIC`\n* StubSource.CORE from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nDocumentation | micropython | - | - | v1.20.0 \nCore | micropython | stm32 | - | v1.20.0 \n',
+    'long_description': '# micropython-stm32-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* Merged stubs from `stubs/micropython-v1_20_0-stm32-merged`\n* Frozen stubs from `stubs/micropython-v1_20_0-frozen/stm32/GENERIC`\n* Core stubs from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nDocumentation | micropython | - | - | v1.20.0 \nCore | micropython | stm32 | - | v1.20.0 \n',
     'author': 'josverl',
     'author_email': 'josverl@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josverl/micropython-stubs#micropython-stubs',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `micropython_stm32_stubs-1.20.0.post1/PKG-INFO` & `micropython_stm32_stubs-1.20.0.post2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-stm32-stubs
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
-* StubSource.MERGED from `stubs/micropython-v1_20_0-stm32-merged`
-* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/stm32/GENERIC`
-* StubSource.CORE from `stubs/micropython-core`
+* Merged stubs from `stubs/micropython-v1_20_0-stm32-merged`
+* Frozen stubs from `stubs/micropython-v1_20_0-frozen/stm32/GENERIC`
+* Core stubs from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
 Documentation | micropython | - | - | v1.20.0 
 Core | micropython | stm32 | - | v1.20.0
```

