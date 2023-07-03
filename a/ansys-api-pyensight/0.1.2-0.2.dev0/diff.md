# Comparing `tmp/ansys-api-pyensight-0.1.2.tar.gz` & `tmp/ansys-api-pyensight-0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-pyensight-0.1.2.tar", last modified: Thu Jun 29 15:15:12 2023, max compression
+gzip compressed data, was "ansys-api-pyensight-0.2.dev0.tar", last modified: Mon Jul  3 09:54:23 2023, max compression
```

## Comparing `ansys-api-pyensight-0.1.2.tar` & `ansys-api-pyensight-0.2.dev0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:15:12.689221 ansys-api-pyensight-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-29 15:14:51.000000 ansys-api-pyensight-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-29 15:15:12.689221 ansys-api-pyensight-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-29 15:14:51.000000 ansys-api-pyensight-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-29 15:14:51.000000 ansys-api-pyensight-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:15:12.689221 ansys-api-pyensight-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-29 15:14:51.000000 ansys-api-pyensight-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:15:12.645221 ansys-api-pyensight-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:15:12.645221 ansys-api-pyensight-0.1.2/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:15:12.645221 ansys-api-pyensight-0.1.2/src/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:15:12.681221 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 15:14:51.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 15:14:51.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-29 15:14:51.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/access_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:15:12.681221 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   926642 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/assets/ensight_api_test_assets.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_animobj.py
--rw-r--r--   0 runner    (1001) docker     (123)    30169 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot.py
--rw-r--r--   0 runner    (1001) docker     (123)    48180 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    34554 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_dial.py
--rw-r--r--   0 runner    (1001) docker     (123)    35302 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_gauge.py
--rw-r--r--   0 runner    (1001) docker     (123)    51383 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_lgnd.py
--rw-r--r--   0 runner    (1001) docker     (123)    35577 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    30261 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    34357 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    65944 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_emitterobj.py
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_flipbook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)   214200 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    22539 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    34491 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_lightsource.py
--rw-r--r--   0 runner    (1001) docker     (123)    33641 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_lpart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    56524 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_palette.py
--rw-r--r--   0 runner    (1001) docker     (123)   264396 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part.py
--rw-r--r--   0 runner    (1001) docker     (123)   195871 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_aux_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)   190146 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_axisymmetric.py
--rw-r--r--   0 runner    (1001) docker     (123)   179413 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_built_up.py
--rw-r--r--   0 runner    (1001) docker     (123)   289827 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)   202105 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)   186771 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_developed_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)   264534 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_discrete_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)   192486 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_elevated_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)   241715 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    63752 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)   192689 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_fx_sep_att.py
--rw-r--r--   0 runner    (1001) docker     (123)   202494 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_fx_shock.py
--rw-r--r--   0 runner    (1001) docker     (123)   192681 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_fx_vortex_core.py
--rw-r--r--   0 runner    (1001) docker     (123)   192954 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_isosurface.py
--rw-r--r--   0 runner    (1001) docker     (123)   183318 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_mat_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)   264486 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   243979 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_particle_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)   181578 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_point.py
--rw-r--r--   0 runner    (1001) docker     (123)   187760 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)   198386 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_tensor_glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)   204686 2023-06-29 15:15:11.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_vector_arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)   236410 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_vof.py
--rw-r--r--   0 runner    (1001) docker     (123)   132145 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_probe.py
--rw-r--r--   0 runner    (1001) docker     (123)    83457 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    18958 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    16447 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_cone.py
--rw-r--r--   0 runner    (1001) docker     (123)    16541 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18693 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_cylinder.py
--rw-r--r--   0 runner    (1001) docker     (123)    20154 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_plane.py
--rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_revolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)    49892 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_var.py
--rw-r--r--   0 runner    (1001) docker     (123)   211317 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_vport.py
--rw-r--r--   0 runner    (1001) docker     (123)  2000687 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ensight_api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:51.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:15:12.681221 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/v0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:51.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-29 15:14:51.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/v0/enshell.proto
--rw-r--r--   0 runner    (1001) docker     (123)    18258 2023-06-29 15:14:51.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/v0/ensight.proto
--rw-r--r--   0 runner    (1001) docker     (123)  2446597 2023-06-29 15:14:51.000000 ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/v0/ensight_api.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:15:12.685222 ansys-api-pyensight-0.1.2/src/ansys_api_pyensight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys_api_pyensight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys_api_pyensight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys_api_pyensight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys_api_pyensight.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys_api_pyensight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 15:15:12.000000 ansys-api-pyensight-0.1.2/src/ansys_api_pyensight.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.660832 ansys-api-pyensight-0.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-03 09:54:23.660832 ansys-api-pyensight-0.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 09:54:23.660832 ansys-api-pyensight-0.2.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.636831 ansys-api-pyensight-0.2.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.636831 ansys-api-pyensight-0.2.dev0/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.636831 ansys-api-pyensight-0.2.dev0/src/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.656832 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/access_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.656832 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   926642 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/assets/ensight_api_test_assets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_animobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30169 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48180 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34554 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35302 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51383 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_lgnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35577 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30261 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34357 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65944 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_emitterobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_flipbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)   214200 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22539 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34491 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_lightsource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33641 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_lpart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56524 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)   264396 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)   195871 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_aux_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   190146 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_axisymmetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179413 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_built_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)   289827 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)   202105 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)   186771 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_developed_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   264534 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_discrete_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192486 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_elevated_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241715 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63752 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192689 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_fx_sep_att.py
+-rw-r--r--   0 runner    (1001) docker     (123)   202494 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_fx_shock.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192681 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_fx_vortex_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192954 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_isosurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   183318 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_mat_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   264486 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   243979 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_particle_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)   181578 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187760 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   198386 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_tensor_glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   204686 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_vector_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)   236410 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_vof.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132145 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_probe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83457 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18958 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16447 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_cone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16541 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18693 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20154 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_revolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49892 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)   211317 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_vport.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2000687 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ensight_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.656832 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/enshell.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    18258 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/ensight.proto
+-rw-r--r--   0 runner    (1001) docker     (123)  2446597 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/ensight_api.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.660832 ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/top_level.txt
```

### Comparing `ansys-api-pyensight-0.1.2/LICENSE` & `ansys-api-pyensight-0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/PKG-INFO` & `ansys-api-pyensight-0.2.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-pyensight
-Version: 0.1.2
-Summary: Autogenerated python gRPC interface package for ansys-api-pyensight, built on 15:15:10 on 29 June 2023
+Version: 0.2.dev0
+Summary: Autogenerated python gRPC interface package for ansys-api-pyensight, built on 09:54:22 on 03 July 2023
 Home-page: https://github.com/ansys/ansys-api-pyensight
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Requires-Python: >=3.8
```

### Comparing `ansys-api-pyensight-0.1.2/README.md` & `ansys-api-pyensight-0.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/setup.py` & `ansys-api-pyensight-0.2.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Installation file for the ansys-api-pyensight package"""
 
 import os
 import sys
 from datetime import datetime
 
-import distutils
 import setuptools
 import setuptools.command.build_py
 import setuptools.command.sdist
-import subprocess
 
 from ansys.tools.protoc_helper import CMDCLASS_OVERRIDE
+import distutils.cmd
+import distutils.log
+import subprocess
 
 # Get the long description from the README file
 HERE = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 product = "pyensight"
@@ -80,15 +81,15 @@
         maintainer_email='pyansys.core@ansys.com',
         description=description,
         long_description=long_description,
         long_description_content_type='text/markdown',
         url=f"https://github.com/ansys/{package_name}",
         license="MIT",
         python_requires=">=3.8",
-        install_requires=["grpcio~=1.17", "protobuf~=3.19"],
+        install_requires=["grpcio>=1.17", "protobuf>=3.19"],
         package_dir = {"": "src"},
         packages=setuptools.find_namespace_packages("src", include=("ansys.*",)),
         package_data={
             "": ["*.proto", "*.pyi", "py.typed", "VERSION", "*.xml", "*ensight_api_test_assets.txt"],
             
         },
         entry_points={
```

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/assets/ensight_api_test_assets.txt` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/assets/ensight_api_test_assets.txt`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_animobj.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_animobj.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_arrow.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_arrow.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_dial.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_dial.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_gauge.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_gauge.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_lgnd.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_lgnd.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_line.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_line.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_logo.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_logo.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_marker.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_marker.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_shape.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_shape.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_annot_text.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_text.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_camera.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_camera.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_case.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_case.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_emitterobj.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_emitterobj.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_flipbook.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_flipbook.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_frame.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_frame.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_globals.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_globals.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_group.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_group.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_lightsource.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_lightsource.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_lpart.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_lpart.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_mat.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_mat.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_palette.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_palette.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_aux_geom.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_aux_geom.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_axisymmetric.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_axisymmetric.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_built_up.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_built_up.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_clip.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_clip.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_contour.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_contour.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_developed_surface.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_developed_surface.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_discrete_particle.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_discrete_particle.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_elevated_surface.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_elevated_surface.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_filter.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_filter.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_frame.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_frame.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_fx_sep_att.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_fx_sep_att.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_fx_shock.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_fx_shock.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_fx_vortex_core.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_fx_vortex_core.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_isosurface.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_isosurface.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_mat_interface.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_mat_interface.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_model.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_model.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_particle_trace.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_particle_trace.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_point.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_point.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_profile.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_profile.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_tensor_glyph.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_tensor_glyph.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_vector_arrow.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_vector_arrow.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_part_vof.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_vof.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_plotter.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_plotter.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_polyline.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_polyline.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_probe.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_probe.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_query.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_query.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_scene.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_scene.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_source.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_source.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_spec.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_spec.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_state.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_state.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_texture.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_texture.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_box.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_box.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_cone.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_cone.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_cursor.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_cursor.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_cylinder.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_cylinder.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_line.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_line.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_plane.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_plane.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_revolution.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_revolution.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_tool_sphere.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_sphere.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_var.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_var.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ens_vport.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_vport.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/ensight_api.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ensight_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Module ensight_api
-Autogenerated from: ensight_api.xml at 2023-06-29T15:15:11.571237
+Autogenerated from: ensight_api.xml at 2023-07-03T09:54:22.953220
 """
 from ansys.pyensight.core import Session
 from ansys.pyensight.core.ensobj import ENSOBJ
 from ansys.pyensight.core import ensobjlist
 from ansys.api.pyensight.ens_annot import ENS_ANNOT
 from ansys.api.pyensight.ens_annot_text import ENS_ANNOT_TEXT
 from ansys.api.pyensight.ens_annot_line import ENS_ANNOT_LINE
```

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/v0/enshell.proto` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/enshell.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/v0/ensight.proto` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/ensight.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys/api/pyensight/v0/ensight_api.xml` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/ensight_api.xml`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.1.2/src/ansys_api_pyensight.egg-info/PKG-INFO` & `ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-pyensight
-Version: 0.1.2
-Summary: Autogenerated python gRPC interface package for ansys-api-pyensight, built on 15:15:10 on 29 June 2023
+Version: 0.2.dev0
+Summary: Autogenerated python gRPC interface package for ansys-api-pyensight, built on 09:54:22 on 03 July 2023
 Home-page: https://github.com/ansys/ansys-api-pyensight
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Requires-Python: >=3.8
```

### Comparing `ansys-api-pyensight-0.1.2/src/ansys_api_pyensight.egg-info/SOURCES.txt` & `ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

