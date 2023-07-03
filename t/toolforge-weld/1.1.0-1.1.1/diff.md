# Comparing `tmp/toolforge-weld-1.1.0.tar.gz` & `tmp/toolforge-weld-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge-weld-1.1.0.tar", last modified: Mon Jun  5 17:51:10 2023, max compression
+gzip compressed data, was "toolforge-weld-1.1.1.tar", last modified: Mon Jul  3 11:53:15 2023, max compression
```

## Comparing `toolforge-weld-1.1.0.tar` & `toolforge-weld-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 17:51:10.111992 toolforge-weld-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    34524 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-05 17:51:10.111992 toolforge-weld-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 17:51:10.111992 toolforge-weld-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      969 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 17:51:10.107992 toolforge-weld-1.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/tests/test_api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2642 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/tests/test_kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)     4508 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/tests/test_kubernetes_config.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 17:51:10.111992 toolforge-weld-1.1.0/toolforge_weld/
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3503 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     3435 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     7555 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)     3684 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/kubernetes_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 17:51:10.111992 toolforge-weld-1.1.0/toolforge_weld/logs/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/logs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2456 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/logs/kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/logs/source.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-06-05 17:51:00.000000 toolforge-weld-1.1.0/toolforge_weld/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 17:51:10.111992 toolforge-weld-1.1.0/toolforge_weld.egg-info/
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-05 17:51:10.000000 toolforge-weld-1.1.0/toolforge_weld.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      668 2023-06-05 17:51:10.000000 toolforge-weld-1.1.0/toolforge_weld.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 17:51:10.000000 toolforge-weld-1.1.0/toolforge_weld.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-05 17:51:10.000000 toolforge-weld-1.1.0/toolforge_weld.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-05 17:51:10.000000 toolforge-weld-1.1.0/toolforge_weld.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:53:15.760692 toolforge-weld-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)    34524 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      686 2023-07-03 11:53:15.760692 toolforge-weld-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 11:53:15.760692 toolforge-weld-1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      969 2023-07-03 11:47:16.000000 toolforge-weld-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:53:15.756692 toolforge-weld-1.1.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/tests/test_api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2642 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/tests/test_kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4508 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/tests/test_kubernetes_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:53:15.756692 toolforge-weld-1.1.1/toolforge_weld/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3503 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3435 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7730 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3684 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/kubernetes_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:53:15.760692 toolforge-weld-1.1.1/toolforge_weld/logs/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/logs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2456 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/logs/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/logs/source.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 11:53:07.000000 toolforge-weld-1.1.1/toolforge_weld/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-07-03 11:38:22.000000 toolforge-weld-1.1.1/toolforge_weld/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:53:15.760692 toolforge-weld-1.1.1/toolforge_weld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      686 2023-07-03 11:53:15.000000 toolforge-weld-1.1.1/toolforge_weld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      668 2023-07-03 11:53:15.000000 toolforge-weld-1.1.1/toolforge_weld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 11:53:15.000000 toolforge-weld-1.1.1/toolforge_weld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-03 11:53:15.000000 toolforge-weld-1.1.1/toolforge_weld.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-03 11:53:15.000000 toolforge-weld-1.1.1/toolforge_weld.egg-info/top_level.txt
```

### Comparing `toolforge-weld-1.1.0/LICENSE` & `toolforge-weld-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.0/PKG-INFO` & `toolforge-weld-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolforge-weld
-Version: 1.1.0
+Version: 1.1.1
 Summary: Shared Python code for Toolforge infrastructure components
 Author: Taavi Väänänen
 Author-email: hi@taavi.wtf
 License: AGPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `toolforge-weld-1.1.0/setup.py` & `toolforge-weld-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 
 setup(
     name="toolforge-weld",
-    version="1.1.0",
+    version="1.1.1",
     author="Taavi Väänänen",
     author_email="hi@taavi.wtf",
     license="AGPL-3.0-or-later",
     packages=find_packages(),
     package_data={"toolforge_weld": ["py.typed"]},
     description="Shared Python code for Toolforge infrastructure components",
     long_description=(this_directory / "README.md").read_text(),
```

### Comparing `toolforge-weld-1.1.0/tests/test_api_client.py` & `toolforge-weld-1.1.1/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.0/tests/test_config.py` & `toolforge-weld-1.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.0/tests/test_kubernetes_config.py` & `toolforge-weld-1.1.1/tests/test_kubernetes_config.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.0/toolforge_weld/api_client.py` & `toolforge-weld-1.1.1/toolforge_weld/api_client.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.0/toolforge_weld/config.py` & `toolforge-weld-1.1.1/toolforge_weld/config.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.0/toolforge_weld/errors.py` & `toolforge-weld-1.1.1/toolforge_weld/errors.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.0/toolforge_weld/kubernetes.py` & `toolforge-weld-1.1.1/toolforge_weld/kubernetes.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,18 @@
     """Base class for exceptions related to the Kubernetes client."""
 
 
 class KubernetesConfigFileNotFoundException(ToolforgeKubernetesError):
     """Raised when a Kubernetes client is attempted to be created but the configuration file does not exist."""
 
 
+def _format_labels(labels: Dict[str, str]) -> str:
+    return ",".join([f"{k}={v}" for k, v in labels.items()])
+
+
 class K8sClient(ToolforgeClient):
     """Kubernetes API client."""
 
     VERSIONS: ClassVar[Dict[str, str]] = {
         "configmaps": "v1",
         "cronjobs": "batch/v1",
         "deployments": "apps/v1",
@@ -109,17 +113,15 @@
         field_selector: Optional[Dict[str, Any]] = None,
         namespace: Optional[str] = None,
     ) -> List[Dict[str, Any]]:
         """Get list of objects of the given kind in the namespace."""
         params: Dict[str, Any] = {}
 
         if label_selector:
-            params["labelSelector"] = ",".join(
-                [f"{k}={v}" for k, v in label_selector.items()]
-            )
+            params["labelSelector"] = _format_labels(label_selector)
         if field_selector:
             params["fieldSelector"] = field_selector
 
         return self.get(
             kind,
             params=params,
             version=K8sClient.VERSIONS[kind],
@@ -138,17 +140,21 @@
             for svc in self.get_objects(kind, label_selector=label_selector):
                 self.delete(
                     kind,
                     name=svc["metadata"]["name"],
                     version=K8sClient.VERSIONS[kind],
                 )
         else:
+            params: Dict[str, Any] = {}
+            if label_selector:
+                params["labelSelector"] = _format_labels(label_selector)
+
             self.delete(
                 kind,
-                params={"labelSelector": label_selector},
+                params=params,
                 version=K8sClient.VERSIONS[kind],
             )
 
     def create_object(self, kind: str, spec: Dict[str, Any]):
         """Create an object of the given kind in the namespace."""
         return self.post(
             kind,
```

### Comparing `toolforge-weld-1.1.0/toolforge_weld/kubernetes_config.py` & `toolforge-weld-1.1.1/toolforge_weld/kubernetes_config.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.0/toolforge_weld/logs/__init__.py` & `toolforge-weld-1.1.1/toolforge_weld/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.0/toolforge_weld/logs/kubernetes.py` & `toolforge-weld-1.1.1/toolforge_weld/logs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.0/toolforge_weld/logs/source.py` & `toolforge-weld-1.1.1/toolforge_weld/logs/source.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-1.1.0/toolforge_weld.egg-info/PKG-INFO` & `toolforge-weld-1.1.1/toolforge_weld.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolforge-weld
-Version: 1.1.0
+Version: 1.1.1
 Summary: Shared Python code for Toolforge infrastructure components
 Author: Taavi Väänänen
 Author-email: hi@taavi.wtf
 License: AGPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `toolforge-weld-1.1.0/toolforge_weld.egg-info/SOURCES.txt` & `toolforge-weld-1.1.1/toolforge_weld.egg-info/SOURCES.txt`

 * *Files identical despite different names*

