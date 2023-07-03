# Comparing `tmp/manabi-1.0.0.tar.gz` & `tmp/manabi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manabi-1.0.0.tar", max compression
+gzip compressed data, was "manabi-1.1.0.tar", max compression
```

## Comparing `manabi-1.0.0.tar` & `manabi-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2519 2023-06-20 12:52:14.834699 manabi-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-05-31 17:06:59.165102 manabi-1.0.0/LICENSE
--rw-r--r--   0        0        0     5260 2023-06-19 16:02:10.707837 manabi-1.0.0/README.md
--rw-r--r--   0        0        0     1372 2023-06-15 12:40:23.020940 manabi-1.0.0/manabi/__init__.py
--rw-r--r--   0        0        0     4300 2023-06-16 14:47:50.897983 manabi-1.0.0/manabi/auth.py
--rw-r--r--   0        0        0     3471 2023-06-19 16:02:10.707837 manabi-1.0.0/manabi/filesystem.py
--rw-r--r--   0        0        0    10021 2023-06-15 12:40:23.020940 manabi-1.0.0/manabi/lock.py
--rw-r--r--   0        0        0     2681 2023-06-15 12:40:23.020940 manabi-1.0.0/manabi/log.py
--rw-r--r--   0        0        0      273 2023-06-15 12:40:23.020940 manabi-1.0.0/manabi/mypy_fix.py
--rw-r--r--   0        0        0     4401 2023-06-16 14:27:26.837088 manabi-1.0.0/manabi/token.py
--rw-r--r--   0        0        0      410 2023-06-09 10:43:33.248961 manabi-1.0.0/manabi/type_alias.py
--rw-r--r--   0        0        0     2763 2023-06-19 16:02:10.707837 manabi-1.0.0/manabi/util.py
--rw-r--r--   0        0        0        0 2023-05-31 17:07:00.845155 manabi-1.0.0/manabi_django/manabi_migrations/__init__.py
--rw-r--r--   0        0        0      165 2023-05-31 17:07:00.845155 manabi-1.0.0/manabi_django/manabi_migrations/apps.py
--rw-r--r--   0        0        0      532 2023-05-31 17:07:00.845155 manabi-1.0.0/manabi_django/manabi_migrations/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-31 17:07:00.845155 manabi-1.0.0/manabi_django/manabi_migrations/migrations/__init__.py
--rw-r--r--   0        0        0      200 2023-05-31 17:07:00.845155 manabi-1.0.0/manabi_django/manabi_migrations/models.py
--rw-r--r--   0        0        0     2428 2023-06-20 12:34:52.252687 manabi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6510 1970-01-01 00:00:00.000000 manabi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2716 2023-07-03 13:09:03.092631 manabi-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-05-31 17:06:59.165102 manabi-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5260 2023-06-19 16:02:10.707837 manabi-1.1.0/README.md
+-rw-r--r--   0        0        0     1372 2023-06-15 12:40:23.020940 manabi-1.1.0/manabi/__init__.py
+-rw-r--r--   0        0        0     4300 2023-06-16 14:47:50.897983 manabi-1.1.0/manabi/auth.py
+-rw-r--r--   0        0        0     4277 2023-06-21 14:54:48.018204 manabi-1.1.0/manabi/filesystem.py
+-rw-r--r--   0        0        0    10021 2023-06-15 12:40:23.020940 manabi-1.1.0/manabi/lock.py
+-rw-r--r--   0        0        0     2681 2023-06-15 12:40:23.020940 manabi-1.1.0/manabi/log.py
+-rw-r--r--   0        0        0      273 2023-06-15 12:40:23.020940 manabi-1.1.0/manabi/mypy_fix.py
+-rw-r--r--   0        0        0     4401 2023-06-16 14:27:26.837088 manabi-1.1.0/manabi/token.py
+-rw-r--r--   0        0        0      524 2023-06-21 14:54:48.024870 manabi-1.1.0/manabi/type_alias.py
+-rw-r--r--   0        0        0     2763 2023-06-19 16:02:10.707837 manabi-1.1.0/manabi/util.py
+-rw-r--r--   0        0        0        0 2023-05-31 17:07:00.845155 manabi-1.1.0/manabi_django/manabi_migrations/__init__.py
+-rw-r--r--   0        0        0      165 2023-05-31 17:07:00.845155 manabi-1.1.0/manabi_django/manabi_migrations/apps.py
+-rw-r--r--   0        0        0      532 2023-05-31 17:07:00.845155 manabi-1.1.0/manabi_django/manabi_migrations/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-31 17:07:00.845155 manabi-1.1.0/manabi_django/manabi_migrations/migrations/__init__.py
+-rw-r--r--   0        0        0      200 2023-05-31 17:07:00.845155 manabi-1.1.0/manabi_django/manabi_migrations/models.py
+-rw-r--r--   0        0        0     2428 2023-07-03 13:06:49.898682 manabi-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6510 1970-01-01 00:00:00.000000 manabi-1.1.0/PKG-INFO
```

### Comparing `manabi-1.0.0/CHANGELOG.md` & `manabi-1.1.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.1.0 (2023-07-03)
+
+### Feature
+* Add pre_write_callback and hook/callback approve write ([`08b6a6f`](https://github.com/projectcaluma/manabi/commit/08b6a6fe2ea76e006de17cc0a7f0be35f2b1e1f6))
+
 ## v1.0.0 (2023-06-20)
 
 ### Feature
 * feat(hook): add pre_write_hook ([`4de0ad6`](https://github.com/projectcaluma/manabi/commit/4de0ad65b95bbd0be5fa19ed986660233fcd6b6c))
 
 ### Fix
 * fix: fuzzying found relative urls like '..' ([`e74b263`](https://github.com/projectcaluma/manabi/commit/e74b2638f9413b339988dea52eb2b8747262a2dc))
```

### Comparing `manabi-1.0.0/LICENSE` & `manabi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manabi-1.0.0/README.md` & `manabi-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `manabi-1.0.0/manabi/__init__.py` & `manabi-1.1.0/manabi/__init__.py`

 * *Files identical despite different names*

### Comparing `manabi-1.0.0/manabi/auth.py` & `manabi-1.1.0/manabi/auth.py`

 * *Files identical despite different names*

### Comparing `manabi-1.0.0/manabi/filesystem.py` & `manabi-1.1.0/manabi/filesystem.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from wsgidav.dav_error import HTTP_FORBIDDEN, DAVError
 from wsgidav.fs_dav_provider import FileResource, FilesystemProvider, FolderResource
 
 from .token import Token
+from .type_alias import PreWriteType
 from .util import requests_session
 
 
 class ManabiFolderResource(FolderResource):
     def get_member_names(self):
         token: Token = self.environ["manabi.token"]
         # type manually checked
@@ -47,16 +48,25 @@
         raise DAVError(HTTP_FORBIDDEN)
 
     def set_last_modified(self, dest_path, time_stamp, dry_run):
         raise DAVError(HTTP_FORBIDDEN)
 
 
 class ManabiFileResource(FileResource):
-    def __init__(self, path, environ, file_path, pre_write_hook=None):
+    def __init__(
+        self,
+        path,
+        environ,
+        file_path,
+        *,
+        pre_write_hook: Optional[str] = None,
+        pre_write_callback: Optional[PreWriteType] = None,
+    ):
         self._pre_write_hook = pre_write_hook
+        self._pre_write_callback = pre_write_callback
         self._token = environ["manabi.token"]
         super().__init__(path, environ, file_path)
 
     def delete(self):
         raise DAVError(HTTP_FORBIDDEN)
 
     def copy_move_single(self, dest_path, is_move):
@@ -65,29 +75,44 @@
     def support_recursive_move(self, dest_path):
         return False
 
     def move_recursive(self, dest_path):
         raise DAVError(HTTP_FORBIDDEN)
 
     def begin_write(self, *, content_type):
-        pre = self._pre_write_hook
         token = self._token
-        if pre and token:
-            session = requests_session()
-            session.post(pre, data=token.encode())
-        # The webhhook returned and hopefully created a new version.
-        # Now we can save.
+        if token:
+            pre_hook = self._pre_write_hook
+            pre_callback = self._pre_write_callback
+
+            if pre_hook:
+                session = requests_session()
+                res = session.post(pre_hook, data=token.encode())
+                if res.status_code != 200:
+                    raise DAVError(HTTP_FORBIDDEN)
+            if pre_callback:
+                if not pre_callback(token):
+                    raise DAVError(HTTP_FORBIDDEN)
+            # The hook returned and hopefully created a new version.
+            # Now we can save.
         return super().begin_write(content_type=content_type)
 
 
 class ManabiProvider(FilesystemProvider):
     def __init__(
-        self, root_folder, *, readonly=False, shadow=None, pre_write_hook=None
+        self,
+        root_folder,
+        *,
+        readonly=False,
+        shadow=None,
+        pre_write_hook: Optional[str] = None,
+        pre_write_callback: Optional[PreWriteType] = None,
     ):
         self._pre_write_hook = pre_write_hook
+        self._pre_write_callback = pre_write_callback
         super().__init__(root_folder, readonly=readonly, shadow=shadow)
 
     def get_resource_inst(self, path: str, environ: Dict[str, Any]):
         token: Token = environ["manabi.token"]
         dir_access = environ["manabi.dir_access"]
         if dir_access:
             assert token.path
@@ -99,11 +124,12 @@
             path = token.path_as_url()
             fp = self._loc_to_file_path(path, environ)
             if Path(fp).exists():
                 return ManabiFileResource(
                     path,
                     environ,
                     fp,
-                    self._pre_write_hook,
+                    pre_write_hook=self._pre_write_hook,
+                    pre_write_callback=self._pre_write_callback,
                 )
             else:
                 return None
```

### Comparing `manabi-1.0.0/manabi/lock.py` & `manabi-1.1.0/manabi/lock.py`

 * *Files identical despite different names*

### Comparing `manabi-1.0.0/manabi/log.py` & `manabi-1.1.0/manabi/log.py`

 * *Files identical despite different names*

### Comparing `manabi-1.0.0/manabi/token.py` & `manabi-1.1.0/manabi/token.py`

 * *Files identical despite different names*

### Comparing `manabi-1.0.0/manabi/util.py` & `manabi-1.1.0/manabi/util.py`

 * *Files identical despite different names*

### Comparing `manabi-1.0.0/manabi_django/manabi_migrations/migrations/0001_initial.py` & `manabi-1.1.0/manabi_django/manabi_migrations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `manabi-1.0.0/pyproject.toml` & `manabi-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "manabi"
-version = "1.0.0"
+version = "1.1.0"
 description = "Provide WebDAV access for documents."
 homepage = "https://github.com/projectcaluma/manabi"
 repository = "https://github.com/projectcaluma/manabi"
 authors = ["Adfinis AG"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
```

### Comparing `manabi-1.0.0/PKG-INFO` & `manabi-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manabi
-Version: 1.0.0
+Version: 1.1.0
 Summary: Provide WebDAV access for documents.
 Home-page: https://github.com/projectcaluma/manabi
 License: AGPL-3.0-or-later
 Author: Adfinis AG
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

