# Comparing `tmp/fast_dash-0.1.7.tar.gz` & `tmp/fast_dash-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_dash-0.1.7.tar", max compression
+gzip compressed data, was "fast_dash-0.2.0.tar", max compression
```

## Comparing `fast_dash-0.1.7.tar` & `fast_dash-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1074 2022-08-22 00:54:22.792575 fast_dash-0.1.7/LICENSE
--rw-r--r--   0        0        0     4877 2022-08-22 00:54:22.792575 fast_dash-0.1.7/README.md
--rw-r--r--   0        0        0    21105 2022-08-22 00:54:22.900577 fast_dash-0.1.7/fast_dash/Components.py
--rw-r--r--   0        0        0      635 2022-08-22 00:54:22.900577 fast_dash-0.1.7/fast_dash/__init__.py
--rw-r--r--   0        0        0    24457 2022-08-22 00:54:22.900577 fast_dash-0.1.7/fast_dash/assets/favicon.ico
--rw-r--r--   0        0        0    14427 2022-08-22 00:54:22.900577 fast_dash-0.1.7/fast_dash/fast_dash.py
--rw-r--r--   0        0        0     5516 2022-08-22 00:54:22.900577 fast_dash-0.1.7/fast_dash/utils.py
--rw-r--r--   0        0        0     2144 2022-08-22 00:54:22.900577 fast_dash-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       39 2022-08-22 00:54:22.900577 fast_dash-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0      262 2022-08-22 00:54:22.900577 fast_dash-0.1.7/tests/conftest.py
--rw-r--r--   0        0        0     3026 2022-08-22 00:54:22.900577 fast_dash-0.1.7/tests/examples.py
--rw-r--r--   0        0        0     2300 2022-08-22 00:54:22.900577 fast_dash-0.1.7/tests/test_examples.py
--rw-r--r--   0        0        0     5831 2022-08-22 00:54:22.900577 fast_dash-0.1.7/tests/test_fast_dash.py
--rw-r--r--   0        0        0    21632 2022-08-22 00:54:22.900577 fast_dash-0.1.7/tests/test_fast_dash_autodetect.py
--rw-r--r--   0        0        0     5870 2022-08-22 00:55:48.589268 fast_dash-0.1.7/setup.py
--rw-r--r--   0        0        0     5949 2022-08-22 00:55:48.590097 fast_dash-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-03 02:52:18.779733 fast_dash-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3585 2023-07-03 02:52:18.779733 fast_dash-0.2.0/README.md
+-rw-r--r--   0        0        0    33784 2023-07-03 02:52:18.891733 fast_dash-0.2.0/fast_dash/Components.py
+-rw-r--r--   0        0        0      635 2023-07-03 02:52:18.891733 fast_dash-0.2.0/fast_dash/__init__.py
+-rw-r--r--   0        0        0    24457 2023-07-03 02:52:18.891733 fast_dash-0.2.0/fast_dash/assets/favicon.ico
+-rw-r--r--   0        0        0    16369 2023-07-03 02:52:18.891733 fast_dash-0.2.0/fast_dash/fast_dash.py
+-rw-r--r--   0        0        0     6723 2023-07-03 02:52:18.891733 fast_dash-0.2.0/fast_dash/utils.py
+-rw-r--r--   0        0        0     2269 2023-07-03 02:52:18.895733 fast_dash-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-07-03 02:52:18.895733 fast_dash-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      314 2023-07-03 02:52:18.895733 fast_dash-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     3026 2023-07-03 02:52:18.895733 fast_dash-0.2.0/tests/examples.py
+-rw-r--r--   0        0        0     2300 2023-07-03 02:52:18.895733 fast_dash-0.2.0/tests/test_examples.py
+-rw-r--r--   0        0        0     5831 2023-07-03 02:52:18.895733 fast_dash-0.2.0/tests/test_fast_dash.py
+-rw-r--r--   0        0        0    21632 2023-07-03 02:52:18.895733 fast_dash-0.2.0/tests/test_fast_dash_autodetect.py
+-rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 fast_dash-0.2.0/PKG-INFO
```

### Comparing `fast_dash-0.1.7/LICENSE` & `fast_dash-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_dash-0.1.7/README.md` & `fast_dash-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,46 @@
-# Overview
+Metadata-Version: 2.1
+Name: fast-dash
+Version: 0.2.0
+Summary: Build Machine Learning prototypes web applications lightning fast.
+Home-page: https://github.com/dkedar7/fast_dash
+License: MIT
+Author: Kedar Dabhadkar
+Author-email: kedar@fastdash.app
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: dev
+Provides-Extra: doc
+Provides-Extra: test
+Requires-Dist: Flask (>=2.0.2,<3.0.0)
+Requires-Dist: Pillow (>=9.2.0,<10.0.0)
+Requires-Dist: dash (>=2.6.1,<3.0.0) ; extra == "test"
+Requires-Dist: dash-bootstrap-components (>=1.0.2,<2.0.0)
+Requires-Dist: dash-iconify (>=0.1.2,<0.2.0)
+Requires-Dist: dash-mantine-components (>=0.12.1,<0.13.0)
+Requires-Dist: matplotlib (<=3.7.1)
+Requires-Dist: numpy (<=1.25.0)
+Requires-Dist: plotly (>=5.5.0,<6.0.0)
+Description-Content-Type: text/markdown
 
+<p align="center">
+  <a href="https://fastdash.app/"><img src="https://storage.googleapis.com/fast_dash/0.1.8/logo.png" alt="Fast Dash" width=300></a>
+</p>
+<p align="center">
+    <em>Open source, Python-based tool to build prototypes lightning fast ⚡</em>
+</p>
 
 <p align="center">
 <a href="https://pypi.python.org/pypi/fast_dash">
     <img src="https://img.shields.io/pypi/v/fast_dash?color=%2334D058"
         alt = "Release Status">
 </a>
 
@@ -19,113 +56,86 @@
 <a href="https://docs.fastdash.app/">
     <img src="https://img.shields.io/badge/Docs-MkDocs-<COLOR>.svg" alt="Documentation">
 </a>
 
 </p>
 
 
-<p align="center">
-  <a href="https://fastdash.app/"><img src="https://raw.githubusercontent.com/dkedar7/fast_dash/main/docs/assets/logo.png" alt="Fast Dash logo"></a>
-</p>
-<p align="center">
-    <em>Open source, Python-based tool to build prototypes lightning fast ⚡</em>
-</p>
-
-
 ---
 
-* Website: <https://fastdash.app/>
-* Documentation: <https://docs.fastdash.app/>
-* Source code: <https://github.com/dkedar7/fast_dash/>
-* Installation: `pip install fast-dash`
+* **Documentation**: [https://docs.fastdash.app](https://docs.fastdash.app)
+* **Source code**: [github.com/dkedar7/fast_dash](https://github.com/dkedar7/fast_dash/)
+* **Installation**: `pip install fast-dash`
 
 ---
 
-Fast Dash is a Python module that makes the development of web applications fast and easy. It is built on top of Plotly Dash and can be used to build web interfaces for Machine Learning models or to showcase any proof of concept without the hassle of developing UI from scratch.
+Fast Dash is a Python module that makes the development of web applications fast and easy. It can build web interfaces for Machine Learning models or to showcase any proof of concept without the hassle of developing UI from scratch.
 
-<p align="center">
+<!-- <p align="center">
   <a href="https://fastdash.app/"><img src="https://raw.githubusercontent.com/dkedar7/fast_dash/main/docs/assets/gallery_4_apps.gif" alt="Fast Dash logo"></a>
-</p>
+</p> -->
 
-## Simple example
+## Examples
 
-With Fast Dash's decorator `fastdash`, it's a breeze to deploy any Python function as a web app. Here's how to use it to write your first Fast Dash app:
+With Fast Dash's decorator `@fastdash`, it's a breeze to deploy any Python function as a web app. Here's how to use it to write your first Fast Dash app:
 ```python
 from fast_dash import fastdash
 
 @fastdash
 def text_to_text_function(input_text):
     return input_text
 
 # * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
 ```
 
 And just like that (🪄), we have a completely functional interactive app!
 
 Output:
-![Simple example](https://raw.githubusercontent.com/dkedar7/fast_dash/decorate/docs/assets/simple_example.gif)
-
+![Simple example](https://storage.googleapis.com/fast_dash/0.1.8/Simple%20text%20to%20text.png)
 ---
 
-Fast Dash can read additional details about a function, like its name, input and output types, docstring, and uses this information to infer which components to use.
+Fast Dash can read all the function details, like its name, input and output types, docstring, and uses this information to infer which components to use.
 
-For example, here's how to deploy an app that takes a string and an integer as inputs and return some text.
+For example, here's how to deploy an app that takes a string and an integer as inputs and returns some text.
 
 ```python
 from fast_dash import fastdash
 
 @fastdash
 def display_selected_text_and_number(text: str, number: int) -> str:
     "Simply display the selected text and number"
     processed_text = f'Selected text is {text} and the number is {number}.'
     return processed_text
 
 # * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
 ```
-Output:
 
-![Simple example with multiple inputs](https://storage.googleapis.com/fast_dash/0.1.7/simple_example_2.gif)
+Output:
+![Simple example with multiple inputs](https://storage.googleapis.com/fast_dash/0.1.8/Simple%20example%202.png)
 
 And with just a few more lines, we can add a title icon, subheader and other social branding details.
 
-```python
-from fast_dash import fastdash
-
-@fastdash(title_image_path='https://raw.githubusercontent.com/dkedar7/fast_dash/main/docs/assets/favicon.jpg',
-        github_url='https://github.com/dkedar7/fast_dash',
-        linkedin_url='https://linkedin.com/in/dkedar7',
-        twitter_url='https://twitter.com/dkedar')
-def display_selected_text_and_number(text: str, number: int) -> str:
-    "Simply display the selected text and number"
-    processed_text = f'Selected text is {text} and the number is {number}.'
-    return processed_text
-```
-
-Output:
+---
 
-![Simple example with multiple inputs and details](https://storage.googleapis.com/fast_dash/0.1.7/simple_example_multiple_inputs_details.png)
+## About
 
----
 Read different ways to build Fast Dash apps and additional details by navigating to the [project documentation](https://docs.fastdash.app/).
 
-## Key features
+### Key features
 
-- Launch an app only by specifying the types of inputs and outputs.
+- Launch an app by adding a decorator only.
 - Use multiple input and output components simultaneously.
 - Flask-based backend allows easy scalability and customizability.
 - Build fast, share and iterate.
 
-Some features are coming up in future releases:
-
-- More input and output components.
-- Deploy to Heroku and Google Cloud.
-- and many more.
-
 ## Community
 
-Fast Dash is built on open-source. You are encouraged to share your own projects, which will be highlighted on a common community gallery (coming up).
+Fast Dash is built using [Plotly Dash](https://github.com/plotly/dash) and it's completely open-source.
 
-## Credits
-
-Fast Dash is built using [Plotly Dash](https://github.com/plotly/dash). Dash's Flask-based backend enables Fast Dash apps to scale easily and makes them highly compatibility with other integration services. This project is partially inspired from [gradio](https://github.com/gradio-app/gradio).
-
-The project template was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and [zillionare/cookiecutter-pypackage](https://github.com/zillionare/cookiecutter-pypackage).
+## Citation
+Please cite Fast Dash it if you use it in your work.
+```
+@software{Kedar_Dabhadkar_Fast_Dash,
+author = {Kedar Dabhadkar},
+title = {{Fast Dash}}
+}
+```
```

### Comparing `fast_dash-0.1.7/fast_dash/__init__.py` & `fast_dash-0.2.0/fast_dash/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Fast Dash."""
 
 __author__ = """Kedar Dabhadkar"""
 __email__ = "kedar@fastdash.app"
-__version__ = "0.1.6"
+__version__ = "0.2.0"
 
 from fast_dash.Components import (
     Graph,
     Image,
     Slider,
     Text,
     TextArea,
```

### Comparing `fast_dash-0.1.7/fast_dash/assets/favicon.ico` & `fast_dash-0.2.0/fast_dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `fast_dash-0.1.7/fast_dash/fast_dash.py` & `fast_dash-0.2.0/fast_dash/fast_dash.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import functools
 import logging
 import re
 import warnings
 
 import dash
+import dash_bootstrap_components as dbc
 import flask
-from dash.dependencies import Input, Output
+from dash import Input, Output
 
-from .Components import DefaultLayout, Text, _infer_components
+from .Components import BaseLayout, SidebarLayout, Text, _infer_components
 from .utils import (
     _assign_ids_to_inputs,
     _assign_ids_to_outputs,
     _make_input_groups,
     _make_output_groups,
+    _transform_outputs,
     theme_mapper,
 )
 
 
 class FastDash:
     """
     Fast Dash app object containing automatically generated UI components and callbacks.
@@ -25,36 +27,45 @@
     a flask WSGI application. It has in-built support for automated UI generation and
     sets all parameters required for Fast Dash app deployment.
     """
 
     def __init__(
         self,
         callback_fn,
+        layout="sidebar",
+        mosaic=None,
         inputs=None,
         outputs=None,
         title=None,
         title_image_path=None,
         subheader=None,
         github_url=None,
         linkedin_url=None,
         twitter_url=None,
         navbar=True,
         footer=True,
-        theme="JOURNAL",
+        theme=None,
         update_live=False,
+        port=8080,
         mode=None,
         minimal=False,
         disable_logs=False,
+        scale_height=1,
+        run_kwargs=dict(),
         **kwargs
     ):
         """
         Args:
             callback_fn (func): Python function that Fast Dash deploys.
                 This function guides the behavior of and interaction between input and output components.
 
+            layout (str, optional): App layout style. Currently supports 'base' and 'sidebar' (default).
+
+            mosaic (str): Mosaic array layout, if sidebar layout is selected.
+
             inputs (Fast component, list of Fast components, optional): Components to represent inputs of the callback function.
                 Defaults to None. If `None`, Fast Dash attempts to infer the best components from callback function's type
                 hints and default values. In the absence of type hints, default components are all `Text`.
 
             outputs (Fast component, list of Fast components, optional): Components to represent outputs of the callback function.
                 Defaults to None. If `None`, Fast Dash attempts to infer the best components from callback function's type hints.
                 In the absence of type hints, default components are all `Text`.
@@ -81,35 +92,47 @@
             footer (bool, optional): Display footer. Defaults to True.
 
             theme (str, optional): Apply theme to the app. Defaults to "JOURNAL". All available themes can be found
                 at https://bootswatch.com/.
 
             update_live (bool, optional): Enable hot reloading. Defaults to False.
 
+            port (int, optional): Port to which the app should be deployed. Defauts to 8080.
+
             mode (str, optional): Mode in which to launch the app. Acceptable options are `None`, `jupyterlab`, `inline`, 'external`.
                 Defaults to None.
 
             minimal (bool, optional): Display minimal version by hiding navbar, title, title image, subheader and footer.
                 Defaults to False.
 
             disable_logs (bool, optional): Hide app logs. Sets logger level to `ERROR`. Defaults to False.
+
+            scale_height (float, optional): Height of the app container is enlarged as a multiple of this. Defaults to 1.
+
+            run_kwargs (dict, optional): All values from this variable are passed to Dash's `.run` method.
         """
 
         self.callback_fn = callback_fn
+        self.layout_pattern = layout
+        self.mosaic = mosaic
         self.inputs = (
             _infer_components(callback_fn, is_input=True) if inputs is None else inputs
         )
         self.outputs = (
             _infer_components(callback_fn, is_input=False)
             if outputs is None
             else outputs
         )
         self.update_live = update_live
         self.mode = mode
         self.disable_logs = disable_logs
+        self.scale_height = scale_height
+        self.port = port
+        self.run_kwargs = run_kwargs
+        self.run_kwargs.update(dict(port=port))
         self.kwargs = kwargs
 
         if self.disable_logs is True:
             log = logging.getLogger("werkzeug")
             log.setLevel(logging.ERROR)
 
         else:
@@ -117,20 +140,21 @@
             log.setLevel(logging.DEBUG)
 
         if title is None:
             title = re.sub("[^0-9a-zA-Z]+", " ", callback_fn.__name__).title()
 
         self.title = title
         self.title_image_path = title_image_path
-        self.subtext = subheader if subheader is not None else callback_fn.__doc__
+        self.subtitle = subheader if subheader is not None else callback_fn.__doc__
         self.github_url = github_url
         self.linkedin_url = linkedin_url
         self.twitter_url = twitter_url
         self.navbar = navbar
         self.footer = footer
+        self.theme = theme or "JOURNAL"
         self.minimal = minimal
 
         # Assign IDs to components
         self.inputs_with_ids = _assign_ids_to_inputs(self.inputs, self.callback_fn)
         self.outputs_with_ids = _assign_ids_to_outputs(self.outputs)
         self.ack_mask = [
             True if input_.ack is not None else False for input_ in self.inputs_with_ids
@@ -140,15 +164,15 @@
         self.output_state_default = [
             output_.placeholder for output_ in self.outputs_with_ids
         ]
 
         # Define Flask server
         server = flask.Flask(__name__)
         external_stylesheets = [
-            theme_mapper(theme),
+            theme_mapper(self.theme),
             "https://use.fontawesome.com/releases/v5.9.0/css/all.css",
         ]
 
         source = dash.Dash
         if self.mode is not None:
             try:
                 from jupyter_dash import JupyterDash
@@ -160,23 +184,18 @@
                 warnings.warn(str(e))
                 warnings.warn("Ignoring mode argument")
 
         self.app = source(
             __name__,
             external_stylesheets=external_stylesheets,
             server=server,
-            meta_tags=[
-                {
-                    "name": "viewport",
-                    "content": "width=device-width, initial-scale=1.0, maximum-scale=1.8, minimum-scale=0.5",
-                }
-            ],
+            **self.kwargs
         )
         # Define app title
-        self.app.title = self.title
+        self.app.title = self.title or ""
 
         # Intialize layout
         self.set_layout()
 
         # Register callbacks
         self.register_callback_fn()
 
@@ -184,47 +203,59 @@
         self.submit_clicks = 0
         self.reset_clicks = 0
         self.app_initialized = False
 
         # Allow easier access to Dash server
         self.server = self.app.server
 
-    def run(self, **kwargs):
-        self.server.run(**kwargs) if self.mode is None else self.app.run_server(
-            mode=self.mode, **kwargs
+    def run(self):
+        self.server.run(
+            **self.run_kwargs
+        ) if self.mode is None else self.app.run_server(
+            mode=self.mode, **self.run_kwargs
         )
 
-    def run_server(self, **kwargs):
-        self.app.run_server(**kwargs) if self.mode is None else self.app.run_server(
-            mode=self.mode, **kwargs
+    def run_server(self):
+        self.app.run_server(
+            **self.run_kwargs
+        ) if self.mode is None else self.app.run_server(
+            mode=self.mode, **self.run_kwargs
         )
 
     def set_layout(self):
-
         if self.inputs is not None:
             input_groups = _make_input_groups(self.inputs_with_ids, self.update_live)
 
         if self.outputs is not None:
             output_groups = _make_output_groups(self.outputs_with_ids, self.update_live)
 
-        default_layout = DefaultLayout(
-            inputs=input_groups,
-            outputs=output_groups,
-            title=self.title,
-            title_image_path=self.title_image_path,
-            subtext=self.subtext,
-            github_url=self.github_url,
-            linkedin_url=self.linkedin_url,
-            twitter_url=self.twitter_url,
-            navbar=self.navbar,
-            footer=self.footer,
-            minimal=self.minimal,
-        )
+        layout_args = {
+            "mosaic": self.mosaic,
+            "inputs": input_groups,
+            "outputs": output_groups,
+            "title": self.title,
+            "title_image_path": self.title_image_path,
+            "subtitle": self.subtitle,
+            "github_url": self.github_url,
+            "linkedin_url": self.linkedin_url,
+            "twitter_url": self.twitter_url,
+            "navbar": self.navbar,
+            "footer": self.footer,
+            "minimal": self.minimal,
+            "scale_height": self.scale_height,
+        }
+
+        if self.layout_pattern == "sidebar":
+            app_layout = SidebarLayout(**layout_args)
+
+        else:
+            app_layout = BaseLayout(**layout_args)
 
-        self.app.layout = default_layout.layout
+        self.layout_object = app_layout
+        self.app.layout = app_layout.generate_layout()
 
     def register_callback_fn(self):
         @self.app.callback(
             [
                 Output(
                     component_id=output_.id,
                     component_property=output_.component_property,
@@ -244,17 +275,17 @@
                 )
                 for input_ in self.inputs_with_ids
             ]
             + [
                 Input(component_id="reset_inputs", component_property="n_clicks"),
                 Input(component_id="submit_inputs", component_property="n_clicks"),
             ],
+            prevent_initial_callback=True,
         )
         def process_input(*args):
-
             reset_button = args[-2]
             submit_button = args[-1]
             ack_components = [
                 ack if mask is True else None
                 for mask, ack in zip(self.ack_mask, list(args[:-2]))
             ]
 
@@ -263,60 +294,72 @@
             ):
                 self.app_initialized = True
                 self.submit_clicks = submit_button
                 output_state = self.callback_fn(*args[:-2])
 
                 if isinstance(output_state, tuple):
                     self.output_state = list(output_state)
-                    return self.output_state + ack_components
 
-                self.output_state = [output_state]
+                else:
+                    self.output_state = [output_state]
+
+                # Transform outputs to fit in the desired components
+                self.output_state = _transform_outputs(self.output_state)
+
                 return self.output_state + ack_components
 
             elif reset_button > self.reset_clicks:
                 self.reset_clicks = reset_button
                 self.output_state = self.output_state_default
                 return self.output_state + ack_components
 
             elif self.app_initialized:
                 return self.output_state + ack_components
 
             else:
                 return self.output_state_default + ack_components
 
+        # Set layout callbacks
+        self.layout_object.callbacks(self.app)
+
 
 def fastdash(
     _callback_fn=None,
     *,
+    layout="sidebar",
+    mosaic=None,
     inputs=None,
     outputs=None,
     title=None,
     title_image_path=None,
     subheader=None,
     github_url=None,
     linkedin_url=None,
     twitter_url=None,
     navbar=True,
     footer=True,
-    theme="JOURNAL",
+    theme=None,
     update_live=False,
+    port=8080,
     mode=None,
     minimal=False,
     disable_logs=False,
-    **run_kwargs
+    scale_height=1,
+    run_kwargs=dict(),
+    **kwargs
 ):
     """
-    Decorator for the `FastDash` class.
-
-    Use the decorated Python callback functions and deployes it using the chosen mode.
-
     Args:
         callback_fn (func): Python function that Fast Dash deploys.
             This function guides the behavior of and interaction between input and output components.
 
+        layout (str, optional): App layout style. Currently supports 'base' and 'sidebar' (default).
+
+        mosaic (str): Mosaic array layout, if sidebar layout is selected.
+
         inputs (Fast component, list of Fast components, optional): Components to represent inputs of the callback function.
             Defaults to None. If `None`, Fast Dash attempts to infer the best components from callback function's type
             hints and default values. In the absence of type hints, default components are all `Text`.
 
         outputs (Fast component, list of Fast components, optional): Components to represent outputs of the callback function.
             Defaults to None. If `None`, Fast Dash attempts to infer the best components from callback function's type hints.
             In the absence of type hints, default components are all `Text`.
@@ -343,49 +386,60 @@
         footer (bool, optional): Display footer. Defaults to True.
 
         theme (str, optional): Apply theme to the app. Defaults to "JOURNAL". All available themes can be found
             at https://bootswatch.com/.
 
         update_live (bool, optional): Enable hot reloading. Defaults to False.
 
+        port (int, optional): Port to which the app should be deployed. Defauts to 8080.
+
         mode (str, optional): Mode in which to launch the app. Acceptable options are `None`, `jupyterlab`, `inline`, 'external`.
             Defaults to None.
 
         minimal (bool, optional): Display minimal version by hiding navbar, title, title image, subheader and footer.
             Defaults to False.
 
         disable_logs (bool, optional): Hide app logs. Sets logger level to `ERROR`. Defaults to False.
+
+        scale_height (float, optional): Height of the app container is enlarged as a multiple of this. Defaults to 1.
+
+        run_kwargs (dict, optional): All values from this variable are passed to Dash's `.run` method.
     """
 
     def decorator_fastdash(callback_fn):
         "Decorator for callback_fn"
 
         @functools.wraps(callback_fn)
         def wrapper_fastdash(**kwargs):
             app = FastDash(callback_fn=callback_fn, **kwargs)
-            app.run(**run_kwargs)
+            app.run()
             return callback_fn
 
         return wrapper_fastdash(
+            layout=layout,
+            mosaic=mosaic,
             inputs=inputs,
             outputs=outputs,
             title=title,
             title_image_path=title_image_path,
             subheader=subheader,
             github_url=github_url,
             linkedin_url=linkedin_url,
             twitter_url=twitter_url,
             navbar=navbar,
             footer=footer,
             theme=theme,
             update_live=update_live,
             mode=mode,
+            port=port,
             minimal=minimal,
             disable_logs=disable_logs,
-            **run_kwargs
+            scale_height=scale_height,
+            run_kwargs=run_kwargs,
+            **kwargs
         )
 
     # If the decorator is called with arguments
     if _callback_fn is None:
         return decorator_fastdash
     # If the decorator is called without arguments. Use default input and output values
     else:
```

### Comparing `fast_dash-0.1.7/fast_dash/utils.py` & `fast_dash-0.2.0/fast_dash/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,30 +3,33 @@
 """
 import base64
 import copy
 import inspect
 from io import BytesIO
 
 import dash_bootstrap_components as dbc
+import matplotlib as mpl
+import matplotlib.pyplot as plt
 from dash import html
+from PIL import ImageFile
 
 
 def Fastify(component, component_property, ack=None, placeholder=None, label_=None):
     """
     Modify a Dash component to a FastComponent.
 
     Args:
-        component (type):
-        component_property (type):
-        ack (type, optional):
-        placeholder (type, optional):
-        label_ (type, optional):
+        component (Dash component): Dash component that needs to be modified
+        component_property (str): Component property that's assigned the input or output values
+        ack (Dash component, optional): Dash component that's displayed as an acknowledgement of the original component
+        placeholder (type, optional): Placeholder value of the component.
+        label_ (type, optional): Component title.
 
     Returns:
-        [type]: [description]
+        Fast component: Dash component modified to make it compatible with Fast Dash.
     """
 
     component.component_property = component_property
     component.ack = ack
     component.label_ = label_
     component.placeholder = placeholder
 
@@ -36,14 +39,15 @@
 # Add themes mapper
 def theme_mapper(theme_name):
     """
     Map theme name string ot a dbc theme object
     """
 
     theme_mapper_dict = {
+        "BOOTSTRAP": dbc.themes.BOOTSTRAP,
         "CERULEAN": dbc.themes.CERULEAN,
         "COSMO": dbc.themes.COSMO,
         "CYBORG": dbc.themes.CYBORG,
         "DARKLY": dbc.themes.DARKLY,
         "FLATLY": dbc.themes.FLATLY,
         "JOURNAL": dbc.themes.JOURNAL,
         "LITERA": dbc.themes.LITERA,
@@ -86,14 +90,32 @@
     img.save(buffered, format="PNG")
     img_str = base64.b64encode(buffered.getvalue()).decode("utf-8")
     img_str = f"data:image/png;base64,{img_str}"
 
     return img_str
 
 
+def _mpl_to_b64(fig):
+    """
+    Utility to convert Matplotlib figure to a base64 string.
+
+    Args:
+        fig (matplotlib.figure.Figure): Input matplotlib plot
+
+    Returns:
+        str: Base64 string of the input image
+    """
+    buffered = BytesIO()
+    fig.savefig(buffered, format="PNG")
+    img_str = base64.b64encode(buffered.getvalue()).decode("utf-8")
+    img_str = f"data:image/png;base64,{img_str}"
+
+    return img_str
+
+
 # Input component utils
 def _get_input_names_from_callback_fn(callback_fn):
     """
     Returns the names of function arguments as a list of strings
     """
     signature = inspect.signature(callback_fn)
     parameters = signature.parameters
@@ -120,15 +142,15 @@
     return inputs_with_ids
 
 
 def _make_input_groups(inputs_with_ids, update_live):
 
     input_groups = []
 
-    input_groups.append(html.H6("INPUT"))
+    input_groups.append(html.H4("INPUTS"))
 
     for idx, input_ in enumerate(inputs_with_ids):
         label = f"{input_.id}" if input_.label_ is None else input_.label_
         label = label.replace("_", " ").upper()
         ack_component = (
             Fastify(component=dbc.Col(), component_property="children")
             if input_.ack is None
@@ -137,15 +159,15 @@
         ack_component.id = f"{input_.id}_ack"
 
         input_.ack = ack_component
 
         input_groups.append(
             dbc.Col(
                 [dbc.Label(label, align="end"), input_, ack_component],
-                align="center",
+                align="left",
             )
         )
 
     button_row = html.Div(
         [
             dbc.Button(
                 "Submit",
@@ -181,26 +203,25 @@
 
     return outputs_with_ids
 
 
 def _make_output_groups(outputs, update_live):
 
     output_groups = []
-    output_groups.append(html.H6("OUTPUT"))
+    # output_groups.append(html.H6("OUTPUT"))
 
     for idx, output_ in enumerate(outputs):
         label = f"Output {idx + 1}" if output_.label_ is None else output_.label_
-        label = label.replace("_", " ").upper()
+        label = label.replace("_", " ")
         output_groups.append(
             dbc.Col(
-                [
-                    dbc.Label(label, align="end"),
-                    dbc.Spinner(children=output_, color="primary"),
-                ],
+                [dbc.Label(label, align="end")] + [output_],
                 align="center",
+                style={"width": "100%", "overflow": "hidden"},
+                class_name="rounded border d-flex flex-column flex-fill",
             )
         )
 
     button_row = html.Div(
         [
             dbc.Button(
                 "Clear",
@@ -215,7 +236,18 @@
         if update_live is False
         else dict(display="none"),
     )
 
     output_groups.append(button_row)
 
     return output_groups
+
+
+def _transform_outputs(outputs):
+    "Transform outputs to fit in the desired components"
+
+    _transform_mapper = {plt.Figure: _mpl_to_b64, ImageFile.ImageFile: _pil_to_b64}
+
+    return [
+        _transform_mapper[type(o)](o) if type(o) in _transform_mapper else o
+        for o in outputs
+    ]
```

### Comparing `fast_dash-0.1.7/pyproject.toml` & `fast_dash-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 [tool]
 [tool.poetry]
 name = "fast_dash"
-version = "0.1.7"
+version = "0.2.0"
 homepage = "https://github.com/dkedar7/fast_dash"
 description = "Build Machine Learning prototypes web applications lightning fast."
 authors = ["Kedar Dabhadkar <kedar@fastdash.app>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
-    'Development Status :: 2 - Pre-Alpha',
+    'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10'
 ]
 packages = [
     { include = "fast_dash" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 
 Flask = "^2.0.2"
 plotly = "^5.5.0"
 dash-bootstrap-components = "^1.0.2"
 Pillow = "^9.2.0"
 dash = "^2.6.1"
+dash-mantine-components = "^0.12.1"
+numpy = "<=1.25.0"
+dash-iconify = "^0.1.2"
+matplotlib = "<=3.7.1"
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "black",
     "isort",
     "flake8",
     "flake8-docstrings",
     "pytest-cov",
     "selenium",
-    "dash[testing]"
+    "dash"
     ]
 
-dev = ["tox", "pre-commit", "virtualenv", "pip", "twine", "toml"]
+dev = ["tox", "pre-commit", "virtualenv", "twine", "toml"]
 
 doc = [
     "mkdocs",
     "livereload",
     "mkdocs-include-markdown-plugin",
     "mkdocs-material",
     "mkdocstrings",
@@ -62,26 +66,29 @@
 black = "^22.6.0"
 isort = "^5.10.1"
 flake8-docstrings = "^1.6.0"
 pytest-cov = "^3.0.0"
 tox = "^3.25.1"
 pre-commit = "^2.20.0"
 virtualenv = "^20.16.3"
-pip = "^22.2.2"
 twine = "^4.0.1"
 toml = "^0.10.2"
 mkdocs = "^1.3.1"
 livereload = "^2.6.3"
 mkdocs-include-markdown-plugin = "^3.6.1"
 mkdocs-material = "^8.3.9"
 mkdocstrings = "^0.19.0"
 mkdocs-autorefs = "^0.4.1"
 jupyter-dash = "^0.4.2"
 dash = {extras = ["testing"], version = "^2.6.1"}
 mkdocstrings-python = "^0.7.1"
+
+[tool.poetry.group.test.dependencies]
+urllib3 = "1.26.15"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
 include = '\.pyi?$'
```

### Comparing `fast_dash-0.1.7/tests/examples.py` & `fast_dash-0.2.0/tests/examples.py`

 * *Files identical despite different names*

### Comparing `fast_dash-0.1.7/tests/test_examples.py` & `fast_dash-0.2.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `fast_dash-0.1.7/tests/test_fast_dash.py` & `fast_dash-0.2.0/tests/test_fast_dash.py`

 * *Files identical despite different names*

### Comparing `fast_dash-0.1.7/tests/test_fast_dash_autodetect.py` & `fast_dash-0.2.0/tests/test_fast_dash_autodetect.py`

 * *Files identical despite different names*

