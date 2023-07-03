# Comparing `tmp/read-and-chat-0.0.0.tar.gz` & `tmp/read-and-chat-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read-and-chat-0.0.0.tar", last modified: Mon Jul  3 21:03:21 2023, max compression
+gzip compressed data, was "read-and-chat-0.0.1.tar", last modified: Mon Jul  3 21:05:14 2023, max compression
```

## Comparing `read-and-chat-0.0.0.tar` & `read-and-chat-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jth30      (501) staff       (20)        0 2023-07-03 21:03:21.756551 read-and-chat-0.0.0/
--rw-r--r--   0 jth30      (501) staff       (20)     1070 2023-07-03 19:42:15.000000 read-and-chat-0.0.0/LICENSE
--rw-r--r--   0 jth30      (501) staff       (20)     2422 2023-07-03 21:03:21.756415 read-and-chat-0.0.0/PKG-INFO
--rw-r--r--   0 jth30      (501) staff       (20)      707 2023-07-03 21:02:41.000000 read-and-chat-0.0.0/README.md
--rw-r--r--   0 jth30      (501) staff       (20)      729 2023-07-03 21:00:36.000000 read-and-chat-0.0.0/pyproject.toml
-drwxr-xr-x   0 jth30      (501) staff       (20)        0 2023-07-03 21:03:21.755451 read-and-chat-0.0.0/read_and_chat/
--rw-r--r--   0 jth30      (501) staff       (20)      126 2023-07-03 20:35:16.000000 read-and-chat-0.0.0/read_and_chat/__init__.py
--rw-r--r--   0 jth30      (501) staff       (20)      193 2023-07-03 20:07:12.000000 read-and-chat-0.0.0/read_and_chat/main.py
--rw-r--r--   0 jth30      (501) staff       (20)      243 2023-07-03 20:40:08.000000 read-and-chat-0.0.0/read_and_chat/main_cli.py
-drwxr-xr-x   0 jth30      (501) staff       (20)        0 2023-07-03 21:03:21.756212 read-and-chat-0.0.0/read_and_chat.egg-info/
--rw-r--r--   0 jth30      (501) staff       (20)     2422 2023-07-03 21:03:21.000000 read-and-chat-0.0.0/read_and_chat.egg-info/PKG-INFO
--rw-r--r--   0 jth30      (501) staff       (20)      303 2023-07-03 21:03:21.000000 read-and-chat-0.0.0/read_and_chat.egg-info/SOURCES.txt
--rw-r--r--   0 jth30      (501) staff       (20)        1 2023-07-03 21:03:21.000000 read-and-chat-0.0.0/read_and_chat.egg-info/dependency_links.txt
--rw-r--r--   0 jth30      (501) staff       (20)       57 2023-07-03 21:03:21.000000 read-and-chat-0.0.0/read_and_chat.egg-info/entry_points.txt
--rw-r--r--   0 jth30      (501) staff       (20)       14 2023-07-03 21:03:21.000000 read-and-chat-0.0.0/read_and_chat.egg-info/top_level.txt
--rw-r--r--   0 jth30      (501) staff       (20)       38 2023-07-03 21:03:21.756597 read-and-chat-0.0.0/setup.cfg
--rw-r--r--   0 jth30      (501) staff       (20)       38 2023-07-03 20:22:47.000000 read-and-chat-0.0.0/setup.py
+drwxr-xr-x   0 jth30      (501) staff       (20)        0 2023-07-03 21:05:14.602034 read-and-chat-0.0.1/
+-rw-r--r--   0 jth30      (501) staff       (20)     1056 2023-07-03 21:05:00.000000 read-and-chat-0.0.1/LICENSE
+-rw-r--r--   0 jth30      (501) staff       (20)     2437 2023-07-03 21:05:14.601904 read-and-chat-0.0.1/PKG-INFO
+-rw-r--r--   0 jth30      (501) staff       (20)      736 2023-07-03 21:03:42.000000 read-and-chat-0.0.1/README.md
+-rw-r--r--   0 jth30      (501) staff       (20)      729 2023-07-03 21:05:07.000000 read-and-chat-0.0.1/pyproject.toml
+drwxr-xr-x   0 jth30      (501) staff       (20)        0 2023-07-03 21:05:14.601113 read-and-chat-0.0.1/read_and_chat/
+-rw-r--r--   0 jth30      (501) staff       (20)      126 2023-07-03 20:35:16.000000 read-and-chat-0.0.1/read_and_chat/__init__.py
+-rw-r--r--   0 jth30      (501) staff       (20)      193 2023-07-03 20:07:12.000000 read-and-chat-0.0.1/read_and_chat/main.py
+-rw-r--r--   0 jth30      (501) staff       (20)      243 2023-07-03 20:40:08.000000 read-and-chat-0.0.1/read_and_chat/main_cli.py
+drwxr-xr-x   0 jth30      (501) staff       (20)        0 2023-07-03 21:05:14.601753 read-and-chat-0.0.1/read_and_chat.egg-info/
+-rw-r--r--   0 jth30      (501) staff       (20)     2437 2023-07-03 21:05:14.000000 read-and-chat-0.0.1/read_and_chat.egg-info/PKG-INFO
+-rw-r--r--   0 jth30      (501) staff       (20)      303 2023-07-03 21:05:14.000000 read-and-chat-0.0.1/read_and_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 jth30      (501) staff       (20)        1 2023-07-03 21:05:14.000000 read-and-chat-0.0.1/read_and_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 jth30      (501) staff       (20)       57 2023-07-03 21:05:14.000000 read-and-chat-0.0.1/read_and_chat.egg-info/entry_points.txt
+-rw-r--r--   0 jth30      (501) staff       (20)       14 2023-07-03 21:05:14.000000 read-and-chat-0.0.1/read_and_chat.egg-info/top_level.txt
+-rw-r--r--   0 jth30      (501) staff       (20)       38 2023-07-03 21:05:14.602077 read-and-chat-0.0.1/setup.cfg
+-rw-r--r--   0 jth30      (501) staff       (20)       38 2023-07-03 20:22:47.000000 read-and-chat-0.0.1/setup.py
```

### Comparing `read-and-chat-0.0.0/LICENSE` & `read-and-chat-0.0.1/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 hssrobotics23
+Copyright (c) 2023
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `read-and-chat-0.0.0/PKG-INFO` & `read-and-chat-0.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: read-and-chat
-Version: 0.0.0
+Version: 0.0.1
 Summary: Using text recognition for a ChatGPT prompt
 Author: Timothy Niko, John Hoffer, Kevin Hill, Tyler Malka
 Maintainer-email: John Hoffer <john@hoff.in>
 License: MIT License
         
-        Copyright (c) 2023 hssrobotics23
+        Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -65,11 +65,12 @@
 python3 -m build --sdist
 python3 -m build --wheel
 ```
 
 To publish to pypi [with credentials][creds] in your `.pypirc`, run:
 
 ```
+python3 -m pip install twine
 python3 -m twine upload dist/*
 ```
 
 [creds]: https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#id71
```

### Comparing `read-and-chat-0.0.0/README.md` & `read-and-chat-0.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -30,11 +30,12 @@
 python3 -m build --sdist
 python3 -m build --wheel
 ```
 
 To publish to pypi [with credentials][creds] in your `.pypirc`, run:
 
 ```
+python3 -m pip install twine
 python3 -m twine upload dist/*
 ```
 
 [creds]: https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#id71
```

### Comparing `read-and-chat-0.0.0/pyproject.toml` & `read-and-chat-0.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "read-and-chat"
-version = "0.0.0"
+version = "0.0.1"
 description = "Using text recognition for a ChatGPT prompt"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = []
 authors = [
   {name = "Timothy Niko"},
```

### Comparing `read-and-chat-0.0.0/read_and_chat.egg-info/PKG-INFO` & `read-and-chat-0.0.1/read_and_chat.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: read-and-chat
-Version: 0.0.0
+Version: 0.0.1
 Summary: Using text recognition for a ChatGPT prompt
 Author: Timothy Niko, John Hoffer, Kevin Hill, Tyler Malka
 Maintainer-email: John Hoffer <john@hoff.in>
 License: MIT License
         
-        Copyright (c) 2023 hssrobotics23
+        Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -65,11 +65,12 @@
 python3 -m build --sdist
 python3 -m build --wheel
 ```
 
 To publish to pypi [with credentials][creds] in your `.pypirc`, run:
 
 ```
+python3 -m pip install twine
 python3 -m twine upload dist/*
 ```
 
 [creds]: https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/#id71
```

