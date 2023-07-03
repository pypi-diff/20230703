# Comparing `tmp/micropython_hints-0.0.4.tar.gz` & `tmp/micropython_hints-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_hints-0.0.4.tar", last modified: Mon Jul  3 07:00:32 2023, max compression
+gzip compressed data, was "micropython_hints-0.0.5.tar", last modified: Mon Jul  3 07:56:45 2023, max compression
```

## Comparing `micropython_hints-0.0.4.tar` & `micropython_hints-0.0.5.tar`

### file list

```diff
@@ -1,73 +1,14 @@
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-03 07:00:32.960814 micropython_hints-0.0.4/
--rw-r--r--   0 meo       (1000) meo       (1000)      446 2023-07-03 07:00:32.960814 micropython_hints-0.0.4/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)       23 2023-07-03 04:14:50.000000 micropython_hints-0.0.4/README.md
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-03 07:00:32.957481 micropython_hints-0.0.4/micropython_hints/
--rw-r--r--   0 meo       (1000) meo       (1000)     1137 2023-07-03 06:59:49.000000 micropython_hints-0.0.4/micropython_hints/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)      697 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/_thread.py
--rw-r--r--   0 meo       (1000) meo       (1000)     8365 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/array.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1606 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/binascii.py
--rw-r--r--   0 meo       (1000) meo       (1000)    55976 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/bluetooth.py
--rw-r--r--   0 meo       (1000) meo       (1000)     8754 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/btree.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1976 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/cmath.py
--rw-r--r--   0 meo       (1000) meo       (1000)     5828 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/collections.py
--rw-r--r--   0 meo       (1000) meo       (1000)     3766 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/cryptolib.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1850 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/errno.py
--rw-r--r--   0 meo       (1000) meo       (1000)     8518 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/esp.py
--rw-r--r--   0 meo       (1000) meo       (1000)    18158 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/esp32.py
--rw-r--r--   0 meo       (1000) meo       (1000)     8369 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/framebuf.py
--rw-r--r--   0 meo       (1000) meo       (1000)     3948 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/gc.py
--rw-r--r--   0 meo       (1000) meo       (1000)     3667 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/hashlib.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1291 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/heapq.py
--rw-r--r--   0 meo       (1000) meo       (1000)    18578 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/io.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1793 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/json.py
--rw-r--r--   0 meo       (1000) meo       (1000)    21847 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/lcd160cr.py
--rw-r--r--   0 meo       (1000) meo       (1000)     4002 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/machine.ADCWiPy.py
--rw-r--r--   0 meo       (1000) meo       (1000)    12210 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/machine.TimerWiPy.py
--rw-r--r--   0 meo       (1000) meo       (1000)   102731 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/machine.py
--rw-r--r--   0 meo       (1000) meo       (1000)     5209 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/math.py
--rw-r--r--   0 meo       (1000) meo       (1000)    11660 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/micropython.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2552 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/neopixel.py
--rw-r--r--   0 meo       (1000) meo       (1000)    35185 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/network.py
--rw-r--r--   0 meo       (1000) meo       (1000)    28184 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/os.py
--rw-r--r--   0 meo       (1000) meo       (1000)   183891 2023-07-03 06:50:09.000000 micropython_hints-0.0.4/micropython_hints/pyb.py
--rw-r--r--   0 meo       (1000) meo       (1000)     4298 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/random.py
--rw-r--r--   0 meo       (1000) meo       (1000)     8251 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/re.py
--rw-r--r--   0 meo       (1000) meo       (1000)     5045 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/select.py
--rw-r--r--   0 meo       (1000) meo       (1000)    18453 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/socket.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2707 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/ssl.py
--rw-r--r--   0 meo       (1000) meo       (1000)     7730 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/stm.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2132 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/struct.py
--rw-r--r--   0 meo       (1000) meo       (1000)     6209 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/sys.py
--rw-r--r--   0 meo       (1000) meo       (1000)    13414 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/time.py
--rw-r--r--   0 meo       (1000) meo       (1000)     8365 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/uarray.py
--rw-r--r--   0 meo       (1000) meo       (1000)    12303 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/uasyncio.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1606 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/ubinascii.py
--rw-r--r--   0 meo       (1000) meo       (1000)    55976 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/ubluetooth.py
--rw-r--r--   0 meo       (1000) meo       (1000)     5828 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/ucollections.py
--rw-r--r--   0 meo       (1000) meo       (1000)     3766 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/ucryptolib.py
--rw-r--r--   0 meo       (1000) meo       (1000)    11686 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/uctypes.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1850 2023-07-03 04:04:26.000000 micropython_hints-0.0.4/micropython_hints/uerrno.py
--rw-r--r--   0 meo       (1000) meo       (1000)     3667 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/uhashlib.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1291 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/uheapq.py
--rw-r--r--   0 meo       (1000) meo       (1000)    18578 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/uio.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1793 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/ujson.py
--rw-r--r--   0 meo       (1000) meo       (1000)    28184 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/uos.py
--rw-r--r--   0 meo       (1000) meo       (1000)     8251 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/ure.py
--rw-r--r--   0 meo       (1000) meo       (1000)     5045 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/uselect.py
--rw-r--r--   0 meo       (1000) meo       (1000)    18453 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/usocket.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2707 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/ussl.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2132 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/ustruct.py
--rw-r--r--   0 meo       (1000) meo       (1000)     6209 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/usys.py
--rw-r--r--   0 meo       (1000) meo       (1000)    13414 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/utime.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2059 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/uzlib.py
--rw-r--r--   0 meo       (1000) meo       (1000)      993 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/wipy.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2059 2023-07-03 04:00:49.000000 micropython_hints-0.0.4/micropython_hints/zlib.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-03 07:00:32.960814 micropython_hints-0.0.4/micropython_hints.egg-info/
--rw-r--r--   0 meo       (1000) meo       (1000)      446 2023-07-03 07:00:32.000000 micropython_hints-0.0.4/micropython_hints.egg-info/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)     1958 2023-07-03 07:00:32.000000 micropython_hints-0.0.4/micropython_hints.egg-info/SOURCES.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-07-03 07:00:32.000000 micropython_hints-0.0.4/micropython_hints.egg-info/dependency_links.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       94 2023-07-03 07:00:32.000000 micropython_hints-0.0.4/micropython_hints.egg-info/entry_points.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        5 2023-07-03 07:00:32.000000 micropython_hints-0.0.4/micropython_hints.egg-info/requires.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       18 2023-07-03 07:00:32.000000 micropython_hints-0.0.4/micropython_hints.egg-info/top_level.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-07-03 07:00:32.960814 micropython_hints-0.0.4/setup.cfg
--rw-r--r--   0 meo       (1000) meo       (1000)     1344 2023-07-03 07:00:23.000000 micropython_hints-0.0.4/setup.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-03 07:56:45.622306 micropython_hints-0.0.5/
+-rw-r--r--   0 meo       (1000) meo       (1000)      446 2023-07-03 07:56:45.618973 micropython_hints-0.0.5/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)       23 2023-07-03 04:14:50.000000 micropython_hints-0.0.5/README.md
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-03 07:56:45.618973 micropython_hints-0.0.5/micropython_hints/
+-rw-r--r--   0 meo       (1000) meo       (1000)     1137 2023-07-03 06:59:49.000000 micropython_hints-0.0.5/micropython_hints/__init__.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-03 07:56:45.618973 micropython_hints-0.0.5/micropython_hints.egg-info/
+-rw-r--r--   0 meo       (1000) meo       (1000)      446 2023-07-03 07:56:45.000000 micropython_hints-0.0.5/micropython_hints.egg-info/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      296 2023-07-03 07:56:45.000000 micropython_hints-0.0.5/micropython_hints.egg-info/SOURCES.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-07-03 07:56:45.000000 micropython_hints-0.0.5/micropython_hints.egg-info/dependency_links.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       94 2023-07-03 07:56:45.000000 micropython_hints-0.0.5/micropython_hints.egg-info/entry_points.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        5 2023-07-03 07:56:45.000000 micropython_hints-0.0.5/micropython_hints.egg-info/requires.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       18 2023-07-03 07:56:45.000000 micropython_hints-0.0.5/micropython_hints.egg-info/top_level.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-07-03 07:56:45.622306 micropython_hints-0.0.5/setup.cfg
+-rw-r--r--   0 meo       (1000) meo       (1000)     1344 2023-07-03 07:56:41.000000 micropython_hints-0.0.5/setup.py
```

### Comparing `micropython_hints-0.0.4/micropython_hints/__init__.py` & `micropython_hints-0.0.5/micropython_hints/__init__.py`

 * *Files identical despite different names*

### Comparing `micropython_hints-0.0.4/setup.py` & `micropython_hints-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 URL = f"https://github.com/miaobuao/{PROJ_NAME}"
 
 setup(
     name         = PROJ_NAME,
     author       =  "miaobuao",
     url          =  URL,
     description  =  "MicroPython type hints",
-    version      =  "0.0.4",
+    version      =  "0.0.5",
     license      =  "MIT License",
     author_email =  "miaobuao@outlook.com",
     long_description     = long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

