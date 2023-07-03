# Comparing `tmp/poetry_jupyter_plugin-0.1.3.tar.gz` & `tmp/poetry_jupyter_plugin-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_jupyter_plugin-0.1.3.tar", max compression
+gzip compressed data, was "poetry_jupyter_plugin-0.1.4.tar", max compression
```

## Comparing `poetry_jupyter_plugin-0.1.3.tar` & `poetry_jupyter_plugin-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-01-12 17:13:13.310476 poetry_jupyter_plugin-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     2197 2023-01-13 03:54:11.575612 poetry_jupyter_plugin-0.1.3/README.md
--rw-r--r--   0        0        0        1 2023-01-12 17:15:58.938110 poetry_jupyter_plugin-0.1.3/poetry_jupyter_plugin/__init__.py
--rw-r--r--   0        0        0   112230 2023-01-13 03:06:16.977001 poetry_jupyter_plugin-0.1.3/poetry_jupyter_plugin/assets/poetry.png
--rw-r--r--   0        0        0     2923 2023-01-12 22:07:07.766576 poetry_jupyter_plugin-0.1.3/poetry_jupyter_plugin/assets/poetry.svg
--rw-r--r--   0        0        0     7179 2023-01-13 03:59:18.908818 poetry_jupyter_plugin-0.1.3/poetry_jupyter_plugin/plugin.py
--rw-r--r--   0        0        0      918 2023-01-13 04:23:45.271558 poetry_jupyter_plugin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3258 1970-01-01 00:00:00.000000 poetry_jupyter_plugin-0.1.3/setup.py
--rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 poetry_jupyter_plugin-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-01-12 17:13:13.310476 poetry_jupyter_plugin-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     2197 2023-01-13 03:54:11.575612 poetry_jupyter_plugin-0.1.4/README.md
+-rw-r--r--   0        0        0       22 2023-07-03 20:34:36.552961 poetry_jupyter_plugin-0.1.4/poetry_jupyter_plugin/__init__.py
+-rw-r--r--   0        0        0   112230 2023-01-13 03:06:16.977001 poetry_jupyter_plugin-0.1.4/poetry_jupyter_plugin/assets/poetry.png
+-rw-r--r--   0        0        0     2923 2023-01-12 22:07:07.766576 poetry_jupyter_plugin-0.1.4/poetry_jupyter_plugin/assets/poetry.svg
+-rw-r--r--   0        0        0     7220 2023-07-03 20:34:09.726887 poetry_jupyter_plugin-0.1.4/poetry_jupyter_plugin/plugin.py
+-rw-r--r--   0        0        0      918 2023-07-03 20:34:40.395044 poetry_jupyter_plugin-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 poetry_jupyter_plugin-0.1.4/PKG-INFO
```

### Comparing `poetry_jupyter_plugin-0.1.3/LICENSE.txt` & `poetry_jupyter_plugin-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `poetry_jupyter_plugin-0.1.3/README.md` & `poetry_jupyter_plugin-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `poetry_jupyter_plugin-0.1.3/poetry_jupyter_plugin/assets/poetry.png` & `poetry_jupyter_plugin-0.1.4/poetry_jupyter_plugin/assets/poetry.png`

 * *Files identical despite different names*

### Comparing `poetry_jupyter_plugin-0.1.3/poetry_jupyter_plugin/assets/poetry.svg` & `poetry_jupyter_plugin-0.1.4/poetry_jupyter_plugin/assets/poetry.svg`

 * *Files identical despite different names*

### Comparing `poetry_jupyter_plugin-0.1.3/poetry_jupyter_plugin/plugin.py` & `poetry_jupyter_plugin-0.1.4/poetry_jupyter_plugin/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from functools import reduce
 from pprint import pprint
+from pathlib import Path
 import tempfile
 import os
 import json
 import platform
 
 import asset
 from cleo.commands.command import Command
@@ -58,15 +59,15 @@
 
 
     def has_ipykernel(self):
         venv = self.get_venv()
         if venv is None:
             return False
         
-        ipykernels = venv.site_packages.find('ipykernel')
+        ipykernels = venv.site_packages.find(Path('ipykernel'))
 
         if len(ipykernels) == 0:
             return False
 
         return True
 
 
@@ -88,15 +89,15 @@
             return None
 
         for key, obj in kernels.items():
             argv = optional_chain(obj, 'spec.argv')
             if argv is None:
                 continue
 
-            if argv[0] == venv.python:
+            if argv[0] == str(venv.python):
                 obj['key'] = key
                 return obj
 
         return None
 
     def get_preferred_spec_prefix(self):
         # fixes on macOS
@@ -162,15 +163,15 @@
             return 1
 
 
 
         with tempfile.TemporaryDirectory() as tmpdir:
             spec = {
                  'argv': [
-                     self.get_venv().python,
+                     str(self.get_venv().python),
                      '-m',
                      'ipykernel_launcher',
                      '-f',
                      '{connection_file}'
                  ],
                  'display_name': kernel['display'],
                  'env': {},
```

### Comparing `poetry_jupyter_plugin-0.1.3/pyproject.toml` & `poetry_jupyter_plugin-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-jupyter-plugin"
-version = "0.1.3"
+version = "0.1.4"
 description = "Poetry plugin to manage Jupyter kernels"
 authors = ["Patrick Kage <patrick.r.kage@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pkage/poetry-jupyter-plugin"
 repository = "https://github.com/pkage/poetry-jupyter-plugin"
 packages = [{include = "poetry_jupyter_plugin"}]
```

### Comparing `poetry_jupyter_plugin-0.1.3/setup.py` & `poetry_jupyter_plugin-0.1.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,99 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: poetry-jupyter-plugin
+Version: 0.1.4
+Summary: Poetry plugin to manage Jupyter kernels
+Home-page: https://github.com/pkage/poetry-jupyter-plugin
+License: MIT
+Keywords: poetry,poetry-plugin,plugin,jupyter,jupyter-kernel
+Author: Patrick Kage
+Author-email: patrick.r.kage@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Framework :: Jupyter
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development
+Classifier: Topic :: Utilities
+Requires-Dist: asset (>=0.6.13,<0.7.0)
+Requires-Dist: jupyter-client (>=7.4.8,<8.0.0)
+Requires-Dist: poetry (>=1.3.2,<2.0.0)
+Project-URL: Repository, https://github.com/pkage/poetry-jupyter-plugin
+Description-Content-Type: text/markdown
+
+# poetry-jupyter-plugin
+
+## overview
+
+This is a really simple plugin to allow you to install your
+[Poetry](https://python-poetry.org) virtual environment as a
+[Jupyter](https://jupyter.org) kernel. You may wish to do this to keep your
+dependencies locked down for reproducible notebooks, or to set up a single
+"data science" notebook for one-off calculations without fiddling about with
+installing packages globally or dealing with `ipykernel` directly.
+
+## getting started
+
+Install the plugin with:
+
+```sh
+$ poetry self add poetry-jupyter-plugin
+```
+
+Then, from within your poetry project:
+
+```sh
+$ poetry install ipykernel -G dev
+$ poetry jupyter install
+```
+
+Remove the kernelspec with:
+
+```sh
+$ poetry jupyter remove
+```
+
+### configuration
+
+By default, the installed kernel will use the name of the project and a default
+Poetry icon. To configure these options, add this block to your `pyproject.toml`:
+
+```toml
+[tool.jupyter.kernel]
+name = "my-cool-kernel"
+display = "My cool kernel"
+icon = "/path/to/icon.png"
+```
+
+## prior art
+
+There are other projects in this space, notably Pathbird's [`poetry-kernel`].
+`poetry-kernel` installs a single kernelspec globally which then patches the
+virtualenv based on the specific project folder that you're running Jupyter in.
+This has some pros and cons over this project.
+
+Pros:
+
+1. Single kernelspec, avoiding polluting the kernelspec list with lots of specs.
+2. Easy context switching between projects.
+
+Cons:
+
+1. Notebooks have to be in the same folder (or a subfolder from) as the
+   `pyproject.toml` folder.
+2. Requires forwarding signals from the launcher into Jupyter, introducing a
+   layer of complexity and is brittle to changes in Jupyter protocol/underlying
+   OS.
+3. Implicit dependency on `ipykernel`, and may fail to start without it.
+
+In contrast, this project installs one kernelspec per virtualenv and leaves it
+up to Jupyter to launch the kernel normally without interception. This design
+decision also allows multiple projects to be based out of one kernel.
+Additionally, the tool checks for the existence of `ipykernel` to make sure
+that the kernel can be installed properly.
 
-packages = \
-['poetry_jupyter_plugin']
+## who?
 
-package_data = \
-{'': ['*'], 'poetry_jupyter_plugin': ['assets/*']}
+This was written by [patrick kage](//ka.ge).
 
-install_requires = \
-['asset>=0.6.13,<0.7.0', 'jupyter-client>=7.4.8,<8.0.0', 'poetry>=1.3.2,<2.0.0']
-
-entry_points = \
-{'poetry.application.plugin': ['jupyter-command = '
-                               'poetry_jupyter_plugin.plugin:JupyterKernelPlugin']}
-
-setup_kwargs = {
-    'name': 'poetry-jupyter-plugin',
-    'version': '0.1.3',
-    'description': 'Poetry plugin to manage Jupyter kernels',
-    'long_description': '# poetry-jupyter-plugin\n\n## overview\n\nThis is a really simple plugin to allow you to install your\n[Poetry](https://python-poetry.org) virtual environment as a\n[Jupyter](https://jupyter.org) kernel. You may wish to do this to keep your\ndependencies locked down for reproducible notebooks, or to set up a single\n"data science" notebook for one-off calculations without fiddling about with\ninstalling packages globally or dealing with `ipykernel` directly.\n\n## getting started\n\nInstall the plugin with:\n\n```sh\n$ poetry self add poetry-jupyter-plugin\n```\n\nThen, from within your poetry project:\n\n```sh\n$ poetry install ipykernel -G dev\n$ poetry jupyter install\n```\n\nRemove the kernelspec with:\n\n```sh\n$ poetry jupyter remove\n```\n\n### configuration\n\nBy default, the installed kernel will use the name of the project and a default\nPoetry icon. To configure these options, add this block to your `pyproject.toml`:\n\n```toml\n[tool.jupyter.kernel]\nname = "my-cool-kernel"\ndisplay = "My cool kernel"\nicon = "/path/to/icon.png"\n```\n\n## prior art\n\nThere are other projects in this space, notably Pathbird\'s [`poetry-kernel`].\n`poetry-kernel` installs a single kernelspec globally which then patches the\nvirtualenv based on the specific project folder that you\'re running Jupyter in.\nThis has some pros and cons over this project.\n\nPros:\n\n1. Single kernelspec, avoiding polluting the kernelspec list with lots of specs.\n2. Easy context switching between projects.\n\nCons:\n\n1. Notebooks have to be in the same folder (or a subfolder from) as the\n   `pyproject.toml` folder.\n2. Requires forwarding signals from the launcher into Jupyter, introducing a\n   layer of complexity and is brittle to changes in Jupyter protocol/underlying\n   OS.\n3. Implicit dependency on `ipykernel`, and may fail to start without it.\n\nIn contrast, this project installs one kernelspec per virtualenv and leaves it\nup to Jupyter to launch the kernel normally without interception. This design\ndecision also allows multiple projects to be based out of one kernel.\nAdditionally, the tool checks for the existence of `ipykernel` to make sure\nthat the kernel can be installed properly.\n\n## who?\n\nThis was written by [patrick kage](//ka.ge).\n',
-    'author': 'Patrick Kage',
-    'author_email': 'patrick.r.kage@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/pkage/poetry-jupyter-plugin',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

