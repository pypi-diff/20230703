# Comparing `tmp/ivt-0.1.3.tar.gz` & `tmp/ivt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivt-0.1.3.tar", last modified: Sat Jul  1 06:36:11 2023, max compression
+gzip compressed data, was "ivt-0.1.4.tar", last modified: Mon Jul  3 17:52:28 2023, max compression
```

## Comparing `ivt-0.1.3.tar` & `ivt-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1123 2023-06-23 02:53:28.491095 ivt-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2174 2023-07-01 06:32:29.559569 ivt-0.1.3/.gitignore
--rw-r--r--   0        0        0     1091 2022-09-20 06:31:32.939829 ivt-0.1.3/LICENSE
--rw-r--r--   0        0        0      776 2023-06-23 02:53:28.491598 ivt-0.1.3/README.md
--rw-r--r--   0        0        0      661 2022-09-20 06:31:32.945331 ivt-0.1.3/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      493 2022-09-20 06:31:32.945832 ivt-0.1.3/docs/_templates/page.html
--rw-r--r--   0        0        0     1012 2022-09-20 06:31:32.946831 ivt-0.1.3/docs/conf.py
--rw-r--r--   0        0        0       58 2022-09-20 06:31:32.946831 ivt-0.1.3/docs/core_install.rst
--rw-r--r--   0        0        0       88 2022-09-20 06:31:32.947332 ivt-0.1.3/docs/core_intro.rst
--rw-r--r--   0        0        0       65 2022-09-20 06:31:32.947832 ivt-0.1.3/docs/forward_intro.rst
--rw-r--r--   0        0        0      605 2022-09-20 06:31:32.948332 ivt-0.1.3/docs/index.rst
--rw-r--r--   0        0        0       66 2022-09-20 06:31:32.948831 ivt-0.1.3/docs/inverse_intro.rst
--rw-r--r--   0        0        0       54 2022-09-20 06:31:32.949332 ivt-0.1.3/docs/plugin_refs.rst
--rw-r--r--   0        0        0       43 2022-09-20 06:31:32.949332 ivt-0.1.3/docs/requirements.txt
--rw-r--r--   0        0        0   268052 2022-09-20 06:31:32.950832 ivt-0.1.3/docs/teaser.png
--rw-r--r--   0        0        0      269 2023-07-01 06:32:29.561078 ivt-0.1.3/ivt/__init__.py
--rw-r--r--   0        0        0       83 2023-06-05 09:53:24.917312 ivt-0.1.3/ivt/config.py
--rw-r--r--   0        0        0      953 2023-06-05 09:53:24.917812 ivt-0.1.3/ivt/connector.py
--rw-r--r--   0        0        0       48 2023-06-05 09:53:24.918311 ivt-0.1.3/ivt/connectors/__init__.py
--rw-r--r--   0        0        0    14825 2023-07-01 06:32:29.562578 ivt-0.1.3/ivt/connectors/psdr_jit_connector.py
--rw-r--r--   0        0        0     5051 2023-06-23 02:53:28.526107 ivt-0.1.3/ivt/io.py
--rw-r--r--   0        0        0     2265 2023-03-07 09:19:51.701658 ivt-0.1.3/ivt/loss.py
--rw-r--r--   0        0        0     1554 2023-06-05 09:53:24.919812 ivt-0.1.3/ivt/model.py
--rw-r--r--   0        0        0     1908 2023-06-23 02:53:28.527105 ivt-0.1.3/ivt/parameter.py
--rw-r--r--   0        0        0     1925 2023-06-05 09:53:24.920815 ivt-0.1.3/ivt/renderer.py
--rw-r--r--   0        0        0     3217 2022-11-23 06:50:05.478582 ivt-0.1.3/ivt/sampling.py
--rw-r--r--   0        0        0     7098 2023-07-01 06:32:29.563079 ivt-0.1.3/ivt/scene.py
--rw-r--r--   0        0        0     3589 2023-07-01 06:32:29.564578 ivt-0.1.3/ivt/transform.py
--rw-r--r--   0        0        0      533 2023-07-01 06:34:46.759478 ivt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1153 1970-01-01 00:00:00.000000 ivt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1123 2023-06-23 02:53:28.491095 ivt-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2174 2023-07-01 06:32:29.559569 ivt-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1091 2022-09-20 06:31:32.939829 ivt-0.1.4/LICENSE
+-rw-r--r--   0        0        0      776 2023-06-23 02:53:28.491598 ivt-0.1.4/README.md
+-rw-r--r--   0        0        0      661 2022-09-20 06:31:32.945331 ivt-0.1.4/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      493 2022-09-20 06:31:32.945832 ivt-0.1.4/docs/_templates/page.html
+-rw-r--r--   0        0        0     1012 2022-09-20 06:31:32.946831 ivt-0.1.4/docs/conf.py
+-rw-r--r--   0        0        0       58 2022-09-20 06:31:32.946831 ivt-0.1.4/docs/core_install.rst
+-rw-r--r--   0        0        0       88 2022-09-20 06:31:32.947332 ivt-0.1.4/docs/core_intro.rst
+-rw-r--r--   0        0        0       65 2022-09-20 06:31:32.947832 ivt-0.1.4/docs/forward_intro.rst
+-rw-r--r--   0        0        0      605 2022-09-20 06:31:32.948332 ivt-0.1.4/docs/index.rst
+-rw-r--r--   0        0        0       66 2022-09-20 06:31:32.948831 ivt-0.1.4/docs/inverse_intro.rst
+-rw-r--r--   0        0        0       54 2022-09-20 06:31:32.949332 ivt-0.1.4/docs/plugin_refs.rst
+-rw-r--r--   0        0        0       43 2022-09-20 06:31:32.949332 ivt-0.1.4/docs/requirements.txt
+-rw-r--r--   0        0        0   268052 2022-09-20 06:31:32.950832 ivt-0.1.4/docs/teaser.png
+-rw-r--r--   0        0        0      269 2023-07-03 17:50:22.568627 ivt-0.1.4/ivt/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-05 09:53:24.917312 ivt-0.1.4/ivt/config.py
+-rw-r--r--   0        0        0      953 2023-06-05 09:53:24.917812 ivt-0.1.4/ivt/connector.py
+-rw-r--r--   0        0        0       48 2023-06-05 09:53:24.918311 ivt-0.1.4/ivt/connectors/__init__.py
+-rw-r--r--   0        0        0    14827 2023-07-03 02:09:02.909218 ivt-0.1.4/ivt/connectors/psdr_jit_connector.py
+-rw-r--r--   0        0        0     3588 2023-07-03 02:06:06.590286 ivt-0.1.4/ivt/io.py
+-rw-r--r--   0        0        0     2265 2023-03-07 09:19:51.701658 ivt-0.1.4/ivt/loss.py
+-rw-r--r--   0        0        0     1554 2023-06-05 09:53:24.919812 ivt-0.1.4/ivt/model.py
+-rw-r--r--   0        0        0     1908 2023-06-23 02:53:28.527105 ivt-0.1.4/ivt/parameter.py
+-rw-r--r--   0        0        0     1925 2023-06-05 09:53:24.920815 ivt-0.1.4/ivt/renderer.py
+-rw-r--r--   0        0        0     3217 2022-11-23 06:50:05.478582 ivt-0.1.4/ivt/sampling.py
+-rw-r--r--   0        0        0     7093 2023-07-03 06:05:49.508316 ivt-0.1.4/ivt/scene.py
+-rw-r--r--   0        0        0     3589 2023-07-01 06:32:29.564578 ivt-0.1.4/ivt/transform.py
+-rw-r--r--   0        0        0      521 2023-07-03 00:44:02.988608 ivt-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 ivt-0.1.4/PKG-INFO
```

### Comparing `ivt-0.1.3/.github/workflows/python-publish.yml` & `ivt-0.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/.gitignore` & `ivt-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/LICENSE` & `ivt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/README.md` & `ivt-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/docs/_static/theme_overrides.css` & `ivt-0.1.4/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/docs/conf.py` & `ivt-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/docs/index.rst` & `ivt-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/docs/teaser.png` & `ivt-0.1.4/docs/teaser.png`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/ivt/connector.py` & `ivt-0.1.4/ivt/connector.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/ivt/connectors/psdr_jit_connector.py` & `ivt-0.1.4/ivt/connectors/psdr_jit_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ..connector import Connector
 from ..scene import *
 from ..config import *
-from ..io import write_obj
+from ..io import write_mesh
 from collections import OrderedDict
 
 import drjit
 import psdr_jit
 from drjit.scalar import Array3f
 from drjit.cuda import Array3f as Vector3fC, Array3i as Vector3iC
 from drjit.cuda.ad import Array3f as Vector3fD, Float32 as FloatD, Matrix4f as Matrix4fD, Matrix3f as Matrix3fD
@@ -208,15 +208,15 @@
             psdr_mesh = psdr_jit.Mesh()
             psdr_mesh.load_raw(Vector3fC(mesh['v']), Vector3iC(mesh['f']))
             psdr_mesh.use_face_normal = mesh['use_face_normal']
 
             psdr_emitter = psdr_jit.AreaLight(mesh['radiance'].tolist()) if mesh['is_emitter'] else None
             psdr_scene.add_Mesh(psdr_mesh, mat_id, psdr_emitter)
         else:
-            write_obj('__psdr_jit_tmp__.obj', mesh['v'], mesh['f'], mesh['uv'], mesh['fuv'])
+            write_mesh('__psdr_jit_tmp__.obj', mesh['v'], mesh['f'], mesh['uv'], mesh['fuv'])
             psdr_emitter = psdr_jit.AreaLight(mesh['radiance']) if mesh['is_emitter'] else None
             psdr_scene.add_Mesh('__psdr_jit_tmp__.obj', mesh['to_world'].reshape(1, 4, 4), mat_id, psdr_emitter)
             os.remove('__psdr_jit_tmp__.obj')
         
         cache['name_map'][name] = f"Mesh[{psdr_scene.num_meshes - 1}]"
 
     psdr_mesh = psdr_scene.param_map[cache['name_map'][name]]
```

### Comparing `ivt-0.1.3/ivt/loss.py` & `ivt-0.1.4/ivt/loss.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/ivt/model.py` & `ivt-0.1.4/ivt/model.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/ivt/parameter.py` & `ivt-0.1.4/ivt/parameter.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/ivt/renderer.py` & `ivt-0.1.4/ivt/renderer.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/ivt/sampling.py` & `ivt-0.1.4/ivt/sampling.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/ivt/scene.py` & `ivt-0.1.4/ivt/scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .parameter import ParamGroup
 from .transform import lookat, perspective, batched_transform_pos, batched_transform_dir
-from .io import read_image, read_obj, to_torch_f, to_torch_i
+from .io import read_image, read_mesh, to_torch_f, to_torch_i
 
 from collections import OrderedDict
 
 import torch
 import torch.nn.functional as F
 
 class Scene:
@@ -119,16 +119,16 @@
         radiance = to_torch_f(radiance)
         is_emitter = radiance.sum() > 0
         self.add_param('is_emitter', is_emitter, help_msg='whether it is used as an emitter')
         self.add_param('radiance', radiance, is_tensor=True, is_diff=True, help_msg='radiance if it is used as an emitter')
 
     @classmethod
     def from_file(cls, filename, mat_id, to_world=torch.eye(4), use_face_normal=True, can_change_topology=False, radiance=torch.zeros(3)):
-        v, tc, n, f, ftc, fn = read_obj(filename)
-        return cls(v, f, tc, ftc, mat_id, to_world, use_face_normal, can_change_topology, radiance)
+        v, f, uv, fuv = read_mesh(filename)
+        return cls(v, f, uv, fuv, mat_id, to_world, use_face_normal, can_change_topology, radiance)
     
 class DiffuseBRDF(ParamGroup):
 
     def __init__(self, d):
         super().__init__()
         
         self.add_param('d', to_torch_f(d), is_tensor=True, is_diff=True, help_msg='diffuse reflectance')
```

### Comparing `ivt-0.1.3/ivt/transform.py` & `ivt-0.1.4/ivt/transform.py`

 * *Files identical despite different names*

### Comparing `ivt-0.1.3/pyproject.toml` & `ivt-0.1.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 readme = "README.md"
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 dependencies = [
     'imageio >= 2.27.0',
     'numpy',
     'gin-config',
-    'trimesh',
-    'libigl'
+    'gpytoolbox'
 ]
 
 [project.urls]
 Home = "https://github.com/uci-rendering/inv-render-toolkit"
 
 [tool.flit.sdist]
 exclude = [
```

### Comparing `ivt-0.1.3/PKG-INFO` & `ivt-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: ivt
-Version: 0.1.3
+Version: 0.1.4
 Summary: Inverse-Rendering Toolkit
 Author-email: Guangyan Cai <gcai3@uci.edu>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: imageio >= 2.27.0
 Requires-Dist: numpy
 Requires-Dist: gin-config
-Requires-Dist: trimesh
-Requires-Dist: libigl
+Requires-Dist: gpytoolbox
 Project-URL: Home, https://github.com/uci-rendering/inv-render-toolkit
 
 # ivt
 `ivt` stands for Inverse-Rendering Toolkit. It is a simple framework for conducting inverse rendering experiments. Since there are a lot differentiable renderers in development, mastering them all and migrating between them can be a headache. `ivt` provides a simple scene representation based on `pytorch` that can be rendered by **connectors** that connect to different differentiable renderers and get the graident of the scene parameters. Migrating between renderers is just a matter of changing the connector. 
 
 ## Installation
 `ivt` depends on `pytorch`. Since it is widely used and some projects might have specific requirements to it, we leave its installation to the user.
```

