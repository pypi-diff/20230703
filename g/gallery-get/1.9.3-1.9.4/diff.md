# Comparing `tmp/gallery_get-1.9.3.tar.gz` & `tmp/gallery_get-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gallery_get-1.9.3.tar", last modified: Wed Dec  7 04:28:23 2022, max compression
+gzip compressed data, was "gallery_get-1.9.4.tar", last modified: Mon Jul  3 01:09:42 2023, max compression
```

## Comparing `gallery_get-1.9.3.tar` & `gallery_get-1.9.4.tar`

### file list

```diff
@@ -1,45 +1,37 @@
-drwxr-xr-x   0 regosen    (501) staff       (20)        0 2022-12-07 04:28:23.339315 gallery_get-1.9.3/
--rwxrwxrwx   0 regosen    (501) staff       (20)     1067 2013-10-30 23:52:18.000000 gallery_get-1.9.3/LICENSE.txt
--rwxr-xr-x   0 regosen    (501) staff       (20)       36 2020-09-07 22:21:28.000000 gallery_get-1.9.3/MANIFEST.in
--rw-r--r--   0 regosen    (501) staff       (20)     4738 2022-12-07 04:28:23.338674 gallery_get-1.9.3/PKG-INFO
--rwxr-xr-x   0 regosen    (501) staff       (20)     3325 2018-01-01 21:24:21.000000 gallery_get-1.9.3/README
--rwxr-xr-x   0 regosen    (501) staff       (20)     4182 2022-01-01 19:04:27.000000 gallery_get-1.9.3/README.md
--rwxr-xr-x   0 regosen    (501) staff       (20)     3983 2018-01-01 22:18:04.000000 gallery_get-1.9.3/README.rst
-drwxr-xr-x   0 regosen    (501) staff       (20)        0 2022-12-07 04:28:23.286921 gallery_get-1.9.3/gallery_get.egg-info/
--rw-r--r--   0 regosen    (501) staff       (20)     4738 2022-12-07 04:28:21.000000 gallery_get-1.9.3/gallery_get.egg-info/PKG-INFO
--rw-r--r--   0 regosen    (501) staff       (20)     1182 2022-12-07 04:28:22.000000 gallery_get-1.9.3/gallery_get.egg-info/SOURCES.txt
--rw-r--r--   0 regosen    (501) staff       (20)        1 2022-12-07 04:28:21.000000 gallery_get-1.9.3/gallery_get.egg-info/dependency_links.txt
--rw-r--r--   0 regosen    (501) staff       (20)       96 2022-12-07 04:28:22.000000 gallery_get-1.9.3/gallery_get.egg-info/entry_points.txt
--rw-r--r--   0 regosen    (501) staff       (20)       25 2022-12-07 04:28:22.000000 gallery_get-1.9.3/gallery_get.egg-info/requires.txt
--rw-r--r--   0 regosen    (501) staff       (20)       16 2022-12-07 04:28:22.000000 gallery_get-1.9.3/gallery_get.egg-info/top_level.txt
--rwxr-xr-x   0 regosen    (501) staff       (20)    18669 2021-12-31 22:58:14.000000 gallery_get-1.9.3/gallery_get.py
--rw-r--r--   0 regosen    (501) staff       (20)     4402 2017-01-06 04:52:46.000000 gallery_get-1.9.3/gallery_get_test.py
--rw-r--r--   0 regosen    (501) staff       (20)      381 2018-01-01 22:24:53.000000 gallery_get-1.9.3/gallery_get_test_input.csv
-drwxr-xr-x   0 regosen    (501) staff       (20)        0 2022-12-07 04:28:23.336332 gallery_get-1.9.3/gallery_plugins/
--rwxr-xr-x   0 regosen    (501) staff       (20)     2341 2021-02-28 00:00:20.000000 gallery_get-1.9.3/gallery_plugins/__init__.py
--rw-r--r--   0 regosen    (501) staff       (20)     1997 2020-09-23 15:41:13.000000 gallery_get-1.9.3/gallery_plugins/plugin_4chan.py
--rw-r--r--   0 regosen    (501) staff       (20)     2021 2021-12-31 22:58:11.000000 gallery_get-1.9.3/gallery_plugins/plugin_alphacoders.py
--rw-r--r--   0 regosen    (501) staff       (20)     1495 2017-06-25 01:12:47.000000 gallery_get-1.9.3/gallery_plugins/plugin_eroshare.py
--rw-r--r--   0 regosen    (501) staff       (20)     1870 2019-12-28 02:10:40.000000 gallery_get-1.9.3/gallery_plugins/plugin_fuskator.py
--rwxr-xr-x   0 regosen    (501) staff       (20)     1310 2021-03-08 04:58:15.000000 gallery_get-1.9.3/gallery_plugins/plugin_generic.py
--rw-r--r--   0 regosen    (501) staff       (20)     1073 2018-01-08 05:38:39.000000 gallery_get-1.9.3/gallery_plugins/plugin_gfycat.py
--rw-r--r--   0 regosen    (501) staff       (20)     1116 2018-01-01 21:22:22.000000 gallery_get-1.9.3/gallery_plugins/plugin_gogoimage.py
--rw-r--r--   0 regosen    (501) staff       (20)     1032 2019-04-07 20:51:37.000000 gallery_get-1.9.3/gallery_plugins/plugin_imagebam.py
--rwxr-xr-x   0 regosen    (501) staff       (20)     1699 2021-02-28 18:02:35.000000 gallery_get-1.9.3/gallery_plugins/plugin_imagefap.py
--rwxr-xr-x   0 regosen    (501) staff       (20)     1715 2018-08-05 18:41:04.000000 gallery_get-1.9.3/gallery_plugins/plugin_imagefaq_info.py
--rwxr-xr-x   0 regosen    (501) staff       (20)     1081 2019-06-17 03:57:36.000000 gallery_get-1.9.3/gallery_plugins/plugin_imagevenue.py
--rwxr-xr-x   0 regosen    (501) staff       (20)     1118 2020-01-26 16:59:58.000000 gallery_get-1.9.3/gallery_plugins/plugin_imgbox.py
--rwxr-xr-x   0 regosen    (501) staff       (20)     1589 2020-12-30 20:50:26.000000 gallery_get-1.9.3/gallery_plugins/plugin_imgur_album.py
--rw-r--r--   0 regosen    (501) staff       (20)     1977 2019-01-02 01:04:16.000000 gallery_get-1.9.3/gallery_plugins/plugin_pornhub_album.py
--rw-r--r--   0 regosen    (501) staff       (20)     1437 2018-05-25 15:09:00.000000 gallery_get-1.9.3/gallery_plugins/plugin_pornhub_video.py
--rw-r--r--   0 regosen    (501) staff       (20)     1411 2021-07-20 03:34:35.000000 gallery_get-1.9.3/gallery_plugins/plugin_reddit_gallery.py
--rw-r--r--   0 regosen    (501) staff       (20)     1738 2017-12-26 21:39:05.000000 gallery_get-1.9.3/gallery_plugins/plugin_shimmie.py
--rwxr-xr-x   0 regosen    (501) staff       (20)     1490 2018-03-07 03:01:22.000000 gallery_get-1.9.3/gallery_plugins/plugin_vidble.py
--rwxrwxrwx   0 regosen    (501) staff       (20)     1157 2018-09-23 01:22:33.000000 gallery_get-1.9.3/gallery_plugins/plugin_vk.py
--rwxr-xr-x   0 regosen    (501) staff       (20)     1688 2020-02-09 02:59:20.000000 gallery_get-1.9.3/gallery_plugins/plugin_xHamster.py
--rw-r--r--   0 regosen    (501) staff       (20)     1251 2018-11-28 04:50:59.000000 gallery_get-1.9.3/gallery_plugins/plugin_xVideos.py
--rw-r--r--   0 regosen    (501) staff       (20)     1158 2021-05-25 03:12:15.000000 gallery_get-1.9.3/gallery_plugins/plugin_xVideos_gallery.py
--rw-r--r--   0 regosen    (501) staff       (20)     2922 2021-02-28 19:12:48.000000 gallery_get-1.9.3/gallery_utils.py
--rwxr-xr-x   0 regosen    (501) staff       (20)     6311 2021-12-31 23:29:40.000000 gallery_get-1.9.3/reddit_get.py
--rw-r--r--   0 regosen    (501) staff       (20)       38 2022-12-07 04:28:23.339612 gallery_get-1.9.3/setup.cfg
--rwxr-xr-x   0 regosen    (501) staff       (20)     1815 2022-12-07 04:24:18.000000 gallery_get-1.9.3/setup.py
+drwxr-xr-x   0 regosen    (501) staff       (20)        0 2023-07-03 01:09:42.121260 gallery_get-1.9.4/
+-rwxrwxrwx   0 regosen    (501) staff       (20)     1067 2013-10-30 23:52:18.000000 gallery_get-1.9.4/LICENSE.txt
+-rw-r--r--   0 regosen    (501) staff       (20)     4935 2023-07-03 01:09:42.120549 gallery_get-1.9.4/PKG-INFO
+-rwxr-xr-x   0 regosen    (501) staff       (20)     4182 2023-01-11 04:37:13.000000 gallery_get-1.9.4/README.md
+drwxr-xr-x   0 regosen    (501) staff       (20)        0 2023-07-03 01:09:42.097310 gallery_get-1.9.4/gallery_get.egg-info/
+-rw-r--r--   0 regosen    (501) staff       (20)     4935 2023-07-03 01:09:40.000000 gallery_get-1.9.4/gallery_get.egg-info/PKG-INFO
+-rw-r--r--   0 regosen    (501) staff       (20)     1059 2023-07-03 01:09:41.000000 gallery_get-1.9.4/gallery_get.egg-info/SOURCES.txt
+-rw-r--r--   0 regosen    (501) staff       (20)        1 2023-07-03 01:09:40.000000 gallery_get-1.9.4/gallery_get.egg-info/dependency_links.txt
+-rw-r--r--   0 regosen    (501) staff       (20)       78 2023-07-03 01:09:41.000000 gallery_get-1.9.4/gallery_get.egg-info/entry_points.txt
+-rw-r--r--   0 regosen    (501) staff       (20)       25 2023-07-03 01:09:41.000000 gallery_get-1.9.4/gallery_get.egg-info/requires.txt
+-rw-r--r--   0 regosen    (501) staff       (20)       16 2023-07-03 01:09:41.000000 gallery_get-1.9.4/gallery_get.egg-info/top_level.txt
+drwxr-xr-x   0 regosen    (501) staff       (20)        0 2023-07-03 01:09:42.118387 gallery_get-1.9.4/gallery_plugins/
+-rwxr-xr-x   0 regosen    (501) staff       (20)     2341 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/__init__.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1997 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_4chan.py
+-rw-r--r--   0 regosen    (501) staff       (20)     2021 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_alphacoders.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1495 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_eroshare.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1870 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_fuskator.py
+-rwxr-xr-x   0 regosen    (501) staff       (20)     1310 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_generic.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1073 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_gfycat.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1116 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_gogoimage.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1032 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_imagebam.py
+-rwxr-xr-x   0 regosen    (501) staff       (20)     1900 2023-07-03 01:00:12.000000 gallery_get-1.9.4/gallery_plugins/plugin_imagefap.py
+-rwxr-xr-x   0 regosen    (501) staff       (20)     1715 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_imagefaq_info.py
+-rwxr-xr-x   0 regosen    (501) staff       (20)     1081 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_imagevenue.py
+-rwxr-xr-x   0 regosen    (501) staff       (20)     1118 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_imgbox.py
+-rwxr-xr-x   0 regosen    (501) staff       (20)     1589 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_imgur_album.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1977 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_pornhub_album.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1437 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_pornhub_video.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1411 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_reddit_gallery.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1738 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_shimmie.py
+-rwxr-xr-x   0 regosen    (501) staff       (20)     1490 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_vidble.py
+-rwxr-xr-x   0 regosen    (501) staff       (20)     1157 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_vk.py
+-rwxr-xr-x   0 regosen    (501) staff       (20)     1688 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_xHamster.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1251 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_xVideos.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1158 2023-01-11 04:37:13.000000 gallery_get-1.9.4/gallery_plugins/plugin_xVideos_gallery.py
+-rw-r--r--   0 regosen    (501) staff       (20)       38 2023-07-03 01:09:42.121490 gallery_get-1.9.4/setup.cfg
+-rwxr-xr-x   0 regosen    (501) staff       (20)     1790 2023-07-03 01:09:14.000000 gallery_get-1.9.4/setup.py
```

### Comparing `gallery_get-1.9.3/LICENSE.txt` & `gallery_get-1.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/PKG-INFO` & `gallery_get-1.9.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,138 @@
-Metadata-Version: 2.1
-Name: gallery_get
-Version: 1.9.3
-Summary: Gallery downloader - supports many galleries and reddit user histories
-Home-page: https://github.com/regosen/gallery_get
-Author: Rego Sen
-Author-email: regosen@gmail.com
-License: MIT
-Keywords: gallery downloader reddit imgur imgbox 4chan xhamster eroshare vidble pornhub xvideos imagebam alphacoders
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Internet
-Classifier: Topic :: Multimedia :: Graphics
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-
-gallery_get (and reddit_get) - *Download entire galleries*
-----------------------------------------------------------
-
-Many galleries make it hard to download all the images from a gallery.  Their image links often redirect to a viewing page rather than the image itself, making it hard to grab all the images on a page (even with popular browser plugins).  To get around this, gallery_get opens the redirect-links and grabs images from there.
-
-reddit_get grabs all imgur albums and pictures submitted by a given reddit user.  It relies on gallery_get.
-	
-
-Tested Versions and Galleries
------------------------------
-
-Platforms, Python Versions:
-
-* OSX (Python 2.7.2 and 3.5.1)
-* Windows (Python 2.7.3 and 3.6.0)
-
-Gallery Plugins:
-
-* 4chan
-* eroshare
-* fuskator
-* gfycat
-* gogoimage
-* imagefap
-* imagevenue
-* imgbox
-* imgur (albums and galleries)
-* Pornhub (albums and single videos)
-* shimmie
-* vidble
-* xHamster
-* xVideos
-
-Generic Plugin works for:
-
-* alafoto.com
-* forum.phun.org
-* setsdb.org
-* (more)
-
-
-Installation
-------------
-
-You can either download locally or install it::
-
-    pip install gallery_get
-
-
-Usage (Command Line)
---------------------
- 
-Syntax for gallery_get::
-
-    python gallery_get.py
-    python gallery_get.py [URL-OF-GALLERY]
-    python gallery_get.py [URL-OF-GALLERY] [DEST]
-
-Syntax for reddit_get::
-
-    python reddit_get.py
-    python reddit_get.py [REDDIT-USERNAME]
-    python reddit_get.py [REDDIT-USERNAME] [DEST]
-
-If you call with no parameters, you'll be prompted for the gallery URL (for gallery_get) or reddit user (for reddit_get).  You will also be prompted for a destination directory, which it will remember as the default for next time.
-
-If you skip [DEST] it will look for the contents of last_gallery_dest.txt, falling back on the current working directory.
-
-
-Usage (Python Environment)
---------------------------
-
-Syntax for gallery_get::
-
-    import gallery_get
-    gallery_get.run()
-    gallery_get.run(URL)
-    gallery_get.run(URL, DESTINATION)
-    
-Syntax for reddit_get::
-
-    import reddit_get
-    reddit_get.run()
-    reddit_get.run(USER)
-    reddit_get.run(USER, DESTINATION)
-
-Skipping parameters results in same corresponding behavior indicated above.
-
-
-Notes
------
-
-If you run gallery_get or reddit_get on the same URL/user and destination more than once, it will skip the already-existing images next time (unless the size has changed).  This allows you to do incremental updates.
-
-gallery_get comes with a few "plugins" customized for certain sites, along with a generic fallback plugin that works on multiple galleries.  Note that galleries will change their markup from time to time, so these plugins may need to be updated to catch up with such changes.  (Which brings us to the next section...)
-
-
-Testing
--------
-
-I've provided a testing suite called gallery_get_test.py that will run gallery_get/reddit_get with provided URLs and users.  Options are as follows::
-
-    --noprompt          don't prompt for extra galleries
-    --input=INPUT_PATH  input CSV for testing (same format as output)
-
-INPUT_PATH defaults to gallery_get_test_input.csv (provided)
-The output is gallery_get_test_output.csv
-
-To add a new gallery/user to the test:
-
-1. run gallery_get_test.py
-2. enter your gallery/user
-3. repeat step 2 for additional galleries/users
-4. if the output looks ok, replace gallery_get_test_input.csv with gallery_get_test_output.csv
-
-
-Contribute
-----------
-
-Feel free to add your own plugins or make updates if you're familiar with regular expressions and/or Python logic!
-
-Each plugin overrides the following with a string, regular expression, or function.
-
-* title
-* redirect links
-* image links
-* whether to use the same filename from the site, or use "001", "002", etc.
-
-See comments in the existing plugin files for more details.
-
-
-License
--------
-
-Licensed under the MIT License.
-
-
+# gallery_get & reddit_get
+
+**Python suite for batch-downloading images from galleries.**
+
+## Introduction
+
+Many galleries make it hard to download all the images from a gallery.  Their image links often redirect to a viewing page rather than the image itself, making it hard to grab all the images on a page (even with popular browser plugins).  To get around this, gallery_get opens the redirect-links and grabs images from there.
+
+reddit_get grabs all imgur albums and pictures submitted by a given reddit user.  It relies on gallery_get.
+
+
+## Tested Versions and Galleries
+
+Platforms, Python Versions:
+
+* macOS (Python 2.7.2 and 3.5.1)
+* Windows (Python 2.7.3 and 3.6.0)
+
+Gallery Plugins:
+
+* 4chan
+* alphacoders
+* eroshare
+* fuskator
+* gfycat
+* gogoimage
+* imagefap
+* imagevenue
+* imgbox
+* imgur (albums and galleries)
+* Pornhub (albums and single videos)
+* reddit
+* shimmie
+* vidble
+* xHamster
+* xVideos
+
+Generic Plugin works for:
+
+* alafoto.com
+* forum.phun.org
+* setsdb.org
+* (more)
+
+## Installation
+
+You can download this repository from GitHub, or grab it from PyPI:
+
+```
+$ pip install gallery_get
+```
+
+PyPI page is here: https://pypi.python.org/pypi/gallery_get
+
+### Requirements
+
+- Python 2.6+ or any version of Python 3
+- Python packages: [selenium](https://pypi.org/project/selenium/) and [chromedriver-py](https://pypi.org/project/chromedriver-py/)
+  - only needed for imgur albums
+  - automatically installed if you use `pip install`
+
+## Usage
+
+### From the Command Line
+ 
+```
+$ [python -m] gallery_get
+$ [python -m] gallery_get [URL-OF-GALLERY]
+$ [python -m] gallery_get [URL-OF-GALLERY] [DEST]
+```
+
+```
+$ [python -m] reddit_get
+$ [python -m] reddit_get [REDDIT-USERNAME]
+$ [python -m] reddit_get [REDDIT-USERNAME] [DEST]
+```
+
+If you call with no parameters, you'll be prompted for the gallery URL (for gallery_get) or reddit user (for reddit_get).  You will also be prompted for a destination directory, which it will remember as the default for next time.
+
+If you skip [DEST] it will look for the contents of last_gallery_dest.txt, falling back on the current working directory.
+
+### From the Python Environment
+
+```python
+import gallery_get
+gallery_get.run()
+gallery_get.run(URL)
+gallery_get.run(URL, DESTINATION)
+```
+
+```python
+import reddit_get
+reddit_get.run()
+reddit_get.run(USER)
+reddit_get.run(USER, DESTINATION)
+```
+Skipping parameters results in same corresponding behavior indicated above.
+
+## Notes
+
+If you run gallery_get or reddit_get on the same URL/user and destination more than once, it will skip the already-existing images next time (unless the size has changed).  This allows you to do incremental updates.
+
+gallery_get comes with a few "plugins" customized for certain sites, along with a generic fallback plugin that works on multiple galleries.  Note that galleries will change their markup from time to time, so these plugins may need to be updated to catch up with such changes.  (Which brings us to the next section...)
+
+## Testing
+
+I've provided a testing suite called gallery_get_test.py that will run gallery_get/reddit_get with provided URLs and users.  Options are as follows
+```
+  --noprompt          don't prompt for extra galleries
+  --input=INPUT_PATH  input CSV for testing (same format as output)
+```
+INPUT_PATH defaults to gallery_get_test_input.csv (provided)
+The output is gallery_get_test_output.csv
+
+To add a new gallery/user to the test:
+
+  1. run gallery_get_test.py
+  2. enter your gallery/user
+  3. repeat step 2 for additional galleries/users
+  4. if the output looks ok, replace gallery_get_test_input.csv with gallery_get_test_output.csv
+
+## Contribute
+
+Feel free to add your own plugins or make updates if you're familiar with regular expressions and/or Python logic!
+
+Each plugin overrides the following with a string, regular expression, or function.
+
+- title
+- redirect links
+- image links
+- whether to use the same filename from the site, or use "001", "002", etc.
+
+See comments in the existing plugin files for more details.
+
+
+## License
+
+Licensed under the MIT License.
```

### Comparing `gallery_get-1.9.3/gallery_plugins/__init__.py` & `gallery_get-1.9.4/gallery_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_4chan.py` & `gallery_get-1.9.4/gallery_plugins/plugin_4chan.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_alphacoders.py` & `gallery_get-1.9.4/gallery_plugins/plugin_alphacoders.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_eroshare.py` & `gallery_get-1.9.4/gallery_plugins/plugin_eroshare.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_fuskator.py` & `gallery_get-1.9.4/gallery_plugins/plugin_fuskator.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_generic.py` & `gallery_get-1.9.4/gallery_plugins/plugin_generic.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_gfycat.py` & `gallery_get-1.9.4/gallery_plugins/plugin_gfycat.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_gogoimage.py` & `gallery_get-1.9.4/gallery_plugins/plugin_gogoimage.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_imagebam.py` & `gallery_get-1.9.4/gallery_plugins/plugin_imagebam.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_imagefap.py` & `gallery_get-1.9.4/gallery_plugins/plugin_imagefaq_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,36 +5,34 @@
 # Each definition can be one of the following:
 # - a string
 # - a regex string
 # - a function that takes source as a parameter and returns an array or a string.
 # If you comment out a parameter, it will use the default defined in __init__.py
 
 # identifier (default = name of this plugin after "plugin_") : If there's a match, we'll attempt to download images using this plugin.
+identifier = "imagefaq.info"
 
 # title: parses the gallery page for a title.  This will be the folder name of the output gallery.
 title = r'<title>(.+?)</title>'
 
 # redirect: if the links in the gallery page go to an html instead of an image, use this to parse the gallery page.
 def redirect(source):
     redirects = []
-    urls = re.findall(r'href=\'(.+?)\'\>', source)
-    if not urls:
-        return redirects
-    cur_url = urls[0].split("?")[0]
+    cur_url = "https://www.imagefaq.info/gallery.php" + re.findall(r'href=\"(.+?page=.+?)\"\>', source)[0].split("&")[0]
     index = 0
     while True:
-        indexed_page = cur_url + "?page=%d" % index
+        indexed_page = cur_url + "&page=%d" % index
         print("Crawling " + indexed_page)
         indexed_source = urlopen_text(indexed_page)
         links = re.findall('href=[\"\'](/photo/.+)[\"\']',indexed_source)
         if links:
-            redirects += map(lambda x: 'http://www.imagefap.com' + x, links)
+            redirects += map(lambda x: 'https://www.imagefaq.info' + x, links)
             index += 1
         else:
             break
     return redirects
 
 # direct_links: if redirect is non-empty, this parses each redirect page for a single image.  Otherwise, this parses the gallery page for all images.
-direct_links = r'name=\"mainPhoto\".*?(https?://.*?\.imagefap.*?\.com/.*?\.(jpe?g?|png|jfif|gif).*?)\"'
+direct_links = r'name="mainPhoto".+?(https?://x.imagefapusercontent.com/.+?\.(jpe?g?|png|gif))'
 
-# same_filename (default=False): if True, uses filename specified on remote link.  Otherwise, creates own filename with incremental index.
+# same_filename (default=False): if True, uses filename specified on remote link.  Otherwise, creates own filename with incremental index. 
 same_filename = True
```

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_imagefaq_info.py` & `gallery_get-1.9.4/gallery_plugins/plugin_shimmie.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # Plugin for gallery_get.
 import re
 from gallery_utils import *
 
 # Each definition can be one of the following:
 # - a string
 # - a regex string
-# - a function that takes source as a parameter and returns an array or a string.
+# - a function that takes source as a parameter and returns an array or a string.  (You may assume that re and urllib are already imported.)
 # If you comment out a parameter, it will use the default defined in __init__.py
 
 # identifier (default = name of this plugin after "plugin_") : If there's a match, we'll attempt to download images using this plugin.
-identifier = "imagefaq.info"
 
 # title: parses the gallery page for a title.  This will be the folder name of the output gallery.
-title = r'<title>(.+?)</title>'
 
 # redirect: if the links in the gallery page go to an html instead of an image, use this to parse the gallery page.
 def redirect(source):
     redirects = []
-    cur_url = "https://www.imagefaq.info/gallery.php" + re.findall(r'href=\"(.+?page=.+?)\"\>', source)[0].split("&")[0]
+    base_url = "http://shimmie.shishnet.org"
+    cur_url = re.findall(r'href="(.+?)"\>Random</a>', source)[0].rsplit("/",1)[0]
     index = 0
     while True:
-        indexed_page = cur_url + "&page=%d" % index
+        indexed_page = "%s%s/%s" % (base_url, cur_url, index)
         print("Crawling " + indexed_page)
-        indexed_source = urlopen_text(indexed_page)
-        links = re.findall('href=[\"\'](/photo/.+)[\"\']',indexed_source)
-        if links:
-            redirects += map(lambda x: 'https://www.imagefaq.info' + x, links)
-            index += 1
-        else:
-            break
+        try:
+          indexed_source = urlopen_text(indexed_page)
+          links = re.findall("href='(.+?)' class='thumb", indexed_source)
+          if links:
+              redirects += map(lambda x: base_url + x, links)
+              index += 1
+          else:
+              break
+        except:
+          break
     return redirects
 
 # direct_links: if redirect is non-empty, this parses each redirect page for a single image.  Otherwise, this parses the gallery page for all images.
-direct_links = r'name="mainPhoto".+?(https?://x.imagefapusercontent.com/.+?\.(jpe?g?|png|gif))'
+direct_links = r"name='ubb_full-img' value='\[img\](.+?)\[/img\]'"
+
 
 # same_filename (default=False): if True, uses filename specified on remote link.  Otherwise, creates own filename with incremental index. 
-same_filename = True
+same_filename = True
```

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_imagevenue.py` & `gallery_get-1.9.4/gallery_plugins/plugin_imagevenue.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_imgbox.py` & `gallery_get-1.9.4/gallery_plugins/plugin_imgbox.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_imgur_album.py` & `gallery_get-1.9.4/gallery_plugins/plugin_imgur_album.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_pornhub_album.py` & `gallery_get-1.9.4/gallery_plugins/plugin_pornhub_album.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_pornhub_video.py` & `gallery_get-1.9.4/gallery_plugins/plugin_pornhub_video.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_reddit_gallery.py` & `gallery_get-1.9.4/gallery_plugins/plugin_reddit_gallery.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_shimmie.py` & `gallery_get-1.9.4/gallery_plugins/plugin_xHamster.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 # Plugin for gallery_get.
 import re
-from gallery_utils import *
+from gallery_utils import urlopen_text
 
 # Each definition can be one of the following:
 # - a string
 # - a regex string
 # - a function that takes source as a parameter and returns an array or a string.  (You may assume that re and urllib are already imported.)
 # If you comment out a parameter, it will use the default defined in __init__.py
 
 # identifier (default = name of this plugin after "plugin_") : If there's a match, we'll attempt to download images using this plugin.
 
 # title: parses the gallery page for a title.  This will be the folder name of the output gallery.
+title = r'<title>(.*) | xHamster</title>'
 
 # redirect: if the links in the gallery page go to an html instead of an image, use this to parse the gallery page.
 def redirect(source):
-    redirects = []
-    base_url = "http://shimmie.shishnet.org"
-    cur_url = re.findall(r'href="(.+?)"\>Random</a>', source)[0].rsplit("/",1)[0]
-    index = 0
+    redirects = re.findall(r'property="og:url" content="(\S+?)"', source)
+    indexed_source = source
     while True:
-        indexed_page = "%s%s/%s" % (base_url, cur_url, index)
-        print("Crawling " + indexed_page)
-        try:
+        next_url = re.findall(r'data-page="next" href="(\S+?)"', indexed_source)
+        if next_url:
+          indexed_page = next_url[0]
+          redirects.append(indexed_page)
+          print("Crawling " + indexed_page)
           indexed_source = urlopen_text(indexed_page)
-          links = re.findall("href='(.+?)' class='thumb", indexed_source)
-          if links:
-              redirects += map(lambda x: base_url + x, links)
-              index += 1
-          else:
-              break
-        except:
+        else:
           break
     return redirects
 
 # direct_links: if redirect is non-empty, this parses each redirect page for a single image.  Otherwise, this parses the gallery page for all images.
-direct_links = r"name='ubb_full-img' value='\[img\](.+?)\[/img\]'"
-
+def direct_links(source):
+    links = re.findall(r'"imageURL":"(\S+?)"',source)
+    return map(lambda x: x.replace("\/", "/"), links)
 
 # same_filename (default=False): if True, uses filename specified on remote link.  Otherwise, creates own filename with incremental index. 
-same_filename = True
+same_filename = True
```

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_vidble.py` & `gallery_get-1.9.4/gallery_plugins/plugin_vidble.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_vk.py` & `gallery_get-1.9.4/gallery_plugins/plugin_vk.py`

 * *Files identical despite different names*

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_xHamster.py` & `gallery_get-1.9.4/gallery_plugins/plugin_xVideos.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# NOTE: For xVideos use the direct link, which should look something like this: "http://www.xvideos.com/video123456/blah_blah_blah"
+
+
 # Plugin for gallery_get.
 import re
-from gallery_utils import urlopen_text
 
 # Each definition can be one of the following:
 # - a string
 # - a regex string
 # - a function that takes source as a parameter and returns an array or a string.  (You may assume that re and urllib are already imported.)
 # If you comment out a parameter, it will use the default defined in __init__.py
 
 # identifier (default = name of this plugin after "plugin_") : If there's a match, we'll attempt to download images using this plugin.
+identifier = "xvideos.com/video"
 
 # title: parses the gallery page for a title.  This will be the folder name of the output gallery.
-title = r'<title>(.*) | xHamster</title>'
+title = r"setVideoTitle\('(.+?)'"
 
 # redirect: if the links in the gallery page go to an html instead of an image, use this to parse the gallery page.
-def redirect(source):
-    redirects = re.findall(r'property="og:url" content="(\S+?)"', source)
-    indexed_source = source
-    while True:
-        next_url = re.findall(r'data-page="next" href="(\S+?)"', indexed_source)
-        if next_url:
-          indexed_page = next_url[0]
-          redirects.append(indexed_page)
-          print("Crawling " + indexed_page)
-          indexed_source = urlopen_text(indexed_page)
-        else:
-          break
-    return redirects
 
 # direct_links: if redirect is non-empty, this parses each redirect page for a single image.  Otherwise, this parses the gallery page for all images.
-def direct_links(source):
-    links = re.findall(r'"imageURL":"(\S+?)"',source)
-    return map(lambda x: x.replace("\/", "/"), links)
+direct_links = r"setVideoUrlHigh\('(\S+?)'"
 
 # same_filename (default=False): if True, uses filename specified on remote link.  Otherwise, creates own filename with incremental index. 
-same_filename = True
+same_filename = False
+
```

### Comparing `gallery_get-1.9.3/gallery_plugins/plugin_xVideos.py` & `gallery_get-1.9.4/gallery_plugins/plugin_xVideos_gallery.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-# NOTE: For xVideos use the direct link, which should look something like this: "http://www.xvideos.com/video123456/blah_blah_blah"
-
-
 # Plugin for gallery_get.
 import re
 
 # Each definition can be one of the following:
 # - a string
 # - a regex string
 # - a function that takes source as a parameter and returns an array or a string.  (You may assume that re and urllib are already imported.)
 # If you comment out a parameter, it will use the default defined in __init__.py
 
 # identifier (default = name of this plugin after "plugin_") : If there's a match, we'll attempt to download images using this plugin.
-identifier = "xvideos.com/video"
+identifier = "xvideos.com/.+/photos/"
 
 # title: parses the gallery page for a title.  This will be the folder name of the output gallery.
-title = r"setVideoTitle\('(.+?)'"
+title = r'"title":"(.+?)"'
 
 # redirect: if the links in the gallery page go to an html instead of an image, use this to parse the gallery page.
 
 # direct_links: if redirect is non-empty, this parses each redirect page for a single image.  Otherwise, this parses the gallery page for all images.
-direct_links = r"setVideoUrlHigh\('(\S+?)'"
+direct_links = r'href="(https://img-hw.xvideos-cdn.com/videos/profiles/galleries/\S+?)"'
 
 # same_filename (default=False): if True, uses filename specified on remote link.  Otherwise, creates own filename with incremental index. 
-same_filename = False
-
+same_filename = True
```

### Comparing `gallery_get-1.9.3/setup.py` & `gallery_get-1.9.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 # https://packaging.python.org/tutorials/packaging-projects/#uploading-your-project-to-pypi
 
 # NOTE: make sure you have the latest setuptools or the requirements may not get installed correctly.
 # python -m pip install --upgrade pip setuptools
 
 import setuptools
 
-setuptools.setup(
-    name = 'gallery_get',
-    version = '1.9.3',
+setuptools.setup(name = 'gallery_get',
+    version = '1.9.4',
     author = 'Rego Sen',
     author_email = 'regosen@gmail.com',
     url = 'https://github.com/regosen/gallery_get',
     description = 'Gallery downloader - supports many galleries and reddit user histories',
-    long_description = open('README.rst', 'r').read(),
+    long_description = open('README.md', 'r').read(),
     long_description_content_type = 'text/markdown',
     license = 'MIT',
     keywords = 'gallery downloader reddit imgur imgbox 4chan xhamster eroshare vidble pornhub xvideos imagebam alphacoders',
     packages = setuptools.find_packages(),
     include_package_data = True,
     install_requires = [
         'chromedriver-py',
@@ -41,12 +40,12 @@
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 3',
         'Topic :: Internet',
         'Topic :: Multimedia :: Graphics',
     ],
     entry_points = {
         'console_scripts': [
-            'gallery_get = gallery_get.__main__:main',
-            'reddit_get = reddit_get.__main__:main',
+            'gallery_get = gallery_get:main',
+            'reddit_get = reddit_get:main',
         ]
     },
 )
```

