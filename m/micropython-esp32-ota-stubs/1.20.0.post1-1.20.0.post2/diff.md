# Comparing `tmp/micropython_esp32_ota_stubs-1.20.0.post1.tar.gz` & `tmp/micropython_esp32_ota_stubs-1.20.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_esp32_ota_stubs-1.20.0.post1.tar", max compression
+gzip compressed data, was "micropython_esp32_ota_stubs-1.20.0.post2.tar", max compression
```

## Comparing `micropython_esp32_ota_stubs-1.20.0.post1.tar` & `micropython_esp32_ota_stubs-1.20.0.post2.tar`

### file list

```diff
@@ -1,90 +1,91 @@
--rw-r--r--   0        0        0       53 2023-05-05 19:49:06.160838 micropython_esp32_ota_stubs-1.20.0.post1/_boot.pyi
--rw-r--r--   0        0        0      277 2023-05-05 19:29:15.108909 micropython_esp32_ota_stubs-1.20.0.post1/_onewire.pyi
--rw-r--r--   0        0        0      848 2023-05-05 19:55:29.203712 micropython_esp32_ota_stubs-1.20.0.post1/_thread.pyi
--rw-r--r--   0        0        0      364 2023-05-05 19:29:15.115217 micropython_esp32_ota_stubs-1.20.0.post1/_uasyncio.pyi
--rw-r--r--   0        0        0      115 2023-05-05 19:49:06.163754 micropython_esp32_ota_stubs-1.20.0.post1/apa106.pyi
--rw-r--r--   0        0        0     1003 2023-05-05 19:55:53.726818 micropython_esp32_ota_stubs-1.20.0.post1/array.pyi
--rw-r--r--   0        0        0     1408 2023-05-05 19:55:53.766054 micropython_esp32_ota_stubs-1.20.0.post1/binascii.pyi
--rw-r--r--   0        0        0    31291 2023-05-05 19:55:53.881702 micropython_esp32_ota_stubs-1.20.0.post1/bluetooth.pyi
--rw-r--r--   0        0        0     3837 2023-05-05 19:55:30.722831 micropython_esp32_ota_stubs-1.20.0.post1/btree.pyi
--rw-r--r--   0        0        0     1454 2023-05-05 19:55:53.786396 micropython_esp32_ota_stubs-1.20.0.post1/cmath.pyi
--rw-r--r--   0        0        0     3640 2023-05-05 19:55:53.819131 micropython_esp32_ota_stubs-1.20.0.post1/collections.pyi
--rw-r--r--   0        0        0     1647 2023-05-05 19:55:31.654886 micropython_esp32_ota_stubs-1.20.0.post1/cryptolib.pyi
--rw-r--r--   0        0        0      344 2023-05-05 19:49:06.167790 micropython_esp32_ota_stubs-1.20.0.post1/dht.pyi
--rw-r--r--   0        0        0      404 2023-05-05 19:49:06.170625 micropython_esp32_ota_stubs-1.20.0.post1/ds18x20.pyi
--rw-r--r--   0        0        0      709 2023-05-05 19:55:31.924993 micropython_esp32_ota_stubs-1.20.0.post1/errno.pyi
--rw-r--r--   0        0        0     1703 2023-05-05 19:55:53.848088 micropython_esp32_ota_stubs-1.20.0.post1/esp.pyi
--rw-r--r--   0        0        0    12242 2023-05-05 19:55:54.054643 micropython_esp32_ota_stubs-1.20.0.post1/esp32.pyi
--rw-r--r--   0        0        0       54 2023-05-05 19:49:06.172981 micropython_esp32_ota_stubs-1.20.0.post1/flashbdev.pyi
--rw-r--r--   0        0        0     6349 2023-05-05 19:55:53.948229 micropython_esp32_ota_stubs-1.20.0.post1/framebuf.pyi
--rw-r--r--   0        0        0     1993 2023-05-05 19:55:53.910702 micropython_esp32_ota_stubs-1.20.0.post1/gc.pyi
--rw-r--r--   0        0        0     1642 2023-05-05 19:55:53.980843 micropython_esp32_ota_stubs-1.20.0.post1/hashlib.pyi
--rw-r--r--   0        0        0      930 2023-05-05 19:55:53.980843 micropython_esp32_ota_stubs-1.20.0.post1/heapq.pyi
--rw-r--r--   0        0        0       77 2023-05-05 19:49:06.175994 micropython_esp32_ota_stubs-1.20.0.post1/inisetup.pyi
--rw-r--r--   0        0        0     2650 2023-05-05 19:55:54.103346 micropython_esp32_ota_stubs-1.20.0.post1/io.pyi
--rw-r--r--   0        0        0     1384 2023-05-05 19:55:54.037967 micropython_esp32_ota_stubs-1.20.0.post1/json.pyi
--rw-r--r--   0        0        0     1092 2023-05-05 20:31:26.121573 micropython_esp32_ota_stubs-1.20.0.post1/LICENSE.md
--rw-r--r--   0        0        0      827 2023-05-05 19:29:15.207207 micropython_esp32_ota_stubs-1.20.0.post1/logging.pyi
--rw-r--r--   0        0        0    52352 2023-05-05 19:55:58.620980 micropython_esp32_ota_stubs-1.20.0.post1/machine.pyi
--rw-r--r--   0        0        0     4654 2023-05-05 19:55:54.241564 micropython_esp32_ota_stubs-1.20.0.post1/math.pyi
--rw-r--r--   0        0        0     7213 2023-04-05 11:07:45.360315 micropython_esp32_ota_stubs-1.20.0.post1/micropython.pyi
--rw-r--r--   0        0        0      598 2023-05-05 19:51:58.147437 micropython_esp32_ota_stubs-1.20.0.post1/mip/__init__.pyi
--rw-r--r--   0        0        0       68 2023-05-05 19:29:15.223246 micropython_esp32_ota_stubs-1.20.0.post1/mip.pyi
--rw-r--r--   0        0        0      448 2023-05-05 19:49:06.179674 micropython_esp32_ota_stubs-1.20.0.post1/neopixel.pyi
--rw-r--r--   0        0        0    10529 2023-05-05 19:55:54.331396 micropython_esp32_ota_stubs-1.20.0.post1/network.pyi
--rw-r--r--   0        0        0       72 2023-05-05 19:49:06.185571 micropython_esp32_ota_stubs-1.20.0.post1/ntptime.pyi
--rw-r--r--   0        0        0      617 2023-05-05 19:49:06.192533 micropython_esp32_ota_stubs-1.20.0.post1/onewire.pyi
--rw-r--r--   0        0        0     9356 2023-05-05 19:55:54.405133 micropython_esp32_ota_stubs-1.20.0.post1/os.pyi
--rw-r--r--   0        0        0      162 2023-05-05 19:29:15.244098 micropython_esp32_ota_stubs-1.20.0.post1/platform.pyi
--rw-r--r--   0        0        0     4038 2023-05-05 20:31:28.094880 micropython_esp32_ota_stubs-1.20.0.post1/pyproject.toml
--rw-r--r--   0        0        0     2638 2023-05-05 19:55:54.364274 micropython_esp32_ota_stubs-1.20.0.post1/random.pyi
--rw-r--r--   0        0        0     2019 2023-05-05 20:31:26.121573 micropython_esp32_ota_stubs-1.20.0.post1/README.md
--rw-r--r--   0        0        0     3853 2023-05-05 19:55:40.631481 micropython_esp32_ota_stubs-1.20.0.post1/select.pyi
--rw-r--r--   0        0        0     9602 2023-05-05 19:55:54.485401 micropython_esp32_ota_stubs-1.20.0.post1/socket.pyi
--rw-r--r--   0        0        0     2668 2023-05-05 19:55:54.426100 micropython_esp32_ota_stubs-1.20.0.post1/ssl.pyi
--rw-r--r--   0        0        0     4241 2023-05-05 19:55:54.445545 micropython_esp32_ota_stubs-1.20.0.post1/struct.pyi
--rw-r--r--   0        0        0      875 2023-05-05 19:55:54.509858 micropython_esp32_ota_stubs-1.20.0.post1/sys.pyi
--rw-r--r--   0        0        0    12515 2023-05-05 19:55:54.501830 micropython_esp32_ota_stubs-1.20.0.post1/time.pyi
--rw-r--r--   0        0        0     1003 2023-05-05 19:55:54.501830 micropython_esp32_ota_stubs-1.20.0.post1/uarray.pyi
--rw-r--r--   0        0        0      132 2023-05-05 19:49:06.046649 micropython_esp32_ota_stubs-1.20.0.post1/uasyncio/__init__.pyi
--rw-r--r--   0        0        0     1530 2023-05-05 19:49:06.047659 micropython_esp32_ota_stubs-1.20.0.post1/uasyncio/core.pyi
--rw-r--r--   0        0        0      625 2023-05-05 19:49:06.055187 micropython_esp32_ota_stubs-1.20.0.post1/uasyncio/event.pyi
--rw-r--r--   0        0        0      390 2023-05-05 19:49:06.060787 micropython_esp32_ota_stubs-1.20.0.post1/uasyncio/funcs.pyi
--rw-r--r--   0        0        0      414 2023-05-05 19:49:06.060787 micropython_esp32_ota_stubs-1.20.0.post1/uasyncio/lock.pyi
--rw-r--r--   0        0        0     1410 2023-05-05 19:51:58.349367 micropython_esp32_ota_stubs-1.20.0.post1/uasyncio/stream.pyi
--rw-r--r--   0        0        0      789 2023-05-05 19:49:06.084965 micropython_esp32_ota_stubs-1.20.0.post1/uasyncio/task.pyi
--rw-r--r--   0        0        0     1408 2023-05-05 19:55:54.543869 micropython_esp32_ota_stubs-1.20.0.post1/ubinascii.pyi
--rw-r--r--   0        0        0    31291 2023-05-05 19:55:54.721985 micropython_esp32_ota_stubs-1.20.0.post1/ubluetooth.pyi
--rw-r--r--   0        0        0     3640 2023-05-05 19:55:54.597670 micropython_esp32_ota_stubs-1.20.0.post1/ucollections.pyi
--rw-r--r--   0        0        0     1647 2023-05-05 19:55:44.095712 micropython_esp32_ota_stubs-1.20.0.post1/ucryptolib.pyi
--rw-r--r--   0        0        0     2363 2023-05-05 19:55:54.695909 micropython_esp32_ota_stubs-1.20.0.post1/uctypes.pyi
--rw-r--r--   0        0        0      709 2023-05-05 19:55:44.620680 micropython_esp32_ota_stubs-1.20.0.post1/uerrno.pyi
--rw-r--r--   0        0        0     1642 2023-05-05 19:55:54.686670 micropython_esp32_ota_stubs-1.20.0.post1/uhashlib.pyi
--rw-r--r--   0        0        0      930 2023-05-05 19:55:54.686670 micropython_esp32_ota_stubs-1.20.0.post1/uheapq.pyi
--rw-r--r--   0        0        0     2650 2023-05-05 19:55:54.783653 micropython_esp32_ota_stubs-1.20.0.post1/uio.pyi
--rw-r--r--   0        0        0     1384 2023-05-05 19:55:54.719004 micropython_esp32_ota_stubs-1.20.0.post1/ujson.pyi
--rw-r--r--   0        0        0    52352 2023-05-05 19:56:01.594931 micropython_esp32_ota_stubs-1.20.0.post1/umachine.pyi
--rw-r--r--   0        0        0        0 2023-05-05 19:49:06.127996 micropython_esp32_ota_stubs-1.20.0.post1/umqtt/__init__.pyi
--rw-r--r--   0        0        0      377 2023-05-05 19:49:06.127996 micropython_esp32_ota_stubs-1.20.0.post1/umqtt/robust.pyi
--rw-r--r--   0        0        0     1292 2023-05-05 19:51:58.397212 micropython_esp32_ota_stubs-1.20.0.post1/umqtt/simple.pyi
--rw-r--r--   0        0        0     9356 2023-05-05 19:55:54.930963 micropython_esp32_ota_stubs-1.20.0.post1/uos.pyi
--rw-r--r--   0        0        0      162 2023-05-05 19:29:15.384914 micropython_esp32_ota_stubs-1.20.0.post1/uplatform.pyi
--rw-r--r--   0        0        0      641 2023-05-05 19:49:06.211075 micropython_esp32_ota_stubs-1.20.0.post1/upysh.pyi
--rw-r--r--   0        0        0     2638 2023-05-05 19:55:54.800156 micropython_esp32_ota_stubs-1.20.0.post1/urandom.pyi
--rw-r--r--   0        0        0      187 2023-05-05 19:29:15.389423 micropython_esp32_ota_stubs-1.20.0.post1/ure.pyi
--rw-r--r--   0        0        0      739 2023-05-05 19:51:58.393263 micropython_esp32_ota_stubs-1.20.0.post1/urequests.pyi
--rw-r--r--   0        0        0     3853 2023-05-05 19:55:49.805637 micropython_esp32_ota_stubs-1.20.0.post1/uselect.pyi
--rw-r--r--   0        0        0     9602 2023-05-05 19:55:55.004580 micropython_esp32_ota_stubs-1.20.0.post1/usocket.pyi
--rw-r--r--   0        0        0     2668 2023-05-05 19:55:54.906690 micropython_esp32_ota_stubs-1.20.0.post1/ussl.pyi
--rw-r--r--   0        0        0     4241 2023-05-05 19:55:54.963950 micropython_esp32_ota_stubs-1.20.0.post1/ustruct.pyi
--rw-r--r--   0        0        0      875 2023-05-05 19:55:54.971965 micropython_esp32_ota_stubs-1.20.0.post1/usys.pyi
--rw-r--r--   0        0        0    12515 2023-05-05 19:55:55.012603 micropython_esp32_ota_stubs-1.20.0.post1/utime.pyi
--rw-r--r--   0        0        0      245 2023-05-05 19:29:15.410622 micropython_esp32_ota_stubs-1.20.0.post1/utimeq.pyi
--rw-r--r--   0        0        0      403 2023-05-05 19:29:15.412371 micropython_esp32_ota_stubs-1.20.0.post1/uwebsocket.pyi
--rw-r--r--   0        0        0     1535 2023-05-05 19:55:55.020595 micropython_esp32_ota_stubs-1.20.0.post1/uzlib.pyi
--rw-r--r--   0        0        0      513 2023-05-05 19:49:06.216864 micropython_esp32_ota_stubs-1.20.0.post1/webrepl.pyi
--rw-r--r--   0        0        0      232 2023-05-05 19:49:06.222477 micropython_esp32_ota_stubs-1.20.0.post1/webrepl_setup.pyi
--rw-r--r--   0        0        0      403 2023-05-05 19:29:15.415811 micropython_esp32_ota_stubs-1.20.0.post1/websocket.pyi
--rw-r--r--   0        0        0     1535 2023-05-05 19:55:55.020595 micropython_esp32_ota_stubs-1.20.0.post1/zlib.pyi
--rw-r--r--   0        0        0     3587 1970-01-01 00:00:00.000000 micropython_esp32_ota_stubs-1.20.0.post1/setup.py
--rw-r--r--   0        0        0     3274 1970-01-01 00:00:00.000000 micropython_esp32_ota_stubs-1.20.0.post1/PKG-INFO
+-rw-r--r--   0        0        0       53 2023-06-07 16:29:08.823669 micropython_esp32_ota_stubs-1.20.0.post2/_boot.pyi
+-rw-r--r--   0        0        0      277 2023-06-07 16:29:08.197734 micropython_esp32_ota_stubs-1.20.0.post2/_onewire.pyi
+-rw-r--r--   0        0        0      848 2023-06-07 16:29:08.198918 micropython_esp32_ota_stubs-1.20.0.post2/_thread.pyi
+-rw-r--r--   0        0        0      364 2023-06-07 16:29:08.200929 micropython_esp32_ota_stubs-1.20.0.post2/_uasyncio.pyi
+-rw-r--r--   0        0        0      115 2023-06-07 16:29:08.824669 micropython_esp32_ota_stubs-1.20.0.post2/apa106.pyi
+-rw-r--r--   0        0        0     1003 2023-06-07 16:29:08.202931 micropython_esp32_ota_stubs-1.20.0.post2/array.pyi
+-rw-r--r--   0        0        0     1408 2023-06-07 16:29:08.204930 micropython_esp32_ota_stubs-1.20.0.post2/binascii.pyi
+-rw-r--r--   0        0        0    31291 2023-06-07 16:29:08.205924 micropython_esp32_ota_stubs-1.20.0.post2/bluetooth.pyi
+-rw-r--r--   0        0        0     3837 2023-06-07 16:29:08.206925 micropython_esp32_ota_stubs-1.20.0.post2/btree.pyi
+-rw-r--r--   0        0        0     1454 2023-06-07 16:29:08.208400 micropython_esp32_ota_stubs-1.20.0.post2/cmath.pyi
+-rw-r--r--   0        0        0     3640 2023-06-07 16:29:08.209413 micropython_esp32_ota_stubs-1.20.0.post2/collections.pyi
+-rw-r--r--   0        0        0     1647 2023-06-07 16:29:08.211408 micropython_esp32_ota_stubs-1.20.0.post2/cryptolib.pyi
+-rw-r--r--   0        0        0      344 2023-06-07 16:29:08.825809 micropython_esp32_ota_stubs-1.20.0.post2/dht.pyi
+-rw-r--r--   0        0        0      404 2023-06-07 16:29:08.827878 micropython_esp32_ota_stubs-1.20.0.post2/ds18x20.pyi
+-rw-r--r--   0        0        0      709 2023-06-07 16:29:08.215407 micropython_esp32_ota_stubs-1.20.0.post2/errno.pyi
+-rw-r--r--   0        0        0     1703 2023-06-07 16:29:08.217409 micropython_esp32_ota_stubs-1.20.0.post2/esp.pyi
+-rw-r--r--   0        0        0    12242 2023-06-07 16:29:08.218698 micropython_esp32_ota_stubs-1.20.0.post2/esp32.pyi
+-rw-r--r--   0        0        0       54 2023-06-07 16:29:08.829008 micropython_esp32_ota_stubs-1.20.0.post2/flashbdev.pyi
+-rw-r--r--   0        0        0     6349 2023-06-07 16:29:08.221029 micropython_esp32_ota_stubs-1.20.0.post2/framebuf.pyi
+-rw-r--r--   0        0        0     1993 2023-06-07 16:29:08.223048 micropython_esp32_ota_stubs-1.20.0.post2/gc.pyi
+-rw-r--r--   0        0        0     1642 2023-06-07 16:29:08.226443 micropython_esp32_ota_stubs-1.20.0.post2/hashlib.pyi
+-rw-r--r--   0        0        0      930 2023-06-07 16:29:08.227435 micropython_esp32_ota_stubs-1.20.0.post2/heapq.pyi
+-rw-r--r--   0        0        0       77 2023-06-07 16:29:08.830015 micropython_esp32_ota_stubs-1.20.0.post2/inisetup.pyi
+-rw-r--r--   0        0        0     2650 2023-06-07 16:29:08.231436 micropython_esp32_ota_stubs-1.20.0.post2/io.pyi
+-rw-r--r--   0        0        0     1384 2023-06-07 16:29:08.233764 micropython_esp32_ota_stubs-1.20.0.post2/json.pyi
+-rw-r--r--   0        0        0     1092 2023-07-03 13:37:56.559921 micropython_esp32_ota_stubs-1.20.0.post2/LICENSE.md
+-rw-r--r--   0        0        0      827 2023-06-07 16:29:08.234771 micropython_esp32_ota_stubs-1.20.0.post2/logging.pyi
+-rw-r--r--   0        0        0    52352 2023-06-07 16:29:08.236782 micropython_esp32_ota_stubs-1.20.0.post2/machine.pyi
+-rw-r--r--   0        0        0     4654 2023-06-07 16:29:08.237772 micropython_esp32_ota_stubs-1.20.0.post2/math.pyi
+-rw-r--r--   0        0        0     8274 2023-07-03 11:26:14.336969 micropython_esp32_ota_stubs-1.20.0.post2/micropython.pyi
+-rw-r--r--   0        0        0     7213 2023-07-03 11:19:19.390108 micropython_esp32_ota_stubs-1.20.0.post2/micropython_.pyi
+-rw-r--r--   0        0        0      598 2023-06-07 16:29:08.832450 micropython_esp32_ota_stubs-1.20.0.post2/mip/__init__.pyi
+-rw-r--r--   0        0        0       68 2023-06-07 16:29:08.242265 micropython_esp32_ota_stubs-1.20.0.post2/mip.pyi
+-rw-r--r--   0        0        0      448 2023-06-07 16:29:08.834648 micropython_esp32_ota_stubs-1.20.0.post2/neopixel.pyi
+-rw-r--r--   0        0        0    10529 2023-06-07 16:29:08.246086 micropython_esp32_ota_stubs-1.20.0.post2/network.pyi
+-rw-r--r--   0        0        0       72 2023-06-07 16:29:08.835649 micropython_esp32_ota_stubs-1.20.0.post2/ntptime.pyi
+-rw-r--r--   0        0        0      617 2023-06-07 16:29:08.837901 micropython_esp32_ota_stubs-1.20.0.post2/onewire.pyi
+-rw-r--r--   0        0        0     9356 2023-06-07 16:29:08.252402 micropython_esp32_ota_stubs-1.20.0.post2/os.pyi
+-rw-r--r--   0        0        0      162 2023-06-07 16:29:08.253924 micropython_esp32_ota_stubs-1.20.0.post2/platform.pyi
+-rw-r--r--   0        0        0     4076 2023-07-03 13:37:58.008955 micropython_esp32_ota_stubs-1.20.0.post2/pyproject.toml
+-rw-r--r--   0        0        0     2638 2023-06-07 16:29:08.255198 micropython_esp32_ota_stubs-1.20.0.post2/random.pyi
+-rw-r--r--   0        0        0     2004 2023-07-03 13:37:56.557924 micropython_esp32_ota_stubs-1.20.0.post2/README.md
+-rw-r--r--   0        0        0     3853 2023-06-07 16:29:08.256609 micropython_esp32_ota_stubs-1.20.0.post2/select.pyi
+-rw-r--r--   0        0        0     9602 2023-06-07 16:29:08.259922 micropython_esp32_ota_stubs-1.20.0.post2/socket.pyi
+-rw-r--r--   0        0        0     2668 2023-06-07 16:29:08.260925 micropython_esp32_ota_stubs-1.20.0.post2/ssl.pyi
+-rw-r--r--   0        0        0     4241 2023-06-07 16:29:08.262922 micropython_esp32_ota_stubs-1.20.0.post2/struct.pyi
+-rw-r--r--   0        0        0      875 2023-06-07 16:29:08.263920 micropython_esp32_ota_stubs-1.20.0.post2/sys.pyi
+-rw-r--r--   0        0        0    12515 2023-06-07 16:29:08.264922 micropython_esp32_ota_stubs-1.20.0.post2/time.pyi
+-rw-r--r--   0        0        0     1003 2023-06-07 16:29:08.266921 micropython_esp32_ota_stubs-1.20.0.post2/uarray.pyi
+-rw-r--r--   0        0        0      132 2023-06-07 16:29:08.838907 micropython_esp32_ota_stubs-1.20.0.post2/uasyncio/__init__.pyi
+-rw-r--r--   0        0        0     1530 2023-06-07 16:29:08.839914 micropython_esp32_ota_stubs-1.20.0.post2/uasyncio/core.pyi
+-rw-r--r--   0        0        0      625 2023-06-07 16:29:08.840907 micropython_esp32_ota_stubs-1.20.0.post2/uasyncio/event.pyi
+-rw-r--r--   0        0        0      390 2023-06-07 16:29:08.842908 micropython_esp32_ota_stubs-1.20.0.post2/uasyncio/funcs.pyi
+-rw-r--r--   0        0        0      414 2023-06-07 16:29:08.843915 micropython_esp32_ota_stubs-1.20.0.post2/uasyncio/lock.pyi
+-rw-r--r--   0        0        0     1410 2023-06-07 16:29:08.845927 micropython_esp32_ota_stubs-1.20.0.post2/uasyncio/stream.pyi
+-rw-r--r--   0        0        0      789 2023-06-07 16:29:08.846935 micropython_esp32_ota_stubs-1.20.0.post2/uasyncio/task.pyi
+-rw-r--r--   0        0        0     1408 2023-06-07 16:29:08.276930 micropython_esp32_ota_stubs-1.20.0.post2/ubinascii.pyi
+-rw-r--r--   0        0        0    31291 2023-06-07 16:29:08.278921 micropython_esp32_ota_stubs-1.20.0.post2/ubluetooth.pyi
+-rw-r--r--   0        0        0     3640 2023-06-07 16:29:08.280077 micropython_esp32_ota_stubs-1.20.0.post2/ucollections.pyi
+-rw-r--r--   0        0        0     1647 2023-06-07 16:29:08.281094 micropython_esp32_ota_stubs-1.20.0.post2/ucryptolib.pyi
+-rw-r--r--   0        0        0     2363 2023-06-07 16:29:08.282303 micropython_esp32_ota_stubs-1.20.0.post2/uctypes.pyi
+-rw-r--r--   0        0        0      709 2023-06-07 16:29:08.283578 micropython_esp32_ota_stubs-1.20.0.post2/uerrno.pyi
+-rw-r--r--   0        0        0     1642 2023-06-07 16:29:08.284756 micropython_esp32_ota_stubs-1.20.0.post2/uhashlib.pyi
+-rw-r--r--   0        0        0      930 2023-06-07 16:29:08.285771 micropython_esp32_ota_stubs-1.20.0.post2/uheapq.pyi
+-rw-r--r--   0        0        0     2650 2023-06-07 16:29:08.287764 micropython_esp32_ota_stubs-1.20.0.post2/uio.pyi
+-rw-r--r--   0        0        0     1384 2023-06-07 16:29:08.288763 micropython_esp32_ota_stubs-1.20.0.post2/ujson.pyi
+-rw-r--r--   0        0        0    52352 2023-06-07 16:29:08.290259 micropython_esp32_ota_stubs-1.20.0.post2/umachine.pyi
+-rw-r--r--   0        0        0        0 2023-06-07 16:29:08.848618 micropython_esp32_ota_stubs-1.20.0.post2/umqtt/__init__.pyi
+-rw-r--r--   0        0        0      377 2023-06-07 16:29:08.848618 micropython_esp32_ota_stubs-1.20.0.post2/umqtt/robust.pyi
+-rw-r--r--   0        0        0     1292 2023-06-07 16:29:08.851415 micropython_esp32_ota_stubs-1.20.0.post2/umqtt/simple.pyi
+-rw-r--r--   0        0        0     9356 2023-06-07 16:29:08.297412 micropython_esp32_ota_stubs-1.20.0.post2/uos.pyi
+-rw-r--r--   0        0        0      162 2023-06-07 16:29:08.299540 micropython_esp32_ota_stubs-1.20.0.post2/uplatform.pyi
+-rw-r--r--   0        0        0      641 2023-06-07 16:29:08.853421 micropython_esp32_ota_stubs-1.20.0.post2/upysh.pyi
+-rw-r--r--   0        0        0     2638 2023-06-07 16:29:08.300542 micropython_esp32_ota_stubs-1.20.0.post2/urandom.pyi
+-rw-r--r--   0        0        0      187 2023-06-07 16:29:08.301756 micropython_esp32_ota_stubs-1.20.0.post2/ure.pyi
+-rw-r--r--   0        0        0      739 2023-06-07 16:29:08.854726 micropython_esp32_ota_stubs-1.20.0.post2/urequests.pyi
+-rw-r--r--   0        0        0     3853 2023-06-07 16:29:08.304597 micropython_esp32_ota_stubs-1.20.0.post2/uselect.pyi
+-rw-r--r--   0        0        0     9602 2023-06-07 16:29:08.306093 micropython_esp32_ota_stubs-1.20.0.post2/usocket.pyi
+-rw-r--r--   0        0        0     2668 2023-06-07 16:29:08.307503 micropython_esp32_ota_stubs-1.20.0.post2/ussl.pyi
+-rw-r--r--   0        0        0     4241 2023-06-07 16:29:08.309630 micropython_esp32_ota_stubs-1.20.0.post2/ustruct.pyi
+-rw-r--r--   0        0        0      875 2023-06-07 16:29:08.310643 micropython_esp32_ota_stubs-1.20.0.post2/usys.pyi
+-rw-r--r--   0        0        0    12515 2023-06-07 16:29:08.312642 micropython_esp32_ota_stubs-1.20.0.post2/utime.pyi
+-rw-r--r--   0        0        0      245 2023-06-07 16:29:08.313638 micropython_esp32_ota_stubs-1.20.0.post2/utimeq.pyi
+-rw-r--r--   0        0        0      403 2023-06-07 16:29:08.314637 micropython_esp32_ota_stubs-1.20.0.post2/uwebsocket.pyi
+-rw-r--r--   0        0        0     1535 2023-06-07 16:29:08.316643 micropython_esp32_ota_stubs-1.20.0.post2/uzlib.pyi
+-rw-r--r--   0        0        0      513 2023-06-07 16:29:08.855898 micropython_esp32_ota_stubs-1.20.0.post2/webrepl.pyi
+-rw-r--r--   0        0        0      232 2023-06-07 16:29:08.857711 micropython_esp32_ota_stubs-1.20.0.post2/webrepl_setup.pyi
+-rw-r--r--   0        0        0      403 2023-06-07 16:29:08.317646 micropython_esp32_ota_stubs-1.20.0.post2/websocket.pyi
+-rw-r--r--   0        0        0     1535 2023-06-07 16:29:08.318642 micropython_esp32_ota_stubs-1.20.0.post2/zlib.pyi
+-rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 micropython_esp32_ota_stubs-1.20.0.post2/setup.py
+-rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 micropython_esp32_ota_stubs-1.20.0.post2/PKG-INFO
```

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/_thread.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/_thread.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/array.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/array.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/binascii.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/binascii.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/bluetooth.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/bluetooth.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/btree.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/btree.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/cmath.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/cmath.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/collections.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/collections.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/cryptolib.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/cryptolib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/errno.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/errno.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/esp.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/esp.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/esp32.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/esp32.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/framebuf.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/framebuf.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/gc.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/gc.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/hashlib.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/hashlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/heapq.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/heapq.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/io.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/io.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/json.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/json.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/LICENSE.md` & `micropython_esp32_ota_stubs-1.20.0.post2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/logging.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/logging.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/machine.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/machine.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/math.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/math.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/micropython.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/micropython_.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/mip/__init__.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/mip/__init__.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/network.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/network.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/onewire.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/onewire.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/os.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/os.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/pyproject.toml` & `micropython_esp32_ota_stubs-1.20.0.post2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropython-esp32-ota-stubs"
-version = "1.20.0.post1"
+version = "1.20.0.post2"
 description = "MicroPython stubs"
 authors = [
     "josverl <josverl@users.noreply.github.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/josverl/micropython-stubs#micropython-stubs"
@@ -57,14 +57,15 @@
     { include = "inisetup.pyi" },
     { include = "io.pyi" },
     { include = "json.pyi" },
     { include = "logging.pyi" },
     { include = "machine.pyi" },
     { include = "math.pyi" },
     { include = "micropython.pyi" },
+    { include = "micropython_.pyi" },
     { include = "mip/__init__.pyi" },
     { include = "mip.pyi" },
     { include = "neopixel.pyi" },
     { include = "network.pyi" },
     { include = "ntptime.pyi" },
     { include = "onewire.pyi" },
     { include = "os.pyi" },
```

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/random.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/random.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/README.md` & `micropython_esp32_ota_stubs-1.20.0.post2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
 
 For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
  * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
 
 Included stubs:
-* StubSource.MERGED from `stubs/micropython-v1_20_0-esp32-ota-merged`
-* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`
-* StubSource.CORE from `stubs/micropython-core`
+* Merged stubs from `stubs/micropython-v1_20_0-esp32-ota-merged`
+* Frozen stubs from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`
+* Core stubs from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
 Documentation | micropython | - | - | v1.20.0 
 Core | micropython | esp32 | - | v1.20.0
```

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/select.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/select.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/socket.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/socket.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/ssl.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/ssl.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/struct.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/struct.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/sys.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/sys.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/time.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/time.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/uarray.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/uarray.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/uasyncio/core.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/uasyncio/core.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/uasyncio/event.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/uasyncio/event.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/uasyncio/stream.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/uasyncio/stream.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/uasyncio/task.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/uasyncio/task.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/ubinascii.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/ubinascii.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/ubluetooth.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/ubluetooth.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/ucollections.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/ucollections.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/ucryptolib.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/ucryptolib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/uctypes.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/uctypes.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/uerrno.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/uerrno.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/uhashlib.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/uhashlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/uheapq.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/uheapq.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/uio.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/uio.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/ujson.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/ujson.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/umachine.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/umachine.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/umqtt/simple.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/umqtt/simple.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/uos.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/uos.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/upysh.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/upysh.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/urandom.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/urandom.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/urequests.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/urequests.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/uselect.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/uselect.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/usocket.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/usocket.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/ussl.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/ussl.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/ustruct.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/ustruct.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/usys.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/usys.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/utime.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/utime.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/uzlib.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/uzlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/webrepl.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/webrepl.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/zlib.pyi` & `micropython_esp32_ota_stubs-1.20.0.post2/zlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/setup.py` & `micropython_esp32_ota_stubs-1.20.0.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
  'inisetup',
  'io',
  'json',
  'logging',
  'machine',
  'math',
  'micropython',
+ 'micropython_',
  '__init__',
  'mip',
  'neopixel',
  'network',
  'ntptime',
  'onewire',
  'os',
@@ -86,17 +87,17 @@
  'websocket',
  'zlib']
 install_requires = \
 ['micropython-stdlib-stubs>=0.9.0']
 
 setup_kwargs = {
     'name': 'micropython-esp32-ota-stubs',
-    'version': '1.20.0.post1',
+    'version': '1.20.0.post2',
     'description': 'MicroPython stubs',
-    'long_description': '# micropython-esp32-ota-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* StubSource.MERGED from `stubs/micropython-v1_20_0-esp32-ota-merged`\n* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`\n* StubSource.CORE from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nDocumentation | micropython | - | - | v1.20.0 \nCore | micropython | esp32 | - | v1.20.0 \n',
+    'long_description': '# micropython-esp32-ota-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* Merged stubs from `stubs/micropython-v1_20_0-esp32-ota-merged`\n* Frozen stubs from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`\n* Core stubs from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nDocumentation | micropython | - | - | v1.20.0 \nCore | micropython | esp32 | - | v1.20.0 \n',
     'author': 'josverl',
     'author_email': 'josverl@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josverl/micropython-stubs#micropython-stubs',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `micropython_esp32_ota_stubs-1.20.0.post1/PKG-INFO` & `micropython_esp32_ota_stubs-1.20.0.post2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-esp32-ota-stubs
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
-* StubSource.MERGED from `stubs/micropython-v1_20_0-esp32-ota-merged`
-* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`
-* StubSource.CORE from `stubs/micropython-core`
+* Merged stubs from `stubs/micropython-v1_20_0-esp32-ota-merged`
+* Frozen stubs from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`
+* Core stubs from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
 Documentation | micropython | - | - | v1.20.0 
 Core | micropython | esp32 | - | v1.20.0
```

