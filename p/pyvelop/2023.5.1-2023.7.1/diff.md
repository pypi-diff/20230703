# Comparing `tmp/pyvelop-2023.5.1.tar.gz` & `tmp/pyvelop-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvelop-2023.5.1.tar", last modified: Mon May  8 20:19:42 2023, max compression
+gzip compressed data, was "pyvelop-2023.7.1.tar", last modified: Mon Jul  3 16:47:13 2023, max compression
```

## Comparing `pyvelop-2023.5.1.tar` & `pyvelop-2023.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 homeassistant-beta   (998) homeassistant-beta   (994)        0 2023-05-08 20:19:42.514030 pyvelop-2023.5.1/
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)     1669 2023-05-08 20:19:42.514030 pyvelop-2023.5.1/PKG-INFO
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)     1371 2023-04-29 07:12:49.000000 pyvelop-2023.5.1/README.rst
-drwxr-xr-x   0 homeassistant-beta   (998) homeassistant-beta   (994)        0 2023-05-08 20:19:42.510030 pyvelop-2023.5.1/pyvelop/
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)      686 2023-04-29 07:12:49.000000 pyvelop-2023.5.1/pyvelop/__init__.py
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)    35723 2023-05-08 19:57:37.000000 pyvelop-2023.5.1/pyvelop/__main__.py
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)     6988 2023-04-29 07:12:49.000000 pyvelop-2023.5.1/pyvelop/base.py
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)      217 2023-05-08 20:15:43.000000 pyvelop-2023.5.1/pyvelop/const.py
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)      574 2023-04-29 07:12:49.000000 pyvelop-2023.5.1/pyvelop/decorators.py
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)    12289 2023-05-04 20:04:14.000000 pyvelop-2023.5.1/pyvelop/device.py
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)     2782 2023-04-29 07:12:49.000000 pyvelop-2023.5.1/pyvelop/exceptions.py
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)    11823 2023-04-29 07:12:49.000000 pyvelop-2023.5.1/pyvelop/jnap.py
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)      764 2023-04-29 07:12:49.000000 pyvelop-2023.5.1/pyvelop/logger.py
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)    61064 2023-05-08 19:57:37.000000 pyvelop-2023.5.1/pyvelop/mesh.py
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)     5242 2023-04-29 07:12:49.000000 pyvelop-2023.5.1/pyvelop/node.py
-drwxr-xr-x   0 homeassistant-beta   (998) homeassistant-beta   (994)        0 2023-05-08 20:19:42.514030 pyvelop-2023.5.1/pyvelop.egg-info/
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)     1669 2023-05-08 20:19:42.000000 pyvelop-2023.5.1/pyvelop.egg-info/PKG-INFO
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)      374 2023-05-08 20:19:42.000000 pyvelop-2023.5.1/pyvelop.egg-info/SOURCES.txt
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)        1 2023-05-08 20:19:42.000000 pyvelop-2023.5.1/pyvelop.egg-info/dependency_links.txt
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)        8 2023-05-08 20:19:42.000000 pyvelop-2023.5.1/pyvelop.egg-info/requires.txt
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)        8 2023-05-08 20:19:42.000000 pyvelop-2023.5.1/pyvelop.egg-info/top_level.txt
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)       38 2023-05-08 20:19:42.518030 pyvelop-2023.5.1/setup.cfg
--rw-r--r--   0 homeassistant-beta   (998) homeassistant-beta   (994)      710 2023-04-29 07:12:49.000000 pyvelop-2023.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:47:13.889329 pyvelop-2023.7.1/
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-07-03 16:47:13.889329 pyvelop-2023.7.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-07-03 15:56:35.000000 pyvelop-2023.7.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:47:13.861329 pyvelop-2023.7.1/pyvelop/
+-rw-r--r--   0 root         (0) root         (0)      686 2023-07-03 15:56:35.000000 pyvelop-2023.7.1/pyvelop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36316 2023-07-03 16:27:01.000000 pyvelop-2023.7.1/pyvelop/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6988 2023-07-03 15:56:35.000000 pyvelop-2023.7.1/pyvelop/base.py
+-rw-r--r--   0 root         (0) root         (0)      217 2023-07-03 16:29:00.000000 pyvelop-2023.7.1/pyvelop/const.py
+-rw-r--r--   0 root         (0) root         (0)      574 2023-07-03 15:56:35.000000 pyvelop-2023.7.1/pyvelop/decorators.py
+-rw-r--r--   0 root         (0) root         (0)    12289 2023-07-03 15:56:35.000000 pyvelop-2023.7.1/pyvelop/device.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-07-03 15:56:35.000000 pyvelop-2023.7.1/pyvelop/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    11823 2023-07-03 15:56:35.000000 pyvelop-2023.7.1/pyvelop/jnap.py
+-rw-r--r--   0 root         (0) root         (0)      764 2023-07-03 15:56:35.000000 pyvelop-2023.7.1/pyvelop/logger.py
+-rw-r--r--   0 root         (0) root         (0)    61095 2023-07-03 16:28:43.000000 pyvelop-2023.7.1/pyvelop/mesh.py
+-rw-r--r--   0 root         (0) root         (0)     5242 2023-07-03 15:56:35.000000 pyvelop-2023.7.1/pyvelop/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:47:13.881329 pyvelop-2023.7.1/pyvelop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-07-03 16:47:12.000000 pyvelop-2023.7.1/pyvelop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      374 2023-07-03 16:47:13.000000 pyvelop-2023.7.1/pyvelop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 16:47:12.000000 pyvelop-2023.7.1/pyvelop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-03 16:47:12.000000 pyvelop-2023.7.1/pyvelop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-03 16:47:12.000000 pyvelop-2023.7.1/pyvelop.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 16:47:13.889329 pyvelop-2023.7.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      710 2023-07-03 15:56:35.000000 pyvelop-2023.7.1/setup.py
```

### Comparing `pyvelop-2023.5.1/PKG-INFO` & `pyvelop-2023.7.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: pyvelop
-Version: 2023.5.1
+Version: 2023.7.1
 Summary: A Python library for the Linksys Velop Mesh system
 Home-page: https://github.com/uvjim/pyvelop
 Author: uvjim
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 pyvelop
 =======
 
 A Python library for the Linksys Velop Mesh system
@@ -60,9 +58,7 @@
 
 ``pyvelop --help`` - *show all available options*
 
 Disclaimer
 ==========
 
 This is **NOT** an official module, and it is **NOT** officially supported by the vendor.
-
-
```

### Comparing `pyvelop-2023.5.1/README.rst` & `pyvelop-2023.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.5.1/pyvelop/__init__.py` & `pyvelop-2023.7.1/pyvelop/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.5.1/pyvelop/__main__.py` & `pyvelop-2023.7.1/pyvelop/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,16 +237,30 @@
     **_,
 ) -> None:
     """Block/Unblock access to the internet."""
     if mesh_obj := await mesh_connect(ctx):
         async with mesh_obj:
             await mesh_obj.async_gather_details()
             try:
-                await mesh_obj.async_device_internet_access_state(
-                    device_id=device_id, state=not block
+                if not block:
+                    rules_to_apply: Dict[str, str] = {}
+                else:
+                    rules_to_apply: Dict[str, str] = dict(
+                        map(
+                            lambda weekday, readable_schedule: (
+                                weekday.name,
+                                readable_schedule,
+                            ),
+                            ParentalControl.WEEKDAYS,
+                            ("00:00-00:00",) * len(ParentalControl.WEEKDAYS),
+                        )
+                    )
+                await mesh_obj.async_set_parental_control_rules(
+                    device_id=device_id,
+                    rules=rules_to_apply,
                 )
             except MeshDeviceNotFoundResponse as err:
                 _LOGGER.error("Device not found: %s", err.devices[0])
             except MeshException as err:
                 _LOGGER.error(err)
```

### Comparing `pyvelop-2023.5.1/pyvelop/base.py` & `pyvelop-2023.7.1/pyvelop/base.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.5.1/pyvelop/decorators.py` & `pyvelop-2023.7.1/pyvelop/decorators.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.5.1/pyvelop/device.py` & `pyvelop-2023.7.1/pyvelop/device.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.5.1/pyvelop/exceptions.py` & `pyvelop-2023.7.1/pyvelop/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.5.1/pyvelop/jnap.py` & `pyvelop-2023.7.1/pyvelop/jnap.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.5.1/pyvelop/logger.py` & `pyvelop-2023.7.1/pyvelop/logger.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.5.1/pyvelop/mesh.py` & `pyvelop-2023.7.1/pyvelop/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -978,15 +978,15 @@
             if cached_schedule:
                 _LOGGER.debug(
                     self._log_formatter.format("Restoring backed up schedule")
                 )
                 new_rule = ParentalControl.backup_to_binary(schedule=cached_schedule)
                 this_device_rules[0]["wanSchedule"] = new_rule
             else:
-                if this_device_rules[0].get("blockedURLs", []):
+                if len(this_device_rules) > 0 and this_device_rules[0].get("blockedURLs", []):
                     _LOGGER.debug(
                         self._log_formatter.format(
                             "Blocked URLs found, applying permissive rule"
                         )
                     )
                     this_device_rules[0]["wanSchedule"] = new_rule
                 else:
```

### Comparing `pyvelop-2023.5.1/pyvelop/node.py` & `pyvelop-2023.7.1/pyvelop/node.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2023.5.1/pyvelop.egg-info/PKG-INFO` & `pyvelop-2023.7.1/pyvelop.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: pyvelop
-Version: 2023.5.1
+Version: 2023.7.1
 Summary: A Python library for the Linksys Velop Mesh system
 Home-page: https://github.com/uvjim/pyvelop
 Author: uvjim
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 pyvelop
 =======
 
 A Python library for the Linksys Velop Mesh system
@@ -60,9 +58,7 @@
 
 ``pyvelop --help`` - *show all available options*
 
 Disclaimer
 ==========
 
 This is **NOT** an official module, and it is **NOT** officially supported by the vendor.
-
-
```

### Comparing `pyvelop-2023.5.1/setup.py` & `pyvelop-2023.7.1/setup.py`

 * *Files identical despite different names*

