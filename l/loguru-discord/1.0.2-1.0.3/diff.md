# Comparing `tmp/loguru_discord-1.0.2.tar.gz` & `tmp/loguru_discord-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loguru_discord-1.0.2.tar", max compression
+gzip compressed data, was "loguru_discord-1.0.3.tar", max compression
```

## Comparing `loguru_discord-1.0.2.tar` & `loguru_discord-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1062 2023-07-03 05:22:29.772535 loguru_discord-1.0.2/LICENSE
--rw-r--r--   0        0        0     1760 2023-07-03 05:22:29.772535 loguru_discord-1.0.2/README.md
--rw-r--r--   0        0        0      194 2023-07-03 05:22:29.772535 loguru_discord-1.0.2/loguru_discord/__init__.py
--rw-r--r--   0        0        0     3209 2023-07-03 05:22:29.772535 loguru_discord-1.0.2/loguru_discord/sink.py
--rw-r--r--   0        0        0     1216 2023-07-03 05:22:29.772535 loguru_discord-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2846 1970-01-01 00:00:00.000000 loguru_discord-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-03 05:35:18.691832 loguru_discord-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1870 2023-07-03 05:35:18.691832 loguru_discord-1.0.3/README.md
+-rw-r--r--   0        0        0      194 2023-07-03 05:35:18.691832 loguru_discord-1.0.3/loguru_discord/__init__.py
+-rw-r--r--   0        0        0     3209 2023-07-03 05:35:18.691832 loguru_discord-1.0.3/loguru_discord/sink.py
+-rw-r--r--   0        0        0     1150 2023-07-03 05:35:18.691832 loguru_discord-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2882 1970-01-01 00:00:00.000000 loguru_discord-1.0.3/PKG-INFO
```

### Comparing `loguru_discord-1.0.2/LICENSE` & `loguru_discord-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loguru_discord-1.0.2/README.md` & `loguru_discord-1.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Loguru-Discord
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/loguru-discord?label=Python) ![PyPI - Status](https://img.shields.io/pypi/status/loguru-discord?label=PyPI%20Status) ![PyPI - Downloads](https://img.shields.io/pypi/dm/loguru-discord?label=PyPI%20Downloads)
+
 Lightweight, easy-to-use [Discord](https://discord.com/) sink for [Loguru](https://github.com/Delgan/loguru).
 
 <p align="center">
     <img src="https://i.imgur.com/aS7wt4c.png" draggable="false">
 </p>
 
 ## Usage
@@ -48,12 +50,10 @@
 -   **Avatar**: Image URL to use for the Discord Webhook message.
 -   **Embed**: Toggle whether to use plain codeblock formatting or rich embeds.
 
 ## Releases
 
 Loguru-Discord follows [Semantic Versioning](https://semver.org/) for tagging releases of the project.
 
-Changelogs can be found on the [Releases](https://github.com/EthanC/Loguru-Discord/releases) page in the [Keep a Changelog](https://keepachangelog.com/) format.
-
 ## Contributing
 
 Bug fixes and optimizations are always welcome. See [`CONTRIBUTING.md`](https://github.com/EthanC/CallofDuty.py/blob/master/.github/CONTRIBUTING.md) for details.
```

### Comparing `loguru_discord-1.0.2/loguru_discord/sink.py` & `loguru_discord-1.0.3/loguru_discord/sink.py`

 * *Files identical despite different names*

### Comparing `loguru_discord-1.0.2/pyproject.toml` & `loguru_discord-1.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "loguru-discord"
-version = "1.0.2"
+version = "1.0.3"
 description = "Lightweight, easy-to-use Discord sink for Loguru."
 authors = ["EthanC <16727756+EthanC@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["loguru", "discord", "logging", "logger", "sink"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -18,15 +18,14 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed"
 ]
 packages = [{ include = "loguru_discord" }]
 
 [tool.poetry.urls]
 "Twitter" = "https://twitter.com/Mxtive"
-"Changelog" = "https://github.com/EthanC/Loguru-Discord/releases"
 "Issue Tracker" = "https://github.com/EthanC/Loguru-Discord/issues"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 discord-webhook = "^1.1.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `loguru_discord-1.0.2/PKG-INFO` & `loguru_discord-1.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loguru-discord
-Version: 1.0.2
+Version: 1.0.3
 Summary: Lightweight, easy-to-use Discord sink for Loguru.
 License: MIT
 Keywords: loguru,discord,logging,logger,sink
 Author: EthanC
 Author-email: 16727756+EthanC@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,21 +15,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: discord-webhook (>=1.1.0,<2.0.0)
-Project-URL: Changelog, https://github.com/EthanC/Loguru-Discord/releases
 Project-URL: Issue Tracker, https://github.com/EthanC/Loguru-Discord/issues
 Project-URL: Twitter, https://twitter.com/Mxtive
 Description-Content-Type: text/markdown
 
 # Loguru-Discord
 
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/loguru-discord?label=Python) ![PyPI - Status](https://img.shields.io/pypi/status/loguru-discord?label=PyPI%20Status) ![PyPI - Downloads](https://img.shields.io/pypi/dm/loguru-discord?label=PyPI%20Downloads)
+
 Lightweight, easy-to-use [Discord](https://discord.com/) sink for [Loguru](https://github.com/Delgan/loguru).
 
 <p align="center">
     <img src="https://i.imgur.com/aS7wt4c.png" draggable="false">
 </p>
 
 ## Usage
@@ -74,13 +75,11 @@
 -   **Avatar**: Image URL to use for the Discord Webhook message.
 -   **Embed**: Toggle whether to use plain codeblock formatting or rich embeds.
 
 ## Releases
 
 Loguru-Discord follows [Semantic Versioning](https://semver.org/) for tagging releases of the project.
 
-Changelogs can be found on the [Releases](https://github.com/EthanC/Loguru-Discord/releases) page in the [Keep a Changelog](https://keepachangelog.com/) format.
-
 ## Contributing
 
 Bug fixes and optimizations are always welcome. See [`CONTRIBUTING.md`](https://github.com/EthanC/CallofDuty.py/blob/master/.github/CONTRIBUTING.md) for details.
```

