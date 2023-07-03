# Comparing `tmp/qwitch-2.2.1.tar.gz` & `tmp/qwitch-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwitch-2.2.1.tar", last modified: Tue May  2 20:57:01 2023, max compression
+gzip compressed data, was "qwitch-2.2.2.tar", last modified: Mon Jul  3 19:36:26 2023, max compression
```

## Comparing `qwitch-2.2.1.tar` & `qwitch-2.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:57:01.615553 qwitch-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-05-02 20:57:01.615553 qwitch-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-05-02 20:56:41.000000 qwitch-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-02 20:56:41.000000 qwitch-2.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:57:01.611553 qwitch-2.2.1/qwitch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:56:41.000000 qwitch-2.2.1/qwitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-05-02 20:56:41.000000 qwitch-2.2.1/qwitch/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-02 20:56:41.000000 qwitch-2.2.1/qwitch/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-05-02 20:56:41.000000 qwitch-2.2.1/qwitch/qwitch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:57:01.615553 qwitch-2.2.1/qwitch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-05-02 20:57:01.000000 qwitch-2.2.1/qwitch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-02 20:57:01.000000 qwitch-2.2.1/qwitch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:57:01.000000 qwitch-2.2.1/qwitch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 20:57:01.000000 qwitch-2.2.1/qwitch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 20:57:01.000000 qwitch-2.2.1/qwitch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 20:57:01.000000 qwitch-2.2.1/qwitch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-02 20:57:01.615553 qwitch-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-02 20:56:41.000000 qwitch-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:36:26.982856 qwitch-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-03 19:36:26.982856 qwitch-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-07-03 19:36:14.000000 qwitch-2.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-03 19:36:14.000000 qwitch-2.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:36:26.982856 qwitch-2.2.2/qwitch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:36:14.000000 qwitch-2.2.2/qwitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-03 19:36:14.000000 qwitch-2.2.2/qwitch/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-03 19:36:14.000000 qwitch-2.2.2/qwitch/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-07-03 19:36:14.000000 qwitch-2.2.2/qwitch/qwitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:36:26.982856 qwitch-2.2.2/qwitch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-03 19:36:26.000000 qwitch-2.2.2/qwitch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-03 19:36:26.000000 qwitch-2.2.2/qwitch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:36:26.000000 qwitch-2.2.2/qwitch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 19:36:26.000000 qwitch-2.2.2/qwitch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:36:26.000000 qwitch-2.2.2/qwitch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 19:36:26.000000 qwitch-2.2.2/qwitch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-03 19:36:26.982856 qwitch-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-03 19:36:14.000000 qwitch-2.2.2/setup.py
```

### Comparing `qwitch-2.2.1/PKG-INFO` & `qwitch-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwitch
-Version: 2.2.1
+Version: 2.2.2
 Summary: Stream twitch in Quicktime.
 Home-page: https://github.com/gencys/qwitch
 Author: Jean-Francois Vaduret
 Author-email: Jean-Francois Vaduret <jean.francois.vaduret@gmail.com>
 Project-URL: Source, https://github.com/gencys/qwitch
 Project-URL: Tracker, https://github.com/gencys/qwitch/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qwitch-2.2.1/README.md` & `qwitch-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `qwitch-2.2.1/pyproject.toml` & `qwitch-2.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qwitch"
-version = "2.2.1"
+version = "2.2.2"
 description = "Stream twitch in Quicktime."
 readme = "README.md"
 authors = [{ name = "Jean-Francois Vaduret", email = "jean.francois.vaduret@gmail.com" }]
 license = {file = "LICENSE"}
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
```

### Comparing `qwitch-2.2.1/qwitch/api.py` & `qwitch-2.2.2/qwitch/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         else:
             print('-------------------------------')
         print('\033[95mTitle:\033[0m        ' + video['title'])
         date = video['published_at'].replace('T', ' ').replace('Z', '')
         print('\033[95mPublished on:\033[0m ' + date)
         print('\033[95mDuration:\033[0m     ' + video['duration'])
         print('\033[95mURL:\033[0m          ' + video['url'])
-        print('\033[95mVideo ID:\033[0m          ' + video['id'])
+        print('\033[95mVideo ID:\033[0m     ' + video['id'])
         resp = input('\nPlay this video? [y/N] ')
         if str(resp).lower() == 'y':
             url = video['url'].replace('https://www.', '')
             return url
     return None
 
 def exec_streamlink(url, streamlink_config, quality = None):
```

### Comparing `qwitch-2.2.1/qwitch/config.py` & `qwitch-2.2.2/qwitch/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     debug_log('A valid auth-token was found. Proceeding...')
     return content[1]
 
 def store_auth(data):
     now = int(time.time())
     data['requested_at'] = now - 1
     if os.path.exists(home_dir + '/qwitch/config.json'):
-        with open(home_dir + '/qwitch/config.json', 'wr', encoding='utf-8') as file:
+        with open(home_dir + '/qwitch/config.json', 'r+', encoding='utf-8') as file:
             cache_json = json.loads(file.read())
             cache_json[0] = data
             json.dump(cache_json, file, ensure_ascii=False, indent=4)
     else:
         with open(home_dir + '/qwitch/config.json', 'w', encoding='utf-8') as file:
             data = [data]
             json.dump(data, file, ensure_ascii=False, indent=4)
```

### Comparing `qwitch-2.2.1/qwitch/qwitch.py` & `qwitch-2.2.2/qwitch/qwitch.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
             description = 'Stream twitch in Quicktime'
         )
         group = cli.add_mutually_exclusive_group(required=True)
 
         cli.add_argument('channel', nargs='?', default = False, help= 'channel name given in red with -s/--streams. Needed to launch livestream or videos.')
         cli.add_argument('quality', nargs='?', default = False, help= 'video quality name, e.g. 720p, 1080p, best, worst, etc... (defaults to best). You can defined a default quality in the config file (see the README)')
         cli.add_argument('-d', '--debug', action = 'store_true', help= 'enable debugging.')
-        cli.add_argument('--version', action='version', version='%(prog)s 2.2.1')
+        cli.add_argument('--version', action='version', version='%(prog)s 2.2.2')
 
         group.add_argument('-l', '--last', action = 'store_true', help= 'play the most recent video of the channel.')
         group.add_argument('-V', '--Videos', action = 'store_true', help= 'list the last 20 videos of the channel.')
         group.add_argument('-s', '--streams', action = 'store_true', help= 'list the streamers you follow which are currently currently live.')
         group.add_argument('-f', '--follows', action = 'store_true', help= 'list the streamers you follow.')
         group.add_argument('-v', '--vod', action = 'store', type = str, help= 'search for a video by keyword(s) or ID. The keyword needs to be in quotation marks and an exact match (this is not a search engine)')
         args = cli.parse_args()
```

### Comparing `qwitch-2.2.1/qwitch.egg-info/PKG-INFO` & `qwitch-2.2.2/qwitch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwitch
-Version: 2.2.1
+Version: 2.2.2
 Summary: Stream twitch in Quicktime.
 Home-page: https://github.com/gencys/qwitch
 Author: Jean-Francois Vaduret
 Author-email: Jean-Francois Vaduret <jean.francois.vaduret@gmail.com>
 Project-URL: Source, https://github.com/gencys/qwitch
 Project-URL: Tracker, https://github.com/gencys/qwitch/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qwitch-2.2.1/setup.cfg` & `qwitch-2.2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qwitch
-version = 2.2.1
+version = 2.2.2
 author = Jean-Francois Vaduret
 author_email = jean.francois.vaduret@gmail.com
 description = Stream twitch in Quicktime.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/gencys/qwitch
 project_urls =
```

