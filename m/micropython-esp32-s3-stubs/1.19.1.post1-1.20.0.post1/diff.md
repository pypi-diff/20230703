# Comparing `tmp/micropython_esp32_s3_stubs-1.19.1.post1.tar.gz` & `tmp/micropython_esp32_s3_stubs-1.20.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_esp32_s3_stubs-1.19.1.post1.tar", max compression
+gzip compressed data, was "micropython_esp32_s3_stubs-1.20.0.post1.tar", max compression
```

## Comparing `micropython_esp32_s3_stubs-1.19.1.post1.tar` & `micropython_esp32_s3_stubs-1.20.0.post1.tar`

### file list

```diff
@@ -1,86 +1,90 @@
--rw-r--r--   0        0        0      174 2023-01-15 15:10:19.531964 micropython_esp32_s3_stubs-1.19.1.post1/_boot.py
--rw-r--r--   0        0        0      658 2023-02-07 15:50:40.347900 micropython_esp32_s3_stubs-1.19.1.post1/_onewire.py
--rw-r--r--   0        0        0     1205 2023-02-07 15:50:40.348900 micropython_esp32_s3_stubs-1.19.1.post1/_thread.py
--rw-r--r--   0        0        0      760 2023-02-07 15:50:40.348900 micropython_esp32_s3_stubs-1.19.1.post1/_uasyncio.py
--rw-r--r--   0        0        0      173 2023-01-15 15:10:19.281298 micropython_esp32_s3_stubs-1.19.1.post1/apa106.py
--rw-r--r--   0        0        0     1344 2023-02-07 15:50:40.349900 micropython_esp32_s3_stubs-1.19.1.post1/array.py
--rw-r--r--   0        0        0     1695 2023-02-07 15:50:40.349900 micropython_esp32_s3_stubs-1.19.1.post1/binascii.py
--rw-r--r--   0        0        0    30021 2023-02-07 15:50:40.350901 micropython_esp32_s3_stubs-1.19.1.post1/bluetooth.py
--rw-r--r--   0        0        0     4068 2023-02-07 15:50:40.352342 micropython_esp32_s3_stubs-1.19.1.post1/btree.py
--rw-r--r--   0        0        0     1780 2023-02-07 15:50:40.352342 micropython_esp32_s3_stubs-1.19.1.post1/cmath.py
--rw-r--r--   0        0        0     4046 2023-02-07 15:50:40.352342 micropython_esp32_s3_stubs-1.19.1.post1/collections.py
--rw-r--r--   0        0        0     1923 2023-02-07 15:50:40.353545 micropython_esp32_s3_stubs-1.19.1.post1/cryptolib.py
--rw-r--r--   0        0        0     1098 2023-01-15 15:10:19.840728 micropython_esp32_s3_stubs-1.19.1.post1/dht.py
--rw-r--r--   0        0        0     1453 2023-01-15 15:10:19.925637 micropython_esp32_s3_stubs-1.19.1.post1/ds18x20.py
--rw-r--r--   0        0        0     1284 2023-02-07 15:50:40.355578 micropython_esp32_s3_stubs-1.19.1.post1/errno.py
--rw-r--r--   0        0        0     2152 2023-02-07 15:50:40.355578 micropython_esp32_s3_stubs-1.19.1.post1/esp.py
--rw-r--r--   0        0        0    11648 2023-02-07 15:50:40.356586 micropython_esp32_s3_stubs-1.19.1.post1/esp32.py
--rw-r--r--   0        0        0      273 2023-01-15 15:10:19.381825 micropython_esp32_s3_stubs-1.19.1.post1/flashbdev.py
--rw-r--r--   0        0        0     5328 2023-02-07 15:50:40.358601 micropython_esp32_s3_stubs-1.19.1.post1/framebuf.py
--rw-r--r--   0        0        0     2284 2023-02-07 15:50:40.358601 micropython_esp32_s3_stubs-1.19.1.post1/gc.py
--rw-r--r--   0        0        0     1978 2023-02-07 15:50:40.359585 micropython_esp32_s3_stubs-1.19.1.post1/hashlib.py
--rw-r--r--   0        0        0     1206 2023-02-07 15:50:40.359585 micropython_esp32_s3_stubs-1.19.1.post1/heapq.py
--rw-r--r--   0        0        0     1066 2023-01-15 15:10:19.454065 micropython_esp32_s3_stubs-1.19.1.post1/inisetup.py
--rw-r--r--   0        0        0     4760 2023-02-07 15:50:40.360694 micropython_esp32_s3_stubs-1.19.1.post1/io.py
--rw-r--r--   0        0        0     1662 2023-02-07 15:50:40.362128 micropython_esp32_s3_stubs-1.19.1.post1/json.py
--rw-r--r--   0        0        0     1092 2023-07-03 13:40:41.537600 micropython_esp32_s3_stubs-1.19.1.post1/LICENSE.md
--rw-r--r--   0        0        0    50527 2023-02-07 15:50:40.362128 micropython_esp32_s3_stubs-1.19.1.post1/machine.py
--rw-r--r--   0        0        0     5103 2023-02-07 15:50:40.363622 micropython_esp32_s3_stubs-1.19.1.post1/math.py
--rw-r--r--   0        0        0     8274 2023-07-03 11:26:14.336969 micropython_esp32_s3_stubs-1.19.1.post1/micropython.pyi
--rw-r--r--   0        0        0     7213 2023-07-03 11:19:19.390108 micropython_esp32_s3_stubs-1.19.1.post1/micropython_.pyi
--rw-r--r--   0        0        0     1387 2023-01-15 19:17:53.454916 micropython_esp32_s3_stubs-1.19.1.post1/neopixel.py
--rw-r--r--   0        0        0     7949 2023-02-07 15:50:40.364638 micropython_esp32_s3_stubs-1.19.1.post1/network.py
--rw-r--r--   0        0        0      946 2023-01-15 15:10:19.757962 micropython_esp32_s3_stubs-1.19.1.post1/ntptime.py
--rw-r--r--   0        0        0     2395 2023-01-15 15:10:20.013507 micropython_esp32_s3_stubs-1.19.1.post1/onewire.py
--rw-r--r--   0        0        0     9964 2023-02-07 15:50:40.366636 micropython_esp32_s3_stubs-1.19.1.post1/os.py
--rw-r--r--   0        0        0      516 2023-02-07 15:50:40.366636 micropython_esp32_s3_stubs-1.19.1.post1/platform.py
--rw-r--r--   0        0        0     1279 2023-07-03 13:40:42.652700 micropython_esp32_s3_stubs-1.19.1.post1/pyproject.toml
--rw-r--r--   0        0        0     2931 2023-02-07 15:50:40.367629 micropython_esp32_s3_stubs-1.19.1.post1/random.py
--rw-r--r--   0        0        0     2075 2023-07-03 13:40:41.536090 micropython_esp32_s3_stubs-1.19.1.post1/README.md
--rw-r--r--   0        0        0     4204 2023-02-07 15:50:40.368669 micropython_esp32_s3_stubs-1.19.1.post1/select.py
--rw-r--r--   0        0        0    10069 2023-02-07 15:50:40.369676 micropython_esp32_s3_stubs-1.19.1.post1/socket.py
--rw-r--r--   0        0        0     2141 2023-02-07 15:50:40.369676 micropython_esp32_s3_stubs-1.19.1.post1/ssl.py
--rw-r--r--   0        0        0     1849 2023-02-07 15:50:40.370677 micropython_esp32_s3_stubs-1.19.1.post1/struct.py
--rw-r--r--   0        0        0     1472 2023-02-07 15:50:40.370677 micropython_esp32_s3_stubs-1.19.1.post1/sys.py
--rw-r--r--   0        0        0    12763 2023-02-07 15:50:40.371675 micropython_esp32_s3_stubs-1.19.1.post1/time.py
--rw-r--r--   0        0        0     1344 2023-02-07 15:50:40.371675 micropython_esp32_s3_stubs-1.19.1.post1/uarray.py
--rw-r--r--   0        0        0      709 2023-01-15 15:10:20.082915 micropython_esp32_s3_stubs-1.19.1.post1/uasyncio/__init__.py
--rw-r--r--   0        0        0     9583 2023-01-15 15:10:20.178431 micropython_esp32_s3_stubs-1.19.1.post1/uasyncio/core.py
--rw-r--r--   0        0        0     1910 2023-01-15 15:10:20.273580 micropython_esp32_s3_stubs-1.19.1.post1/uasyncio/event.py
--rw-r--r--   0        0        0     4277 2023-01-15 15:10:20.357577 micropython_esp32_s3_stubs-1.19.1.post1/uasyncio/funcs.py
--rw-r--r--   0        0        0     1767 2023-01-15 15:10:20.436178 micropython_esp32_s3_stubs-1.19.1.post1/uasyncio/lock.py
--rw-r--r--   0        0        0     4391 2023-01-15 15:10:20.554743 micropython_esp32_s3_stubs-1.19.1.post1/uasyncio/stream.py
--rw-r--r--   0        0        0     5607 2023-01-15 15:10:20.951367 micropython_esp32_s3_stubs-1.19.1.post1/uasyncio/task.py
--rw-r--r--   0        0        0     1695 2023-02-07 15:50:40.376020 micropython_esp32_s3_stubs-1.19.1.post1/ubinascii.py
--rw-r--r--   0        0        0    30021 2023-02-07 15:50:40.376020 micropython_esp32_s3_stubs-1.19.1.post1/ubluetooth.py
--rw-r--r--   0        0        0     4046 2023-02-07 15:50:40.376020 micropython_esp32_s3_stubs-1.19.1.post1/ucollections.py
--rw-r--r--   0        0        0     1923 2023-02-07 15:50:40.377458 micropython_esp32_s3_stubs-1.19.1.post1/ucryptolib.py
--rw-r--r--   0        0        0     3249 2023-02-07 15:50:40.377458 micropython_esp32_s3_stubs-1.19.1.post1/uctypes.py
--rw-r--r--   0        0        0     1284 2023-02-07 15:50:40.378466 micropython_esp32_s3_stubs-1.19.1.post1/uerrno.py
--rw-r--r--   0        0        0     1978 2023-02-07 15:50:40.378466 micropython_esp32_s3_stubs-1.19.1.post1/uhashlib.py
--rw-r--r--   0        0        0     1206 2023-02-07 15:50:40.379466 micropython_esp32_s3_stubs-1.19.1.post1/uheapq.py
--rw-r--r--   0        0        0     4760 2023-02-07 15:50:40.379466 micropython_esp32_s3_stubs-1.19.1.post1/uio.py
--rw-r--r--   0        0        0     1662 2023-02-07 15:50:40.379466 micropython_esp32_s3_stubs-1.19.1.post1/ujson.py
--rw-r--r--   0        0        0    50527 2023-02-07 15:50:40.380551 micropython_esp32_s3_stubs-1.19.1.post1/umachine.py
--rw-r--r--   0        0        0     9964 2023-02-07 15:50:40.381559 micropython_esp32_s3_stubs-1.19.1.post1/uos.py
--rw-r--r--   0        0        0     8782 2023-01-15 15:10:19.628314 micropython_esp32_s3_stubs-1.19.1.post1/upip.py
--rw-r--r--   0        0        0     2371 2023-01-15 15:10:19.694639 micropython_esp32_s3_stubs-1.19.1.post1/upip_utarfile.py
--rw-r--r--   0        0        0      517 2023-02-07 15:50:40.381559 micropython_esp32_s3_stubs-1.19.1.post1/uplatform.py
--rw-r--r--   0        0        0     2931 2023-02-07 15:50:40.381559 micropython_esp32_s3_stubs-1.19.1.post1/urandom.py
--rw-r--r--   0        0        0      545 2023-02-07 15:50:40.382776 micropython_esp32_s3_stubs-1.19.1.post1/ure.py
--rw-r--r--   0        0        0     4204 2023-02-07 15:50:40.382776 micropython_esp32_s3_stubs-1.19.1.post1/uselect.py
--rw-r--r--   0        0        0    10069 2023-02-07 15:50:40.383782 micropython_esp32_s3_stubs-1.19.1.post1/usocket.py
--rw-r--r--   0        0        0     2141 2023-02-07 15:50:40.383782 micropython_esp32_s3_stubs-1.19.1.post1/ussl.py
--rw-r--r--   0        0        0     1849 2023-02-07 15:50:40.384782 micropython_esp32_s3_stubs-1.19.1.post1/ustruct.py
--rw-r--r--   0        0        0     1472 2023-02-07 15:50:40.385784 micropython_esp32_s3_stubs-1.19.1.post1/usys.py
--rw-r--r--   0        0        0    12763 2023-02-07 15:50:40.385784 micropython_esp32_s3_stubs-1.19.1.post1/utime.py
--rw-r--r--   0        0        0      616 2023-02-07 15:50:40.385784 micropython_esp32_s3_stubs-1.19.1.post1/utimeq.py
--rw-r--r--   0        0        0      811 2023-02-07 15:50:40.387207 micropython_esp32_s3_stubs-1.19.1.post1/uwebsocket.py
--rw-r--r--   0        0        0     1855 2023-02-07 15:50:40.387207 micropython_esp32_s3_stubs-1.19.1.post1/uzlib.py
--rw-r--r--   0        0        0     2321 2023-01-15 15:10:20.640516 micropython_esp32_s3_stubs-1.19.1.post1/webrepl.py
--rw-r--r--   0        0        0     2859 2023-01-15 19:17:53.495248 micropython_esp32_s3_stubs-1.19.1.post1/webrepl_setup.py
--rw-r--r--   0        0        0      810 2023-02-07 15:50:40.387207 micropython_esp32_s3_stubs-1.19.1.post1/websocket.py
--rw-r--r--   0        0        0     1717 2023-01-15 15:10:20.780498 micropython_esp32_s3_stubs-1.19.1.post1/websocket_helper.py
--rw-r--r--   0        0        0     1855 2023-02-07 15:50:40.388440 micropython_esp32_s3_stubs-1.19.1.post1/zlib.py
--rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 micropython_esp32_s3_stubs-1.19.1.post1/setup.py
--rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 micropython_esp32_s3_stubs-1.19.1.post1/PKG-INFO
+-rw-r--r--   0        0        0       53 2023-06-07 16:29:08.823669 micropython_esp32_s3_stubs-1.20.0.post1/_boot.pyi
+-rw-r--r--   0        0        0      277 2023-06-07 16:29:08.435041 micropython_esp32_s3_stubs-1.20.0.post1/_onewire.pyi
+-rw-r--r--   0        0        0      848 2023-06-07 16:29:08.436040 micropython_esp32_s3_stubs-1.20.0.post1/_thread.pyi
+-rw-r--r--   0        0        0      364 2023-06-07 16:29:08.437500 micropython_esp32_s3_stubs-1.20.0.post1/_uasyncio.pyi
+-rw-r--r--   0        0        0      115 2023-06-07 16:29:08.824669 micropython_esp32_s3_stubs-1.20.0.post1/apa106.pyi
+-rw-r--r--   0        0        0     1003 2023-06-07 16:29:08.440120 micropython_esp32_s3_stubs-1.20.0.post1/array.pyi
+-rw-r--r--   0        0        0     1408 2023-06-07 16:29:08.441129 micropython_esp32_s3_stubs-1.20.0.post1/binascii.pyi
+-rw-r--r--   0        0        0    31291 2023-06-07 16:29:08.442129 micropython_esp32_s3_stubs-1.20.0.post1/bluetooth.pyi
+-rw-r--r--   0        0        0     3837 2023-06-07 16:29:08.443272 micropython_esp32_s3_stubs-1.20.0.post1/btree.pyi
+-rw-r--r--   0        0        0     1454 2023-06-07 16:29:08.444573 micropython_esp32_s3_stubs-1.20.0.post1/cmath.pyi
+-rw-r--r--   0        0        0     3640 2023-06-07 16:29:08.444573 micropython_esp32_s3_stubs-1.20.0.post1/collections.pyi
+-rw-r--r--   0        0        0     1647 2023-06-07 16:29:08.446065 micropython_esp32_s3_stubs-1.20.0.post1/cryptolib.pyi
+-rw-r--r--   0        0        0      344 2023-06-07 16:29:08.825809 micropython_esp32_s3_stubs-1.20.0.post1/dht.pyi
+-rw-r--r--   0        0        0      404 2023-06-07 16:29:08.827878 micropython_esp32_s3_stubs-1.20.0.post1/ds18x20.pyi
+-rw-r--r--   0        0        0      709 2023-06-07 16:29:08.452087 micropython_esp32_s3_stubs-1.20.0.post1/errno.pyi
+-rw-r--r--   0        0        0     1703 2023-06-07 16:29:08.453205 micropython_esp32_s3_stubs-1.20.0.post1/esp.pyi
+-rw-r--r--   0        0        0    11354 2023-06-07 16:29:08.454223 micropython_esp32_s3_stubs-1.20.0.post1/esp32.pyi
+-rw-r--r--   0        0        0       54 2023-06-07 16:29:08.829008 micropython_esp32_s3_stubs-1.20.0.post1/flashbdev.pyi
+-rw-r--r--   0        0        0     6349 2023-06-07 16:29:08.458216 micropython_esp32_s3_stubs-1.20.0.post1/framebuf.pyi
+-rw-r--r--   0        0        0     1993 2023-06-07 16:29:08.458216 micropython_esp32_s3_stubs-1.20.0.post1/gc.pyi
+-rw-r--r--   0        0        0     1642 2023-06-07 16:29:08.460215 micropython_esp32_s3_stubs-1.20.0.post1/hashlib.pyi
+-rw-r--r--   0        0        0      930 2023-06-07 16:29:08.461398 micropython_esp32_s3_stubs-1.20.0.post1/heapq.pyi
+-rw-r--r--   0        0        0       77 2023-06-07 16:29:08.830015 micropython_esp32_s3_stubs-1.20.0.post1/inisetup.pyi
+-rw-r--r--   0        0        0     2650 2023-06-07 16:29:08.464410 micropython_esp32_s3_stubs-1.20.0.post1/io.pyi
+-rw-r--r--   0        0        0     1384 2023-06-07 16:29:08.465480 micropython_esp32_s3_stubs-1.20.0.post1/json.pyi
+-rw-r--r--   0        0        0     1092 2023-07-03 13:38:06.742719 micropython_esp32_s3_stubs-1.20.0.post1/LICENSE.md
+-rw-r--r--   0        0        0    52167 2023-06-07 16:29:08.467962 micropython_esp32_s3_stubs-1.20.0.post1/machine.pyi
+-rw-r--r--   0        0        0     4654 2023-06-07 16:29:08.469273 micropython_esp32_s3_stubs-1.20.0.post1/math.pyi
+-rw-r--r--   0        0        0     8274 2023-07-03 11:26:14.336969 micropython_esp32_s3_stubs-1.20.0.post1/micropython.pyi
+-rw-r--r--   0        0        0     7213 2023-07-03 11:19:19.390108 micropython_esp32_s3_stubs-1.20.0.post1/micropython_.pyi
+-rw-r--r--   0        0        0      598 2023-06-07 16:29:08.832450 micropython_esp32_s3_stubs-1.20.0.post1/mip/__init__.pyi
+-rw-r--r--   0        0        0       68 2023-06-07 16:29:08.471533 micropython_esp32_s3_stubs-1.20.0.post1/mip.pyi
+-rw-r--r--   0        0        0      448 2023-06-07 16:29:08.834648 micropython_esp32_s3_stubs-1.20.0.post1/neopixel.pyi
+-rw-r--r--   0        0        0     7545 2023-06-07 16:29:08.473837 micropython_esp32_s3_stubs-1.20.0.post1/network.pyi
+-rw-r--r--   0        0        0       72 2023-06-07 16:29:08.835649 micropython_esp32_s3_stubs-1.20.0.post1/ntptime.pyi
+-rw-r--r--   0        0        0      617 2023-06-07 16:29:08.837901 micropython_esp32_s3_stubs-1.20.0.post1/onewire.pyi
+-rw-r--r--   0        0        0     9356 2023-06-07 16:29:08.478171 micropython_esp32_s3_stubs-1.20.0.post1/os.pyi
+-rw-r--r--   0        0        0      162 2023-06-07 16:29:08.479184 micropython_esp32_s3_stubs-1.20.0.post1/platform.pyi
+-rw-r--r--   0        0        0     4042 2023-07-03 13:38:08.175318 micropython_esp32_s3_stubs-1.20.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     2638 2023-06-07 16:29:08.480178 micropython_esp32_s3_stubs-1.20.0.post1/random.pyi
+-rw-r--r--   0        0        0     2002 2023-07-03 13:38:06.740713 micropython_esp32_s3_stubs-1.20.0.post1/README.md
+-rw-r--r--   0        0        0     3853 2023-06-07 16:29:08.481601 micropython_esp32_s3_stubs-1.20.0.post1/select.pyi
+-rw-r--r--   0        0        0     9602 2023-06-07 16:29:08.484187 micropython_esp32_s3_stubs-1.20.0.post1/socket.pyi
+-rw-r--r--   0        0        0     2668 2023-06-07 16:29:08.485194 micropython_esp32_s3_stubs-1.20.0.post1/ssl.pyi
+-rw-r--r--   0        0        0     4241 2023-06-07 16:29:08.487197 micropython_esp32_s3_stubs-1.20.0.post1/struct.pyi
+-rw-r--r--   0        0        0      875 2023-06-07 16:29:08.488487 micropython_esp32_s3_stubs-1.20.0.post1/sys.pyi
+-rw-r--r--   0        0        0    12515 2023-06-07 16:29:08.489505 micropython_esp32_s3_stubs-1.20.0.post1/time.pyi
+-rw-r--r--   0        0        0     1003 2023-06-07 16:29:08.491911 micropython_esp32_s3_stubs-1.20.0.post1/uarray.pyi
+-rw-r--r--   0        0        0      132 2023-06-07 16:29:08.838907 micropython_esp32_s3_stubs-1.20.0.post1/uasyncio/__init__.pyi
+-rw-r--r--   0        0        0     1530 2023-06-07 16:29:08.839914 micropython_esp32_s3_stubs-1.20.0.post1/uasyncio/core.pyi
+-rw-r--r--   0        0        0      625 2023-06-07 16:29:08.840907 micropython_esp32_s3_stubs-1.20.0.post1/uasyncio/event.pyi
+-rw-r--r--   0        0        0      390 2023-06-07 16:29:08.842908 micropython_esp32_s3_stubs-1.20.0.post1/uasyncio/funcs.pyi
+-rw-r--r--   0        0        0      414 2023-06-07 16:29:08.843915 micropython_esp32_s3_stubs-1.20.0.post1/uasyncio/lock.pyi
+-rw-r--r--   0        0        0     1410 2023-06-07 16:29:08.845927 micropython_esp32_s3_stubs-1.20.0.post1/uasyncio/stream.pyi
+-rw-r--r--   0        0        0      789 2023-06-07 16:29:08.846935 micropython_esp32_s3_stubs-1.20.0.post1/uasyncio/task.pyi
+-rw-r--r--   0        0        0     1408 2023-06-07 16:29:08.504582 micropython_esp32_s3_stubs-1.20.0.post1/ubinascii.pyi
+-rw-r--r--   0        0        0    31291 2023-06-07 16:29:08.505581 micropython_esp32_s3_stubs-1.20.0.post1/ubluetooth.pyi
+-rw-r--r--   0        0        0     3640 2023-06-07 16:29:08.507849 micropython_esp32_s3_stubs-1.20.0.post1/ucollections.pyi
+-rw-r--r--   0        0        0     1647 2023-06-07 16:29:08.509849 micropython_esp32_s3_stubs-1.20.0.post1/ucryptolib.pyi
+-rw-r--r--   0        0        0     2363 2023-06-07 16:29:08.511281 micropython_esp32_s3_stubs-1.20.0.post1/uctypes.pyi
+-rw-r--r--   0        0        0      709 2023-06-07 16:29:08.512551 micropython_esp32_s3_stubs-1.20.0.post1/uerrno.pyi
+-rw-r--r--   0        0        0     1642 2023-06-07 16:29:08.513557 micropython_esp32_s3_stubs-1.20.0.post1/uhashlib.pyi
+-rw-r--r--   0        0        0      930 2023-06-07 16:29:08.515559 micropython_esp32_s3_stubs-1.20.0.post1/uheapq.pyi
+-rw-r--r--   0        0        0     2650 2023-06-07 16:29:08.516794 micropython_esp32_s3_stubs-1.20.0.post1/uio.pyi
+-rw-r--r--   0        0        0     1384 2023-06-07 16:29:08.518806 micropython_esp32_s3_stubs-1.20.0.post1/ujson.pyi
+-rw-r--r--   0        0        0    52167 2023-06-07 16:29:08.521100 micropython_esp32_s3_stubs-1.20.0.post1/umachine.pyi
+-rw-r--r--   0        0        0        0 2023-06-07 16:29:08.848618 micropython_esp32_s3_stubs-1.20.0.post1/umqtt/__init__.pyi
+-rw-r--r--   0        0        0      377 2023-06-07 16:29:08.848618 micropython_esp32_s3_stubs-1.20.0.post1/umqtt/robust.pyi
+-rw-r--r--   0        0        0     1292 2023-06-07 16:29:08.851415 micropython_esp32_s3_stubs-1.20.0.post1/umqtt/simple.pyi
+-rw-r--r--   0        0        0     9356 2023-06-07 16:29:08.527107 micropython_esp32_s3_stubs-1.20.0.post1/uos.pyi
+-rw-r--r--   0        0        0      162 2023-06-07 16:29:08.529483 micropython_esp32_s3_stubs-1.20.0.post1/uplatform.pyi
+-rw-r--r--   0        0        0      641 2023-06-07 16:29:08.853421 micropython_esp32_s3_stubs-1.20.0.post1/upysh.pyi
+-rw-r--r--   0        0        0     2638 2023-06-07 16:29:08.530484 micropython_esp32_s3_stubs-1.20.0.post1/urandom.pyi
+-rw-r--r--   0        0        0      187 2023-06-07 16:29:08.531495 micropython_esp32_s3_stubs-1.20.0.post1/ure.pyi
+-rw-r--r--   0        0        0      739 2023-06-07 16:29:08.854726 micropython_esp32_s3_stubs-1.20.0.post1/urequests.pyi
+-rw-r--r--   0        0        0     3853 2023-06-07 16:29:08.535631 micropython_esp32_s3_stubs-1.20.0.post1/uselect.pyi
+-rw-r--r--   0        0        0     9602 2023-06-07 16:29:08.536638 micropython_esp32_s3_stubs-1.20.0.post1/usocket.pyi
+-rw-r--r--   0        0        0     2668 2023-06-07 16:29:08.538643 micropython_esp32_s3_stubs-1.20.0.post1/ussl.pyi
+-rw-r--r--   0        0        0     4241 2023-06-07 16:29:08.539644 micropython_esp32_s3_stubs-1.20.0.post1/ustruct.pyi
+-rw-r--r--   0        0        0      875 2023-06-07 16:29:08.541646 micropython_esp32_s3_stubs-1.20.0.post1/usys.pyi
+-rw-r--r--   0        0        0    12515 2023-06-07 16:29:08.542644 micropython_esp32_s3_stubs-1.20.0.post1/utime.pyi
+-rw-r--r--   0        0        0      245 2023-06-07 16:29:08.544644 micropython_esp32_s3_stubs-1.20.0.post1/utimeq.pyi
+-rw-r--r--   0        0        0      403 2023-06-07 16:29:08.545647 micropython_esp32_s3_stubs-1.20.0.post1/uwebsocket.pyi
+-rw-r--r--   0        0        0     1535 2023-06-07 16:29:08.546646 micropython_esp32_s3_stubs-1.20.0.post1/uzlib.pyi
+-rw-r--r--   0        0        0      513 2023-06-07 16:29:08.855898 micropython_esp32_s3_stubs-1.20.0.post1/webrepl.pyi
+-rw-r--r--   0        0        0      232 2023-06-07 16:29:08.857711 micropython_esp32_s3_stubs-1.20.0.post1/webrepl_setup.pyi
+-rw-r--r--   0        0        0      403 2023-06-07 16:29:08.547643 micropython_esp32_s3_stubs-1.20.0.post1/websocket.pyi
+-rw-r--r--   0        0        0     1535 2023-06-07 16:29:08.549941 micropython_esp32_s3_stubs-1.20.0.post1/zlib.pyi
+-rw-r--r--   0        0        0     3574 1970-01-01 00:00:00.000000 micropython_esp32_s3_stubs-1.20.0.post1/setup.py
+-rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 micropython_esp32_s3_stubs-1.20.0.post1/PKG-INFO
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/binascii.py` & `micropython_esp32_s3_stubs-1.20.0.post1/binascii.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,43 @@
 """
-binary/ASCII conversions. See: https://docs.micropython.org/en/v1.19.1/library/binascii.html
+binary/ASCII conversions. See: https://docs.micropython.org/en/v1.20.0/library/binascii.html
 
 |see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
 
 This module implements conversions between binary data and various
 encodings of it in ASCII form (in both directions).
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Any
 
-
-def crc32(*args, **kwargs) -> Any:
-    ...
-
-
+def crc32(*args, **kwargs) -> Any: ...
 def hexlify(data, sep: Optional[Any] = None) -> bytes:
     """
     Convert the bytes in the *data* object to a hexadecimal representation.
     Returns a bytes object.
 
     If the additional argument *sep* is supplied it is used as a separator
     between hexadecimal values.
     """
     ...
 
-
 def unhexlify(data) -> bytes:
     """
     Convert hexadecimal data to binary representation. Returns bytes string.
     (i.e. inverse of hexlify)
     """
     ...
 
-
 def b2a_base64(data, *, newline=True) -> bytes:
     """
     Encode binary data in base64 format, as in `RFC 3548
     <https://tools.ietf.org/html/rfc3548.html>`_. Returns the encoded data
     followed by a newline character if newline is true, as a bytes object.
     """
     ...
 
-
 def a2b_base64(data) -> bytes:
     """
     Decode base64-encoded data, ignoring invalid characters in the input.
     Conforms to `RFC 2045 s.6.8 <https://tools.ietf.org/html/rfc2045#section-6.8>`_.
     Returns a bytes object.
     """
     ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/bluetooth.py` & `micropython_esp32_s3_stubs-1.20.0.post1/bluetooth.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,80 +1,50 @@
 """
-Low-level Bluetooth radio functionality. See: https://docs.micropython.org/en/v1.19.1/library/bluetooth.html
+Low-level Bluetooth radio functionality. See: https://docs.micropython.org/en/v1.20.0/library/bluetooth.html
 
 This module provides an interface to a Bluetooth controller on a board.
 Currently this supports Bluetooth Low Energy (BLE) in Central, Peripheral,
 Broadcaster, and Observer roles, as well as GATT Server and Client and L2CAP
 connection-oriented-channels. A device may operate in multiple roles
 concurrently. Pairing (and bonding) is supported on some ports.
 
 This API is intended to match the low-level Bluetooth protocol and provide
 building-blocks for higher-level abstractions such as specific device types.
 
+``Note:`` For most applications, we recommend using the higher-level
+          `aioble library <https://github.com/micropython/micropython-lib/tree/master/micropython/bluetooth/aioble>`_.
+
 ``Note:`` This module is still under development and its classes, functions,
           methods and constants are subject to change.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Tuple, Any
 
-FLAG_NOTIFY = 16  # type: int
-FLAG_READ = 2  # type: int
-FLAG_WRITE = 8  # type: int
-FLAG_INDICATE = 32  # type: int
-FLAG_WRITE_NO_RESPONSE = 4  # type: int
-
+FLAG_NOTIFY: int
+FLAG_READ: int
+FLAG_WRITE: int
+FLAG_INDICATE: int
+FLAG_WRITE_NO_RESPONSE: int
 
 class UUID:
     """
     Creates a UUID instance with the specified **value**.
 
     The **value** can be either:
 
     - A 16-bit integer. e.g. ``0x2908``.
     - A 128-bit UUID string. e.g. ``'6E400001-B5A3-F393-E0A9-E50E24DCCA9E'``.
     """
 
-    def __init__(self, value, /) -> None:
-        ...
-
+    def __init__(self, value, /) -> None: ...
 
 class BLE:
     """
     Returns the singleton BLE object.
     """
 
-    def gatts_notify(self, conn_handle, value_handle, data=None, /) -> None:
-        """
-        Sends a notification request to a connected client.
-
-        If *data* is not ``None``, then that value is sent to the client as part of
-        the notification. The local value will not be modified.
-
-        Otherwise, if *data* is ``None``, then the current local value (as
-        set with :meth:`gatts_write <BLE.gatts_write>`) will be sent.
-
-        **Note:** The notification will be sent regardless of the subscription
-        status of the client to this characteristic.
-        """
-        ...
-
-    def gatts_indicate(self, conn_handle, value_handle, /) -> None:
-        """
-        Sends an indication request containing the characteristic's current value to
-        a connected client.
-
-        On acknowledgment (or failure, e.g. timeout), the
-        ``_IRQ_GATTS_INDICATE_DONE`` event will be raised.
-
-        **Note:** The indication will be sent regardless of the subscription
-        status of the client to this characteristic.
-        """
-        ...
-
     def gattc_write(self, conn_handle, value_handle, data, mode=0, /) -> None:
         """
         Issue a remote write to a connected server for the specified
         characteristic or descriptor handle.
 
         The argument *mode* specifies the write behaviour, with the currently
         supported values being:
@@ -86,70 +56,99 @@
               requested to send a response/acknowledgement that it received the
               data.
 
         If a response is received from the remote server the
         ``_IRQ_GATTC_WRITE_DONE`` event will be raised.
         """
         ...
+    def gatts_indicate(self, conn_handle, value_handle, data=None, /) -> None:
+        """
+        Sends a indication request to a connected client.
+
+        If *data* is ``None`` (the default), then the current local value (as set
+        with :meth:`gatts_write <BLE.gatts_write>`) will be sent.
 
+        Otherwise, if *data* is not ``None``, then that value is sent to the client
+        as part of the indication. The local value will not be modified.
+
+        On acknowledgment (or failure, e.g. timeout), the
+        ``_IRQ_GATTS_INDICATE_DONE`` event will be raised.
+
+        **Note:** The indication will be sent regardless of the subscription
+        status of the client to this characteristic.
+        """
+        ...
+    def gattc_discover_services(self, conn_handle, uuid=None, /) -> Any:
+        """
+        Query a connected server for its services.
+
+        Optionally specify a service *uuid* to query for that service only.
+
+        For each service discovered, the ``_IRQ_GATTC_SERVICE_RESULT`` event will
+        be raised, followed by ``_IRQ_GATTC_SERVICE_DONE`` on completion.
+        """
+        ...
     def gattc_read(self, conn_handle, value_handle, /) -> None:
         """
         Issue a remote read to a connected server for the specified
         characteristic or descriptor handle.
 
         When a value is available, the ``_IRQ_GATTC_READ_RESULT`` event will be
         raised. Additionally, the ``_IRQ_GATTC_READ_DONE`` will be raised.
         """
         ...
-
     def gattc_exchange_mtu(self, conn_handle, /) -> Any:
         """
         Initiate MTU exchange with a connected server, using the preferred MTU
         set using ``BLE.config(mtu=value)``.
 
         The ``_IRQ_MTU_EXCHANGED`` event will be raised when MTU exchange
         completes.
 
         **Note:** MTU exchange is typically initiated by the central. When using
         the BlueKitchen stack in the central role, it does not support a remote
         peripheral initiating the MTU exchange. NimBLE works for both roles.
 
         """
         ...
-
-    def gatts_read(self, value_handle, /) -> Any:
+    def gatts_set_buffer(self, value_handle, len, append=False, /) -> None:
         """
-        Reads the local value for this handle (which has either been written by
-        :meth:`gatts_write <BLE.gatts_write>` or by a remote client).
+        Sets the internal buffer size for a value in bytes. This will limit the
+        largest possible write that can be received. The default is 20.
+
+        Setting *append* to ``True`` will make all remote writes append to, rather
+        than replace, the current value. At most *len* bytes can be buffered in
+        this way. When you use :meth:`gatts_read <BLE.gatts_read>`, the value will
+        be cleared after reading. This feature is useful when implementing something
+        like the Nordic UART Service.
         """
         ...
-
     def gatts_write(self, value_handle, data, send_update=False, /) -> None:
         """
         Writes the local value for this handle, which can be read by a client.
 
         If *send_update* is ``True``, then any subscribed clients will be notified
         (or indicated, depending on what they're subscribed to and which operations
         the characteristic supports) about this write.
         """
         ...
-
-    def gatts_set_buffer(self, value_handle, len, append=False, /) -> None:
+    def gatts_notify(self, conn_handle, value_handle, data=None, /) -> None:
         """
-        Sets the internal buffer size for a value in bytes. This will limit the
-        largest possible write that can be received. The default is 20.
+        Sends a notification request to a connected client.
 
-        Setting *append* to ``True`` will make all remote writes append to, rather
-        than replace, the current value. At most *len* bytes can be buffered in
-        this way. When you use :meth:`gatts_read <BLE.gatts_read>`, the value will
-        be cleared after reading. This feature is useful when implementing something
-        like the Nordic UART Service.
+        If *data* is ``None`` (the default), then the current local value (as set
+        with :meth:`gatts_write <BLE.gatts_write>`) will be sent.
+
+        Otherwise, if *data* is not ``None``, then that value is sent to the client
+        as part of the notification. The local value will not be modified.
+
+        **Note:** The notification will be sent regardless of the subscription
+        status of the client to this characteristic.
         """
         ...
-
     def gatts_register_services(self, services_definition, /) -> Any:
         """
         Configures the server with the specified services, replacing any
         existing services.
 
         *services_definition* is a list of **services**, where each **service** is a
         two-element tuple containing a UUID and a list of **characteristics**.
@@ -204,15 +203,20 @@
             _FLAG_WRITE_ENCRYPTED = const(0x1000)
             _FLAG_WRITE_AUTHENTICATED = const(0x2000)
             _FLAG_WRITE_AUTHORIZED = const(0x4000)
 
         As for the IRQs above, any required constants should be added to your Python code.
         """
         ...
-
+    def gatts_read(self, value_handle, /) -> Any:
+        """
+        Reads the local value for this handle (which has either been written by
+        :meth:`gatts_write <BLE.gatts_write>` or by a remote client).
+        """
+        ...
     def irq(self, handler, /) -> int:
         """
             Registers a callback for events from the BLE stack. The *handler* takes two
             arguments, ``event`` (which will be one of the codes below) and ``data``
             (which is an event-specific tuple of values).
 
             **Note:** As an optimisation to prevent unnecessary allocations, the ``addr``,
@@ -266,15 +270,15 @@
                         conn_handle, start_handle, end_handle, uuid = data
                     elif event == _IRQ_GATTC_SERVICE_DONE:
                         # Called once service discovery is complete.
                         # Note: Status will be zero on success, implementation-specific value otherwise.
                         conn_handle, status = data
                     elif event == _IRQ_GATTC_CHARACTERISTIC_RESULT:
                         # Called for each characteristic found by gattc_discover_services().
-                        conn_handle, def_handle, value_handle, properties, uuid = data
+                        conn_handle, end_handle, value_handle, properties, uuid = data
                     elif event == _IRQ_GATTC_CHARACTERISTIC_DONE:
                         # Called once service discovery is complete.
                         # Note: Status will be zero on success, implementation-specific value otherwise.
                         conn_handle, status = data
                     elif event == _IRQ_GATTC_DESCRIPTOR_RESULT:
                         # Called for each descriptor found by gattc_discover_descriptors().
                         conn_handle, dsc_handle, uuid = data
@@ -283,20 +287,18 @@
                         # Note: Status will be zero on success, implementation-specific value otherwise.
                         conn_handle, status = data
                     elif event == _IRQ_GATTC_READ_RESULT:
                         # A gattc_read() has completed.
                         conn_handle, value_handle, char_data = data
                     elif event == _IRQ_GATTC_READ_DONE:
                         # A gattc_read() has completed.
-                        # Note: The value_handle will be zero on btstack (but present on NimBLE).
                         # Note: Status will be zero on success, implementation-specific value otherwise.
                         conn_handle, value_handle, status = data
                     elif event == _IRQ_GATTC_WRITE_DONE:
                         # A gattc_write() has completed.
-                        # Note: The value_handle will be zero on btstack (but present on NimBLE).
                         # Note: Status will be zero on success, implementation-specific value otherwise.
                         conn_handle, value_handle, status = data
                     elif event == _IRQ_GATTC_NOTIFY:
                         # A server has sent a notify request.
                         conn_handle, value_handle, notify_data = data
                     elif event == _IRQ_GATTC_INDICATE:
                         # A server has sent an indicate request.
@@ -401,15 +403,31 @@
 
         In order to save space in the firmware, these constants are not included on the
         :mod:`bluetooth` module. Add the ones that you need from the list above to your
         program.
 
         """
         ...
+    def gap_advertise(self, interval_us, adv_data=None, *, resp_data=None, connectable=True) -> Any:
+        """
+        Starts advertising at the specified interval (in **micro** seconds). This
+        interval will be rounded down to the nearest 625us. To stop advertising, set
+        *interval_us* to ``None``.
+
+        *adv_data* and *resp_data* can be any type that implements the buffer
+        protocol (e.g. ``bytes``, ``bytearray``, ``str``). *adv_data* is included
+        in all broadcasts, and *resp_data* is send in reply to an active scan.
 
+        **Note:** if *adv_data* (or *resp_data*) is ``None``, then the data passed
+        to the previous call to ``gap_advertise`` will be re-used. This allows a
+        broadcaster to resume advertising with just ``gap_advertise(interval_us)``.
+        To clear the advertising payload pass an empty ``bytes``, i.e. ``b''``.
+
+        """
+        ...
     def gap_connect(self, addr_type, addr, scan_duration_ms=2000, min_conn_interval_us=None, max_conn_interval_us=None, /) -> None:
         """
         Connect to a peripheral.
 
         See :meth:`gap_scan <BLE.gap_scan>` for details about address types.
 
         To cancel an outstanding connection attempt early, call
@@ -426,33 +444,22 @@
         or both of *min_conn_interval_us* and *max_conn_interval_us*. Otherwise a
         default interval will be chosen, typically between 30000 and 50000
         microseconds. A shorter interval will increase throughput, at the expense
         of power usage.
 
         """
         ...
-
-    def gap_advertise(self, interval_us, adv_data=None, *, resp_data=None, connectable=True) -> Any:
+    def gattc_discover_descriptors(self, conn_handle, start_handle, end_handle, /) -> Any:
         """
-        Starts advertising at the specified interval (in **micro** seconds). This
-        interval will be rounded down to the nearest 625us. To stop advertising, set
-        *interval_us* to ``None``.
-
-        *adv_data* and *resp_data* can be any type that implements the buffer
-        protocol (e.g. ``bytes``, ``bytearray``, ``str``). *adv_data* is included
-        in all broadcasts, and *resp_data* is send in reply to an active scan.
-
-        **Note:** if *adv_data* (or *resp_data*) is ``None``, then the data passed
-        to the previous call to ``gap_advertise`` will be re-used. This allows a
-        broadcaster to resume advertising with just ``gap_advertise(interval_us)``.
-        To clear the advertising payload pass an empty ``bytes``, i.e. ``b''``.
+        Query a connected server for descriptors in the specified range.
 
+        For each descriptor discovered, the ``_IRQ_GATTC_DESCRIPTOR_RESULT`` event
+        will be raised, followed by ``_IRQ_GATTC_DESCRIPTOR_DONE`` on completion.
         """
         ...
-
     def config(self, param, /) -> Tuple:
         """
         Get or set configuration values of the BLE interface.  To get a value the
         parameter name should be quoted as a string, and just one parameter is
         queried at a time.  To set values use the keyword syntax, and one ore more
         parameter can be set at a time.
 
@@ -508,75 +515,22 @@
             _IO_CAPABILITY_NO_INPUT_OUTPUT = const(3)
             _IO_CAPABILITY_KEYBOARD_DISPLAY = const(4)
 
         - ``'le_secure'``: Sets whether "LE Secure" pairing is required. Default is
           false (i.e. allow "Legacy Pairing").
         """
         ...
-
     def active(self, active: Optional[Any] = None, /) -> Any:
         """
         Optionally changes the active state of the BLE radio, and returns the
         current state.
 
         The radio must be made active before using any other methods on this class.
         """
         ...
-
-    def gattc_discover_services(self, conn_handle, uuid=None, /) -> Any:
-        """
-        Query a connected server for its services.
-
-        Optionally specify a service *uuid* to query for that service only.
-
-        For each service discovered, the ``_IRQ_GATTC_SERVICE_RESULT`` event will
-        be raised, followed by ``_IRQ_GATTC_SERVICE_DONE`` on completion.
-        """
-        ...
-
-    def gap_disconnect(self, conn_handle, /) -> bool:
-        """
-        Disconnect the specified connection handle. This can either be a
-        central that has connected to this device (if acting as a peripheral)
-        or a peripheral that was previously connected to by this device (if acting
-        as a central).
-
-        On success, the ``_IRQ_PERIPHERAL_DISCONNECT`` or ``_IRQ_CENTRAL_DISCONNECT``
-        event will be raised.
-
-        Returns ``False`` if the connection handle wasn't connected, and ``True``
-        otherwise.
-
-        """
-        ...
-
-    def gattc_discover_descriptors(self, conn_handle, start_handle, end_handle, /) -> Any:
-        """
-        Query a connected server for descriptors in the specified range.
-
-        For each descriptor discovered, the ``_IRQ_GATTC_DESCRIPTOR_RESULT`` event
-        will be raised, followed by ``_IRQ_GATTC_DESCRIPTOR_DONE`` on completion.
-        """
-        ...
-
-    def gattc_discover_characteristics(self, conn_handle, start_handle, end_handle, uuid=None, /) -> Any:
-        """
-        Query a connected server for characteristics in the specified range.
-
-        Optionally specify a characteristic *uuid* to query for that
-        characteristic only.
-
-        You can use ``start_handle=1``, ``end_handle=0xffff`` to search for a
-        characteristic in any service.
-
-        For each characteristic discovered, the ``_IRQ_GATTC_CHARACTERISTIC_RESULT``
-        event will be raised, followed by ``_IRQ_GATTC_CHARACTERISTIC_DONE`` on completion.
-        """
-        ...
-
     def gap_scan(self, duration_ms, interval_us=1280000, window_us=11250, active=False, /) -> Any:
         """
         Run a scan operation lasting for the specified duration (in **milli** seconds).
 
         To scan indefinitely, set *duration_ms* to ``0``.
 
         To stop scanning, set *duration_ms* to ``None``.
@@ -605,10 +559,65 @@
         ``active`` can be set ``True`` if you want to receive scan responses in the results.
 
         When scanning is stopped (either due to the duration finishing or when
         explicitly stopped), the ``_IRQ_SCAN_DONE`` event will be raised.
 
         """
         ...
+    def gattc_discover_characteristics(self, conn_handle, start_handle, end_handle, uuid=None, /) -> Any:
+        """
+        Query a connected server for characteristics in the specified range.
+
+        Optionally specify a characteristic *uuid* to query for that
+        characteristic only.
+
+        You can use ``start_handle=1``, ``end_handle=0xffff`` to search for a
+        characteristic in any service.
+
+        For each characteristic discovered, the ``_IRQ_GATTC_CHARACTERISTIC_RESULT``
+        event will be raised, followed by ``_IRQ_GATTC_CHARACTERISTIC_DONE`` on completion.
+        """
+        ...
+    def gap_disconnect(self, conn_handle, /) -> bool:
+        """
+        Disconnect the specified connection handle. This can either be a
+        central that has connected to this device (if acting as a peripheral)
+        or a peripheral that was previously connected to by this device (if acting
+        as a central).
+
+        On success, the ``_IRQ_PERIPHERAL_DISCONNECT`` or ``_IRQ_CENTRAL_DISCONNECT``
+        event will be raised.
+
+        Returns ``False`` if the connection handle wasn't connected, and ``True``
+        otherwise.
+
+        """
+        ...
+    def gap_passkey(self, conn_handle, action, passkey, /) -> Any:
+        """
+        Respond to a ``_IRQ_PASSKEY_ACTION`` event for the specified *conn_handle*
+        and *action*.
+
+        The *passkey* is a numeric value and will depend on on the
+        *action* (which will depend on what I/O capability has been set):
+
+            * When the *action* is ``_PASSKEY_ACTION_INPUT``, then the application should
+              prompt the user to enter the passkey that is shown on the remote device.
+            * When the *action* is ``_PASSKEY_ACTION_DISPLAY``, then the application should
+              generate a random 6-digit passkey and show it to the user.
+            * When the *action* is ``_PASSKEY_ACTION_NUMERIC_COMPARISON``, then the application
+              should show the passkey that was provided in the ``_IRQ_PASSKEY_ACTION`` event
+              and then respond with either ``0`` (cancel pairing), or ``1`` (accept pairing).
 
-    def __init__(self) -> None:
+        """
+        ...
+    def gap_pair(self, conn_handle, /) -> Any:
+        """
+        Initiate pairing with the remote device.
+
+        Before calling this, ensure that the ``io``, ``mitm``, ``le_secure``, and
+        ``bond`` configuration options are set (via :meth:`config<BLE.config>`).
+
+        On successful pairing, the ``_IRQ_ENCRYPTION_UPDATE`` event will be raised.
+        """
         ...
+    def __init__(self) -> None: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/btree.py` & `micropython_esp32_s3_stubs-1.20.0.post1/btree.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
-simple BTree database. See: https://docs.micropython.org/en/v1.19.1/library/btree.html
+simple BTree database. See: https://docs.micropython.org/en/v1.20.0/library/btree.html
 
 The ``btree`` module implements a simple key-value database using external
 storage (disk files, or in general case, a random-access `stream`). Keys are
 stored sorted in the database, and besides efficient retrieval by a key
 value, a database also supports efficient ordered range scans (retrieval
 of values with the keys in a given range). On the application interface
 side, BTree database work as close a possible to a way standard `dict`
 type works, one notable difference is that both keys and values must
-be `bytes` objects (so, if you want to store objects of other types, you
-need to serialize them to `bytes` first).
+be `bytes`-like objects (so, if you want to store objects of other types, you
+need to first serialize them to `str` or `bytes` or another type that supports
+the buffer protocol).
 
 The module is based on the well-known BerkelyDB library, version 1.xx.
 
 Example::
 
     import btree
 
@@ -66,21 +67,18 @@
 
     db.close()
 
     # Don't forget to close the underlying stream!
     f.close()
 
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Dict, Optional, Any
 
-DESC = 2  # type: int
-INCL = 1  # type: int
-
+DESC: int
+INCL: int
 
 def open(stream, *, flags=0, pagesize=0, cachesize=0, minkeypage=0) -> Dict:
     """
     Open a database from a random-access `stream` (like an open file). All
     other parameters are optional and keyword-only, and allow to tweak advanced
     parameters of the database operation (most users will not need them):
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/cmath.py` & `micropython_esp32_s3_stubs-1.20.0.post1/cmath.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,69 @@
 """
-mathematical functions for complex numbers. See: https://docs.micropython.org/en/v1.19.1/library/cmath.html
+mathematical functions for complex numbers. See: https://docs.micropython.org/en/v1.20.0/library/cmath.html
 
 |see_cpython_module| :mod:`python:cmath` https://docs.python.org/3/library/cmath.html .
 
 The ``cmath`` module provides some basic mathematical functions for
 working with complex numbers.
 
 Availability: not available on WiPy and ESP8266. Floating point support
 required for this module.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Tuple, Any
 
-e = 2.718282  # type: float
-pi = 3.141593  # type: float
-
+e: float
+pi: float
 
 def polar(z) -> Tuple:
     """
     Returns, as a tuple, the polar form of ``z``.
     """
     ...
 
-
 def sqrt(z) -> Any:
     """
     Return the square-root of ``z``.
     """
     ...
 
-
 def rect(r, phi) -> float:
     """
     Returns the complex number with modulus ``r`` and phase ``phi``.
     """
     ...
 
-
 def sin(z) -> float:
     """
     Return the sine of ``z``.
     """
     ...
 
-
 def exp(z) -> float:
     """
     Return the exponential of ``z``.
     """
     ...
 
-
 def cos(z) -> float:
     """
     Return the cosine of ``z``.
     """
     ...
 
-
 def phase(z) -> float:
     """
     Returns the phase of the number ``z``, in the range (-pi, +pi].
     """
     ...
 
-
 def log(z) -> float:
     """
     Return the natural logarithm of ``z``.  The branch cut is along the negative real axis.
     """
     ...
 
-
 def log10(z) -> float:
     """
     Return the base-10 logarithm of ``z``.  The branch cut is along the negative real axis.
     """
     ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/collections.py` & `micropython_esp32_s3_stubs-1.20.0.post1/collections.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """
-collection and container types. See: https://docs.micropython.org/en/v1.19.1/library/collections.html
+collection and container types. See: https://docs.micropython.org/en/v1.20.0/library/collections.html
 
 |see_cpython_module| :mod:`python:collections` https://docs.python.org/3/library/collections.html .
 
 This module implements advanced collection and container types to
 hold/accumulate various objects.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Any
 from queue import Queue
 
-
 def namedtuple(name, fields) -> Any:
     """
     This is factory function to create a new namedtuple type with a specific
     name and set of fields. A namedtuple is a subclass of tuple which allows
     to access its fields not just by numeric index, but also with an attribute
     access syntax using symbolic field names. Fields is a sequence of strings
     specifying field names. For compatibility with CPython it can also be a
@@ -28,16 +25,15 @@
         t1 = MyTuple(1, "foo")
         t2 = MyTuple(2, "bar")
         print(t1.name)
         assert t2.name == t2[1]
     """
     ...
 
-
-class OrderedDict:
+class OrderedDict(dict):
     """
     ``dict`` type subclass which remembers and preserves the order of keys
     added. When ordered dict is iterated over, keys/items are returned in
     the order they were added::
 
         from collections import OrderedDict
 
@@ -54,53 +50,29 @@
 
         z 1
         a 2
         w 5
         b 3
     """
 
-    def popitem(self, *args, **kwargs) -> Any:
-        ...
-
-    def pop(self, *args, **kwargs) -> Any:
-        ...
-
-    def values(self, *args, **kwargs) -> Any:
-        ...
-
-    def setdefault(self, *args, **kwargs) -> Any:
-        ...
-
-    def update(self, *args, **kwargs) -> Any:
-        ...
-
-    def copy(self, *args, **kwargs) -> Any:
-        ...
-
-    def clear(self, *args, **kwargs) -> Any:
-        ...
-
-    def keys(self, *args, **kwargs) -> Any:
-        ...
-
-    def get(self, *args, **kwargs) -> Any:
-        ...
-
-    def items(self, *args, **kwargs) -> Any:
-        ...
-
+    def popitem(self, *args, **kwargs) -> Any: ...
+    def pop(self, *args, **kwargs) -> Any: ...
+    def values(self, *args, **kwargs) -> Any: ...
+    def setdefault(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def copy(self, *args, **kwargs) -> Any: ...
+    def clear(self, *args, **kwargs) -> Any: ...
+    def keys(self, *args, **kwargs) -> Any: ...
+    def get(self, *args, **kwargs) -> Any: ...
+    def items(self, *args, **kwargs) -> Any: ...
     @classmethod
-    def fromkeys(cls, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, *args, **kwargs) -> None:
-        ...
-
+    def fromkeys(cls, *args, **kwargs) -> Any: ...
+    def __init__(self, *args, **kwargs) -> None: ...
 
-class deque:
+class deque(Queue):
     """
     Deques (double-ended queues) are a list-like container that support O(1)
     appends and pops from either side of the deque.  New deques are created
     using the following arguments:
 
         - *iterable* must be the empty tuple, and the new deque is created empty.
 
@@ -116,17 +88,14 @@
 
     def popleft(self) -> Any:
         """
         Remove and return an item from the left side of the deque.
         Raises IndexError if no items are present.
         """
         ...
-
     def append(self, x) -> Any:
         """
         Add *x* to the right side of the deque.
         Raises IndexError if overflow checking is enabled and there is no more room left.
         """
         ...
-
-    def __init__(self, iterable, maxlen, flags: Optional[Any] = None) -> None:
-        ...
+    def __init__(self, iterable, maxlen, flags: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/cryptolib.py` & `micropython_esp32_s3_stubs-1.20.0.post1/cryptolib.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 """
-cryptographic ciphers. See: https://docs.micropython.org/en/v1.19.1/library/cryptolib.html
+cryptographic ciphers. See: https://docs.micropython.org/en/v1.20.0/library/cryptolib.html
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Any
 
-
 class aes:
     def encrypt(self, in_buf, out_buf: Optional[Any] = None) -> Any:
         """
         Encrypt *in_buf*. If no *out_buf* is given result is returned as a
         newly allocated `bytes` object. Otherwise, result is written into
         mutable buffer *out_buf*. *in_buf* and *out_buf* can also refer
         to the same mutable buffer, in which case data is encrypted in-place.
         """
         ...
-
     def decrypt(self, in_buf, out_buf: Optional[Any] = None) -> Any:
         """
         Like `encrypt()`, but for decryption.
         """
         ...
-
     def __init__(self, key, mode, IV: Optional[Any] = None) -> None:
         """
         Initialize cipher object, suitable for encryption/decryption. Note:
         after initialization, cipher object can be use only either for
         encryption or decryption. Running decrypt() operation after encrypt()
         or vice versa is not supported.
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/esp.py` & `micropython_esp32_s3_stubs-1.20.0.post1/esp.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,23 @@
 """
-functions related to the ESP8266 and ESP32. See: https://docs.micropython.org/en/v1.19.1/library/esp.html
+functions related to the ESP8266 and ESP32. See: https://docs.micropython.org/en/v1.20.0/library/esp.html
 
 The ``esp`` module contains specific functions related to both the ESP8266 and
 ESP32 modules.  Some functions are only available on one or the other of these
 ports.
 
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Any
 
-LOG_NONE = 0  # type: int
-LOG_WARNING = 2  # type: int
-LOG_VERBOSE = 5  # type: int
-LOG_DEBUG = 4  # type: int
-LOG_INFO = 3  # type: int
-LOG_ERROR = 1  # type: int
-
-
-def flash_user_start() -> Any:
-    """
-    Read the memory offset at which the user flash space begins.
-    """
-    ...
-
-
-def flash_write(byte_offset, bytes) -> Any:
-    ...
-
-
-def gpio_matrix_in(*args, **kwargs) -> Any:
-    ...
-
-
-def gpio_matrix_out(*args, **kwargs) -> Any:
-    ...
-
+LOG_NONE: int
+LOG_WARNING: int
+LOG_VERBOSE: int
+LOG_DEBUG: int
+LOG_INFO: int
+LOG_ERROR: int
 
 def osdebug(level) -> None:
     """
     Turn esp os debugging messages on or off.
 
     The *level* parameter sets the threshold for the log messages for all esp components.
     The log levels are defined as constants:
@@ -50,25 +28,23 @@
         * ``LOG_INFO`` -- Information messages which describe normal flow of events
         * ``LOG_DEBUG`` -- Extra information which is not necessary for normal use (values, pointers, sizes, etc)
         * ``LOG_VERBOSE`` -- Bigger chunks of debugging information, or frequent messages
           which can potentially flood the output
     """
     ...
 
+def flash_write(byte_offset, bytes) -> Any: ...
+def gpio_matrix_in(*args, **kwargs) -> Any: ...
+def gpio_matrix_out(*args, **kwargs) -> Any: ...
+def flash_user_start() -> Any:
+    """
+    Read the memory offset at which the user flash space begins.
+    """
+    ...
 
+def flash_erase(sector_no) -> Any: ...
+def flash_read(byte_offset, length_or_buffer) -> Any: ...
 def flash_size() -> Any:
     """
     Read the total size of the flash memory.
     """
     ...
-
-
-def dht_readinto(*args, **kwargs) -> Any:
-    ...
-
-
-def flash_erase(sector_no) -> Any:
-    ...
-
-
-def flash_read(byte_offset, length_or_buffer) -> Any:
-    ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/esp32.py` & `micropython_esp32_s3_stubs-1.20.0.post1/esp32.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,21 @@
 """
-functionality specific to the ESP32. See: https://docs.micropython.org/en/v1.19.1/library/esp32.html
+functionality specific to the ESP32. See: https://docs.micropython.org/en/v1.20.0/library/esp32.html
 
 The ``esp32`` module contains functions and classes specifically aimed at
 controlling ESP32 modules.
 
 """
 from __future__ import annotations
-
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import List, Optional, Tuple, Union, Any
 
-WAKEUP_ALL_LOW = False  # type: bool
-WAKEUP_ANY_HIGH = True  # type: bool
-HEAP_EXEC = 1  # type: int
-HEAP_DATA = 4  # type: int
-
-
-def wake_on_touch(wake) -> None:
-    """
-    Configure whether or not a touch will wake the device from sleep.
-    *wake* should be a boolean value.
-    """
-    ...
-
-
-def wake_on_ext1(pins, level) -> None:
-    """
-    Configure how EXT1 wakes the device from sleep.  *pins* can be ``None``
-    or a tuple/list of valid Pin objects.  *level* should be ``esp32.WAKEUP_ALL_LOW``
-    or ``esp32.WAKEUP_ANY_HIGH``.
-    """
-    ...
-
+WAKEUP_ALL_LOW: bool
+WAKEUP_ANY_HIGH: bool
+HEAP_EXEC: int
+HEAP_DATA: int
 
 def idf_heap_info(capabilities) -> List[Tuple]:
     """
     Returns information about the ESP-IDF heap memory regions. One of them contains
     the MicroPython heap and the others are used by ESP-IDF, e.g., for network
     buffers and other data. This data is useful to get a sense of how much memory
     is available to ESP-IDF and the networking stack in particular. It may shed
@@ -56,83 +35,94 @@
 
         >>> import esp32; esp32.idf_heap_info(esp32.HEAP_DATA)
         [(240, 0, 0, 0), (7288, 0, 0, 0), (16648, 4, 4, 4), (79912, 35712, 35512, 35108),
          (15072, 15036, 15036, 15036), (113840, 0, 0, 0)]
     """
     ...
 
+def wake_on_touch(wake) -> None:
+    """
+    Configure whether or not a touch will wake the device from sleep.
+    *wake* should be a boolean value.
+    """
+    ...
 
 def wake_on_ext0(pin, level) -> None:
     """
     Configure how EXT0 wakes the device from sleep.  *pin* can be ``None``
     or a valid Pin object.  *level* should be ``esp32.WAKEUP_ALL_LOW`` or
     ``esp32.WAKEUP_ANY_HIGH``.
     """
     ...
 
+def wake_on_ext1(pins, level) -> None:
+    """
+    Configure how EXT1 wakes the device from sleep.  *pins* can be ``None``
+    or a tuple/list of valid Pin objects.  *level* should be ``esp32.WAKEUP_ALL_LOW``
+    or ``esp32.WAKEUP_ANY_HIGH``.
+    """
+    ...
+
+def wake_on_ulp(wake) -> None:
+    """
+    Configure whether or not the Ultra-Low-Power co-processor can wake the
+    device from sleep. *wake* should be a boolean value.
+    """
+    ...
 
 def gpio_deep_sleep_hold(enable) -> None:
     """
     Configure whether non-RTC GPIO pin configuration is retained during
     deep-sleep mode for held pads. *enable* should be a boolean value.
     """
     ...
 
-
 class NVS:
     """
     Create an object providing access to a namespace (which is automatically created if not
     present).
     """
 
     def get_i32(self, key) -> int:
         """
         Returns the signed integer value for the specified key. Raises an OSError if the key does not
         exist or has a different type.
         """
         ...
-
     def set_i32(self, key, value) -> None:
         """
         Sets a 32-bit signed integer value for the specified key. Remember to call *commit*!
         """
         ...
-
     def set_blob(self, key, value) -> None:
         """
         Sets a binary blob value for the specified key. The value passed in must support the buffer
         protocol, e.g. bytes, bytearray, str. (Note that esp-idf distinguishes blobs and strings, this
         method always writes a blob even if a string is passed in as value.)
         Remember to call *commit*!
         """
         ...
-
     def commit(self) -> Any:
         """
         Commits changes made by *set_xxx* methods to flash.
         """
         ...
-
     def get_blob(self, key, buffer) -> int:
         """
         Reads the value of the blob for the specified key into the buffer, which must be a bytearray.
         Returns the actual length read. Raises an OSError if the key does not exist, has a different
         type, or if the buffer is too small.
         """
         ...
-
     def erase_key(self, key) -> Any:
         """
         Erases a key-value pair.
         """
         ...
-
-    def __init__(self, namespace) -> None:
-        ...
-
+    def __init__(self, namespace) -> None: ...
 
 class RMT:
     """
     This class provides access to one of the eight RMT channels. *channel* is
     required and identifies which RMT channel (0-7) will be configured. *pin*,
     also required, configures which Pin is bound to the RMT channel. *clock_div*
     is an 8-bit clock divider that divides the source clock (80MHz) to the RMT
@@ -149,33 +139,30 @@
 
     def source_freq(self) -> Any:
         """
         Returns the source clock frequency. Currently the source clock is not
         configurable so this will always return 80MHz.
         """
         ...
-
     def loop(self, enable_loop) -> None:
         """
         Configure looping on the channel. *enable_loop* is bool, set to ``True`` to
         enable looping on the *next* call to `RMT.write_pulses`. If called with
         ``False`` while a looping sequence is currently being transmitted then the
         current loop iteration will be completed and then transmission will stop.
         """
         ...
-
     def wait_done(self, *, timeout=0) -> bool:
         """
         Returns ``True`` if the channel is idle or ``False`` if a sequence of
         pulses started with `RMT.write_pulses` is being transmitted. If the
         *timeout* keyword argument is given then block for up to this many
         milliseconds for transmission to complete.
         """
         ...
-
     def write_pulses(self, duration, data: Union[bool, int] = True) -> Any:
         """
         Begin transmitting a sequence. There are three ways to specify this:
 
         **Mode 1:** *duration* is a list or tuple of durations. The optional *data*
         argument specifies the initial output level. The output level will toggle
         after each duration.
@@ -197,111 +184,92 @@
         If looping has been enabled with `RMT.loop`, the sequence will be
         repeated indefinitely. Further calls to this method will block until the
         end of the current loop iteration before immediately beginning to loop the
         new sequence of pulses. Looping sequences longer than 126 pulses is not
         supported by the hardware.
         """
         ...
-
     @staticmethod
     def bitstream_channel(value: Optional[Any] = None) -> int:
         """
         Select which RMT channel is used by the `machine.bitstream` implementation.
         *value* can be ``None`` or a valid RMT channel number.  The default RMT
         channel is the highest numbered one.
 
         Passing in ``None`` disables the use of RMT and instead selects a bit-banging
         implementation for `machine.bitstream`.
 
         Passing in no argument will not change the channel.  This function returns
         the current channel number.
         """
         ...
-
-    def deinit(self, *args, **kwargs) -> Any:
-        ...
-
+    def deinit(self, *args, **kwargs) -> Any: ...
     def clock_div(self) -> Any:
         """
         Return the clock divider. Note that the channel resolution is
         ``1 / (source_freq / clock_div)``.
         """
         ...
-
-    def __init__(self, channel, *, pin=None, clock_div=8, idle_level=False, tx_carrier=None) -> None:
-        ...
-
+    def __init__(self, channel, *, pin=None, clock_div=8, idle_level=False, tx_carrier=None) -> None: ...
 
 class Partition:
     """
     Create an object representing a partition.  *id* can be a string which is the label
     of the partition to retrieve, or one of the constants: ``BOOT`` or ``RUNNING``.
     *block_size* specifies the byte size of an individual block.
     """
 
-    RUNNING = 1  # type: int
-    TYPE_APP = 0  # type: int
-    TYPE_DATA = 1  # type: int
-    BOOT = 0  # type: int
-
-    def readblocks(self, block_num, buf, offset: Optional[int] = 0) -> Any:
-        ...
-
+    RUNNING: int
+    TYPE_APP: int
+    TYPE_DATA: int
+    BOOT: int
+    def readblocks(self, block_num, buf, offset: Optional[int] = 0) -> Any: ...
     def ioctl(self, cmd, arg) -> Any:
         """
         These methods implement the simple and :ref:`extended
         <block-device-interface>` block protocol defined by
         :class:`os.AbstractBlockDev`.
         """
         ...
-
     def set_boot(self) -> None:
         """
         Sets the partition as the boot partition.
         """
         ...
-
-    def writeblocks(self, block_num, buf, offset: Optional[int] = 0) -> Any:
-        ...
-
+    def writeblocks(self, block_num, buf, offset: Optional[int] = 0) -> Any: ...
     def info(self) -> Tuple:
         """
         Returns a 6-tuple ``(type, subtype, addr, size, label, encrypted)``.
         """
         ...
-
     @classmethod
     def find(cls, type=TYPE_APP, subtype=0xFF, label=None, block_size=4096) -> List:
         """
         Find a partition specified by *type*, *subtype* and *label*.  Returns a
         (possibly empty) list of Partition objects. Note: ``subtype=0xff`` matches any subtype
         and ``label=None`` matches any label.
 
         *block_size* specifies the byte size of an individual block used by the returned
         objects.
         """
         ...
-
     def get_next_update(self) -> Partition:
         """
         Gets the next update partition after this one, and returns a new Partition object.
         Typical usage is ``Partition(Partition.RUNNING).get_next_update()``
         which returns the next partition to update given the current running one.
         """
         ...
-
     @classmethod
     def mark_app_valid_cancel_rollback(cls) -> Any:
         """
         Signals that the current boot is considered successful.
         Calling ``mark_app_valid_cancel_rollback`` is required on the first boot of a new
         partition to avoid an automatic rollback at the next boot.
         This uses the ESP-IDF "app rollback" feature with "CONFIG_BOOTLOADER_APP_ROLLBACK_ENABLE"
         and  an ``OSError(-261)`` is raised if called on firmware that doesn't have the
         feature enabled.
         It is OK to call ``mark_app_valid_cancel_rollback`` on every boot and it is not
         necessary when booting firmare that was loaded using esptool.
         """
         ...
-
-    def __init__(self, id, block_size=4096, /) -> None:
-        ...
+    def __init__(self, id, block_size=4096, /) -> None: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/framebuf.py` & `micropython_esp32_s3_stubs-1.20.0.post1/framebuf.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 """
-Frame buffer manipulation. See: https://docs.micropython.org/en/v1.19.1/library/framebuf.html
+Frame buffer manipulation. See: https://docs.micropython.org/en/v1.20.0/library/framebuf.html
 
 This module provides a general frame buffer which can be used to create
 bitmap images, which can then be sent to a display.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Any
 
-MONO_HMSB = 4  # type: int
-MONO_HLSB = 3  # type: int
-RGB565 = 1  # type: int
-MONO_VLSB = 0  # type: int
-MVLSB = 0  # type: int
-GS2_HMSB = 5  # type: int
-GS8 = 6  # type: int
-GS4_HMSB = 2  # type: int
-
-
-def FrameBuffer1(*args, **kwargs) -> Any:
-    ...
+MONO_HMSB: int
+MONO_HLSB: int
+RGB565: int
+MONO_VLSB: int
+MVLSB: int
+GS2_HMSB: int
+GS8: int
+GS4_HMSB: int
 
+def FrameBuffer1(*args, **kwargs) -> Any: ...
 
 class FrameBuffer:
     """
     Construct a FrameBuffer object.  The parameters are:
 
         - *buffer* is an object with a buffer protocol which must be large
           enough to contain every pixel defined by the width, height and
@@ -44,86 +39,102 @@
           an increased step size.
 
     One must specify valid *buffer*, *width*, *height*, *format* and
     optionally *stride*.  Invalid *buffer* size or dimensions may lead to
     unexpected errors.
     """
 
-    def rect(self, x, y, w, h, c) -> Any:
-        ...
+    def poly(self, x, y, coords, c, f: Optional[Any] = None) -> Any:
+        """
+        Given a list of coordinates, draw an arbitrary (convex or concave) closed
+        polygon at the given x, y location using the given color.
 
+        The *coords* must be specified as a :mod:`array` of integers, e.g.
+        ``array('h', [x0, y0, x1, y1, ... xn, yn])``.
+
+        The optional *f* parameter can be set to ``True`` to fill the polygon.
+        Otherwise just a one pixel outline is drawn.
+        """
+        ...
+    def vline(self, x, y, h, c) -> Any: ...
     def pixel(self, x, y, c: Optional[Any] = None) -> Any:
         """
         If *c* is not given, get the color value of the specified pixel.
         If *c* is given, set the specified pixel to the given color.
         """
         ...
+    def text(self, s, x, y, c: Optional[Any] = None) -> None:
+        """
+        Write text to the FrameBuffer using the the coordinates as the upper-left
+        corner of the text. The color of the text can be defined by the optional
+        argument but is otherwise a default value of 1. All characters have
+        dimensions of 8x8 pixels and there is currently no way to change the font.
 
-    def vline(self, x, y, h, c) -> Any:
+        """
         ...
+    def rect(self, x, y, w, h, c, f: Optional[Any] = None) -> None:
+        """
+        Draw a rectangle at the given location, size and color.
 
+        The optional *f* parameter can be set to ``True`` to fill the rectangle.
+        Otherwise just a one pixel outline is drawn.
+        """
+        ...
     def scroll(self, xstep, ystep) -> Any:
         """
         Shift the contents of the FrameBuffer by the given vector. This may
         leave a footprint of the previous colors in the FrameBuffer.
         """
         ...
-
-    def text(self, s, x, y, c: Optional[Any] = None) -> None:
+    def ellipse(self, x, y, xr, yr, c, f, m: Optional[Any] = None) -> None:
         """
-        Write text to the FrameBuffer using the the coordinates as the upper-left
-        corner of the text. The color of the text can be defined by the optional
-        argument but is otherwise a default value of 1. All characters have
-        dimensions of 8x8 pixels and there is currently no way to change the font.
-
+        Draw an ellipse at the given location. Radii *xr* and *yr* define the
+        geometry; equal values cause a circle to be drawn. The *c* parameter
+        defines the color.
+
+        The optional *f* parameter can be set to ``True`` to fill the ellipse.
+        Otherwise just a one pixel outline is drawn.
+
+        The optional *m* parameter enables drawing to be restricted to certain
+        quadrants of the ellipse. The LS four bits determine which quadrants are
+        to be drawn, with bit 0 specifying Q1, b1 Q2, b2 Q3 and b3 Q4. Quadrants
+        are numbered counterclockwise with Q1 being top right.
         """
         ...
-
-    def fill(self, c) -> None:
+    def line(self, x1, y1, x2, y2, c) -> None:
         """
-        Fill the entire FrameBuffer with the specified color.
+        Draw a line from a set of coordinates using the given color and
+        a thickness of 1 pixel. The `line` method draws the line up to
+        a second set of coordinates whereas the `hline` and `vline`
+        methods draw horizontal and vertical lines respectively up to
+        a given length.
         """
         ...
-
     def blit(self, fbuf, x, y, key=-1, palette=None) -> None:
         """
         Draw another FrameBuffer on top of the current one at the given coordinates.
         If *key* is specified then it should be a color integer and the
         corresponding color will be considered transparent: all pixels with that
-        color value will not be drawn.
+        color value will not be drawn. (If the *palette* is specified then the *key*
+        is compared to the value from *palette*, not to the value directly from
+        *fbuf*.)
 
         The *palette* argument enables blitting between FrameBuffers with differing
         formats. Typical usage is to render a monochrome or grayscale glyph/icon to
         a color display. The *palette* is a FrameBuffer instance whose format is
         that of the current FrameBuffer. The *palette* height is one pixel and its
         pixel width is the number of colors in the source FrameBuffer. The *palette*
         for an N-bit source needs 2**N pixels; the *palette* for a monochrome source
         would have 2 pixels representing background and foreground colors. The
         application assigns a color to each pixel in the *palette*. The color of the
         current pixel will be that of that *palette* pixel whose x position is the
         color of the corresponding source pixel.
         """
         ...
-
-    def line(self, x1, y1, x2, y2, c) -> None:
-        """
-        Draw a line from a set of coordinates using the given color and
-        a thickness of 1 pixel. The `line` method draws the line up to
-        a second set of coordinates whereas the `hline` and `vline`
-        methods draw horizontal and vertical lines respectively up to
-        a given length.
-        """
-        ...
-
-    def fill_rect(self, x, y, w, h, c) -> None:
+    def hline(self, x, y, w, c) -> Any: ...
+    def fill(self, c) -> None:
         """
-        Draw a rectangle at the given location, size and color. The `rect`
-        method draws only a 1 pixel outline whereas the `fill_rect` method
-        draws both the outline and interior.
+        Fill the entire FrameBuffer with the specified color.
         """
         ...
-
-    def hline(self, x, y, w, c) -> Any:
-        ...
-
-    def __init__(self, buffer, width, height, format, stride=-1, /) -> None:
-        ...
+    def fill_rect(self, *args, **kwargs) -> Any: ...
+    def __init__(self, buffer, width, height, format, stride=-1, /) -> None: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/hashlib.py` & `micropython_esp32_s3_stubs-1.20.0.post1/hashlib.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-hashing algorithms. See: https://docs.micropython.org/en/v1.19.1/library/hashlib.html
+hashing algorithms. See: https://docs.micropython.org/en/v1.20.0/library/hashlib.html
 
 |see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
 
 This module implements binary data hashing algorithms. The exact inventory
 of available algorithms depends on a board. Among the algorithms which may
 be implemented:
 
@@ -17,40 +17,26 @@
   applications, so boards targeting network connectivity and
   interoperability will try to provide this.
 
 * MD5 - A legacy algorithm, not considered cryptographically secure. Only
   selected boards, targeting interoperability with legacy applications,
   will offer this.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Any
 
-
 class sha256:
     """
     Create an SHA256 hasher object and optionally feed ``data`` into it.
     """
 
-    def digest(self, *args, **kwargs) -> Any:
-        ...
-
-    def update(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, data: Optional[Any] = None) -> None:
-        ...
-
+    def digest(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def __init__(self, data: Optional[Any] = None) -> None: ...
 
 class sha1:
     """
     Create an SHA1 hasher object and optionally feed ``data`` into it.
     """
 
-    def digest(self, *args, **kwargs) -> Any:
-        ...
-
-    def update(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, data: Optional[Any] = None) -> None:
-        ...
+    def digest(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def __init__(self, data: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/heapq.py` & `micropython_esp32_s3_stubs-1.20.0.post1/heapq.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 """
-heap queue algorithm. See: https://docs.micropython.org/en/v1.19.1/library/heapq.html
+heap queue algorithm. See: https://docs.micropython.org/en/v1.20.0/library/heapq.html
 
 |see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
 
 This module implements the
 `min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
 
 A heap queue is essentially a list that has its elements stored in such a way
 that the first item of the list is always the smallest.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Any
 
-
 def heappop(heap) -> Any:
     """
     Pop the first item from the ``heap``, and return it.  Raise ``IndexError`` if
     ``heap`` is empty.
 
     The returned item will be the smallest item in the ``heap``.
     """
     ...
 
-
 def heappush(heap, item) -> Any:
     """
     Push the ``item`` onto the ``heap``.
     """
     ...
 
-
 def heapify(x) -> Any:
     """
     Convert the list ``x`` into a heap.  This is an in-place operation.
     """
     ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/json.py` & `micropython_esp32_s3_stubs-1.20.0.post1/json.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 """
-JSON encoding and decoding. See: https://docs.micropython.org/en/v1.19.1/library/json.html
+JSON encoding and decoding. See: https://docs.micropython.org/en/v1.20.0/library/json.html
 
 |see_cpython_module| :mod:`python:json` https://docs.python.org/3/library/json.html .
 
 This modules allows to convert between Python objects and the JSON
 data format.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Any
 
-
 def loads(str) -> Any:
     """
     Parse the JSON *str* and return an object.  Raises :exc:`ValueError` if the
     string is not correctly formed.
     """
     ...
 
-
 def load(stream) -> Any:
     """
     Parse the given *stream*, interpreting it as a JSON string and
     deserialising the data to a Python object.  The resulting object is
     returned.
 
     Parsing continues until end-of-file is encountered.
     A :exc:`ValueError` is raised if the data in *stream* is not correctly formed.
     """
     ...
 
-
 def dumps(obj, separators=None) -> str:
     """
     Return *obj* represented as a JSON string.
 
     The arguments have the same meaning as in `dump`.
     """
     ...
 
-
 def dump(obj, stream, separators=None) -> Any:
     """
     Serialise *obj* to a JSON string, writing it to the given *stream*.
 
     If specified, separators should be an ``(item_separator, key_separator)``
     tuple. The default is ``(', ', ': ')``. To get the most compact JSON
     representation, you should specify ``(',', ':')`` to eliminate whitespace.
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/LICENSE.md` & `micropython_esp32_s3_stubs-1.20.0.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/machine.py` & `micropython_esp32_s3_stubs-1.20.0.post1/machine.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,50 @@
 """
-functions related to the hardware. See: https://docs.micropython.org/en/v1.19.1/library/machine.html
+functions related to the hardware. See: https://docs.micropython.org/en/v1.20.0/library/machine.html
 
 The ``machine`` module contains specific functions related to the hardware
 on a particular board. Most functions in this module allow to achieve direct
 and unrestricted access to and control of hardware blocks on a system
 (like CPU, timers, buses, etc.). Used incorrectly, this can lead to
 malfunction, lockups, crashes of your board, and in extreme cases, hardware
 damage.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Callable, List, NoReturn, Optional, Tuple, Union, Any
 
-TOUCHPAD_WAKE = 5  # type: int
-HARD_RESET = 2  # type: int
-SOFT_RESET = 5  # type: int
-PWRON_RESET = 1  # type: int
-PIN_WAKE = 2  # type: int
-TIMER_WAKE = 4  # type: int
-SLEEP = 2  # type: int
-WDT_RESET = 3  # type: int
-EXT1_WAKE = 3  # type: int
-ULP_WAKE = 6  # type: int
-EXT0_WAKE = 2  # type: int
-DEEPSLEEP = 4  # type: int
-DEEPSLEEP_RESET = 4  # type: int
+SLEEP: int
+HARD_RESET: int
+SOFT_RESET: int
+PWRON_RESET: int
+PIN_WAKE: int
+TOUCHPAD_WAKE: int
+TIMER_WAKE: int
+WDT_RESET: int
+EXT1_WAKE: int
+ULP_WAKE: int
+EXT0_WAKE: int
+DEEPSLEEP: int
+DEEPSLEEP_RESET: int
 
+def disable_irq() -> Any:
+    """
+    Disable interrupt requests.
+    Returns the previous IRQ state which should be considered an opaque value.
+    This return value should be passed to the `enable_irq()` function to restore
+    interrupts to their original state, before `disable_irq()` was called.
+    """
+    ...
 
 def enable_irq(state) -> Any:
     """
     Re-enable interrupt requests.
     The *state* parameter should be the value that was returned from the most
     recent call to the `disable_irq()` function.
     """
     ...
 
-
-def wake_reason() -> Any:
-    """
-    Get the wake reason. See :ref:`constants <machine_constants>` for the possible return values.
-
-    Availability: ESP32, WiPy.
-    """
-    ...
-
-
 def bitstream(pin, encoding, timing, data, /) -> Any:
     """
     Transmits *data* by bit-banging the specified *pin*. The *encoding* argument
     specifies how the bits are encoded, and *timing* is an encoding-specific timing
     specification.
 
     The supported encodings are:
@@ -65,25 +61,15 @@
     will be closer to +/-30ns.
 
     ``Note:`` For controlling WS2812 / NeoPixel strips, see the :mod:`neopixel`
        module for a higher-level API.
     """
     ...
 
-
-def disable_irq() -> Any:
-    """
-    Disable interrupt requests.
-    Returns the previous IRQ state which should be considered an opaque value.
-    This return value should be passed to the `enable_irq()` function to restore
-    interrupts to their original state, before `disable_irq()` was called.
-    """
-    ...
-
-
+def dht_readinto(*args, **kwargs) -> Any: ...
 def deepsleep(time_ms: Optional[Any] = None) -> NoReturn:
     """
     Stops execution in an attempt to enter a low power state.
 
     If *time_ms* is specified then this will be the maximum time in milliseconds that
     the sleep will last for.  Otherwise the sleep can last indefinitely.
 
@@ -101,31 +87,36 @@
       peripherals or network interfaces).  Upon wake execution is resumed from the main
       script, similar to a hard or power-on reset. The `reset_cause()` function will
       return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
       from other resets.
     """
     ...
 
+def wake_reason() -> Any:
+    """
+    Get the wake reason. See :ref:`constants <machine_constants>` for the possible return values.
+
+    Availability: ESP32, WiPy.
+    """
+    ...
 
 def sleep() -> Any:
     """
     ``Note:`` This function is deprecated, use `lightsleep()` instead with no arguments.
     """
     ...
 
-
 def soft_reset() -> NoReturn:
     """
     Performs a soft reset of the interpreter, deleting all Python objects and
     resetting the Python heap.  It tries to retain the method by which the user
     is connected to the MicroPython REPL (eg serial, USB, Wifi).
     """
     ...
 
-
 def time_pulse_us(pin, pulse_level, timeout_us=1000000, /) -> int:
     """
     Time a pulse on the given *pin*, and return the duration of the pulse in
     microseconds.  The *pulse_level* argument should be 0 to time a low pulse
     or 1 to time a high pulse.
 
     If the current input value of the pin is different to *pulse_level*,
@@ -136,51 +127,46 @@
     The function will return -2 if there was timeout waiting for condition marked
     (*) above, and -1 if there was timeout during the main measurement, marked (**)
     above. The timeout is the same for both cases and given by *timeout_us* (which
     is in microseconds).
     """
     ...
 
-
 def unique_id() -> bytes:
     """
     Returns a byte string with a unique identifier of a board/SoC. It will vary
     from a board/SoC instance to another, if underlying hardware allows. Length
     varies by hardware (so use substring of a full value if you expect a short
     ID). In some MicroPython ports, ID corresponds to the network MAC address.
     """
     ...
 
-
 def freq(hz: Optional[Any] = None) -> Any:
     """
     Returns the CPU frequency in hertz.
 
     On some ports this can also be used to set the CPU frequency by passing in *hz*.
     """
     ...
 
-
 def reset_cause() -> int:
     """
     Get the reset cause. See :ref:`constants <machine_constants>` for the possible return values.
     """
     ...
 
-
 def idle() -> Any:
     """
     Gates the clock to the CPU, useful to reduce power consumption at any time during
     short or long periods. Peripherals continue working and execution resumes as soon
     as any interrupt is triggered (on many ports this includes system timer
     interrupt occurring at regular intervals on the order of millisecond).
     """
     ...
 
-
 def lightsleep(time_ms: Optional[Any] = None) -> Any:
     """
     Stops execution in an attempt to enter a low power state.
 
     If *time_ms* is specified then this will be the maximum time in milliseconds that
     the sleep will last for.  Otherwise the sleep can last indefinitely.
 
@@ -198,23 +184,21 @@
       peripherals or network interfaces).  Upon wake execution is resumed from the main
       script, similar to a hard or power-on reset. The `reset_cause()` function will
       return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
       from other resets.
     """
     ...
 
-
 def reset() -> NoReturn:
     """
     Resets the device in a manner similar to pushing the external RESET
     button.
     """
     ...
 
-
 class PWM:
     """
     Construct and return a new PWM object using the following parameters:
 
        - *dest* is the entity on which the PWM is output, which is usually a
          :ref:`machine.Pin <machine.Pin>` object, but a port may allow other values,
          like integers.
@@ -235,55 +219,46 @@
 
         With no arguments the duty cycle is returned.
 
         With a single *value* argument the duty cycle is set to that value, measured
         as the ratio ``value / 65535``.
         """
         ...
-
     def init(self, *, freq, duty_u16, duty_ns) -> None:
         """
         Modify settings for the PWM object.  See the above constructor for details
         about the parameters.
         """
         ...
-
     def freq(self, value: Optional[Any] = None) -> Any:
         """
         Get or set the current frequency of the PWM output.
 
         With no arguments the frequency in Hz is returned.
 
         With a single *value* argument the frequency is set to that value in Hz.  The
         method may raise a ``ValueError`` if the frequency is outside the valid range.
         """
         ...
-
     def deinit(self) -> None:
         """
         Disable the PWM output.
         """
         ...
-
     def duty_ns(self, value: Optional[Any] = None) -> int:
         """
         Get or set the current pulse width of the PWM output, as a value in nanoseconds.
 
         With no arguments the pulse width in nanoseconds is returned.
 
         With a single *value* argument the pulse width is set to that value.
         """
         ...
-
-    def duty(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, dest, *, freq=0, duty=0, duty_u16=0, duty_ns=0) -> None:
-        ...
-
+    def duty(self, *args, **kwargs) -> Any: ...
+    def __init__(self, dest, *, freq=0, duty=0, duty_u16=0, duty_ns=0) -> None: ...
 
 class Pin:
     """
     Access the pin peripheral (GPIO pin) associated with the given ``id``.  If
     additional arguments are given in the constructor then they are used to initialise
     the pin.  Any settings that are not specified will remain in their previous state.
 
@@ -341,28 +316,27 @@
     alternate-function mode are usually not used as GPIO but are instead driven by other
     hardware peripherals.  The only operation supported on such a pin is re-initialising,
     by calling the constructor or :meth:`Pin.init` method.  If a pin that is configured in
     alternate-function mode is re-initialised with ``Pin.IN``, ``Pin.OUT``, or
     ``Pin.OPEN_DRAIN``, the alternate function will be removed from the pin.
     """
 
-    OPEN_DRAIN = 7  # type: int
-    IRQ_FALLING = 2  # type: int
-    IRQ_RISING = 1  # type: int
-    PULL_UP = 2  # type: int
-    OUT = 3  # type: int
-    PULL_DOWN = 1  # type: int
-    WAKE_HIGH = 5  # type: int
-    DRIVE_0 = 0  # type: int
-    IN = 1  # type: int
-    WAKE_LOW = 4  # type: int
-    DRIVE_3 = 3  # type: int
-    DRIVE_1 = 1  # type: int
-    DRIVE_2 = 2  # type: int
-
+    OPEN_DRAIN: int
+    IRQ_FALLING: int
+    IRQ_RISING: int
+    PULL_UP: int
+    OUT: int
+    PULL_DOWN: int
+    WAKE_HIGH: int
+    DRIVE_0: int
+    IN: int
+    WAKE_LOW: int
+    DRIVE_3: int
+    DRIVE_1: int
+    DRIVE_2: int
     def irq(self, handler=None, trigger=IRQ_FALLING, *, priority=1, wake=None, hard=False) -> Callable[..., Any]:
         """
            Configure an interrupt handler to be called when the trigger source of the
            pin is active.  If the pin mode is ``Pin.IN`` then the trigger source is
            the external value on the pin.  If the pin mode is ``Pin.OUT`` then the
            trigger source is the output buffer of the pin.  Otherwise, if the pin mode
            is ``Pin.OPEN_DRAIN`` then the trigger source is the output buffer for
@@ -399,37 +373,33 @@
                Not all ports support this argument.
 
            This method returns a callback object.
 
         The following methods are not part of the core Pin API and only implemented on certain ports.
         """
         ...
-
     def off(self) -> None:
         """
         Set pin to "0" output level.
         """
         ...
-
     def on(self) -> None:
         """
         Set pin to "1" output level.
         """
         ...
-
     def init(self, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
         """
         Re-initialise the pin using the given parameters.  Only those arguments that
         are specified will be set.  The rest of the pin peripheral state will remain
         unchanged.  See the constructor documentation for details of the arguments.
 
         Returns ``None``.
         """
         ...
-
     def value(self, x: Optional[Any] = None) -> int:
         """
         This method allows to set and get the value of the pin, depending on whether
         the argument ``x`` is supplied or not.
 
         If the argument is omitted then this method gets the digital logic level of
         the pin, returning 0 or 1 corresponding to low and high voltage signals
@@ -455,43 +425,26 @@
           - ``Pin.OUT`` - The output buffer is set to the given value immediately.
           - ``Pin.OPEN_DRAIN`` - If the value is '0' the pin is set to a low voltage
             state.  Otherwise the pin is set to high-impedance state.
 
         When setting the value this method returns ``None``.
         """
         ...
-
-    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
-        ...
-
-
-mem8: Any  ## <class 'mem'> = <8-bit memory>
-mem32: Any  ## <class 'mem'> = <32-bit memory>
-
-
-class WDT:
-    """
-    Create a WDT object and start it. The timeout must be given in milliseconds.
-    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
-
-    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
-    cannot be specified, it is determined by the underlying system.
-    """
-
-    def feed(self) -> None:
+    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None: ...
+    def __call__(self, x: Optional[Any] = None) -> Any:
         """
-        Feed the WDT to prevent it from resetting the system. The application
-        should place this call in a sensible place ensuring that the WDT is
-        only fed after verifying that everything is functioning correctly.
+        Pin objects are callable.  The call method provides a (fast) shortcut to set
+        and get the value of the pin.  It is equivalent to Pin.value([x]).
+        See :meth:`Pin.value` for more details.
         """
         ...
 
-    def __init__(self, id=0, timeout=5000) -> None:
-        ...
-
+mem8: Any
+mem32: Any
+mem16: Any
 
 class I2S:
     """
     Construct an I2S object of the given id:
 
     - ``id`` identifies a particular I2S bus; it is board and port specific
 
@@ -511,69 +464,60 @@
 
     For all ports, DMA runs continuously in the background and allows user applications to perform other operations while
     sample data is transfered between the internal buffer and the I2S peripheral unit.
     Increasing the size of the internal buffer has the potential to increase the time that user applications can perform non-I2S operations
     before underflow (e.g. ``write`` method) or overflow (e.g. ``readinto`` method).
     """
 
-    RX = 9  # type: int
-    MONO = 0  # type: int
-    STEREO = 1  # type: int
-    TX = 5  # type: int
-
+    RX: int
+    MONO: int
+    STEREO: int
+    TX: int
     @staticmethod
     def shift(*, buf, bits, shift) -> Any:
         """
         bitwise shift of all samples contained in ``buf``. ``bits`` specifies sample size in bits. ``shift`` specifies the number of bits to shift each sample.
         Positive for left shift, negative for right shift.
         Typically used for volume control.  Each bit shift changes sample volume by 6dB.
         """
         ...
-
     def init(self, sck, *args, **kwargs) -> Any:
         """
         see Constructor for argument descriptions
         """
         ...
-
     def irq(self, handler) -> Any:
         """
         Set a callback. ``handler`` is called when ``buf`` is emptied (``write`` method) or becomes full (``readinto`` method).
         Setting a callback changes the ``write`` and ``readinto`` methods to non-blocking operation.
         ``handler`` is called in the context of the MicroPython scheduler.
         """
         ...
-
     def readinto(self, buf) -> int:
         """
         Read audio samples into the buffer specified by ``buf``.  ``buf`` must support the buffer protocol, such as bytearray or array.
         "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
         the left channel sample data is used.
         Returns number of bytes read
         """
         ...
-
     def deinit(self) -> Any:
         """
         Deinitialize the I2S bus
         """
         ...
-
     def write(self, buf) -> int:
         """
         Write audio samples contained in ``buf``. ``buf`` must support the buffer protocol, such as bytearray or array.
         "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
         the sample data is written to both the right and left channels.
         Returns number of bytes written
         """
         ...
-
-    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None:
-        ...
-
+    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None: ...
 
 class ADC:
     """
     Access the ADC associated with a source identified by *id*.  This
     *id* may be an integer (usually specifying a channel number), a
     :ref:`Pin <machine.Pin>` object, or other value supported by the
     underlying machine.
@@ -583,66 +527,53 @@
     previous or default values.  The settings are:
 
       - *sample_ns* is the sampling time in nanoseconds.
 
       - *atten* specifies the input attenuation.
     """
 
-    ATTN_2_5DB = 1  # type: int
-    WIDTH_12BIT = 12  # type: int
-    ATTN_6DB = 2  # type: int
-    ATTN_11DB = 3  # type: int
-    ATTN_0DB = 0  # type: int
-
+    ATTN_2_5DB: int
+    WIDTH_12BIT: int
+    ATTN_6DB: int
+    ATTN_11DB: int
+    ATTN_0DB: int
     def read_u16(self) -> int:
         """
         Take an analog reading and return an integer in the range 0-65535.
         The return value represents the raw reading taken by the ADC, scaled
         such that the minimum value is 0 and the maximum value is 65535.
         """
         ...
-
     def init(self, *, sample_ns, atten) -> Any:
         """
         Apply the given settings to the ADC.  Only those arguments that are
         specified will be changed.  See the ADC constructor above for what the
         arguments are.
         """
         ...
-
     def read_uv(self) -> int:
         """
         Take an analog reading and return an integer value with units of
         microvolts.  It is up to the particular port whether or not this value
         is calibrated, and how calibration is done.
         """
         ...
-
-    def width(self, *args, **kwargs) -> Any:
-        ...
-
-    def read(self, *args, **kwargs) -> Any:
-        ...
-
+    def width(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
     def block(self) -> Any:
         """
         Return the :ref:`ADCBlock <machine.ADCBlock>` instance associated with
         this ADC object.
 
         This method only exists if the port supports the
         :ref:`ADCBlock <machine.ADCBlock>` class.
         """
         ...
-
-    def atten(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None:
-        ...
-
+    def atten(self, *args, **kwargs) -> Any: ...
+    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None: ...
 
 class ADCBlock:
     """
     Access the ADC peripheral identified by *id*, which may be an integer
     or string.
 
     The *bits* argument, if given, sets the resolution in bits of the
@@ -652,15 +583,14 @@
 
     def init(self, *, bits) -> None:
         """
         Configure the ADC peripheral.  *bits* will set the resolution of the
         conversion process.
         """
         ...
-
     def connect(self, channel, source) -> Any:
         """
         Connect up a channel on the ADC peripheral so it is ready for sampling,
         and return an :ref:`ADC <machine.ADC>` object that represents that connection.
 
         The *channel* argument must be an integer, and *source* must be an object
         (for example a :ref:`Pin <machine.Pin>`) which can be connected up for sampling.
@@ -670,29 +600,28 @@
         If only *source* is given then that object is connected to a default
         channel ready for sampling.
 
         If both *channel* and *source* are given then they are connected together
         and made ready for sampling.
         """
         ...
-
-    def __init__(self, id, *, bits) -> None:
-        ...
-
+    def __init__(self, id, *, bits) -> None: ...
 
 class I2C:
     """
     Construct and return a new I2C object using the following parameters:
 
        - *id* identifies a particular I2C peripheral.  Allowed values for
          depend on the particular port/board
        - *scl* should be a pin object specifying the pin to use for SCL.
        - *sda* should be a pin object specifying the pin to use for SDA.
        - *freq* should be an integer which sets the maximum frequency
          for SCL.
+       - *timeout* is the maximum time in microseconds to allow for I2C
+         transactions.  This parameter is not allowed on some ports.
 
     Note that some ports/boards will have default values of *scl* and *sda*
     that can be changed in this constructor.  Others will have fixed values
     of *scl* and *sda* that cannot be changed.
     """
 
     def readfrom_mem_into(self, addr, memaddr, buf, *, addrsize=8) -> None:
@@ -702,63 +631,57 @@
         length of *buf*.
         The argument *addrsize* specifies the address size in bits (on ESP8266
         this argument is not recognised and the address size is always 8 bits).
 
         The method returns ``None``.
         """
         ...
-
     def readfrom_into(self, addr, buf, stop=True, /) -> None:
         """
         Read into *buf* from the peripheral specified by *addr*.
         The number of bytes read will be the length of *buf*.
         If *stop* is true then a STOP condition is generated at the end of the transfer.
 
         The method returns ``None``.
         """
         ...
-
     def readfrom_mem(self, addr, memaddr, nbytes, *, addrsize=8) -> bytes:
         """
         Read *nbytes* from the peripheral specified by *addr* starting from the memory
         address specified by *memaddr*.
         The argument *addrsize* specifies the address size in bits.
         Returns a `bytes` object with the data read.
         """
         ...
-
     def writeto_mem(self, addr, memaddr, buf, *, addrsize=8) -> None:
         """
         Write *buf* to the peripheral specified by *addr* starting from the
         memory address specified by *memaddr*.
         The argument *addrsize* specifies the address size in bits (on ESP8266
         this argument is not recognised and the address size is always 8 bits).
 
         The method returns ``None``.
         """
         ...
-
     def scan(self) -> List:
         """
         Scan all I2C addresses between 0x08 and 0x77 inclusive and return a list of
         those that respond.  A device responds if it pulls the SDA line low after
         its address (including a write bit) is sent on the bus.
         """
         ...
-
     def writeto(self, addr, buf, stop=True, /) -> int:
         """
         Write the bytes from *buf* to the peripheral specified by *addr*.  If a
         NACK is received following the write of a byte from *buf* then the
         remaining bytes are not sent.  If *stop* is true then a STOP condition is
         generated at the end of the transfer, even if a NACK is received.
         The function returns the number of ACKs that were received.
         """
         ...
-
     def writevto(self, addr, vector, stop=True, /) -> int:
         """
         Write the bytes contained in *vector* to the peripheral specified by *addr*.
         *vector* should be a tuple or list of objects with the buffer protocol.
         The *addr* is sent once and then the bytes from each object in *vector*
         are written out sequentially.  The objects in *vector* may be zero bytes
         in length in which case they don't contribute to the output.
@@ -766,182 +689,132 @@
         If a NACK is received following the write of a byte from one of the
         objects in *vector* then the remaining bytes, and any remaining objects,
         are not sent.  If *stop* is true then a STOP condition is generated at
         the end of the transfer, even if a NACK is received.  The function
         returns the number of ACKs that were received.
         """
         ...
-
     def start(self) -> None:
         """
         Generate a START condition on the bus (SDA transitions to low while SCL is high).
         """
         ...
-
     def readfrom(self, addr, nbytes, stop=True, /) -> bytes:
         """
         Read *nbytes* from the peripheral specified by *addr*.
         If *stop* is true then a STOP condition is generated at the end of the transfer.
         Returns a `bytes` object with the data read.
         """
         ...
-
     def readinto(self, buf, nack=True, /) -> Any:
         """
         Reads bytes from the bus and stores them into *buf*.  The number of bytes
         read is the length of *buf*.  An ACK will be sent on the bus after
         receiving all but the last byte.  After the last byte is received, if *nack*
         is true then a NACK will be sent, otherwise an ACK will be sent (and in this
         case the peripheral assumes more bytes are going to be read in a later call).
         """
         ...
-
     def init(self, scl, sda, *, freq=400000) -> None:
         """
         Initialise the I2C bus with the given arguments:
 
            - *scl* is a pin object for the SCL line
            - *sda* is a pin object for the SDA line
            - *freq* is the SCL clock rate
+
+         In the case of hardware I2C the actual clock frequency may be lower than the
+         requested frequency. This is dependant on the platform hardware. The actual
+         rate may be determined by printing the I2C object.
         """
         ...
-
     def stop(self) -> None:
         """
         Generate a STOP condition on the bus (SDA transitions to high while SCL is high).
         """
         ...
-
     def write(self, buf) -> int:
         """
         Write the bytes from *buf* to the bus.  Checks that an ACK is received
         after each byte and stops transmitting the remaining bytes if a NACK is
         received.  The function returns the number of ACKs that were received.
         """
         ...
-
     def __init__(
-        self, id: Union[int, str] = -1, *, scl: Optional[Union[Pin, str]] = None, sda: Optional[Union[Pin, str]] = None, freq=400_000
-    ) -> None:
-        ...
-
+        self,
+        id: Union[int, str] = -1,
+        *,
+        scl: Optional[Union[Pin, str]] = None,
+        sda: Optional[Union[Pin, str]] = None,
+        freq=400_000,
+        timeout=50000,
+    ) -> None: ...
 
-class SoftI2C:
+class WDT:
     """
-    Construct a new software I2C object.  The parameters are:
+    Create a WDT object and start it. The timeout must be given in milliseconds.
+    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
 
-       - *scl* should be a pin object specifying the pin to use for SCL.
-       - *sda* should be a pin object specifying the pin to use for SDA.
-       - *freq* should be an integer which sets the maximum frequency
-         for SCL.
-       - *timeout* is the maximum time in microseconds to wait for clock
-         stretching (SCL held low by another device on the bus), after
-         which an ``OSError(ETIMEDOUT)`` exception is raised.
+    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
+    cannot be specified, it is determined by the underlying system. On rp2040 devices,
+    the maximum timeout is 8388 ms.
     """
 
-    def readfrom_mem_into(self, *args, **kwargs) -> Any:
-        ...
-
-    def readfrom_into(self, *args, **kwargs) -> Any:
-        ...
-
-    def readfrom_mem(self, *args, **kwargs) -> Any:
-        ...
-
-    def writeto_mem(self, *args, **kwargs) -> Any:
-        ...
-
-    def scan(self, *args, **kwargs) -> Any:
-        ...
-
-    def writeto(self, *args, **kwargs) -> Any:
-        ...
-
-    def writevto(self, *args, **kwargs) -> Any:
-        ...
-
-    def start(self, *args, **kwargs) -> Any:
-        ...
-
-    def readfrom(self, *args, **kwargs) -> Any:
-        ...
-
-    def readinto(self, *args, **kwargs) -> Any:
-        ...
-
-    def init(self, *args, **kwargs) -> Any:
-        ...
-
-    def stop(self, *args, **kwargs) -> Any:
-        ...
-
-    def write(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None:
+    def feed(self) -> None:
+        """
+        Feed the WDT to prevent it from resetting the system. The application
+        should place this call in a sensible place ensuring that the WDT is
+        only fed after verifying that everything is functioning correctly.
+        """
         ...
-
+    def __init__(self, id=0, timeout=5000) -> None: ...
 
 class SoftSPI:
     """
     Construct a new software SPI object.  Additional parameters must be
     given, usually at least *sck*, *mosi* and *miso*, and these are used
     to initialise the bus.  See `SPI.init` for a description of the parameters.
     """
 
-    LSB = 1  # type: int
-    MSB = 0  # type: int
-
-    def deinit(self, *args, **kwargs) -> Any:
-        ...
-
-    def init(self, *args, **kwargs) -> Any:
-        ...
-
-    def write_readinto(self, *args, **kwargs) -> Any:
-        ...
-
-    def read(self, *args, **kwargs) -> Any:
-        ...
-
-    def write(self, *args, **kwargs) -> Any:
-        ...
-
-    def readinto(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None:
-        ...
-
+    LSB: int
+    MSB: int
+    def deinit(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def write_readinto(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None: ...
 
 class Timer:
     """
     Construct a new timer object of the given ``id``. ``id`` of -1 constructs a
     virtual timer (if supported by a board).
     ``id`` shall not be passed as a keyword argument.
 
     See ``init`` for parameters of initialisation.
     """
 
-    ONE_SHOT = 0  # type: int
-    PERIODIC = 1  # type: int
-
+    ONE_SHOT: int
+    PERIODIC: int
     def deinit(self) -> None:
         """
         Deinitialises the timer. Stops the timer, and disables the timer peripheral.
         """
         ...
-
-    def init(self, *, mode=PERIODIC, period=-1, callback=None) -> None:
+    def init(self, *, mode=PERIODIC, freq=-1, period=-1, callback=None) -> None:
         """
         Initialise the timer. Example::
 
             def mycallback(t):
                 pass
 
+            # periodic at 1kHz
+            tim.init(mode=Timer.PERIODIC, freq=1000, callback=mycallback)
+
             # periodic with 100ms period
             tim.init(period=100, callback=mycallback)
 
             # one shot firing after 1000ms
             tim.init(mode=Timer.ONE_SHOT, period=1000, callback=mycallback)
 
         Keyword arguments:
@@ -949,49 +822,62 @@
           - ``mode`` can be one of:
 
             - ``Timer.ONE_SHOT`` - The timer runs once until the configured
               period of the channel expires.
             - ``Timer.PERIODIC`` - The timer runs periodically at the configured
               frequency of the channel.
 
+          - ``freq`` - The timer frequency, in units of Hz.  The upper bound of
+            the frequency is dependent on the port.  When both the ``freq`` and
+            ``period`` arguments are given, ``freq`` has a higher priority and
+            ``period`` is ignored.
+
           - ``period`` - The timer period, in milliseconds.
 
           - ``callback`` - The callable to call upon expiration of the timer period.
             The callback must take one argument, which is passed the Timer object.
             The ``callback`` argument shall be specified. Otherwise an exception
             will occurr upon timer expiration:
             ``TypeError: 'NoneType' object isn't callable``
         """
         ...
+    def value(self, *args, **kwargs) -> Any: ...
+    def __init__(self, id=-1, *args, **kwargs) -> None: ...
 
-    def value(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, id=-1, *args, **kwargs) -> None:
-        ...
-
+class TouchPad:
+    def config(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def __init__(self, *argv, **kwargs) -> None: ...
 
 class UART:
     """
     Construct a UART object of the given id.
     """
 
-    INV_RTS = 64  # type: int
-    INV_RX = 4  # type: int
-    CTS = 2  # type: int
-    INV_CTS = 8  # type: int
-    INV_TX = 32  # type: int
-    RTS = 1  # type: int
-
+    INV_CTS: int
+    CTS: int
+    INV_TX: int
+    INV_RTS: int
+    INV_RX: int
+    RTS: int
     def deinit(self) -> None:
         """
         Turn off the UART bus.
+
+        .. note::
+          You will not be able to call ``init()`` on the object after ``deinit()``.
+          A new instance needs to be created in that case.
+        """
+        ...
+    def sendbreak(self) -> None:
+        """
+        Send a break condition on the bus. This drives the bus low for a duration
+        longer than required for a normal transmission of a character.
         """
         ...
-
     def init(self, baudrate=9600, bits=8, parity=None, stop=1, *args, **kwargs) -> None:
         """
         Initialise the UART bus with the given parameters:
 
           - *baudrate* is the clock rate.
           - *bits* is the number of bits per character, 7, 8 or 9.
           - *parity* is the parity, ``None``, 0 (even) or 1 (odd).
@@ -1027,158 +913,116 @@
         On the WiPy only the following keyword-only parameter is supported:
 
           - *pins* is a 4 or 2 item list indicating the TX, RX, RTS and CTS pins (in that order).
             Any of the pins can be None if one wants the UART to operate with limited functionality.
             If the RTS pin is given the the RX pin must be given as well. The same applies to CTS.
             When no pins are given, then the default set of TX and RX pins is taken, and hardware
             flow control will be disabled. If *pins* is ``None``, no pin assignment will be made.
+
+        .. note::
+          It is possible to call ``init()`` multiple times on the same object in
+          order to reconfigure  UART on the fly. That allows using single UART
+          peripheral to serve different devices attached to different GPIO pins.
+          Only one device can be served at a time in that case.
+          Also do not call ``deinit()`` as it will prevent calling ``init()``
+          again.
         """
         ...
-
-    def sendbreak(self) -> None:
+    def flush(self) -> Any:
         """
-        Send a break condition on the bus. This drives the bus low for a duration
-        longer than required for a normal transmission of a character.
+        Waits until all data has been sent. In case of a timeout, an exception is raised. The timeout
+        duration depends on the tx buffer size and the baud rate. Unless flow control is enabled, a timeout
+        should not occur.
+
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call returns while the last byte is sent.
+            If required, a one character wait time has to be added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
         """
         ...
+    def txdone(self) -> bool:
+        """
+        Tells whether all data has been sent or no data transfer is happening. In this case,
+        it returns ``True``. If a data transmission is ongoing it returns ``False``.
 
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call may return ``True`` even if the last byte
+            of a transfer is still being sent. If required, a one character wait time has to be
+            added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
+        """
+        ...
     def read(self, nbytes: Optional[Any] = None) -> bytes:
         """
         Read characters.  If ``nbytes`` is specified then read at most that many bytes,
         otherwise read as much data as possible. It may return sooner if a timeout
         is reached. The timeout is configurable in the constructor.
 
         Return value: a bytes object containing the bytes read in.  Returns ``None``
         on timeout.
         """
         ...
-
     def any(self) -> int:
         """
         Returns an integer counting the number of characters that can be read without
         blocking.  It will return 0 if there are no characters available and a positive
         number if there are characters.  The method may return 1 even if there is more
         than one character available for reading.
 
         For more sophisticated querying of available characters use select.poll::
 
          poll = select.poll()
          poll.register(uart, select.POLLIN)
          poll.poll(timeout)
         """
         ...
-
     def write(self, buf) -> int:
         """
         Write the buffer of bytes to the bus.
 
         Return value: number of bytes written or ``None`` on timeout.
         """
         ...
-
     def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
         """
         Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
         that many bytes.  Otherwise, read at most ``len(buf)`` bytes. It may return sooner if a timeout
         is reached. The timeout is configurable in the constructor.
 
         Return value: number of bytes read and stored into ``buf`` or ``None`` on
         timeout.
         """
         ...
-
     def readline(self) -> None:
         """
         Read a line, ending in a newline character. It may return sooner if a timeout
         is reached. The timeout is configurable in the constructor.
 
         Return value: the line read or ``None`` on timeout.
         """
         ...
-
-    def __init__(self, id, *args, **kwargs) -> None:
-        ...
-
-
-mem16: Any  ## <class 'mem'> = <16-bit memory>
-
-
-class Signal:
-    """
-            Signal(pin_arguments..., *, invert=False)
-
-    Create a Signal object. There're two ways to create it:
-
-    * By wrapping existing Pin object - universal method which works for
-      any board.
-    * By passing required Pin parameters directly to Signal constructor,
-      skipping the need to create intermediate Pin object. Available on
-      many, but not all boards.
-
-    The arguments are:
-
-      - ``pin_obj`` is existing Pin object.
-
-      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
-
-      - ``invert`` - if True, the signal will be inverted (active low).
-    """
-
-    def off(self) -> None:
-        """
-        Deactivate signal.
-        """
-        ...
-
-    def on(self) -> None:
-        """
-        Activate signal.
-        """
-        ...
-
-    def value(self, x: Optional[Any] = None) -> int:
-        """
-        This method allows to set and get the value of the signal, depending on whether
-        the argument ``x`` is supplied or not.
-
-        If the argument is omitted then this method gets the signal level, 1 meaning
-        signal is asserted (active) and 0 - signal inactive.
-
-        If the argument is supplied then this method sets the signal level. The
-        argument ``x`` can be anything that converts to a boolean. If it converts
-        to ``True``, the signal is active, otherwise it is inactive.
-
-        Correspondence between signal being active and actual logic level on the
-        underlying pin depends on whether signal is inverted (active-low) or not.
-        For non-inverted signal, active status corresponds to logical 1, inactive -
-        to logical 0. For inverted/active-low signal, active status corresponds
-        to logical 0, while inactive - to logical 1.
-        """
-        ...
-
-    def __init__(self, pin_obj, *args, invert=False) -> None:
-        ...
-
+    def __init__(self, id, *args, **kwargs) -> None: ...
 
 class RTC:
     """
     Create an RTC object. See init for parameters of initialization.
     """
 
     def init(self, datetime) -> None:
         """
         Initialise the RTC. Datetime is a tuple of the form:
 
            ``(year, month, day[, hour[, minute[, second[, microsecond[, tzinfo]]]]])``
         """
         ...
-
-    def memory(self, *args, **kwargs) -> Any:
-        ...
-
+    def memory(self, *args, **kwargs) -> Any: ...
     def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
         """
         Get or set the date and time of the RTC.
 
         With no arguments, this method returns an 8-tuple with the current
         date and time.  With 1 argument (being an 8-tuple) it sets the date
         and time.
@@ -1186,18 +1030,43 @@
         The 8-tuple has the following format:
 
             (year, month, day, weekday, hours, minutes, seconds, subseconds)
 
         The meaning of the ``subseconds`` field is hardware dependent.
         """
         ...
+    def __init__(self, id=0, *args, **kwargs) -> None: ...
 
-    def __init__(self, id=0, *args, **kwargs) -> None:
-        ...
+class SoftI2C(I2C):
+    """
+    Construct a new software I2C object.  The parameters are:
+
+       - *scl* should be a pin object specifying the pin to use for SCL.
+       - *sda* should be a pin object specifying the pin to use for SDA.
+       - *freq* should be an integer which sets the maximum frequency
+         for SCL.
+       - *timeout* is the maximum time in microseconds to wait for clock
+         stretching (SCL held low by another device on the bus), after
+         which an ``OSError(ETIMEDOUT)`` exception is raised.
+    """
 
+    def readfrom_mem_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_mem(self, *args, **kwargs) -> Any: ...
+    def writeto_mem(self, *args, **kwargs) -> Any: ...
+    def scan(self, *args, **kwargs) -> Any: ...
+    def writeto(self, *args, **kwargs) -> Any: ...
+    def writevto(self, *args, **kwargs) -> Any: ...
+    def start(self, *args, **kwargs) -> Any: ...
+    def readfrom(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def stop(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None: ...
 
 class SDCard:
     """
     This class provides access to SD or MMC storage cards using either
     a dedicated SD/MMC interface hardware or through an SPI channel.
     The class implements the block protocol defined by :class:`os.AbstractBlockDev`.
     This allows the mounting of an SD card to be as simple as::
@@ -1222,54 +1091,40 @@
      - *mosi* can be used to specify an SPI mosi pin.
 
      - *cs* can be used to specify an SPI chip select pin.
 
      - *freq* selects the SD/MMC interface frequency in Hz (only supported on the ESP32).
     """
 
-    def ioctl(self, *args, **kwargs) -> Any:
-        ...
-
-    def readblocks(self, *args, **kwargs) -> Any:
-        ...
-
-    def writeblocks(self, *args, **kwargs) -> Any:
-        ...
-
-    def info(self, *args, **kwargs) -> Any:
-        ...
-
-    def deinit(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, slot=1, width=1, cd=None, wp=None, sck=None, miso=None, mosi=None, cs=None, freq=20000000) -> None:
-        ...
-
+    def ioctl(self, *args, **kwargs) -> Any: ...
+    def readblocks(self, *args, **kwargs) -> Any: ...
+    def writeblocks(self, *args, **kwargs) -> Any: ...
+    def info(self, *args, **kwargs) -> Any: ...
+    def deinit(self, *args, **kwargs) -> Any: ...
+    def __init__(self, slot=1, width=1, cd=None, wp=None, sck=None, miso=None, mosi=None, cs=None, freq=20000000) -> None: ...
 
 class SPI:
     """
     Construct an SPI object on the given bus, *id*. Values of *id* depend
     on a particular port and its hardware. Values 0, 1, etc. are commonly used
     to select hardware SPI block #0, #1, etc.
 
     With no additional parameters, the SPI object is created but not
     initialised (it has the settings from the last initialisation of
     the bus, if any).  If extra arguments are given, the bus is initialised.
     See ``init`` for parameters of initialisation.
     """
 
-    LSB = 1  # type: int
-    MSB = 0  # type: int
-
+    LSB: int
+    MSB: int
     def deinit(self) -> None:
         """
         Turn off the SPI bus.
         """
         ...
-
     def init(
         self, baudrate=1000000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None, pins: Optional[Tuple]
     ) -> None:
         """
         Initialise the SPI bus with the given parameters:
 
           - ``baudrate`` is the SCK clock rate.
@@ -1287,48 +1142,94 @@
             specify them as a tuple of ``pins`` parameter.
 
         In the case of hardware SPI the actual clock frequency may be lower than the
         requested baudrate. This is dependant on the platform hardware. The actual
         rate may be determined by printing the SPI object.
         """
         ...
-
     def write_readinto(self, write_buf, read_buf) -> int:
         """
         Write the bytes from ``write_buf`` while reading into ``read_buf``.  The
         buffers can be the same or different, but both buffers must have the
         same length.
         Returns ``None``.
 
         Note: on WiPy this function returns the number of bytes written.
         """
         ...
-
     def read(self, nbytes, write=0x00) -> bytes:
         """
         Read a number of bytes specified by ``nbytes`` while continuously writing
         the single byte given by ``write``.
         Returns a ``bytes`` object with the data that was read.
         """
         ...
-
     def write(self, buf) -> int:
         """
         Write the bytes contained in ``buf``.
         Returns ``None``.
 
         Note: on WiPy this function returns the number of bytes written.
         """
         ...
-
     def readinto(self, buf, write=0x00) -> int:
         """
         Read into the buffer specified by ``buf`` while continuously writing the
         single byte given by ``write``.
         Returns ``None``.
 
         Note: on WiPy this function returns the number of bytes read.
         """
         ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
 
-    def __init__(self, id, *args, **kwargs) -> None:
+class Signal(Pin):
+    """
+            Signal(pin_arguments..., *, invert=False)
+
+    Create a Signal object. There're two ways to create it:
+
+    * By wrapping existing Pin object - universal method which works for
+      any board.
+    * By passing required Pin parameters directly to Signal constructor,
+      skipping the need to create intermediate Pin object. Available on
+      many, but not all boards.
+
+    The arguments are:
+
+      - ``pin_obj`` is existing Pin object.
+
+      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
+
+      - ``invert`` - if True, the signal will be inverted (active low).
+    """
+
+    def off(self) -> None:
+        """
+        Deactivate signal.
+        """
+        ...
+    def on(self) -> None:
+        """
+        Activate signal.
+        """
+        ...
+    def value(self, x: Optional[Any] = None) -> int:
+        """
+        This method allows to set and get the value of the signal, depending on whether
+        the argument ``x`` is supplied or not.
+
+        If the argument is omitted then this method gets the signal level, 1 meaning
+        signal is asserted (active) and 0 - signal inactive.
+
+        If the argument is supplied then this method sets the signal level. The
+        argument ``x`` can be anything that converts to a boolean. If it converts
+        to ``True``, the signal is active, otherwise it is inactive.
+
+        Correspondence between signal being active and actual logic level on the
+        underlying pin depends on whether signal is inverted (active-low) or not.
+        For non-inverted signal, active status corresponds to logical 1, inactive -
+        to logical 0. For inverted/active-low signal, active status corresponds
+        to logical 0, while inactive - to logical 1.
+        """
         ...
+    def __init__(self, pin_obj, *args, invert=False) -> None: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/math.py` & `micropython_esp32_s3_stubs-1.20.0.post1/math.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,300 +1,254 @@
 """
-mathematical functions. See: https://docs.micropython.org/en/v1.19.1/library/math.html
+mathematical functions. See: https://docs.micropython.org/en/v1.20.0/library/math.html
 
 |see_cpython_module| :mod:`python:math` https://docs.python.org/3/library/math.html .
 
 The ``math`` module provides some basic mathematical functions for
 working with floating-point numbers.
 
 *Note:* On the pyboard, floating-point numbers have 32-bit precision.
 
 Availability: not available on WiPy. Floating point support required
 for this module.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Tuple, Any
 
-inf = inf  # type: float
-nan = nan  # type: float
-pi = 3.141593  # type: float
-e = 2.718282  # type: float
-tau = 6.283185  # type: float
-
+inf: float
+nan: float
+pi: float
+e: float
+tau: float
 
 def ldexp(x, exp) -> Any:
     """
     Return ``x * (2**exp)``.
     """
     ...
 
-
 def lgamma(x) -> float:
     """
     Return the natural logarithm of the gamma function of ``x``.
     """
     ...
 
-
 def trunc(x) -> int:
     """
     Return an integer, being ``x`` rounded towards 0.
     """
     ...
 
-
-def isclose(*args, **kwargs) -> Any:
-    ...
-
-
+def isclose(*args, **kwargs) -> Any: ...
 def gamma(x) -> Any:
     """
     Return the gamma function of ``x``.
     """
     ...
 
-
 def isnan(x) -> bool:
     """
     Return ``True`` if ``x`` is not-a-number
     """
     ...
 
-
 def isfinite(x) -> bool:
     """
     Return ``True`` if ``x`` is finite.
     """
     ...
 
-
 def isinf(x) -> bool:
     """
     Return ``True`` if ``x`` is infinite.
     """
     ...
 
-
 def sqrt(x) -> Any:
     """
     Return the square root of ``x``.
     """
     ...
 
-
 def sinh(x) -> float:
     """
     Return the hyperbolic sine of ``x``.
     """
     ...
 
-
 def log(x) -> float:
     """
     Return the natural logarithm of ``x``.
     """
     ...
 
-
 def tan(x) -> float:
     """
     Return the tangent of ``x``.
     """
     ...
 
-
 def tanh(x) -> float:
     """
     Return the hyperbolic tangent of ``x``.
     """
     ...
 
-
 def log2(x) -> float:
     """
     Return the base-2 logarithm of ``x``.
     """
     ...
 
-
 def log10(x) -> float:
     """
     Return the base-10 logarithm of ``x``.
     """
     ...
 
-
 def sin(x) -> float:
     """
     Return the sine of ``x``.
     """
     ...
 
-
 def modf(x) -> Tuple:
     """
     Return a tuple of two floats, being the fractional and integral parts of
     ``x``.  Both return values have the same sign as ``x``.
     """
     ...
 
-
 def radians(x) -> Any:
     """
     Return degrees ``x`` converted to radians.
     """
     ...
 
-
 def atanh(x) -> float:
     """
     Return the inverse hyperbolic tangent of ``x``.
     """
     ...
 
-
 def atan2(y, x) -> float:
     """
     Return the principal value of the inverse tangent of ``y/x``.
     """
     ...
 
-
 def atan(x) -> float:
     """
     Return the inverse tangent of ``x``.
     """
     ...
 
-
 def ceil(x) -> int:
     """
     Return an integer, being ``x`` rounded towards positive infinity.
     """
     ...
 
-
 def copysign(x, y) -> Any:
     """
     Return ``x`` with the sign of ``y``.
     """
     ...
 
-
 def frexp(x) -> Any:
     """
     Decomposes a floating-point number into its mantissa and exponent.
     The returned value is the tuple ``(m, e)`` such that ``x == m * 2**e``
     exactly.  If ``x == 0`` then the function returns ``(0.0, 0)``, otherwise
     the relation ``0.5 <= abs(m) < 1`` holds.
     """
     ...
 
-
 def acos(x) -> float:
     """
     Return the inverse cosine of ``x``.
     """
     ...
 
-
 def pow(x, y) -> Any:
     """
     Returns ``x`` to the power of ``y``.
     """
     ...
 
-
 def asinh(x) -> float:
     """
     Return the inverse hyperbolic sine of ``x``.
     """
     ...
 
-
 def acosh(x) -> float:
     """
     Return the inverse hyperbolic cosine of ``x``.
     """
     ...
 
-
 def asin(x) -> float:
     """
     Return the inverse sine of ``x``.
     """
     ...
 
-
-def factorial(*args, **kwargs) -> Any:
-    ...
-
-
+def factorial(*args, **kwargs) -> Any: ...
 def fabs(x) -> Any:
     """
     Return the absolute value of ``x``.
     """
     ...
 
-
 def expm1(x) -> Any:
     """
     Return ``exp(x) - 1``.
     """
     ...
 
-
 def floor(x) -> int:
     """
     Return an integer, being ``x`` rounded towards negative infinity.
     """
     ...
 
-
 def fmod(x, y) -> Any:
     """
     Return the remainder of ``x/y``.
     """
     ...
 
-
 def cos(x) -> float:
     """
     Return the cosine of ``x``.
     """
     ...
 
-
 def degrees(x) -> Any:
     """
     Return radians ``x`` converted to degrees.
     """
     ...
 
-
 def cosh(x) -> float:
     """
     Return the hyperbolic cosine of ``x``.
     """
     ...
 
-
 def exp(x) -> float:
     """
     Return the exponential of ``x``.
     """
     ...
 
-
 def erf(x) -> Any:
     """
     Return the error function of ``x``.
     """
     ...
 
-
 def erfc(x) -> Any:
     """
     Return the complementary error function of ``x``.
     """
     ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/micropython.pyi` & `micropython_esp32_s3_stubs-1.20.0.post1/micropython.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/micropython_.pyi` & `micropython_esp32_s3_stubs-1.20.0.post1/micropython_.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/network.py` & `micropython_esp32_s3_stubs-1.20.0.post1/network.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-network configuration. See: https://docs.micropython.org/en/v1.19.1/library/network.html
+network configuration. See: https://docs.micropython.org/en/v1.20.0/library/network.html
 
 This module provides network drivers and routing configuration. To use this
 module, a MicroPython variant/build with network capabilities must be installed.
 Network drivers for specific hardware are available within this module and are
 used to configure hardware network interface(s). Network services provided
 by configured interfaces are then available for use via the :mod:`socket`
 module.
@@ -27,107 +27,103 @@
     addr = socket.getaddrinfo('micropython.org', 80)[0][-1]
     s = socket.socket()
     s.connect(addr)
     s.send(b'GET / HTTP/1.1\r\nHost: micropython.org\r\n\r\n')
     data = s.recv(1000)
     s.close()
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import List, Optional, Tuple, Union, Any
 
-STAT_ASSOC_FAIL = 203  # type: int
-STAT_BEACON_TIMEOUT = 200  # type: int
-STAT_CONNECTING = 1001  # type: int
-MODE_11N = 4  # type: int
-MODE_11G = 2  # type: int
-MODE_11B = 1  # type: int
-STAT_NO_AP_FOUND = 201  # type: int
-STAT_WRONG_PASSWORD = 202  # type: int
-STAT_GOT_IP = 1010  # type: int
-STAT_IDLE = 1000  # type: int
-STAT_HANDSHAKE_TIMEOUT = 204  # type: int
-STA_IF = 0  # type: int
-AUTH_WAPI_PSK = 8  # type: int
-AUTH_WPA_WPA2_PSK = 4  # type: int
-AUTH_WEP = 1  # type: int
-AP_IF = 1  # type: int
-AUTH_OPEN = 0  # type: int
-AUTH_MAX = 9  # type: int
-AUTH_WPA3_PSK = 6  # type: int
-AUTH_WPA2_ENTERPRISE = 5  # type: int
-AUTH_WPA_PSK = 2  # type: int
-AUTH_WPA2_PSK = 3  # type: int
-AUTH_WPA2_WPA3_PSK = 7  # type: int
-
+STA_IF: int
+STAT_WRONG_PASSWORD: int
+STAT_ASSOC_FAIL: int
+MODE_11G: int
+MODE_LR: int
+MODE_11N: int
+STAT_IDLE: int
+STAT_BEACON_TIMEOUT: int
+STAT_NO_AP_FOUND: int
+STAT_CONNECTING: int
+STAT_HANDSHAKE_TIMEOUT: int
+STAT_GOT_IP: int
+AUTH_WAPI_PSK: int
+MODE_11B: int
+AUTH_WEP: int
+AP_IF: int
+AUTH_OPEN: int
+AUTH_MAX: int
+AUTH_WPA_PSK: int
+AUTH_WPA2_ENTERPRISE: int
+AUTH_WPA_WPA2_PSK: int
+AUTH_WPA2_PSK: int
+AUTH_WPA3_PSK: int
+AUTH_WPA2_WPA3_PSK: int
+
+def country(*args, **kwargs) -> Any: ...
+def hostname(*args, **kwargs) -> Any: ...
+def phy_mode(*args, **kwargs) -> Any: ...
 
 class WLAN:
     """
     Create a WLAN network interface object. Supported interfaces are
     ``network.STA_IF`` (station aka client, connects to upstream WiFi access
     points) and ``network.AP_IF`` (access point, allows other WiFi clients to
     connect). Availability of the methods below depends on interface type.
     For example, only STA interface may `WLAN.connect()` to an access point.
     """
 
-    def __init__(self, interface_id) -> None:
-        ...
-
+    def __init__(self, interface_id) -> None: ...
     def active(self, is_active: Optional[Any] = None) -> None:
         """
         Activate ("up") or deactivate ("down") network interface, if boolean
         argument is passed. Otherwise, query current state if no argument is
         provided. Most other methods require active interface.
         """
         ...
-
-    def connect(self, ssid=None, password=None, *, bssid=None) -> None:
+    def connect(self, ssid=None, key=None, *, bssid=None) -> None:
         """
-        Connect to the specified wireless network, using the specified password.
+        Connect to the specified wireless network, using the specified key.
         If *bssid* is given then the connection will be restricted to the
         access-point with that MAC address (the *ssid* must also be specified
         in this case).
         """
         ...
-
     def disconnect(self) -> None:
         """
         Disconnect from the currently connected wireless network.
         """
         ...
-
     def scan(self) -> List[Tuple]:
         """
         Scan for the available wireless networks.
         Hidden networks -- where the SSID is not broadcast -- will also be scanned
         if the WLAN interface allows it.
 
         Scanning is only possible on STA interface. Returns list of tuples with
         the information about WiFi access points:
 
-            (ssid, bssid, channel, RSSI, authmode, hidden)
+            (ssid, bssid, channel, RSSI, security, hidden)
 
         *bssid* is hardware address of an access point, in binary form, returned as
         bytes object. You can use `binascii.hexlify()` to convert it to ASCII form.
 
-        There are five values for authmode:
+        There are five values for security:
 
             * 0 -- open
             * 1 -- WEP
             * 2 -- WPA-PSK
             * 3 -- WPA2-PSK
             * 4 -- WPA/WPA2-PSK
 
         and two for hidden:
 
             * 0 -- visible
             * 1 -- hidden
         """
         ...
-
     def status(self, param: Optional[Any] = None) -> Any:
         """
         Return the current status of the wireless connection.
 
         When called with no argument the return value describes the network link status.
         The possible statuses are defined as constants:
 
@@ -138,68 +134,59 @@
             * ``STAT_CONNECT_FAIL`` -- failed due to other problems,
             * ``STAT_GOT_IP`` -- connection successful.
 
         When called with one argument *param* should be a string naming the status
         parameter to retrieve.  Supported parameters in WiFI STA mode are: ``'rssi'``.
         """
         ...
-
     def isconnected(self) -> bool:
         """
         In case of STA mode, returns ``True`` if connected to a WiFi access
         point and has a valid IP address.  In AP mode returns ``True`` when a
         station is connected. Returns ``False`` otherwise.
         """
         ...
-
     def ifconfig(self, configtuple: Optional[Any] = None) -> Tuple:
         """
         Get/set IP-level network interface parameters: IP address, subnet mask,
         gateway and DNS server. When called with no arguments, this method returns
         a 4-tuple with the above information. To set the above values, pass a
         4-tuple with the required information.  For example::
 
          nic.ifconfig(('192.168.0.4', '255.255.255.0', '192.168.0.1', '8.8.8.8'))
         """
         ...
-
     def config(self, *args, **kwargs) -> Any:
         """
         Get or set general network interface parameters. These methods allow to work
         with additional parameters beyond standard IP configuration (as dealt with by
         `WLAN.ifconfig()`). These include network-specific and hardware-specific
         parameters. For setting parameters, keyword argument syntax should be used,
         multiple parameters can be set at once. For querying, parameters name should
         be quoted as a string, and only one parameter can be queries at time::
 
-         # Set WiFi access point name (formally known as ESSID) and WiFi channel
-         ap.config(essid='My AP', channel=11)
+         # Set WiFi access point name (formally known as SSID) and WiFi channel
+         ap.config(ssid='My AP', channel=11)
          # Query params one by one
-         print(ap.config('essid'))
+         print(ap.config('ssid'))
          print(ap.config('channel'))
 
         Following are commonly supported parameters (availability of a specific parameter
         depends on network technology type, driver, and :term:`MicroPython port`).
 
         =============  ===========
         Parameter      Description
         =============  ===========
         mac            MAC address (bytes)
-        essid          WiFi access point name (string)
+        ssid           WiFi access point name (string)
         channel        WiFi channel (integer)
-        hidden         Whether ESSID is hidden (boolean)
-        authmode       Authentication mode supported (enumeration, see module constants)
-        password       Access password (string)
-        dhcp_hostname  The DHCP hostname to use
+        hidden         Whether SSID is hidden (boolean)
+        security       Security protocol supported (enumeration, see module constants)
+        key            Access key (string)
+        hostname       The hostname that will be sent to DHCP (STA interfaces) and mDNS (if supported, both STA and AP). (Deprecated, use :func:`network.hostname` instead)
         reconnects     Number of reconnect attempts to make (integer, 0=none, -1=unlimited)
         txpower        Maximum transmit power in dBm (integer or float)
         =============  ===========
         """
         ...
 
-
-def phy_mode(*args, **kwargs) -> Any:
-    ...
-
-
-def PPP(*args, **kwargs) -> Any:
-    ...
+def PPP(*args, **kwargs) -> Any: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/os.py` & `micropython_esp32_s3_stubs-1.20.0.post1/os.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 """
-basic "operating system" services. See: https://docs.micropython.org/en/v1.19.1/library/os.html
+basic "operating system" services. See: https://docs.micropython.org/en/v1.20.0/library/os.html
 
 |see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
 
 The ``os`` module contains functions for filesystem access and mounting,
 terminal redirection and duplication, and the ``uname`` and ``urandom``
 functions.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import IO, Iterator, Optional, Tuple, Any
 from stdlib.os import uname_result
 
-
 def stat(path) -> Any:
     """
     Get the status of a file or directory.
     """
     ...
 
-
 def rmdir(path) -> None:
     """
     Remove a directory.
     """
     ...
 
-
 def rename(old_path, new_path) -> None:
     """
     Rename a file.
     """
     ...
 
-
 def mount(fsobj, mount_point, *, readonly) -> Any:
     """
     Mount the filesystem object *fsobj* at the location in the VFS given by the
     *mount_point* string.  *fsobj* can be a a VFS object that has a ``mount()``
     method, or a block device.  If it's a block device then the filesystem type
     is automatically detected (an exception is raised if no filesystem was
     recognised).  *mount_point* may be ``'/'`` to mount *fsobj* at the root,
@@ -48,22 +42,20 @@
     During the mount process the method ``mount()`` is called on the filesystem
     object.
 
     Will raise ``OSError(EPERM)`` if *mount_point* is already mounted.
     """
     ...
 
-
 def mkdir(path) -> Any:
     """
     Create a new directory.
     """
     ...
 
-
 def statvfs(path) -> Tuple:
     """
     Get the status of a fileystem.
 
     Returns a tuple with the filesystem information in the following order:
 
          * ``f_bsize`` -- file system block size
@@ -79,60 +71,52 @@
 
     Parameters related to inodes: ``f_files``, ``f_ffree``, ``f_avail``
     and the ``f_flags`` parameter may return ``0`` as they can be unavailable
     in a port-specific implementation.
     """
     ...
 
-
-def unlink(*args, **kwargs) -> Any:
-    ...
-
-
+def unlink(*args, **kwargs) -> Any: ...
 def uname() -> uname_result:
     """
     Return a tuple (possibly a named tuple) containing information about the
     underlying machine and/or its operating system.  The tuple has five fields
     in the following order, each of them being a string:
 
          * ``sysname`` -- the name of the underlying system
          * ``nodename`` -- the network name (can be the same as ``sysname``)
          * ``release`` -- the version of the underlying system
          * ``version`` -- the MicroPython version and build date
          * ``machine`` -- an identifier for the underlying hardware (eg board, CPU)
     """
     ...
 
-
 def umount(mount_point) -> Any:
     """
     Unmount a filesystem. *mount_point* can be a string naming the mount location,
     or a previously-mounted filesystem object.  During the unmount process the
     method ``umount()`` is called on the filesystem object.
 
     Will raise ``OSError(EINVAL)`` if *mount_point* is not found.
     """
     ...
 
-
 def urandom(n) -> bytes:
     """
     Return a bytes object with *n* random bytes. Whenever possible, it is
     generated by the hardware random number generator.
     """
     ...
 
-
 def chdir(path) -> Any:
     """
     Change current directory.
     """
     ...
 
-
 def dupterm(stream_object, index=0, /) -> IO:
     """
     Duplicate or switch the MicroPython terminal (the REPL) on the given `stream`-like
     object. The *stream_object* argument must be a native stream object, or derive
     from ``io.IOBase`` and implement the ``readinto()`` and
     ``write()`` methods.  The stream should be in non-blocking mode and
     ``readinto()`` should return ``None`` if there is no data available for reading.
@@ -148,33 +132,27 @@
     If ``None`` is passed as the *stream_object* then duplication is cancelled on
     the slot given by *index*.
 
     The function returns the previous stream-like object in the given slot.
     """
     ...
 
-
 def remove(path) -> None:
     """
     Remove a file.
     """
     ...
 
-
 def listdir(dir: Optional[Any] = None) -> Any:
     """
     With no argument, list the current directory.  Otherwise list the given directory.
     """
     ...
 
-
-def dupterm_notify(*args, **kwargs) -> Any:
-    ...
-
-
+def dupterm_notify(*args, **kwargs) -> Any: ...
 def ilistdir(dir: Optional[Any] = None) -> Iterator[Tuple]:
     """
     This function returns an iterator which then yields tuples corresponding to
     the entries in the directory that it is listing.  With no argument it lists the
     current directory, otherwise it lists the directory given by *dir*.
 
     The tuples have the form *(name, type, inode[, size])*:
@@ -188,22 +166,20 @@
      - Some platforms may return a 4-tuple that includes the entry's *size*.  For
        file entries, *size* is an integer representing the size of the file
        or -1 if unknown.  Its meaning is currently undefined for directory
        entries.
     """
     ...
 
-
 def getcwd() -> Any:
     """
     Get the current directory.
     """
     ...
 
-
 class VfsLfs2:
     """
     Create a filesystem object that uses the `littlefs v2 filesystem format`_.
     Storage of the littlefs filesystem is provided by *block_dev*, which must
     support the :ref:`extended interface <block-device-interface>`.
     Objects created by this constructor can be mounted using :func:`mount`.
 
@@ -214,109 +190,56 @@
     timestamps will work without reformatting and timestamps will be added
     transparently to existing files once they are opened for writing.  When *mtime*
     is enabled `os.stat` on files without timestamps will return 0 for the timestamp.
 
     See :ref:`filesystem` for more information.
     """
 
-    def rename(self, *args, **kwargs) -> Any:
-        ...
-
+    def rename(self, *args, **kwargs) -> Any: ...
     @staticmethod
     def mkfs(block_dev, readsize=32, progsize=32, lookahead=32) -> None:
         """
             Build a Lfs2 filesystem on *block_dev*.
 
         ``Note:`` There are reports of littlefs v2 failing in certain situations,
                   for details see `littlefs issue 295`_.
         """
         ...
-
-    def mount(self, *args, **kwargs) -> Any:
-        ...
-
-    def statvfs(self, *args, **kwargs) -> Any:
-        ...
-
-    def rmdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def stat(self, *args, **kwargs) -> Any:
-        ...
-
-    def umount(self, *args, **kwargs) -> Any:
-        ...
-
-    def remove(self, *args, **kwargs) -> Any:
-        ...
-
-    def mkdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def open(self, *args, **kwargs) -> Any:
-        ...
-
-    def ilistdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def chdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def getcwd(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None:
-        ...
-
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None: ...
 
 class VfsFat:
     """
     Create a filesystem object that uses the FAT filesystem format.  Storage of
     the FAT filesystem is provided by *block_dev*.
     Objects created by this constructor can be mounted using :func:`mount`.
     """
 
-    def rename(self, *args, **kwargs) -> Any:
-        ...
-
+    def rename(self, *args, **kwargs) -> Any: ...
     @staticmethod
     def mkfs(block_dev) -> None:
         """
         Build a FAT filesystem on *block_dev*.
         """
         ...
-
-    def mount(self, *args, **kwargs) -> Any:
-        ...
-
-    def statvfs(self, *args, **kwargs) -> Any:
-        ...
-
-    def rmdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def stat(self, *args, **kwargs) -> Any:
-        ...
-
-    def umount(self, *args, **kwargs) -> Any:
-        ...
-
-    def remove(self, *args, **kwargs) -> Any:
-        ...
-
-    def mkdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def open(self, *args, **kwargs) -> Any:
-        ...
-
-    def ilistdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def chdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def getcwd(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, block_dev) -> None:
-        ...
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev) -> None: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/random.py` & `micropython_esp32_s3_stubs-1.20.0.post1/random.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-random numbers. See: https://docs.micropython.org/en/v1.19.1/library/random.html
+random numbers. See: https://docs.micropython.org/en/v1.20.0/library/random.html
 
 This module implements a pseudo-random number generator (PRNG).
 
 |see_cpython_module| :mod:`python:random` https://docs.python.org/3/library/random.html . .
 
 .. note::
 
@@ -21,75 +21,65 @@
 .. note::
 
    The :func:`randrange`, :func:`randint` and :func:`choice` functions are only
    available if the ``MICROPY_PY_URANDOM_EXTRA_FUNCS`` configuration option is
    enabled.
 
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Any
 
-
 def randrange(start, stop, step: Optional[Any] = None) -> int:
     """
     The first form returns a random integer from the range [0, *stop*).
     The second form returns a random integer from the range [*start*, *stop*).
     The third form returns a random integer from the range [*start*, *stop*) in
     steps of *step*.  For instance, calling ``randrange(1, 10, 2)`` will
     return odd numbers between 1 and 9 inclusive.
 
     """
     ...
 
-
 class random:
     """
     Return a random floating point number in the range [0.0, 1.0).
     """
 
-    def __init__(self) -> None:
-        ...
-
+    def __init__(self) -> None: ...
 
 def seed(n=None, /) -> None:
     """
     Initialise the random number generator module with the seed *n* which should
     be an integer.  When no argument (or ``None``) is passed in it will (if
     supported by the port) initialise the PRNG with a true random number
     (usually a hardware generated random number).
 
     The ``None`` case only works if ``MICROPY_PY_URANDOM_SEED_INIT_FUNC`` is
     enabled by the port, otherwise it raises ``ValueError``.
     """
     ...
 
-
 def uniform(a, b) -> int:
     """
     Return a random floating point number N such that *a* <= N <= *b* for *a* <= *b*,
     and *b* <= N <= *a* for *b* < *a*.
 
     """
     ...
 
-
 def choice(sequence) -> Any:
     """
     Chooses and returns one item at random from *sequence* (tuple, list or
     any object that supports the subscript operation).
     """
     ...
 
-
 def randint(a, b) -> int:
     """
     Return a random integer in the range [*a*, *b*].
     """
     ...
 
-
 def getrandbits(n) -> int:
     """
     Return an integer with *n* random bits (0 <= n <= 32).
     """
     ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/README.md` & `micropython_esp32_s3_stubs-1.20.0.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 
 If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
 
 For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
  * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
 
 Included stubs:
-* Merged stubs from `stubs/micropython-v1_19_1-esp32-s3-merged`
-* Frozen stubs from `stubs/micropython-v1_19_1-frozen/esp32/GENERIC`
+* Merged stubs from `stubs/micropython-v1_20_0-esp32-s3-merged`
+* Frozen stubs from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`
 * Core stubs from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
-Firmware | micropython | esp32 | ESP32S3 module with ESP32S3 | v1.19.1 
-Documentation | micropython | - | - | v1.19.1 
-Core | micropython | esp32 | - | v1.19.1 
+Documentation | micropython | - | - | v1.20.0 
+Core | micropython | esp32 | - | v1.20.0
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/select.py` & `micropython_esp32_s3_stubs-1.20.0.post1/select.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 """
-wait for events on a set of streams. See: https://docs.micropython.org/en/v1.19.1/library/select.html
+wait for events on a set of streams. See: https://docs.micropython.org/en/v1.20.0/library/select.html
 
 |see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
 
 This module provides functions to efficiently wait for events on multiple
 `streams <stream>` (select streams which are ready for operations).
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Iterator, List, Optional, Tuple, Any
 
-POLLOUT = 4  # type: int
-POLLIN = 1  # type: int
-POLLHUP = 16  # type: int
-POLLERR = 8  # type: int
-
+POLLOUT: int
+POLLIN: int
+POLLHUP: int
+POLLERR: int
 
 class select:
     """
     Wait for activity on a set of objects.
 
     This function is provided by some MicroPython ports for compatibility
     and is not efficient. Usage of :class:`Poll` is recommended instead.
     """
 
-    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None:
-        ...
-
+    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None: ...
 
 class poll:
     """
     Create an instance of the Poll class.
     """
 
-    def __init__(self) -> None:
-        ...
-
+    def __init__(self) -> None: ...
     def register(self, obj, eventmask: Optional[Any] = None) -> None:
         """
         Register `stream` *obj* for polling. *eventmask* is logical OR of:
 
         * ``select.POLLIN``  - data available for reading
         * ``select.POLLOUT`` - more data can be written
 
@@ -51,28 +44,25 @@
         *eventmask* defaults to ``select.POLLIN | select.POLLOUT``.
 
         It is OK to call this function multiple times for the same *obj*.
         Successive calls will update *obj*'s eventmask to the value of
         *eventmask* (i.e. will behave as `modify()`).
         """
         ...
-
     def unregister(self, obj) -> Any:
         """
         Unregister *obj* from polling.
         """
         ...
-
     def modify(self, obj, eventmask) -> None:
         """
         Modify the *eventmask* for *obj*. If *obj* is not registered, `OSError`
         is raised with error of ENOENT.
         """
         ...
-
     def poll(self, timeout=-1, /) -> List:
         """
         Wait for at least one of the registered objects to become ready or have an
         exceptional condition, with optional timeout in milliseconds (if *timeout*
         arg is not specified or -1, there is no timeout).
 
         Returns list of (``obj``, ``event``, ...) tuples. There may be other elements in
@@ -84,15 +74,14 @@
         corresponding stream unregistered from poll and likely closed), because
         otherwise all further invocations of `poll()` may return immediately with
         these flags set for this stream again.
 
         In case of timeout, an empty list is returned.
         """
         ...
-
     def ipoll(self, timeout=-1, flags=0, /) -> Iterator[Tuple]:
         """
         Like :meth:`poll.poll`, but instead returns an iterator which yields a
         `callee-owned tuple`. This function provides an efficient, allocation-free
         way to poll on streams.
 
         If *flags* is 1, one-shot behaviour for events is employed: streams for
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/socket.py` & `micropython_esp32_s3_stubs-1.20.0.post1/socket.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """
-socket module. See: https://docs.micropython.org/en/v1.19.1/library/socket.html
+socket module. See: https://docs.micropython.org/en/v1.20.0/library/socket.html
 
 |see_cpython_module| :mod:`python:socket` https://docs.python.org/3/library/socket.html .
 
 This module provides access to the BSD socket interface.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import IO, Optional, Tuple, Any
 
-SOCK_RAW = 3  # type: int
-SOCK_DGRAM = 2  # type: int
-IP_ADD_MEMBERSHIP = 3  # type: int
-SOCK_STREAM = 1  # type: int
-SOL_SOCKET = 4095  # type: int
-SO_REUSEADDR = 4  # type: int
-AF_INET6 = 10  # type: int
-AF_INET = 2  # type: int
-IPPROTO_UDP = 17  # type: int
-IPPROTO_IP = 0  # type: int
-IPPROTO_TCP = 6  # type: int
-
+SOCK_RAW: int
+SOCK_DGRAM: int
+IP_ADD_MEMBERSHIP: int
+SOCK_STREAM: int
+SOL_SOCKET: int
+SO_REUSEADDR: int
+AF_INET6: int
+AF_INET: int
+IPPROTO_UDP: int
+IPPROTO_IP: int
+IPPROTO_TCP: int
 
 def getaddrinfo(host, port, af=0, type=0, proto=0, flags=0, /) -> Any:
     """
     Translate the host/port argument into a sequence of 5-tuples that contain all the
     necessary arguments for creating a socket connected to that service. Arguments
     *af*, *type*, and *proto* (which have the same meaning as for the `socket()` function)
     can be used to filter which kind of addresses are returned. If a parameter is not
@@ -47,15 +44,14 @@
        s = socket.socket()
        # Guaranteed to return an address which can be connect'ed to for
        # stream operation.
        s.connect(socket.getaddrinfo('www.micropython.org', 80, 0, SOCK_STREAM)[0][-1])
     """
     ...
 
-
 class socket:
     """
     Create a new socket using the given address family, socket type and
     protocol number. Note that specifying *proto* in most cases is not
     required (and not recommended, as some MicroPython ports may omit
     ``IPPROTO_*`` constants). Instead, *type* argument will select needed
     protocol automatically::
@@ -69,82 +65,72 @@
     def recvfrom(self, bufsize) -> Tuple:
         """
         Receive data from the socket. The return value is a pair *(bytes, address)* where *bytes* is a
         bytes object representing the data received and *address* is the address of the socket sending
         the data.
         """
         ...
-
     def recv(self, bufsize) -> bytes:
         """
         Receive data from the socket. The return value is a bytes object representing the data
         received. The maximum amount of data to be received at once is specified by bufsize.
         """
         ...
-
     def makefile(self, mode="rb", buffering=0, /) -> IO:
         """
         Return a file object associated with the socket. The exact returned type depends on the arguments
         given to makefile(). The support is limited to binary modes only ('rb', 'wb', and 'rwb').
         CPython's arguments: *encoding*, *errors* and *newline* are not supported.
         """
         ...
-
     def listen(self, backlog: Optional[Any] = None) -> None:
         """
         Enable a server to accept connections. If *backlog* is specified, it must be at least 0
         (if it's lower, it will be set to 0); and specifies the number of unaccepted connections
         that the system will allow before refusing new connections. If not specified, a default
         reasonable value is chosen.
         """
         ...
-
-    def fileno(self, *args, **kwargs) -> Any:
-        ...
-
+    def fileno(self, *args, **kwargs) -> Any: ...
     def sendall(self, bytes) -> int:
         """
         Send all data to the socket. The socket must be connected to a remote socket.
         Unlike `send()`, this method will try to send all of data, by sending data
         chunk by chunk consecutively.
 
         The behaviour of this method on non-blocking sockets is undefined. Due to this,
         on MicroPython, it's recommended to use `write()` method instead, which
         has the same "no short writes" policy for blocking sockets, and will return
         number of bytes sent on non-blocking sockets.
         """
         ...
-
     def setsockopt(self, level, optname, value) -> None:
         """
         Set the value of the given socket option. The needed symbolic constants are defined in the
         socket module (SO_* etc.). The *value* can be an integer or a bytes-like object representing
         a buffer.
         """
         ...
-
     def setblocking(self, flag) -> Any:
         """
         Set blocking or non-blocking mode of the socket: if flag is false, the socket is set to non-blocking,
         else to blocking mode.
 
         This method is a shorthand for certain `settimeout()` calls:
 
         * ``sock.setblocking(True)`` is equivalent to ``sock.settimeout(None)``
         * ``sock.setblocking(False)`` is equivalent to ``sock.settimeout(0)``
         """
         ...
-
     def sendto(self, bytes, address) -> None:
         """
         Send data to the socket. The socket should not be connected to a remote socket, since the
         destination socket is specified by *address*.
         """
         ...
-
     def settimeout(self, value) -> Any:
         """
         **Note**: Not every port supports this method, see below.
 
         Set a timeout on blocking socket operations. The value argument can be a nonnegative floating
         point number expressing seconds, or None. If a non-zero value is given, subsequent socket operations
         will raise an `OSError` exception if the timeout period value has elapsed before the operation has
@@ -164,89 +150,78 @@
              poller = select.poll()
              poller.register(s, select.POLLIN)
              res = poller.poll(1000)  # time in milliseconds
              if not res:
                  # s is still not ready for input, i.e. operation timed out
         """
         ...
-
     def readline(self) -> Any:
         """
         Read a line, ending in a newline character.
 
         Return value: the line read.
         """
         ...
-
     def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
         """
         Read bytes into the *buf*.  If *nbytes* is specified then read at most
         that many bytes.  Otherwise, read at most *len(buf)* bytes. Just as
         `read()`, this method follows "no short reads" policy.
 
         Return value: number of bytes read and stored into *buf*.
         """
         ...
-
     def read(self, size: Optional[Any] = None) -> bytes:
         """
         Read up to size bytes from the socket. Return a bytes object. If *size* is not given, it
         reads all data available from the socket until EOF; as such the method will not return until
         the socket is closed. This function tries to read as much data as
         requested (no "short reads"). This may be not possible with
         non-blocking socket though, and then less data will be returned.
         """
         ...
-
     def close(self) -> Any:
         """
         Mark the socket closed and release all resources. Once that happens, all future operations
         on the socket object will fail. The remote end will receive EOF indication if
         supported by protocol.
 
         Sockets are automatically closed when they are garbage-collected, but it is recommended
         to `close()` them explicitly as soon you finished working with them.
         """
         ...
-
     def connect(self, address) -> None:
         """
         Connect to a remote socket at *address*.
         """
         ...
-
     def send(self, bytes) -> int:
         """
         Send data to the socket. The socket must be connected to a remote socket.
         Returns number of bytes sent, which may be smaller than the length of data
         ("short write").
         """
         ...
-
     def bind(self, address) -> Any:
         """
         Bind the socket to *address*. The socket must not already be bound.
         """
         ...
-
     def accept(self) -> Tuple:
         """
         Accept a connection. The socket must be bound to an address and listening for connections.
         The return value is a pair (conn, address) where conn is a new socket object usable to send
         and receive data on the connection, and address is the address bound to the socket on the
         other end of the connection.
         """
         ...
-
     def write(self, buf) -> int:
         """
         Write the buffer of bytes to the socket. This function will try to
         write all data to a socket (no "short writes"). This may be not possible
         with a non-blocking socket though, and returned value will be less than
         the length of *buf*.
 
         Return value: number of bytes written.
         """
         ...
-
-    def __init__(self, af=AF_INET, type=SOCK_STREAM, proto=IPPROTO_TCP, /) -> None:
-        ...
+    def __init__(self, af=AF_INET, type=SOCK_STREAM, proto=IPPROTO_TCP, /) -> None: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/time.py` & `micropython_esp32_s3_stubs-1.20.0.post1/time.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
-time related functions. See: https://docs.micropython.org/en/v1.19.1/library/time.html
+time related functions. See: https://docs.micropython.org/en/v1.20.0/library/time.html
 
 |see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
 
 The ``time`` module provides functions for getting the current time and date,
 measuring time intervals, and for delays.
 
 **Time Epoch**: Unix port uses standard for POSIX systems epoch of
-1970-01-01 00:00:00 UTC. However, embedded ports use epoch of
-2000-01-01 00:00:00 UTC.
+1970-01-01 00:00:00 UTC. However, some embedded ports use epoch of
+2000-01-01 00:00:00 UTC. Epoch year may be determined with ``gmtime(0)[0]``.
 
 **Maintaining actual calendar date/time**: This requires a
 Real Time Clock (RTC). On systems with underlying OS (including some
 RTOS), an RTC may be implicit. Setting and maintaining actual calendar
 time is responsibility of OS/RTOS and is done outside of MicroPython,
 it just uses OS API to query date/time. On baremetal ports however
 system time depends on ``machine.RTC()`` object. The current calendar time
@@ -26,19 +26,16 @@
   RTC time across hard resets, though some may require setting it again
   in such case).
 
 If actual calendar time is not maintained with a system/MicroPython RTC,
 functions below which require reference to current absolute time may
 behave not as expected.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Tuple, Any
 
-
 def ticks_diff(ticks1, ticks2) -> int:
     """
     Measure ticks difference between values returned from `ticks_ms()`, `ticks_us()`,
     or `ticks_cpu()` functions, as a signed value which may wrap around.
 
     The argument order is the same as for subtraction
     operator, ``ticks_diff(ticks1, ticks2)`` has the same meaning as ``ticks1 - ticks2``.
@@ -98,15 +95,14 @@
     Note: Do not pass `time()` values to `ticks_diff()`, you should use
     normal mathematical operations on them. But note that `time()` may (and will)
     also overflow. This is known as https://en.wikipedia.org/wiki/Year_2038_problem .
 
     """
     ...
 
-
 def ticks_add(ticks, delta) -> Any:
     """
     Offset ticks value by a given number, which can be either positive or negative.
     Given a *ticks* value, this function allows to calculate ticks value *delta*
     ticks before or after it, following modular-arithmetic definition of tick values
     (see `ticks_ms()` above). *ticks* parameter must be a direct result of call
     to `ticks_ms()`, `ticks_us()`, or `ticks_cpu()` functions (or from previous
@@ -127,15 +123,14 @@
 
          # Find out TICKS_MAX used by this port
          print(ticks_add(0, -1))
 
     """
     ...
 
-
 def ticks_cpu() -> Any:
     """
     Similar to `ticks_ms()` and `ticks_us()`, but with the highest possible resolution
     in the system. This is usually CPU clocks, and that's why the function is named that
     way. But it doesn't have to be a CPU clock, some other timing source available in a
     system (e.g. high-resolution timer) can be used instead. The exact timing unit
     (resolution) of this function is not specified on ``time`` module level, but
@@ -144,31 +139,28 @@
     Avoid using it in portable code.
 
     Availability: Not every port implements this function.
 
     """
     ...
 
-
 class time:
     """
     Returns the number of seconds, as an integer, since the Epoch, assuming that
     underlying RTC is set and maintained as described above. If an RTC is not set, this
     function returns number of seconds since a port-specific reference point in time (for
     embedded boards without a battery-backed RTC, usually since power up or reset). If you
     want to develop portable MicroPython application, you should not rely on this function
     to provide higher than second precision.  If you need higher precision, absolute
     timestamps, use `time_ns()`.  If relative times are acceptable then use the
     `ticks_ms()` and `ticks_us()` functions.  If you need calendar time, `gmtime()` or
     `localtime()` without an argument is a better choice.
     """
 
-    def __init__(self) -> None:
-        ...
-
+    def __init__(self) -> None: ...
 
 def ticks_ms() -> int:
     """
     Returns an increasing millisecond counter with an arbitrary reference point, that
     wraps around after some value.
 
     The wrap-around value is not explicitly exposed, but we will
@@ -186,30 +178,27 @@
     operators (<, <=, >, >=) directly on these value will lead to invalid
     result. Performing mathematical operations and then passing their results
     as arguments to `ticks_diff()` or `ticks_add()` will also lead to
     invalid results from the latter functions.
     """
     ...
 
-
 def ticks_us() -> Any:
     """
     Just like `ticks_ms()` above, but in microseconds.
     """
     ...
 
-
 def time_ns() -> int:
     """
     Similar to `time()` but returns nanoseconds since the Epoch, as an integer (usually
     a big integer, so will allocate on the heap).
     """
     ...
 
-
 def localtime(secs: Optional[Any] = None) -> Tuple:
     """
     Convert the time *secs* expressed in seconds since the Epoch (see above) into an
     8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
     If *secs* is not provided or None, then the current time from the RTC is used.
 
     The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
@@ -224,26 +213,24 @@
     * minute  is 0-59
     * second  is 0-59
     * weekday is 0-6 for Mon-Sun
     * yearday is 1-366
     """
     ...
 
-
 def sleep_us(us) -> None:
     """
     Delay for given number of microseconds, should be positive or 0.
 
     This function attempts to provide an accurate delay of at least *us*
     microseconds, but it may take longer if the system has other higher priority
     processing to perform.
     """
     ...
 
-
 def gmtime(secs: Optional[Any] = None) -> Tuple:
     """
     Convert the time *secs* expressed in seconds since the Epoch (see above) into an
     8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
     If *secs* is not provided or None, then the current time from the RTC is used.
 
     The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
@@ -258,36 +245,33 @@
     * minute  is 0-59
     * second  is 0-59
     * weekday is 0-6 for Mon-Sun
     * yearday is 1-366
     """
     ...
 
-
 def sleep_ms(ms) -> None:
     """
     Delay for given number of milliseconds, should be positive or 0.
 
     This function will delay for at least the given number of milliseconds, but
     may take longer than that if other processing must take place, for example
     interrupt handlers or other threads.  Passing in 0 for *ms* will still allow
     this other processing to occur.  Use `sleep_us()` for more precise delays.
     """
     ...
 
-
 def mktime() -> int:
     """
     This is inverse function of localtime. It's argument is a full 8-tuple
     which expresses a time as per localtime. It returns an integer which is
     the number of seconds since Jan 1, 2000.
     """
     ...
 
-
 def sleep(seconds) -> Any:
     """
     Sleep for the given number of seconds. Some boards may accept *seconds* as a
     floating-point number to sleep for a fractional number of seconds. Note that
     other boards may not accept a floating-point argument, for compatibility with
     them use `sleep_ms()` and `sleep_us()` functions.
     """
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/ubinascii.py` & `micropython_esp32_s3_stubs-1.20.0.post1/ubinascii.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,43 @@
 """
-binary/ASCII conversions. See: https://docs.micropython.org/en/v1.19.1/library/binascii.html
+binary/ASCII conversions. See: https://docs.micropython.org/en/v1.20.0/library/binascii.html
 
 |see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
 
 This module implements conversions between binary data and various
 encodings of it in ASCII form (in both directions).
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Any
 
-
-def crc32(*args, **kwargs) -> Any:
-    ...
-
-
+def crc32(*args, **kwargs) -> Any: ...
 def hexlify(data, sep: Optional[Any] = None) -> bytes:
     """
     Convert the bytes in the *data* object to a hexadecimal representation.
     Returns a bytes object.
 
     If the additional argument *sep* is supplied it is used as a separator
     between hexadecimal values.
     """
     ...
 
-
 def unhexlify(data) -> bytes:
     """
     Convert hexadecimal data to binary representation. Returns bytes string.
     (i.e. inverse of hexlify)
     """
     ...
 
-
 def b2a_base64(data, *, newline=True) -> bytes:
     """
     Encode binary data in base64 format, as in `RFC 3548
     <https://tools.ietf.org/html/rfc3548.html>`_. Returns the encoded data
     followed by a newline character if newline is true, as a bytes object.
     """
     ...
 
-
 def a2b_base64(data) -> bytes:
     """
     Decode base64-encoded data, ignoring invalid characters in the input.
     Conforms to `RFC 2045 s.6.8 <https://tools.ietf.org/html/rfc2045#section-6.8>`_.
     Returns a bytes object.
     """
     ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/ubluetooth.py` & `micropython_esp32_s3_stubs-1.20.0.post1/ubluetooth.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,80 +1,50 @@
 """
-Low-level Bluetooth radio functionality. See: https://docs.micropython.org/en/v1.19.1/library/bluetooth.html
+Low-level Bluetooth radio functionality. See: https://docs.micropython.org/en/v1.20.0/library/bluetooth.html
 
 This module provides an interface to a Bluetooth controller on a board.
 Currently this supports Bluetooth Low Energy (BLE) in Central, Peripheral,
 Broadcaster, and Observer roles, as well as GATT Server and Client and L2CAP
 connection-oriented-channels. A device may operate in multiple roles
 concurrently. Pairing (and bonding) is supported on some ports.
 
 This API is intended to match the low-level Bluetooth protocol and provide
 building-blocks for higher-level abstractions such as specific device types.
 
+``Note:`` For most applications, we recommend using the higher-level
+          `aioble library <https://github.com/micropython/micropython-lib/tree/master/micropython/bluetooth/aioble>`_.
+
 ``Note:`` This module is still under development and its classes, functions,
           methods and constants are subject to change.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Tuple, Any
 
-FLAG_NOTIFY = 16  # type: int
-FLAG_READ = 2  # type: int
-FLAG_WRITE = 8  # type: int
-FLAG_INDICATE = 32  # type: int
-FLAG_WRITE_NO_RESPONSE = 4  # type: int
-
+FLAG_NOTIFY: int
+FLAG_READ: int
+FLAG_WRITE: int
+FLAG_INDICATE: int
+FLAG_WRITE_NO_RESPONSE: int
 
 class UUID:
     """
     Creates a UUID instance with the specified **value**.
 
     The **value** can be either:
 
     - A 16-bit integer. e.g. ``0x2908``.
     - A 128-bit UUID string. e.g. ``'6E400001-B5A3-F393-E0A9-E50E24DCCA9E'``.
     """
 
-    def __init__(self, value, /) -> None:
-        ...
-
+    def __init__(self, value, /) -> None: ...
 
 class BLE:
     """
     Returns the singleton BLE object.
     """
 
-    def gatts_notify(self, conn_handle, value_handle, data=None, /) -> None:
-        """
-        Sends a notification request to a connected client.
-
-        If *data* is not ``None``, then that value is sent to the client as part of
-        the notification. The local value will not be modified.
-
-        Otherwise, if *data* is ``None``, then the current local value (as
-        set with :meth:`gatts_write <BLE.gatts_write>`) will be sent.
-
-        **Note:** The notification will be sent regardless of the subscription
-        status of the client to this characteristic.
-        """
-        ...
-
-    def gatts_indicate(self, conn_handle, value_handle, /) -> None:
-        """
-        Sends an indication request containing the characteristic's current value to
-        a connected client.
-
-        On acknowledgment (or failure, e.g. timeout), the
-        ``_IRQ_GATTS_INDICATE_DONE`` event will be raised.
-
-        **Note:** The indication will be sent regardless of the subscription
-        status of the client to this characteristic.
-        """
-        ...
-
     def gattc_write(self, conn_handle, value_handle, data, mode=0, /) -> None:
         """
         Issue a remote write to a connected server for the specified
         characteristic or descriptor handle.
 
         The argument *mode* specifies the write behaviour, with the currently
         supported values being:
@@ -86,70 +56,99 @@
               requested to send a response/acknowledgement that it received the
               data.
 
         If a response is received from the remote server the
         ``_IRQ_GATTC_WRITE_DONE`` event will be raised.
         """
         ...
+    def gatts_indicate(self, conn_handle, value_handle, data=None, /) -> None:
+        """
+        Sends a indication request to a connected client.
+
+        If *data* is ``None`` (the default), then the current local value (as set
+        with :meth:`gatts_write <BLE.gatts_write>`) will be sent.
 
+        Otherwise, if *data* is not ``None``, then that value is sent to the client
+        as part of the indication. The local value will not be modified.
+
+        On acknowledgment (or failure, e.g. timeout), the
+        ``_IRQ_GATTS_INDICATE_DONE`` event will be raised.
+
+        **Note:** The indication will be sent regardless of the subscription
+        status of the client to this characteristic.
+        """
+        ...
+    def gattc_discover_services(self, conn_handle, uuid=None, /) -> Any:
+        """
+        Query a connected server for its services.
+
+        Optionally specify a service *uuid* to query for that service only.
+
+        For each service discovered, the ``_IRQ_GATTC_SERVICE_RESULT`` event will
+        be raised, followed by ``_IRQ_GATTC_SERVICE_DONE`` on completion.
+        """
+        ...
     def gattc_read(self, conn_handle, value_handle, /) -> None:
         """
         Issue a remote read to a connected server for the specified
         characteristic or descriptor handle.
 
         When a value is available, the ``_IRQ_GATTC_READ_RESULT`` event will be
         raised. Additionally, the ``_IRQ_GATTC_READ_DONE`` will be raised.
         """
         ...
-
     def gattc_exchange_mtu(self, conn_handle, /) -> Any:
         """
         Initiate MTU exchange with a connected server, using the preferred MTU
         set using ``BLE.config(mtu=value)``.
 
         The ``_IRQ_MTU_EXCHANGED`` event will be raised when MTU exchange
         completes.
 
         **Note:** MTU exchange is typically initiated by the central. When using
         the BlueKitchen stack in the central role, it does not support a remote
         peripheral initiating the MTU exchange. NimBLE works for both roles.
 
         """
         ...
-
-    def gatts_read(self, value_handle, /) -> Any:
+    def gatts_set_buffer(self, value_handle, len, append=False, /) -> None:
         """
-        Reads the local value for this handle (which has either been written by
-        :meth:`gatts_write <BLE.gatts_write>` or by a remote client).
+        Sets the internal buffer size for a value in bytes. This will limit the
+        largest possible write that can be received. The default is 20.
+
+        Setting *append* to ``True`` will make all remote writes append to, rather
+        than replace, the current value. At most *len* bytes can be buffered in
+        this way. When you use :meth:`gatts_read <BLE.gatts_read>`, the value will
+        be cleared after reading. This feature is useful when implementing something
+        like the Nordic UART Service.
         """
         ...
-
     def gatts_write(self, value_handle, data, send_update=False, /) -> None:
         """
         Writes the local value for this handle, which can be read by a client.
 
         If *send_update* is ``True``, then any subscribed clients will be notified
         (or indicated, depending on what they're subscribed to and which operations
         the characteristic supports) about this write.
         """
         ...
-
-    def gatts_set_buffer(self, value_handle, len, append=False, /) -> None:
+    def gatts_notify(self, conn_handle, value_handle, data=None, /) -> None:
         """
-        Sets the internal buffer size for a value in bytes. This will limit the
-        largest possible write that can be received. The default is 20.
+        Sends a notification request to a connected client.
 
-        Setting *append* to ``True`` will make all remote writes append to, rather
-        than replace, the current value. At most *len* bytes can be buffered in
-        this way. When you use :meth:`gatts_read <BLE.gatts_read>`, the value will
-        be cleared after reading. This feature is useful when implementing something
-        like the Nordic UART Service.
+        If *data* is ``None`` (the default), then the current local value (as set
+        with :meth:`gatts_write <BLE.gatts_write>`) will be sent.
+
+        Otherwise, if *data* is not ``None``, then that value is sent to the client
+        as part of the notification. The local value will not be modified.
+
+        **Note:** The notification will be sent regardless of the subscription
+        status of the client to this characteristic.
         """
         ...
-
     def gatts_register_services(self, services_definition, /) -> Any:
         """
         Configures the server with the specified services, replacing any
         existing services.
 
         *services_definition* is a list of **services**, where each **service** is a
         two-element tuple containing a UUID and a list of **characteristics**.
@@ -204,15 +203,20 @@
             _FLAG_WRITE_ENCRYPTED = const(0x1000)
             _FLAG_WRITE_AUTHENTICATED = const(0x2000)
             _FLAG_WRITE_AUTHORIZED = const(0x4000)
 
         As for the IRQs above, any required constants should be added to your Python code.
         """
         ...
-
+    def gatts_read(self, value_handle, /) -> Any:
+        """
+        Reads the local value for this handle (which has either been written by
+        :meth:`gatts_write <BLE.gatts_write>` or by a remote client).
+        """
+        ...
     def irq(self, handler, /) -> int:
         """
             Registers a callback for events from the BLE stack. The *handler* takes two
             arguments, ``event`` (which will be one of the codes below) and ``data``
             (which is an event-specific tuple of values).
 
             **Note:** As an optimisation to prevent unnecessary allocations, the ``addr``,
@@ -266,15 +270,15 @@
                         conn_handle, start_handle, end_handle, uuid = data
                     elif event == _IRQ_GATTC_SERVICE_DONE:
                         # Called once service discovery is complete.
                         # Note: Status will be zero on success, implementation-specific value otherwise.
                         conn_handle, status = data
                     elif event == _IRQ_GATTC_CHARACTERISTIC_RESULT:
                         # Called for each characteristic found by gattc_discover_services().
-                        conn_handle, def_handle, value_handle, properties, uuid = data
+                        conn_handle, end_handle, value_handle, properties, uuid = data
                     elif event == _IRQ_GATTC_CHARACTERISTIC_DONE:
                         # Called once service discovery is complete.
                         # Note: Status will be zero on success, implementation-specific value otherwise.
                         conn_handle, status = data
                     elif event == _IRQ_GATTC_DESCRIPTOR_RESULT:
                         # Called for each descriptor found by gattc_discover_descriptors().
                         conn_handle, dsc_handle, uuid = data
@@ -283,20 +287,18 @@
                         # Note: Status will be zero on success, implementation-specific value otherwise.
                         conn_handle, status = data
                     elif event == _IRQ_GATTC_READ_RESULT:
                         # A gattc_read() has completed.
                         conn_handle, value_handle, char_data = data
                     elif event == _IRQ_GATTC_READ_DONE:
                         # A gattc_read() has completed.
-                        # Note: The value_handle will be zero on btstack (but present on NimBLE).
                         # Note: Status will be zero on success, implementation-specific value otherwise.
                         conn_handle, value_handle, status = data
                     elif event == _IRQ_GATTC_WRITE_DONE:
                         # A gattc_write() has completed.
-                        # Note: The value_handle will be zero on btstack (but present on NimBLE).
                         # Note: Status will be zero on success, implementation-specific value otherwise.
                         conn_handle, value_handle, status = data
                     elif event == _IRQ_GATTC_NOTIFY:
                         # A server has sent a notify request.
                         conn_handle, value_handle, notify_data = data
                     elif event == _IRQ_GATTC_INDICATE:
                         # A server has sent an indicate request.
@@ -401,15 +403,31 @@
 
         In order to save space in the firmware, these constants are not included on the
         :mod:`bluetooth` module. Add the ones that you need from the list above to your
         program.
 
         """
         ...
+    def gap_advertise(self, interval_us, adv_data=None, *, resp_data=None, connectable=True) -> Any:
+        """
+        Starts advertising at the specified interval (in **micro** seconds). This
+        interval will be rounded down to the nearest 625us. To stop advertising, set
+        *interval_us* to ``None``.
+
+        *adv_data* and *resp_data* can be any type that implements the buffer
+        protocol (e.g. ``bytes``, ``bytearray``, ``str``). *adv_data* is included
+        in all broadcasts, and *resp_data* is send in reply to an active scan.
 
+        **Note:** if *adv_data* (or *resp_data*) is ``None``, then the data passed
+        to the previous call to ``gap_advertise`` will be re-used. This allows a
+        broadcaster to resume advertising with just ``gap_advertise(interval_us)``.
+        To clear the advertising payload pass an empty ``bytes``, i.e. ``b''``.
+
+        """
+        ...
     def gap_connect(self, addr_type, addr, scan_duration_ms=2000, min_conn_interval_us=None, max_conn_interval_us=None, /) -> None:
         """
         Connect to a peripheral.
 
         See :meth:`gap_scan <BLE.gap_scan>` for details about address types.
 
         To cancel an outstanding connection attempt early, call
@@ -426,33 +444,22 @@
         or both of *min_conn_interval_us* and *max_conn_interval_us*. Otherwise a
         default interval will be chosen, typically between 30000 and 50000
         microseconds. A shorter interval will increase throughput, at the expense
         of power usage.
 
         """
         ...
-
-    def gap_advertise(self, interval_us, adv_data=None, *, resp_data=None, connectable=True) -> Any:
+    def gattc_discover_descriptors(self, conn_handle, start_handle, end_handle, /) -> Any:
         """
-        Starts advertising at the specified interval (in **micro** seconds). This
-        interval will be rounded down to the nearest 625us. To stop advertising, set
-        *interval_us* to ``None``.
-
-        *adv_data* and *resp_data* can be any type that implements the buffer
-        protocol (e.g. ``bytes``, ``bytearray``, ``str``). *adv_data* is included
-        in all broadcasts, and *resp_data* is send in reply to an active scan.
-
-        **Note:** if *adv_data* (or *resp_data*) is ``None``, then the data passed
-        to the previous call to ``gap_advertise`` will be re-used. This allows a
-        broadcaster to resume advertising with just ``gap_advertise(interval_us)``.
-        To clear the advertising payload pass an empty ``bytes``, i.e. ``b''``.
+        Query a connected server for descriptors in the specified range.
 
+        For each descriptor discovered, the ``_IRQ_GATTC_DESCRIPTOR_RESULT`` event
+        will be raised, followed by ``_IRQ_GATTC_DESCRIPTOR_DONE`` on completion.
         """
         ...
-
     def config(self, param, /) -> Tuple:
         """
         Get or set configuration values of the BLE interface.  To get a value the
         parameter name should be quoted as a string, and just one parameter is
         queried at a time.  To set values use the keyword syntax, and one ore more
         parameter can be set at a time.
 
@@ -508,75 +515,22 @@
             _IO_CAPABILITY_NO_INPUT_OUTPUT = const(3)
             _IO_CAPABILITY_KEYBOARD_DISPLAY = const(4)
 
         - ``'le_secure'``: Sets whether "LE Secure" pairing is required. Default is
           false (i.e. allow "Legacy Pairing").
         """
         ...
-
     def active(self, active: Optional[Any] = None, /) -> Any:
         """
         Optionally changes the active state of the BLE radio, and returns the
         current state.
 
         The radio must be made active before using any other methods on this class.
         """
         ...
-
-    def gattc_discover_services(self, conn_handle, uuid=None, /) -> Any:
-        """
-        Query a connected server for its services.
-
-        Optionally specify a service *uuid* to query for that service only.
-
-        For each service discovered, the ``_IRQ_GATTC_SERVICE_RESULT`` event will
-        be raised, followed by ``_IRQ_GATTC_SERVICE_DONE`` on completion.
-        """
-        ...
-
-    def gap_disconnect(self, conn_handle, /) -> bool:
-        """
-        Disconnect the specified connection handle. This can either be a
-        central that has connected to this device (if acting as a peripheral)
-        or a peripheral that was previously connected to by this device (if acting
-        as a central).
-
-        On success, the ``_IRQ_PERIPHERAL_DISCONNECT`` or ``_IRQ_CENTRAL_DISCONNECT``
-        event will be raised.
-
-        Returns ``False`` if the connection handle wasn't connected, and ``True``
-        otherwise.
-
-        """
-        ...
-
-    def gattc_discover_descriptors(self, conn_handle, start_handle, end_handle, /) -> Any:
-        """
-        Query a connected server for descriptors in the specified range.
-
-        For each descriptor discovered, the ``_IRQ_GATTC_DESCRIPTOR_RESULT`` event
-        will be raised, followed by ``_IRQ_GATTC_DESCRIPTOR_DONE`` on completion.
-        """
-        ...
-
-    def gattc_discover_characteristics(self, conn_handle, start_handle, end_handle, uuid=None, /) -> Any:
-        """
-        Query a connected server for characteristics in the specified range.
-
-        Optionally specify a characteristic *uuid* to query for that
-        characteristic only.
-
-        You can use ``start_handle=1``, ``end_handle=0xffff`` to search for a
-        characteristic in any service.
-
-        For each characteristic discovered, the ``_IRQ_GATTC_CHARACTERISTIC_RESULT``
-        event will be raised, followed by ``_IRQ_GATTC_CHARACTERISTIC_DONE`` on completion.
-        """
-        ...
-
     def gap_scan(self, duration_ms, interval_us=1280000, window_us=11250, active=False, /) -> Any:
         """
         Run a scan operation lasting for the specified duration (in **milli** seconds).
 
         To scan indefinitely, set *duration_ms* to ``0``.
 
         To stop scanning, set *duration_ms* to ``None``.
@@ -605,10 +559,65 @@
         ``active`` can be set ``True`` if you want to receive scan responses in the results.
 
         When scanning is stopped (either due to the duration finishing or when
         explicitly stopped), the ``_IRQ_SCAN_DONE`` event will be raised.
 
         """
         ...
+    def gattc_discover_characteristics(self, conn_handle, start_handle, end_handle, uuid=None, /) -> Any:
+        """
+        Query a connected server for characteristics in the specified range.
+
+        Optionally specify a characteristic *uuid* to query for that
+        characteristic only.
+
+        You can use ``start_handle=1``, ``end_handle=0xffff`` to search for a
+        characteristic in any service.
+
+        For each characteristic discovered, the ``_IRQ_GATTC_CHARACTERISTIC_RESULT``
+        event will be raised, followed by ``_IRQ_GATTC_CHARACTERISTIC_DONE`` on completion.
+        """
+        ...
+    def gap_disconnect(self, conn_handle, /) -> bool:
+        """
+        Disconnect the specified connection handle. This can either be a
+        central that has connected to this device (if acting as a peripheral)
+        or a peripheral that was previously connected to by this device (if acting
+        as a central).
+
+        On success, the ``_IRQ_PERIPHERAL_DISCONNECT`` or ``_IRQ_CENTRAL_DISCONNECT``
+        event will be raised.
+
+        Returns ``False`` if the connection handle wasn't connected, and ``True``
+        otherwise.
+
+        """
+        ...
+    def gap_passkey(self, conn_handle, action, passkey, /) -> Any:
+        """
+        Respond to a ``_IRQ_PASSKEY_ACTION`` event for the specified *conn_handle*
+        and *action*.
+
+        The *passkey* is a numeric value and will depend on on the
+        *action* (which will depend on what I/O capability has been set):
+
+            * When the *action* is ``_PASSKEY_ACTION_INPUT``, then the application should
+              prompt the user to enter the passkey that is shown on the remote device.
+            * When the *action* is ``_PASSKEY_ACTION_DISPLAY``, then the application should
+              generate a random 6-digit passkey and show it to the user.
+            * When the *action* is ``_PASSKEY_ACTION_NUMERIC_COMPARISON``, then the application
+              should show the passkey that was provided in the ``_IRQ_PASSKEY_ACTION`` event
+              and then respond with either ``0`` (cancel pairing), or ``1`` (accept pairing).
 
-    def __init__(self) -> None:
+        """
+        ...
+    def gap_pair(self, conn_handle, /) -> Any:
+        """
+        Initiate pairing with the remote device.
+
+        Before calling this, ensure that the ``io``, ``mitm``, ``le_secure``, and
+        ``bond`` configuration options are set (via :meth:`config<BLE.config>`).
+
+        On successful pairing, the ``_IRQ_ENCRYPTION_UPDATE`` event will be raised.
+        """
         ...
+    def __init__(self) -> None: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/ucollections.py` & `micropython_esp32_s3_stubs-1.20.0.post1/ucollections.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """
-collection and container types. See: https://docs.micropython.org/en/v1.19.1/library/collections.html
+collection and container types. See: https://docs.micropython.org/en/v1.20.0/library/collections.html
 
 |see_cpython_module| :mod:`python:collections` https://docs.python.org/3/library/collections.html .
 
 This module implements advanced collection and container types to
 hold/accumulate various objects.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Any
 from queue import Queue
 
-
 def namedtuple(name, fields) -> Any:
     """
     This is factory function to create a new namedtuple type with a specific
     name and set of fields. A namedtuple is a subclass of tuple which allows
     to access its fields not just by numeric index, but also with an attribute
     access syntax using symbolic field names. Fields is a sequence of strings
     specifying field names. For compatibility with CPython it can also be a
@@ -28,16 +25,15 @@
         t1 = MyTuple(1, "foo")
         t2 = MyTuple(2, "bar")
         print(t1.name)
         assert t2.name == t2[1]
     """
     ...
 
-
-class OrderedDict:
+class OrderedDict(dict):
     """
     ``dict`` type subclass which remembers and preserves the order of keys
     added. When ordered dict is iterated over, keys/items are returned in
     the order they were added::
 
         from collections import OrderedDict
 
@@ -54,53 +50,29 @@
 
         z 1
         a 2
         w 5
         b 3
     """
 
-    def popitem(self, *args, **kwargs) -> Any:
-        ...
-
-    def pop(self, *args, **kwargs) -> Any:
-        ...
-
-    def values(self, *args, **kwargs) -> Any:
-        ...
-
-    def setdefault(self, *args, **kwargs) -> Any:
-        ...
-
-    def update(self, *args, **kwargs) -> Any:
-        ...
-
-    def copy(self, *args, **kwargs) -> Any:
-        ...
-
-    def clear(self, *args, **kwargs) -> Any:
-        ...
-
-    def keys(self, *args, **kwargs) -> Any:
-        ...
-
-    def get(self, *args, **kwargs) -> Any:
-        ...
-
-    def items(self, *args, **kwargs) -> Any:
-        ...
-
+    def popitem(self, *args, **kwargs) -> Any: ...
+    def pop(self, *args, **kwargs) -> Any: ...
+    def values(self, *args, **kwargs) -> Any: ...
+    def setdefault(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def copy(self, *args, **kwargs) -> Any: ...
+    def clear(self, *args, **kwargs) -> Any: ...
+    def keys(self, *args, **kwargs) -> Any: ...
+    def get(self, *args, **kwargs) -> Any: ...
+    def items(self, *args, **kwargs) -> Any: ...
     @classmethod
-    def fromkeys(cls, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, *args, **kwargs) -> None:
-        ...
-
+    def fromkeys(cls, *args, **kwargs) -> Any: ...
+    def __init__(self, *args, **kwargs) -> None: ...
 
-class deque:
+class deque(Queue):
     """
     Deques (double-ended queues) are a list-like container that support O(1)
     appends and pops from either side of the deque.  New deques are created
     using the following arguments:
 
         - *iterable* must be the empty tuple, and the new deque is created empty.
 
@@ -116,17 +88,14 @@
 
     def popleft(self) -> Any:
         """
         Remove and return an item from the left side of the deque.
         Raises IndexError if no items are present.
         """
         ...
-
     def append(self, x) -> Any:
         """
         Add *x* to the right side of the deque.
         Raises IndexError if overflow checking is enabled and there is no more room left.
         """
         ...
-
-    def __init__(self, iterable, maxlen, flags: Optional[Any] = None) -> None:
-        ...
+    def __init__(self, iterable, maxlen, flags: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/ucryptolib.py` & `micropython_esp32_s3_stubs-1.20.0.post1/ucryptolib.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 """
-cryptographic ciphers. See: https://docs.micropython.org/en/v1.19.1/library/cryptolib.html
+cryptographic ciphers. See: https://docs.micropython.org/en/v1.20.0/library/cryptolib.html
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Any
 
-
 class aes:
     def encrypt(self, in_buf, out_buf: Optional[Any] = None) -> Any:
         """
         Encrypt *in_buf*. If no *out_buf* is given result is returned as a
         newly allocated `bytes` object. Otherwise, result is written into
         mutable buffer *out_buf*. *in_buf* and *out_buf* can also refer
         to the same mutable buffer, in which case data is encrypted in-place.
         """
         ...
-
     def decrypt(self, in_buf, out_buf: Optional[Any] = None) -> Any:
         """
         Like `encrypt()`, but for decryption.
         """
         ...
-
     def __init__(self, key, mode, IV: Optional[Any] = None) -> None:
         """
         Initialize cipher object, suitable for encryption/decryption. Note:
         after initialization, cipher object can be use only either for
         encryption or decryption. Running decrypt() operation after encrypt()
         or vice versa is not supported.
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/uhashlib.py` & `micropython_esp32_s3_stubs-1.20.0.post1/uhashlib.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-hashing algorithms. See: https://docs.micropython.org/en/v1.19.1/library/hashlib.html
+hashing algorithms. See: https://docs.micropython.org/en/v1.20.0/library/hashlib.html
 
 |see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
 
 This module implements binary data hashing algorithms. The exact inventory
 of available algorithms depends on a board. Among the algorithms which may
 be implemented:
 
@@ -17,40 +17,26 @@
   applications, so boards targeting network connectivity and
   interoperability will try to provide this.
 
 * MD5 - A legacy algorithm, not considered cryptographically secure. Only
   selected boards, targeting interoperability with legacy applications,
   will offer this.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Any
 
-
 class sha256:
     """
     Create an SHA256 hasher object and optionally feed ``data`` into it.
     """
 
-    def digest(self, *args, **kwargs) -> Any:
-        ...
-
-    def update(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, data: Optional[Any] = None) -> None:
-        ...
-
+    def digest(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def __init__(self, data: Optional[Any] = None) -> None: ...
 
 class sha1:
     """
     Create an SHA1 hasher object and optionally feed ``data`` into it.
     """
 
-    def digest(self, *args, **kwargs) -> Any:
-        ...
-
-    def update(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, data: Optional[Any] = None) -> None:
-        ...
+    def digest(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def __init__(self, data: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/uheapq.py` & `micropython_esp32_s3_stubs-1.20.0.post1/uheapq.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 """
-heap queue algorithm. See: https://docs.micropython.org/en/v1.19.1/library/heapq.html
+heap queue algorithm. See: https://docs.micropython.org/en/v1.20.0/library/heapq.html
 
 |see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
 
 This module implements the
 `min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
 
 A heap queue is essentially a list that has its elements stored in such a way
 that the first item of the list is always the smallest.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Any
 
-
 def heappop(heap) -> Any:
     """
     Pop the first item from the ``heap``, and return it.  Raise ``IndexError`` if
     ``heap`` is empty.
 
     The returned item will be the smallest item in the ``heap``.
     """
     ...
 
-
 def heappush(heap, item) -> Any:
     """
     Push the ``item`` onto the ``heap``.
     """
     ...
 
-
 def heapify(x) -> Any:
     """
     Convert the list ``x`` into a heap.  This is an in-place operation.
     """
     ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/ujson.py` & `micropython_esp32_s3_stubs-1.20.0.post1/ujson.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 """
-JSON encoding and decoding. See: https://docs.micropython.org/en/v1.19.1/library/json.html
+JSON encoding and decoding. See: https://docs.micropython.org/en/v1.20.0/library/json.html
 
 |see_cpython_module| :mod:`python:json` https://docs.python.org/3/library/json.html .
 
 This modules allows to convert between Python objects and the JSON
 data format.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Any
 
-
 def loads(str) -> Any:
     """
     Parse the JSON *str* and return an object.  Raises :exc:`ValueError` if the
     string is not correctly formed.
     """
     ...
 
-
 def load(stream) -> Any:
     """
     Parse the given *stream*, interpreting it as a JSON string and
     deserialising the data to a Python object.  The resulting object is
     returned.
 
     Parsing continues until end-of-file is encountered.
     A :exc:`ValueError` is raised if the data in *stream* is not correctly formed.
     """
     ...
 
-
 def dumps(obj, separators=None) -> str:
     """
     Return *obj* represented as a JSON string.
 
     The arguments have the same meaning as in `dump`.
     """
     ...
 
-
 def dump(obj, stream, separators=None) -> Any:
     """
     Serialise *obj* to a JSON string, writing it to the given *stream*.
 
     If specified, separators should be an ``(item_separator, key_separator)``
     tuple. The default is ``(', ', ': ')``. To get the most compact JSON
     representation, you should specify ``(',', ':')`` to eliminate whitespace.
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/umachine.py` & `micropython_esp32_s3_stubs-1.20.0.post1/umachine.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,50 @@
 """
-functions related to the hardware. See: https://docs.micropython.org/en/v1.19.1/library/machine.html
+functions related to the hardware. See: https://docs.micropython.org/en/v1.20.0/library/machine.html
 
 The ``machine`` module contains specific functions related to the hardware
 on a particular board. Most functions in this module allow to achieve direct
 and unrestricted access to and control of hardware blocks on a system
 (like CPU, timers, buses, etc.). Used incorrectly, this can lead to
 malfunction, lockups, crashes of your board, and in extreme cases, hardware
 damage.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Callable, List, NoReturn, Optional, Tuple, Union, Any
 
-TOUCHPAD_WAKE = 5  # type: int
-HARD_RESET = 2  # type: int
-SOFT_RESET = 5  # type: int
-PWRON_RESET = 1  # type: int
-PIN_WAKE = 2  # type: int
-TIMER_WAKE = 4  # type: int
-SLEEP = 2  # type: int
-WDT_RESET = 3  # type: int
-EXT1_WAKE = 3  # type: int
-ULP_WAKE = 6  # type: int
-EXT0_WAKE = 2  # type: int
-DEEPSLEEP = 4  # type: int
-DEEPSLEEP_RESET = 4  # type: int
+SLEEP: int
+HARD_RESET: int
+SOFT_RESET: int
+PWRON_RESET: int
+PIN_WAKE: int
+TOUCHPAD_WAKE: int
+TIMER_WAKE: int
+WDT_RESET: int
+EXT1_WAKE: int
+ULP_WAKE: int
+EXT0_WAKE: int
+DEEPSLEEP: int
+DEEPSLEEP_RESET: int
 
+def disable_irq() -> Any:
+    """
+    Disable interrupt requests.
+    Returns the previous IRQ state which should be considered an opaque value.
+    This return value should be passed to the `enable_irq()` function to restore
+    interrupts to their original state, before `disable_irq()` was called.
+    """
+    ...
 
 def enable_irq(state) -> Any:
     """
     Re-enable interrupt requests.
     The *state* parameter should be the value that was returned from the most
     recent call to the `disable_irq()` function.
     """
     ...
 
-
-def wake_reason() -> Any:
-    """
-    Get the wake reason. See :ref:`constants <machine_constants>` for the possible return values.
-
-    Availability: ESP32, WiPy.
-    """
-    ...
-
-
 def bitstream(pin, encoding, timing, data, /) -> Any:
     """
     Transmits *data* by bit-banging the specified *pin*. The *encoding* argument
     specifies how the bits are encoded, and *timing* is an encoding-specific timing
     specification.
 
     The supported encodings are:
@@ -65,25 +61,15 @@
     will be closer to +/-30ns.
 
     ``Note:`` For controlling WS2812 / NeoPixel strips, see the :mod:`neopixel`
        module for a higher-level API.
     """
     ...
 
-
-def disable_irq() -> Any:
-    """
-    Disable interrupt requests.
-    Returns the previous IRQ state which should be considered an opaque value.
-    This return value should be passed to the `enable_irq()` function to restore
-    interrupts to their original state, before `disable_irq()` was called.
-    """
-    ...
-
-
+def dht_readinto(*args, **kwargs) -> Any: ...
 def deepsleep(time_ms: Optional[Any] = None) -> NoReturn:
     """
     Stops execution in an attempt to enter a low power state.
 
     If *time_ms* is specified then this will be the maximum time in milliseconds that
     the sleep will last for.  Otherwise the sleep can last indefinitely.
 
@@ -101,31 +87,36 @@
       peripherals or network interfaces).  Upon wake execution is resumed from the main
       script, similar to a hard or power-on reset. The `reset_cause()` function will
       return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
       from other resets.
     """
     ...
 
+def wake_reason() -> Any:
+    """
+    Get the wake reason. See :ref:`constants <machine_constants>` for the possible return values.
+
+    Availability: ESP32, WiPy.
+    """
+    ...
 
 def sleep() -> Any:
     """
     ``Note:`` This function is deprecated, use `lightsleep()` instead with no arguments.
     """
     ...
 
-
 def soft_reset() -> NoReturn:
     """
     Performs a soft reset of the interpreter, deleting all Python objects and
     resetting the Python heap.  It tries to retain the method by which the user
     is connected to the MicroPython REPL (eg serial, USB, Wifi).
     """
     ...
 
-
 def time_pulse_us(pin, pulse_level, timeout_us=1000000, /) -> int:
     """
     Time a pulse on the given *pin*, and return the duration of the pulse in
     microseconds.  The *pulse_level* argument should be 0 to time a low pulse
     or 1 to time a high pulse.
 
     If the current input value of the pin is different to *pulse_level*,
@@ -136,51 +127,46 @@
     The function will return -2 if there was timeout waiting for condition marked
     (*) above, and -1 if there was timeout during the main measurement, marked (**)
     above. The timeout is the same for both cases and given by *timeout_us* (which
     is in microseconds).
     """
     ...
 
-
 def unique_id() -> bytes:
     """
     Returns a byte string with a unique identifier of a board/SoC. It will vary
     from a board/SoC instance to another, if underlying hardware allows. Length
     varies by hardware (so use substring of a full value if you expect a short
     ID). In some MicroPython ports, ID corresponds to the network MAC address.
     """
     ...
 
-
 def freq(hz: Optional[Any] = None) -> Any:
     """
     Returns the CPU frequency in hertz.
 
     On some ports this can also be used to set the CPU frequency by passing in *hz*.
     """
     ...
 
-
 def reset_cause() -> int:
     """
     Get the reset cause. See :ref:`constants <machine_constants>` for the possible return values.
     """
     ...
 
-
 def idle() -> Any:
     """
     Gates the clock to the CPU, useful to reduce power consumption at any time during
     short or long periods. Peripherals continue working and execution resumes as soon
     as any interrupt is triggered (on many ports this includes system timer
     interrupt occurring at regular intervals on the order of millisecond).
     """
     ...
 
-
 def lightsleep(time_ms: Optional[Any] = None) -> Any:
     """
     Stops execution in an attempt to enter a low power state.
 
     If *time_ms* is specified then this will be the maximum time in milliseconds that
     the sleep will last for.  Otherwise the sleep can last indefinitely.
 
@@ -198,23 +184,21 @@
       peripherals or network interfaces).  Upon wake execution is resumed from the main
       script, similar to a hard or power-on reset. The `reset_cause()` function will
       return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
       from other resets.
     """
     ...
 
-
 def reset() -> NoReturn:
     """
     Resets the device in a manner similar to pushing the external RESET
     button.
     """
     ...
 
-
 class PWM:
     """
     Construct and return a new PWM object using the following parameters:
 
        - *dest* is the entity on which the PWM is output, which is usually a
          :ref:`machine.Pin <machine.Pin>` object, but a port may allow other values,
          like integers.
@@ -235,55 +219,46 @@
 
         With no arguments the duty cycle is returned.
 
         With a single *value* argument the duty cycle is set to that value, measured
         as the ratio ``value / 65535``.
         """
         ...
-
     def init(self, *, freq, duty_u16, duty_ns) -> None:
         """
         Modify settings for the PWM object.  See the above constructor for details
         about the parameters.
         """
         ...
-
     def freq(self, value: Optional[Any] = None) -> Any:
         """
         Get or set the current frequency of the PWM output.
 
         With no arguments the frequency in Hz is returned.
 
         With a single *value* argument the frequency is set to that value in Hz.  The
         method may raise a ``ValueError`` if the frequency is outside the valid range.
         """
         ...
-
     def deinit(self) -> None:
         """
         Disable the PWM output.
         """
         ...
-
     def duty_ns(self, value: Optional[Any] = None) -> int:
         """
         Get or set the current pulse width of the PWM output, as a value in nanoseconds.
 
         With no arguments the pulse width in nanoseconds is returned.
 
         With a single *value* argument the pulse width is set to that value.
         """
         ...
-
-    def duty(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, dest, *, freq=0, duty=0, duty_u16=0, duty_ns=0) -> None:
-        ...
-
+    def duty(self, *args, **kwargs) -> Any: ...
+    def __init__(self, dest, *, freq=0, duty=0, duty_u16=0, duty_ns=0) -> None: ...
 
 class Pin:
     """
     Access the pin peripheral (GPIO pin) associated with the given ``id``.  If
     additional arguments are given in the constructor then they are used to initialise
     the pin.  Any settings that are not specified will remain in their previous state.
 
@@ -341,28 +316,27 @@
     alternate-function mode are usually not used as GPIO but are instead driven by other
     hardware peripherals.  The only operation supported on such a pin is re-initialising,
     by calling the constructor or :meth:`Pin.init` method.  If a pin that is configured in
     alternate-function mode is re-initialised with ``Pin.IN``, ``Pin.OUT``, or
     ``Pin.OPEN_DRAIN``, the alternate function will be removed from the pin.
     """
 
-    OPEN_DRAIN = 7  # type: int
-    IRQ_FALLING = 2  # type: int
-    IRQ_RISING = 1  # type: int
-    PULL_UP = 2  # type: int
-    OUT = 3  # type: int
-    PULL_DOWN = 1  # type: int
-    WAKE_HIGH = 5  # type: int
-    DRIVE_0 = 0  # type: int
-    IN = 1  # type: int
-    WAKE_LOW = 4  # type: int
-    DRIVE_3 = 3  # type: int
-    DRIVE_1 = 1  # type: int
-    DRIVE_2 = 2  # type: int
-
+    OPEN_DRAIN: int
+    IRQ_FALLING: int
+    IRQ_RISING: int
+    PULL_UP: int
+    OUT: int
+    PULL_DOWN: int
+    WAKE_HIGH: int
+    DRIVE_0: int
+    IN: int
+    WAKE_LOW: int
+    DRIVE_3: int
+    DRIVE_1: int
+    DRIVE_2: int
     def irq(self, handler=None, trigger=IRQ_FALLING, *, priority=1, wake=None, hard=False) -> Callable[..., Any]:
         """
            Configure an interrupt handler to be called when the trigger source of the
            pin is active.  If the pin mode is ``Pin.IN`` then the trigger source is
            the external value on the pin.  If the pin mode is ``Pin.OUT`` then the
            trigger source is the output buffer of the pin.  Otherwise, if the pin mode
            is ``Pin.OPEN_DRAIN`` then the trigger source is the output buffer for
@@ -399,37 +373,33 @@
                Not all ports support this argument.
 
            This method returns a callback object.
 
         The following methods are not part of the core Pin API and only implemented on certain ports.
         """
         ...
-
     def off(self) -> None:
         """
         Set pin to "0" output level.
         """
         ...
-
     def on(self) -> None:
         """
         Set pin to "1" output level.
         """
         ...
-
     def init(self, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
         """
         Re-initialise the pin using the given parameters.  Only those arguments that
         are specified will be set.  The rest of the pin peripheral state will remain
         unchanged.  See the constructor documentation for details of the arguments.
 
         Returns ``None``.
         """
         ...
-
     def value(self, x: Optional[Any] = None) -> int:
         """
         This method allows to set and get the value of the pin, depending on whether
         the argument ``x`` is supplied or not.
 
         If the argument is omitted then this method gets the digital logic level of
         the pin, returning 0 or 1 corresponding to low and high voltage signals
@@ -455,43 +425,26 @@
           - ``Pin.OUT`` - The output buffer is set to the given value immediately.
           - ``Pin.OPEN_DRAIN`` - If the value is '0' the pin is set to a low voltage
             state.  Otherwise the pin is set to high-impedance state.
 
         When setting the value this method returns ``None``.
         """
         ...
-
-    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
-        ...
-
-
-mem8: Any  ## <class 'mem'> = <8-bit memory>
-mem32: Any  ## <class 'mem'> = <32-bit memory>
-
-
-class WDT:
-    """
-    Create a WDT object and start it. The timeout must be given in milliseconds.
-    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
-
-    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
-    cannot be specified, it is determined by the underlying system.
-    """
-
-    def feed(self) -> None:
+    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None: ...
+    def __call__(self, x: Optional[Any] = None) -> Any:
         """
-        Feed the WDT to prevent it from resetting the system. The application
-        should place this call in a sensible place ensuring that the WDT is
-        only fed after verifying that everything is functioning correctly.
+        Pin objects are callable.  The call method provides a (fast) shortcut to set
+        and get the value of the pin.  It is equivalent to Pin.value([x]).
+        See :meth:`Pin.value` for more details.
         """
         ...
 
-    def __init__(self, id=0, timeout=5000) -> None:
-        ...
-
+mem8: Any
+mem32: Any
+mem16: Any
 
 class I2S:
     """
     Construct an I2S object of the given id:
 
     - ``id`` identifies a particular I2S bus; it is board and port specific
 
@@ -511,69 +464,60 @@
 
     For all ports, DMA runs continuously in the background and allows user applications to perform other operations while
     sample data is transfered between the internal buffer and the I2S peripheral unit.
     Increasing the size of the internal buffer has the potential to increase the time that user applications can perform non-I2S operations
     before underflow (e.g. ``write`` method) or overflow (e.g. ``readinto`` method).
     """
 
-    RX = 9  # type: int
-    MONO = 0  # type: int
-    STEREO = 1  # type: int
-    TX = 5  # type: int
-
+    RX: int
+    MONO: int
+    STEREO: int
+    TX: int
     @staticmethod
     def shift(*, buf, bits, shift) -> Any:
         """
         bitwise shift of all samples contained in ``buf``. ``bits`` specifies sample size in bits. ``shift`` specifies the number of bits to shift each sample.
         Positive for left shift, negative for right shift.
         Typically used for volume control.  Each bit shift changes sample volume by 6dB.
         """
         ...
-
     def init(self, sck, *args, **kwargs) -> Any:
         """
         see Constructor for argument descriptions
         """
         ...
-
     def irq(self, handler) -> Any:
         """
         Set a callback. ``handler`` is called when ``buf`` is emptied (``write`` method) or becomes full (``readinto`` method).
         Setting a callback changes the ``write`` and ``readinto`` methods to non-blocking operation.
         ``handler`` is called in the context of the MicroPython scheduler.
         """
         ...
-
     def readinto(self, buf) -> int:
         """
         Read audio samples into the buffer specified by ``buf``.  ``buf`` must support the buffer protocol, such as bytearray or array.
         "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
         the left channel sample data is used.
         Returns number of bytes read
         """
         ...
-
     def deinit(self) -> Any:
         """
         Deinitialize the I2S bus
         """
         ...
-
     def write(self, buf) -> int:
         """
         Write audio samples contained in ``buf``. ``buf`` must support the buffer protocol, such as bytearray or array.
         "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
         the sample data is written to both the right and left channels.
         Returns number of bytes written
         """
         ...
-
-    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None:
-        ...
-
+    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None: ...
 
 class ADC:
     """
     Access the ADC associated with a source identified by *id*.  This
     *id* may be an integer (usually specifying a channel number), a
     :ref:`Pin <machine.Pin>` object, or other value supported by the
     underlying machine.
@@ -583,66 +527,53 @@
     previous or default values.  The settings are:
 
       - *sample_ns* is the sampling time in nanoseconds.
 
       - *atten* specifies the input attenuation.
     """
 
-    ATTN_2_5DB = 1  # type: int
-    WIDTH_12BIT = 12  # type: int
-    ATTN_6DB = 2  # type: int
-    ATTN_11DB = 3  # type: int
-    ATTN_0DB = 0  # type: int
-
+    ATTN_2_5DB: int
+    WIDTH_12BIT: int
+    ATTN_6DB: int
+    ATTN_11DB: int
+    ATTN_0DB: int
     def read_u16(self) -> int:
         """
         Take an analog reading and return an integer in the range 0-65535.
         The return value represents the raw reading taken by the ADC, scaled
         such that the minimum value is 0 and the maximum value is 65535.
         """
         ...
-
     def init(self, *, sample_ns, atten) -> Any:
         """
         Apply the given settings to the ADC.  Only those arguments that are
         specified will be changed.  See the ADC constructor above for what the
         arguments are.
         """
         ...
-
     def read_uv(self) -> int:
         """
         Take an analog reading and return an integer value with units of
         microvolts.  It is up to the particular port whether or not this value
         is calibrated, and how calibration is done.
         """
         ...
-
-    def width(self, *args, **kwargs) -> Any:
-        ...
-
-    def read(self, *args, **kwargs) -> Any:
-        ...
-
+    def width(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
     def block(self) -> Any:
         """
         Return the :ref:`ADCBlock <machine.ADCBlock>` instance associated with
         this ADC object.
 
         This method only exists if the port supports the
         :ref:`ADCBlock <machine.ADCBlock>` class.
         """
         ...
-
-    def atten(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None:
-        ...
-
+    def atten(self, *args, **kwargs) -> Any: ...
+    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None: ...
 
 class ADCBlock:
     """
     Access the ADC peripheral identified by *id*, which may be an integer
     or string.
 
     The *bits* argument, if given, sets the resolution in bits of the
@@ -652,15 +583,14 @@
 
     def init(self, *, bits) -> None:
         """
         Configure the ADC peripheral.  *bits* will set the resolution of the
         conversion process.
         """
         ...
-
     def connect(self, channel, source) -> Any:
         """
         Connect up a channel on the ADC peripheral so it is ready for sampling,
         and return an :ref:`ADC <machine.ADC>` object that represents that connection.
 
         The *channel* argument must be an integer, and *source* must be an object
         (for example a :ref:`Pin <machine.Pin>`) which can be connected up for sampling.
@@ -670,29 +600,28 @@
         If only *source* is given then that object is connected to a default
         channel ready for sampling.
 
         If both *channel* and *source* are given then they are connected together
         and made ready for sampling.
         """
         ...
-
-    def __init__(self, id, *, bits) -> None:
-        ...
-
+    def __init__(self, id, *, bits) -> None: ...
 
 class I2C:
     """
     Construct and return a new I2C object using the following parameters:
 
        - *id* identifies a particular I2C peripheral.  Allowed values for
          depend on the particular port/board
        - *scl* should be a pin object specifying the pin to use for SCL.
        - *sda* should be a pin object specifying the pin to use for SDA.
        - *freq* should be an integer which sets the maximum frequency
          for SCL.
+       - *timeout* is the maximum time in microseconds to allow for I2C
+         transactions.  This parameter is not allowed on some ports.
 
     Note that some ports/boards will have default values of *scl* and *sda*
     that can be changed in this constructor.  Others will have fixed values
     of *scl* and *sda* that cannot be changed.
     """
 
     def readfrom_mem_into(self, addr, memaddr, buf, *, addrsize=8) -> None:
@@ -702,63 +631,57 @@
         length of *buf*.
         The argument *addrsize* specifies the address size in bits (on ESP8266
         this argument is not recognised and the address size is always 8 bits).
 
         The method returns ``None``.
         """
         ...
-
     def readfrom_into(self, addr, buf, stop=True, /) -> None:
         """
         Read into *buf* from the peripheral specified by *addr*.
         The number of bytes read will be the length of *buf*.
         If *stop* is true then a STOP condition is generated at the end of the transfer.
 
         The method returns ``None``.
         """
         ...
-
     def readfrom_mem(self, addr, memaddr, nbytes, *, addrsize=8) -> bytes:
         """
         Read *nbytes* from the peripheral specified by *addr* starting from the memory
         address specified by *memaddr*.
         The argument *addrsize* specifies the address size in bits.
         Returns a `bytes` object with the data read.
         """
         ...
-
     def writeto_mem(self, addr, memaddr, buf, *, addrsize=8) -> None:
         """
         Write *buf* to the peripheral specified by *addr* starting from the
         memory address specified by *memaddr*.
         The argument *addrsize* specifies the address size in bits (on ESP8266
         this argument is not recognised and the address size is always 8 bits).
 
         The method returns ``None``.
         """
         ...
-
     def scan(self) -> List:
         """
         Scan all I2C addresses between 0x08 and 0x77 inclusive and return a list of
         those that respond.  A device responds if it pulls the SDA line low after
         its address (including a write bit) is sent on the bus.
         """
         ...
-
     def writeto(self, addr, buf, stop=True, /) -> int:
         """
         Write the bytes from *buf* to the peripheral specified by *addr*.  If a
         NACK is received following the write of a byte from *buf* then the
         remaining bytes are not sent.  If *stop* is true then a STOP condition is
         generated at the end of the transfer, even if a NACK is received.
         The function returns the number of ACKs that were received.
         """
         ...
-
     def writevto(self, addr, vector, stop=True, /) -> int:
         """
         Write the bytes contained in *vector* to the peripheral specified by *addr*.
         *vector* should be a tuple or list of objects with the buffer protocol.
         The *addr* is sent once and then the bytes from each object in *vector*
         are written out sequentially.  The objects in *vector* may be zero bytes
         in length in which case they don't contribute to the output.
@@ -766,182 +689,132 @@
         If a NACK is received following the write of a byte from one of the
         objects in *vector* then the remaining bytes, and any remaining objects,
         are not sent.  If *stop* is true then a STOP condition is generated at
         the end of the transfer, even if a NACK is received.  The function
         returns the number of ACKs that were received.
         """
         ...
-
     def start(self) -> None:
         """
         Generate a START condition on the bus (SDA transitions to low while SCL is high).
         """
         ...
-
     def readfrom(self, addr, nbytes, stop=True, /) -> bytes:
         """
         Read *nbytes* from the peripheral specified by *addr*.
         If *stop* is true then a STOP condition is generated at the end of the transfer.
         Returns a `bytes` object with the data read.
         """
         ...
-
     def readinto(self, buf, nack=True, /) -> Any:
         """
         Reads bytes from the bus and stores them into *buf*.  The number of bytes
         read is the length of *buf*.  An ACK will be sent on the bus after
         receiving all but the last byte.  After the last byte is received, if *nack*
         is true then a NACK will be sent, otherwise an ACK will be sent (and in this
         case the peripheral assumes more bytes are going to be read in a later call).
         """
         ...
-
     def init(self, scl, sda, *, freq=400000) -> None:
         """
         Initialise the I2C bus with the given arguments:
 
            - *scl* is a pin object for the SCL line
            - *sda* is a pin object for the SDA line
            - *freq* is the SCL clock rate
+
+         In the case of hardware I2C the actual clock frequency may be lower than the
+         requested frequency. This is dependant on the platform hardware. The actual
+         rate may be determined by printing the I2C object.
         """
         ...
-
     def stop(self) -> None:
         """
         Generate a STOP condition on the bus (SDA transitions to high while SCL is high).
         """
         ...
-
     def write(self, buf) -> int:
         """
         Write the bytes from *buf* to the bus.  Checks that an ACK is received
         after each byte and stops transmitting the remaining bytes if a NACK is
         received.  The function returns the number of ACKs that were received.
         """
         ...
-
     def __init__(
-        self, id: Union[int, str] = -1, *, scl: Optional[Union[Pin, str]] = None, sda: Optional[Union[Pin, str]] = None, freq=400_000
-    ) -> None:
-        ...
-
+        self,
+        id: Union[int, str] = -1,
+        *,
+        scl: Optional[Union[Pin, str]] = None,
+        sda: Optional[Union[Pin, str]] = None,
+        freq=400_000,
+        timeout=50000,
+    ) -> None: ...
 
-class SoftI2C:
+class WDT:
     """
-    Construct a new software I2C object.  The parameters are:
+    Create a WDT object and start it. The timeout must be given in milliseconds.
+    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
 
-       - *scl* should be a pin object specifying the pin to use for SCL.
-       - *sda* should be a pin object specifying the pin to use for SDA.
-       - *freq* should be an integer which sets the maximum frequency
-         for SCL.
-       - *timeout* is the maximum time in microseconds to wait for clock
-         stretching (SCL held low by another device on the bus), after
-         which an ``OSError(ETIMEDOUT)`` exception is raised.
+    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
+    cannot be specified, it is determined by the underlying system. On rp2040 devices,
+    the maximum timeout is 8388 ms.
     """
 
-    def readfrom_mem_into(self, *args, **kwargs) -> Any:
-        ...
-
-    def readfrom_into(self, *args, **kwargs) -> Any:
-        ...
-
-    def readfrom_mem(self, *args, **kwargs) -> Any:
-        ...
-
-    def writeto_mem(self, *args, **kwargs) -> Any:
-        ...
-
-    def scan(self, *args, **kwargs) -> Any:
-        ...
-
-    def writeto(self, *args, **kwargs) -> Any:
-        ...
-
-    def writevto(self, *args, **kwargs) -> Any:
-        ...
-
-    def start(self, *args, **kwargs) -> Any:
-        ...
-
-    def readfrom(self, *args, **kwargs) -> Any:
-        ...
-
-    def readinto(self, *args, **kwargs) -> Any:
-        ...
-
-    def init(self, *args, **kwargs) -> Any:
-        ...
-
-    def stop(self, *args, **kwargs) -> Any:
-        ...
-
-    def write(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None:
+    def feed(self) -> None:
+        """
+        Feed the WDT to prevent it from resetting the system. The application
+        should place this call in a sensible place ensuring that the WDT is
+        only fed after verifying that everything is functioning correctly.
+        """
         ...
-
+    def __init__(self, id=0, timeout=5000) -> None: ...
 
 class SoftSPI:
     """
     Construct a new software SPI object.  Additional parameters must be
     given, usually at least *sck*, *mosi* and *miso*, and these are used
     to initialise the bus.  See `SPI.init` for a description of the parameters.
     """
 
-    LSB = 1  # type: int
-    MSB = 0  # type: int
-
-    def deinit(self, *args, **kwargs) -> Any:
-        ...
-
-    def init(self, *args, **kwargs) -> Any:
-        ...
-
-    def write_readinto(self, *args, **kwargs) -> Any:
-        ...
-
-    def read(self, *args, **kwargs) -> Any:
-        ...
-
-    def write(self, *args, **kwargs) -> Any:
-        ...
-
-    def readinto(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None:
-        ...
-
+    LSB: int
+    MSB: int
+    def deinit(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def write_readinto(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None: ...
 
 class Timer:
     """
     Construct a new timer object of the given ``id``. ``id`` of -1 constructs a
     virtual timer (if supported by a board).
     ``id`` shall not be passed as a keyword argument.
 
     See ``init`` for parameters of initialisation.
     """
 
-    ONE_SHOT = 0  # type: int
-    PERIODIC = 1  # type: int
-
+    ONE_SHOT: int
+    PERIODIC: int
     def deinit(self) -> None:
         """
         Deinitialises the timer. Stops the timer, and disables the timer peripheral.
         """
         ...
-
-    def init(self, *, mode=PERIODIC, period=-1, callback=None) -> None:
+    def init(self, *, mode=PERIODIC, freq=-1, period=-1, callback=None) -> None:
         """
         Initialise the timer. Example::
 
             def mycallback(t):
                 pass
 
+            # periodic at 1kHz
+            tim.init(mode=Timer.PERIODIC, freq=1000, callback=mycallback)
+
             # periodic with 100ms period
             tim.init(period=100, callback=mycallback)
 
             # one shot firing after 1000ms
             tim.init(mode=Timer.ONE_SHOT, period=1000, callback=mycallback)
 
         Keyword arguments:
@@ -949,49 +822,62 @@
           - ``mode`` can be one of:
 
             - ``Timer.ONE_SHOT`` - The timer runs once until the configured
               period of the channel expires.
             - ``Timer.PERIODIC`` - The timer runs periodically at the configured
               frequency of the channel.
 
+          - ``freq`` - The timer frequency, in units of Hz.  The upper bound of
+            the frequency is dependent on the port.  When both the ``freq`` and
+            ``period`` arguments are given, ``freq`` has a higher priority and
+            ``period`` is ignored.
+
           - ``period`` - The timer period, in milliseconds.
 
           - ``callback`` - The callable to call upon expiration of the timer period.
             The callback must take one argument, which is passed the Timer object.
             The ``callback`` argument shall be specified. Otherwise an exception
             will occurr upon timer expiration:
             ``TypeError: 'NoneType' object isn't callable``
         """
         ...
+    def value(self, *args, **kwargs) -> Any: ...
+    def __init__(self, id=-1, *args, **kwargs) -> None: ...
 
-    def value(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, id=-1, *args, **kwargs) -> None:
-        ...
-
+class TouchPad:
+    def config(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def __init__(self, *argv, **kwargs) -> None: ...
 
 class UART:
     """
     Construct a UART object of the given id.
     """
 
-    INV_RTS = 64  # type: int
-    INV_RX = 4  # type: int
-    CTS = 2  # type: int
-    INV_CTS = 8  # type: int
-    INV_TX = 32  # type: int
-    RTS = 1  # type: int
-
+    INV_CTS: int
+    CTS: int
+    INV_TX: int
+    INV_RTS: int
+    INV_RX: int
+    RTS: int
     def deinit(self) -> None:
         """
         Turn off the UART bus.
+
+        .. note::
+          You will not be able to call ``init()`` on the object after ``deinit()``.
+          A new instance needs to be created in that case.
+        """
+        ...
+    def sendbreak(self) -> None:
+        """
+        Send a break condition on the bus. This drives the bus low for a duration
+        longer than required for a normal transmission of a character.
         """
         ...
-
     def init(self, baudrate=9600, bits=8, parity=None, stop=1, *args, **kwargs) -> None:
         """
         Initialise the UART bus with the given parameters:
 
           - *baudrate* is the clock rate.
           - *bits* is the number of bits per character, 7, 8 or 9.
           - *parity* is the parity, ``None``, 0 (even) or 1 (odd).
@@ -1027,158 +913,116 @@
         On the WiPy only the following keyword-only parameter is supported:
 
           - *pins* is a 4 or 2 item list indicating the TX, RX, RTS and CTS pins (in that order).
             Any of the pins can be None if one wants the UART to operate with limited functionality.
             If the RTS pin is given the the RX pin must be given as well. The same applies to CTS.
             When no pins are given, then the default set of TX and RX pins is taken, and hardware
             flow control will be disabled. If *pins* is ``None``, no pin assignment will be made.
+
+        .. note::
+          It is possible to call ``init()`` multiple times on the same object in
+          order to reconfigure  UART on the fly. That allows using single UART
+          peripheral to serve different devices attached to different GPIO pins.
+          Only one device can be served at a time in that case.
+          Also do not call ``deinit()`` as it will prevent calling ``init()``
+          again.
         """
         ...
-
-    def sendbreak(self) -> None:
+    def flush(self) -> Any:
         """
-        Send a break condition on the bus. This drives the bus low for a duration
-        longer than required for a normal transmission of a character.
+        Waits until all data has been sent. In case of a timeout, an exception is raised. The timeout
+        duration depends on the tx buffer size and the baud rate. Unless flow control is enabled, a timeout
+        should not occur.
+
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call returns while the last byte is sent.
+            If required, a one character wait time has to be added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
         """
         ...
+    def txdone(self) -> bool:
+        """
+        Tells whether all data has been sent or no data transfer is happening. In this case,
+        it returns ``True``. If a data transmission is ongoing it returns ``False``.
 
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call may return ``True`` even if the last byte
+            of a transfer is still being sent. If required, a one character wait time has to be
+            added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
+        """
+        ...
     def read(self, nbytes: Optional[Any] = None) -> bytes:
         """
         Read characters.  If ``nbytes`` is specified then read at most that many bytes,
         otherwise read as much data as possible. It may return sooner if a timeout
         is reached. The timeout is configurable in the constructor.
 
         Return value: a bytes object containing the bytes read in.  Returns ``None``
         on timeout.
         """
         ...
-
     def any(self) -> int:
         """
         Returns an integer counting the number of characters that can be read without
         blocking.  It will return 0 if there are no characters available and a positive
         number if there are characters.  The method may return 1 even if there is more
         than one character available for reading.
 
         For more sophisticated querying of available characters use select.poll::
 
          poll = select.poll()
          poll.register(uart, select.POLLIN)
          poll.poll(timeout)
         """
         ...
-
     def write(self, buf) -> int:
         """
         Write the buffer of bytes to the bus.
 
         Return value: number of bytes written or ``None`` on timeout.
         """
         ...
-
     def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
         """
         Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
         that many bytes.  Otherwise, read at most ``len(buf)`` bytes. It may return sooner if a timeout
         is reached. The timeout is configurable in the constructor.
 
         Return value: number of bytes read and stored into ``buf`` or ``None`` on
         timeout.
         """
         ...
-
     def readline(self) -> None:
         """
         Read a line, ending in a newline character. It may return sooner if a timeout
         is reached. The timeout is configurable in the constructor.
 
         Return value: the line read or ``None`` on timeout.
         """
         ...
-
-    def __init__(self, id, *args, **kwargs) -> None:
-        ...
-
-
-mem16: Any  ## <class 'mem'> = <16-bit memory>
-
-
-class Signal:
-    """
-            Signal(pin_arguments..., *, invert=False)
-
-    Create a Signal object. There're two ways to create it:
-
-    * By wrapping existing Pin object - universal method which works for
-      any board.
-    * By passing required Pin parameters directly to Signal constructor,
-      skipping the need to create intermediate Pin object. Available on
-      many, but not all boards.
-
-    The arguments are:
-
-      - ``pin_obj`` is existing Pin object.
-
-      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
-
-      - ``invert`` - if True, the signal will be inverted (active low).
-    """
-
-    def off(self) -> None:
-        """
-        Deactivate signal.
-        """
-        ...
-
-    def on(self) -> None:
-        """
-        Activate signal.
-        """
-        ...
-
-    def value(self, x: Optional[Any] = None) -> int:
-        """
-        This method allows to set and get the value of the signal, depending on whether
-        the argument ``x`` is supplied or not.
-
-        If the argument is omitted then this method gets the signal level, 1 meaning
-        signal is asserted (active) and 0 - signal inactive.
-
-        If the argument is supplied then this method sets the signal level. The
-        argument ``x`` can be anything that converts to a boolean. If it converts
-        to ``True``, the signal is active, otherwise it is inactive.
-
-        Correspondence between signal being active and actual logic level on the
-        underlying pin depends on whether signal is inverted (active-low) or not.
-        For non-inverted signal, active status corresponds to logical 1, inactive -
-        to logical 0. For inverted/active-low signal, active status corresponds
-        to logical 0, while inactive - to logical 1.
-        """
-        ...
-
-    def __init__(self, pin_obj, *args, invert=False) -> None:
-        ...
-
+    def __init__(self, id, *args, **kwargs) -> None: ...
 
 class RTC:
     """
     Create an RTC object. See init for parameters of initialization.
     """
 
     def init(self, datetime) -> None:
         """
         Initialise the RTC. Datetime is a tuple of the form:
 
            ``(year, month, day[, hour[, minute[, second[, microsecond[, tzinfo]]]]])``
         """
         ...
-
-    def memory(self, *args, **kwargs) -> Any:
-        ...
-
+    def memory(self, *args, **kwargs) -> Any: ...
     def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
         """
         Get or set the date and time of the RTC.
 
         With no arguments, this method returns an 8-tuple with the current
         date and time.  With 1 argument (being an 8-tuple) it sets the date
         and time.
@@ -1186,18 +1030,43 @@
         The 8-tuple has the following format:
 
             (year, month, day, weekday, hours, minutes, seconds, subseconds)
 
         The meaning of the ``subseconds`` field is hardware dependent.
         """
         ...
+    def __init__(self, id=0, *args, **kwargs) -> None: ...
 
-    def __init__(self, id=0, *args, **kwargs) -> None:
-        ...
+class SoftI2C(I2C):
+    """
+    Construct a new software I2C object.  The parameters are:
+
+       - *scl* should be a pin object specifying the pin to use for SCL.
+       - *sda* should be a pin object specifying the pin to use for SDA.
+       - *freq* should be an integer which sets the maximum frequency
+         for SCL.
+       - *timeout* is the maximum time in microseconds to wait for clock
+         stretching (SCL held low by another device on the bus), after
+         which an ``OSError(ETIMEDOUT)`` exception is raised.
+    """
 
+    def readfrom_mem_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_mem(self, *args, **kwargs) -> Any: ...
+    def writeto_mem(self, *args, **kwargs) -> Any: ...
+    def scan(self, *args, **kwargs) -> Any: ...
+    def writeto(self, *args, **kwargs) -> Any: ...
+    def writevto(self, *args, **kwargs) -> Any: ...
+    def start(self, *args, **kwargs) -> Any: ...
+    def readfrom(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def stop(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None: ...
 
 class SDCard:
     """
     This class provides access to SD or MMC storage cards using either
     a dedicated SD/MMC interface hardware or through an SPI channel.
     The class implements the block protocol defined by :class:`os.AbstractBlockDev`.
     This allows the mounting of an SD card to be as simple as::
@@ -1222,54 +1091,40 @@
      - *mosi* can be used to specify an SPI mosi pin.
 
      - *cs* can be used to specify an SPI chip select pin.
 
      - *freq* selects the SD/MMC interface frequency in Hz (only supported on the ESP32).
     """
 
-    def ioctl(self, *args, **kwargs) -> Any:
-        ...
-
-    def readblocks(self, *args, **kwargs) -> Any:
-        ...
-
-    def writeblocks(self, *args, **kwargs) -> Any:
-        ...
-
-    def info(self, *args, **kwargs) -> Any:
-        ...
-
-    def deinit(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, slot=1, width=1, cd=None, wp=None, sck=None, miso=None, mosi=None, cs=None, freq=20000000) -> None:
-        ...
-
+    def ioctl(self, *args, **kwargs) -> Any: ...
+    def readblocks(self, *args, **kwargs) -> Any: ...
+    def writeblocks(self, *args, **kwargs) -> Any: ...
+    def info(self, *args, **kwargs) -> Any: ...
+    def deinit(self, *args, **kwargs) -> Any: ...
+    def __init__(self, slot=1, width=1, cd=None, wp=None, sck=None, miso=None, mosi=None, cs=None, freq=20000000) -> None: ...
 
 class SPI:
     """
     Construct an SPI object on the given bus, *id*. Values of *id* depend
     on a particular port and its hardware. Values 0, 1, etc. are commonly used
     to select hardware SPI block #0, #1, etc.
 
     With no additional parameters, the SPI object is created but not
     initialised (it has the settings from the last initialisation of
     the bus, if any).  If extra arguments are given, the bus is initialised.
     See ``init`` for parameters of initialisation.
     """
 
-    LSB = 1  # type: int
-    MSB = 0  # type: int
-
+    LSB: int
+    MSB: int
     def deinit(self) -> None:
         """
         Turn off the SPI bus.
         """
         ...
-
     def init(
         self, baudrate=1000000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None, pins: Optional[Tuple]
     ) -> None:
         """
         Initialise the SPI bus with the given parameters:
 
           - ``baudrate`` is the SCK clock rate.
@@ -1287,48 +1142,94 @@
             specify them as a tuple of ``pins`` parameter.
 
         In the case of hardware SPI the actual clock frequency may be lower than the
         requested baudrate. This is dependant on the platform hardware. The actual
         rate may be determined by printing the SPI object.
         """
         ...
-
     def write_readinto(self, write_buf, read_buf) -> int:
         """
         Write the bytes from ``write_buf`` while reading into ``read_buf``.  The
         buffers can be the same or different, but both buffers must have the
         same length.
         Returns ``None``.
 
         Note: on WiPy this function returns the number of bytes written.
         """
         ...
-
     def read(self, nbytes, write=0x00) -> bytes:
         """
         Read a number of bytes specified by ``nbytes`` while continuously writing
         the single byte given by ``write``.
         Returns a ``bytes`` object with the data that was read.
         """
         ...
-
     def write(self, buf) -> int:
         """
         Write the bytes contained in ``buf``.
         Returns ``None``.
 
         Note: on WiPy this function returns the number of bytes written.
         """
         ...
-
     def readinto(self, buf, write=0x00) -> int:
         """
         Read into the buffer specified by ``buf`` while continuously writing the
         single byte given by ``write``.
         Returns ``None``.
 
         Note: on WiPy this function returns the number of bytes read.
         """
         ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
 
-    def __init__(self, id, *args, **kwargs) -> None:
+class Signal(Pin):
+    """
+            Signal(pin_arguments..., *, invert=False)
+
+    Create a Signal object. There're two ways to create it:
+
+    * By wrapping existing Pin object - universal method which works for
+      any board.
+    * By passing required Pin parameters directly to Signal constructor,
+      skipping the need to create intermediate Pin object. Available on
+      many, but not all boards.
+
+    The arguments are:
+
+      - ``pin_obj`` is existing Pin object.
+
+      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
+
+      - ``invert`` - if True, the signal will be inverted (active low).
+    """
+
+    def off(self) -> None:
+        """
+        Deactivate signal.
+        """
+        ...
+    def on(self) -> None:
+        """
+        Activate signal.
+        """
+        ...
+    def value(self, x: Optional[Any] = None) -> int:
+        """
+        This method allows to set and get the value of the signal, depending on whether
+        the argument ``x`` is supplied or not.
+
+        If the argument is omitted then this method gets the signal level, 1 meaning
+        signal is asserted (active) and 0 - signal inactive.
+
+        If the argument is supplied then this method sets the signal level. The
+        argument ``x`` can be anything that converts to a boolean. If it converts
+        to ``True``, the signal is active, otherwise it is inactive.
+
+        Correspondence between signal being active and actual logic level on the
+        underlying pin depends on whether signal is inverted (active-low) or not.
+        For non-inverted signal, active status corresponds to logical 1, inactive -
+        to logical 0. For inverted/active-low signal, active status corresponds
+        to logical 0, while inactive - to logical 1.
+        """
         ...
+    def __init__(self, pin_obj, *args, invert=False) -> None: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/uos.py` & `micropython_esp32_s3_stubs-1.20.0.post1/uos.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 """
-basic "operating system" services. See: https://docs.micropython.org/en/v1.19.1/library/os.html
+basic "operating system" services. See: https://docs.micropython.org/en/v1.20.0/library/os.html
 
 |see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
 
 The ``os`` module contains functions for filesystem access and mounting,
 terminal redirection and duplication, and the ``uname`` and ``urandom``
 functions.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import IO, Iterator, Optional, Tuple, Any
 from stdlib.os import uname_result
 
-
 def stat(path) -> Any:
     """
     Get the status of a file or directory.
     """
     ...
 
-
 def rmdir(path) -> None:
     """
     Remove a directory.
     """
     ...
 
-
 def rename(old_path, new_path) -> None:
     """
     Rename a file.
     """
     ...
 
-
 def mount(fsobj, mount_point, *, readonly) -> Any:
     """
     Mount the filesystem object *fsobj* at the location in the VFS given by the
     *mount_point* string.  *fsobj* can be a a VFS object that has a ``mount()``
     method, or a block device.  If it's a block device then the filesystem type
     is automatically detected (an exception is raised if no filesystem was
     recognised).  *mount_point* may be ``'/'`` to mount *fsobj* at the root,
@@ -48,22 +42,20 @@
     During the mount process the method ``mount()`` is called on the filesystem
     object.
 
     Will raise ``OSError(EPERM)`` if *mount_point* is already mounted.
     """
     ...
 
-
 def mkdir(path) -> Any:
     """
     Create a new directory.
     """
     ...
 
-
 def statvfs(path) -> Tuple:
     """
     Get the status of a fileystem.
 
     Returns a tuple with the filesystem information in the following order:
 
          * ``f_bsize`` -- file system block size
@@ -79,60 +71,52 @@
 
     Parameters related to inodes: ``f_files``, ``f_ffree``, ``f_avail``
     and the ``f_flags`` parameter may return ``0`` as they can be unavailable
     in a port-specific implementation.
     """
     ...
 
-
-def unlink(*args, **kwargs) -> Any:
-    ...
-
-
+def unlink(*args, **kwargs) -> Any: ...
 def uname() -> uname_result:
     """
     Return a tuple (possibly a named tuple) containing information about the
     underlying machine and/or its operating system.  The tuple has five fields
     in the following order, each of them being a string:
 
          * ``sysname`` -- the name of the underlying system
          * ``nodename`` -- the network name (can be the same as ``sysname``)
          * ``release`` -- the version of the underlying system
          * ``version`` -- the MicroPython version and build date
          * ``machine`` -- an identifier for the underlying hardware (eg board, CPU)
     """
     ...
 
-
 def umount(mount_point) -> Any:
     """
     Unmount a filesystem. *mount_point* can be a string naming the mount location,
     or a previously-mounted filesystem object.  During the unmount process the
     method ``umount()`` is called on the filesystem object.
 
     Will raise ``OSError(EINVAL)`` if *mount_point* is not found.
     """
     ...
 
-
 def urandom(n) -> bytes:
     """
     Return a bytes object with *n* random bytes. Whenever possible, it is
     generated by the hardware random number generator.
     """
     ...
 
-
 def chdir(path) -> Any:
     """
     Change current directory.
     """
     ...
 
-
 def dupterm(stream_object, index=0, /) -> IO:
     """
     Duplicate or switch the MicroPython terminal (the REPL) on the given `stream`-like
     object. The *stream_object* argument must be a native stream object, or derive
     from ``io.IOBase`` and implement the ``readinto()`` and
     ``write()`` methods.  The stream should be in non-blocking mode and
     ``readinto()`` should return ``None`` if there is no data available for reading.
@@ -148,33 +132,27 @@
     If ``None`` is passed as the *stream_object* then duplication is cancelled on
     the slot given by *index*.
 
     The function returns the previous stream-like object in the given slot.
     """
     ...
 
-
 def remove(path) -> None:
     """
     Remove a file.
     """
     ...
 
-
 def listdir(dir: Optional[Any] = None) -> Any:
     """
     With no argument, list the current directory.  Otherwise list the given directory.
     """
     ...
 
-
-def dupterm_notify(*args, **kwargs) -> Any:
-    ...
-
-
+def dupterm_notify(*args, **kwargs) -> Any: ...
 def ilistdir(dir: Optional[Any] = None) -> Iterator[Tuple]:
     """
     This function returns an iterator which then yields tuples corresponding to
     the entries in the directory that it is listing.  With no argument it lists the
     current directory, otherwise it lists the directory given by *dir*.
 
     The tuples have the form *(name, type, inode[, size])*:
@@ -188,22 +166,20 @@
      - Some platforms may return a 4-tuple that includes the entry's *size*.  For
        file entries, *size* is an integer representing the size of the file
        or -1 if unknown.  Its meaning is currently undefined for directory
        entries.
     """
     ...
 
-
 def getcwd() -> Any:
     """
     Get the current directory.
     """
     ...
 
-
 class VfsLfs2:
     """
     Create a filesystem object that uses the `littlefs v2 filesystem format`_.
     Storage of the littlefs filesystem is provided by *block_dev*, which must
     support the :ref:`extended interface <block-device-interface>`.
     Objects created by this constructor can be mounted using :func:`mount`.
 
@@ -214,109 +190,56 @@
     timestamps will work without reformatting and timestamps will be added
     transparently to existing files once they are opened for writing.  When *mtime*
     is enabled `os.stat` on files without timestamps will return 0 for the timestamp.
 
     See :ref:`filesystem` for more information.
     """
 
-    def rename(self, *args, **kwargs) -> Any:
-        ...
-
+    def rename(self, *args, **kwargs) -> Any: ...
     @staticmethod
     def mkfs(block_dev, readsize=32, progsize=32, lookahead=32) -> None:
         """
             Build a Lfs2 filesystem on *block_dev*.
 
         ``Note:`` There are reports of littlefs v2 failing in certain situations,
                   for details see `littlefs issue 295`_.
         """
         ...
-
-    def mount(self, *args, **kwargs) -> Any:
-        ...
-
-    def statvfs(self, *args, **kwargs) -> Any:
-        ...
-
-    def rmdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def stat(self, *args, **kwargs) -> Any:
-        ...
-
-    def umount(self, *args, **kwargs) -> Any:
-        ...
-
-    def remove(self, *args, **kwargs) -> Any:
-        ...
-
-    def mkdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def open(self, *args, **kwargs) -> Any:
-        ...
-
-    def ilistdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def chdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def getcwd(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None:
-        ...
-
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None: ...
 
 class VfsFat:
     """
     Create a filesystem object that uses the FAT filesystem format.  Storage of
     the FAT filesystem is provided by *block_dev*.
     Objects created by this constructor can be mounted using :func:`mount`.
     """
 
-    def rename(self, *args, **kwargs) -> Any:
-        ...
-
+    def rename(self, *args, **kwargs) -> Any: ...
     @staticmethod
     def mkfs(block_dev) -> None:
         """
         Build a FAT filesystem on *block_dev*.
         """
         ...
-
-    def mount(self, *args, **kwargs) -> Any:
-        ...
-
-    def statvfs(self, *args, **kwargs) -> Any:
-        ...
-
-    def rmdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def stat(self, *args, **kwargs) -> Any:
-        ...
-
-    def umount(self, *args, **kwargs) -> Any:
-        ...
-
-    def remove(self, *args, **kwargs) -> Any:
-        ...
-
-    def mkdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def open(self, *args, **kwargs) -> Any:
-        ...
-
-    def ilistdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def chdir(self, *args, **kwargs) -> Any:
-        ...
-
-    def getcwd(self, *args, **kwargs) -> Any:
-        ...
-
-    def __init__(self, block_dev) -> None:
-        ...
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev) -> None: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/urandom.py` & `micropython_esp32_s3_stubs-1.20.0.post1/urandom.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-random numbers. See: https://docs.micropython.org/en/v1.19.1/library/random.html
+random numbers. See: https://docs.micropython.org/en/v1.20.0/library/random.html
 
 This module implements a pseudo-random number generator (PRNG).
 
 |see_cpython_module| :mod:`python:random` https://docs.python.org/3/library/random.html . .
 
 .. note::
 
@@ -21,75 +21,65 @@
 .. note::
 
    The :func:`randrange`, :func:`randint` and :func:`choice` functions are only
    available if the ``MICROPY_PY_URANDOM_EXTRA_FUNCS`` configuration option is
    enabled.
 
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Any
 
-
 def randrange(start, stop, step: Optional[Any] = None) -> int:
     """
     The first form returns a random integer from the range [0, *stop*).
     The second form returns a random integer from the range [*start*, *stop*).
     The third form returns a random integer from the range [*start*, *stop*) in
     steps of *step*.  For instance, calling ``randrange(1, 10, 2)`` will
     return odd numbers between 1 and 9 inclusive.
 
     """
     ...
 
-
 class random:
     """
     Return a random floating point number in the range [0.0, 1.0).
     """
 
-    def __init__(self) -> None:
-        ...
-
+    def __init__(self) -> None: ...
 
 def seed(n=None, /) -> None:
     """
     Initialise the random number generator module with the seed *n* which should
     be an integer.  When no argument (or ``None``) is passed in it will (if
     supported by the port) initialise the PRNG with a true random number
     (usually a hardware generated random number).
 
     The ``None`` case only works if ``MICROPY_PY_URANDOM_SEED_INIT_FUNC`` is
     enabled by the port, otherwise it raises ``ValueError``.
     """
     ...
 
-
 def uniform(a, b) -> int:
     """
     Return a random floating point number N such that *a* <= N <= *b* for *a* <= *b*,
     and *b* <= N <= *a* for *b* < *a*.
 
     """
     ...
 
-
 def choice(sequence) -> Any:
     """
     Chooses and returns one item at random from *sequence* (tuple, list or
     any object that supports the subscript operation).
     """
     ...
 
-
 def randint(a, b) -> int:
     """
     Return a random integer in the range [*a*, *b*].
     """
     ...
 
-
 def getrandbits(n) -> int:
     """
     Return an integer with *n* random bits (0 <= n <= 32).
     """
     ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/uselect.py` & `micropython_esp32_s3_stubs-1.20.0.post1/uselect.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 """
-wait for events on a set of streams. See: https://docs.micropython.org/en/v1.19.1/library/select.html
+wait for events on a set of streams. See: https://docs.micropython.org/en/v1.20.0/library/select.html
 
 |see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
 
 This module provides functions to efficiently wait for events on multiple
 `streams <stream>` (select streams which are ready for operations).
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Iterator, List, Optional, Tuple, Any
 
-POLLOUT = 4  # type: int
-POLLIN = 1  # type: int
-POLLHUP = 16  # type: int
-POLLERR = 8  # type: int
-
+POLLOUT: int
+POLLIN: int
+POLLHUP: int
+POLLERR: int
 
 class select:
     """
     Wait for activity on a set of objects.
 
     This function is provided by some MicroPython ports for compatibility
     and is not efficient. Usage of :class:`Poll` is recommended instead.
     """
 
-    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None:
-        ...
-
+    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None: ...
 
 class poll:
     """
     Create an instance of the Poll class.
     """
 
-    def __init__(self) -> None:
-        ...
-
+    def __init__(self) -> None: ...
     def register(self, obj, eventmask: Optional[Any] = None) -> None:
         """
         Register `stream` *obj* for polling. *eventmask* is logical OR of:
 
         * ``select.POLLIN``  - data available for reading
         * ``select.POLLOUT`` - more data can be written
 
@@ -51,28 +44,25 @@
         *eventmask* defaults to ``select.POLLIN | select.POLLOUT``.
 
         It is OK to call this function multiple times for the same *obj*.
         Successive calls will update *obj*'s eventmask to the value of
         *eventmask* (i.e. will behave as `modify()`).
         """
         ...
-
     def unregister(self, obj) -> Any:
         """
         Unregister *obj* from polling.
         """
         ...
-
     def modify(self, obj, eventmask) -> None:
         """
         Modify the *eventmask* for *obj*. If *obj* is not registered, `OSError`
         is raised with error of ENOENT.
         """
         ...
-
     def poll(self, timeout=-1, /) -> List:
         """
         Wait for at least one of the registered objects to become ready or have an
         exceptional condition, with optional timeout in milliseconds (if *timeout*
         arg is not specified or -1, there is no timeout).
 
         Returns list of (``obj``, ``event``, ...) tuples. There may be other elements in
@@ -84,15 +74,14 @@
         corresponding stream unregistered from poll and likely closed), because
         otherwise all further invocations of `poll()` may return immediately with
         these flags set for this stream again.
 
         In case of timeout, an empty list is returned.
         """
         ...
-
     def ipoll(self, timeout=-1, flags=0, /) -> Iterator[Tuple]:
         """
         Like :meth:`poll.poll`, but instead returns an iterator which yields a
         `callee-owned tuple`. This function provides an efficient, allocation-free
         way to poll on streams.
 
         If *flags* is 1, one-shot behaviour for events is employed: streams for
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/usocket.py` & `micropython_esp32_s3_stubs-1.20.0.post1/usocket.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """
-socket module. See: https://docs.micropython.org/en/v1.19.1/library/socket.html
+socket module. See: https://docs.micropython.org/en/v1.20.0/library/socket.html
 
 |see_cpython_module| :mod:`python:socket` https://docs.python.org/3/library/socket.html .
 
 This module provides access to the BSD socket interface.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import IO, Optional, Tuple, Any
 
-SOCK_RAW = 3  # type: int
-SOCK_DGRAM = 2  # type: int
-IP_ADD_MEMBERSHIP = 3  # type: int
-SOCK_STREAM = 1  # type: int
-SOL_SOCKET = 4095  # type: int
-SO_REUSEADDR = 4  # type: int
-AF_INET6 = 10  # type: int
-AF_INET = 2  # type: int
-IPPROTO_UDP = 17  # type: int
-IPPROTO_IP = 0  # type: int
-IPPROTO_TCP = 6  # type: int
-
+SOCK_RAW: int
+SOCK_DGRAM: int
+IP_ADD_MEMBERSHIP: int
+SOCK_STREAM: int
+SOL_SOCKET: int
+SO_REUSEADDR: int
+AF_INET6: int
+AF_INET: int
+IPPROTO_UDP: int
+IPPROTO_IP: int
+IPPROTO_TCP: int
 
 def getaddrinfo(host, port, af=0, type=0, proto=0, flags=0, /) -> Any:
     """
     Translate the host/port argument into a sequence of 5-tuples that contain all the
     necessary arguments for creating a socket connected to that service. Arguments
     *af*, *type*, and *proto* (which have the same meaning as for the `socket()` function)
     can be used to filter which kind of addresses are returned. If a parameter is not
@@ -47,15 +44,14 @@
        s = socket.socket()
        # Guaranteed to return an address which can be connect'ed to for
        # stream operation.
        s.connect(socket.getaddrinfo('www.micropython.org', 80, 0, SOCK_STREAM)[0][-1])
     """
     ...
 
-
 class socket:
     """
     Create a new socket using the given address family, socket type and
     protocol number. Note that specifying *proto* in most cases is not
     required (and not recommended, as some MicroPython ports may omit
     ``IPPROTO_*`` constants). Instead, *type* argument will select needed
     protocol automatically::
@@ -69,82 +65,72 @@
     def recvfrom(self, bufsize) -> Tuple:
         """
         Receive data from the socket. The return value is a pair *(bytes, address)* where *bytes* is a
         bytes object representing the data received and *address* is the address of the socket sending
         the data.
         """
         ...
-
     def recv(self, bufsize) -> bytes:
         """
         Receive data from the socket. The return value is a bytes object representing the data
         received. The maximum amount of data to be received at once is specified by bufsize.
         """
         ...
-
     def makefile(self, mode="rb", buffering=0, /) -> IO:
         """
         Return a file object associated with the socket. The exact returned type depends on the arguments
         given to makefile(). The support is limited to binary modes only ('rb', 'wb', and 'rwb').
         CPython's arguments: *encoding*, *errors* and *newline* are not supported.
         """
         ...
-
     def listen(self, backlog: Optional[Any] = None) -> None:
         """
         Enable a server to accept connections. If *backlog* is specified, it must be at least 0
         (if it's lower, it will be set to 0); and specifies the number of unaccepted connections
         that the system will allow before refusing new connections. If not specified, a default
         reasonable value is chosen.
         """
         ...
-
-    def fileno(self, *args, **kwargs) -> Any:
-        ...
-
+    def fileno(self, *args, **kwargs) -> Any: ...
     def sendall(self, bytes) -> int:
         """
         Send all data to the socket. The socket must be connected to a remote socket.
         Unlike `send()`, this method will try to send all of data, by sending data
         chunk by chunk consecutively.
 
         The behaviour of this method on non-blocking sockets is undefined. Due to this,
         on MicroPython, it's recommended to use `write()` method instead, which
         has the same "no short writes" policy for blocking sockets, and will return
         number of bytes sent on non-blocking sockets.
         """
         ...
-
     def setsockopt(self, level, optname, value) -> None:
         """
         Set the value of the given socket option. The needed symbolic constants are defined in the
         socket module (SO_* etc.). The *value* can be an integer or a bytes-like object representing
         a buffer.
         """
         ...
-
     def setblocking(self, flag) -> Any:
         """
         Set blocking or non-blocking mode of the socket: if flag is false, the socket is set to non-blocking,
         else to blocking mode.
 
         This method is a shorthand for certain `settimeout()` calls:
 
         * ``sock.setblocking(True)`` is equivalent to ``sock.settimeout(None)``
         * ``sock.setblocking(False)`` is equivalent to ``sock.settimeout(0)``
         """
         ...
-
     def sendto(self, bytes, address) -> None:
         """
         Send data to the socket. The socket should not be connected to a remote socket, since the
         destination socket is specified by *address*.
         """
         ...
-
     def settimeout(self, value) -> Any:
         """
         **Note**: Not every port supports this method, see below.
 
         Set a timeout on blocking socket operations. The value argument can be a nonnegative floating
         point number expressing seconds, or None. If a non-zero value is given, subsequent socket operations
         will raise an `OSError` exception if the timeout period value has elapsed before the operation has
@@ -164,89 +150,78 @@
              poller = select.poll()
              poller.register(s, select.POLLIN)
              res = poller.poll(1000)  # time in milliseconds
              if not res:
                  # s is still not ready for input, i.e. operation timed out
         """
         ...
-
     def readline(self) -> Any:
         """
         Read a line, ending in a newline character.
 
         Return value: the line read.
         """
         ...
-
     def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
         """
         Read bytes into the *buf*.  If *nbytes* is specified then read at most
         that many bytes.  Otherwise, read at most *len(buf)* bytes. Just as
         `read()`, this method follows "no short reads" policy.
 
         Return value: number of bytes read and stored into *buf*.
         """
         ...
-
     def read(self, size: Optional[Any] = None) -> bytes:
         """
         Read up to size bytes from the socket. Return a bytes object. If *size* is not given, it
         reads all data available from the socket until EOF; as such the method will not return until
         the socket is closed. This function tries to read as much data as
         requested (no "short reads"). This may be not possible with
         non-blocking socket though, and then less data will be returned.
         """
         ...
-
     def close(self) -> Any:
         """
         Mark the socket closed and release all resources. Once that happens, all future operations
         on the socket object will fail. The remote end will receive EOF indication if
         supported by protocol.
 
         Sockets are automatically closed when they are garbage-collected, but it is recommended
         to `close()` them explicitly as soon you finished working with them.
         """
         ...
-
     def connect(self, address) -> None:
         """
         Connect to a remote socket at *address*.
         """
         ...
-
     def send(self, bytes) -> int:
         """
         Send data to the socket. The socket must be connected to a remote socket.
         Returns number of bytes sent, which may be smaller than the length of data
         ("short write").
         """
         ...
-
     def bind(self, address) -> Any:
         """
         Bind the socket to *address*. The socket must not already be bound.
         """
         ...
-
     def accept(self) -> Tuple:
         """
         Accept a connection. The socket must be bound to an address and listening for connections.
         The return value is a pair (conn, address) where conn is a new socket object usable to send
         and receive data on the connection, and address is the address bound to the socket on the
         other end of the connection.
         """
         ...
-
     def write(self, buf) -> int:
         """
         Write the buffer of bytes to the socket. This function will try to
         write all data to a socket (no "short writes"). This may be not possible
         with a non-blocking socket though, and returned value will be less than
         the length of *buf*.
 
         Return value: number of bytes written.
         """
         ...
-
-    def __init__(self, af=AF_INET, type=SOCK_STREAM, proto=IPPROTO_TCP, /) -> None:
-        ...
+    def __init__(self, af=AF_INET, type=SOCK_STREAM, proto=IPPROTO_TCP, /) -> None: ...
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/utime.py` & `micropython_esp32_s3_stubs-1.20.0.post1/utime.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
-time related functions. See: https://docs.micropython.org/en/v1.19.1/library/time.html
+time related functions. See: https://docs.micropython.org/en/v1.20.0/library/time.html
 
 |see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
 
 The ``time`` module provides functions for getting the current time and date,
 measuring time intervals, and for delays.
 
 **Time Epoch**: Unix port uses standard for POSIX systems epoch of
-1970-01-01 00:00:00 UTC. However, embedded ports use epoch of
-2000-01-01 00:00:00 UTC.
+1970-01-01 00:00:00 UTC. However, some embedded ports use epoch of
+2000-01-01 00:00:00 UTC. Epoch year may be determined with ``gmtime(0)[0]``.
 
 **Maintaining actual calendar date/time**: This requires a
 Real Time Clock (RTC). On systems with underlying OS (including some
 RTOS), an RTC may be implicit. Setting and maintaining actual calendar
 time is responsibility of OS/RTOS and is done outside of MicroPython,
 it just uses OS API to query date/time. On baremetal ports however
 system time depends on ``machine.RTC()`` object. The current calendar time
@@ -26,19 +26,16 @@
   RTC time across hard resets, though some may require setting it again
   in such case).
 
 If actual calendar time is not maintained with a system/MicroPython RTC,
 functions below which require reference to current absolute time may
 behave not as expected.
 """
-# MCU: {'ver': 'v1.19.1', 'build': '', 'platform': 'esp32', 'port': 'esp32', 'machine': 'ESP32S3 module with ESP32S3', 'release': '1.19.1', 'nodename': 'esp32', 'name': 'micropython', 'family': 'micropython', 'sysname': 'esp32', 'version': '1.19.1'}
-# Stubber: 1.11.2
 from typing import Optional, Tuple, Any
 
-
 def ticks_diff(ticks1, ticks2) -> int:
     """
     Measure ticks difference between values returned from `ticks_ms()`, `ticks_us()`,
     or `ticks_cpu()` functions, as a signed value which may wrap around.
 
     The argument order is the same as for subtraction
     operator, ``ticks_diff(ticks1, ticks2)`` has the same meaning as ``ticks1 - ticks2``.
@@ -98,15 +95,14 @@
     Note: Do not pass `time()` values to `ticks_diff()`, you should use
     normal mathematical operations on them. But note that `time()` may (and will)
     also overflow. This is known as https://en.wikipedia.org/wiki/Year_2038_problem .
 
     """
     ...
 
-
 def ticks_add(ticks, delta) -> Any:
     """
     Offset ticks value by a given number, which can be either positive or negative.
     Given a *ticks* value, this function allows to calculate ticks value *delta*
     ticks before or after it, following modular-arithmetic definition of tick values
     (see `ticks_ms()` above). *ticks* parameter must be a direct result of call
     to `ticks_ms()`, `ticks_us()`, or `ticks_cpu()` functions (or from previous
@@ -127,15 +123,14 @@
 
          # Find out TICKS_MAX used by this port
          print(ticks_add(0, -1))
 
     """
     ...
 
-
 def ticks_cpu() -> Any:
     """
     Similar to `ticks_ms()` and `ticks_us()`, but with the highest possible resolution
     in the system. This is usually CPU clocks, and that's why the function is named that
     way. But it doesn't have to be a CPU clock, some other timing source available in a
     system (e.g. high-resolution timer) can be used instead. The exact timing unit
     (resolution) of this function is not specified on ``time`` module level, but
@@ -144,31 +139,28 @@
     Avoid using it in portable code.
 
     Availability: Not every port implements this function.
 
     """
     ...
 
-
 class time:
     """
     Returns the number of seconds, as an integer, since the Epoch, assuming that
     underlying RTC is set and maintained as described above. If an RTC is not set, this
     function returns number of seconds since a port-specific reference point in time (for
     embedded boards without a battery-backed RTC, usually since power up or reset). If you
     want to develop portable MicroPython application, you should not rely on this function
     to provide higher than second precision.  If you need higher precision, absolute
     timestamps, use `time_ns()`.  If relative times are acceptable then use the
     `ticks_ms()` and `ticks_us()` functions.  If you need calendar time, `gmtime()` or
     `localtime()` without an argument is a better choice.
     """
 
-    def __init__(self) -> None:
-        ...
-
+    def __init__(self) -> None: ...
 
 def ticks_ms() -> int:
     """
     Returns an increasing millisecond counter with an arbitrary reference point, that
     wraps around after some value.
 
     The wrap-around value is not explicitly exposed, but we will
@@ -186,30 +178,27 @@
     operators (<, <=, >, >=) directly on these value will lead to invalid
     result. Performing mathematical operations and then passing their results
     as arguments to `ticks_diff()` or `ticks_add()` will also lead to
     invalid results from the latter functions.
     """
     ...
 
-
 def ticks_us() -> Any:
     """
     Just like `ticks_ms()` above, but in microseconds.
     """
     ...
 
-
 def time_ns() -> int:
     """
     Similar to `time()` but returns nanoseconds since the Epoch, as an integer (usually
     a big integer, so will allocate on the heap).
     """
     ...
 
-
 def localtime(secs: Optional[Any] = None) -> Tuple:
     """
     Convert the time *secs* expressed in seconds since the Epoch (see above) into an
     8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
     If *secs* is not provided or None, then the current time from the RTC is used.
 
     The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
@@ -224,26 +213,24 @@
     * minute  is 0-59
     * second  is 0-59
     * weekday is 0-6 for Mon-Sun
     * yearday is 1-366
     """
     ...
 
-
 def sleep_us(us) -> None:
     """
     Delay for given number of microseconds, should be positive or 0.
 
     This function attempts to provide an accurate delay of at least *us*
     microseconds, but it may take longer if the system has other higher priority
     processing to perform.
     """
     ...
 
-
 def gmtime(secs: Optional[Any] = None) -> Tuple:
     """
     Convert the time *secs* expressed in seconds since the Epoch (see above) into an
     8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
     If *secs* is not provided or None, then the current time from the RTC is used.
 
     The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
@@ -258,36 +245,33 @@
     * minute  is 0-59
     * second  is 0-59
     * weekday is 0-6 for Mon-Sun
     * yearday is 1-366
     """
     ...
 
-
 def sleep_ms(ms) -> None:
     """
     Delay for given number of milliseconds, should be positive or 0.
 
     This function will delay for at least the given number of milliseconds, but
     may take longer than that if other processing must take place, for example
     interrupt handlers or other threads.  Passing in 0 for *ms* will still allow
     this other processing to occur.  Use `sleep_us()` for more precise delays.
     """
     ...
 
-
 def mktime() -> int:
     """
     This is inverse function of localtime. It's argument is a full 8-tuple
     which expresses a time as per localtime. It returns an integer which is
     the number of seconds since Jan 1, 2000.
     """
     ...
 
-
 def sleep(seconds) -> Any:
     """
     Sleep for the given number of seconds. Some boards may accept *seconds* as a
     floating-point number to sleep for a fractional number of seconds. Note that
     other boards may not accept a floating-point argument, for compatibility with
     them use `sleep_ms()` and `sleep_us()` functions.
     """
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/setup.py` & `micropython_esp32_s3_stubs-1.20.0.post1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,102 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
-['micropython', 'micropython_']
+['_boot',
+ '_onewire',
+ '_thread',
+ '_uasyncio',
+ 'apa106',
+ 'array',
+ 'binascii',
+ 'bluetooth',
+ 'btree',
+ 'cmath',
+ 'collections',
+ 'cryptolib',
+ 'dht',
+ 'ds18x20',
+ 'errno',
+ 'esp',
+ 'esp32',
+ 'flashbdev',
+ 'framebuf',
+ 'gc',
+ 'hashlib',
+ 'heapq',
+ 'inisetup',
+ 'io',
+ 'json',
+ 'machine',
+ 'math',
+ 'micropython',
+ 'micropython_',
+ '__init__',
+ 'mip',
+ 'neopixel',
+ 'network',
+ 'ntptime',
+ 'onewire',
+ 'os',
+ 'platform',
+ 'random',
+ 'select',
+ 'socket',
+ 'ssl',
+ 'struct',
+ 'sys',
+ 'time',
+ 'uarray',
+ 'core',
+ 'event',
+ 'funcs',
+ 'lock',
+ 'stream',
+ 'task',
+ 'ubinascii',
+ 'ubluetooth',
+ 'ucollections',
+ 'ucryptolib',
+ 'uctypes',
+ 'uerrno',
+ 'uhashlib',
+ 'uheapq',
+ 'uio',
+ 'ujson',
+ 'umachine',
+ 'robust',
+ 'simple',
+ 'uos',
+ 'uplatform',
+ 'upysh',
+ 'urandom',
+ 'ure',
+ 'urequests',
+ 'uselect',
+ 'usocket',
+ 'ussl',
+ 'ustruct',
+ 'usys',
+ 'utime',
+ 'utimeq',
+ 'uwebsocket',
+ 'uzlib',
+ 'webrepl',
+ 'webrepl_setup',
+ 'websocket',
+ 'zlib']
 install_requires = \
 ['micropython-stdlib-stubs>=0.9.0']
 
 setup_kwargs = {
     'name': 'micropython-esp32-s3-stubs',
-    'version': '1.19.1.post1',
+    'version': '1.20.0.post1',
     'description': 'MicroPython stubs',
-    'long_description': '# micropython-esp32-s3-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* Merged stubs from `stubs/micropython-v1_19_1-esp32-s3-merged`\n* Frozen stubs from `stubs/micropython-v1_19_1-frozen/esp32/GENERIC`\n* Core stubs from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nFirmware | micropython | esp32 | ESP32S3 module with ESP32S3 | v1.19.1 \nDocumentation | micropython | - | - | v1.19.1 \nCore | micropython | esp32 | - | v1.19.1 \n',
+    'long_description': '# micropython-esp32-s3-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* Merged stubs from `stubs/micropython-v1_20_0-esp32-s3-merged`\n* Frozen stubs from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`\n* Core stubs from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nDocumentation | micropython | - | - | v1.20.0 \nCore | micropython | esp32 | - | v1.20.0 \n',
     'author': 'josverl',
     'author_email': 'josverl@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josverl/micropython-stubs#micropython-stubs',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `micropython_esp32_s3_stubs-1.19.1.post1/PKG-INFO` & `micropython_esp32_s3_stubs-1.20.0.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-esp32-s3-stubs
-Version: 1.19.1.post1
+Version: 1.20.0.post1
 Summary: MicroPython stubs
 Home-page: https://github.com/josverl/micropython-stubs#micropython-stubs
 License: MIT
 Author: josverl
 Author-email: josverl@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -52,18 +52,17 @@
 
 If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
 
 For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
  * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
 
 Included stubs:
-* Merged stubs from `stubs/micropython-v1_19_1-esp32-s3-merged`
-* Frozen stubs from `stubs/micropython-v1_19_1-frozen/esp32/GENERIC`
+* Merged stubs from `stubs/micropython-v1_20_0-esp32-s3-merged`
+* Frozen stubs from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`
 * Core stubs from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
-Firmware | micropython | esp32 | ESP32S3 module with ESP32S3 | v1.19.1 
-Documentation | micropython | - | - | v1.19.1 
-Core | micropython | esp32 | - | v1.19.1 
+Documentation | micropython | - | - | v1.20.0 
+Core | micropython | esp32 | - | v1.20.0
```

