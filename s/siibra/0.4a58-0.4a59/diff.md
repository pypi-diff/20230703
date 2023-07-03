# Comparing `tmp/siibra-0.4a58.tar.gz` & `tmp/siibra-0.4a59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siibra-0.4a58.tar", last modified: Tue Jun 27 11:07:25 2023, max compression
+gzip compressed data, was "siibra-0.4a59.tar", last modified: Mon Jul  3 11:01:32 2023, max compression
```

## Comparing `siibra-0.4a58.tar` & `siibra-0.4a59.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.531540 siibra-0.4a58/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 11:05:55.000000 siibra-0.4a58/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-27 11:05:55.000000 siibra-0.4a58/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-06-27 11:07:25.527539 siibra-0.4a58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-06-27 11:05:55.000000 siibra-0.4a58/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 11:07:25.531540 siibra-0.4a58/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-27 11:05:55.000000 siibra-0.4a58/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.519539 siibra-0.4a58/siibra/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25127 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.519539 siibra-0.4a58/siibra/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/configuration/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.519539 siibra-0.4a58/siibra/core/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/core/atlas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/core/concept.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/core/parcellation.py
--rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/core/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.519539 siibra-0.4a58/siibra/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/anchor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.519539 siibra-0.4a58/siibra/features/connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/connectivity/functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/connectivity/regional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/connectivity/streamline_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/connectivity/streamline_lengths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/connectivity/tracer_connectivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.519539 siibra-0.4a58/siibra/features/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/dataset/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (123)    15995 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.523539 siibra-0.4a58/siibra/features/image/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/image/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/image/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/image/volume_of_interest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.523539 siibra-0.4a58/siibra/features/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/bigbrain_intensity_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/cell_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/cortical_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/gene_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/layerwise_bigbrain_intensities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/layerwise_cell_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/receptor_density_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/receptor_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/regional_timeseries_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/features/tabular/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.523539 siibra-0.4a58/siibra/livequeries/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/livequeries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/livequeries/allen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/livequeries/bigbrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/livequeries/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/livequeries/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.523539 siibra-0.4a58/siibra/locations/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/locations/boundingbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/locations/location.py
--rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/locations/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/locations/pointset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.523539 siibra-0.4a58/siibra/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/retrieval/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/retrieval/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.527539 siibra-0.4a58/siibra/retrieval/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/retrieval/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26557 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/retrieval/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    20780 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/retrieval/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.527539 siibra-0.4a58/siibra/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/vocabularies/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)  1647972 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/vocabularies/gene_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/vocabularies/receptor_symbols.json
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/vocabularies/region_aliases.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.527539 siibra-0.4a58/siibra/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/volumes/gifti.py
--rw-r--r--   0 runner    (1001) docker     (123)    24048 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/volumes/neuroglancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/volumes/nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)    42497 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/volumes/parcellationmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/volumes/sparsemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-06-27 11:05:55.000000 siibra-0.4a58/siibra/volumes/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.519539 siibra-0.4a58/siibra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-06-27 11:07:25.000000 siibra-0.4a58/siibra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-27 11:07:25.000000 siibra-0.4a58/siibra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:07:25.000000 siibra-0.4a58/siibra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-27 11:07:25.000000 siibra-0.4a58/siibra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 11:07:25.000000 siibra-0.4a58/siibra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:07:25.527539 siibra-0.4a58/test/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-27 11:05:55.000000 siibra-0.4a58/test/test_siibra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.949725 siibra-0.4a59/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 11:00:14.000000 siibra-0.4a59/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-03 11:00:14.000000 siibra-0.4a59/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-03 11:01:32.949725 siibra-0.4a59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-03 11:00:14.000000 siibra-0.4a59/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:01:32.949725 siibra-0.4a59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-03 11:00:14.000000 siibra-0.4a59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.937725 siibra-0.4a59/siibra/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25127 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.941725 siibra-0.4a59/siibra/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/configuration/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.941725 siibra-0.4a59/siibra/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/core/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/core/concept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/core/parcellation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/core/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.941725 siibra-0.4a59/siibra/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/anchor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.941725 siibra-0.4a59/siibra/features/connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/connectivity/functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/connectivity/regional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/connectivity/streamline_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/connectivity/streamline_lengths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/connectivity/tracer_connectivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.941725 siibra-0.4a59/siibra/features/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/dataset/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16210 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.941725 siibra-0.4a59/siibra/features/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/image/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/image/volume_of_interest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.945725 siibra-0.4a59/siibra/features/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/bigbrain_intensity_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/cell_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/cortical_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/gene_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/layerwise_bigbrain_intensities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/layerwise_cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/receptor_density_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/receptor_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/regional_timeseries_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.945725 siibra-0.4a59/siibra/livequeries/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/livequeries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/livequeries/allen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/livequeries/bigbrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/livequeries/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/livequeries/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.945725 siibra-0.4a59/siibra/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/locations/boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/locations/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/locations/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/locations/pointset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.945725 siibra-0.4a59/siibra/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/retrieval/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/retrieval/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.945725 siibra-0.4a59/siibra/retrieval/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/retrieval/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26557 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/retrieval/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20780 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/retrieval/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.949725 siibra-0.4a59/siibra/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/vocabularies/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1647972 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/vocabularies/gene_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/vocabularies/receptor_symbols.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/vocabularies/region_aliases.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.949725 siibra-0.4a59/siibra/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/volumes/gifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24048 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/volumes/neuroglancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/volumes/nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43140 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/volumes/parcellationmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/volumes/sparsemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/volumes/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.941725 siibra-0.4a59/siibra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-03 11:01:32.000000 siibra-0.4a59/siibra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-03 11:01:32.000000 siibra-0.4a59/siibra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:01:32.000000 siibra-0.4a59/siibra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-03 11:01:32.000000 siibra-0.4a59/siibra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 11:01:32.000000 siibra-0.4a59/siibra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.949725 siibra-0.4a59/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-03 11:00:14.000000 siibra-0.4a59/test/test_siibra.py
```

### Comparing `siibra-0.4a58/LICENSE` & `siibra-0.4a59/LICENSE`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/PKG-INFO` & `siibra-0.4a59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 0.4a58
+Version: 0.4a59
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `siibra-0.4a58/README.rst` & `siibra-0.4a59/README.rst`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/setup.py` & `siibra-0.4a59/setup.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/__init__.py` & `siibra-0.4a59/siibra/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/commons.py` & `siibra-0.4a59/siibra/commons.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/configuration/__init__.py` & `siibra-0.4a59/siibra/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/configuration/configuration.py` & `siibra-0.4a59/siibra/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/configuration/factory.py` & `siibra-0.4a59/siibra/configuration/factory.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/core/__init__.py` & `siibra-0.4a59/siibra/core/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/core/atlas.py` & `siibra-0.4a59/siibra/core/atlas.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/core/concept.py` & `siibra-0.4a59/siibra/core/concept.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/core/parcellation.py` & `siibra-0.4a59/siibra/core/parcellation.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/core/region.py` & `siibra-0.4a59/siibra/core/region.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/core/space.py` & `siibra-0.4a59/siibra/core/space.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/__init__.py` & `siibra-0.4a59/siibra/features/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/anchor.py` & `siibra-0.4a59/siibra/features/anchor.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/connectivity/__init__.py` & `siibra-0.4a59/siibra/features/connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/connectivity/functional_connectivity.py` & `siibra-0.4a59/siibra/features/connectivity/functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/connectivity/regional_connectivity.py` & `siibra-0.4a59/siibra/features/connectivity/regional_connectivity.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,22 @@
 from .. import anchor as _anchor
 
 from ...commons import logger, QUIET, siibra_tqdm
 from ...core import region as _region
 from ...locations import pointset
 from ...retrieval.repositories import RepositoryConnector
 
-from typing import Callable, Dict, Union, List
 import pandas as pd
 import numpy as np
+from typing import Callable, Dict, Union, List
+try:
+    from typing import Literal
+except ImportError:  # support python 3.7
+    from typing_extensions import Literal
+
 
 
 class RegionalConnectivity(Feature):
     """
     Parcellation-averaged connectivity, providing one or more matrices of a
     given modality for a given parcellation.
     """
@@ -134,29 +139,34 @@
             subject = next(iter(self._files.keys()))
         if subject not in self._files:
             raise ValueError(f"Subject name '{subject}' not known, use one of: {', '.join(self._files)}")
         if subject not in self._matrices:
             self._matrices[subject] = self._load_matrix(subject)
         return self._matrices[subject].copy()
 
-    def plot_matrix(self, subject: str = None, regions: List[str] = None, logscale: bool = False, **kwargs):
+    def plot_matrix(
+        self, subject: str = None, regions: List[str] = None,
+        logscale: bool = False, *args, backend="nilearn", **kwargs
+    ):
         """
         Plots the heatmap of the connectivity matrix using nilearn.plotting.
 
         Parameters
         ----------
         subject: str
             Name of the subject (see ConnectivityMatrix.subjects for available names).
             If "mean" or None is given, the mean is taken in case of multiple
             available matrices.
         regions: list[str]
             Display the matrix only for selected regions. By default, shows all the regions.
             It can only be a subset of regions of the feature.
         logscale: bool
             Display the data in log10 scale
+        backend: str
+            "nilearn" or "plotly"
         **kwargs:
             Can take all the arguments `nilearn.plotting.plot_matrix` can take. See the doc at
             https://nilearn.github.io/stable/modules/generated/nilearn.plotting.plot_matrix.html
         """
         if regions is None:
             regions = self.regions
         indices = [self.regions.index(r) for r in regions]
@@ -167,49 +177,64 @@
 
         # default kwargs
         subject_title = subject or ""
         kwargs["title"] = kwargs.get(
             "title",
             f"{subject_title} - {self.modality} in {', '.join({_.name for _ in self.anchor.regions})}"
         )
-        kwargs["figure"] = kwargs.get("figure", (15, 15))
 
-        from nilearn import plotting
-        plotting.plot_matrix(
-            matrix,
-            labels=regions,
-            **kwargs
-        )
+        if kwargs.get("reorder") or (backend == "nilearn"):
+            kwargs["figure"] = kwargs.get("figure", (15, 15))
+            from nilearn import plotting
+            plotting.plot_matrix(
+                matrix,
+                labels=regions,
+                **kwargs
+            )
+        elif backend == "plotly":
+            from plotly.express import imshow
+            return imshow(matrix, *args, x=regions, y=regions, **kwargs)
+        else:
+            raise NotImplementedError(
+                f"Plotting connectivity matrices with {backend} is not supported."
+            )
 
     def __iter__(self):
         return ((sid, self.get_matrix(sid)) for sid in self._files)
 
     def get_profile(
         self,
         region: Union[str, _region.Region],
         subject: str = None,
         min_connectivity: float = 0,
-        max_rows: int = None
+        max_rows: int = None,
+        direction: Literal['column', 'row'] = 'column'
     ):
         """
-        Extract a regional profile from the matrix, to obtain a tabular data feature
-        with the connectivity as the single column.
-
-        Rows will be sorted by descending connection strength.
-        Regions with connectivity smaller than "min_connectivity" will be discarded.
-        If max_rows is given, only the subset of regions with highest connectivity is returned.
+        Extract a regional profile from the matrix, to obtain a tabular data
+        feature with the connectivity as the single column. Rows are be sorted
+        by descending connection strength.
 
         Parameters
         ----------
         region: str, Region
         subject: str, default: None
         min_connectivity: float, default: 0
+            Regions with connectivity less than this value are discarded.
         max_rows: int, default: None
+            Max number of regions with highest connectivity.
+        direction: str, default: 'column'
+            Choose the direction of profile extraction particularly for
+            non-symmetric matrices. ('column' or 'row')
         """
         matrix = self.get_matrix(subject)
+        if direction.lower() not in ['column', 'row']:
+            raise ValueError("Direction can only be 'column' or 'row'")
+        if direction.lower() == 'row':
+            matrix = matrix.transpose()
 
         def matches(r1, r2):
             if isinstance(r1, tuple):
                 return any(r.matches(r2) for r in r1)
             else:
                 assert isinstance(r1, _region.Region)
                 return r1.matches(r2)
@@ -287,14 +312,16 @@
 
     def _array_to_dataframe(self, array: np.ndarray) -> pd.DataFrame:
         """
         Convert a numpy array with the connectivity matrix to
         a DataFrame with regions as column and row headers.
         """
         df = pd.DataFrame(array)
+        if not all(all(df.iloc[:, i] == df.iloc[i, :]) for i in range(len(df))):
+            logger.warning("The connectivity matrix is not symmetric.")
         parcellations = self.anchor.represented_parcellations()
         assert len(parcellations) == 1
         parc = next(iter(parcellations))
         with QUIET:
             indexmap = {
                 i: parc.get_region(regionname, allow_tuple=True)
                 for i, regionname in enumerate(self.regions)
@@ -303,15 +330,15 @@
         try:
             assert len(indexmap) == nrows
             remapper = {
                 label - min(indexmap.keys()): region
                 for label, region in indexmap.items()
             }
             df = df.rename(index=remapper).rename(columns=remapper)
-        except:
+        except Exception:
             raise RuntimeError("Could not decode connectivity matrix regions.")
         return df
 
     def _load_matrix(self, subject: str):
         """
         Extract connectivity matrix.
         """
```

### Comparing `siibra-0.4a58/siibra/features/connectivity/streamline_counts.py` & `siibra-0.4a59/siibra/features/connectivity/streamline_counts.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/connectivity/streamline_lengths.py` & `siibra-0.4a59/siibra/features/connectivity/streamline_lengths.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/connectivity/tracer_connectivity.py` & `siibra-0.4a59/siibra/features/connectivity/tracer_connectivity.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/dataset/__init__.py` & `siibra-0.4a59/siibra/features/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/dataset/ebrains.py` & `siibra-0.4a59/siibra/features/dataset/ebrains.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/feature.py` & `siibra-0.4a59/siibra/features/feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,18 @@
         ]
         logger.debug(
             f"Built {len(cls._preconfigured_instances)} preconfigured {cls.__name__} "
             f"objects from {cls._configuration_folder}."
         )
         return cls._preconfigured_instances
 
+    def plot(self, *args, **kwargs):
+        """Feature subclasses override this with their customized plot methods."""
+        raise NotImplementedError("Generic feature class does not have a standardized plot.")
+
     @classmethod
     def clean_instances(cls):
         """ Removes all instantiated object instances"""
         cls._preconfigured_instances = None
 
     def matches(self, concept: concept.AtlasConcept) -> bool:
         if self.anchor and self.anchor.matches(concept):
```

### Comparing `siibra-0.4a58/siibra/features/image/__init__.py` & `siibra-0.4a59/siibra/features/image/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/image/image.py` & `siibra-0.4a59/siibra/features/image/image.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/image/sections.py` & `siibra-0.4a59/siibra/features/image/sections.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/image/volume_of_interest.py` & `siibra-0.4a59/siibra/features/image/volume_of_interest.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/tabular/__init__.py` & `siibra-0.4a59/siibra/features/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/tabular/bigbrain_intensity_profile.py` & `siibra-0.4a59/siibra/features/tabular/bigbrain_intensity_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/tabular/cell_density_profile.py` & `siibra-0.4a59/siibra/features/tabular/cell_density_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/tabular/cortical_profile.py` & `siibra-0.4a59/siibra/features/tabular/cortical_profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -155,47 +155,56 @@
     def data(self):
         """Return a pandas Series representing the profile."""
         self._check_sanity()
         return pd.DataFrame(
             self._values, index=self._depths, columns=[f"{self.modality} ({self.unit})"]
         )
 
-    def plot(self, **kwargs):
+    def plot(self, *args, backend="matplotlib", **kwargs):
         """
         Plot the profile.
 
-        Keyword arguments are passed on to the plot command.
-        'layercolor' can be used to specify a color for cortical layer shading.
+        Parameters
+        ----------
+        backend: str
+            "matplotlib", "plotly", or others supported by pandas DataFrame
+            plotting backend.
+        **kwargs
+            Keyword arguments are passed on to the plot command.
+            'layercolor' can be used to specify a color for cortical layer shading.
         """
         wrapwidth = kwargs.pop("textwrap") if "textwrap" in kwargs else 40
 
         kwargs["title"] = kwargs.get("title", "\n".join(wrap(self.name, wrapwidth)))
-        kwargs["xlabel"] = kwargs.get("xlabel", "Cortical depth")
-        kwargs["ylabel"] = kwargs.get("ylabel", self.unit)
-        kwargs["grid"] = kwargs.get("grid", True)
-        kwargs["ylim"] = kwargs.get("ylim", (0, max(self._values)))
-        layercolor = kwargs.pop("layercolor") if "layercolor" in kwargs else "black"
-        axs = self.data.plot(**kwargs)
-
-        if self.boundaries_mapped:
-            bvals = list(self.boundary_positions.values())
-            for i, (d1, d2) in enumerate(list(zip(bvals[:-1], bvals[1:]))):
-                axs.text(
-                    d1 + (d2 - d1) / 2.0,
-                    10,
-                    self.LAYERS[i + 1],
-                    weight="normal",
-                    ha="center",
-                )
-                if i % 2 == 0:
-                    axs.axvspan(d1, d2, color=layercolor, alpha=0.1)
 
-        axs.set_title(axs.get_title(), fontsize="medium")
-
-        return axs
+        if backend == "matplotlib":
+            kwargs["xlabel"] = kwargs.get("xlabel", "Cortical depth")
+            kwargs["ylabel"] = kwargs.get("ylabel", self.unit)
+            kwargs["grid"] = kwargs.get("grid", True)
+            kwargs["ylim"] = kwargs.get("ylim", (0, max(self._values)))
+            layercolor = kwargs.pop("layercolor") if "layercolor" in kwargs else "black"
+            axs = self.data.plot(*args, **kwargs, backend=backend)
+
+            if self.boundaries_mapped:
+                bvals = list(self.boundary_positions.values())
+                for i, (d1, d2) in enumerate(list(zip(bvals[:-1], bvals[1:]))):
+                    axs.text(
+                        d1 + (d2 - d1) / 2.0,
+                        10,
+                        self.LAYERS[i + 1],
+                        weight="normal",
+                        ha="center",
+                    )
+                    if i % 2 == 0:
+                        axs.axvspan(d1, d2, color=layercolor, alpha=0.1)
+
+            axs.set_title(axs.get_title(), fontsize="medium")
+            return axs
+        else:
+            return self.data.plot(*args, **kwargs, backend=backend)
 
     @property
     def _depths(self):
         """
         Returns a list of the relative cortical depths of the measured values in the range [0..1].
 
         To be implemented in derived class.
```

### Comparing `siibra-0.4a58/siibra/features/tabular/gene_expression.py` & `siibra-0.4a59/siibra/features/tabular/gene_expression.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .. import anchor as _anchor
 from . import tabular
 
-from ... import commons
+from ... import logger
 
 import pandas as pd
 from textwrap import wrap
 from typing import List
 try:
     from typing import TypedDict
 except ImportError:
@@ -92,15 +92,15 @@
         assert len(z_scores) == len(levels)
         assert len(genes) == len(levels)
         if additional_columns is not None:
             assert all(len(lst) == len(levels) for lst in additional_columns.values())
         else:
             additional_columns = {}
 
-        data = pd.DataFrame(
+        _data_cahced = pd.DataFrame(
             dict(
                 **{'level': levels, 'zscore': z_scores, 'gene': genes},
                 **additional_columns
             )
         )
         # data.index.name = 'probe_id'
         tabular.Tabular.__init__(
@@ -109,40 +109,54 @@
                 (self.DESCRIPTION + self.ALLEN_ATLAS_NOTIFICATION)
                 .replace('\n', ' ')
                 .replace('\t', '')
                 .strip()
             ),
             modality="Gene expression",
             anchor=anchor,
-            data=data,
+            data=_data_cahced,
             datasets=datasets
         )
         self.unit = "expression level"
 
-    def plot(self, **kwargs):
-        """ Create a bar plot of the average per gene."""
-
-        try:
-            import matplotlib.pyplot as plt
-        except ImportError:
-            commons.logger.error("matplotlib not available. Plotting of fingerprints disabled.")
-            return None
-
+    def plot(self, *args, backend="matplotlib", **kwargs):
+        """
+        Create a bar plot of the average per gene.
+        Parameters
+        ----------
+        backend: str
+            "matplotlib", "plotly", or others supported by pandas DataFrame
+            plotting backend.
+        **kwargs
+            Keyword arguments are passed on to the plot command.
+        """
         wrapwidth = kwargs.pop("textwrap") if "textwrap" in kwargs else 40
-
-        for arg in ['yerr', 'y', 'ylabel', 'xlabel', 'width']:
-            assert arg not in kwargs
-
         title = kwargs.pop("title", None) \
             or "\n".join(wrap(f"{self.modality} measured in {self.anchor._regionspec}", wrapwidth))
-        kwargs["grid"] = kwargs.get("grid", True)
-        kwargs["legend"] = kwargs.get("legend", False)
+        if backend == "matplotlib":
+            try:
+                import matplotlib.pyplot as plt
+            except ImportError:
+                logger.error("matplotlib not available. Plotting of fingerprints disabled.")
+                raise
+
+            for arg in ['yerr', 'y', 'ylabel', 'xlabel', 'width']:
+                assert arg not in kwargs
+            passed_kwarg = {
+                "kind": 'box', "grid": True, "legend": False, 'by': "gene",
+                'column': ['level'], 'showfliers': False, 'ax': None,
+                **kwargs
+            }
+            ax = self.data.plot(
+                *args, **passed_kwarg, backend=backend
+            )
 
-        # ax = plot_data.plot(kind="bar", **kwargs)
-        ax = self.data.boxplot(column=['level'], by='gene', ax=kwargs.get('ax', None), showfliers=False)
-        plt.title('')
-        plt.suptitle('')
-        ax.set_title(title, fontsize="medium")
-        ax.set_xticklabels(ax.get_xticklabels(), rotation=60, ha="right")
-        ax.set_xlabel("")
+            plt.title('')
+            plt.suptitle('')
+            ax.set_title(title, fontsize="medium")
+            ax.set_xticklabels(ax.get_xticklabels(), rotation=60, ha="right")
+            ax.set_xlabel("")
 
-        plt.tight_layout()
+            plt.tight_layout()
+            return ax
+        else:
+            return self.data.plot(kind='box', y='level', x='gene', **kwargs)
```

### Comparing `siibra-0.4a58/siibra/features/tabular/layerwise_bigbrain_intensities.py` & `siibra-0.4a59/siibra/features/tabular/layerwise_bigbrain_intensities.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/tabular/layerwise_cell_density.py` & `siibra-0.4a59/siibra/features/tabular/layerwise_cell_density.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,10 +105,10 @@
         assert len(self.species) == 1
         return commons.create_key("{}_{}_{}".format(
             self.dataset_id,
             self.species[0]['name'],
             self.regionspec
         ))
 
-    def plot(self, **kwargs):
+    def plot(self, *args, **kwargs):
         kwargs['ylabel'] = self.unit
-        super().plot(**kwargs)
+        super().plot(*args, **kwargs)
```

### Comparing `siibra-0.4a58/siibra/features/tabular/receptor_density_fingerprint.py` & `siibra-0.4a59/siibra/features/tabular/receptor_density_fingerprint.py`

 * *Files 12% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                     self._loader.data[mean_col],
                     self._loader.data[std_col]
                 ]).T,
                 index=self._loader.data[label_col],
                 columns=['mean', 'std']
             )
             self._data_cached.index.name = 'receptor'
-        return self._data_cached
+        return self._data_cached.copy()
 
     @classmethod
     def parse_tsv_data(cls, data: dict):
         units = {list(v.values())[3] for v in data.values()}
         labels = list(data.keys())
         assert len(units) == 1
         try:
@@ -107,54 +107,81 @@
         return {
             'unit': next(iter(units)),
             'labels': labels,
             'means': [float(m) if m.isnumeric() else 0 for m in mean],
             'stds': [float(s) if s.isnumeric() else 0 for s in std],
         }
 
-    def polar_plot(self, **kwargs):
-        """ Create a polar plot of the fingerprint. """
-        try:
-            import matplotlib.pyplot as plt
-        except ImportError:
-            commons.logger.error("matplotlib not available. Plotting of fingerprints disabled.")
-            return None
-        from collections import deque
+    def polar_plot(self, *args, backend='matplotlib', **kwargs):
+        """
+        Create a polar plot of the fingerprint.
+        backend: str
+            "matplotlib" or "plotly"
+        """
+        if backend == "matplotlib":
+            try:
+                import matplotlib.pyplot as plt
+            except ImportError:
+                commons.logger.error("matplotlib not available. Plotting of fingerprints disabled.")
+                return None
+            from collections import deque
 
-        # default args
-        wrapwidth = 40
-        y = kwargs.pop("y") if "y" in kwargs else self.data.columns[0]
-        yerr = kwargs.pop("yerr") if "yerr" in kwargs else None
-        if yerr is None:
-            yerr = 'std' if 'std' in self.data.columns else None
-        ax = kwargs.pop("ax") if "ax" in kwargs else plt.subplot(111, projection="polar")
+            # default args
+            wrapwidth = 40
+            y = kwargs.pop("y") if "y" in kwargs else self.data.columns[0]
+            yerr = kwargs.pop("yerr") if "yerr" in kwargs else None
+            if yerr is None:
+                yerr = 'std' if 'std' in self.data.columns else None
+            ax = kwargs.pop("ax") if "ax" in kwargs else plt.subplot(111, projection="polar")
 
-        datafield = y or self.data.columns[0]
-        if yerr is None and 'std' in self.data.columns:
-            yerr = 'std'
-        # values = list(self.data[datafield])
-        angles = deque(np.linspace(0, 2 * np.pi, self.data.shape[0] + 1)[:-1][::-1])
-        angles.rotate(5)
-        angles = list(angles)
-        # for the values, repeat the first element to have a closed plot
-        indices = list(range(self.data.shape[0])) + [0]
-        y = list(self.data[datafield].iloc[indices])
-        plt.plot(angles + [angles[0]], y, "k-", lw=3, **kwargs)
-        if yerr:
-            bounds0 = y - self.data[yerr].iloc[indices]
-            plt.plot(angles + [angles[0]], bounds0, "k", lw=0.5, **kwargs)
-            bounds1 = y + self.data[yerr].iloc[indices]
-            plt.plot(angles + [angles[0]], bounds1, "k", lw=0.5, **kwargs)
-        ax.set_xticks(angles)
-        ax.set_xticklabels([_ for _ in self.data.index])
-        ax.set_ylabel(self.unit)
-        ax.set_title(
-            "\n".join(wrap(f"{self.modality} anchored at {self.anchor._regionspec}", wrapwidth))
-        )
-        ax.tick_params(pad=9, labelsize=10)
-        ax.tick_params(axis="y", labelsize=8)
-        plt.tight_layout()
-        return ax
+            datafield = y or self.data.columns[0]
+            if yerr is None and 'std' in self.data.columns:
+                yerr = 'std'
+            # values = list(self.data[datafield])
+            angles = deque(np.linspace(0, 2 * np.pi, self.data.shape[0] + 1)[:-1][::-1])
+            angles.rotate(5)
+            angles = list(angles)
+            # for the values, repeat the first element to have a closed plot
+            indices = list(range(self.data.shape[0])) + [0]
+            y = list(self.data[datafield].iloc[indices])
+            plt.plot(angles + [angles[0]], y, "k-", lw=3, **kwargs)
+            if yerr:
+                bounds0 = y - self.data[yerr].iloc[indices]
+                plt.plot(angles + [angles[0]], bounds0, "k", lw=0.5, **kwargs)
+                bounds1 = y + self.data[yerr].iloc[indices]
+                plt.plot(angles + [angles[0]], bounds1, "k", lw=0.5, **kwargs)
+            ax.set_xticks(angles)
+            ax.set_xticklabels([_ for _ in self.data.index])
+            ax.set_ylabel(self.unit)
+            ax.set_title(
+                "\n".join(wrap(f"{self.modality} anchored at {self.anchor._regionspec}", wrapwidth))
+            )
+            ax.tick_params(pad=9, labelsize=10)
+            ax.tick_params(axis="y", labelsize=8)
+            plt.tight_layout()
+            return ax
+        elif backend == "plotly":
+            from plotly.express import line_polar
+            df = pd.DataFrame(
+                {
+                    "values": pd.concat(
+                        [
+                            self.data["mean"],
+                            self.data["mean"] - self.data["std"],
+                            self.data["mean"] + self.data["std"]
+                        ]
+                    ),
+                    "cat":
+                        len(self.data) * ["mean"] +\
+                        len(self.data) * ["mean - std"] +\
+                        len(self.data) * ["mean + std"]
+                }
+            )
+            return line_polar(
+                df, r="values", theta=df.index, color="cat", line_close=True, **kwargs
+            )
+        else:
+            raise NotImplementedError
 
-    def plot(self, **kwargs):
+    def plot(self, *args, **kwargs):
         kwargs['xlabel'] = ""
-        return super().plot(**kwargs)
+        return super().plot(*args, **kwargs)
```

### Comparing `siibra-0.4a58/siibra/features/tabular/receptor_density_profile.py` & `siibra-0.4a59/siibra/features/tabular/receptor_density_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/features/tabular/regional_timeseries_activity.py` & `siibra-0.4a59/siibra/features/tabular/regional_timeseries_activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,18 +192,18 @@
             remapper = {
                 label - min(indexmap.keys()): region
                 for label, region in indexmap.items()
             }
             df = df.rename(columns=remapper)
         return df
 
-    def plot(self, subject: str = None, **kwargs):
+    def plot(self, subject: str = None, *args, backend="matplotlib", **kwargs):
         table = self.get_table(subject)
         table.columns = [str(r) for r in table.columns]
-        return table.mean().plot(kind="bar", **kwargs)
+        return table.mean().plot(kind="bar", *args, backend=backend, **kwargs)
 
 
 class RegionalBOLD(
     RegionalTimeseriesActivity,
     configuration_folder="features/tabular/activity_timeseries/bold",
     category="functional"
 ):
```

### Comparing `siibra-0.4a58/siibra/features/tabular/tabular.py` & `siibra-0.4a59/siibra/features/tabular/tabular.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,45 +51,57 @@
             anchor=anchor,
             datasets=datasets
         )
         self._data_cached = data
 
     @property
     def data(self):
-        return self._data_cached
+        return self._data_cached.copy()
 
-    def plot(self, **kwargs):
+    def plot(self, *args, backend="matplotlib", **kwargs):
         """
         Create a bar plot of a columns of the data.
         Parameters
         ----------
+        backend: str
+            "matplotlib", "plotly", or others supported by pandas DataFrame
+            plotting backend.
         **kwargs
             takes Matplotlib.pyplot keyword arguments
         """
-
-        try:
-            import matplotlib.pyplot as plt
-        except ImportError:
-            commons.logger.error("matplotlib not available. Plotting of fingerprints disabled.")
-            return None
-
-        wrapwidth = kwargs.pop("textwrap") if "textwrap" in kwargs else 40
-
-        # default kwargs
         kwargs["y"] = kwargs.get("y", self.data.columns[0])
-        kwargs["yerr"] = kwargs.get("yerr", 'std' if 'std' in self.data.columns else None)
-        kwargs["width"] = kwargs.get("width", 0.95)
-        kwargs["ylabel"] = kwargs.get(
-            "ylabel",
-            f"{kwargs['y']} {self.unit if hasattr(self, 'unit') else ''}"
-        )
-        kwargs["xlabel"] = kwargs.get("xlabel")
-        kwargs["title"] = kwargs.get(
-            "title",
-            "\n".join(wrap(f"{self.modality} in {', '.join({_.name for _ in self.anchor.regions})}", wrapwidth))
-        )
-        kwargs["grid"] = kwargs.get("grid", True)
-        kwargs["legend"] = kwargs.get("legend", False)
-        ax = self.data.plot(kind="bar", **kwargs)
-        ax.set_title(ax.get_title(), fontsize="medium")
-        ax.set_xticklabels(ax.get_xticklabels(), rotation=60, ha="right")
-        plt.tight_layout()
+        if backend == "matplotlib":
+            try:
+                import matplotlib.pyplot as plt
+            except ImportError:
+                commons.logger.error("matplotlib not available. Plotting of fingerprints disabled.")
+                return None
+
+            wrapwidth = kwargs.pop("textwrap") if "textwrap" in kwargs else 40
+            # default kwargs
+            if kwargs.get("error_y") is None:
+                kwargs["yerr"] = kwargs.get("yerr", 'std' if 'std' in self.data.columns else None)
+            kwargs["width"] = kwargs.get("width", 0.95)
+            kwargs["ylabel"] = kwargs.get(
+                "ylabel",
+                f"{kwargs['y']} {self.unit if hasattr(self, 'unit') else ''}"
+            )
+            kwargs["title"] = kwargs.get(
+                "title",
+                "\n".join(wrap(f"{self.modality} in {', '.join({_.name for _ in self.anchor.regions})}", wrapwidth))
+            )
+            kwargs["grid"] = kwargs.get("grid", True)
+            kwargs["legend"] = kwargs.get("legend", False)
+            ax = self.data.plot(kind="bar", *args, backend=backend, **kwargs)
+            ax.set_title(ax.get_title(), fontsize="medium")
+            ax.set_xticklabels(ax.get_xticklabels(), rotation=60, ha="right")
+            plt.tight_layout()
+            return ax
+        elif backend == "plotly":
+            kwargs["labels"] = {
+                "index": kwargs.pop("xlabel", ""),
+                "value": kwargs.pop("ylabel", f"{kwargs.get('y')} {self.unit if hasattr(self, 'unit') else ''}")
+            }
+            kwargs["error_y"] = kwargs.get("yerr", 'std' if 'std' in self.data.columns else None)
+            return self.data.plot(kind="bar", *args, backend=backend, **kwargs)
+        else:
+            return self.data.plot(*args, backend=backend, **kwargs)
```

### Comparing `siibra-0.4a58/siibra/livequeries/__init__.py` & `siibra-0.4a59/siibra/livequeries/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/livequeries/allen.py` & `siibra-0.4a59/siibra/livequeries/allen.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/livequeries/bigbrain.py` & `siibra-0.4a59/siibra/livequeries/bigbrain.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/livequeries/ebrains.py` & `siibra-0.4a59/siibra/livequeries/ebrains.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/livequeries/query.py` & `siibra-0.4a59/siibra/livequeries/query.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/locations/__init__.py` & `siibra-0.4a59/siibra/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/locations/boundingbox.py` & `siibra-0.4a59/siibra/locations/boundingbox.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/locations/location.py` & `siibra-0.4a59/siibra/locations/location.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/locations/point.py` & `siibra-0.4a59/siibra/locations/point.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/locations/pointset.py` & `siibra-0.4a59/siibra/locations/pointset.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/retrieval/__init__.py` & `siibra-0.4a59/siibra/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/retrieval/cache.py` & `siibra-0.4a59/siibra/retrieval/cache.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/retrieval/datasets.py` & `siibra-0.4a59/siibra/retrieval/datasets.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/retrieval/repositories.py` & `siibra-0.4a59/siibra/retrieval/repositories.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/retrieval/requests.py` & `siibra-0.4a59/siibra/retrieval/requests.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/vocabularies/__init__.py` & `siibra-0.4a59/siibra/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/vocabularies/gene_names.json` & `siibra-0.4a59/siibra/vocabularies/gene_names.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/vocabularies/receptor_symbols.json` & `siibra-0.4a59/siibra/vocabularies/receptor_symbols.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/vocabularies/region_aliases.json` & `siibra-0.4a59/siibra/vocabularies/region_aliases.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/volumes/__init__.py` & `siibra-0.4a59/siibra/volumes/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/volumes/gifti.py` & `siibra-0.4a59/siibra/volumes/gifti.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/volumes/neuroglancer.py` & `siibra-0.4a59/siibra/volumes/neuroglancer.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/volumes/nifti.py` & `siibra-0.4a59/siibra/volumes/nifti.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/volumes/parcellationmap.py` & `siibra-0.4a59/siibra/volumes/parcellationmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -597,15 +597,36 @@
             centroid_vox = np.array(np.where(maparr == index.label)).mean(1)
             assert regionname not in centroids
             centroids[regionname] = point.Point(
                 np.dot(mapimg.affine, np.r_[centroid_vox, 1])[:3], space=self.space
             )
         return centroids
 
-    def colorize(self, values: dict, **kwargs):
+    def get_resampled_template(self, **fetch_kwargs) -> Nifti1Image:
+        """
+        Resample the reference space template to fetched map image. Uses
+        nilearn.image.resample_to_img to resample the template.
+
+        Parameters
+        ----------
+        **fetch_kwargs: takes the arguments of Map.fetch()
+
+        Returns
+        -------
+        Nifti1Image
+        """
+        source_template = self.space.get_template().fetch()
+        map_image = self.fetch(**fetch_kwargs)
+        return image.resample_to_img(
+            source_template,
+            map_image,
+            interpolation='continuous'
+        )
+
+    def colorize(self, values: dict, **kwargs) -> Nifti1Image:
         """Colorize the map with the provided regional values.
 
         Parameters
         ----------
         values : dict
             Dictionary mapping regions to values
```

### Comparing `siibra-0.4a58/siibra/volumes/sparsemap.py` & `siibra-0.4a59/siibra/volumes/sparsemap.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra/volumes/volume.py` & `siibra-0.4a59/siibra/volumes/volume.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/siibra.egg-info/PKG-INFO` & `siibra-0.4a59/siibra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 0.4a58
+Version: 0.4a59
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `siibra-0.4a58/siibra.egg-info/SOURCES.txt` & `siibra-0.4a59/siibra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `siibra-0.4a58/test/test_siibra.py` & `siibra-0.4a59/test/test_siibra.py`

 * *Files identical despite different names*

