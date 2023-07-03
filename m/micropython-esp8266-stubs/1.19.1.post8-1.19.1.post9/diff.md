# Comparing `tmp/micropython_esp8266_stubs-1.19.1.post8.tar.gz` & `tmp/micropython_esp8266_stubs-1.19.1.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_esp8266_stubs-1.19.1.post8.tar", max compression
+gzip compressed data, was "micropython_esp8266_stubs-1.19.1.post9.tar", max compression
```

## Comparing `micropython_esp8266_stubs-1.19.1.post8.tar` & `micropython_esp8266_stubs-1.19.1.post9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     1070 2023-01-16 00:45:13.571132 micropython_esp8266_stubs-1.19.1.post8/LICENSE.md
--rw-r--r--   0        0        0     2044 2023-01-16 00:45:13.571132 micropython_esp8266_stubs-1.19.1.post8/README.md
--rw-r--r--   0        0        0        0 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/_boot.pyi
--rw-r--r--   0        0        0      269 2023-01-16 00:44:33.643086 micropython_esp8266_stubs-1.19.1.post8/_onewire.pyi
--rw-r--r--   0        0        0      245 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/apa102.pyi
--rw-r--r--   0        0        0     1017 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/array.pyi
--rw-r--r--   0        0        0     1326 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/binascii.pyi
--rw-r--r--   0        0        0     3670 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/btree.pyi
--rw-r--r--   0        0        0      329 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/dht.pyi
--rw-r--r--   0        0        0      389 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/ds18x20.pyi
--rw-r--r--   0        0        0      676 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/errno.pyi
--rw-r--r--   0        0        0     5146 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/esp.pyi
--rw-r--r--   0        0        0      403 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/flashbdev.pyi
--rw-r--r--   0        0        0     4787 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/framebuf.pyi
--rw-r--r--   0        0        0     1935 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/gc.pyi
--rw-r--r--   0        0        0     1600 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/hashlib.pyi
--rw-r--r--   0        0        0      897 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/heapq.pyi
--rw-r--r--   0        0        0       98 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/inisetup.pyi
--rw-r--r--   0        0        0     1339 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/json.pyi
--rw-r--r--   0        0        0     1323 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/lwip.pyi
--rw-r--r--   0        0        0    39924 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/machine.pyi
--rw-r--r--   0        0        0     3082 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/math.pyi
--rw-r--r--   0        0        0     7055 2023-01-16 00:44:33.363086 micropython_esp8266_stubs-1.19.1.post8/micropython.pyi
--rw-r--r--   0        0        0      433 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/neopixel.pyi
--rw-r--r--   0        0        0     6963 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/network.pyi
--rw-r--r--   0        0        0       69 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/ntptime.pyi
--rw-r--r--   0        0        0      596 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/onewire.pyi
--rw-r--r--   0        0        0     8096 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/os.pyi
--rw-r--r--   0        0        0       24 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/port_diag.pyi
--rw-r--r--   0        0        0     3279 2023-01-16 00:45:14.007132 micropython_esp8266_stubs-1.19.1.post8/pyproject.toml
--rw-r--r--   0        0        0     1510 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/random.pyi
--rw-r--r--   0        0        0     3760 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/select.pyi
--rw-r--r--   0        0        0     9417 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/socket.pyi
--rw-r--r--   0        0        0     1836 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/ssl.pyi
--rw-r--r--   0        0        0     1521 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/struct.pyi
--rw-r--r--   0        0        0      820 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/sys.pyi
--rw-r--r--   0        0        0    12180 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/time.pyi
--rw-r--r--   0        0        0     1017 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/uarray.pyi
--rw-r--r--   0        0        0     1326 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/ubinascii.pyi
--rw-r--r--   0        0        0     3526 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/ucollections.pyi
--rw-r--r--   0        0        0     1608 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/ucryptolib.pyi
--rw-r--r--   0        0        0     2277 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/uctypes.pyi
--rw-r--r--   0        0        0      676 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/uerrno.pyi
--rw-r--r--   0        0        0     1600 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/uhashlib.pyi
--rw-r--r--   0        0        0      897 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/uheapq.pyi
--rw-r--r--   0        0        0     3914 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/uio.pyi
--rw-r--r--   0        0        0     1339 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/ujson.pyi
--rw-r--r--   0        0        0    39924 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/umachine.pyi
--rw-r--r--   0        0        0     8096 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/uos.pyi
--rw-r--r--   0        0        0      717 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/upip.pyi
--rw-r--r--   0        0        0      689 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/upip_utarfile.pyi
--rw-r--r--   0        0        0     1510 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/urandom.pyi
--rw-r--r--   0        0        0      181 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/ure.pyi
--rw-r--r--   0        0        0     3760 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/uselect.pyi
--rw-r--r--   0        0        0     9417 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/usocket.pyi
--rw-r--r--   0        0        0     1836 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/ussl.pyi
--rw-r--r--   0        0        0     1521 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/ustruct.pyi
--rw-r--r--   0        0        0      820 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/usys.pyi
--rw-r--r--   0        0        0    12180 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/utime.pyi
--rw-r--r--   0        0        0      238 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/utimeq.pyi
--rw-r--r--   0        0        0      393 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/uwebsocket.pyi
--rw-r--r--   0        0        0     1503 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/uzlib.pyi
--rw-r--r--   0        0        0      366 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/webrepl.pyi
--rw-r--r--   0        0        0      222 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/webrepl_setup.pyi
--rw-r--r--   0        0        0      393 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/websocket.pyi
--rw-r--r--   0        0        0       92 2023-01-16 00:44:33.663086 micropython_esp8266_stubs-1.19.1.post8/websocket_helper.pyi
--rw-r--r--   0        0        0     1503 2023-01-16 00:44:33.647086 micropython_esp8266_stubs-1.19.1.post8/zlib.pyi
--rw-r--r--   0        0        0     3444 1970-01-01 00:00:00.000000 micropython_esp8266_stubs-1.19.1.post8/setup.py
--rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 micropython_esp8266_stubs-1.19.1.post8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-01-16 08:09:16.027548 micropython_esp8266_stubs-1.19.1.post9/LICENSE.md
+-rw-r--r--   0        0        0     2044 2023-01-16 08:09:16.027548 micropython_esp8266_stubs-1.19.1.post9/README.md
+-rw-r--r--   0        0        0        0 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/_boot.pyi
+-rw-r--r--   0        0        0      269 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/_onewire.pyi
+-rw-r--r--   0        0        0      245 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/apa102.pyi
+-rw-r--r--   0        0        0     1017 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/array.pyi
+-rw-r--r--   0        0        0     1326 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/binascii.pyi
+-rw-r--r--   0        0        0     3670 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/btree.pyi
+-rw-r--r--   0        0        0      329 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/dht.pyi
+-rw-r--r--   0        0        0      389 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/ds18x20.pyi
+-rw-r--r--   0        0        0      676 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/errno.pyi
+-rw-r--r--   0        0        0     5146 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/esp.pyi
+-rw-r--r--   0        0        0      403 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/flashbdev.pyi
+-rw-r--r--   0        0        0     4787 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/framebuf.pyi
+-rw-r--r--   0        0        0     1935 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/gc.pyi
+-rw-r--r--   0        0        0     1600 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/hashlib.pyi
+-rw-r--r--   0        0        0      897 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/heapq.pyi
+-rw-r--r--   0        0        0       98 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/inisetup.pyi
+-rw-r--r--   0        0        0     1339 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/json.pyi
+-rw-r--r--   0        0        0     1323 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/lwip.pyi
+-rw-r--r--   0        0        0    39924 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/machine.pyi
+-rw-r--r--   0        0        0     3082 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/math.pyi
+-rw-r--r--   0        0        0     7055 2023-01-16 08:08:33.968085 micropython_esp8266_stubs-1.19.1.post9/micropython.pyi
+-rw-r--r--   0        0        0      433 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/neopixel.pyi
+-rw-r--r--   0        0        0     6963 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/network.pyi
+-rw-r--r--   0        0        0       69 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/ntptime.pyi
+-rw-r--r--   0        0        0      596 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/onewire.pyi
+-rw-r--r--   0        0        0     8096 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/os.pyi
+-rw-r--r--   0        0        0       24 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/port_diag.pyi
+-rw-r--r--   0        0        0     3279 2023-01-16 08:09:16.527541 micropython_esp8266_stubs-1.19.1.post9/pyproject.toml
+-rw-r--r--   0        0        0     1510 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/random.pyi
+-rw-r--r--   0        0        0     3760 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/select.pyi
+-rw-r--r--   0        0        0     9417 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/socket.pyi
+-rw-r--r--   0        0        0     1836 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/ssl.pyi
+-rw-r--r--   0        0        0     1521 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/struct.pyi
+-rw-r--r--   0        0        0      820 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/sys.pyi
+-rw-r--r--   0        0        0    12180 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/time.pyi
+-rw-r--r--   0        0        0     1017 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/uarray.pyi
+-rw-r--r--   0        0        0     1326 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/ubinascii.pyi
+-rw-r--r--   0        0        0     3526 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/ucollections.pyi
+-rw-r--r--   0        0        0     1608 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/ucryptolib.pyi
+-rw-r--r--   0        0        0     2277 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/uctypes.pyi
+-rw-r--r--   0        0        0      676 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/uerrno.pyi
+-rw-r--r--   0        0        0     1600 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/uhashlib.pyi
+-rw-r--r--   0        0        0      897 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/uheapq.pyi
+-rw-r--r--   0        0        0     3914 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/uio.pyi
+-rw-r--r--   0        0        0     1339 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/ujson.pyi
+-rw-r--r--   0        0        0    39924 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/umachine.pyi
+-rw-r--r--   0        0        0     8096 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/uos.pyi
+-rw-r--r--   0        0        0      717 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/upip.pyi
+-rw-r--r--   0        0        0      689 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/upip_utarfile.pyi
+-rw-r--r--   0        0        0     1510 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/urandom.pyi
+-rw-r--r--   0        0        0      181 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/ure.pyi
+-rw-r--r--   0        0        0     3760 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/uselect.pyi
+-rw-r--r--   0        0        0     9417 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/usocket.pyi
+-rw-r--r--   0        0        0     1836 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/ussl.pyi
+-rw-r--r--   0        0        0     1521 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/ustruct.pyi
+-rw-r--r--   0        0        0      820 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/usys.pyi
+-rw-r--r--   0        0        0    12180 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/utime.pyi
+-rw-r--r--   0        0        0      238 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/utimeq.pyi
+-rw-r--r--   0        0        0      393 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/uwebsocket.pyi
+-rw-r--r--   0        0        0     1503 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/uzlib.pyi
+-rw-r--r--   0        0        0      366 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/webrepl.pyi
+-rw-r--r--   0        0        0      222 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/webrepl_setup.pyi
+-rw-r--r--   0        0        0      393 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/websocket.pyi
+-rw-r--r--   0        0        0       92 2023-01-16 08:08:34.272081 micropython_esp8266_stubs-1.19.1.post9/websocket_helper.pyi
+-rw-r--r--   0        0        0     1503 2023-01-16 08:08:34.256082 micropython_esp8266_stubs-1.19.1.post9/zlib.pyi
+-rw-r--r--   0        0        0     3444 1970-01-01 00:00:00.000000 micropython_esp8266_stubs-1.19.1.post9/setup.py
+-rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 micropython_esp8266_stubs-1.19.1.post9/PKG-INFO
```

### Comparing `micropython_esp8266_stubs-1.19.1.post8/LICENSE.md` & `micropython_esp8266_stubs-1.19.1.post9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/README.md` & `micropython_esp8266_stubs-1.19.1.post9/README.md`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/array.pyi` & `micropython_esp8266_stubs-1.19.1.post9/array.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/binascii.pyi` & `micropython_esp8266_stubs-1.19.1.post9/binascii.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/btree.pyi` & `micropython_esp8266_stubs-1.19.1.post9/btree.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/errno.pyi` & `micropython_esp8266_stubs-1.19.1.post9/errno.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/esp.pyi` & `micropython_esp8266_stubs-1.19.1.post9/esp.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/framebuf.pyi` & `micropython_esp8266_stubs-1.19.1.post9/framebuf.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/gc.pyi` & `micropython_esp8266_stubs-1.19.1.post9/gc.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/hashlib.pyi` & `micropython_esp8266_stubs-1.19.1.post9/hashlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/heapq.pyi` & `micropython_esp8266_stubs-1.19.1.post9/heapq.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/json.pyi` & `micropython_esp8266_stubs-1.19.1.post9/json.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/lwip.pyi` & `micropython_esp8266_stubs-1.19.1.post9/lwip.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/machine.pyi` & `micropython_esp8266_stubs-1.19.1.post9/machine.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/math.pyi` & `micropython_esp8266_stubs-1.19.1.post9/math.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/micropython.pyi` & `micropython_esp8266_stubs-1.19.1.post9/micropython.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/network.pyi` & `micropython_esp8266_stubs-1.19.1.post9/network.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/onewire.pyi` & `micropython_esp8266_stubs-1.19.1.post9/onewire.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/os.pyi` & `micropython_esp8266_stubs-1.19.1.post9/os.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/pyproject.toml` & `micropython_esp8266_stubs-1.19.1.post9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropython-esp8266-stubs"
-version = "1.19.1.post8"
+version = "1.19.1.post9"
 description = "MicroPython stubs"
 authors = [
     "josverl <josverl@users.noreply.github.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/josverl/micropython-stubs#micropython-stubs"
```

### Comparing `micropython_esp8266_stubs-1.19.1.post8/random.pyi` & `micropython_esp8266_stubs-1.19.1.post9/random.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/select.pyi` & `micropython_esp8266_stubs-1.19.1.post9/select.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/socket.pyi` & `micropython_esp8266_stubs-1.19.1.post9/socket.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/ssl.pyi` & `micropython_esp8266_stubs-1.19.1.post9/ssl.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/struct.pyi` & `micropython_esp8266_stubs-1.19.1.post9/struct.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/sys.pyi` & `micropython_esp8266_stubs-1.19.1.post9/sys.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/time.pyi` & `micropython_esp8266_stubs-1.19.1.post9/time.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/uarray.pyi` & `micropython_esp8266_stubs-1.19.1.post9/uarray.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/ubinascii.pyi` & `micropython_esp8266_stubs-1.19.1.post9/ubinascii.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/ucollections.pyi` & `micropython_esp8266_stubs-1.19.1.post9/ucollections.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/ucryptolib.pyi` & `micropython_esp8266_stubs-1.19.1.post9/ucryptolib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/uctypes.pyi` & `micropython_esp8266_stubs-1.19.1.post9/uctypes.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/uerrno.pyi` & `micropython_esp8266_stubs-1.19.1.post9/uerrno.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/uhashlib.pyi` & `micropython_esp8266_stubs-1.19.1.post9/uhashlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/uheapq.pyi` & `micropython_esp8266_stubs-1.19.1.post9/uheapq.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/uio.pyi` & `micropython_esp8266_stubs-1.19.1.post9/uio.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/ujson.pyi` & `micropython_esp8266_stubs-1.19.1.post9/ujson.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/umachine.pyi` & `micropython_esp8266_stubs-1.19.1.post9/umachine.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/uos.pyi` & `micropython_esp8266_stubs-1.19.1.post9/uos.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/upip.pyi` & `micropython_esp8266_stubs-1.19.1.post9/upip.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/upip_utarfile.pyi` & `micropython_esp8266_stubs-1.19.1.post9/upip_utarfile.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/urandom.pyi` & `micropython_esp8266_stubs-1.19.1.post9/urandom.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/uselect.pyi` & `micropython_esp8266_stubs-1.19.1.post9/uselect.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/usocket.pyi` & `micropython_esp8266_stubs-1.19.1.post9/usocket.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/ussl.pyi` & `micropython_esp8266_stubs-1.19.1.post9/ussl.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/ustruct.pyi` & `micropython_esp8266_stubs-1.19.1.post9/ustruct.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/usys.pyi` & `micropython_esp8266_stubs-1.19.1.post9/usys.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/utime.pyi` & `micropython_esp8266_stubs-1.19.1.post9/utime.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/uzlib.pyi` & `micropython_esp8266_stubs-1.19.1.post9/uzlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/zlib.pyi` & `micropython_esp8266_stubs-1.19.1.post9/zlib.pyi`

 * *Files identical despite different names*

### Comparing `micropython_esp8266_stubs-1.19.1.post8/setup.py` & `micropython_esp8266_stubs-1.19.1.post9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
  'websocket_helper',
  'zlib']
 install_requires = \
 ['micropython-stdlib-stubs>=0.9.0']
 
 setup_kwargs = {
     'name': 'micropython-esp8266-stubs',
-    'version': '1.19.1.post8',
+    'version': '1.19.1.post9',
     'description': 'MicroPython stubs',
     'long_description': '# micropython-esp8266-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* Merged stubs from `stubs/micropython-v1_19_1-esp8266-merged`\n* Frozen stubs from `stubs/micropython-v1_19_1-frozen/esp8266/GENERIC`\n* Core Stubs from `stubs/cpython_core-pycopy`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nFirmware | micropython | esp8266 | ESP module (1M) with ESP8266 | v1.19.1 \nDocumentation | micropython | - | - | v1.19.1 \nCore | micropython | esp8266 | - | v1.19.1 \n',
     'author': 'josverl',
     'author_email': 'josverl@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josverl/micropython-stubs#micropython-stubs',
```

### Comparing `micropython_esp8266_stubs-1.19.1.post8/PKG-INFO` & `micropython_esp8266_stubs-1.19.1.post9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-esp8266-stubs
-Version: 1.19.1.post8
+Version: 1.19.1.post9
 Summary: MicroPython stubs
 Home-page: https://github.com/josverl/micropython-stubs#micropython-stubs
 License: MIT
 Author: josverl
 Author-email: josverl@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

