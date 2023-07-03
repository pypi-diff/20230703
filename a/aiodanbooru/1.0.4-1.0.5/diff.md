# Comparing `tmp/aiodanbooru-1.0.4.tar.gz` & `tmp/aiodanbooru-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodanbooru-1.0.4.tar", last modified: Thu Jun 29 21:22:21 2023, max compression
+gzip compressed data, was "aiodanbooru-1.0.5.tar", last modified: Mon Jul  3 15:19:36 2023, max compression
```

## Comparing `aiodanbooru-1.0.4.tar` & `aiodanbooru-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 21:22:21.260038 aiodanbooru-1.0.4/
--rw-rw-rw-   0        0        0     1087 2023-06-29 10:35:25.000000 aiodanbooru-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     3022 2023-06-29 21:22:21.259005 aiodanbooru-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2003 2023-06-29 11:13:08.000000 aiodanbooru-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 21:22:21.248487 aiodanbooru-1.0.4/aiodanbooru/
--rw-rw-rw-   0        0        0        0 2023-06-29 10:45:27.000000 aiodanbooru-1.0.4/aiodanbooru/__init__.py
--rw-rw-rw-   0        0        0     1778 2023-06-29 20:53:59.000000 aiodanbooru-1.0.4/aiodanbooru/api.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:22:21.257003 aiodanbooru-1.0.4/aiodanbooru/dispatcher/
--rw-rw-rw-   0        0        0        0 2023-06-29 21:07:02.000000 aiodanbooru-1.0.4/aiodanbooru/dispatcher/__init__.py
--rw-rw-rw-   0        0        0     3184 2023-06-29 21:13:02.000000 aiodanbooru-1.0.4/aiodanbooru/dispatcher/filters.py
--rw-rw-rw-   0        0        0     1017 2023-06-29 21:05:35.000000 aiodanbooru-1.0.4/aiodanbooru/dispatcher/handler.py
--rw-rw-rw-   0        0        0     1971 2023-06-29 21:19:41.000000 aiodanbooru-1.0.4/aiodanbooru/dispatcher.py
--rw-rw-rw-   0        0        0     3247 2023-06-29 21:18:06.000000 aiodanbooru-1.0.4/aiodanbooru/models.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:22:21.255003 aiodanbooru-1.0.4/aiodanbooru.egg-info/
--rw-rw-rw-   0        0        0     3022 2023-06-29 21:22:21.000000 aiodanbooru-1.0.4/aiodanbooru.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-06-29 21:22:21.000000 aiodanbooru-1.0.4/aiodanbooru.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 21:22:21.000000 aiodanbooru-1.0.4/aiodanbooru.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 21:22:21.000000 aiodanbooru-1.0.4/aiodanbooru.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-29 21:22:21.000000 aiodanbooru-1.0.4/aiodanbooru.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 21:22:21.260038 aiodanbooru-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1108 2023-06-29 21:22:02.000000 aiodanbooru-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:22:21.258003 aiodanbooru-1.0.4/tests/
--rw-rw-rw-   0        0        0     1466 2023-06-29 20:35:36.000000 aiodanbooru-1.0.4/tests/test_api.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:19:36.996037 aiodanbooru-1.0.5/
+-rw-rw-rw-   0        0        0     1087 2023-06-29 10:35:25.000000 aiodanbooru-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3022 2023-07-03 15:19:36.995037 aiodanbooru-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2003 2023-06-29 11:13:08.000000 aiodanbooru-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 15:19:36.986246 aiodanbooru-1.0.5/aiodanbooru/
+-rw-rw-rw-   0        0        0        0 2023-06-29 10:45:27.000000 aiodanbooru-1.0.5/aiodanbooru/__init__.py
+-rw-rw-rw-   0        0        0     1668 2023-07-03 15:18:05.000000 aiodanbooru-1.0.5/aiodanbooru/api.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:19:36.993030 aiodanbooru-1.0.5/aiodanbooru/base/
+-rw-rw-rw-   0        0        0        0 2023-06-29 21:07:02.000000 aiodanbooru-1.0.5/aiodanbooru/base/__init__.py
+-rw-rw-rw-   0        0        0     3184 2023-06-29 21:13:02.000000 aiodanbooru-1.0.5/aiodanbooru/base/filters.py
+-rw-rw-rw-   0        0        0     1011 2023-07-03 15:15:24.000000 aiodanbooru-1.0.5/aiodanbooru/base/handler.py
+-rw-rw-rw-   0        0        0     1953 2023-07-03 15:15:24.000000 aiodanbooru-1.0.5/aiodanbooru/dispatcher.py
+-rw-rw-rw-   0        0        0     3237 2023-06-29 21:25:14.000000 aiodanbooru-1.0.5/aiodanbooru/models.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:19:36.990409 aiodanbooru-1.0.5/aiodanbooru.egg-info/
+-rw-rw-rw-   0        0        0     3022 2023-07-03 15:19:36.000000 aiodanbooru-1.0.5/aiodanbooru.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-03 15:19:36.000000 aiodanbooru-1.0.5/aiodanbooru.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 15:19:36.000000 aiodanbooru-1.0.5/aiodanbooru.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-03 15:19:36.000000 aiodanbooru-1.0.5/aiodanbooru.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-03 15:19:36.000000 aiodanbooru-1.0.5/aiodanbooru.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 15:19:36.996037 aiodanbooru-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2023-07-03 15:16:03.000000 aiodanbooru-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:19:36.994036 aiodanbooru-1.0.5/tests/
+-rw-rw-rw-   0        0        0     1466 2023-06-29 20:35:36.000000 aiodanbooru-1.0.5/tests/test_api.py
```

### Comparing `aiodanbooru-1.0.4/LICENSE` & `aiodanbooru-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.4/PKG-INFO` & `aiodanbooru-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodanbooru
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python library for interacting with the Danbooru API
 Author: lrdcxdes
 Author-email: lordgrief176@email.com
 License: MIT
 Project-URL: Source, https://github.com/lrdcxdes/aiodanbooru
 Project-URL: Bug Reports, https://github.com/lrdcxdes/aiodanbooru/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiodanbooru-1.0.4/README.md` & `aiodanbooru-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.4/aiodanbooru/api.py` & `aiodanbooru-1.0.5/aiodanbooru/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 from typing import List
 
 import aiohttp
 
 from aiodanbooru.models import DanbooruPost
 
 
@@ -33,18 +32,16 @@
             endpoint = "/posts.json"
             params = {}
             if tags is not None:
                 params["tags"] = " ".join(tags)
             if limit is not None:
                 params["limit"] = str(limit)
             response = await self._get(session, endpoint, params)
-            posts = [
-                DanbooruPost(**post, loop=asyncio.get_event_loop()) for post in response
-            ]
+            posts = [DanbooruPost(**post) for post in response]
             return posts
 
     async def get_random_post(self) -> DanbooruPost:
         async with aiohttp.ClientSession() as session:
             endpoint = "/posts/random.json"
             response = await self._get(session, endpoint)
-            post = DanbooruPost(**response, loop=asyncio.get_event_loop())
+            post = DanbooruPost(**response)
             return post
```

### Comparing `aiodanbooru-1.0.4/aiodanbooru/dispatcher/filters.py` & `aiodanbooru-1.0.5/aiodanbooru/base/filters.py`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.4/aiodanbooru/dispatcher/handler.py` & `aiodanbooru-1.0.5/aiodanbooru/base/handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 from typing import Callable, Union, List
 
-from aiodanbooru.dispatcher.filters import Filter
+from aiodanbooru.base.filters import Filter
 from aiodanbooru.models import DanbooruPost
 
 
 class Handler(object):
     def __init__(self, func, filters: Union[List[Filter], Filter] = None):
         self.func: Callable = func
         self.filters: Union[List[Filter], Filter] = filters
```

### Comparing `aiodanbooru-1.0.4/aiodanbooru/dispatcher.py` & `aiodanbooru-1.0.5/aiodanbooru/dispatcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 from typing import List, Union
 
 from aiodanbooru.api import DanbooruPost, DanbooruAPI
-from aiodanbooru.dispatcher.filters import Filter
-from aiodanbooru.dispatcher.handler import Handler
+from aiodanbooru.base.filters import Filter
+from aiodanbooru.base.handler import Handler
 
 
 class Dispatcher:
     def __init__(self):
         self.queue = asyncio.Queue()
         self._handlers: List[Handler] = []
         self.api = DanbooruAPI()
@@ -47,15 +47,15 @@
         loop = asyncio.get_event_loop()
         loop.create_task(self.watch_posts())
         loop.create_task(self.handle_events())
         loop.run_forever()
 
 
 if __name__ == "__main__":
-    from aiodanbooru.dispatcher import filters
+    from aiodanbooru.base import filters
 
     dispatcher = Dispatcher()
 
     @dispatcher.new_post(filters.all)
     async def handle_new_post(post_id):
         print(f"New post with ID {post_id} has appeared on the site!")
```

### Comparing `aiodanbooru-1.0.4/aiodanbooru/models.py` & `aiodanbooru-1.0.5/aiodanbooru/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import asyncio
-from typing import Optional
+from typing import Optional, List
 
 import aiohttp
 from pydantic import BaseModel, Field, HttpUrl, validator
 
 
 class DanbooruPost(BaseModel):
     id: int
@@ -62,15 +61,15 @@
         )
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as response:
                 response.raise_for_status()
                 return await response.read()
 
     @property
-    def tags(self) -> list[str]:
+    def tags(self) -> List[str]:
         return self.tag_string.split()
 
     @property
     def link(self):
         return f"https://danbooru.donmai.us/posts/{self.id}"
 
     @property
```

### Comparing `aiodanbooru-1.0.4/aiodanbooru.egg-info/PKG-INFO` & `aiodanbooru-1.0.5/aiodanbooru.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodanbooru
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python library for interacting with the Danbooru API
 Author: lrdcxdes
 Author-email: lordgrief176@email.com
 License: MIT
 Project-URL: Source, https://github.com/lrdcxdes/aiodanbooru
 Project-URL: Bug Reports, https://github.com/lrdcxdes/aiodanbooru/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiodanbooru-1.0.4/setup.py` & `aiodanbooru-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aiodanbooru",
-    version="1.0.4",
+    version="1.0.5",
     description="A Python library for interacting with the Danbooru API",
     author="lrdcxdes",
     author_email="lordgrief176@email.com",
     packages=find_packages(exclude=["tests"]),
     install_requires=[
         "aiohttp",
         "pydantic",
```

### Comparing `aiodanbooru-1.0.4/tests/test_api.py` & `aiodanbooru-1.0.5/tests/test_api.py`

 * *Files identical despite different names*

