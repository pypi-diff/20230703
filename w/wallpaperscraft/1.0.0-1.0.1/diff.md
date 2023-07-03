# Comparing `tmp/wallpaperscraft-1.0.0.tar.gz` & `tmp/wallpaperscraft-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wallpaperscraft-1.0.0.tar", last modified: Fri Jun 16 14:09:17 2023, max compression
+gzip compressed data, was "wallpaperscraft-1.0.1.tar", last modified: Mon Jul  3 11:30:31 2023, max compression
```

## Comparing `wallpaperscraft-1.0.0.tar` & `wallpaperscraft-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 14:09:17.353334 wallpaperscraft-1.0.0/
--rw-rw-rw-   0        0        0    11558 2023-06-13 14:39:33.000000 wallpaperscraft-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3018 2023-06-16 14:09:17.352333 wallpaperscraft-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2279 2023-06-16 14:04:39.000000 wallpaperscraft-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 14:09:17.353334 wallpaperscraft-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-06-16 14:06:58.000000 wallpaperscraft-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:09:17.327348 wallpaperscraft-1.0.0/wallpaperscraft/
--rw-rw-rw-   0        0        0      164 2023-06-16 13:19:42.000000 wallpaperscraft-1.0.0/wallpaperscraft/__init__.py
--rw-rw-rw-   0        0        0     3901 2023-06-16 13:10:11.000000 wallpaperscraft-1.0.0/wallpaperscraft/api.py
--rw-rw-rw-   0        0        0     3242 2023-06-16 13:13:11.000000 wallpaperscraft-1.0.0/wallpaperscraft/asyncapi.py
--rw-rw-rw-   0        0        0     2870 2023-06-16 12:51:57.000000 wallpaperscraft-1.0.0/wallpaperscraft/types.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:09:17.350334 wallpaperscraft-1.0.0/wallpaperscraft.egg-info/
--rw-rw-rw-   0        0        0     3018 2023-06-16 14:09:17.000000 wallpaperscraft-1.0.0/wallpaperscraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-06-16 14:09:17.000000 wallpaperscraft-1.0.0/wallpaperscraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 14:09:17.000000 wallpaperscraft-1.0.0/wallpaperscraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-16 14:09:17.000000 wallpaperscraft-1.0.0/wallpaperscraft.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 11:30:31.522201 wallpaperscraft-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2023-06-13 14:39:33.000000 wallpaperscraft-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3018 2023-07-03 11:30:31.522201 wallpaperscraft-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2279 2023-06-16 14:04:39.000000 wallpaperscraft-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 11:30:31.523200 wallpaperscraft-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-06-16 14:06:58.000000 wallpaperscraft-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:30:31.487054 wallpaperscraft-1.0.1/wallpaperscraft/
+-rw-rw-rw-   0        0        0      164 2023-07-03 11:04:45.000000 wallpaperscraft-1.0.1/wallpaperscraft/__init__.py
+-rw-rw-rw-   0        0        0     3886 2023-07-03 11:04:14.000000 wallpaperscraft-1.0.1/wallpaperscraft/api.py
+-rw-rw-rw-   0        0        0     3227 2023-07-03 11:04:31.000000 wallpaperscraft-1.0.1/wallpaperscraft/asyncapi.py
+-rw-rw-rw-   0        0        0     2962 2023-07-03 11:27:19.000000 wallpaperscraft-1.0.1/wallpaperscraft/types.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:30:31.520202 wallpaperscraft-1.0.1/wallpaperscraft.egg-info/
+-rw-rw-rw-   0        0        0     3018 2023-07-03 11:30:31.000000 wallpaperscraft-1.0.1/wallpaperscraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-07-03 11:30:31.000000 wallpaperscraft-1.0.1/wallpaperscraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 11:30:31.000000 wallpaperscraft-1.0.1/wallpaperscraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-03 11:30:31.000000 wallpaperscraft-1.0.1/wallpaperscraft.egg-info/top_level.txt
```

### Comparing `wallpaperscraft-1.0.0/LICENSE` & `wallpaperscraft-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wallpaperscraft-1.0.0/PKG-INFO` & `wallpaperscraft-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallpaperscraft
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial API WallpapersCraft (wallpaperscraft.com)
 Home-page: https://github.com/Den4ikSuperOstryyPer4ik/WallpapersCraftAPI/
 Download-URL: https://github.com/Den4ikSuperOstryyPer4ik/WallpapersCraftAPI//releases/latest
 Author: Den4ikSuperOstryyPer4ik
 License: Apache2.0
 Keywords: python3 wallpaperscraft wallpapers craft WallpapersCraftAPI
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wallpaperscraft-1.0.0/README.md` & `wallpaperscraft-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wallpaperscraft-1.0.0/setup.py` & `wallpaperscraft-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `wallpaperscraft-1.0.0/wallpaperscraft/api.py` & `wallpaperscraft-1.0.1/wallpaperscraft/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     
     def get(self, query: str = "/", **kwargs):
         if not query.startswith(self.WEBSITE):
             query = self.WEBSITE + query
         
         responce = get(query, **kwargs)
         if not responce.raise_for_status():
-            return BeautifulSoup(responce.text, "html.parser")
+            return BeautifulSoup(responce.text)
     
     def get_all_pictures_from_page(self, page: BeautifulSoup):
         return [
             Picture(
                 link=self.WEBSITE + pic.find("a", {"class": "wallpapers__link"}).get("href"),
                 info=pic.find("a", {"class": "wallpapers__link"}).find_all("span", {"class": "wallpapers__info"})[1].text,
                 downloads=pic.find("a", {"class": "wallpapers__link"}).find_all("span", {"class": "wallpapers__info"})[0].find("span", {"class": "wallpapers__info-downloads"}).text,
```

### Comparing `wallpaperscraft-1.0.0/wallpaperscraft/asyncapi.py` & `wallpaperscraft-1.0.1/wallpaperscraft/asyncapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     async def get(self, query: str = "/", **kwargs):
         if not query.startswith(self.WEBSITE):
             query = self.WEBSITE + query
         
         async with ClientSession() as session:
             responce = await session.get(query, **kwargs)
             if not responce.raise_for_status():
-                return BeautifulSoup(await responce.text(), "html.parser")
+                return BeautifulSoup(await responce.text())
     
     async def get_wallpaper(self, link: str):
         return (await self.get(link)).find("img", {"class": "wallpaper__image"}).get("src")
 
     async def all(self, page: int = 1, resolution: str = "") -> List[Picture]:
         """All pictures."""
         if resolution:
```

### Comparing `wallpaperscraft-1.0.0/wallpaperscraft/types.py` & `wallpaperscraft-1.0.1/wallpaperscraft/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,16 +60,18 @@
 
     def download(self, resolution: str = "1024x768"):
         """
         Get link for picture by resolution
         """
         if resolution not in RESOLUTIONS:
             raise ValueError("Parameter <resolution> isn't a valid screen resolution! Please set a valid resolution.")
-        
-        return self.api_class.get_wallpaper(f"{self.link.replace('/wallpaper/', '/download/')}/{resolution}")
+        URL = f"{self.link.replace('/wallpaper/', '/download/')}"
+        if not any(URL.endswith(i) for i in RESOLUTIONS):
+            URL += f"/{resolution}"
+        return self.api_class.get_wallpaper(URL)
 
 
 class CATALOG(Enum):
     _3D = "3d"
     ABSTRACT = "abstract"
     ANIMALS = "animals"
     ANIME = "anime"
```

### Comparing `wallpaperscraft-1.0.0/wallpaperscraft.egg-info/PKG-INFO` & `wallpaperscraft-1.0.1/wallpaperscraft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallpaperscraft
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial API WallpapersCraft (wallpaperscraft.com)
 Home-page: https://github.com/Den4ikSuperOstryyPer4ik/WallpapersCraftAPI/
 Download-URL: https://github.com/Den4ikSuperOstryyPer4ik/WallpapersCraftAPI//releases/latest
 Author: Den4ikSuperOstryyPer4ik
 License: Apache2.0
 Keywords: python3 wallpaperscraft wallpapers craft WallpapersCraftAPI
 Classifier: Programming Language :: Python :: 3.11
```

