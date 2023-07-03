# Comparing `tmp/gitcoll-0.0.18.tar.gz` & `tmp/gitcoll-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitcoll-0.0.18.tar", last modified: Sat Jul  1 02:37:58 2023, max compression
+gzip compressed data, was "gitcoll-0.0.19.tar", last modified: Mon Jul  3 05:28:15 2023, max compression
```

## Comparing `gitcoll-0.0.18.tar` & `gitcoll-0.0.19.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 02:37:58.080368 gitcoll-0.0.18/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-01 02:37:54.000000 gitcoll-0.0.18/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12145 2023-07-01 02:37:58.080368 gitcoll-0.0.18/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11731 2023-06-11 11:48:27.000000 gitcoll-0.0.18/README.md
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-06-11 11:48:27.000000 gitcoll-0.0.18/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-07-01 02:37:58.080368 gitcoll-0.0.18/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      169 2023-06-11 11:48:27.000000 gitcoll-0.0.18/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 02:37:58.072368 gitcoll-0.0.18/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 02:37:58.080368 gitcoll-0.0.18/src/gcln/
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-11 11:48:27.000000 gitcoll-0.0.18/src/gcln/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6751 2023-06-11 11:48:27.000000 gitcoll-0.0.18/src/gcln/cfg_file.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-11 11:48:27.000000 gitcoll-0.0.18/src/gcln/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7232 2023-06-11 11:48:27.000000 gitcoll-0.0.18/src/gcln/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    43203 2023-06-11 11:48:27.000000 gitcoll-0.0.18/src/gcln/main.py
--rw-rw-rw-   0 root         (0) root         (0)    29661 2023-06-11 11:48:27.000000 gitcoll-0.0.18/src/gcln/main_context.py
--rw-rw-rw-   0 root         (0) root         (0)     4207 2023-06-11 11:48:27.000000 gitcoll-0.0.18/src/gcln/records.py
--rw-rw-rw-   0 root         (0) root         (0)    12693 2023-06-11 11:48:27.000000 gitcoll-0.0.18/src/gcln/srv_connector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 02:37:58.080368 gitcoll-0.0.18/src/gcln2/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-01 02:37:55.000000 gitcoll-0.0.18/src/gcln2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5317 2023-06-11 11:48:27.000000 gitcoll-0.0.18/src/gcln2/db.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-11 11:48:27.000000 gitcoll-0.0.18/src/gcln2/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8917 2023-06-11 11:48:27.000000 gitcoll-0.0.18/src/gcln2/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    37738 2023-07-01 02:37:54.000000 gitcoll-0.0.18/src/gcln2/main.py
--rw-rw-rw-   0 root         (0) root         (0)     2238 2023-06-11 11:48:27.000000 gitcoll-0.0.18/src/gcln2/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-06-11 11:48:27.000000 gitcoll-0.0.18/src/gcln2/yaml_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 02:37:58.080368 gitcoll-0.0.18/src/gitcoll.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12145 2023-07-01 02:37:58.000000 gitcoll-0.0.18/src/gitcoll.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-01 02:37:58.000000 gitcoll-0.0.18/src/gitcoll.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 02:37:58.000000 gitcoll-0.0.18/src/gitcoll.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-07-01 02:37:58.000000 gitcoll-0.0.18/src/gitcoll.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      115 2023-07-01 02:37:58.000000 gitcoll-0.0.18/src/gitcoll.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-01 02:37:58.000000 gitcoll-0.0.18/src/gitcoll.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 05:28:15.134808 gitcoll-0.0.19/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 05:28:11.000000 gitcoll-0.0.19/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    12145 2023-07-03 05:28:15.134808 gitcoll-0.0.19/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2023-06-11 11:48:27.000000 gitcoll-0.0.19/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-07-03 05:28:11.000000 gitcoll-0.0.19/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-07-03 05:28:15.134808 gitcoll-0.0.19/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      169 2023-06-11 11:48:27.000000 gitcoll-0.0.19/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 05:28:15.130807 gitcoll-0.0.19/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 05:28:15.134808 gitcoll-0.0.19/src/gcln/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-11 11:48:27.000000 gitcoll-0.0.19/src/gcln/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6751 2023-06-11 11:48:27.000000 gitcoll-0.0.19/src/gcln/cfg_file.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-11 11:48:27.000000 gitcoll-0.0.19/src/gcln/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7232 2023-06-11 11:48:27.000000 gitcoll-0.0.19/src/gcln/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    43203 2023-06-11 11:48:27.000000 gitcoll-0.0.19/src/gcln/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    29661 2023-06-11 11:48:27.000000 gitcoll-0.0.19/src/gcln/main_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     4207 2023-06-11 11:48:27.000000 gitcoll-0.0.19/src/gcln/records.py
+-rw-rw-rw-   0 root         (0) root         (0)    12693 2023-06-11 11:48:27.000000 gitcoll-0.0.19/src/gcln/srv_connector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 05:28:15.134808 gitcoll-0.0.19/src/gcln2/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-03 05:28:12.000000 gitcoll-0.0.19/src/gcln2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7717 2023-07-03 05:28:11.000000 gitcoll-0.0.19/src/gcln2/db.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-11 11:48:27.000000 gitcoll-0.0.19/src/gcln2/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8916 2023-07-03 05:28:11.000000 gitcoll-0.0.19/src/gcln2/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    38626 2023-07-03 05:28:11.000000 gitcoll-0.0.19/src/gcln2/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     2238 2023-06-11 11:48:27.000000 gitcoll-0.0.19/src/gcln2/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7888 2023-07-03 05:28:11.000000 gitcoll-0.0.19/src/gcln2/sync.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-06-11 11:48:27.000000 gitcoll-0.0.19/src/gcln2/yaml_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 05:28:15.134808 gitcoll-0.0.19/src/gitcoll.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12145 2023-07-03 05:28:15.000000 gitcoll-0.0.19/src/gitcoll.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-03 05:28:15.000000 gitcoll-0.0.19/src/gitcoll.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 05:28:15.000000 gitcoll-0.0.19/src/gitcoll.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-03 05:28:15.000000 gitcoll-0.0.19/src/gitcoll.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      115 2023-07-03 05:28:15.000000 gitcoll-0.0.19/src/gitcoll.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-03 05:28:15.000000 gitcoll-0.0.19/src/gitcoll.egg-info/top_level.txt
```

### Comparing `gitcoll-0.0.18/PKG-INFO` & `gitcoll-0.0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitcoll
-Version: 0.0.18
+Version: 0.0.19
 Summary: Git collection utilities
 Home-page: https://gitlab.com/jesrib/gitcoll
 Author: Jesper Ribbe
 Author-email: jesper@ribbe.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gitcoll-0.0.18/README.md` & `gitcoll-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.18/setup.cfg` & `gitcoll-0.0.19/setup.cfg`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.18/src/gcln/cfg_file.py` & `gitcoll-0.0.19/src/gcln/cfg_file.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.18/src/gcln/helpers.py` & `gitcoll-0.0.19/src/gcln/helpers.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.18/src/gcln/main.py` & `gitcoll-0.0.19/src/gcln/main.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.18/src/gcln/main_context.py` & `gitcoll-0.0.19/src/gcln/main_context.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.18/src/gcln/records.py` & `gitcoll-0.0.19/src/gcln/records.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.18/src/gcln/srv_connector.py` & `gitcoll-0.0.19/src/gcln/srv_connector.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.18/src/gcln2/helpers.py` & `gitcoll-0.0.19/src/gcln2/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,8 +262,7 @@
             parents = []
         comm_oid = r.create_commit("refs/heads/_config", signature, signature, "create _config", tree_oid, parents)
 
         if not no_push:
             print("Pushing change to origin:")
             cmd(["git", "push", "origin", "_config"], work_dir=self.repo_path, allow_nonzero=True)
 
-
```

### Comparing `gitcoll-0.0.18/src/gcln2/main.py` & `gitcoll-0.0.19/src/gcln2/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,28 +18,31 @@
 import concurrent.futures
 
 #non-std packages (requirement.txt)
 import yaml
 import gitlab   # pip3 install python-gitlab
 import pygit2   # pip3 install pygit2
 
+
 #local modules
 try:
     from gcln2 import db
     from gcln2 import schema
     from gcln2 import helpers
     from gcln2 import exceptions
     from gcln2 import yaml_loader
+    from gcln2 import sync
     from . import __version__
 except:
     import db
     import schema
     import helpers
     import exceptions
     import yaml_loader
+    import sync
     from __init__ import __version__
 
 
 if os.name == "nt":
     import win32file
 
 
@@ -70,16 +73,19 @@
         self.cfg = schema.MainConfig(**cfg_tmp)
 
 
 ############
 
 class ServerConnector:
     def __init__(self, args, mc: MainConfig):
-        self.gl: gitlab.Gitlab = gitlab.Gitlab(mc.cfg.general.server.api_url, private_token=mc.cfg.general.server.api_key)
-
+        self.gl: gitlab.Gitlab = gitlab.Gitlab(
+            mc.cfg.general.server.api_url,
+            private_token=mc.cfg.general.server.api_key,
+            keep_base_url=True,  # important as it might be via ssh tunnel or similar
+        )
 
 #################
 
 class UpdateContext:
     """Class that collects data needed for the various functions that update information from the server"""
     def __init__(self, args, sc: "ServerConnector" = None, cache: db.Cache= None):
         self.mc = MainConfig()
@@ -117,15 +123,20 @@
             if " => " in vp:
                 a, b = vp.split()
             else:
                 a = vp
                 b = ""
             self.re_valid_paths.append((a, b))
 
+
     def update_cache_from_server(self):
+
+        #####
+        # TODO: use db.Cache.update_cache_from_server instead
+
         SINCE = helpers.timestamp2isotime(self.cache.timestamp)
         with concurrent.futures.ThreadPoolExecutor(max_workers=5) as executor:
             futures = []
             #for gl_proj in self.sc.gl.projects.list(iterator=True, last_repository_updated_at=SINCE):    # note that iterator=True and as_list=False has the same meaning, different versions of the connector
             for gl_proj in self.sc.gl.projects.list(iterator=True, last_activity_after=SINCE):    # note that iterator=True and as_list=False has the same meaning, different versions of the connector
                 futures.append(executor.submit(db.Project.from_gl, gl_proj, self))
                 print("Got %d projects " % len(futures), end="\r")
@@ -930,14 +941,15 @@
 
     do_git_config(args.root, config, do_print=True)
 
     print("\nDone")
 
 
 
+
 def main(in_args):
     time_start = time.time()
 
     if gitlab.__version__ < "3.14.0":
         print ("Warning: mainly tested with python-gitlab 3.14.0. Running with older version %s" % gitlab.__version__)
 
     parser = argparse.ArgumentParser(prog="gcln2", description="Git Collection 2 - tool to manage many repositories in gitlab")
@@ -961,23 +973,40 @@
 
     p_clean_ws = subparsers.add_parser("clean_ws", help="Remove all local workspaces that do not match server _if_ they've pushed everything and are clean")
     p_clean_ws.add_argument("--yes", action="store_true", help="actually remove the directories")
     p_clean_ws.set_defaults(func=main_clean_ws )
 
     p_set_uid = subparsers.add_parser("set_uid", help="set uid in repo, ie, create _config branch and yaml file in that")
     p_set_uid .add_argument("--uid", default="", help="use this as uid instead of random value")
-    p_set_uid .add_argument("--nopush", action="store_true", help="do not push the result to the server")
-    p_set_uid.set_defaults(func=main_set_uid )
+    p_set_uid.add_argument("--nopush", action="store_true", help="do not push the result to the server")
+    p_set_uid.set_defaults(func=main_set_uid)
 
     p_uid_clean_gitmodules = subparsers.add_parser("clean_gitmodules", help="rewrite .gitmodules with uid lookup etc")
     p_uid_clean_gitmodules.set_defaults(func=main_uid_clean_gitmodules)
 
     p_uid_clean_gitmodules = subparsers.add_parser("git_config", help="apply git config in all repos")
     p_uid_clean_gitmodules.set_defaults(func=main_git_config)
 
+    p_sync = subparsers.add_parser("sync", help="Sync gitlab servers")
+    p_sync.add_argument(
+        "controlfile", type=argparse.FileType("r"), help="defines how/what to sync"
+    )
+    p_sync.set_defaults(func=sync.main_sync)
+
+    p_local_copy = subparsers.add_parser(
+        "local_sync", help="Helper to locally sync a normal ws tree to sync tree"
+    )
+    p_local_copy.add_argument(
+        "cache_file", type=str, help="cache file for the normal gcln2 tree"
+    )
+    p_local_copy.add_argument(
+        "sync_ctrlfile", type=argparse.FileType("r"), help="sync ctrl file"
+    )
+    p_local_copy.set_defaults(func=sync.local_sync_copy)
+
     p_test1 = subparsers.add_parser("test1", help="Testing #1")
     p_test1.set_defaults(func=main_test1)
 
     args = parser.parse_args(in_args)
 
     num_lvl = getattr(logging, args.log)
     logging.basicConfig(level=num_lvl)
```

### Comparing `gitcoll-0.0.18/src/gcln2/schema.py` & `gitcoll-0.0.19/src/gcln2/schema.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.18/src/gitcoll.egg-info/PKG-INFO` & `gitcoll-0.0.19/src/gitcoll.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitcoll
-Version: 0.0.18
+Version: 0.0.19
 Summary: Git collection utilities
 Home-page: https://gitlab.com/jesrib/gitcoll
 Author: Jesper Ribbe
 Author-email: jesper@ribbe.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gitcoll-0.0.18/src/gitcoll.egg-info/SOURCES.txt` & `gitcoll-0.0.19/src/gitcoll.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/gcln/srv_connector.py
 src/gcln2/__init__.py
 src/gcln2/db.py
 src/gcln2/exceptions.py
 src/gcln2/helpers.py
 src/gcln2/main.py
 src/gcln2/schema.py
+src/gcln2/sync.py
 src/gcln2/yaml_loader.py
 src/gitcoll.egg-info/PKG-INFO
 src/gitcoll.egg-info/SOURCES.txt
 src/gitcoll.egg-info/dependency_links.txt
 src/gitcoll.egg-info/entry_points.txt
 src/gitcoll.egg-info/requires.txt
 src/gitcoll.egg-info/top_level.txt
```

