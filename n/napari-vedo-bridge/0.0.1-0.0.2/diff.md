# Comparing `tmp/napari-vedo-bridge-0.0.1.tar.gz` & `tmp/napari-vedo-bridge-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-vedo-bridge-0.0.1.tar", last modified: Mon Jul  3 15:31:54 2023, max compression
+gzip compressed data, was "napari-vedo-bridge-0.0.2.tar", last modified: Mon Jul  3 15:51:08 2023, max compression
```

## Comparing `napari-vedo-bridge-0.0.1.tar` & `napari-vedo-bridge-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 15:31:54.329509 napari-vedo-bridge-0.0.1/
--rw-rw-rw-   0        0        0     1533 2023-06-08 13:53:21.000000 napari-vedo-bridge-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      138 2023-06-12 09:46:01.000000 napari-vedo-bridge-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4547 2023-07-03 15:31:54.329509 napari-vedo-bridge-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3572 2023-06-15 11:58:49.000000 napari-vedo-bridge-0.0.1/README.md
--rw-rw-rw-   0        0        0     1233 2023-06-08 13:53:21.000000 napari-vedo-bridge-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1519 2023-07-03 15:31:54.329509 napari-vedo-bridge-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 15:31:54.204491 napari-vedo-bridge-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 15:31:54.267001 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge/
--rw-rw-rw-   0        0        0       21 2023-06-08 14:00:07.000000 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge/__init__.py
--rw-rw-rw-   0        0        0     7895 2023-06-26 14:28:46.000000 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge/_cutter_widget.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:31:54.313870 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge/_tests/
--rw-rw-rw-   0        0        0        0 2023-06-08 13:53:21.000000 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge/_tests/__init__.py
--rw-rw-rw-   0        0        0     1906 2023-07-03 15:31:11.000000 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge/_tests/test_widget.py
--rw-rw-rw-   0        0        0      345 2023-06-08 13:58:19.000000 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge/napari.yaml
--rw-rw-rw-   0        0        0     2945 2023-06-26 12:59:23.000000 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge/vedo_extension.ui
-drwxrwxrwx   0        0        0        0 2023-07-03 15:31:54.313870 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge.egg-info/
--rw-rw-rw-   0        0        0     4547 2023-07-03 15:31:54.000000 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2023-07-03 15:31:54.000000 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 15:31:54.000000 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-07-03 15:31:54.000000 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       91 2023-07-03 15:31:54.000000 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-03 15:31:54.000000 napari-vedo-bridge-0.0.1/src/napari_vedo_bridge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:51:08.380338 napari-vedo-bridge-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-03 15:51:08.380338 napari-vedo-bridge-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-03 15:51:08.380338 napari-vedo-bridge-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:51:08.376338 napari-vedo-bridge-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:51:08.380338 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/_cutter_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:51:08.380338 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-03 15:50:51.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/vedo_extension.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:51:08.380338 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-03 15:51:08.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-03 15:51:08.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:51:08.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-03 15:51:08.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-03 15:51:08.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 15:51:08.000000 napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/top_level.txt
```

### Comparing `napari-vedo-bridge-0.0.1/LICENSE` & `napari-vedo-bridge-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-
-Copyright (c) 2023, Johannes Soltwedel, Marco Musy
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+Copyright (c) 2023, Johannes Soltwedel, Marco Musy
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `napari-vedo-bridge-0.0.1/PKG-INFO` & `napari-vedo-bridge-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-Metadata-Version: 2.1
-Name: napari-vedo-bridge
-Version: 0.0.1
-Summary: Transfer mesh data between napari and vedo for interactive processing
-Author: Johannes Soltwedel, Marco Musy
-Author-email: johannes_richard.soltwedel@tu-dresden.de
-License: BSD-3-Clause
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: napari
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
-# napari-vedo-bridge
-
-[![License BSD-3](https://img.shields.io/pypi/l/napari-vedo-bridge.svg?color=green)](https://github.com/jo-mueller/napari-vedo-bridge/raw/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/napari-vedo-bridge.svg?color=green)](https://pypi.org/project/napari-vedo-bridge)
-[![Python Version](https://img.shields.io/pypi/pyversions/napari-vedo-bridge.svg?color=green)](https://python.org)
-[![tests](https://github.com/jo-mueller/napari-vedo-bridge/workflows/tests/badge.svg)](https://github.com/jo-mueller/napari-vedo-bridge/actions)
-[![codecov](https://codecov.io/gh/jo-mueller/napari-vedo-bridge/branch/main/graph/badge.svg)](https://codecov.io/gh/jo-mueller/napari-vedo-bridge)
-[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-vedo-bridge)](https://napari-hub.org/plugins/napari-vedo-bridge)
-
-To be able to use interactive processing of meshes in napari, this plugin provides a bridge to the vedo library. It allows to transfer meshes between napari and vedo and to use the interactive processing capabilities of vedo in napari. 
-
-## Interactive mesh cutting
-To interactively cut meshes in the napari-vedo MeshCutter, install the plugin (see below) and open the plugin it from the napari plugins menu (`Plugins > Mesh Cutter (napari-vedo-bridge)`). 
-
-To cut meshes you can use the following cutters:
-- `PlaneCutter`: cuts a mesh with a plane
-- `SphereCutter`: cuts a mesh with a sphere
-- `BoxCutter`: cuts a mesh with a box
-
-![](docs/imgs/screenshot_box_cutter.png)
-
-To send and get data into and from the plugin, you can:
-
-- Retrieve the current mesh from napari (click `Retrieve mesh from napari`) - this imports the **currently selected mesh layer** from napari
-- Load a mesh from file (click `Load mesh`)
-- Send a mesh to napari (click `Send back to napari`) - this creates a new mesh layer in napari
-
-
-
-
-----------------------------------
-
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
-
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/stable/plugins/index.html
--->
-
-## Installation
-
-You can install `napari-vedo-bridge` via [pip]:
-
-    pip install napari-vedo-bridge
-
-
-
-
-## Contributing
-
-Contributions are very welcome. Tests can be run with [tox], please ensure
-the coverage at least stays the same before you submit a pull request.
-
-## License
-
-Distributed under the terms of the [BSD-3] license,
-"napari-vedo-bridge" is free and open source software
-
-## Issues
-
-If you encounter any problems, please [file an issue] along with a detailed description.
-
-[napari]: https://github.com/napari/napari
-[Cookiecutter]: https://github.com/audreyr/cookiecutter
-[@napari]: https://github.com/napari
-[MIT]: http://opensource.org/licenses/MIT
-[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
-[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
-[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-
-[napari]: https://github.com/napari/napari
-[tox]: https://tox.readthedocs.io/en/latest/
-[pip]: https://pypi.org/project/pip/
-[PyPI]: https://pypi.org/
+Metadata-Version: 2.1
+Name: napari-vedo-bridge
+Version: 0.0.2
+Summary: Transfer mesh data between napari and vedo for interactive processing
+Author: Johannes Soltwedel, Marco Musy
+Author-email: johannes_richard.soltwedel@tu-dresden.de
+License: BSD-3-Clause
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Framework :: napari
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE
+
+# napari-vedo-bridge
+
+[![License BSD-3](https://img.shields.io/pypi/l/napari-vedo-bridge.svg?color=green)](https://github.com/jo-mueller/napari-vedo-bridge/raw/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/napari-vedo-bridge.svg?color=green)](https://pypi.org/project/napari-vedo-bridge)
+[![Python Version](https://img.shields.io/pypi/pyversions/napari-vedo-bridge.svg?color=green)](https://python.org)
+[![tests](https://github.com/jo-mueller/napari-vedo-bridge/workflows/tests/badge.svg)](https://github.com/jo-mueller/napari-vedo-bridge/actions)
+[![codecov](https://codecov.io/gh/jo-mueller/napari-vedo-bridge/branch/main/graph/badge.svg)](https://codecov.io/gh/jo-mueller/napari-vedo-bridge)
+[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-vedo-bridge)](https://napari-hub.org/plugins/napari-vedo-bridge)
+
+To be able to use interactive processing of meshes in napari, this plugin provides a bridge to the vedo library. It allows to transfer meshes between napari and vedo and to use the interactive processing capabilities of vedo in napari. 
+
+## Interactive mesh cutting
+To interactively cut meshes in the napari-vedo MeshCutter, install the plugin (see below) and open the plugin it from the napari plugins menu (`Plugins > Mesh Cutter (napari-vedo-bridge)`). 
+
+To cut meshes you can use the following cutters:
+- `PlaneCutter`: cuts a mesh with a plane
+- `SphereCutter`: cuts a mesh with a sphere
+- `BoxCutter`: cuts a mesh with a box
+
+![](docs/imgs/screenshot_box_cutter.png)
+
+To send and get data into and from the plugin, you can:
+
+- Retrieve the current mesh from napari (click `Retrieve mesh from napari`) - this imports the **currently selected mesh layer** from napari
+- Load a mesh from file (click `Load mesh`)
+- Send a mesh to napari (click `Send back to napari`) - this creates a new mesh layer in napari
+
+
+
+
+----------------------------------
+
+This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
+
+<!--
+Don't miss the full getting started guide to set up your new package:
+https://github.com/napari/cookiecutter-napari-plugin#getting-started
+
+and review the napari docs for plugin developers:
+https://napari.org/stable/plugins/index.html
+-->
+
+## Installation
+
+You can install `napari-vedo-bridge` via [pip]:
+
+    pip install napari-vedo-bridge
+
+
+
+
+## Contributing
+
+Contributions are very welcome. Tests can be run with [tox], please ensure
+the coverage at least stays the same before you submit a pull request.
+
+## License
+
+Distributed under the terms of the [BSD-3] license,
+"napari-vedo-bridge" is free and open source software
+
+## Issues
+
+If you encounter any problems, please [file an issue] along with a detailed description.
+
+[napari]: https://github.com/napari/napari
+[Cookiecutter]: https://github.com/audreyr/cookiecutter
+[@napari]: https://github.com/napari
+[MIT]: http://opensource.org/licenses/MIT
+[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
+[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
+[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
+[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
+[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
+[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
+
+[napari]: https://github.com/napari/napari
+[tox]: https://tox.readthedocs.io/en/latest/
+[pip]: https://pypi.org/project/pip/
+[PyPI]: https://pypi.org/
```

### Comparing `napari-vedo-bridge-0.0.1/README.md` & `napari-vedo-bridge-0.0.2/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-# napari-vedo-bridge
-
-[![License BSD-3](https://img.shields.io/pypi/l/napari-vedo-bridge.svg?color=green)](https://github.com/jo-mueller/napari-vedo-bridge/raw/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/napari-vedo-bridge.svg?color=green)](https://pypi.org/project/napari-vedo-bridge)
-[![Python Version](https://img.shields.io/pypi/pyversions/napari-vedo-bridge.svg?color=green)](https://python.org)
-[![tests](https://github.com/jo-mueller/napari-vedo-bridge/workflows/tests/badge.svg)](https://github.com/jo-mueller/napari-vedo-bridge/actions)
-[![codecov](https://codecov.io/gh/jo-mueller/napari-vedo-bridge/branch/main/graph/badge.svg)](https://codecov.io/gh/jo-mueller/napari-vedo-bridge)
-[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-vedo-bridge)](https://napari-hub.org/plugins/napari-vedo-bridge)
-
-To be able to use interactive processing of meshes in napari, this plugin provides a bridge to the vedo library. It allows to transfer meshes between napari and vedo and to use the interactive processing capabilities of vedo in napari. 
-
-## Interactive mesh cutting
-To interactively cut meshes in the napari-vedo MeshCutter, install the plugin (see below) and open the plugin it from the napari plugins menu (`Plugins > Mesh Cutter (napari-vedo-bridge)`). 
-
-To cut meshes you can use the following cutters:
-- `PlaneCutter`: cuts a mesh with a plane
-- `SphereCutter`: cuts a mesh with a sphere
-- `BoxCutter`: cuts a mesh with a box
-
-![](docs/imgs/screenshot_box_cutter.png)
-
-To send and get data into and from the plugin, you can:
-
-- Retrieve the current mesh from napari (click `Retrieve mesh from napari`) - this imports the **currently selected mesh layer** from napari
-- Load a mesh from file (click `Load mesh`)
-- Send a mesh to napari (click `Send back to napari`) - this creates a new mesh layer in napari
-
-
-
-
-----------------------------------
-
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
-
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/stable/plugins/index.html
--->
-
-## Installation
-
-You can install `napari-vedo-bridge` via [pip]:
-
-    pip install napari-vedo-bridge
-
-
-
-
-## Contributing
-
-Contributions are very welcome. Tests can be run with [tox], please ensure
-the coverage at least stays the same before you submit a pull request.
-
-## License
-
-Distributed under the terms of the [BSD-3] license,
-"napari-vedo-bridge" is free and open source software
-
-## Issues
-
-If you encounter any problems, please [file an issue] along with a detailed description.
-
-[napari]: https://github.com/napari/napari
-[Cookiecutter]: https://github.com/audreyr/cookiecutter
-[@napari]: https://github.com/napari
-[MIT]: http://opensource.org/licenses/MIT
-[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
-[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
-[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-
-[napari]: https://github.com/napari/napari
-[tox]: https://tox.readthedocs.io/en/latest/
-[pip]: https://pypi.org/project/pip/
-[PyPI]: https://pypi.org/
+# napari-vedo-bridge
+
+[![License BSD-3](https://img.shields.io/pypi/l/napari-vedo-bridge.svg?color=green)](https://github.com/jo-mueller/napari-vedo-bridge/raw/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/napari-vedo-bridge.svg?color=green)](https://pypi.org/project/napari-vedo-bridge)
+[![Python Version](https://img.shields.io/pypi/pyversions/napari-vedo-bridge.svg?color=green)](https://python.org)
+[![tests](https://github.com/jo-mueller/napari-vedo-bridge/workflows/tests/badge.svg)](https://github.com/jo-mueller/napari-vedo-bridge/actions)
+[![codecov](https://codecov.io/gh/jo-mueller/napari-vedo-bridge/branch/main/graph/badge.svg)](https://codecov.io/gh/jo-mueller/napari-vedo-bridge)
+[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-vedo-bridge)](https://napari-hub.org/plugins/napari-vedo-bridge)
+
+To be able to use interactive processing of meshes in napari, this plugin provides a bridge to the vedo library. It allows to transfer meshes between napari and vedo and to use the interactive processing capabilities of vedo in napari. 
+
+## Interactive mesh cutting
+To interactively cut meshes in the napari-vedo MeshCutter, install the plugin (see below) and open the plugin it from the napari plugins menu (`Plugins > Mesh Cutter (napari-vedo-bridge)`). 
+
+To cut meshes you can use the following cutters:
+- `PlaneCutter`: cuts a mesh with a plane
+- `SphereCutter`: cuts a mesh with a sphere
+- `BoxCutter`: cuts a mesh with a box
+
+![](docs/imgs/screenshot_box_cutter.png)
+
+To send and get data into and from the plugin, you can:
+
+- Retrieve the current mesh from napari (click `Retrieve mesh from napari`) - this imports the **currently selected mesh layer** from napari
+- Load a mesh from file (click `Load mesh`)
+- Send a mesh to napari (click `Send back to napari`) - this creates a new mesh layer in napari
+
+
+
+
+----------------------------------
+
+This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
+
+<!--
+Don't miss the full getting started guide to set up your new package:
+https://github.com/napari/cookiecutter-napari-plugin#getting-started
+
+and review the napari docs for plugin developers:
+https://napari.org/stable/plugins/index.html
+-->
+
+## Installation
+
+You can install `napari-vedo-bridge` via [pip]:
+
+    pip install napari-vedo-bridge
+
+
+
+
+## Contributing
+
+Contributions are very welcome. Tests can be run with [tox], please ensure
+the coverage at least stays the same before you submit a pull request.
+
+## License
+
+Distributed under the terms of the [BSD-3] license,
+"napari-vedo-bridge" is free and open source software
+
+## Issues
+
+If you encounter any problems, please [file an issue] along with a detailed description.
+
+[napari]: https://github.com/napari/napari
+[Cookiecutter]: https://github.com/audreyr/cookiecutter
+[@napari]: https://github.com/napari
+[MIT]: http://opensource.org/licenses/MIT
+[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
+[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
+[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
+[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
+[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
+[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
+
+[napari]: https://github.com/napari/napari
+[tox]: https://tox.readthedocs.io/en/latest/
+[pip]: https://pypi.org/project/pip/
+[PyPI]: https://pypi.org/
```

### Comparing `napari-vedo-bridge-0.0.1/setup.cfg` & `napari-vedo-bridge-0.0.2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,92 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 206e 6170 6172 692d 7665 646f 2d62   = napari-vedo-b
-00000020: 7269 6467 650d 0a76 6572 7369 6f6e 203d  ridge..version =
-00000030: 2061 7474 723a 206e 6170 6172 695f 7665   attr: napari_ve
-00000040: 646f 5f62 7269 6467 652e 5f5f 7665 7273  do_bridge.__vers
-00000050: 696f 6e5f 5f0d 0a64 6573 6372 6970 7469  ion__..descripti
-00000060: 6f6e 203d 2054 7261 6e73 6665 7220 6d65  on = Transfer me
-00000070: 7368 2064 6174 6120 6265 7477 6565 6e20  sh data between 
-00000080: 6e61 7061 7269 2061 6e64 2076 6564 6f20  napari and vedo 
-00000090: 666f 7220 696e 7465 7261 6374 6976 6520  for interactive 
-000000a0: 7072 6f63 6573 7369 6e67 0d0a 6c6f 6e67  processing..long
-000000b0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-000000c0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000e0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-000000f0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a61  text/markdown..a
-00000100: 7574 686f 7220 3d20 4a6f 6861 6e6e 6573  uthor = Johannes
-00000110: 2053 6f6c 7477 6564 656c 2c20 4d61 7263   Soltwedel, Marc
-00000120: 6f20 4d75 7379 0d0a 6175 7468 6f72 5f65  o Musy..author_e
-00000130: 6d61 696c 203d 206a 6f68 616e 6e65 735f  mail = johannes_
-00000140: 7269 6368 6172 642e 736f 6c74 7765 6465  richard.soltwede
-00000150: 6c40 7475 2d64 7265 7364 656e 2e64 650d  l@tu-dresden.de.
-00000160: 0a6c 6963 656e 7365 203d 2042 5344 2d33  .license = BSD-3
-00000170: 2d43 6c61 7573 650d 0a6c 6963 656e 7365  -Clause..license
-00000180: 5f66 696c 6573 203d 204c 4943 454e 5345  _files = LICENSE
-00000190: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-000001a0: 0d0a 0944 6576 656c 6f70 6d65 6e74 2053  ...Development S
-000001b0: 7461 7475 7320 3a3a 2032 202d 2050 7265  tatus :: 2 - Pre
-000001c0: 2d41 6c70 6861 0d0a 0946 7261 6d65 776f  -Alpha...Framewo
-000001d0: 726b 203a 3a20 6e61 7061 7269 0d0a 0949  rk :: napari...I
-000001e0: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
-000001f0: 203a 3a20 4465 7665 6c6f 7065 7273 0d0a   :: Developers..
-00000200: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-00000210: 4170 7072 6f76 6564 203a 3a20 4253 4420  Approved :: BSD 
-00000220: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
-00000230: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-00000240: 2049 6e64 6570 656e 6465 6e74 0d0a 0950   Independent...P
-00000250: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000260: 6167 6520 3a3a 2050 7974 686f 6e0d 0a09  age :: Python...
-00000270: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000280: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000290: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
-000002a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002b0: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
-000002c0: 790d 0a09 5072 6f67 7261 6d6d 696e 6720  y...Programming 
-000002d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002e0: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
-000002f0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000300: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000310: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
-00000320: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000330: 6f6e 203a 3a20 332e 3130 0d0a 0954 6f70  on :: 3.10...Top
-00000340: 6963 203a 3a20 5363 6965 6e74 6966 6963  ic :: Scientific
-00000350: 2f45 6e67 696e 6565 7269 6e67 203a 3a20  /Engineering :: 
-00000360: 496d 6167 6520 5072 6f63 6573 7369 6e67  Image Processing
-00000370: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
-00000380: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-00000390: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-000003a0: 7320 3d20 0d0a 096e 756d 7079 0d0a 096d  s = ...numpy...m
-000003b0: 6167 6963 6775 690d 0a09 7174 7079 0d0a  agicgui...qtpy..
-000003c0: 0976 6564 6f3e 3d32 3032 332e 342e 360d  .vedo>=2023.4.6.
-000003d0: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-000003e0: 203d 203e 3d33 2e38 0d0a 696e 636c 7564   = >=3.8..includ
-000003f0: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
-00000400: 2054 7275 650d 0a70 6163 6b61 6765 5f64   True..package_d
-00000410: 6972 203d 200d 0a09 3d73 7263 0d0a 0d0a  ir = ...=src....
-00000420: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000430: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-00000440: 2073 7263 0d0a 0d0a 5b6f 7074 696f 6e73   src....[options
-00000450: 2e65 6e74 7279 5f70 6f69 6e74 735d 0d0a  .entry_points]..
-00000460: 6e61 7061 7269 2e6d 616e 6966 6573 7420  napari.manifest 
-00000470: 3d20 0d0a 096e 6170 6172 692d 7665 646f  = ...napari-vedo
-00000480: 2d62 7269 6467 6520 3d20 6e61 7061 7269  -bridge = napari
-00000490: 5f76 6564 6f5f 6272 6964 6765 3a6e 6170  _vedo_bridge:nap
-000004a0: 6172 692e 7961 6d6c 0d0a 0d0a 5b6f 7074  ari.yaml....[opt
-000004b0: 696f 6e73 2e65 7874 7261 735f 7265 7175  ions.extras_requ
-000004c0: 6972 655d 0d0a 7465 7374 696e 6720 3d20  ire]..testing = 
-000004d0: 0d0a 0974 6f78 0d0a 0970 7974 6573 7420  ...tox...pytest 
-000004e0: 2023 2068 7474 7073 3a2f 2f64 6f63 732e   # https://docs.
-000004f0: 7079 7465 7374 2e6f 7267 2f65 6e2f 6c61  pytest.org/en/la
-00000500: 7465 7374 2f63 6f6e 7465 6e74 732e 6874  test/contents.ht
-00000510: 6d6c 0d0a 0970 7974 6573 742d 636f 7620  ml...pytest-cov 
-00000520: 2023 2068 7474 7073 3a2f 2f70 7974 6573   # https://pytes
-00000530: 742d 636f 762e 7265 6164 7468 6564 6f63  t-cov.readthedoc
-00000540: 732e 696f 2f65 6e2f 6c61 7465 7374 2f0d  s.io/en/latest/.
-00000550: 0a09 7079 7465 7374 2d71 7420 2023 2068  ..pytest-qt  # h
-00000560: 7474 7073 3a2f 2f70 7974 6573 742d 7174  ttps://pytest-qt
-00000570: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00000580: 656e 2f6c 6174 6573 742f 0d0a 096e 6170  en/latest/...nap
-00000590: 6172 690d 0a09 7079 7174 350d 0a0d 0a5b  ari...pyqt5....[
-000005a0: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
-000005b0: 6461 7461 5d0d 0a2a 203d 202a 2e79 616d  data]..* = *.yam
-000005c0: 6c0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  l....[egg_info].
-000005d0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-000005e0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6e61 7061 7269 2d76 6564 6f2d 6272  = napari-vedo-br
+00000020: 6964 6765 0a76 6572 7369 6f6e 203d 2061  idge.version = a
+00000030: 7474 723a 206e 6170 6172 695f 7665 646f  ttr: napari_vedo
+00000040: 5f62 7269 6467 652e 5f5f 7665 7273 696f  _bridge.__versio
+00000050: 6e5f 5f0a 6465 7363 7269 7074 696f 6e20  n__.description 
+00000060: 3d20 5472 616e 7366 6572 206d 6573 6820  = Transfer mesh 
+00000070: 6461 7461 2062 6574 7765 656e 206e 6170  data between nap
+00000080: 6172 6920 616e 6420 7665 646f 2066 6f72  ari and vedo for
+00000090: 2069 6e74 6572 6163 7469 7665 2070 726f   interactive pro
+000000a0: 6365 7373 696e 670a 6c6f 6e67 5f64 6573  cessing.long_des
+000000b0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
+000000c0: 2052 4541 444d 452e 6d64 0a6c 6f6e 675f   README.md.long_
+000000d0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
+000000e0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
+000000f0: 6d61 726b 646f 776e 0a61 7574 686f 7220  markdown.author 
+00000100: 3d20 4a6f 6861 6e6e 6573 2053 6f6c 7477  = Johannes Soltw
+00000110: 6564 656c 2c20 4d61 7263 6f20 4d75 7379  edel, Marco Musy
+00000120: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
+00000130: 6a6f 6861 6e6e 6573 5f72 6963 6861 7264  johannes_richard
+00000140: 2e73 6f6c 7477 6564 656c 4074 752d 6472  .soltwedel@tu-dr
+00000150: 6573 6465 6e2e 6465 0a6c 6963 656e 7365  esden.de.license
+00000160: 203d 2042 5344 2d33 2d43 6c61 7573 650a   = BSD-3-Clause.
+00000170: 6c69 6365 6e73 655f 6669 6c65 7320 3d20  license_files = 
+00000180: 4c49 4345 4e53 450a 636c 6173 7369 6669  LICENSE.classifi
+00000190: 6572 7320 3d20 0a09 4465 7665 6c6f 706d  ers = ..Developm
+000001a0: 656e 7420 5374 6174 7573 203a 3a20 3220  ent Status :: 2 
+000001b0: 2d20 5072 652d 416c 7068 610a 0946 7261  - Pre-Alpha..Fra
+000001c0: 6d65 776f 726b 203a 3a20 6e61 7061 7269  mework :: napari
+000001d0: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
+000001e0: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
+000001f0: 730a 094c 6963 656e 7365 203a 3a20 4f53  s..License :: OS
+00000200: 4920 4170 7072 6f76 6564 203a 3a20 4253  I Approved :: BS
+00000210: 4420 4c69 6365 6e73 650a 094f 7065 7261  D License..Opera
+00000220: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+00000230: 5320 496e 6465 7065 6e64 656e 740a 0950  S Independent..P
+00000240: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000250: 6167 6520 3a3a 2050 7974 686f 6e0a 0950  age :: Python..P
+00000260: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000270: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000280: 2033 0a09 5072 6f67 7261 6d6d 696e 6720   3..Programming 
+00000290: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002a0: 6f6e 203a 3a20 3320 3a3a 204f 6e6c 790a  on :: 3 :: Only.
+000002b0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000002c0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000002d0: 3a3a 2033 2e38 0a09 5072 6f67 7261 6d6d  :: 3.8..Programm
+000002e0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002f0: 5079 7468 6f6e 203a 3a20 332e 390a 0950  Python :: 3.9..P
+00000300: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000310: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000320: 2033 2e31 300a 0954 6f70 6963 203a 3a20   3.10..Topic :: 
+00000330: 5363 6965 6e74 6966 6963 2f45 6e67 696e  Scientific/Engin
+00000340: 6565 7269 6e67 203a 3a20 496d 6167 6520  eering :: Image 
+00000350: 5072 6f63 6573 7369 6e67 0a0a 5b6f 7074  Processing..[opt
+00000360: 696f 6e73 5d0a 7061 636b 6167 6573 203d  ions].packages =
+00000370: 2066 696e 643a 0a69 6e73 7461 6c6c 5f72   find:.install_r
+00000380: 6571 7569 7265 7320 3d20 0a09 6e75 6d70  equires = ..nump
+00000390: 790a 096d 6167 6963 6775 690a 0971 7470  y..magicgui..qtp
+000003a0: 790a 0976 6564 6f3e 3d32 3032 332e 342e  y..vedo>=2023.4.
+000003b0: 360a 7079 7468 6f6e 5f72 6571 7569 7265  6.python_require
+000003c0: 7320 3d20 3e3d 332e 380a 696e 636c 7564  s = >=3.8.includ
+000003d0: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
+000003e0: 2054 7275 650a 7061 636b 6167 655f 6469   True.package_di
+000003f0: 7220 3d20 0a09 3d73 7263 0a0a 5b6f 7074  r = ..=src..[opt
+00000400: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+00000410: 6e64 5d0a 7768 6572 6520 3d20 7372 630a  nd].where = src.
+00000420: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
+00000430: 706f 696e 7473 5d0a 6e61 7061 7269 2e6d  points].napari.m
+00000440: 616e 6966 6573 7420 3d20 0a09 6e61 7061  anifest = ..napa
+00000450: 7269 2d76 6564 6f2d 6272 6964 6765 203d  ri-vedo-bridge =
+00000460: 206e 6170 6172 695f 7665 646f 5f62 7269   napari_vedo_bri
+00000470: 6467 653a 6e61 7061 7269 2e79 616d 6c0a  dge:napari.yaml.
+00000480: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
+00000490: 5f72 6571 7569 7265 5d0a 7465 7374 696e  _require].testin
+000004a0: 6720 3d20 0a09 746f 780a 0970 7974 6573  g = ..tox..pytes
+000004b0: 7420 2023 2068 7474 7073 3a2f 2f64 6f63  t  # https://doc
+000004c0: 732e 7079 7465 7374 2e6f 7267 2f65 6e2f  s.pytest.org/en/
+000004d0: 6c61 7465 7374 2f63 6f6e 7465 6e74 732e  latest/contents.
+000004e0: 6874 6d6c 0a09 7079 7465 7374 2d63 6f76  html..pytest-cov
+000004f0: 2020 2320 6874 7470 733a 2f2f 7079 7465    # https://pyte
+00000500: 7374 2d63 6f76 2e72 6561 6474 6865 646f  st-cov.readthedo
+00000510: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000520: 0a09 7079 7465 7374 2d71 7420 2023 2068  ..pytest-qt  # h
+00000530: 7474 7073 3a2f 2f70 7974 6573 742d 7174  ttps://pytest-qt
+00000540: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000550: 656e 2f6c 6174 6573 742f 0a09 6e61 7061  en/latest/..napa
+00000560: 7269 0a09 7079 7174 350a 0a5b 6f70 7469  ri..pyqt5..[opti
+00000570: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
+00000580: 5d0a 2a20 3d20 2a2e 7961 6d6c 0a0a 5b65  ].* = *.yaml..[e
+00000590: 6767 5f69 6e66 6f5d 0a74 6167 5f62 7569  gg_info].tag_bui
+000005a0: 6c64 203d 200a 7461 675f 6461 7465 203d  ld = .tag_date =
+000005b0: 2030 0a0a                                 0..
```

### Comparing `napari-vedo-bridge-0.0.1/src/napari_vedo_bridge/_tests/test_widget.py` & `napari-vedo-bridge-0.0.2/src/napari_vedo_bridge/_tests/test_widget.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-import numpy as np
-from .._cutter_widget import VedoCutter
-
-
-# make_napari_viewer is a pytest fixture that returns a napari viewer object
-def test_cutter_widget(make_napari_viewer):
-
-    # make viewer and add an image layer using our fixture
-    viewer = make_napari_viewer()
-
-    # create our widget, passing in the viewer
-    my_widget = VedoCutter(viewer)
-    viewer.window.add_dock_widget(my_widget, area='right')
-
-
-def test_get_from_napari(make_napari_viewer):
-    # Load the test mesh into the napari viewer
-    import vedo
-    viewer = make_napari_viewer()
-    mesh = vedo.load("https://vedo.embl.es/examples/data/270.vtk")
-    viewer.add_surface((mesh.points(), np.asarray(mesh.faces())), name="test_mesh")
-
-    vedo_cutter = VedoCutter(viewer)
-    vedo_cutter.get_from_napari()
-
-    # Assert that the mesh is loaded and displayed correctly in vedo
-    assert vedo_cutter.mesh is not None
-
-    n_layers = len(viewer.layers)
-    vedo_cutter.send_to_napari()
-    assert len(viewer.layers) == n_layers + 1
-
-
-def test_cutters(make_napari_viewer):
-    import vedo
-    viewer = make_napari_viewer()
-    mesh = vedo.load("https://vedo.embl.es/examples/data/270.vtk")
-    viewer.add_surface((mesh.points(), np.asarray(mesh.faces())), name="test_mesh")
-
-    vedo_cutter = VedoCutter(viewer)
-    vedo_cutter.get_from_napari()
-
-    vedo_cutter.buttonGroup.buttons()[0].click()
-    n_checked_buttons = len([b for b in vedo_cutter.buttonGroup.buttons() if b.isChecked()])
-    assert n_checked_buttons == 1
-
-    vedo_cutter.buttonGroup.buttons()[1].click()
-    n_checked_buttons = len([b for b in vedo_cutter.buttonGroup.buttons() if b.isChecked()])
-    assert n_checked_buttons == 1
-
-    vedo_cutter.buttonGroup.buttons()[2].click()
-    n_checked_buttons = len([b for b in vedo_cutter.buttonGroup.buttons() if b.isChecked()])
+import numpy as np
+from .._cutter_widget import VedoCutter
+
+
+# make_napari_viewer is a pytest fixture that returns a napari viewer object
+def test_cutter_widget(make_napari_viewer):
+
+    # make viewer and add an image layer using our fixture
+    viewer = make_napari_viewer()
+
+    # create our widget, passing in the viewer
+    my_widget = VedoCutter(viewer)
+    viewer.window.add_dock_widget(my_widget, area='right')
+
+
+def test_get_from_napari(make_napari_viewer):
+    # Load the test mesh into the napari viewer
+    import vedo
+    viewer = make_napari_viewer()
+    mesh = vedo.load("https://vedo.embl.es/examples/data/270.vtk")
+    viewer.add_surface((mesh.points(), np.asarray(mesh.faces())), name="test_mesh")
+
+    vedo_cutter = VedoCutter(viewer)
+    vedo_cutter.get_from_napari()
+
+    # Assert that the mesh is loaded and displayed correctly in vedo
+    assert vedo_cutter.mesh is not None
+
+    n_layers = len(viewer.layers)
+    vedo_cutter.send_to_napari()
+    assert len(viewer.layers) == n_layers + 1
+
+
+def test_cutters(make_napari_viewer):
+    import vedo
+    viewer = make_napari_viewer()
+    mesh = vedo.load("https://vedo.embl.es/examples/data/270.vtk")
+    viewer.add_surface((mesh.points(), np.asarray(mesh.faces())), name="test_mesh")
+
+    vedo_cutter = VedoCutter(viewer)
+    vedo_cutter.get_from_napari()
+
+    vedo_cutter.buttonGroup.buttons()[0].click()
+    n_checked_buttons = len([b for b in vedo_cutter.buttonGroup.buttons() if b.isChecked()])
+    assert n_checked_buttons == 1
+
+    vedo_cutter.buttonGroup.buttons()[1].click()
+    n_checked_buttons = len([b for b in vedo_cutter.buttonGroup.buttons() if b.isChecked()])
+    assert n_checked_buttons == 1
+
+    vedo_cutter.buttonGroup.buttons()[2].click()
+    n_checked_buttons = len([b for b in vedo_cutter.buttonGroup.buttons() if b.isChecked()])
     assert n_checked_buttons == 1
```

### Comparing `napari-vedo-bridge-0.0.1/src/napari_vedo_bridge.egg-info/PKG-INFO` & `napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-Metadata-Version: 2.1
-Name: napari-vedo-bridge
-Version: 0.0.1
-Summary: Transfer mesh data between napari and vedo for interactive processing
-Author: Johannes Soltwedel, Marco Musy
-Author-email: johannes_richard.soltwedel@tu-dresden.de
-License: BSD-3-Clause
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: napari
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
-# napari-vedo-bridge
-
-[![License BSD-3](https://img.shields.io/pypi/l/napari-vedo-bridge.svg?color=green)](https://github.com/jo-mueller/napari-vedo-bridge/raw/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/napari-vedo-bridge.svg?color=green)](https://pypi.org/project/napari-vedo-bridge)
-[![Python Version](https://img.shields.io/pypi/pyversions/napari-vedo-bridge.svg?color=green)](https://python.org)
-[![tests](https://github.com/jo-mueller/napari-vedo-bridge/workflows/tests/badge.svg)](https://github.com/jo-mueller/napari-vedo-bridge/actions)
-[![codecov](https://codecov.io/gh/jo-mueller/napari-vedo-bridge/branch/main/graph/badge.svg)](https://codecov.io/gh/jo-mueller/napari-vedo-bridge)
-[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-vedo-bridge)](https://napari-hub.org/plugins/napari-vedo-bridge)
-
-To be able to use interactive processing of meshes in napari, this plugin provides a bridge to the vedo library. It allows to transfer meshes between napari and vedo and to use the interactive processing capabilities of vedo in napari. 
-
-## Interactive mesh cutting
-To interactively cut meshes in the napari-vedo MeshCutter, install the plugin (see below) and open the plugin it from the napari plugins menu (`Plugins > Mesh Cutter (napari-vedo-bridge)`). 
-
-To cut meshes you can use the following cutters:
-- `PlaneCutter`: cuts a mesh with a plane
-- `SphereCutter`: cuts a mesh with a sphere
-- `BoxCutter`: cuts a mesh with a box
-
-![](docs/imgs/screenshot_box_cutter.png)
-
-To send and get data into and from the plugin, you can:
-
-- Retrieve the current mesh from napari (click `Retrieve mesh from napari`) - this imports the **currently selected mesh layer** from napari
-- Load a mesh from file (click `Load mesh`)
-- Send a mesh to napari (click `Send back to napari`) - this creates a new mesh layer in napari
-
-
-
-
-----------------------------------
-
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
-
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/stable/plugins/index.html
--->
-
-## Installation
-
-You can install `napari-vedo-bridge` via [pip]:
-
-    pip install napari-vedo-bridge
-
-
-
-
-## Contributing
-
-Contributions are very welcome. Tests can be run with [tox], please ensure
-the coverage at least stays the same before you submit a pull request.
-
-## License
-
-Distributed under the terms of the [BSD-3] license,
-"napari-vedo-bridge" is free and open source software
-
-## Issues
-
-If you encounter any problems, please [file an issue] along with a detailed description.
-
-[napari]: https://github.com/napari/napari
-[Cookiecutter]: https://github.com/audreyr/cookiecutter
-[@napari]: https://github.com/napari
-[MIT]: http://opensource.org/licenses/MIT
-[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
-[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
-[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-
-[napari]: https://github.com/napari/napari
-[tox]: https://tox.readthedocs.io/en/latest/
-[pip]: https://pypi.org/project/pip/
-[PyPI]: https://pypi.org/
+Metadata-Version: 2.1
+Name: napari-vedo-bridge
+Version: 0.0.2
+Summary: Transfer mesh data between napari and vedo for interactive processing
+Author: Johannes Soltwedel, Marco Musy
+Author-email: johannes_richard.soltwedel@tu-dresden.de
+License: BSD-3-Clause
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Framework :: napari
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE
+
+# napari-vedo-bridge
+
+[![License BSD-3](https://img.shields.io/pypi/l/napari-vedo-bridge.svg?color=green)](https://github.com/jo-mueller/napari-vedo-bridge/raw/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/napari-vedo-bridge.svg?color=green)](https://pypi.org/project/napari-vedo-bridge)
+[![Python Version](https://img.shields.io/pypi/pyversions/napari-vedo-bridge.svg?color=green)](https://python.org)
+[![tests](https://github.com/jo-mueller/napari-vedo-bridge/workflows/tests/badge.svg)](https://github.com/jo-mueller/napari-vedo-bridge/actions)
+[![codecov](https://codecov.io/gh/jo-mueller/napari-vedo-bridge/branch/main/graph/badge.svg)](https://codecov.io/gh/jo-mueller/napari-vedo-bridge)
+[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-vedo-bridge)](https://napari-hub.org/plugins/napari-vedo-bridge)
+
+To be able to use interactive processing of meshes in napari, this plugin provides a bridge to the vedo library. It allows to transfer meshes between napari and vedo and to use the interactive processing capabilities of vedo in napari. 
+
+## Interactive mesh cutting
+To interactively cut meshes in the napari-vedo MeshCutter, install the plugin (see below) and open the plugin it from the napari plugins menu (`Plugins > Mesh Cutter (napari-vedo-bridge)`). 
+
+To cut meshes you can use the following cutters:
+- `PlaneCutter`: cuts a mesh with a plane
+- `SphereCutter`: cuts a mesh with a sphere
+- `BoxCutter`: cuts a mesh with a box
+
+![](docs/imgs/screenshot_box_cutter.png)
+
+To send and get data into and from the plugin, you can:
+
+- Retrieve the current mesh from napari (click `Retrieve mesh from napari`) - this imports the **currently selected mesh layer** from napari
+- Load a mesh from file (click `Load mesh`)
+- Send a mesh to napari (click `Send back to napari`) - this creates a new mesh layer in napari
+
+
+
+
+----------------------------------
+
+This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
+
+<!--
+Don't miss the full getting started guide to set up your new package:
+https://github.com/napari/cookiecutter-napari-plugin#getting-started
+
+and review the napari docs for plugin developers:
+https://napari.org/stable/plugins/index.html
+-->
+
+## Installation
+
+You can install `napari-vedo-bridge` via [pip]:
+
+    pip install napari-vedo-bridge
+
+
+
+
+## Contributing
+
+Contributions are very welcome. Tests can be run with [tox], please ensure
+the coverage at least stays the same before you submit a pull request.
+
+## License
+
+Distributed under the terms of the [BSD-3] license,
+"napari-vedo-bridge" is free and open source software
+
+## Issues
+
+If you encounter any problems, please [file an issue] along with a detailed description.
+
+[napari]: https://github.com/napari/napari
+[Cookiecutter]: https://github.com/audreyr/cookiecutter
+[@napari]: https://github.com/napari
+[MIT]: http://opensource.org/licenses/MIT
+[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
+[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
+[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
+[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
+[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
+[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
+
+[napari]: https://github.com/napari/napari
+[tox]: https://tox.readthedocs.io/en/latest/
+[pip]: https://pypi.org/project/pip/
+[PyPI]: https://pypi.org/
```

### Comparing `napari-vedo-bridge-0.0.1/src/napari_vedo_bridge.egg-info/SOURCES.txt` & `napari-vedo-bridge-0.0.2/src/napari_vedo_bridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

