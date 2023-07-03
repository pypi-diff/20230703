# Comparing `tmp/reflex-icons-1.0.0.tar.gz` & `tmp/reflex-icons-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-icons-1.0.0.tar", last modified: Sun Jul  2 06:49:09 2023, max compression
+gzip compressed data, was "reflex-icons-1.0.2.tar", last modified: Mon Jul  3 07:46:56 2023, max compression
```

## Comparing `reflex-icons-1.0.0.tar` & `reflex-icons-1.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-07-02 06:49:09.971417 reflex-icons-1.0.0/
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1072 2023-07-02 05:59:42.000000 reflex-icons-1.0.0/LICENSE
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1221 2023-07-02 06:49:09.971417 reflex-icons-1.0.0/PKG-INFO
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      789 2023-07-02 06:40:42.000000 reflex-icons-1.0.0/README.md
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-07-02 06:49:09.969417 reflex-icons-1.0.0/reflex_icons/
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    79486 2023-07-02 06:02:07.000000 reflex-icons-1.0.0/reflex_icons/AntDesign.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)   253875 2023-07-02 06:02:07.000000 reflex-icons-1.0.0/reflex_icons/BootStrap.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)   153929 2023-07-02 06:02:07.000000 reflex-icons-1.0.0/reflex_icons/BoxIcons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    25537 2023-07-02 06:02:07.000000 reflex-icons-1.0.0/reflex_icons/CircumIcons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    16833 2023-07-02 06:02:07.000000 reflex-icons-1.0.0/reflex_icons/Devicons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    25033 2023-07-02 06:02:07.000000 reflex-icons-1.0.0/reflex_icons/Feather.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    29853 2023-07-02 06:02:07.000000 reflex-icons-1.0.0/reflex_icons/FlatColorIcons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)   145451 2023-07-02 06:02:07.000000 reflex-icons-1.0.0/reflex_icons/FontAwesome5.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)   187950 2023-07-02 06:02:07.000000 reflex-icons-1.0.0/reflex_icons/FontAwesome6.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)   369939 2023-07-02 06:02:07.000000 reflex-icons-1.0.0/reflex_icons/GameIcons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    23497 2023-07-02 06:02:07.000000 reflex-icons-1.0.0/reflex_icons/GithubOcticonsicons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    54757 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/Grommet-Icons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    44885 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/Heroicons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    90049 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/Heroicons2.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    42653 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/IcoMoonFree.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)   152611 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/Icons8LineAwesome.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    64489 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/Ionicons4.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)   130153 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/Ionicons5.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    94003 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/Lucide.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)   435749 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/MaterialDesignIcons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)   756693 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/PhosphorIcons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    29155 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/RadixIcons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)   217921 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/SimpleIcons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    16751 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/SimpleLineIcons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)   401667 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/TablerIcons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    32803 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/ThemifyIcons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    31593 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/Typicons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    40607 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/VSCodeIcons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    21405 2023-07-02 06:02:08.000000 reflex-icons-1.0.0/reflex_icons/WeatherIcons.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)        0 2023-07-02 06:36:09.000000 reflex-icons-1.0.0/reflex_icons/__init__.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)    64111 2023-07-02 06:02:07.000000 reflex-icons-1.0.0/reflex_icons/css_gg.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      543 2023-07-02 06:02:07.000000 reflex-icons-1.0.0/reflex_icons/extractor.py
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-07-02 06:49:09.970417 reflex-icons-1.0.0/reflex_icons.egg-info/
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1221 2023-07-02 06:49:09.000000 reflex-icons-1.0.0/reflex_icons.egg-info/PKG-INFO
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1096 2023-07-02 06:49:09.000000 reflex-icons-1.0.0/reflex_icons.egg-info/SOURCES.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)        1 2023-07-02 06:49:09.000000 reflex-icons-1.0.0/reflex_icons.egg-info/dependency_links.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)        7 2023-07-02 06:49:09.000000 reflex-icons-1.0.0/reflex_icons.egg-info/requires.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)       13 2023-07-02 06:49:09.000000 reflex-icons-1.0.0/reflex_icons.egg-info/top_level.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)       38 2023-07-02 06:49:09.971417 reflex-icons-1.0.0/setup.cfg
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      775 2023-07-02 06:43:56.000000 reflex-icons-1.0.0/setup.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-07-03 07:46:56.805307 reflex-icons-1.0.2/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1072 2023-07-02 05:59:42.000000 reflex-icons-1.0.2/LICENSE
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1257 2023-07-03 07:46:56.805307 reflex-icons-1.0.2/PKG-INFO
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      825 2023-07-03 07:45:12.000000 reflex-icons-1.0.2/README.md
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-07-03 07:46:56.804308 reflex-icons-1.0.2/reflex_icons/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    79486 2023-07-02 06:02:07.000000 reflex-icons-1.0.2/reflex_icons/AntDesign.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)   253875 2023-07-02 06:02:07.000000 reflex-icons-1.0.2/reflex_icons/BootStrap.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)   153929 2023-07-02 06:02:07.000000 reflex-icons-1.0.2/reflex_icons/BoxIcons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    25537 2023-07-02 06:02:07.000000 reflex-icons-1.0.2/reflex_icons/CircumIcons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    16833 2023-07-02 06:02:07.000000 reflex-icons-1.0.2/reflex_icons/Devicons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    25033 2023-07-02 06:02:07.000000 reflex-icons-1.0.2/reflex_icons/Feather.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    29853 2023-07-02 06:02:07.000000 reflex-icons-1.0.2/reflex_icons/FlatColorIcons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)   145451 2023-07-02 06:02:07.000000 reflex-icons-1.0.2/reflex_icons/FontAwesome5.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)   187950 2023-07-02 06:02:07.000000 reflex-icons-1.0.2/reflex_icons/FontAwesome6.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)   369939 2023-07-02 06:02:07.000000 reflex-icons-1.0.2/reflex_icons/GameIcons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    23497 2023-07-02 06:02:07.000000 reflex-icons-1.0.2/reflex_icons/GithubOcticonsicons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    54757 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/Grommet-Icons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    44885 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/Heroicons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    90049 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/Heroicons2.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    42653 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/IcoMoonFree.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)   152611 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/Icons8LineAwesome.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    64489 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/Ionicons4.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)   130153 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/Ionicons5.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    94003 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/Lucide.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)   435749 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/MaterialDesignIcons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)   756693 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/PhosphorIcons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    29155 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/RadixIcons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)   217921 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/SimpleIcons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    16751 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/SimpleLineIcons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)   401667 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/TablerIcons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    32803 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/ThemifyIcons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    31593 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/Typicons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    40607 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/VSCodeIcons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    21405 2023-07-02 06:02:08.000000 reflex-icons-1.0.2/reflex_icons/WeatherIcons.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)        0 2023-07-02 06:36:09.000000 reflex-icons-1.0.2/reflex_icons/__init__.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)    64111 2023-07-02 06:02:07.000000 reflex-icons-1.0.2/reflex_icons/css_gg.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      543 2023-07-02 06:02:07.000000 reflex-icons-1.0.2/reflex_icons/extractor.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-07-03 07:46:56.805307 reflex-icons-1.0.2/reflex_icons.egg-info/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1257 2023-07-03 07:46:56.000000 reflex-icons-1.0.2/reflex_icons.egg-info/PKG-INFO
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1096 2023-07-03 07:46:56.000000 reflex-icons-1.0.2/reflex_icons.egg-info/SOURCES.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)        1 2023-07-03 07:46:56.000000 reflex-icons-1.0.2/reflex_icons.egg-info/dependency_links.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)        7 2023-07-03 07:46:56.000000 reflex-icons-1.0.2/reflex_icons.egg-info/requires.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       13 2023-07-03 07:46:56.000000 reflex-icons-1.0.2/reflex_icons.egg-info/top_level.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       38 2023-07-03 07:46:56.805307 reflex-icons-1.0.2/setup.cfg
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      775 2023-07-03 07:45:31.000000 reflex-icons-1.0.2/setup.py
```

### Comparing `reflex-icons-1.0.0/LICENSE` & `reflex-icons-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/PKG-INFO` & `reflex-icons-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-icons
-Version: 1.0.0
+Version: 1.0.2
 Summary:  This library provides all icons of React-icons wrapped for ReFlex framework
 Home-page: https://github.com/saurabhwadekar/Reflex-Icons
 Author: Saurabh Wadekar [ INDIA ]
 Maintainer: Saurabh Wadekar
 Maintainer-email: saurabhwadekar420@gmail.com
 License: MIT
 Keywords: react icons,icons,reflex-icons,reflex
@@ -22,25 +22,28 @@
 ## Upgradation
 ```
 pip install reflex-icons --upgrade
 ```
 
 ## Add react-icons in rxconfig.py
 ```python
-frontend_packages=[
+config = rx.Config(
+    ...,
+    frontend_packages=[
         "react-icons",
-    ]
+    ],
+)
 ```
 ## Use
 ```python
 import reflex as rx
 from reflex_icons.BootStrap import BsFill0CircleFill
 
 def index():
-    return pc.box(
+    return rx.box(
         BsFill0CircleFill()
     )
 ```
 
 
 
 #### [📖 View all Icons ](https://react-icons.github.io/react-icons)
```

### Comparing `reflex-icons-1.0.0/README.md` & `reflex-icons-1.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -9,25 +9,28 @@
 ## Upgradation
 ```
 pip install reflex-icons --upgrade
 ```
 
 ## Add react-icons in rxconfig.py
 ```python
-frontend_packages=[
+config = rx.Config(
+    ...,
+    frontend_packages=[
         "react-icons",
-    ]
+    ],
+)
 ```
 ## Use
 ```python
 import reflex as rx
 from reflex_icons.BootStrap import BsFill0CircleFill
 
 def index():
-    return pc.box(
+    return rx.box(
         BsFill0CircleFill()
     )
 ```
 
 
 
 #### [📖 View all Icons ](https://react-icons.github.io/react-icons)
```

### Comparing `reflex-icons-1.0.0/reflex_icons/AntDesign.py` & `reflex-icons-1.0.2/reflex_icons/AntDesign.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/BootStrap.py` & `reflex-icons-1.0.2/reflex_icons/BootStrap.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/BoxIcons.py` & `reflex-icons-1.0.2/reflex_icons/BoxIcons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/CircumIcons.py` & `reflex-icons-1.0.2/reflex_icons/CircumIcons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/Devicons.py` & `reflex-icons-1.0.2/reflex_icons/Devicons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/Feather.py` & `reflex-icons-1.0.2/reflex_icons/Feather.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/FlatColorIcons.py` & `reflex-icons-1.0.2/reflex_icons/FlatColorIcons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/FontAwesome5.py` & `reflex-icons-1.0.2/reflex_icons/FontAwesome5.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/FontAwesome6.py` & `reflex-icons-1.0.2/reflex_icons/FontAwesome6.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/GameIcons.py` & `reflex-icons-1.0.2/reflex_icons/GameIcons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/GithubOcticonsicons.py` & `reflex-icons-1.0.2/reflex_icons/GithubOcticonsicons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/Grommet-Icons.py` & `reflex-icons-1.0.2/reflex_icons/Grommet-Icons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/Heroicons.py` & `reflex-icons-1.0.2/reflex_icons/Heroicons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/Heroicons2.py` & `reflex-icons-1.0.2/reflex_icons/Heroicons2.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/IcoMoonFree.py` & `reflex-icons-1.0.2/reflex_icons/IcoMoonFree.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/Icons8LineAwesome.py` & `reflex-icons-1.0.2/reflex_icons/Icons8LineAwesome.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/Ionicons4.py` & `reflex-icons-1.0.2/reflex_icons/Ionicons4.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/Ionicons5.py` & `reflex-icons-1.0.2/reflex_icons/Ionicons5.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/Lucide.py` & `reflex-icons-1.0.2/reflex_icons/Lucide.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/MaterialDesignIcons.py` & `reflex-icons-1.0.2/reflex_icons/MaterialDesignIcons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/PhosphorIcons.py` & `reflex-icons-1.0.2/reflex_icons/PhosphorIcons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/RadixIcons.py` & `reflex-icons-1.0.2/reflex_icons/RadixIcons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/SimpleIcons.py` & `reflex-icons-1.0.2/reflex_icons/SimpleIcons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/SimpleLineIcons.py` & `reflex-icons-1.0.2/reflex_icons/SimpleLineIcons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/TablerIcons.py` & `reflex-icons-1.0.2/reflex_icons/TablerIcons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/ThemifyIcons.py` & `reflex-icons-1.0.2/reflex_icons/ThemifyIcons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/Typicons.py` & `reflex-icons-1.0.2/reflex_icons/Typicons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/VSCodeIcons.py` & `reflex-icons-1.0.2/reflex_icons/VSCodeIcons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/WeatherIcons.py` & `reflex-icons-1.0.2/reflex_icons/WeatherIcons.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/css_gg.py` & `reflex-icons-1.0.2/reflex_icons/css_gg.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons/extractor.py` & `reflex-icons-1.0.2/reflex_icons/extractor.py`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/reflex_icons.egg-info/PKG-INFO` & `reflex-icons-1.0.2/reflex_icons.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-icons
-Version: 1.0.0
+Version: 1.0.2
 Summary:  This library provides all icons of React-icons wrapped for ReFlex framework
 Home-page: https://github.com/saurabhwadekar/Reflex-Icons
 Author: Saurabh Wadekar [ INDIA ]
 Maintainer: Saurabh Wadekar
 Maintainer-email: saurabhwadekar420@gmail.com
 License: MIT
 Keywords: react icons,icons,reflex-icons,reflex
@@ -22,25 +22,28 @@
 ## Upgradation
 ```
 pip install reflex-icons --upgrade
 ```
 
 ## Add react-icons in rxconfig.py
 ```python
-frontend_packages=[
+config = rx.Config(
+    ...,
+    frontend_packages=[
         "react-icons",
-    ]
+    ],
+)
 ```
 ## Use
 ```python
 import reflex as rx
 from reflex_icons.BootStrap import BsFill0CircleFill
 
 def index():
-    return pc.box(
+    return rx.box(
         BsFill0CircleFill()
     )
 ```
 
 
 
 #### [📖 View all Icons ](https://react-icons.github.io/react-icons)
```

### Comparing `reflex-icons-1.0.0/reflex_icons.egg-info/SOURCES.txt` & `reflex-icons-1.0.2/reflex_icons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reflex-icons-1.0.0/setup.py` & `reflex-icons-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = "reflex-icons",
-    version = "1.0.0",
+    version = "1.0.2",
     author="Saurabh Wadekar [ INDIA ]",
     packages=["reflex_icons"],
     license="MIT",
     maintainer="Saurabh Wadekar",
     maintainer_email="saurabhwadekar420@gmail.com",
     keywords=["react icons","icons","reflex-icons","reflex"],
     description=" This library provides all icons of React-icons wrapped for ReFlex framework",
```

