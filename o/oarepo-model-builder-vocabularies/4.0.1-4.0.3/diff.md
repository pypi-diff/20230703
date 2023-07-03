# Comparing `tmp/oarepo-model-builder-vocabularies-4.0.1.tar.gz` & `tmp/oarepo-model-builder-vocabularies-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-vocabularies-4.0.1.tar", last modified: Mon May 29 11:44:26 2023, max compression
+gzip compressed data, was "oarepo-model-builder-vocabularies-4.0.3.tar", last modified: Mon Jul  3 13:14:18 2023, max compression
```

## Comparing `oarepo-model-builder-vocabularies-4.0.1.tar` & `oarepo-model-builder-vocabularies-4.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:44:26.151791 oarepo-model-builder-vocabularies-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-29 11:44:26.155791 oarepo-model-builder-vocabularies-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:44:26.151791 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:44:26.151791 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/builders/setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:44:26.151791 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/models/vocabulary.json
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/models/vocabulary.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:44:26.151791 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-29 11:44:26.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-29 11:44:26.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 11:44:26.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-29 11:44:26.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 11:42:01.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-29 11:44:26.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 11:44:26.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-29 11:44:26.155791 oarepo-model-builder-vocabularies-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:14:18.614374 oarepo-model-builder-vocabularies-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-03 13:14:18.614374 oarepo-model-builder-vocabularies-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:14:18.610374 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:14:18.614374 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/builders/setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:14:18.614374 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/models/vocabulary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/models/vocabulary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:14:18.614374 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-03 13:14:18.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-03 13:14:18.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:14:18.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-03 13:14:18.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:11:19.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-03 13:14:18.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-03 13:14:18.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-03 13:14:18.614374 oarepo-model-builder-vocabularies-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/setup.py
```

### Comparing `oarepo-model-builder-vocabularies-4.0.1/PKG-INFO` & `oarepo-model-builder-vocabularies-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-vocabularies
-Version: 4.0.1
+Version: 4.0.3
 Summary: "A model builder plugin to reference vocabularies"
 Home-page: https://github.com/oarepo/oarepo-model-builder-vocabularies
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio vocabulary model builder
 Platform: any
```

### Comparing `oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/components.py` & `oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/components.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/datatypes.py` & `oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/datatypes.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/models/vocabulary.json` & `oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/models/vocabulary.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998399872832247%*

 * *Differences: {"'model'": "{'properties': {'description': {'marshmallow': {'field-class': 'ma.fields.Nested'}}, "*

 * *            "'icon': {'marshmallow': {'field-class': 'ma.fields.String'}, 'ui': {'marshmallow': "*

 * *            "{'field-class': 'ma.fields.String'}}}, 'id': {'marshmallow': {'field-class': "*

 * *            "'ma.fields.String'}, 'ui': {'marshmallow': {'field-class': 'ma.fields.String'}}}, "*

 * *            "'props': {'marshmallow': {'field': 'ma.fields.Dict(allow_none=False, "*

 * *            "keys=fields.Str(), values=fi […]*

```diff
@@ -51,37 +51,37 @@
                     "invenio_cli_setup_cfg"
                 ]
             }
         },
         "properties": {
             "$schema": {
                 "marshmallow": {
-                    "field-class": "ma_fields.String",
+                    "field-class": "ma.fields.String",
                     "imports": [],
                     "read": false,
                     "validators": [],
                     "write": false
                 },
                 "sample": {
                     "skip": true
                 },
                 "type": "keyword",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String",
+                        "field-class": "ma.fields.String",
                         "imports": [],
                         "read": false,
                         "validators": [],
                         "write": false
                     }
                 }
             },
             "created": {
                 "marshmallow": {
-                    "field-class": "ma_fields.String",
+                    "field-class": "ma.fields.String",
                     "imports": [
                         {
                             "import": "datetime.datetime.strptime"
                         }
                     ],
                     "read": true,
                     "validators": [
@@ -91,15 +91,15 @@
                 },
                 "sample": {
                     "skip": true
                 },
                 "type": "date",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String",
+                        "field-class": "ma.fields.String",
                         "imports": [
                             {
                                 "import": "datetime.datetime.strptime"
                             }
                         ],
                         "read": true,
                         "validators": [
@@ -115,15 +115,15 @@
                 },
                 "mapping": {
                     "dynamic": true
                 },
                 "marshmallow": {
                     "class": "invenio_vocabularies.services.records.schema.DescriptionSchema",
                     "field": "i18n_strings",
-                    "field-class": "ma_fields.Nested",
+                    "field-class": "ma.fields.Nested",
                     "generate": false,
                     "imports": [
                         {
                             "import": "invenio_vocabularies.services.schema.i18n_strings"
                         }
                     ],
                     "read": false,
@@ -144,24 +144,24 @@
                             }
                         ]
                     }
                 }
             },
             "icon": {
                 "marshmallow": {
-                    "field-class": "ma_fields.String",
+                    "field-class": "ma.fields.String",
                     "imports": [],
                     "read": false,
                     "validators": [],
                     "write": false
                 },
                 "type": "keyword",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String",
+                        "field-class": "ma.fields.String",
                         "imports": [],
                         "read": false,
                         "validators": [],
                         "write": false
                     }
                 }
             },
@@ -170,120 +170,120 @@
                     "fields": {
                         "text": {
                             "type": "search_as_you_type"
                         }
                     }
                 },
                 "marshmallow": {
-                    "field-class": "ma_fields.String",
+                    "field-class": "ma.fields.String",
                     "imports": [],
                     "read": false,
                     "validators": [],
                     "write": false
                 },
                 "sample": {
                     "skip": true
                 },
                 "type": "keyword",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String",
+                        "field-class": "ma.fields.String",
                         "imports": [],
                         "read": false,
                         "validators": [],
                         "write": false
                     }
                 }
             },
             "pid": {
                 "marshmallow": {
                     "class": "invenio_vocabularies.services.records.schema.PidSchema",
-                    "field-class": "ma_fields.Nested",
+                    "field-class": "ma.fields.Nested",
                     "generate": false,
                     "imports": [],
                     "read": false,
                     "validators": [],
                     "write": false
                 },
                 "properties": {
                     "obj_type": {
                         "marshmallow": {
-                            "field-class": "ma_fields.String",
+                            "field-class": "ma.fields.String",
                             "imports": [],
                             "validators": []
                         },
                         "type": "keyword",
                         "ui": {
                             "marshmallow": {
-                                "field-class": "ma_fields.String",
+                                "field-class": "ma.fields.String",
                                 "imports": [],
                                 "validators": []
                             }
                         }
                     },
                     "pid_type": {
                         "marshmallow": {
-                            "field-class": "ma_fields.String",
+                            "field-class": "ma.fields.String",
                             "imports": [],
                             "validators": []
                         },
                         "type": "keyword",
                         "ui": {
                             "marshmallow": {
-                                "field-class": "ma_fields.String",
+                                "field-class": "ma.fields.String",
                                 "imports": [],
                                 "validators": []
                             }
                         }
                     },
                     "pk": {
                         "marshmallow": {
-                            "field-class": "ma_fields.Integer",
+                            "field-class": "ma.fields.Integer",
                             "imports": [],
                             "validators": []
                         },
                         "required": true,
                         "type": "integer",
                         "ui": {
                             "marshmallow": {
-                                "field-class": "ma_fields.Integer",
+                                "field-class": "ma.fields.Integer",
                                 "imports": [],
                                 "validators": []
                             }
                         }
                     },
                     "status": {
                         "enum": [
                             "N",
                             "K",
                             "R",
                             "M",
                             "D"
                         ],
                         "marshmallow": {
-                            "field-class": "ma_fields.String",
+                            "field-class": "ma.fields.String",
                             "imports": [],
                             "validators": []
                         },
                         "required": true,
                         "type": "keyword",
                         "ui": {
                             "marshmallow": {
-                                "field-class": "ma_fields.String",
+                                "field-class": "ma.fields.String",
                                 "imports": [],
                                 "validators": []
                             }
                         }
                     }
                 },
                 "type": "object",
                 "ui": {
                     "marshmallow": {
                         "class": "invenio_vocabularies.services.records.schema.PidSchema",
-                        "field-class": "ma_fields.Nested",
+                        "field-class": "ma.fields.Nested",
                         "generate": false,
                         "imports": [],
                         "read": false,
                         "validators": [],
                         "write": false
                     }
                 }
@@ -293,63 +293,63 @@
                     "type": "keyword"
                 },
                 "mapping": {
                     "dynamic:true": null
                 },
                 "marshmallow": {
                     "class": "invenio_vocabularies.services.records.schema.PropsSchema",
-                    "field": "ma_fields.Dict(allow_none=False, keys=fields.Str(), values=fields.Str())",
-                    "field-class": "ma_fields.Nested",
+                    "field": "ma.fields.Dict(allow_none=False, keys=fields.Str(), values=fields.Str())",
+                    "field-class": "ma.fields.Nested",
                     "generate": false,
                     "imports": [],
                     "read": false,
                     "validators": [],
                     "write": false
                 },
                 "type": "object",
                 "ui": {
                     "marshmallow": {
                         "class": "invenio_vocabularies.services.records.schema.PropsSchema",
-                        "field": "ma_fields.Dict(allow_none=False, keys=fields.Str(), values=fields.Str())",
-                        "field-class": "ma_fields.Nested",
+                        "field": "ma.fields.Dict(allow_none=False, keys=fields.Str(), values=fields.Str())",
+                        "field-class": "ma.fields.Nested",
                         "generate": false,
                         "imports": [],
                         "read": false,
                         "validators": [],
                         "write": false
                     }
                 }
             },
             "tags": {
                 "items": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String",
+                        "field-class": "ma.fields.String",
                         "imports": [],
                         "validators": []
                     },
                     "type": "keyword",
                     "ui": {
                         "marshmallow": {
-                            "field-class": "ma_fields.String",
+                            "field-class": "ma.fields.String",
                             "imports": [],
                             "validators": []
                         }
                     }
                 },
                 "marshmallow": {
-                    "field-class": "ma_fields.List",
+                    "field-class": "ma.fields.List",
                     "imports": [],
                     "read": false,
                     "validators": [],
                     "write": false
                 },
                 "type": "array",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.List",
+                        "field-class": "ma.fields.List",
                         "imports": [],
                         "read": false,
                         "validators": [],
                         "write": false
                     }
                 }
             },
@@ -365,15 +365,15 @@
                             "type": "search_as_you_type"
                         }
                     }
                 },
                 "marshmallow": {
                     "class": "invenio_vocabularies.services.records.schema.TitleSchema",
                     "field": "i18n_strings",
-                    "field-class": "ma_fields.Nested",
+                    "field-class": "ma.fields.Nested",
                     "generate": false,
                     "imports": [
                         {
                             "import": "invenio_vocabularies.services.schema.i18n_strings"
                         }
                     ],
                     "read": false,
@@ -397,89 +397,89 @@
                 }
             },
             "title_sort": {
                 "jsonschema": {
                     "generate": false
                 },
                 "marshmallow": {
-                    "field-class": "ma_fields.String",
+                    "field-class": "ma.fields.String",
                     "imports": [],
                     "read": false,
                     "validators": [],
                     "write": false
                 },
                 "type": "keyword",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String",
+                        "field-class": "ma.fields.String",
                         "imports": [],
                         "read": false,
                         "validators": [],
                         "write": false
                     }
                 }
             },
             "type": {
                 "marshmallow": {
                     "class": "invenio_vocabularies.services.records.schema.TypeSchema",
-                    "field-class": "ma_fields.Nested",
+                    "field-class": "ma.fields.Nested",
                     "generate": false,
                     "imports": [],
                     "read": false,
                     "validators": [],
                     "write": false
                 },
                 "properties": {
                     "id": {
                         "marshmallow": {
-                            "field-class": "ma_fields.String",
+                            "field-class": "ma.fields.String",
                             "imports": [],
                             "validators": []
                         },
                         "type": "keyword",
                         "ui": {
                             "marshmallow": {
-                                "field-class": "ma_fields.String",
+                                "field-class": "ma.fields.String",
                                 "imports": [],
                                 "validators": []
                             }
                         }
                     },
                     "pid_type": {
                         "marshmallow": {
-                            "field-class": "ma_fields.String",
+                            "field-class": "ma.fields.String",
                             "imports": [],
                             "validators": []
                         },
                         "type": "keyword",
                         "ui": {
                             "marshmallow": {
-                                "field-class": "ma_fields.String",
+                                "field-class": "ma.fields.String",
                                 "imports": [],
                                 "validators": []
                             }
                         }
                     }
                 },
                 "type": "object",
                 "ui": {
                     "marshmallow": {
                         "class": "invenio_vocabularies.services.records.schema.TypeSchema",
-                        "field-class": "ma_fields.Nested",
+                        "field-class": "ma.fields.Nested",
                         "generate": false,
                         "imports": [],
                         "read": false,
                         "validators": [],
                         "write": false
                     }
                 }
             },
             "updated": {
                 "marshmallow": {
-                    "field-class": "ma_fields.String",
+                    "field-class": "ma.fields.String",
                     "imports": [
                         {
                             "import": "datetime.datetime.strptime"
                         }
                     ],
                     "read": true,
                     "validators": [
@@ -489,15 +489,15 @@
                 },
                 "sample": {
                     "skip": true
                 },
                 "type": "date",
                 "ui": {
                     "marshmallow": {
-                        "field-class": "ma_fields.String",
+                        "field-class": "ma.fields.String",
                         "imports": [
                             {
                                 "import": "datetime.datetime.strptime"
                             }
                         ],
                         "read": true,
                         "validators": [
```

### Comparing `oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/models/vocabulary.yaml` & `oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/models/vocabulary.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
       obj_type: keyword
       ^marshmallow: {read: false, write: false}
     props:
       type: object
       mapping: {dynamic: true}
       additionalProperties:
         type: keyword
-      marshmallow: {read: false, write: false, field: "ma_fields.Dict(allow_none=False, keys=fields.Str(), values=fields.Str())"}
+      marshmallow: {read: false, write: false, field: "ma.fields.Dict(allow_none=False, keys=fields.Str(), values=fields.Str())"}
     tags[]: 
       type: keyword
       ^marshmallow: {read: false, write: false}
     title: 
       use: "#/$defs/i18nObjectString"
       mapping: {dynamic: true, properties: { en: {type: search_as_you_type, copy_to: title_sort}}}
       marshmallow: {read: false, write: false, field: "i18n_strings", imports: [{"import-path": "invenio_vocabularies.services.schema.i18n_strings"}]}
```

### Comparing `oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/PKG-INFO` & `oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-vocabularies
-Version: 4.0.1
+Version: 4.0.3
 Summary: "A model builder plugin to reference vocabularies"
 Home-page: https://github.com/oarepo/oarepo-model-builder-vocabularies
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio vocabulary model builder
 Platform: any
```

### Comparing `oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt` & `oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-4.0.1/setup.cfg` & `oarepo-model-builder-vocabularies-4.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-vocabularies
-version = 4.0.1
+version = 4.0.3
 description = "A model builder plugin to reference vocabularies"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio vocabulary model builder
 license = MIT
 author = Miroslav Simek
 author_email = simek.miroslav@techlib.cz
```

