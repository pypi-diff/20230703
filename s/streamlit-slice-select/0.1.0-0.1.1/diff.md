# Comparing `tmp/streamlit_slice_select-0.1.0.tar.gz` & `tmp/streamlit_slice_select-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_slice_select-0.1.0.tar", last modified: Sun Jul  2 23:31:51 2023, max compression
+gzip compressed data, was "streamlit_slice_select-0.1.1.tar", last modified: Mon Jul  3 13:29:16 2023, max compression
```

## Comparing `streamlit_slice_select-0.1.0.tar` & `streamlit_slice_select-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jailop    (1000) jailop    (1000)        0 2023-07-02 23:31:51.996760 streamlit_slice_select-0.1.0/
--rw-r--r--   0 jailop    (1000) jailop    (1000)    11357 2023-07-02 22:46:33.000000 streamlit_slice_select-0.1.0/LICENSE.txt
--rw-r--r--   0 jailop    (1000) jailop    (1000)    13199 2023-07-02 23:31:51.996760 streamlit_slice_select-0.1.0/PKG-INFO
--rw-r--r--   0 jailop    (1000) jailop    (1000)       60 2023-07-02 22:12:17.000000 streamlit_slice_select-0.1.0/README.md
--rw-r--r--   0 jailop    (1000) jailop    (1000)      490 2023-07-02 23:31:28.000000 streamlit_slice_select-0.1.0/pyproject.toml
--rw-r--r--   0 jailop    (1000) jailop    (1000)       38 2023-07-02 23:31:51.996760 streamlit_slice_select-0.1.0/setup.cfg
-drwxr-xr-x   0 jailop    (1000) jailop    (1000)        0 2023-07-02 23:31:51.996760 streamlit_slice_select-0.1.0/src/
-drwxr-xr-x   0 jailop    (1000) jailop    (1000)        0 2023-07-02 23:31:51.996760 streamlit_slice_select-0.1.0/src/streamlit_slice_select/
--rw-r--r--   0 jailop    (1000) jailop    (1000)      995 2023-07-02 22:36:00.000000 streamlit_slice_select-0.1.0/src/streamlit_slice_select/__init__.py
-drwxr-xr-x   0 jailop    (1000) jailop    (1000)        0 2023-07-02 23:31:51.996760 streamlit_slice_select-0.1.0/src/streamlit_slice_select.egg-info/
--rw-r--r--   0 jailop    (1000) jailop    (1000)    13199 2023-07-02 23:31:51.000000 streamlit_slice_select-0.1.0/src/streamlit_slice_select.egg-info/PKG-INFO
--rw-r--r--   0 jailop    (1000) jailop    (1000)      324 2023-07-02 23:31:51.000000 streamlit_slice_select-0.1.0/src/streamlit_slice_select.egg-info/SOURCES.txt
--rw-r--r--   0 jailop    (1000) jailop    (1000)        1 2023-07-02 23:31:51.000000 streamlit_slice_select-0.1.0/src/streamlit_slice_select.egg-info/dependency_links.txt
--rw-r--r--   0 jailop    (1000) jailop    (1000)       42 2023-07-02 23:31:51.000000 streamlit_slice_select-0.1.0/src/streamlit_slice_select.egg-info/requires.txt
--rw-r--r--   0 jailop    (1000) jailop    (1000)       23 2023-07-02 23:31:51.000000 streamlit_slice_select-0.1.0/src/streamlit_slice_select.egg-info/top_level.txt
+drwxr-xr-x   0 jailop    (1000) jailop    (1000)        0 2023-07-03 13:29:16.416742 streamlit_slice_select-0.1.1/
+-rw-r--r--   0 jailop    (1000) jailop    (1000)    11357 2023-07-02 22:46:33.000000 streamlit_slice_select-0.1.1/LICENSE.txt
+-rw-r--r--   0 jailop    (1000) jailop    (1000)    13199 2023-07-03 13:29:16.416742 streamlit_slice_select-0.1.1/PKG-INFO
+-rw-r--r--   0 jailop    (1000) jailop    (1000)       60 2023-07-02 22:12:17.000000 streamlit_slice_select-0.1.1/README.md
+-rw-r--r--   0 jailop    (1000) jailop    (1000)      490 2023-07-03 03:38:54.000000 streamlit_slice_select-0.1.1/pyproject.toml
+-rw-r--r--   0 jailop    (1000) jailop    (1000)       38 2023-07-03 13:29:16.416742 streamlit_slice_select-0.1.1/setup.cfg
+drwxr-xr-x   0 jailop    (1000) jailop    (1000)        0 2023-07-03 13:29:16.416742 streamlit_slice_select-0.1.1/src/
+drwxr-xr-x   0 jailop    (1000) jailop    (1000)        0 2023-07-03 13:29:16.416742 streamlit_slice_select-0.1.1/src/streamlit_slice_select/
+-rw-r--r--   0 jailop    (1000) jailop    (1000)      938 2023-07-03 13:28:30.000000 streamlit_slice_select-0.1.1/src/streamlit_slice_select/__init__.py
+drwxr-xr-x   0 jailop    (1000) jailop    (1000)        0 2023-07-03 13:29:16.416742 streamlit_slice_select-0.1.1/src/streamlit_slice_select.egg-info/
+-rw-r--r--   0 jailop    (1000) jailop    (1000)    13199 2023-07-03 13:29:16.000000 streamlit_slice_select-0.1.1/src/streamlit_slice_select.egg-info/PKG-INFO
+-rw-r--r--   0 jailop    (1000) jailop    (1000)      324 2023-07-03 13:29:16.000000 streamlit_slice_select-0.1.1/src/streamlit_slice_select.egg-info/SOURCES.txt
+-rw-r--r--   0 jailop    (1000) jailop    (1000)        1 2023-07-03 13:29:16.000000 streamlit_slice_select-0.1.1/src/streamlit_slice_select.egg-info/dependency_links.txt
+-rw-r--r--   0 jailop    (1000) jailop    (1000)       42 2023-07-03 13:29:16.000000 streamlit_slice_select-0.1.1/src/streamlit_slice_select.egg-info/requires.txt
+-rw-r--r--   0 jailop    (1000) jailop    (1000)       23 2023-07-03 13:29:16.000000 streamlit_slice_select-0.1.1/src/streamlit_slice_select.egg-info/top_level.txt
```

### Comparing `streamlit_slice_select-0.1.0/LICENSE.txt` & `streamlit_slice_select-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_slice_select-0.1.0/PKG-INFO` & `streamlit_slice_select-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_slice_select
-Version: 0.1.0
+Version: 0.1.1
 Summary: A like Excel-slicer input widget for Streamlit
 Author-email: Jaime Lopez <jaime.lopez@datainquiry.dev>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `streamlit_slice_select-0.1.0/src/streamlit_slice_select/__init__.py` & `streamlit_slice_select-0.1.1/src/streamlit_slice_select/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,13 @@
+"""
+Streamlit Slice Select Python Interface
+"""
+
 import os
+import json
 import streamlit.components.v1 as components
 
 _RELEASE = False
 
 parent_path = os.path.dirname(os.path.abspath(__file__))
 build_dir = os.path.join(parent_path, "frontend", "dist")
 
@@ -13,19 +18,16 @@
 
 def slice_select(name, default=[], key=None):
     component_value = _component_func(name=name, key=key, default=default)
     return component_value
 
 if __name__ == "__main__":
     import streamlit as st
-    options = slice_select("Options",
-            default=["Hello", "World", "Everybody"])
-    color_values = [
-        {"label": "blue", "status": False, "enabled": True},
-        {"label": "red", "status": True, "enabled": True},
-        {"label": "yellow", "status": False, "enabled": False},
-        {"label": "violet", "status": True, "enabled": False},
-    ]
-    st.session_state["colors"] = color_values
-    slice_select("Colors", default=color_values, key="colors")
-    st.write("Hello")
-    st.write(options)
+    st.subheader("A like Excel-slicer input widget for Streamlit")
+    st.text("This is a custom component that behaves like Excel's slicer control")
+    col1, col2 = st.columns(2)
+    with col1:
+        options = slice_select("Colors",
+                default=["Yellow", "Blue", "Red", "Violet", "Green",
+                        "Orange", "Brown"])
+        st.write("below")
+    col2.write(options)
```

### Comparing `streamlit_slice_select-0.1.0/src/streamlit_slice_select.egg-info/PKG-INFO` & `streamlit_slice_select-0.1.1/src/streamlit_slice_select.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-slice-select
-Version: 0.1.0
+Version: 0.1.1
 Summary: A like Excel-slicer input widget for Streamlit
 Author-email: Jaime Lopez <jaime.lopez@datainquiry.dev>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

