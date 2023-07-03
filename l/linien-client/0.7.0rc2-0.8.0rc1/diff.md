# Comparing `tmp/linien-client-0.7.0rc2.tar.gz` & `tmp/linien-client-0.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-client-0.7.0rc2.tar", last modified: Tue Mar 21 15:47:56 2023, max compression
+gzip compressed data, was "linien-client-0.8.0rc1.tar", last modified: Mon Jul  3 12:17:21 2023, max compression
```

## Comparing `linien-client-0.7.0rc2.tar` & `linien-client-0.8.0rc1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:56.521108 linien-client-0.7.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-21 15:47:56.521108 linien-client-0.7.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:56.521108 linien-client-0.7.0rc2/linien_client/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-21 15:47:14.000000 linien-client-0.7.0rc2/linien_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-03-21 15:47:14.000000 linien-client-0.7.0rc2/linien_client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-03-21 15:47:14.000000 linien-client-0.7.0rc2/linien_client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-21 15:47:14.000000 linien-client-0.7.0rc2/linien_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-03-21 15:47:14.000000 linien-client-0.7.0rc2/linien_client/remote_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:56.521108 linien-client-0.7.0rc2/linien_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-21 15:47:56.000000 linien-client-0.7.0rc2/linien_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-21 15:47:56.000000 linien-client-0.7.0rc2/linien_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:47:56.000000 linien-client-0.7.0rc2/linien_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-21 15:47:56.000000 linien-client-0.7.0rc2/linien_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-21 15:47:56.000000 linien-client-0.7.0rc2/linien_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 15:47:56.521108 linien-client-0.7.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-21 15:47:14.000000 linien-client-0.7.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:17:21.773297 linien-client-0.8.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-03 12:17:21.769297 linien-client-0.8.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:17:21.769297 linien-client-0.8.0rc1/linien_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 12:16:37.000000 linien-client-0.8.0rc1/linien_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-03 12:16:37.000000 linien-client-0.8.0rc1/linien_client/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-03 12:16:37.000000 linien-client-0.8.0rc1/linien_client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-03 12:16:37.000000 linien-client-0.8.0rc1/linien_client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-03 12:16:37.000000 linien-client-0.8.0rc1/linien_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-03 12:16:37.000000 linien-client-0.8.0rc1/linien_client/remote_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:17:21.769297 linien-client-0.8.0rc1/linien_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-03 12:17:21.000000 linien-client-0.8.0rc1/linien_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 12:17:21.000000 linien-client-0.8.0rc1/linien_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:17:21.000000 linien-client-0.8.0rc1/linien_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 12:17:21.000000 linien-client-0.8.0rc1/linien_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 12:17:21.000000 linien-client-0.8.0rc1/linien_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:17:21.773297 linien-client-0.8.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-03 12:16:37.000000 linien-client-0.8.0rc1/setup.py
```

### Comparing `linien-client-0.7.0rc2/PKG-INFO` & `linien-client-0.8.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-client
-Version: 0.7.0rc2
+Version: 0.8.0rc1
 Summary: Client components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien/
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-client-0.7.0rc2/linien_client/connection.py` & `linien-client-0.8.0rc1/linien_client/connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,49 +17,35 @@
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import random
 import string
 from socket import gaierror
 from time import sleep
 from traceback import print_exc
-from typing import Callable
+from typing import Callable, Optional
 
-import linien_client
 import rpyc
-from linien_client.deploy import start_remote_server
-from linien_client.exceptions import (
+from linien_common.config import DEFAULT_SERVER_PORT
+
+from . import __version__
+from .communication import LinienControlService
+from .deploy import start_remote_server
+from .exceptions import (
     GeneralConnectionErrorException,
     InvalidServerVersionException,
     RPYCAuthenticationException,
     ServerNotRunningException,
 )
-from linien_client.remote_parameters import RemoteParameters
-from linien_common.common import hash_username_and_password
-from linien_common.config import DEFAULT_SERVER_PORT
+from .remote_parameters import RemoteParameters
 
 
-class RPYCClientWithAuthentication(rpyc.Service):
-    """
-    An rpyc client that authenticates using a hash.
-
-    This class is run on the client side and exposes the client's unique id to the
-    server.
-    """
-
-    def __init__(self, uuid, user, password):
+class RPYCServiceWithUUID(rpyc.Service):
+    def __init__(self, uuid: str):
         super().__init__()
-
         self.exposed_uuid = uuid
-        self.auth_hash = hash_username_and_password(user, password).encode()
-
-    def _connect(self, channel, config):
-        # send auth hash before rpyc takes over
-        channel.stream.sock.send(self.auth_hash)
-
-        return super()._connect(channel, config)
 
 
 class LinienClient:
     def __init__(
         self,
         host: str,
         user: str,
@@ -78,43 +64,55 @@
             # RP is configured such that "localhost" doesn't point to 127.0.0.1 in all
             # cases
             self.host = "127.0.0.1"
 
         self.uuid = "".join(random.choice(string.ascii_lowercase) for _ in range(10))
 
         # for exposing client's uuid to server
-        self.client_service = RPYCClientWithAuthentication(self.uuid, user, password)
+        self.client_service = RPYCServiceWithUUID(self.uuid)
 
     def connect(
         self,
         autostart_server: bool,
         use_parameter_cache: bool,
-        call_on_error: Callable = None,
+        call_on_error: Optional[Callable] = None,
     ) -> None:
         self.connection = None
 
         i = -1
         while True:
             i += 1
             try:
                 print(f"Try to connect to {self.host}:{self.port}")
-                self._connect_rpyc(
-                    use_parameter_cache,
-                    call_on_error=call_on_error,
+
+                self.connection = rpyc.connect(
+                    self.host,
+                    self.port,
+                    service=self.client_service,
+                    config={"allow_pickle": True},
+                )
+
+                cls = RemoteParameters
+                if call_on_error:
+                    cls = self._catch_network_errors(cls, call_on_error)
+
+                self.parameters = cls(
+                    self.connection.root, self.uuid, use_parameter_cache
                 )
-                self.control = self.connection.root
+
+                self.control: LinienControlService = self.connection.root
                 break
             except gaierror:
                 # host not found
                 print(f"Error: host {self.host} not found")
                 break
             except EOFError:
                 print("EOFError! Probably authentication failed")
                 raise RPYCAuthenticationException()
-            except Exception:
+            except ConnectionRefusedError:
                 if not autostart_server:
                     raise ServerNotRunningException()
 
                 if i == 0:
                     print("Server is not running. Launching it!")
                     start_remote_server(self.host, self.user, self.password)
                     sleep(3)
@@ -130,36 +128,26 @@
                         break
 
         if self.connection is None:
             raise GeneralConnectionErrorException()
 
         # now check that the remote version is the same as ours
         remote_version = self.connection.root.exposed_get_server_version().split("+")[0]
-        local_version = linien_client.__version__.split("+")[0]
+        local_version = __version__.split("+")[0]
 
         if (remote_version != local_version) and not ("dev" in local_version):
             raise InvalidServerVersionException(local_version, remote_version)
 
         self.connected = True
         print("Connection established!")
 
-    def _connect_rpyc(self, use_parameter_cache, call_on_error=None):
-        """Connect to the server using rpyc and instanciate `RemoteParameters`."""
-        self.connection = rpyc.connect(
-            self.host,
-            self.port,
-            service=self.client_service,
-            config={"allow_pickle": True},
-        )
-
-        cls = RemoteParameters
-        if call_on_error:
-            cls = self._catch_network_errors(cls, call_on_error)
-
-        self.parameters = cls(self.connection.root, self.uuid, use_parameter_cache)
+    def disconnect(self) -> None:
+        if self.connection is not None:
+            self.connection.close()
+        self.connected = False
 
     def _catch_network_errors(self, cls, call_on_error):
         """
         This method can be used for patching RemoteParameters such that network errors
         are redirected to `call_on_error`
         """
         function_type = type(lambda x: x)
@@ -180,11 +168,7 @@
                             self.connected = False
                             call_on_error()
                             raise
 
                     setattr(cls, attr_name, wrapped)
 
         return cls
-
-    def disconnect(self) -> None:
-        self.connection.close()
-        self.connected = False
```

### Comparing `linien-client-0.7.0rc2/linien_client/deploy.py` & `linien-client-0.8.0rc1/linien_client/deploy.py`

 * *Files identical despite different names*

### Comparing `linien-client-0.7.0rc2/linien_client/exceptions.py` & `linien-client-0.8.0rc1/linien_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `linien-client-0.7.0rc2/linien_client/remote_parameters.py` & `linien-client-0.8.0rc1/linien_client/remote_parameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,248 +12,210 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Callable
+import pickle
+from typing import Any, Callable, Dict, Iterator, List, Tuple, Union
 
-import rpyc
-from linien_common.common import pack, unpack
 from rpyc import async_
+from rpyc.core.async_ import AsyncResult
 
+from .communication import LinienControlService
 
-class RemoteParameters:
-    """
-    A class that provides access to a remote `parameters.Parameters` instance.
 
-    It clones the functionality of the remote `Parameters` instance. E.g.:
+class RemoteParameter:
+    """A helper class for `RemoteParameters`, representing a single remote parameter."""
 
-        # on the remote side
-        p = Parameters(...)
-        p.my_param.value = 123
-
-        # on the client side
-        r = RemoteParameters(...)
-
-        # RemoteParameters allows for accessing the remote value:
-        print(r.my_param.value) # outputs 123
-
-        # it's also possible to set the value (this change is automatically
-        # propagated to the server)
-        r.my_param.value = 123
-
-        # and we can set up a callback function that is called whenever a
-        # parameter changes
-        def on_change(value):
-            # this function is called whenever `my_param` changes on the server.
-            # note that this only works if `call_listeners` is called from
-            # time to time as this function is responsible for checking for
-            # changed parameters.
-            print('parameter arrived!', value)
-        r.my_param.on_change(on_change)
-        while True:
-            r.call_listeners()
-            sleep(.1)
-
-    The arguments for __init__ are:
-
-        `remote`:    The root of the rpyc connection ot the server
-        `uuid`:      A random unique identifier for this client
-        `use_cache`: A boolean indicating whether (most) parameters should be
-                     cached locally. If this is not enabled, every access of
-                     `r.my_param.value` results in a request to the server.
-                     If `use_cache` is enabled, a local cache is used instead.
-                     For that purpose, a listener is installed such that the
-                     server automatically pushes changes to the client and
-                     thus updates the cache. No matter how often you access
-                     `r.my_param.value`, each parameter value is only transmitted
-                     once (after it was changed).
-                     Note that calling `call_listeners` is required for this.
-    """
+    def __init__(
+        self,
+        parent: "RemoteParameters",
+        name: str,
+        use_cache: bool,
+        restorable: bool,
+        loggable: bool,
+        log: bool,
+    ):
+        self.name = name
+        self.parent = parent
+        self.use_cache = use_cache
+        self.restorable = restorable
+        self.loggable = loggable
+        self.log = log
 
-    def __init__(self, remote, uuid: str, use_cache: bool):
-        self.remote = remote
-        self.uuid = uuid
-        self._async_listener_queue = None
-        self._async_listener_registering = None
+    @property
+    def value(self) -> Any:
+        """Return the locally cached value (if it exists). Otherwise ask the server."""
+        if hasattr(self, "_cached_value"):
+            return self._cached_value
+        return pickle.loads(self.parent.remote.exposed_get_param(self.name))
+
+    @value.setter
+    def value(self, value: Any):
+        """Notify the server of the new value"""
+        return self.parent.remote.exposed_set_param(self.name, pickle.dumps(value))
 
-        self._listeners_pending_remote_registration = []
-        self._listeners = {}
+    @property
+    def log(self) -> bool:
+        return self.parent.remote.exposed_get_parameter_log(self.name)
 
-        self._mimic_remote_parameters(use_cache)
-        self._attributes_locked = True
+    @log.setter
+    def log(self, value: bool) -> None:
+        self.parent.remote.exposed_set_parameter_log(self.name, value)
+
+    def add_callback(self, callback: Callable, call_with_first_value: bool = True):
+        """
+        Register a callback function that is called whenever the parameter changes.
+        """
+
+        if self.name not in self.parent._callbacks and not self.use_cache:
+            # Make sure that the server knows that we want to be notified about changes.
+            # Parameters that use the cache are already registered, see `__init__`.
+            self.parent._listeners_pending_remote_registration.append(self.name)
 
-        self.call_listeners()
+        self.parent._callbacks.setdefault(self.name, [])
+        self.parent._callbacks[self.name].append(callback)
 
-    def __setattr__(self, name, value):
-        """In order to set the value of a parameter,
+        if call_with_first_value:
+            callback(self.value)
 
-            parameters.my_param.value = 123
+    def reset(self) -> None:
+        """Reset the value to its initial value"""
+        self.parent.remote.exposed_reset_param(self.name)
 
-        is used. In order to prevent accidentally forgetting the .value part, i.e.
+    def update_cache(self, value: Any) -> None:
+        self._cached_value = value
 
-            parameters.my_param = 123
 
-        we raise an error in this case."""
+class RemoteParameters:
+    def __init__(self, remote: LinienControlService, uuid: str, use_cache: bool):
+        """
+        Provides access to a remote `Parameters` instance and minics its functionality.
+
+        :param remote: root of the rpyc connection to the server
+        :param uuid: random unique identifier for this client
+        :param use_cache: A boolean indicating whether (most) parameters should be
+            cached locally. If this is not enabled, every access of `r.my_param.value`
+            results in a request to the server. If `use_cache` is enabled, a local cache
+            is used instead. For that purpose, a listener is installed such that the
+            server notifies the client about changed parameters, whenever the
+            `check_for_changed_parameters` method is called.
+        """
+        self.remote = remote
+        self.uuid = uuid
+
+        self._async_changed_parameters_queue: Union[AsyncResult, None] = None
+        self._async_listener_registering: Union[AsyncResult, None] = None
+
+        self._listeners_pending_remote_registration: List[str] = []
+        self._callbacks: Dict[str, List[Callable]] = {}
+
+        # mimic functionality of `parameters.Parameters`:
+        all_parameters = pickle.loads(
+            self.remote.exposed_init_parameter_sync(self.uuid)
+        )
+        for name, value, can_be_cached, restorable, loggable, log in all_parameters:
+            param = RemoteParameter(
+                parent=self,
+                name=name,
+                use_cache=use_cache and can_be_cached,
+                restorable=restorable,
+                loggable=loggable,
+                log=log,
+            )
+            setattr(self, name, param)
+            if param.use_cache:
+                param.update_cache(value)
+        self._attributes_locked = True
+
+        self.check_for_changed_parameters()
+
+    def __iter__(self) -> Iterator[Tuple[str, "RemoteParameter"]]:
+        for param_name, param in self.__dict__.items():
+            if isinstance(param, RemoteParameter):
+                yield param_name, param
+
+    def __setattr__(self, name: str, value: Any) -> None:
+        # Prevents accidentally overwriting parameters.
         if (
             hasattr(self, "_attributes_locked")
             and self._attributes_locked
             and not name.startswith("_")
         ):
-            raise Exception(
-                "Parameters are locked! Did you mean to set the value of this "
-                "parameter instead, i.e. parameters.%s.value = %s" % (name, value)
+            raise AttributeError(
+                "Parameters are locked! Did you mean to set the value of this parameter"
+                f" instead, i.e. parameters.{name}.value = {value}"
             )
         super().__setattr__(name, value)
 
-    def _mimic_remote_parameters(self, use_cache: bool):
-        """For every remote parameter, instanciate a `RemoteParameter` object
-        that allows to mimics the functionality of the remote parameter."""
-        # when directly iterating over `exposed_init_parameter_sync`, each iteration
-        # triggers a request as it is a netref over an iterator
-        # --> the `list` call prevents this and improves startup performance
-        all_parameters = unpack(self.remote.exposed_init_parameter_sync(self.uuid))
-
-        for name, param, value, can_be_cached in all_parameters:
-            param = RemoteParameter(self, param, name, use_cache and can_be_cached)
-            setattr(self, name, param)
-            if use_cache and can_be_cached:
-                # obtain takes care that we really don't deal with netrefs
-                # (np.float64 is not automatically serialized)
-                param._update_cache(rpyc.classic.obtain(value))
+    def check_for_changed_parameters(self) -> None:
+        """
+        Ask the server for changed parameters and trigger the respective callbacks.
+
+        This call takes place asynchronously, i.e. the first run of
+        `check_for_changed_parameters` just issues the call but does not wait for it in
+        order not to block the GUI. The following calls check whether a result has
+        arrived (also not blocking GUI).
+
+        In Linien GUI client, this function is called periodically. If you use the
+        python client and want to use callbacks for changed parameters you have to call
+        this method manually from time to time.
+        """
+
+        if self._async_changed_parameters_queue is None:
+            # This means that the async call was not started yet --> start it. The next
+            # call to `check_for_changed_parameters` will then check whether the result
+            # is ready. Issues an asynchronous call (that does not block the GUI) to the
+            # server in order to retrieve a batch of changed parameters.
+            self._async_changed_parameters_queue = async_(
+                self.remote.exposed_get_changed_parameters_queue
+            )(self.uuid)
 
-        self._attributes_locked = True
-
-    def _register_listener(self, param, callback: Callable):
-        """Tells the server to notify our client (identified by `self.uuid`)
-        when `param` changes. Registers a function `callback` that will be
-        called in this case."""
-        if param.name not in self._listeners:
-            # parameters that use the cache don't have to be registered on remote
-            # side because the client automatically listens for changes.
-            # This happens using `init_parameter_sync`
-            if not param.use_cache:
-                self._listeners_pending_remote_registration.append(param.name)
-
-        self._listeners.setdefault(param.name, [])
-        self._listeners[param.name].append(callback)
-
-    def call_listeners(self):
-        """Ask the server for changed parameters and call the respective
-        callback functions. This call takes place asynchronously, i.e. the first
-        run of `call_listeners` just issues the call but does not wait for it
-        in order not to block the GUI. The following calls check whether a
-        result has arrived (also not blocking GUI).
-
-        In Linien GUI client, this function is called periodically.
-        If you use the python client and want to use callbacks for changed
-        parameters you have to call this method manually from time to time."""
-
-        def _get_listener_queue_async():
-            """Issues an asynchronous call (that does not block the GUI) to the
-            server in order to retrieve a batch of changed parameters."""
-            self._async_listener_queue = async_(self.remote.get_listener_queue)(
-                self.uuid
-            )
-
-        def _register_listeners_async():
-            """Issues an asynchronous call to the server containing all the
-            parameters that this client wants to be notified of in case of a
-            changed value."""
+        if self._async_listener_registering is None:
+            # Issues an asynchronous call to the server containing all the parameters
+            # that this client wants to be notified of in case of a changed value.
             pending = self._listeners_pending_remote_registration
             if pending:
-                # this copies the list before clearing it below. Otherwise
-                # we just transmit an epmty list in the async call
+                # This copies the list before clearing it below. Otherwise we just
+                # transmit an empty list in the async call
                 pending = pending[:]
                 self._async_listener_registering = async_(
                     self.remote.exposed_register_remote_listeners
                 )(self.uuid, pending)
                 self._listeners_pending_remote_registration.clear()
 
-        if self._async_listener_queue is None:
-            # this means that the async call was not started yet --> start it
-            # the next call to `call_listeners` will then check whether the
-            # the result is ready.
-            _get_listener_queue_async()
-
-        if self._async_listener_registering is None:
-            _register_listeners_async()
-
-        if self._async_listener_queue is not None and self._async_listener_queue.ready:
-            # we have a result
-            queue = unpack(self._async_listener_queue.value)
+        if (
+            self._async_changed_parameters_queue is not None
+            and self._async_changed_parameters_queue.ready
+        ):
+            # We have a result.
+            queue: List[Tuple[str, Any]] = pickle.loads(
+                self._async_changed_parameters_queue.value
+            )
 
-            # now that we have our result, we can start the next call
-            _get_listener_queue_async()
+            # Now that we have our result, we can start the next call.
+            self._async_changed_parameters_queue = async_(
+                self.remote.exposed_get_changed_parameters_queue
+            )(self.uuid)
 
-            # before calling listeners, we update cache for all received parameters
-            # at once
+            # Before calling listeners, we update cache for all received parameters at
+            # once.
             for param_name, value in queue:
-                param = getattr(self, param_name)
+                param: RemoteParameter = getattr(self, param_name)
                 if param.use_cache:
-                    param._update_cache(value)
+                    param.update_cache(value)
 
-            # iterate over all canged parameters and call the respective
-            # callback functions
+            # Iterate over all canged parameters and call respective callback functions.
             for param_name, value in queue:
-                if param_name in self._listeners:
-                    for listener in self._listeners[param_name]:
-                        listener(value)
+                if param_name in self._callbacks:
+                    for callback in self._callbacks[param_name]:
+                        callback(value)
 
         if (
             self._async_listener_registering is not None
             and self._async_listener_registering.ready
         ):
-            # registration of listeners was successful on the remote side
-            # now we can clear the async call object such that a new one may
-            # be issued (if required)
+            # Registration of listeners was successful on the remote side. Now we can
+            # clear the async call object such that a new one may be issued if required.
             self._async_listener_registering = None
-
-    def _get_param(self, param_name):
-        return unpack(self.remote.exposed_get_param(param_name))
-
-    def _set_param(self, param_name, value):
-        return self.remote.exposed_set_param(param_name, pack(value))
-
-
-class RemoteParameter:
-    """A helper class for `RemoteParameters`, representing a single remote
-    parameter."""
-
-    def __init__(
-        self, parent: RemoteParameters, remote_param, name: str, use_cache: bool
-    ):
-        self._remote_param = remote_param
-        self.name = name
-        self.parent = parent
-        self.use_cache = use_cache
-
-    @property
-    def value(self):
-        """Return the locally cached value (if it exists). Otherwise ask the
-        server."""
-        if hasattr(self, "_cached_value"):
-            return self._cached_value
-        return self.parent._get_param(self.name)
-
-    @value.setter
-    def value(self, value):
-        """Notify the server of the new value"""
-        return self.parent._set_param(self.name, value)
-
-    def on_change(self, callback_on_change, call_listener_with_first_value=True):
-        """Tells the server that `callback_on_change` should be called whenever
-        the parameter changes."""
-        self.parent._register_listener(self, callback_on_change)
-
-        if call_listener_with_first_value:
-            # call the callback with the initial value
-            callback_on_change(self.value)
-
-    def reset(self):
-        """Reset the value to its initial value"""
-        self._remote_param.reset()
-
-    def _update_cache(self, value):
-        self._cached_value = value
```

### Comparing `linien-client-0.7.0rc2/linien_client.egg-info/PKG-INFO` & `linien-client-0.8.0rc1/linien_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-client
-Version: 0.7.0rc2
+Version: 0.8.0rc1
 Summary: Client components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien/
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-client-0.7.0rc2/setup.py` & `linien-client-0.8.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
-version = "0.7.0rc2"
+version = "0.8.0rc1"
 
 setup(
     name="linien-client",
     version=version,
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
@@ -38,12 +38,11 @@
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8",
     install_requires=[
         "fabric>=2.7.0",
         "numpy>=1.22",
         "patchwork>=1.0.1",
-        "rpyc>=4.0,<5.0",
         "scipy>=1.4.1",
         f"linien-common=={version}",
     ],
 )
```

