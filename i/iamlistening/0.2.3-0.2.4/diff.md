# Comparing `tmp/iamlistening-0.2.3.tar.gz` & `tmp/iamlistening-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-0.2.3.tar", max compression
+gzip compressed data, was "iamlistening-0.2.4.tar", max compression
```

## Comparing `iamlistening-0.2.3.tar` & `iamlistening-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-26 19:13:45.407692 iamlistening-0.2.3/LICENSE
--rw-r--r--   0        0        0     1857 2023-06-26 19:13:45.407692 iamlistening-0.2.3/README.md
--rw-r--r--   0        0        0       99 2023-06-26 19:13:46.099709 iamlistening-0.2.3/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-06-26 19:13:45.407692 iamlistening-0.2.3/iamlistening/config.py
--rw-r--r--   0        0        0      868 2023-06-26 19:13:45.407692 iamlistening-0.2.3/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     3839 2023-06-26 19:13:45.407692 iamlistening-0.2.3/iamlistening/main.py
--rw-r--r--   0        0        0     2163 2023-06-26 19:13:46.099709 iamlistening-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 iamlistening-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-03 12:56:47.972866 iamlistening-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1857 2023-07-03 12:56:47.972866 iamlistening-0.2.4/README.md
+-rw-r--r--   0        0        0       99 2023-07-03 12:56:48.948867 iamlistening-0.2.4/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-03 12:56:47.972866 iamlistening-0.2.4/iamlistening/config.py
+-rw-r--r--   0        0        0      805 2023-07-03 12:56:47.972866 iamlistening-0.2.4/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     3839 2023-07-03 12:56:47.972866 iamlistening-0.2.4/iamlistening/main.py
+-rw-r--r--   0        0        0     2163 2023-07-03 12:56:48.948867 iamlistening-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 iamlistening-0.2.4/PKG-INFO
```

### Comparing `iamlistening-0.2.3/LICENSE` & `iamlistening-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.3/README.md` & `iamlistening-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.3/iamlistening/config.py` & `iamlistening-0.2.4/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.3/iamlistening/default_settings.toml` & `iamlistening-0.2.4/iamlistening/default_settings.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-###############################################################################
-###                           DEFAULT SETTINGS                              ###
-###############################################################################
+#########################################################
+###                  DEFAULT SETTINGS                 ###
+#########################################################
 # Any of those settings can be overwritten by the user.
 # To overwrite a setting, create a settings.toml
-# or load the settings from .env file.
+# or load the settings from .env file or vars.
 # As an example, to disable the iamlistening object:
 # settings.toml
 # [default]
 # iamlistening_enabled = false
 
 [default]
-
 iamlistening_enabled = true
 bot_token = ""
 bot_channel_id = ""
 telethon_api_id = ""
 telethon_api_hash = ""
 matrix_hostname = ""
 matrix_user = ""
 matrix_pass = ""
 
 
-
-
-
 [testing]
-
 VALUE = "On Testing"
 iamlistening_enabled = true
 bot_token = ""
 bot_channel_id = ""
 telethon_api_id = ""
 telethon_api_hash = ""
 matrix_hostname = ""
```

### Comparing `iamlistening-0.2.3/iamlistening/main.py` & `iamlistening-0.2.4/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.3/pyproject.toml` & `iamlistening-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamlistening"
-version = "0.2.3"
+version = "0.2.4"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
```

### Comparing `iamlistening-0.2.3/PKG-INFO` & `iamlistening-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 0.2.3
+Version: 0.2.4
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

