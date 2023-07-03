# Comparing `tmp/poe_shell-0.1.5.tar.gz` & `tmp/poe_shell-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poe_shell-0.1.5.tar", max compression
+gzip compressed data, was "poe_shell-0.1.6.tar", max compression
```

## Comparing `poe_shell-0.1.5.tar` & `poe_shell-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,14 @@
--rw-r--r--   0        0        0      760 2023-06-30 04:11:45.326714 poe_shell-0.1.5/README.md
--rw-r--r--   0        0        0       35 2023-06-30 07:35:34.125904 poe_shell-0.1.5/poe_shell/__init__.py
--rw-r--r--   0        0        0     1560 2023-06-30 08:29:11.644029 poe_shell-0.1.5/poe_shell/__main__.py
--rw-r--r--   0        0        0       67 2023-06-30 08:28:39.799053 poe_shell-0.1.5/poe_shell/config.py
--rw-r--r--   0        0        0        0 2023-06-30 03:02:37.315128 poe_shell-0.1.5/poe_shell/handlers/__init__.py
--rw-r--r--   0        0        0      180 2023-06-30 03:04:19.592632 poe_shell-0.1.5/poe_shell/handlers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2015 2023-06-30 03:59:17.025656 poe_shell-0.1.5/poe_shell/handlers/__pycache__/chat_handler.cpython-311.pyc
--rw-r--r--   0        0        0     1063 2023-06-30 03:26:22.131426 poe_shell-0.1.5/poe_shell/handlers/__pycache__/handler.cpython-311.pyc
--rw-r--r--   0        0        0     1187 2023-06-30 03:27:40.596752 poe_shell-0.1.5/poe_shell/handlers/__pycache__/one_off_handler.cpython-311.pyc
--rw-r--r--   0        0        0     2761 2023-06-30 03:29:26.961034 poe_shell-0.1.5/poe_shell/handlers/__pycache__/shell_handler.cpython-311.pyc
--rw-r--r--   0        0        0      942 2023-06-30 03:28:19.430015 poe_shell-0.1.5/poe_shell/handlers/chat_handler.py
--rw-r--r--   0        0        0      291 2023-06-30 03:22:17.474038 poe_shell-0.1.5/poe_shell/handlers/handler.py
--rw-r--r--   0        0        0      375 2023-06-30 03:22:44.232937 poe_shell-0.1.5/poe_shell/handlers/one_off_handler.py
--rw-r--r--   0        0        0     1634 2023-06-30 08:37:45.068549 poe_shell-0.1.5/poe_shell/handlers/shell_handler.py
--rw-r--r--   0        0        0      889 2023-06-30 08:30:30.576523 poe_shell-0.1.5/poe_shell/poe_client.py
--rw-r--r--   0        0        0     1245 2023-06-30 03:02:37.315873 poe_shell-0.1.5/poe_shell/roles.py
--rw-r--r--   0        0        0      646 2023-06-30 03:02:37.315982 poe_shell-0.1.5/poe_shell/utils.py
--rw-r--r--   0        0        0      424 2023-06-30 08:38:46.974239 poe_shell-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 poe_shell-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      760 2023-06-30 04:11:45.326714 poe_shell-0.1.6/README.md
+-rw-r--r--   0        0        0       35 2023-06-30 07:35:34.125904 poe_shell-0.1.6/poe_shell/__init__.py
+-rw-r--r--   0        0        0     1825 2023-07-03 08:41:25.597445 poe_shell-0.1.6/poe_shell/__main__.py
+-rw-r--r--   0        0        0       67 2023-06-30 08:28:39.799053 poe_shell-0.1.6/poe_shell/config.py
+-rw-r--r--   0        0        0        0 2023-06-30 03:02:37.315128 poe_shell-0.1.6/poe_shell/handlers/__init__.py
+-rw-r--r--   0        0        0      942 2023-06-30 03:28:19.430015 poe_shell-0.1.6/poe_shell/handlers/chat_handler.py
+-rw-r--r--   0        0        0      291 2023-06-30 03:22:17.474038 poe_shell-0.1.6/poe_shell/handlers/handler.py
+-rw-r--r--   0        0        0      375 2023-06-30 03:22:44.232937 poe_shell-0.1.6/poe_shell/handlers/one_off_handler.py
+-rw-r--r--   0        0        0     1837 2023-07-03 08:39:26.017436 poe_shell-0.1.6/poe_shell/handlers/shell_handler.py
+-rw-r--r--   0        0        0     1172 2023-07-03 08:18:33.605929 poe_shell-0.1.6/poe_shell/poe_client.py
+-rw-r--r--   0        0        0     1245 2023-06-30 03:02:37.315873 poe_shell-0.1.6/poe_shell/roles.py
+-rw-r--r--   0        0        0      646 2023-06-30 03:02:37.315982 poe_shell-0.1.6/poe_shell/utils.py
+-rw-r--r--   0        0        0      424 2023-07-03 08:46:28.881318 poe_shell-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 poe_shell-0.1.6/PKG-INFO
```

### Comparing `poe_shell-0.1.5/README.md` & `poe_shell-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.5/poe_shell/__main__.py` & `poe_shell-0.1.6/poe_shell/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,27 +29,37 @@
     ),
     bots: bool = typer.Option(
         False,
         "--bots",
         help="Return the list of bots.",
         rich_help_panel="Assistance Options",
     ),
+    remove_api_key: bool = typer.Option(
+        False,
+        "--remove-api-key",
+        help="Remove the saved API key.",
+        rich_help_panel="Assistance Options",
+    ),
 ):
     if not os.path.exists(STORAGE_PATH):
         os.makedirs(STORAGE_PATH)
 
-    client = PoeClient().client
+    if remove_api_key:
+        PoeClient().remove_api_key()
+        return
+
+    client = PoeClient().connect()
 
     stdin_passed = not sys.stdin.isatty()
 
     if shell:
         from .handlers.shell_handler import ShellHandler
 
         handler = ShellHandler(client)
-        handler.handle()
+        handler.handle(message)
 
     elif bots:
         list = client.bot_names
         print(list)
 
     elif chat:
         from .handlers.chat_handler import ChatHandler
```

### Comparing `poe_shell-0.1.5/poe_shell/handlers/chat_handler.py` & `poe_shell-0.1.6/poe_shell/handlers/chat_handler.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.5/poe_shell/poe_client.py` & `poe_shell-0.1.6/poe_shell/poe_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import poe
 import pickle
+import os
 
 from .config import STORAGE_PATH
 
 
 class PoeClient:
     API_KEY_PICKLE_FILE = STORAGE_PATH + "api_key.pickle"
 
-    def __init__(self):
+    def connect(self) -> poe.Client:
         api_key = self.get_api_key()
 
         if api_key is None:
             api_key = self.set_api_key()
 
         self.client = poe.Client(self.get_api_key())
+        return self.client
 
     def get_api_key(self) -> str | None:
         """Get the API Key from pickled file."""
         try:
             with open(self.API_KEY_PICKLE_FILE, "rb") as f:
                 return pickle.load(f)
         except FileNotFoundError:
@@ -28,7 +30,15 @@
         api_key = input("Please enter your POE API key: ").strip()
 
         with open(self.API_KEY_PICKLE_FILE, "wb") as f:
             pickle.dump(api_key, f)
         print("API key saved.")
 
         return api_key
+
+    def remove_api_key(self):
+        """Remove the API Key from the pickled file."""
+        try:
+            os.remove(self.API_KEY_PICKLE_FILE)
+        except FileNotFoundError:
+            pass
+        print("API key removed.")
```

### Comparing `poe_shell-0.1.5/poe_shell/roles.py` & `poe_shell-0.1.6/poe_shell/roles.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.5/poe_shell/utils.py` & `poe_shell-0.1.6/poe_shell/utils.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.5/PKG-INFO` & `poe_shell-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-shell
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Samson Hui
 Author-email: hui.kawang@yahoo.com.hk
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: poe-api (>=0.4.6,<0.5.0)
```

