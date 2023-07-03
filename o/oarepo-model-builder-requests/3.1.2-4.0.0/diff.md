# Comparing `tmp/oarepo-model-builder-requests-3.1.2.tar.gz` & `tmp/oarepo-model-builder-requests-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-requests-3.1.2.tar", last modified: Thu Apr 20 14:34:14 2023, max compression
+gzip compressed data, was "oarepo-model-builder-requests-4.0.0.tar", last modified: Mon Jul  3 15:19:33 2023, max compression
```

## Comparing `oarepo-model-builder-requests-3.1.2.tar` & `oarepo-model-builder-requests-4.0.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.950141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/invenio_requests_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/invenio_requests_actions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/invenio_requests_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/invenio_requests_resolvers.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/invenio_requests_types.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/invenio_requests_views.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/model_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/model_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/model_preprocessors/invenio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/invenio_requests_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/invenio_requests_test_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.950141 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-20 14:34:14.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-20 14:34:14.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:34:14.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-20 14:34:14.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 14:34:14.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 14:34:14.000000 oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-20 14:34:14.958141 oarepo-model-builder-requests-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:34:14.954141 oarepo-model-builder-requests-3.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-20 14:29:09.000000 oarepo-model-builder-requests-3.1.2/tests/test_custom_action.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.308831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.308831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.308831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/datatypes/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.308831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/datatypes/components/requests_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/datatypes/components/requests_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/datatypes/components/requests_model/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/invenio_requests_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/invenio_requests_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/invenio_requests_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/invenio_requests_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/invenio_requests_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/invenio_requests_actions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/invenio_requests_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/invenio_requests_resolvers.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/invenio_requests_types.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/invenio_requests_views.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/invenio_requests_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/invenio_requests_test_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.308831 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-03 15:19:33.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-03 15:19:33.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:19:33.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-03 15:19:33.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 15:19:33.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 15:19:33.000000 oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:19:33.312831 oarepo-model-builder-requests-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-03 15:16:05.000000 oarepo-model-builder-requests-4.0.0/tests/test_custom_action.py
```

### Comparing `oarepo-model-builder-requests-3.1.2/LICENSE` & `oarepo-model-builder-requests-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-3.1.2/PKG-INFO` & `oarepo-model-builder-requests-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-requests
-Version: 3.1.2
+Version: 4.0.0
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo model builder requests
 Plugin for oarepo-model-builder to allow specifying requests 
 tied to the base model, based on invenio requests. <br>
```

### Comparing `oarepo-model-builder-requests-3.1.2/README.md` & `oarepo-model-builder-requests-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/invenio/templates/invenio_requests_types.py.jinja2` & `oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/invenio/templates/invenio_requests_types.py.jinja2`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-{% for request_data in requests.values() %}
-{% if request_data.type_generate %}
-from {{ request_data.approve_action_class|package_name }} import {{ request_data.approve_action_class|base_name }}
-    {% for type_base in request_data.type_bases %}
-from {{ type_base|package_name }} import {{ type_base|base_name }}
-    {% endfor %}
+{% for request_data in vars.requests.values() %}
+    {% if request_data.type.generate %}
+{{ request_data.actions['approve'].class|generate_import }}
+{{ request_data.type.imports|generate_import }}
 {% endif %}
 {% endfor %}
 
-{% for request, request_data in requests.items() %}
-{% if request_data.type_generate %}
-class {{ request_data.type_class|base_name }}{% if request_data.type_bases %}({% for type_base in request_data.type_bases%}{{ type_base|base_name }}{{ ", " if not loop.last else "" }}{% endfor %}){% endif %}:
+{% for request_name, request_data in vars.requests.items() %}
+{% if request_data.type.generate %}
+class {{ request_data.type|class_header }}:
 
-    type_id = "{{ request }}"
-    name = "{{ request.capitalize() }}"
+    type_id = "{{ request_name }}"
+    name = "{{ request_name.capitalize() }}"
 
     available_actions = {
         **RequestType.available_actions,
-        "accept": {{ request_data.approve_action_class|base_name }}
+        "accept": {{ request_data.actions['approve'].class|base_name }}
     }
 
-    allowed_topic_ref_types = ["{{ current_model.model_name }}"] # On the Request record object, the topic is referenced by pid. This pid is
+    allowed_topic_ref_types = ["{{ vars.module.prefix_snake }}"] # On the Request record object, the topic is referenced by pid. This pid is
                                          # extracted by Resolver subclassed from RecordResolver, which has hardcoded
                                          # {"record": {pid}} as reference value. This reference is then by
                                          # setattr set on the Request record topic ReferencedEntityField, and the set
                                          # operation checks, whether this key is in allowed_topic_ref_types
     #TODO would it make sense to customize the topic ref types?
 {% endif %}
 {% endfor %}
```

### Comparing `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2` & `oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from flask_security.utils import hash_password
 from invenio_app.factory import create_api
 from invenio_records_resources.services.uow import UnitOfWork, RecordCommitOp
 from invenio_requests.customizations import CommentEventType, LogEventType
-from {{ current_model.record_class|package_name }} import {{ current_model.record_class|base_name }}
 from flask_principal import Identity, Need, UserNeed
-from {{ current_model.proxies_current_service|package_name }} import {{ current_model.proxies_current_service|base_name }}
 import pytest
 from invenio_requests.proxies import current_requests
 from invenio_requests.records.api import RequestEventFormat
 from invenio_access.models import ActionRoles
 from invenio_access.permissions import superuser_access
 from invenio_accounts.models import Role
 
+{{ vars.record|generate_import }}
+from {{ vars.proxy.module }} import {{ vars.service.proxy }}
 
 @pytest.fixture(scope="module")
 def app_config(app_config):
 
     app_config["REQUESTS_REGISTERED_EVENT_TYPES"] = [LogEventType(), CommentEventType()]
     return app_config
 
@@ -118,14 +118,14 @@
     ret = {"title": "Doc1 approval", "payload": {
         "content": "Can you approve my document doc1 please?",
         "format": RequestEventFormat.HTML.value,
     }}
     return ret
 
 @pytest.fixture(scope="function")
-def example_{{ current_model.record_prefix_snake }}(app, db, sample_metadata_list):
+def example_topic(app, db, sample_metadata_list):
     # return record
     with UnitOfWork(db.session) as uow:
-        record = {{ current_model.record_class|base_name }}.create(sample_metadata_list[0])
-        uow.register(RecordCommitOp(record, {{ current_model.proxies_current_service|base_name }}.indexer, True))
+        record = {{ vars.record.class|base_name }}.create(sample_metadata_list[0])
+        uow.register(RecordCommitOp(record, {{ vars.service.proxy }}.indexer, True))
         uow.commit()
         return record
```

### Comparing `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2` & `oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2`

 * *Files 20% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 def test_custom_type_request(
     app,
     identity_simple,
     identity_simple_2,
     submit_request,
     request_events_service,
     requests_service,
-    example_{{ current_model.record_prefix_snake }},
+    example_topic,
     users,
     request_record_input_data,
 ):
     receiver_user = users[1]
     sender_identity = identity_simple
     receiver_identity = identity_simple_2
     request_types = app.extensions["invenio-requests"].request_type_registry
     for request_type in request_types:
-        if request_type.__module__ != "{{ current_model.requests_types }}":
+        if request_type.__module__ != "{{ vars.requests_modules.types_module }}": #not a generated request
             continue
         request = submit_request(
             sender_identity,
             data=request_record_input_data,
-            topic=example_{{ current_model.record_prefix_snake }},
+            topic=example_topic,
             request_type=request_type,
             receiver=receiver_user,
         )
-        # assert current_service.read(sender_identity, example_{{ current_model.record_prefix_snake }}["id"])["metadata"][
+        # assert current_service.read(sender_identity, example_topic["id"])["metadata"][
         #           "status"] == "not approved"
         request_id = request.id
 
     # approve request by receiver
         payload = {
             "payload": {
                 "content": "Ok doc1 is good enough and therefore approved.",
@@ -42,15 +42,15 @@
         # the sender can't approve the request
         with pytest.raises(PermissionDeniedError):
             requests_service.execute_action(sender_identity, request_id, "accept", payload)
         # the reciever can
         approve_response = requests_service.execute_action(
             receiver_identity, request_id, "accept", payload
         )
-        # assert current_service.read(sender_identity, example_{{ current_model.record_prefix_snake }}["id"])["metadata"][
+        # assert current_service.read(sender_identity, example_topic["id"])["metadata"][
         #           "status"] == "approved"
         request = approve_response._request
         RequestEvent.index.refresh()
 
         assert "accepted" == request.status
         events = request_events_service.search(sender_identity, request_id)
         assert 3 == events.total  # two comments and accept log
```

### Comparing `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/PKG-INFO` & `oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-requests
-Version: 3.1.2
+Version: 4.0.0
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo model builder requests
 Plugin for oarepo-model-builder to allow specifying requests 
 tied to the base model, based on invenio requests. <br>
```

### Comparing `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/SOURCES.txt` & `oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,29 +7,28 @@
 oarepo_model_builder_requests/__init__.py
 oarepo_model_builder_requests.egg-info/PKG-INFO
 oarepo_model_builder_requests.egg-info/SOURCES.txt
 oarepo_model_builder_requests.egg-info/dependency_links.txt
 oarepo_model_builder_requests.egg-info/entry_points.txt
 oarepo_model_builder_requests.egg-info/requires.txt
 oarepo_model_builder_requests.egg-info/top_level.txt
+oarepo_model_builder_requests/datatypes/__init__.py
+oarepo_model_builder_requests/datatypes/components/__init__.py
+oarepo_model_builder_requests/datatypes/components/requests_model/__init__.py
+oarepo_model_builder_requests/datatypes/components/requests_model/requests.py
 oarepo_model_builder_requests/invenio/__init__.py
 oarepo_model_builder_requests/invenio/invenio_requests_actions.py
-oarepo_model_builder_requests/invenio/invenio_requests_builder.py
 oarepo_model_builder_requests/invenio/invenio_requests_config.py
 oarepo_model_builder_requests/invenio/invenio_requests_resolvers.py
-oarepo_model_builder_requests/invenio/invenio_requests_setup_cfg.py
 oarepo_model_builder_requests/invenio/invenio_requests_types.py
 oarepo_model_builder_requests/invenio/invenio_requests_views.py
 oarepo_model_builder_requests/invenio/templates/invenio_requests_actions.py.jinja2
 oarepo_model_builder_requests/invenio/templates/invenio_requests_config.py.jinja2
 oarepo_model_builder_requests/invenio/templates/invenio_requests_resolvers.py.jinja2
 oarepo_model_builder_requests/invenio/templates/invenio_requests_types.py.jinja2
 oarepo_model_builder_requests/invenio/templates/invenio_requests_views.py.jinja2
-oarepo_model_builder_requests/model_preprocessors/__init__.py
-oarepo_model_builder_requests/model_preprocessors/invenio.py
 oarepo_model_builder_requests/tests/__init__.py
 oarepo_model_builder_requests/tests/invenio_requests_conftest.py
 oarepo_model_builder_requests/tests/invenio_requests_test_requests.py
 oarepo_model_builder_requests/tests/templates/conftest.py.jinja2
 oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2
-oarepo_model_builder_requests/validation/__init__.py
 tests/test_custom_action.py
```

### Comparing `oarepo-model-builder-requests-3.1.2/oarepo_model_builder_requests.egg-info/entry_points.txt` & `oarepo-model-builder-requests-4.0.0/oarepo_model_builder_requests.egg-info/entry_points.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-[oarepo_model_builder.builders.model]
+[oarepo_model_builder.builders.record]
 2210-invenio_requests_actions = oarepo_model_builder_requests.invenio.invenio_requests_actions:InvenioRequestsActionsBuilder
 2211-invenio_requests_resolvers = oarepo_model_builder_requests.invenio.invenio_requests_resolvers:InvenioRequestsResolversBuilder
 2212-invenio_requests_types = oarepo_model_builder_requests.invenio.invenio_requests_types:InvenioRequestsTypesBuilder
-2213-invenio_requests_setup_cfg = oarepo_model_builder_requests.invenio.invenio_requests_setup_cfg:InvenioRequestsSetupCfgBuilder
 2214-invenio_requests_views = oarepo_model_builder_requests.invenio.invenio_requests_views:InvenioRequestsViewsBuilder
 2215-invenio_requests_config = oarepo_model_builder_requests.invenio.invenio_requests_config:InvenioRequestsConfigBuilder
 2216-invenio_requests_conftest = oarepo_model_builder_requests.tests.invenio_requests_conftest:InvenioRequestsConftestBuilder
 2219-invenio_requests_test_requests = oarepo_model_builder_requests.tests.invenio_requests_test_requests:InvenioRequestsTestRequestsBuilder
 
-[oarepo_model_builder.model_preprocessors.model]
-30-invenio_requests = oarepo_model_builder_requests.model_preprocessors.invenio:InvenioModelPreprocessor
+[oarepo_model_builder.datatypes.components]
+invenio_requests = oarepo_model_builder_requests.datatypes.components:requests_components
 
 [oarepo_model_builder.templates]
 98-requests_templates = oarepo_model_builder_requests.invenio
 99-requests_tests_templates = oarepo_model_builder_requests.tests
-
-[oarepo_model_builder.validation]
-requests-validation = oarepo_model_builder_requests.validation:validators
```

### Comparing `oarepo-model-builder-requests-3.1.2/setup.cfg` & `oarepo-model-builder-requests-4.0.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 [metadata]
 name = oarepo-model-builder-requests
-version = 3.1.2
+version = 4.0.0
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
 python = >=3.9
 install_requires = 
-	oarepo-model-builder-tests>=3.1.0
+	oarepo-model-builder
+	oarepo-model-builder-tests
 
 [options.package_data]
 * = *.json, *.rst, *.md, *.json5, *.jinja2
 
 [options.packages.find]
 exclude = example_model
 
 [options.entry_points]
-oarepo_model_builder.validation = 
-	requests-validation = oarepo_model_builder_requests.validation:validators
-oarepo_model_builder.builders.model = 
+oarepo_model_builder.datatypes.components = 
+	invenio_requests = oarepo_model_builder_requests.datatypes.components:requests_components
+oarepo_model_builder.builders.record = 
 	2210-invenio_requests_actions  = oarepo_model_builder_requests.invenio.invenio_requests_actions:InvenioRequestsActionsBuilder
 	2211-invenio_requests_resolvers  = oarepo_model_builder_requests.invenio.invenio_requests_resolvers:InvenioRequestsResolversBuilder
 	2212-invenio_requests_types  = oarepo_model_builder_requests.invenio.invenio_requests_types:InvenioRequestsTypesBuilder
-	2213-invenio_requests_setup_cfg = oarepo_model_builder_requests.invenio.invenio_requests_setup_cfg:InvenioRequestsSetupCfgBuilder
 	2214-invenio_requests_views = oarepo_model_builder_requests.invenio.invenio_requests_views:InvenioRequestsViewsBuilder
 	2215-invenio_requests_config = oarepo_model_builder_requests.invenio.invenio_requests_config:InvenioRequestsConfigBuilder
 	2216-invenio_requests_conftest = oarepo_model_builder_requests.tests.invenio_requests_conftest:InvenioRequestsConftestBuilder
 	2219-invenio_requests_test_requests = oarepo_model_builder_requests.tests.invenio_requests_test_requests:InvenioRequestsTestRequestsBuilder
 oarepo_model_builder.templates = 
 	98-requests_templates  = oarepo_model_builder_requests.invenio
 	99-requests_tests_templates = oarepo_model_builder_requests.tests
-oarepo_model_builder.model_preprocessors.model = 
-	30-invenio_requests  = oarepo_model_builder_requests.model_preprocessors.invenio:InvenioModelPreprocessor
 
 [options.extras_require]
 tests = 
 	pytest-invenio>=1.4.11
 
 [egg_info]
 tag_build =
```

### Comparing `oarepo-model-builder-requests-3.1.2/tests/test_custom_action.py` & `oarepo-model-builder-requests-4.0.0/tests/test_custom_action.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 from invenio_requests.records.api import RequestEventFormat
-
-from example_document.proxies import current_service
-from example_document.requests.types import CustomApproveActionRequestType
 from test_custom_classes.request_test_actions import ActuallyApproveRecordAction
+from thesis.proxies import current_service
+from thesis.records.requests.types import CustomApproveActionRequestType
+
 
 def test_action_changes_topic_status(
     app,
     identity_simple,
     identity_simple_2,
     submit_request,
     request_events_service,
     requests_service,
-    example_example_document,
+    example_topic,
     users,
     request_record_input_data,
 ):
     receiver_user = users[1]
     sender_identity = identity_simple
     receiver_identity = identity_simple_2
     request_types = app.extensions["invenio-requests"].request_type_registry
     for request_type in request_types:
         if not request_type == CustomApproveActionRequestType:
             continue
         assert request_type.available_actions["accept"] == ActuallyApproveRecordAction
         request = submit_request(
             sender_identity,
             data=request_record_input_data,
-            topic=example_example_document,
+            topic=example_topic,
             request_type=request_type,
             receiver=receiver_user,
         )
-        # assert current_service.read(identity_simple, example_example_document["id"])["metadata"][
-        #           "status"] == "not approved"
+
         request_id = request.id
 
         # approve request by receiver
         payload = {
             "payload": {
                 "content": "Ok doc1 is good enough and therefore approved.",
                 "format": RequestEventFormat.HTML.value,
             }
         }
         # the reciever can
         requests_service.execute_action(
             receiver_identity, request_id, "accept", payload
         )
-        assert current_service.read(sender_identity, example_example_document["id"])["metadata"][
-                  "status"] == "approved" # this part checks whether the topic status was approved
+        assert (
+            current_service.read(sender_identity, example_topic["id"])["metadata"][
+                "status"
+            ]
+            == "approved"
+        )  # this part checks whether the topic status was approved
```

