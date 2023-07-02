# Comparing `tmp/hatena_cli-0.1.0.tar.gz` & `tmp/hatena_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatena_cli-0.1.0.tar", max compression
+gzip compressed data, was "hatena_cli-1.0.1.tar", max compression
```

## Comparing `hatena_cli-0.1.0.tar` & `hatena_cli-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-07-01 20:56:32.132090 hatena_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0     2275 2023-07-02 16:07:34.372306 hatena_cli-0.1.0/README.md
--rw-r--r--   0        0        0      108 2023-07-01 13:28:34.940946 hatena_cli-0.1.0/hatena_cli/__init__.py
--rw-r--r--   0        0        0      167 2023-07-01 13:28:37.323237 hatena_cli-0.1.0/hatena_cli/__main__.py
--rw-r--r--   0        0        0     8202 2023-07-02 12:56:29.714242 hatena_cli-0.1.0/hatena_cli/api.py
--rw-r--r--   0        0        0     2854 2023-07-02 13:18:17.170727 hatena_cli-0.1.0/hatena_cli/auth.py
--rw-r--r--   0        0        0     1998 2023-07-02 13:21:12.391783 hatena_cli-0.1.0/hatena_cli/config.py
--rw-r--r--   0        0        0     4350 2023-07-02 16:12:49.614944 hatena_cli-0.1.0/hatena_cli/main.py
--rw-r--r--   0        0        0      560 2023-07-02 03:10:41.673116 hatena_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2884 1970-01-01 00:00:00.000000 hatena_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-01 20:56:32.132090 hatena_cli-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3604 2023-07-02 22:43:16.850360 hatena_cli-1.0.1/README.md
+-rw-r--r--   0        0        0      108 2023-07-02 22:50:23.571797 hatena_cli-1.0.1/hatena_cli/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-01 13:28:37.323237 hatena_cli-1.0.1/hatena_cli/__main__.py
+-rw-r--r--   0        0        0     7654 2023-07-02 22:48:02.229384 hatena_cli-1.0.1/hatena_cli/api.py
+-rw-r--r--   0        0        0     2843 2023-07-02 22:02:29.804307 hatena_cli-1.0.1/hatena_cli/auth.py
+-rw-r--r--   0        0        0      606 2023-07-02 21:48:41.197507 hatena_cli-1.0.1/hatena_cli/cli.py
+-rw-r--r--   0        0        0     2017 2023-07-02 21:45:39.576527 hatena_cli-1.0.1/hatena_cli/config.py
+-rw-r--r--   0        0        0     4350 2023-07-02 21:41:54.369502 hatena_cli-1.0.1/hatena_cli/main.py
+-rw-r--r--   0        0        0      576 2023-07-02 22:50:12.264754 hatena_cli-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4250 1970-01-01 00:00:00.000000 hatena_cli-1.0.1/PKG-INFO
```

### Comparing `hatena_cli-0.1.0/LICENSE` & `hatena_cli-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hatena_cli-0.1.0/hatena_cli/api.py` & `hatena_cli-1.0.1/hatena_cli/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,65 +3,42 @@
 import re
 import requests
 from urllib import parse
 from pathlib import Path
 from requests_oauthlib import OAuth1
 from bs4 import BeautifulSoup
 from rich import print
-from rich.progress import (
-    Progress,
-    SpinnerColumn,
-    TextColumn,
-    BarColumn,
-    TaskProgressColumn,
-    TimeRemainingColumn,
-)
+
 import typer
 
+from .cli import ProgressBar, Spinner
+from .auth import get_auth
 from .config import get_config
 
 
-_HATENA_BLOG_URL = f"https://blog.hatena.ne.jp/"
+_HATENA_BLOG_URL = f"https://blog.hatena.ne.jp"
 _HATENA_FOTOLIFE_POST_URL = "https://f.hatena.ne.jp/atom/post"
 _HATENA_FOTOLIFE_EDIT_URL = "https://f.hatena.ne.jp/atom/edit"
 
 
-class Spinner(Progress):
-    def __init__(self):
-        super().__init__(
-            SpinnerColumn(),
-            TextColumn("[progress.description]{task.description}"),
-        )
-
-
-class ProgressBar(Progress):
-    def __init__(self):
-        super().__init__(
-            TextColumn("[progress.description]{task.description}"),
-            BarColumn(),
-            TaskProgressColumn(),
-            TimeRemainingColumn(elapsed_when_finished=True),
-        )
-
-
 def _convert(blog_path: Path = None):
     with Spinner() as progress:
         progress.add_task("Converting Markdown to HTML...")
 
         pandoc_path = get_config("path:pandoc")
-        template_path = get_config("path:tempalte")
+        template_path = get_config("path:template")
         os.system(
             f"{pandoc_path} --quiet --standalone --template '{template_path}' \
-                    --output '{blog_path.with_suffix('.html')}' '{blog_path}'"
+                            --output '{blog_path.with_suffix('.html')}' '{blog_path}'"
         )
 
 
 def upload_entry(blog_title: str, blog_path: Path, with_images: bool, publish: bool):
     _convert(blog_path)
-    auth = auth.get()
+    auth = get_auth()
     if with_images:
         _upload_images(blog_title, blog_path, auth)
     _upload_html(blog_title, blog_path, publish, auth)
 
 
 def _upload_images(blog_title: str, blog_path: Path, auth: OAuth1):
     with ProgressBar() as progress:
@@ -70,23 +47,25 @@
         with open(blog_path.with_suffix(".html"), mode="r") as file:
             content = file.read()
 
         total = len(re.findall(image_pattern, content))
         task = progress.add_task("Uploading images...", total=total)
 
         def callback(match: re.Match):
-            progress.advance(task, 1)
             image_path = parse.unquote(match.group(1))
             image_url = _upload_image(blog_title, image_path, auth)
+            progress.advance(task, 1)
             return image_replace.replace(r"\1", image_url)
 
-        re.sub(image_pattern, callback, content)
+        content = re.sub(image_pattern, callback, content)
+        with open(blog_path.with_suffix(".html"), mode="w") as file:
+            file.write(content)
 
 
-def _upload_image(blog_title: str, image_path: Path, auth: OAuth1) -> Path:
+def _upload_image(blog_title: str, image_path: Path, auth: OAuth1) -> str:
     with open(image_path, mode="rb") as file:
         content = file.read()
         content = base64.b64encode(content).decode()
 
     # Maximum length for <dc:subject /> is 24
     res = requests.post(
         _HATENA_FOTOLIFE_POST_URL,
@@ -104,110 +83,109 @@
 
     if res.status_code != 201:
         print("[red]Error while uploading image.")
         raise typer.Abort()
 
     xml = BeautifulSoup(res.text, features="xml")
     url = xml.find("entry").find("hatena:imageurl").text
-    return Path(url)
+    return url
 
 
 def _upload_html(blog_title: str, blog_path: Path, publish: bool, auth: OAuth1):
     with Spinner() as progress:
         progress.add_task("Uploading HTML...")
 
-        with open(blog_path.with_suffix("html"), mode="r") as file:
+        with open(blog_path.with_suffix(".html"), mode="r") as file:
             content = file.read()
 
         username = get_config("blog:username")
         domain = get_config("blog:domain")
         res = requests.post(
             f"{_HATENA_BLOG_URL}/{username}/{domain}/atom/entry",
             auth=auth,
             timeout=None,
             headers={"Content-Type": "application/xml; charset=utf-8"},
             data=f"""\
-    <?xml version="1.0" encoding="utf-8"?>
-    <entry xmlns="http://www.w3.org/2005/Atom" xmlns:app="http://www.w3.org/2007/app">
-        <title>{blog_title}</title>
-        <author><name>name</name></author>
-        <content type="text/html"><![CDATA[{content}]]></content>
-        <app:control><app:draft>{'no' if publish else 'yes'}</app:draft></app:control>
-    </entry>""".encode(
+<?xml version="1.0" encoding="utf-8"?>
+<entry xmlns="http://www.w3.org/2005/Atom" xmlns:app="http://www.w3.org/2007/app">
+    <title>{blog_title}</title>
+    <author><name>name</name></author>
+    <content type="text/html"><![CDATA[{content}]]></content>
+    <app:control><app:draft>{'no' if publish else 'yes'}</app:draft></app:control>
+</entry>""".encode(
                 "utf-8"
             ),
         )
 
         if res.status_code != 201:
             print("[red]Error while uploading HTML.")
             raise typer.Abort()
 
 
 def update_entry(
     blog_id: int, blog_title: str, blog_path: Path, with_images: bool, publish: bool
 ):
     _convert(blog_path)
-    auth = auth.get()
+    auth = get_auth()
     if with_images:
         _update_images(blog_id, blog_title, blog_path, auth)
     _update_html(blog_id, blog_title, blog_path, publish, auth)
 
 
 def _update_images(blog_id: int, blog_title: str, blog_path: Path, auth: OAuth1):
-    with Spinner() as progress:
-        progress.add_task("Updating images...")
-        _delete_images(blog_id, auth)
-        _upload_images(blog_title, blog_path, auth)
+    _delete_images(blog_id, auth)
+    _upload_images(blog_title, blog_path, auth)
 
 
 def _update_html(
     blog_id: int, blog_title: str, blog_path: Path, publish: bool, auth: OAuth1
 ):
     with Spinner() as progress:
         progress.add_task("Updating HTML...")
 
-        with open(blog_path.with_suffix("html"), mode="r") as file:
+        with open(blog_path.with_suffix(".html"), mode="r") as file:
             content = file.read()
 
         username = get_config("blog:username")
         domain = get_config("blog:domain")
         res = requests.put(
             f"{_HATENA_BLOG_URL}/{username}/{domain}/atom/entry/{blog_id}",
             auth=auth,
             timeout=None,
             headers={"Content-Type": "application/xml; charset=utf-8"},
             data=f"""\
-    <?xml version="1.0" encoding="utf-8"?>
-    <entry xmlns="http://www.w3.org/2005/Atom" xmlns:app="http://www.w3.org/2007/app">
-        <title>{blog_title}</title>
-        <author><name>name</name></author>
-        <content type="text/html"><![CDATA[{content}]]></content>
-        <app:control><app:draft>{'no' if publish else 'yes'}</app:draft></app:control>
-    </entry>""".encode(
+<?xml version="1.0" encoding="utf-8"?>
+<entry xmlns="http://www.w3.org/2005/Atom" xmlns:app="http://www.w3.org/2007/app">
+    <title>{blog_title}</title>
+    <author><name>name</name></author>
+    <content type="text/html"><![CDATA[{content}]]></content>
+    <app:control><app:draft>{'no' if publish else 'yes'}</app:draft></app:control>
+</entry>""".encode(
                 "utf-8"
             ),
         )
+
         if res.status_code != 200:
             print("[red]Error while updating HTML.")
             raise typer.Abort()
 
 
 def delete_entry(blog_id: int, with_images: bool):
-    auth = auth.get()
+    auth = get_auth()
     if with_images:
         _delete_images(blog_id, auth)
     _delete_html(blog_id, auth)
 
 
 def _delete_images(blog_id: int, auth: OAuth1):
     with ProgressBar() as progress:
         username = get_config("blog:username")
         domain = get_config("blog:domain")
         res = requests.get(
-            f"{_HATENA_BLOG_URL}/{username}/{domain}/{blog_id}",
+            f"{_HATENA_BLOG_URL}/{username}/{domain}/atom/entry/{blog_id}",
             auth=auth,
             timeout=None,
         )
 
         if res.status_code != 200:
             print("[red]Error while downloading HTML.")
             raise typer.Abort()
@@ -217,35 +195,35 @@
         content = parse.unquote(content)
 
         image_pattern = get_config("image:pattern")
         total = len(re.findall(image_pattern, content))
         task = progress.add_task("Deleting images...", total=total)
 
         def callback(match: re.Match):
-            progress.advance(task, 1)
             image_path = parse.unquote(match.group(1))
             image_id = os.path.splitext(os.path.basename(image_path))[0]
             res = requests.delete(
                 f"{_HATENA_FOTOLIFE_EDIT_URL}/{image_id}", auth=auth, timeout=None
             )
             if res.status_code != 200:
                 print("[red]Error while deleting image.")
                 raise typer.Abort()
+            progress.advance(task, 1)
 
         re.sub(image_pattern, callback, content)
 
 
 def _delete_html(blog_id: int, auth: OAuth1):
     with Spinner() as progress:
         progress.add_task("Deleting HTML...")
 
         username = get_config("blog:username")
         domain = get_config("blog:domain")
         res = requests.delete(
-            f"{_HATENA_BLOG_URL}/{username}/{domain}/{blog_id}",
+            f"{_HATENA_BLOG_URL}/{username}/{domain}/atom/entry/{blog_id}",
             auth=auth,
             timeout=None,
         )
 
         if res.status_code != 200:
             print("[red]Error while deleting HTML.")
             raise typer.Abort()
```

### Comparing `hatena_cli-0.1.0/hatena_cli/auth.py` & `hatena_cli-1.0.1/hatena_cli/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Tuple
 from urllib import parse
 from datetime import datetime, timedelta
 from requests_oauthlib import OAuth1
 import requests
 import typer
 
-from hatena_cli.api import Spinner
-
+from .cli import Spinner
 from .config import get_config, set_config
 
 
 _HATENA_SCOPES = ["read_public", "write_public", "read_private", "write_private"]
 _HATENA_INITIATE_URL = "https://www.hatena.com/oauth/initiate"
 _HATENA_AUTHORIZE_URL = "https://www.hatena.ne.jp/oauth/authorize"
 _HATENA_ACCESS_TOKEN_URL = "https://www.hatena.com/oauth/token"
@@ -29,15 +28,15 @@
 def check_auth():
     access_token = get_config("auth:access_token")
     access_secret = get_config("auth:access_secret")
     expires = get_config("auth:expires")
     api_key = get_config("auth:api_key")
     api_secret = get_config("auth:api_secret")
 
-    if access_token != "" or access_secret != "" or datetime.now() >= expires:
+    if access_token == "" or access_secret == "" or datetime.now() >= expires:
         access_token, access_secret = _get_access_token(api_key, api_secret)
         expires = datetime.now() + timedelta(days=60)
 
     set_config("auth:access_token", access_token)
     set_config("auth:access_secret", access_secret)
     set_config("auth:expires", expires)
```

### Comparing `hatena_cli-0.1.0/hatena_cli/config.py` & `hatena_cli-1.0.1/hatena_cli/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     if not _CONFIG_PATH.exists():
         with open(_CONFIG_PATH, "w") as file:
             toml.dump(_DEFAULT_CONFIG.as_dict(), file)
     if not _TEMPLATE_PATH.exists():
         with open(_TEMPLATE_PATH, "w") as file:
             file.write(_DEFAULT_TEMPLATE)
 
+    global _config
     if _config is None:
         _config = _Config(toml.load(_CONFIG_PATH))
 
 
 def iter_config() -> any:
     check_config()
```

### Comparing `hatena_cli-0.1.0/hatena_cli/main.py` & `hatena_cli-1.0.1/hatena_cli/main.py`

 * *Files identical despite different names*

### Comparing `hatena_cli-0.1.0/pyproject.toml` & `hatena_cli-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hatena-cli"
-version = "0.1.0"
+version = "1.0.1"
 description = ""
 authors = ["Taichi Maeda <taichi.maeda.up@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hatena_cli"}]
 
 
 [tool.poetry.scripts]
@@ -16,12 +16,13 @@
 typer = {extras = ["all"], version = "^0.9.0"}
 requests = "^2.31.0"
 requests-oauthlib = "^1.3.1"
 beautifulsoup4 = "^4.12.2"
 typing-extensions = "^4.7.0"
 toml = "^0.10.2"
 flatdict = "^4.0.1"
+lxml = "^4.9.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

