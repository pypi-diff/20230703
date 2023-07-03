# Comparing `tmp/encord-0.1.83.tar.gz` & `tmp/encord-0.1.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.83.tar", max compression
+gzip compressed data, was "encord-0.1.84.tar", max compression
```

## Comparing `encord-0.1.83.tar` & `encord-0.1.84.tar`

### file list

```diff
@@ -1,76 +1,90 @@
--rw-r--r--   0        0        0    11330 2023-06-20 14:01:34.440626 encord-0.1.83/LICENSE
--rw-r--r--   0        0        0     2037 2023-06-20 14:01:34.440626 encord-0.1.83/README.md
--rw-r--r--   0        0        0       84 2023-06-20 14:01:34.440626 encord-0.1.83/cord/__init__.py
--rw-r--r--   0        0        0      158 2023-06-20 14:01:34.456626 encord-0.1.83/encord/__init__.py
--rw-r--r--   0        0        0      214 2023-06-20 14:01:34.456626 encord-0.1.83/encord/_version.py
--rw-r--r--   0        0        0    49810 2023-06-20 14:01:34.456626 encord-0.1.83/encord/client.py
--rw-r--r--   0        0        0    10852 2023-06-20 14:01:34.456626 encord-0.1.83/encord/configs.py
--rw-r--r--   0        0        0        0 2023-06-20 14:01:34.456626 encord-0.1.83/encord/constants/__init__.py
--rw-r--r--   0        0        0      866 2023-06-20 14:01:34.456626 encord-0.1.83/encord/constants/enums.py
--rw-r--r--   0        0        0     3293 2023-06-20 14:01:34.456626 encord-0.1.83/encord/constants/model.py
--rw-r--r--   0        0        0     6068 2023-06-20 14:01:34.456626 encord-0.1.83/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-06-20 14:01:34.456626 encord-0.1.83/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-06-20 14:01:34.456626 encord-0.1.83/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-06-20 14:01:34.456626 encord-0.1.83/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-06-20 14:01:34.456626 encord-0.1.83/encord/dataset.py
--rw-r--r--   0        0        0     6346 2023-06-20 14:01:34.456626 encord-0.1.83/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-20 14:01:34.456626 encord-0.1.83/encord/http/__init__.py
--rw-r--r--   0        0        0     5315 2023-06-20 14:01:34.456626 encord-0.1.83/encord/http/bundle.py
--rw-r--r--   0        0        0      535 2023-06-20 14:01:34.456626 encord-0.1.83/encord/http/constants.py
--rw-r--r--   0        0        0     7234 2023-06-20 14:01:34.460626 encord-0.1.83/encord/http/error_utils.py
--rw-r--r--   0        0        0      103 2023-06-20 14:01:34.460626 encord-0.1.83/encord/http/limits.py
--rw-r--r--   0        0        0     7928 2023-06-20 14:01:34.460626 encord-0.1.83/encord/http/querier.py
--rw-r--r--   0        0        0      697 2023-06-20 14:01:34.460626 encord-0.1.83/encord/http/query_methods.py
--rw-r--r--   0        0        0     1719 2023-06-20 14:01:34.460626 encord-0.1.83/encord/http/request.py
--rw-r--r--   0        0        0     6182 2023-06-20 14:01:34.460626 encord-0.1.83/encord/http/utils.py
--rw-r--r--   0        0        0      340 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/__init__.py
--rw-r--r--   0        0        0     5164 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/bitmask.py
--rw-r--r--   0        0        0      182 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/classification.py
--rw-r--r--   0        0        0    31614 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/common.py
--rw-r--r--   0        0        0      151 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/constants.py
--rw-r--r--   0        0        0     5748 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3461 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/frames.py
--rw-r--r--   0        0        0    21557 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   143304 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      174 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      185 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/project.py
--rw-r--r--   0        0        0     1289 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-06-20 14:01:34.460626 encord-0.1.83/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/__init__.py
--rw-r--r--   0        0        0      982 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/api_key.py
--rw-r--r--   0        0        0     5335 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32844 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/dataset.py
--rw-r--r--   0        0        0      828 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      175 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/formatter.py
--rw-r--r--   0        0        0     1146 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/label_log.py
--rw-r--r--   0        0        0    11889 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6687 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/model.py
--rw-r--r--   0        0        0      823 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/ontology.py
--rw-r--r--   0        0        0     8966 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0      314 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/workflow.py
--rw-r--r--   0        0        0    39504 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project.py
--rw-r--r--   0        0        0        0 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9676 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    29047 2023-06-20 14:01:34.460626 encord-0.1.83/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-06-20 14:01:34.460626 encord-0.1.83/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4282 2023-06-20 14:01:34.460626 encord-0.1.83/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-06-20 14:01:34.460626 encord-0.1.83/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-06-20 14:01:34.460626 encord-0.1.83/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-06-20 14:01:34.460626 encord-0.1.83/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-06-20 14:01:34.460626 encord-0.1.83/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-06-20 14:01:34.460626 encord-0.1.83/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1945 2023-06-20 14:01:34.460626 encord-0.1.83/pyproject.toml
--rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 encord-0.1.83/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-07-03 15:48:01.847013 encord-0.1.84/LICENSE
+-rw-r--r--   0        0        0     2037 2023-07-03 15:48:01.847013 encord-0.1.84/README.md
+-rw-r--r--   0        0        0       84 2023-07-03 15:48:01.847013 encord-0.1.84/cord/__init__.py
+-rw-r--r--   0        0        0      158 2023-07-03 15:48:01.867013 encord-0.1.84/encord/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-03 15:48:01.867013 encord-0.1.84/encord/_version.py
+-rw-r--r--   0        0        0    49540 2023-07-03 15:48:01.867013 encord-0.1.84/encord/client.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:48:01.867013 encord-0.1.84/encord/common/__init__.py
+-rw-r--r--   0        0        0       45 2023-07-03 15:48:01.867013 encord-0.1.84/encord/common/constants.py
+-rw-r--r--   0        0        0      464 2023-07-03 15:48:01.867013 encord-0.1.84/encord/common/enum.py
+-rw-r--r--   0        0        0    10852 2023-07-03 15:48:01.867013 encord-0.1.84/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:48:01.867013 encord-0.1.84/encord/constants/__init__.py
+-rw-r--r--   0        0        0      866 2023-07-03 15:48:01.867013 encord-0.1.84/encord/constants/enums.py
+-rw-r--r--   0        0        0     3196 2023-07-03 15:48:01.867013 encord-0.1.84/encord/constants/model.py
+-rw-r--r--   0        0        0     4522 2023-07-03 15:48:01.867013 encord-0.1.84/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-07-03 15:48:01.867013 encord-0.1.84/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:48:01.867013 encord-0.1.84/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-07-03 15:48:01.867013 encord-0.1.84/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16035 2023-07-03 15:48:01.867013 encord-0.1.84/encord/dataset.py
+-rw-r--r--   0        0        0     6355 2023-07-03 15:48:01.867013 encord-0.1.84/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/__init__.py
+-rw-r--r--   0        0        0     5315 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/bundle.py
+-rw-r--r--   0        0        0      319 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/common.py
+-rw-r--r--   0        0        0      535 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/constants.py
+-rw-r--r--   0        0        0     7234 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/error_utils.py
+-rw-r--r--   0        0        0      103 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/limits.py
+-rw-r--r--   0        0        0     7870 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/querier.py
+-rw-r--r--   0        0        0      747 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1738 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/request.py
+-rw-r--r--   0        0        0     6182 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/utils.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/v2/__init__.py
+-rw-r--r--   0        0        0     3447 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/v2/api_client.py
+-rw-r--r--   0        0        0      964 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/v2/error_utils.py
+-rw-r--r--   0        0        0      216 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/v2/payloads.py
+-rw-r--r--   0        0        0     2249 2023-07-03 15:48:01.867013 encord-0.1.84/encord/http/v2/request_signer.py
+-rw-r--r--   0        0        0      340 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/__init__.py
+-rw-r--r--   0        0        0     5164 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/bitmask.py
+-rw-r--r--   0        0        0      182 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/classification.py
+-rw-r--r--   0        0        0    31763 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/common.py
+-rw-r--r--   0        0        0      151 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/constants.py
+-rw-r--r--   0        0        0     5748 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3461 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/frames.py
+-rw-r--r--   0        0        0    21521 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   144757 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      174 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      185 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/project.py
+-rw-r--r--   0        0        0     1504 2023-07-03 15:48:01.867013 encord-0.1.84/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-07-03 15:48:01.867013 encord-0.1.84/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/analytics.py
+-rw-r--r--   0        0        0      982 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/api_key.py
+-rw-r--r--   0        0        0      626 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/base_dto/__init__.py
+-rw-r--r--   0        0        0      337 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/base_dto/base_dto_interface.py
+-rw-r--r--   0        0        0     1418 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/base_dto/base_dto_pydantic_v1.py
+-rw-r--r--   0        0        0     1366 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/base_dto/base_dto_pydantic_v2.py
+-rw-r--r--   0        0        0     5335 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32857 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/dataset.py
+-rw-r--r--   0        0        0      829 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      256 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1146 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11889 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6679 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/model.py
+-rw-r--r--   0        0        0      874 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8658 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0      314 2023-07-03 15:48:01.871013 encord-0.1.84/encord/orm/workflow.py
+-rw-r--r--   0        0        0    41298 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9676 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-07-03 15:48:01.871013 encord-0.1.84/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    29244 2023-07-03 15:48:01.871013 encord-0.1.84/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:48:01.871013 encord-0.1.84/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4282 2023-07-03 15:48:01.871013 encord-0.1.84/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-07-03 15:48:01.871013 encord-0.1.84/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-07-03 15:48:01.871013 encord-0.1.84/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-07-03 15:48:01.871013 encord-0.1.84/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-07-03 15:48:01.871013 encord-0.1.84/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-07-03 15:48:01.871013 encord-0.1.84/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1966 2023-07-03 15:48:01.871013 encord-0.1.84/pyproject.toml
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 encord-0.1.84/PKG-INFO
```

### Comparing `encord-0.1.83/LICENSE` & `encord-0.1.84/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/README.md` & `encord-0.1.84/README.md`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/client.py` & `encord-0.1.84/encord/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,23 +40,24 @@
 import os.path
 import time
 import typing
 import uuid
 from datetime import datetime
 from math import ceil
 from pathlib import Path
-from typing import Iterable, List, Optional, Tuple, Union
+from typing import Iterable, List, Optional, Tuple, Union, cast
 
 import requests
 
 import encord.exceptions
 from encord.configs import ENCORD_DOMAIN, ApiKeyConfig, Config, EncordConfig
 from encord.constants.enums import DataType
 from encord.constants.model import AutomationModels, Device
 from encord.constants.string_constants import *
+from encord.exceptions import EncordException
 from encord.http.constants import DEFAULT_REQUESTS_SETTINGS, RequestsSettings
 from encord.http.querier import Querier
 from encord.http.utils import (
     CloudUploadSettings,
     upload_images_to_encord,
     upload_to_signed_url_list,
     upload_video_to_encord,
@@ -1096,28 +1097,20 @@
                 files.append(
                     {
                         "uid": str(uuid.uuid4()),  # Add uuid as inference identifier
                         "base64_str": base64_string.decode("utf-8"),  # base64 string to utf-8
                     }
                 )
 
-        if isinstance(device, Device):
-            device = device.value
-
-        if device is None or not Device.has_value(device):  # Backward compatibility with string options
-            raise encord.exceptions.EncordException(
-                message="You must pass a device from the `from encord.constants.model.Device` Enum to run inference."
-            )
-
         inference_params = ModelInferenceParams(
             {
                 "files": files,
                 "conf_thresh": conf_thresh,
                 "iou_thresh": iou_thresh,
-                "device": device,
+                "device": _device_to_string(device),
                 "detection_frame_range": detection_frame_range,
                 "allocation_enabled": allocation_enabled,
                 "data_hashes": data_hashes,
                 "rdp_thresh": rdp_thresh,
             }
         )
 
@@ -1154,29 +1147,21 @@
             raise encord.exceptions.EncordException(message="You must set a batch size to train a model.")
 
         if weights is None or not isinstance(weights, ModelTrainingWeights):
             raise encord.exceptions.EncordException(
                 message="You must pass weights from the `encord.constants.model_weights` module to train a model."
             )
 
-        if isinstance(device, Device):
-            device = device.value
-
-        if device is None or not Device.has_value(device):  # Backward compatibility with string options
-            raise encord.exceptions.EncordException(
-                message="You must pass a device from the `from encord.constants.model.Device` Enum to train a model."
-            )
-
         training_params = ModelTrainingParams(
             {
                 "label_rows": label_rows,
                 "epochs": epochs,
                 "batch_size": batch_size,
                 "weights": weights,
-                "device": device,
+                "device": _device_to_string(device),
             }
         )
 
         model = Model(
             {
                 "model_operation": ModelOperations.TRAIN.value,
                 "model_parameters": training_params,
@@ -1316,8 +1301,17 @@
         self._querier.basic_setter(
             LabelWorkflowGraphNode,
             label_hashes,
             payload=LabelWorkflowGraphNodePayload({"action": WorkflowAction.COMPLETE.value}),
         )
 
 
+def _device_to_string(device: Device) -> str:
+    if not isinstance(device, Device):
+        if device is None or not Device.has_value(device):  # Backward compatibility with string options
+            raise EncordException(message="You must pass a device from the `from encord.constants.model.Device` enum.")
+        return cast(str, device)
+
+    return device.value
+
+
 CordClientProject = EncordClientProject
```

### Comparing `encord-0.1.83/encord/configs.py` & `encord-0.1.84/encord/configs.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/constants/enums.py` & `encord-0.1.84/encord/constants/enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Any
 
-from encord.orm.project import StringEnum
+from encord.common.enum import StringEnum
 
 
 class DataType(StringEnum):
     VIDEO = "video"
     IMG_GROUP = "img_group"
     DICOM = "dicom"
     IMAGE = "image"
```

### Comparing `encord-0.1.83/encord/constants/model.py` & `encord-0.1.84/encord/constants/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     RESNET18 = "resnet18"
     RESNET34 = "resnet34"
     RESNET50 = "resnet50"
     RESNET101 = "resnet101"
     RESNET152 = "resnet152"
     VGG16 = "vgg16"
     VGG19 = "vgg19"
-    YOLOV5 = "yolov5"
     FASTER_RCNN = "faster_rcnn"
     MASK_RCNN = "mask_rcnn"
 
     @staticmethod
     def classification_options() -> Set[AutomationModels]:
         """
         Returns:
@@ -64,15 +63,15 @@
     @staticmethod
     def object_detection_options() -> Set[AutomationModels]:
         """
         Returns:
             Model types that can be used with bounding_box type
             ``<feature_node_hashes>`` from the ``objects`` part of the project ontology.
         """
-        return {AutomationModels.YOLOV5, AutomationModels.FASTER_RCNN}
+        return {AutomationModels.FASTER_RCNN}
 
     @staticmethod
     def instance_segmentation_options() -> Set[AutomationModels]:
         """
         Returns:
             Model types that can be used with polygon type ``<feature_node_hashes>``
             from the ``objects`` part of the project ontology.
@@ -90,10 +89,9 @@
 RESNET18 = cast(str, AutomationModels.RESNET18.value)
 RESNET34 = cast(str, AutomationModels.RESNET34.value)
 RESNET50 = cast(str, AutomationModels.RESNET50.value)
 RESNET101 = cast(str, AutomationModels.RESNET101.value)
 RESNET152 = cast(str, AutomationModels.RESNET152.value)
 VGG16 = cast(str, AutomationModels.VGG16.value)
 VGG19 = cast(str, AutomationModels.VGG19.value)
-YOLOV5 = cast(str, AutomationModels.YOLOV5.value)
 FASTER_RCNN = cast(str, AutomationModels.FASTER_RCNN.value)
 MASK_RCNN = cast(str, AutomationModels.MASK_RCNN.value)
```

### Comparing `encord-0.1.83/encord/constants/string_constants.py` & `encord-0.1.84/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/constants/test/test_enums.py` & `encord-0.1.84/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/dataset.py` & `encord-0.1.84/encord/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/exceptions.py` & `encord-0.1.84/encord/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     pass
 
 
 class ModelWeightsInconsistentError(EncordException):
     """
     Exception thrown when an attempted model training iteration has a different
     type of weights than what is recorded (i.e. if type of model_hash (uid) is faster_rcnn,
-    but is attempted trained with yolov5 weights).
+    but is attempted trained with different model weights).
     """
 
     pass
 
 
 class ModelFeaturesInconsistentError(EncordException):
     """
```

### Comparing `encord-0.1.83/encord/http/bundle.py` & `encord-0.1.84/encord/http/bundle.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/http/constants.py` & `encord-0.1.84/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/http/error_utils.py` & `encord-0.1.84/encord/http/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/http/querier.py` & `encord-0.1.84/encord/http/querier.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,41 +14,37 @@
 # under the License.
 import dataclasses
 import logging
 import platform
 import random
 import uuid
 from contextlib import contextmanager
-from typing import Any, Generator, List, Optional, Tuple, Type, TypeVar
+from typing import Any, Generator, List, Tuple, Type, TypeVar
 
 import requests
 import requests.exceptions
 from requests import Response, Session
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
 from encord._version import __version__ as encord_version
 from encord.configs import BaseConfig
 from encord.exceptions import *
+from encord.http.common import (
+    HEADER_CLOUD_TRACE_CONTEXT,
+    HEADER_USER_AGENT,
+    RequestContext,
+)
 from encord.http.error_utils import check_error_response
 from encord.http.query_methods import QueryMethods
 from encord.http.request import Request
 from encord.orm.formatter import Formatter
 
 logger = logging.getLogger(__name__)
 
-HEADER_USER_AGENT = "User-Agent"
-HEADER_CLOUD_TRACE_CONTEXT = "X-Cloud-Trace-Context"
-
-
-@dataclass
-class RequestContext(ExceptionContext):
-    trace_id: Optional[str] = None
-    span_id: Optional[str] = None
-
 
 class Querier:
     """Querier for DB get/post requests."""
 
     T = TypeVar("T")
 
     def __init__(self, config: BaseConfig):
@@ -84,17 +80,17 @@
             )
 
     @staticmethod
     def _parse_response(object_type: Type[T], item: dict) -> T:
         if issubclass(object_type, Formatter):
             return object_type.from_dict(item)
         elif dataclasses.is_dataclass(object_type):
-            return object_type(**item)
+            return object_type(**item)  # type: ignore
         else:
-            return object_type(item)
+            return object_type(item)  # type: ignore
 
     def basic_delete(self, db_object_type: Type[T], uid=None):
         """Single DB object getter."""
         request = self._request(
             QueryMethods.DELETE,
             db_object_type,
             uid,
@@ -155,30 +151,30 @@
 
             x_cloud_trace_context = x_cloud_trace_context.split(";")[0]
             trace_id, span_id = (x_cloud_trace_context.split("/") + [None, None])[:2]
             return RequestContext(trace_id=trace_id, span_id=span_id)
         except Exception:
             return RequestContext()
 
-    def _request(self, method, db_object_type: Type[T], uid, timeout, payload=None):
+    def _request(self, method: QueryMethods, db_object_type: Type[T], uid, timeout, payload=None):
         request = Request(method, db_object_type, uid, timeout, self._config.connect_timeout, payload)
 
         request.headers = self._config.define_headers(request.data)
         request.headers[HEADER_USER_AGENT] = self._user_agent()
         request.headers[HEADER_CLOUD_TRACE_CONTEXT] = self._tracing_id()
 
         return request
 
     def _execute(self, request: Request, enable_logging=True) -> Tuple[Any, RequestContext]:
         """Execute a request."""
         if enable_logging:
             logger.info("Request: %s", (request.data[:100] + "..") if len(request.data) > 100 else request.data)
 
         req = requests.Request(
-            method=request.http_method,
+            method=str(request.http_method),
             url=self._config.endpoint,
             headers=request.headers,
             data=request.data,
         ).prepare()
 
         timeouts = (request.connect_timeout, request.timeout)
```

### Comparing `encord-0.1.83/encord/http/query_methods.py` & `encord-0.1.84/encord/orm/dataset_with_user_role.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 #
-# Copyright (c) 2023 Cord Technologies Limited
+# Copyright (c) 2022 Cord Technologies Limited
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may
 # not use this file except in compliance with the License. You may obtain
 # a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+from dataclasses import dataclass
 
-class QueryMethods(object):
-    GET = "GET"
-    POST = "POST"
-    PUT = "PUT"
-    DELETE = "DELETE"
+
+@dataclass(frozen=True)
+class DatasetWithUserRole:
+    """
+    This is a helper class denoting the relationship between the current user and a project
+    """
+
+    user_role: int
+    dataset: dict
```

### Comparing `encord-0.1.83/encord/http/request.py` & `encord-0.1.84/encord/http/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 class Request(object):
     """
     Request object. Takes query parameters and prepares them for execution.
     """
 
     def __init__(
         self,
-        query_method,
+        query_method: QueryMethods,
         db_object_type,
         uid,
         timeout,
         connect_timeout,
         payload,
     ) -> None:
         self.http_method = QueryMethods.POST
         self.data: str = json.dumps(
             {
                 "query_type": db_object_type.__name__.lower(),
-                "query_method": query_method,
+                "query_method": str(query_method),
                 "values": {
                     "uid": uid,
                     "payload": payload,
                 },
             }
         )
         self.timeout = timeout
```

### Comparing `encord-0.1.83/encord/http/utils.py` & `encord-0.1.84/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/objects/bitmask.py` & `encord-0.1.84/encord/objects/bitmask.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/objects/common.py` & `encord-0.1.84/encord/objects/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 import re
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import (
     Any,
     Dict,
+    Generic,
     Iterable,
     List,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
+from encord.common.enum import StringEnum
 from encord.exceptions import OntologyError
 from encord.objects.utils import (
     _decode_nested_uid,
     check_type,
     filter_by_type,
     short_uuid_str,
 )
-from encord.orm.project import StringEnum
 
 NestedID = List[int]
 
 
 class PropertyType(StringEnum):
     RADIO = "radio"
     TEXT = "text"
@@ -41,15 +42,18 @@
     POINT = "point"
     SKELETON = "skeleton"
     POLYLINE = "polyline"
     ROTATABLE_BOUNDING_BOX = "rotatable_bounding_box"
     BITMASK = "bitmask"
 
 
-class Attribute(ABC):
+OptionType = TypeVar("OptionType", bound="Option")
+
+
+class Attribute(ABC, Generic[OptionType]):
     """
     Base class for shared Attribute fields
     """
 
     uid: NestedID
     feature_node_hash: str
     name: str
@@ -64,15 +68,15 @@
         self.uid = uid
         self.feature_node_hash = feature_node_hash
         self.name = name
         self.required = required
         self.dynamic = dynamic
 
     @property
-    def options(self) -> Sequence[Option]:
+    def options(self) -> Sequence[OptionType]:
         return []
 
     @staticmethod
     @abstractmethod
     def get_property_type() -> PropertyType:
         pass
 
@@ -194,15 +198,15 @@
 
     def __eq__(self, other: object):
         return (
             isinstance(other, Attribute) and self.uid == other.uid and self.feature_node_hash == other.feature_node_hash
         )
 
 
-class RadioAttribute(Attribute):
+class RadioAttribute(Attribute["NestableOption"]):
     """
     This class is currently in BETA. Its API might change in future minor version releases.
     """
 
     _options: List[NestableOption]
 
     def __init__(
@@ -214,15 +218,15 @@
         dynamic: bool,
         options: Optional[List[NestableOption]] = None,
     ):
         super().__init__(uid, feature_node_hash, name, required, dynamic)
         self._options = options if options is not None else []
 
     @property
-    def options(self) -> Sequence[Option]:
+    def options(self) -> Sequence[NestableOption]:
         return self._options
 
     @staticmethod
     def get_property_type() -> PropertyType:
         return PropertyType.RADIO
 
     @staticmethod
@@ -288,15 +292,15 @@
 
         Returns:
             a `NestableOption` instance attached to the attribute. This can be further specified by adding nested attributes.
         """
         return _add_option(self._options, NestableOption, label, self.uid, local_uid, feature_node_hash, value)
 
 
-class ChecklistAttribute(Attribute):
+class ChecklistAttribute(Attribute["FlatOption"]):
     """
     This class is currently in BETA. Its API might change in future minor version releases.
     """
 
     _options: List[FlatOption]
 
     def __init__(
@@ -321,15 +325,15 @@
 
     def _encode_options(self) -> Optional[List[Dict[str, Any]]]:
         if len(self._options) == 0:
             return None
         return [option.to_dict() for option in self._options]
 
     @property
-    def options(self) -> Sequence[Option]:
+    def options(self) -> Sequence[FlatOption]:
         return self._options
 
     def get_child_by_hash(
         self,
         feature_node_hash: str,
         type_: Optional[OntologyElementType] = None,
     ) -> OntologyElement:
@@ -377,15 +381,15 @@
                     omit this unless the aim is to create an exact clone of existing ontology
         Returns:
             a `FlatOption` instance attached to the attribute.
         """
         return _add_option(self._options, FlatOption, label, self.uid, local_uid, feature_node_hash, value)
 
 
-class TextAttribute(Attribute):
+class TextAttribute(Attribute["FlatOption"]):
     """
     This class is currently in BETA. Its API might change in future minor version releases.
     """
 
     def __init__(self, uid: NestedID, feature_node_hash: str, name: str, required: bool, dynamic: bool):
         super().__init__(uid, feature_node_hash, name, required, dynamic)
```

### Comparing `encord-0.1.83/encord/objects/coordinates.py` & `encord-0.1.84/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/objects/frames.py` & `encord-0.1.84/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/objects/internal_helpers.py` & `encord-0.1.84/encord/objects/internal_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from copy import deepcopy
 from dataclasses import dataclass
 from typing import (
     Any,
     Dict,
     Generic,
     Iterable,
     List,
@@ -71,15 +70,15 @@
 
     @is_manual_annotation.setter
     def is_manual_annotation(self, value: bool) -> None:
         self._is_manual_annotation = value
 
     @property
     def ontology_attribute(self) -> AttributeType:
-        return deepcopy(self._ontology_attribute)
+        return self._ontology_attribute
 
     @ontology_attribute.setter
     def ontology_attribute(self, v: Any) -> NoReturn:
         raise RuntimeError("Cannot reset the ontology attribute of an instantiated answer.")
 
     @abstractmethod
     def set(self, value: ValueType) -> None:
```

### Comparing `encord-0.1.83/encord/objects/ontology_labels_impl.py` & `encord-0.1.84/encord/objects/ontology_labels_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,15 +397,15 @@
 
     @classification_hash.setter
     def classification_hash(self, v: Any) -> NoReturn:
         raise LabelRowError("Cannot set the object hash on an instantiated label object.")
 
     @property
     def ontology_item(self) -> Classification:
-        return deepcopy(self._ontology_classification)
+        return self._ontology_classification
 
     @property
     def classification_name(self) -> str:
         """Classification name from the project ontology"""
         return self._ontology_classification.attributes[0].name
 
     @property
@@ -486,25 +486,37 @@
                 last_edited_by=last_edited_by,
                 reviews=reviews,
             )
 
         if self.is_assigned_to_label_row():
             assert self._parent is not None
             self._parent._add_frames_to_classification(self.ontology_item, frames_list)
-            self._parent._add_to_frame_to_hashes_map(self)
+            self._parent._add_to_frame_to_hashes_map(self, frames_list)
 
     def get_annotation(self, frame: Union[int, str] = 0) -> Annotation:
         """
         Args:
             frame: Either the frame number or the image hash if the data type is an image or image group.
                 Defaults to the first frame.
         """
         if isinstance(frame, str):
-            frame = self._parent.get_frame_number(frame)
-        return self.Annotation(self, frame)
+            # TODO: this check should be consistent for both string and integer frames,
+            #       but currently it is not possible due to the parsing logic
+            if not self._parent:
+                raise LabelRowError(
+                    "Cannot get annotation for a classification instance that is not assigned to a label row."
+                )
+
+            frame_num = self._parent.get_frame_number(frame)
+            if frame_num is None:
+                raise LabelRowError(f"Image hash {frame} is not present in the label row.")
+        else:
+            frame_num = frame
+
+        return self.Annotation(self, frame_num)
 
     def remove_from_frames(self, frames: Frames) -> None:
         frame_list = frames_class_to_frames_list(frames)
         for frame in frame_list:
             self._frames_to_data.pop(frame)
 
         if self.is_assigned_to_label_row():
@@ -524,15 +536,15 @@
 
     def is_valid(self) -> None:
         if not len(self._frames_to_data) > 0:
             raise LabelRowError("ClassificationInstance is not on any frames. Please add it to at least one frame.")
 
     def set_answer(
         self,
-        answer: Union[str, Option, Iterable[Option]],
+        answer: Union[str, Option, Sequence[Option]],
         attribute: Optional[Attribute] = None,
         overwrite: bool = False,
     ) -> None:
         """
         Set the answer for a given ontology Attribute. This is the equivalent of e.g. selecting a checkbox in the
         UI after adding a ClassificationInstance. There is only one answer per ClassificationInstance per Attribute.
 
@@ -568,15 +580,15 @@
     def set_answer_from_list(self, answers_list: List[Dict[str, Any]]) -> None:
         """
         This is a low level helper function and should not be used directly.
 
         Sets the answer for the classification from a dictionary.
 
         Args:
-            answer_dict: The dictionary to set the answer from.
+            answers_list: The list to set the answer from.
         """
 
         for answer_dict in answers_list:
             attribute = _get_attribute_by_hash(answer_dict["featureHash"], self._ontology_classification.attributes)
             if attribute is None:
                 raise LabelRowError(
                     "One of the attributes does not exist in the ontology. Cannot create a valid LabelRow."
@@ -775,15 +787,15 @@
         reviews: Optional[List[dict]] = None
 
         @staticmethod
         def from_dict(d: dict) -> ClassificationInstance.FrameData:
             if "lastEditedAt" in d:
                 last_edited_at = parse(d["lastEditedAt"])
             else:
-                last_edited_at = None
+                last_edited_at = datetime.now()
 
             return ClassificationInstance.FrameData(
                 created_at=parse(d["createdAt"]),
                 created_by=d["createdBy"],
                 confidence=d["confidence"],
                 manual_annotation=d["manualAnnotation"],
                 last_edited_at=last_edited_at,
@@ -989,14 +1001,16 @@
         """
         if self.__is_tms2_project:
             raise WrongProjectTypeError(
                 '"annotation_task_status" property returns incorrect results for workflow-based projects.\
              Please use "workflow_graph_node" property instead.'
             )
 
+        assert self._label_row_read_only_data.annotation_task_status is not None  # Never None for Workflow projects
+
         return self._label_row_read_only_data.annotation_task_status
 
     @property
     def workflow_graph_node(self) -> Optional[WorkflowGraphNode]:
         return self._label_row_read_only_data.workflow_graph_node
 
     @property
@@ -1256,14 +1270,15 @@
         self._check_labelling_is_initalised()
 
         dict_labels = self.to_encord_dict()
 
         if bundle is None:
             self._project_client.save_label_row(uid=self.label_hash, label=dict_labels)
         else:
+            assert self.label_hash is not None  # Checked earlier, assert is mostly to silence mypy
             bundle.add(
                 operation=self._project_client.save_label_rows,
                 request_reducer=self._batch_save_rows_reducer,
                 result_mapper=None,
                 payload=BundledSaveRowsPayload(uids=[self.label_hash], payload=[dict_labels]),
                 limit=LABEL_ROW_BUNDLE_SAVE_LIMIT,
             )
@@ -1280,16 +1295,21 @@
         """
         Args:
             frame: Either the frame number or the image hash if the data type is an image or image group.
                 Defaults to the first frame.
         """
         self._check_labelling_is_initalised()
         if isinstance(frame, str):
-            frame = self.get_frame_number(frame)
-        return self.FrameView(self, self._label_row_read_only_data, frame)
+            frame_num = self.get_frame_number(frame)
+            if frame_num is None:
+                raise LabelRowError(f"Image hash {frame} not found in the label row")
+        else:
+            frame_num = frame
+
+        return self.FrameView(self, self._label_row_read_only_data, frame_num)
 
     def get_frame_views(self) -> List[FrameView]:
         """
         Returns:
             A list of frame views in order of available frames.
         """
         self._check_labelling_is_initalised()
@@ -1370,15 +1390,16 @@
             )
         elif object_hash in self._objects_map and force:
             self._objects_map.pop(object_hash)
 
         self._objects_map[object_hash] = object_instance
         object_instance._parent = self
 
-        self._add_to_frame_to_hashes_map(object_instance)
+        frames = set(_frame_views_to_frame_numbers(object_instance.get_annotations()))
+        self._add_to_frame_to_hashes_map(object_instance, frames)
 
     def add_classification_instance(self, classification_instance: ClassificationInstance, force: bool = False) -> None:
         """
         Add a classification instance to the label row.
 
         Args:
             classification_instance: The object instance to add.
@@ -1391,18 +1412,20 @@
         if classification_instance.is_assigned_to_label_row():
             raise LabelRowError(
                 "The supplied ClassificationInstance is already part of a LabelRowV2. You can only add a ClassificationInstance"
                 " to one LabelRowV2. You can do a ClassificationInstance.copy() to create an identical ObjectInstance which is "
                 "not part of any LabelRowV2."
             )
 
+        frames = set(_frame_views_to_frame_numbers(classification_instance.get_annotations()))
+
         classification_hash = classification_instance.classification_hash
         already_present_frame = self._is_classification_already_present(
             classification_instance.ontology_item,
-            _frame_views_to_frame_numbers(classification_instance.get_annotations()),
+            frames,
         )
         if classification_hash in self._classifications_map and not force:
             raise LabelRowError(
                 "The supplied ClassificationInstance was already previously added. (the classification_hash is the same)."
             )
 
         if already_present_frame is not None and not force:
@@ -1414,18 +1437,16 @@
 
         if classification_hash in self._classifications_map and force:
             self._classifications_map.pop(classification_hash)
 
         self._classifications_map[classification_hash] = classification_instance
         classification_instance._parent = self
 
-        self._classifications_to_frames[classification_instance.ontology_item].update(
-            set(_frame_views_to_frame_numbers(classification_instance.get_annotations()))
-        )
-        self._add_to_frame_to_hashes_map(classification_instance)
+        self._classifications_to_frames[classification_instance.ontology_item].update(frames)
+        self._add_to_frame_to_hashes_map(classification_instance, frames)
 
     def remove_classification(self, classification_instance: ClassificationInstance):
         """Remove a classification instance from a label row."""
         self._check_labelling_is_initalised()
 
         classification_hash = classification_instance.classification_hash
         self._classifications_map.pop(classification_hash)
@@ -1724,27 +1745,27 @@
             return self._label_row_read_only_data.frame_level_data[self._frame]
 
         def __repr__(self):
             return f"FrameView(label_row={self._label_row}, frame={self._frame})"
 
     @dataclass(frozen=True)
     class FrameLevelImageGroupData:
-        """This is an internal helper class. A user should not directly interract with it."""
+        """This is an internal helper class. A user should not directly interact with it."""
 
         image_hash: str
         image_title: str
         file_type: str
         frame_number: int
         width: int
         height: int
         data_link: Optional[str] = None
 
     @dataclass(frozen=True)
     class LabelRowReadOnlyData:
-        """This is an internal helper class. A user should not directly interract with it."""
+        """This is an internal helper class. A user should not directly interact with it."""
 
         label_hash: Optional[str]
         """This is None if the label row does not have any labels and was not initialised for labelling."""
         created_at: Optional[datetime]
         """This is None if the label row does not have any labels and was not initialised for labelling."""
         last_edited_at: Optional[datetime]
         """This is None if the label row does not have any labels and was not initialised for labelling."""
@@ -1833,15 +1854,15 @@
         return ret
 
     def _to_encord_data_unit(self, frame_level_data: FrameLevelImageGroupData) -> Dict[str, Any]:
         ret: Dict[str, Any] = {}
 
         data_type = self._label_row_read_only_data.data_type
         if data_type == DataType.IMG_GROUP:
-            data_sequence = str(frame_level_data.frame_number)
+            data_sequence: Union[str, int] = str(frame_level_data.frame_number)
         elif data_type in (DataType.VIDEO, DataType.DICOM, DataType.IMAGE):
             data_sequence = frame_level_data.frame_number
         else:
             raise NotImplementedError(f"The data type {data_type} is not implemented yet.")
 
         ret["data_hash"] = frame_level_data.image_hash
         ret["data_title"] = frame_level_data.image_title
@@ -2000,18 +2021,19 @@
         self._classifications_to_frames[classification].update(set(frames))
 
     def _remove_frames_from_classification(self, classification: Classification, frames: Iterable[int]) -> None:
         present_frames = self._classifications_to_frames.get(classification, set())
         for frame in frames:
             present_frames.remove(frame)
 
-    def _add_to_frame_to_hashes_map(self, label_item: Union[ObjectInstance, ClassificationInstance]) -> None:
-        """This can be called by the ObjectInstance."""
-        for frame_view in label_item.get_annotations():
-            self.add_to_single_frame_to_hashes_map(label_item, frame_view.frame)
+    def _add_to_frame_to_hashes_map(
+        self, label_item: Union[ObjectInstance, ClassificationInstance], frames: Iterable[int]
+    ) -> None:
+        for frame in frames:
+            self.add_to_single_frame_to_hashes_map(label_item, frame)
 
     def _remove_from_frame_to_hashes_map(self, frames: Iterable[int], item_hash: str):
         for frame in frames:
             self._frame_to_hashes[frame].remove(item_hash)
 
     def _parse_label_row_metadata(self, label_row_metadata: LabelRowMetadata) -> LabelRowV2.LabelRowReadOnlyData:
         data_type = DataType.from_upper_case_string(label_row_metadata.data_type)
@@ -2293,16 +2315,16 @@
 
     @property
     def object_hash(self) -> str:
         """A unique identifier for the object instance."""
         return self._object_hash
 
     @property
-    def ontology_item(self) -> Any:
-        return deepcopy(self._ontology_object)
+    def ontology_item(self) -> Object:
+        return self._ontology_object
 
     @property
     def feature_hash(self) -> str:
         """Feature node hash from the project ontology"""
         return self._ontology_object.feature_node_hash
 
     @property
@@ -2372,15 +2394,15 @@
         answer: Union[str, Option, Sequence[Option]],
         attribute: Optional[Attribute] = None,
         frames: Optional[Frames] = None,
         overwrite: bool = False,
     ) -> None:
         """
         Set the answer for a given ontology Attribute. This is the equivalent of e.g. selecting a checkbox in the
-        UI after drowing the ObjectInstance. There is only one answer per ObjectInstance per Attribute, unless
+        UI after drawing the ObjectInstance. There is only one answer per ObjectInstance per Attribute, unless
         the attribute is dynamic (check the args list for more instructions on how to set dynamic answers).
 
         Args:
             answer: The answer to set.
             attribute: The ontology attribute to set the answer for. If not set, this will be attempted to be
                 inferred.  For answers to :class:`encord.objects.common.RadioAttribute` or
                 :class:`encord.objects.common.ChecklistAttribute`, this can be inferred automatically. For
@@ -2423,15 +2445,15 @@
     def set_answer_from_list(self, answers_list: List[Dict[str, Any]]) -> None:
         """
         This is a low level helper function and should usually not be used directly.
 
         Sets the answer for the classification from a dictionary.
 
         Args:
-            answer_dict: The dictionary to set the answer from.
+            answers_list: The list of dictionaries to set the answer from.
         """
 
         for answer_dict in answers_list:
             attribute = _get_attribute_by_hash(answer_dict["featureHash"], self._ontology_object.attributes)
             if attribute is None:
                 raise LabelRowError(
                     "One of the attributes does not exist in the ontology. Cannot create a valid LabelRow."
@@ -2557,17 +2579,28 @@
         """
         Get the annotation for the object instance on the specified frame.
 
         Args:
             frame: Either the frame number or the image hash if the data type is an image or image group.
                 Defaults to the first frame.
         """
+
         if isinstance(frame, str):
-            frame = self._parent.get_frame_number(frame)
-        return self.Annotation(self, frame)
+            # TODO: this check should be consistent for both string and integer frames,
+            #       but currently it is not possible due to the parsing logic
+            if not self._parent:
+                raise LabelRowError("Cannot get annotation for an object instance that is not assigned to a label row.")
+
+            frame_num = self._parent.get_frame_number(frame)
+            if frame_num is None:
+                raise LabelRowError(f"Image hash {frame} is not present in the label row.")
+        else:
+            frame_num = frame
+
+        return self.Annotation(self, frame_num)
 
     def copy(self) -> ObjectInstance:
         """
         Creates an exact copy of this ObjectInstance but with a new object hash and without being associated to any
         LabelRowV2. This is useful if you want to add the semantically same ObjectInstance to multiple
         `LabelRowV2`s.
         """
@@ -2750,15 +2783,15 @@
         is_deleted: Optional[bool] = None
 
         @staticmethod
         def from_dict(d: dict):
             if "lastEditedAt" in d:
                 last_edited_at = parse(d["lastEditedAt"])
             else:
-                last_edited_at = None
+                last_edited_at = datetime.now()
 
             return ObjectInstance.FrameInfo(
                 created_at=parse(d["createdAt"]),
                 created_by=d["createdBy"],
                 last_edited_at=last_edited_at,
                 last_edited_by=d.get("lastEditedBy"),
                 confidence=d["confidence"],
@@ -2797,15 +2830,19 @@
     @dataclass
     class FrameData:
         coordinates: Coordinates
         object_frame_instance_info: ObjectInstance.FrameInfo
         # Probably the above can be flattened out into this class.
 
     def _set_answer_unsafe(
-        self, answer: Union[str, Option, Iterable[Option]], attribute: Attribute, track_hash: str, ranges: Ranges
+        self,
+        answer: Union[str, Option, Iterable[Option]],
+        attribute: Attribute,
+        track_hash: str,
+        ranges: Optional[Ranges],
     ) -> None:
         if attribute.dynamic:
             self._dynamic_answer_manager.set_answer(answer, attribute, frames=ranges)
 
         else:
             static_answer = self._static_answer_map[attribute.feature_node_hash]
             static_answer.set(answer)
@@ -3301,17 +3338,14 @@
             raise ValueError(f"Duplicate feature_node_hash '{feature_node_hash}'")
 
         cls = Classification(uid, feature_node_hash, list())
         self.classifications.append(cls)
         return cls
 
 
-DATETIME_STRING_FORMAT = "%Y-%m-%d %H:%M:%S"
-
-
 class OntologyUserRole(IntEnum):
     ADMIN = 0
     USER = 1
 
 
 class Ontology(dict, Formatter):
     def __init__(
```

### Comparing `encord-0.1.83/encord/objects/project.py` & `encord-0.1.84/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/objects/utils.py` & `encord-0.1.84/encord/objects/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,19 @@
     return base64.b64encode(uuid.uuid4().bytes[:6]).decode("utf-8")
 
 
 def _lower_snake_case(s: str):
     return s.lower().replace(" ", "_")
 
 
+def _snake_to_camel(snake_case_str: str) -> str:
+    camel = re.sub("([0-9A-Za-z])_(?=[0-9A-Z])", lambda m: m.group(1), snake_case_str.title())
+    return re.sub("(^_*[A-Z])", lambda m: m.group(1).lower(), camel)
+
+
 def check_type(obj: Any, type_: Optional[Type[Any]]) -> None:
     if not does_type_match(obj, type_):
         raise TypeError(f"Expected {type_}, got {type(obj)}")
 
 
 def does_type_match(obj: Any, type_: Optional[Type[Any]]) -> bool:
     if type_ is None:
```

### Comparing `encord-0.1.83/encord/ontology.py` & `encord-0.1.84/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/orm/api_key.py` & `encord-0.1.84/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/orm/base_orm.py` & `encord-0.1.84/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/orm/dataset.py` & `encord-0.1.84/encord/orm/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,22 +20,21 @@
 from datetime import datetime
 from enum import Enum, IntEnum
 from typing import Any, Dict, List, Optional
 from uuid import UUID
 
 from dateutil import parser
 
+from encord.common.constants import DATETIME_STRING_FORMAT
 from encord.constants.enums import DataType
 from encord.exceptions import EncordException
 from encord.orm import base_orm
 from encord.orm.formatter import Formatter
 from encord.utilities.common import _get_dict_without_none_keys
 
-DATETIME_STRING_FORMAT = "%Y-%m-%d %H:%M:%S"
-
 
 class DatasetUserRole(IntEnum):
     ADMIN = 0
     USER = 1
 
 
 @dataclasses.dataclass(frozen=True)
```

### Comparing `encord-0.1.83/encord/orm/dataset_with_user_role.py` & `encord-0.1.84/encord/orm/project_with_user_role.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 from dataclasses import dataclass
 
 
 @dataclass(frozen=True)
-class DatasetWithUserRole:
+class ProjectWithUserRole:
     """
     This is a helper class denoting the relationship between the current user an a project
     """
 
-    user_role: str
-    dataset: dict
+    user_role: int
+    project: dict
```

### Comparing `encord-0.1.83/encord/orm/label_log.py` & `encord-0.1.84/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/orm/label_row.py` & `encord-0.1.84/encord/orm/label_row.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/orm/labeling_algorithm.py` & `encord-0.1.84/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/orm/model.py` & `encord-0.1.84/encord/orm/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 
         return ModelTrainingLabel.from_dict(model_training_labels)
 
 
 class ModelRow(base_orm.BaseORM):
     """
     A model row contains a set of features and a model (resnet18, resnet34, resnet50, resnet101, resnet152,
-    vgg16, vgg19, yolov5, faster_rcnn, mask_rcnn).
+    vgg16, vgg19, faster_rcnn, mask_rcnn).
 
     ORM:
 
     model_hash (uid),
     title,
     description,
     features,
```

### Comparing `encord-0.1.83/encord/orm/ontology.py` & `encord-0.1.84/encord/orm/ontology.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 # pylint: disable=unused-import
-from encord.objects.ontology_labels_impl import (
-    DATETIME_STRING_FORMAT,
-    Ontology,
-    OntologyUserRole,
-)
+from encord.common.constants import DATETIME_STRING_FORMAT
+
+# pylint: disable=unused-import
+from encord.objects.ontology_labels_impl import Ontology, OntologyUserRole
 
 # Importing here for backwards compatibility
```

### Comparing `encord-0.1.83/encord/orm/project.py` & `encord-0.1.84/encord/orm/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import datetime
 from collections import OrderedDict
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Dict, List, Optional, Union
 
+from encord.common.enum import StringEnum
 from encord.orm import base_orm
 
 
 class Project(base_orm.BaseORM):
     """
     DEPRECATED - prefer using the `encord.project.Project` class instead.
 
@@ -96,15 +97,15 @@
                 created_labels_list = []
                 for label in labels_list:
                     if label is not None:  # None values will fail the operation
                         created_labels_list.append(label)
 
                 label_rows = project.get_label_rows(created_labels_list, get_signed_url=False)
         """
-        labels = self.to_dic().get("label_rows")
+        labels = self.to_dic().get("label_rows", [])
         res = []
         for label in labels:
             res.append(label.get("label_hash"))
         return res
 
     @property
     def project_hash(self):
@@ -252,28 +253,14 @@
 
 Currently one of:
     :class:`ManualReviewWorkflowSettings`: a workflow with optional manual reviews
     :class:`BenchmarkQaWorkflowSettings`: annotators are presented with "benchmark" or "honeypot" data
 """
 
 
-class StringEnum(Enum):
-    """
-    Use this enum class if you need the helper that creates the enum instance from a string.
-    """
-
-    def __str__(self):
-        return self.name
-
-    @classmethod
-    def from_string(cls, value: str) -> Optional[StringEnum]:
-        # pylint: disable-next=no-member
-        return cls._value2member_map_.get(value)
-
-
 class ReviewMode(StringEnum):
     """
     UNLABELLED:
         The labels are added to the images. However, the one person must still go over
             all of the labels before submitting them for review.
     LABELLED:
         The labels are added to the images and are marked as labelled. A reviewer will
```

### Comparing `encord-0.1.83/encord/orm/project_api_key.py` & `encord-0.1.84/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/orm/project_with_user_role.py` & `encord-0.1.84/encord/http/query_methods.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 #
-# Copyright (c) 2022 Cord Technologies Limited
+# Copyright (c) 2023 Cord Technologies Limited
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may
 # not use this file except in compliance with the License. You may obtain
 # a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
+from encord.constants.enums import StringEnum
 
-from dataclasses import dataclass
 
-
-@dataclass(frozen=True)
-class ProjectWithUserRole:
-    """
-    This is a helper class denoting the relationship between the current user an a project
-    """
-
-    user_role: int
-    project: dict
+class QueryMethods(StringEnum):
+    GET = "GET"
+    POST = "POST"
+    PUT = "PUT"
+    DELETE = "DELETE"
```

### Comparing `encord-0.1.83/encord/orm/test/test_dataset.py` & `encord-0.1.84/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/project.py` & `encord-0.1.84/encord/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import datetime
+from pathlib import Path
 from typing import Iterable, List, Optional, Set, Tuple, Union
 
 from encord.client import EncordClientProject
 from encord.constants.model import AutomationModels, Device
 from encord.http.bundle import Bundle
+from encord.http.v2.api_client import ApiClient
+from encord.http.v2.payloads import Page
 from encord.objects import LabelRowV2
 from encord.ontology import Ontology
+from encord.orm.analytics import (
+    CollaboratorTimer,
+    CollaboratorTimerParams,
+    CollaboratorTimersGroupBy,
+)
 from encord.orm.cloud_integration import CloudIntegration
 from encord.orm.dataset import Image, Video
 from encord.orm.label_log import LabelLog
 from encord.orm.label_row import (
     AnnotationTaskStatus,
     LabelRow,
     LabelRowMetadata,
@@ -26,16 +34,19 @@
 
 
 class Project:
     """
     Access project related data and manipulate the project.
     """
 
-    def __init__(self, client: EncordClientProject, project_instance: OrmProject, ontology: Ontology):
+    def __init__(
+        self, client: EncordClientProject, project_instance: OrmProject, ontology: Ontology, client_v2: ApiClient
+    ):
         self._client = client
+        self._client_v2 = client_v2
         self._project_instance = project_instance
         self._ontology = ontology
 
     @property
     def project_hash(self) -> str:
         """
         Get the project hash (i.e. the Project ID).
@@ -954,7 +965,48 @@
     def create_bundle(self) -> Bundle:
         """
         Initialises a bundle to reduce amount of network calls performed by the Encord SDK
 
         See the :class:`encord.http.bundle.Bundle` documentation for more details
         """
         return Bundle()
+
+    def list_collaborator_timers(
+        self,
+        after: datetime.datetime,
+        before: Optional[datetime.datetime] = None,
+        group_by_data_unit: bool = True,
+    ) -> Iterable[CollaboratorTimer]:
+        """
+        Provides information about time spent for each collaborator that has worked on the project within a specified
+        range of dates.
+
+        Args:
+             after: the beginning of the period of interest.
+             before: the end of period of interest.
+             group_by_data_unit: if True, time spent by a collaborator for each data unit is provided separately,
+                                 and if False, all time spent in the scope of the project is aggregated together.
+
+        Returns:
+            Iterable[CollaboratorTimer]
+        """
+
+        params = CollaboratorTimerParams(
+            project_hash=self.project_hash,
+            after=after,
+            before=before,
+            group_by=CollaboratorTimersGroupBy.DATA_UNIT if group_by_data_unit else CollaboratorTimersGroupBy.PROJECT,
+            page_size=100,
+        )
+
+        while True:
+            page = self._client_v2.get(
+                Path("analytics/collaborators/timers"), params=params, result_type=Page[CollaboratorTimer]
+            )
+
+            for result in page.results:
+                yield result
+
+            if page.next_page_token is not None:
+                params.page_token = page.next_page_token
+            else:
+                break
```

### Comparing `encord-0.1.83/encord/project_ontology/classification_attribute.py` & `encord-0.1.84/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/project_ontology/classification_option.py` & `encord-0.1.84/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/project_ontology/ontology.py` & `encord-0.1.84/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/project_ontology/ontology_classification.py` & `encord-0.1.84/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/project_ontology/ontology_object.py` & `encord-0.1.84/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/user_client.py` & `encord-0.1.84/encord/user_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
 
 import base64
 import logging
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
-import dateutil
+from dateutil import parser as datetime_parser
 
 # add this for backward compatible class comparisons
 # pylint: disable-next=import-error
-from cord.utilities.client_utilities import LocalImport as CordLocalImport
+from cord.utilities.client_utilities import (
+    LocalImport as CordLocalImport,  # type: ignore
+)
 from encord.client import EncordClient, EncordClientDataset, EncordClientProject
 from encord.configs import SshConfig, UserConfig, get_env_ssh_key
 from encord.constants.string_constants import TYPE_DATASET, TYPE_ONTOLOGY, TYPE_PROJECT
 from encord.dataset import Dataset
 from encord.http.constants import DEFAULT_REQUESTS_SETTINGS, RequestsSettings
 from encord.http.querier import Querier
 from encord.http.utils import (
     CloudUploadSettings,
     upload_images_to_encord,
     upload_to_signed_url_list,
 )
+from encord.http.v2.api_client import ApiClient
 from encord.objects.common import (
     DeidentifyRedactTextMode,
     SaveDeidentifiedDicomCondition,
 )
 from encord.objects.ontology_labels_impl import Ontology as OrmOntology
 from encord.objects.ontology_labels_impl import OntologyStructure
 from encord.ontology import Ontology
@@ -74,14 +77,15 @@
 log = logging.getLogger(__name__)
 
 
 class EncordUserClient:
     def __init__(self, user_config: UserConfig, querier: Querier):
         self.user_config = user_config
         self.querier = querier
+        self._api_client = ApiClient(user_config)
 
     def get_dataset(
         self, dataset_hash: str, dataset_access_settings: DatasetAccessSettings = DEFAULT_DATASET_ACCESS_SETTINGS
     ) -> Dataset:
         """
         Get the Project class to access project fields and manipulate a project.
 
@@ -124,15 +128,15 @@
         # Querying ontology using project querier to avoid permission error,
         # as there might be only read-only ontology structure access in scope of the project,
         # not full access, that is implied by get_ontology method
         ontology_hash = orm_project["ontology_hash"]
         config = SshConfig(self.user_config, resource_type=TYPE_ONTOLOGY, resource_id=ontology_hash)
         project_ontology = Ontology(querier, config)
 
-        return Project(client, orm_project, project_ontology)
+        return Project(client, orm_project, project_ontology, client_v2=self._api_client)
 
     def get_ontology(self, ontology_hash: str) -> Ontology:
         config = SshConfig(self.user_config, resource_type=TYPE_ONTOLOGY, resource_id=ontology_hash)
         querier = Querier(config)
         return Ontology(querier, config)
 
     def create_private_dataset(
@@ -205,15 +209,15 @@
         title_like: Optional[str] = None,
         desc_eq: Optional[str] = None,
         desc_like: Optional[str] = None,
         created_before: Optional[Union[str, datetime]] = None,
         created_after: Optional[Union[str, datetime]] = None,
         edited_before: Optional[Union[str, datetime]] = None,
         edited_after: Optional[Union[str, datetime]] = None,
-    ) -> List[Dict]:
+    ) -> List[Dict[str, Any]]:
         """
         List either all (if called with no arguments) or matching datasets the user has access to.
 
         Args:
             title_eq: optional exact title filter
             title_like: optional fuzzy title filter; SQL syntax
             desc_eq: optional exact description filter
@@ -227,16 +231,16 @@
             list of (role, dataset) pairs for datasets  matching filter conditions.
         """
         properties_filter = self.__validate_filter(locals())
         # a hack to be able to share validation code without too much c&p
         data = self.querier.get_multiple(DatasetWithUserRole, payload={"filter": properties_filter})
 
         def convert_dates(dataset):
-            dataset["created_at"] = dateutil.parser.isoparse(dataset["created_at"])
-            dataset["last_edited_at"] = dateutil.parser.isoparse(dataset["last_edited_at"])
+            dataset["created_at"] = datetime_parser.isoparse(dataset["created_at"])
+            dataset["last_edited_at"] = datetime_parser.isoparse(dataset["last_edited_at"])
             return dataset
 
         return [
             {"dataset": DatasetInfo(**convert_dates(d.dataset)), "user_role": DatasetUserRole(d.user_role)}
             for d in data
         ]
 
@@ -610,15 +614,15 @@
                 else:
                     continue
             elif not isinstance(clause, ListingFilter):
                 continue
 
             if clause.value.endswith("before") or clause.value.endswith("after"):
                 if isinstance(val, str):
-                    val = dateutil.parser.isoparse(val)
+                    val = datetime_parser.isoparse(val)
                 if isinstance(val, datetime):
                     val = val.isoformat()
                 else:
                     raise ValueError(f"Value for {clause.name} filter should be a datetime")
 
             ret[clause.value] = val
```

### Comparing `encord-0.1.83/encord/utilities/client_utilities.py` & `encord-0.1.84/encord/utilities/client_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/utilities/label_utilities.py` & `encord-0.1.84/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/encord/utilities/project_user.py` & `encord-0.1.84/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.83/pyproject.toml` & `encord-0.1.84/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.83"
+version = "0.1.84"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["cord", "encord"]
 packages = [
     { include = "cord"},
     { include = "encord"},
@@ -21,14 +21,15 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 python-dateutil = "^2.8.2"
 requests = "^2.25.0"
 cryptography = ">=3.4.8"
 tqdm = "^4.32.1"
 importlib_metadata = {version = "^6.1.0", python = "<3.8"}
+pydantic = ">=1.7.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.1.2"
 pre-commit = "^2.16.0"
 black = "^23.3.0"
 sphinx-tabs = "^3.3.1"
 sphinx-autodoc-typehints = "1.15.2"
```

### Comparing `encord-0.1.83/PKG-INFO` & `encord-0.1.84/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.83
+Version: 0.1.84
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
 Keywords: cord,encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.7,<4.0
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=3.4.8)
 Requires-Dist: importlib_metadata (>=6.1.0,<7.0.0) ; python_version < "3.8"
+Requires-Dist: pydantic (>=1.7.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.25.0,<3.0.0)
 Requires-Dist: tqdm (>=4.32.1,<5.0.0)
 Project-URL: Documentation, https://python.docs.encord.com/
 Project-URL: Repository, https://github.com/encord-team/encord-client-python
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.83 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.84 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: cord,encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.7,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: cryptography (>=3.4.8) Requires-Dist: importlib_metadata (>=6.1.0,<7.0.0)
-; python_version < "3.8" Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: requests (>=2.25.0,<3.0.0) Requires-Dist: tqdm (>=4.32.1,<5.0.0)
-Project-URL: Documentation, https://python.docs.encord.com/ Project-URL:
-Repository, https://github.com/encord-team/encord-client-python Description-
-Content-Type: text/markdown
+; python_version < "3.8" Requires-Dist: pydantic (>=1.7.0) Requires-Dist:
+python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: requests (>=2.25.0,<3.0.0)
+Requires-Dist: tqdm (>=4.32.1,<5.0.0) Project-URL: Documentation, https://
+python.docs.encord.com/ Project-URL: Repository, https://github.com/encord-
+team/encord-client-python Description-Content-Type: text/markdown
                ****** Encord Python API Client[Cord_logo] ******
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https:
 //opensource.org/licenses/Apache-2.0) # The data engine for computer vision ##
 ð» Features - Minimal low-level Python client that allows you to interact
 with Encord's API - Supports Python: `3.7`, `3.8`, `3.9`, `3.10` and `3.11` ##
 â¨ Relevant Links * [Encord website](https://encord.com) * [Encord web app]
 (https://app.encord.com) * [Encord documentation](https://docs.encord.com) ##
```

