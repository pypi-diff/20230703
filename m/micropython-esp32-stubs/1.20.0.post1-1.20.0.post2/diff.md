# Comparing `tmp/micropython_esp32_stubs-1.20.0.post1.tar.gz` & `tmp/micropython_esp32_stubs-1.20.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_esp32_stubs-1.20.0.post1.tar", max compression
+gzip compressed data, was "micropython_esp32_stubs-1.20.0.post2.tar", max compression
```

## Comparing `micropython_esp32_stubs-1.20.0.post1.tar` & `micropython_esp32_stubs-1.20.0.post2.tar`

### file list

```diff
@@ -1,90 +1,91 @@
--rw-r--r--   0        0        0       53 2023-05-05 19:49:06.160838 micropython_esp32_stubs-1.20.0.post1/_boot.pyi
--rw-r--r--   0        0        0      277 2023-05-05 20:22:59.220054 micropython_esp32_stubs-1.20.0.post1/_onewire.pyi
--rw-r--r--   0        0        0      848 2023-05-05 20:23:06.206407 micropython_esp32_stubs-1.20.0.post1/_thread.pyi
--rw-r--r--   0        0        0      364 2023-05-05 20:22:59.228399 micropython_esp32_stubs-1.20.0.post1/_uasyncio.pyi
--rw-r--r--   0        0        0      115 2023-05-05 19:49:06.163754 micropython_esp32_stubs-1.20.0.post1/apa106.pyi
--rw-r--r--   0        0        0     1003 2023-05-05 20:23:25.942461 micropython_esp32_stubs-1.20.0.post1/array.pyi
--rw-r--r--   0        0        0     1408 2023-05-05 20:23:26.029016 micropython_esp32_stubs-1.20.0.post1/binascii.pyi
--rw-r--r--   0        0        0    31291 2023-05-05 20:23:26.116139 micropython_esp32_stubs-1.20.0.post1/bluetooth.pyi
--rw-r--r--   0        0        0     3837 2023-05-05 20:23:07.461038 micropython_esp32_stubs-1.20.0.post1/btree.pyi
--rw-r--r--   0        0        0     1454 2023-05-05 20:23:26.163497 micropython_esp32_stubs-1.20.0.post1/cmath.pyi
--rw-r--r--   0        0        0     3640 2023-05-05 20:23:26.161452 micropython_esp32_stubs-1.20.0.post1/collections.pyi
--rw-r--r--   0        0        0     1647 2023-05-05 20:23:08.299942 micropython_esp32_stubs-1.20.0.post1/cryptolib.pyi
--rw-r--r--   0        0        0      344 2023-05-05 19:49:06.167790 micropython_esp32_stubs-1.20.0.post1/dht.pyi
--rw-r--r--   0        0        0      404 2023-05-05 19:49:06.170625 micropython_esp32_stubs-1.20.0.post1/ds18x20.pyi
--rw-r--r--   0        0        0      709 2023-05-05 20:23:08.509119 micropython_esp32_stubs-1.20.0.post1/errno.pyi
--rw-r--r--   0        0        0     1703 2023-05-05 20:23:26.202466 micropython_esp32_stubs-1.20.0.post1/esp.pyi
--rw-r--r--   0        0        0    12242 2023-05-05 20:23:26.332028 micropython_esp32_stubs-1.20.0.post1/esp32.pyi
--rw-r--r--   0        0        0       54 2023-05-05 19:49:06.172981 micropython_esp32_stubs-1.20.0.post1/flashbdev.pyi
--rw-r--r--   0        0        0     6349 2023-05-05 20:23:26.258860 micropython_esp32_stubs-1.20.0.post1/framebuf.pyi
--rw-r--r--   0        0        0     1993 2023-05-05 20:23:26.246651 micropython_esp32_stubs-1.20.0.post1/gc.pyi
--rw-r--r--   0        0        0     1642 2023-05-05 20:23:26.258860 micropython_esp32_stubs-1.20.0.post1/hashlib.pyi
--rw-r--r--   0        0        0      930 2023-05-05 20:23:26.279660 micropython_esp32_stubs-1.20.0.post1/heapq.pyi
--rw-r--r--   0        0        0       77 2023-05-05 19:49:06.175994 micropython_esp32_stubs-1.20.0.post1/inisetup.pyi
--rw-r--r--   0        0        0     2650 2023-05-05 20:23:26.364596 micropython_esp32_stubs-1.20.0.post1/io.pyi
--rw-r--r--   0        0        0     1384 2023-05-05 20:23:26.291952 micropython_esp32_stubs-1.20.0.post1/json.pyi
--rw-r--r--   0        0        0     1092 2023-05-05 20:31:11.115559 micropython_esp32_stubs-1.20.0.post1/LICENSE.md
--rw-r--r--   0        0        0      827 2023-05-05 20:22:59.278622 micropython_esp32_stubs-1.20.0.post1/logging.pyi
--rw-r--r--   0        0        0    52352 2023-05-05 20:23:29.666884 micropython_esp32_stubs-1.20.0.post1/machine.pyi
--rw-r--r--   0        0        0     4654 2023-05-05 20:23:26.479425 micropython_esp32_stubs-1.20.0.post1/math.pyi
--rw-r--r--   0        0        0     7213 2023-04-05 11:07:45.360315 micropython_esp32_stubs-1.20.0.post1/micropython.pyi
--rw-r--r--   0        0        0      598 2023-05-05 19:51:58.147437 micropython_esp32_stubs-1.20.0.post1/mip/__init__.pyi
--rw-r--r--   0        0        0       68 2023-05-05 20:22:59.278622 micropython_esp32_stubs-1.20.0.post1/mip.pyi
--rw-r--r--   0        0        0      448 2023-05-05 19:49:06.179674 micropython_esp32_stubs-1.20.0.post1/neopixel.pyi
--rw-r--r--   0        0        0    10529 2023-05-05 20:23:26.560051 micropython_esp32_stubs-1.20.0.post1/network.pyi
--rw-r--r--   0        0        0       72 2023-05-05 19:49:06.185571 micropython_esp32_stubs-1.20.0.post1/ntptime.pyi
--rw-r--r--   0        0        0      617 2023-05-05 19:49:06.192533 micropython_esp32_stubs-1.20.0.post1/onewire.pyi
--rw-r--r--   0        0        0     9356 2023-05-05 20:23:26.672646 micropython_esp32_stubs-1.20.0.post1/os.pyi
--rw-r--r--   0        0        0      162 2023-05-05 20:22:59.295467 micropython_esp32_stubs-1.20.0.post1/platform.pyi
--rw-r--r--   0        0        0     4034 2023-05-05 20:31:13.441563 micropython_esp32_stubs-1.20.0.post1/pyproject.toml
--rw-r--r--   0        0        0     2638 2023-05-05 20:23:26.583649 micropython_esp32_stubs-1.20.0.post1/random.pyi
--rw-r--r--   0        0        0     2011 2023-05-05 20:31:11.114544 micropython_esp32_stubs-1.20.0.post1/README.md
--rw-r--r--   0        0        0     3853 2023-05-05 20:23:15.774982 micropython_esp32_stubs-1.20.0.post1/select.pyi
--rw-r--r--   0        0        0     9602 2023-05-05 20:23:26.730375 micropython_esp32_stubs-1.20.0.post1/socket.pyi
--rw-r--r--   0        0        0     2668 2023-05-05 20:23:26.688689 micropython_esp32_stubs-1.20.0.post1/ssl.pyi
--rw-r--r--   0        0        0     4241 2023-05-05 20:23:26.761968 micropython_esp32_stubs-1.20.0.post1/struct.pyi
--rw-r--r--   0        0        0      875 2023-05-05 20:23:26.737644 micropython_esp32_stubs-1.20.0.post1/sys.pyi
--rw-r--r--   0        0        0    12515 2023-05-05 20:23:26.805066 micropython_esp32_stubs-1.20.0.post1/time.pyi
--rw-r--r--   0        0        0     1003 2023-05-05 20:23:26.788193 micropython_esp32_stubs-1.20.0.post1/uarray.pyi
--rw-r--r--   0        0        0      132 2023-05-05 19:49:06.046649 micropython_esp32_stubs-1.20.0.post1/uasyncio/__init__.pyi
--rw-r--r--   0        0        0     1530 2023-05-05 19:49:06.047659 micropython_esp32_stubs-1.20.0.post1/uasyncio/core.pyi
--rw-r--r--   0        0        0      625 2023-05-05 19:49:06.055187 micropython_esp32_stubs-1.20.0.post1/uasyncio/event.pyi
--rw-r--r--   0        0        0      390 2023-05-05 19:49:06.060787 micropython_esp32_stubs-1.20.0.post1/uasyncio/funcs.pyi
--rw-r--r--   0        0        0      414 2023-05-05 19:49:06.060787 micropython_esp32_stubs-1.20.0.post1/uasyncio/lock.pyi
--rw-r--r--   0        0        0     1410 2023-05-05 19:51:58.349367 micropython_esp32_stubs-1.20.0.post1/uasyncio/stream.pyi
--rw-r--r--   0        0        0      789 2023-05-05 19:49:06.084965 micropython_esp32_stubs-1.20.0.post1/uasyncio/task.pyi
--rw-r--r--   0        0        0     1408 2023-05-05 20:23:26.891363 micropython_esp32_stubs-1.20.0.post1/ubinascii.pyi
--rw-r--r--   0        0        0    31291 2023-05-05 20:23:27.051854 micropython_esp32_stubs-1.20.0.post1/ubluetooth.pyi
--rw-r--r--   0        0        0     3640 2023-05-05 20:23:26.981894 micropython_esp32_stubs-1.20.0.post1/ucollections.pyi
--rw-r--r--   0        0        0     1647 2023-05-05 20:23:18.641139 micropython_esp32_stubs-1.20.0.post1/ucryptolib.pyi
--rw-r--r--   0        0        0     2363 2023-05-05 20:23:27.063883 micropython_esp32_stubs-1.20.0.post1/uctypes.pyi
--rw-r--r--   0        0        0      709 2023-05-05 20:23:19.110558 micropython_esp32_stubs-1.20.0.post1/uerrno.pyi
--rw-r--r--   0        0        0     1642 2023-05-05 20:23:27.055940 micropython_esp32_stubs-1.20.0.post1/uhashlib.pyi
--rw-r--r--   0        0        0      930 2023-05-05 20:23:27.088447 micropython_esp32_stubs-1.20.0.post1/uheapq.pyi
--rw-r--r--   0        0        0     2650 2023-05-05 20:23:27.155029 micropython_esp32_stubs-1.20.0.post1/uio.pyi
--rw-r--r--   0        0        0     1384 2023-05-05 20:23:27.113374 micropython_esp32_stubs-1.20.0.post1/ujson.pyi
--rw-r--r--   0        0        0    52352 2023-05-05 20:23:31.772392 micropython_esp32_stubs-1.20.0.post1/umachine.pyi
--rw-r--r--   0        0        0        0 2023-05-05 19:49:06.127996 micropython_esp32_stubs-1.20.0.post1/umqtt/__init__.pyi
--rw-r--r--   0        0        0      377 2023-05-05 19:49:06.127996 micropython_esp32_stubs-1.20.0.post1/umqtt/robust.pyi
--rw-r--r--   0        0        0     1292 2023-05-05 19:51:58.397212 micropython_esp32_stubs-1.20.0.post1/umqtt/simple.pyi
--rw-r--r--   0        0        0     9356 2023-05-05 20:23:27.332182 micropython_esp32_stubs-1.20.0.post1/uos.pyi
--rw-r--r--   0        0        0      162 2023-05-05 20:22:59.331083 micropython_esp32_stubs-1.20.0.post1/uplatform.pyi
--rw-r--r--   0        0        0      641 2023-05-05 19:49:06.211075 micropython_esp32_stubs-1.20.0.post1/upysh.pyi
--rw-r--r--   0        0        0     2638 2023-05-05 20:23:27.212075 micropython_esp32_stubs-1.20.0.post1/urandom.pyi
--rw-r--r--   0        0        0      187 2023-05-05 20:22:59.338712 micropython_esp32_stubs-1.20.0.post1/ure.pyi
--rw-r--r--   0        0        0      739 2023-05-05 19:51:58.393263 micropython_esp32_stubs-1.20.0.post1/urequests.pyi
--rw-r--r--   0        0        0     3853 2023-05-05 20:23:23.154717 micropython_esp32_stubs-1.20.0.post1/uselect.pyi
--rw-r--r--   0        0        0     9602 2023-05-05 20:23:27.360579 micropython_esp32_stubs-1.20.0.post1/usocket.pyi
--rw-r--r--   0        0        0     2668 2023-05-05 20:23:27.285085 micropython_esp32_stubs-1.20.0.post1/ussl.pyi
--rw-r--r--   0        0        0     4241 2023-05-05 20:23:27.315416 micropython_esp32_stubs-1.20.0.post1/ustruct.pyi
--rw-r--r--   0        0        0      875 2023-05-05 20:23:27.365511 micropython_esp32_stubs-1.20.0.post1/usys.pyi
--rw-r--r--   0        0        0    12515 2023-05-05 20:23:27.446527 micropython_esp32_stubs-1.20.0.post1/utime.pyi
--rw-r--r--   0        0        0      245 2023-05-05 20:22:59.351492 micropython_esp32_stubs-1.20.0.post1/utimeq.pyi
--rw-r--r--   0        0        0      403 2023-05-05 20:22:59.351492 micropython_esp32_stubs-1.20.0.post1/uwebsocket.pyi
--rw-r--r--   0        0        0     1535 2023-05-05 20:23:27.431524 micropython_esp32_stubs-1.20.0.post1/uzlib.pyi
--rw-r--r--   0        0        0      513 2023-05-05 19:49:06.216864 micropython_esp32_stubs-1.20.0.post1/webrepl.pyi
--rw-r--r--   0        0        0      232 2023-05-05 19:49:06.222477 micropython_esp32_stubs-1.20.0.post1/webrepl_setup.pyi
--rw-r--r--   0        0        0      403 2023-05-05 20:22:59.357196 micropython_esp32_stubs-1.20.0.post1/websocket.pyi
--rw-r--r--   0        0        0     1535 2023-05-05 20:23:27.462203 micropython_esp32_stubs-1.20.0.post1/zlib.pyi
--rw-r--r--   0        0        0     3575 1970-01-01 00:00:00.000000 micropython_esp32_stubs-1.20.0.post1/setup.py
--rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 micropython_esp32_stubs-1.20.0.post1/PKG-INFO
+-rw-r--r--   0        0        0       53 2023-06-07 16:29:08.823669 micropython_esp32_stubs-1.20.0.post2/_boot.pyi
+-rw-r--r--   0        0        0      277 2023-06-07 16:29:08.637849 micropython_esp32_stubs-1.20.0.post2/_onewire.pyi
+-rw-r--r--   0        0        0      848 2023-06-07 16:29:08.638853 micropython_esp32_stubs-1.20.0.post2/_thread.pyi
+-rw-r--r--   0        0        0      364 2023-06-07 16:29:08.640854 micropython_esp32_stubs-1.20.0.post2/_uasyncio.pyi
+-rw-r--r--   0        0        0      115 2023-06-07 16:29:08.824669 micropython_esp32_stubs-1.20.0.post2/apa106.pyi
+-rw-r--r--   0        0        0     1003 2023-06-07 16:29:08.641853 micropython_esp32_stubs-1.20.0.post2/array.pyi
+-rw-r--r--   0        0        0     1408 2023-06-07 16:29:08.644316 micropython_esp32_stubs-1.20.0.post2/binascii.pyi
+-rw-r--r--   0        0        0    31291 2023-06-07 16:29:08.645735 micropython_esp32_stubs-1.20.0.post2/bluetooth.pyi
+-rw-r--r--   0        0        0     3837 2023-06-07 16:29:08.646762 micropython_esp32_stubs-1.20.0.post2/btree.pyi
+-rw-r--r--   0        0        0     1454 2023-06-07 16:29:08.647746 micropython_esp32_stubs-1.20.0.post2/cmath.pyi
+-rw-r--r--   0        0        0     3640 2023-06-07 16:29:08.649848 micropython_esp32_stubs-1.20.0.post2/collections.pyi
+-rw-r--r--   0        0        0     1647 2023-06-07 16:29:08.650854 micropython_esp32_stubs-1.20.0.post2/cryptolib.pyi
+-rw-r--r--   0        0        0      344 2023-06-07 16:29:08.825809 micropython_esp32_stubs-1.20.0.post2/dht.pyi
+-rw-r--r--   0        0        0      404 2023-06-07 16:29:08.827878 micropython_esp32_stubs-1.20.0.post2/ds18x20.pyi
+-rw-r--r--   0        0        0      709 2023-06-07 16:29:08.656390 micropython_esp32_stubs-1.20.0.post2/errno.pyi
+-rw-r--r--   0        0        0     1703 2023-06-07 16:29:08.656390 micropython_esp32_stubs-1.20.0.post2/esp.pyi
+-rw-r--r--   0        0        0    12242 2023-06-07 16:29:08.658868 micropython_esp32_stubs-1.20.0.post2/esp32.pyi
+-rw-r--r--   0        0        0       54 2023-06-07 16:29:08.829008 micropython_esp32_stubs-1.20.0.post2/flashbdev.pyi
+-rw-r--r--   0        0        0     6349 2023-06-07 16:29:08.661333 micropython_esp32_stubs-1.20.0.post2/framebuf.pyi
+-rw-r--r--   0        0        0     1993 2023-06-07 16:29:08.662340 micropython_esp32_stubs-1.20.0.post2/gc.pyi
+-rw-r--r--   0        0        0     1642 2023-06-07 16:29:08.664342 micropython_esp32_stubs-1.20.0.post2/hashlib.pyi
+-rw-r--r--   0        0        0      930 2023-06-07 16:29:08.665340 micropython_esp32_stubs-1.20.0.post2/heapq.pyi
+-rw-r--r--   0        0        0       77 2023-06-07 16:29:08.830015 micropython_esp32_stubs-1.20.0.post2/inisetup.pyi
+-rw-r--r--   0        0        0     2650 2023-06-07 16:29:08.667345 micropython_esp32_stubs-1.20.0.post2/io.pyi
+-rw-r--r--   0        0        0     1384 2023-06-07 16:29:08.668339 micropython_esp32_stubs-1.20.0.post2/json.pyi
+-rw-r--r--   0        0        0     1092 2023-07-03 13:37:44.170742 micropython_esp32_stubs-1.20.0.post2/LICENSE.md
+-rw-r--r--   0        0        0      827 2023-06-07 16:29:08.670341 micropython_esp32_stubs-1.20.0.post2/logging.pyi
+-rw-r--r--   0        0        0    52352 2023-06-07 16:29:08.671340 micropython_esp32_stubs-1.20.0.post2/machine.pyi
+-rw-r--r--   0        0        0     4654 2023-06-07 16:29:08.672341 micropython_esp32_stubs-1.20.0.post2/math.pyi
+-rw-r--r--   0        0        0     8274 2023-07-03 11:26:14.336969 micropython_esp32_stubs-1.20.0.post2/micropython.pyi
+-rw-r--r--   0        0        0     7213 2023-07-03 11:19:19.390108 micropython_esp32_stubs-1.20.0.post2/micropython_.pyi
+-rw-r--r--   0        0        0      598 2023-06-07 16:29:08.832450 micropython_esp32_stubs-1.20.0.post2/mip/__init__.pyi
+-rw-r--r--   0        0        0       68 2023-06-07 16:29:08.674341 micropython_esp32_stubs-1.20.0.post2/mip.pyi
+-rw-r--r--   0        0        0      448 2023-06-07 16:29:08.834648 micropython_esp32_stubs-1.20.0.post2/neopixel.pyi
+-rw-r--r--   0        0        0    10529 2023-06-07 16:29:08.677345 micropython_esp32_stubs-1.20.0.post2/network.pyi
+-rw-r--r--   0        0        0       72 2023-06-07 16:29:08.835649 micropython_esp32_stubs-1.20.0.post2/ntptime.pyi
+-rw-r--r--   0        0        0      617 2023-06-07 16:29:08.837901 micropython_esp32_stubs-1.20.0.post2/onewire.pyi
+-rw-r--r--   0        0        0     9356 2023-06-07 16:29:08.679350 micropython_esp32_stubs-1.20.0.post2/os.pyi
+-rw-r--r--   0        0        0      162 2023-06-07 16:29:08.680343 micropython_esp32_stubs-1.20.0.post2/platform.pyi
+-rw-r--r--   0        0        0     4072 2023-07-03 13:37:46.772976 micropython_esp32_stubs-1.20.0.post2/pyproject.toml
+-rw-r--r--   0        0        0     2638 2023-06-07 16:29:08.681637 micropython_esp32_stubs-1.20.0.post2/random.pyi
+-rw-r--r--   0        0        0     1996 2023-07-03 13:37:44.168738 micropython_esp32_stubs-1.20.0.post2/README.md
+-rw-r--r--   0        0        0     3853 2023-06-07 16:29:08.682643 micropython_esp32_stubs-1.20.0.post2/select.pyi
+-rw-r--r--   0        0        0     9602 2023-06-07 16:29:08.683643 micropython_esp32_stubs-1.20.0.post2/socket.pyi
+-rw-r--r--   0        0        0     2668 2023-06-07 16:29:08.684652 micropython_esp32_stubs-1.20.0.post2/ssl.pyi
+-rw-r--r--   0        0        0     4241 2023-06-07 16:29:08.685647 micropython_esp32_stubs-1.20.0.post2/struct.pyi
+-rw-r--r--   0        0        0      875 2023-06-07 16:29:08.687646 micropython_esp32_stubs-1.20.0.post2/sys.pyi
+-rw-r--r--   0        0        0    12515 2023-06-07 16:29:08.688644 micropython_esp32_stubs-1.20.0.post2/time.pyi
+-rw-r--r--   0        0        0     1003 2023-06-07 16:29:08.689653 micropython_esp32_stubs-1.20.0.post2/uarray.pyi
+-rw-r--r--   0        0        0      132 2023-06-07 16:29:08.838907 micropython_esp32_stubs-1.20.0.post2/uasyncio/__init__.pyi
+-rw-r--r--   0        0        0     1530 2023-06-07 16:29:08.839914 micropython_esp32_stubs-1.20.0.post2/uasyncio/core.pyi
+-rw-r--r--   0        0        0      625 2023-06-07 16:29:08.840907 micropython_esp32_stubs-1.20.0.post2/uasyncio/event.pyi
+-rw-r--r--   0        0        0      390 2023-06-07 16:29:08.842908 micropython_esp32_stubs-1.20.0.post2/uasyncio/funcs.pyi
+-rw-r--r--   0        0        0      414 2023-06-07 16:29:08.843915 micropython_esp32_stubs-1.20.0.post2/uasyncio/lock.pyi
+-rw-r--r--   0        0        0     1410 2023-06-07 16:29:08.845927 micropython_esp32_stubs-1.20.0.post2/uasyncio/stream.pyi
+-rw-r--r--   0        0        0      789 2023-06-07 16:29:08.846935 micropython_esp32_stubs-1.20.0.post2/uasyncio/task.pyi
+-rw-r--r--   0        0        0     1408 2023-06-07 16:29:08.697875 micropython_esp32_stubs-1.20.0.post2/ubinascii.pyi
+-rw-r--r--   0        0        0    31291 2023-06-07 16:29:08.698871 micropython_esp32_stubs-1.20.0.post2/ubluetooth.pyi
+-rw-r--r--   0        0        0     3640 2023-06-07 16:29:08.699872 micropython_esp32_stubs-1.20.0.post2/ucollections.pyi
+-rw-r--r--   0        0        0     1647 2023-06-07 16:29:08.700870 micropython_esp32_stubs-1.20.0.post2/ucryptolib.pyi
+-rw-r--r--   0        0        0     2363 2023-06-07 16:29:08.701873 micropython_esp32_stubs-1.20.0.post2/uctypes.pyi
+-rw-r--r--   0        0        0      709 2023-06-07 16:29:08.702871 micropython_esp32_stubs-1.20.0.post2/uerrno.pyi
+-rw-r--r--   0        0        0     1642 2023-06-07 16:29:08.702871 micropython_esp32_stubs-1.20.0.post2/uhashlib.pyi
+-rw-r--r--   0        0        0      930 2023-06-07 16:29:08.703870 micropython_esp32_stubs-1.20.0.post2/uheapq.pyi
+-rw-r--r--   0        0        0     2650 2023-06-07 16:29:08.704870 micropython_esp32_stubs-1.20.0.post2/uio.pyi
+-rw-r--r--   0        0        0     1384 2023-06-07 16:29:08.705870 micropython_esp32_stubs-1.20.0.post2/ujson.pyi
+-rw-r--r--   0        0        0    52352 2023-06-07 16:29:08.706872 micropython_esp32_stubs-1.20.0.post2/umachine.pyi
+-rw-r--r--   0        0        0        0 2023-06-07 16:29:08.848618 micropython_esp32_stubs-1.20.0.post2/umqtt/__init__.pyi
+-rw-r--r--   0        0        0      377 2023-06-07 16:29:08.848618 micropython_esp32_stubs-1.20.0.post2/umqtt/robust.pyi
+-rw-r--r--   0        0        0     1292 2023-06-07 16:29:08.851415 micropython_esp32_stubs-1.20.0.post2/umqtt/simple.pyi
+-rw-r--r--   0        0        0     9356 2023-06-07 16:29:08.710740 micropython_esp32_stubs-1.20.0.post2/uos.pyi
+-rw-r--r--   0        0        0      162 2023-06-07 16:29:08.711744 micropython_esp32_stubs-1.20.0.post2/uplatform.pyi
+-rw-r--r--   0        0        0      641 2023-06-07 16:29:08.853421 micropython_esp32_stubs-1.20.0.post2/upysh.pyi
+-rw-r--r--   0        0        0     2638 2023-06-07 16:29:08.712755 micropython_esp32_stubs-1.20.0.post2/urandom.pyi
+-rw-r--r--   0        0        0      187 2023-06-07 16:29:08.713747 micropython_esp32_stubs-1.20.0.post2/ure.pyi
+-rw-r--r--   0        0        0      739 2023-06-07 16:29:08.854726 micropython_esp32_stubs-1.20.0.post2/urequests.pyi
+-rw-r--r--   0        0        0     3853 2023-06-07 16:29:08.714752 micropython_esp32_stubs-1.20.0.post2/uselect.pyi
+-rw-r--r--   0        0        0     9602 2023-06-07 16:29:08.715745 micropython_esp32_stubs-1.20.0.post2/usocket.pyi
+-rw-r--r--   0        0        0     2668 2023-06-07 16:29:08.716745 micropython_esp32_stubs-1.20.0.post2/ussl.pyi
+-rw-r--r--   0        0        0     4241 2023-06-07 16:29:08.717753 micropython_esp32_stubs-1.20.0.post2/ustruct.pyi
+-rw-r--r--   0        0        0      875 2023-06-07 16:29:08.718751 micropython_esp32_stubs-1.20.0.post2/usys.pyi
+-rw-r--r--   0        0        0    12515 2023-06-07 16:29:08.719754 micropython_esp32_stubs-1.20.0.post2/utime.pyi
+-rw-r--r--   0        0        0      245 2023-06-07 16:29:08.720747 micropython_esp32_stubs-1.20.0.post2/utimeq.pyi
+-rw-r--r--   0        0        0      403 2023-06-07 16:29:08.720747 micropython_esp32_stubs-1.20.0.post2/uwebsocket.pyi
+-rw-r--r--   0        0        0     1535 2023-06-07 16:29:08.721754 micropython_esp32_stubs-1.20.0.post2/uzlib.pyi
+-rw-r--r--   0        0        0      513 2023-06-07 16:29:08.855898 micropython_esp32_stubs-1.20.0.post2/webrepl.pyi
+-rw-r--r--   0        0        0      232 2023-06-07 16:29:08.857711 micropython_esp32_stubs-1.20.0.post2/webrepl_setup.pyi
+-rw-r--r--   0        0        0      403 2023-06-07 16:29:08.722758 micropython_esp32_stubs-1.20.0.post2/websocket.pyi
+-rw-r--r--   0        0        0     1535 2023-06-07 16:29:08.723751 micropython_esp32_stubs-1.20.0.post2/zlib.pyi
+-rw-r--r--   0        0        0     3577 1970-01-01 00:00:00.000000 micropython_esp32_stubs-1.20.0.post2/setup.py
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 micropython_esp32_stubs-1.20.0.post2/PKG-INFO
```

### Comparing `micropython_esp32_stubs-1.20.0.post1/_thread.pyi` & `micropython_esp32_stubs-1.20.0.post2/_thread.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/array.pyi` & `micropython_esp32_stubs-1.20.0.post2/array.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/binascii.pyi` & `micropython_esp32_stubs-1.20.0.post2/binascii.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/bluetooth.pyi` & `micropython_esp32_stubs-1.20.0.post2/bluetooth.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/btree.pyi` & `micropython_esp32_stubs-1.20.0.post2/btree.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/cmath.pyi` & `micropython_esp32_stubs-1.20.0.post2/cmath.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/collections.pyi` & `micropython_esp32_stubs-1.20.0.post2/collections.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/cryptolib.pyi` & `micropython_esp32_stubs-1.20.0.post2/cryptolib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/errno.pyi` & `micropython_esp32_stubs-1.20.0.post2/errno.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/esp.pyi` & `micropython_esp32_stubs-1.20.0.post2/esp.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/esp32.pyi` & `micropython_esp32_stubs-1.20.0.post2/esp32.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/framebuf.pyi` & `micropython_esp32_stubs-1.20.0.post2/framebuf.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/gc.pyi` & `micropython_esp32_stubs-1.20.0.post2/gc.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/hashlib.pyi` & `micropython_esp32_stubs-1.20.0.post2/hashlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/heapq.pyi` & `micropython_esp32_stubs-1.20.0.post2/heapq.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/io.pyi` & `micropython_esp32_stubs-1.20.0.post2/io.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/json.pyi` & `micropython_esp32_stubs-1.20.0.post2/json.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/LICENSE.md` & `micropython_esp32_stubs-1.20.0.post2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/logging.pyi` & `micropython_esp32_stubs-1.20.0.post2/logging.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/machine.pyi` & `micropython_esp32_stubs-1.20.0.post2/machine.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/math.pyi` & `micropython_esp32_stubs-1.20.0.post2/math.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/micropython.pyi` & `micropython_esp32_stubs-1.20.0.post2/micropython_.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/mip/__init__.pyi` & `micropython_esp32_stubs-1.20.0.post2/mip/__init__.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/network.pyi` & `micropython_esp32_stubs-1.20.0.post2/network.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/onewire.pyi` & `micropython_esp32_stubs-1.20.0.post2/onewire.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/os.pyi` & `micropython_esp32_stubs-1.20.0.post2/os.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/pyproject.toml` & `micropython_esp32_stubs-1.20.0.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropython-esp32-stubs"
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

### Comparing `micropython_esp32_stubs-1.20.0.post1/random.pyi` & `micropython_esp32_stubs-1.20.0.post2/random.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/README.md` & `micropython_esp32_stubs-1.20.0.post2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
 
 For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
  * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
 
 Included stubs:
-* StubSource.MERGED from `stubs/micropython-v1_20_0-esp32-merged`
-* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`
-* StubSource.CORE from `stubs/micropython-core`
+* Merged stubs from `stubs/micropython-v1_20_0-esp32-merged`
+* Frozen stubs from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`
+* Core stubs from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
 Documentation | micropython | - | - | v1.20.0 
 Core | micropython | esp32 | - | v1.20.0
```

### Comparing `micropython_esp32_stubs-1.20.0.post1/select.pyi` & `micropython_esp32_stubs-1.20.0.post2/select.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/socket.pyi` & `micropython_esp32_stubs-1.20.0.post2/socket.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/ssl.pyi` & `micropython_esp32_stubs-1.20.0.post2/ssl.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/struct.pyi` & `micropython_esp32_stubs-1.20.0.post2/struct.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/sys.pyi` & `micropython_esp32_stubs-1.20.0.post2/sys.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/time.pyi` & `micropython_esp32_stubs-1.20.0.post2/time.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/uarray.pyi` & `micropython_esp32_stubs-1.20.0.post2/uarray.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/uasyncio/core.pyi` & `micropython_esp32_stubs-1.20.0.post2/uasyncio/core.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/uasyncio/event.pyi` & `micropython_esp32_stubs-1.20.0.post2/uasyncio/event.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/uasyncio/stream.pyi` & `micropython_esp32_stubs-1.20.0.post2/uasyncio/stream.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/uasyncio/task.pyi` & `micropython_esp32_stubs-1.20.0.post2/uasyncio/task.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/ubinascii.pyi` & `micropython_esp32_stubs-1.20.0.post2/ubinascii.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/ubluetooth.pyi` & `micropython_esp32_stubs-1.20.0.post2/ubluetooth.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/ucollections.pyi` & `micropython_esp32_stubs-1.20.0.post2/ucollections.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/ucryptolib.pyi` & `micropython_esp32_stubs-1.20.0.post2/ucryptolib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/uctypes.pyi` & `micropython_esp32_stubs-1.20.0.post2/uctypes.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/uerrno.pyi` & `micropython_esp32_stubs-1.20.0.post2/uerrno.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/uhashlib.pyi` & `micropython_esp32_stubs-1.20.0.post2/uhashlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/uheapq.pyi` & `micropython_esp32_stubs-1.20.0.post2/uheapq.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/uio.pyi` & `micropython_esp32_stubs-1.20.0.post2/uio.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/ujson.pyi` & `micropython_esp32_stubs-1.20.0.post2/ujson.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/umachine.pyi` & `micropython_esp32_stubs-1.20.0.post2/umachine.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/umqtt/simple.pyi` & `micropython_esp32_stubs-1.20.0.post2/umqtt/simple.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/uos.pyi` & `micropython_esp32_stubs-1.20.0.post2/uos.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/upysh.pyi` & `micropython_esp32_stubs-1.20.0.post2/upysh.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/urandom.pyi` & `micropython_esp32_stubs-1.20.0.post2/urandom.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/urequests.pyi` & `micropython_esp32_stubs-1.20.0.post2/urequests.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/uselect.pyi` & `micropython_esp32_stubs-1.20.0.post2/uselect.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/usocket.pyi` & `micropython_esp32_stubs-1.20.0.post2/usocket.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/ussl.pyi` & `micropython_esp32_stubs-1.20.0.post2/ussl.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/ustruct.pyi` & `micropython_esp32_stubs-1.20.0.post2/ustruct.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/usys.pyi` & `micropython_esp32_stubs-1.20.0.post2/usys.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/utime.pyi` & `micropython_esp32_stubs-1.20.0.post2/utime.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/uzlib.pyi` & `micropython_esp32_stubs-1.20.0.post2/uzlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/webrepl.pyi` & `micropython_esp32_stubs-1.20.0.post2/webrepl.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/zlib.pyi` & `micropython_esp32_stubs-1.20.0.post2/zlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp32_stubs-1.20.0.post1/setup.py` & `micropython_esp32_stubs-1.20.0.post2/setup.py`

 * *Files 8% similar despite different names*

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
     'name': 'micropython-esp32-stubs',
-    'version': '1.20.0.post1',
+    'version': '1.20.0.post2',
     'description': 'MicroPython stubs',
-    'long_description': '# micropython-esp32-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* StubSource.MERGED from `stubs/micropython-v1_20_0-esp32-merged`\n* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`\n* StubSource.CORE from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nDocumentation | micropython | - | - | v1.20.0 \nCore | micropython | esp32 | - | v1.20.0 \n',
+    'long_description': '# micropython-esp32-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* Merged stubs from `stubs/micropython-v1_20_0-esp32-merged`\n* Frozen stubs from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`\n* Core stubs from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nDocumentation | micropython | - | - | v1.20.0 \nCore | micropython | esp32 | - | v1.20.0 \n',
     'author': 'josverl',
     'author_email': 'josverl@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josverl/micropython-stubs#micropython-stubs',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `micropython_esp32_stubs-1.20.0.post1/PKG-INFO` & `micropython_esp32_stubs-1.20.0.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-esp32-stubs
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
-* StubSource.MERGED from `stubs/micropython-v1_20_0-esp32-merged`
-* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`
-* StubSource.CORE from `stubs/micropython-core`
+* Merged stubs from `stubs/micropython-v1_20_0-esp32-merged`
+* Frozen stubs from `stubs/micropython-v1_20_0-frozen/esp32/GENERIC`
+* Core stubs from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
 Documentation | micropython | - | - | v1.20.0 
 Core | micropython | esp32 | - | v1.20.0
```

