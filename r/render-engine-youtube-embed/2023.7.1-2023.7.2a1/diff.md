# Comparing `tmp/render_engine_youtube_embed-2023.7.1.tar.gz` & `tmp/render_engine_youtube_embed-2023.7.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine_youtube_embed-2023.7.1.tar", last modified: Sun Jul  2 22:10:30 2023, max compression
+gzip compressed data, was "render_engine_youtube_embed-2023.7.2a1.tar", last modified: Sun Jul  2 23:28:50 2023, max compression
```

## Comparing `render_engine_youtube_embed-2023.7.1.tar` & `render_engine_youtube_embed-2023.7.2a1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:10:30.262642 render_engine_youtube_embed-2023.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:10:30.262642 render_engine_youtube_embed-2023.7.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-02 22:10:11.000000 render_engine_youtube_embed-2023.7.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:10:30.262642 render_engine_youtube_embed-2023.7.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-02 22:10:11.000000 render_engine_youtube_embed-2023.7.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:10:30.262642 render_engine_youtube_embed-2023.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-02 22:10:11.000000 render_engine_youtube_embed-2023.7.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-02 22:10:11.000000 render_engine_youtube_embed-2023.7.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-02 22:10:11.000000 render_engine_youtube_embed-2023.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-02 22:10:11.000000 render_engine_youtube_embed-2023.7.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-02 22:10:11.000000 render_engine_youtube_embed-2023.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-02 22:10:30.262642 render_engine_youtube_embed-2023.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-02 22:10:11.000000 render_engine_youtube_embed-2023.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-02 22:10:11.000000 render_engine_youtube_embed-2023.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-02 22:10:11.000000 render_engine_youtube_embed-2023.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 22:10:30.262642 render_engine_youtube_embed-2023.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:10:30.258643 render_engine_youtube_embed-2023.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:10:30.262642 render_engine_youtube_embed-2023.7.1/src/render_engine_youtube_embed/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-02 22:10:11.000000 render_engine_youtube_embed-2023.7.1/src/render_engine_youtube_embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-02 22:10:11.000000 render_engine_youtube_embed-2023.7.1/src/render_engine_youtube_embed/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-02 22:10:11.000000 render_engine_youtube_embed-2023.7.1/src/render_engine_youtube_embed/youtube_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:10:30.262642 render_engine_youtube_embed-2023.7.1/src/render_engine_youtube_embed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-02 22:10:30.000000 render_engine_youtube_embed-2023.7.1/src/render_engine_youtube_embed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-02 22:10:30.000000 render_engine_youtube_embed-2023.7.1/src/render_engine_youtube_embed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:10:30.000000 render_engine_youtube_embed-2023.7.1/src/render_engine_youtube_embed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-02 22:10:30.000000 render_engine_youtube_embed-2023.7.1/src/render_engine_youtube_embed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-02 22:10:30.000000 render_engine_youtube_embed-2023.7.1/src/render_engine_youtube_embed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:10:30.262642 render_engine_youtube_embed-2023.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-02 22:10:11.000000 render_engine_youtube_embed-2023.7.1/tests/test_link_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:28:50.388292 render_engine_youtube_embed-2023.7.2a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:28:50.384292 render_engine_youtube_embed-2023.7.2a1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-02 23:28:33.000000 render_engine_youtube_embed-2023.7.2a1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:28:50.384292 render_engine_youtube_embed-2023.7.2a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-02 23:28:33.000000 render_engine_youtube_embed-2023.7.2a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:28:50.384292 render_engine_youtube_embed-2023.7.2a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-02 23:28:33.000000 render_engine_youtube_embed-2023.7.2a1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-02 23:28:33.000000 render_engine_youtube_embed-2023.7.2a1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-02 23:28:33.000000 render_engine_youtube_embed-2023.7.2a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-02 23:28:33.000000 render_engine_youtube_embed-2023.7.2a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-02 23:28:33.000000 render_engine_youtube_embed-2023.7.2a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-02 23:28:50.388292 render_engine_youtube_embed-2023.7.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-02 23:28:33.000000 render_engine_youtube_embed-2023.7.2a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-02 23:28:33.000000 render_engine_youtube_embed-2023.7.2a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-02 23:28:33.000000 render_engine_youtube_embed-2023.7.2a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 23:28:50.388292 render_engine_youtube_embed-2023.7.2a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:28:50.384292 render_engine_youtube_embed-2023.7.2a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:28:50.388292 render_engine_youtube_embed-2023.7.2a1/src/render_engine_youtube_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-02 23:28:33.000000 render_engine_youtube_embed-2023.7.2a1/src/render_engine_youtube_embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-02 23:28:33.000000 render_engine_youtube_embed-2023.7.2a1/src/render_engine_youtube_embed/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-02 23:28:33.000000 render_engine_youtube_embed-2023.7.2a1/src/render_engine_youtube_embed/youtube_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:28:50.388292 render_engine_youtube_embed-2023.7.2a1/src/render_engine_youtube_embed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-02 23:28:50.000000 render_engine_youtube_embed-2023.7.2a1/src/render_engine_youtube_embed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-02 23:28:50.000000 render_engine_youtube_embed-2023.7.2a1/src/render_engine_youtube_embed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 23:28:50.000000 render_engine_youtube_embed-2023.7.2a1/src/render_engine_youtube_embed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-02 23:28:50.000000 render_engine_youtube_embed-2023.7.2a1/src/render_engine_youtube_embed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-02 23:28:50.000000 render_engine_youtube_embed-2023.7.2a1/src/render_engine_youtube_embed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:28:50.388292 render_engine_youtube_embed-2023.7.2a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-02 23:28:33.000000 render_engine_youtube_embed-2023.7.2a1/tests/test_link_detect.py
```

### Comparing `render_engine_youtube_embed-2023.7.1/.devcontainer/devcontainer.json` & `render_engine_youtube_embed-2023.7.2a1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.7.1/.github/workflows/publish.yml` & `render_engine_youtube_embed-2023.7.2a1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.7.1/.gitignore` & `render_engine_youtube_embed-2023.7.2a1/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.7.1/CODE_OF_CONDUCT.md` & `render_engine_youtube_embed-2023.7.2a1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.7.1/LICENSE` & `render_engine_youtube_embed-2023.7.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.7.1/PKG-INFO` & `render_engine_youtube_embed-2023.7.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render_engine_youtube_embed
-Version: 2023.7.1
+Version: 2023.7.2a1
 Summary: A Render Engine Plugin for replacing Youtube Links with Embed Links
 Project-URL: homepage, https://github.com/kjaymiller/render-engine-youtube-link-embed
 Project-URL: repository, https://github.com/kjaymiller/render-engine-youtube-link-embed
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `render_engine_youtube_embed-2023.7.1/README.md` & `render_engine_youtube_embed-2023.7.2a1/README.md`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.7.1/pyproject.toml` & `render_engine_youtube_embed-2023.7.2a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.7.1/src/render_engine_youtube_embed/youtube_embed.py` & `render_engine_youtube_embed-2023.7.2a1/src/render_engine_youtube_embed/youtube_embed.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,19 +23,19 @@
         return url.path.split('/')[-1]
 
 
 
 
 def get_all_links(content: str) -> typing.Generator[str, None, None]:
     """get all youtube link types"""
-
-    youtube_links = r'^ *<p>https://www.youtube.com/watch\?v=[\w\d_]+</p> *$'
-    youtube_slash_links = r'^ *<p>https://www.youtube.com/watch\/[\w\d_]+</p> *$'
-    youtube_shortlinks = r'^ *<p>https://youtu.be/[\w\d_]+</p> *$'
-    youtube_shorts = r'^ *<p>https://www.youtube.com/shorts/[\w\d_]+</p> *$'
+    youtube_links = r'^[ \t]*<p>https://www.youtube.com/watch\?v=[\w\d_]+</p>\s*$'
+    youtube_slash_links = r'^[ \t]*<p>https://www.youtube.com/watch\/[\w\d_]+</p>\s*$'
+    youtube_shortlinks = r'^[ \t]*<p>https://youtu.be/[\w\d_]+</p>\s*$'
+    youtube_shorts = r'^[ \t]*<p>https://www.youtube.com/shorts/[\w\d_]*</p>\s*$'
+    
 
     links = [youtube_links, youtube_slash_links, youtube_shortlinks, youtube_shorts]
     link_groups = [re.findall(link_type, content, re.MULTILINE) for link_type in links]
 
     return itertools.chain(*link_groups)
 
 def replace_youtube_links_with_embeds(content: str) -> str:
```

### Comparing `render_engine_youtube_embed-2023.7.1/src/render_engine_youtube_embed.egg-info/PKG-INFO` & `render_engine_youtube_embed-2023.7.2a1/src/render_engine_youtube_embed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-engine-youtube-embed
-Version: 2023.7.1
+Version: 2023.7.2a1
 Summary: A Render Engine Plugin for replacing Youtube Links with Embed Links
 Project-URL: homepage, https://github.com/kjaymiller/render-engine-youtube-link-embed
 Project-URL: repository, https://github.com/kjaymiller/render-engine-youtube-link-embed
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `render_engine_youtube_embed-2023.7.1/src/render_engine_youtube_embed.egg-info/SOURCES.txt` & `render_engine_youtube_embed-2023.7.2a1/src/render_engine_youtube_embed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

