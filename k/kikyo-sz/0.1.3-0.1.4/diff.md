# Comparing `tmp/kikyo-sz-0.1.3.tar.gz` & `tmp/kikyo-sz-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kikyo-sz-0.1.3.tar", last modified: Thu Mar 16 08:38:35 2023, max compression
+gzip compressed data, was "dist/kikyo-sz-0.1.4.tar", last modified: Mon Jul  3 03:17:37 2023, max compression
```

## Comparing `kikyo-sz-0.1.3.tar` & `kikyo-sz-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-03-16 08:38:35.000000 kikyo-sz-0.1.3/
--rw-r--r--   0 jadbin     (501) staff       (20)     1063 2021-03-30 06:22:21.000000 kikyo-sz-0.1.3/LICENSE
--rw-r--r--   0 jadbin     (501) staff       (20)      141 2023-03-14 08:19:45.000000 kikyo-sz-0.1.3/MANIFEST.in
--rw-r--r--   0 jadbin     (501) staff       (20)      484 2023-03-16 08:38:35.000000 kikyo-sz-0.1.3/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)       36 2023-03-14 08:10:35.000000 kikyo-sz-0.1.3/README.rst
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-03-16 08:38:35.000000 kikyo-sz-0.1.3/kikyo_sz/
--rw-r--r--   0 jadbin     (501) staff       (20)       22 2023-03-16 08:38:26.000000 kikyo-sz-0.1.3/kikyo_sz/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      132 2023-03-16 01:40:07.000000 kikyo-sz-0.1.3/kikyo_sz/config.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1939 2023-03-16 01:45:18.000000 kikyo-sz-0.1.3/kikyo_sz/oss.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-03-16 08:38:35.000000 kikyo-sz-0.1.3/kikyo_sz.egg-info/
--rw-r--r--   0 jadbin     (501) staff       (20)      484 2023-03-16 08:38:35.000000 kikyo-sz-0.1.3/kikyo_sz.egg-info/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)      386 2023-03-16 08:38:35.000000 kikyo-sz-0.1.3/kikyo_sz.egg-info/SOURCES.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2023-03-16 08:38:35.000000 kikyo-sz-0.1.3/kikyo_sz.egg-info/dependency_links.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       43 2023-03-16 08:38:35.000000 kikyo-sz-0.1.3/kikyo_sz.egg-info/entry_points.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2023-03-14 08:18:27.000000 kikyo-sz-0.1.3/kikyo_sz.egg-info/not-zip-safe
--rw-r--r--   0 jadbin     (501) staff       (20)       45 2023-03-16 08:38:35.000000 kikyo-sz-0.1.3/kikyo_sz.egg-info/requires.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        9 2023-03-16 08:38:35.000000 kikyo-sz-0.1.3/kikyo_sz.egg-info/top_level.txt
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-03-16 08:38:35.000000 kikyo-sz-0.1.3/requirements/
--rw-r--r--   0 jadbin     (501) staff       (20)       18 2021-03-30 06:22:21.000000 kikyo-sz-0.1.3/requirements/test.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       38 2023-03-16 08:38:35.000000 kikyo-sz-0.1.3/setup.cfg
--rw-r--r--   0 jadbin     (501) staff       (20)     1948 2023-03-16 08:38:31.000000 kikyo-sz-0.1.3/setup.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-03-16 08:38:35.000000 kikyo-sz-0.1.3/tests/
--rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-03-30 06:22:21.000000 kikyo-sz-0.1.3/tests/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      538 2023-03-16 01:32:54.000000 kikyo-sz-0.1.3/tests/test_filesys_oss.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/
+-rw-r--r--   0 jadbin     (501) staff       (20)     1063 2021-03-30 06:22:21.000000 kikyo-sz-0.1.4/LICENSE
+-rw-r--r--   0 jadbin     (501) staff       (20)      141 2023-03-14 08:19:45.000000 kikyo-sz-0.1.4/MANIFEST.in
+-rw-r--r--   0 jadbin     (501) staff       (20)      484 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/PKG-INFO
+-rw-r--r--   0 jadbin     (501) staff       (20)       36 2023-03-14 08:10:35.000000 kikyo-sz-0.1.4/README.rst
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz/
+-rw-r--r--   0 jadbin     (501) staff       (20)       22 2023-07-03 03:17:12.000000 kikyo-sz-0.1.4/kikyo_sz/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      132 2023-03-16 01:40:07.000000 kikyo-sz-0.1.4/kikyo_sz/config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2288 2023-07-03 03:15:05.000000 kikyo-sz-0.1.4/kikyo_sz/oss.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/
+-rw-r--r--   0 jadbin     (501) staff       (20)      484 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/PKG-INFO
+-rw-r--r--   0 jadbin     (501) staff       (20)      386 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/SOURCES.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)        1 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/dependency_links.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)       43 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/entry_points.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)        1 2023-03-14 08:18:27.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/not-zip-safe
+-rw-r--r--   0 jadbin     (501) staff       (20)       45 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/requires.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)        9 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/kikyo_sz.egg-info/top_level.txt
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/requirements/
+-rw-r--r--   0 jadbin     (501) staff       (20)       18 2021-03-30 06:22:21.000000 kikyo-sz-0.1.4/requirements/test.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)       38 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/setup.cfg
+-rw-r--r--   0 jadbin     (501) staff       (20)     1948 2023-03-16 08:38:31.000000 kikyo-sz-0.1.4/setup.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2023-07-03 03:17:37.000000 kikyo-sz-0.1.4/tests/
+-rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-03-30 06:22:21.000000 kikyo-sz-0.1.4/tests/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      538 2023-03-16 01:32:54.000000 kikyo-sz-0.1.4/tests/test_filesys_oss.py
```

### Comparing `kikyo-sz-0.1.3/LICENSE` & `kikyo-sz-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kikyo-sz-0.1.3/kikyo_sz/oss.py` & `kikyo-sz-0.1.4/kikyo_sz/oss.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,7 +55,18 @@
 
         return self.get_object_link(key)
 
     def get_object(self, key: str) -> Any:
         resp = self._session.get(f'{self._name}/{key}')
         resp.raise_for_status()
         return resp.content
+
+    def object_exists(self, key: str) -> bool:
+        resp = self._session.head(f'{self._name}/{key}')
+        if resp.status_code == 404:
+            return False
+        resp.raise_for_status()
+        return True
+
+    def remove_object(self, key: str):
+        resp = self._session.delete(f'{self._name}/{key}')
+        resp.raise_for_status()
```

### Comparing `kikyo-sz-0.1.3/setup.py` & `kikyo-sz-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `kikyo-sz-0.1.3/tests/test_filesys_oss.py` & `kikyo-sz-0.1.4/tests/test_filesys_oss.py`

 * *Files identical despite different names*

