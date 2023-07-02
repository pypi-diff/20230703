# Comparing `tmp/watchgha-1.0.0.tar.gz` & `tmp/watchgha-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nedbatchelder/watchgha/dist/.tmp-0i05rj4h/watchgha-1.0.0.tar", last modified: Sat Apr 15 13:01:55 2023, max compression
+gzip compressed data, was "/Users/nedbatchelder/watchgha/dist/.tmp-ie4eys2t/watchgha-2.0.0.tar", last modified: Sun Jul  2 23:16:07 2023, max compression
```

## Comparing `watchgha-1.0.0.tar` & `watchgha-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-15 13:01:55.000000 watchgha-1.0.0/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      515 2022-12-02 14:22:28.000000 watchgha-1.0.0/.editorconfig
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    10177 2022-12-02 14:18:16.000000 watchgha-1.0.0/LICENSE.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       68 2023-04-14 22:41:09.000000 watchgha-1.0.0/MANIFEST.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2477 2023-04-15 11:28:19.000000 watchgha-1.0.0/Makefile
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     7745 2023-04-15 13:01:55.000000 watchgha-1.0.0/PKG-INFO
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     6797 2023-04-15 11:30:39.000000 watchgha-1.0.0/README.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       84 2023-04-14 22:39:37.000000 watchgha-1.0.0/dev-requirements.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1390 2023-04-14 22:56:48.000000 watchgha-1.0.0/pyproject.toml
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       38 2023-04-15 13:01:55.000000 watchgha-1.0.0/setup.cfg
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-15 13:01:55.000000 watchgha-1.0.0/src/
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-15 13:01:55.000000 watchgha-1.0.0/src/watchgha/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       22 2023-04-15 11:30:28.000000 watchgha-1.0.0/src/watchgha/__init__.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      729 2023-03-16 17:18:38.000000 watchgha-1.0.0/src/watchgha/bucketer.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2571 2023-04-14 19:49:22.000000 watchgha-1.0.0/src/watchgha/utils.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     8279 2023-04-06 12:05:08.000000 watchgha-1.0.0/src/watchgha/watch_runs.py
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-04-15 13:01:55.000000 watchgha-1.0.0/src/watchgha.egg-info/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     7745 2023-04-15 13:01:55.000000 watchgha-1.0.0/src/watchgha.egg-info/PKG-INFO
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      410 2023-04-15 13:01:55.000000 watchgha-1.0.0/src/watchgha.egg-info/SOURCES.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)        1 2023-04-15 13:01:55.000000 watchgha-1.0.0/src/watchgha.egg-info/dependency_links.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       60 2023-04-15 13:01:55.000000 watchgha-1.0.0/src/watchgha.egg-info/entry_points.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       37 2023-04-15 13:01:55.000000 watchgha-1.0.0/src/watchgha.egg-info/requires.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)        9 2023-04-15 13:01:55.000000 watchgha-1.0.0/src/watchgha.egg-info/top_level.txt
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-02 23:16:07.000000 watchgha-2.0.0/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      515 2022-12-02 14:22:28.000000 watchgha-2.0.0/.editorconfig
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10177 2022-12-02 14:18:16.000000 watchgha-2.0.0/LICENSE.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       86 2023-07-02 23:07:34.000000 watchgha-2.0.0/MANIFEST.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2597 2023-07-01 16:34:52.000000 watchgha-2.0.0/Makefile
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10472 2023-07-02 23:16:07.000000 watchgha-2.0.0/PKG-INFO
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     9524 2023-07-02 23:09:11.000000 watchgha-2.0.0/README.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       91 2023-06-30 21:19:24.000000 watchgha-2.0.0/dev-requirements.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1405 2023-06-29 12:20:29.000000 watchgha-2.0.0/pyproject.toml
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       38 2023-07-02 23:16:07.000000 watchgha-2.0.0/setup.cfg
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       22 2023-07-02 23:10:57.000000 watchgha-2.0.0/src/watchgha/__init__.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      729 2023-03-16 17:18:38.000000 watchgha-2.0.0/src/watchgha/bucketer.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     6273 2023-07-02 20:54:10.000000 watchgha-2.0.0/src/watchgha/data_core.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3077 2023-07-02 20:03:45.000000 watchgha-2.0.0/src/watchgha/demo.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      404 2023-06-29 12:20:29.000000 watchgha-2.0.0/src/watchgha/git_help.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     3152 2023-06-30 21:19:24.000000 watchgha-2.0.0/src/watchgha/http_help.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1108 2023-06-30 21:19:24.000000 watchgha-2.0.0/src/watchgha/utils.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     4232 2023-07-02 23:12:28.000000 watchgha-2.0.0/src/watchgha/watch_runs.py
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha.egg-info/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10472 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha.egg-info/PKG-INFO
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      518 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha.egg-info/SOURCES.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)        1 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha.egg-info/dependency_links.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       60 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha.egg-info/entry_points.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       45 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha.egg-info/requires.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)        9 2023-07-02 23:16:07.000000 watchgha-2.0.0/src/watchgha.egg-info/top_level.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)   393385 2023-07-02 21:07:54.000000 watchgha-2.0.0/watch.gif
```

### Comparing `watchgha-1.0.0/.editorconfig` & `watchgha-2.0.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `watchgha-1.0.0/LICENSE.txt` & `watchgha-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `watchgha-1.0.0/Makefile` & `watchgha-2.0.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 help: 	## Display this help message.
 	@echo "Please use \`make <target>' where <target> is one of:"
 	@awk -F ':.*?## ' '/^[a-zA-Z]/ && NF==2 {printf "  %-20s %s\n", $$1, $$2}' $(MAKEFILE_LIST) | sort
 
 clean: 	## Remove stuff we don't need.
 	find . -name '__pycache__' -exec rm -rf {} +
 	rm -fr build/ dist/ src/*.egg-info
-	rm -f get_*.json
+	rm -f get_*.json get_index.txt
 
 tools:	## Install the development tools.
 	python -m pip install -r dev-requirements.txt
 
 dist: 	## Build the distributions.
 	python -m build --sdist --wheel
 	python -m twine check dist/*
@@ -23,14 +23,19 @@
 
 pypi:	## Upload the built distributions to PyPI.
 	python -m twine upload --verbose dist/*
 
 pipx:	## Install locally as a command
 	pipx install --force -e .
 
+.PHONY: cog_docs
+
+cog_docs:	## Run cog to get docs right
+	python -m cogapp -crP --verbosity=1 README.rst
+
 test_release: clean check_release dist test_pypi	## Do all the steps for a test release
 
 release: clean check_release dist pypi tag gh_release	## Do all the steps for a release
 
 check_release: _check_manifest _check_tree _check_readme _check_version	## Check that we are ready for a release
 	@echo "Release checks passed"
```

### Comparing `watchgha-1.0.0/pyproject.toml` & `watchgha-2.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "Programming Language :: Python :: 3.11",
 ]
 
 requires-python = ">= 3.7"
 
 dependencies = [
     "click",
+    "dulwich",
     "exceptiongroup",
     "httpx",
     "rich",
     "trio",
 ]
 
 dynamic = ["version"]
```

### Comparing `watchgha-1.0.0/src/watchgha/bucketer.py` & `watchgha-2.0.0/src/watchgha/bucketer.py`

 * *Files identical despite different names*

### Comparing `watchgha-1.0.0/src/watchgha/utils.py` & `watchgha-2.0.0/src/watchgha/http_help.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,94 +1,97 @@
-import datetime
+"""
+Helper for getting data from URLs.
+"""
+
 import itertools
 import mimetypes
 import os
-import time
 
 import httpx
+import trio
 
+from .utils import WatchGhaError
 
-class WatchGhaError(Exception):
-    pass
-
-
-def nice_time(dt):
-    dt = dt.astimezone()
-    now = datetime.datetime.now()
-    if dt.date() != now.date():
-        if dt.year != now.year:
-            fmt = "%Y-%m-%d %I:%M%p"
-        else:
-            fmt = "%m-%d %I:%M%p"
-    else:
-        fmt = "%I:%M%p"
-    return dt.strftime(fmt).lower()
-
-
-def to_datetime(isostr):
-    # 3.11 accepts Z, but older Pythons don't.
-    isostr = isostr.replace("Z", "+00:00")
-    return datetime.datetime.fromisoformat(isostr)
-
-
-class DictAttr:
-    def __init__(self, d):
-        self.d = d
-
-    def __getattr__(self, name):
-        return self.d[name]
 
+RETRY_STATUS_CODES = {502}
 
 class Http:
     """
     Helper for getting data from URLs.
 
     Uses the GITHUB_TOKEN environment variable (if set) as authentication.
 
-    Define SAVE_DATA=1 in the environment to save retrieved data in get_*.* files.
+    Define SAVE_DATA=1 in the environment to save retrieved data in get_*.*
+    files.
 
     """
 
-    # $set_env.py: SAVE_DATA - save all fetched data to get_* files.
-
-    RETRY_STATUS_CODES = {502}
-
     def __init__(self):
+        # $set_env.py: SAVE_DATA - save all fetched data to get_* files.
         self.save = bool(int(os.environ.get("SAVE_DATA", "0")))
         if self.save:
             with open("get_index.txt", "w") as index:
-                print("# URLs fetched:", file=index)
+                index.write("# URLs fetched:\n")
             self.count = itertools.count()
         self.headers = {}
         token = os.environ.get("GITHUB_TOKEN", "")
         if token:
             self.headers["Authorization"] = f"Bearer {token}"
 
     async def get_data(self, url):
         async with httpx.AsyncClient() as client:
-            for _ in range(3):
-                try:
+            resp = None
+            try:
+                for ntry in range(3):
                     resp = await client.get(
-                        url, headers=self.headers, timeout=30, follow_redirects=True
+                        url,
+                        headers=self.headers,
+                        timeout=30,
+                        follow_redirects=True,
                     )
-                except httpx.HTTPError as e:
-                    raise WatchGhaError(e)
-                if resp.status_code not in self.RETRY_STATUS_CODES:
-                    break
-            resp.raise_for_status()
+                    if resp.status_code not in RETRY_STATUS_CODES:
+                        break
+                    await trio.sleep(.05 * 2 ** ntry)
+                resp.raise_for_status()
+            except httpx.HTTPError as e:
+                # Some error messages have the URL, and some don't.  Add it in
+                # if it isn't there already.
+                if len(url) > 10 and url in str(e):
+                    msg = str(e)
+                else:
+                    msg = f"Couldn't get {url!r}: {e}"
+                if resp is not None:
+                    try:
+                        for label, text in resp.json().items():
+                            msg += f"\n{label}: {text}"
+                    except Exception:
+                        msg += f"\n{resp.text}"
+                raise WatchGhaError(msg) from e
             data = resp.text
             if self.save:
                 ext = extension_for_content(resp)
                 filename = f"get_{next(self.count):03d}{ext}"
-                with open("get_index.txt", "a") as index:
-                    print(f"{filename}: {url}", file=index)
-                with open(filename, "w") as out:
-                    out.write(data)
+                async with await trio.open_file("get_index.txt", "a") as index:
+                    await index.write(f"{filename}: {url}\n")
+                async with await trio.open_file(filename, "w") as out:
+                    await out.write(data)
             return data
 
 
 def extension_for_content(response):
     content_type = response.headers["content-type"].partition(";")[0].strip()
     return mimetypes.guess_extension(content_type)
 
 
-get_data = Http().get_data
+_get_data = Http().get_data
+
+
+async def get_data(*args, **kwargs):
+    """Run get_data three times, with retry."""
+    # I don't like that this has a retry loop and get_data above also does.
+    for ntry in range(3):
+        try:
+            return await _get_data(*args, **kwargs)
+        except Exception as exc:
+            exc_to_raise = exc
+            await trio.sleep(.05 * 2 ** ntry)
+    raise exc_to_raise
```

