# Comparing `tmp/micropython_rp2_pico_w_stubs-1.20.0.post1.tar.gz` & `tmp/micropython_rp2_pico_w_stubs-1.20.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_rp2_pico_w_stubs-1.20.0.post1.tar", max compression
+gzip compressed data, was "micropython_rp2_pico_w_stubs-1.20.0.post2.tar", max compression
```

## Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1.tar` & `micropython_rp2_pico_w_stubs-1.20.0.post2.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0       71 2023-04-30 14:05:00.188832 micropython_rp2_pico_w_stubs-1.20.0.post1/_boot.pyi
--rw-r--r--   0        0        0       71 2023-04-30 14:05:00.189851 micropython_rp2_pico_w_stubs-1.20.0.post1/_boot_fat.pyi
--rw-r--r--   0        0        0      277 2023-04-30 14:20:27.679578 micropython_rp2_pico_w_stubs-1.20.0.post1/_onewire.pyi
--rw-r--r--   0        0        0     1406 2023-04-30 14:20:27.682493 micropython_rp2_pico_w_stubs-1.20.0.post1/_rp2.pyi
--rw-r--r--   0        0        0      846 2023-04-30 15:02:27.973877 micropython_rp2_pico_w_stubs-1.20.0.post1/_thread.pyi
--rw-r--r--   0        0        0      364 2023-04-30 14:20:27.685499 micropython_rp2_pico_w_stubs-1.20.0.post1/_uasyncio.pyi
--rw-r--r--   0        0        0      999 2023-04-30 15:02:28.479029 micropython_rp2_pico_w_stubs-1.20.0.post1/array.pyi
--rw-r--r--   0        0        0     1400 2023-04-30 15:02:28.887681 micropython_rp2_pico_w_stubs-1.20.0.post1/binascii.pyi
--rw-r--r--   0        0        0     1436 2023-04-30 15:02:29.456920 micropython_rp2_pico_w_stubs-1.20.0.post1/cmath.pyi
--rw-r--r--   0        0        0     3634 2023-04-30 15:02:30.134603 micropython_rp2_pico_w_stubs-1.20.0.post1/collections.pyi
--rw-r--r--   0        0        0     1645 2023-04-30 15:02:30.555064 micropython_rp2_pico_w_stubs-1.20.0.post1/cryptolib.pyi
--rw-r--r--   0        0        0      344 2023-04-30 14:05:00.193359 micropython_rp2_pico_w_stubs-1.20.0.post1/dht.pyi
--rw-r--r--   0        0        0      404 2023-04-30 14:05:00.193359 micropython_rp2_pico_w_stubs-1.20.0.post1/ds18x20.pyi
--rw-r--r--   0        0        0      707 2023-04-30 15:02:30.963520 micropython_rp2_pico_w_stubs-1.20.0.post1/errno.pyi
--rw-r--r--   0        0        0     6345 2023-04-30 15:02:31.936942 micropython_rp2_pico_w_stubs-1.20.0.post1/framebuf.pyi
--rw-r--r--   0        0        0     1981 2023-04-30 15:02:32.392636 micropython_rp2_pico_w_stubs-1.20.0.post1/gc.pyi
--rw-r--r--   0        0        0     1636 2023-04-30 15:02:32.937906 micropython_rp2_pico_w_stubs-1.20.0.post1/hashlib.pyi
--rw-r--r--   0        0        0      924 2023-04-30 15:02:33.352957 micropython_rp2_pico_w_stubs-1.20.0.post1/heapq.pyi
--rw-r--r--   0        0        0     2467 2023-04-30 15:02:33.790261 micropython_rp2_pico_w_stubs-1.20.0.post1/io.pyi
--rw-r--r--   0        0        0     1376 2023-04-30 15:02:33.968618 micropython_rp2_pico_w_stubs-1.20.0.post1/json.pyi
--rw-r--r--   0        0        0     1092 2023-05-04 19:20:41.377508 micropython_rp2_pico_w_stubs-1.20.0.post1/LICENSE.md
--rw-r--r--   0        0        0      827 2023-04-30 14:20:27.717853 micropython_rp2_pico_w_stubs-1.20.0.post1/logging.pyi
--rw-r--r--   0        0        0     1385 2023-04-30 14:20:27.721145 micropython_rp2_pico_w_stubs-1.20.0.post1/lwip.pyi
--rw-r--r--   0        0        0    48918 2023-04-30 15:02:36.568304 micropython_rp2_pico_w_stubs-1.20.0.post1/machine.pyi
--rw-r--r--   0        0        0     4578 2023-04-30 15:02:38.025468 micropython_rp2_pico_w_stubs-1.20.0.post1/math.pyi
--rw-r--r--   0        0        0     7213 2023-04-05 11:07:45.360315 micropython_rp2_pico_w_stubs-1.20.0.post1/micropython.pyi
--rw-r--r--   0        0        0       68 2023-04-30 14:20:27.727021 micropython_rp2_pico_w_stubs-1.20.0.post1/mip.pyi
--rw-r--r--   0        0        0      448 2023-04-30 14:05:00.199241 micropython_rp2_pico_w_stubs-1.20.0.post1/neopixel.pyi
--rw-r--r--   0        0        0      953 2023-04-30 14:20:27.727021 micropython_rp2_pico_w_stubs-1.20.0.post1/network.pyi
--rw-r--r--   0        0        0      134 2023-04-30 14:20:27.734529 micropython_rp2_pico_w_stubs-1.20.0.post1/ntptime.pyi
--rw-r--r--   0        0        0      617 2023-04-30 14:05:00.201127 micropython_rp2_pico_w_stubs-1.20.0.post1/onewire.pyi
--rw-r--r--   0        0        0     2136 2023-04-30 14:20:27.734529 micropython_rp2_pico_w_stubs-1.20.0.post1/os.pyi
--rw-r--r--   0        0        0     3542 2023-05-04 19:20:46.368947 micropython_rp2_pico_w_stubs-1.20.0.post1/pyproject.toml
--rw-r--r--   0        0        0      321 2023-04-30 14:20:27.734529 micropython_rp2_pico_w_stubs-1.20.0.post1/random.pyi
--rw-r--r--   0        0        0     1928 2023-05-04 19:20:41.377508 micropython_rp2_pico_w_stubs-1.20.0.post1/README.md
--rw-r--r--   0        0        0     1918 2023-04-30 14:05:00.202944 micropython_rp2_pico_w_stubs-1.20.0.post1/rp2.pyi
--rw-r--r--   0        0        0      163 2023-04-30 14:20:27.742540 micropython_rp2_pico_w_stubs-1.20.0.post1/select.pyi
--rw-r--r--   0        0        0     1385 2023-04-30 14:20:27.744967 micropython_rp2_pico_w_stubs-1.20.0.post1/socket.pyi
--rw-r--r--   0        0        0      130 2023-04-30 14:20:27.744967 micropython_rp2_pico_w_stubs-1.20.0.post1/ssl.pyi
--rw-r--r--   0        0        0      239 2023-04-30 14:20:27.744967 micropython_rp2_pico_w_stubs-1.20.0.post1/struct.pyi
--rw-r--r--   0        0        0      319 2023-04-30 14:20:27.750974 micropython_rp2_pico_w_stubs-1.20.0.post1/sys.pyi
--rw-r--r--   0        0        0      578 2023-04-30 14:20:27.750974 micropython_rp2_pico_w_stubs-1.20.0.post1/time.pyi
--rw-r--r--   0        0        0      196 2023-04-30 14:20:27.750974 micropython_rp2_pico_w_stubs-1.20.0.post1/uarray.pyi
--rw-r--r--   0        0        0      132 2023-04-30 14:05:00.203475 micropython_rp2_pico_w_stubs-1.20.0.post1/uasyncio/__init__.pyi
--rw-r--r--   0        0        0     1530 2023-04-30 14:05:00.207637 micropython_rp2_pico_w_stubs-1.20.0.post1/uasyncio/core.pyi
--rw-r--r--   0        0        0      625 2023-04-30 14:05:00.210009 micropython_rp2_pico_w_stubs-1.20.0.post1/uasyncio/event.pyi
--rw-r--r--   0        0        0      390 2023-04-30 14:05:00.211770 micropython_rp2_pico_w_stubs-1.20.0.post1/uasyncio/funcs.pyi
--rw-r--r--   0        0        0      414 2023-04-30 14:05:00.211770 micropython_rp2_pico_w_stubs-1.20.0.post1/uasyncio/lock.pyi
--rw-r--r--   0        0        0     1410 2023-04-30 14:05:00.211770 micropython_rp2_pico_w_stubs-1.20.0.post1/uasyncio/stream.pyi
--rw-r--r--   0        0        0      789 2023-04-30 14:05:00.217879 micropython_rp2_pico_w_stubs-1.20.0.post1/uasyncio/task.pyi
--rw-r--r--   0        0        0      242 2023-04-30 14:20:27.750974 micropython_rp2_pico_w_stubs-1.20.0.post1/ubinascii.pyi
--rw-r--r--   0        0        0      893 2023-04-30 14:20:27.750974 micropython_rp2_pico_w_stubs-1.20.0.post1/ucollections.pyi
--rw-r--r--   0        0        0      196 2023-04-30 14:20:27.758993 micropython_rp2_pico_w_stubs-1.20.0.post1/ucryptolib.pyi
--rw-r--r--   0        0        0      694 2023-04-30 14:20:27.758993 micropython_rp2_pico_w_stubs-1.20.0.post1/uctypes.pyi
--rw-r--r--   0        0        0      341 2023-04-30 14:20:27.758993 micropython_rp2_pico_w_stubs-1.20.0.post1/uerrno.pyi
--rw-r--r--   0        0        0      368 2023-04-30 14:20:27.758993 micropython_rp2_pico_w_stubs-1.20.0.post1/uhashlib.pyi
--rw-r--r--   0        0        0      153 2023-04-30 14:20:27.758993 micropython_rp2_pico_w_stubs-1.20.0.post1/uheapq.pyi
--rw-r--r--   0        0        0     1193 2023-04-30 14:20:27.767004 micropython_rp2_pico_w_stubs-1.20.0.post1/uio.pyi
--rw-r--r--   0        0        0      184 2023-04-30 14:20:27.768328 micropython_rp2_pico_w_stubs-1.20.0.post1/ujson.pyi
--rw-r--r--   0        0        0     7384 2023-04-30 14:20:30.596278 micropython_rp2_pico_w_stubs-1.20.0.post1/umachine.pyi
--rw-r--r--   0        0        0     2136 2023-04-30 14:20:27.770057 micropython_rp2_pico_w_stubs-1.20.0.post1/uos.pyi
--rw-r--r--   0        0        0      321 2023-04-30 14:20:27.775065 micropython_rp2_pico_w_stubs-1.20.0.post1/urandom.pyi
--rw-r--r--   0        0        0      187 2023-04-30 14:20:27.775065 micropython_rp2_pico_w_stubs-1.20.0.post1/ure.pyi
--rw-r--r--   0        0        0      508 2023-04-30 14:20:27.775065 micropython_rp2_pico_w_stubs-1.20.0.post1/urequests.pyi
--rw-r--r--   0        0        0      163 2023-04-30 14:20:27.775065 micropython_rp2_pico_w_stubs-1.20.0.post1/uselect.pyi
--rw-r--r--   0        0        0     1385 2023-04-30 14:20:27.783079 micropython_rp2_pico_w_stubs-1.20.0.post1/usocket.pyi
--rw-r--r--   0        0        0      130 2023-04-30 14:20:27.783079 micropython_rp2_pico_w_stubs-1.20.0.post1/ussl.pyi
--rw-r--r--   0        0        0      239 2023-04-30 14:20:27.783079 micropython_rp2_pico_w_stubs-1.20.0.post1/ustruct.pyi
--rw-r--r--   0        0        0      319 2023-04-30 14:20:27.783079 micropython_rp2_pico_w_stubs-1.20.0.post1/usys.pyi
--rw-r--r--   0        0        0      578 2023-04-30 14:20:27.783079 micropython_rp2_pico_w_stubs-1.20.0.post1/utime.pyi
--rw-r--r--   0        0        0      403 2023-04-30 14:20:27.793084 micropython_rp2_pico_w_stubs-1.20.0.post1/uwebsocket.pyi
--rw-r--r--   0        0        0      299 2023-04-30 14:20:27.794381 micropython_rp2_pico_w_stubs-1.20.0.post1/uzlib.pyi
--rw-r--r--   0        0        0      403 2023-04-30 14:20:27.794381 micropython_rp2_pico_w_stubs-1.20.0.post1/websocket.pyi
--rw-r--r--   0        0        0      299 2023-04-30 14:20:27.799298 micropython_rp2_pico_w_stubs-1.20.0.post1/zlib.pyi
--rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 micropython_rp2_pico_w_stubs-1.20.0.post1/setup.py
--rw-r--r--   0        0        0     3186 1970-01-01 00:00:00.000000 micropython_rp2_pico_w_stubs-1.20.0.post1/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-06-07 16:29:09.755582 micropython_rp2_pico_w_stubs-1.20.0.post2/_boot.pyi
+-rw-r--r--   0        0        0       71 2023-06-07 16:29:09.756991 micropython_rp2_pico_w_stubs-1.20.0.post2/_boot_fat.pyi
+-rw-r--r--   0        0        0      277 2023-06-07 16:29:10.525652 micropython_rp2_pico_w_stubs-1.20.0.post2/_onewire.pyi
+-rw-r--r--   0        0        0     1406 2023-06-07 16:29:10.526976 micropython_rp2_pico_w_stubs-1.20.0.post2/_rp2.pyi
+-rw-r--r--   0        0        0      846 2023-06-07 16:29:10.528395 micropython_rp2_pico_w_stubs-1.20.0.post2/_thread.pyi
+-rw-r--r--   0        0        0      364 2023-06-07 16:29:10.530401 micropython_rp2_pico_w_stubs-1.20.0.post2/_uasyncio.pyi
+-rw-r--r--   0        0        0      999 2023-06-07 16:29:10.531401 micropython_rp2_pico_w_stubs-1.20.0.post2/array.pyi
+-rw-r--r--   0        0        0     1400 2023-06-07 16:29:10.533403 micropython_rp2_pico_w_stubs-1.20.0.post2/binascii.pyi
+-rw-r--r--   0        0        0     1436 2023-06-07 16:29:10.534895 micropython_rp2_pico_w_stubs-1.20.0.post2/cmath.pyi
+-rw-r--r--   0        0        0     3634 2023-06-07 16:29:10.536904 micropython_rp2_pico_w_stubs-1.20.0.post2/collections.pyi
+-rw-r--r--   0        0        0     1645 2023-06-07 16:29:10.537909 micropython_rp2_pico_w_stubs-1.20.0.post2/cryptolib.pyi
+-rw-r--r--   0        0        0      344 2023-06-07 16:29:09.758150 micropython_rp2_pico_w_stubs-1.20.0.post2/dht.pyi
+-rw-r--r--   0        0        0      404 2023-06-07 16:29:09.759157 micropython_rp2_pico_w_stubs-1.20.0.post2/ds18x20.pyi
+-rw-r--r--   0        0        0      707 2023-06-07 16:29:10.544706 micropython_rp2_pico_w_stubs-1.20.0.post2/errno.pyi
+-rw-r--r--   0        0        0     6345 2023-06-07 16:29:10.546971 micropython_rp2_pico_w_stubs-1.20.0.post2/framebuf.pyi
+-rw-r--r--   0        0        0     1981 2023-06-07 16:29:10.548985 micropython_rp2_pico_w_stubs-1.20.0.post2/gc.pyi
+-rw-r--r--   0        0        0     1636 2023-06-07 16:29:10.549969 micropython_rp2_pico_w_stubs-1.20.0.post2/hashlib.pyi
+-rw-r--r--   0        0        0      924 2023-06-07 16:29:10.551416 micropython_rp2_pico_w_stubs-1.20.0.post2/heapq.pyi
+-rw-r--r--   0        0        0     2467 2023-06-07 16:29:10.553425 micropython_rp2_pico_w_stubs-1.20.0.post2/io.pyi
+-rw-r--r--   0        0        0     1376 2023-06-07 16:29:10.553425 micropython_rp2_pico_w_stubs-1.20.0.post2/json.pyi
+-rw-r--r--   0        0        0     1092 2023-07-03 13:38:37.623576 micropython_rp2_pico_w_stubs-1.20.0.post2/LICENSE.md
+-rw-r--r--   0        0        0      827 2023-06-07 16:29:10.556270 micropython_rp2_pico_w_stubs-1.20.0.post2/logging.pyi
+-rw-r--r--   0        0        0     1385 2023-06-07 16:29:10.557277 micropython_rp2_pico_w_stubs-1.20.0.post2/lwip.pyi
+-rw-r--r--   0        0        0    48918 2023-06-07 16:29:10.559775 micropython_rp2_pico_w_stubs-1.20.0.post2/machine.pyi
+-rw-r--r--   0        0        0     4578 2023-06-07 16:29:10.560786 micropython_rp2_pico_w_stubs-1.20.0.post2/math.pyi
+-rw-r--r--   0        0        0     8274 2023-07-03 11:26:14.336969 micropython_rp2_pico_w_stubs-1.20.0.post2/micropython.pyi
+-rw-r--r--   0        0        0     7213 2023-07-03 11:19:19.390108 micropython_rp2_pico_w_stubs-1.20.0.post2/micropython_.pyi
+-rw-r--r--   0        0        0       68 2023-06-07 16:29:10.563934 micropython_rp2_pico_w_stubs-1.20.0.post2/mip.pyi
+-rw-r--r--   0        0        0      448 2023-06-07 16:29:09.760540 micropython_rp2_pico_w_stubs-1.20.0.post2/neopixel.pyi
+-rw-r--r--   0        0        0      953 2023-06-07 16:29:10.566928 micropython_rp2_pico_w_stubs-1.20.0.post2/network.pyi
+-rw-r--r--   0        0        0      134 2023-06-07 16:29:10.567938 micropython_rp2_pico_w_stubs-1.20.0.post2/ntptime.pyi
+-rw-r--r--   0        0        0      617 2023-06-07 16:29:09.761978 micropython_rp2_pico_w_stubs-1.20.0.post2/onewire.pyi
+-rw-r--r--   0        0        0     2136 2023-06-07 16:29:10.571335 micropython_rp2_pico_w_stubs-1.20.0.post2/os.pyi
+-rw-r--r--   0        0        0     3580 2023-07-03 13:38:39.047320 micropython_rp2_pico_w_stubs-1.20.0.post2/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-06-07 16:29:10.572335 micropython_rp2_pico_w_stubs-1.20.0.post2/random.pyi
+-rw-r--r--   0        0        0     1913 2023-07-03 13:38:37.621565 micropython_rp2_pico_w_stubs-1.20.0.post2/README.md
+-rw-r--r--   0        0        0     1918 2023-06-07 16:29:09.762992 micropython_rp2_pico_w_stubs-1.20.0.post2/rp2.pyi
+-rw-r--r--   0        0        0      163 2023-06-07 16:29:10.576188 micropython_rp2_pico_w_stubs-1.20.0.post2/select.pyi
+-rw-r--r--   0        0        0     1385 2023-06-07 16:29:10.577196 micropython_rp2_pico_w_stubs-1.20.0.post2/socket.pyi
+-rw-r--r--   0        0        0      130 2023-06-07 16:29:10.578191 micropython_rp2_pico_w_stubs-1.20.0.post2/ssl.pyi
+-rw-r--r--   0        0        0      239 2023-06-07 16:29:10.580391 micropython_rp2_pico_w_stubs-1.20.0.post2/struct.pyi
+-rw-r--r--   0        0        0      319 2023-06-07 16:29:10.582728 micropython_rp2_pico_w_stubs-1.20.0.post2/sys.pyi
+-rw-r--r--   0        0        0      578 2023-06-07 16:29:10.583727 micropython_rp2_pico_w_stubs-1.20.0.post2/time.pyi
+-rw-r--r--   0        0        0      196 2023-06-07 16:29:10.584844 micropython_rp2_pico_w_stubs-1.20.0.post2/uarray.pyi
+-rw-r--r--   0        0        0      132 2023-06-07 16:29:09.765033 micropython_rp2_pico_w_stubs-1.20.0.post2/uasyncio/__init__.pyi
+-rw-r--r--   0        0        0     1530 2023-06-07 16:29:09.766515 micropython_rp2_pico_w_stubs-1.20.0.post2/uasyncio/core.pyi
+-rw-r--r--   0        0        0      625 2023-06-07 16:29:09.767702 micropython_rp2_pico_w_stubs-1.20.0.post2/uasyncio/event.pyi
+-rw-r--r--   0        0        0      390 2023-06-07 16:29:09.767702 micropython_rp2_pico_w_stubs-1.20.0.post2/uasyncio/funcs.pyi
+-rw-r--r--   0        0        0      414 2023-06-07 16:29:09.769186 micropython_rp2_pico_w_stubs-1.20.0.post2/uasyncio/lock.pyi
+-rw-r--r--   0        0        0     1410 2023-06-07 16:29:09.770631 micropython_rp2_pico_w_stubs-1.20.0.post2/uasyncio/stream.pyi
+-rw-r--r--   0        0        0      789 2023-06-07 16:29:09.771838 micropython_rp2_pico_w_stubs-1.20.0.post2/uasyncio/task.pyi
+-rw-r--r--   0        0        0      242 2023-06-07 16:29:10.596614 micropython_rp2_pico_w_stubs-1.20.0.post2/ubinascii.pyi
+-rw-r--r--   0        0        0      893 2023-06-07 16:29:10.597953 micropython_rp2_pico_w_stubs-1.20.0.post2/ucollections.pyi
+-rw-r--r--   0        0        0      196 2023-06-07 16:29:10.598964 micropython_rp2_pico_w_stubs-1.20.0.post2/ucryptolib.pyi
+-rw-r--r--   0        0        0      694 2023-06-07 16:29:10.599964 micropython_rp2_pico_w_stubs-1.20.0.post2/uctypes.pyi
+-rw-r--r--   0        0        0      341 2023-06-07 16:29:10.600966 micropython_rp2_pico_w_stubs-1.20.0.post2/uerrno.pyi
+-rw-r--r--   0        0        0      368 2023-06-07 16:29:10.601967 micropython_rp2_pico_w_stubs-1.20.0.post2/uhashlib.pyi
+-rw-r--r--   0        0        0      153 2023-06-07 16:29:10.602966 micropython_rp2_pico_w_stubs-1.20.0.post2/uheapq.pyi
+-rw-r--r--   0        0        0     1193 2023-06-07 16:29:10.603961 micropython_rp2_pico_w_stubs-1.20.0.post2/uio.pyi
+-rw-r--r--   0        0        0      184 2023-06-07 16:29:10.604962 micropython_rp2_pico_w_stubs-1.20.0.post2/ujson.pyi
+-rw-r--r--   0        0        0     7384 2023-06-07 16:29:10.605960 micropython_rp2_pico_w_stubs-1.20.0.post2/umachine.pyi
+-rw-r--r--   0        0        0     2136 2023-06-07 16:29:10.606961 micropython_rp2_pico_w_stubs-1.20.0.post2/uos.pyi
+-rw-r--r--   0        0        0      321 2023-06-07 16:29:10.607963 micropython_rp2_pico_w_stubs-1.20.0.post2/urandom.pyi
+-rw-r--r--   0        0        0      187 2023-06-07 16:29:10.609963 micropython_rp2_pico_w_stubs-1.20.0.post2/ure.pyi
+-rw-r--r--   0        0        0      508 2023-06-07 16:29:10.610960 micropython_rp2_pico_w_stubs-1.20.0.post2/urequests.pyi
+-rw-r--r--   0        0        0      163 2023-06-07 16:29:10.611960 micropython_rp2_pico_w_stubs-1.20.0.post2/uselect.pyi
+-rw-r--r--   0        0        0     1385 2023-06-07 16:29:10.613086 micropython_rp2_pico_w_stubs-1.20.0.post2/usocket.pyi
+-rw-r--r--   0        0        0      130 2023-06-07 16:29:10.614425 micropython_rp2_pico_w_stubs-1.20.0.post2/ussl.pyi
+-rw-r--r--   0        0        0      239 2023-06-07 16:29:10.614934 micropython_rp2_pico_w_stubs-1.20.0.post2/ustruct.pyi
+-rw-r--r--   0        0        0      319 2023-06-07 16:29:10.616290 micropython_rp2_pico_w_stubs-1.20.0.post2/usys.pyi
+-rw-r--r--   0        0        0      578 2023-06-07 16:29:10.617740 micropython_rp2_pico_w_stubs-1.20.0.post2/utime.pyi
+-rw-r--r--   0        0        0      403 2023-06-07 16:29:10.618752 micropython_rp2_pico_w_stubs-1.20.0.post2/uwebsocket.pyi
+-rw-r--r--   0        0        0      299 2023-06-07 16:29:10.620046 micropython_rp2_pico_w_stubs-1.20.0.post2/uzlib.pyi
+-rw-r--r--   0        0        0      403 2023-06-07 16:29:10.621059 micropython_rp2_pico_w_stubs-1.20.0.post2/websocket.pyi
+-rw-r--r--   0        0        0      299 2023-06-07 16:29:10.622054 micropython_rp2_pico_w_stubs-1.20.0.post2/zlib.pyi
+-rw-r--r--   0        0        0     3344 1970-01-01 00:00:00.000000 micropython_rp2_pico_w_stubs-1.20.0.post2/setup.py
+-rw-r--r--   0        0        0     3171 1970-01-01 00:00:00.000000 micropython_rp2_pico_w_stubs-1.20.0.post2/PKG-INFO
```

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/_rp2.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/_rp2.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/_thread.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/_thread.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/array.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/array.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/binascii.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/binascii.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/cmath.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/cmath.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/collections.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/collections.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/cryptolib.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/cryptolib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/errno.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/errno.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/framebuf.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/framebuf.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/gc.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/gc.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/hashlib.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/hashlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/heapq.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/heapq.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/io.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/io.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/json.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/json.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/LICENSE.md` & `micropython_rp2_pico_w_stubs-1.20.0.post2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/logging.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/logging.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/lwip.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/lwip.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/machine.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/machine.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/math.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/math.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/micropython.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/micropython_.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/network.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/network.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/onewire.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/onewire.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/os.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/os.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/pyproject.toml` & `micropython_rp2_pico_w_stubs-1.20.0.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropython-rp2-pico_w-stubs"
-version = "1.20.0.post1"
+version = "1.20.0.post2"
 description = "MicroPython stubs"
 authors = [
     "josverl <josverl@users.noreply.github.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/josverl/micropython-stubs#micropython-stubs"
@@ -53,14 +53,15 @@
     { include = "io.pyi" },
     { include = "json.pyi" },
     { include = "logging.pyi" },
     { include = "lwip.pyi" },
     { include = "machine.pyi" },
     { include = "math.pyi" },
     { include = "micropython.pyi" },
+    { include = "micropython_.pyi" },
     { include = "mip.pyi" },
     { include = "neopixel.pyi" },
     { include = "network.pyi" },
     { include = "ntptime.pyi" },
     { include = "onewire.pyi" },
     { include = "os.pyi" },
     { include = "random.pyi" },
```

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/README.md` & `micropython_rp2_pico_w_stubs-1.20.0.post2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 
 If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
 
 For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
  * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
 
 Included stubs:
-* StubSource.MERGED from `stubs/micropython-v1_20_0-rp2-pico_w-merged`
-* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`
-* StubSource.CORE from `stubs/micropython-core`
+* Merged stubs from `stubs/micropython-v1_20_0-rp2-pico_w-merged`
+* Frozen stubs from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`
+* Core stubs from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
```

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/rp2.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/rp2.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/socket.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/socket.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/time.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/time.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/uasyncio/core.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/uasyncio/core.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/uasyncio/event.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/uasyncio/event.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/uasyncio/stream.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/uasyncio/stream.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/uasyncio/task.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/uasyncio/task.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/ucollections.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/ucollections.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/uctypes.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/uctypes.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/uio.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/uio.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/umachine.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/umachine.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/uos.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/uos.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/usocket.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/usocket.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/utime.pyi` & `micropython_rp2_pico_w_stubs-1.20.0.post2/utime.pyi`

 * *Files identical despite different names*

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/setup.py` & `micropython_rp2_pico_w_stubs-1.20.0.post2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  'io',
  'json',
  'logging',
  'lwip',
  'machine',
  'math',
  'micropython',
+ 'micropython_',
  'mip',
  'neopixel',
  'network',
  'ntptime',
  'onewire',
  'os',
  'random',
@@ -74,17 +75,17 @@
  'websocket',
  'zlib']
 install_requires = \
 ['micropython-stdlib-stubs>=0.9.0']
 
 setup_kwargs = {
     'name': 'micropython-rp2-pico-w-stubs',
-    'version': '1.20.0.post1',
+    'version': '1.20.0.post2',
     'description': 'MicroPython stubs',
-    'long_description': '# micropython-rp2-pico_w-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* StubSource.MERGED from `stubs/micropython-v1_20_0-rp2-pico_w-merged`\n* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`\n* StubSource.CORE from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\n',
+    'long_description': '# micropython-rp2-pico_w-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* Merged stubs from `stubs/micropython-v1_20_0-rp2-pico_w-merged`\n* Frozen stubs from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`\n* Core stubs from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\n',
     'author': 'josverl',
     'author_email': 'josverl@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josverl/micropython-stubs#micropython-stubs',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `micropython_rp2_pico_w_stubs-1.20.0.post1/PKG-INFO` & `micropython_rp2_pico_w_stubs-1.20.0.post2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-rp2-pico-w-stubs
-Version: 1.20.0.post1
+Version: 1.20.0.post2
 Summary: MicroPython stubs
 Home-page: https://github.com/josverl/micropython-stubs#micropython-stubs
 License: MIT
 Author: josverl
 Author-email: josverl@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -52,15 +52,15 @@
 
 If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
 
 For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
  * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
 
 Included stubs:
-* StubSource.MERGED from `stubs/micropython-v1_20_0-rp2-pico_w-merged`
-* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`
-* StubSource.CORE from `stubs/micropython-core`
+* Merged stubs from `stubs/micropython-v1_20_0-rp2-pico_w-merged`
+* Frozen stubs from `stubs/micropython-v1_20_0-frozen/rp2/GENERIC`
+* Core stubs from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
```

