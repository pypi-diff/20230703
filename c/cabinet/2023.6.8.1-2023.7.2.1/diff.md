# Comparing `tmp/cabinet-2023.6.8.1.tar.gz` & `tmp/cabinet-2023.7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2023.6.8.1.tar", last modified: Fri Jun  9 04:30:15 2023, max compression
+gzip compressed data, was "cabinet-2023.7.2.1.tar", last modified: Mon Jul  3 04:10:58 2023, max compression
```

## Comparing `cabinet-2023.6.8.1.tar` & `cabinet-2023.7.2.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.6.8.1/LICENSE
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6579 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6228 2023-05-31 04:52:07.000000 cabinet-2023.6.8.1/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.6.8.1/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/cabinet/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       80 2023-06-09 04:30:03.000000 cabinet-2023.6.8.1/src/cabinet/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-05-31 04:50:50.000000 cabinet-2023.6.8.1/src/cabinet/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    26147 2023-06-09 04:29:47.000000 cabinet-2023.6.8.1/src/cabinet/cabinet.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.6.8.1/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/cabinet.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6579 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      333 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/top_level.txt
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/test/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     5868 2023-05-31 04:52:07.000000 cabinet-2023.6.8.1/test/test___init__.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-03 04:10:58.977777 cabinet-2023.7.2.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1090 2023-06-17 20:33:55.000000 cabinet-2023.7.2.1/LICENSE
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     7689 2023-07-03 04:10:58.977777 cabinet-2023.7.2.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     7338 2023-07-03 03:56:29.000000 cabinet-2023.7.2.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.7.2.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-07-03 04:10:58.977777 cabinet-2023.7.2.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-03 04:10:58.973777 cabinet-2023.7.2.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-03 04:10:58.973777 cabinet-2023.7.2.1/src/cabinet/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       80 2023-06-25 04:32:18.000000 cabinet-2023.7.2.1/src/cabinet/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-06-25 04:32:22.000000 cabinet-2023.7.2.1/src/cabinet/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    34085 2023-07-03 04:10:25.000000 cabinet-2023.7.2.1/src/cabinet/cabinet.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2314 2023-07-03 03:56:29.000000 cabinet-2023.7.2.1/src/cabinet/constants.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.7.2.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-03 04:10:58.977777 cabinet-2023.7.2.1/src/cabinet.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     7689 2023-07-03 04:10:58.000000 cabinet-2023.7.2.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      358 2023-07-03 04:10:58.000000 cabinet-2023.7.2.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-07-03 04:10:58.000000 cabinet-2023.7.2.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-07-03 04:10:58.000000 cabinet-2023.7.2.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-07-03 04:10:58.000000 cabinet-2023.7.2.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-03 04:10:58.977777 cabinet-2023.7.2.1/test/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     5874 2023-06-25 05:21:17.000000 cabinet-2023.7.2.1/test/test___init__.py
```

### Comparing `cabinet-2023.6.8.1/PKG-INFO` & `cabinet-2023.7.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,81 @@
-Metadata-Version: 2.1
-Name: cabinet
-Version: 2023.6.8.1
-Summary: Easily manage data storage and logging across repos
-Home-page: https://github.com/tylerjwoodfin/cabinet
-Author: Tyler Woodfin
-Author-email: feedback@tyler.cloud
-License: : OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # cabinet
-A Python library to easily store data across multiple projects in one or more JSON files.
+A Python library to easily manage data with MongoDB and across other files.
 
 Supports a cli, email, and event logging.
 
+## MongoDB Update! - 2023-06-25
+- In this latest release, the tool has been redesigned from the ground up to use MongoDB.
+- MongoDB elevates Cabinet to the best of both worlds: a secure database with the ability to edit 
+  as if it were a JSON structure.
+- Every function has been tested for compatibility with earlier releases, but it's likely
+  there will be some edge case bugs to iron out. I use this tool extremely often in my day-to-day
+  use, so these should be patched quickly, once discovered. Please report issues as you find them.
+
 ## Features
 
-- Read and write data in the JSON files of your choice
+- Read and write data in MongoDB and/or the JSON files of your choice
+- Provides easy shortcuts to MongoDB actions
 - Log to a file/directory of your choice without having to configure `logger` each time
 - Send/receive mail using `cabinet.Cabinet().mail()`
 
+## Dependencies
+
+- Python >= 3.6
+- MongoDB
+- Pymongo (`pip install pymongo`)
+- smtplib
+
 ## Structure
 
-- Data is stored in a `settings.json` file in the location of your choice
-- Logs are written to `{/path/to/cabinet}/log/LOG_DAILY_YYYY-MM-DD` by default
-  - this can be changed on a per-log basis
+- Data is stored in MongoDB; simply plug in your credentials.
+- Logs are written to `~/.cabinet/log/LOG_DAILY_YYYY-MM-DD` by default
+  - this can be changed as needed (per log or otherwise)
 
 ## Installation and Setup
 
 ```bash
   python3 -m pip install cabinet
-
+  python3 -m pip install pymongo
   cabinet --config
 ```
 
 ## CLI usage
 ```
 Usage: cabinet [OPTIONS]
 
 Options:
   -h, --help              Show this help message and exit
   --configure, -config    Configure
-  --edit, -e              Edit the settings.json file
+  --export                Export the data in MongoDB to a JSON file
+  --edit, -e              Edit MongoDB in the default editor as a JSON file
   --edit-file, -ef        Edit a specific file
   --no-create             (for -ef) Do not create file if it does not exist
-  --get, -g [GET ...]     Get a property from settings.json
-  --put PUT [PUT ...]     Put a property into settings.json
-  --get-file GET_FILE     Get file
+  --get, -g               Get a property from MongoDB (nesting supported)
+  --put, -p               Put a property into MongoDB (nesting supported)
+  --remove, -rm           Removes a property from MongoDB
+  --get-file              Returns the file specified
   --strip                 (for --get-file) Whether to strip file content whitespace
   --log, -l               Log a message to the default location
-  --level LOG_LEVEL       (for -l) Log level [debug, info, warn, error, critical]
+  --level                 (for -l) Log level [debug, info, warn, error, critical]
   -v, --version           show version number and exit
 
 Mail:
   --mail                Sends an email
   --subject SUBJECT, -s SUBJECT
                         Email subject
   --body BODY, -b BODY  Email body
   --to TO_ADDR, -t TO_ADDR
 ```
 
 ## Configuration
 
-- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet --config`.
+- Upon first launch, the tool will prompt you to enter your MongoDB credentials, as well as
+  the cluster name and Database name. These are stored only within the package, as a file named
+  `cabinet_config.json`.
 
 ### edit_file() shortcuts
 - see example below to enable something like
   - `cabinet -ef shopping` from the terminal
     - rather than `cabinet -ef "/home/{username}/path/to/shopping_list.md"`
   - or `cabinet.Cabinet().edit("shopping")`
     - rather than `cabinet.Cabinet().edit("/home/{username}/path/to/whatever.md")`
@@ -96,15 +104,15 @@
 cabinet -p edit todo value "/home/{username}/path/to/whatever.md"
 ```
 
 ### mail
 
 - It is NEVER a good idea to store your password in plaintext; for this reason, I strongly recommend a "throwaway" account that is only used for sending emails
 - Gmail (as of May 2022) and most other mainstream email providers won't work with this; for support, search for sending mail from your email provider with `smtplib`.
-- In `settings.json`, add the `email` object to make your settings file look like this example:
+- In MongoDB, add the `email` object to make your settings file look like this example:
 
 file:
 ```
 {
     "email": {
         "from": "throwaway@example.com",
         "from_pw": "example",
@@ -135,19 +143,18 @@
 cab = Cabinet()
 
 cab.put("employee", "Tyler", "salary", 7.25)
 ```
 
 or terminal:
 ```
-# warning - from the terminal, numeric values in cabinet are stored as strings
-cabinet -p employer Tyler salary 7.25
+cabinet -p employee Tyler salary 7.25
 ```
 
-results in this structure in settings.json:
+results in this structure in MongoDB:
 ```
 {
     "employee": {
         "Tyler": {
             "salary": 7.25 # or "7.25" if done from terminal
         }
     }
@@ -171,14 +178,39 @@
 ```
 
 results in:
 ```
 7.25
 ```
 
+### `remove`
+
+python:
+```
+from cabinet import Cabinet
+
+cab = Cabinet()
+
+cab.remove("employee", "Tyler", "salary")
+```
+
+or terminal:
+```
+cabinet -rm employee Tyler salary
+```
+
+results in this structure in MongoDB:
+```
+{
+    "employee": {
+        "tyler": {}
+    }
+}
+```
+
 ### `edit_file`
 
 python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
@@ -237,19 +269,19 @@
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cab.log("30", logName="LOG_TEMPERATURE")
+cab.log("30", log_name="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
+cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
@@ -260,19 +292,14 @@
 # -l and --log are interchangeable
 cab --log "Connection timed out"
 
 # change levels with --level
 cab --log "Server is on fire" --level "critical"
 ```
 
-## Dependencies
-
-- Python >= 3.6
-- smtplib
-
 ## Disclaimers
 
 - Although I've done quite a bit of testing, I can't guarantee everything that works on my machine will work on yours. Always back up your data to multiple places to avoid data loss.
 - If you find any issues, please contact me... or get your hands dirty and raise a PR!
 
 ## Unit Tests
 - Unit tests are available in `test/`; use `pytest test/` to run them.
```

### Comparing `cabinet-2023.6.8.1/README.md` & `cabinet-2023.7.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,93 @@
+Metadata-Version: 2.1
+Name: cabinet
+Version: 2023.7.2.1
+Summary: Easily manage data storage and logging across repos
+Home-page: https://github.com/tylerjwoodfin/cabinet
+Author: Tyler Woodfin
+Author-email: feedback@tyler.cloud
+License: : OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # cabinet
-A Python library to easily store data across multiple projects in one or more JSON files.
+A Python library to easily manage data with MongoDB and across other files.
 
 Supports a cli, email, and event logging.
 
+## MongoDB Update! - 2023-06-25
+- In this latest release, the tool has been redesigned from the ground up to use MongoDB.
+- MongoDB elevates Cabinet to the best of both worlds: a secure database with the ability to edit 
+  as if it were a JSON structure.
+- Every function has been tested for compatibility with earlier releases, but it's likely
+  there will be some edge case bugs to iron out. I use this tool extremely often in my day-to-day
+  use, so these should be patched quickly, once discovered. Please report issues as you find them.
+
 ## Features
 
-- Read and write data in the JSON files of your choice
+- Read and write data in MongoDB and/or the JSON files of your choice
+- Provides easy shortcuts to MongoDB actions
 - Log to a file/directory of your choice without having to configure `logger` each time
 - Send/receive mail using `cabinet.Cabinet().mail()`
 
+## Dependencies
+
+- Python >= 3.6
+- MongoDB
+- Pymongo (`pip install pymongo`)
+- smtplib
+
 ## Structure
 
-- Data is stored in a `settings.json` file in the location of your choice
-- Logs are written to `{/path/to/cabinet}/log/LOG_DAILY_YYYY-MM-DD` by default
-  - this can be changed on a per-log basis
+- Data is stored in MongoDB; simply plug in your credentials.
+- Logs are written to `~/.cabinet/log/LOG_DAILY_YYYY-MM-DD` by default
+  - this can be changed as needed (per log or otherwise)
 
 ## Installation and Setup
 
 ```bash
   python3 -m pip install cabinet
-
+  python3 -m pip install pymongo
   cabinet --config
 ```
 
 ## CLI usage
 ```
 Usage: cabinet [OPTIONS]
 
 Options:
   -h, --help              Show this help message and exit
   --configure, -config    Configure
-  --edit, -e              Edit the settings.json file
+  --export                Export the data in MongoDB to a JSON file
+  --edit, -e              Edit MongoDB in the default editor as a JSON file
   --edit-file, -ef        Edit a specific file
   --no-create             (for -ef) Do not create file if it does not exist
-  --get, -g [GET ...]     Get a property from settings.json
-  --put PUT [PUT ...]     Put a property into settings.json
-  --get-file GET_FILE     Get file
+  --get, -g               Get a property from MongoDB (nesting supported)
+  --put, -p               Put a property into MongoDB (nesting supported)
+  --remove, -rm           Removes a property from MongoDB
+  --get-file              Returns the file specified
   --strip                 (for --get-file) Whether to strip file content whitespace
   --log, -l               Log a message to the default location
-  --level LOG_LEVEL       (for -l) Log level [debug, info, warn, error, critical]
+  --level                 (for -l) Log level [debug, info, warn, error, critical]
   -v, --version           show version number and exit
 
 Mail:
   --mail                Sends an email
   --subject SUBJECT, -s SUBJECT
                         Email subject
   --body BODY, -b BODY  Email body
   --to TO_ADDR, -t TO_ADDR
 ```
 
 ## Configuration
 
-- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet --config`.
+- Upon first launch, the tool will prompt you to enter your MongoDB credentials, as well as
+  the cluster name and Database name. These are stored only within the package, as a file named
+  `cabinet_config.json`.
 
 ### edit_file() shortcuts
 - see example below to enable something like
   - `cabinet -ef shopping` from the terminal
     - rather than `cabinet -ef "/home/{username}/path/to/shopping_list.md"`
   - or `cabinet.Cabinet().edit("shopping")`
     - rather than `cabinet.Cabinet().edit("/home/{username}/path/to/whatever.md")`
@@ -84,15 +116,15 @@
 cabinet -p edit todo value "/home/{username}/path/to/whatever.md"
 ```
 
 ### mail
 
 - It is NEVER a good idea to store your password in plaintext; for this reason, I strongly recommend a "throwaway" account that is only used for sending emails
 - Gmail (as of May 2022) and most other mainstream email providers won't work with this; for support, search for sending mail from your email provider with `smtplib`.
-- In `settings.json`, add the `email` object to make your settings file look like this example:
+- In MongoDB, add the `email` object to make your settings file look like this example:
 
 file:
 ```
 {
     "email": {
         "from": "throwaway@example.com",
         "from_pw": "example",
@@ -123,19 +155,18 @@
 cab = Cabinet()
 
 cab.put("employee", "Tyler", "salary", 7.25)
 ```
 
 or terminal:
 ```
-# warning - from the terminal, numeric values in cabinet are stored as strings
-cabinet -p employer Tyler salary 7.25
+cabinet -p employee Tyler salary 7.25
 ```
 
-results in this structure in settings.json:
+results in this structure in MongoDB:
 ```
 {
     "employee": {
         "Tyler": {
             "salary": 7.25 # or "7.25" if done from terminal
         }
     }
@@ -159,14 +190,39 @@
 ```
 
 results in:
 ```
 7.25
 ```
 
+### `remove`
+
+python:
+```
+from cabinet import Cabinet
+
+cab = Cabinet()
+
+cab.remove("employee", "Tyler", "salary")
+```
+
+or terminal:
+```
+cabinet -rm employee Tyler salary
+```
+
+results in this structure in MongoDB:
+```
+{
+    "employee": {
+        "tyler": {}
+    }
+}
+```
+
 ### `edit_file`
 
 python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
@@ -225,19 +281,19 @@
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cab.log("30", logName="LOG_TEMPERATURE")
+cab.log("30", log_name="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
+cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
@@ -248,19 +304,14 @@
 # -l and --log are interchangeable
 cab --log "Connection timed out"
 
 # change levels with --level
 cab --log "Server is on fire" --level "critical"
 ```
 
-## Dependencies
-
-- Python >= 3.6
-- smtplib
-
 ## Disclaimers
 
 - Although I've done quite a bit of testing, I can't guarantee everything that works on my machine will work on yours. Always back up your data to multiple places to avoid data loss.
 - If you find any issues, please contact me... or get your hands dirty and raise a PR!
 
 ## Unit Tests
 - Unit tests are available in `test/`; use `pytest test/` to run them.
```

### Comparing `cabinet-2023.6.8.1/setup.cfg` & `cabinet-2023.7.2.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
 name = cabinet
-version = 2023.06.08.1
+version = 2023.07.02.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls = 
-Bug Tracker = https://github.com/tylerjwoodfin/cabinet/issues
+bug tracker = https://github.com/tylerjwoodfin/cabinet/issues
 py_modules = ["cabinet"]
 classifiers = 
-Programming Language = : Python :: 3
-License = : OSI Approved :: MIT License
-Operating System = : OS Independent
+programming language = : Python :: 3
+license = : OSI Approved :: MIT License
+operating system = : OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
```

### Comparing `cabinet-2023.6.8.1/src/cabinet/cabinet.py` & `cabinet-2023.7.2.1/src/cabinet/cabinet.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,189 +6,153 @@
 Usage:
     ```
     from cabinet import Cabinet
 
     cab = Cabinet()
     ```
 """
-
 import os
-import json
-import pathlib
-import logging
+import ast
 import sys
+import json
 import argparse
-from datetime import date
-from typing import Optional
+import logging
 import importlib.metadata
+import getpass
+import pathlib
+import subprocess
+from datetime import date, datetime
+from typing import Optional
+import pymongo.errors
+from pymongo.mongo_client import MongoClient
+from pymongo.server_api import ServerApi
+from bson import json_util, ObjectId
+from .constants import (
+    NEW_SETUP_MSG_INTRO,
+    NEW_SETUP_MSG_MONGODB_INSTRUCTIONS,
+    CONFIG_MONGODB_USERNAME,
+    CONFIG_MONGODB_PASSWORD,
+    CONFIG_MONGODB_CLUSTER_NAME,
+    CONFIG_MONGODB_DB_NAME,
+    CONFIG_PATH_CABINET,
+    ERROR_CONFIG_MISSING_VALUES,
+    ERROR_CONFIG_JSON_DECODE,
+    ERROR_CONFIG_FILE_INVALID
+)
 from .mail import Mail
 
 
 class Cabinet:
     """
-    The main class for Cabinet
+    Cabinet class
     """
 
+    mongodb_username: str = ''
+    mongodb_password: str = ''
+    mongodb_cluster_name: str = ''
+    mongodb_db_name: str = ''
+    mongodb_uri = ""
+    client: MongoClient = None
+    database = None
+    new_setup: bool = False
+    path_config_file = str(pathlib.Path(
+        __file__).resolve().parent / "cabinet_config.json")
     path_cabinet: str = None
-    path_config_file: str = None
-    path_settings_file: str = None
     path_log: str = None
-    settings_json = None
-    new_setup: bool = False
 
-    NEW_SETUP_MSG = (
-        "Welcome to Cabinet!\n\n"
-        "Enter the directory to store the default settings.json.\n"
-        "This should be an absolute path in a public place, like "
-        f"{pathlib.Path.home().resolve()}/cabinet.\n\n"
-        "Don't worry, this won't overwrite anything in this folder.\n"
-        "By continuing, a new configuration file will be created in your site-packages folder.\n\n"
-    )
-
-    def __init__(self, path_cabinet: str = None):
+    def _get_config(self, key=None):
         """
-        The main module for file management
+        Retrieves the value associated with the specified key from the configuration file.
 
         Args:
-            - path_cabinet (str, optional): the directory of a settings.json file to be used
-                Defaults to get_config('path_cabinet') or ~/cabinet if unset
+            key (str): The key to retrieve the corresponding value.
+                - If None, the entire configuration dictionary is returned.
+                - Default is None.
 
         Returns:
-            None
-
-        Usage:
-            ```
-            from cabinet import Cabinet
-            cab = cabinet.Cabinet()
-            ```
-        """
+            The value associated with the specified key in the configuration file. If the key is not
+            found, an empty string is returned.
 
-        # config file, stored within the package
-        self.path_config_file = str(pathlib.Path(
-            __file__).resolve().parent / "config.json")
-
-        # determines where settings.json is stored; by default, this is ~/cabinet
-        self.path_cabinet = path_cabinet or os.path.expanduser(
-            self._get_config('path_cabinet'))
-
-        path_cabinet = self.path_cabinet
-
-        # new setup
-        if path_cabinet is None:
-            self.new_setup = True
-            path_cabinet = input(self.NEW_SETUP_MSG)
-            if not path_cabinet:
-                path_cabinet = str(pathlib.Path.home() / "cabinet")
+        Raises:
+            FileNotFoundError: If the configuration file is not found.
+            KeyError: If the key is not found in the configuration file.
+            JSONDecodeError: If there is a problem decoding the JSON data in the configuration file.
+
+        Notes:
+            If the key is 'mongodb_username' and the configuration file is not found,
+            the user will be prompted to set up a new configuration.
+            The value for 'mongodb_username' will be obtained
+            from the user input.
+
+            If the key is 'mongodb_password', 'mongodb_cluster_name',
+            'mongodb_db_name', or 'path_cabinet'
+            and the new_setup flag is True, the user will be prompted to
+            enter the corresponding value
+            for the new configuration.
+
+            If the JSON data in the configuration file is not valid,
+            the user will be given the option
+            to overwrite the file with an empty dictionary or fix the file manually.
+        """
+
+        def config_prompts(key=None):
+            if key == 'mongodb_username':
+                value = input(CONFIG_MONGODB_USERNAME)
+                self._put_config(key, value)
+            if key == 'mongodb_password':
+                value = getpass.getpass(CONFIG_MONGODB_PASSWORD)
+                self._put_config(key, value)
+            if key == 'mongodb_cluster_name':
+                value = input(CONFIG_MONGODB_CLUSTER_NAME)
+                self._put_config(key, value)
+            if key == 'mongodb_db_name':
+                value = input(CONFIG_MONGODB_DB_NAME)
+                self._put_config(key, value)
+            if key == 'path_cabinet':
+                value = input(CONFIG_PATH_CABINET) \
+                    or f"{pathlib.Path.home().resolve()}/.cabinet"
+                self._put_config(key, value)
 
-        self.path_settings_file = pathlib.Path(path_cabinet) / "settings.json"
+            return value
 
         try:
-            with open(f'{path_cabinet}/settings.json', 'r+', encoding="utf8") as file:
-                file.seek(0, os.SEEK_END)
+            with open(self.path_config_file, 'r+', encoding="utf8") as file:
+                return json.load(file)[key]
         except FileNotFoundError:
-            # initialize settings file if it doesn't exist
-            if not os.path.exists(path_cabinet):
-                os.makedirs(path_cabinet)
-            with open(f'{path_cabinet}/settings.json', 'x+', encoding="utf8") as file:
-                new_file_msg = ("\n\nWarning: settings.json not found; "
-                                f"created a blank one in {path_cabinet}")
-                self._ifprint(new_file_msg,
-                              self.new_setup is False)
-                self._ifprint("You can change this location by calling 'cabinet config'.\n\n",
-                              self.new_setup is False)
-                file.write('{}')
-
-        try:
-            self.settings_json = json.load(
-                open(f'{path_cabinet}/settings.json', encoding="utf8"))
+            # setup
+            self.new_setup = True
 
-        except json.decoder.JSONDecodeError as error:
-            print(f"{error}\n")
+            # make .cabinet directory, if needed
+            expanded_path = os.path.expanduser("~/.cabinet")
+            directory_path = os.path.abspath(expanded_path)
+            directory_path_with_slash = os.path.join(directory_path, '')
+            if not os.path.exists(directory_path_with_slash):
+                os.makedirs(directory_path_with_slash)
 
-            response = input(f"The settings file ({path_cabinet}/settings.json) is not valid JSON. "
-                             "Do you want to replace it with an empty JSON file? "
-                             f"(The existing file will be backed up in {path_cabinet}) (y/n)\n")
+            has_mongodb = input(NEW_SETUP_MSG_INTRO)
 
-            if response.lower().startswith("y"):
-                print("Backing up...")
+            if not has_mongodb.lower().startswith('y'):
+                input(NEW_SETUP_MSG_MONGODB_INSTRUCTIONS)
 
-                # for some reason, this only works when you call touch; TODO fix this
-                os.system(
-                    f"touch {path_cabinet}/settings-backup.json \
-                        && cp {path_cabinet}/settings.json {path_cabinet}/settings-backup.json")
-                print(f"Backed up to {path_cabinet}/settings-backup.json")
-                with open(f'{path_cabinet}/settings.json', 'w+', encoding="utf8") as file:
-                    file.write('{}')
-                print("Done. Please try your last command again.")
+            return config_prompts(key)
+        except KeyError:
+            if self.new_setup:
+                return config_prompts(key)
             else:
                 print(
-                    f"OK. Please fix {path_cabinet}/settings.json and try again.")
-
-            sys.exit(-1)
-
-        path_log = self.get('path', 'log')
-
-        if path_log is None:
-            path_log = self.put(
-                'path', 'log', f"{path_cabinet}/log", file_name='settings.json')
-            print(
-                f"\nCalling cabinet.log in Python (or 'cabinet --log' in the terminal) "
-                f"will write to {path_cabinet}/log by default.\n"
-                f"You can change this in {path_cabinet}/settings.json.\n\n"
-            )
-        if not os.path.exists(path_log):
-            os.makedirs(path_log)
-        if not path_log[-1] == '/':
-            path_log += '/'
-
-        self.path_log = path_log
-        self.new_setup = False
-
-    def _get_config(self, key=None):
-        """
-        Gets a property from the internal configuration file.
-
-        Args:
-        - key (str): The key to search for in the JSON file.
-
-        Returns:
-        - The value of the key in the JSON file.
-
-        If the JSON file does not exist or is not valid JSON,
-            the function provides default behavior:
-        - If `key` is `path_cabinet`, the function prompts
-            the user to enter a directory to store settings.json.
-        - If `key` is not found, the function returns an empty string.
-        - If the file is not valid JSON, the function prompts
-            the user to replace the file with an empty JSON file.
-        """
-
-        try:
-            with open(self.path_config_file, 'r+', encoding="utf8") as file:
-                return json.load(file)[key]
-        except FileNotFoundError:
-            if key == 'path_cabinet':
-                # setup
-                self.new_setup = True
-                path_cabinet = input(self.NEW_SETUP_MSG)
-
-                self._put_config(key, path_cabinet)
-                return path_cabinet
-        except KeyError:
-            print(f"Warning: Key error for key: {key}")
+                    f"Warning: Could not find {key} in {self.path_config_file}")
             return ""
         except json.decoder.JSONDecodeError:
-            response = input(
-                f"The config file ({self.path_config_file}) is not valid JSON.\n"
-                "Do you want to replace it with an empty JSON file? "
-                "(you will lose existing data) (y/n)\n")
+            err_msg = f"Problem reading {self.path_config_file}.\n\n{ERROR_CONFIG_JSON_DECODE}"
+            response = input(err_msg)
+
             if response.lower().startswith("y"):
                 with open(self.path_config_file, 'w+', encoding="utf8") as file:
                     file.write('{}')
-                print("Done. Please try your last command again.")
+                print("Done. Please try again.")
             else:
                 print(f"OK. Please fix {self.path_config_file} and try again.")
 
             sys.exit(-1)
 
     def _put_config(self, key: str = None, value: str = None):
         """
@@ -204,36 +168,14 @@
         Raises:
             FileNotFoundError: If the configuration file cannot be found.
         """
 
         if value == "":
             print("No changes were made.")
             sys.exit(1)
-        else:
-
-            # error correction
-            if key == 'path_cabinet' and value[0] != '/' and value[0] != '~':
-                value = f"/{value}"
-            if key == 'path_cabinet' and value[-1] == '/':
-                value = f"{value[:-1]}"
-
-            # warn about potential problems
-            if not os.path.exists(os.path.expanduser(value)):
-                print(f"Warning: {value} doesn't exist.")
-                create_dir = input(
-                    "Do you want to create the directory? (y/n): ")
-                if create_dir.lower().startswith("y"):
-                    os.makedirs(os.path.expanduser(value))
-                    print("Done.")
-                else:
-                    print("OK, but if you run into problems, "
-                          "run 'cabinet --config' to change to an existing directory.")
-            if value[0] == '~':
-                print("Warning: using tilde expansions may cause problems ",
-                      "if using cabinet for multiple users. It is recommended to use full paths.""")
 
         try:
             with open(self.path_config_file, 'r+', encoding="utf8") as file:
                 config = json.load(file)
         except FileNotFoundError:
             with open(self.path_config_file, 'x+', encoding="utf8") as file:
                 self._ifprint(
@@ -243,104 +185,216 @@
                 config = {}
 
         config[key] = value
 
         with open(self.path_config_file, 'w+', encoding="utf8") as file:
             json.dump(config, file, indent=4)
 
-        print(f"\n\nUpdated configuration file ({self.path_config_file}).")
+        print(f"\nUpdated configuration file ({self.path_config_file}).")
         self._ifprint(f"{key} is now {value}\n", self.new_setup is False)
 
         return value
 
-    def _get_logger(self, log_name: str = None, level: int = logging.INFO,
-                    file_path: str = None, is_quiet: bool = False) -> logging.Logger:
+    def _ifprint(self, message: str, is_print: bool):
+        """
+        Prints the message if `print` is true.
         """
-        A helper function for log()
 
-        Returns a customized logger object with the specified name and level,
-        and optionally logs to a file.
+        # check for valid JSON
+        try:
+            json.loads(message)
+            if is_print:
+                print(json.dumps(message, indent=2))
+        except TypeError:
+            if is_print:
+                print(json.dumps(message, indent=2))
+        except json.JSONDecodeError:
+            if is_print:
+                print(message)
+            return message
+
+    def __init__(self, path_cabinet: str = None):
+        """
+        Initializes the Cabinet instance with the provided or default configuration.
 
         Args:
-        - log_name (str): the name of the logger (defaults to 'root')
-        - level (int): the logging level to use (defaults to logging.INFO)
-        - file_path (str): the path to a file to log to
-            (defaults to None, meaning log only to console)
-        - is_quiet (bool): if True, only logs to file and not to console (defaults to False)
+            path_cabinet (str, optional): The path to the cabinet directory. Defaults to None.
+
+        Notes:
+            - The configuration is read from the `cabinet_config.json` internal file
+            file located in the 'path_cabinet' directory.
+            - If 'path_cabinet' is not provided, the default location
+            is '~/.cabinet'.
+            - The attributes of the Cabinet instance are set based on the configuration values.
 
-        Returns:
-        - logger (Logger): the configured logger object
         """
 
-        today = str(date.today())
+        self.path_cabinet = path_cabinet or os.path.expanduser(
+            self._get_config('path_cabinet'))
 
-        if file_path is None:
-            file_path = f"{self.path_log or self.path_cabinet + '/log/'}{today}"
-        if log_name is None:
-            log_name = f"LOG_DAILY_{today}"
+        # these should match class attributes above
+        keys = ["mongodb_username", "mongodb_password",
+                "mongodb_cluster_name", "mongodb_db_name", "path_cabinet"]
+
+        for key in keys:
+            value = self._get_config(key)
+            setattr(self, key, value)
+
+        if any(getattr(self, key) is None or getattr(self, key) == '' for key in keys):
+            input(ERROR_CONFIG_MISSING_VALUES)
+            self.config()
+            sys.exit(-1)
 
-        # create path if necessary
-        if not os.path.exists(file_path):
-            self._ifprint(f"Creating {file_path}", self.new_setup is True)
-            os.makedirs(file_path)
+        self.new_setup = False
 
-        logger = logging.getLogger(log_name)
+        try:
+            self.uri = (f"mongodb+srv://{self.mongodb_username}:{self.mongodb_password}"
+                        f"@{self.mongodb_cluster_name}.1jxchnk.mongodb.net/"
+                        f"{self.mongodb_db_name}?retryWrites=true&w=majority")
+            self.client = MongoClient(self.uri, server_api=ServerApi('1'))
+            self.database = self.client.cabinet
+        except pymongo.errors.InvalidURI as error:
+            print(ERROR_CONFIG_FILE_INVALID)
+            print(error._message)
 
-        logger.setLevel(level)
+            sys.exit(-1)
 
-        if logger.handlers:
-            logger.handlers = []
+        path_log = self.get('path', 'log') or '~/.cabinet/log'
 
-        format_string = "%(asctime)s — %(levelname)s — %(message)s"
-        log_format = logging.Formatter(format_string)
+        expanded_path = os.path.expanduser(path_log)
+        directory_path = os.path.abspath(expanded_path)
+        directory_path_with_slash = os.path.join(directory_path, '')
+
+        # Create the directory if it doesn't exist
+        if not os.path.exists(directory_path_with_slash):
+            os.makedirs(directory_path_with_slash)
+
+        self.path_log = directory_path_with_slash
+
+    def config(self):
+        """
+        Opens the configuration file for editing using the default editor.
+
+        If the function is called from a terminal, the configuration file is opened with the default
+        editor defined in the 'EDITOR' environment variable.
+        If the 'EDITOR' variable is not set, 'vi'
+        is used as the default editor.
+
+        If the function is called from a non-terminal environment,
+        such as a graphical user interface,
+        the behavior depends on the operating system:
+        - On Windows, the configuration file is opened using
+        the default associated editor for JSON files.
+        - On macOS, the configuration file is opened using
+        the default application associated with JSON files.
+        - On Linux, the configuration file is opened using
+        the default application for opening files with
+        the 'xdg-open' command.
+
+        If none of the above conditions are met, a message is displayed
+        instructing the user to manually
+        edit the configuration file.
 
-        if not is_quiet:
-            console_handler = logging.StreamHandler(sys.stdout)
-            console_handler.setFormatter(log_format)
-            logger.addHandler(console_handler)
-
-        file_handler = logging.FileHandler(
-            f"{file_path}/{log_name}.log", mode='a')
-        file_handler.setFormatter(log_format)
+        Raises:
+            FileNotFoundError:
+                If the default editor or the associated application for opening files is not found.
 
-        logger.addHandler(file_handler)
-        return logger
+        Notes:
+            - The configuration file is defined by the 'path_config_file' attribute of the class.
+            - The function uses the 'subprocess.run' method
+            to execute the necessary command for opening the file.
+            - The 'check=True' argument ensures that an error
+            is raised if the command execution fails.
 
-    def _ifprint(self, message: str, is_print: bool):
         """
-        Prints a string if `print` is true.
-        """
-        if is_print:
-            print(message)
 
-    def configure(self):
+        if os.isatty(sys.stdin.fileno()):
+            # User is in a terminal, open with default editor
+            try:
+                subprocess.run(
+                    [os.environ.get('EDITOR', 'vi'), self.path_config_file], check=True)
+            except FileNotFoundError:
+                print("Default editor not found. Unable to open the file.")
+        else:
+            if sys.platform.startswith('win32'):
+                # Windows
+                subprocess.run(
+                    ['start', '', self.path_config_file], shell=True, check=True)
+            elif sys.platform.startswith('darwin'):
+                # macOS
+                subprocess.run(['open', self.path_config_file], check=True)
+            elif sys.platform.startswith('linux'):
+                # Linux
+                subprocess.run(['xdg-open', self.path_config_file], check=True)
+            else:
+                print(f"Please edit ${self.path_config_file} to configure.")
+
+    def edit_db(self):
         """
-        Configures the Cabinet instance based on command line arguments or user input.
+        Opens the data in self.database.cabinet within a JSON file in Vim.
+        When the file is closed, it replaces the data in this collection in MongoDB.
         """
 
-        message = f"""
-Enter the full path of the directory where you want to store
-all data (currently {self.path_cabinet}):\n"""
+        # Export the data from the collection to a JSON file
+        collection_data = self.database.cabinet.find()
+        json_data = json.dumps(list(collection_data),
+                               indent=4, default=json_util.default)
 
-        self._put_config('path_cabinet', input(message))
+        temp_file_path = "temp_mongodb_cabinet.json"
 
-    def edit(self):
-        """
-        Edits and saves the settings file.
-        """
-        self.edit_file(self.path_settings_file)
+        try:
+            # Write the JSON data to a temporary file
+            with open(temp_file_path, "w", encoding="utf-8") as temp_file:
+                temp_file.write(json_data)
+
+            # Open the temporary file in Vim
+            subprocess.run(["vim", temp_file_path], check=True)
+
+            # Read the modified JSON data from the temporary file
+            with open(temp_file_path, "r", encoding="utf-8") as temp_file:
+                modified_json_data = temp_file.read()
+
+            # Check if any changes were made
+            if modified_json_data == json_data:
+                print("No changes.")
+                return
+
+            # Replace the data in the collection with the modified data
+            modified_data = json.loads(modified_json_data)
+            for document in modified_data:
+                document.pop("_id", None)  # Remove the existing _id field
+                document["_id"] = ObjectId()  # Assign a new ObjectId
+
+            self.database.cabinet.drop()  # Drop the existing collection
+            self.database.cabinet.insert_many(
+                modified_data)  # Insert the modified data
+
+            print("Data in the collection has been updated.")
+
+        except FileNotFoundError:
+            print("Error: Temporary file not found.")
+        except subprocess.CalledProcessError:
+            print("Error: Failed to open the file in Vim.")
+        except json.JSONDecodeError:
+            print("Error: Failed to parse the modified JSON data.")
+        except Exception as error:  # pylint: disable=W0703
+            print(f"Error: {str(error)}")
+
+        finally:
+            # Remove the temporary file
+            subprocess.run(["rm", temp_file_path], check=True,
+                           stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
 
     def edit_file(self, file_path: str = None, create_if_not_exist: bool = True) -> None:
         """
         Edit and save a file in Vim.
 
         Args:
             - file_path (str, optional): The path to the file to edit.
-                Allows for shortcuts by setting paths in settings.json -> path -> edit
-                If unset, edit settings.json
+                Allows for shortcuts by setting paths in MongoDB -> path -> edit
 
             - create_if_not_exist (bool, optional): Whether to create the file if it does not exist.
                 Defaults to False.
 
         Raises:
             - ValueError: If the file_path is not a string.
 
@@ -348,27 +402,29 @@
 
         Returns:
             None
         """
 
         path_edit = self.get("path", "edit")
 
-        # edit settings.json if no file_path
+        # edit MongoDB Directly if no file_path
         if file_path is None:
-            message = (
+            path = input(
                 "Enter the path of the file you want to edit "
-                f"(default: {self.path_cabinet}/settings.json):\n"
+                "(default: edit Cabinet's MongoDB collection):\n"
             )
 
-            path = self.path_settings_file or input(
-                message) or f"{self.path_cabinet}/settings.json"
+            if path == "":
+                self.edit_db()
+                return
+
             self.edit_file(path)
             return
 
-        # allows for shortcuts by setting paths in settings.json -> path -> edit
+        # allows for shortcuts by setting paths in MongoDB -> path -> edit
         if path_edit and file_path in path_edit:
             item = self.get("path", "edit", file_path)
             if not isinstance(item, dict) or "value" not in item.keys():
                 self.log(f"Could not use shortcut for {file_path} \
                     in getItem(path -> edit); should be a JSON object with value", level="warn")
             else:
                 file_path = item["value"]
@@ -389,110 +445,265 @@
 
         with open(file_path, "r", encoding="utf-8") as file:
             new_contents = file.readlines()
 
         if original_contents == new_contents:
             print("No changes.")
 
+    def merge_nested_data(self, existing_data, new_data):
+        """
+        Merge Nested Data
+        """
+        merged_data = {}
+
+        for key, value in existing_data.items():
+            if key in new_data and isinstance(value, dict) and isinstance(new_data[key], dict):
+                merged_data[key] = self.merge_nested_data(value, new_data[key])
+            else:
+                merged_data[key] = value
+
+        for key, value in new_data.items():
+            if key not in merged_data:
+                merged_data[key] = value
+            else:
+                if isinstance(value, dict) and isinstance(merged_data[key], dict):
+                    merged_data[key] = self.merge_nested_data(
+                        merged_data[key], value)
+                else:
+                    merged_data[key] = value
+
+        return merged_data
+
+    def put(self, *attribute, value=None, is_print: bool = False):
+        """
+        Adds or replaces a property
+        """
+
+        def parse_arg(value):
+            """
+            Infer the value type (e.g. 2 will not be parsed as a string)
+            """
+            if value == "null":
+                return None
+            try:
+                return int(value)
+            except ValueError:
+                try:
+                    return float(value)
+                except ValueError:
+                    if value.lower() == 'true':
+                        return True
+                    if value.lower() == 'false':
+                        return False
+                    try:
+                        return ast.literal_eval(value)
+                    except (SyntaxError, ValueError):
+                        return value
+            except TypeError:
+                return value
+
+        custom_filter = {}
+
+        if value is None:  # Check if value argument is None
+            value = parse_arg(attribute[-1])
+
+        cache = value
+        json_structure = {}
+        for item in reversed(attribute[:-1]):
+            try:
+                json_structure = {}
+                json_structure[item] = cache
+                cache = json_structure
+            except TypeError as error:
+                print(error)
+
+        existing_data = self.database.cabinet.find_one({}, {"_id": 0})
+
+        # Merge the new data with the existing data
+        update = {"$set": {}}
+
+        if len(attribute) > 2:
+            update["$set"][attribute[0]] = self.merge_nested_data(existing_data.get(
+                attribute[0], {}), json_structure[attribute[0]])
+        else:
+            update = {"$set": json_structure}
+
+        result = self.database.cabinet.update_many(custom_filter, update)
+
+        if is_print:
+            print(f"Modified {result.modified_count} item(s)")
+            print(
+                f"{' -> '.join(attribute[:-1])} set to {value}\n")
+
+        return value
+
     def get(self, *attributes, warn_missing=False, is_print=False):
         """
-        Returns a property in a JSON file based on the input attributes.
+        Returns a property from MongoDB based on the input attributes.
 
         Args:
-            - attributes (str): the attributes to traverse in the JSON file
+            - attributes (str): the attributes check in MongoDB
             - warn_missing (bool, optional): whether to warn if an attribute is missing
+            - is_print (bool, optional): whether to print the return value
 
         Returns:
-            - The value of the attribute if it exists in the JSON file, otherwise default.
+            - The value of the attribute if it exists in MongoDB, otherwise default.
 
         Usage:
-            - get('person', 'tyler', 'salary') returns person -> tyler -> salary from self.settings
+            - get('person', 'tyler', 'salary') returns person -> tyler -> salary from self.db
         """
 
-        if self.settings_json is None:
-            self._ifprint("None", is_print)
+        collection = self.database.cabinet
+
+        document = collection.find_one(
+            {}, {attribute: 1 for attribute in attributes})
+
+        if document:
+            result = document
+            for attribute in attributes:
+                if attribute in result:
+                    result = result[attribute]
+                else:
+                    if warn_missing:
+                        self.log(
+                            f"Attribute '{attribute}' is missing", level="warn")
+                    return None
+        else:
+            if warn_missing:
+                self.log("No document found in MongoDB", level="warn")
             return None
 
-        settings = self.settings_json
+        if is_print:
+            print(result)
 
-        for index, item in enumerate(attributes):
-            if item in settings:
-                settings = settings[item]
-            elif warn_missing and (len(attributes) < 2 or attributes[1] != "edit"):
-                msg_settings = settings if index > 0 else f'{self.path_cabinet}/settings.json'
-                self._ifprint(
-                    f"Warning: {item} not found in {msg_settings}",
-                    is_print)
-                self._ifprint("None", is_print)
-                return None
-            else:
-                self._ifprint("None", is_print)
-                return None
+        return result
+
+    def remove(self, *attribute, is_print: bool = False):
+        """
+        Removes a property from the data
+        """
+
+        custom_filter = {}
+
+        cache = attribute[-1]
+        json_structure = {}
+        for item in reversed(attribute[:-1]):
+            try:
+                json_structure = {}
+                json_structure[item] = cache
+                cache = json_structure
+            except TypeError as error:
+                print(error)
+
+        if len(attribute) > 1:
+            update = {"$unset": {attribute[0]: json_structure[attribute[0]]}}
+        else:
+            json_structure[attribute[0]] = 1
+            update = {"$unset": json_structure}
+
+        result = self.database.cabinet.update_many(custom_filter, update)
 
-        self._ifprint(settings, is_print)
-        return settings
+        if is_print:
+            print(f"Modified {result.modified_count} item(s)")
+            print(f"{' -> '.join(attribute)} removed\n")
 
-    def put(self, *attribute, value=None, file_name='settings.json', is_print=False):
+    def log(self, message: str = '', log_name: str = None, level: str = None,
+            file_path: str = None, is_quiet: bool = False) -> None:
         """
-        Adds or replaces a property in a JSON file (default name: settings.json).
+        Logs a message using the specified log level
+        and writes it to a file if a file path is provided.
 
         Args:
-            *attribute (str): A series of keys in the JSON object
-                to identify the location of the property.
-            value (optional): The value to put into the property.
-                If not specified, the last argument will be used.
-            file_name (str): The name of the JSON file to put the property in.
-                File must be in the `path_cabinet` folder.
-                Default: 'settings.json'
+            message (str, optional): The message to log. Defaults to ''.
+            log_name (str, optional): The name of the logger to use. Defaults to None.
+            level (str, optional): The log level to use.
+                Must be one of 'debug', 'info', 'warning', 'error', or 'critical'.
+                Defaults to 'info'.
+            file_path (str, optional): The path to the log file.
+                If not provided, logs will be saved to MongoDB -> path -> log.
+                Defaults to None.
+            is_quiet (bool, optional): If True, logging output will be silenced. Defaults to False.
+
+        Raises:
+            ValueError: If an invalid log level is provided.
 
         Returns:
-            The value that was put into the property.
+            None
         """
 
-        path_full = f"{self.path_cabinet}/{file_name}"
+        def _get_logger(log_name: str = None, level: int = logging.INFO,
+                        file_path: str = None, is_quiet: bool = False) -> logging.Logger:
+            """
+            A helper function for log()
+
+            Returns a customized logger object with the specified name and level,
+            and optionally logs to a file.
+
+            Args:
+            - log_name (str): the name of the logger (defaults to 'root')
+            - level (int): the logging level to use (defaults to logging.INFO)
+            - file_path (str): the path to a file to log to
+                (defaults to None, meaning log only to console)
+            - is_quiet (bool): if True, only logs to file and not to console (defaults to False)
+
+            Returns:
+            - logger (Logger): the configured logger object
+            """
 
-        maximum_attribute_index = 0
-        attribute_max_attribute_index = attribute
+            today = str(date.today())
 
-        if not value:
-            value = attribute[-1]
-            maximum_attribute_index = -1
-            attribute_max_attribute_index = attribute[:maximum_attribute_index]
+            if file_path is None:
+                file_path = f"{self.path_log or self.path_cabinet + '/log/'}{today}"
+            if log_name is None:
+                log_name = f"LOG_DAILY_{today}"
 
-        _settings = self.settings_json if file_name == 'settings.json' else json.load(
-            open(path_full, encoding="utf8"))
+            # create path if necessary
+            if not os.path.exists(file_path):
+                self._ifprint(f"Creating {file_path}", self.new_setup is True)
+                os.makedirs(file_path)
 
-        # iterate through entire JSON object and replace 2nd to last attribute with value
+            logger = logging.getLogger(log_name)
 
-        partition = _settings
+            logger.setLevel(level)
 
-        for index, item in enumerate(attribute_max_attribute_index):
-            if item not in partition:
-                try:
-                    partition[item] = value if index == len(
-                        attribute) + maximum_attribute_index - 1 else {}
-                    partition = partition[item]
-                    self.log(
-                        f"Adding new key '{item}' to {partition if index > 0 else path_full}",
-                        is_quiet=self.new_setup)
-                except TypeError as error:
-                    self.log(f"{error}\n\n{attribute[index-1]} is currently a string, so it cannot \
-be treated as an object with multiple properties.", level="error")
-            else:
-                if index == len(attribute) + maximum_attribute_index - 1:
-                    partition[item] = value
-                else:
-                    partition = partition[item]
+            if logger.handlers:
+                logger.handlers = []
 
-        with open(path_full, 'w+', encoding="utf8") as file:
-            json.dump(_settings, file, indent=4)
+            format_string = "%(asctime)s — %(levelname)s — %(message)s"
+            log_format = logging.Formatter(format_string)
 
-        self._ifprint(
-            f"{' -> '.join(attribute[:-1])} set to {value}", is_print)
-        return value
+            if not is_quiet:
+                console_handler = logging.StreamHandler(sys.stdout)
+                console_handler.setFormatter(log_format)
+                logger.addHandler(console_handler)
+
+            file_handler = logging.FileHandler(
+                f"{file_path}/{log_name}.log", mode='a')
+            file_handler.setFormatter(log_format)
+
+            logger.addHandler(file_handler)
+            return logger
+
+        if level is None:
+            level = 'info'
+
+        # validate log level
+        valid_levels = {'debug', 'info', 'warn',
+                        'warning', 'error', 'critical'}
+        if level.lower() not in valid_levels:
+            raise ValueError(
+                f"Invalid log level: {level}. Must be one of {', '.join(valid_levels)}.")
+
+        # get logger instance
+        logger = _get_logger(log_name=log_name, level=level.upper(),
+                             file_path=file_path, is_quiet=is_quiet)
+
+        # Log message
+        if not is_quiet:
+            getattr(logger, level.lower())(message)
 
     def get_file_as_array(self, item: str, file_path=None, strip: bool = True,
                           ignore_not_found: bool = False):
         """
         Reads a file and returns its contents as a list of lines.
         The file is assumed to be encoded in UTF-8.
 
@@ -562,55 +773,48 @@
             if not is_quiet:
                 print(f"Wrote to '{file_path}/{file_name}'")
             return True
         except (OSError, IOError) as error:
             self.log(f"write_file: {error}", level="error")
             return False
 
-    def log(self, message: str = '', log_name: str = None, level: str = None,
-            file_path: str = None, is_quiet: bool = False) -> None:
+    def ping(self, is_print: bool = False):
         """
-        Logs a message using the specified log level
-        and writes it to a file if a file path is provided.
-
-        Args:
-            message (str, optional): The message to log. Defaults to ''.
-            log_name (str, optional): The name of the logger to use. Defaults to None.
-            level (str, optional): The log level to use.
-                Must be one of 'debug', 'info', 'warning', 'error', or 'critical'.
-                Defaults to 'info'.
-            file_path (str, optional): The path to the log file.
-                If not provided, logs will be saved to settings.json -> path -> log.
-                Defaults to None.
-            is_quiet (bool, optional): If True, logging output will be silenced. Defaults to False.
-
-        Raises:
-            ValueError: If an invalid log level is provided.
+        Send a ping to verify successful connection
+        """
+        try:
+            self.client.admin.command('ping')
+            self._ifprint("Ping Successful", is_print)
+            return True
+        except Exception as error:  # pylint: disable=W0703
+            print(error)
+            return False
 
-        Returns:
-            None
+    def export(self):
+        """
+        Exports all data to JSON
         """
+        data = self.database.cabinet.find_one({}, {"_id": 0})
+        json_data = json.dumps(data, indent=4)
 
-        if level is None:
-            level = 'info'
+        path_export = '~/.cabinet/export'
+        expanded_path = os.path.expanduser(path_export)
+        directory_path = os.path.abspath(expanded_path)
+        directory_path_with_slash = os.path.join(directory_path, '')
 
-        # validate log level
-        valid_levels = {'debug', 'info', 'warn',
-                        'warning', 'error', 'critical'}
-        if level.lower() not in valid_levels:
-            raise ValueError(
-                f"Invalid log level: {level}. Must be one of {', '.join(valid_levels)}.")
+        # Create the directory if it doesn't exist
+        if not os.path.exists(directory_path_with_slash):
+            os.makedirs(directory_path_with_slash)
 
-        # get logger instance
-        logger = self._get_logger(log_name=log_name, level=level.upper(),
-                                  file_path=file_path, is_quiet=is_quiet)
+        current_datetime = datetime.now()
+        formatted_datetime = current_datetime.strftime("%Y-%m-%d %H:%M:%S")
+        file_name = f"cabinet export {formatted_datetime}"
 
-        # Log message
-        if not is_quiet:
-            getattr(logger, level.lower())(message)
+        with open(file_name, 'w', encoding='utf-8') as file:
+            file.write(json_data)
 
 
 def main():
     """
     Main function for running Cabinet.
 
     Args:
@@ -618,39 +822,57 @@
 
     Returns:
         None
 
     Usage:
         (from the terminal)
         cabinet config
-        cabinet edit <file path/name, optional; default: settings.json>
+        cabinet edit <file path/name, optional; default: edit entire MongoDB>
     """
 
     cab = Cabinet()
     package_name = sys.modules[__name__].__package__.split('.')[0]
     version = importlib.metadata.version(package_name)
 
+    class ValidatePutArgs(argparse.Action):
+        """
+        Custom argparse action to validate the number of arguments for the --put option.
+        Ensures that a minimum of 2 arguments are provided.
+        """
+
+        def __call__(self, parser, namespace, values, option_string=None):
+            if len(values) < 2:
+                if len(values) == 1 and values[0] == 'ut':
+                    print("I think you meant to use '--put' or '-p'.\n")
+                parser.error(
+                    f"At least 2 arguments are required for {option_string}")
+            setattr(namespace, self.dest, values)
+
     parser = argparse.ArgumentParser(
         description=f"Cabinet ({version})")
 
     parser.add_argument('--configure', '-config', dest='configure',
                         action='store_true', help='Configure')
     parser.add_argument('--edit', '-e', dest='edit', action='store_true',
-                        help='Edit the settings.json file')
+                        help='Edit the entire MongoDB')
     parser.add_argument('--edit-file', '-ef', type=str, dest='edit_file',
                         help='Edit a specific file')
     parser.add_argument('--no-create', dest='create',
                         action='store_false',
                         help='(for -ef) Do not create file if it does not exist')
     parser.add_argument('--get', '-g', dest='get', nargs='+',
-                        help='Get a property from settings.json')
-    parser.add_argument('--put', '-p', dest='put', nargs='+',
-                        help='Put a property into settings.json')
+                        help='Get a property from MongoDB')
+    parser.add_argument('--put', '-p', dest='put', nargs='+', action=ValidatePutArgs,
+                        help='Put a property into MongoDB')
+    parser.add_argument('--remove', '-rm', dest='remove',
+                        nargs='+', help='Remove a property from MongoDB')
     parser.add_argument('--get-file', dest='get_file',
                         type=str, help='Get file')
+    parser.add_argument('--export', dest='export', action='store_true',
+                        help='Exports MongoDB to ~/.cabinet/export')
     parser.add_argument('--strip', dest='strip', action='store_false',
                         help='(for --get-file) Whether to strip file content whitespace')
     parser.add_argument('--log', '-l', type=str,
                         dest='log', help='Log a message to the default location')
     parser.add_argument('--level', type=str, dest='log_level',
                         help='(for -l) Log level [debug, info, warn, error, critical]')
 
@@ -666,30 +888,35 @@
 
     parser.add_argument('-v', '--version',
                         action='version', help='Show version number and exit', version=version)
 
     args = parser.parse_args()
 
     if args.configure:
-        cab.configure()
+        cab.config()
     elif args.edit:
-        cab.edit()
+        cab.edit_db()
     elif args.edit_file:
         cab.edit_file(file_path=args.edit_file,
                       create_if_not_exist=args.create)
     elif args.get:
-        cab.get(is_print=True, *args.get)
+        cab.get(is_print=True, warn_missing=True, *args.get)
     elif args.put:
         attribute_values = args.put
         cab.put(*attribute_values, is_print=True)
+    elif args.remove:
+        attribute_values = args.remove
+        cab.remove(*attribute_values, is_print=True)
     elif args.get_file:
         cab.get_file_as_array(item=args.get_file,
                               file_path=None, strip=args.strip)
     elif args.log:
         cab.log(message=args.log, level=args.log_level)
+    elif args.export:
+        cab.export()
     elif args.mail:
         to_addr = None
         if args.to_addr:
             to_addr = ''.join(args.to_addr).split(',')
         Mail().send(args.subject, args.body, to_addr=to_addr)
```

### Comparing `cabinet-2023.6.8.1/src/cabinet/mail.py` & `cabinet-2023.7.2.1/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2023.6.8.1/src/cabinet.egg-info/PKG-INFO` & `cabinet-2023.7.2.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,93 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.6.8.1
+Version: 2023.7.2.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cabinet
-A Python library to easily store data across multiple projects in one or more JSON files.
+A Python library to easily manage data with MongoDB and across other files.
 
 Supports a cli, email, and event logging.
 
+## MongoDB Update! - 2023-06-25
+- In this latest release, the tool has been redesigned from the ground up to use MongoDB.
+- MongoDB elevates Cabinet to the best of both worlds: a secure database with the ability to edit 
+  as if it were a JSON structure.
+- Every function has been tested for compatibility with earlier releases, but it's likely
+  there will be some edge case bugs to iron out. I use this tool extremely often in my day-to-day
+  use, so these should be patched quickly, once discovered. Please report issues as you find them.
+
 ## Features
 
-- Read and write data in the JSON files of your choice
+- Read and write data in MongoDB and/or the JSON files of your choice
+- Provides easy shortcuts to MongoDB actions
 - Log to a file/directory of your choice without having to configure `logger` each time
 - Send/receive mail using `cabinet.Cabinet().mail()`
 
+## Dependencies
+
+- Python >= 3.6
+- MongoDB
+- Pymongo (`pip install pymongo`)
+- smtplib
+
 ## Structure
 
-- Data is stored in a `settings.json` file in the location of your choice
-- Logs are written to `{/path/to/cabinet}/log/LOG_DAILY_YYYY-MM-DD` by default
-  - this can be changed on a per-log basis
+- Data is stored in MongoDB; simply plug in your credentials.
+- Logs are written to `~/.cabinet/log/LOG_DAILY_YYYY-MM-DD` by default
+  - this can be changed as needed (per log or otherwise)
 
 ## Installation and Setup
 
 ```bash
   python3 -m pip install cabinet
-
+  python3 -m pip install pymongo
   cabinet --config
 ```
 
 ## CLI usage
 ```
 Usage: cabinet [OPTIONS]
 
 Options:
   -h, --help              Show this help message and exit
   --configure, -config    Configure
-  --edit, -e              Edit the settings.json file
+  --export                Export the data in MongoDB to a JSON file
+  --edit, -e              Edit MongoDB in the default editor as a JSON file
   --edit-file, -ef        Edit a specific file
   --no-create             (for -ef) Do not create file if it does not exist
-  --get, -g [GET ...]     Get a property from settings.json
-  --put PUT [PUT ...]     Put a property into settings.json
-  --get-file GET_FILE     Get file
+  --get, -g               Get a property from MongoDB (nesting supported)
+  --put, -p               Put a property into MongoDB (nesting supported)
+  --remove, -rm           Removes a property from MongoDB
+  --get-file              Returns the file specified
   --strip                 (for --get-file) Whether to strip file content whitespace
   --log, -l               Log a message to the default location
-  --level LOG_LEVEL       (for -l) Log level [debug, info, warn, error, critical]
+  --level                 (for -l) Log level [debug, info, warn, error, critical]
   -v, --version           show version number and exit
 
 Mail:
   --mail                Sends an email
   --subject SUBJECT, -s SUBJECT
                         Email subject
   --body BODY, -b BODY  Email body
   --to TO_ADDR, -t TO_ADDR
 ```
 
 ## Configuration
 
-- Upon first launch, will prompt you to choose a location for `settings.json`. You can change this at any time with `cabinet --config`.
+- Upon first launch, the tool will prompt you to enter your MongoDB credentials, as well as
+  the cluster name and Database name. These are stored only within the package, as a file named
+  `cabinet_config.json`.
 
 ### edit_file() shortcuts
 - see example below to enable something like
   - `cabinet -ef shopping` from the terminal
     - rather than `cabinet -ef "/home/{username}/path/to/shopping_list.md"`
   - or `cabinet.Cabinet().edit("shopping")`
     - rather than `cabinet.Cabinet().edit("/home/{username}/path/to/whatever.md")`
@@ -96,15 +116,15 @@
 cabinet -p edit todo value "/home/{username}/path/to/whatever.md"
 ```
 
 ### mail
 
 - It is NEVER a good idea to store your password in plaintext; for this reason, I strongly recommend a "throwaway" account that is only used for sending emails
 - Gmail (as of May 2022) and most other mainstream email providers won't work with this; for support, search for sending mail from your email provider with `smtplib`.
-- In `settings.json`, add the `email` object to make your settings file look like this example:
+- In MongoDB, add the `email` object to make your settings file look like this example:
 
 file:
 ```
 {
     "email": {
         "from": "throwaway@example.com",
         "from_pw": "example",
@@ -135,19 +155,18 @@
 cab = Cabinet()
 
 cab.put("employee", "Tyler", "salary", 7.25)
 ```
 
 or terminal:
 ```
-# warning - from the terminal, numeric values in cabinet are stored as strings
-cabinet -p employer Tyler salary 7.25
+cabinet -p employee Tyler salary 7.25
 ```
 
-results in this structure in settings.json:
+results in this structure in MongoDB:
 ```
 {
     "employee": {
         "Tyler": {
             "salary": 7.25 # or "7.25" if done from terminal
         }
     }
@@ -171,14 +190,39 @@
 ```
 
 results in:
 ```
 7.25
 ```
 
+### `remove`
+
+python:
+```
+from cabinet import Cabinet
+
+cab = Cabinet()
+
+cab.remove("employee", "Tyler", "salary")
+```
+
+or terminal:
+```
+cabinet -rm employee Tyler salary
+```
+
+results in this structure in MongoDB:
+```
+{
+    "employee": {
+        "tyler": {}
+    }
+}
+```
+
 ### `edit_file`
 
 python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
@@ -237,19 +281,19 @@
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cab.log("30", logName="LOG_TEMPERATURE")
+cab.log("30", log_name="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
+cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
@@ -260,19 +304,14 @@
 # -l and --log are interchangeable
 cab --log "Connection timed out"
 
 # change levels with --level
 cab --log "Server is on fire" --level "critical"
 ```
 
-## Dependencies
-
-- Python >= 3.6
-- smtplib
-
 ## Disclaimers
 
 - Although I've done quite a bit of testing, I can't guarantee everything that works on my machine will work on yours. Always back up your data to multiple places to avoid data loss.
 - If you find any issues, please contact me... or get your hands dirty and raise a PR!
 
 ## Unit Tests
 - Unit tests are available in `test/`; use `pytest test/` to run them.
```

### Comparing `cabinet-2023.6.8.1/test/test___init__.py` & `cabinet-2023.7.2.1/test/test___init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 def test_cabinet_initialization_with_custom_path_cabinet():
     """
     tests custom path
     """
     custom_path_cabinet = '~/pytest/path/to/custom/cabinet'
     cab = Cabinet(path_cabinet=custom_path_cabinet)
     assert cab.path_cabinet == custom_path_cabinet
-    assert str(
-        cab.path_settings_file) == f"{custom_path_cabinet}/settings.json"
+    # assert str(
+    #     cab.path_settings_file) == f"{custom_path_cabinet}/settings.json"
     assert cab.path_log == f"{custom_path_cabinet}/log/"
 
 def test_get_config_non_existing_key():
     """
     Test getting a non-existing key from the config file
     """
     cab = Cabinet()
@@ -196,15 +196,15 @@
         "name": "example",
         "value": 42
     }
     with open(f"{cab.path_cabinet}/{file_name}", "w", encoding="utf8") as file:
         json.dump(custom_file_json, file)
 
     # Perform the put operation
-    cab.put("name", value=value, file_name=file_name)
+    # cab.put("name", value=value, file_name=file_name)
 
     # Read the modified JSON file
     with open(f"{cab.path_cabinet}/{file_name}", "r", encoding="utf8") as file:
         modified_json = json.load(file)
 
     # Assert the attribute value has been updated
     assert modified_json["name"] == value
```

