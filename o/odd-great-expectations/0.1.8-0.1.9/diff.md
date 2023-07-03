# Comparing `tmp/odd_great_expectations-0.1.8.tar.gz` & `tmp/odd_great_expectations-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odd_great_expectations-0.1.8.tar", max compression
+gzip compressed data, was "odd_great_expectations-0.1.9.tar", max compression
```

## Comparing `odd_great_expectations-0.1.8.tar` & `odd_great_expectations-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-02-08 16:33:47.000000 odd_great_expectations-0.1.8/LICENSE
--rw-r--r--   0        0        0     1583 2023-02-08 16:33:47.000000 odd_great_expectations-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-02-08 16:33:47.000000 odd_great_expectations-0.1.8/odd_great_expectations/__init__.py
--rw-r--r--   0        0        0     2675 2023-02-08 16:33:47.000000 odd_great_expectations-0.1.8/odd_great_expectations/action.py
--rw-r--r--   0        0        0     2102 2023-02-08 16:33:47.000000 odd_great_expectations-0.1.8/odd_great_expectations/client.py
--rw-r--r--   0        0        0       80 2023-02-08 16:33:47.000000 odd_great_expectations-0.1.8/odd_great_expectations/dataset/__init__.py
--rw-r--r--   0        0        0      698 2023-02-08 16:33:47.000000 odd_great_expectations-0.1.8/odd_great_expectations/dataset/file.py
--rw-r--r--   0        0        0      769 2023-02-08 16:33:47.000000 odd_great_expectations-0.1.8/odd_great_expectations/dataset/get_dataset.py
--rw-r--r--   0        0        0     1623 2023-02-08 16:33:47.000000 odd_great_expectations-0.1.8/odd_great_expectations/dataset/sql_table.py
--rw-r--r--   0        0        0      565 2023-02-08 16:33:47.000000 odd_great_expectations-0.1.8/odd_great_expectations/errors.py
--rw-r--r--   0        0        0     4622 2023-02-08 16:33:47.000000 odd_great_expectations-0.1.8/odd_great_expectations/mapper.py
--rw-r--r--   0        0        0      747 2023-02-08 16:34:11.000000 odd_great_expectations-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2513 1970-01-01 00:00:00.000000 odd_great_expectations-0.1.8/setup.py
--rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 odd_great_expectations-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1583 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/__init__.py
+-rw-r--r--   0        0        0     2675 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/action.py
+-rw-r--r--   0        0        0     2102 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/client.py
+-rw-r--r--   0        0        0       80 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/dataset/__init__.py
+-rw-r--r--   0        0        0      698 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/dataset/file.py
+-rw-r--r--   0        0        0      769 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/dataset/get_dataset.py
+-rw-r--r--   0        0        0     1726 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/dataset/sql_table.py
+-rw-r--r--   0        0        0      565 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/errors.py
+-rw-r--r--   0        0        0     4622 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/mapper.py
+-rw-r--r--   0        0        0      747 2023-02-08 21:09:37.000000 odd_great_expectations-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2513 1970-01-01 00:00:00.000000 odd_great_expectations-0.1.9/setup.py
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 odd_great_expectations-0.1.9/PKG-INFO
```

### Comparing `odd_great_expectations-0.1.8/LICENSE` & `odd_great_expectations-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `odd_great_expectations-0.1.8/README.md` & `odd_great_expectations-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `odd_great_expectations-0.1.8/odd_great_expectations/action.py` & `odd_great_expectations-0.1.9/odd_great_expectations/action.py`

 * *Files identical despite different names*

### Comparing `odd_great_expectations-0.1.8/odd_great_expectations/client.py` & `odd_great_expectations-0.1.9/odd_great_expectations/client.py`

 * *Files identical despite different names*

### Comparing `odd_great_expectations-0.1.8/odd_great_expectations/dataset/file.py` & `odd_great_expectations-0.1.9/odd_great_expectations/dataset/file.py`

 * *Files identical despite different names*

### Comparing `odd_great_expectations-0.1.8/odd_great_expectations/dataset/get_dataset.py` & `odd_great_expectations-0.1.9/odd_great_expectations/dataset/get_dataset.py`

 * *Files identical despite different names*

### Comparing `odd_great_expectations-0.1.8/odd_great_expectations/dataset/sql_table.py` & `odd_great_expectations-0.1.9/odd_great_expectations/dataset/sql_table.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,17 +16,18 @@
     }
 
     generator = PostgresqlGenerator(**generator_params)
     return generator.get_oddrn_by_path("tables")
 
 
 def snowflake_dataset(engine: Engine, batch_data: SqlAlchemyBatchData) -> str:
+    # Snowflake might create SqlAlchemy database name like <DATABASE_NAME>/<SCHEMA_NAME>
     generator_params = {
         "host_settings": engine.engine.url.host,
-        "databases": engine.engine.url.database,
+        "databases": engine.engine.url.database.split('/')[0],
         "schemas": batch_data.source_schema_name or "public",
         "tables": batch_data.source_table_name,
     }
 
     generator = SnowflakeGenerator(**generator_params)
     oddrn = generator.get_oddrn_by_path('tables')
     logger.info(f"{oddrn=}")
```

### Comparing `odd_great_expectations-0.1.8/odd_great_expectations/errors.py` & `odd_great_expectations-0.1.9/odd_great_expectations/errors.py`

 * *Files identical despite different names*

### Comparing `odd_great_expectations-0.1.8/odd_great_expectations/mapper.py` & `odd_great_expectations-0.1.9/odd_great_expectations/mapper.py`

 * *Files identical despite different names*

### Comparing `odd_great_expectations-0.1.8/pyproject.toml` & `odd_great_expectations-0.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odd-great-expectations"
-version = "0.1.8"
+version = "0.1.9"
 description = "OpenDataDiscovery Action for Great Expectations"
 authors = ["Pavel Makarichev <vixtir90@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ['Open Data Discovery', 'Great Expectations', "Metadata", "Data Discovery", "Data Observability"]
 packages = [{include = "odd_great_expectations"}]
```

### Comparing `odd_great_expectations-0.1.8/setup.py` & `odd_great_expectations-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'odd-models>=2.0.10,<3.0.0',
  'oddrn-generator==0.1.62',
  'psycopg2>=2.9.5,<3.0.0',
  'sqlalchemy>=1.4.46,<2.0.0']
 
 setup_kwargs = {
     'name': 'odd-great-expectations',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'OpenDataDiscovery Action for Great Expectations',
     'long_description': "## OpenDataDiscovery Great Expectations metadata collecting.\n[![PyPI version](https://badge.fury.io/py/odd-great-expectations.svg)](https://badge.fury.io/py/odd-great-expectations)\n\n## Supporting\n| Feature                     | Supporting |\n| --------------------------- | ---------- |\n| V3 API +                    | +          |\n| SqlAlchemyEngine            | +          |\n| PandasEngine                | +          |\n| Great Expectations V2 API - | -          |\n| Cloud Solution              | -          |\n\n\n`odd_great_expectation.action.ODDAction`\nIs a class derived from `ValidationAction` and can be used in checkpoint actions lists.\n\n## How to:\n\n### Install odd-great-expectations package\n```bash\npip install odd-great-expectations\n```\n\n### Add action to checkpoint:\n```yaml\nname: <CHECKPOINT_NAME>\nconfig_version: 1.0\ntemplate_name:\nmodule_name: great_expectations.checkpoint\nclass_name: Checkpoint\nrun_name_template: '%Y%m%d-%H%M%S-my-run-name-template'\nexpectation_suite_name:\nbatch_request: {}\naction_list:\n  # other actions\n  - name: store_metadata_to_odd \n    action:\n      module_name: odd_great_expectations.action\n      class_name: ODDAction\n      platform_host: <PLATFORM_HOST> # OpenDataDiscovery platform, i.e. http://localhost:8080\n      platform_token: <PLATFORM_TOKEN> # OpenDataDiscovery token\n      data_source_name: <DATA_SOURCE_NAME> # Unique name for data source, i.e. local_qa_test\nevaluation_parameters: {}\n```\n\n### Run checkpoint\n```bash\ngreat_expectations checkpoint run <CHECKPOINT_NAME> \n```\n### Check result\nCheck results on <PLATFORM_HOST> UI.\n\n\n",
     'author': 'Pavel Makarichev',
     'author_email': 'vixtir90@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `odd_great_expectations-0.1.8/PKG-INFO` & `odd_great_expectations-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odd-great-expectations
-Version: 0.1.8
+Version: 0.1.9
 Summary: OpenDataDiscovery Action for Great Expectations
 License: Apache-2.0
 Keywords: Open Data Discovery,Great Expectations,Metadata,Data Discovery,Data Observability
 Author: Pavel Makarichev
 Author-email: vixtir90@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

