# Comparing `tmp/linien-client-0.8.0rc2.tar.gz` & `tmp/linien-client-0.8.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-client-0.8.0rc2.tar", last modified: Mon Jul  3 12:45:07 2023, max compression
+gzip compressed data, was "linien-client-0.8.0rc4.tar", last modified: Mon Jul  3 13:55:19 2023, max compression
```

## Comparing `linien-client-0.8.0rc2.tar` & `linien-client-0.8.0rc4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:45:07.687663 linien-client-0.8.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-03 12:45:07.687663 linien-client-0.8.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:45:07.683663 linien-client-0.8.0rc2/linien_client/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 12:44:27.000000 linien-client-0.8.0rc2/linien_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-03 12:44:27.000000 linien-client-0.8.0rc2/linien_client/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-03 12:44:27.000000 linien-client-0.8.0rc2/linien_client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-03 12:44:27.000000 linien-client-0.8.0rc2/linien_client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-03 12:44:27.000000 linien-client-0.8.0rc2/linien_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-03 12:44:27.000000 linien-client-0.8.0rc2/linien_client/remote_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:45:07.687663 linien-client-0.8.0rc2/linien_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-03 12:45:07.000000 linien-client-0.8.0rc2/linien_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 12:45:07.000000 linien-client-0.8.0rc2/linien_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:45:07.000000 linien-client-0.8.0rc2/linien_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 12:45:07.000000 linien-client-0.8.0rc2/linien_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 12:45:07.000000 linien-client-0.8.0rc2/linien_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:45:07.687663 linien-client-0.8.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-03 12:44:27.000000 linien-client-0.8.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:55:19.410786 linien-client-0.8.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-03 13:55:19.410786 linien-client-0.8.0rc4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:55:19.410786 linien-client-0.8.0rc4/linien_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 13:54:39.000000 linien-client-0.8.0rc4/linien_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-03 13:54:39.000000 linien-client-0.8.0rc4/linien_client/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-03 13:54:39.000000 linien-client-0.8.0rc4/linien_client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-03 13:54:39.000000 linien-client-0.8.0rc4/linien_client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-03 13:54:39.000000 linien-client-0.8.0rc4/linien_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-03 13:54:39.000000 linien-client-0.8.0rc4/linien_client/remote_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:55:19.410786 linien-client-0.8.0rc4/linien_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-03 13:55:19.000000 linien-client-0.8.0rc4/linien_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 13:55:19.000000 linien-client-0.8.0rc4/linien_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:55:19.000000 linien-client-0.8.0rc4/linien_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 13:55:19.000000 linien-client-0.8.0rc4/linien_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 13:55:19.000000 linien-client-0.8.0rc4/linien_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:55:19.410786 linien-client-0.8.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-03 13:54:39.000000 linien-client-0.8.0rc4/setup.py
```

### Comparing `linien-client-0.8.0rc2/PKG-INFO` & `linien-client-0.8.0rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-client
-Version: 0.8.0rc2
+Version: 0.8.0rc4
 Summary: Client components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien/
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-client-0.8.0rc2/linien_client/communication.py` & `linien-client-0.8.0rc4/linien_client/communication.py`

 * *Files identical despite different names*

### Comparing `linien-client-0.8.0rc2/linien_client/connection.py` & `linien-client-0.8.0rc4/linien_client/connection.py`

 * *Files identical despite different names*

### Comparing `linien-client-0.8.0rc2/linien_client/deploy.py` & `linien-client-0.8.0rc4/linien_client/deploy.py`

 * *Files identical despite different names*

### Comparing `linien-client-0.8.0rc2/linien_client/exceptions.py` & `linien-client-0.8.0rc4/linien_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `linien-client-0.8.0rc2/linien_client/remote_parameters.py` & `linien-client-0.8.0rc4/linien_client/remote_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
-import pickle
 from typing import Any, Callable, Dict, Iterator, List, Tuple, Union
 
+from linien_common.communication import pack, unpack
 from rpyc import async_
 from rpyc.core.async_ import AsyncResult
 
 from .communication import LinienControlService
 
 
 class RemoteParameter:
@@ -45,20 +45,20 @@
         self.log = log
 
     @property
     def value(self) -> Any:
         """Return the locally cached value (if it exists). Otherwise ask the server."""
         if hasattr(self, "_cached_value"):
             return self._cached_value
-        return pickle.loads(self.parent.remote.exposed_get_param(self.name))
+        return unpack(self.parent.remote.exposed_get_param(self.name))
 
     @value.setter
     def value(self, value: Any):
         """Notify the server of the new value"""
-        return self.parent.remote.exposed_set_param(self.name, pickle.dumps(value))
+        return self.parent.remote.exposed_set_param(self.name, pack(value))
 
     @property
     def log(self) -> bool:
         return self.parent.remote.exposed_get_parameter_log(self.name)
 
     @log.setter
     def log(self, value: bool) -> None:
@@ -108,17 +108,15 @@
         self._async_changed_parameters_queue: Union[AsyncResult, None] = None
         self._async_listener_registering: Union[AsyncResult, None] = None
 
         self._listeners_pending_remote_registration: List[str] = []
         self._callbacks: Dict[str, List[Callable]] = {}
 
         # mimic functionality of `parameters.Parameters`:
-        all_parameters = pickle.loads(
-            self.remote.exposed_init_parameter_sync(self.uuid)
-        )
+        all_parameters = unpack(self.remote.exposed_init_parameter_sync(self.uuid))
         for name, value, can_be_cached, restorable, loggable, log in all_parameters:
             param = RemoteParameter(
                 parent=self,
                 name=name,
                 use_cache=use_cache and can_be_cached,
                 restorable=restorable,
                 loggable=loggable,
@@ -186,15 +184,15 @@
                 self._listeners_pending_remote_registration.clear()
 
         if (
             self._async_changed_parameters_queue is not None
             and self._async_changed_parameters_queue.ready
         ):
             # We have a result.
-            queue: List[Tuple[str, Any]] = pickle.loads(
+            queue: List[Tuple[str, Any]] = unpack(
                 self._async_changed_parameters_queue.value
             )
 
             # Now that we have our result, we can start the next call.
             self._async_changed_parameters_queue = async_(
                 self.remote.exposed_get_changed_parameters_queue
             )(self.uuid)
```

### Comparing `linien-client-0.8.0rc2/linien_client.egg-info/PKG-INFO` & `linien-client-0.8.0rc4/linien_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-client
-Version: 0.8.0rc2
+Version: 0.8.0rc4
 Summary: Client components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien/
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-client-0.8.0rc2/setup.py` & `linien-client-0.8.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
-version = "0.8.0rc2"
+version = "0.8.0rc4"
 
 setup(
     name="linien-client",
     version=version,
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
```

