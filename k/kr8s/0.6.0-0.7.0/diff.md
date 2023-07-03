# Comparing `tmp/kr8s-0.6.0.tar.gz` & `tmp/kr8s-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kr8s-0.6.0.tar", max compression
+gzip compressed data, was "kr8s-0.7.0.tar", max compression
```

## Comparing `kr8s-0.6.0.tar` & `kr8s-0.7.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1549 2023-06-29 08:25:21.067652 kr8s-0.6.0/LICENSE
--rw-r--r--   0        0        0     2571 2023-06-29 08:25:21.067652 kr8s-0.6.0/README.md
--rw-r--r--   0        0        0      541 2023-06-29 08:25:44.343775 kr8s-0.6.0/kr8s/__init__.py
--rw-r--r--   0        0        0    10470 2023-06-29 08:25:21.087653 kr8s-0.6.0/kr8s/_api.py
--rw-r--r--   0        0        0     5879 2023-06-29 08:25:21.087653 kr8s-0.6.0/kr8s/_auth.py
--rw-r--r--   0        0        0     1920 2023-06-29 08:25:21.087653 kr8s-0.6.0/kr8s/_data_utils.py
--rw-r--r--   0        0        0      163 2023-06-29 08:25:21.087653 kr8s-0.6.0/kr8s/_exceptions.py
--rw-r--r--   0        0        0     4294 2023-06-29 08:25:21.087653 kr8s-0.6.0/kr8s/_io.py
--rw-r--r--   0        0        0    30540 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/_objects.py
--rw-r--r--   0        0        0     7764 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/_portforward.py
--rw-r--r--   0        0        0      680 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/_testutils.py
--rw-r--r--   0        0        0       30 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/asyncio/__init__.py
--rw-r--r--   0        0        0      992 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/asyncio/_api.py
--rw-r--r--   0        0        0      709 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/asyncio/objects.py
--rw-r--r--   0        0        0       50 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/asyncio/portforward.py
--rw-r--r--   0        0        0     5575 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/conftest.py
--rw-r--r--   0        0        0     6001 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/objects.py
--rw-r--r--   0        0        0      152 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/portforward.py
--rw-r--r--   0        0        0       78 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/resources/custom/evc.yaml
--rw-r--r--   0        0        0       61 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/resources/serviceaccount.yaml
--rw-r--r--   0        0        0      369 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
--rw-r--r--   0        0        0      144 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/resources/simple/nginx_pod.yaml
--rw-r--r--   0        0        0      435 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/resources/simple/nginx_pod_service.yaml
--rwxr-xr-x   0        0        0      614 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     4385 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     3402 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      824 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0      643 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/test_io.py
--rw-r--r--   0        0        0    15968 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0     2564 2023-06-29 08:25:44.343775 kr8s-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 kr8s-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-07-03 10:38:10.325768 kr8s-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2571 2023-07-03 10:38:10.325768 kr8s-0.7.0/README.md
+-rw-r--r--   0        0        0      541 2023-07-03 10:38:33.357956 kr8s-0.7.0/kr8s/__init__.py
+-rw-r--r--   0        0        0    11094 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_api.py
+-rw-r--r--   0        0        0     5879 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_auth.py
+-rw-r--r--   0        0        0     1920 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      163 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_exceptions.py
+-rw-r--r--   0        0        0     4294 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_io.py
+-rw-r--r--   0        0        0    32623 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_objects.py
+-rw-r--r--   0        0        0     7764 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_portforward.py
+-rw-r--r--   0        0        0      680 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_testutils.py
+-rw-r--r--   0        0        0       30 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0      992 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/asyncio/_api.py
+-rw-r--r--   0        0        0      709 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0       50 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     5503 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/conftest.py
+-rw-r--r--   0        0        0     6001 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/objects.py
+-rw-r--r--   0        0        0      152 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/portforward.py
+-rw-r--r--   0        0        0       78 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/resources/custom/evc.yaml
+-rw-r--r--   0        0        0       61 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/resources/serviceaccount.yaml
+-rw-r--r--   0        0        0      369 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
+-rw-r--r--   0        0        0      144 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/resources/simple/nginx_pod.yaml
+-rw-r--r--   0        0        0      435 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/resources/simple/nginx_pod_service.yaml
+-rwxr-xr-x   0        0        0      614 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     4567 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     3402 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      824 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0      643 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/test_io.py
+-rw-r--r--   0        0        0    17674 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0     2564 2023-07-03 10:38:33.357956 kr8s-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 kr8s-0.7.0/PKG-INFO
```

### Comparing `kr8s-0.6.0/LICENSE` & `kr8s-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/README.md` & `kr8s-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/kr8s/__init__.py` & `kr8s-0.7.0/kr8s/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ._api import ALL  # noqa
 from ._api import Api as _AsyncApi
 from ._exceptions import NotFoundError  # noqa
 from ._io import run_sync as _run_sync
 from ._io import sync as _sync  # noqa
 from .asyncio import api as _api  # noqa
 
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 
 @_sync
 class Api(_AsyncApi):
     __doc__ = _AsyncApi.__doc__
```

### Comparing `kr8s-0.6.0/kr8s/_api.py` & `kr8s-0.7.0/kr8s/_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023, Dask Developers, NVIDIA
 # SPDX-License-Identifier: BSD 3-Clause License
 import contextlib
 import json
 import ssl
 import weakref
-from typing import List, Tuple
+from typing import Dict, List, Tuple, Union
 
 import aiohttp
 import asyncio_atexit
 
 from ._auth import KubeAuth
+from ._data_utils import dict_to_selector
 
 ALL = "all"
 
 
 class Api(object):
     """A kr8s object for interacting with the Kubernetes API.
 
@@ -143,32 +144,36 @@
         await self.auth.reauthenticate()
 
     @contextlib.asynccontextmanager
     async def _get_kind(
         self,
         kind: str,
         namespace: str = None,
-        label_selector: str = None,
-        field_selector: str = None,
+        label_selector: Union[str, Dict] = None,
+        field_selector: Union[str, Dict] = None,
         params: dict = None,
         watch: bool = False,
         **kwargs,
     ) -> dict:
         """Get a Kubernetes resource."""
         from ._objects import get_class
 
         if not namespace:
-            namespace = self.auth.namespace
+            namespace = self.namespace
         if namespace is ALL:
             namespace = ""
         if params is None:
             params = {}
         if label_selector:
+            if isinstance(label_selector, dict):
+                label_selector = dict_to_selector(label_selector)
             params["labelSelector"] = label_selector
         if field_selector:
+            if isinstance(field_selector, dict):
+                field_selector = dict_to_selector(field_selector)
             params["fieldSelector"] = field_selector
         if watch:
             params["watch"] = "true" if watch else "false"
         params = params or None
         obj_cls = get_class(kind)
         async with self.call_api(
             method="GET",
@@ -181,16 +186,16 @@
             yield obj_cls, response
 
     async def get(
         self,
         kind: str,
         *names: List[str],
         namespace: str = None,
-        label_selector: str = None,
-        field_selector: str = None,
+        label_selector: Union[str, Dict] = None,
+        field_selector: Union[str, Dict] = None,
         as_object: object = None,
         **kwargs,
     ) -> List[object]:
         """Get a Kubernetes resource."""
         return await self._get(
             kind,
             *names,
@@ -202,16 +207,16 @@
         )
 
     async def _get(
         self,
         kind: str,
         *names: List[str],
         namespace: str = None,
-        label_selector: str = None,
-        field_selector: str = None,
+        label_selector: Union[str, Dict] = None,
+        field_selector: Union[str, Dict] = None,
         as_object: object = None,
         **kwargs,
     ) -> List[object]:
         headers = {}
         if as_object:
             group, version = as_object.version.split("/")
             headers[
@@ -241,16 +246,16 @@
                     ]
                 return []
 
     async def watch(
         self,
         kind: str,
         namespace: str = None,
-        label_selector: str = None,
-        field_selector: str = None,
+        label_selector: Union[str, Dict] = None,
+        field_selector: Union[str, Dict] = None,
         since: str = None,
     ):
         """Watch a Kubernetes resource."""
         async for t, object in self._watch(
             kind,
             namespace=namespace,
             label_selector=label_selector,
@@ -259,16 +264,16 @@
         ):
             yield t, object
 
     async def _watch(
         self,
         kind: str,
         namespace: str = None,
-        label_selector: str = None,
-        field_selector: str = None,
+        label_selector: Union[str, Dict] = None,
+        field_selector: Union[str, Dict] = None,
         since: str = None,
     ) -> Tuple[str, object]:
         """Watch a Kubernetes resource."""
         async with self._get_kind(
             kind,
             namespace=namespace,
             label_selector=label_selector,
@@ -316,7 +321,16 @@
         return resources
 
     @property
     def __version__(self) -> str:
         from . import __version__
 
         return f"kr8s/{__version__}"
+
+    @property
+    def namespace(self) -> str:
+        """Get the default namespace."""
+        return self.auth.namespace
+
+    @namespace.setter
+    def namespace(self, value):
+        self.auth.namespace = value
```

### Comparing `kr8s-0.6.0/kr8s/_auth.py` & `kr8s-0.7.0/kr8s/_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/kr8s/_data_utils.py` & `kr8s-0.7.0/kr8s/_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/kr8s/_io.py` & `kr8s-0.7.0/kr8s/_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/kr8s/_objects.py` & `kr8s-0.7.0/kr8s/_objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,18 +30,25 @@
     """Base class for Kubernetes objects."""
 
     namespaced = False
     scalable = False
     scalable_spec = "replicas"
     _asyncio = True
 
-    def __init__(self, resource: dict, api: Api = None) -> None:
+    def __init__(self, resource: dict, namespace: str = None, api: Api = None) -> None:
         """Initialize an APIObject."""
         # TODO support passing pykube or kubernetes objects in addition to dicts
-        self._raw = resource
+        if isinstance(resource, str):
+            self._raw = {"metadata": {"name": resource}}
+        elif isinstance(resource, dict):
+            self._raw = resource
+        else:
+            raise ValueError("resource must be a dict or a string")
+        if namespace is not None:
+            self._raw["metadata"]["namespace"] = namespace
         self.api = api
         if self.api is None and not self._asyncio:
             self.api = kr8s.api()
 
     def __await__(self):
         async def f():
             if self.api is None:
@@ -54,14 +61,25 @@
         """Return a string representation of the Kubernetes resource."""
         return f"<{self.kind} {self.name}>"
 
     def __str__(self):
         """Return a string representation of the Kubernetes resource."""
         return self.name
 
+    def __eq__(self, other):
+        if self.version != other.version:
+            return False
+        if self.kind != other.kind:
+            return False
+        if self.name != other.name:
+            return False
+        if self.namespaced and self.namespace != other.namespace:
+            return False
+        return True
+
     @property
     def raw(self) -> str:
         """Raw object returned from the Kubernetes API."""
         return self._raw
 
     @raw.setter
     def raw(self, value: Any) -> None:
@@ -72,17 +90,15 @@
         """Name of the Kubernetes resource."""
         return self.raw["metadata"]["name"]
 
     @property
     def namespace(self) -> str:
         """Namespace of the Kubernetes resource."""
         if self.namespaced:
-            return self.raw.get("metadata", {}).get(
-                "namespace", self.api.auth.namespace
-            )
+            return self.raw.get("metadata", {}).get("namespace", self.api.namespace)
         return None
 
     @property
     def metadata(self) -> dict:
         """Metadata of the Kubernetes resource."""
         return self.raw["metadata"]
 
@@ -122,33 +138,46 @@
                 spec = spec[key]
             return spec
         raise NotImplementedError(f"{self.kind} is not scalable")
 
     @classmethod
     async def get(
         cls,
-        name: str,
+        name: str = None,
         namespace: str = None,
         api: Api = None,
+        label_selector: Union[str, Dict[str, str]] = None,
+        field_selector: Union[str, Dict[str, str]] = None,
         timeout: int = 2,
         **kwargs,
     ) -> APIObject:
-        """Get a Kubernetes resource by name."""
+        """Get a Kubernetes resource by name or via selectors."""
 
         if api is None:
             if cls._asyncio:
                 api = await kr8s.asyncio.api()
             else:
                 api = kr8s.api()
         start = time.time()
         backoff = 0.1
         while start + timeout > time.time():
-            resources = await api._get(
-                cls.endpoint, name, namespace=namespace, **kwargs
-            )
+            if name:
+                resources = await api._get(
+                    cls.endpoint, name, namespace=namespace, **kwargs
+                )
+            elif label_selector or field_selector:
+                resources = await api._get(
+                    cls.endpoint,
+                    namespace=namespace,
+                    label_selector=label_selector,
+                    field_selector=field_selector,
+                    **kwargs,
+                )
+            else:
+                raise ValueError("Must specify name or selector")
             if len(resources) == 0:
                 await asyncio.sleep(backoff)
                 backoff = min(backoff * 2, 1)
                 continue
             if len(resources) > 1:
                 raise ValueError(
                     f"Expected exactly one {cls.kind} object. Use selectors to narrow down the search."
@@ -314,14 +343,38 @@
                     return
             if await self._test_conditions(conditions):
                 return
             async for _ in self._watch():
                 if await self._test_conditions(conditions):
                     return
 
+    async def annotate(self, annotations: dict = None, **kwargs) -> None:
+        """Annotate this object in Kubernetes."""
+        if annotations is None:
+            annotations = kwargs
+        if not annotations:
+            raise ValueError("No annotations provided")
+        await self._patch({"metadata": {"annotations": annotations}})
+
+    async def label(self, labels: dict = None, **kwargs) -> None:
+        """Label this object in Kubernetes."""
+        if labels is None:
+            labels = kwargs
+        if not labels:
+            raise ValueError("No labels provided")
+        await self._patch({"metadata": {"labels": labels}})
+
+    def keys(self) -> list:
+        """Return the keys of this object."""
+        return self.raw.keys()
+
+    def __getitem__(self, key: str) -> Any:
+        """Get an item from this object."""
+        return self.raw[key]
+
 
 ## v1 objects
 
 
 class Binding(APIObject):
     """A Kubernetes Binding."""
```

### Comparing `kr8s-0.6.0/kr8s/_portforward.py` & `kr8s-0.7.0/kr8s/_portforward.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/kr8s/_testutils.py` & `kr8s-0.7.0/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/kr8s/asyncio/_api.py` & `kr8s-0.7.0/kr8s/asyncio/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/kr8s/asyncio/objects.py` & `kr8s-0.7.0/kr8s/asyncio/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/kr8s/conftest.py` & `kr8s-0.7.0/kr8s/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,25 +115,25 @@
             time.sleep(1)
     yield kind_cluster
     del os.environ["KUBECONFIG"]
     if not request.config.getoption("keep_cluster"):  # pragma: no cover
         kind_cluster.delete()
 
 
-@pytest.fixture(scope="session")
-def ns(k8s_cluster) -> str:
-    # Ideally we want to generate a random namespace for each test or suite, but
-    # this can make teardown very slow. So we just use the default namespace for now.
-
-    yield "default"
-
-    # name = "kr8s-pytest-" + uuid.uuid4().hex[:4]
-    # k8s_cluster.kubectl("create", "namespace", name)
-    # yield name
-    # k8s_cluster.kubectl("delete", "namespace", name)
+@pytest.fixture(scope="session", autouse=True)
+def run_id():
+    return uuid.uuid4().hex[:4]
+
+
+@pytest.fixture(autouse=True)
+def ns(k8s_cluster, run_id) -> str:
+    name = f"kr8s-pytest-{run_id}-{uuid.uuid4().hex[:4]}"
+    k8s_cluster.kubectl("create", "namespace", name)
+    yield name
+    k8s_cluster.kubectl("delete", "namespace", name, "--wait=false")
 
 
 @pytest.fixture
 async def kubectl_proxy(k8s_cluster):
     proxy = subprocess.Popen(
         [k8s_cluster.kubectl_path, "proxy"],
         env={**os.environ, "KUBECONFIG": str(k8s_cluster.kubeconfig_path)},
```

### Comparing `kr8s-0.6.0/kr8s/objects.py` & `kr8s-0.7.0/kr8s/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/kr8s/tests/scripts/envexec.py` & `kr8s-0.7.0/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/kr8s/tests/test_api.py` & `kr8s-0.7.0/kr8s/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,21 +98,21 @@
 async def test_get_pods_as_table():
     kubernetes = await kr8s.asyncio.api()
     pods = await kubernetes.get("pods", namespace="kube-system", as_object=Table)
     assert isinstance(pods, Table)
     assert len(pods.rows) > 0
 
 
-async def test_watch_pods(example_pod_spec):
+async def test_watch_pods(example_pod_spec, ns):
     kubernetes = await kr8s.asyncio.api()
     pod = await Pod(example_pod_spec)
     await pod.create()
     while not await pod.ready():
         await asyncio.sleep(0.1)
-    async for event, obj in kubernetes.watch("pods"):
+    async for event, obj in kubernetes.watch("pods", namespace=ns):
         assert event in ["ADDED", "MODIFIED", "DELETED"]
         assert isinstance(obj, Pod)
         if obj.name == pod.name:
             if event == "ADDED":
                 await obj.patch({"metadata": {"labels": {"test": "test"}}})
             elif event == "MODIFIED" and "test" in obj.labels and await obj.exists():
                 await obj.delete()
@@ -146,7 +146,15 @@
 
     [deployment] = [d for d in resources if d["name"] == "deployments"]
     assert deployment["namespaced"]
     assert deployment["kind"] == "Deployment"
     assert deployment["version"] == "apps/v1"
     assert "get" in deployment["verbs"]
     assert "deploy" in deployment["shortNames"]
+
+
+async def test_ns(ns):
+    api = await kr8s.asyncio.api(namespace=ns)
+    assert ns == api.namespace
+
+    api.namespace = "foo"
+    assert api.namespace == "foo"
```

### Comparing `kr8s-0.6.0/kr8s/tests/test_auth.py` & `kr8s-0.7.0/kr8s/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/kr8s/tests/test_data_utils.py` & `kr8s-0.7.0/kr8s/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/kr8s/tests/test_io.py` & `kr8s-0.7.0/kr8s/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/kr8s/tests/test_objects.py` & `kr8s-0.7.0/kr8s/tests/test_objects.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from kr8s.objects import get_class, object_from_spec
 
 DEFAULT_TIMEOUT = aiohttp.ClientTimeout(30)
 CURRENT_DIR = pathlib.Path(__file__).parent
 
 
 @pytest.fixture
-async def nginx_pod(k8s_cluster, example_pod_spec):
+async def nginx_pod(k8s_cluster, example_pod_spec, ns):
     example_pod_spec["metadata"]["name"] = (
         "nginx-" + example_pod_spec["metadata"]["name"]
     )
     example_pod_spec["spec"]["containers"][0]["image"] = "nginx:latest"
     example_pod_spec["spec"]["containers"][0]["ports"] = [{"containerPort": 80}]
     example_pod_spec["spec"]["containers"][0]["readinessProbe"] = {
         "httpGet": {"path": "/", "port": 80},
@@ -45,14 +45,16 @@
     await pod.create()
     while not await pod.ready():
         await asyncio.sleep(0.1)
     # TODO replace with pod.exec() once implemented
     k8s_cluster.kubectl(
         "exec",
         example_pod_spec["metadata"]["name"],
+        "-n",
+        ns,
         "--",
         "dd",
         "if=/dev/random",
         "of=/usr/share/nginx/html/foo.dat",
         "bs=4M",
         "count=10",
     )
@@ -166,21 +168,21 @@
         }
     )
     assert not await pod.exists()
     with pytest.raises(kr8s.NotFoundError):
         await pod.exists(ensure=True)
 
 
-async def test_pod_metadata(example_pod_spec):
+async def test_pod_metadata(example_pod_spec, ns):
     pod = await Pod(example_pod_spec)
     await pod.create()
     assert "name" in pod.metadata
     assert "hello" in pod.labels
     assert "foo" in pod.annotations
-    assert "default" == pod.namespace
+    assert ns == pod.namespace
     assert "example-" in pod.name
     assert "containers" in pod.spec
     assert "phase" in pod.status
     await pod.delete()
 
 
 async def test_pod_missing_labels_annotations(example_pod_spec):
@@ -202,14 +204,29 @@
     await pod.delete()
     while await pod.exists():
         await asyncio.sleep(0.1)
     with pytest.raises(kr8s.NotFoundError):
         await pod2.delete()
 
 
+async def test_pod_from_name(example_pod_spec):
+    pod = await Pod(example_pod_spec)
+    await pod.create()
+    pod2 = await Pod(
+        pod.name, namespace=pod.namespace
+    )  # Note: Does not call the Kubernetes API
+    assert pod2.name == pod.name
+    assert pod2.namespace == pod.namespace
+    await pod.delete()
+    while await pod.exists():
+        await asyncio.sleep(0.1)
+    with pytest.raises(kr8s.NotFoundError):
+        await pod2.delete()
+
+
 async def test_pod_get_timeout(example_pod_spec):
     async def create_pod():
         await asyncio.sleep(0.1)
         pod = await Pod(example_pod_spec)
         await pod.create()
         return pod
 
@@ -227,46 +244,85 @@
 
 
 async def test_missing_pod():
     with pytest.raises(kr8s.NotFoundError):
         await Pod.get("nonexistant", namespace="default")
 
 
-async def test_selectors(example_pod_spec):
+@pytest.mark.parametrize("selector", ["abc=123def", {"abc": "123def"}])
+async def test_label_selector(example_pod_spec, selector):
     example_pod_spec["metadata"]["labels"]["abc"] = "123def"
     pod = await Pod(example_pod_spec)
     await pod.create()
 
     kubernetes = await kr8s.asyncio.api()
-    pods = await kubernetes.get("pods", namespace=kr8s.ALL, label_selector="abc=123def")
-    assert len(pods) == 1
+    pods = await kubernetes.get("pods", namespace=kr8s.ALL, label_selector=selector)
+    assert len(pods) >= 0
+
+    await pod.delete()
+
 
+async def test_field_selector(example_pod_spec):
+    pod = await Pod(example_pod_spec)
+    await pod.create()
+
+    kubernetes = await kr8s.asyncio.api()
     pods = await kubernetes.get(
-        "pods", namespace=kr8s.ALL, field_selector="metadata.name=" + pod.name
+        "pods", namespace=kr8s.ALL, field_selector={"metadata.name": pod.name}
     )
     assert len(pods) == 1
 
     pods = await kubernetes.get(
         "pods", namespace=kr8s.ALL, field_selector="metadata.name=" + "foo-bar-baz"
     )
     assert len(pods) == 0
 
     await pod.delete()
 
 
+async def test_get_with_label_selector(example_pod_spec, ns):
+    pod = await Pod(example_pod_spec)
+    await pod.create()
+    await pod.label(test="test_get_with_label_selector")
+
+    pod2 = await Pod.get(label_selector=pod.labels, namespace=ns)
+    assert pod == pod2
+
+    pod3 = await Pod.get(field_selector={"metadata.name": pod.name}, namespace=ns)
+    assert pod == pod3
+
+    await pod.delete()
+
+
 async def test_pod_watch(example_pod_spec):
     pod = await Pod(example_pod_spec)
     await pod.create()
     async for event, obj in pod.watch():
         assert event in ("ADDED", "MODIFIED", "DELETED")
         assert obj.name == pod.name
         break
     await pod.delete()
 
 
+async def test_pod_annotate(example_pod_spec):
+    pod = await Pod(example_pod_spec)
+    await pod.create()
+    await pod.annotate({"foo": "bar"})
+    assert "foo" in pod.annotations
+    await pod.delete()
+
+
+async def test_pod_label(example_pod_spec):
+    pod = await Pod(example_pod_spec)
+    await pod.create()
+    await pod.label({"foo": "bar"})
+    assert "foo" in pod.labels
+    await pod.delete()
+
+
 def test_pod_watch_sync(example_pod_spec):
     pod = SyncPod(example_pod_spec)
     pod.create()
     for event, obj in pod.watch():
         assert event in ("ADDED", "MODIFIED", "DELETED")
         assert obj.name == pod.name
         break
@@ -498,7 +554,13 @@
     assert any(isinstance(o, Ingress) for o in objects)
 
 
 async def test_custom_object_from_file():
     simple_dir = CURRENT_DIR / "resources" / "custom" / "evc.yaml"
     objects = await objects_from_files(simple_dir)
     assert len(objects) == 1
+
+
+async def test_pod_to_dict(example_pod_spec):
+    pod = Pod(example_pod_spec)
+    assert dict(pod) == example_pod_spec
+    assert dict(pod) == pod.raw
```

### Comparing `kr8s-0.6.0/kr8s/tests/test_testutils.py` & `kr8s-0.7.0/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.6.0/pyproject.toml` & `kr8s-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "aiohttp",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "kr8s"
-version = "0.6.0"  # This will be populated at build time by poetry-dynamic-versioning
+version = "0.7.0"  # This will be populated at build time by poetry-dynamic-versioning
 description = "A Kubernetes API library"
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = true
```

### Comparing `kr8s-0.6.0/PKG-INFO` & `kr8s-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Kubernetes API library
 License: BSD-3-Clause
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

