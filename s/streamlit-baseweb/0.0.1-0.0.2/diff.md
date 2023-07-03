# Comparing `tmp/streamlit_baseweb-0.0.1.tar.gz` & `tmp/streamlit_baseweb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_baseweb-0.0.1.tar", last modified: Mon Jul  3 17:28:16 2023, max compression
+gzip compressed data, was "streamlit_baseweb-0.0.2.tar", last modified: Mon Jul  3 17:42:48 2023, max compression
```

## Comparing `streamlit_baseweb-0.0.1.tar` & `streamlit_baseweb-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 17:28:16.724638 streamlit_baseweb-0.0.1/
--rw-rw-rw-   0        0        0     1076 2023-07-03 17:27:05.000000 streamlit_baseweb-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       42 2023-07-03 17:26:06.000000 streamlit_baseweb-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3885 2023-07-03 17:28:16.723636 streamlit_baseweb-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1979 2023-07-03 17:27:21.000000 streamlit_baseweb-0.0.1/README.md
--rw-rw-rw-   0        0        0      892 2023-07-03 17:19:07.000000 streamlit_baseweb-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 17:28:16.724638 streamlit_baseweb-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-07-03 17:18:42.000000 streamlit_baseweb-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:28:16.708069 streamlit_baseweb-0.0.1/streamlit_baseweb/
--rw-rw-rw-   0        0        0     2226 2023-07-03 16:16:42.000000 streamlit_baseweb-0.0.1/streamlit_baseweb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:28:16.722401 streamlit_baseweb-0.0.1/streamlit_baseweb.egg-info/
--rw-rw-rw-   0        0        0     3885 2023-07-03 17:28:16.000000 streamlit_baseweb-0.0.1/streamlit_baseweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-07-03 17:28:16.000000 streamlit_baseweb-0.0.1/streamlit_baseweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 17:28:16.000000 streamlit_baseweb-0.0.1/streamlit_baseweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-03 17:28:16.000000 streamlit_baseweb-0.0.1/streamlit_baseweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2023-07-03 17:28:16.000000 streamlit_baseweb-0.0.1/streamlit_baseweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-03 17:28:16.000000 streamlit_baseweb-0.0.1/streamlit_baseweb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 17:42:48.054383 streamlit_baseweb-0.0.2/
+-rw-rw-rw-   0        0        0     1076 2023-07-03 17:27:05.000000 streamlit_baseweb-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       44 2023-07-03 17:33:16.000000 streamlit_baseweb-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3871 2023-07-03 17:42:48.052454 streamlit_baseweb-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1965 2023-07-03 17:37:38.000000 streamlit_baseweb-0.0.2/README.md
+-rw-rw-rw-   0        0        0      892 2023-07-03 17:41:14.000000 streamlit_baseweb-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 17:42:48.054383 streamlit_baseweb-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-07-03 17:41:09.000000 streamlit_baseweb-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:42:48.042592 streamlit_baseweb-0.0.2/streamlit_baseweb/
+-rw-rw-rw-   0        0        0     2225 2023-07-03 17:37:38.000000 streamlit_baseweb-0.0.2/streamlit_baseweb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:42:48.051489 streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/
+-rw-rw-rw-   0        0        0     3871 2023-07-03 17:42:48.000000 streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-07-03 17:42:48.000000 streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 17:42:48.000000 streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-03 17:42:48.000000 streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2023-07-03 17:42:48.000000 streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-03 17:42:48.000000 streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/top_level.txt
```

### Comparing `streamlit_baseweb-0.0.1/LICENSE` & `streamlit_baseweb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_baseweb-0.0.1/PKG-INFO` & `streamlit_baseweb-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_baseweb
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Streamlit implementation of the Base Web library.
 Home-page: https://github.com/thomasbs17/streamlit-contributions/baseweb_components
 Author: Thomas Bouamoud
 Author-email: Thomas Bouamoud <thomas.bouamoud@gmail.com>
 License: Copyright (c) 2023 Thomas Bouamoud
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -51,15 +51,15 @@
 
 ```python
 import streamlit as st
 from streamlit_baseweb import base_web_modal
 
 st.title("Testing Streamlit Baseweb")
 if st.button(label="open modal"):
-    base_web_modal(title="modal", body="testing modal", is_open=True, key="base_web_modal")
+    base_web_modal(title="modal", body="testing modal", key="base_web_modal")
 
 ```
 
 For more details on available components and their usage, refer to the package documentation.
 
 ## Contributing
 Contributions to Streamlit Baseweb are welcome! If you find any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/thomasbs17/streamlit-contributions/tree/master/baseweb_components). If you'd like to contribute code, you can fork the repository, make your changes, and submit a pull request.
```

### Comparing `streamlit_baseweb-0.0.1/README.md` & `streamlit_baseweb-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ```python
 import streamlit as st
 from streamlit_baseweb import base_web_modal
 
 st.title("Testing Streamlit Baseweb")
 if st.button(label="open modal"):
-    base_web_modal(title="modal", body="testing modal", is_open=True, key="base_web_modal")
+    base_web_modal(title="modal", body="testing modal", key="base_web_modal")
 
 ```
 
 For more details on available components and their usage, refer to the package documentation.
 
 ## Contributing
 Contributions to Streamlit Baseweb are welcome! If you find any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/thomasbs17/streamlit-contributions/tree/master/baseweb_components). If you'd like to contribute code, you can fork the repository, make your changes, and submit a pull request.
```

### Comparing `streamlit_baseweb-0.0.1/pyproject.toml` & `streamlit_baseweb-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit_baseweb"
-version = "0.0.1"
+version = "0.0.2"
 description = "A Streamlit implementation of the Base Web library."
 readme = "README.md"
 authors = [{ name = "Thomas Bouamoud", email = "thomas.bouamoud@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `streamlit_baseweb-0.0.1/setup.py` & `streamlit_baseweb-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_baseweb",
-    version="0.0.1",
+    version="0.0.2",
     author="Thomas Bouamoud",
     author_email="thomas.bouamoud@gmail.com",
     description="A Streamlit implementation of the Base Web library.",
     long_description="https://baseweb.design/",
     long_description_content_type="text/plain",
     url="https://github.com/thomasbs17/streamlit-contributions/baseweb_components",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_baseweb-0.0.1/streamlit_baseweb/__init__.py` & `streamlit_baseweb-0.0.2/streamlit_baseweb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from typing import Literal
 
 import streamlit as st
 import streamlit.components.v1 as components
 
-_RELEASE = False
+_RELEASE = True
 
 __title__ = "Baseweb UI"
 __author__ = "Thomas Bouamoud"
 
 if not _RELEASE:
     _base_web_modal = components.declare_component(
         "base_web_modal", url="http://localhost:3000",
```

### Comparing `streamlit_baseweb-0.0.1/streamlit_baseweb.egg-info/PKG-INFO` & `streamlit_baseweb-0.0.2/streamlit_baseweb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-baseweb
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Streamlit implementation of the Base Web library.
 Home-page: https://github.com/thomasbs17/streamlit-contributions/baseweb_components
 Author: Thomas Bouamoud
 Author-email: Thomas Bouamoud <thomas.bouamoud@gmail.com>
 License: Copyright (c) 2023 Thomas Bouamoud
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -51,15 +51,15 @@
 
 ```python
 import streamlit as st
 from streamlit_baseweb import base_web_modal
 
 st.title("Testing Streamlit Baseweb")
 if st.button(label="open modal"):
-    base_web_modal(title="modal", body="testing modal", is_open=True, key="base_web_modal")
+    base_web_modal(title="modal", body="testing modal", key="base_web_modal")
 
 ```
 
 For more details on available components and their usage, refer to the package documentation.
 
 ## Contributing
 Contributions to Streamlit Baseweb are welcome! If you find any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/thomasbs17/streamlit-contributions/tree/master/baseweb_components). If you'd like to contribute code, you can fork the repository, make your changes, and submit a pull request.
```

