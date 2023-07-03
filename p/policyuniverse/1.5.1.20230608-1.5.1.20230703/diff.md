# Comparing `tmp/policyuniverse-1.5.1.20230608.tar.gz` & `tmp/policyuniverse-1.5.1.20230703.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policyuniverse-1.5.1.20230608.tar", last modified: Thu Jun  8 14:00:28 2023, max compression
+gzip compressed data, was "policyuniverse-1.5.1.20230703.tar", last modified: Mon Jul  3 18:22:09 2023, max compression
```

## Comparing `policyuniverse-1.5.1.20230608.tar` & `policyuniverse-1.5.1.20230703.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:00:28.743653 policyuniverse-1.5.1.20230608/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-08 14:00:28.743653 policyuniverse-1.5.1.20230608/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:00:28.739653 policyuniverse-1.5.1.20230608/policyuniverse/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/action_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/arn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/common.py
--rw-r--r--   0 runner    (1001) docker     (123)  7833102 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/data.json
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/expander_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:00:28.743653 policyuniverse-1.5.1.20230608/policyuniverse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-08 14:00:28.000000 policyuniverse-1.5.1.20230608/policyuniverse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-08 14:00:28.000000 policyuniverse-1.5.1.20230608/policyuniverse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:00:28.000000 policyuniverse-1.5.1.20230608/policyuniverse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:00:28.000000 policyuniverse-1.5.1.20230608/policyuniverse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 14:00:28.000000 policyuniverse-1.5.1.20230608/policyuniverse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 14:00:28.000000 policyuniverse-1.5.1.20230608/policyuniverse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 14:00:28.743653 policyuniverse-1.5.1.20230608/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:22:09.007771 policyuniverse-1.5.1.20230703/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-03 18:22:09.007771 policyuniverse-1.5.1.20230703/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:22:09.007771 policyuniverse-1.5.1.20230703/policyuniverse/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/action_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/arn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7970603 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/expander_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:22:09.007771 policyuniverse-1.5.1.20230703/policyuniverse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-03 18:22:08.000000 policyuniverse-1.5.1.20230703/policyuniverse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 18:22:08.000000 policyuniverse-1.5.1.20230703/policyuniverse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:22:08.000000 policyuniverse-1.5.1.20230703/policyuniverse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:22:08.000000 policyuniverse-1.5.1.20230703/policyuniverse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-03 18:22:08.000000 policyuniverse-1.5.1.20230703/policyuniverse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 18:22:08.000000 policyuniverse-1.5.1.20230703/policyuniverse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-03 18:22:09.011771 policyuniverse-1.5.1.20230703/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/setup.py
```

### Comparing `policyuniverse-1.5.1.20230608/LICENSE` & `policyuniverse-1.5.1.20230703/LICENSE`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230608/PKG-INFO` & `policyuniverse-1.5.1.20230703/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyuniverse
-Version: 1.5.1.20230608
+Version: 1.5.1.20230703
 Summary: Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.
 Home-page: https://github.com/Netflix-Skunkworks/policyuniverse
 Author: Patrick Kelley
 Author-email: patrickbarrettkelley@gmail.com
 Keywords: iam,arn,action_groups,condition,policy,statement,wildcard
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
```

### Comparing `policyuniverse-1.5.1.20230608/README.md` & `policyuniverse-1.5.1.20230703/README.md`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230608/policyuniverse/__init__.py` & `policyuniverse-1.5.1.20230703/policyuniverse/__init__.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230608/policyuniverse/action.py` & `policyuniverse-1.5.1.20230703/policyuniverse/action.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230608/policyuniverse/action_categories.py` & `policyuniverse-1.5.1.20230703/policyuniverse/action_categories.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230608/policyuniverse/arn.py` & `policyuniverse-1.5.1.20230703/policyuniverse/arn.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230608/policyuniverse/common.py` & `policyuniverse-1.5.1.20230703/policyuniverse/common.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230608/policyuniverse/data.json` & `policyuniverse-1.5.1.20230703/policyuniverse/data.json`

 * *Files 0% similar despite different names*

```diff
@@ -605,15 +605,15 @@
         ],
         "calculated_action_group": "Permissions",
         "condition_keys": [],
         "description": "Grants permission to add certificates for mutual TLS authentication to a domain name. This is an additional authorization control for managing the DomainName resource due to the sensitive nature of mTLS",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/api-reference/ADD_CERTIFICATE_TO_DOMAIN.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/latest/api/API_Operations.html"
         }
       },
       "DELETE": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -621,29 +621,29 @@
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
         "description": "Grants permission to delete a particular resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/api-reference/API_DELETE.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/latest/api/API_Operations.html"
         }
       },
       "GET": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to read a particular resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/api-reference/API_GET.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/latest/api/API_Operations.html"
         }
       },
       "PATCH": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -651,15 +651,15 @@
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
         "description": "Grants permission to update a particular resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/api-reference/API_PATCH.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/latest/api/API_Operations.html"
         }
       },
       "POST": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -667,15 +667,15 @@
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
         "description": "Grants permission to create a particular resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/api-reference/API_POST.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/latest/api/API_Operations.html"
         }
       },
       "PUT": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -683,54 +683,54 @@
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
         "description": "Grants permission to update a particular resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/api-reference/API_PUT.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/latest/api/API_Operations.html"
         }
       },
       "RemoveCertificateFromDomain": {
         "aws_action_groups": [
           "Permissions"
         ],
         "calculated_action_group": "Permissions",
         "condition_keys": [],
         "description": "Grants permission to remove certificates for mutual TLS authentication from a domain name. This is an additional authorization control for managing the DomainName resource due to the sensitive nature of mTLS",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/api-reference/REMOVE_CERTIFICATE_FROM_DOMAIN.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/latest/api/API_Operations.html"
         }
       },
       "SetWebACL": {
         "aws_action_groups": [
           "Permissions"
         ],
         "calculated_action_group": "Permissions",
         "condition_keys": [],
-        "description": "Grants permission set a WAF access control list (ACL). This is an additional authorization control for managing the Stage resource due to the sensitive nature of WebAcl's",
+        "description": "Grants permission to set a WAF access control list (ACL). This is an additional authorization control for managing the Stage resource due to the sensitive nature of WebAcl's",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/api-reference/WEBACL_SET.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/latest/api/API_Operations.html"
         }
       },
       "UpdateRestApiPolicy": {
         "aws_action_groups": [
           "Permissions"
         ],
         "calculated_action_group": "Permissions",
         "condition_keys": [],
         "description": "Grants permission to manage the IAM resource policy for an API. This is an additional authorization control for managing an API due to the sensitive nature of the resource policy",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/api-reference/UPDATE_REST_API_POLICY.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/apigateway/latest/api/API_Operations.html"
         }
       }
     },
     "arn_format": "arn:${Partition}:apigateway:${Region}::${ApiGatewayResourcePath}",
     "arn_regex": "^arn:${Partition}:apigateway:.+",
     "description": "Amazon API Gateway Management V2",
     "docs": {
@@ -7107,14 +7107,414 @@
       "api_reference_doc_page": "https://docs.aws.amazon.com/appconfig/2019-10-09/APIReference/Welcome.html",
       "authz_doc_page": "https://docs.aws.amazon.com/appconfig/latest/userguide/getting-started-with-appconfig-permissions.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/appconfig/latest/userguide/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/appconfig/latest/userguide/getting-started-with-appconfig-permissions.html"
     },
     "prefix": "appconfig"
   },
+  "AppFabric": {
+    "actions": {
+      "BatchGetUserAccessTasks": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to start user access tasks for multiple users",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_BatchGetUserAccessTasks.html"
+        }
+      },
+      "ConnectAppAuthorization": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to connect application authorizations",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_ConnectAppAuthorization.html"
+        }
+      },
+      "CreateAppAuthorization": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create application authorizations for application bundles",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_CreateAppAuthorization.html"
+        }
+      },
+      "CreateAppBundle": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create application bundles in your account",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_CreateAppBundle.html"
+        }
+      },
+      "CreateIngestion": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create ingestions for application bundles",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_CreateIngestion.html"
+        }
+      },
+      "CreateIngestionDestination": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create ingestion destinations for application bundles",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_CreateIngestionDestination.html"
+        }
+      },
+      "DeleteAppAuthorization": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete application authorizations within an application bundle",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_DeleteAppAuthorization.html"
+        }
+      },
+      "DeleteAppBundle": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete application bundles in your account",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_DeleteAppBundle.html"
+        }
+      },
+      "DeleteIngestion": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete ingestions within an application bundle",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_DeleteIngestion.html"
+        }
+      },
+      "DeleteIngestionDestination": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete destinations within an ingestion",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_DeleteIngestionDestination.html"
+        }
+      },
+      "GetAppAuthorization": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to view details about application authorizations",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_GetAppAuthorization.html"
+        }
+      },
+      "GetAppBundle": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to view details about application bundles",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_GetAppBundle.html"
+        }
+      },
+      "GetIngestion": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to view details about ingestions",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_GetIngestion.html"
+        }
+      },
+      "GetIngestionDestination": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to view details about ingestion destinations",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_GetIngestionDestination.html"
+        }
+      },
+      "ListAppAuthorizations": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve a list of application authorizations within an application bundle",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_ListAppAuthorizations.html"
+        }
+      },
+      "ListAppBundles": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve a list of application bundles in your account",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_ListAppBundles.html"
+        }
+      },
+      "ListIngestionDestinations": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve a list of destinations within an ingestion",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_ListIngestionDestinations.html"
+        }
+      },
+      "ListIngestions": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve a list of ingestions within an application bundle",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_ListIngestions.html"
+        }
+      },
+      "ListTagsForResource": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to list tags for AppFabric resouces",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_ListTagsForResource.html"
+        }
+      },
+      "StartIngestion": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to start ingestions",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_StartIngestion.html"
+        }
+      },
+      "StartUserAccessTasks": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to start user access tasks",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_StartUserAccessTasks.html"
+        }
+      },
+      "StopIngestion": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to stop ingestions",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_StopIngestion.html"
+        }
+      },
+      "TagResource": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "Tagging"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to tag AppFabric resources",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_TagResource.html"
+        }
+      },
+      "UntagResource": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "Tagging"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to untag AppFabric resources",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_UntagResource.html"
+        }
+      },
+      "UpdateAppAuthorization": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to update application authorizations within application bundles",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_UpdateAppAuthorization.html"
+        }
+      },
+      "UpdateIngestionDestination": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to update destinations within ingestions",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_UpdateIngestionDestination.html"
+        }
+      }
+    },
+    "arn_format": "arn:${Partition}:appfabric:${Region}:${Account}:${ResourceInfo}",
+    "arn_regex": "^arn:${Partition}:appfabric:.+:.+:.+",
+    "description": "AWS AppFabric",
+    "docs": {
+      "actions_doc_root": "https://docs.aws.amazon.com/appfabric/latest/api/",
+      "api_detail_root": "",
+      "api_doc_root": "",
+      "api_reference_doc_page": "https://docs.aws.amazon.com/appfabric/latest/api/",
+      "authz_doc_page": "https://docs.aws.amazon.com/appfabric/latest/adminguide/security.html",
+      "concepts_doc_root": "https://docs.aws.amazon.com/appfabric/latest/adminguide/",
+      "context_keys_doc_root": "https://docs.aws.amazon.com/appfabric/latest/adminguide/"
+    },
+    "prefix": "appfabric"
+  },
   "AppFlow": {
     "actions": {
       "CancelFlowExecutions": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -7395,14 +7795,27 @@
         "description": "Grants permission to register an Amazon AppFlow connector",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appflow/1.0/APIReference/API_RegisterConnector.html"
         }
       },
+      "ResetConnectorMetadataCache": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to resets metadata of connector entities that Amazon AppFlow stored in its cache",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appflow/1.0/APIReference/API_ResetConnectorMetadataCache.html"
+        }
+      },
       "RunFlow": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to run a flow configured in Amazon AppFlow (Console Only)",
@@ -7444,15 +7857,15 @@
           "Tagging"
         ],
         "calculated_action_group": "Tagging",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
-        "description": "Grants permission to tag a flow",
+        "description": "Grants permission to tag a flow or a connector",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appflow/1.0/APIReference/API_TagResource.html"
         }
       },
       "UnRegisterConnector": {
@@ -7476,15 +7889,15 @@
           "ReadWrite",
           "Tagging"
         ],
         "calculated_action_group": "Tagging",
         "condition_keys": [
           "aws:TagKeys"
         ],
-        "description": "Grants permission to untag a flow",
+        "description": "Grants permission to untag a flow or a connector",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appflow/1.0/APIReference/API_UntagResource.html"
         }
       },
       "UpdateConnectorProfile": {
@@ -7531,28 +7944,28 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to use a connector profile while creating a flow in Amazon AppFlow",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/appflow/1.0/APIReference/API_UseConnectorProfile.html"
+          "doc_page": "API_CreateFlow.html",
+          "doc_page_rel": "API_CreateFlow.html"
         }
       }
     },
     "arn_format": "arn:${Partition}:appflow:${Region}:${Account}:${ResourceType}/${ResourceName}",
     "arn_regex": "^arn:${Partition}:appflow:.+:.+:.+",
     "description": "Amazon AppFlow",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/appflow/1.0/APIReference/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/appflow/1.0/APIReference/Welcome.html",
-      "authz_doc_page": "https://docs.aws.amazon.com/appflow/latest/userguide/auth-and-access-control.html",
+      "authz_doc_page": "https://docs.aws.amazon.com/appflow/latest/userguide/security-iam.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/appflow/latest/userguide/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/appflow/latest/userguide/identity-access-management.html/"
     },
     "prefix": "appflow"
   },
   "AppIntegrations": {
     "actions": {
@@ -7855,14 +8268,29 @@
       "concepts_doc_root": "https://docs.aws.amazon.com/connect/latest/adminguide/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/connect/latest/adminguide/security_iam_service-with-iam.html"
     },
     "prefix": "app-integrations"
   },
   "AppStream 2.0": {
     "actions": {
+      "AssociateAppBlockBuilderAppBlock": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to associate the specified app block builder with the app block",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_AssociateAppBlockBuilderAppBlock.html"
+        }
+      },
       "AssociateApplicationFleet": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
@@ -7960,14 +8388,45 @@
         "description": "Grants permission to create an app block. App blocks store details about the virtual hard disk that contains the files for the application in an S3 bucket. It also stores the setup script with details about how to mount the virtual hard disk. App blocks are only supported for Elastic fleets",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_CreateAppBlock.html"
         }
       },
+      "CreateAppBlockBuilder": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create an app block builder. An app block builder is a virtual machine that is used to create an app block",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_CreateAppBlockBuilder.html"
+        }
+      },
+      "CreateAppBlockBuilderStreamingURL": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to create a URL to start an app block builder streaming session",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_CreateAppBlockBuilderStreamingURL.html"
+        }
+      },
       "CreateApplication": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
@@ -8139,14 +8598,29 @@
         "description": "Grants permission to delete the specified app block",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_DeleteAppBlock.html"
         }
       },
+      "DeleteAppBlockBuilder": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to delete the specified app block builder and release capacity",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_DeleteAppBlockBuilder.html"
+        }
+      },
       "DeleteApplication": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
@@ -8281,14 +8755,42 @@
         "description": "Grants permission to delete a user from the user pool",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_DeleteUser.html"
         }
       },
+      "DescribeAppBlockBuilderAppBlockAssociations": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve the associations that are associated with the specified app block builder or app block",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_DescribeAppBlockBuilderAppBlockAssociations.html"
+        }
+      },
+      "DescribeAppBlockBuilders": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve a list that describes one or more specified app block builders, if the app block builder names are provided. Otherwise, all app block builders in the account are described",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_DescribeAppBlockBuilders.html"
+        }
+      },
       "DescribeAppBlocks": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -8490,14 +8992,29 @@
         "description": "Grants permission to disable the specified user in the user pool. This action does not delete the user",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_DisableUser.html"
         }
       },
+      "DisassociateAppBlockBuilderAppBlock": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to disassociate the specified app block builder with the app block",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_DisassociateAppBlockBuilderAppBlock.html"
+        }
+      },
       "DisassociateApplicationFleet": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
@@ -8616,14 +9133,29 @@
         "description": "Grants permission to retrieve a list of all tags for the specified AppStream 2.0 resource. The following resources can be tagged: Image builders, images, fleets, and stacks",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_ListTagsForResource.html"
         }
       },
+      "StartAppBlockBuilder": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to start the specified app block builder",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_StartAppBlockBuilder.html"
+        }
+      },
       "StartFleet": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
@@ -8646,14 +9178,29 @@
         "description": "Grants permission to start the specified image builder",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_StartImageBuilder.html"
         }
       },
+      "StopAppBlockBuilder": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to stop the specified app block builder",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_StopAppBlockBuilder.html"
+        }
+      },
       "StopFleet": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
@@ -8725,14 +9272,29 @@
         "description": "Grants permission to disassociate one or more tags from the specified AppStream 2.0 resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_UntagResource.html"
         }
       },
+      "UpdateAppBlockBuilder": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to update a specific app block builder. An app block builder is a virtual machine that is used to create an app block",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appstream2/latest/APIReference/API_UpdateAppBlockBuilder.html"
+        }
+      },
       "UpdateApplication": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
@@ -10145,30 +10707,32 @@
       },
       "DeleteTags": {
         "aws_action_groups": [
           "Tagging",
           "ReadWrite"
         ],
         "calculated_action_group": "Tagging",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:TagKeys"
+        ],
         "description": "Grants permission to DeleteTags API. DeleteTags deletes the association between configuration items and one or more tags. This API accepts a list of multiple configuration items",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/application-discovery/latest/APIReference/API_DeleteTags.html"
         }
       },
       "DescribeAgents": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Grants permission to DescribeAgents API. DescribeAgents lists agents or the Connector by ID or lists all agents/Connectors associated with your user account if you did not specify an ID",
+        "description": "Grants permission to DescribeAgents API. DescribeAgents lists agents or the Connector by ID or lists all agents/Connectors associated with your user if you did not specify an ID",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/application-discovery/latest/APIReference/API_DescribeAgents.html"
         }
       },
       "DescribeConfigurations": {
@@ -10188,15 +10752,15 @@
       "DescribeContinuousExports": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Grants permission to DescribeContinuousExports API. DescribeContinuousExports lists exports as specified by ID. All continuous exports associated with your user account can be listed if you call DescribeContinuousExports as is without passing any parameters",
+        "description": "Grants permission to DescribeContinuousExports API. DescribeContinuousExports lists exports as specified by ID. All continuous exports associated with your user can be listed if you call DescribeContinuousExports as is without passing any parameters",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/application-discovery/latest/APIReference/API_DescribeContinuousExports.html"
         }
       },
       "DescribeExportConfigurations": {
@@ -10231,15 +10795,15 @@
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
-        "description": "Grants permission to DescribeImportTasks API. DescribeImportTasks returns an array of import tasks for your account, including status information, times, IDs, the Amazon S3 Object URL for the import file, and more",
+        "description": "Grants permission to DescribeImportTasks API. DescribeImportTasks returns an array of import tasks for your user, including status information, times, IDs, the Amazon S3 Object URL for the import file, and more",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/application-discovery/latest/APIReference/API_DescribeImportTasks.html"
         }
       },
       "DescribeTags": {
@@ -10436,15 +11000,15 @@
     "arn_regex": "",
     "description": "AWS Application Discovery Service",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/application-discovery/latest/APIReference/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/application-discovery/latest/APIReference/",
-      "authz_doc_page": "https://docs.aws.amazon.com/application-discovery/latest/userguide/before_you_install.html#appdisc-user-policy",
+      "authz_doc_page": "https://docs.aws.amazon.com/application-discovery/latest/userguide/security_iam_service-with-iam.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/application-discovery/latest/userguide/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/application-discovery/latest/userguide/"
     },
     "prefix": "discovery"
   },
   "Application Discovery Arsenal": {
     "actions": {
@@ -11960,14 +12524,28 @@
         "description": "Grants permission to get all the evidence from an evidence folder in AWS Audit Manager",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/audit-manager/latest/APIReference/API_GetEvidenceByEvidenceFolder.html"
         }
       },
+      "GetEvidenceFileUploadUrl": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get a presigned Amazon S3 URL that can be used to upload a file as manual evidence",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/audit-manager/latest/APIReference/API_GetEvidenceFileUploadUrl.html"
+        }
+      },
       "GetEvidenceFolder": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -13431,18 +14009,15 @@
         }
       },
       "StartBackupJob": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [
-          "aws:RequestTag/${TagKey}",
-          "aws:TagKeys"
-        ],
+        "condition_keys": [],
         "description": "Grants permission to start a new backup job",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/aws-backup/latest/devguide/API_StartBackupJob.html"
         }
       },
@@ -13532,34 +14107,28 @@
         }
       },
       "UpdateBackupPlan": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [
-          "aws:RequestTag/${TagKey}",
-          "aws:TagKeys"
-        ],
+        "condition_keys": [],
         "description": "Grants permission to update a backup plan",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/aws-backup/latest/devguide/API_UpdateBackupPlan.html"
         }
       },
       "UpdateFramework": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [
-          "aws:RequestTag/${TagKey}",
-          "aws:TagKeys"
-        ],
+        "condition_keys": [],
         "description": "Grants permission to update a framework",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/aws-backup/latest/devguide/API_UpdateFramework.html"
         }
       },
@@ -23206,14 +23775,27 @@
       "concepts_doc_root": "https://docs.aws.amazon.com/cloud9/latest/user-guide/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/IAM/latest/UserGuide/list_awscloud9.html#"
     },
     "prefix": "cloud9"
   },
   "CloudFormation": {
     "actions": {
+      "ActivateOrganizationsAccess": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to activate trusted access between StackSets and Organizations. With trusted access between StackSets and Organizations activated, the management account has permissions to create and manage StackSets for your organization",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/AWSCloudFormation/latest/APIReference/API_ActivateOrganizationsAccess.html"
+        }
+      },
       "ActivateType": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to activate a public third-party extension, making it available for use in stack templates",
@@ -23376,14 +23958,27 @@
         "description": "Grants permission to upload templates to Amazon S3 buckets. Used only by the AWS CloudFormation console and is not documented in the API reference",
         "docs": {
           "api_doc": "",
           "doc_page": "${DocHomeURL}AWSCloudFormation/latest/UserGuide/using-iam-template.html",
           "doc_page_rel": "https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-iam-template.html"
         }
       },
+      "DeactivateOrganizationsAccess": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to deactivate trusted access between StackSets and Organizations. If trusted access is deactivated, the management account does not have permissions to create and manage service-managed StackSets for your organization",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/AWSCloudFormation/latest/APIReference/API_DeactivateOrganizationsAccess.html"
+        }
+      },
       "DeactivateType": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to deactivate a public extension that was previously activated in this account and region",
@@ -23519,14 +24114,28 @@
         "description": "Grants permission to return the Hook invocation information for the specified change set",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AWSCloudFormation/latest/APIReference/API_DescribeChangeSetHooks.html"
         }
       },
+      "DescribeOrganizationsAccess": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to return information about the account's OrganizationAccess status",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/AWSCloudFormation/latest/APIReference/API_DescribeOrganizationsAccess.html"
+        }
+      },
       "DescribePublisher": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -23736,15 +24345,17 @@
       },
       "EstimateTemplateCost": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
-        "condition_keys": [],
+        "condition_keys": [
+          "cloudformation:TemplateUrl"
+        ],
         "description": "Grants permission to return the estimated monthly cost of a template",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AWSCloudFormation/latest/APIReference/API_EstimateTemplateCost.html"
         }
       },
@@ -23821,15 +24432,17 @@
       },
       "GetTemplateSummary": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
-        "condition_keys": [],
+        "condition_keys": [
+          "cloudformation:TemplateUrl"
+        ],
         "description": "Grants permission to return information about a new or existing template",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AWSCloudFormation/latest/APIReference/API_GetTemplateSummary.html"
         }
       },
@@ -23915,14 +24528,29 @@
         "description": "Grants permission to list resources in your account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/cloudcontrolapi/latest/APIReference/API_ListResources.html"
         }
       },
+      "ListStackInstanceResourceDrifts": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to return drift information for the resources that have been checked for drift in the specified stack instance",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/AWSCloudFormation/latest/APIReference/API_ListStackInstanceResourceDrifts.html"
+        }
+      },
       "ListStackInstances": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -24316,15 +24944,17 @@
       },
       "ValidateTemplate": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
-        "condition_keys": [],
+        "condition_keys": [
+          "cloudformation:TemplateUrl"
+        ],
         "description": "Grants permission to validate a specified template",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AWSCloudFormation/latest/APIReference/API_ValidateTemplate.html"
         }
       }
@@ -25734,27 +26364,14 @@
         "description": "Grants permission to update the configuration for a web distribution",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/cloudfront/latest/APIReference/API_UpdateDistribution.html"
         }
       },
-      "UpdateDistributionWithStagingConfig": {
-        "aws_action_groups": [
-          "ReadWrite"
-        ],
-        "calculated_action_group": "Write",
-        "condition_keys": [],
-        "description": "Grants permission to copy the staging distribution's configuration to its corresponding primary distribution",
-        "docs": {
-          "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/cloudfront/latest/APIReference/API_UpdateDistributionWithStagingConfig.html"
-        }
-      },
       "UpdateFieldLevelEncryptionConfig": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update a field-level encryption configuration",
@@ -29337,14 +29954,27 @@
         "description": "Grants permission to create a new log stream with the specified name",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_CreateLogStream.html"
         }
       },
+      "DeleteAccountPolicy": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a data protection policy attached to an account",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DeleteDataProtectionPolicy.html"
+        }
+      },
       "DeleteDataProtectionPolicy": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete a data protection policy attached to a log group",
@@ -29467,14 +30097,29 @@
         "description": "Grants permission to delete a subscription filter associated with the specified log group",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DeleteSubscriptionFilter.html"
         }
       },
+      "DescribeAccountPolicies": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve a data protection policy attached to an account",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DescribeAccountPolicies.html"
+        }
+      },
       "DescribeDestinations": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -29771,14 +30416,27 @@
         "description": "Grants permission to list the tags for the specified log group",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_ListTagsLogGroup.html"
         }
       },
+      "PutAccountPolicy": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to attach a data protection policy at account level to detect and redact sensitive information from log events",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_PutAccountPolicy.html"
+        }
+      },
       "PutDataProtectionPolicy": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to attach a data protection policy to detect and redact sensitive information from log events",
@@ -34962,16 +35620,19 @@
         }
       },
       "CreateScan": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
-        "description": "Grants permission to create CodeGuru Security scan",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create a CodeGuru Security scan",
         "docs": {
           "api_doc": "",
           "doc_page": "${APIReferenceDocPage}",
           "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
         }
       },
       "CreateUploadUrl": {
@@ -35025,21 +35686,37 @@
         "description": "Grants permission to retrieve findings for a scan generated by CodeGuru Security",
         "docs": {
           "api_doc": "",
           "doc_page": "${APIReferenceDocPage}",
           "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
         }
       },
-      "GetScan": {
+      "GetMetricsSummary": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
+        "description": "Grants permission to retrieve AWS accout level metrics summary generated by CodeGuru Security",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${APIReferenceDocPage}",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+        }
+      },
+      "GetScan": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to retrieve CodeGuru Security scan metadata",
         "docs": {
           "api_doc": "",
           "doc_page": "${APIReferenceDocPage}",
           "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
         }
       },
@@ -35054,14 +35731,29 @@
         "description": "Grants permission to retrieve findings generated by CodeGuru Security",
         "docs": {
           "api_doc": "",
           "doc_page": "${APIReferenceDocPage}",
           "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
         }
       },
+      "ListFindingsMetrics": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ListOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve a list of account level findings metrics within a date range",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${APIReferenceDocPage}",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+        }
+      },
       "ListScans": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite",
           "ListOnly"
         ],
         "calculated_action_group": "List",
@@ -35069,14 +35761,63 @@
         "description": "Grants permission to retrieve list of CodeGuru Security scan metadata",
         "docs": {
           "api_doc": "",
           "doc_page": "${APIReferenceDocPage}",
           "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
         }
       },
+      "ListTagsForResource": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to retrieve a list of tags for a scan name ARN",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${APIReferenceDocPage}",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+        }
+      },
+      "TagResource": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "Tagging"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to add tags to a scan name ARN",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${APIReferenceDocPage}",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+        }
+      },
+      "UntagResource": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "Tagging"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to remove tags from a scan name ARN",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${APIReferenceDocPage}",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+        }
+      },
       "UpdateAccountConfiguration": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update the account level configurations",
@@ -44472,14 +45213,48 @@
         "description": "Grants permission to search phone number resources in an Amazon Connect instance or traffic distribution group",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/connect/latest/APIReference/API_SearchAvailablePhoneNumbers.html"
         }
       },
+      "SearchHoursOfOperations": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "connect:InstanceId",
+          "connect:SearchTag/${TagKey}"
+        ],
+        "description": "Grants permission to search hours of operation resources in an Amazon Connect instance",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/connect/latest/APIReference/API_SearchHoursOfOperations.html"
+        }
+      },
+      "SearchPrompts": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "connect:InstanceId",
+          "connect:SearchTag/${TagKey}"
+        ],
+        "description": "Grants permission to search prompt resources in an Amazon Connect instance",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/connect/latest/APIReference/API_SearchPrompts.html"
+        }
+      },
       "SearchQueues": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [
@@ -44489,14 +45264,49 @@
         "description": "Grants permission to search queue resources in an Amazon Connect instance",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/connect/latest/APIReference/API_SearchQueues.html"
         }
       },
+      "SearchQuickConnects": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "connect:InstanceId",
+          "connect:SearchTag/${TagKey}"
+        ],
+        "description": "Grants permission to search quick connect resources in an Amazon Connect instance",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/connect/latest/APIReference/API_SearchQuickConnects.html"
+        }
+      },
+      "SearchResourceTags": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "connect:InstanceId"
+        ],
+        "description": "Grants permission to search tags used in an Amazon Connect instance",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/connect/latest/APIReference/API_SearchResourceTags.html"
+        }
+      },
       "SearchRoutingProfiles": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [
@@ -48280,28 +49090,56 @@
         "description": "Grants permission to describe the status of the connections that have been made between the replication instance and an endpoint",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_DescribeConnections.html"
         }
       },
+      "DescribeConversionConfiguration": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to return information about DMS Schema Conversion project configuration",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "DescribeDataMigrations": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to return information about database migrations for your account in the specified region",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
         }
       },
+      "DescribeDataProviders": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to list the AWS DMS attributes for a data providers. Note. This action should be added along with ListDataProviders, but does not currently authorize the described Schema Conversion operation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "Welcome.html",
+          "doc_page_rel": "Welcome.html"
+        }
+      },
       "DescribeEndpointSettings": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -48378,14 +49216,28 @@
         "description": "Grants permission to list events for a given source identifier and source type",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_DescribeEvents.html"
         }
       },
+      "DescribeExtensionPackAssociations": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to list the AWS DMS attributes for extension packs. Note. This action should be added along with ListExtensionPacks, but does not currently authorize the described Schema Conversion operation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "Welcome.html",
+          "doc_page_rel": "Welcome.html"
+        }
+      },
       "DescribeFleetAdvisorCollectors": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -48448,14 +49300,112 @@
         "description": "Grants permission to return a paginated list of schemas discovered by your Fleet Advisor collectors based on filter settings",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_DescribeFleetAdvisorSchemas.html"
         }
       },
+      "DescribeInstanceProfiles": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to list the AWS DMS attributes for a instance profiles. Note. This action should be added along with ListInstanceProfiles, but does not currently authorize the described Schema Conversion operation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "Welcome.html",
+          "doc_page_rel": "Welcome.html"
+        }
+      },
+      "DescribeMetadataModelAssessments": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to list the AWS DMS attributes for metadata model assessments. Note. This action should be added along with ListMetadataModelAssessments, but does not currently authorize the described Schema Conversion operation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "Welcome.html",
+          "doc_page_rel": "Welcome.html"
+        }
+      },
+      "DescribeMetadataModelConversions": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to list the AWS DMS attributes for a metadata model conversions. Note. This action should be added along with ListMetadataModelConversions, but does not currently authorize the described Schema Conversion operation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "Welcome.html",
+          "doc_page_rel": "Welcome.html"
+        }
+      },
+      "DescribeMetadataModelExportsAsScript": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to list the AWS DMS attributes for a metadata model exports. Note. This action should be added along with ListMetadataModelExports, but does not currently authorize the described Schema Conversion operation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "Welcome.html",
+          "doc_page_rel": "Welcome.html"
+        }
+      },
+      "DescribeMetadataModelExportsToTarget": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to list the AWS DMS attributes for a metadata model exports. Note. This action should be added along with ListMetadataModelExports, but does not currently authorize the described Schema Conversion operation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "Welcome.html",
+          "doc_page_rel": "Welcome.html"
+        }
+      },
+      "DescribeMetadataModelImports": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to return information about start metadata model import operations for a migration project",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
+      "DescribeMigrationProjects": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to list the AWS DMS attributes for a migration projects. Note. This action should be added along with ListMigrationProjects, but does not currently authorize the described Schema Conversion operation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "Welcome.html",
+          "doc_page_rel": "Welcome.html"
+        }
+      },
       "DescribeOrderableReplicationInstances": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -48871,27 +49821,53 @@
         "description": "Grants permission to list all tags for an AWS DMS resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_ListTagsForResource.html"
         }
       },
+      "ModifyConversionConfiguration": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update a conversion configuration. Note. This action should be added along with UpdateConversionConfiguration, but does not currently authorize the described Schema Conversion operation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "Welcome.html",
+          "doc_page_rel": "Welcome.html"
+        }
+      },
       "ModifyDataMigration": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to modify the specified database migration",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
         }
       },
+      "ModifyDataProvider": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to modify the specified data provider. Note. This action should be added along with UpdateDataProvider, but does not currently authorize the described Schema Conversion operation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "Welcome.html",
+          "doc_page_rel": "Welcome.html"
+        }
+      },
       "ModifyEndpoint": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to modify the specified endpoint",
@@ -48936,14 +49912,40 @@
         "description": "Grants permission to modify the status of the specified Fleet Advisor collector",
         "docs": {
           "api_doc": "",
           "doc_page": "${DocHomeURL}dms/latest/APIReference/Welcome.html",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
         }
       },
+      "ModifyInstanceProfile": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to modify the specified instance profile. Note. This action should be added along with UpdateInstanceProfile, but does not currently authorize the described Schema Conversion operation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "Welcome.html",
+          "doc_page_rel": "Welcome.html"
+        }
+      },
+      "ModifyMigrationProject": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to modify the specified migration project. Note. This action should be added along with UpdateMigrationProject, but does not currently authorize the described Schema Conversion operation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "Welcome.html",
+          "doc_page_rel": "Welcome.html"
+        }
+      },
       "ModifyReplicationConfig": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to modify the specified replication config",
@@ -49095,14 +50097,27 @@
         "description": "Grants permission to start the database migration",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
         }
       },
+      "StartExtensionPackAssociation": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to associate an extension pack. Note. This action should be added along with AssociateExtensionPack, but does not currently authorize the described Schema Conversion operation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "Welcome.html",
+          "doc_page_rel": "Welcome.html"
+        }
+      },
       "StartMetadataModelAssessment": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to start a new assessment of metadata model",
@@ -49121,14 +50136,27 @@
         "description": "Grants permission to start a new conversion of metadata model",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
         }
       },
+      "StartMetadataModelExportAsScript": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to start a new export of metadata model as script. Note. This action should be added along with StartMetadataModelExportAsScripts, but does not currently authorize the described Schema Conversion operation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "Welcome.html",
+          "doc_page_rel": "Welcome.html"
+        }
+      },
       "StartMetadataModelExportAsScripts": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to start a new export of metadata model as script",
@@ -49386,14 +50414,30 @@
         "description": "Grants permission to get associate failback client to recovery instance",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}drs-apis.html",
           "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/userguide/drs-apis.html"
         }
       },
+      "AssociateSourceNetworkStack": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to associate CloudFormation stack with source network",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/APIReference/API_AssociateSourceNetworkStack.html"
+        }
+      },
       "BatchCreateVolumeSnapshotGroupForDrs": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to batch create volume snapshot group",
@@ -49492,14 +50536,30 @@
         "description": "Grants permission to create replication configuration template",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/APIReference/API_CreateReplicationConfigurationTemplate.html"
         }
       },
+      "CreateSourceNetwork": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create a source network",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/APIReference/API_CreateSourceNetwork.html"
+        }
+      },
       "CreateSourceServerForDrs": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
@@ -49560,14 +50620,27 @@
         "description": "Grants permission to delete replication configuration template",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/APIReference/API_DeleteReplicationConfigurationTemplate.html"
         }
       },
+      "DeleteSourceNetwork": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete source network",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/APIReference/API_DeleteSourceNetwork.html"
+        }
+      },
       "DeleteSourceServer": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete source server",
@@ -49685,14 +50758,28 @@
         "description": "Grants permission to describe snapshot requests",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}drs-apis.html",
           "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/userguide/drs-apis.html"
         }
       },
+      "DescribeSourceNetworks": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to describe source networks",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/APIReference/API_DescribeSourceNetworks.html"
+        }
+      },
       "DescribeSourceServers": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -49725,14 +50812,30 @@
         "description": "Grants permission to disconnect source server",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/APIReference/API_DisconnectSourceServer.html"
         }
       },
+      "ExportSourceNetworkCfnTemplate": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to export CloudFormation template which contains source network resources",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/APIReference/API_ExportSourceNetworkCfnTemplate.html"
+        }
+      },
       "GetAgentCommandForDrs": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -50218,14 +51321,43 @@
         "description": "Grants permission to start replication",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/APIReference/API_StartReplication.html"
         }
       },
+      "StartSourceNetworkRecovery": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to start network recovery",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/APIReference/API_StartSourceNetworkRecovery.html"
+        }
+      },
+      "StartSourceNetworkReplication": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to start network replication",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/APIReference/API_StartSourceNetworkReplication.html"
+        }
+      },
       "StopFailback": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to stop failback",
@@ -50244,14 +51376,27 @@
         "description": "Grants permission to stop replication",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/APIReference/API_StopReplication.html"
         }
       },
+      "StopSourceNetworkReplication": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to stop network replication",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/drs/latest/APIReference/API_StopSourceNetworkReplication.html"
+        }
+      },
       "TagResource": {
         "aws_action_groups": [
           "Tagging",
           "ReadWrite"
         ],
         "calculated_action_group": "Tagging",
         "condition_keys": [
@@ -52835,14 +53980,29 @@
         "description": "Grants permission to update the name of an agent",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/datasync/latest/userguide/API_UpdateAgent.html"
         }
       },
+      "UpdateDiscoveryJob": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to update a discovery job",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/datasync/latest/userguide/API_UpdateDiscoveryJob.html"
+        }
+      },
       "UpdateLocationHdfs": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
@@ -61611,14 +62771,31 @@
         "description": "Grants permission to create an Amazon EBS-backed AMI from a stopped or running Amazon EBS-backed instance",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateImage.html"
         }
       },
+      "CreateInstanceConnectEndpoint": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys",
+          "ec2:Region"
+        ],
+        "description": "Grants permission to create an EC2 Instance Connect Endpoint that allows you to connect to an instance without a public IPv4 address",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateInstanceConnectEndpoint.html"
+        }
+      },
       "CreateInstanceEventWindow": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
@@ -62883,14 +64060,29 @@
         "description": "Grants permission to delete an Amazon FPGA Image (AFI)",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DeleteFpgaImage.html"
         }
       },
+      "DeleteInstanceConnectEndpoint": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "ec2:Region"
+        ],
+        "description": "Grants permission to delete an EC2 Instance Connect Endpoint",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DeleteInstanceConnectEndpoint.html"
+        }
+      },
       "DeleteInstanceEventWindow": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "ec2:Region"
@@ -64715,14 +65907,31 @@
         "description": "Grants permission to describe the attributes of an instance",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstanceAttribute.html"
         }
       },
+      "DescribeInstanceConnectEndpoints": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [
+          "ec2:Region"
+        ],
+        "description": "Grants permission to describe EC2 Instance Connect Endpoints",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstanceConnectEndpoints.html"
+        }
+      },
       "DescribeInstanceCreditSpecifications": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -71918,14 +73127,27 @@
       "concepts_doc_root": "https://docs.aws.amazon.com/imagebuilder/latest/userguide/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/imagebuilder/latest/userguide/"
     },
     "prefix": "imagebuilder"
   },
   "EC2 Instance Connect": {
     "actions": {
+      "OpenTunnel": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to establish SSH connection to an EC2 instance using EC2 Instance Connect Endpoint",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/ec2-instance-connect/latest/APIReference/API_OpenTunnel.html"
+        }
+      },
       "SendSSHPublicKey": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "ec2:osuser"
@@ -73239,15 +74461,18 @@
   "ELB v2": {
     "actions": {
       "AddListenerCertificates": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to add the specified certificates to the specified secure listener",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_AddListenerCertificates.html"
         }
       },
@@ -73255,97 +74480,116 @@
         "aws_action_groups": [
           "Tagging",
           "ReadWrite"
         ],
         "calculated_action_group": "Tagging",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
+          "aws:ResourceTag/${TagKey}",
           "aws:TagKeys",
-          "elasticloadbalancing:CreateAction"
+          "elasticloadbalancing:CreateAction",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
         ],
         "description": "Grants permission to add the specified tags to the specified load balancer. Each load balancer can have a maximum of 10 tags",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_AddTags.html"
         }
       },
       "ApplySecurityGroupsToLoadBalancer": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to associate one or more security groups with your load balancer in a virtual private cloud (VPC)",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_ApplySecurityGroupsToLoadBalancer.html"
         }
       },
       "AttachLoadBalancerToSubnets": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to add one or more subnets to the set of configured subnets for the specified load balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_AttachLoadBalancerToSubnets.html"
         }
       },
       "ConfigureHealthCheck": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to specify the health check settings to use when evaluating the health state of your back-end instances",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_ConfigureHealthCheck.html"
         }
       },
       "CreateAppCookieStickinessPolicy": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to generate a stickiness policy with sticky session lifetimes that follow that of an application-generated cookie",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_CreateAppCookieStickinessPolicy.html"
         }
       },
       "CreateLBCookieStickinessPolicy": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to generate a stickiness policy with sticky session lifetimes controlled by the lifetime of the browser (user-agent) or a specified expiration period",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_CreateLBCookieStickinessPolicy.html"
         }
       },
       "CreateListener": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
-          "aws:TagKeys"
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
         ],
         "description": "Grants permission to create a listener for the specified Application Load Balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_CreateListener.html"
         }
@@ -73353,57 +74597,67 @@
       "CreateLoadBalancer": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
-          "aws:TagKeys"
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
         ],
         "description": "Grants permission to create a load balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_CreateLoadBalancer.html"
         }
       },
       "CreateLoadBalancerListeners": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to create one or more listeners for the specified load balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_CreateLoadBalancerListeners.html"
         }
       },
       "CreateLoadBalancerPolicy": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to create a policy with the specified attributes for the specified load balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_CreateLoadBalancerPolicy.html"
         }
       },
       "CreateRule": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
-          "aws:TagKeys"
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
         ],
         "description": "Grants permission to create a rule for the specified listener",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_CreateRule.html"
         }
@@ -73411,120 +74665,146 @@
       "CreateTargetGroup": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
-          "aws:TagKeys"
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
         ],
         "description": "Grants permission to create a target group",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_CreateTargetGroup.html"
         }
       },
       "DeleteListener": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to delete the specified listener",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_DeleteListener.html"
         }
       },
       "DeleteLoadBalancer": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to delete the specified load balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_DeleteLoadBalancer.html"
         }
       },
       "DeleteLoadBalancerListeners": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to delete the specified listeners from the specified load balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_DeleteLoadBalancerListeners.html"
         }
       },
       "DeleteLoadBalancerPolicy": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to delete the specified policy from the specified load balancer. This policy must not be enabled for any listeners",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_DeleteLoadBalancerPolicy.html"
         }
       },
       "DeleteRule": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to delete the specified rule",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_DeleteRule.html"
         }
       },
       "DeleteTargetGroup": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to delete the specified target group",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_DeleteTargetGroup.html"
         }
       },
       "DeregisterInstancesFromLoadBalancer": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to deregister the specified instances from the specified load balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_DeregisterInstancesFromLoadBalancer.html"
         }
       },
       "DeregisterTargets": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to deregister the specified targets from the specified target group",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_DeregisterTargets.html"
         }
       },
@@ -73726,145 +75006,178 @@
         }
       },
       "DetachLoadBalancerFromSubnets": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to remove the specified subnets from the set of configured subnets for the load balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_DetachLoadBalancerFromSubnets.html"
         }
       },
       "DisableAvailabilityZonesForLoadBalancer": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to remove the specified Availability Zones from the set of Availability Zones for the specified load balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_DisableAvailabilityZonesForLoadBalancer.html"
         }
       },
       "EnableAvailabilityZonesForLoadBalancer": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to add the specified Availability Zones to the set of Availability Zones for the specified load balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_EnableAvailabilityZonesForLoadBalancer.html"
         }
       },
       "ModifyListener": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to modify the specified properties of the specified listener",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_ModifyListener.html"
         }
       },
       "ModifyLoadBalancerAttributes": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to modify the attributes of the specified load balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_ModifyLoadBalancerAttributes.html"
         }
       },
       "ModifyRule": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to modify the specified rule",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_ModifyRule.html"
         }
       },
       "ModifyTargetGroup": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to modify the health checks used when evaluating the health state of the targets in the specified target group",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_ModifyTargetGroup.html"
         }
       },
       "ModifyTargetGroupAttributes": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to modify the specified attributes of the specified target group",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_ModifyTargetGroupAttributes.html"
         }
       },
       "RegisterInstancesWithLoadBalancer": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to add the specified instances to the specified load balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_RegisterInstancesWithLoadBalancer.html"
         }
       },
       "RegisterTargets": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to register the specified targets with the specified target group",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_RegisterTargets.html"
         }
       },
       "RemoveListenerCertificates": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to remove the specified certificates of the specified secure listener",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_RemoveListenerCertificates.html"
         }
       },
@@ -73872,68 +75185,82 @@
         "aws_action_groups": [
           "Tagging",
           "ReadWrite"
         ],
         "calculated_action_group": "Tagging",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
-          "aws:TagKeys"
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
         ],
         "description": "Grants permission to remove one or more tags from the specified load balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_RemoveTags.html"
         }
       },
       "SetIpAddressType": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to set the type of IP addresses used by the subnets of the specified load balancer",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_SetIpAddressType.html"
         }
       },
       "SetLoadBalancerListenerSSLCertificate": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to set the certificate that terminates the specified listener's SSL connections",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_SetLoadBalancerListenerSSLCertificate.html"
         }
       },
       "SetLoadBalancerPoliciesForBackendServer": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to replace the set of policies associated with the specified port on which the back-end server is listening with a new set of policies",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_SetLoadBalancerPoliciesForBackendServer.html"
         }
       },
       "SetLoadBalancerPoliciesOfListener": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to replace the current set of policies for the specified load balancer port with the specified set of policies",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/2012-06-01/APIReference/API_SetLoadBalancerPoliciesOfListener.html"
         }
       },
@@ -73951,28 +75278,34 @@
         }
       },
       "SetSecurityGroups": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to associate the specified security groups with the specified load balancer ",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_SetSecurityGroups.html"
         }
       },
       "SetSubnets": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "elasticloadbalancing:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to enable the Availability Zone for the specified subnets for the specified load balancer ",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_SetSubnets.html"
         }
       },
@@ -73988,15 +75321,15 @@
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_SetWebAcl.html"
         }
       }
     },
     "arn_format": "arn:${Partition}:elasticloadbalancing:${Region}:${Account}:${ResourceType}/${ResourceId}",
     "arn_regex": "^arn:${Partition}:elasticloadbalancing:.+",
-    "description": "Elastic Load Balancing V2",
+    "description": "AWS Elastic Load Balancing V2",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/",
       "authz_doc_page": "https://docs.aws.amazon.com/elasticloadbalancing/latest/userguide/load-balancer-authentication-access-control.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/elasticloadbalancing/latest/userguide/",
@@ -74717,14 +76050,29 @@
         "description": "Grants permission to list summary information about EMR Studios",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}emr-studio.html",
           "doc_page_rel": "https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-studio.html"
         }
       },
+      "ListSupportedInstanceTypes": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list the Amazon EC2 instance types that an Amazon EMR release supports",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/emr/latest/APIReference/API_ListSupportedInstanceTypes.html"
+        }
+      },
       "ListWorkspaceAccessIdentities": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -95981,15 +97329,15 @@
       },
       "ChangePassword": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission for an IAM user to change their own password",
+        "description": "Grants permission to an IAM user to change their own password",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/IAM/latest/APIReference/API_ChangePassword.html"
         }
       },
       "CreateAccessKey": {
@@ -96580,15 +97928,20 @@
         }
       },
       "EnableMFADevice": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "iam:FIDO-FIPS-140-2-certification",
+          "iam:FIDO-FIPS-140-3-certification",
+          "iam:FIDO-certification",
+          "iam:RegisterSecurityKey"
+        ],
         "description": "Grants permission to enable an MFA device and associate it with the specified IAM user",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/IAM/latest/APIReference/API_EnableMFADevice.html"
         }
       },
@@ -96830,14 +98183,28 @@
         "description": "Grants permission to retrieve the user name and password creation date for the specified IAM user",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/IAM/latest/APIReference/API_GetLoginProfile.html"
         }
       },
+      "GetMFADevice": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve information about an MFA device for the specified user",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/IAM/latest/APIReference/API_GetMFADevice.html"
+        }
+      },
       "GetOpenIDConnectProvider": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -98330,15 +99697,15 @@
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/IAM/latest/APIReference/API_UploadSigningCertificate.html"
         }
       }
     },
     "arn_format": "arn:${Partition}:iam::${Account}:${ResourceType}/${ResourceName}",
     "arn_regex": "^arn:${Partition}:iam::.+",
-    "description": "AWS Identity and Access Management",
+    "description": "AWS Identity and Access Management (IAM)",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/IAM/latest/APIReference/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/IAM/latest/APIReference/",
       "authz_doc_page": "https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/IAM/latest/UserGuide/",
@@ -100970,28 +102337,54 @@
         "description": "Grants permission to delete an existing attachment",
         "docs": {
           "api_doc": "",
           "doc_page": "https://aws.amazon.com/iq/",
           "doc_page_rel": "https://aws.amazon.com/iq/"
         }
       },
+      "DisableIndividualPublicProfile": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to disable individual public profile page",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "https://aws.amazon.com/iq/",
+          "doc_page_rel": "https://aws.amazon.com/iq/"
+        }
+      },
       "DownloadAttachment": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to download existing attachment",
         "docs": {
           "api_doc": "",
           "doc_page": "https://aws.amazon.com/iq/",
           "doc_page_rel": "https://aws.amazon.com/iq/"
         }
       },
+      "EnableIndividualPublicProfile": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to enable individual public profile page",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "https://aws.amazon.com/iq/",
+          "doc_page_rel": "https://aws.amazon.com/iq/"
+        }
+      },
       "EndCall": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to end a voice/video call",
@@ -101067,14 +102460,28 @@
         "description": "Grants permission to request a websocket token for the conversation notifications",
         "docs": {
           "api_doc": "",
           "doc_page": "https://aws.amazon.com/iq/",
           "doc_page_rel": "https://aws.amazon.com/iq/"
         }
       },
+      "GetCompanyChatMessages": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to read chat messages in a company conversation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "https://aws.amazon.com/iq/",
+          "doc_page_rel": "https://aws.amazon.com/iq/"
+        }
+      },
       "GetCompanyProfile": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -101219,14 +102626,27 @@
         "description": "Grants permission to start a voice/video call",
         "docs": {
           "api_doc": "",
           "doc_page": "https://aws.amazon.com/iq/",
           "doc_page_rel": "https://aws.amazon.com/iq/"
         }
       },
+      "LinkAwsCertification": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to link an AWS certification to individual profile",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "https://aws.amazon.com/iq/",
+          "doc_page_rel": "https://aws.amazon.com/iq/"
+        }
+      },
       "ListAttachments": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -101248,14 +102668,28 @@
         "description": "Grants permission to list existing conversations",
         "docs": {
           "api_doc": "",
           "doc_page": "https://aws.amazon.com/iq/",
           "doc_page_rel": "https://aws.amazon.com/iq/"
         }
       },
+      "ListExpertAccessLogs": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to list access logs of expert activity",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "https://aws.amazon.com/iq/",
+          "doc_page_rel": "https://aws.amazon.com/iq/"
+        }
+      },
       "ListListings": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -101396,14 +102830,27 @@
         "description": "Grants permission to unarchive a conversation",
         "docs": {
           "api_doc": "",
           "doc_page": "https://aws.amazon.com/iq/",
           "doc_page_rel": "https://aws.amazon.com/iq/"
         }
       },
+      "UnlinkAwsCertification": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to unlink an AWS certification from individual profile",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "https://aws.amazon.com/iq/",
+          "doc_page_rel": "https://aws.amazon.com/iq/"
+        }
+      },
       "UpdateCompanyProfile": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update a company profile",
@@ -103896,14 +105343,27 @@
         "description": "Grants permission to cancel the generation of a findings report",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/inspector/v2/APIReference/API_CancelFindingsReport.html"
         }
       },
+      "CancelSbomExport": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to cancel the generation of an SBOM report",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/inspector/v2/APIReference/API_CancelSbomExport.html"
+        }
+      },
       "CreateFilter": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
@@ -103925,14 +105385,27 @@
         "description": "Grants permission to request the generation of a findings report",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/inspector/v2/APIReference/API_CreateFindingsReport.html"
         }
       },
+      "CreateSbomExport": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to request the generation of an SBOM report",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/inspector/v2/APIReference/API_CreateSbomExport.html"
+        }
+      },
       "DeleteFilter": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete a findings filter",
@@ -104059,14 +105532,28 @@
         "description": "Grants permission to retrieve ec2 deep inspection configuration for standalone accounts, delegated administrator and member account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/inspector/v2/APIReference/API_GetEc2DeepInspectionConfiguration.html"
         }
       },
+      "GetEncryptionKey": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "ReadOnly"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve information about the KMS key used to encrypt code snippets with",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/inspector/v2/APIReference/API_GetEncryptionKey.html"
+        }
+      },
       "GetFindingsReportStatus": {
         "aws_action_groups": [
           "ReadWrite",
           "ReadOnly"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -104087,14 +105574,28 @@
         "description": "Grants permission to retrieve information about an account that's associated with an Amazon Inspector administrator account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/inspector/v2/APIReference/API_GetMember.html"
         }
       },
+      "GetSbomExport": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "ReadOnly"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve a requested SBOM report",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/inspector/v2/APIReference/API_GetSbomExport.html"
+        }
+      },
       "ListAccountPermissions": {
         "aws_action_groups": [
           "ReadWrite",
           "ReadOnly",
           "ListOnly"
         ],
         "calculated_action_group": "List",
@@ -104236,14 +105737,27 @@
         "description": "Grants permission to retrieve aggregated usage data for an account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/inspector/v2/APIReference/API_ListUsageTotals.html"
         }
       },
+      "ResetEncryptionKey": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to let a customer reset to use an Amazon-owned KMS key to encrypt code snippets with",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/inspector/v2/APIReference/API_ResetEncryptionKey.html"
+        }
+      },
       "SearchVulnerabilities": {
         "aws_action_groups": [
           "ReadWrite",
           "ReadOnly"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -104310,14 +105824,27 @@
         "description": "Grants permission to update ec2 deep inspection configuration by delegated administrator, member and standalone account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/inspector/v2/APIReference/API_UpdateEc2DeepInspectionConfiguration.html"
         }
       },
+      "UpdateEncryptionKey": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to let a customer use a KMS key to encrypt code snippets with",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/inspector/v2/APIReference/API_UpdateEncryptionKey.html"
+        }
+      },
       "UpdateFilter": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
@@ -104569,14 +106096,28 @@
         "description": "Grants permission to get the channel configuration for a specified channel ARN",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/ivs/latest/APIReference/API_GetChannel.html"
         }
       },
+      "GetParticipant": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get participant information for a specified stage ARN, session, and participant",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/ivs/latest/RealTimeAPIReference/API_GetParticipant.html"
+        }
+      },
       "GetPlaybackKeyPair": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -104611,14 +106152,28 @@
         "description": "Grants permission to get stage information for a specified ARN",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/ivs/latest/RealTimeAPIReference/API_GetStage.html"
         }
       },
+      "GetStageSession": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get stage session information for a specified stage ARN and session",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/ivs/latest/RealTimeAPIReference/API_GetStageSession.html"
+        }
+      },
       "GetStream": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -104684,14 +106239,44 @@
         "description": "Grants permission to get summary information about channels",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/ivs/latest/APIReference/API_ListChannels.html"
         }
       },
+      "ListParticipantEvents": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list participant events for a specified stage ARN, session, and participant",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/ivs/latest/RealTimeAPIReference/API_ListParticipantEvents.html"
+        }
+      },
+      "ListParticipants": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list participants for a specified stage ARN and session",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/ivs/latest/RealTimeAPIReference/API_ListParticipants.html"
+        }
+      },
       "ListPlaybackKeyPairs": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -104714,14 +106299,29 @@
         "description": "Grants permission to get summary information about recording configurations",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/ivs/latest/APIReference/API_ListRecordingConfigurations.html"
         }
       },
+      "ListStageSessions": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list stage sessions for a specified stage ARN",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/ivs/latest/RealTimeAPIReference/API_ListStageSessions.html"
+        }
+      },
       "ListStages": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -119346,14 +120946,30 @@
         "description": "Grants permission to query documents and faqs",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/kendra/latest/dg/API_Query.html"
         }
       },
+      "Retrieve": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "ReadOnly"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to retrieve relevant content from an index",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/kendra/latest/dg/API_Retrieve.html"
+        }
+      },
       "StartDataSourceSyncJob": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
@@ -120912,14 +122528,27 @@
         "description": "Grants permission to create a Kinesis video stream",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/kinesisvideostreams/latest/dg/API_CreateStream.html"
         }
       },
+      "DeleteEdgeConfiguration": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete the edge configuration of your Kinesis Video Stream",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/kinesisvideostreams/latest/dg/API_DeleteEdgeConfiguration.html"
+        }
+      },
       "DeleteSignalingChannel": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete an existing signaling channel",
@@ -121178,14 +122807,29 @@
         "description": "Grants permission to join a storage session for a channel",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/kinesisvideostreams/latest/dg/API_AWSAcuityRoutingServiceLambda_JoinStorageSession.html"
         }
       },
+      "ListEdgeAgentConfigurations": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list an edge agent configurations",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/kinesisvideostreams/latest/dg/API_ListEdgeAgentConfigurations.html"
+        }
+      },
       "ListFragments": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -123377,54 +125021,54 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create new items in an existing custom vocabulary",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_BatchCreateCustomVocabularyItem.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_BatchCreateCustomVocabularyItem.html"
         }
       },
       "BatchDeleteCustomVocabularyItem": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete existing items in an existing custom vocabulary",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_BatchDeleteCustomVocabularyItem.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_BatchDeleteCustomVocabularyItem.html"
         }
       },
       "BatchUpdateCustomVocabularyItem": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update existing items in an existing custom vocabulary",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_BatchUpdateCustomVocabularyItem.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_BatchUpdateCustomVocabularyItem.html"
         }
       },
       "BuildBotLocale": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to build an existing bot locale in a bot",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_BuildBotLocale.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_BuildBotLocale.html"
         }
       },
       "CreateBot": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -123432,15 +125076,15 @@
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
         "description": "Grants permission to create a new bot and a test bot alias pointing to the DRAFT bot version",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_CreateBot.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_CreateBot.html"
         }
       },
       "CreateBotAlias": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -123448,41 +125092,41 @@
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
         "description": "Grants permission to create a new bot alias in a bot",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_CreateBotAlias.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_CreateBotAlias.html"
         }
       },
       "CreateBotChannel": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create a bot channel in an existing bot",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
+          "doc_page": "${ConceptsDocRoot}deploying-messaging-platform.html",
           "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/deploying-messaging-platform.html"
         }
       },
       "CreateBotLocale": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create a new bot locale in an existing bot",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_CreateBotLocale.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_CreateBotLocale.html"
         }
       },
       "CreateBotVersion": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -123499,42 +125143,42 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create a new custom vocabulary in an existing bot locale",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
+          "doc_page": "${ConceptsDocRoot}vocab.html",
           "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/vocab.html"
         }
       },
       "CreateExport": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create an export for an existing resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_CreateExport.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_CreateExport.html"
         }
       },
       "CreateIntent": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create a new intent in an existing bot locale",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_CreateIntent.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_CreateIntent.html"
         }
       },
       "CreateIntentVersion": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -123552,41 +125196,41 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create a new resource policy for a Lex resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_CreateResourcePolicy.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_CreateResourcePolicy.html"
         }
       },
       "CreateSlot": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create a new slot in an intent",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_CreateSlot.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_CreateSlot.html"
         }
       },
       "CreateSlotType": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create a new slot type in an existing bot locale",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_CreateSlotType.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_CreateSlotType.html"
         }
       },
       "CreateSlotTypeVersion": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -123594,25 +125238,51 @@
         "description": "Creates a new version based on the $LATEST version of the specified slot type",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/lex/latest/dg/API_CreateSlotTypeVersion.html"
         }
       },
+      "CreateTestSet": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to import a new test-set",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${ConceptsDocRoot}create-test-set-from-CSV.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/create-test-set-from-CSV.html"
+        }
+      },
+      "CreateTestSetDiscrepancyReport": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to create a test set discrepancy report",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_CreateTestSetDiscrepancyReport.html"
+        }
+      },
       "CreateUploadUrl": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create an upload url for import file",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_CreateUploadUrl.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_CreateUploadUrl.html"
         }
       },
       "DeleteBot": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -123642,15 +125312,15 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete an existing bot channel",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
+          "doc_page": "${ConceptsDocRoot}deploying-messaging-platform.html",
           "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/deploying-messaging-platform.html"
         }
       },
       "DeleteBotChannelAssociation": {
         "aws_action_groups": [
           "ReadWrite"
         ],
@@ -123671,15 +125341,15 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete an existing bot locale in a bot",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DeleteBotLocale.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DeleteBotLocale.html"
         }
       },
       "DeleteBotVersion": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -123697,41 +125367,41 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete an existing custom vocabulary in a bot locale",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DeleteCustomVocabulary.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DeleteCustomVocabulary.html"
         }
       },
       "DeleteExport": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete an existing export",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DeleteExport.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DeleteExport.html"
         }
       },
       "DeleteImport": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete an existing import",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DeleteImport.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DeleteImport.html"
         }
       },
       "DeleteIntent": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -123762,15 +125432,15 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete an existing resource policy for a Lex resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DeleteResourcePolicy.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DeleteResourcePolicy.html"
         }
       },
       "DeleteSession": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -123788,15 +125458,15 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete an existing slot in an intent",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DeleteSlot.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DeleteSlot.html"
         }
       },
       "DeleteSlotType": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -123817,14 +125487,27 @@
         "description": "Deletes a specific version of a slot type",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/lex/latest/dg/API_DeleteSlotTypeVersion.html"
         }
       },
+      "DeleteTestSet": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete an existing test set",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DeleteTestSet.html"
+        }
+      },
       "DeleteUtterances": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Deletes the information Amazon Lex maintains for utterances on a specific bot and userId",
@@ -123841,197 +125524,253 @@
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve an existing bot",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DescribeBot.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeBot.html"
         }
       },
       "DescribeBotAlias": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve an existing bot alias",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DescribeBotAlias.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeBotAlias.html"
         }
       },
       "DescribeBotChannel": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve an existing bot channel",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
+          "doc_page": "${ConceptsDocRoot}deploying-messaging-platform.html",
           "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/deploying-messaging-platform.html"
         }
       },
       "DescribeBotLocale": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve an existing bot locale",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DescribeBotLocale.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeBotLocale.html"
         }
       },
       "DescribeBotRecommendation": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve metadata information about a bot recommendation",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DescribeBotRecommendation.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeBotRecommendation.html"
         }
       },
       "DescribeBotVersion": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve an existing bot version",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DescribeBotVersion.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeBotVersion.html"
         }
       },
       "DescribeCustomVocabulary": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve an existing custom vocabulary",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
+          "doc_page": "${ConceptsDocRoot}vocab.html",
           "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/vocab.html"
         }
       },
       "DescribeCustomVocabularyMetadata": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve metadata of an existing custom vocabulary",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DescribeCustomVocabularyMetadata.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeCustomVocabularyMetadata.html"
         }
       },
       "DescribeExport": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve an existing export",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DescribeExport.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeExport.html"
         }
       },
       "DescribeImport": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve an existing import",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DescribeImport.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeImport.html"
         }
       },
       "DescribeIntent": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve an existing intent",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DescribeIntent.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeIntent.html"
         }
       },
       "DescribeResourcePolicy": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve an existing resource policy for a Lex resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DescribeResourcePolicy.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeResourcePolicy.html"
         }
       },
       "DescribeSlot": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve an existing slot",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DescribeSlot.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeSlot.html"
         }
       },
       "DescribeSlotType": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve an existing slot type",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_DescribeSlotType.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeSlotType.html"
+        }
+      },
+      "DescribeTestExecution": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve test execution metadata",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeTestExecution.html"
+        }
+      },
+      "DescribeTestSet": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve an existing test set",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeTestSet.html"
+        }
+      },
+      "DescribeTestSetDiscrepancyReport": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve test set discrepancy report metadata",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeTestSetDiscrepancyReport.html"
+        }
+      },
+      "DescribeTestSetGeneration": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve test set generation metadata",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_DescribeTestSetGeneration.html"
         }
       },
       "GetBot": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
@@ -124331,14 +126070,28 @@
         "description": "Returns information for the $LATEST version of all slot types, subject to filters provided by the client",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/lex/latest/dg/API_GetSlotTypes.html"
         }
       },
+      "GetTestExecutionArtifactsUrl": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve artifacts URL for a test execution",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_GetTestExecutionArtifactsUrl.html"
+        }
+      },
       "GetUtterancesView": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -124358,44 +126111,44 @@
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list utterances and statistics for a bot",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListAggregatedUtterances.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListAggregatedUtterances.html"
         }
       },
       "ListBotAliases": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list bot aliases in an bot",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListBotAliases.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListBotAliases.html"
         }
       },
       "ListBotChannels": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list bot channels",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
+          "doc_page": "${ConceptsDocRoot}deploying-messaging-platform.html",
           "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/deploying-messaging-platform.html"
         }
       },
       "ListBotLocales": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
@@ -124403,195 +126156,195 @@
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list bot locales in a bot",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListBotLocales.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListBotLocales.html"
         }
       },
       "ListBotRecommendations": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to get a list of bot recommendations that meet the specified criteria",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListBotRecommendations.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListBotRecommendations.html"
         }
       },
       "ListBotVersions": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list existing bot versions",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListBotVersions.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListBotVersions.html"
         }
       },
       "ListBots": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list existing bots",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListBots.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListBots.html"
         }
       },
       "ListBuiltInIntents": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list built-in intents",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListBuiltInIntents.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListBuiltInIntents.html"
         }
       },
       "ListBuiltInSlotTypes": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list built-in slot types",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListBuiltInSlotTypes.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListBuiltInSlotTypes.html"
         }
       },
       "ListCustomVocabularyItems": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list items of an existing custom vocabulary",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListCustomVocabularyItems.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListCustomVocabularyItems.html"
         }
       },
       "ListExports": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list existing exports",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListExports.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListExports.html"
         }
       },
       "ListImports": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list existing imports",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListImports.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListImports.html"
         }
       },
       "ListIntents": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list intents in a bot",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListIntents.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListIntents.html"
         }
       },
       "ListRecommendedIntents": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to get a list of recommended intents provided by the bot recommendation",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListRecommendedIntents.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListRecommendedIntents.html"
         }
       },
       "ListSlotTypes": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list slot types in a bot",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListSlotTypes.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListSlotTypes.html"
         }
       },
       "ListSlots": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list slots in an intent",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_ListSlots.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListSlots.html"
         }
       },
       "ListTagsForResource": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
@@ -124600,14 +126353,72 @@
         "description": "Lists tags for a Lex resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/lex/latest/dg/API_ListTagsForResource.html"
         }
       },
+      "ListTestExecutionResultItems": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve test results data for a test execution",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListTestExecutionResultItems.html"
+        }
+      },
+      "ListTestExecutions": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list test executions",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListTestExecutions.html"
+        }
+      },
+      "ListTestSetRecords": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve records inside an existing test set",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListTestSetRecords.html"
+        }
+      },
+      "ListTestSets": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list test sets",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_ListTestSets.html"
+        }
+      },
       "PostContent": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Sends user input (text or speech) to Amazon Lex",
@@ -124710,69 +126521,69 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to send user input (text-only) to an bot alias",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_runtime_RecognizeText.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_runtime_RecognizeText.html"
         }
       },
       "RecognizeUtterance": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to send user input (text or speech) to an bot alias",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_runtime_RecognizeUtterance.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_runtime_RecognizeUtterance.html"
         }
       },
       "SearchAssociatedTranscripts": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to search for associated transcripts that meet the specified criteria",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_SearchAssociatedTranscripts.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_SearchAssociatedTranscripts.html"
         }
       },
       "StartBotRecommendation": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to start a bot recommendation for an existing bot locale",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_StartBotRecommendation.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_StartBotRecommendation.html"
         }
       },
       "StartConversation": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to stream user input (speech/text/DTMF) to a bot alias",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_runtime_StartConversation.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_runtime_StartConversation.html"
         }
       },
       "StartImport": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -124793,25 +126604,51 @@
         "description": "Grants permission to migrate a bot from Amazon Lex v1 to Amazon Lex v2",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/lex/latest/dg/API_StartMigration.html"
         }
       },
+      "StartTestExecution": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to start a test execution using a test set",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_StartTestExecution.html"
+        }
+      },
+      "StartTestSetGeneration": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to generate a test set",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_StartTestSetGeneration.html"
+        }
+      },
       "StopBotRecommendation": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to stop a bot recommendation for an existing bot locale",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_StopBotRecommendation.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_StopBotRecommendation.html"
         }
       },
       "TagResource": {
         "aws_action_groups": [
           "ReadWrite",
           "Tagging"
         ],
@@ -124850,143 +126687,156 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update an existing bot",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_UpdateBot.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_UpdateBot.html"
         }
       },
       "UpdateBotAlias": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update an existing bot alias",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_UpdateBotAlias.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_UpdateBotAlias.html"
         }
       },
       "UpdateBotLocale": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update an existing bot locale",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_UpdateBotLocale.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_UpdateBotLocale.html"
         }
       },
       "UpdateBotRecommendation": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update an existing bot recommendation request",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_UpdateBotRecommendation.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_UpdateBotRecommendation.html"
         }
       },
       "UpdateCustomVocabulary": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update an existing custom vocabulary",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
+          "doc_page": "${ConceptsDocRoot}vocab.html",
           "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/vocab.html"
         }
       },
       "UpdateExport": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update an existing export",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_UpdateExport.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_UpdateExport.html"
         }
       },
       "UpdateIntent": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update an existing intent",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_UpdateIntent.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_UpdateIntent.html"
         }
       },
       "UpdateResourcePolicy": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update an existing resource policy for a Lex resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_UpdateResourcePolicy.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_UpdateResourcePolicy.html"
         }
       },
       "UpdateSlot": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update an existing slot",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_UpdateSlot.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_UpdateSlot.html"
         }
       },
       "UpdateSlotType": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update an existing slot type",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/dg/API_UpdateSlotType.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_UpdateSlotType.html"
+        }
+      },
+      "UpdateTestSet": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update an existing test set",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/lexv2/latest/APIReference/API_UpdateTestSet.html"
         }
       }
     },
     "arn_format": "arn:${Partition}:lex:${Region}:${Account}:${ResourceType}/${ResourceId}",
     "arn_regex": "^arn:${Partition}:lex:.+:[0-9]+:.+",
     "description": "Amazon Lex V2",
     "docs": {
-      "actions_doc_root": "https://docs.aws.amazon.com/lexv2/latest/dg/",
+      "actions_doc_root": "https://docs.aws.amazon.com/lexv2/latest/APIReference/",
       "api_detail_root": "",
       "api_doc_root": "",
-      "api_reference_doc_page": "https://docs.aws.amazon.com/lexv2/latest/dg/API_Reference.html",
+      "api_reference_doc_page": "https://docs.aws.amazon.com/lexv2/latest/APIReference/welcome.html",
       "authz_doc_page": "https://docs.aws.amazon.com/lexv2/latest/dg/security-iam.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/lexv2/latest/dg/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/lexv2/latest/dg/"
     },
     "prefix": "lex"
   },
   "License Manager": {
@@ -131003,14 +132853,29 @@
         "description": "Grants permission to list the import tasks",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/mgn/latest/APIReference/API_ListImports.html"
         }
       },
+      "ListManagedAccounts": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list managed accounts",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mgn/latest/APIReference/API_ListManagedAccounts.html"
+        }
+      },
       "ListSourceServerActions": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -131140,14 +133005,27 @@
         "description": "Grants permission to notify vcenter client started",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}mgn-apis.html",
           "doc_page_rel": "https://docs.aws.amazon.com/mgn/latest/ug/mgn-apis.html"
         }
       },
+      "PauseReplication": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to pause replication",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mgn/latest/APIReference/API_PauseReplication.html"
+        }
+      },
       "PutSourceServerAction": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to put source server action document",
@@ -131208,14 +133086,27 @@
         "description": "Grants permission to remove launch configuration template action document",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/mgn/latest/APIReference/API_RemoveTemplateAction.html"
         }
       },
+      "ResumeReplication": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to resume replication",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mgn/latest/APIReference/API_ResumeReplication.html"
+        }
+      },
       "RetryDataReplication": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to retry replication",
@@ -131396,14 +133287,27 @@
         "description": "Grants permission to start test",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/mgn/latest/APIReference/API_StartTest.html"
         }
       },
+      "StopReplication": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to stop replication",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/mgn/latest/APIReference/API_StopReplication.html"
+        }
+      },
       "TagResource": {
         "aws_action_groups": [
           "Tagging",
           "ReadWrite"
         ],
         "calculated_action_group": "Tagging",
         "condition_keys": [
@@ -139175,30 +141079,30 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to make GetHeadObject requests to MediaPackage",
         "docs": {
           "api_doc": "",
-          "doc_page": "API_GetChannelPolicy.html",
-          "doc_page_rel": "API_GetChannelPolicy.html"
+          "doc_page": "${DocHomeURL}mediapackage/latest/userguide/dataplane-apis.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/userguide/dataplane-apis.html"
         }
       },
       "GetObject": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to make GetObject requests to MediaPackage",
         "docs": {
           "api_doc": "",
-          "doc_page": "API_GetChannelPolicy.html",
-          "doc_page_rel": "API_GetChannelPolicy.html"
+          "doc_page": "${DocHomeURL}mediapackage/latest/userguide/dataplane-apis.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/userguide/dataplane-apis.html"
         }
       },
       "GetOriginEndpoint": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
@@ -139302,16 +141206,16 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to make PutObject requests to MediaPackage",
         "docs": {
           "api_doc": "",
-          "doc_page": "API_PutChannelPolicy.html",
-          "doc_page_rel": "API_PutChannelPolicy.html"
+          "doc_page": "${DocHomeURL}mediapackage/latest/userguide/dataplane-apis.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/mediapackage/latest/userguide/dataplane-apis.html"
         }
       },
       "PutOriginEndpointPolicy": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -145519,15 +147423,15 @@
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/networkmanager/latest/APIReference/API_UpdateVpcAttachment.html"
         }
       }
     },
-    "arn_format": "arn:${Partition}:networkmanager::${AccountId}:${ResourceType}/${ResourceName}",
+    "arn_format": "arn:${Partition}:networkmanager::${Account}:${ResourceType}/${ResourceName}",
     "arn_regex": "^arn:${Partition}:networkmanager::.+:.+",
     "description": "AWS Network Manager",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/networkmanager/latest/APIReference/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/networkmanager/latest/APIReference/",
@@ -152594,14 +154498,557 @@
       "api_reference_doc_page": "https://docs.aws.amazon.com/panorama/latest/api/Welcome.html",
       "authz_doc_page": "https://docs.aws.amazon.com/panorama/latest/dev/panorama-permissions.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/panorama/latest/dev/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html#"
     },
     "prefix": "panorama"
   },
+  "Payment Cryptography": {
+    "actions": {
+      "CreateAlias": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to create a user-friendly name for a Key",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_CreateAlias.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_CreateAlias.html"
+        }
+      },
+      "CreateKey": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys",
+          "payment-cryptography:KeyAlgorithm",
+          "payment-cryptography:KeyClass",
+          "payment-cryptography:KeyUsage"
+        ],
+        "description": "Grants permission to create a unique customer managed key in the caller's AWS account and region",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_CreateKey.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_CreateKey.html"
+        }
+      },
+      "DecryptData": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to decrypt ciphertext data to plaintext using symmetric, asymmetric or DUKPT data encryption key",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/DataAPIReference/API_DecryptData.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/DataAPIReference/API_DecryptData.html"
+        }
+      },
+      "DeleteAlias": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to delete the specified alias",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_DeleteAlias.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_DeleteAlias.html"
+        }
+      },
+      "DeleteKey": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to schedule the deletion of a Key",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_DeleteKey.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_DeleteKey.html"
+        }
+      },
+      "EncryptData": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to encrypt plaintext data to ciphertext using symmetric, asymmetric or DUKPT data encryption key",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/DataAPIReference/API_EncryptData.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/DataAPIReference/API_EncryptData.html"
+        }
+      },
+      "ExportKey": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:CertificateAuthorityPublicKeyIdentifier",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases",
+          "payment-cryptography:WrappingKeyIdentifier"
+        ],
+        "description": "Grants permission to export a key from the service",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_ExportKey.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_ExportKey.html"
+        }
+      },
+      "GenerateCardValidationData": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to generate card-related data using algorithms such as Card Verification Values (CVV/CVV2), Dynamic Card Verification Values (dCVV/dCVV2) or Card Security Codes (CSC) that check the validity of a magnetic stripe card",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/DataAPIReference/API_GenerateCardValidationData.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/DataAPIReference/API_GenerateCardValidationData.html"
+        }
+      },
+      "GenerateMac": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to generate a MAC (Message Authentication Code) cryptogram",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/DataAPIReference/API_GenerateMac.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/DataAPIReference/API_GenerateMac.html"
+        }
+      },
+      "GeneratePinData": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to generate pin-related data such as PIN, PIN Verification Value (PVV), PIN Block and PIN Offset during new card issuance or card re-issuance",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/DataAPIReference/API_GeneratePinData.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/DataAPIReference/API_GeneratePinData.html"
+        }
+      },
+      "GetAlias": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to return the keyArn associated with an aliasName",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_GetAlias.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_GetAlias.html"
+        }
+      },
+      "GetKey": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to return the detailed information about the specified key",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_GetKey.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_GetKey.html"
+        }
+      },
+      "GetParametersForExport": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get the export token and the signing key certificate to initiate a TR-34 key export",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_GetParametersForExport.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_GetParametersForExport.html"
+        }
+      },
+      "GetParametersForImport": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get the import token and the wrapping key certificate to initiate a TR-34 key import",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_GetParametersForImport.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_GetParametersForImport.html"
+        }
+      },
+      "GetPublicKeyCertificate": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to return the public key from a key of class PUBLIC_KEY",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_GetPublicKeyCertificate.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_GetPublicKeyCertificate.html"
+        }
+      },
+      "ImportKey": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys",
+          "payment-cryptography:CertificateAuthorityPublicKeyIdentifier",
+          "payment-cryptography:ImportKeyMaterial",
+          "payment-cryptography:WrappingKeyIdentifier"
+        ],
+        "description": "Grants permission to imports keys and public key certificates",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_ImportKey.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_ImportKey.html"
+        }
+      },
+      "ListAliases": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to return a list of aliases created for all keys in the caller's AWS account and Region",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_ListAliases.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_ListAliases.html"
+        }
+      },
+      "ListKeys": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to return a list of keys created in the caller's AWS account and Region",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_ListKeys.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_ListKeys.html"
+        }
+      },
+      "ListTagsForResource": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to return a list of tags created in the caller's AWS account and Region",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_ListTagsForResource.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_ListTagsForResource.html"
+        }
+      },
+      "ReEncryptData": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to re-encrypt ciphertext using DUKPT, Symmetric and Asymmetric Data Encryption Keys",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/DataAPIReference/API_ReEncryptData.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/DataAPIReference/API_ReEncryptData.html"
+        }
+      },
+      "RestoreKey": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to cancel a scheduled key deletion if at any point during the waiting period a Key needs to be revived",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_RestoreKey.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_RestoreKey.html"
+        }
+      },
+      "StartKeyUsage": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to enable a disabled Key",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_StartKeyUsage.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_StartKeyUsage.html"
+        }
+      },
+      "StopKeyUsage": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to disable an enabled Key",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_StopKeyUsage.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_StopKeyUsage.html"
+        }
+      },
+      "TagResource": {
+        "aws_action_groups": [
+          "Tagging",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to add or overwrites one or more tags for the specified resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_TagResource.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_TagResource.html"
+        }
+      },
+      "TranslatePinData": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to translate encrypted PIN block from and to ISO 9564 formats 0,1,3,4",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/DataAPIReference/API_TranslatePinData.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/DataAPIReference/API_TranslatePinData.html"
+        }
+      },
+      "UntagResource": {
+        "aws_action_groups": [
+          "Tagging",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to remove the specified tag or tags from the specified resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_UntagResource.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_UntagResource.html"
+        }
+      },
+      "UpdateAlias": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to change the key to which an alias is assigned, or unassign it from its current key",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/APIReference/API_UpdateAlias.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/API_UpdateAlias.html"
+        }
+      },
+      "VerifyAuthRequestCryptogram": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to verify Authorization Request Cryptogram (ARQC) for a EMV chip payment card authorization",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/DataAPIReference/API_VerifyAuthRequestCryptogram.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/DataAPIReference/API_VerifyAuthRequestCryptogram.html"
+        }
+      },
+      "VerifyCardValidationData": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to verify card-related validation data using algorithms such as Card Verification Values (CVV/CVV2), Dynamic Card Verification Values (dCVV/dCVV2) and Card Security Codes (CSC)",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/DataAPIReference/API_VerifyCardValidationData.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/DataAPIReference/API_VerifyCardValidationData.html"
+        }
+      },
+      "VerifyMac": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to verify MAC (Message Authentication Code) of input data against a provided MAC",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/DataAPIReference/API_VerifyMac.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/DataAPIReference/API_VerifyMac.html"
+        }
+      },
+      "VerifyPinData": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "payment-cryptography:RequestAlias",
+          "payment-cryptography:ResourceAliases"
+        ],
+        "description": "Grants permission to verify pin-related data such as PIN and PIN Offset using algorithms including VISA PVV and IBM3624",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}payment-cryptography/latest/DataAPIReference/API_VerifyPinData.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/payment-cryptography/latest/DataAPIReference/API_VerifyPinData.html"
+        }
+      }
+    },
+    "arn_format": "arn:${Partition}:payment-cryptography:${Region}:${Account}:${ResourceType}/${Id}",
+    "arn_regex": "^arn:${Partition}:payment-cryptography:.+",
+    "description": "AWS Payment Cryptography",
+    "docs": {
+      "actions_doc_root": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/",
+      "api_detail_root": "",
+      "api_doc_root": "",
+      "api_reference_doc_page": "https://docs.aws.amazon.com/payment-cryptography/latest/APIReference/",
+      "authz_doc_page": "https://docs.aws.amazon.com/payment-cryptography/latest/userguide/security-iam.html",
+      "concepts_doc_root": "https://docs.aws.amazon.com/payment-cryptography/latest/userguide/",
+      "context_keys_doc_root": "https://docs.aws.amazon.com/payment-cryptography/latest/userguide/"
+    },
+    "prefix": "payment-cryptography"
+  },
   "Payments": {
     "actions": {
       "CreatePaymentInstrument": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -157983,14 +160430,30 @@
         "description": "Grants permission to add a profile key",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_AddProfileKey.html"
         }
       },
+      "CreateCalculatedAttributeDefinition": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create a calculated attribute definition in the domain",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_CreateCalculatedAttributeDefinition.html"
+        }
+      },
       "CreateDomain": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
@@ -157999,14 +160462,30 @@
         "description": "Grants permission to create a Domain",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_CreateDomain.html"
         }
       },
+      "CreateEventStream": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to put an event stream in a domain",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_CreateEventStream.html"
+        }
+      },
       "CreateIntegrationWorkflow": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
@@ -158028,27 +160507,53 @@
         "description": "Grants permission to create a profile in the domain",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_CreateProfile.html"
         }
       },
+      "DeleteCalculatedAttributeDefinition": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a calculated attribute definition in the domain",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_DeleteCalculatedAttributeDefinition.html"
+        }
+      },
       "DeleteDomain": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete a Domain",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_DeleteDomain.html"
         }
       },
+      "DeleteEventStream": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete an event stream in a domain",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_DeleteEventStream.html"
+        }
+      },
       "DeleteIntegration": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete a integration in a domain",
@@ -158133,28 +160638,70 @@
         "description": "Grants permission to get a preview of auto merging in a domain",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_GetAutoMergingPreview.html"
         }
       },
+      "GetCalculatedAttributeDefinition": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get a calculated attribute definition in the domain",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_GetCalculatedAttributeDefinition.html"
+        }
+      },
+      "GetCalculatedAttributeForProfile": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve a calculated attribute for a specific profile in the domain",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_GetCalculatedAttributeForProfile.html"
+        }
+      },
       "GetDomain": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to get a specific domain in an account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_GetDomain.html"
         }
       },
+      "GetEventStream": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get a specific event stream in a domain",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_GetEventStream.html"
+        }
+      },
       "GetIdentityResolutionJob": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -158261,14 +160808,44 @@
         "description": "Grants permission to list all the integrations in the account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_ListAccountIntegrations.html"
         }
       },
+      "ListCalculatedAttributeDefinitions": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite",
+          "ListOnly"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list all the calculated attribute definitions in the domain",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_ListCalculatedAttributeDefinitions.html"
+        }
+      },
+      "ListCalculatedAttributesForProfile": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite",
+          "ListOnly"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list all calculated attributes for a specific profile in the domain",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_ListCalculatedAttributesForProfile.html"
+        }
+      },
       "ListDomains": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite",
           "ListOnly"
         ],
         "calculated_action_group": "List",
@@ -158276,14 +160853,29 @@
         "description": "Grants permission to list all the domains in an account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_ListDomains.html"
         }
       },
+      "ListEventStreams": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite",
+          "ListOnly"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list all the event streams in a specific domain",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_ListEventStreams.html"
+        }
+      },
       "ListIdentityResolutionJobs": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -158486,14 +161078,27 @@
         "description": "Grants permission to remove tags from a resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_UntagResource.html"
         }
       },
+      "UpdateCalculatedAttributeDefinition": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update a calculated attribute definition in the domain",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_UpdateCalculatedAttributeDefinition.html"
+        }
+      },
       "UpdateDomain": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update a Domain",
@@ -160096,28 +162701,33 @@
   "Purchase Orders": {
     "actions": {
       "AddPurchaseOrder": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
         "description": "Grants permission to add a new purchase order",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}billing-permissions-ref.html#user-permissions",
           "doc_page_rel": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions"
         }
       },
       "DeletePurchaseOrder": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to delete a purchase order",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}billing-permissions-ref.html#user-permissions",
           "doc_page_rel": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions"
         }
       },
@@ -160137,30 +162747,34 @@
       },
       "GetPurchaseOrder": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to get a purchase order",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}billing-permissions-ref.html#user-permissions",
           "doc_page_rel": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions"
         }
       },
       "ListPurchaseOrderInvoices": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to list purchase order invoices",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}billing-permissions-ref.html#user-permissions",
           "doc_page_rel": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions"
         }
       },
@@ -160168,34 +162782,89 @@
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
-        "description": "Grants permission to get all available purchase orders",
+        "description": "Grants permission to list all purchase orders for an account",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${ConceptsDocRoot}billing-permissions-ref.html#user-permissions",
+          "doc_page_rel": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions"
+        }
+      },
+      "ListTagsForResource": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to list tags for a purchase order",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}billing-permissions-ref.html#user-permissions",
           "doc_page_rel": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions"
         }
       },
       "ModifyPurchaseOrders": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys"
+        ],
         "description": "Grants permission to modify purchase orders and details",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}billing-permissions-ref.html#user-permissions",
           "doc_page_rel": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions"
         }
       },
+      "TagResource": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "Tagging"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to tag purchase orders with given key value pairs",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${ConceptsDocRoot}billing-permissions-ref.html#user-permissions",
+          "doc_page_rel": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions"
+        }
+      },
+      "UntagResource": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "Tagging"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to remove tags from a purchase order",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${ConceptsDocRoot}billing-permissions-ref.html#user-permissions",
+          "doc_page_rel": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions"
+        }
+      },
       "UpdateConsoleActionSetEnforced": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to change whether existing or fine-grained IAM actions will be used to control authorization to Billing, Cost Management, and Account consoles",
@@ -160206,52 +162875,58 @@
         }
       },
       "UpdatePurchaseOrder": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to update an existing purchase order",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}billing-permissions-ref.html#user-permissions",
           "doc_page_rel": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions"
         }
       },
       "UpdatePurchaseOrderStatus": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to set purchase order status",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}billing-permissions-ref.html#user-permissions",
           "doc_page_rel": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions"
         }
       },
       "ViewPurchaseOrders": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
         "description": "Grants permission to view purchase orders and details",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}billing-permissions-ref.html#user-permissions",
           "doc_page_rel": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions"
         }
       }
     },
-    "arn_format": "arn:${Partition}:purchase-orders::${Account}:${ResourceType}:${ResourceName}",
-    "arn_regex": "^arn:${Partition}:purchase-orders::.+:.+:.+",
+    "arn_format": "arn:${Partition}:purchase-orders::${Account}:${ResourceType}/${ResourceName}",
+    "arn_regex": "^arn:${Partition}:purchase-orders::.+:.+",
     "description": "AWS Purchase Orders Console",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/",
       "authz_doc_page": "https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions",
@@ -162232,14 +164907,29 @@
         "description": "Grants permission to list custom permissions resources in QuickSight account",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}iam-actions.html",
           "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/user/iam-actions.html"
         }
       },
+      "ListCustomerManagedKeys": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list all registered customer managed keys",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${ConceptsDocRoot}key-management.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/user/key-management.html"
+        }
+      },
       "ListDashboardVersions": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -162405,14 +165095,29 @@
         "description": "Grants permission to list all SPICE ingestions on a dataset",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/APIReference/API_ListIngestions.html"
         }
       },
+      "ListKMSKeysForUser": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list a user's KMS keys",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${ConceptsDocRoot}key-management.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/user/key-management.html"
+        }
+      },
       "ListNamespaces": {
         "aws_action_groups": [
           "ReadWrite",
           "ListOnly",
           "ReadOnly"
         ],
         "calculated_action_group": "List",
@@ -162667,27 +165372,53 @@
         "description": "Grants permission to put dataset refresh properties for a dataset",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/APIReference/API_PutDataSetRefreshProperties.html"
         }
       },
+      "RegisterCustomerManagedKey": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to register a customer managed key",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${ConceptsDocRoot}key-management.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/user/key-management.html"
+        }
+      },
       "RegisterUser": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create a QuickSight user, whose identity is associated with the IAM identity/role specified in the request",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/APIReference/API_RegisterUser.html"
         }
       },
+      "RemoveCustomerManagedKey": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to remove a customer managed key",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${ConceptsDocRoot}key-management.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/quicksight/latest/user/key-management.html"
+        }
+      },
       "RestoreAnalysis": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to restore a deleted analysis",
@@ -166173,14 +168904,27 @@
         "description": "Grants permission to automatically create the specified Amazon Redshift user if it does not exist",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}mgmt/generating-iam-credentials-role-permissions.html",
           "doc_page_rel": "https://docs.aws.amazon.com/redshift/latest/mgmt/generating-iam-credentials-role-permissions.html"
         }
       },
+      "CreateCustomDomainAssociation": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to create a custom domain name for a cluster",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "API_CreateCustomDomainAssociation.html",
+          "doc_page_rel": "API_CreateCustomDomainAssociation.html"
+        }
+      },
       "CreateEndpointAccess": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create a redshift-managed vpc endpoint",
@@ -166418,14 +169162,27 @@
         "description": "Grants permission to delete a cluster subnet group",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/redshift/latest/APIReference/API_DeleteClusterSubnetGroup.html"
         }
       },
+      "DeleteCustomDomainAssociation": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a custom domain name for a cluster",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "API_DeleteCustomDomainAssociation.html",
+          "doc_page_rel": "API_DeleteCustomDomainAssociation.html"
+        }
+      },
       "DeleteEndpointAccess": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete a redshift-managed vpc endpoint",
@@ -166721,14 +169478,29 @@
         "description": "Grants permission to describe properties of provisioned clusters",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/redshift/latest/APIReference/API_DescribeClusters.html"
         }
       },
+      "DescribeCustomDomainAssociations": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to describe custom domain names for a cluster",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "API_DescribeCustomDomainAssociations.html",
+          "doc_page_rel": "API_DescribeCustomDomainAssociations.html"
+        }
+      },
       "DescribeDataShares": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -167486,14 +170258,27 @@
         "description": "Grants permission to modify a cluster subnet group to include the specified list of VPC subnets",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/redshift/latest/APIReference/API_ModifyClusterSubnetGroup.html"
         }
       },
+      "ModifyCustomDomainAssociation": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to modify a custom domain name for a cluster",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "API_ModifiyCustomDomainAssociation.html",
+          "doc_page_rel": "API_ModifiyCustomDomainAssociation.html"
+        }
+      },
       "ModifyEndpointAccess": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to modify a redshift-managed vpc endpoint",
@@ -168550,14 +171335,27 @@
       "concepts_doc_root": "https://docs.aws.amazon.com/redshift/latest/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/redshift/latest/"
     },
     "prefix": "redshift-serverless"
   },
   "Rekognition": {
     "actions": {
+      "AssociateFaces": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to associate multiple individual faces with a single user",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/rekognition/latest/APIReference/API_AssociateFaces.html"
+        }
+      },
       "CompareFaces": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -168667,14 +171465,27 @@
         "description": "Grants permission to create an Amazon Rekognition stream processor",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CreateStreamProcessor.html"
         }
       },
+      "CreateUser": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to create a new user in a collection using a unique user ID you provide",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/rekognition/latest/APIReference/API_CreateUser.html"
+        }
+      },
       "DeleteCollection": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete the specified collection",
@@ -168762,14 +171573,27 @@
         "description": "Grants permission to delete the specified stream processor",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteStreamProcessor.html"
         }
       },
+      "DeleteUser": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a user from a collection based on the provided user ID",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DeleteUser.html"
+        }
+      },
       "DescribeCollection": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -168920,14 +171744,27 @@
         "description": "Grants permission to detect text in the input image and convert it into machine-readable text",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DetectText.html"
         }
       },
+      "DisassociateFaces": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to remove the association between a user ID and a face ID",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/rekognition/latest/APIReference/API_DisassociateFaces.html"
+        }
+      },
       "DistributeDatasetEntries": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to distribute the entries in a training dataset across the training dataset and the test dataset for a project",
@@ -169187,14 +172024,28 @@
         "description": "Grants permission to return a list of tags associated with a resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListTagsForResource.html"
         }
       },
+      "ListUsers": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to list UserIds and the UserStatus",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/rekognition/latest/APIReference/API_ListUsers.html"
+        }
+      },
       "PutProjectPolicy": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to attach a resource policy to a project",
@@ -169242,14 +172093,42 @@
         "description": "Grants permission to search the specificed collection for the largest face in the input image",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/rekognition/latest/APIReference/API_SearchFacesByImage.html"
         }
       },
+      "SearchUsers": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to search the specificed collection for user match result with given either face ID or user ID",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/rekognition/latest/APIReference/API_SearchUsers.html"
+        }
+      },
+      "SearchUsersByImage": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to search the specificed collection for user match result by using the largest face in the input image",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/rekognition/latest/APIReference/API_SearchUsersByImage.html"
+        }
+      },
       "StartCelebrityRecognition": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to start the asynchronous recognition of celebrities in a stored video",
@@ -184141,14 +187020,27 @@
         "description": "Grants permission to a queue for a specific principal",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/API_AddPermission.html"
         }
       },
+      "CancelMessageMoveTask": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to cancel an in progress message move task",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/API_CancelMessageMoveTask.html"
+        }
+      },
       "ChangeMessageVisibility": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to change the visibility timeout of a specified message in a queue to a new value",
@@ -184238,14 +187130,28 @@
         "description": "Grants permission to return a list of your queues that have the RedrivePolicy queue attribute configured with a dead letter queue",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/API_ListDeadLetterSourceQueues.html"
         }
       },
+      "ListMessageMoveTasks": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to list message move tasks",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/API_ListMessageMoveTasks.html"
+        }
+      },
       "ListQueueTags": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -184332,14 +187238,27 @@
         "description": "Grants permission to set the value of one or more queue attributes",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/API_SetQueueAttributes.html"
         }
       },
+      "StartMessageMoveTask": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to start a message move task",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/API_StartMessageMoveTask.html"
+        }
+      },
       "TagQueue": {
         "aws_action_groups": [
           "Tagging",
           "ReadWrite"
         ],
         "calculated_action_group": "Tagging",
         "condition_keys": [
@@ -185470,15 +188389,16 @@
         "aws_action_groups": [
           "Tagging",
           "ReadWrite"
         ],
         "calculated_action_group": "Tagging",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
-          "aws:TagKeys"
+          "aws:TagKeys",
+          "sagemaker:TaggingAction"
         ],
         "description": "Grants permission to add or overwrite one or more tags for the specified Amazon SageMaker resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AddTags.html"
         }
@@ -191429,14 +194349,27 @@
         "description": "Grants permission to accept Security Hub invitations to become a member account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/securityhub/1.0/APIReference/API_AcceptInvitation.html"
         }
       },
+      "BatchDeleteAutomationRules": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete one or more automation rules in Security Hub",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}securityhub/latest/userguide/automation-rules",
+          "doc_page_rel": "https://docs.aws.amazon.com/securityhub/latest/userguide/automation-rules"
+        }
+      },
       "BatchDisableStandards": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to disable standards in Security Hub",
@@ -191455,14 +194388,28 @@
         "description": "Grants permission to enable standards in Security Hub",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/securityhub/1.0/APIReference/API_BatchEnableStandards.html"
         }
       },
+      "BatchGetAutomationRules": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve a list of details for automation rules from Security Hub based on rule Amazon Resource Names (ARNs)",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}securityhub/latest/userguide/automation-rules",
+          "doc_page_rel": "https://docs.aws.amazon.com/securityhub/latest/userguide/automation-rules"
+        }
+      },
       "BatchGetControlEvaluations": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -191512,14 +194459,27 @@
         "description": "Grants permission to import findings into Security Hub from an integrated product",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/securityhub/1.0/APIReference/API_BatchImportFindings.html"
         }
       },
+      "BatchUpdateAutomationRules": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update one or more automation rules from Security Hub based on rule Amazon Resource Names (ARNs) and input parameters",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}securityhub/latest/userguide/automation-rules",
+          "doc_page_rel": "https://docs.aws.amazon.com/securityhub/latest/userguide/automation-rules"
+        }
+      },
       "BatchUpdateFindings": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "securityhub:ASFFSyntaxPath/${ASFFSyntaxPath}"
@@ -191553,14 +194513,30 @@
         "description": "Grants permission to create custom actions in Security Hub",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/securityhub/1.0/APIReference/API_CreateActionTarget.html"
         }
       },
+      "CreateAutomationRule": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create an automation rule based on input parameters",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}securityhub/latest/userguide/automation-rules",
+          "doc_page_rel": "https://docs.aws.amazon.com/securityhub/latest/userguide/automation-rules"
+        }
+      },
       "CreateFindingAggregator": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create a finding aggregator, which contains the cross-Region finding aggregation configuration",
@@ -192113,14 +195089,29 @@
         "description": "Grants permission to invite other AWS accounts to become Security Hub member accounts",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/securityhub/1.0/APIReference/API_InviteMembers.html"
         }
       },
+      "ListAutomationRules": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve a list of automation rules and their metadata for the calling account from Security Hub",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}securityhub/latest/userguide/automation-rules",
+          "doc_page_rel": "https://docs.aws.amazon.com/securityhub/latest/userguide/automation-rules"
+        }
+      },
       "ListControlEvaluationSummaries": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -197358,14 +200349,29 @@
         "description": "Grants permission to create a state machine",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_CreateStateMachine.html"
         }
       },
+      "CreateStateMachineAlias": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "states:StateMachineQualifier"
+        ],
+        "description": "Grants permission to create a state machine alias",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_CreateStateMachineAlias.html"
+        }
+      },
       "DeleteActivity": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete an activity",
@@ -197384,14 +200390,44 @@
         "description": "Grants permission to delete a state machine",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_DeleteStateMachine.html"
         }
       },
+      "DeleteStateMachineAlias": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "states:StateMachineQualifier"
+        ],
+        "description": "Grants permission to delete a state machine alias",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_DeleteStateMachineAlias.html"
+        }
+      },
+      "DeleteStateMachineVersion": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "states:StateMachineQualifier"
+        ],
+        "description": "Grants permission to delete a state machine version",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_DeleteStateMachineVersion.html"
+        }
+      },
       "DescribeActivity": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -197432,22 +200468,40 @@
       },
       "DescribeStateMachine": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
-        "condition_keys": [],
+        "condition_keys": [
+          "states:StateMachineQualifier"
+        ],
         "description": "Grants permission to describe a state machine",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_DescribeStateMachine.html"
         }
       },
+      "DescribeStateMachineAlias": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "states:StateMachineQualifier"
+        ],
+        "description": "Grants permission to describe a state machine alias",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_DescribeStateMachineAlias.html"
+        }
+      },
       "DescribeStateMachineForExecution": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -197498,19 +200552,22 @@
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_ListActivities.html"
         }
       },
       "ListExecutions": {
         "aws_action_groups": [
+          "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
-        "calculated_action_group": "Read",
-        "condition_keys": [],
+        "calculated_action_group": "List",
+        "condition_keys": [
+          "states:StateMachineQualifier"
+        ],
         "description": "Grants permission to list the executions of a state machine",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_ListExecutions.html"
         }
       },
@@ -197525,14 +200582,46 @@
         "description": "Grants permission to list the map runs of an execution",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_ListMapRuns.html"
         }
       },
+      "ListStateMachineAliases": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [
+          "states:StateMachineQualifier"
+        ],
+        "description": "Grants permission to list the aliases of a state machine",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_ListStateMachineAliases.html"
+        }
+      },
+      "ListStateMachineVersions": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list the versions of a state machine",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_ListStateMachineVersions.html"
+        }
+      },
       "ListStateMachines": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -197542,26 +200631,40 @@
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_ListStateMachines.html"
         }
       },
       "ListTagsForResource": {
         "aws_action_groups": [
+          "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
-        "calculated_action_group": "Read",
+        "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list tags for an AWS Step Functions resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_ListTagsForResource.html"
         }
       },
+      "PublishStateMachineVersion": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to publish a state machine version",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_PublishStateMachineVersion.html"
+        }
+      },
       "SendTaskFailure": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to report that the task identified by the taskToken failed",
@@ -197598,28 +200701,32 @@
         }
       },
       "StartExecution": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "states:StateMachineQualifier"
+        ],
         "description": "Grants permission to start a state machine execution",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_StartExecution.html"
         }
       },
       "StartSyncExecution": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "states:StateMachineQualifier"
+        ],
         "description": "Grants permission to start a Synchronous Express state machine execution",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_StartSyncExecution.html"
         }
       },
@@ -197693,14 +200800,29 @@
         ],
         "description": "Grants permission to update a state machine",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_UpdateStateMachine.html"
         }
+      },
+      "UpdateStateMachineAlias": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "states:StateMachineQualifier"
+        ],
+        "description": "Grants permission to update a state machine alias",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/step-functions/latest/apireference/API_UpdateStateMachineAlias.html"
+        }
       }
     },
     "arn_format": "arn:${Partition}:states:${Region}:${Account}:${ResourceType}:${ResourceName}",
     "arn_regex": "^arn:${Partition}:states:.+",
     "description": "AWS Step Functions",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/step-functions/latest/apireference/",
@@ -199002,317 +202124,345 @@
     "actions": {
       "AddAttachmentsToSet": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Adds one or more attachments to an AWS Support case.",
+        "description": "Grants permission to add one or more attachments to an AWS Support case",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_AddAttachmentsToSet.html"
         }
       },
       "AddCommunicationToCase": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Adds a customer communication to an AWS Support case.",
+        "description": "Grants permission to add a customer communication to an AWS Support case",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_AddCommunicationToCase.html"
         }
       },
       "CreateCase": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Creates a new AWS Support case.",
+        "description": "Grants permission to creates a new AWS Support case",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_CreateCase.html"
         }
       },
       "DescribeAttachment": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Returns the description for an attachment.",
+        "description": "Grants permission to describe attachment detail",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_DescribeAttachment.html"
         }
       },
       "DescribeCaseAttributes": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "This is an internally managed function which allows secondary services to read AWS Support case attributes.",
+        "description": "Grants permission to allow secondary services to read AWS Support case attributes.This is an internally managed function",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/"
+          "doc_page": "${DocHomeURL}awssupport/latest/user/accessing-support.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/user/accessing-support.html"
         }
       },
       "DescribeCases": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Returns a list of AWS Support cases that matches the given inputs.",
+        "description": "Grants permission to list AWS Support cases that matches the given inputs",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_DescribeCases.html"
         }
       },
       "DescribeCommunications": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Returns the communications and attachments for one or more AWS Support cases.",
+        "description": "Grants permission to list the communications and attachments for one or more AWS Support cases",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_DescribeCommunications.html"
         }
       },
-      "DescribeIssueTypes": {
+      "DescribeCreateCaseOptions": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Returns issue types for AWS Support cases.",
+        "description": "Grants permission to describes the available options for creating a support case",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/"
+          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_DescribeCreateCaseOptions.html"
+        }
+      },
+      "DescribeIssueTypes": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to return issue types for AWS Support cases",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}awssupport/latest/user/accessing-support.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/user/accessing-support.html"
         }
       },
       "DescribeServices": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Returns the current list of AWS services and categories that applies to each service.",
+        "description": "Grants permission to list AWS services and categories that applies to each service",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_DescribeServices.html"
         }
       },
       "DescribeSeverityLevels": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Returns the list of severity levels that can be assigned to an AWS Support case.",
+        "description": "Grants permission to list severity levels that can be assigned to an AWS Support case",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_DescribeSeverityLevels.html"
         }
       },
       "DescribeSupportLevel": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Returns the support level for an AWS Account identifier.",
+        "description": "Grants permission to return the support level for an AWS Account identifier",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}awssupport/latest/user/accessing-support.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/user/accessing-support.html"
+        }
+      },
+      "DescribeSupportedLanguages": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to describes the available support languages for a given category code, service code and issue type",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/"
+          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_DescribeSupportedLanguages.html"
         }
       },
       "DescribeTrustedAdvisorCheckRefreshStatuses": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Returns the status of a Trusted Advisor refresh check based on a list of check identifiers.",
+        "description": "Grants permission to get the status of a Trusted Advisor refresh check based on a list of check identifiers",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_DescribeTrustedAdvisorCheckRefreshStatuses.html"
         }
       },
       "DescribeTrustedAdvisorCheckResult": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Returns the results of the Trusted Advisor check that has the specified check identifier.",
+        "description": "Grants permission to get the results of the Trusted Advisor check that has the specified check identifier",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_DescribeTrustedAdvisorCheckResult.html"
         }
       },
       "DescribeTrustedAdvisorCheckSummaries": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Returns the summaries of the results of the Trusted Advisor checks that have the specified check identifiers.",
+        "description": "Grants permission to get the summaries of the results of the Trusted Advisor checks that have the specified check identifiers",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_DescribeTrustedAdvisorCheckSummaries.html"
         }
       },
       "DescribeTrustedAdvisorChecks": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Returns a list of all available Trusted Advisor checks, including name, identifier, category and description.",
+        "description": "Grants permission to get a list of all available Trusted Advisor checks, including name, identifier, category and description",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_DescribeTrustedAdvisorChecks.html"
         }
       },
       "InitiateCallForCase": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "This is an internally managed function to initiate a call on AWS Support Center.",
+        "description": "Grants permission to initiate a call on AWS Support Center. This is an internally managed function",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/"
+          "doc_page": "${DocHomeURL}awssupport/latest/user/accessing-support.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/user/accessing-support.html"
         }
       },
       "InitiateChatForCase": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "This is an internally managed function to initiate a chat on AWS Support Center.",
+        "description": "Grants permission to initiate a chat on AWS Support Center.This is an internally managed function",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/"
+          "doc_page": "${DocHomeURL}awssupport/latest/user/accessing-support.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/user/accessing-support.html"
         }
       },
       "PutCaseAttributes": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "This is an internally managed function which allows secondary services to attach attributes to AWS Support cases.",
+        "description": "Grants permission to allow secondary services to attach attributes to AWS Support cases. This is an internally managed function",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/"
+          "doc_page": "${DocHomeURL}awssupport/latest/user/accessing-support.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/user/accessing-support.html"
         }
       },
       "RateCaseCommunication": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Rate an AWS Support case communication.",
+        "description": "Grants permission to rate an AWS Support case communication",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/"
+          "doc_page": "${DocHomeURL}awssupport/latest/user/accessing-support.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/user/accessing-support.html"
         }
       },
       "RefreshTrustedAdvisorCheck": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Requests a refresh of the Trusted Advisor check that has the specified check identifier.",
+        "description": "Grants permission to requests a refresh of the Trusted Advisor check that has the specified check identifier",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_RefreshTrustedAdvisorCheck.html"
         }
       },
       "ResolveCase": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Resolves an AWS Support case.",
+        "description": "Grants permission to resolve an AWS Support case",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/API_ResolveCase.html"
         }
       },
       "SearchForCases": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Returns a list of AWS Support cases that matches the given inputs.",
+        "description": "Grants permission to return a list of AWS Support cases that matches the given inputs",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/APIReference/"
+          "doc_page": "${DocHomeURL}awssupport/latest/user/accessing-support.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/awssupport/latest/user/accessing-support.html"
         }
       }
     },
     "arn_format": "",
     "arn_regex": "",
     "description": "AWS Support",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/awssupport/latest/APIReference/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/awssupport/latest/APIReference/Welcome.html",
-      "authz_doc_page": "https://docs.aws.amazon.com/awssupport/latest/user/access_permissions.html",
+      "authz_doc_page": "https://docs.aws.amazon.com/awssupport/latest/user/security.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/awssupport/latest/user/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/awssupport/latest/user/"
     },
     "prefix": "support"
   },
   "Support App": {
     "actions": {
@@ -207715,14 +210865,358 @@
       "api_reference_doc_page": "https://docs.aws.amazon.com/AWSEC2/latest/APIReference/operation-list-verified-access.html",
       "authz_doc_page": "https://docs.aws.amazon.com/verified-access/latest/ug/security_iam_id-based-policy-examples.html#security_iam_id-based-policy-examples-create-instance",
       "concepts_doc_root": "https://docs.aws.amazon.com/verified-access/latest/ug/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/verified-access/latest/ug/"
     },
     "prefix": "verified-access"
   },
+  "Verified Permissions": {
+    "actions": {
+      "CreateIdentitySource": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to create a reference to an external identity provider (IdP) that is compatible with OpenID Connect (OIDC) authentication protocol, such as Amazon Cognito",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_CreateIdentitySource.html"
+        }
+      },
+      "CreatePolicy": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to create a Cedar policy and save it in the specified policy store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_CreatePolicy.html"
+        }
+      },
+      "CreatePolicyStore": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to create a Cedar policy and save it in the specified policy store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_CreatePolicyStore.html"
+        }
+      },
+      "CreatePolicyTemplate": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to create a policy template",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_CreatePolicyTemplate.html"
+        }
+      },
+      "DeleteIdentitySource": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete an identity source that references an identity provider (IdP) such as Amazon Cognito",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_DeleteIdentitySource.html"
+        }
+      },
+      "DeletePolicy": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete the specified policy from the policy store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_DeletePolicy.html"
+        }
+      },
+      "DeletePolicyStore": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete the specified policy store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_DeletePolicyStore.html"
+        }
+      },
+      "DeletePolicyTemplate": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete the specified policy template from the policy store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_DeletePolicyTemplate.html"
+        }
+      },
+      "GetIdentitySource": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve the details about the specified identity source",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_GetIdentitySource.html"
+        }
+      },
+      "GetPolicy": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve information about the specified policy",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_GetPolicy.html"
+        }
+      },
+      "GetPolicyStore": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve details about a policy store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_GetPolicyStore.html"
+        }
+      },
+      "GetPolicyTemplate": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve the details for the specified policy template in the specified policy store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_GetPolicyTemplate.html"
+        }
+      },
+      "GetSchema": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve the details for the specified schema in the specified policy store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_GetSchema.html"
+        }
+      },
+      "IsAuthorized": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to make an authorization decision about a service request described in the parameters",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_IsAuthorized.html"
+        }
+      },
+      "IsAuthorizedWithToken": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to make an authorization decision about a service request described in the parameters. The principal in this request comes from an external identity source",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_IsAuthorizedWithToken.html"
+        }
+      },
+      "ListIdentitySources": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to return a paginated list of all of the identity sources defined in the specified policy store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_ListIdentitySources.html"
+        }
+      },
+      "ListPolicies": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to return a paginated list of all policies stored in the specified policy store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_ListPolicies.html"
+        }
+      },
+      "ListPolicyStores": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to return a paginated list of all policy stores in the calling Amazon Web Services account",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_ListPolicyStores.html"
+        }
+      },
+      "ListPolicyTemplates": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to return a paginated list of all policy templates in the specified policy store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_ListPolicyTemplates.html"
+        }
+      },
+      "PutSchema": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to create or update the policy schema in the specified policy store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_PutSchema.html"
+        }
+      },
+      "UpdateIdentitySource": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update the specified identity source to use a new identity provider (IdP) source, or to change the mapping of identities from the IdP to a different principal entity type",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_UpdateIdentitySource.html"
+        }
+      },
+      "UpdatePolicy": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to modify the specified Cedar static policy in the specified policy store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_UpdatePolicy.html"
+        }
+      },
+      "UpdatePolicyStore": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to modify the validation setting for a policy store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_UpdatePolicyStore.html"
+        }
+      },
+      "UpdatePolicyTemplate": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update the specified policy template",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/API_UpdatePolicyTemplate.html"
+        }
+      }
+    },
+    "arn_format": "arn:${Partition}:verifiedpermissions:${Region}:${Account}:${ResourceType}/${ResourceId}",
+    "arn_regex": "^arn:${Partition}:verifiedpermissions:.+",
+    "description": "Amazon Verified Permissions",
+    "docs": {
+      "actions_doc_root": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/",
+      "api_detail_root": "",
+      "api_doc_root": "",
+      "api_reference_doc_page": "https://docs.aws.amazon.com/verifiedpermissions/latest/apireference/",
+      "authz_doc_page": "https://docs.aws.amazon.com/verifiedpermissions/latest/userguide/security-iam.html",
+      "concepts_doc_root": "https://docs.aws.amazon.com/verifiedpermissions/latest/userguide/",
+      "context_keys_doc_root": "https://docs.aws.amazon.com/verifiedpermissions/latest/userguide/"
+    },
+    "prefix": "verifiedpermissions"
+  },
   "Voice ID": {
     "actions": {
       "AssociateFraudster": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -211259,14 +214753,27 @@
         "description": "Grants permission to associate a lens to the specified workload",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_AssociateLenses.html"
         }
       },
+      "AssociateProfiles": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to associate a profile to the specified workload",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_AssociateProfiles.html"
+        }
+      },
       "CreateLensShare": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to an owner of a lens to share with other AWS accounts and IAM Users",
@@ -211298,14 +214805,43 @@
         "description": "Grants permission to create a new milestone for the specified workload",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_CreateMilestone.html"
         }
       },
+      "CreateProfile": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create a new profile",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_CreateProfile.html"
+        }
+      },
+      "CreateProfileShare": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to an owner of a profile to share with other AWS accounts and IAM Users",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_CreateProfileShare.html"
+        }
+      },
       "CreateWorkload": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
@@ -211353,14 +214889,40 @@
         "description": "Grants permission to delete an existing lens share",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_DeleteLensShare.html"
         }
       },
+      "DeleteProfile": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a profile",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_DeleteProfile.html"
+        }
+      },
+      "DeleteProfileShare": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete an existing profile share",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_DeleteProfileShare.html"
+        }
+      },
       "DeleteWorkload": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete an existing workload",
@@ -211392,14 +214954,27 @@
         "description": "Grants permission to disassociate a lens from the specified workload",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_DisassociateLenses.html"
         }
       },
+      "DisassociateProfiles": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to disassociate a profile from the specified workload",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_DisassociateProfiles.html"
+        }
+      },
       "ExportLens": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -211506,14 +215081,44 @@
         "description": "Grants permission to retrieve the specified milestone of the specified workload",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_GetMilestone.html"
         }
       },
+      "GetProfile": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to retrieve the specified profile",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_GetProfile.html"
+        }
+      },
+      "GetProfileTemplate": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve the specified profile template",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_GetProfileTemplate.html"
+        }
+      },
       "GetWorkload": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [
@@ -211673,14 +215278,59 @@
         "description": "Grants permission to list notifications related to the account or specified resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_ListNotifications.html"
         }
       },
+      "ListProfileNotifications": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list profile notifications related to specified resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_ListProfileNotifications.html"
+        }
+      },
+      "ListProfileShares": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list all shares created for a profile",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_ListProfileShares.html"
+        }
+      },
+      "ListProfiles": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list the profiles available to this account",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_ListProfiles.html"
+        }
+      },
       "ListShareInvitations": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -211806,14 +215456,27 @@
         "description": "Grants permission to update properties of the specified lens review",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_UpdateLensReview.html"
         }
       },
+      "UpdateProfile": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update properties of the specified profile",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_UpdateProfile.html"
+        }
+      },
       "UpdateShareInvitation": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update status of the specified workload share invitation",
@@ -211857,14 +215520,27 @@
         "condition_keys": [],
         "description": "Grants permission to upgrade the specified lens review to use the latest version of the associated lens",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_UpgradeLensReview.html"
         }
+      },
+      "UpgradeProfileVersion": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to upgrade the specified workload to use the latest version of the associated profile",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/API_UpgradeProfileVersion.html"
+        }
       }
     },
     "arn_format": "arn:${Partition}:wellarchitected:${Region}:${Account}:${ResourceName}/${ResourceId}",
     "arn_regex": "^arn:${Partition}:wellarchitected:.+",
     "description": "AWS Well-Architected Tool",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/wellarchitected/latest/APIReference/",
```

### Comparing `policyuniverse-1.5.1.20230608/policyuniverse/expander_minimizer.py` & `policyuniverse-1.5.1.20230703/policyuniverse/expander_minimizer.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230608/policyuniverse/organization.py` & `policyuniverse-1.5.1.20230703/policyuniverse/organization.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230608/policyuniverse/policy.py` & `policyuniverse-1.5.1.20230703/policyuniverse/policy.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230608/policyuniverse/statement.py` & `policyuniverse-1.5.1.20230703/policyuniverse/statement.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230608/policyuniverse.egg-info/PKG-INFO` & `policyuniverse-1.5.1.20230703/policyuniverse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyuniverse
-Version: 1.5.1.20230608
+Version: 1.5.1.20230703
 Summary: Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.
 Home-page: https://github.com/Netflix-Skunkworks/policyuniverse
 Author: Patrick Kelley
 Author-email: patrickbarrettkelley@gmail.com
 Keywords: iam,arn,action_groups,condition,policy,statement,wildcard
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
```

### Comparing `policyuniverse-1.5.1.20230608/policyuniverse.egg-info/SOURCES.txt` & `policyuniverse-1.5.1.20230703/policyuniverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230608/setup.py` & `policyuniverse-1.5.1.20230703/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ROOT = os.path.realpath(os.path.join(os.path.dirname(__file__)))
 
 tests_require = ["pytest", "coveralls", "bandit"]
 dev_require = ["pre-commit", "black"]
 
 setup(
     name="policyuniverse",
-    version="1.5.1.20230608",
+    version="1.5.1.20230703",
     description="Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.",
     long_description=open(os.path.join(ROOT, "README.md")).read(),
     long_description_content_type="text/markdown",
     author="Patrick Kelley",
     author_email="patrickbarrettkelley@gmail.com",
     url="https://github.com/Netflix-Skunkworks/policyuniverse",
     keywords=[
```

