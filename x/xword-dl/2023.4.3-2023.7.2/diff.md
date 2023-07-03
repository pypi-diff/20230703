# Comparing `tmp/xword_dl-2023.4.3.tar.gz` & `tmp/xword_dl-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xword_dl-2023.4.3.tar", last modified: Tue Apr  4 02:19:37 2023, max compression
+gzip compressed data, was "xword_dl-2023.7.2.tar", last modified: Mon Jul  3 00:32:57 2023, max compression
```

## Comparing `xword_dl-2023.4.3.tar` & `xword_dl-2023.7.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2023-04-04 02:19:37.438047 xword_dl-2023.4.3/
--rw-rw-r--   0 parker    (1000) parker    (1000)     1071 2022-11-13 21:48:05.000000 xword_dl-2023.4.3/LICENSE
--rw-rw-r--   0 parker    (1000) parker    (1000)       25 2023-01-17 18:23:19.000000 xword_dl-2023.4.3/MANIFEST.in
--rw-rw-r--   0 parker    (1000) parker    (1000)     6302 2023-04-04 02:19:37.438047 xword_dl-2023.4.3/PKG-INFO
--rw-rw-r--   0 parker    (1000) parker    (1000)     5945 2023-04-04 02:08:50.000000 xword_dl-2023.4.3/README.md
--rw-rw-r--   0 parker    (1000) parker    (1000)      151 2023-01-20 03:14:17.000000 xword_dl-2023.4.3/requirements.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)       38 2023-04-04 02:19:37.438047 xword_dl-2023.4.3/setup.cfg
--rw-rw-r--   0 parker    (1000) parker    (1000)     1040 2023-01-17 18:23:19.000000 xword_dl-2023.4.3/setup.py
-drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2023-04-04 02:19:37.434047 xword_dl-2023.4.3/xword_dl/
--rw-rw-r--   0 parker    (1000) parker    (1000)       24 2022-11-13 21:48:05.000000 xword_dl-2023.4.3/xword_dl/__init__.py
--rw-rw-r--   0 parker    (1000) parker    (1000)       40 2022-11-13 21:48:05.000000 xword_dl-2023.4.3/xword_dl/__main__.py
-drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2023-04-04 02:19:37.438047 xword_dl-2023.4.3/xword_dl/downloader/
--rw-rw-r--   0 parker    (1000) parker    (1000)      812 2022-11-18 17:32:25.000000 xword_dl-2023.4.3/xword_dl/downloader/__init__.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     3652 2022-11-19 15:45:14.000000 xword_dl-2023.4.3/xword_dl/downloader/amuniversaldownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     8389 2023-01-31 23:05:55.000000 xword_dl-2023.4.3/xword_dl/downloader/amuselabsdownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)      820 2022-11-13 21:48:05.000000 xword_dl-2023.4.3/xword_dl/downloader/atlanticdownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     3402 2022-11-19 14:47:56.000000 xword_dl-2023.4.3/xword_dl/downloader/basedownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     2643 2023-04-04 00:39:33.000000 xword_dl-2023.4.3/xword_dl/downloader/compilerdownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     2358 2023-04-04 02:08:50.000000 xword_dl-2023.4.3/xword_dl/downloader/crosswordclubdownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)      991 2022-11-13 21:48:05.000000 xword_dl-2023.4.3/xword_dl/downloader/dailybeastdownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     2798 2022-11-26 20:36:10.000000 xword_dl-2023.4.3/xword_dl/downloader/derstandarddownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     1992 2022-11-19 14:47:56.000000 xword_dl-2023.4.3/xword_dl/downloader/globeandmaildownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     5728 2022-11-19 14:47:56.000000 xword_dl-2023.4.3/xword_dl/downloader/guardiandownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     1161 2022-11-13 21:48:05.000000 xword_dl-2023.4.3/xword_dl/downloader/latimesdownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     2732 2023-04-04 02:08:50.000000 xword_dl-2023.4.3/xword_dl/downloader/mckinseydownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)      844 2022-11-13 21:48:05.000000 xword_dl-2023.4.3/xword_dl/downloader/newsdaydownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     3175 2022-11-19 14:47:56.000000 xword_dl-2023.4.3/xword_dl/downloader/newyorkerdownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     8705 2023-01-17 18:23:19.000000 xword_dl-2023.4.3/xword_dl/downloader/newyorktimesdownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     3341 2023-04-04 00:35:26.000000 xword_dl-2023.4.3/xword_dl/downloader/puzzlesocietydownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)      596 2022-11-13 21:48:05.000000 xword_dl-2023.4.3/xword_dl/downloader/voxdownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)      814 2022-11-13 21:48:05.000000 xword_dl-2023.4.3/xword_dl/downloader/wapodownloader.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     3858 2023-01-31 20:04:10.000000 xword_dl-2023.4.3/xword_dl/downloader/wsjdownloader.py
-drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2023-04-04 02:19:37.438047 xword_dl-2023.4.3/xword_dl/util/
--rw-rw-r--   0 parker    (1000) parker    (1000)       21 2022-11-13 21:48:05.000000 xword_dl-2023.4.3/xword_dl/util/__init__.py
--rw-rw-r--   0 parker    (1000) parker    (1000)     2276 2022-12-16 00:48:10.000000 xword_dl-2023.4.3/xword_dl/util/utils.py
--rw-rw-r--   0 parker    (1000) parker    (1000)        9 2023-04-04 02:12:05.000000 xword_dl-2023.4.3/xword_dl/version
--rw-rw-r--   0 parker    (1000) parker    (1000)     8139 2022-12-26 18:18:52.000000 xword_dl-2023.4.3/xword_dl/xword_dl.py
-drwxrwxr-x   0 parker    (1000) parker    (1000)        0 2023-04-04 02:19:37.434047 xword_dl-2023.4.3/xword_dl.egg-info/
--rw-rw-r--   0 parker    (1000) parker    (1000)     6302 2023-04-04 02:19:37.000000 xword_dl-2023.4.3/xword_dl.egg-info/PKG-INFO
--rw-rw-r--   0 parker    (1000) parker    (1000)     1216 2023-04-04 02:19:37.000000 xword_dl-2023.4.3/xword_dl.egg-info/SOURCES.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)        1 2023-04-04 02:19:37.000000 xword_dl-2023.4.3/xword_dl.egg-info/dependency_links.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)       52 2023-04-04 02:19:37.000000 xword_dl-2023.4.3/xword_dl.egg-info/entry_points.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)      151 2023-04-04 02:19:37.000000 xword_dl-2023.4.3/xword_dl.egg-info/requires.txt
--rw-rw-r--   0 parker    (1000) parker    (1000)        9 2023-04-04 02:19:37.000000 xword_dl-2023.4.3/xword_dl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:32:57.184921 xword_dl-2023.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-03 00:32:57.184921 xword_dl-2023.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 00:32:57.184921 xword_dl-2023.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:32:57.180921 xword_dl-2023.7.2/xword_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:32:57.184921 xword_dl-2023.7.2/xword_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/amuniversaldownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/amuselabsdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/atlanticdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/basedownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/compilerdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/crosswordclubdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/dailybeastdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/derstandarddownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/globeandmaildownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/guardiandownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/latimesdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/mckinseydownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/newsdaydownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/newyorkerdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/newyorktimesdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/puzzlesocietydownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/voxdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/wapodownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/downloader/wsjdownloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:32:57.184921 xword_dl-2023.7.2/xword_dl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/version
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-07-03 00:32:47.000000 xword_dl-2023.7.2/xword_dl/xword_dl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:32:57.184921 xword_dl-2023.7.2/xword_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-03 00:32:57.000000 xword_dl-2023.7.2/xword_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-03 00:32:57.000000 xword_dl-2023.7.2/xword_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 00:32:57.000000 xword_dl-2023.7.2/xword_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 00:32:57.000000 xword_dl-2023.7.2/xword_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-03 00:32:57.000000 xword_dl-2023.7.2/xword_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 00:32:57.000000 xword_dl-2023.7.2/xword_dl.egg-info/top_level.txt
```

### Comparing `xword_dl-2023.4.3/LICENSE` & `xword_dl-2023.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/PKG-INFO` & `xword_dl-2023.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xword_dl
-Version: 2023.4.3
+Version: 2023.7.2
 Summary: a download tool for online crossword puzzles
 Home-page: https://github.com/thisisparker/xword-dl
 Author: Parker Higgins
 Author-email: parker@parkerhiggins.net
 License: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `xword_dl-2023.4.3/README.md` & `xword_dl-2023.7.2/README.md`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/setup.py` & `xword_dl-2023.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/__init__.py` & `xword_dl-2023.7.2/xword_dl/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/amuniversaldownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/amuniversaldownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/amuselabsdownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/amuselabsdownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/atlanticdownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/atlanticdownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/basedownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/basedownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/compilerdownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/compilerdownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/crosswordclubdownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/crosswordclubdownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/dailybeastdownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/dailybeastdownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/derstandarddownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/derstandarddownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/globeandmaildownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/globeandmaildownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/guardiandownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/guardiandownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/latimesdownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/latimesdownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/mckinseydownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/mckinseydownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/newsdaydownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/newsdaydownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/newyorkerdownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/newyorkerdownloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,25 +54,24 @@
         try:
             res.raise_for_status()
         except requests.exceptions.HTTPError:
             raise XWordDLException('Unable to load {}'.format(url))
 
         soup = BeautifulSoup(res.text, "html.parser")
 
-        script_tag = soup.find('script', attrs={'type': 'application/ld+json'})
-
-        json_data = json.loads(script_tag.contents[0])
-
-        iframe_url = json_data['articleBody'].strip().strip('[]')[
-            len('#crossword: '):]
+        iframe_tag = soup.find('iframe', id='crossword')
 
         try:
+            iframe_url = iframe_tag['data-src']
             query = urllib.parse.urlparse(iframe_url).query
             query_id = urllib.parse.parse_qs(query)['id']
             self.id = query_id[0]
+
+        # Will hit this KeyError if there's no matching iframe
+        # or if there's no 'id' query string
         except KeyError:
             raise XWordDLException('Cannot find puzzle at {}.'.format(url))
 
         pubdate = soup.find('time').get_text()
         pubdate_dt = dateparser.parse(pubdate)
 
         self.date = pubdate_dt
```

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/newyorktimesdownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/newyorktimesdownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/puzzlesocietydownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/puzzlesocietydownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/voxdownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/voxdownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/wapodownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/wapodownloader.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/downloader/wsjdownloader.py` & `xword_dl-2023.7.2/xword_dl/downloader/wsjdownloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,18 +25,21 @@
 
     def find_latest(self):
         url = "https://www.wsj.com/news/puzzle"
 
         res = requests.get(url, headers=self.headers)
         soup = BeautifulSoup(res.text, 'html.parser')
 
+        exclude_urls = ['https://www.wsj.com/articles/contest-crosswords-101-how-to-solve-puzzles-11625757841']
+
         for article in soup.find_all('article'):
             if 'crossword' in article.find('span').get_text().lower():
                 latest_url = article.find('a').get('href')
-                break
+                if latest_url not in exclude_urls:
+                    break
         else:
             raise XWordDLException('Unable to find latest puzzle.')
 
         return latest_url
 
     def find_solver(self, url):
         if '/puzzles/crossword/' in url:
```

### Comparing `xword_dl-2023.4.3/xword_dl/util/utils.py` & `xword_dl-2023.7.2/xword_dl/util/utils.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl/xword_dl.py` & `xword_dl-2023.7.2/xword_dl/xword_dl.py`

 * *Files identical despite different names*

### Comparing `xword_dl-2023.4.3/xword_dl.egg-info/PKG-INFO` & `xword_dl-2023.7.2/xword_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xword-dl
-Version: 2023.4.3
+Version: 2023.7.2
 Summary: a download tool for online crossword puzzles
 Home-page: https://github.com/thisisparker/xword-dl
 Author: Parker Higgins
 Author-email: parker@parkerhiggins.net
 License: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `xword_dl-2023.4.3/xword_dl.egg-info/SOURCES.txt` & `xword_dl-2023.7.2/xword_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

