# Comparing `tmp/ocp-freecad-cam-0.9.3.tar.gz` & `tmp/ocp-freecad-cam-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp-freecad-cam-0.9.3.tar", last modified: Thu Jun 22 16:37:49 2023, max compression
+gzip compressed data, was "ocp-freecad-cam-0.9.4.tar", last modified: Mon Jul  3 19:06:50 2023, max compression
```

## Comparing `ocp-freecad-cam-0.9.3.tar` & `ocp-freecad-cam-0.9.4.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:49.127799 ocp-freecad-cam-0.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:49.115799 ocp-freecad-cam-0.9.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:49.119799 ocp-freecad-cam-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-22 16:37:49.127799 ocp-freecad-cam-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:49.119799 ocp-freecad-cam-0.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:49.119799 ocp-freecad-cam-0.9.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/examples/cq_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/examples/cq_drill.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/examples/cq_helix.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/examples/cq_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/examples/cq_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/examples/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/examples/generate_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:49.119799 ocp-freecad-cam-0.9.3/docs/examples/images/
--rw-r--r--   0 runner    (1001) docker     (123)    22857 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/examples/images/cq_adaptive.png
--rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/examples/images/cq_drill.png
--rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/examples/images/cq_helix.png
--rw-r--r--   0 runner    (1001) docker     (123)    22366 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/examples/images/cq_pocket.png
--rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/examples/images/cq_profile.png
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 16:37:49.127799 ocp-freecad-cam-0.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:49.115799 ocp-freecad-cam-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:49.123799 ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33993 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/api_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/api_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    28562 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/fc_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/fc_impl_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:49.123799 ocp-freecad-cam-0.9.3/src/ocp_freecad_cam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-22 16:37:49.000000 ocp-freecad-cam-0.9.3/src/ocp_freecad_cam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-22 16:37:49.000000 ocp-freecad-cam-0.9.3/src/ocp_freecad_cam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:37:49.000000 ocp-freecad-cam-0.9.3/src/ocp_freecad_cam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 16:37:49.000000 ocp-freecad-cam-0.9.3/src/ocp_freecad_cam.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:49.115799 ocp-freecad-cam-0.9.3/stubs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:49.123799 ocp-freecad-cam-0.9.3/stubs/Part/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/stubs/Part/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:37:49.127799 ocp-freecad-cam-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/tests/test_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/tests/test_dressup.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/tests/test_drill.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/tests/test_engrave.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/tests/test_gcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/tests/test_helix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/tests/test_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-22 16:37:30.000000 ocp-freecad-cam-0.9.3/tests/test_waterline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:50.887810 ocp-freecad-cam-0.9.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:50.883810 ocp-freecad-cam-0.9.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:50.883810 ocp-freecad-cam-0.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-03 19:06:50.887810 ocp-freecad-cam-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:50.883810 ocp-freecad-cam-0.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:50.883810 ocp-freecad-cam-0.9.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/examples/b3d_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/examples/cq_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/examples/cq_drill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/examples/cq_helix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/examples/cq_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/examples/cq_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/examples/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/examples/generate_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:50.883810 ocp-freecad-cam-0.9.4/docs/examples/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    22857 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/examples/images/cq_adaptive.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/examples/images/cq_drill.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/examples/images/cq_helix.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22366 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/examples/images/cq_pocket.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/examples/images/cq_profile.png
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:06:50.887810 ocp-freecad-cam-0.9.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:50.879810 ocp-freecad-cam-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:50.887810 ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33993 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/api_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/api_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28562 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/fc_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/fc_impl_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:50.887810 ocp-freecad-cam-0.9.4/src/ocp_freecad_cam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-03 19:06:50.000000 ocp-freecad-cam-0.9.4/src/ocp_freecad_cam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-03 19:06:50.000000 ocp-freecad-cam-0.9.4/src/ocp_freecad_cam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:06:50.000000 ocp-freecad-cam-0.9.4/src/ocp_freecad_cam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 19:06:50.000000 ocp-freecad-cam-0.9.4/src/ocp_freecad_cam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:50.879810 ocp-freecad-cam-0.9.4/stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:50.887810 ocp-freecad-cam-0.9.4/stubs/Part/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/stubs/Part/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:50.887810 ocp-freecad-cam-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/tests/test_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/tests/test_dressup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/tests/test_drill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/tests/test_engrave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/tests/test_gcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/tests/test_helix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-03 19:06:39.000000 ocp-freecad-cam-0.9.4/tests/test_waterline.py
```

### Comparing `ocp-freecad-cam-0.9.3/.github/workflows/ci.yml` & `ocp-freecad-cam-0.9.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/.github/workflows/release.yml` & `ocp-freecad-cam-0.9.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/.readthedocs.yaml` & `ocp-freecad-cam-0.9.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/LICENSE` & `ocp-freecad-cam-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/PKG-INFO` & `ocp-freecad-cam-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-freecad-cam
-Version: 0.9.3
+Version: 0.9.4
 Summary: OCP FreeCAD CAM
 Author-email: Matti Eiden <snaipperi@gmail.com>
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/voneiden/ocp-freecad-cam/issues/
 Project-URL: Documentation, https://github.com/voneiden/ocp-freecad-cam/
 Project-URL: Source Code, https://github.com/voneiden/ocp-freecad-cam/
 Keywords: cadquery,viewer
```

### Comparing `ocp-freecad-cam-0.9.3/README.md` & `ocp-freecad-cam-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/docs/Makefile` & `ocp-freecad-cam-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/docs/api.rst` & `ocp-freecad-cam-0.9.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/docs/conf.py` & `ocp-freecad-cam-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/docs/examples/examples.rst` & `ocp-freecad-cam-0.9.4/docs/examples/examples.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 .. tabs::
 
    .. tab:: CadQuery
 
         .. literalinclude :: cq_profile.py
            :language: python
 
-   .. tab:: Build123d (todo)
+   .. tab:: Build123d
+        .. literalinclude :: b3d_profile.py
+           :language: python
 
 .. image:: images/cq_profile.png
 
 
 2.5D Pocketing
 -------------------------
```

### Comparing `ocp-freecad-cam-0.9.3/docs/examples/generate_image.py` & `ocp-freecad-cam-0.9.4/docs/examples/generate_image.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/docs/examples/images/cq_adaptive.png` & `ocp-freecad-cam-0.9.4/docs/examples/images/cq_adaptive.png`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/docs/examples/images/cq_drill.png` & `ocp-freecad-cam-0.9.4/docs/examples/images/cq_drill.png`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/docs/examples/images/cq_helix.png` & `ocp-freecad-cam-0.9.4/docs/examples/images/cq_helix.png`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/docs/examples/images/cq_pocket.png` & `ocp-freecad-cam-0.9.4/docs/examples/images/cq_pocket.png`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/docs/examples/images/cq_profile.png` & `ocp-freecad-cam-0.9.4/docs/examples/images/cq_profile.png`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/docs/index.rst` & `ocp-freecad-cam-0.9.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/pyproject.toml` & `ocp-freecad-cam-0.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/requirements-dev.txt` & `ocp-freecad-cam-0.9.4/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/__init__.py` & `ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/api.py` & `ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/api.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/api_tool.py` & `ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/api_tool.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/api_util.py` & `ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/api_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 def extract_topods_shapes(
     shape_source: ShapeSourceOrIterable, compound=False
 ) -> list[TopoDS_ShapeTypes]:
     if isinstance(shape_source, list):
         shapes = []
         for source in shape_source:
-            shapes += extract_topods_shapes(source)
+            shapes += extract_topods_shapes(source, compound=compound)
         return shapes
 
     if cq:
         valid_cq_shapes = (
             [cq.Compound, cq.Solid]
             if compound
             else [cq.Face, cq.Wire, cq.Edge, cq.Vertex]
```

### Comparing `ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/common.py` & `ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/common.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/fc_impl.py` & `ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/fc_impl.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/fc_impl_util.py` & `ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/fc_impl_util.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/src/ocp_freecad_cam/visualizer.py` & `ocp-freecad-cam-0.9.4/src/ocp_freecad_cam/visualizer.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/src/ocp_freecad_cam.egg-info/PKG-INFO` & `ocp-freecad-cam-0.9.4/src/ocp_freecad_cam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-freecad-cam
-Version: 0.9.3
+Version: 0.9.4
 Summary: OCP FreeCAD CAM
 Author-email: Matti Eiden <snaipperi@gmail.com>
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/voneiden/ocp-freecad-cam/issues/
 Project-URL: Documentation, https://github.com/voneiden/ocp-freecad-cam/
 Project-URL: Source Code, https://github.com/voneiden/ocp-freecad-cam/
 Keywords: cadquery,viewer
```

### Comparing `ocp-freecad-cam-0.9.3/src/ocp_freecad_cam.egg-info/SOURCES.txt` & `ocp-freecad-cam-0.9.4/src/ocp_freecad_cam.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 .github/CODEOWNERS
 .github/workflows/ci.yml
 .github/workflows/release.yml
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/index.rst
+docs/examples/b3d_profile.py
 docs/examples/cq_adaptive.py
 docs/examples/cq_drill.py
 docs/examples/cq_helix.py
 docs/examples/cq_pocket.py
 docs/examples/cq_profile.py
 docs/examples/examples.rst
 docs/examples/generate_image.py
```

### Comparing `ocp-freecad-cam-0.9.3/tests/test_adaptive.py` & `ocp-freecad-cam-0.9.4/tests/test_adaptive.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/tests/test_dressup.py` & `ocp-freecad-cam-0.9.4/tests/test_dressup.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/tests/test_drill.py` & `ocp-freecad-cam-0.9.4/tests/test_drill.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/tests/test_engrave.py` & `ocp-freecad-cam-0.9.4/tests/test_engrave.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/tests/test_gcode.py` & `ocp-freecad-cam-0.9.4/tests/test_gcode.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/tests/test_helix.py` & `ocp-freecad-cam-0.9.4/tests/test_helix.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/tests/test_params.py` & `ocp-freecad-cam-0.9.4/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/tests/test_profile.py` & `ocp-freecad-cam-0.9.4/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `ocp-freecad-cam-0.9.3/tests/test_waterline.py` & `ocp-freecad-cam-0.9.4/tests/test_waterline.py`

 * *Files identical despite different names*

