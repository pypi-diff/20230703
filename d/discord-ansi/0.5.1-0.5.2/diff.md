# Comparing `tmp/discord-ansi-0.5.1.tar.gz` & `tmp/discord-ansi-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-ansi-0.5.1.tar", last modified: Mon Jul  3 10:33:57 2023, max compression
+gzip compressed data, was "discord-ansi-0.5.2.tar", last modified: Mon Jul  3 10:36:11 2023, max compression
```

## Comparing `discord-ansi-0.5.1.tar` & `discord-ansi-0.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 10:33:57.183971 discord-ansi-0.5.1/
--rw-rw-rw-   0        0        0     4804 2023-07-03 10:33:57.182410 discord-ansi-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4185 2023-07-03 10:20:46.000000 discord-ansi-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 10:33:57.167107 discord-ansi-0.5.1/discord_ansi/
--rw-rw-rw-   0        0        0     7614 2023-07-03 10:17:02.000000 discord-ansi-0.5.1/discord_ansi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:33:57.181435 discord-ansi-0.5.1/discord_ansi.egg-info/
--rw-rw-rw-   0        0        0     4804 2023-07-03 10:33:57.000000 discord-ansi-0.5.1/discord_ansi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-07-03 10:33:57.000000 discord-ansi-0.5.1/discord_ansi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 10:33:57.000000 discord-ansi-0.5.1/discord_ansi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-03 10:33:57.000000 discord-ansi-0.5.1/discord_ansi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 10:33:57.000000 discord-ansi-0.5.1/discord_ansi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      781 2023-07-03 10:32:23.000000 discord-ansi-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 10:33:57.183971 discord-ansi-0.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 10:36:11.793425 discord-ansi-0.5.2/
+-rw-rw-rw-   0        0        0     4803 2023-07-03 10:36:11.793425 discord-ansi-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4184 2023-07-03 10:35:31.000000 discord-ansi-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 10:36:11.763684 discord-ansi-0.5.2/discord_ansi/
+-rw-rw-rw-   0        0        0     7614 2023-07-03 10:17:02.000000 discord-ansi-0.5.2/discord_ansi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:36:11.788381 discord-ansi-0.5.2/discord_ansi.egg-info/
+-rw-rw-rw-   0        0        0     4803 2023-07-03 10:36:11.000000 discord-ansi-0.5.2/discord_ansi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-07-03 10:36:11.000000 discord-ansi-0.5.2/discord_ansi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 10:36:11.000000 discord-ansi-0.5.2/discord_ansi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-03 10:36:11.000000 discord-ansi-0.5.2/discord_ansi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 10:36:11.000000 discord-ansi-0.5.2/discord_ansi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      781 2023-07-03 10:35:39.000000 discord-ansi-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 10:36:11.793425 discord-ansi-0.5.2/setup.cfg
```

### Comparing `discord-ansi-0.5.1/PKG-INFO` & `discord-ansi-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-ansi
-Version: 0.5.1
+Version: 0.5.2
 Summary: Discord messages with ANSI (message builder + ANSI Art)
 Author-email: GEOEGII555 <geoegii2001555@gmail.com>, "GEOEGII555 (Alternative email)" <webmaster@geoegii555.eu.org>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -90,16 +90,15 @@
 # Or you can send a direct request to Discord API
 # requests.post("https://discord.com/api/v10/channels/.../messages", json=dict(content=text), headers=dict(authorization="Bot <token>"))
 ```
 # More info
 Q: What are the colours available?
 A: Tutorial:
 1. Open your Python interpreter
-2.
-```py
+2. ```py
 import discord_ansi
 print(discord_ansi.foreground_colors.keys())
 print(discord_ansi.background_colors.keys())
 ```
 If you are making an ANSI art, use background colors
 Q: What if I want to send a colored output from a **terminal command**?
 A: If you want to insert it into a subclass of MessageBuilder:
```

### Comparing `discord-ansi-0.5.1/README.md` & `discord-ansi-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -77,16 +77,15 @@
 # Or you can send a direct request to Discord API
 # requests.post("https://discord.com/api/v10/channels/.../messages", json=dict(content=text), headers=dict(authorization="Bot <token>"))
 ```
 # More info
 Q: What are the colours available?
 A: Tutorial:
 1. Open your Python interpreter
-2.
-```py
+2. ```py
 import discord_ansi
 print(discord_ansi.foreground_colors.keys())
 print(discord_ansi.background_colors.keys())
 ```
 If you are making an ANSI art, use background colors
 Q: What if I want to send a colored output from a **terminal command**?
 A: If you want to insert it into a subclass of MessageBuilder:
```

### Comparing `discord-ansi-0.5.1/discord_ansi/__init__.py` & `discord-ansi-0.5.2/discord_ansi/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-ansi-0.5.1/discord_ansi.egg-info/PKG-INFO` & `discord-ansi-0.5.2/discord_ansi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-ansi
-Version: 0.5.1
+Version: 0.5.2
 Summary: Discord messages with ANSI (message builder + ANSI Art)
 Author-email: GEOEGII555 <geoegii2001555@gmail.com>, "GEOEGII555 (Alternative email)" <webmaster@geoegii555.eu.org>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -90,16 +90,15 @@
 # Or you can send a direct request to Discord API
 # requests.post("https://discord.com/api/v10/channels/.../messages", json=dict(content=text), headers=dict(authorization="Bot <token>"))
 ```
 # More info
 Q: What are the colours available?
 A: Tutorial:
 1. Open your Python interpreter
-2.
-```py
+2. ```py
 import discord_ansi
 print(discord_ansi.foreground_colors.keys())
 print(discord_ansi.background_colors.keys())
 ```
 If you are making an ANSI art, use background colors
 Q: What if I want to send a colored output from a **terminal command**?
 A: If you want to insert it into a subclass of MessageBuilder:
```

### Comparing `discord-ansi-0.5.1/pyproject.toml` & `discord-ansi-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "discord-ansi"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="GEOEGII555", email="geoegii2001555@gmail.com" },
   { name="GEOEGII555 (Alternative email)", email="webmaster@geoegii555.eu.org" },
 ]
 description = "Discord messages with ANSI (message builder + ANSI Art)"
 readme = "README.md"
 requires-python = ">=3.7"
```

