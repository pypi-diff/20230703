# Comparing `tmp/qxxkey-0.0.2.tar.gz` & `tmp/qxxkey-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qxxkey-0.0.2.tar", max compression
+gzip compressed data, was "qxxkey-0.0.3.tar", max compression
```

## Comparing `qxxkey-0.0.2.tar` & `qxxkey-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      249 2023-07-03 09:25:40.643664 qxxkey-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       24 2023-07-03 09:18:09.435120 qxxkey-0.0.2/qxxkey/__init__.py
--rw-r--r--   0        0        0     1297 2023-07-03 09:24:13.078137 qxxkey-0.0.2/qxxkey/vault.py
--rw-r--r--   0        0        0        0 2023-07-03 08:39:08.911479 qxxkey-0.0.2/README.md
--rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 qxxkey-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-07-03 09:44:15.848388 qxxkey-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-07-03 09:18:09.435120 qxxkey-0.0.3/qxxkey/__init__.py
+-rw-r--r--   0        0        0     1618 2023-07-03 09:43:49.124341 qxxkey-0.0.3/qxxkey/vault.py
+-rw-r--r--   0        0        0        0 2023-07-03 08:39:08.911479 qxxkey-0.0.3/README.md
+-rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 qxxkey-0.0.3/PKG-INFO
```

### Comparing `qxxkey-0.0.2/qxxkey/vault.py` & `qxxkey-0.0.3/qxxkey/vault.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 class Vault:
     def __init__(self, alias):
         import os
         import json
 
         self.alias = alias
-        self.appdata = os.getenv("APPDATA")
-
         self.cwd = os.getcwd()
+
+        # get appdata direcotry weather it is windows or linux or mac
+        if os.name == "nt":
+            self.appdata = os.getenv("APPDATA")
+        else:
+            print("This machine is not natively supported. The local appdata directory will be used. If you want this to change please open an issue on github.")
+            self.appdata = self.cwd
+
         self.vault_path = os.path.join(self.appdata, "qxxkey", "vaults", self.alias + ".json")
 
         if not os.path.exists(self.vault_path):
             self.new()
         else:
             with open(self.vault_path, "r") as f:
                 self.vault = json.load(f)
```

