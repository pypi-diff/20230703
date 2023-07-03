# Comparing `tmp/kedro-datasets-1.4.1.tar.gz` & `tmp/kedro-datasets-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-datasets-1.4.1.tar", last modified: Tue Jun 13 16:50:01 2023, max compression
+gzip compressed data, was "kedro-datasets-1.4.2.tar", last modified: Mon Jul  3 09:51:23 2023, max compression
```

## Comparing `kedro-datasets-1.4.1.tar` & `kedro-datasets-1.4.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.935040 kedro-datasets-1.4.1/kedro_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/api/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/api/api_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/biosequence/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/biosequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/biosequence/biosequence_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/dask/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/dask/parquet_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16973 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/databricks/managed_table_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/email/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/email/message_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/geopandas/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/geopandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/geopandas/geojson_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/holoviews/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/holoviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/holoviews/holoviews_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/json/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/json/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/matplotlib/matplotlib_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/networkx/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/networkx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/networkx/gml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/networkx/graphml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/networkx/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.943040 kedro-datasets-1.4.1/kedro_datasets/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/feather_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/gbq_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/generic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/hdf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/parquet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/sql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/xml_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.943040 kedro-datasets-1.4.1/kedro_datasets/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pickle/pickle_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.943040 kedro-datasets-1.4.1/kedro_datasets/pillow/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pillow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pillow/image_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.943040 kedro-datasets-1.4.1/kedro_datasets/plotly/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/plotly/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/plotly/plotly_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.943040 kedro-datasets-1.4.1/kedro_datasets/polars/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/polars/csv_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.943040 kedro-datasets-1.4.1/kedro_datasets/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/redis/redis_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.943040 kedro-datasets-1.4.1/kedro_datasets/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/snowflake/snowpark_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/kedro_datasets/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/spark/deltatable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/spark/spark_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/spark/spark_hive_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/spark/spark_jdbc_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/spark/spark_streaming_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/kedro_datasets/svmlight/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/svmlight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/svmlight/svmlight_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/kedro_datasets/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/tensorflow/tensorflow_model_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/kedro_datasets/text/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/text/text_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/kedro_datasets/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/tracking/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/tracking/metrics_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/kedro_datasets/video/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/video/video_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/kedro_datasets/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/yaml/yaml_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-13 16:50:01.000000 kedro-datasets-1.4.1/kedro_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-13 16:50:01.000000 kedro-datasets-1.4.1/kedro_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:50:01.000000 kedro-datasets-1.4.1/kedro_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-13 16:50:01.000000 kedro-datasets-1.4.1/kedro_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 16:50:01.000000 kedro-datasets-1.4.1/kedro_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.892485 kedro-datasets-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-03 09:51:23.892485 kedro-datasets-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/api/api_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/biosequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/biosequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/biosequence/biosequence_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/dask/parquet_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/databricks/managed_table_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/email/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/email/message_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/geopandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/geopandas/geojson_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/holoviews/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/holoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/holoviews/holoviews_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/json/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/matplotlib/matplotlib_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/networkx/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/networkx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/networkx/gml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/networkx/graphml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/networkx/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/feather_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/gbq_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9944 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/generic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/hdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/parquet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/sql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/xml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pickle/pickle_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/pillow/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pillow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pillow/image_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/plotly/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/plotly/plotly_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/polars/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/polars/csv_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/redis/redis_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/snowflake/snowpark_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/spark/deltatable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/spark/spark_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/spark/spark_hive_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/spark/spark_jdbc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/spark/spark_streaming_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/svmlight/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/svmlight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/svmlight/svmlight_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/tensorflow/tensorflow_model_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.892485 kedro-datasets-1.4.2/kedro_datasets/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/text/text_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.892485 kedro-datasets-1.4.2/kedro_datasets/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/tracking/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/tracking/metrics_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.892485 kedro-datasets-1.4.2/kedro_datasets/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/video/video_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.892485 kedro-datasets-1.4.2/kedro_datasets/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/yaml/yaml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-03 09:51:23.000000 kedro-datasets-1.4.2/kedro_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-03 09:51:23.000000 kedro-datasets-1.4.2/kedro_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:51:23.000000 kedro-datasets-1.4.2/kedro_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-03 09:51:23.000000 kedro-datasets-1.4.2/kedro_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 09:51:23.000000 kedro-datasets-1.4.2/kedro_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 09:51:23.892485 kedro-datasets-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/setup.py
```

### Comparing `kedro-datasets-1.4.1/PKG-INFO` & `kedro-datasets-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-datasets
-Version: 1.4.1
+Version: 1.4.2
 Summary: Kedro-Datasets is where you can find all of Kedro's data connectors.
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: <3.11,>=3.7
```

### Comparing `kedro-datasets-1.4.1/README.md` & `kedro-datasets-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/api/api_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/api/api_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/biosequence/biosequence_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/biosequence/biosequence_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 from typing import Any, Dict, List
 
 import fsspec
 from Bio import SeqIO
 from kedro.io.core import AbstractDataSet, get_filepath_str, get_protocol_and_path
 
 
-class BioSequenceDataSet(
-    AbstractDataSet[List, List]
-):  # pylint:disable=too-many-instance-attributes
+class BioSequenceDataSet(AbstractDataSet[List, List]):
     r"""``BioSequenceDataSet`` loads and saves data to a sequence file.
 
     Example:
     ::
 
         >>> from kedro_datasets.biosequence import BioSequenceDataSet
         >>> from io import StringIO
```

### Comparing `kedro-datasets-1.4.1/kedro_datasets/dask/parquet_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/dask/parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/databricks/managed_table_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/databricks/managed_table_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pyspark.sql.types import StructType
 from pyspark.sql.utils import AnalysisException, ParseException
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass(frozen=True)
-class ManagedTable:  # pylint: disable=too-many-instance-attributes
+class ManagedTable:
     """Stores the definition of a managed table"""
 
     # regex for tables, catalogs and schemas
     _NAMING_REGEX = r"\b[0-9a-zA-Z_-]{1,}\b"
     _VALID_WRITE_MODES = ["overwrite", "upsert", "append"]
     _VALID_DATAFRAME_TYPES = ["spark", "pandas"]
     database: str
@@ -140,55 +140,56 @@
         except (KeyError, ValueError) as exc:
             raise DataSetError(exc) from exc
         return schema
 
 
 class ManagedTableDataSet(AbstractVersionedDataSet):
     """``ManagedTableDataSet`` loads and saves data into managed delta tables on Databricks.
-        Load and save can be in Spark or Pandas dataframes, specified in dataframe_type.
-        When saving data, you can specify one of three modes: overwrite(default), append,
-        or upsert. Upsert requires you to specify the primary_column parameter which
-        will be used as part of the join condition. This dataset works best with
-        the databricks kedro starter. That starter comes with hooks that allow this
-        dataset to function properly. Follow the instructions in that starter to
-        setup your project for this dataset.
-
-        Example usage for the
-        `YAML API <https://kedro.readthedocs.io/en/stable/data/\
-        data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
-
-        .. code-block:: yaml
-
-            names_and_ages@spark:
-              type: databricks.ManagedTableDataSet
-              table: names_and_ages
-
-            names_and_ages@pandas:
-              type: databricks.ManagedTableDataSet
-              table: names_and_ages
-              dataframe_type: pandas
-
-        Example usage for the
-        `Python API <https://kedro.readthedocs.io/en/stable/data/\
-        data_catalog.html#use-the-data-catalog-with-the-code-api>`_:
-        .. code-block:: python
-
-            from pyspark.sql import SparkSession
-            from pyspark.sql.types import (StructField, StringType,
-                                            IntegerType, StructType)
-            from kedro_datasets.databricks import ManagedTableDataSet
-            schema = StructType([StructField("name", StringType(), True),
-                                 StructField("age", IntegerType(), True)])
-            data = [('Alex', 31), ('Bob', 12), ('Clarke', 65), ('Dave', 29)]
-            spark_df = SparkSession.builder.getOrCreate().createDataFrame(data, schema)
-            data_set = ManagedTableDataSet(table="names_and_ages")
-            data_set.save(spark_df)
-            reloaded = data_set.load()
-            reloaded.take(4)
-        """
+    Load and save can be in Spark or Pandas dataframes, specified in dataframe_type.
+    When saving data, you can specify one of three modes: overwrite(default), append,
+    or upsert. Upsert requires you to specify the primary_column parameter which
+    will be used as part of the join condition. This dataset works best with
+    the databricks kedro starter. That starter comes with hooks that allow this
+    dataset to function properly. Follow the instructions in that starter to
+    setup your project for this dataset.
+
+    Example usage for the
+    `YAML API <https://kedro.readthedocs.io/en/stable/data/\
+    data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
+
+    .. code-block:: yaml
+
+        names_and_ages@spark:
+            type: databricks.ManagedTableDataSet
+            table: names_and_ages
+
+        names_and_ages@pandas:
+            type: databricks.ManagedTableDataSet
+            table: names_and_ages
+            dataframe_type: pandas
+
+    Example usage for the
+    `Python API <https://kedro.readthedocs.io/en/stable/data/\
+    data_catalog.html#use-the-data-catalog-with-the-code-api>`_:
+
+    .. code-block:: python
+
+        from pyspark.sql import SparkSession
+        from pyspark.sql.types import (StructField, StringType,
+                                        IntegerType, StructType)
+        from kedro_datasets.databricks import ManagedTableDataSet
+        schema = StructType([StructField("name", StringType(), True),
+                                StructField("age", IntegerType(), True)])
+        data = [('Alex', 31), ('Bob', 12), ('Clarke', 65), ('Dave', 29)]
+        spark_df = SparkSession.builder.getOrCreate().createDataFrame(data, schema)
+        data_set = ManagedTableDataSet(table="names_and_ages")
+        data_set.save(spark_df)
+        reloaded = data_set.load()
+        reloaded.take(4)
+    """
 
     # this dataset cannot be used with ``ParallelRunner``,
     # therefore it has the attribute ``_SINGLE_PROCESS = True``
     # for parallelism within a Spark pipeline please consider
     # using ``ThreadRunner`` instead
     _SINGLE_PROCESS = True
 
@@ -207,36 +208,36 @@
         schema: Dict[str, Any] = None,
         partition_columns: List[str] = None,
         owner_group: str = None,
     ) -> None:
         """Creates a new instance of ``ManagedTableDataSet``
 
         Args:
-            table (str): the name of the table
-            catalog (str, optional): the name of the catalog in Unity.
+            table: the name of the table
+            catalog: the name of the catalog in Unity.
              Defaults to None.
-            database (str, optional): the name of the database.
+            database: the name of the database.
              (also referred to as schema). Defaults to "default".
-            write_mode (str, optional): the mode to write the data into the table.
+            write_mode: the mode to write the data into the table.
              Options are:["overwrite", "append", "upsert"].
              "upsert" mode requires primary_key field to be populated.
              Defaults to "overwrite".
-            dataframe_type (str, optional): "pandas" or "spark" dataframe.
+            dataframe_type: "pandas" or "spark" dataframe.
              Defaults to "spark".
-            primary_key (Union[str, List[str]], optional): the primary key of the table.
+            primary_key: the primary key of the table.
              Can be in the form of a list. Defaults to None.
-            version (Version, optional): kedro.io.core.Version instance to load the data.
+            version: kedro.io.core.Version instance to load the data.
              Defaults to None.
-            schema (Dict[str, Any], optional): the schema of the table in JSON form.
+            schema: the schema of the table in JSON form.
              Dataframes will be truncated to match the schema if provided.
              Used by the hooks to create the table if the schema is provided
              Defaults to None.
-            partition_columns (List[str], optional): the columns to use for partitioning the table.
+            partition_columns: the columns to use for partitioning the table.
              Used by the hooks. Defaults to None.
-            owner_group (str, optional): if table access control is enabled in your workspace,
+            owner_group: if table access control is enabled in your workspace,
              specifying owner_group will transfer ownership of the table and database to
              this owner. All databases should have the same owner_group. Defaults to None.
         Raises:
             DataSetError: Invalid configuration supplied (through ManagedTable validation)
         """
 
         self._table = ManagedTable(
```

### Comparing `kedro-datasets-1.4.1/kedro_datasets/email/message_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/email/message_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,15 @@
     DataSetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
 
 
-class EmailMessageDataSet(
-    AbstractVersionedDataSet[Message, Message]
-):  # pylint: disable=too-many-instance-attributes
+class EmailMessageDataSet(AbstractVersionedDataSet[Message, Message]):
     """``EmailMessageDataSet`` loads/saves an email message from/to a file
     using an underlying filesystem (e.g.: local, S3, GCS). It uses the
     ``email`` package in the standard library to manage email messages.
 
     Note that ``EmailMessageDataSet`` doesn't handle sending email messages.
 
     Example:
```

### Comparing `kedro-datasets-1.4.1/kedro_datasets/geopandas/geojson_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/geopandas/geojson_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/holoviews/holoviews_writer.py` & `kedro-datasets-1.4.2/kedro_datasets/holoviews/holoviews_writer.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/json/json_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/json/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/matplotlib/matplotlib_writer.py` & `kedro-datasets-1.4.2/kedro_datasets/matplotlib/matplotlib_writer.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/networkx/gml_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/networkx/gml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/networkx/graphml_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/networkx/graphml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/networkx/json_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/networkx/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/pandas/__init__.py` & `kedro-datasets-1.4.2/kedro_datasets/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/pandas/csv_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/pandas/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/pandas/excel_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/pandas/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/pandas/feather_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/pandas/feather_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/pandas/gbq_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/pandas/gbq_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,15 @@
     DataSetError,
     get_filepath_str,
     get_protocol_and_path,
     validate_on_forbidden_chars,
 )
 
 
-class GBQTableDataSet(
-    AbstractDataSet[None, pd.DataFrame]
-):  # pylint:disable=too-many-instance-attributes
+class GBQTableDataSet(AbstractDataSet[None, pd.DataFrame]):
     """``GBQTableDataSet`` loads and saves data from/to Google BigQuery.
     It uses pandas-gbq to read and write from/to BigQuery table.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
 
@@ -174,17 +172,15 @@
                 """"load_args['location']" is different from "save_args['location']". """
                 "The 'location' defines where BigQuery data is stored, therefore has "
                 "to be the same for save and load args. "
                 "Details: https://cloud.google.com/bigquery/docs/locations"
             )
 
 
-class GBQQueryDataSet(
-    AbstractDataSet[None, pd.DataFrame]
-):  # pylint:disable=too-many-instance-attributes
+class GBQQueryDataSet(AbstractDataSet[None, pd.DataFrame]):
     """``GBQQueryDataSet`` loads data from a provided SQL query from Google
     BigQuery. It uses ``pandas.read_gbq`` which itself uses ``pandas-gbq``
     internally to read from BigQuery table. Therefore it supports all allowed
     pandas options on ``read_gbq``.
 
     Example adding a catalog entry with the ``YAML API``:
```

### Comparing `kedro-datasets-1.4.1/kedro_datasets/pandas/generic_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/pandas/generic_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,15 @@
     "records",
     "timestamp",
     "xarray",
     "sql_table",
 ]
 
 
-class GenericDataSet(
-    AbstractVersionedDataSet[pd.DataFrame, pd.DataFrame]
-):  # pylint:disable=too-many-instance-attributes
+class GenericDataSet(AbstractVersionedDataSet[pd.DataFrame, pd.DataFrame]):
     """`pandas.GenericDataSet` loads/saves data from/to a data file using an underlying
     filesystem (e.g.: local, S3, GCS). It uses pandas to dynamically select the
     appropriate type of read/write target on a best effort basis.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
```

### Comparing `kedro-datasets-1.4.1/kedro_datasets/pandas/hdf_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/pandas/hdf_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,15 @@
     get_filepath_str,
     get_protocol_and_path,
 )
 
 HDFSTORE_DRIVER = "H5FD_CORE"
 
 
-class HDFDataSet(
-    AbstractVersionedDataSet[pd.DataFrame, pd.DataFrame]
-):  # pylint:disable=too-many-instance-attributes
+class HDFDataSet(AbstractVersionedDataSet[pd.DataFrame, pd.DataFrame]):
     """``HDFDataSet`` loads/saves data from/to a hdf file using an underlying
     filesystem (e.g. local, S3, GCS). It uses pandas.HDFStore to handle the hdf file.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
```

### Comparing `kedro-datasets-1.4.1/kedro_datasets/pandas/json_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/pandas/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/pandas/parquet_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/pandas/parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/pandas/sql_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/pandas/sql_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/pandas/xml_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/pandas/xml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/pickle/pickle_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/pickle/pickle_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,15 @@
     DataSetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
 
 
-class PickleDataSet(
-    AbstractVersionedDataSet[Any, Any]
-):  # pylint:disable=too-many-instance-attributes
+class PickleDataSet(AbstractVersionedDataSet[Any, Any]):
     """``PickleDataSet`` loads/saves data from/to a Pickle file using an underlying
     filesystem (e.g.: local, S3, GCS). The underlying functionality is supported by
     the specified backend library passed in (defaults to the ``pickle`` library), so it
     supports all allowed options for loading and saving pickle files.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
```

### Comparing `kedro-datasets-1.4.1/kedro_datasets/pillow/image_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/pillow/image_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/plotly/json_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/plotly/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/plotly/plotly_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/plotly/plotly_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/polars/csv_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/polars/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/redis/redis_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/redis/redis_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 from copy import deepcopy
 from typing import Any, Dict
 
 import redis
 from kedro.io.core import AbstractDataSet, DataSetError
 
 
-class PickleDataSet(
-    AbstractDataSet[Any, Any]
-):  # pylint:disable=too-many-instance-attributes
+class PickleDataSet(AbstractDataSet[Any, Any]):
     """``PickleDataSet`` loads/saves data from/to a Redis database. The
     underlying functionality is supported by the redis library, so it supports
     all allowed options for instantiating the redis app ``from_url`` and setting
     a value.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
```

### Comparing `kedro-datasets-1.4.1/kedro_datasets/snowflake/snowpark_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/snowflake/snowpark_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 import snowflake.snowpark as sp
 from kedro.io.core import AbstractDataSet, DataSetError
 
 logger = logging.getLogger(__name__)
 
 
-class SnowparkTableDataSet(
-    AbstractDataSet
-):  # pylint:disable=too-many-instance-attributes
+class SnowparkTableDataSet(AbstractDataSet):
     """``SnowparkTableDataSet`` loads and saves Snowpark dataframes.
 
     As of Mar-2023, the snowpark connector only works with Python 3.8.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
```

### Comparing `kedro-datasets-1.4.1/kedro_datasets/spark/__init__.py` & `kedro-datasets-1.4.2/kedro_datasets/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/spark/deltatable_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/spark/deltatable_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/spark/spark_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/spark/spark_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/spark/spark_hive_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/spark/spark_hive_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/spark/spark_jdbc_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/spark/spark_jdbc_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/spark/spark_streaming_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/spark/spark_streaming_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,65 +11,67 @@
     SparkDataSet,
     _split_filepath,
     _strip_dbfs_prefix,
 )
 
 
 class SparkStreamingDataSet(AbstractDataSet):
-    """``SparkStreamingDataSet`` loads data into Spark Streaming Dataframe objects.
+    """``SparkStreamingDataSet`` loads data to Spark Streaming Dataframe objects.
+
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
+
     .. code-block:: yaml
+
         raw.new_inventory:
-        type: streaming.extras.datasets.spark_streaming_dataset.SparkStreamingDataSet
-        filepath: data/01_raw/stream/inventory/
-        file_format: json
-        save_args:
+          type: spark.SparkStreamingDataSet
+          filepath: data/01_raw/stream/inventory/
+          file_format: json
+          save_args:
             output_mode: append
             checkpoint: data/04_checkpoint/raw_new_inventory
             header: True
-        load_args:
+          load_args:
             schema:
-              filepath: data/01_raw/schema/inventory_schema.json
+                filepath: data/01_raw/schema/inventory_schema.json
     """
 
     DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
     DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
 
     def __init__(
         self,
         filepath: str = "",
         file_format: str = "",
         save_args: Dict[str, Any] = None,
         load_args: Dict[str, Any] = None,
     ) -> None:
         """Creates a new instance of SparkStreamingDataSet.
+
         Args:
             filepath: Filepath in POSIX format to a Spark dataframe. When using Databricks
                 specify ``filepath``s starting with ``/dbfs/``. For message brokers such as
                 Kafka and all filepath is not required.
-            file_format: File format used during load and save
-                operations. These are formats supported by the running
-                SparkContext include parquet, csv, delta. For a list of supported
-                formats please refer to Apache Spark documentation at
+            file_format: File format used during load and save operations.
+                These are formats supported by the running SparkContext including parquet,
+                csv, and delta. For a list of supported formats please refer to the Apache
+                Spark documentation at
                 https://spark.apache.org/docs/latest/structured-streaming-programming-guide.html
             load_args: Load args passed to Spark DataFrameReader load method.
-                It is dependent on the selected file format. You can find
-                a list of read options for each supported format
-                in Spark DataFrame read documentation:
-                https://spark.apache.org/docs/latest/structured-streaming-programming-guide.html,
+                It is dependent on the selected file format. You can find a list of read options
+                for each selected format in Spark DataFrame read documentation, see
+                https://spark.apache.org/docs/latest/structured-streaming-programming-guide.html.
                 Please note that a schema is mandatory for a streaming DataFrame
                 if ``schemaInference`` is not True.
-            save_args: Save args passed to Spark DataFrame write options.
-                Similar to load_args this is dependent on the selected file
-                format. You can pass ``mode`` and ``partitionBy`` to specify
-                your overwrite mode and partitioning respectively. You can find
-                a list of options for each format in Spark DataFrame
-                write documentation:
+            save_args: Save args passed to Spark DataFrameReader write options.
+                Similar to load_args, this is dependent on the selected file format. You can pass
+                ``mode`` and ``partitionBy`` to specify your overwrite mode and partitioning
+                respectively. You can find a list of options for each selected format in
+                Spark DataFrame write documentation, see
                 https://spark.apache.org/docs/latest/structured-streaming-programming-guide.html
         """
         self._file_format = file_format
         self._save_args = save_args
         self._load_args = load_args
 
         fs_prefix, filepath = _split_filepath(filepath)
```

### Comparing `kedro-datasets-1.4.1/kedro_datasets/svmlight/svmlight_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/svmlight/svmlight_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/tensorflow/tensorflow_model_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/tensorflow/tensorflow_model_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/text/text_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/text/text_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/tracking/json_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/tracking/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/tracking/metrics_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/tracking/metrics_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/video/video_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/video/video_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets/yaml/yaml_dataset.py` & `kedro-datasets-1.4.2/kedro_datasets/yaml/yaml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets.egg-info/PKG-INFO` & `kedro-datasets-1.4.2/kedro_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-datasets
-Version: 1.4.1
+Version: 1.4.2
 Summary: Kedro-Datasets is where you can find all of Kedro's data connectors.
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: <3.11,>=3.7
```

### Comparing `kedro-datasets-1.4.1/kedro_datasets.egg-info/SOURCES.txt` & `kedro-datasets-1.4.2/kedro_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.1/kedro_datasets.egg-info/requires.txt` & `kedro-datasets-1.4.2/kedro_datasets.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -74,22 +74,23 @@
 [databricks.ManagedTableDataSet]
 pyspark<4.0,>=2.2
 pandas<3.0,>=1.3
 delta-spark~=1.2.1
 
 [docs]
 docutils==0.16
-sphinx~=3.4.3
-sphinx_rtd_theme==0.4.1
-nbsphinx==0.8.1
-nbstripout~=0.4
-sphinx-autodoc-typehints==1.11.1
+sphinx~=5.3.0
+sphinx_rtd_theme==1.2.0
+sphinx-autodoc-typehints==1.20.2
 sphinx_copybutton==0.3.1
+sphinx-notfound-page
 ipykernel<7.0,>=5.3
-myst-parser~=0.17.2
+sphinxcontrib-mermaid~=0.7.1
+myst-parser~=1.0.0
+Jinja2<3.1.0
 
 [geopandas]
 geopandas<1.0,>=0.6.0
 pyproj~=3.0
 
 [geopandas.GeoJSONDataSet]
 geopandas<1.0,>=0.6.0
```

### Comparing `kedro-datasets-1.4.1/pyproject.toml` & `kedro-datasets-1.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     "pylint.extensions.no_self_use"
 ]
 extension-pkg-whitelist = "cv2"
 unsafe-load-any-extension = false
 [tool.pylint.messages_control]
 disable = [
     "ungrouped-imports",
-    "duplicate-code"
+    "duplicate-code",
+    "too-many-instance-attributes"
 ]
 enable = ["useless-suppression"]
 [tool.pylint.refactoring]
 max-nested-blocks = 5
 [tool.pylint.format]
 indent-after-paren=4
 indent-string="    "
```

### Comparing `kedro-datasets-1.4.1/setup.py` & `kedro-datasets-1.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -118,21 +118,26 @@
     **tensorflow_require,
     **video_require,
     **yaml_require,
 }
 
 extras_require["all"] = _collect_requirements(extras_require)
 extras_require["docs"] = [
+    # docutils>=0.17 changed the HTML
+    # see https://github.com/readthedocs/sphinx_rtd_theme/issues/1115
     "docutils==0.16",
-    "sphinx~=3.4.3",
-    "sphinx_rtd_theme==0.4.1",
-    "nbsphinx==0.8.1",
-    "nbstripout~=0.4",
-    "sphinx-autodoc-typehints==1.11.1",
+    "sphinx~=5.3.0",
+    "sphinx_rtd_theme==1.2.0",
+    # Regression on sphinx-autodoc-typehints 1.21
+    # that creates some problematic docstrings
+    "sphinx-autodoc-typehints==1.20.2",
     "sphinx_copybutton==0.3.1",
+    "sphinx-notfound-page",
     "ipykernel>=5.3, <7.0",
-    "myst-parser~=0.17.2",
+    "sphinxcontrib-mermaid~=0.7.1",
+    "myst-parser~=1.0.0",
+    "Jinja2<3.1.0",
 ]
 
 setup(
     extras_require=extras_require,
 )
```

