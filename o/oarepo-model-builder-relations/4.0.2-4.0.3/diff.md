# Comparing `tmp/oarepo-model-builder-relations-4.0.2.tar.gz` & `tmp/oarepo-model-builder-relations-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-relations-4.0.2.tar", last modified: Mon May 22 19:53:25 2023, max compression
+gzip compressed data, was "oarepo-model-builder-relations-4.0.3.tar", last modified: Mon Jul  3 11:26:33 2023, max compression
```

## Comparing `oarepo-model-builder-relations-4.0.2.tar` & `oarepo-model-builder-relations-4.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:25.827743 oarepo-model-builder-relations-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 19:48:21.000000 oarepo-model-builder-relations-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-22 19:53:25.827743 oarepo-model-builder-relations-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-22 19:48:21.000000 oarepo-model-builder-relations-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:25.823743 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-22 19:48:21.000000 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-22 19:48:21.000000 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-05-22 19:48:21.000000 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-22 19:48:21.000000 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:25.823743 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:48:21.000000 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-22 19:48:21.000000 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations/templates/record.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:25.823743 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-22 19:53:25.000000 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-22 19:53:25.000000 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:53:25.000000 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-22 19:53:25.000000 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:49:20.000000 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-22 19:53:25.000000 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 19:53:25.000000 oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 19:48:21.000000 oarepo-model-builder-relations-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-22 19:53:25.827743 oarepo-model-builder-relations-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-22 19:48:21.000000 oarepo-model-builder-relations-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:26:33.255978 oarepo-model-builder-relations-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 11:21:24.000000 oarepo-model-builder-relations-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-03 11:26:33.255978 oarepo-model-builder-relations-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-03 11:21:24.000000 oarepo-model-builder-relations-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:26:33.251978 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-03 11:21:24.000000 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-03 11:21:24.000000 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-03 11:21:24.000000 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-03 11:21:24.000000 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:26:33.255978 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:21:24.000000 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 11:21:24.000000 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations/templates/record.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:26:33.255978 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-03 11:26:33.000000 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-03 11:26:33.000000 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:26:33.000000 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-03 11:26:33.000000 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:22:21.000000 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-03 11:26:33.000000 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-03 11:26:33.000000 oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 11:21:24.000000 oarepo-model-builder-relations-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-03 11:26:33.255978 oarepo-model-builder-relations-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-03 11:21:24.000000 oarepo-model-builder-relations-4.0.3/setup.py
```

### Comparing `oarepo-model-builder-relations-4.0.2/PKG-INFO` & `oarepo-model-builder-relations-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-relations
-Version: 4.0.2
+Version: 4.0.3
 Summary: "A model builder plugin to reference relations"
 Home-page: https://github.com/oarepo/oarepo-model-builder-relations
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio relations model builder
 Platform: any
```

### Comparing `oarepo-model-builder-relations-4.0.2/README.md` & `oarepo-model-builder-relations-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations/builders.py` & `oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations/builders.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations/components.py` & `oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,20 +106,20 @@
 
         children["@v"] = datatypes.get_datatype(
             datatype,
             {
                 "type": "keyword",
                 "marshmallow": {
                     "field-name": "_version",
-                    "field-class": "ma_fields.String",
+                    "field-class": "ma.fields.String",
                 },
                 "ui": {
                     "marshmallow": {
                         "field-name": "_version",
-                        "field-class": "ma_fields.String",
+                        "field-class": "ma.fields.String",
                     }
                 },
             },
             "@v",
             datatype.model,
             datatype.schema,
         )
```

### Comparing `oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations/datatypes.py` & `oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations/datatypes.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations.egg-info/PKG-INFO` & `oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-relations
-Version: 4.0.2
+Version: 4.0.3
 Summary: "A model builder plugin to reference relations"
 Home-page: https://github.com/oarepo/oarepo-model-builder-relations
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio relations model builder
 Platform: any
```

### Comparing `oarepo-model-builder-relations-4.0.2/oarepo_model_builder_relations.egg-info/SOURCES.txt` & `oarepo-model-builder-relations-4.0.3/oarepo_model_builder_relations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-relations-4.0.2/setup.cfg` & `oarepo-model-builder-relations-4.0.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-relations
-version = 4.0.2
+version = 4.0.3
 description = "A model builder plugin to reference relations"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio relations model builder
 license = MIT
 author = Miroslav Simek
 author_email = simek.miroslav@techlib.cz
```

