# Comparing `tmp/heygptcli-0.1.5.tar.gz` & `tmp/heygptcli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heygptcli-0.1.5.tar", max compression
+gzip compressed data, was "heygptcli-0.1.6.tar", max compression
```

## Comparing `heygptcli-0.1.5.tar` & `heygptcli-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       87 2023-06-23 09:09:49.068212 heygptcli-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/__init__.py
--rw-r--r--   0        0        0      774 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/api.py
--rwxr-xr-x   0        0        0     5292 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/cli.py
--rw-r--r--   0        0        0     2249 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/constant.py
--rw-r--r--   0        0        0     3515 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/core.py
--rw-r--r--   0        0        0     1984 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/serve.py
--rw-r--r--   0        0        0      153 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/serve_prompts.py
--rw-r--r--   0        0        0      849 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/utils.py
--rw-r--r--   0        0        0      677 2023-06-23 09:09:49.068212 heygptcli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 heygptcli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-07-03 16:05:18.682204 heygptcli-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/__init__.py
+-rw-r--r--   0        0        0      774 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/api.py
+-rwxr-xr-x   0        0        0     5292 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/cli.py
+-rw-r--r--   0        0        0     2249 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/constant.py
+-rw-r--r--   0        0        0     3542 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/core.py
+-rw-r--r--   0        0        0     2162 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/serve.py
+-rw-r--r--   0        0        0      153 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/serve_prompts.py
+-rw-r--r--   0        0        0      849 2023-07-03 16:05:18.682204 heygptcli-0.1.6/heygpt/utils.py
+-rw-r--r--   0        0        0      677 2023-07-03 16:05:18.682204 heygptcli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 heygptcli-0.1.6/PKG-INFO
```

### Comparing `heygptcli-0.1.5/heygpt/api.py` & `heygptcli-0.1.6/heygpt/api.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.5/heygpt/cli.py` & `heygptcli-0.1.6/heygpt/cli.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.5/heygpt/constant.py` & `heygptcli-0.1.6/heygpt/constant.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.5/heygpt/core.py` & `heygptcli-0.1.6/heygpt/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,16 @@
             max_tokens=1000,
             stream=True,
             top_p=1,
         )
         for chunk in completion:
             c = chunk["choices"][0]["text"]
             out += c
-            console.print(c, end="", markup=True)
+            if _print:
+                console.print(c, end="", markup=True)
 
     return out
 
 
 def completion_bard(text: str, command: str = "", _print=False):
     """
     ref: https://github.com/dsdanielpark/Bard-API
```

### Comparing `heygptcli-0.1.5/heygpt/serve.py` & `heygptcli-0.1.6/heygpt/serve.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,18 +49,24 @@
             _selected_prompt = ""
 
         if submit:
             if use_model != "Bard":
                 completion = completion_openai_gpt(
                     command=_selected_prompt, text=ask, model=_options[use_model]
                 )
+                if "davinci" in use_model.lower():
+                    st.markdown(f"```{completion}")
+                else:
+                    st.markdown(completion)
+
             else:
                 completion = completion_bard(command=_selected_prompt, text=ask)
+                st.markdown(completion)
+
             content = completion
-            st.markdown(content)
 
     with col3:
         if content != "":
             st.download_button(
                 label="Download text",
                 data=content.encode("utf-8"),
                 file_name="output.txt",
```

### Comparing `heygptcli-0.1.5/heygpt/utils.py` & `heygptcli-0.1.6/heygpt/utils.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.5/pyproject.toml` & `heygptcli-0.1.6/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heygptcli"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Rishang <rishang@localhost.com>"]
 readme = "README.md"
 packages = [
   { include = "heygpt" }
 ]
```

### Comparing `heygptcli-0.1.5/PKG-INFO` & `heygptcli-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heygptcli
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Rishang
 Author-email: rishang@localhost.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

