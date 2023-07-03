# Comparing `tmp/wallpaperscraft-1.0.1.tar.gz` & `tmp/wallpaperscraft-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wallpaperscraft-1.0.1.tar", last modified: Mon Jul  3 11:30:31 2023, max compression
+gzip compressed data, was "wallpaperscraft-1.0.2.tar", last modified: Mon Jul  3 19:47:41 2023, max compression
```

## Comparing `wallpaperscraft-1.0.1.tar` & `wallpaperscraft-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 11:30:31.522201 wallpaperscraft-1.0.1/
--rw-rw-rw-   0        0        0    11558 2023-06-13 14:39:33.000000 wallpaperscraft-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3018 2023-07-03 11:30:31.522201 wallpaperscraft-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2279 2023-06-16 14:04:39.000000 wallpaperscraft-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 11:30:31.523200 wallpaperscraft-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-06-16 14:06:58.000000 wallpaperscraft-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 11:30:31.487054 wallpaperscraft-1.0.1/wallpaperscraft/
--rw-rw-rw-   0        0        0      164 2023-07-03 11:04:45.000000 wallpaperscraft-1.0.1/wallpaperscraft/__init__.py
--rw-rw-rw-   0        0        0     3886 2023-07-03 11:04:14.000000 wallpaperscraft-1.0.1/wallpaperscraft/api.py
--rw-rw-rw-   0        0        0     3227 2023-07-03 11:04:31.000000 wallpaperscraft-1.0.1/wallpaperscraft/asyncapi.py
--rw-rw-rw-   0        0        0     2962 2023-07-03 11:27:19.000000 wallpaperscraft-1.0.1/wallpaperscraft/types.py
-drwxrwxrwx   0        0        0        0 2023-07-03 11:30:31.520202 wallpaperscraft-1.0.1/wallpaperscraft.egg-info/
--rw-rw-rw-   0        0        0     3018 2023-07-03 11:30:31.000000 wallpaperscraft-1.0.1/wallpaperscraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-07-03 11:30:31.000000 wallpaperscraft-1.0.1/wallpaperscraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 11:30:31.000000 wallpaperscraft-1.0.1/wallpaperscraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-03 11:30:31.000000 wallpaperscraft-1.0.1/wallpaperscraft.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 19:47:41.300566 wallpaperscraft-1.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-06-13 14:39:33.000000 wallpaperscraft-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2944 2023-07-03 19:47:41.299059 wallpaperscraft-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2279 2023-06-16 14:04:39.000000 wallpaperscraft-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 19:47:41.300566 wallpaperscraft-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1217 2023-07-03 11:30:58.000000 wallpaperscraft-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 19:47:41.259798 wallpaperscraft-1.0.2/wallpaperscraft/
+-rw-rw-rw-   0        0        0      164 2023-07-03 19:44:42.000000 wallpaperscraft-1.0.2/wallpaperscraft/__init__.py
+-rw-rw-rw-   0        0        0     4058 2023-07-03 19:44:29.000000 wallpaperscraft-1.0.2/wallpaperscraft/api.py
+-rw-rw-rw-   0        0        0     3227 2023-07-03 11:04:31.000000 wallpaperscraft-1.0.2/wallpaperscraft/asyncapi.py
+-rw-rw-rw-   0        0        0     2980 2023-07-03 19:42:58.000000 wallpaperscraft-1.0.2/wallpaperscraft/types.py
+drwxrwxrwx   0        0        0        0 2023-07-03 19:47:41.298059 wallpaperscraft-1.0.2/wallpaperscraft.egg-info/
+-rw-rw-rw-   0        0        0     2944 2023-07-03 19:47:41.000000 wallpaperscraft-1.0.2/wallpaperscraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-07-03 19:47:41.000000 wallpaperscraft-1.0.2/wallpaperscraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 19:47:41.000000 wallpaperscraft-1.0.2/wallpaperscraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-03 19:47:41.000000 wallpaperscraft-1.0.2/wallpaperscraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-03 19:47:41.000000 wallpaperscraft-1.0.2/wallpaperscraft.egg-info/top_level.txt
```

### Comparing `wallpaperscraft-1.0.1/LICENSE` & `wallpaperscraft-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wallpaperscraft-1.0.1/PKG-INFO` & `wallpaperscraft-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: wallpaperscraft
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unofficial API WallpapersCraft (wallpaperscraft.com)
 Home-page: https://github.com/Den4ikSuperOstryyPer4ik/WallpapersCraftAPI/
 Download-URL: https://github.com/Den4ikSuperOstryyPer4ik/WallpapersCraftAPI//releases/latest
 Author: Den4ikSuperOstryyPer4ik
 License: Apache2.0
 Keywords: python3 wallpaperscraft wallpapers craft WallpapersCraftAPI
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Requires: bs4
-Requires: requests
-Requires: aiohttp
-Requires: pydantic
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WallpapersCraftAPI
 > Unofficial API WallpapersCraft (wallpaperscraft.com)
```

### Comparing `wallpaperscraft-1.0.1/README.md` & `wallpaperscraft-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wallpaperscraft-1.0.1/setup.py` & `wallpaperscraft-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     author="Den4ikSuperOstryyPer4ik",
     description="Unofficial API WallpapersCraft (wallpaperscraft.com)",
     long_description=get_readme(),
     long_description_content_type="text/markdown",
     url=github,
     packages=find_packages(),
     download_url=f"{github}/releases/latest",
-    requires=[
+    install_requires=[
         "bs4",
         "requests",
         "aiohttp",
         "pydantic",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.11",
```

### Comparing `wallpaperscraft-1.0.1/wallpaperscraft/api.py` & `wallpaperscraft-1.0.2/wallpaperscraft/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         responce = get(query, **kwargs)
         if not responce.raise_for_status():
             return BeautifulSoup(responce.text)
     
     def get_all_pictures_from_page(self, page: BeautifulSoup):
         return [
             Picture(
+                preview=pic.find("a", {"class": "wallpapers__link"}).find("span", {"class": "wallpapers__canvas"}).find("img", {"class": "wallpapers__image"}).get("src"),
                 link=self.WEBSITE + pic.find("a", {"class": "wallpapers__link"}).get("href"),
                 info=pic.find("a", {"class": "wallpapers__link"}).find_all("span", {"class": "wallpapers__info"})[1].text,
                 downloads=pic.find("a", {"class": "wallpapers__link"}).find_all("span", {"class": "wallpapers__info"})[0].find("span", {"class": "wallpapers__info-downloads"}).text,
                 rating=pic.find("a", {"class": "wallpapers__link"}).find_all("span", {"class": "wallpapers__info"})[0].find("span", {"class": "wallpapers__info-rating"}).text.strip(),
                 api_class=self
             )
             for pic in page.find_all("li", {"class": "wallpapers__item"})
```

### Comparing `wallpaperscraft-1.0.1/wallpaperscraft/asyncapi.py` & `wallpaperscraft-1.0.2/wallpaperscraft/asyncapi.py`

 * *Files identical despite different names*

### Comparing `wallpaperscraft-1.0.1/wallpaperscraft/types.py` & `wallpaperscraft-1.0.2/wallpaperscraft/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     "2560x1080",
     "3840x2400",
     "3840x2160",
 ]
 
 
 class Picture(BaseModel):
+    preview: str
     link: str
     info: str
     downloads: int
     rating: Optional[str] = None
     api_class: Any
 
     def download(self, resolution: str = "1024x768"):
```

### Comparing `wallpaperscraft-1.0.1/wallpaperscraft.egg-info/PKG-INFO` & `wallpaperscraft-1.0.2/wallpaperscraft.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: wallpaperscraft
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unofficial API WallpapersCraft (wallpaperscraft.com)
 Home-page: https://github.com/Den4ikSuperOstryyPer4ik/WallpapersCraftAPI/
 Download-URL: https://github.com/Den4ikSuperOstryyPer4ik/WallpapersCraftAPI//releases/latest
 Author: Den4ikSuperOstryyPer4ik
 License: Apache2.0
 Keywords: python3 wallpaperscraft wallpapers craft WallpapersCraftAPI
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Requires: bs4
-Requires: requests
-Requires: aiohttp
-Requires: pydantic
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WallpapersCraftAPI
 > Unofficial API WallpapersCraft (wallpaperscraft.com)
```

