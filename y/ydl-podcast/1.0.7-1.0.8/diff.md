# Comparing `tmp/ydl_podcast-1.0.7.tar.gz` & `tmp/ydl_podcast-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydl_podcast-1.0.7.tar", max compression
+gzip compressed data, was "ydl_podcast-1.0.8.tar", max compression
```

## Comparing `ydl_podcast-1.0.7.tar` & `ydl_podcast-1.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1102 2023-06-12 02:15:43.271076 ydl_podcast-1.0.7/LICENSE
--rw-r--r--   0        0        0     2748 2023-06-12 02:15:43.271076 ydl_podcast-1.0.7/README.md
--rw-r--r--   0        0        0      895 2023-06-13 13:18:24.930680 ydl_podcast-1.0.7/pyproject.toml
--rw-r--r--   0        0        0    12630 2023-06-13 13:17:25.297576 ydl_podcast-1.0.7/ydl_podcast/__init__.py
--rwxr-xr-x   0        0        0     1830 2023-06-12 02:15:43.271076 ydl_podcast-1.0.7/ydl_podcast/__main__.py
--rw-r--r--   0        0        0      982 2023-06-13 00:52:22.553108 ydl_podcast-1.0.7/ydl_podcast/template.py
--rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 ydl_podcast-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-07-03 20:16:08.783020 ydl_podcast-1.0.8/LICENSE
+-rw-r--r--   0        0        0     2830 2023-07-03 20:16:08.787020 ydl_podcast-1.0.8/README.md
+-rw-r--r--   0        0        0      895 2023-07-03 20:16:08.787020 ydl_podcast-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0    12989 2023-07-03 20:16:08.787020 ydl_podcast-1.0.8/ydl_podcast/__init__.py
+-rwxr-xr-x   0        0        0     1830 2023-07-03 20:16:08.787020 ydl_podcast-1.0.8/ydl_podcast/__main__.py
+-rw-r--r--   0        0        0      982 2023-07-03 20:16:08.787020 ydl_podcast-1.0.8/ydl_podcast/template.py
+-rw-r--r--   0        0        0     3918 1970-01-01 00:00:00.000000 ydl_podcast-1.0.8/PKG-INFO
```

### Comparing `ydl_podcast-1.0.7/LICENSE` & `ydl_podcast-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.7/README.md` & `ydl_podcast-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-![Pypi Version Shield](https://img.shields.io/pypi/v/ydl-podcast.svg?style=flat-square)
-![Pypi License Shield](https://img.shields.io/pypi/l/ydl-podcast.svg?style=flat-square)
+[![Pypi Version Shield](https://img.shields.io/pypi/v/ydl-podcast.svg?style=flat-square)](https://pypi.org/project/ydl-podcast/)
+[![Pypi License Shield](https://img.shields.io/pypi/l/ydl-podcast.svg?style=flat-square)](https://pypi.org/project/ydl-podcast/)
 
 # ydl-podcast
 
 A simple tool to generate Podcast-like RSS feeds from youtube (or other
 youtube-dl supported services) channels, using
 [`youtube-dl`](https://github.com/rg3/youtube-dl).
```

### Comparing `ydl_podcast-1.0.7/pyproject.toml` & `ydl_podcast-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ydl-podcast"
-version = "1.0.7"
+version = "1.0.8"
 description = "A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl"
 license = "MIT"
 authors = ["nbr23 <max@23.tf>"]
 homepage = "https://github.com/nbr23/ydl-podcast"
 repository = "https://github.com/nbr23/ydl-podcast"
 keywords = ["podcast", "youtube-dl"]
 readme = "README.md"
```

### Comparing `ydl_podcast-1.0.7/ydl_podcast/__init__.py` & `ydl_podcast-1.0.8/ydl_podcast/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,18 @@
                     ydl._out_files.error = io.StringIO()
                 else:
                     ydl._err_file = io.StringIO()
             ydl.download([url])
         except ydl_mod.utils.YoutubeDLError as e:
             if not quiet:
                 print(e)
-    return json.loads(output.getvalue().split("\n")[0])
+    md = output.getvalue().split("\n")[0]
+    if len(md) == 0:
+        return None
+    return json.loads(md)
 
 def process_options(ydl_mod, sub):
     options = {
         "outtmpl": os.path.join(
             sub["output_dir"], sub["name"], sub["filename_template"]
         ),
         "writeinfojson": True,
@@ -228,26 +231,34 @@
             pass
 
 
 def download(ydl_mod, sub):
     downloaded = []
     options = process_options(ydl_mod, sub)
     metadata = get_metadata(ydl_mod, sub["url"], options, sub["quiet"])
+
+    if metadata is None:
+        print("No metadata found for %s" % sub["name"])
+        return
     entries = metadata.get("entries", [])
 
     # Handle podcast icon
     get_podcast_icon(ydl_mod, sub, metadata)
 
     # Filter out older entries
     if sub["download_last"] is not None and not sub.get("initialize", False):
         entries = entries[: sub["download_last"]]
 
     # Go through entries and download them
     for i, md in enumerate(entries):
         entry = get_video_metadata(ydl_mod, md["url"], options, quiet=True)
+        if entry is None:
+            if not sub["quiet"]:
+                print("No metadata found for %s, skipping (likely due to the video upload date being out of range)" % md["url"])
+            continue
         mdfile_name = "%s.meta" % ".".join(entry["_filename"].split(".")[:-1])
         if not os.path.isfile(mdfile_name) and not entry.get("is_live", False):
             with ydl_mod.YoutubeDL(options) as ydl:
                 if sub["quiet"]:
                     ydl._screen_file = io.StringIO()
                     if ydl._out_files is not None:
                         ydl._out_files.out = io.StringIO()
```

### Comparing `ydl_podcast-1.0.7/ydl_podcast/__main__.py` & `ydl_podcast-1.0.8/ydl_podcast/__main__.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.7/ydl_podcast/template.py` & `ydl_podcast-1.0.8/ydl_podcast/template.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.7/PKG-INFO` & `ydl_podcast-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydl-podcast
-Version: 1.0.7
+Version: 1.0.8
 Summary: A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl
 Home-page: https://github.com/nbr23/ydl-podcast
 License: MIT
 Keywords: podcast,youtube-dl
 Author: nbr23
 Author-email: max@23.tf
 Requires-Python: >=3.7,<4.0
@@ -21,16 +21,16 @@
 Requires-Dist: MarkupSafe (>=2.1.1,<3.0.0)
 Requires-Dist: PyYAML (==6.0)
 Requires-Dist: youtube-dl (>=2021.12.17) ; extra == "youtube-dl"
 Requires-Dist: yt-dlp (>=2022.10.4) ; extra == "yt-dlp"
 Project-URL: Repository, https://github.com/nbr23/ydl-podcast
 Description-Content-Type: text/markdown
 
-![Pypi Version Shield](https://img.shields.io/pypi/v/ydl-podcast.svg?style=flat-square)
-![Pypi License Shield](https://img.shields.io/pypi/l/ydl-podcast.svg?style=flat-square)
+[![Pypi Version Shield](https://img.shields.io/pypi/v/ydl-podcast.svg?style=flat-square)](https://pypi.org/project/ydl-podcast/)
+[![Pypi License Shield](https://img.shields.io/pypi/l/ydl-podcast.svg?style=flat-square)](https://pypi.org/project/ydl-podcast/)
 
 # ydl-podcast
 
 A simple tool to generate Podcast-like RSS feeds from youtube (or other
 youtube-dl supported services) channels, using
 [`youtube-dl`](https://github.com/rg3/youtube-dl).
```

