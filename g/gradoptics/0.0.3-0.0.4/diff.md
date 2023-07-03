# Comparing `tmp/gradoptics-0.0.3.tar.gz` & `tmp/gradoptics-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradoptics-0.0.3.tar", last modified: Mon Apr 17 21:40:14 2023, max compression
+gzip compressed data, was "gradoptics-0.0.4.tar", last modified: Mon Jul  3 16:25:44 2023, max compression
```

## Comparing `gradoptics-0.0.3.tar` & `gradoptics-0.0.4.tar`

### file list

```diff
@@ -1,58 +1,62 @@
-drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.323735 gradoptics-0.0.3/
--rw-r--r--   0 sgaz     (1449223128) 1704612529     1087 2022-07-22 00:01:52.000000 gradoptics-0.0.3/LICENSE
--rw-r--r--   0 sgaz     (1449223128) 1704612529       34 2022-07-22 00:01:52.000000 gradoptics-0.0.3/MANIFEST.in
--rw-r--r--   0 sgaz     (1449223128) 1704612529     4733 2023-04-17 21:40:14.323141 gradoptics-0.0.3/PKG-INFO
--rw-r--r--   0 sgaz     (1449223128) 1704612529     2738 2023-01-30 17:18:04.000000 gradoptics-0.0.3/README.md
--rw-r--r--   0 sgaz     (1449223128) 1704612529      751 2023-04-17 21:39:47.000000 gradoptics-0.0.3/pyproject.toml
--rw-r--r--   0 sgaz     (1449223128) 1704612529       38 2023-04-17 21:40:14.323928 gradoptics-0.0.3/setup.cfg
--rw-r--r--   0 sgaz     (1449223128) 1704612529      760 2023-04-17 21:33:43.000000 gradoptics-0.0.3/setup.py
-drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.294388 gradoptics-0.0.3/src/
-drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.300853 gradoptics-0.0.3/src/gradoptics/
--rw-r--r--   0 sgaz     (1449223128) 1704612529     1409 2023-04-17 21:19:43.000000 gradoptics-0.0.3/src/gradoptics/__init__.py
-drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.306364 gradoptics-0.0.3/src/gradoptics/distributions/
--rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/distributions/__init__.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     6934 2023-04-17 21:19:43.000000 gradoptics-0.0.3/src/gradoptics/distributions/atom_cloud.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     6265 2023-04-17 21:19:43.000000 gradoptics-0.0.3/src/gradoptics/distributions/atom_cloud_donut.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529      884 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/distributions/base_distribution.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529      981 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/distributions/gaussian_distribution.py
-drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.307903 gradoptics-0.0.3/src/gradoptics/inference/
--rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/inference/__init__.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     1926 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/inference/rejection_sampling.py
-drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.310094 gradoptics-0.0.3/src/gradoptics/integrator/
--rw-r--r--   0 sgaz     (1449223128) 1704612529      116 2023-04-17 21:19:15.000000 gradoptics-0.0.3/src/gradoptics/integrator/__init__.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529      789 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/integrator/base_integrator.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     1512 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/integrator/stratified_sampling_integrator.py
-drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.311863 gradoptics-0.0.3/src/gradoptics/light_sources/
--rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/light_sources/__init__.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     1196 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/light_sources/base_light_source.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     2322 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/light_sources/light_source_from_distribution.py
-drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.318530 gradoptics-0.0.3/src/gradoptics/optics/
--rw-r--r--   0 sgaz     (1449223128) 1704612529      359 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/__init__.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     1547 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/base_optics.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     4592 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/bounding_box.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529      642 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/bounding_shape.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     3686 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/bounding_sphere.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     1775 2023-01-30 17:18:04.000000 gradoptics-0.0.3/src/gradoptics/optics/camera.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529    16601 2023-04-17 21:19:15.000000 gradoptics-0.0.3/src/gradoptics/optics/lens.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     9249 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/mirror.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     1275 2023-01-30 17:18:04.000000 gradoptics-0.0.3/src/gradoptics/optics/psf.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     6532 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/ray.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529    10692 2023-04-17 21:19:15.000000 gradoptics-0.0.3/src/gradoptics/optics/sensor.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     4168 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/optics/vector.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     7566 2023-04-17 21:19:15.000000 gradoptics-0.0.3/src/gradoptics/optics/window.py
-drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.320016 gradoptics-0.0.3/src/gradoptics/ray_tracing/
--rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/ray_tracing/__init__.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     6222 2023-04-17 21:19:15.000000 gradoptics-0.0.3/src/gradoptics/ray_tracing/ray_tracing.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529      828 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/ray_tracing/scene.py
-drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.321924 gradoptics-0.0.3/src/gradoptics/transforms/
--rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/transforms/__init__.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     3964 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/transforms/base_transform.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     2307 2023-04-17 21:19:15.000000 gradoptics-0.0.3/src/gradoptics/transforms/look_at_transform.py
--rw-r--r--   0 sgaz     (1449223128) 1704612529     2453 2022-07-22 00:01:52.000000 gradoptics-0.0.3/src/gradoptics/transforms/simple_transform.py
-drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.303481 gradoptics-0.0.3/src/gradoptics.egg-info/
--rw-r--r--   0 sgaz     (1449223128) 1704612529     4733 2023-04-17 21:40:14.000000 gradoptics-0.0.3/src/gradoptics.egg-info/PKG-INFO
--rw-r--r--   0 sgaz     (1449223128) 1704612529     1595 2023-04-17 21:40:14.000000 gradoptics-0.0.3/src/gradoptics.egg-info/SOURCES.txt
--rw-r--r--   0 sgaz     (1449223128) 1704612529        1 2023-04-17 21:40:14.000000 gradoptics-0.0.3/src/gradoptics.egg-info/dependency_links.txt
--rw-r--r--   0 sgaz     (1449223128) 1704612529       11 2023-04-17 21:40:14.000000 gradoptics-0.0.3/src/gradoptics.egg-info/top_level.txt
-drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-04-17 21:40:14.322336 gradoptics-0.0.3/tests/
--rw-r--r--   0 sgaz     (1449223128) 1704612529    26254 2023-04-17 21:19:15.000000 gradoptics-0.0.3/tests/tests.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-07-03 16:25:44.096496 gradoptics-0.0.4/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1087 2023-06-30 19:17:20.000000 gradoptics-0.0.4/LICENSE
+-rw-r--r--   0 sgaz     (1449223128) 1704612529       34 2023-06-30 19:17:20.000000 gradoptics-0.0.4/MANIFEST.in
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     4782 2023-07-03 16:25:44.095909 gradoptics-0.0.4/PKG-INFO
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     2738 2023-06-30 19:17:20.000000 gradoptics-0.0.4/README.md
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      805 2023-06-30 19:17:20.000000 gradoptics-0.0.4/pyproject.toml
+-rw-r--r--   0 sgaz     (1449223128) 1704612529       38 2023-07-03 16:25:44.096725 gradoptics-0.0.4/setup.cfg
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      794 2023-06-30 19:17:20.000000 gradoptics-0.0.4/setup.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-07-03 16:25:44.055244 gradoptics-0.0.4/src/
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-07-03 16:25:44.060098 gradoptics-0.0.4/src/gradoptics/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1633 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/__init__.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-07-03 16:25:44.068609 gradoptics-0.0.4/src/gradoptics/distributions/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/distributions/__init__.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     6934 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/distributions/atom_cloud.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     6265 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/distributions/atom_cloud_donut.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      884 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/distributions/base_distribution.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      981 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/distributions/gaussian_distribution.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      943 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/distributions/point_source.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     5342 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/distributions/simple_atom_cloud.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-07-03 16:25:44.069691 gradoptics-0.0.4/src/gradoptics/inference/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/inference/__init__.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1926 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/inference/rejection_sampling.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-07-03 16:25:44.072718 gradoptics-0.0.4/src/gradoptics/integrator/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      193 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/integrator/__init__.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      789 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/integrator/base_integrator.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     4254 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/integrator/hierarchical_sampling_integrator.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1512 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/integrator/stratified_sampling_integrator.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-07-03 16:25:44.075939 gradoptics-0.0.4/src/gradoptics/light_sources/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/light_sources/__init__.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1196 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/light_sources/base_light_source.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     2920 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/light_sources/light_source_from_distribution.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     2254 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/light_sources/light_source_from_neural_net.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-07-03 16:25:44.087344 gradoptics-0.0.4/src/gradoptics/optics/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      359 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/optics/__init__.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1547 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/optics/base_optics.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     4592 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/optics/bounding_box.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      642 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/optics/bounding_shape.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     3686 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/optics/bounding_sphere.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1775 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/optics/camera.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529    16671 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/optics/lens.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     9249 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/optics/mirror.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1275 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/optics/psf.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     6532 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/optics/ray.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529    12897 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/optics/sensor.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     4168 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/optics/vector.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     9207 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/optics/window.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-07-03 16:25:44.089765 gradoptics-0.0.4/src/gradoptics/ray_tracing/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/ray_tracing/__init__.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529    10222 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/ray_tracing/ray_tracing.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529      828 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/ray_tracing/scene.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-07-03 16:25:44.093628 gradoptics-0.0.4/src/gradoptics/transforms/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529        0 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/transforms/__init__.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     3964 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/transforms/base_transform.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     2591 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/transforms/look_at_transform.py
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     2453 2023-06-30 19:17:20.000000 gradoptics-0.0.4/src/gradoptics/transforms/simple_transform.py
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-07-03 16:25:44.063002 gradoptics-0.0.4/src/gradoptics.egg-info/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     4782 2023-07-03 16:25:43.000000 gradoptics-0.0.4/src/gradoptics.egg-info/PKG-INFO
+-rw-r--r--   0 sgaz     (1449223128) 1704612529     1813 2023-07-03 16:25:43.000000 gradoptics-0.0.4/src/gradoptics.egg-info/SOURCES.txt
+-rw-r--r--   0 sgaz     (1449223128) 1704612529        1 2023-07-03 16:25:43.000000 gradoptics-0.0.4/src/gradoptics.egg-info/dependency_links.txt
+-rw-r--r--   0 sgaz     (1449223128) 1704612529       11 2023-07-03 16:25:43.000000 gradoptics-0.0.4/src/gradoptics.egg-info/top_level.txt
+drwxr-xr-x   0 sgaz     (1449223128) 1704612529        0 2023-07-03 16:25:44.094528 gradoptics-0.0.4/tests/
+-rw-r--r--   0 sgaz     (1449223128) 1704612529    27676 2023-06-30 19:17:20.000000 gradoptics-0.0.4/tests/tests.py
```

### Comparing `gradoptics-0.0.3/LICENSE` & `gradoptics-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/PKG-INFO` & `gradoptics-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gradoptics
-Version: 0.0.3
+Version: 0.0.4
 Summary: Differentiable Optics via Ray Tracing
 Home-page: https://github.com/magis-slac/gradoptics
-Author: Sean Gasiorowski, Michael Kagan, Maxime Vandegar
-Author-email: Sean Gasiorowski <sgaz@slac.stanford.edu>, Michael Kagan <makagan@slac.stanford.edu>, Maxime Vandegar <maxime.vandegar@slac.stanford.edu>
+Author: Sean Gasiorowski, Michael Kagan, Maxime Vandegar, Sanha Cheong
+Author-email: Sean Gasiorowski <sgaz@slac.stanford.edu>, Michael Kagan <makagan@slac.stanford.edu>, Maxime Vandegar <maxime.vandegar@slac.stanford.edu>, Sanha Cheong <sanha@stanford.edu>
 License: MIT License
         
         Copyright (c) 2021 Michael Kagan, Maxime Vandegar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -36,15 +36,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/magis-slac/gradoptics/actions/workflows/main.yml/badge.svg)](https://github.com/magis-slac/gradoptics/actions)
 [![Build Status](https://travis-ci.com/magis-slac/gradoptics.svg?token=LBAvFbnCy9PEgexzsTUS&branch=main)](https://travis-ci.com/magis-slac/gradoptics)
 [![Documentation Status](https://readthedocs.org/projects/gradoptics/badge/?version=latest)](https://gradoptics.readthedocs.io/en/latest/?badge=latest)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/magis-slac/gradoptics/blob/master/README.md)
-![version](https://img.shields.io/badge/version-0.0.2-blue)
+![version](https://img.shields.io/badge/version-0.0.4-blue)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 # Differentiable Optics via Ray Tracing
 [*gradoptics*](https://github.com/magis-slac/gradoptics) is a ray tracing based optical simulator built using PyTorch [[1]](#1) to enable automatic differentiation. 
 
 The API is designed similar to rendering softwares, and has been heavily inspired by *Physically Based Rendering* (Pharr, Jakob, Humphreys) [[2]](#2).
```

### Comparing `gradoptics-0.0.3/README.md` & `gradoptics-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![Tests](https://github.com/magis-slac/gradoptics/actions/workflows/main.yml/badge.svg)](https://github.com/magis-slac/gradoptics/actions)
 [![Build Status](https://travis-ci.com/magis-slac/gradoptics.svg?token=LBAvFbnCy9PEgexzsTUS&branch=main)](https://travis-ci.com/magis-slac/gradoptics)
 [![Documentation Status](https://readthedocs.org/projects/gradoptics/badge/?version=latest)](https://gradoptics.readthedocs.io/en/latest/?badge=latest)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/magis-slac/gradoptics/blob/master/README.md)
-![version](https://img.shields.io/badge/version-0.0.2-blue)
+![version](https://img.shields.io/badge/version-0.0.4-blue)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 # Differentiable Optics via Ray Tracing
 [*gradoptics*](https://github.com/magis-slac/gradoptics) is a ray tracing based optical simulator built using PyTorch [[1]](#1) to enable automatic differentiation. 
 
 The API is designed similar to rendering softwares, and has been heavily inspired by *Physically Based Rendering* (Pharr, Jakob, Humphreys) [[2]](#2).
```

### Comparing `gradoptics-0.0.3/setup.py` & `gradoptics-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
   name='gradoptics',
-  version='0.0.3',
+  version='0.0.4',
   description='End-to-end differentiable optics',
   long_description=long_description,
   long_description_content_type="text/markdown",
-  author='Sean Gasiorowski, Michael Kagan, Maxime Vandegar',
-  author_email='sgaz@slac.stanford.edu, makagan@slac.stanford.edu, maxime.vandegar@slac.stanford.edu',
+  author='Sean Gasiorowski, Michael Kagan, Maxime Vandegar, Sanha Cheong',
+  author_email='sgaz@slac.stanford.edu, makagan@slac.stanford.edu, maxime.vandegar@slac.stanford.edu, sanha@stanford.edu',
   url="https://github.com/magis-slac/gradoptics",
   classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
   package_dir={'': 'src'},
```

### Comparing `gradoptics-0.0.3/src/gradoptics/__init__.py` & `gradoptics-0.0.4/src/gradoptics/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from gradoptics.optics.vector import vector3d, batch_vector, normalize_batch_vector, normalize_vector, dot_product
 
 from gradoptics.distributions.gaussian_distribution import GaussianDistribution
 from gradoptics.distributions.base_distribution import BaseDistribution
+from gradoptics.distributions.point_source import PointSource
 from gradoptics.distributions.atom_cloud import AtomCloud
+from gradoptics.distributions.simple_atom_cloud import SimpleAtomCloud
 from gradoptics.distributions.atom_cloud_donut import AtomCloudDonut
 
 from gradoptics.inference.rejection_sampling import rejection_sampling
 
 from gradoptics.optics.lens import PerfectLens, ThickLens
 from gradoptics.optics.mirror import FlatMirror, CurvedMirror
 from gradoptics.optics.ray import Ray, Rays, empty_like, cat
@@ -17,14 +19,15 @@
 
 from gradoptics.ray_tracing.scene import Scene
 
 from gradoptics.ray_tracing.ray_tracing import forward_ray_tracing
 from gradoptics.ray_tracing.ray_tracing import backward_ray_tracing
 
 from gradoptics.light_sources.light_source_from_distribution import LightSourceFromDistribution
+from gradoptics.light_sources.light_source_from_neural_net import LightSourceFromNeuralNet
 
 from gradoptics.transforms import base_transform, look_at_transform, simple_transform
 
 from gradoptics.optics.psf import PSF
 
 from gradoptics.integrator.base_integrator import BaseIntegrator
 from gradoptics.integrator.stratified_sampling_integrator import StratifiedSamplingIntegrator
```

### Comparing `gradoptics-0.0.3/src/gradoptics/distributions/atom_cloud.py` & `gradoptics-0.0.4/src/gradoptics/distributions/atom_cloud.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/distributions/atom_cloud_donut.py` & `gradoptics-0.0.4/src/gradoptics/distributions/atom_cloud_donut.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/distributions/base_distribution.py` & `gradoptics-0.0.4/src/gradoptics/distributions/base_distribution.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/distributions/gaussian_distribution.py` & `gradoptics-0.0.4/src/gradoptics/distributions/gaussian_distribution.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/inference/rejection_sampling.py` & `gradoptics-0.0.4/src/gradoptics/inference/rejection_sampling.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/integrator/base_integrator.py` & `gradoptics-0.0.4/src/gradoptics/integrator/base_integrator.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/integrator/stratified_sampling_integrator.py` & `gradoptics-0.0.4/src/gradoptics/integrator/stratified_sampling_integrator.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/light_sources/base_light_source.py` & `gradoptics-0.0.4/src/gradoptics/light_sources/base_light_source.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/light_sources/light_source_from_distribution.py` & `gradoptics-0.0.4/src/gradoptics/light_sources/light_source_from_distribution.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 import torch
 
 from gradoptics import Rays
 from gradoptics.light_sources.base_light_source import BaseLightSource
-from gradoptics.optics import batch_vector
+from gradoptics.optics import batch_vector, normalize_batch_vector
 
 
 class LightSourceFromDistribution(BaseLightSource):
     """
     Models a light source from a distribution. It emits rays in 4pi, with their origins sampled from the distribution.
     """
 
@@ -41,14 +41,27 @@
         del azimuthal_angle
         del polar_angle
         torch.cuda.empty_cache()
 
         return Rays(self.distribution.sample(nb_rays, device=device).type(emitted_direction.dtype), emitted_direction,
                     device=device)
 
+    def sample_pointed_rays(self, nb_rays, target_point, device='cpu'):
+        # Sample origins from underlying distribution
+        origins = self.distribution.sample(nb_rays, device=device)
+        directions = normalize_batch_vector(target_point - origins)
+
+        # TODO: implement intensity weights based on solid angle calculation
+        # Solid angle calculation reference: http://websites.umich.edu/~ners311/CourseLibrary/SolidAngleOfADiskOffAxis.pdf
+
+        torch.cuda.empty_cache()
+
+        return Rays(origins, directions,
+                    device=device)
+
     def plot(self, ax, **kwargs):
         return self.distribution.plot(ax, **kwargs)
 
     def pdf(self, x):
         """
         Returns the pdf function of the distribution evaluated at ``x``
```

### Comparing `gradoptics-0.0.3/src/gradoptics/optics/base_optics.py` & `gradoptics-0.0.4/src/gradoptics/optics/base_optics.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/optics/bounding_box.py` & `gradoptics-0.0.4/src/gradoptics/optics/bounding_box.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/optics/bounding_shape.py` & `gradoptics-0.0.4/src/gradoptics/optics/bounding_shape.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/optics/bounding_sphere.py` & `gradoptics-0.0.4/src/gradoptics/optics/bounding_sphere.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/optics/camera.py` & `gradoptics-0.0.4/src/gradoptics/optics/camera.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/optics/lens.py` & `gradoptics-0.0.4/src/gradoptics/optics/lens.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def sample_points_on_lens(self, nb_points, device='cpu'):
         """
         Sample points uniformly on the lens
 
         :param nb_points: Number of points to sample (:obj:`int`)
         :param device: The desired device of returned tensor (:obj:`str`). Default is ``'cpu'``
 
-        :return: Sampled points (:obj:`torch.tensor`)
+        :return: (:obj:`tuple`) Sampled points (:obj:`torch.tensor`) and p(A) (:obj:`float`)
         """
         raise NotImplemented
 
 
 class PerfectLens(Lens):
     """
     Models a thin lens.
@@ -106,15 +106,16 @@
         lens_radius = self.f * self.na / 2
         # Sampling uniformly on a disk.
         # See https://stats.stackexchange.com/questions/481543/generating-random-points-uniformly-on-a-disk
         r_squared = torch.rand(nb_points, device=device) * lens_radius ** 2
         theta = torch.rand(nb_points, device=device) * 2 * np.pi
         points[:, 1] = torch.sqrt(r_squared) * torch.cos(theta)
         points[:, 2] = torch.sqrt(r_squared) * torch.sin(theta)
-        return self.transform.apply_transform_(points)
+        return self.transform.apply_transform_(points), 1 / (np.pi * lens_radius**2)
+
 
     def plot(self, ax, s=0.1, color='lightblue', resolution=100):
         # @Todo, change this to plot_surface
         y = torch.arange(-self.f * self.na / 2, self.f * self.na / 2, (self.f * self.na) / resolution)
         z = torch.arange(-self.f * self.na / 2, self.f * self.na / 2, (self.f * self.na) / resolution)
         y, z = torch.meshgrid(y, z)
```

### Comparing `gradoptics-0.0.3/src/gradoptics/optics/mirror.py` & `gradoptics-0.0.4/src/gradoptics/optics/mirror.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/optics/psf.py` & `gradoptics-0.0.4/src/gradoptics/optics/psf.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/optics/ray.py` & `gradoptics-0.0.4/src/gradoptics/optics/ray.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/optics/sensor.py` & `gradoptics-0.0.4/src/gradoptics/optics/sensor.py`

 * *Files 17% similar despite different names*

```diff
@@ -98,15 +98,17 @@
                     hit_positions_psf = hit_positions[mask] * self.psf_ratio
                     self.pixelize(depth_id, hit_positions_psf, incident_rays.luminosities[mask],
                                   quantum_efficiency=quantum_efficiency)
                     nb_processed_rays += mask.sum()
 
                 if not (nb_processed_rays == hit_positions.shape[0]):
                     raise Exception(
-                        "Some rays were not processed: their origins' depths were not included in the psfs.")
+                        f"Some rays were not processed. {nb_processed_rays} were processed, but {hit_positions.shape[0]} hit the sensor! Their origins' depths might not be included in the psfs.")
+                    # print(f"WARNING! Out of {nb_processed_rays} processed rays, only {hit_positions.shape[0]} hit the sensor!")
+                    # print("The ray origins' depths might not have been included in the PSF-defining bins!")
 
             else:
                 self.pixelize(0, hit_positions, incident_rays.luminosities, quantum_efficiency=quantum_efficiency)
 
         # No rays reflected or refracted
         return None, torch.zeros(origins.shape[0], dtype=torch.bool, device=origins.device)
 
@@ -124,31 +126,41 @@
 
         if hit_positions.shape[0] == 0:
             return
 
         if quantum_efficiency:
             luminosities *= self.quantum_efficiency
 
-        # Update pixel values
-        indices = torch.floor(hit_positions[:, 1].type(torch.float64)).type(torch.int64) * (
-                    self.resolution[1] * self.psf_ratio) + \
-                  torch.floor(hit_positions[:, 0].type(torch.float64)).type(torch.int64)
-        max_nb_identical_indices = indices.unique(return_counts=True)[1].max()
-        sorted_indices, arg_sorted_indices = torch.sort(indices)
-
-        for i in range(max_nb_identical_indices):
-            ind = sorted_indices[i::max_nb_identical_indices]
-            arg_ind = arg_sorted_indices[i::max_nb_identical_indices]
-
-            # Sanity check, should be removed
-            cond = (ind[1:] == ind[:-1])
-            assert cond.sum().item() == 0, "Should not happen"
+        # Alternative implementation using `torch.histgoramdd()`
+        x_bins = torch.arange(self.resolution[0] * self.psf_ratio + 1).type(hit_positions.dtype)
+        y_bins = torch.arange(self.resolution[1] * self.psf_ratio + 1).type(hit_positions.dtype)
+
+        # Image convention: vertical axis first, horizontal axis second
+        img, bins = torch.histogramdd(hit_positions[:, :2].cpu(), bins=(y_bins, x_bins), weight=luminosities.cpu())
+        img = torch.unsqueeze(img, -1)
+
+        self.depth_images[depth_id] += img.to(hit_positions.device)
+
+        # # Update pixel values
+        # indices = torch.floor(hit_positions[:, 1].type(torch.float64)).type(torch.int64) * (
+        #             self.resolution[1] * self.psf_ratio) + \
+        #           torch.floor(hit_positions[:, 0].type(torch.float64)).type(torch.int64)
+        # max_nb_identical_indices = indices.unique(return_counts=True)[1].max()
+        # sorted_indices, arg_sorted_indices = torch.sort(indices)
+
+        # for i in range(max_nb_identical_indices):
+        #     ind = sorted_indices[i::max_nb_identical_indices]
+        #     arg_ind = arg_sorted_indices[i::max_nb_identical_indices]
+
+        #     # Sanity check, should be removed
+        #     cond = (ind[1:] == ind[:-1])
+        #     assert cond.sum().item() == 0, "Should not happen"
 
-            self.depth_images[depth_id][ind % (self.resolution[1] * self.psf_ratio),
-                                        ind // (self.resolution[1] * self.psf_ratio)] += luminosities[arg_ind, None]
+        #     self.depth_images[depth_id][ind % (self.resolution[1] * self.psf_ratio),
+        #                                 ind // (self.resolution[1] * self.psf_ratio)] += luminosities[arg_ind, None]
 
     def readout(self, add_poisson_noise=True, destructive_readout=True):
         """
         Readouts the sensor
 
         :param add_poisson_noise: Whether to add poisson noise or no (:obj:`bool`)
         :param destructive_readout: Whether the accumulated photons should be destroyed or no (:obj:`bool`)
@@ -215,7 +227,34 @@
 
         points = torch.zeros((nb_points, 3), device=device)
         points[:, 0] = torch.rand(nb_points, device=device) * (self.pixel_size[0] * self.resolution[0]) - (
                 self.pixel_size[0] * self.resolution[0] / 2)
         points[:, 1] = torch.rand(nb_points, device=device) * (self.pixel_size[1] * self.resolution[1]) - (
                 self.pixel_size[1] * self.resolution[1] / 2)
         return self.c2w.apply_transform_(points)
+
+    def sample_on_pixels(self, samples_per_pixel, idx, idy, device='cpu'):
+        """
+        Sample data on the pixels whose id are provided
+
+        :param samples_per_pixel: Number of samples per pixel (:obj:`int`)
+        :param idx: Pixel indices along the horizontal axis, assuming a coordinate system centered in the center of
+                    the image(:obj:`torch.tensor`)
+        :param idy: Pixel indices along the vertical axis, assuming a coordinate system centered in the center of
+                    the image(:obj:`torch.tensor`)
+        :param device: The desired device of returned tensor (:obj:`str`). Default is ``'cpu'``
+
+        :return: (:obj:`tuple`) Sampled points (:obj:`torch.tensor`) and p(A) (:obj:`float`)
+        """
+
+        assert idx.shape[0] == idy.shape[0]
+        nb_pixels = idx.shape[0]
+
+        samples = torch.zeros((nb_pixels, samples_per_pixel, 3), device=device)
+        samples[:, :, 0] = (idx.to(device)[..., None] - .5) * self.pixel_size[0]
+        samples[:, :, 1] = (idy.to(device)[..., None] - .5) * self.pixel_size[1]
+
+        return (self.c2w.apply_transform_(samples.reshape(-1, 3)).reshape((nb_pixels, samples_per_pixel, 3)),
+                1 / (self.resolution[0] * self.pixel_size[0] * self.resolution[1] * self.pixel_size[1]))
+
+
+
```

### Comparing `gradoptics-0.0.3/src/gradoptics/optics/vector.py` & `gradoptics-0.0.4/src/gradoptics/optics/vector.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/optics/window.py` & `gradoptics-0.0.4/src/gradoptics/optics/window.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import torch
 
 from gradoptics.optics.base_optics import BaseOptics
 from gradoptics.optics.ray import Rays
 from gradoptics.optics.vector import dot_product
+from gradoptics.transforms.simple_transform import SimpleTransform
 
 
 class Window(BaseOptics):
     """
     Models a medium with a refractive index between two parallel surfaces. Refraction is modelled using Snell's law.
     """
 
     def __init__(self, left_interface_x_position, right_interface_x_position, n_ext=1.000293, n_glass=1.494,
-                 diameter=0.137, eps=1e-15):
+                 diameter=0.137, eps=1e-15, orientation=(0., 0., 0.)):
         """
         :param left_interface_x_position: Position of the left interface along the x axis (:obj:`float`)
         :param right_interface_x_position: Position of the right interface along the x axis (:obj:`float`)
         :param n_ext: Refractive index of the external medium (:obj:`float`)
         :param n_glass: Refractive index of the medium (:obj:`float`)
         :param diameter: Diameter of the interfaces (:obj:`float`)
         :param eps: Parameter used for numerical stability in the different class methods (:obj:`float`). Default
@@ -27,21 +28,25 @@
 
         self.diameter = diameter
         self.right_interface_x_position = right_interface_x_position
         self.left_interface_x_position = left_interface_x_position
         self.n_ext = n_ext
         self.n_glass = n_glass
         self.eps = eps
+        self.w2obj = SimpleTransform(*orientation, torch.zeros(3))
 
     def _get_ray_intersection_left_interface(self, incident_rays):
         """
         Computes the times t at which the incident rays will intersect the left interface of the window
         :param incident_rays:
         :return:
         """
+        # Rotate to coords with window along positive x
+        incident_rays = self.w2obj.apply_inverse_transform(incident_rays) 
+
         origins = incident_rays.origins
         directions = incident_rays.directions
         t = (self.left_interface_x_position - origins[:, 0]) / (directions[:, 0] + self.eps)
         y = origins[:, 1] + t * directions[:, 1]
         z = origins[:, 2] + t * directions[:, 2]
         # Check that the intersection is real (t>0) and within the windows' aperture
         condition = (t > 1e-3) & ((y ** 2 + z ** 2) < (self.diameter / 2) ** 2)
@@ -51,25 +56,31 @@
     @torch.no_grad()
     def _get_ray_intersection_right_interface(self, incident_rays):
         """
         Computes the times t at which the incident rays will intersect the right interface of the window
         :param incident_rays:
         :return:
         """
+        # Rotate to coords with window along positive x
+        incident_rays = self.w2obj.apply_inverse_transform(incident_rays) 
+
         origins = incident_rays.origins
         directions = incident_rays.directions
         t = (self.right_interface_x_position - origins[:, 0]) / (directions[:, 0] + self.eps)
         y = origins[:, 1] + t * directions[:, 1]
         z = origins[:, 2] + t * directions[:, 2]
         # Check that the intersection is real (t>0) and within the windows' aperture
         condition = (t > 1e-3) & ((y ** 2 + z ** 2) < (self.diameter / 2) ** 2)
         t[~condition] = float('inf')
         return t
 
     def _get_rays_inside_window(self, incident_rays, t):
+        
+        # Rotate to coords with window along positive x
+        incident_rays = self.w2obj.apply_inverse_transform(incident_rays)
 
         origins = incident_rays.origins
         directions = incident_rays.directions
         origin_refracted_rays = origins + t.unsqueeze(1) * directions
 
         # Interaction with the first interface
         window_normal = torch.zeros(directions.shape, device=directions.device, dtype=directions.dtype)
@@ -81,16 +92,27 @@
         mu = self.n_ext / self.n_glass
         # See https://physics.stackexchange.com/questions/435512/snells-law-in-vector-form
         tmp = 1 - mu ** 2 * (1 - (dot_product(window_normal, directions)) ** 2)
         c = dot_product(window_normal, directions)
         direction_refracted_rays = torch.sqrt(tmp).unsqueeze(1) * window_normal + mu * (
                 directions - c.unsqueeze(1) * window_normal)
 
-        return Rays(origin_refracted_rays, direction_refracted_rays, luminosities=incident_rays.luminosities,
-                    device=incident_rays.device), window_normal
+        output_rays = Rays(origin_refracted_rays, direction_refracted_rays, luminosities=incident_rays.luminosities,
+                    device=incident_rays.device)
+
+        # Rotate to back to world coords
+        output_rays = self.w2obj.apply_transform(output_rays) 
+
+        window_normal = torch.matmul(self.w2obj.transform.to(window_normal.device),
+                             torch.cat((window_normal.type(torch.double),
+                                        torch.zeros((window_normal.shape[0], 1), dtype=torch.double,
+                                                    device=window_normal.device)), dim=1).unsqueeze(-1))[:, :3, 0].type(
+                                    window_normal.dtype)
+                    
+        return output_rays, window_normal
 
     def _get_t_min(self, incident_rays):
         """
         Computes the times t at which the incident rays will intersect the window
         :param incident_rays:
         :return:
         """
@@ -129,14 +151,17 @@
         ray_in_glass, window_normal = self._get_rays_inside_window(incident_rays, t)
 
         # Interaction with the second interface
         t = self._get_t_min(ray_in_glass)
         ray_in_glass = ray_in_glass[~torch.isnan(t)]
         incident_rays.origins = incident_rays.origins[~torch.isnan(t)]
         incident_rays.directions = incident_rays.directions[~torch.isnan(t)]
+        incident_rays.luminosities = incident_rays.luminosities[~torch.isnan(t)]
+        for key in incident_rays.meta.keys():
+            incident_rays.meta[key] = incident_rays.meta[key][~torch.isnan(t)]
         window_normal = window_normal[~torch.isnan(t)]
         t = t[~torch.isnan(t)]
         origins = ray_in_glass.origins
         directions = ray_in_glass.directions
         origin_refracted_rays = origins + t.unsqueeze(1) * directions
         mu = self.n_glass / self.n_ext
         tmp = 1 - mu ** 2 * (1 - (dot_product(window_normal, directions)) ** 2)
@@ -160,9 +185,11 @@
 
         indices = (y ** 2 + z ** 2) < (self.diameter / 2) ** 2
         x_left = x[indices] + self.left_interface_x_position
         x_right = x[indices] + self.right_interface_x_position
         y = y[indices]
         z = z[indices]
 
-        ax.scatter(x_left, y, z, s=s, c=color)
-        ax.scatter(x_right, y, z, s=s, c=color)
+        x_left, y_left, z_left = self.w2obj.apply_transform_(torch.cat((x_left[:, None], y[:, None], z[:, None]), dim=1)).T
+        x_right, y_right, z_right = self.w2obj.apply_transform_(torch.cat((x_right[:, None], y[:, None], z[:, None]), dim=1)).T
+        ax.scatter(x_left, y_left, z_left, s=s, c=color)
+        ax.scatter(x_right, y_right, z_right, s=s, c=color)
```

### Comparing `gradoptics-0.0.3/src/gradoptics/ray_tracing/scene.py` & `gradoptics-0.0.4/src/gradoptics/ray_tracing/scene.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/transforms/base_transform.py` & `gradoptics-0.0.4/src/gradoptics/transforms/base_transform.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics/transforms/look_at_transform.py` & `gradoptics-0.0.4/src/gradoptics/transforms/look_at_transform.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,14 +21,20 @@
         :param pos: position of the object (:obj:`torch.tensor`)
         :param up: a vector that orients the object with respect to the viewing direction (:obj:`torch.tensor`).
                    For example, if up=torch.tensor([0, 0, 1]) the top of the object will point upwards.
                    If up=torch.tensor([0, 0, -1]), the top of the object will point downwards.
         """
         dir_ = normalize_vector(viewing_direction)
         left = normalize_vector(cross_product(normalize_vector(up), dir_))
+        if torch.allclose(left, torch.zeros(3)):
+            if torch.allclose(normalize_vector(up), torch.tensor([0., 0., 1.])):
+                left = torch.tensor([0., 1., 0.])
+            else:
+                raise NotImplementedError("Singular configuration!")
+                
         new_up = cross_product(dir_, left)
 
         self.transform = torch.tensor([[left[0], new_up[0], dir_[0], pos[0]],
                                        [left[1], new_up[1], dir_[1], pos[1]],
                                        [left[2], new_up[2], dir_[2], pos[2]],
                                        [0., 0., 0., 1.]], dtype=torch.double)
         self.inverse_transform = torch.inverse(self.transform)
```

### Comparing `gradoptics-0.0.3/src/gradoptics/transforms/simple_transform.py` & `gradoptics-0.0.4/src/gradoptics/transforms/simple_transform.py`

 * *Files identical despite different names*

### Comparing `gradoptics-0.0.3/src/gradoptics.egg-info/PKG-INFO` & `gradoptics-0.0.4/src/gradoptics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gradoptics
-Version: 0.0.3
+Version: 0.0.4
 Summary: Differentiable Optics via Ray Tracing
 Home-page: https://github.com/magis-slac/gradoptics
-Author: Sean Gasiorowski, Michael Kagan, Maxime Vandegar
-Author-email: Sean Gasiorowski <sgaz@slac.stanford.edu>, Michael Kagan <makagan@slac.stanford.edu>, Maxime Vandegar <maxime.vandegar@slac.stanford.edu>
+Author: Sean Gasiorowski, Michael Kagan, Maxime Vandegar, Sanha Cheong
+Author-email: Sean Gasiorowski <sgaz@slac.stanford.edu>, Michael Kagan <makagan@slac.stanford.edu>, Maxime Vandegar <maxime.vandegar@slac.stanford.edu>, Sanha Cheong <sanha@stanford.edu>
 License: MIT License
         
         Copyright (c) 2021 Michael Kagan, Maxime Vandegar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -36,15 +36,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/magis-slac/gradoptics/actions/workflows/main.yml/badge.svg)](https://github.com/magis-slac/gradoptics/actions)
 [![Build Status](https://travis-ci.com/magis-slac/gradoptics.svg?token=LBAvFbnCy9PEgexzsTUS&branch=main)](https://travis-ci.com/magis-slac/gradoptics)
 [![Documentation Status](https://readthedocs.org/projects/gradoptics/badge/?version=latest)](https://gradoptics.readthedocs.io/en/latest/?badge=latest)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/magis-slac/gradoptics/blob/master/README.md)
-![version](https://img.shields.io/badge/version-0.0.2-blue)
+![version](https://img.shields.io/badge/version-0.0.4-blue)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 # Differentiable Optics via Ray Tracing
 [*gradoptics*](https://github.com/magis-slac/gradoptics) is a ray tracing based optical simulator built using PyTorch [[1]](#1) to enable automatic differentiation. 
 
 The API is designed similar to rendering softwares, and has been heavily inspired by *Physically Based Rendering* (Pharr, Jakob, Humphreys) [[2]](#2).
```

### Comparing `gradoptics-0.0.3/src/gradoptics.egg-info/SOURCES.txt` & `gradoptics-0.0.4/src/gradoptics.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,22 +9,26 @@
 src/gradoptics.egg-info/dependency_links.txt
 src/gradoptics.egg-info/top_level.txt
 src/gradoptics/distributions/__init__.py
 src/gradoptics/distributions/atom_cloud.py
 src/gradoptics/distributions/atom_cloud_donut.py
 src/gradoptics/distributions/base_distribution.py
 src/gradoptics/distributions/gaussian_distribution.py
+src/gradoptics/distributions/point_source.py
+src/gradoptics/distributions/simple_atom_cloud.py
 src/gradoptics/inference/__init__.py
 src/gradoptics/inference/rejection_sampling.py
 src/gradoptics/integrator/__init__.py
 src/gradoptics/integrator/base_integrator.py
+src/gradoptics/integrator/hierarchical_sampling_integrator.py
 src/gradoptics/integrator/stratified_sampling_integrator.py
 src/gradoptics/light_sources/__init__.py
 src/gradoptics/light_sources/base_light_source.py
 src/gradoptics/light_sources/light_source_from_distribution.py
+src/gradoptics/light_sources/light_source_from_neural_net.py
 src/gradoptics/optics/__init__.py
 src/gradoptics/optics/base_optics.py
 src/gradoptics/optics/bounding_box.py
 src/gradoptics/optics/bounding_shape.py
 src/gradoptics/optics/bounding_sphere.py
 src/gradoptics/optics/camera.py
 src/gradoptics/optics/lens.py
```

### Comparing `gradoptics-0.0.3/tests/tests.py` & `gradoptics-0.0.4/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,14 @@
     plt.savefig('test_lens_transform.pdf')
     plt.close()
 
     return 0
 
 
 def _test_thick_lens(nb_rays=64):
-
     position = torch.tensor([0., 0., 0.])
     transform = optics.simple_transform.SimpleTransform(0, 0, 0, position)
     lens = optics.ThickLens(1.5, 1., 1, 1e-1, transform)
 
     # Create rays parallel to the optical axis
     y_pos = torch.linspace(-.1, .1, int(np.sqrt(nb_rays)))
     z_pos = torch.linspace(-.1, .1, int(np.sqrt(nb_rays)))
@@ -226,15 +225,15 @@
 
 
 def _ray_marching_test_lens(eps=1e-3):
     f = 0.05
     na = 1 / 1.4
 
     lens = optics.PerfectLens(f=f, na=na)
-    pts = lens.sample_points_on_lens(1000000)
+    pts, _ = lens.sample_points_on_lens(1000000)
 
     plt.figure()
     plt.hist2d(pts[:, 1].numpy(), pts[:, 2].numpy(), bins=40)
     plt.gca().set_aspect('equal')
     plt.colorbar()
     plt.savefig('test_ray_marching_lens.pdf')
     plt.close()
@@ -574,14 +573,40 @@
     plt.imshow(image)
     plt.savefig('test_backward_ray_tracing.pdf')
     plt.close()
 
     return 0
 
 
+def _test_render_pixel(f=0.05, m=0.15, N=60, device='cpu'):
+    # Creating a scene
+    lens = optics.PerfectLens(f=f, na=1 / 1.4, position=[0., 0., 0.], m=m)
+    sensor = optics.Sensor(resolution=(9600, 9600), pixel_size=(3.76e-6, 3.76e-6), position=(-f * (1 + m), 0, 0),
+                           poisson_noise_mean=2, quantum_efficiency=0.8)
+    atom_cloud = optics.AtomCloud(n=int(1e6), f=2, position=[f * (1 + m) / m, 0., 0.], phi=0.1)
+    light_source_bounding_shape = optics.BoundingSphere(radii=2e-3, xc=f * (1 + m) / m, yc=0.0, zc=0.0)
+    light_source = optics.LightSourceFromDistribution(atom_cloud, bounding_shape=light_source_bounding_shape)
+    scene = optics.Scene(light_source)
+    scene.add_object(lens)
+    scene.sensor = sensor
+
+    px_j, px_i = torch.meshgrid(torch.linspace(N, -N + 1, steps=N * 2), torch.linspace(N, -N + 1, steps=N * 2))
+    px_j = px_j.reshape(-1).type(torch.long)
+    px_i = px_i.reshape(-1).type(torch.long)
+
+    integrator = optics.StratifiedSamplingIntegrator(100)
+    img = optics.ray_tracing.ray_tracing.render_pixels(sensor, lens, scene, light_source, 5, 5, px_i, px_j,
+                                                       integrator, device='cpu', max_iterations=3)
+    img = img.reshape(2 * N, 2 * N)
+    plt.imshow(img.data.numpy())
+    plt.savefig('test_render_pixel.pdf')
+    plt.close()
+    return 0
+
+
 def _test_curved_mirrors():
     # Creating a scene
     f = 0.05
     m = 0.15
     lens = optics.PerfectLens(f=f, na=1 / 1.4, position=[0., 0., 0.], m=m)
     sensor = optics.Sensor(position=(-f * (1 + m), 0, 0))
     atom_cloud = optics.AtomCloud(n=int(1e6), f=2, position=[f * (1 + m) / m / 2, 0., 0.], phi=0.1)
@@ -693,7 +718,11 @@
 
 def test_backward_ray_tracing():
     assert _test_backward_ray_tracing() == 0
 
 
 def test_curved_mirrors():
     assert _test_curved_mirrors() == 0
+
+
+def test_render_pixel():
+    assert _test_render_pixel() == 0
```

