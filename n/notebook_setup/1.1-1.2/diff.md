# Comparing `tmp/notebook_setup-1.1.tar.gz` & `tmp/notebook_setup-1.2.tar.gz`

## Comparing `notebook_setup-1.1.tar` & `notebook_setup-1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 notebook_setup-1.1/.python-version
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 notebook_setup-1.1/Example.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notebook_setup-1.1/temp.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 notebook_setup-1.1/notebook_setup/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 notebook_setup-1.1/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 notebook_setup-1.1/LICENSE
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 notebook_setup-1.1/README.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 notebook_setup-1.1/pyproject.toml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 notebook_setup-1.1/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 notebook_setup-1.2/.python-version
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 notebook_setup-1.2/Example.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notebook_setup-1.2/temp.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 notebook_setup-1.2/notebook_setup/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 notebook_setup-1.2/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 notebook_setup-1.2/LICENSE
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 notebook_setup-1.2/README.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 notebook_setup-1.2/pyproject.toml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 notebook_setup-1.2/PKG-INFO
```

### Comparing `notebook_setup-1.1/Example.ipynb` & `notebook_setup-1.2/Example.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'cells'": "{0: {'execution_count': 5}, 1: {'execution_count': 6}, 2: {'execution_count': 8, "*

 * *            "'outputs': [], 'source': ['notebook_config_plotly_rendering(force_small_file=True, "*

 * *            'global_renderer="svg")\']}}'}*

```diff
@@ -1,21 +1,21 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from notebook_setup import notebook_setup, notebook_config_plotly_rendering"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "The autoreload extension is already loaded. To reload it, use:\n",
@@ -42,36 +42,19 @@
             ],
             "source": [
                 "notebook_setup(autoreload=True, background_transparent=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 8,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "<span style=\"color:red\">Warning: </span>global_renderer=\"svg\" has no effect, set force_small_file=False"
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.HTML object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "notebook_config_plotly_rendering(\n",
-                "    force_small_file=True,\n",
-                "    global_renderer=\"svg\",\n",
-                "    verbose=True,\n",
-                ")"
+                "notebook_config_plotly_rendering(force_small_file=True, global_renderer=\"svg\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `notebook_setup-1.1/notebook_setup/__init__.py` & `notebook_setup-1.2/notebook_setup/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,14 @@
             """,
         )
 
 
 def notebook_config_plotly_rendering(
     force_small_file: bool = True,
     global_renderer: str = None,
-    verbose=True,
 ):
     """
     Configures the behavior of Plotly figures in Jupyter notebooks. -> Make small files and render on GitHub.
     Only figures with fig.show() are effected by this configuration.
     This function monkey patches (modifies at runtime) behavior of fig.show(). Tested with VS Code.
 
     Args:
@@ -65,17 +64,16 @@
                 return pio.show(self, *args, renderer=renderer, **kwargs)
             else:
                 display(
                     self,
                     # raw=True,
                 )
 
-        if verbose and global_renderer:
-            msg = f"""global_renderer="{global_renderer}" has no effect, set force_small_file=False"""
-            display(HTML(f"""<span style="color:red">Warning: </span>{msg}"""))
+        # msg = f"""global_renderer="{global_renderer}" has no effect, set force_small_file=False"""
+        # display(HTML(f"""<span style="color:red">Warning: </span>{msg}"""))
 
     else:
         if global_renderer:
             pio.renderers.default = global_renderer
 
         def show(self, *args, **kwargs):
             "Plotly default implementation"
```

### Comparing `notebook_setup-1.1/.gitignore` & `notebook_setup-1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `notebook_setup-1.1/LICENSE` & `notebook_setup-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook_setup-1.1/pyproject.toml` & `notebook_setup-1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 description = 'Tools to setup and configure jupyter notebooks (ipynb files) with line and cell magic'
 keywords = ["ipynb", "notebook", "jupyter", "line magic", "cell magic", "autoreload", "plotly render"]
 license = "MIT"
 name = "notebook_setup"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "1.1"
+version = "1.2"
 
 dependencies = ["ipython", "ipykernel"]
 
 [project.urls]
 homepage = "https://github.com/1081/notebook_setup"
 
 [tool.hatch.build.targets.wheel]
```

