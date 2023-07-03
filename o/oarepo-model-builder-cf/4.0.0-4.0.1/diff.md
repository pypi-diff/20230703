# Comparing `tmp/oarepo-model-builder-cf-4.0.0.tar.gz` & `tmp/oarepo-model-builder-cf-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-cf-4.0.0.tar", last modified: Sat May 20 15:31:12 2023, max compression
+gzip compressed data, was "oarepo-model-builder-cf-4.0.1.tar", last modified: Mon Jul  3 10:43:14 2023, max compression
```

## Comparing `oarepo-model-builder-cf-4.0.0.tar` & `oarepo-model-builder-cf-4.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:31:12.247445 oarepo-model-builder-cf-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 15:28:14.000000 oarepo-model-builder-cf-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-20 15:31:12.247445 oarepo-model-builder-cf-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-20 15:28:14.000000 oarepo-model-builder-cf-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:31:12.247445 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-20 15:28:14.000000 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-20 15:28:14.000000 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-20 15:28:14.000000 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:31:12.247445 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 15:28:14.000000 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-20 15:28:14.000000 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf/templates/record.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:31:12.247445 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-20 15:31:12.000000 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-20 15:31:12.000000 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 15:31:12.000000 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-20 15:31:12.000000 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 15:29:02.000000 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-20 15:31:12.000000 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-20 15:31:12.000000 oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-20 15:28:14.000000 oarepo-model-builder-cf-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-20 15:31:12.251445 oarepo-model-builder-cf-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-20 15:28:14.000000 oarepo-model-builder-cf-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:43:14.809239 oarepo-model-builder-cf-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 10:39:38.000000 oarepo-model-builder-cf-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-03 10:43:14.809239 oarepo-model-builder-cf-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-03 10:39:38.000000 oarepo-model-builder-cf-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:43:14.809239 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-03 10:39:38.000000 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-03 10:39:38.000000 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-03 10:39:38.000000 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:43:14.809239 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:39:38.000000 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-03 10:39:38.000000 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf/templates/record.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:43:14.809239 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-03 10:43:14.000000 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-03 10:43:14.000000 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:43:14.000000 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-03 10:43:14.000000 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:40:31.000000 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-03 10:43:14.000000 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 10:43:14.000000 oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 10:39:38.000000 oarepo-model-builder-cf-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-03 10:43:14.813239 oarepo-model-builder-cf-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-03 10:39:38.000000 oarepo-model-builder-cf-4.0.1/setup.py
```

### Comparing `oarepo-model-builder-cf-4.0.0/PKG-INFO` & `oarepo-model-builder-cf-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-cf
-Version: 4.0.0
+Version: 4.0.1
 Summary: "A model builder plugin for custom fields support"
 Home-page: https://github.com/oarepo/oarepo-model-builder-cf
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio cf model builder
 Platform: any
```

### Comparing `oarepo-model-builder-cf-4.0.0/README.md` & `oarepo-model-builder-cf-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf/components.py` & `oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf/components.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,37 +50,23 @@
             "service-config",
             "imports",
             {
                 "import": "invenio_records_resources.services.records.components.DataComponent"
             },
         )
 
-    def after_model_prepare(self, datatype, **kwargs):
+    def process_marshmallow(self, datatype, section=None, **kwargs):
+
         for cf in datatype.definition.get("custom-fields", []):
             element = cf.get("element", None)
             config = cf.get("config", None)
             if not element:
-                prepend_array(
-                    datatype,
-                    "marshmallow",
-                    "base-classes",
-                    "InlinedCustomFieldsSchemaMixin",
-                )
-                append_array(
-                    datatype,
-                    "marshmallow",
-                    "imports",
-                    {"import": "oarepo_runtime.cf.InlinedCustomFieldsSchemaMixin"},
-                )
-                append_array(
-                    datatype,
-                    "marshmallow",
-                    "extra-fields",
-                    {"name": "CUSTOM_FIELDS_VAR", "value": f'"{config}"'},
-                )
+                section.config["base-classes"] = [ "InlinedCustomFieldsSchemaMixin" ] + section.config["base-classes"]
+                section.config["imports"] += [ {"import": "oarepo_runtime.cf.InlinedCustomFieldsSchemaMixin"} ]
+                section.config.setdefault("extra-fields", []).append({"name": "CUSTOM_FIELDS_VAR", "value": f'"{config}"'})
 
 
 class CustomFieldsElementModelComponent(DataTypeComponent):
     eligible_datatypes = [ModelDataType]
     affects = [DefaultsModelComponent]
 
     def before_model_prepare(self, datatype, **kwargs):
@@ -99,14 +85,28 @@
                         "imports": [
                             {
                                 "import": "invenio_records_resources.services.custom_fields.CustomFieldsSchema"
                             },
                             {"import": "functools.partial"},
                             {"import": "marshmallow_utils.fields.NestedAttribute"},
                         ],
+                        "generate": False
+                    },
+                    "ui": {
+                        "marshmallow": {
+                            "field": f'NestedAttribute(partial(CustomFieldsSchema, fields_var="{config}"))',
+                            "imports": [
+                                {
+                                    "import": "invenio_records_resources.services.custom_fields.CustomFieldsSchema"
+                                },
+                                {"import": "functools.partial"},
+                                {"import": "marshmallow_utils.fields.NestedAttribute"},
+                            ],
+                            "generate": False
+                        }
                     },
                     "sample": {"skip": True},
                 }
             else:
                 # just make the schema and mapping extensible
                 set_default(datatype, "jsonschema", {}).setdefault(
                     "additionalProperties", True
```

### Comparing `oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf/templates/record.py.jinja2` & `oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf/templates/record.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf.egg-info/PKG-INFO` & `oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-cf
-Version: 4.0.0
+Version: 4.0.1
 Summary: "A model builder plugin for custom fields support"
 Home-page: https://github.com/oarepo/oarepo-model-builder-cf
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio cf model builder
 Platform: any
```

### Comparing `oarepo-model-builder-cf-4.0.0/oarepo_model_builder_cf.egg-info/SOURCES.txt` & `oarepo-model-builder-cf-4.0.1/oarepo_model_builder_cf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-cf-4.0.0/setup.cfg` & `oarepo-model-builder-cf-4.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-cf
-version = 4.0.0
+version = 4.0.1
 description = "A model builder plugin for custom fields support"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio cf model builder
 license = MIT
 author = Miroslav Simek
 author_email = simek.miroslav@techlib.cz
```

