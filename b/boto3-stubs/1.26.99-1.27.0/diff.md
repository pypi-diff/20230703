# Comparing `tmp/boto3-stubs-1.26.99.tar.gz` & `tmp/boto3-stubs-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3-stubs-1.26.99.tar", last modified: Fri Mar 24 19:32:26 2023, max compression
+gzip compressed data, was "boto3-stubs-1.27.0.tar", last modified: Mon Jul  3 19:50:22 2023, max compression
```

## Comparing `boto3-stubs-1.26.99.tar` & `boto3-stubs-1.27.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:26.953894 boto3-stubs-1.26.99/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-24 19:31:52.000000 boto3-stubs-1.26.99/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    74184 2023-03-24 19:32:26.953894 boto3-stubs-1.26.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    63011 2023-03-24 19:31:52.000000 boto3-stubs-1.26.99/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:26.953894 boto3-stubs-1.26.99/boto3-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)   183900 2023-03-24 19:31:55.000000 boto3-stubs-1.26.99/boto3-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/compat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:26.953894 boto3-stubs-1.26.99/boto3-stubs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/docs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/docs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:26.953894 boto3-stubs-1.26.99/boto3-stubs/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/dynamodb/conditions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/dynamodb/table.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/dynamodb/transform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/dynamodb/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:26.953894 boto3-stubs-1.26.99/boto3-stubs/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/ec2/createtags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/ec2/deletetags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 19:31:58.000000 boto3-stubs-1.26.99/boto3-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:26.953894 boto3-stubs-1.26.99/boto3-stubs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/resources/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/resources/action.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/resources/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/resources/collection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/resources/factory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/resources/model.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/resources/params.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/resources/response.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:26.953894 boto3-stubs-1.26.99/boto3-stubs/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/s3/inject.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/s3/transfer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   208787 2023-03-24 19:31:58.000000 boto3-stubs-1.26.99/boto3-stubs/session.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/boto3-stubs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 19:32:26.953894 boto3-stubs-1.26.99/boto3_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    74184 2023-03-24 19:32:26.000000 boto3-stubs-1.26.99/boto3_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-03-24 19:32:26.000000 boto3-stubs-1.26.99/boto3_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 19:32:26.000000 boto3-stubs-1.26.99/boto3_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 19:32:26.000000 boto3-stubs-1.26.99/boto3_stubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)    32448 2023-03-24 19:32:26.000000 boto3-stubs-1.26.99/boto3_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-24 19:32:26.000000 boto3-stubs-1.26.99/boto3_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 19:32:26.953894 boto3-stubs-1.26.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    44966 2023-03-24 19:31:51.000000 boto3-stubs-1.26.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.202816 boto3-stubs-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:31:45.000000 boto3-stubs-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    75725 2023-07-03 19:50:22.202816 boto3-stubs-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    64299 2023-07-03 19:31:45.000000 boto3-stubs-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.186816 boto3-stubs-1.27.0/boto3-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)   188206 2023-07-03 19:31:52.000000 boto3-stubs-1.27.0/boto3-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.186816 boto3-stubs-1.27.0/boto3-stubs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/docs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 19:31:45.000000 boto3-stubs-1.27.0/boto3-stubs/docs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.186816 boto3-stubs-1.27.0/boto3-stubs/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:31:45.000000 boto3-stubs-1.27.0/boto3-stubs/dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-03 19:31:45.000000 boto3-stubs-1.27.0/boto3-stubs/dynamodb/conditions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-03 19:31:45.000000 boto3-stubs-1.27.0/boto3-stubs/dynamodb/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-03 19:31:45.000000 boto3-stubs-1.27.0/boto3-stubs/dynamodb/transform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-03 19:31:45.000000 boto3-stubs-1.27.0/boto3-stubs/dynamodb/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.186816 boto3-stubs-1.27.0/boto3-stubs/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/ec2/createtags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/ec2/deletetags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:31:52.000000 boto3-stubs-1.27.0/boto3-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.198816 boto3-stubs-1.27.0/boto3-stubs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/resources/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/resources/action.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/resources/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/resources/collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/resources/factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/resources/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/resources/params.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/resources/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.198816 boto3-stubs-1.27.0/boto3-stubs/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:31:45.000000 boto3-stubs-1.27.0/boto3-stubs/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-03 19:31:45.000000 boto3-stubs-1.27.0/boto3-stubs/s3/inject.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-03 19:31:45.000000 boto3-stubs-1.27.0/boto3-stubs/s3/transfer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   213622 2023-07-03 19:31:49.000000 boto3-stubs-1.27.0/boto3-stubs/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-03 19:31:44.000000 boto3-stubs-1.27.0/boto3-stubs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.202816 boto3-stubs-1.27.0/boto3_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    75725 2023-07-03 19:50:22.000000 boto3-stubs-1.27.0/boto3_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-03 19:50:22.000000 boto3-stubs-1.27.0/boto3_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 boto3-stubs-1.27.0/boto3_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 boto3-stubs-1.27.0/boto3_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)    33283 2023-07-03 19:50:22.000000 boto3-stubs-1.27.0/boto3_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 19:50:22.000000 boto3-stubs-1.27.0/boto3_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:22.202816 boto3-stubs-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    46039 2023-07-03 19:31:45.000000 boto3-stubs-1.27.0/setup.py
```

### Comparing `boto3-stubs-1.26.99/LICENSE` & `boto3-stubs-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/PKG-INFO` & `boto3-stubs-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boto3-stubs
-Version: 1.26.99
-Summary: Type annotations for boto3 1.26.99 generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3 1.27.0 generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -41,14 +41,15 @@
 Provides-Extra: amplifybackend
 Provides-Extra: amplifyuibuilder
 Provides-Extra: apigateway
 Provides-Extra: apigatewaymanagementapi
 Provides-Extra: apigatewayv2
 Provides-Extra: appconfig
 Provides-Extra: appconfigdata
+Provides-Extra: appfabric
 Provides-Extra: appflow
 Provides-Extra: appintegrations
 Provides-Extra: application-autoscaling
 Provides-Extra: application-insights
 Provides-Extra: applicationcostprofiler
 Provides-Extra: appmesh
 Provides-Extra: apprunner
@@ -88,14 +89,15 @@
 Provides-Extra: cloudwatch
 Provides-Extra: codeartifact
 Provides-Extra: codebuild
 Provides-Extra: codecatalyst
 Provides-Extra: codecommit
 Provides-Extra: codedeploy
 Provides-Extra: codeguru-reviewer
+Provides-Extra: codeguru-security
 Provides-Extra: codeguruprofiler
 Provides-Extra: codepipeline
 Provides-Extra: codestar
 Provides-Extra: codestar-connections
 Provides-Extra: codestar-notifications
 Provides-Extra: cognito-identity
 Provides-Extra: cognito-idp
@@ -237,14 +239,15 @@
 Provides-Extra: marketplace-entitlement
 Provides-Extra: marketplacecommerceanalytics
 Provides-Extra: mediaconnect
 Provides-Extra: mediaconvert
 Provides-Extra: medialive
 Provides-Extra: mediapackage
 Provides-Extra: mediapackage-vod
+Provides-Extra: mediapackagev2
 Provides-Extra: mediastore
 Provides-Extra: mediastore-data
 Provides-Extra: mediatailor
 Provides-Extra: memorydb
 Provides-Extra: meteringmarketplace
 Provides-Extra: mgh
 Provides-Extra: mgn
@@ -263,16 +266,19 @@
 Provides-Extra: oam
 Provides-Extra: omics
 Provides-Extra: opensearch
 Provides-Extra: opensearchserverless
 Provides-Extra: opsworks
 Provides-Extra: opsworkscm
 Provides-Extra: organizations
+Provides-Extra: osis
 Provides-Extra: outposts
 Provides-Extra: panorama
+Provides-Extra: payment-cryptography
+Provides-Extra: payment-cryptography-data
 Provides-Extra: personalize
 Provides-Extra: personalize-events
 Provides-Extra: personalize-runtime
 Provides-Extra: pi
 Provides-Extra: pinpoint
 Provides-Extra: pinpoint-email
 Provides-Extra: pinpoint-sms-voice
@@ -356,15 +362,17 @@
 Provides-Extra: textract
 Provides-Extra: timestream-query
 Provides-Extra: timestream-write
 Provides-Extra: tnb
 Provides-Extra: transcribe
 Provides-Extra: transfer
 Provides-Extra: translate
+Provides-Extra: verifiedpermissions
 Provides-Extra: voice-id
+Provides-Extra: vpc-lattice
 Provides-Extra: waf
 Provides-Extra: waf-regional
 Provides-Extra: wafv2
 Provides-Extra: wellarchitected
 Provides-Extra: wisdom
 Provides-Extra: workdocs
 Provides-Extra: worklink
@@ -377,30 +385,30 @@
 
 <a id="boto3-stubs"></a>
 
 # boto3-stubs
 
 [![PyPI - boto3-stubs](https://img.shields.io/pypi/v/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/boto3-stubs?color=blue)](https://pypistats.org/packages/boto3-stubs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/1.26.99/index.html)
+[boto3 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/1.27.0/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [boto3-stubs docs](https://youtype.github.io/boto3_stubs_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
@@ -765,15 +773,15 @@
 in [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder/issues/)
 repository.
 
 <a id="submodules"></a>
 
 ## Submodules
 
-- `boto3-stubs[all]` - Type annotations for all 342 services.
+- `boto3-stubs[all]` - Type annotations for all 350 services.
 - `boto3-stubs[essential]` - Type annotations for
   [CloudFormation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/),
   [DynamoDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/),
   [EC2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/),
   [Lambda](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/),
   [RDS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/),
   [S3](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/) and
@@ -816,14 +824,17 @@
   service.
 - `boto3-stubs[appconfig]` - Type annotations for
   [AppConfig](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
   service.
 - `boto3-stubs[appconfigdata]` - Type annotations for
   [AppConfigData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/)
   service.
+- `boto3-stubs[appfabric]` - Type annotations for
+  [AppFabric](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/)
+  service.
 - `boto3-stubs[appflow]` - Type annotations for
   [Appflow](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
   service.
 - `boto3-stubs[appintegrations]` - Type annotations for
   [AppIntegrationsService](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
   service.
 - `boto3-stubs[application-autoscaling]` - Type annotations for
@@ -957,14 +968,17 @@
   service.
 - `boto3-stubs[codedeploy]` - Type annotations for
   [CodeDeploy](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
   service.
 - `boto3-stubs[codeguru-reviewer]` - Type annotations for
   [CodeGuruReviewer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
   service.
+- `boto3-stubs[codeguru-security]` - Type annotations for
+  [CodeGuruSecurity](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
+  service.
 - `boto3-stubs[codeguruprofiler]` - Type annotations for
   [CodeGuruProfiler](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
   service.
 - `boto3-stubs[codepipeline]` - Type annotations for
   [CodePipeline](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
   service.
 - `boto3-stubs[codestar]` - Type annotations for
@@ -1386,14 +1400,17 @@
   service.
 - `boto3-stubs[mediapackage]` - Type annotations for
   [MediaPackage](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
   service.
 - `boto3-stubs[mediapackage-vod]` - Type annotations for
   [MediaPackageVod](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
   service.
+- `boto3-stubs[mediapackagev2]` - Type annotations for
+  [mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
+  service.
 - `boto3-stubs[mediastore]` - Type annotations for
   [MediaStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
   service.
 - `boto3-stubs[mediastore-data]` - Type annotations for
   [MediaStoreData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
   service.
 - `boto3-stubs[mediatailor]` - Type annotations for
@@ -1461,20 +1478,29 @@
   service.
 - `boto3-stubs[opsworkscm]` - Type annotations for
   [OpsWorksCM](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
   service.
 - `boto3-stubs[organizations]` - Type annotations for
   [Organizations](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_organizations/)
   service.
+- `boto3-stubs[osis]` - Type annotations for
+  [OpenSearchIngestion](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
+  service.
 - `boto3-stubs[outposts]` - Type annotations for
   [Outposts](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
   service.
 - `boto3-stubs[panorama]` - Type annotations for
   [Panorama](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
   service.
+- `boto3-stubs[payment-cryptography]` - Type annotations for
+  [PaymentCryptographyControlPlane](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/)
+  service.
+- `boto3-stubs[payment-cryptography-data]` - Type annotations for
+  [PaymentCryptographyDataPlane](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/)
+  service.
 - `boto3-stubs[personalize]` - Type annotations for
   [Personalize](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
   service.
 - `boto3-stubs[personalize-events]` - Type annotations for
   [PersonalizeEvents](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/)
   service.
 - `boto3-stubs[personalize-runtime]` - Type annotations for
@@ -1727,17 +1753,23 @@
   service.
 - `boto3-stubs[transfer]` - Type annotations for
   [Transfer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
   service.
 - `boto3-stubs[translate]` - Type annotations for
   [Translate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
   service.
+- `boto3-stubs[verifiedpermissions]` - Type annotations for
+  [VerifiedPermissions](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
+  service.
 - `boto3-stubs[voice-id]` - Type annotations for
   [VoiceID](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
   service.
+- `boto3-stubs[vpc-lattice]` - Type annotations for
+  [VPCLattice](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
+  service.
 - `boto3-stubs[waf]` - Type annotations for
   [WAF](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/) service.
 - `boto3-stubs[waf-regional]` - Type annotations for
   [WAFRegional](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
   service.
 - `boto3-stubs[wafv2]` - Type annotations for
   [WAFV2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
```

### Comparing `boto3-stubs-1.26.99/README.md` & `boto3-stubs-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="boto3-stubs"></a>
 
 # boto3-stubs
 
 [![PyPI - boto3-stubs](https://img.shields.io/pypi/v/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/boto3-stubs?color=blue)](https://pypistats.org/packages/boto3-stubs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/1.26.99/index.html)
+[boto3 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/1.27.0/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [boto3-stubs docs](https://youtype.github.io/boto3_stubs_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
@@ -388,15 +388,15 @@
 in [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder/issues/)
 repository.
 
 <a id="submodules"></a>
 
 ## Submodules
 
-- `boto3-stubs[all]` - Type annotations for all 342 services.
+- `boto3-stubs[all]` - Type annotations for all 350 services.
 - `boto3-stubs[essential]` - Type annotations for
   [CloudFormation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/),
   [DynamoDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/),
   [EC2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/),
   [Lambda](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/),
   [RDS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/),
   [S3](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/) and
@@ -439,14 +439,17 @@
   service.
 - `boto3-stubs[appconfig]` - Type annotations for
   [AppConfig](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
   service.
 - `boto3-stubs[appconfigdata]` - Type annotations for
   [AppConfigData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/)
   service.
+- `boto3-stubs[appfabric]` - Type annotations for
+  [AppFabric](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/)
+  service.
 - `boto3-stubs[appflow]` - Type annotations for
   [Appflow](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
   service.
 - `boto3-stubs[appintegrations]` - Type annotations for
   [AppIntegrationsService](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
   service.
 - `boto3-stubs[application-autoscaling]` - Type annotations for
@@ -580,14 +583,17 @@
   service.
 - `boto3-stubs[codedeploy]` - Type annotations for
   [CodeDeploy](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
   service.
 - `boto3-stubs[codeguru-reviewer]` - Type annotations for
   [CodeGuruReviewer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
   service.
+- `boto3-stubs[codeguru-security]` - Type annotations for
+  [CodeGuruSecurity](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
+  service.
 - `boto3-stubs[codeguruprofiler]` - Type annotations for
   [CodeGuruProfiler](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
   service.
 - `boto3-stubs[codepipeline]` - Type annotations for
   [CodePipeline](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
   service.
 - `boto3-stubs[codestar]` - Type annotations for
@@ -1009,14 +1015,17 @@
   service.
 - `boto3-stubs[mediapackage]` - Type annotations for
   [MediaPackage](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
   service.
 - `boto3-stubs[mediapackage-vod]` - Type annotations for
   [MediaPackageVod](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
   service.
+- `boto3-stubs[mediapackagev2]` - Type annotations for
+  [mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
+  service.
 - `boto3-stubs[mediastore]` - Type annotations for
   [MediaStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
   service.
 - `boto3-stubs[mediastore-data]` - Type annotations for
   [MediaStoreData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
   service.
 - `boto3-stubs[mediatailor]` - Type annotations for
@@ -1084,20 +1093,29 @@
   service.
 - `boto3-stubs[opsworkscm]` - Type annotations for
   [OpsWorksCM](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
   service.
 - `boto3-stubs[organizations]` - Type annotations for
   [Organizations](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_organizations/)
   service.
+- `boto3-stubs[osis]` - Type annotations for
+  [OpenSearchIngestion](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
+  service.
 - `boto3-stubs[outposts]` - Type annotations for
   [Outposts](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
   service.
 - `boto3-stubs[panorama]` - Type annotations for
   [Panorama](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
   service.
+- `boto3-stubs[payment-cryptography]` - Type annotations for
+  [PaymentCryptographyControlPlane](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/)
+  service.
+- `boto3-stubs[payment-cryptography-data]` - Type annotations for
+  [PaymentCryptographyDataPlane](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/)
+  service.
 - `boto3-stubs[personalize]` - Type annotations for
   [Personalize](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
   service.
 - `boto3-stubs[personalize-events]` - Type annotations for
   [PersonalizeEvents](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/)
   service.
 - `boto3-stubs[personalize-runtime]` - Type annotations for
@@ -1350,17 +1368,23 @@
   service.
 - `boto3-stubs[transfer]` - Type annotations for
   [Transfer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
   service.
 - `boto3-stubs[translate]` - Type annotations for
   [Translate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
   service.
+- `boto3-stubs[verifiedpermissions]` - Type annotations for
+  [VerifiedPermissions](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
+  service.
 - `boto3-stubs[voice-id]` - Type annotations for
   [VoiceID](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
   service.
+- `boto3-stubs[vpc-lattice]` - Type annotations for
+  [VPCLattice](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
+  service.
 - `boto3-stubs[waf]` - Type annotations for
   [WAF](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/) service.
 - `boto3-stubs[waf-regional]` - Type annotations for
   [WAFRegional](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
   service.
 - `boto3-stubs[wafv2]` - Type annotations for
   [WAFV2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
```

### Comparing `boto3-stubs-1.26.99/boto3-stubs/__init__.pyi` & `boto3-stubs-1.27.0/boto3-stubs/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from mypy_boto3_amplifybackend.client import AmplifyBackendClient
 from mypy_boto3_amplifyuibuilder.client import AmplifyUIBuilderClient
 from mypy_boto3_apigateway.client import APIGatewayClient
 from mypy_boto3_apigatewaymanagementapi.client import ApiGatewayManagementApiClient
 from mypy_boto3_apigatewayv2.client import ApiGatewayV2Client
 from mypy_boto3_appconfig.client import AppConfigClient
 from mypy_boto3_appconfigdata.client import AppConfigDataClient
+from mypy_boto3_appfabric.client import AppFabricClient
 from mypy_boto3_appflow.client import AppflowClient
 from mypy_boto3_appintegrations.client import AppIntegrationsServiceClient
 from mypy_boto3_application_autoscaling.client import ApplicationAutoScalingClient
 from mypy_boto3_application_insights.client import ApplicationInsightsClient
 from mypy_boto3_applicationcostprofiler.client import ApplicationCostProfilerClient
 from mypy_boto3_appmesh.client import AppMeshClient
 from mypy_boto3_apprunner.client import AppRunnerClient
@@ -65,14 +66,15 @@
 from mypy_boto3_cloudwatch.service_resource import CloudWatchServiceResource
 from mypy_boto3_codeartifact.client import CodeArtifactClient
 from mypy_boto3_codebuild.client import CodeBuildClient
 from mypy_boto3_codecatalyst.client import CodeCatalystClient
 from mypy_boto3_codecommit.client import CodeCommitClient
 from mypy_boto3_codedeploy.client import CodeDeployClient
 from mypy_boto3_codeguru_reviewer.client import CodeGuruReviewerClient
+from mypy_boto3_codeguru_security.client import CodeGuruSecurityClient
 from mypy_boto3_codeguruprofiler.client import CodeGuruProfilerClient
 from mypy_boto3_codepipeline.client import CodePipelineClient
 from mypy_boto3_codestar.client import CodeStarClient
 from mypy_boto3_codestar_connections.client import CodeStarconnectionsClient
 from mypy_boto3_codestar_notifications.client import CodeStarNotificationsClient
 from mypy_boto3_cognito_identity.client import CognitoIdentityClient
 from mypy_boto3_cognito_idp.client import CognitoIdentityProviderClient
@@ -222,14 +224,15 @@
 from mypy_boto3_marketplace_entitlement.client import MarketplaceEntitlementServiceClient
 from mypy_boto3_marketplacecommerceanalytics.client import MarketplaceCommerceAnalyticsClient
 from mypy_boto3_mediaconnect.client import MediaConnectClient
 from mypy_boto3_mediaconvert.client import MediaConvertClient
 from mypy_boto3_medialive.client import MediaLiveClient
 from mypy_boto3_mediapackage.client import MediaPackageClient
 from mypy_boto3_mediapackage_vod.client import MediaPackageVodClient
+from mypy_boto3_mediapackagev2.client import mediapackagev2Client
 from mypy_boto3_mediastore.client import MediaStoreClient
 from mypy_boto3_mediastore_data.client import MediaStoreDataClient
 from mypy_boto3_mediatailor.client import MediaTailorClient
 from mypy_boto3_memorydb.client import MemoryDBClient
 from mypy_boto3_meteringmarketplace.client import MarketplaceMeteringClient
 from mypy_boto3_mgh.client import MigrationHubClient
 from mypy_boto3_mgn.client import mgnClient
@@ -249,16 +252,19 @@
 from mypy_boto3_omics.client import OmicsClient
 from mypy_boto3_opensearch.client import OpenSearchServiceClient
 from mypy_boto3_opensearchserverless.client import OpenSearchServiceServerlessClient
 from mypy_boto3_opsworks.client import OpsWorksClient
 from mypy_boto3_opsworks.service_resource import OpsWorksServiceResource
 from mypy_boto3_opsworkscm.client import OpsWorksCMClient
 from mypy_boto3_organizations.client import OrganizationsClient
+from mypy_boto3_osis.client import OpenSearchIngestionClient
 from mypy_boto3_outposts.client import OutpostsClient
 from mypy_boto3_panorama.client import PanoramaClient
+from mypy_boto3_payment_cryptography.client import PaymentCryptographyControlPlaneClient
+from mypy_boto3_payment_cryptography_data.client import PaymentCryptographyDataPlaneClient
 from mypy_boto3_personalize.client import PersonalizeClient
 from mypy_boto3_personalize_events.client import PersonalizeEventsClient
 from mypy_boto3_personalize_runtime.client import PersonalizeRuntimeClient
 from mypy_boto3_pi.client import PIClient
 from mypy_boto3_pinpoint.client import PinpointClient
 from mypy_boto3_pinpoint_email.client import PinpointEmailClient
 from mypy_boto3_pinpoint_sms_voice.client import PinpointSMSVoiceClient
@@ -345,15 +351,17 @@
 from mypy_boto3_textract.client import TextractClient
 from mypy_boto3_timestream_query.client import TimestreamQueryClient
 from mypy_boto3_timestream_write.client import TimestreamWriteClient
 from mypy_boto3_tnb.client import TelcoNetworkBuilderClient
 from mypy_boto3_transcribe.client import TranscribeServiceClient
 from mypy_boto3_transfer.client import TransferClient
 from mypy_boto3_translate.client import TranslateClient
+from mypy_boto3_verifiedpermissions.client import VerifiedPermissionsClient
 from mypy_boto3_voice_id.client import VoiceIDClient
+from mypy_boto3_vpc_lattice.client import VPCLatticeClient
 from mypy_boto3_waf.client import WAFClient
 from mypy_boto3_waf_regional.client import WAFRegionalClient
 from mypy_boto3_wafv2.client import WAFV2Client
 from mypy_boto3_wellarchitected.client import WellArchitectedClient
 from mypy_boto3_wisdom.client import ConnectWisdomServiceClient
 from mypy_boto3_workdocs.client import WorkDocsClient
 from mypy_boto3_worklink.client import WorkLinkClient
@@ -568,14 +576,27 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> AppConfigDataClient: ...
 @overload
 def client(
+    service_name: Literal["appfabric"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> AppFabricClient: ...
+@overload
+def client(
     service_name: Literal["appflow"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
@@ -1179,14 +1200,27 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> CodeGuruReviewerClient: ...
 @overload
 def client(
+    service_name: Literal["codeguru-security"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> CodeGuruSecurityClient: ...
+@overload
+def client(
     service_name: Literal["codeguruprofiler"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
@@ -3116,14 +3150,27 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> MediaPackageVodClient: ...
 @overload
 def client(
+    service_name: Literal["mediapackagev2"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> mediapackagev2Client: ...
+@overload
+def client(
     service_name: Literal["mediastore"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
@@ -3454,14 +3501,27 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> OrganizationsClient: ...
 @overload
 def client(
+    service_name: Literal["osis"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> OpenSearchIngestionClient: ...
+@overload
+def client(
     service_name: Literal["outposts"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
@@ -3480,14 +3540,40 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> PanoramaClient: ...
 @overload
 def client(
+    service_name: Literal["payment-cryptography"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> PaymentCryptographyControlPlaneClient: ...
+@overload
+def client(
+    service_name: Literal["payment-cryptography-data"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> PaymentCryptographyDataPlaneClient: ...
+@overload
+def client(
     service_name: Literal["personalize"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
@@ -4663,27 +4749,53 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> TranslateClient: ...
 @overload
 def client(
+    service_name: Literal["verifiedpermissions"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> VerifiedPermissionsClient: ...
+@overload
+def client(
     service_name: Literal["voice-id"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> VoiceIDClient: ...
 @overload
 def client(
+    service_name: Literal["vpc-lattice"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> VPCLatticeClient: ...
+@overload
+def client(
     service_name: Literal["waf"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
```

### Comparing `boto3-stubs-1.26.99/boto3-stubs/docs/utils.pyi` & `boto3-stubs-1.27.0/boto3-stubs/docs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3-stubs/dynamodb/conditions.pyi` & `boto3-stubs-1.27.0/boto3-stubs/dynamodb/conditions.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3-stubs/dynamodb/table.pyi` & `boto3-stubs-1.27.0/boto3-stubs/dynamodb/table.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3-stubs/dynamodb/transform.pyi` & `boto3-stubs-1.27.0/boto3-stubs/dynamodb/transform.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3-stubs/dynamodb/types.pyi` & `boto3-stubs-1.27.0/boto3-stubs/dynamodb/types.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3-stubs/exceptions.pyi` & `boto3-stubs-1.27.0/boto3-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3-stubs/resources/action.pyi` & `boto3-stubs-1.27.0/boto3-stubs/resources/action.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3-stubs/resources/base.pyi` & `boto3-stubs-1.27.0/boto3-stubs/resources/base.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3-stubs/resources/collection.pyi` & `boto3-stubs-1.27.0/boto3-stubs/resources/collection.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3-stubs/resources/model.pyi` & `boto3-stubs-1.27.0/boto3-stubs/resources/model.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3-stubs/resources/params.pyi` & `boto3-stubs-1.27.0/boto3-stubs/resources/params.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3-stubs/resources/response.pyi` & `boto3-stubs-1.27.0/boto3-stubs/resources/response.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3-stubs/s3/inject.pyi` & `boto3-stubs-1.27.0/boto3-stubs/s3/inject.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3-stubs/s3/transfer.pyi` & `boto3-stubs-1.27.0/boto3-stubs/s3/transfer.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3-stubs/session.pyi` & `boto3-stubs-1.27.0/boto3-stubs/session.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import sys
-from typing import Any, List, Optional, Union, overload
+from typing import List, Optional, Union, overload
 
-import boto3
-import boto3.utils
-import botocore.session
 from boto3.exceptions import ResourceNotExistsError as ResourceNotExistsError
 from boto3.exceptions import UnknownAPIVersionError as UnknownAPIVersionError
 from boto3.resources.factory import ResourceFactory
-from botocore.client import Config
 from botocore.config import Config
 from botocore.credentials import Credentials
 from botocore.exceptions import DataNotFoundError as DataNotFoundError
 from botocore.exceptions import UnknownServiceError as UnknownServiceError
+from botocore.hooks import BaseEventHooks
 from botocore.loaders import Loader
 from botocore.model import ServiceModel as ServiceModel
+from botocore.session import Session as BotocoreSession
 from mypy_boto3_accessanalyzer.client import AccessAnalyzerClient
 from mypy_boto3_account.client import AccountClient
 from mypy_boto3_acm.client import ACMClient
 from mypy_boto3_acm_pca.client import ACMPCAClient
 from mypy_boto3_alexaforbusiness.client import AlexaForBusinessClient
 from mypy_boto3_amp.client import PrometheusServiceClient
 from mypy_boto3_amplify.client import AmplifyClient
 from mypy_boto3_amplifybackend.client import AmplifyBackendClient
 from mypy_boto3_amplifyuibuilder.client import AmplifyUIBuilderClient
 from mypy_boto3_apigateway.client import APIGatewayClient
 from mypy_boto3_apigatewaymanagementapi.client import ApiGatewayManagementApiClient
 from mypy_boto3_apigatewayv2.client import ApiGatewayV2Client
 from mypy_boto3_appconfig.client import AppConfigClient
 from mypy_boto3_appconfigdata.client import AppConfigDataClient
+from mypy_boto3_appfabric.client import AppFabricClient
 from mypy_boto3_appflow.client import AppflowClient
 from mypy_boto3_appintegrations.client import AppIntegrationsServiceClient
 from mypy_boto3_application_autoscaling.client import ApplicationAutoScalingClient
 from mypy_boto3_application_insights.client import ApplicationInsightsClient
 from mypy_boto3_applicationcostprofiler.client import ApplicationCostProfilerClient
 from mypy_boto3_appmesh.client import AppMeshClient
 from mypy_boto3_apprunner.client import AppRunnerClient
@@ -73,14 +72,15 @@
 from mypy_boto3_cloudwatch.service_resource import CloudWatchServiceResource
 from mypy_boto3_codeartifact.client import CodeArtifactClient
 from mypy_boto3_codebuild.client import CodeBuildClient
 from mypy_boto3_codecatalyst.client import CodeCatalystClient
 from mypy_boto3_codecommit.client import CodeCommitClient
 from mypy_boto3_codedeploy.client import CodeDeployClient
 from mypy_boto3_codeguru_reviewer.client import CodeGuruReviewerClient
+from mypy_boto3_codeguru_security.client import CodeGuruSecurityClient
 from mypy_boto3_codeguruprofiler.client import CodeGuruProfilerClient
 from mypy_boto3_codepipeline.client import CodePipelineClient
 from mypy_boto3_codestar.client import CodeStarClient
 from mypy_boto3_codestar_connections.client import CodeStarconnectionsClient
 from mypy_boto3_codestar_notifications.client import CodeStarNotificationsClient
 from mypy_boto3_cognito_identity.client import CognitoIdentityClient
 from mypy_boto3_cognito_idp.client import CognitoIdentityProviderClient
@@ -230,14 +230,15 @@
 from mypy_boto3_marketplace_entitlement.client import MarketplaceEntitlementServiceClient
 from mypy_boto3_marketplacecommerceanalytics.client import MarketplaceCommerceAnalyticsClient
 from mypy_boto3_mediaconnect.client import MediaConnectClient
 from mypy_boto3_mediaconvert.client import MediaConvertClient
 from mypy_boto3_medialive.client import MediaLiveClient
 from mypy_boto3_mediapackage.client import MediaPackageClient
 from mypy_boto3_mediapackage_vod.client import MediaPackageVodClient
+from mypy_boto3_mediapackagev2.client import mediapackagev2Client
 from mypy_boto3_mediastore.client import MediaStoreClient
 from mypy_boto3_mediastore_data.client import MediaStoreDataClient
 from mypy_boto3_mediatailor.client import MediaTailorClient
 from mypy_boto3_memorydb.client import MemoryDBClient
 from mypy_boto3_meteringmarketplace.client import MarketplaceMeteringClient
 from mypy_boto3_mgh.client import MigrationHubClient
 from mypy_boto3_mgn.client import mgnClient
@@ -257,16 +258,19 @@
 from mypy_boto3_omics.client import OmicsClient
 from mypy_boto3_opensearch.client import OpenSearchServiceClient
 from mypy_boto3_opensearchserverless.client import OpenSearchServiceServerlessClient
 from mypy_boto3_opsworks.client import OpsWorksClient
 from mypy_boto3_opsworks.service_resource import OpsWorksServiceResource
 from mypy_boto3_opsworkscm.client import OpsWorksCMClient
 from mypy_boto3_organizations.client import OrganizationsClient
+from mypy_boto3_osis.client import OpenSearchIngestionClient
 from mypy_boto3_outposts.client import OutpostsClient
 from mypy_boto3_panorama.client import PanoramaClient
+from mypy_boto3_payment_cryptography.client import PaymentCryptographyControlPlaneClient
+from mypy_boto3_payment_cryptography_data.client import PaymentCryptographyDataPlaneClient
 from mypy_boto3_personalize.client import PersonalizeClient
 from mypy_boto3_personalize_events.client import PersonalizeEventsClient
 from mypy_boto3_personalize_runtime.client import PersonalizeRuntimeClient
 from mypy_boto3_pi.client import PIClient
 from mypy_boto3_pinpoint.client import PinpointClient
 from mypy_boto3_pinpoint_email.client import PinpointEmailClient
 from mypy_boto3_pinpoint_sms_voice.client import PinpointSMSVoiceClient
@@ -353,15 +357,17 @@
 from mypy_boto3_textract.client import TextractClient
 from mypy_boto3_timestream_query.client import TimestreamQueryClient
 from mypy_boto3_timestream_write.client import TimestreamWriteClient
 from mypy_boto3_tnb.client import TelcoNetworkBuilderClient
 from mypy_boto3_transcribe.client import TranscribeServiceClient
 from mypy_boto3_transfer.client import TransferClient
 from mypy_boto3_translate.client import TranslateClient
+from mypy_boto3_verifiedpermissions.client import VerifiedPermissionsClient
 from mypy_boto3_voice_id.client import VoiceIDClient
+from mypy_boto3_vpc_lattice.client import VPCLatticeClient
 from mypy_boto3_waf.client import WAFClient
 from mypy_boto3_waf_regional.client import WAFRegionalClient
 from mypy_boto3_wafv2.client import WAFV2Client
 from mypy_boto3_wellarchitected.client import WellArchitectedClient
 from mypy_boto3_wisdom.client import ConnectWisdomServiceClient
 from mypy_boto3_workdocs.client import WorkDocsClient
 from mypy_boto3_worklink.client import WorkLinkClient
@@ -404,33 +410,33 @@
     "us-west-1",
     "us-west-2",
 ]
 
 class Session:
     def __init__(
         self,
-        aws_access_key_id: Optional[str] = None,
-        aws_secret_access_key: Optional[str] = None,
-        aws_session_token: Optional[str] = None,
-        region_name: Optional[str] = None,
-        botocore_session: Optional[BotocoreSession] = None,
-        profile_name: Optional[str] = None,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        region_name: Optional[str] = ...,
+        botocore_session: Optional[BotocoreSession] = ...,
+        profile_name: Optional[str] = ...,
     ) -> None:
         self._session: BotocoreSession
         self.resource_factory: ResourceFactory
         self._loader: Loader
     def __repr__(self) -> str: ...
     @property
     def profile_name(self) -> str: ...
     @property
     def region_name(self) -> _RegionName: ...
     @property
-    def events(self) -> List[Any]: ...
+    def events(self) -> BaseEventHooks: ...
     @property
-    def available_profiles(self) -> List[Any]: ...
+    def available_profiles(self) -> List[str]: ...
     def _setup_loader(self) -> None: ...
     def get_available_services(self) -> List[str]: ...
     def get_available_resources(self) -> List[str]: ...
     def get_available_partitions(self) -> List[str]: ...
     def get_available_regions(
         self,
         service_name: str,
@@ -635,14 +641,28 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> AppConfigDataClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["appfabric"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> AppFabricClient: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["appflow"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
@@ -1293,14 +1313,28 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> CodeGuruReviewerClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["codeguru-security"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> CodeGuruSecurityClient: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["codeguruprofiler"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
@@ -3379,14 +3413,28 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> MediaPackageVodClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["mediapackagev2"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> mediapackagev2Client: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["mediastore"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
@@ -3743,14 +3791,28 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> OrganizationsClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["osis"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> OpenSearchIngestionClient: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["outposts"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
@@ -3771,14 +3833,42 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> PanoramaClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["payment-cryptography"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> PaymentCryptographyControlPlaneClient: ...
+    @overload
+    def client(
+        self,
+        service_name: Literal["payment-cryptography-data"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> PaymentCryptographyDataPlaneClient: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["personalize"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
@@ -5045,28 +5135,56 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> TranslateClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["verifiedpermissions"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> VerifiedPermissionsClient: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["voice-id"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> VoiceIDClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["vpc-lattice"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> VPCLatticeClient: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["waf"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
```

### Comparing `boto3-stubs-1.26.99/boto3-stubs/utils.pyi` & `boto3-stubs-1.27.0/boto3-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3_stubs.egg-info/PKG-INFO` & `boto3-stubs-1.27.0/boto3_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boto3-stubs
-Version: 1.26.99
-Summary: Type annotations for boto3 1.26.99 generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3 1.27.0 generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -41,14 +41,15 @@
 Provides-Extra: amplifybackend
 Provides-Extra: amplifyuibuilder
 Provides-Extra: apigateway
 Provides-Extra: apigatewaymanagementapi
 Provides-Extra: apigatewayv2
 Provides-Extra: appconfig
 Provides-Extra: appconfigdata
+Provides-Extra: appfabric
 Provides-Extra: appflow
 Provides-Extra: appintegrations
 Provides-Extra: application-autoscaling
 Provides-Extra: application-insights
 Provides-Extra: applicationcostprofiler
 Provides-Extra: appmesh
 Provides-Extra: apprunner
@@ -88,14 +89,15 @@
 Provides-Extra: cloudwatch
 Provides-Extra: codeartifact
 Provides-Extra: codebuild
 Provides-Extra: codecatalyst
 Provides-Extra: codecommit
 Provides-Extra: codedeploy
 Provides-Extra: codeguru-reviewer
+Provides-Extra: codeguru-security
 Provides-Extra: codeguruprofiler
 Provides-Extra: codepipeline
 Provides-Extra: codestar
 Provides-Extra: codestar-connections
 Provides-Extra: codestar-notifications
 Provides-Extra: cognito-identity
 Provides-Extra: cognito-idp
@@ -237,14 +239,15 @@
 Provides-Extra: marketplace-entitlement
 Provides-Extra: marketplacecommerceanalytics
 Provides-Extra: mediaconnect
 Provides-Extra: mediaconvert
 Provides-Extra: medialive
 Provides-Extra: mediapackage
 Provides-Extra: mediapackage-vod
+Provides-Extra: mediapackagev2
 Provides-Extra: mediastore
 Provides-Extra: mediastore-data
 Provides-Extra: mediatailor
 Provides-Extra: memorydb
 Provides-Extra: meteringmarketplace
 Provides-Extra: mgh
 Provides-Extra: mgn
@@ -263,16 +266,19 @@
 Provides-Extra: oam
 Provides-Extra: omics
 Provides-Extra: opensearch
 Provides-Extra: opensearchserverless
 Provides-Extra: opsworks
 Provides-Extra: opsworkscm
 Provides-Extra: organizations
+Provides-Extra: osis
 Provides-Extra: outposts
 Provides-Extra: panorama
+Provides-Extra: payment-cryptography
+Provides-Extra: payment-cryptography-data
 Provides-Extra: personalize
 Provides-Extra: personalize-events
 Provides-Extra: personalize-runtime
 Provides-Extra: pi
 Provides-Extra: pinpoint
 Provides-Extra: pinpoint-email
 Provides-Extra: pinpoint-sms-voice
@@ -356,15 +362,17 @@
 Provides-Extra: textract
 Provides-Extra: timestream-query
 Provides-Extra: timestream-write
 Provides-Extra: tnb
 Provides-Extra: transcribe
 Provides-Extra: transfer
 Provides-Extra: translate
+Provides-Extra: verifiedpermissions
 Provides-Extra: voice-id
+Provides-Extra: vpc-lattice
 Provides-Extra: waf
 Provides-Extra: waf-regional
 Provides-Extra: wafv2
 Provides-Extra: wellarchitected
 Provides-Extra: wisdom
 Provides-Extra: workdocs
 Provides-Extra: worklink
@@ -377,30 +385,30 @@
 
 <a id="boto3-stubs"></a>
 
 # boto3-stubs
 
 [![PyPI - boto3-stubs](https://img.shields.io/pypi/v/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/boto3-stubs?color=blue)](https://pypistats.org/packages/boto3-stubs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.26.99](https://boto3.amazonaws.com/v1/documentation/api/1.26.99/index.html)
+[boto3 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/1.27.0/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [boto3-stubs docs](https://youtype.github.io/boto3_stubs_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
@@ -765,15 +773,15 @@
 in [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder/issues/)
 repository.
 
 <a id="submodules"></a>
 
 ## Submodules
 
-- `boto3-stubs[all]` - Type annotations for all 342 services.
+- `boto3-stubs[all]` - Type annotations for all 350 services.
 - `boto3-stubs[essential]` - Type annotations for
   [CloudFormation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/),
   [DynamoDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/),
   [EC2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/),
   [Lambda](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/),
   [RDS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/),
   [S3](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/) and
@@ -816,14 +824,17 @@
   service.
 - `boto3-stubs[appconfig]` - Type annotations for
   [AppConfig](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
   service.
 - `boto3-stubs[appconfigdata]` - Type annotations for
   [AppConfigData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/)
   service.
+- `boto3-stubs[appfabric]` - Type annotations for
+  [AppFabric](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/)
+  service.
 - `boto3-stubs[appflow]` - Type annotations for
   [Appflow](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/)
   service.
 - `boto3-stubs[appintegrations]` - Type annotations for
   [AppIntegrationsService](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
   service.
 - `boto3-stubs[application-autoscaling]` - Type annotations for
@@ -957,14 +968,17 @@
   service.
 - `boto3-stubs[codedeploy]` - Type annotations for
   [CodeDeploy](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
   service.
 - `boto3-stubs[codeguru-reviewer]` - Type annotations for
   [CodeGuruReviewer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
   service.
+- `boto3-stubs[codeguru-security]` - Type annotations for
+  [CodeGuruSecurity](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
+  service.
 - `boto3-stubs[codeguruprofiler]` - Type annotations for
   [CodeGuruProfiler](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguruprofiler/)
   service.
 - `boto3-stubs[codepipeline]` - Type annotations for
   [CodePipeline](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
   service.
 - `boto3-stubs[codestar]` - Type annotations for
@@ -1386,14 +1400,17 @@
   service.
 - `boto3-stubs[mediapackage]` - Type annotations for
   [MediaPackage](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
   service.
 - `boto3-stubs[mediapackage-vod]` - Type annotations for
   [MediaPackageVod](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
   service.
+- `boto3-stubs[mediapackagev2]` - Type annotations for
+  [mediapackagev2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
+  service.
 - `boto3-stubs[mediastore]` - Type annotations for
   [MediaStore](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
   service.
 - `boto3-stubs[mediastore-data]` - Type annotations for
   [MediaStoreData](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
   service.
 - `boto3-stubs[mediatailor]` - Type annotations for
@@ -1461,20 +1478,29 @@
   service.
 - `boto3-stubs[opsworkscm]` - Type annotations for
   [OpsWorksCM](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
   service.
 - `boto3-stubs[organizations]` - Type annotations for
   [Organizations](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_organizations/)
   service.
+- `boto3-stubs[osis]` - Type annotations for
+  [OpenSearchIngestion](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
+  service.
 - `boto3-stubs[outposts]` - Type annotations for
   [Outposts](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
   service.
 - `boto3-stubs[panorama]` - Type annotations for
   [Panorama](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
   service.
+- `boto3-stubs[payment-cryptography]` - Type annotations for
+  [PaymentCryptographyControlPlane](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/)
+  service.
+- `boto3-stubs[payment-cryptography-data]` - Type annotations for
+  [PaymentCryptographyDataPlane](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/)
+  service.
 - `boto3-stubs[personalize]` - Type annotations for
   [Personalize](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
   service.
 - `boto3-stubs[personalize-events]` - Type annotations for
   [PersonalizeEvents](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/)
   service.
 - `boto3-stubs[personalize-runtime]` - Type annotations for
@@ -1727,17 +1753,23 @@
   service.
 - `boto3-stubs[transfer]` - Type annotations for
   [Transfer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
   service.
 - `boto3-stubs[translate]` - Type annotations for
   [Translate](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
   service.
+- `boto3-stubs[verifiedpermissions]` - Type annotations for
+  [VerifiedPermissions](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
+  service.
 - `boto3-stubs[voice-id]` - Type annotations for
   [VoiceID](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
   service.
+- `boto3-stubs[vpc-lattice]` - Type annotations for
+  [VPCLattice](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_vpc_lattice/)
+  service.
 - `boto3-stubs[waf]` - Type annotations for
   [WAF](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/) service.
 - `boto3-stubs[waf-regional]` - Type annotations for
   [WAFRegional](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
   service.
 - `boto3-stubs[wafv2]` - Type annotations for
   [WAFV2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
```

### Comparing `boto3-stubs-1.26.99/boto3_stubs.egg-info/SOURCES.txt` & `boto3-stubs-1.27.0/boto3_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.26.99/boto3_stubs.egg-info/requires.txt` & `boto3-stubs-1.27.0/boto3_stubs.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,1388 +1,1420 @@
 botocore-stubs
 types-s3transfer
 
 [:python_version < "3.9"]
 typing-extensions>=4.1.0
 
 [accessanalyzer]
-mypy-boto3-accessanalyzer<1.27.0,>=1.26.0
+mypy-boto3-accessanalyzer<1.28.0,>=1.27.0
 
 [account]
-mypy-boto3-account<1.27.0,>=1.26.0
+mypy-boto3-account<1.28.0,>=1.27.0
 
 [acm]
-mypy-boto3-acm<1.27.0,>=1.26.0
+mypy-boto3-acm<1.28.0,>=1.27.0
 
 [acm-pca]
-mypy-boto3-acm-pca<1.27.0,>=1.26.0
+mypy-boto3-acm-pca<1.28.0,>=1.27.0
 
 [alexaforbusiness]
-mypy-boto3-alexaforbusiness<1.27.0,>=1.26.0
+mypy-boto3-alexaforbusiness<1.28.0,>=1.27.0
 
 [all]
-mypy-boto3-accessanalyzer<1.27.0,>=1.26.0
-mypy-boto3-account<1.27.0,>=1.26.0
-mypy-boto3-acm<1.27.0,>=1.26.0
-mypy-boto3-acm-pca<1.27.0,>=1.26.0
-mypy-boto3-alexaforbusiness<1.27.0,>=1.26.0
-mypy-boto3-amp<1.27.0,>=1.26.0
-mypy-boto3-amplify<1.27.0,>=1.26.0
-mypy-boto3-amplifybackend<1.27.0,>=1.26.0
-mypy-boto3-amplifyuibuilder<1.27.0,>=1.26.0
-mypy-boto3-apigateway<1.27.0,>=1.26.0
-mypy-boto3-apigatewaymanagementapi<1.27.0,>=1.26.0
-mypy-boto3-apigatewayv2<1.27.0,>=1.26.0
-mypy-boto3-appconfig<1.27.0,>=1.26.0
-mypy-boto3-appconfigdata<1.27.0,>=1.26.0
-mypy-boto3-appflow<1.27.0,>=1.26.0
-mypy-boto3-appintegrations<1.27.0,>=1.26.0
-mypy-boto3-application-autoscaling<1.27.0,>=1.26.0
-mypy-boto3-application-insights<1.27.0,>=1.26.0
-mypy-boto3-applicationcostprofiler<1.27.0,>=1.26.0
-mypy-boto3-appmesh<1.27.0,>=1.26.0
-mypy-boto3-apprunner<1.27.0,>=1.26.0
-mypy-boto3-appstream<1.27.0,>=1.26.0
-mypy-boto3-appsync<1.27.0,>=1.26.0
-mypy-boto3-arc-zonal-shift<1.27.0,>=1.26.0
-mypy-boto3-athena<1.27.0,>=1.26.0
-mypy-boto3-auditmanager<1.27.0,>=1.26.0
-mypy-boto3-autoscaling<1.27.0,>=1.26.0
-mypy-boto3-autoscaling-plans<1.27.0,>=1.26.0
-mypy-boto3-backup<1.27.0,>=1.26.0
-mypy-boto3-backup-gateway<1.27.0,>=1.26.0
-mypy-boto3-backupstorage<1.27.0,>=1.26.0
-mypy-boto3-batch<1.27.0,>=1.26.0
-mypy-boto3-billingconductor<1.27.0,>=1.26.0
-mypy-boto3-braket<1.27.0,>=1.26.0
-mypy-boto3-budgets<1.27.0,>=1.26.0
-mypy-boto3-ce<1.27.0,>=1.26.0
-mypy-boto3-chime<1.27.0,>=1.26.0
-mypy-boto3-chime-sdk-identity<1.27.0,>=1.26.0
-mypy-boto3-chime-sdk-media-pipelines<1.27.0,>=1.26.0
-mypy-boto3-chime-sdk-meetings<1.27.0,>=1.26.0
-mypy-boto3-chime-sdk-messaging<1.27.0,>=1.26.0
-mypy-boto3-chime-sdk-voice<1.27.0,>=1.26.0
-mypy-boto3-cleanrooms<1.27.0,>=1.26.0
-mypy-boto3-cloud9<1.27.0,>=1.26.0
-mypy-boto3-cloudcontrol<1.27.0,>=1.26.0
-mypy-boto3-clouddirectory<1.27.0,>=1.26.0
-mypy-boto3-cloudformation<1.27.0,>=1.26.0
-mypy-boto3-cloudfront<1.27.0,>=1.26.0
-mypy-boto3-cloudhsm<1.27.0,>=1.26.0
-mypy-boto3-cloudhsmv2<1.27.0,>=1.26.0
-mypy-boto3-cloudsearch<1.27.0,>=1.26.0
-mypy-boto3-cloudsearchdomain<1.27.0,>=1.26.0
-mypy-boto3-cloudtrail<1.27.0,>=1.26.0
-mypy-boto3-cloudtrail-data<1.27.0,>=1.26.0
-mypy-boto3-cloudwatch<1.27.0,>=1.26.0
-mypy-boto3-codeartifact<1.27.0,>=1.26.0
-mypy-boto3-codebuild<1.27.0,>=1.26.0
-mypy-boto3-codecatalyst<1.27.0,>=1.26.0
-mypy-boto3-codecommit<1.27.0,>=1.26.0
-mypy-boto3-codedeploy<1.27.0,>=1.26.0
-mypy-boto3-codeguru-reviewer<1.27.0,>=1.26.0
-mypy-boto3-codeguruprofiler<1.27.0,>=1.26.0
-mypy-boto3-codepipeline<1.27.0,>=1.26.0
-mypy-boto3-codestar<1.27.0,>=1.26.0
-mypy-boto3-codestar-connections<1.27.0,>=1.26.0
-mypy-boto3-codestar-notifications<1.27.0,>=1.26.0
-mypy-boto3-cognito-identity<1.27.0,>=1.26.0
-mypy-boto3-cognito-idp<1.27.0,>=1.26.0
-mypy-boto3-cognito-sync<1.27.0,>=1.26.0
-mypy-boto3-comprehend<1.27.0,>=1.26.0
-mypy-boto3-comprehendmedical<1.27.0,>=1.26.0
-mypy-boto3-compute-optimizer<1.27.0,>=1.26.0
-mypy-boto3-config<1.27.0,>=1.26.0
-mypy-boto3-connect<1.27.0,>=1.26.0
-mypy-boto3-connect-contact-lens<1.27.0,>=1.26.0
-mypy-boto3-connectcampaigns<1.27.0,>=1.26.0
-mypy-boto3-connectcases<1.27.0,>=1.26.0
-mypy-boto3-connectparticipant<1.27.0,>=1.26.0
-mypy-boto3-controltower<1.27.0,>=1.26.0
-mypy-boto3-cur<1.27.0,>=1.26.0
-mypy-boto3-customer-profiles<1.27.0,>=1.26.0
-mypy-boto3-databrew<1.27.0,>=1.26.0
-mypy-boto3-dataexchange<1.27.0,>=1.26.0
-mypy-boto3-datapipeline<1.27.0,>=1.26.0
-mypy-boto3-datasync<1.27.0,>=1.26.0
-mypy-boto3-dax<1.27.0,>=1.26.0
-mypy-boto3-detective<1.27.0,>=1.26.0
-mypy-boto3-devicefarm<1.27.0,>=1.26.0
-mypy-boto3-devops-guru<1.27.0,>=1.26.0
-mypy-boto3-directconnect<1.27.0,>=1.26.0
-mypy-boto3-discovery<1.27.0,>=1.26.0
-mypy-boto3-dlm<1.27.0,>=1.26.0
-mypy-boto3-dms<1.27.0,>=1.26.0
-mypy-boto3-docdb<1.27.0,>=1.26.0
-mypy-boto3-docdb-elastic<1.27.0,>=1.26.0
-mypy-boto3-drs<1.27.0,>=1.26.0
-mypy-boto3-ds<1.27.0,>=1.26.0
-mypy-boto3-dynamodb<1.27.0,>=1.26.0
-mypy-boto3-dynamodbstreams<1.27.0,>=1.26.0
-mypy-boto3-ebs<1.27.0,>=1.26.0
-mypy-boto3-ec2<1.27.0,>=1.26.0
-mypy-boto3-ec2-instance-connect<1.27.0,>=1.26.0
-mypy-boto3-ecr<1.27.0,>=1.26.0
-mypy-boto3-ecr-public<1.27.0,>=1.26.0
-mypy-boto3-ecs<1.27.0,>=1.26.0
-mypy-boto3-efs<1.27.0,>=1.26.0
-mypy-boto3-eks<1.27.0,>=1.26.0
-mypy-boto3-elastic-inference<1.27.0,>=1.26.0
-mypy-boto3-elasticache<1.27.0,>=1.26.0
-mypy-boto3-elasticbeanstalk<1.27.0,>=1.26.0
-mypy-boto3-elastictranscoder<1.27.0,>=1.26.0
-mypy-boto3-elb<1.27.0,>=1.26.0
-mypy-boto3-elbv2<1.27.0,>=1.26.0
-mypy-boto3-emr<1.27.0,>=1.26.0
-mypy-boto3-emr-containers<1.27.0,>=1.26.0
-mypy-boto3-emr-serverless<1.27.0,>=1.26.0
-mypy-boto3-es<1.27.0,>=1.26.0
-mypy-boto3-events<1.27.0,>=1.26.0
-mypy-boto3-evidently<1.27.0,>=1.26.0
-mypy-boto3-finspace<1.27.0,>=1.26.0
-mypy-boto3-finspace-data<1.27.0,>=1.26.0
-mypy-boto3-firehose<1.27.0,>=1.26.0
-mypy-boto3-fis<1.27.0,>=1.26.0
-mypy-boto3-fms<1.27.0,>=1.26.0
-mypy-boto3-forecast<1.27.0,>=1.26.0
-mypy-boto3-forecastquery<1.27.0,>=1.26.0
-mypy-boto3-frauddetector<1.27.0,>=1.26.0
-mypy-boto3-fsx<1.27.0,>=1.26.0
-mypy-boto3-gamelift<1.27.0,>=1.26.0
-mypy-boto3-gamesparks<1.27.0,>=1.26.0
-mypy-boto3-glacier<1.27.0,>=1.26.0
-mypy-boto3-globalaccelerator<1.27.0,>=1.26.0
-mypy-boto3-glue<1.27.0,>=1.26.0
-mypy-boto3-grafana<1.27.0,>=1.26.0
-mypy-boto3-greengrass<1.27.0,>=1.26.0
-mypy-boto3-greengrassv2<1.27.0,>=1.26.0
-mypy-boto3-groundstation<1.27.0,>=1.26.0
-mypy-boto3-guardduty<1.27.0,>=1.26.0
-mypy-boto3-health<1.27.0,>=1.26.0
-mypy-boto3-healthlake<1.27.0,>=1.26.0
-mypy-boto3-honeycode<1.27.0,>=1.26.0
-mypy-boto3-iam<1.27.0,>=1.26.0
-mypy-boto3-identitystore<1.27.0,>=1.26.0
-mypy-boto3-imagebuilder<1.27.0,>=1.26.0
-mypy-boto3-importexport<1.27.0,>=1.26.0
-mypy-boto3-inspector<1.27.0,>=1.26.0
-mypy-boto3-inspector2<1.27.0,>=1.26.0
-mypy-boto3-internetmonitor<1.27.0,>=1.26.0
-mypy-boto3-iot<1.27.0,>=1.26.0
-mypy-boto3-iot-data<1.27.0,>=1.26.0
-mypy-boto3-iot-jobs-data<1.27.0,>=1.26.0
-mypy-boto3-iot-roborunner<1.27.0,>=1.26.0
-mypy-boto3-iot1click-devices<1.27.0,>=1.26.0
-mypy-boto3-iot1click-projects<1.27.0,>=1.26.0
-mypy-boto3-iotanalytics<1.27.0,>=1.26.0
-mypy-boto3-iotdeviceadvisor<1.27.0,>=1.26.0
-mypy-boto3-iotevents<1.27.0,>=1.26.0
-mypy-boto3-iotevents-data<1.27.0,>=1.26.0
-mypy-boto3-iotfleethub<1.27.0,>=1.26.0
-mypy-boto3-iotfleetwise<1.27.0,>=1.26.0
-mypy-boto3-iotsecuretunneling<1.27.0,>=1.26.0
-mypy-boto3-iotsitewise<1.27.0,>=1.26.0
-mypy-boto3-iotthingsgraph<1.27.0,>=1.26.0
-mypy-boto3-iottwinmaker<1.27.0,>=1.26.0
-mypy-boto3-iotwireless<1.27.0,>=1.26.0
-mypy-boto3-ivs<1.27.0,>=1.26.0
-mypy-boto3-ivs-realtime<1.27.0,>=1.26.0
-mypy-boto3-ivschat<1.27.0,>=1.26.0
-mypy-boto3-kafka<1.27.0,>=1.26.0
-mypy-boto3-kafkaconnect<1.27.0,>=1.26.0
-mypy-boto3-kendra<1.27.0,>=1.26.0
-mypy-boto3-kendra-ranking<1.27.0,>=1.26.0
-mypy-boto3-keyspaces<1.27.0,>=1.26.0
-mypy-boto3-kinesis<1.27.0,>=1.26.0
-mypy-boto3-kinesis-video-archived-media<1.27.0,>=1.26.0
-mypy-boto3-kinesis-video-media<1.27.0,>=1.26.0
-mypy-boto3-kinesis-video-signaling<1.27.0,>=1.26.0
-mypy-boto3-kinesis-video-webrtc-storage<1.27.0,>=1.26.0
-mypy-boto3-kinesisanalytics<1.27.0,>=1.26.0
-mypy-boto3-kinesisanalyticsv2<1.27.0,>=1.26.0
-mypy-boto3-kinesisvideo<1.27.0,>=1.26.0
-mypy-boto3-kms<1.27.0,>=1.26.0
-mypy-boto3-lakeformation<1.27.0,>=1.26.0
-mypy-boto3-lambda<1.27.0,>=1.26.0
-mypy-boto3-lex-models<1.27.0,>=1.26.0
-mypy-boto3-lex-runtime<1.27.0,>=1.26.0
-mypy-boto3-lexv2-models<1.27.0,>=1.26.0
-mypy-boto3-lexv2-runtime<1.27.0,>=1.26.0
-mypy-boto3-license-manager<1.27.0,>=1.26.0
-mypy-boto3-license-manager-linux-subscriptions<1.27.0,>=1.26.0
-mypy-boto3-license-manager-user-subscriptions<1.27.0,>=1.26.0
-mypy-boto3-lightsail<1.27.0,>=1.26.0
-mypy-boto3-location<1.27.0,>=1.26.0
-mypy-boto3-logs<1.27.0,>=1.26.0
-mypy-boto3-lookoutequipment<1.27.0,>=1.26.0
-mypy-boto3-lookoutmetrics<1.27.0,>=1.26.0
-mypy-boto3-lookoutvision<1.27.0,>=1.26.0
-mypy-boto3-m2<1.27.0,>=1.26.0
-mypy-boto3-machinelearning<1.27.0,>=1.26.0
-mypy-boto3-macie<1.27.0,>=1.26.0
-mypy-boto3-macie2<1.27.0,>=1.26.0
-mypy-boto3-managedblockchain<1.27.0,>=1.26.0
-mypy-boto3-marketplace-catalog<1.27.0,>=1.26.0
-mypy-boto3-marketplace-entitlement<1.27.0,>=1.26.0
-mypy-boto3-marketplacecommerceanalytics<1.27.0,>=1.26.0
-mypy-boto3-mediaconnect<1.27.0,>=1.26.0
-mypy-boto3-mediaconvert<1.27.0,>=1.26.0
-mypy-boto3-medialive<1.27.0,>=1.26.0
-mypy-boto3-mediapackage<1.27.0,>=1.26.0
-mypy-boto3-mediapackage-vod<1.27.0,>=1.26.0
-mypy-boto3-mediastore<1.27.0,>=1.26.0
-mypy-boto3-mediastore-data<1.27.0,>=1.26.0
-mypy-boto3-mediatailor<1.27.0,>=1.26.0
-mypy-boto3-memorydb<1.27.0,>=1.26.0
-mypy-boto3-meteringmarketplace<1.27.0,>=1.26.0
-mypy-boto3-mgh<1.27.0,>=1.26.0
-mypy-boto3-mgn<1.27.0,>=1.26.0
-mypy-boto3-migration-hub-refactor-spaces<1.27.0,>=1.26.0
-mypy-boto3-migrationhub-config<1.27.0,>=1.26.0
-mypy-boto3-migrationhuborchestrator<1.27.0,>=1.26.0
-mypy-boto3-migrationhubstrategy<1.27.0,>=1.26.0
-mypy-boto3-mobile<1.27.0,>=1.26.0
-mypy-boto3-mq<1.27.0,>=1.26.0
-mypy-boto3-mturk<1.27.0,>=1.26.0
-mypy-boto3-mwaa<1.27.0,>=1.26.0
-mypy-boto3-neptune<1.27.0,>=1.26.0
-mypy-boto3-network-firewall<1.27.0,>=1.26.0
-mypy-boto3-networkmanager<1.27.0,>=1.26.0
-mypy-boto3-nimble<1.27.0,>=1.26.0
-mypy-boto3-oam<1.27.0,>=1.26.0
-mypy-boto3-omics<1.27.0,>=1.26.0
-mypy-boto3-opensearch<1.27.0,>=1.26.0
-mypy-boto3-opensearchserverless<1.27.0,>=1.26.0
-mypy-boto3-opsworks<1.27.0,>=1.26.0
-mypy-boto3-opsworkscm<1.27.0,>=1.26.0
-mypy-boto3-organizations<1.27.0,>=1.26.0
-mypy-boto3-outposts<1.27.0,>=1.26.0
-mypy-boto3-panorama<1.27.0,>=1.26.0
-mypy-boto3-personalize<1.27.0,>=1.26.0
-mypy-boto3-personalize-events<1.27.0,>=1.26.0
-mypy-boto3-personalize-runtime<1.27.0,>=1.26.0
-mypy-boto3-pi<1.27.0,>=1.26.0
-mypy-boto3-pinpoint<1.27.0,>=1.26.0
-mypy-boto3-pinpoint-email<1.27.0,>=1.26.0
-mypy-boto3-pinpoint-sms-voice<1.27.0,>=1.26.0
-mypy-boto3-pinpoint-sms-voice-v2<1.27.0,>=1.26.0
-mypy-boto3-pipes<1.27.0,>=1.26.0
-mypy-boto3-polly<1.27.0,>=1.26.0
-mypy-boto3-pricing<1.27.0,>=1.26.0
-mypy-boto3-privatenetworks<1.27.0,>=1.26.0
-mypy-boto3-proton<1.27.0,>=1.26.0
-mypy-boto3-qldb<1.27.0,>=1.26.0
-mypy-boto3-qldb-session<1.27.0,>=1.26.0
-mypy-boto3-quicksight<1.27.0,>=1.26.0
-mypy-boto3-ram<1.27.0,>=1.26.0
-mypy-boto3-rbin<1.27.0,>=1.26.0
-mypy-boto3-rds<1.27.0,>=1.26.0
-mypy-boto3-rds-data<1.27.0,>=1.26.0
-mypy-boto3-redshift<1.27.0,>=1.26.0
-mypy-boto3-redshift-data<1.27.0,>=1.26.0
-mypy-boto3-redshift-serverless<1.27.0,>=1.26.0
-mypy-boto3-rekognition<1.27.0,>=1.26.0
-mypy-boto3-resiliencehub<1.27.0,>=1.26.0
-mypy-boto3-resource-explorer-2<1.27.0,>=1.26.0
-mypy-boto3-resource-groups<1.27.0,>=1.26.0
-mypy-boto3-resourcegroupstaggingapi<1.27.0,>=1.26.0
-mypy-boto3-robomaker<1.27.0,>=1.26.0
-mypy-boto3-rolesanywhere<1.27.0,>=1.26.0
-mypy-boto3-route53<1.27.0,>=1.26.0
-mypy-boto3-route53-recovery-cluster<1.27.0,>=1.26.0
-mypy-boto3-route53-recovery-control-config<1.27.0,>=1.26.0
-mypy-boto3-route53-recovery-readiness<1.27.0,>=1.26.0
-mypy-boto3-route53domains<1.27.0,>=1.26.0
-mypy-boto3-route53resolver<1.27.0,>=1.26.0
-mypy-boto3-rum<1.27.0,>=1.26.0
-mypy-boto3-s3<1.27.0,>=1.26.0
-mypy-boto3-s3control<1.27.0,>=1.26.0
-mypy-boto3-s3outposts<1.27.0,>=1.26.0
-mypy-boto3-sagemaker<1.27.0,>=1.26.0
-mypy-boto3-sagemaker-a2i-runtime<1.27.0,>=1.26.0
-mypy-boto3-sagemaker-edge<1.27.0,>=1.26.0
-mypy-boto3-sagemaker-featurestore-runtime<1.27.0,>=1.26.0
-mypy-boto3-sagemaker-geospatial<1.27.0,>=1.26.0
-mypy-boto3-sagemaker-metrics<1.27.0,>=1.26.0
-mypy-boto3-sagemaker-runtime<1.27.0,>=1.26.0
-mypy-boto3-savingsplans<1.27.0,>=1.26.0
-mypy-boto3-scheduler<1.27.0,>=1.26.0
-mypy-boto3-schemas<1.27.0,>=1.26.0
-mypy-boto3-sdb<1.27.0,>=1.26.0
-mypy-boto3-secretsmanager<1.27.0,>=1.26.0
-mypy-boto3-securityhub<1.27.0,>=1.26.0
-mypy-boto3-securitylake<1.27.0,>=1.26.0
-mypy-boto3-serverlessrepo<1.27.0,>=1.26.0
-mypy-boto3-service-quotas<1.27.0,>=1.26.0
-mypy-boto3-servicecatalog<1.27.0,>=1.26.0
-mypy-boto3-servicecatalog-appregistry<1.27.0,>=1.26.0
-mypy-boto3-servicediscovery<1.27.0,>=1.26.0
-mypy-boto3-ses<1.27.0,>=1.26.0
-mypy-boto3-sesv2<1.27.0,>=1.26.0
-mypy-boto3-shield<1.27.0,>=1.26.0
-mypy-boto3-signer<1.27.0,>=1.26.0
-mypy-boto3-simspaceweaver<1.27.0,>=1.26.0
-mypy-boto3-sms<1.27.0,>=1.26.0
-mypy-boto3-sms-voice<1.27.0,>=1.26.0
-mypy-boto3-snow-device-management<1.27.0,>=1.26.0
-mypy-boto3-snowball<1.27.0,>=1.26.0
-mypy-boto3-sns<1.27.0,>=1.26.0
-mypy-boto3-sqs<1.27.0,>=1.26.0
-mypy-boto3-ssm<1.27.0,>=1.26.0
-mypy-boto3-ssm-contacts<1.27.0,>=1.26.0
-mypy-boto3-ssm-incidents<1.27.0,>=1.26.0
-mypy-boto3-ssm-sap<1.27.0,>=1.26.0
-mypy-boto3-sso<1.27.0,>=1.26.0
-mypy-boto3-sso-admin<1.27.0,>=1.26.0
-mypy-boto3-sso-oidc<1.27.0,>=1.26.0
-mypy-boto3-stepfunctions<1.27.0,>=1.26.0
-mypy-boto3-storagegateway<1.27.0,>=1.26.0
-mypy-boto3-sts<1.27.0,>=1.26.0
-mypy-boto3-support<1.27.0,>=1.26.0
-mypy-boto3-support-app<1.27.0,>=1.26.0
-mypy-boto3-swf<1.27.0,>=1.26.0
-mypy-boto3-synthetics<1.27.0,>=1.26.0
-mypy-boto3-textract<1.27.0,>=1.26.0
-mypy-boto3-timestream-query<1.27.0,>=1.26.0
-mypy-boto3-timestream-write<1.27.0,>=1.26.0
-mypy-boto3-tnb<1.27.0,>=1.26.0
-mypy-boto3-transcribe<1.27.0,>=1.26.0
-mypy-boto3-transfer<1.27.0,>=1.26.0
-mypy-boto3-translate<1.27.0,>=1.26.0
-mypy-boto3-voice-id<1.27.0,>=1.26.0
-mypy-boto3-waf<1.27.0,>=1.26.0
-mypy-boto3-waf-regional<1.27.0,>=1.26.0
-mypy-boto3-wafv2<1.27.0,>=1.26.0
-mypy-boto3-wellarchitected<1.27.0,>=1.26.0
-mypy-boto3-wisdom<1.27.0,>=1.26.0
-mypy-boto3-workdocs<1.27.0,>=1.26.0
-mypy-boto3-worklink<1.27.0,>=1.26.0
-mypy-boto3-workmail<1.27.0,>=1.26.0
-mypy-boto3-workmailmessageflow<1.27.0,>=1.26.0
-mypy-boto3-workspaces<1.27.0,>=1.26.0
-mypy-boto3-workspaces-web<1.27.0,>=1.26.0
-mypy-boto3-xray<1.27.0,>=1.26.0
+mypy-boto3-accessanalyzer<1.28.0,>=1.27.0
+mypy-boto3-account<1.28.0,>=1.27.0
+mypy-boto3-acm<1.28.0,>=1.27.0
+mypy-boto3-acm-pca<1.28.0,>=1.27.0
+mypy-boto3-alexaforbusiness<1.28.0,>=1.27.0
+mypy-boto3-amp<1.28.0,>=1.27.0
+mypy-boto3-amplify<1.28.0,>=1.27.0
+mypy-boto3-amplifybackend<1.28.0,>=1.27.0
+mypy-boto3-amplifyuibuilder<1.28.0,>=1.27.0
+mypy-boto3-apigateway<1.28.0,>=1.27.0
+mypy-boto3-apigatewaymanagementapi<1.28.0,>=1.27.0
+mypy-boto3-apigatewayv2<1.28.0,>=1.27.0
+mypy-boto3-appconfig<1.28.0,>=1.27.0
+mypy-boto3-appconfigdata<1.28.0,>=1.27.0
+mypy-boto3-appfabric<1.28.0,>=1.27.0
+mypy-boto3-appflow<1.28.0,>=1.27.0
+mypy-boto3-appintegrations<1.28.0,>=1.27.0
+mypy-boto3-application-autoscaling<1.28.0,>=1.27.0
+mypy-boto3-application-insights<1.28.0,>=1.27.0
+mypy-boto3-applicationcostprofiler<1.28.0,>=1.27.0
+mypy-boto3-appmesh<1.28.0,>=1.27.0
+mypy-boto3-apprunner<1.28.0,>=1.27.0
+mypy-boto3-appstream<1.28.0,>=1.27.0
+mypy-boto3-appsync<1.28.0,>=1.27.0
+mypy-boto3-arc-zonal-shift<1.28.0,>=1.27.0
+mypy-boto3-athena<1.28.0,>=1.27.0
+mypy-boto3-auditmanager<1.28.0,>=1.27.0
+mypy-boto3-autoscaling<1.28.0,>=1.27.0
+mypy-boto3-autoscaling-plans<1.28.0,>=1.27.0
+mypy-boto3-backup<1.28.0,>=1.27.0
+mypy-boto3-backup-gateway<1.28.0,>=1.27.0
+mypy-boto3-backupstorage<1.28.0,>=1.27.0
+mypy-boto3-batch<1.28.0,>=1.27.0
+mypy-boto3-billingconductor<1.28.0,>=1.27.0
+mypy-boto3-braket<1.28.0,>=1.27.0
+mypy-boto3-budgets<1.28.0,>=1.27.0
+mypy-boto3-ce<1.28.0,>=1.27.0
+mypy-boto3-chime<1.28.0,>=1.27.0
+mypy-boto3-chime-sdk-identity<1.28.0,>=1.27.0
+mypy-boto3-chime-sdk-media-pipelines<1.28.0,>=1.27.0
+mypy-boto3-chime-sdk-meetings<1.28.0,>=1.27.0
+mypy-boto3-chime-sdk-messaging<1.28.0,>=1.27.0
+mypy-boto3-chime-sdk-voice<1.28.0,>=1.27.0
+mypy-boto3-cleanrooms<1.28.0,>=1.27.0
+mypy-boto3-cloud9<1.28.0,>=1.27.0
+mypy-boto3-cloudcontrol<1.28.0,>=1.27.0
+mypy-boto3-clouddirectory<1.28.0,>=1.27.0
+mypy-boto3-cloudformation<1.28.0,>=1.27.0
+mypy-boto3-cloudfront<1.28.0,>=1.27.0
+mypy-boto3-cloudhsm<1.28.0,>=1.27.0
+mypy-boto3-cloudhsmv2<1.28.0,>=1.27.0
+mypy-boto3-cloudsearch<1.28.0,>=1.27.0
+mypy-boto3-cloudsearchdomain<1.28.0,>=1.27.0
+mypy-boto3-cloudtrail<1.28.0,>=1.27.0
+mypy-boto3-cloudtrail-data<1.28.0,>=1.27.0
+mypy-boto3-cloudwatch<1.28.0,>=1.27.0
+mypy-boto3-codeartifact<1.28.0,>=1.27.0
+mypy-boto3-codebuild<1.28.0,>=1.27.0
+mypy-boto3-codecatalyst<1.28.0,>=1.27.0
+mypy-boto3-codecommit<1.28.0,>=1.27.0
+mypy-boto3-codedeploy<1.28.0,>=1.27.0
+mypy-boto3-codeguru-reviewer<1.28.0,>=1.27.0
+mypy-boto3-codeguru-security<1.28.0,>=1.27.0
+mypy-boto3-codeguruprofiler<1.28.0,>=1.27.0
+mypy-boto3-codepipeline<1.28.0,>=1.27.0
+mypy-boto3-codestar<1.28.0,>=1.27.0
+mypy-boto3-codestar-connections<1.28.0,>=1.27.0
+mypy-boto3-codestar-notifications<1.28.0,>=1.27.0
+mypy-boto3-cognito-identity<1.28.0,>=1.27.0
+mypy-boto3-cognito-idp<1.28.0,>=1.27.0
+mypy-boto3-cognito-sync<1.28.0,>=1.27.0
+mypy-boto3-comprehend<1.28.0,>=1.27.0
+mypy-boto3-comprehendmedical<1.28.0,>=1.27.0
+mypy-boto3-compute-optimizer<1.28.0,>=1.27.0
+mypy-boto3-config<1.28.0,>=1.27.0
+mypy-boto3-connect<1.28.0,>=1.27.0
+mypy-boto3-connect-contact-lens<1.28.0,>=1.27.0
+mypy-boto3-connectcampaigns<1.28.0,>=1.27.0
+mypy-boto3-connectcases<1.28.0,>=1.27.0
+mypy-boto3-connectparticipant<1.28.0,>=1.27.0
+mypy-boto3-controltower<1.28.0,>=1.27.0
+mypy-boto3-cur<1.28.0,>=1.27.0
+mypy-boto3-customer-profiles<1.28.0,>=1.27.0
+mypy-boto3-databrew<1.28.0,>=1.27.0
+mypy-boto3-dataexchange<1.28.0,>=1.27.0
+mypy-boto3-datapipeline<1.28.0,>=1.27.0
+mypy-boto3-datasync<1.28.0,>=1.27.0
+mypy-boto3-dax<1.28.0,>=1.27.0
+mypy-boto3-detective<1.28.0,>=1.27.0
+mypy-boto3-devicefarm<1.28.0,>=1.27.0
+mypy-boto3-devops-guru<1.28.0,>=1.27.0
+mypy-boto3-directconnect<1.28.0,>=1.27.0
+mypy-boto3-discovery<1.28.0,>=1.27.0
+mypy-boto3-dlm<1.28.0,>=1.27.0
+mypy-boto3-dms<1.28.0,>=1.27.0
+mypy-boto3-docdb<1.28.0,>=1.27.0
+mypy-boto3-docdb-elastic<1.28.0,>=1.27.0
+mypy-boto3-drs<1.28.0,>=1.27.0
+mypy-boto3-ds<1.28.0,>=1.27.0
+mypy-boto3-dynamodb<1.28.0,>=1.27.0
+mypy-boto3-dynamodbstreams<1.28.0,>=1.27.0
+mypy-boto3-ebs<1.28.0,>=1.27.0
+mypy-boto3-ec2<1.28.0,>=1.27.0
+mypy-boto3-ec2-instance-connect<1.28.0,>=1.27.0
+mypy-boto3-ecr<1.28.0,>=1.27.0
+mypy-boto3-ecr-public<1.28.0,>=1.27.0
+mypy-boto3-ecs<1.28.0,>=1.27.0
+mypy-boto3-efs<1.28.0,>=1.27.0
+mypy-boto3-eks<1.28.0,>=1.27.0
+mypy-boto3-elastic-inference<1.28.0,>=1.27.0
+mypy-boto3-elasticache<1.28.0,>=1.27.0
+mypy-boto3-elasticbeanstalk<1.28.0,>=1.27.0
+mypy-boto3-elastictranscoder<1.28.0,>=1.27.0
+mypy-boto3-elb<1.28.0,>=1.27.0
+mypy-boto3-elbv2<1.28.0,>=1.27.0
+mypy-boto3-emr<1.28.0,>=1.27.0
+mypy-boto3-emr-containers<1.28.0,>=1.27.0
+mypy-boto3-emr-serverless<1.28.0,>=1.27.0
+mypy-boto3-es<1.28.0,>=1.27.0
+mypy-boto3-events<1.28.0,>=1.27.0
+mypy-boto3-evidently<1.28.0,>=1.27.0
+mypy-boto3-finspace<1.28.0,>=1.27.0
+mypy-boto3-finspace-data<1.28.0,>=1.27.0
+mypy-boto3-firehose<1.28.0,>=1.27.0
+mypy-boto3-fis<1.28.0,>=1.27.0
+mypy-boto3-fms<1.28.0,>=1.27.0
+mypy-boto3-forecast<1.28.0,>=1.27.0
+mypy-boto3-forecastquery<1.28.0,>=1.27.0
+mypy-boto3-frauddetector<1.28.0,>=1.27.0
+mypy-boto3-fsx<1.28.0,>=1.27.0
+mypy-boto3-gamelift<1.28.0,>=1.27.0
+mypy-boto3-gamesparks<1.28.0,>=1.27.0
+mypy-boto3-glacier<1.28.0,>=1.27.0
+mypy-boto3-globalaccelerator<1.28.0,>=1.27.0
+mypy-boto3-glue<1.28.0,>=1.27.0
+mypy-boto3-grafana<1.28.0,>=1.27.0
+mypy-boto3-greengrass<1.28.0,>=1.27.0
+mypy-boto3-greengrassv2<1.28.0,>=1.27.0
+mypy-boto3-groundstation<1.28.0,>=1.27.0
+mypy-boto3-guardduty<1.28.0,>=1.27.0
+mypy-boto3-health<1.28.0,>=1.27.0
+mypy-boto3-healthlake<1.28.0,>=1.27.0
+mypy-boto3-honeycode<1.28.0,>=1.27.0
+mypy-boto3-iam<1.28.0,>=1.27.0
+mypy-boto3-identitystore<1.28.0,>=1.27.0
+mypy-boto3-imagebuilder<1.28.0,>=1.27.0
+mypy-boto3-importexport<1.28.0,>=1.27.0
+mypy-boto3-inspector<1.28.0,>=1.27.0
+mypy-boto3-inspector2<1.28.0,>=1.27.0
+mypy-boto3-internetmonitor<1.28.0,>=1.27.0
+mypy-boto3-iot<1.28.0,>=1.27.0
+mypy-boto3-iot-data<1.28.0,>=1.27.0
+mypy-boto3-iot-jobs-data<1.28.0,>=1.27.0
+mypy-boto3-iot-roborunner<1.28.0,>=1.27.0
+mypy-boto3-iot1click-devices<1.28.0,>=1.27.0
+mypy-boto3-iot1click-projects<1.28.0,>=1.27.0
+mypy-boto3-iotanalytics<1.28.0,>=1.27.0
+mypy-boto3-iotdeviceadvisor<1.28.0,>=1.27.0
+mypy-boto3-iotevents<1.28.0,>=1.27.0
+mypy-boto3-iotevents-data<1.28.0,>=1.27.0
+mypy-boto3-iotfleethub<1.28.0,>=1.27.0
+mypy-boto3-iotfleetwise<1.28.0,>=1.27.0
+mypy-boto3-iotsecuretunneling<1.28.0,>=1.27.0
+mypy-boto3-iotsitewise<1.28.0,>=1.27.0
+mypy-boto3-iotthingsgraph<1.28.0,>=1.27.0
+mypy-boto3-iottwinmaker<1.28.0,>=1.27.0
+mypy-boto3-iotwireless<1.28.0,>=1.27.0
+mypy-boto3-ivs<1.28.0,>=1.27.0
+mypy-boto3-ivs-realtime<1.28.0,>=1.27.0
+mypy-boto3-ivschat<1.28.0,>=1.27.0
+mypy-boto3-kafka<1.28.0,>=1.27.0
+mypy-boto3-kafkaconnect<1.28.0,>=1.27.0
+mypy-boto3-kendra<1.28.0,>=1.27.0
+mypy-boto3-kendra-ranking<1.28.0,>=1.27.0
+mypy-boto3-keyspaces<1.28.0,>=1.27.0
+mypy-boto3-kinesis<1.28.0,>=1.27.0
+mypy-boto3-kinesis-video-archived-media<1.28.0,>=1.27.0
+mypy-boto3-kinesis-video-media<1.28.0,>=1.27.0
+mypy-boto3-kinesis-video-signaling<1.28.0,>=1.27.0
+mypy-boto3-kinesis-video-webrtc-storage<1.28.0,>=1.27.0
+mypy-boto3-kinesisanalytics<1.28.0,>=1.27.0
+mypy-boto3-kinesisanalyticsv2<1.28.0,>=1.27.0
+mypy-boto3-kinesisvideo<1.28.0,>=1.27.0
+mypy-boto3-kms<1.28.0,>=1.27.0
+mypy-boto3-lakeformation<1.28.0,>=1.27.0
+mypy-boto3-lambda<1.28.0,>=1.27.0
+mypy-boto3-lex-models<1.28.0,>=1.27.0
+mypy-boto3-lex-runtime<1.28.0,>=1.27.0
+mypy-boto3-lexv2-models<1.28.0,>=1.27.0
+mypy-boto3-lexv2-runtime<1.28.0,>=1.27.0
+mypy-boto3-license-manager<1.28.0,>=1.27.0
+mypy-boto3-license-manager-linux-subscriptions<1.28.0,>=1.27.0
+mypy-boto3-license-manager-user-subscriptions<1.28.0,>=1.27.0
+mypy-boto3-lightsail<1.28.0,>=1.27.0
+mypy-boto3-location<1.28.0,>=1.27.0
+mypy-boto3-logs<1.28.0,>=1.27.0
+mypy-boto3-lookoutequipment<1.28.0,>=1.27.0
+mypy-boto3-lookoutmetrics<1.28.0,>=1.27.0
+mypy-boto3-lookoutvision<1.28.0,>=1.27.0
+mypy-boto3-m2<1.28.0,>=1.27.0
+mypy-boto3-machinelearning<1.28.0,>=1.27.0
+mypy-boto3-macie<1.28.0,>=1.27.0
+mypy-boto3-macie2<1.28.0,>=1.27.0
+mypy-boto3-managedblockchain<1.28.0,>=1.27.0
+mypy-boto3-marketplace-catalog<1.28.0,>=1.27.0
+mypy-boto3-marketplace-entitlement<1.28.0,>=1.27.0
+mypy-boto3-marketplacecommerceanalytics<1.28.0,>=1.27.0
+mypy-boto3-mediaconnect<1.28.0,>=1.27.0
+mypy-boto3-mediaconvert<1.28.0,>=1.27.0
+mypy-boto3-medialive<1.28.0,>=1.27.0
+mypy-boto3-mediapackage<1.28.0,>=1.27.0
+mypy-boto3-mediapackage-vod<1.28.0,>=1.27.0
+mypy-boto3-mediapackagev2<1.28.0,>=1.27.0
+mypy-boto3-mediastore<1.28.0,>=1.27.0
+mypy-boto3-mediastore-data<1.28.0,>=1.27.0
+mypy-boto3-mediatailor<1.28.0,>=1.27.0
+mypy-boto3-memorydb<1.28.0,>=1.27.0
+mypy-boto3-meteringmarketplace<1.28.0,>=1.27.0
+mypy-boto3-mgh<1.28.0,>=1.27.0
+mypy-boto3-mgn<1.28.0,>=1.27.0
+mypy-boto3-migration-hub-refactor-spaces<1.28.0,>=1.27.0
+mypy-boto3-migrationhub-config<1.28.0,>=1.27.0
+mypy-boto3-migrationhuborchestrator<1.28.0,>=1.27.0
+mypy-boto3-migrationhubstrategy<1.28.0,>=1.27.0
+mypy-boto3-mobile<1.28.0,>=1.27.0
+mypy-boto3-mq<1.28.0,>=1.27.0
+mypy-boto3-mturk<1.28.0,>=1.27.0
+mypy-boto3-mwaa<1.28.0,>=1.27.0
+mypy-boto3-neptune<1.28.0,>=1.27.0
+mypy-boto3-network-firewall<1.28.0,>=1.27.0
+mypy-boto3-networkmanager<1.28.0,>=1.27.0
+mypy-boto3-nimble<1.28.0,>=1.27.0
+mypy-boto3-oam<1.28.0,>=1.27.0
+mypy-boto3-omics<1.28.0,>=1.27.0
+mypy-boto3-opensearch<1.28.0,>=1.27.0
+mypy-boto3-opensearchserverless<1.28.0,>=1.27.0
+mypy-boto3-opsworks<1.28.0,>=1.27.0
+mypy-boto3-opsworkscm<1.28.0,>=1.27.0
+mypy-boto3-organizations<1.28.0,>=1.27.0
+mypy-boto3-osis<1.28.0,>=1.27.0
+mypy-boto3-outposts<1.28.0,>=1.27.0
+mypy-boto3-panorama<1.28.0,>=1.27.0
+mypy-boto3-payment-cryptography<1.28.0,>=1.27.0
+mypy-boto3-payment-cryptography-data<1.28.0,>=1.27.0
+mypy-boto3-personalize<1.28.0,>=1.27.0
+mypy-boto3-personalize-events<1.28.0,>=1.27.0
+mypy-boto3-personalize-runtime<1.28.0,>=1.27.0
+mypy-boto3-pi<1.28.0,>=1.27.0
+mypy-boto3-pinpoint<1.28.0,>=1.27.0
+mypy-boto3-pinpoint-email<1.28.0,>=1.27.0
+mypy-boto3-pinpoint-sms-voice<1.28.0,>=1.27.0
+mypy-boto3-pinpoint-sms-voice-v2<1.28.0,>=1.27.0
+mypy-boto3-pipes<1.28.0,>=1.27.0
+mypy-boto3-polly<1.28.0,>=1.27.0
+mypy-boto3-pricing<1.28.0,>=1.27.0
+mypy-boto3-privatenetworks<1.28.0,>=1.27.0
+mypy-boto3-proton<1.28.0,>=1.27.0
+mypy-boto3-qldb<1.28.0,>=1.27.0
+mypy-boto3-qldb-session<1.28.0,>=1.27.0
+mypy-boto3-quicksight<1.28.0,>=1.27.0
+mypy-boto3-ram<1.28.0,>=1.27.0
+mypy-boto3-rbin<1.28.0,>=1.27.0
+mypy-boto3-rds<1.28.0,>=1.27.0
+mypy-boto3-rds-data<1.28.0,>=1.27.0
+mypy-boto3-redshift<1.28.0,>=1.27.0
+mypy-boto3-redshift-data<1.28.0,>=1.27.0
+mypy-boto3-redshift-serverless<1.28.0,>=1.27.0
+mypy-boto3-rekognition<1.28.0,>=1.27.0
+mypy-boto3-resiliencehub<1.28.0,>=1.27.0
+mypy-boto3-resource-explorer-2<1.28.0,>=1.27.0
+mypy-boto3-resource-groups<1.28.0,>=1.27.0
+mypy-boto3-resourcegroupstaggingapi<1.28.0,>=1.27.0
+mypy-boto3-robomaker<1.28.0,>=1.27.0
+mypy-boto3-rolesanywhere<1.28.0,>=1.27.0
+mypy-boto3-route53<1.28.0,>=1.27.0
+mypy-boto3-route53-recovery-cluster<1.28.0,>=1.27.0
+mypy-boto3-route53-recovery-control-config<1.28.0,>=1.27.0
+mypy-boto3-route53-recovery-readiness<1.28.0,>=1.27.0
+mypy-boto3-route53domains<1.28.0,>=1.27.0
+mypy-boto3-route53resolver<1.28.0,>=1.27.0
+mypy-boto3-rum<1.28.0,>=1.27.0
+mypy-boto3-s3<1.28.0,>=1.27.0
+mypy-boto3-s3control<1.28.0,>=1.27.0
+mypy-boto3-s3outposts<1.28.0,>=1.27.0
+mypy-boto3-sagemaker<1.28.0,>=1.27.0
+mypy-boto3-sagemaker-a2i-runtime<1.28.0,>=1.27.0
+mypy-boto3-sagemaker-edge<1.28.0,>=1.27.0
+mypy-boto3-sagemaker-featurestore-runtime<1.28.0,>=1.27.0
+mypy-boto3-sagemaker-geospatial<1.28.0,>=1.27.0
+mypy-boto3-sagemaker-metrics<1.28.0,>=1.27.0
+mypy-boto3-sagemaker-runtime<1.28.0,>=1.27.0
+mypy-boto3-savingsplans<1.28.0,>=1.27.0
+mypy-boto3-scheduler<1.28.0,>=1.27.0
+mypy-boto3-schemas<1.28.0,>=1.27.0
+mypy-boto3-sdb<1.28.0,>=1.27.0
+mypy-boto3-secretsmanager<1.28.0,>=1.27.0
+mypy-boto3-securityhub<1.28.0,>=1.27.0
+mypy-boto3-securitylake<1.28.0,>=1.27.0
+mypy-boto3-serverlessrepo<1.28.0,>=1.27.0
+mypy-boto3-service-quotas<1.28.0,>=1.27.0
+mypy-boto3-servicecatalog<1.28.0,>=1.27.0
+mypy-boto3-servicecatalog-appregistry<1.28.0,>=1.27.0
+mypy-boto3-servicediscovery<1.28.0,>=1.27.0
+mypy-boto3-ses<1.28.0,>=1.27.0
+mypy-boto3-sesv2<1.28.0,>=1.27.0
+mypy-boto3-shield<1.28.0,>=1.27.0
+mypy-boto3-signer<1.28.0,>=1.27.0
+mypy-boto3-simspaceweaver<1.28.0,>=1.27.0
+mypy-boto3-sms<1.28.0,>=1.27.0
+mypy-boto3-sms-voice<1.28.0,>=1.27.0
+mypy-boto3-snow-device-management<1.28.0,>=1.27.0
+mypy-boto3-snowball<1.28.0,>=1.27.0
+mypy-boto3-sns<1.28.0,>=1.27.0
+mypy-boto3-sqs<1.28.0,>=1.27.0
+mypy-boto3-ssm<1.28.0,>=1.27.0
+mypy-boto3-ssm-contacts<1.28.0,>=1.27.0
+mypy-boto3-ssm-incidents<1.28.0,>=1.27.0
+mypy-boto3-ssm-sap<1.28.0,>=1.27.0
+mypy-boto3-sso<1.28.0,>=1.27.0
+mypy-boto3-sso-admin<1.28.0,>=1.27.0
+mypy-boto3-sso-oidc<1.28.0,>=1.27.0
+mypy-boto3-stepfunctions<1.28.0,>=1.27.0
+mypy-boto3-storagegateway<1.28.0,>=1.27.0
+mypy-boto3-sts<1.28.0,>=1.27.0
+mypy-boto3-support<1.28.0,>=1.27.0
+mypy-boto3-support-app<1.28.0,>=1.27.0
+mypy-boto3-swf<1.28.0,>=1.27.0
+mypy-boto3-synthetics<1.28.0,>=1.27.0
+mypy-boto3-textract<1.28.0,>=1.27.0
+mypy-boto3-timestream-query<1.28.0,>=1.27.0
+mypy-boto3-timestream-write<1.28.0,>=1.27.0
+mypy-boto3-tnb<1.28.0,>=1.27.0
+mypy-boto3-transcribe<1.28.0,>=1.27.0
+mypy-boto3-transfer<1.28.0,>=1.27.0
+mypy-boto3-translate<1.28.0,>=1.27.0
+mypy-boto3-verifiedpermissions<1.28.0,>=1.27.0
+mypy-boto3-voice-id<1.28.0,>=1.27.0
+mypy-boto3-vpc-lattice<1.28.0,>=1.27.0
+mypy-boto3-waf<1.28.0,>=1.27.0
+mypy-boto3-waf-regional<1.28.0,>=1.27.0
+mypy-boto3-wafv2<1.28.0,>=1.27.0
+mypy-boto3-wellarchitected<1.28.0,>=1.27.0
+mypy-boto3-wisdom<1.28.0,>=1.27.0
+mypy-boto3-workdocs<1.28.0,>=1.27.0
+mypy-boto3-worklink<1.28.0,>=1.27.0
+mypy-boto3-workmail<1.28.0,>=1.27.0
+mypy-boto3-workmailmessageflow<1.28.0,>=1.27.0
+mypy-boto3-workspaces<1.28.0,>=1.27.0
+mypy-boto3-workspaces-web<1.28.0,>=1.27.0
+mypy-boto3-xray<1.28.0,>=1.27.0
 
 [amp]
-mypy-boto3-amp<1.27.0,>=1.26.0
+mypy-boto3-amp<1.28.0,>=1.27.0
 
 [amplify]
-mypy-boto3-amplify<1.27.0,>=1.26.0
+mypy-boto3-amplify<1.28.0,>=1.27.0
 
 [amplifybackend]
-mypy-boto3-amplifybackend<1.27.0,>=1.26.0
+mypy-boto3-amplifybackend<1.28.0,>=1.27.0
 
 [amplifyuibuilder]
-mypy-boto3-amplifyuibuilder<1.27.0,>=1.26.0
+mypy-boto3-amplifyuibuilder<1.28.0,>=1.27.0
 
 [apigateway]
-mypy-boto3-apigateway<1.27.0,>=1.26.0
+mypy-boto3-apigateway<1.28.0,>=1.27.0
 
 [apigatewaymanagementapi]
-mypy-boto3-apigatewaymanagementapi<1.27.0,>=1.26.0
+mypy-boto3-apigatewaymanagementapi<1.28.0,>=1.27.0
 
 [apigatewayv2]
-mypy-boto3-apigatewayv2<1.27.0,>=1.26.0
+mypy-boto3-apigatewayv2<1.28.0,>=1.27.0
 
 [appconfig]
-mypy-boto3-appconfig<1.27.0,>=1.26.0
+mypy-boto3-appconfig<1.28.0,>=1.27.0
 
 [appconfigdata]
-mypy-boto3-appconfigdata<1.27.0,>=1.26.0
+mypy-boto3-appconfigdata<1.28.0,>=1.27.0
+
+[appfabric]
+mypy-boto3-appfabric<1.28.0,>=1.27.0
 
 [appflow]
-mypy-boto3-appflow<1.27.0,>=1.26.0
+mypy-boto3-appflow<1.28.0,>=1.27.0
 
 [appintegrations]
-mypy-boto3-appintegrations<1.27.0,>=1.26.0
+mypy-boto3-appintegrations<1.28.0,>=1.27.0
 
 [application-autoscaling]
-mypy-boto3-application-autoscaling<1.27.0,>=1.26.0
+mypy-boto3-application-autoscaling<1.28.0,>=1.27.0
 
 [application-insights]
-mypy-boto3-application-insights<1.27.0,>=1.26.0
+mypy-boto3-application-insights<1.28.0,>=1.27.0
 
 [applicationcostprofiler]
-mypy-boto3-applicationcostprofiler<1.27.0,>=1.26.0
+mypy-boto3-applicationcostprofiler<1.28.0,>=1.27.0
 
 [appmesh]
-mypy-boto3-appmesh<1.27.0,>=1.26.0
+mypy-boto3-appmesh<1.28.0,>=1.27.0
 
 [apprunner]
-mypy-boto3-apprunner<1.27.0,>=1.26.0
+mypy-boto3-apprunner<1.28.0,>=1.27.0
 
 [appstream]
-mypy-boto3-appstream<1.27.0,>=1.26.0
+mypy-boto3-appstream<1.28.0,>=1.27.0
 
 [appsync]
-mypy-boto3-appsync<1.27.0,>=1.26.0
+mypy-boto3-appsync<1.28.0,>=1.27.0
 
 [arc-zonal-shift]
-mypy-boto3-arc-zonal-shift<1.27.0,>=1.26.0
+mypy-boto3-arc-zonal-shift<1.28.0,>=1.27.0
 
 [athena]
-mypy-boto3-athena<1.27.0,>=1.26.0
+mypy-boto3-athena<1.28.0,>=1.27.0
 
 [auditmanager]
-mypy-boto3-auditmanager<1.27.0,>=1.26.0
+mypy-boto3-auditmanager<1.28.0,>=1.27.0
 
 [autoscaling]
-mypy-boto3-autoscaling<1.27.0,>=1.26.0
+mypy-boto3-autoscaling<1.28.0,>=1.27.0
 
 [autoscaling-plans]
-mypy-boto3-autoscaling-plans<1.27.0,>=1.26.0
+mypy-boto3-autoscaling-plans<1.28.0,>=1.27.0
 
 [backup]
-mypy-boto3-backup<1.27.0,>=1.26.0
+mypy-boto3-backup<1.28.0,>=1.27.0
 
 [backup-gateway]
-mypy-boto3-backup-gateway<1.27.0,>=1.26.0
+mypy-boto3-backup-gateway<1.28.0,>=1.27.0
 
 [backupstorage]
-mypy-boto3-backupstorage<1.27.0,>=1.26.0
+mypy-boto3-backupstorage<1.28.0,>=1.27.0
 
 [batch]
-mypy-boto3-batch<1.27.0,>=1.26.0
+mypy-boto3-batch<1.28.0,>=1.27.0
 
 [billingconductor]
-mypy-boto3-billingconductor<1.27.0,>=1.26.0
+mypy-boto3-billingconductor<1.28.0,>=1.27.0
 
 [boto3]
-boto3==1.26.99
-botocore==1.29.99
+boto3==1.27.0
+botocore==1.30.0
 
 [braket]
-mypy-boto3-braket<1.27.0,>=1.26.0
+mypy-boto3-braket<1.28.0,>=1.27.0
 
 [budgets]
-mypy-boto3-budgets<1.27.0,>=1.26.0
+mypy-boto3-budgets<1.28.0,>=1.27.0
 
 [ce]
-mypy-boto3-ce<1.27.0,>=1.26.0
+mypy-boto3-ce<1.28.0,>=1.27.0
 
 [chime]
-mypy-boto3-chime<1.27.0,>=1.26.0
+mypy-boto3-chime<1.28.0,>=1.27.0
 
 [chime-sdk-identity]
-mypy-boto3-chime-sdk-identity<1.27.0,>=1.26.0
+mypy-boto3-chime-sdk-identity<1.28.0,>=1.27.0
 
 [chime-sdk-media-pipelines]
-mypy-boto3-chime-sdk-media-pipelines<1.27.0,>=1.26.0
+mypy-boto3-chime-sdk-media-pipelines<1.28.0,>=1.27.0
 
 [chime-sdk-meetings]
-mypy-boto3-chime-sdk-meetings<1.27.0,>=1.26.0
+mypy-boto3-chime-sdk-meetings<1.28.0,>=1.27.0
 
 [chime-sdk-messaging]
-mypy-boto3-chime-sdk-messaging<1.27.0,>=1.26.0
+mypy-boto3-chime-sdk-messaging<1.28.0,>=1.27.0
 
 [chime-sdk-voice]
-mypy-boto3-chime-sdk-voice<1.27.0,>=1.26.0
+mypy-boto3-chime-sdk-voice<1.28.0,>=1.27.0
 
 [cleanrooms]
-mypy-boto3-cleanrooms<1.27.0,>=1.26.0
+mypy-boto3-cleanrooms<1.28.0,>=1.27.0
 
 [cloud9]
-mypy-boto3-cloud9<1.27.0,>=1.26.0
+mypy-boto3-cloud9<1.28.0,>=1.27.0
 
 [cloudcontrol]
-mypy-boto3-cloudcontrol<1.27.0,>=1.26.0
+mypy-boto3-cloudcontrol<1.28.0,>=1.27.0
 
 [clouddirectory]
-mypy-boto3-clouddirectory<1.27.0,>=1.26.0
+mypy-boto3-clouddirectory<1.28.0,>=1.27.0
 
 [cloudformation]
-mypy-boto3-cloudformation<1.27.0,>=1.26.0
+mypy-boto3-cloudformation<1.28.0,>=1.27.0
 
 [cloudfront]
-mypy-boto3-cloudfront<1.27.0,>=1.26.0
+mypy-boto3-cloudfront<1.28.0,>=1.27.0
 
 [cloudhsm]
-mypy-boto3-cloudhsm<1.27.0,>=1.26.0
+mypy-boto3-cloudhsm<1.28.0,>=1.27.0
 
 [cloudhsmv2]
-mypy-boto3-cloudhsmv2<1.27.0,>=1.26.0
+mypy-boto3-cloudhsmv2<1.28.0,>=1.27.0
 
 [cloudsearch]
-mypy-boto3-cloudsearch<1.27.0,>=1.26.0
+mypy-boto3-cloudsearch<1.28.0,>=1.27.0
 
 [cloudsearchdomain]
-mypy-boto3-cloudsearchdomain<1.27.0,>=1.26.0
+mypy-boto3-cloudsearchdomain<1.28.0,>=1.27.0
 
 [cloudtrail]
-mypy-boto3-cloudtrail<1.27.0,>=1.26.0
+mypy-boto3-cloudtrail<1.28.0,>=1.27.0
 
 [cloudtrail-data]
-mypy-boto3-cloudtrail-data<1.27.0,>=1.26.0
+mypy-boto3-cloudtrail-data<1.28.0,>=1.27.0
 
 [cloudwatch]
-mypy-boto3-cloudwatch<1.27.0,>=1.26.0
+mypy-boto3-cloudwatch<1.28.0,>=1.27.0
 
 [codeartifact]
-mypy-boto3-codeartifact<1.27.0,>=1.26.0
+mypy-boto3-codeartifact<1.28.0,>=1.27.0
 
 [codebuild]
-mypy-boto3-codebuild<1.27.0,>=1.26.0
+mypy-boto3-codebuild<1.28.0,>=1.27.0
 
 [codecatalyst]
-mypy-boto3-codecatalyst<1.27.0,>=1.26.0
+mypy-boto3-codecatalyst<1.28.0,>=1.27.0
 
 [codecommit]
-mypy-boto3-codecommit<1.27.0,>=1.26.0
+mypy-boto3-codecommit<1.28.0,>=1.27.0
 
 [codedeploy]
-mypy-boto3-codedeploy<1.27.0,>=1.26.0
+mypy-boto3-codedeploy<1.28.0,>=1.27.0
 
 [codeguru-reviewer]
-mypy-boto3-codeguru-reviewer<1.27.0,>=1.26.0
+mypy-boto3-codeguru-reviewer<1.28.0,>=1.27.0
+
+[codeguru-security]
+mypy-boto3-codeguru-security<1.28.0,>=1.27.0
 
 [codeguruprofiler]
-mypy-boto3-codeguruprofiler<1.27.0,>=1.26.0
+mypy-boto3-codeguruprofiler<1.28.0,>=1.27.0
 
 [codepipeline]
-mypy-boto3-codepipeline<1.27.0,>=1.26.0
+mypy-boto3-codepipeline<1.28.0,>=1.27.0
 
 [codestar]
-mypy-boto3-codestar<1.27.0,>=1.26.0
+mypy-boto3-codestar<1.28.0,>=1.27.0
 
 [codestar-connections]
-mypy-boto3-codestar-connections<1.27.0,>=1.26.0
+mypy-boto3-codestar-connections<1.28.0,>=1.27.0
 
 [codestar-notifications]
-mypy-boto3-codestar-notifications<1.27.0,>=1.26.0
+mypy-boto3-codestar-notifications<1.28.0,>=1.27.0
 
 [cognito-identity]
-mypy-boto3-cognito-identity<1.27.0,>=1.26.0
+mypy-boto3-cognito-identity<1.28.0,>=1.27.0
 
 [cognito-idp]
-mypy-boto3-cognito-idp<1.27.0,>=1.26.0
+mypy-boto3-cognito-idp<1.28.0,>=1.27.0
 
 [cognito-sync]
-mypy-boto3-cognito-sync<1.27.0,>=1.26.0
+mypy-boto3-cognito-sync<1.28.0,>=1.27.0
 
 [comprehend]
-mypy-boto3-comprehend<1.27.0,>=1.26.0
+mypy-boto3-comprehend<1.28.0,>=1.27.0
 
 [comprehendmedical]
-mypy-boto3-comprehendmedical<1.27.0,>=1.26.0
+mypy-boto3-comprehendmedical<1.28.0,>=1.27.0
 
 [compute-optimizer]
-mypy-boto3-compute-optimizer<1.27.0,>=1.26.0
+mypy-boto3-compute-optimizer<1.28.0,>=1.27.0
 
 [config]
-mypy-boto3-config<1.27.0,>=1.26.0
+mypy-boto3-config<1.28.0,>=1.27.0
 
 [connect]
-mypy-boto3-connect<1.27.0,>=1.26.0
+mypy-boto3-connect<1.28.0,>=1.27.0
 
 [connect-contact-lens]
-mypy-boto3-connect-contact-lens<1.27.0,>=1.26.0
+mypy-boto3-connect-contact-lens<1.28.0,>=1.27.0
 
 [connectcampaigns]
-mypy-boto3-connectcampaigns<1.27.0,>=1.26.0
+mypy-boto3-connectcampaigns<1.28.0,>=1.27.0
 
 [connectcases]
-mypy-boto3-connectcases<1.27.0,>=1.26.0
+mypy-boto3-connectcases<1.28.0,>=1.27.0
 
 [connectparticipant]
-mypy-boto3-connectparticipant<1.27.0,>=1.26.0
+mypy-boto3-connectparticipant<1.28.0,>=1.27.0
 
 [controltower]
-mypy-boto3-controltower<1.27.0,>=1.26.0
+mypy-boto3-controltower<1.28.0,>=1.27.0
 
 [cur]
-mypy-boto3-cur<1.27.0,>=1.26.0
+mypy-boto3-cur<1.28.0,>=1.27.0
 
 [customer-profiles]
-mypy-boto3-customer-profiles<1.27.0,>=1.26.0
+mypy-boto3-customer-profiles<1.28.0,>=1.27.0
 
 [databrew]
-mypy-boto3-databrew<1.27.0,>=1.26.0
+mypy-boto3-databrew<1.28.0,>=1.27.0
 
 [dataexchange]
-mypy-boto3-dataexchange<1.27.0,>=1.26.0
+mypy-boto3-dataexchange<1.28.0,>=1.27.0
 
 [datapipeline]
-mypy-boto3-datapipeline<1.27.0,>=1.26.0
+mypy-boto3-datapipeline<1.28.0,>=1.27.0
 
 [datasync]
-mypy-boto3-datasync<1.27.0,>=1.26.0
+mypy-boto3-datasync<1.28.0,>=1.27.0
 
 [dax]
-mypy-boto3-dax<1.27.0,>=1.26.0
+mypy-boto3-dax<1.28.0,>=1.27.0
 
 [detective]
-mypy-boto3-detective<1.27.0,>=1.26.0
+mypy-boto3-detective<1.28.0,>=1.27.0
 
 [devicefarm]
-mypy-boto3-devicefarm<1.27.0,>=1.26.0
+mypy-boto3-devicefarm<1.28.0,>=1.27.0
 
 [devops-guru]
-mypy-boto3-devops-guru<1.27.0,>=1.26.0
+mypy-boto3-devops-guru<1.28.0,>=1.27.0
 
 [directconnect]
-mypy-boto3-directconnect<1.27.0,>=1.26.0
+mypy-boto3-directconnect<1.28.0,>=1.27.0
 
 [discovery]
-mypy-boto3-discovery<1.27.0,>=1.26.0
+mypy-boto3-discovery<1.28.0,>=1.27.0
 
 [dlm]
-mypy-boto3-dlm<1.27.0,>=1.26.0
+mypy-boto3-dlm<1.28.0,>=1.27.0
 
 [dms]
-mypy-boto3-dms<1.27.0,>=1.26.0
+mypy-boto3-dms<1.28.0,>=1.27.0
 
 [docdb]
-mypy-boto3-docdb<1.27.0,>=1.26.0
+mypy-boto3-docdb<1.28.0,>=1.27.0
 
 [docdb-elastic]
-mypy-boto3-docdb-elastic<1.27.0,>=1.26.0
+mypy-boto3-docdb-elastic<1.28.0,>=1.27.0
 
 [drs]
-mypy-boto3-drs<1.27.0,>=1.26.0
+mypy-boto3-drs<1.28.0,>=1.27.0
 
 [ds]
-mypy-boto3-ds<1.27.0,>=1.26.0
+mypy-boto3-ds<1.28.0,>=1.27.0
 
 [dynamodb]
-mypy-boto3-dynamodb<1.27.0,>=1.26.0
+mypy-boto3-dynamodb<1.28.0,>=1.27.0
 
 [dynamodbstreams]
-mypy-boto3-dynamodbstreams<1.27.0,>=1.26.0
+mypy-boto3-dynamodbstreams<1.28.0,>=1.27.0
 
 [ebs]
-mypy-boto3-ebs<1.27.0,>=1.26.0
+mypy-boto3-ebs<1.28.0,>=1.27.0
 
 [ec2]
-mypy-boto3-ec2<1.27.0,>=1.26.0
+mypy-boto3-ec2<1.28.0,>=1.27.0
 
 [ec2-instance-connect]
-mypy-boto3-ec2-instance-connect<1.27.0,>=1.26.0
+mypy-boto3-ec2-instance-connect<1.28.0,>=1.27.0
 
 [ecr]
-mypy-boto3-ecr<1.27.0,>=1.26.0
+mypy-boto3-ecr<1.28.0,>=1.27.0
 
 [ecr-public]
-mypy-boto3-ecr-public<1.27.0,>=1.26.0
+mypy-boto3-ecr-public<1.28.0,>=1.27.0
 
 [ecs]
-mypy-boto3-ecs<1.27.0,>=1.26.0
+mypy-boto3-ecs<1.28.0,>=1.27.0
 
 [efs]
-mypy-boto3-efs<1.27.0,>=1.26.0
+mypy-boto3-efs<1.28.0,>=1.27.0
 
 [eks]
-mypy-boto3-eks<1.27.0,>=1.26.0
+mypy-boto3-eks<1.28.0,>=1.27.0
 
 [elastic-inference]
-mypy-boto3-elastic-inference<1.27.0,>=1.26.0
+mypy-boto3-elastic-inference<1.28.0,>=1.27.0
 
 [elasticache]
-mypy-boto3-elasticache<1.27.0,>=1.26.0
+mypy-boto3-elasticache<1.28.0,>=1.27.0
 
 [elasticbeanstalk]
-mypy-boto3-elasticbeanstalk<1.27.0,>=1.26.0
+mypy-boto3-elasticbeanstalk<1.28.0,>=1.27.0
 
 [elastictranscoder]
-mypy-boto3-elastictranscoder<1.27.0,>=1.26.0
+mypy-boto3-elastictranscoder<1.28.0,>=1.27.0
 
 [elb]
-mypy-boto3-elb<1.27.0,>=1.26.0
+mypy-boto3-elb<1.28.0,>=1.27.0
 
 [elbv2]
-mypy-boto3-elbv2<1.27.0,>=1.26.0
+mypy-boto3-elbv2<1.28.0,>=1.27.0
 
 [emr]
-mypy-boto3-emr<1.27.0,>=1.26.0
+mypy-boto3-emr<1.28.0,>=1.27.0
 
 [emr-containers]
-mypy-boto3-emr-containers<1.27.0,>=1.26.0
+mypy-boto3-emr-containers<1.28.0,>=1.27.0
 
 [emr-serverless]
-mypy-boto3-emr-serverless<1.27.0,>=1.26.0
+mypy-boto3-emr-serverless<1.28.0,>=1.27.0
 
 [es]
-mypy-boto3-es<1.27.0,>=1.26.0
+mypy-boto3-es<1.28.0,>=1.27.0
 
 [essential]
-mypy-boto3-cloudformation<1.27.0,>=1.26.0
-mypy-boto3-dynamodb<1.27.0,>=1.26.0
-mypy-boto3-ec2<1.27.0,>=1.26.0
-mypy-boto3-lambda<1.27.0,>=1.26.0
-mypy-boto3-rds<1.27.0,>=1.26.0
-mypy-boto3-s3<1.27.0,>=1.26.0
-mypy-boto3-sqs<1.27.0,>=1.26.0
+mypy-boto3-cloudformation<1.28.0,>=1.27.0
+mypy-boto3-dynamodb<1.28.0,>=1.27.0
+mypy-boto3-ec2<1.28.0,>=1.27.0
+mypy-boto3-lambda<1.28.0,>=1.27.0
+mypy-boto3-rds<1.28.0,>=1.27.0
+mypy-boto3-s3<1.28.0,>=1.27.0
+mypy-boto3-sqs<1.28.0,>=1.27.0
 
 [events]
-mypy-boto3-events<1.27.0,>=1.26.0
+mypy-boto3-events<1.28.0,>=1.27.0
 
 [evidently]
-mypy-boto3-evidently<1.27.0,>=1.26.0
+mypy-boto3-evidently<1.28.0,>=1.27.0
 
 [finspace]
-mypy-boto3-finspace<1.27.0,>=1.26.0
+mypy-boto3-finspace<1.28.0,>=1.27.0
 
 [finspace-data]
-mypy-boto3-finspace-data<1.27.0,>=1.26.0
+mypy-boto3-finspace-data<1.28.0,>=1.27.0
 
 [firehose]
-mypy-boto3-firehose<1.27.0,>=1.26.0
+mypy-boto3-firehose<1.28.0,>=1.27.0
 
 [fis]
-mypy-boto3-fis<1.27.0,>=1.26.0
+mypy-boto3-fis<1.28.0,>=1.27.0
 
 [fms]
-mypy-boto3-fms<1.27.0,>=1.26.0
+mypy-boto3-fms<1.28.0,>=1.27.0
 
 [forecast]
-mypy-boto3-forecast<1.27.0,>=1.26.0
+mypy-boto3-forecast<1.28.0,>=1.27.0
 
 [forecastquery]
-mypy-boto3-forecastquery<1.27.0,>=1.26.0
+mypy-boto3-forecastquery<1.28.0,>=1.27.0
 
 [frauddetector]
-mypy-boto3-frauddetector<1.27.0,>=1.26.0
+mypy-boto3-frauddetector<1.28.0,>=1.27.0
 
 [fsx]
-mypy-boto3-fsx<1.27.0,>=1.26.0
+mypy-boto3-fsx<1.28.0,>=1.27.0
 
 [gamelift]
-mypy-boto3-gamelift<1.27.0,>=1.26.0
+mypy-boto3-gamelift<1.28.0,>=1.27.0
 
 [gamesparks]
-mypy-boto3-gamesparks<1.27.0,>=1.26.0
+mypy-boto3-gamesparks<1.28.0,>=1.27.0
 
 [glacier]
-mypy-boto3-glacier<1.27.0,>=1.26.0
+mypy-boto3-glacier<1.28.0,>=1.27.0
 
 [globalaccelerator]
-mypy-boto3-globalaccelerator<1.27.0,>=1.26.0
+mypy-boto3-globalaccelerator<1.28.0,>=1.27.0
 
 [glue]
-mypy-boto3-glue<1.27.0,>=1.26.0
+mypy-boto3-glue<1.28.0,>=1.27.0
 
 [grafana]
-mypy-boto3-grafana<1.27.0,>=1.26.0
+mypy-boto3-grafana<1.28.0,>=1.27.0
 
 [greengrass]
-mypy-boto3-greengrass<1.27.0,>=1.26.0
+mypy-boto3-greengrass<1.28.0,>=1.27.0
 
 [greengrassv2]
-mypy-boto3-greengrassv2<1.27.0,>=1.26.0
+mypy-boto3-greengrassv2<1.28.0,>=1.27.0
 
 [groundstation]
-mypy-boto3-groundstation<1.27.0,>=1.26.0
+mypy-boto3-groundstation<1.28.0,>=1.27.0
 
 [guardduty]
-mypy-boto3-guardduty<1.27.0,>=1.26.0
+mypy-boto3-guardduty<1.28.0,>=1.27.0
 
 [health]
-mypy-boto3-health<1.27.0,>=1.26.0
+mypy-boto3-health<1.28.0,>=1.27.0
 
 [healthlake]
-mypy-boto3-healthlake<1.27.0,>=1.26.0
+mypy-boto3-healthlake<1.28.0,>=1.27.0
 
 [honeycode]
-mypy-boto3-honeycode<1.27.0,>=1.26.0
+mypy-boto3-honeycode<1.28.0,>=1.27.0
 
 [iam]
-mypy-boto3-iam<1.27.0,>=1.26.0
+mypy-boto3-iam<1.28.0,>=1.27.0
 
 [identitystore]
-mypy-boto3-identitystore<1.27.0,>=1.26.0
+mypy-boto3-identitystore<1.28.0,>=1.27.0
 
 [imagebuilder]
-mypy-boto3-imagebuilder<1.27.0,>=1.26.0
+mypy-boto3-imagebuilder<1.28.0,>=1.27.0
 
 [importexport]
-mypy-boto3-importexport<1.27.0,>=1.26.0
+mypy-boto3-importexport<1.28.0,>=1.27.0
 
 [inspector]
-mypy-boto3-inspector<1.27.0,>=1.26.0
+mypy-boto3-inspector<1.28.0,>=1.27.0
 
 [inspector2]
-mypy-boto3-inspector2<1.27.0,>=1.26.0
+mypy-boto3-inspector2<1.28.0,>=1.27.0
 
 [internetmonitor]
-mypy-boto3-internetmonitor<1.27.0,>=1.26.0
+mypy-boto3-internetmonitor<1.28.0,>=1.27.0
 
 [iot]
-mypy-boto3-iot<1.27.0,>=1.26.0
+mypy-boto3-iot<1.28.0,>=1.27.0
 
 [iot-data]
-mypy-boto3-iot-data<1.27.0,>=1.26.0
+mypy-boto3-iot-data<1.28.0,>=1.27.0
 
 [iot-jobs-data]
-mypy-boto3-iot-jobs-data<1.27.0,>=1.26.0
+mypy-boto3-iot-jobs-data<1.28.0,>=1.27.0
 
 [iot-roborunner]
-mypy-boto3-iot-roborunner<1.27.0,>=1.26.0
+mypy-boto3-iot-roborunner<1.28.0,>=1.27.0
 
 [iot1click-devices]
-mypy-boto3-iot1click-devices<1.27.0,>=1.26.0
+mypy-boto3-iot1click-devices<1.28.0,>=1.27.0
 
 [iot1click-projects]
-mypy-boto3-iot1click-projects<1.27.0,>=1.26.0
+mypy-boto3-iot1click-projects<1.28.0,>=1.27.0
 
 [iotanalytics]
-mypy-boto3-iotanalytics<1.27.0,>=1.26.0
+mypy-boto3-iotanalytics<1.28.0,>=1.27.0
 
 [iotdeviceadvisor]
-mypy-boto3-iotdeviceadvisor<1.27.0,>=1.26.0
+mypy-boto3-iotdeviceadvisor<1.28.0,>=1.27.0
 
 [iotevents]
-mypy-boto3-iotevents<1.27.0,>=1.26.0
+mypy-boto3-iotevents<1.28.0,>=1.27.0
 
 [iotevents-data]
-mypy-boto3-iotevents-data<1.27.0,>=1.26.0
+mypy-boto3-iotevents-data<1.28.0,>=1.27.0
 
 [iotfleethub]
-mypy-boto3-iotfleethub<1.27.0,>=1.26.0
+mypy-boto3-iotfleethub<1.28.0,>=1.27.0
 
 [iotfleetwise]
-mypy-boto3-iotfleetwise<1.27.0,>=1.26.0
+mypy-boto3-iotfleetwise<1.28.0,>=1.27.0
 
 [iotsecuretunneling]
-mypy-boto3-iotsecuretunneling<1.27.0,>=1.26.0
+mypy-boto3-iotsecuretunneling<1.28.0,>=1.27.0
 
 [iotsitewise]
-mypy-boto3-iotsitewise<1.27.0,>=1.26.0
+mypy-boto3-iotsitewise<1.28.0,>=1.27.0
 
 [iotthingsgraph]
-mypy-boto3-iotthingsgraph<1.27.0,>=1.26.0
+mypy-boto3-iotthingsgraph<1.28.0,>=1.27.0
 
 [iottwinmaker]
-mypy-boto3-iottwinmaker<1.27.0,>=1.26.0
+mypy-boto3-iottwinmaker<1.28.0,>=1.27.0
 
 [iotwireless]
-mypy-boto3-iotwireless<1.27.0,>=1.26.0
+mypy-boto3-iotwireless<1.28.0,>=1.27.0
 
 [ivs]
-mypy-boto3-ivs<1.27.0,>=1.26.0
+mypy-boto3-ivs<1.28.0,>=1.27.0
 
 [ivs-realtime]
-mypy-boto3-ivs-realtime<1.27.0,>=1.26.0
+mypy-boto3-ivs-realtime<1.28.0,>=1.27.0
 
 [ivschat]
-mypy-boto3-ivschat<1.27.0,>=1.26.0
+mypy-boto3-ivschat<1.28.0,>=1.27.0
 
 [kafka]
-mypy-boto3-kafka<1.27.0,>=1.26.0
+mypy-boto3-kafka<1.28.0,>=1.27.0
 
 [kafkaconnect]
-mypy-boto3-kafkaconnect<1.27.0,>=1.26.0
+mypy-boto3-kafkaconnect<1.28.0,>=1.27.0
 
 [kendra]
-mypy-boto3-kendra<1.27.0,>=1.26.0
+mypy-boto3-kendra<1.28.0,>=1.27.0
 
 [kendra-ranking]
-mypy-boto3-kendra-ranking<1.27.0,>=1.26.0
+mypy-boto3-kendra-ranking<1.28.0,>=1.27.0
 
 [keyspaces]
-mypy-boto3-keyspaces<1.27.0,>=1.26.0
+mypy-boto3-keyspaces<1.28.0,>=1.27.0
 
 [kinesis]
-mypy-boto3-kinesis<1.27.0,>=1.26.0
+mypy-boto3-kinesis<1.28.0,>=1.27.0
 
 [kinesis-video-archived-media]
-mypy-boto3-kinesis-video-archived-media<1.27.0,>=1.26.0
+mypy-boto3-kinesis-video-archived-media<1.28.0,>=1.27.0
 
 [kinesis-video-media]
-mypy-boto3-kinesis-video-media<1.27.0,>=1.26.0
+mypy-boto3-kinesis-video-media<1.28.0,>=1.27.0
 
 [kinesis-video-signaling]
-mypy-boto3-kinesis-video-signaling<1.27.0,>=1.26.0
+mypy-boto3-kinesis-video-signaling<1.28.0,>=1.27.0
 
 [kinesis-video-webrtc-storage]
-mypy-boto3-kinesis-video-webrtc-storage<1.27.0,>=1.26.0
+mypy-boto3-kinesis-video-webrtc-storage<1.28.0,>=1.27.0
 
 [kinesisanalytics]
-mypy-boto3-kinesisanalytics<1.27.0,>=1.26.0
+mypy-boto3-kinesisanalytics<1.28.0,>=1.27.0
 
 [kinesisanalyticsv2]
-mypy-boto3-kinesisanalyticsv2<1.27.0,>=1.26.0
+mypy-boto3-kinesisanalyticsv2<1.28.0,>=1.27.0
 
 [kinesisvideo]
-mypy-boto3-kinesisvideo<1.27.0,>=1.26.0
+mypy-boto3-kinesisvideo<1.28.0,>=1.27.0
 
 [kms]
-mypy-boto3-kms<1.27.0,>=1.26.0
+mypy-boto3-kms<1.28.0,>=1.27.0
 
 [lakeformation]
-mypy-boto3-lakeformation<1.27.0,>=1.26.0
+mypy-boto3-lakeformation<1.28.0,>=1.27.0
 
 [lambda]
-mypy-boto3-lambda<1.27.0,>=1.26.0
+mypy-boto3-lambda<1.28.0,>=1.27.0
 
 [lex-models]
-mypy-boto3-lex-models<1.27.0,>=1.26.0
+mypy-boto3-lex-models<1.28.0,>=1.27.0
 
 [lex-runtime]
-mypy-boto3-lex-runtime<1.27.0,>=1.26.0
+mypy-boto3-lex-runtime<1.28.0,>=1.27.0
 
 [lexv2-models]
-mypy-boto3-lexv2-models<1.27.0,>=1.26.0
+mypy-boto3-lexv2-models<1.28.0,>=1.27.0
 
 [lexv2-runtime]
-mypy-boto3-lexv2-runtime<1.27.0,>=1.26.0
+mypy-boto3-lexv2-runtime<1.28.0,>=1.27.0
 
 [license-manager]
-mypy-boto3-license-manager<1.27.0,>=1.26.0
+mypy-boto3-license-manager<1.28.0,>=1.27.0
 
 [license-manager-linux-subscriptions]
-mypy-boto3-license-manager-linux-subscriptions<1.27.0,>=1.26.0
+mypy-boto3-license-manager-linux-subscriptions<1.28.0,>=1.27.0
 
 [license-manager-user-subscriptions]
-mypy-boto3-license-manager-user-subscriptions<1.27.0,>=1.26.0
+mypy-boto3-license-manager-user-subscriptions<1.28.0,>=1.27.0
 
 [lightsail]
-mypy-boto3-lightsail<1.27.0,>=1.26.0
+mypy-boto3-lightsail<1.28.0,>=1.27.0
 
 [location]
-mypy-boto3-location<1.27.0,>=1.26.0
+mypy-boto3-location<1.28.0,>=1.27.0
 
 [logs]
-mypy-boto3-logs<1.27.0,>=1.26.0
+mypy-boto3-logs<1.28.0,>=1.27.0
 
 [lookoutequipment]
-mypy-boto3-lookoutequipment<1.27.0,>=1.26.0
+mypy-boto3-lookoutequipment<1.28.0,>=1.27.0
 
 [lookoutmetrics]
-mypy-boto3-lookoutmetrics<1.27.0,>=1.26.0
+mypy-boto3-lookoutmetrics<1.28.0,>=1.27.0
 
 [lookoutvision]
-mypy-boto3-lookoutvision<1.27.0,>=1.26.0
+mypy-boto3-lookoutvision<1.28.0,>=1.27.0
 
 [m2]
-mypy-boto3-m2<1.27.0,>=1.26.0
+mypy-boto3-m2<1.28.0,>=1.27.0
 
 [machinelearning]
-mypy-boto3-machinelearning<1.27.0,>=1.26.0
+mypy-boto3-machinelearning<1.28.0,>=1.27.0
 
 [macie]
-mypy-boto3-macie<1.27.0,>=1.26.0
+mypy-boto3-macie<1.28.0,>=1.27.0
 
 [macie2]
-mypy-boto3-macie2<1.27.0,>=1.26.0
+mypy-boto3-macie2<1.28.0,>=1.27.0
 
 [managedblockchain]
-mypy-boto3-managedblockchain<1.27.0,>=1.26.0
+mypy-boto3-managedblockchain<1.28.0,>=1.27.0
 
 [marketplace-catalog]
-mypy-boto3-marketplace-catalog<1.27.0,>=1.26.0
+mypy-boto3-marketplace-catalog<1.28.0,>=1.27.0
 
 [marketplace-entitlement]
-mypy-boto3-marketplace-entitlement<1.27.0,>=1.26.0
+mypy-boto3-marketplace-entitlement<1.28.0,>=1.27.0
 
 [marketplacecommerceanalytics]
-mypy-boto3-marketplacecommerceanalytics<1.27.0,>=1.26.0
+mypy-boto3-marketplacecommerceanalytics<1.28.0,>=1.27.0
 
 [mediaconnect]
-mypy-boto3-mediaconnect<1.27.0,>=1.26.0
+mypy-boto3-mediaconnect<1.28.0,>=1.27.0
 
 [mediaconvert]
-mypy-boto3-mediaconvert<1.27.0,>=1.26.0
+mypy-boto3-mediaconvert<1.28.0,>=1.27.0
 
 [medialive]
-mypy-boto3-medialive<1.27.0,>=1.26.0
+mypy-boto3-medialive<1.28.0,>=1.27.0
 
 [mediapackage]
-mypy-boto3-mediapackage<1.27.0,>=1.26.0
+mypy-boto3-mediapackage<1.28.0,>=1.27.0
 
 [mediapackage-vod]
-mypy-boto3-mediapackage-vod<1.27.0,>=1.26.0
+mypy-boto3-mediapackage-vod<1.28.0,>=1.27.0
+
+[mediapackagev2]
+mypy-boto3-mediapackagev2<1.28.0,>=1.27.0
 
 [mediastore]
-mypy-boto3-mediastore<1.27.0,>=1.26.0
+mypy-boto3-mediastore<1.28.0,>=1.27.0
 
 [mediastore-data]
-mypy-boto3-mediastore-data<1.27.0,>=1.26.0
+mypy-boto3-mediastore-data<1.28.0,>=1.27.0
 
 [mediatailor]
-mypy-boto3-mediatailor<1.27.0,>=1.26.0
+mypy-boto3-mediatailor<1.28.0,>=1.27.0
 
 [memorydb]
-mypy-boto3-memorydb<1.27.0,>=1.26.0
+mypy-boto3-memorydb<1.28.0,>=1.27.0
 
 [meteringmarketplace]
-mypy-boto3-meteringmarketplace<1.27.0,>=1.26.0
+mypy-boto3-meteringmarketplace<1.28.0,>=1.27.0
 
 [mgh]
-mypy-boto3-mgh<1.27.0,>=1.26.0
+mypy-boto3-mgh<1.28.0,>=1.27.0
 
 [mgn]
-mypy-boto3-mgn<1.27.0,>=1.26.0
+mypy-boto3-mgn<1.28.0,>=1.27.0
 
 [migration-hub-refactor-spaces]
-mypy-boto3-migration-hub-refactor-spaces<1.27.0,>=1.26.0
+mypy-boto3-migration-hub-refactor-spaces<1.28.0,>=1.27.0
 
 [migrationhub-config]
-mypy-boto3-migrationhub-config<1.27.0,>=1.26.0
+mypy-boto3-migrationhub-config<1.28.0,>=1.27.0
 
 [migrationhuborchestrator]
-mypy-boto3-migrationhuborchestrator<1.27.0,>=1.26.0
+mypy-boto3-migrationhuborchestrator<1.28.0,>=1.27.0
 
 [migrationhubstrategy]
-mypy-boto3-migrationhubstrategy<1.27.0,>=1.26.0
+mypy-boto3-migrationhubstrategy<1.28.0,>=1.27.0
 
 [mobile]
-mypy-boto3-mobile<1.27.0,>=1.26.0
+mypy-boto3-mobile<1.28.0,>=1.27.0
 
 [mq]
-mypy-boto3-mq<1.27.0,>=1.26.0
+mypy-boto3-mq<1.28.0,>=1.27.0
 
 [mturk]
-mypy-boto3-mturk<1.27.0,>=1.26.0
+mypy-boto3-mturk<1.28.0,>=1.27.0
 
 [mwaa]
-mypy-boto3-mwaa<1.27.0,>=1.26.0
+mypy-boto3-mwaa<1.28.0,>=1.27.0
 
 [neptune]
-mypy-boto3-neptune<1.27.0,>=1.26.0
+mypy-boto3-neptune<1.28.0,>=1.27.0
 
 [network-firewall]
-mypy-boto3-network-firewall<1.27.0,>=1.26.0
+mypy-boto3-network-firewall<1.28.0,>=1.27.0
 
 [networkmanager]
-mypy-boto3-networkmanager<1.27.0,>=1.26.0
+mypy-boto3-networkmanager<1.28.0,>=1.27.0
 
 [nimble]
-mypy-boto3-nimble<1.27.0,>=1.26.0
+mypy-boto3-nimble<1.28.0,>=1.27.0
 
 [oam]
-mypy-boto3-oam<1.27.0,>=1.26.0
+mypy-boto3-oam<1.28.0,>=1.27.0
 
 [omics]
-mypy-boto3-omics<1.27.0,>=1.26.0
+mypy-boto3-omics<1.28.0,>=1.27.0
 
 [opensearch]
-mypy-boto3-opensearch<1.27.0,>=1.26.0
+mypy-boto3-opensearch<1.28.0,>=1.27.0
 
 [opensearchserverless]
-mypy-boto3-opensearchserverless<1.27.0,>=1.26.0
+mypy-boto3-opensearchserverless<1.28.0,>=1.27.0
 
 [opsworks]
-mypy-boto3-opsworks<1.27.0,>=1.26.0
+mypy-boto3-opsworks<1.28.0,>=1.27.0
 
 [opsworkscm]
-mypy-boto3-opsworkscm<1.27.0,>=1.26.0
+mypy-boto3-opsworkscm<1.28.0,>=1.27.0
 
 [organizations]
-mypy-boto3-organizations<1.27.0,>=1.26.0
+mypy-boto3-organizations<1.28.0,>=1.27.0
+
+[osis]
+mypy-boto3-osis<1.28.0,>=1.27.0
 
 [outposts]
-mypy-boto3-outposts<1.27.0,>=1.26.0
+mypy-boto3-outposts<1.28.0,>=1.27.0
 
 [panorama]
-mypy-boto3-panorama<1.27.0,>=1.26.0
+mypy-boto3-panorama<1.28.0,>=1.27.0
+
+[payment-cryptography]
+mypy-boto3-payment-cryptography<1.28.0,>=1.27.0
+
+[payment-cryptography-data]
+mypy-boto3-payment-cryptography-data<1.28.0,>=1.27.0
 
 [personalize]
-mypy-boto3-personalize<1.27.0,>=1.26.0
+mypy-boto3-personalize<1.28.0,>=1.27.0
 
 [personalize-events]
-mypy-boto3-personalize-events<1.27.0,>=1.26.0
+mypy-boto3-personalize-events<1.28.0,>=1.27.0
 
 [personalize-runtime]
-mypy-boto3-personalize-runtime<1.27.0,>=1.26.0
+mypy-boto3-personalize-runtime<1.28.0,>=1.27.0
 
 [pi]
-mypy-boto3-pi<1.27.0,>=1.26.0
+mypy-boto3-pi<1.28.0,>=1.27.0
 
 [pinpoint]
-mypy-boto3-pinpoint<1.27.0,>=1.26.0
+mypy-boto3-pinpoint<1.28.0,>=1.27.0
 
 [pinpoint-email]
-mypy-boto3-pinpoint-email<1.27.0,>=1.26.0
+mypy-boto3-pinpoint-email<1.28.0,>=1.27.0
 
 [pinpoint-sms-voice]
-mypy-boto3-pinpoint-sms-voice<1.27.0,>=1.26.0
+mypy-boto3-pinpoint-sms-voice<1.28.0,>=1.27.0
 
 [pinpoint-sms-voice-v2]
-mypy-boto3-pinpoint-sms-voice-v2<1.27.0,>=1.26.0
+mypy-boto3-pinpoint-sms-voice-v2<1.28.0,>=1.27.0
 
 [pipes]
-mypy-boto3-pipes<1.27.0,>=1.26.0
+mypy-boto3-pipes<1.28.0,>=1.27.0
 
 [polly]
-mypy-boto3-polly<1.27.0,>=1.26.0
+mypy-boto3-polly<1.28.0,>=1.27.0
 
 [pricing]
-mypy-boto3-pricing<1.27.0,>=1.26.0
+mypy-boto3-pricing<1.28.0,>=1.27.0
 
 [privatenetworks]
-mypy-boto3-privatenetworks<1.27.0,>=1.26.0
+mypy-boto3-privatenetworks<1.28.0,>=1.27.0
 
 [proton]
-mypy-boto3-proton<1.27.0,>=1.26.0
+mypy-boto3-proton<1.28.0,>=1.27.0
 
 [qldb]
-mypy-boto3-qldb<1.27.0,>=1.26.0
+mypy-boto3-qldb<1.28.0,>=1.27.0
 
 [qldb-session]
-mypy-boto3-qldb-session<1.27.0,>=1.26.0
+mypy-boto3-qldb-session<1.28.0,>=1.27.0
 
 [quicksight]
-mypy-boto3-quicksight<1.27.0,>=1.26.0
+mypy-boto3-quicksight<1.28.0,>=1.27.0
 
 [ram]
-mypy-boto3-ram<1.27.0,>=1.26.0
+mypy-boto3-ram<1.28.0,>=1.27.0
 
 [rbin]
-mypy-boto3-rbin<1.27.0,>=1.26.0
+mypy-boto3-rbin<1.28.0,>=1.27.0
 
 [rds]
-mypy-boto3-rds<1.27.0,>=1.26.0
+mypy-boto3-rds<1.28.0,>=1.27.0
 
 [rds-data]
-mypy-boto3-rds-data<1.27.0,>=1.26.0
+mypy-boto3-rds-data<1.28.0,>=1.27.0
 
 [redshift]
-mypy-boto3-redshift<1.27.0,>=1.26.0
+mypy-boto3-redshift<1.28.0,>=1.27.0
 
 [redshift-data]
-mypy-boto3-redshift-data<1.27.0,>=1.26.0
+mypy-boto3-redshift-data<1.28.0,>=1.27.0
 
 [redshift-serverless]
-mypy-boto3-redshift-serverless<1.27.0,>=1.26.0
+mypy-boto3-redshift-serverless<1.28.0,>=1.27.0
 
 [rekognition]
-mypy-boto3-rekognition<1.27.0,>=1.26.0
+mypy-boto3-rekognition<1.28.0,>=1.27.0
 
 [resiliencehub]
-mypy-boto3-resiliencehub<1.27.0,>=1.26.0
+mypy-boto3-resiliencehub<1.28.0,>=1.27.0
 
 [resource-explorer-2]
-mypy-boto3-resource-explorer-2<1.27.0,>=1.26.0
+mypy-boto3-resource-explorer-2<1.28.0,>=1.27.0
 
 [resource-groups]
-mypy-boto3-resource-groups<1.27.0,>=1.26.0
+mypy-boto3-resource-groups<1.28.0,>=1.27.0
 
 [resourcegroupstaggingapi]
-mypy-boto3-resourcegroupstaggingapi<1.27.0,>=1.26.0
+mypy-boto3-resourcegroupstaggingapi<1.28.0,>=1.27.0
 
 [robomaker]
-mypy-boto3-robomaker<1.27.0,>=1.26.0
+mypy-boto3-robomaker<1.28.0,>=1.27.0
 
 [rolesanywhere]
-mypy-boto3-rolesanywhere<1.27.0,>=1.26.0
+mypy-boto3-rolesanywhere<1.28.0,>=1.27.0
 
 [route53]
-mypy-boto3-route53<1.27.0,>=1.26.0
+mypy-boto3-route53<1.28.0,>=1.27.0
 
 [route53-recovery-cluster]
-mypy-boto3-route53-recovery-cluster<1.27.0,>=1.26.0
+mypy-boto3-route53-recovery-cluster<1.28.0,>=1.27.0
 
 [route53-recovery-control-config]
-mypy-boto3-route53-recovery-control-config<1.27.0,>=1.26.0
+mypy-boto3-route53-recovery-control-config<1.28.0,>=1.27.0
 
 [route53-recovery-readiness]
-mypy-boto3-route53-recovery-readiness<1.27.0,>=1.26.0
+mypy-boto3-route53-recovery-readiness<1.28.0,>=1.27.0
 
 [route53domains]
-mypy-boto3-route53domains<1.27.0,>=1.26.0
+mypy-boto3-route53domains<1.28.0,>=1.27.0
 
 [route53resolver]
-mypy-boto3-route53resolver<1.27.0,>=1.26.0
+mypy-boto3-route53resolver<1.28.0,>=1.27.0
 
 [rum]
-mypy-boto3-rum<1.27.0,>=1.26.0
+mypy-boto3-rum<1.28.0,>=1.27.0
 
 [s3]
-mypy-boto3-s3<1.27.0,>=1.26.0
+mypy-boto3-s3<1.28.0,>=1.27.0
 
 [s3control]
-mypy-boto3-s3control<1.27.0,>=1.26.0
+mypy-boto3-s3control<1.28.0,>=1.27.0
 
 [s3outposts]
-mypy-boto3-s3outposts<1.27.0,>=1.26.0
+mypy-boto3-s3outposts<1.28.0,>=1.27.0
 
 [sagemaker]
-mypy-boto3-sagemaker<1.27.0,>=1.26.0
+mypy-boto3-sagemaker<1.28.0,>=1.27.0
 
 [sagemaker-a2i-runtime]
-mypy-boto3-sagemaker-a2i-runtime<1.27.0,>=1.26.0
+mypy-boto3-sagemaker-a2i-runtime<1.28.0,>=1.27.0
 
 [sagemaker-edge]
-mypy-boto3-sagemaker-edge<1.27.0,>=1.26.0
+mypy-boto3-sagemaker-edge<1.28.0,>=1.27.0
 
 [sagemaker-featurestore-runtime]
-mypy-boto3-sagemaker-featurestore-runtime<1.27.0,>=1.26.0
+mypy-boto3-sagemaker-featurestore-runtime<1.28.0,>=1.27.0
 
 [sagemaker-geospatial]
-mypy-boto3-sagemaker-geospatial<1.27.0,>=1.26.0
+mypy-boto3-sagemaker-geospatial<1.28.0,>=1.27.0
 
 [sagemaker-metrics]
-mypy-boto3-sagemaker-metrics<1.27.0,>=1.26.0
+mypy-boto3-sagemaker-metrics<1.28.0,>=1.27.0
 
 [sagemaker-runtime]
-mypy-boto3-sagemaker-runtime<1.27.0,>=1.26.0
+mypy-boto3-sagemaker-runtime<1.28.0,>=1.27.0
 
 [savingsplans]
-mypy-boto3-savingsplans<1.27.0,>=1.26.0
+mypy-boto3-savingsplans<1.28.0,>=1.27.0
 
 [scheduler]
-mypy-boto3-scheduler<1.27.0,>=1.26.0
+mypy-boto3-scheduler<1.28.0,>=1.27.0
 
 [schemas]
-mypy-boto3-schemas<1.27.0,>=1.26.0
+mypy-boto3-schemas<1.28.0,>=1.27.0
 
 [sdb]
-mypy-boto3-sdb<1.27.0,>=1.26.0
+mypy-boto3-sdb<1.28.0,>=1.27.0
 
 [secretsmanager]
-mypy-boto3-secretsmanager<1.27.0,>=1.26.0
+mypy-boto3-secretsmanager<1.28.0,>=1.27.0
 
 [securityhub]
-mypy-boto3-securityhub<1.27.0,>=1.26.0
+mypy-boto3-securityhub<1.28.0,>=1.27.0
 
 [securitylake]
-mypy-boto3-securitylake<1.27.0,>=1.26.0
+mypy-boto3-securitylake<1.28.0,>=1.27.0
 
 [serverlessrepo]
-mypy-boto3-serverlessrepo<1.27.0,>=1.26.0
+mypy-boto3-serverlessrepo<1.28.0,>=1.27.0
 
 [service-quotas]
-mypy-boto3-service-quotas<1.27.0,>=1.26.0
+mypy-boto3-service-quotas<1.28.0,>=1.27.0
 
 [servicecatalog]
-mypy-boto3-servicecatalog<1.27.0,>=1.26.0
+mypy-boto3-servicecatalog<1.28.0,>=1.27.0
 
 [servicecatalog-appregistry]
-mypy-boto3-servicecatalog-appregistry<1.27.0,>=1.26.0
+mypy-boto3-servicecatalog-appregistry<1.28.0,>=1.27.0
 
 [servicediscovery]
-mypy-boto3-servicediscovery<1.27.0,>=1.26.0
+mypy-boto3-servicediscovery<1.28.0,>=1.27.0
 
 [ses]
-mypy-boto3-ses<1.27.0,>=1.26.0
+mypy-boto3-ses<1.28.0,>=1.27.0
 
 [sesv2]
-mypy-boto3-sesv2<1.27.0,>=1.26.0
+mypy-boto3-sesv2<1.28.0,>=1.27.0
 
 [shield]
-mypy-boto3-shield<1.27.0,>=1.26.0
+mypy-boto3-shield<1.28.0,>=1.27.0
 
 [signer]
-mypy-boto3-signer<1.27.0,>=1.26.0
+mypy-boto3-signer<1.28.0,>=1.27.0
 
 [simspaceweaver]
-mypy-boto3-simspaceweaver<1.27.0,>=1.26.0
+mypy-boto3-simspaceweaver<1.28.0,>=1.27.0
 
 [sms]
-mypy-boto3-sms<1.27.0,>=1.26.0
+mypy-boto3-sms<1.28.0,>=1.27.0
 
 [sms-voice]
-mypy-boto3-sms-voice<1.27.0,>=1.26.0
+mypy-boto3-sms-voice<1.28.0,>=1.27.0
 
 [snow-device-management]
-mypy-boto3-snow-device-management<1.27.0,>=1.26.0
+mypy-boto3-snow-device-management<1.28.0,>=1.27.0
 
 [snowball]
-mypy-boto3-snowball<1.27.0,>=1.26.0
+mypy-boto3-snowball<1.28.0,>=1.27.0
 
 [sns]
-mypy-boto3-sns<1.27.0,>=1.26.0
+mypy-boto3-sns<1.28.0,>=1.27.0
 
 [sqs]
-mypy-boto3-sqs<1.27.0,>=1.26.0
+mypy-boto3-sqs<1.28.0,>=1.27.0
 
 [ssm]
-mypy-boto3-ssm<1.27.0,>=1.26.0
+mypy-boto3-ssm<1.28.0,>=1.27.0
 
 [ssm-contacts]
-mypy-boto3-ssm-contacts<1.27.0,>=1.26.0
+mypy-boto3-ssm-contacts<1.28.0,>=1.27.0
 
 [ssm-incidents]
-mypy-boto3-ssm-incidents<1.27.0,>=1.26.0
+mypy-boto3-ssm-incidents<1.28.0,>=1.27.0
 
 [ssm-sap]
-mypy-boto3-ssm-sap<1.27.0,>=1.26.0
+mypy-boto3-ssm-sap<1.28.0,>=1.27.0
 
 [sso]
-mypy-boto3-sso<1.27.0,>=1.26.0
+mypy-boto3-sso<1.28.0,>=1.27.0
 
 [sso-admin]
-mypy-boto3-sso-admin<1.27.0,>=1.26.0
+mypy-boto3-sso-admin<1.28.0,>=1.27.0
 
 [sso-oidc]
-mypy-boto3-sso-oidc<1.27.0,>=1.26.0
+mypy-boto3-sso-oidc<1.28.0,>=1.27.0
 
 [stepfunctions]
-mypy-boto3-stepfunctions<1.27.0,>=1.26.0
+mypy-boto3-stepfunctions<1.28.0,>=1.27.0
 
 [storagegateway]
-mypy-boto3-storagegateway<1.27.0,>=1.26.0
+mypy-boto3-storagegateway<1.28.0,>=1.27.0
 
 [sts]
-mypy-boto3-sts<1.27.0,>=1.26.0
+mypy-boto3-sts<1.28.0,>=1.27.0
 
 [support]
-mypy-boto3-support<1.27.0,>=1.26.0
+mypy-boto3-support<1.28.0,>=1.27.0
 
 [support-app]
-mypy-boto3-support-app<1.27.0,>=1.26.0
+mypy-boto3-support-app<1.28.0,>=1.27.0
 
 [swf]
-mypy-boto3-swf<1.27.0,>=1.26.0
+mypy-boto3-swf<1.28.0,>=1.27.0
 
 [synthetics]
-mypy-boto3-synthetics<1.27.0,>=1.26.0
+mypy-boto3-synthetics<1.28.0,>=1.27.0
 
 [textract]
-mypy-boto3-textract<1.27.0,>=1.26.0
+mypy-boto3-textract<1.28.0,>=1.27.0
 
 [timestream-query]
-mypy-boto3-timestream-query<1.27.0,>=1.26.0
+mypy-boto3-timestream-query<1.28.0,>=1.27.0
 
 [timestream-write]
-mypy-boto3-timestream-write<1.27.0,>=1.26.0
+mypy-boto3-timestream-write<1.28.0,>=1.27.0
 
 [tnb]
-mypy-boto3-tnb<1.27.0,>=1.26.0
+mypy-boto3-tnb<1.28.0,>=1.27.0
 
 [transcribe]
-mypy-boto3-transcribe<1.27.0,>=1.26.0
+mypy-boto3-transcribe<1.28.0,>=1.27.0
 
 [transfer]
-mypy-boto3-transfer<1.27.0,>=1.26.0
+mypy-boto3-transfer<1.28.0,>=1.27.0
 
 [translate]
-mypy-boto3-translate<1.27.0,>=1.26.0
+mypy-boto3-translate<1.28.0,>=1.27.0
+
+[verifiedpermissions]
+mypy-boto3-verifiedpermissions<1.28.0,>=1.27.0
 
 [voice-id]
-mypy-boto3-voice-id<1.27.0,>=1.26.0
+mypy-boto3-voice-id<1.28.0,>=1.27.0
+
+[vpc-lattice]
+mypy-boto3-vpc-lattice<1.28.0,>=1.27.0
 
 [waf]
-mypy-boto3-waf<1.27.0,>=1.26.0
+mypy-boto3-waf<1.28.0,>=1.27.0
 
 [waf-regional]
-mypy-boto3-waf-regional<1.27.0,>=1.26.0
+mypy-boto3-waf-regional<1.28.0,>=1.27.0
 
 [wafv2]
-mypy-boto3-wafv2<1.27.0,>=1.26.0
+mypy-boto3-wafv2<1.28.0,>=1.27.0
 
 [wellarchitected]
-mypy-boto3-wellarchitected<1.27.0,>=1.26.0
+mypy-boto3-wellarchitected<1.28.0,>=1.27.0
 
 [wisdom]
-mypy-boto3-wisdom<1.27.0,>=1.26.0
+mypy-boto3-wisdom<1.28.0,>=1.27.0
 
 [workdocs]
-mypy-boto3-workdocs<1.27.0,>=1.26.0
+mypy-boto3-workdocs<1.28.0,>=1.27.0
 
 [worklink]
-mypy-boto3-worklink<1.27.0,>=1.26.0
+mypy-boto3-worklink<1.28.0,>=1.27.0
 
 [workmail]
-mypy-boto3-workmail<1.27.0,>=1.26.0
+mypy-boto3-workmail<1.28.0,>=1.27.0
 
 [workmailmessageflow]
-mypy-boto3-workmailmessageflow<1.27.0,>=1.26.0
+mypy-boto3-workmailmessageflow<1.28.0,>=1.27.0
 
 [workspaces]
-mypy-boto3-workspaces<1.27.0,>=1.26.0
+mypy-boto3-workspaces<1.28.0,>=1.27.0
 
 [workspaces-web]
-mypy-boto3-workspaces-web<1.27.0,>=1.26.0
+mypy-boto3-workspaces-web<1.28.0,>=1.27.0
 
 [xray]
-mypy-boto3-xray<1.27.0,>=1.26.0
+mypy-boto3-xray<1.28.0,>=1.27.0
```

### Comparing `boto3-stubs-1.26.99/setup.py` & `boto3-stubs-1.27.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="boto3-stubs",
-    version="1.26.99",
+    version="1.27.0",
     packages=["boto3-stubs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3 1.26.99 generated with mypy-boto3-builder 7.14.2",
+    description="Type annotations for boto3 1.27.0 generated with mypy-boto3-builder 7.14.5",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
@@ -48,721 +48,737 @@
     install_requires=[
         "botocore-stubs",
         "types-s3transfer",
         'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     extras_require={
         "all": [
-            "mypy-boto3-accessanalyzer>=1.26.0, <1.27.0",
-            "mypy-boto3-account>=1.26.0, <1.27.0",
-            "mypy-boto3-acm>=1.26.0, <1.27.0",
-            "mypy-boto3-acm-pca>=1.26.0, <1.27.0",
-            "mypy-boto3-alexaforbusiness>=1.26.0, <1.27.0",
-            "mypy-boto3-amp>=1.26.0, <1.27.0",
-            "mypy-boto3-amplify>=1.26.0, <1.27.0",
-            "mypy-boto3-amplifybackend>=1.26.0, <1.27.0",
-            "mypy-boto3-amplifyuibuilder>=1.26.0, <1.27.0",
-            "mypy-boto3-apigateway>=1.26.0, <1.27.0",
-            "mypy-boto3-apigatewaymanagementapi>=1.26.0, <1.27.0",
-            "mypy-boto3-apigatewayv2>=1.26.0, <1.27.0",
-            "mypy-boto3-appconfig>=1.26.0, <1.27.0",
-            "mypy-boto3-appconfigdata>=1.26.0, <1.27.0",
-            "mypy-boto3-appflow>=1.26.0, <1.27.0",
-            "mypy-boto3-appintegrations>=1.26.0, <1.27.0",
-            "mypy-boto3-application-autoscaling>=1.26.0, <1.27.0",
-            "mypy-boto3-application-insights>=1.26.0, <1.27.0",
-            "mypy-boto3-applicationcostprofiler>=1.26.0, <1.27.0",
-            "mypy-boto3-appmesh>=1.26.0, <1.27.0",
-            "mypy-boto3-apprunner>=1.26.0, <1.27.0",
-            "mypy-boto3-appstream>=1.26.0, <1.27.0",
-            "mypy-boto3-appsync>=1.26.0, <1.27.0",
-            "mypy-boto3-arc-zonal-shift>=1.26.0, <1.27.0",
-            "mypy-boto3-athena>=1.26.0, <1.27.0",
-            "mypy-boto3-auditmanager>=1.26.0, <1.27.0",
-            "mypy-boto3-autoscaling>=1.26.0, <1.27.0",
-            "mypy-boto3-autoscaling-plans>=1.26.0, <1.27.0",
-            "mypy-boto3-backup>=1.26.0, <1.27.0",
-            "mypy-boto3-backup-gateway>=1.26.0, <1.27.0",
-            "mypy-boto3-backupstorage>=1.26.0, <1.27.0",
-            "mypy-boto3-batch>=1.26.0, <1.27.0",
-            "mypy-boto3-billingconductor>=1.26.0, <1.27.0",
-            "mypy-boto3-braket>=1.26.0, <1.27.0",
-            "mypy-boto3-budgets>=1.26.0, <1.27.0",
-            "mypy-boto3-ce>=1.26.0, <1.27.0",
-            "mypy-boto3-chime>=1.26.0, <1.27.0",
-            "mypy-boto3-chime-sdk-identity>=1.26.0, <1.27.0",
-            "mypy-boto3-chime-sdk-media-pipelines>=1.26.0, <1.27.0",
-            "mypy-boto3-chime-sdk-meetings>=1.26.0, <1.27.0",
-            "mypy-boto3-chime-sdk-messaging>=1.26.0, <1.27.0",
-            "mypy-boto3-chime-sdk-voice>=1.26.0, <1.27.0",
-            "mypy-boto3-cleanrooms>=1.26.0, <1.27.0",
-            "mypy-boto3-cloud9>=1.26.0, <1.27.0",
-            "mypy-boto3-cloudcontrol>=1.26.0, <1.27.0",
-            "mypy-boto3-clouddirectory>=1.26.0, <1.27.0",
-            "mypy-boto3-cloudformation>=1.26.0, <1.27.0",
-            "mypy-boto3-cloudfront>=1.26.0, <1.27.0",
-            "mypy-boto3-cloudhsm>=1.26.0, <1.27.0",
-            "mypy-boto3-cloudhsmv2>=1.26.0, <1.27.0",
-            "mypy-boto3-cloudsearch>=1.26.0, <1.27.0",
-            "mypy-boto3-cloudsearchdomain>=1.26.0, <1.27.0",
-            "mypy-boto3-cloudtrail>=1.26.0, <1.27.0",
-            "mypy-boto3-cloudtrail-data>=1.26.0, <1.27.0",
-            "mypy-boto3-cloudwatch>=1.26.0, <1.27.0",
-            "mypy-boto3-codeartifact>=1.26.0, <1.27.0",
-            "mypy-boto3-codebuild>=1.26.0, <1.27.0",
-            "mypy-boto3-codecatalyst>=1.26.0, <1.27.0",
-            "mypy-boto3-codecommit>=1.26.0, <1.27.0",
-            "mypy-boto3-codedeploy>=1.26.0, <1.27.0",
-            "mypy-boto3-codeguru-reviewer>=1.26.0, <1.27.0",
-            "mypy-boto3-codeguruprofiler>=1.26.0, <1.27.0",
-            "mypy-boto3-codepipeline>=1.26.0, <1.27.0",
-            "mypy-boto3-codestar>=1.26.0, <1.27.0",
-            "mypy-boto3-codestar-connections>=1.26.0, <1.27.0",
-            "mypy-boto3-codestar-notifications>=1.26.0, <1.27.0",
-            "mypy-boto3-cognito-identity>=1.26.0, <1.27.0",
-            "mypy-boto3-cognito-idp>=1.26.0, <1.27.0",
-            "mypy-boto3-cognito-sync>=1.26.0, <1.27.0",
-            "mypy-boto3-comprehend>=1.26.0, <1.27.0",
-            "mypy-boto3-comprehendmedical>=1.26.0, <1.27.0",
-            "mypy-boto3-compute-optimizer>=1.26.0, <1.27.0",
-            "mypy-boto3-config>=1.26.0, <1.27.0",
-            "mypy-boto3-connect>=1.26.0, <1.27.0",
-            "mypy-boto3-connect-contact-lens>=1.26.0, <1.27.0",
-            "mypy-boto3-connectcampaigns>=1.26.0, <1.27.0",
-            "mypy-boto3-connectcases>=1.26.0, <1.27.0",
-            "mypy-boto3-connectparticipant>=1.26.0, <1.27.0",
-            "mypy-boto3-controltower>=1.26.0, <1.27.0",
-            "mypy-boto3-cur>=1.26.0, <1.27.0",
-            "mypy-boto3-customer-profiles>=1.26.0, <1.27.0",
-            "mypy-boto3-databrew>=1.26.0, <1.27.0",
-            "mypy-boto3-dataexchange>=1.26.0, <1.27.0",
-            "mypy-boto3-datapipeline>=1.26.0, <1.27.0",
-            "mypy-boto3-datasync>=1.26.0, <1.27.0",
-            "mypy-boto3-dax>=1.26.0, <1.27.0",
-            "mypy-boto3-detective>=1.26.0, <1.27.0",
-            "mypy-boto3-devicefarm>=1.26.0, <1.27.0",
-            "mypy-boto3-devops-guru>=1.26.0, <1.27.0",
-            "mypy-boto3-directconnect>=1.26.0, <1.27.0",
-            "mypy-boto3-discovery>=1.26.0, <1.27.0",
-            "mypy-boto3-dlm>=1.26.0, <1.27.0",
-            "mypy-boto3-dms>=1.26.0, <1.27.0",
-            "mypy-boto3-docdb>=1.26.0, <1.27.0",
-            "mypy-boto3-docdb-elastic>=1.26.0, <1.27.0",
-            "mypy-boto3-drs>=1.26.0, <1.27.0",
-            "mypy-boto3-ds>=1.26.0, <1.27.0",
-            "mypy-boto3-dynamodb>=1.26.0, <1.27.0",
-            "mypy-boto3-dynamodbstreams>=1.26.0, <1.27.0",
-            "mypy-boto3-ebs>=1.26.0, <1.27.0",
-            "mypy-boto3-ec2>=1.26.0, <1.27.0",
-            "mypy-boto3-ec2-instance-connect>=1.26.0, <1.27.0",
-            "mypy-boto3-ecr>=1.26.0, <1.27.0",
-            "mypy-boto3-ecr-public>=1.26.0, <1.27.0",
-            "mypy-boto3-ecs>=1.26.0, <1.27.0",
-            "mypy-boto3-efs>=1.26.0, <1.27.0",
-            "mypy-boto3-eks>=1.26.0, <1.27.0",
-            "mypy-boto3-elastic-inference>=1.26.0, <1.27.0",
-            "mypy-boto3-elasticache>=1.26.0, <1.27.0",
-            "mypy-boto3-elasticbeanstalk>=1.26.0, <1.27.0",
-            "mypy-boto3-elastictranscoder>=1.26.0, <1.27.0",
-            "mypy-boto3-elb>=1.26.0, <1.27.0",
-            "mypy-boto3-elbv2>=1.26.0, <1.27.0",
-            "mypy-boto3-emr>=1.26.0, <1.27.0",
-            "mypy-boto3-emr-containers>=1.26.0, <1.27.0",
-            "mypy-boto3-emr-serverless>=1.26.0, <1.27.0",
-            "mypy-boto3-es>=1.26.0, <1.27.0",
-            "mypy-boto3-events>=1.26.0, <1.27.0",
-            "mypy-boto3-evidently>=1.26.0, <1.27.0",
-            "mypy-boto3-finspace>=1.26.0, <1.27.0",
-            "mypy-boto3-finspace-data>=1.26.0, <1.27.0",
-            "mypy-boto3-firehose>=1.26.0, <1.27.0",
-            "mypy-boto3-fis>=1.26.0, <1.27.0",
-            "mypy-boto3-fms>=1.26.0, <1.27.0",
-            "mypy-boto3-forecast>=1.26.0, <1.27.0",
-            "mypy-boto3-forecastquery>=1.26.0, <1.27.0",
-            "mypy-boto3-frauddetector>=1.26.0, <1.27.0",
-            "mypy-boto3-fsx>=1.26.0, <1.27.0",
-            "mypy-boto3-gamelift>=1.26.0, <1.27.0",
-            "mypy-boto3-gamesparks>=1.26.0, <1.27.0",
-            "mypy-boto3-glacier>=1.26.0, <1.27.0",
-            "mypy-boto3-globalaccelerator>=1.26.0, <1.27.0",
-            "mypy-boto3-glue>=1.26.0, <1.27.0",
-            "mypy-boto3-grafana>=1.26.0, <1.27.0",
-            "mypy-boto3-greengrass>=1.26.0, <1.27.0",
-            "mypy-boto3-greengrassv2>=1.26.0, <1.27.0",
-            "mypy-boto3-groundstation>=1.26.0, <1.27.0",
-            "mypy-boto3-guardduty>=1.26.0, <1.27.0",
-            "mypy-boto3-health>=1.26.0, <1.27.0",
-            "mypy-boto3-healthlake>=1.26.0, <1.27.0",
-            "mypy-boto3-honeycode>=1.26.0, <1.27.0",
-            "mypy-boto3-iam>=1.26.0, <1.27.0",
-            "mypy-boto3-identitystore>=1.26.0, <1.27.0",
-            "mypy-boto3-imagebuilder>=1.26.0, <1.27.0",
-            "mypy-boto3-importexport>=1.26.0, <1.27.0",
-            "mypy-boto3-inspector>=1.26.0, <1.27.0",
-            "mypy-boto3-inspector2>=1.26.0, <1.27.0",
-            "mypy-boto3-internetmonitor>=1.26.0, <1.27.0",
-            "mypy-boto3-iot>=1.26.0, <1.27.0",
-            "mypy-boto3-iot-data>=1.26.0, <1.27.0",
-            "mypy-boto3-iot-jobs-data>=1.26.0, <1.27.0",
-            "mypy-boto3-iot-roborunner>=1.26.0, <1.27.0",
-            "mypy-boto3-iot1click-devices>=1.26.0, <1.27.0",
-            "mypy-boto3-iot1click-projects>=1.26.0, <1.27.0",
-            "mypy-boto3-iotanalytics>=1.26.0, <1.27.0",
-            "mypy-boto3-iotdeviceadvisor>=1.26.0, <1.27.0",
-            "mypy-boto3-iotevents>=1.26.0, <1.27.0",
-            "mypy-boto3-iotevents-data>=1.26.0, <1.27.0",
-            "mypy-boto3-iotfleethub>=1.26.0, <1.27.0",
-            "mypy-boto3-iotfleetwise>=1.26.0, <1.27.0",
-            "mypy-boto3-iotsecuretunneling>=1.26.0, <1.27.0",
-            "mypy-boto3-iotsitewise>=1.26.0, <1.27.0",
-            "mypy-boto3-iotthingsgraph>=1.26.0, <1.27.0",
-            "mypy-boto3-iottwinmaker>=1.26.0, <1.27.0",
-            "mypy-boto3-iotwireless>=1.26.0, <1.27.0",
-            "mypy-boto3-ivs>=1.26.0, <1.27.0",
-            "mypy-boto3-ivs-realtime>=1.26.0, <1.27.0",
-            "mypy-boto3-ivschat>=1.26.0, <1.27.0",
-            "mypy-boto3-kafka>=1.26.0, <1.27.0",
-            "mypy-boto3-kafkaconnect>=1.26.0, <1.27.0",
-            "mypy-boto3-kendra>=1.26.0, <1.27.0",
-            "mypy-boto3-kendra-ranking>=1.26.0, <1.27.0",
-            "mypy-boto3-keyspaces>=1.26.0, <1.27.0",
-            "mypy-boto3-kinesis>=1.26.0, <1.27.0",
-            "mypy-boto3-kinesis-video-archived-media>=1.26.0, <1.27.0",
-            "mypy-boto3-kinesis-video-media>=1.26.0, <1.27.0",
-            "mypy-boto3-kinesis-video-signaling>=1.26.0, <1.27.0",
-            "mypy-boto3-kinesis-video-webrtc-storage>=1.26.0, <1.27.0",
-            "mypy-boto3-kinesisanalytics>=1.26.0, <1.27.0",
-            "mypy-boto3-kinesisanalyticsv2>=1.26.0, <1.27.0",
-            "mypy-boto3-kinesisvideo>=1.26.0, <1.27.0",
-            "mypy-boto3-kms>=1.26.0, <1.27.0",
-            "mypy-boto3-lakeformation>=1.26.0, <1.27.0",
-            "mypy-boto3-lambda>=1.26.0, <1.27.0",
-            "mypy-boto3-lex-models>=1.26.0, <1.27.0",
-            "mypy-boto3-lex-runtime>=1.26.0, <1.27.0",
-            "mypy-boto3-lexv2-models>=1.26.0, <1.27.0",
-            "mypy-boto3-lexv2-runtime>=1.26.0, <1.27.0",
-            "mypy-boto3-license-manager>=1.26.0, <1.27.0",
-            "mypy-boto3-license-manager-linux-subscriptions>=1.26.0, <1.27.0",
-            "mypy-boto3-license-manager-user-subscriptions>=1.26.0, <1.27.0",
-            "mypy-boto3-lightsail>=1.26.0, <1.27.0",
-            "mypy-boto3-location>=1.26.0, <1.27.0",
-            "mypy-boto3-logs>=1.26.0, <1.27.0",
-            "mypy-boto3-lookoutequipment>=1.26.0, <1.27.0",
-            "mypy-boto3-lookoutmetrics>=1.26.0, <1.27.0",
-            "mypy-boto3-lookoutvision>=1.26.0, <1.27.0",
-            "mypy-boto3-m2>=1.26.0, <1.27.0",
-            "mypy-boto3-machinelearning>=1.26.0, <1.27.0",
-            "mypy-boto3-macie>=1.26.0, <1.27.0",
-            "mypy-boto3-macie2>=1.26.0, <1.27.0",
-            "mypy-boto3-managedblockchain>=1.26.0, <1.27.0",
-            "mypy-boto3-marketplace-catalog>=1.26.0, <1.27.0",
-            "mypy-boto3-marketplace-entitlement>=1.26.0, <1.27.0",
-            "mypy-boto3-marketplacecommerceanalytics>=1.26.0, <1.27.0",
-            "mypy-boto3-mediaconnect>=1.26.0, <1.27.0",
-            "mypy-boto3-mediaconvert>=1.26.0, <1.27.0",
-            "mypy-boto3-medialive>=1.26.0, <1.27.0",
-            "mypy-boto3-mediapackage>=1.26.0, <1.27.0",
-            "mypy-boto3-mediapackage-vod>=1.26.0, <1.27.0",
-            "mypy-boto3-mediastore>=1.26.0, <1.27.0",
-            "mypy-boto3-mediastore-data>=1.26.0, <1.27.0",
-            "mypy-boto3-mediatailor>=1.26.0, <1.27.0",
-            "mypy-boto3-memorydb>=1.26.0, <1.27.0",
-            "mypy-boto3-meteringmarketplace>=1.26.0, <1.27.0",
-            "mypy-boto3-mgh>=1.26.0, <1.27.0",
-            "mypy-boto3-mgn>=1.26.0, <1.27.0",
-            "mypy-boto3-migration-hub-refactor-spaces>=1.26.0, <1.27.0",
-            "mypy-boto3-migrationhub-config>=1.26.0, <1.27.0",
-            "mypy-boto3-migrationhuborchestrator>=1.26.0, <1.27.0",
-            "mypy-boto3-migrationhubstrategy>=1.26.0, <1.27.0",
-            "mypy-boto3-mobile>=1.26.0, <1.27.0",
-            "mypy-boto3-mq>=1.26.0, <1.27.0",
-            "mypy-boto3-mturk>=1.26.0, <1.27.0",
-            "mypy-boto3-mwaa>=1.26.0, <1.27.0",
-            "mypy-boto3-neptune>=1.26.0, <1.27.0",
-            "mypy-boto3-network-firewall>=1.26.0, <1.27.0",
-            "mypy-boto3-networkmanager>=1.26.0, <1.27.0",
-            "mypy-boto3-nimble>=1.26.0, <1.27.0",
-            "mypy-boto3-oam>=1.26.0, <1.27.0",
-            "mypy-boto3-omics>=1.26.0, <1.27.0",
-            "mypy-boto3-opensearch>=1.26.0, <1.27.0",
-            "mypy-boto3-opensearchserverless>=1.26.0, <1.27.0",
-            "mypy-boto3-opsworks>=1.26.0, <1.27.0",
-            "mypy-boto3-opsworkscm>=1.26.0, <1.27.0",
-            "mypy-boto3-organizations>=1.26.0, <1.27.0",
-            "mypy-boto3-outposts>=1.26.0, <1.27.0",
-            "mypy-boto3-panorama>=1.26.0, <1.27.0",
-            "mypy-boto3-personalize>=1.26.0, <1.27.0",
-            "mypy-boto3-personalize-events>=1.26.0, <1.27.0",
-            "mypy-boto3-personalize-runtime>=1.26.0, <1.27.0",
-            "mypy-boto3-pi>=1.26.0, <1.27.0",
-            "mypy-boto3-pinpoint>=1.26.0, <1.27.0",
-            "mypy-boto3-pinpoint-email>=1.26.0, <1.27.0",
-            "mypy-boto3-pinpoint-sms-voice>=1.26.0, <1.27.0",
-            "mypy-boto3-pinpoint-sms-voice-v2>=1.26.0, <1.27.0",
-            "mypy-boto3-pipes>=1.26.0, <1.27.0",
-            "mypy-boto3-polly>=1.26.0, <1.27.0",
-            "mypy-boto3-pricing>=1.26.0, <1.27.0",
-            "mypy-boto3-privatenetworks>=1.26.0, <1.27.0",
-            "mypy-boto3-proton>=1.26.0, <1.27.0",
-            "mypy-boto3-qldb>=1.26.0, <1.27.0",
-            "mypy-boto3-qldb-session>=1.26.0, <1.27.0",
-            "mypy-boto3-quicksight>=1.26.0, <1.27.0",
-            "mypy-boto3-ram>=1.26.0, <1.27.0",
-            "mypy-boto3-rbin>=1.26.0, <1.27.0",
-            "mypy-boto3-rds>=1.26.0, <1.27.0",
-            "mypy-boto3-rds-data>=1.26.0, <1.27.0",
-            "mypy-boto3-redshift>=1.26.0, <1.27.0",
-            "mypy-boto3-redshift-data>=1.26.0, <1.27.0",
-            "mypy-boto3-redshift-serverless>=1.26.0, <1.27.0",
-            "mypy-boto3-rekognition>=1.26.0, <1.27.0",
-            "mypy-boto3-resiliencehub>=1.26.0, <1.27.0",
-            "mypy-boto3-resource-explorer-2>=1.26.0, <1.27.0",
-            "mypy-boto3-resource-groups>=1.26.0, <1.27.0",
-            "mypy-boto3-resourcegroupstaggingapi>=1.26.0, <1.27.0",
-            "mypy-boto3-robomaker>=1.26.0, <1.27.0",
-            "mypy-boto3-rolesanywhere>=1.26.0, <1.27.0",
-            "mypy-boto3-route53>=1.26.0, <1.27.0",
-            "mypy-boto3-route53-recovery-cluster>=1.26.0, <1.27.0",
-            "mypy-boto3-route53-recovery-control-config>=1.26.0, <1.27.0",
-            "mypy-boto3-route53-recovery-readiness>=1.26.0, <1.27.0",
-            "mypy-boto3-route53domains>=1.26.0, <1.27.0",
-            "mypy-boto3-route53resolver>=1.26.0, <1.27.0",
-            "mypy-boto3-rum>=1.26.0, <1.27.0",
-            "mypy-boto3-s3>=1.26.0, <1.27.0",
-            "mypy-boto3-s3control>=1.26.0, <1.27.0",
-            "mypy-boto3-s3outposts>=1.26.0, <1.27.0",
-            "mypy-boto3-sagemaker>=1.26.0, <1.27.0",
-            "mypy-boto3-sagemaker-a2i-runtime>=1.26.0, <1.27.0",
-            "mypy-boto3-sagemaker-edge>=1.26.0, <1.27.0",
-            "mypy-boto3-sagemaker-featurestore-runtime>=1.26.0, <1.27.0",
-            "mypy-boto3-sagemaker-geospatial>=1.26.0, <1.27.0",
-            "mypy-boto3-sagemaker-metrics>=1.26.0, <1.27.0",
-            "mypy-boto3-sagemaker-runtime>=1.26.0, <1.27.0",
-            "mypy-boto3-savingsplans>=1.26.0, <1.27.0",
-            "mypy-boto3-scheduler>=1.26.0, <1.27.0",
-            "mypy-boto3-schemas>=1.26.0, <1.27.0",
-            "mypy-boto3-sdb>=1.26.0, <1.27.0",
-            "mypy-boto3-secretsmanager>=1.26.0, <1.27.0",
-            "mypy-boto3-securityhub>=1.26.0, <1.27.0",
-            "mypy-boto3-securitylake>=1.26.0, <1.27.0",
-            "mypy-boto3-serverlessrepo>=1.26.0, <1.27.0",
-            "mypy-boto3-service-quotas>=1.26.0, <1.27.0",
-            "mypy-boto3-servicecatalog>=1.26.0, <1.27.0",
-            "mypy-boto3-servicecatalog-appregistry>=1.26.0, <1.27.0",
-            "mypy-boto3-servicediscovery>=1.26.0, <1.27.0",
-            "mypy-boto3-ses>=1.26.0, <1.27.0",
-            "mypy-boto3-sesv2>=1.26.0, <1.27.0",
-            "mypy-boto3-shield>=1.26.0, <1.27.0",
-            "mypy-boto3-signer>=1.26.0, <1.27.0",
-            "mypy-boto3-simspaceweaver>=1.26.0, <1.27.0",
-            "mypy-boto3-sms>=1.26.0, <1.27.0",
-            "mypy-boto3-sms-voice>=1.26.0, <1.27.0",
-            "mypy-boto3-snow-device-management>=1.26.0, <1.27.0",
-            "mypy-boto3-snowball>=1.26.0, <1.27.0",
-            "mypy-boto3-sns>=1.26.0, <1.27.0",
-            "mypy-boto3-sqs>=1.26.0, <1.27.0",
-            "mypy-boto3-ssm>=1.26.0, <1.27.0",
-            "mypy-boto3-ssm-contacts>=1.26.0, <1.27.0",
-            "mypy-boto3-ssm-incidents>=1.26.0, <1.27.0",
-            "mypy-boto3-ssm-sap>=1.26.0, <1.27.0",
-            "mypy-boto3-sso>=1.26.0, <1.27.0",
-            "mypy-boto3-sso-admin>=1.26.0, <1.27.0",
-            "mypy-boto3-sso-oidc>=1.26.0, <1.27.0",
-            "mypy-boto3-stepfunctions>=1.26.0, <1.27.0",
-            "mypy-boto3-storagegateway>=1.26.0, <1.27.0",
-            "mypy-boto3-sts>=1.26.0, <1.27.0",
-            "mypy-boto3-support>=1.26.0, <1.27.0",
-            "mypy-boto3-support-app>=1.26.0, <1.27.0",
-            "mypy-boto3-swf>=1.26.0, <1.27.0",
-            "mypy-boto3-synthetics>=1.26.0, <1.27.0",
-            "mypy-boto3-textract>=1.26.0, <1.27.0",
-            "mypy-boto3-timestream-query>=1.26.0, <1.27.0",
-            "mypy-boto3-timestream-write>=1.26.0, <1.27.0",
-            "mypy-boto3-tnb>=1.26.0, <1.27.0",
-            "mypy-boto3-transcribe>=1.26.0, <1.27.0",
-            "mypy-boto3-transfer>=1.26.0, <1.27.0",
-            "mypy-boto3-translate>=1.26.0, <1.27.0",
-            "mypy-boto3-voice-id>=1.26.0, <1.27.0",
-            "mypy-boto3-waf>=1.26.0, <1.27.0",
-            "mypy-boto3-waf-regional>=1.26.0, <1.27.0",
-            "mypy-boto3-wafv2>=1.26.0, <1.27.0",
-            "mypy-boto3-wellarchitected>=1.26.0, <1.27.0",
-            "mypy-boto3-wisdom>=1.26.0, <1.27.0",
-            "mypy-boto3-workdocs>=1.26.0, <1.27.0",
-            "mypy-boto3-worklink>=1.26.0, <1.27.0",
-            "mypy-boto3-workmail>=1.26.0, <1.27.0",
-            "mypy-boto3-workmailmessageflow>=1.26.0, <1.27.0",
-            "mypy-boto3-workspaces>=1.26.0, <1.27.0",
-            "mypy-boto3-workspaces-web>=1.26.0, <1.27.0",
-            "mypy-boto3-xray>=1.26.0, <1.27.0",
+            "mypy-boto3-accessanalyzer>=1.27.0, <1.28.0",
+            "mypy-boto3-account>=1.27.0, <1.28.0",
+            "mypy-boto3-acm>=1.27.0, <1.28.0",
+            "mypy-boto3-acm-pca>=1.27.0, <1.28.0",
+            "mypy-boto3-alexaforbusiness>=1.27.0, <1.28.0",
+            "mypy-boto3-amp>=1.27.0, <1.28.0",
+            "mypy-boto3-amplify>=1.27.0, <1.28.0",
+            "mypy-boto3-amplifybackend>=1.27.0, <1.28.0",
+            "mypy-boto3-amplifyuibuilder>=1.27.0, <1.28.0",
+            "mypy-boto3-apigateway>=1.27.0, <1.28.0",
+            "mypy-boto3-apigatewaymanagementapi>=1.27.0, <1.28.0",
+            "mypy-boto3-apigatewayv2>=1.27.0, <1.28.0",
+            "mypy-boto3-appconfig>=1.27.0, <1.28.0",
+            "mypy-boto3-appconfigdata>=1.27.0, <1.28.0",
+            "mypy-boto3-appfabric>=1.27.0, <1.28.0",
+            "mypy-boto3-appflow>=1.27.0, <1.28.0",
+            "mypy-boto3-appintegrations>=1.27.0, <1.28.0",
+            "mypy-boto3-application-autoscaling>=1.27.0, <1.28.0",
+            "mypy-boto3-application-insights>=1.27.0, <1.28.0",
+            "mypy-boto3-applicationcostprofiler>=1.27.0, <1.28.0",
+            "mypy-boto3-appmesh>=1.27.0, <1.28.0",
+            "mypy-boto3-apprunner>=1.27.0, <1.28.0",
+            "mypy-boto3-appstream>=1.27.0, <1.28.0",
+            "mypy-boto3-appsync>=1.27.0, <1.28.0",
+            "mypy-boto3-arc-zonal-shift>=1.27.0, <1.28.0",
+            "mypy-boto3-athena>=1.27.0, <1.28.0",
+            "mypy-boto3-auditmanager>=1.27.0, <1.28.0",
+            "mypy-boto3-autoscaling>=1.27.0, <1.28.0",
+            "mypy-boto3-autoscaling-plans>=1.27.0, <1.28.0",
+            "mypy-boto3-backup>=1.27.0, <1.28.0",
+            "mypy-boto3-backup-gateway>=1.27.0, <1.28.0",
+            "mypy-boto3-backupstorage>=1.27.0, <1.28.0",
+            "mypy-boto3-batch>=1.27.0, <1.28.0",
+            "mypy-boto3-billingconductor>=1.27.0, <1.28.0",
+            "mypy-boto3-braket>=1.27.0, <1.28.0",
+            "mypy-boto3-budgets>=1.27.0, <1.28.0",
+            "mypy-boto3-ce>=1.27.0, <1.28.0",
+            "mypy-boto3-chime>=1.27.0, <1.28.0",
+            "mypy-boto3-chime-sdk-identity>=1.27.0, <1.28.0",
+            "mypy-boto3-chime-sdk-media-pipelines>=1.27.0, <1.28.0",
+            "mypy-boto3-chime-sdk-meetings>=1.27.0, <1.28.0",
+            "mypy-boto3-chime-sdk-messaging>=1.27.0, <1.28.0",
+            "mypy-boto3-chime-sdk-voice>=1.27.0, <1.28.0",
+            "mypy-boto3-cleanrooms>=1.27.0, <1.28.0",
+            "mypy-boto3-cloud9>=1.27.0, <1.28.0",
+            "mypy-boto3-cloudcontrol>=1.27.0, <1.28.0",
+            "mypy-boto3-clouddirectory>=1.27.0, <1.28.0",
+            "mypy-boto3-cloudformation>=1.27.0, <1.28.0",
+            "mypy-boto3-cloudfront>=1.27.0, <1.28.0",
+            "mypy-boto3-cloudhsm>=1.27.0, <1.28.0",
+            "mypy-boto3-cloudhsmv2>=1.27.0, <1.28.0",
+            "mypy-boto3-cloudsearch>=1.27.0, <1.28.0",
+            "mypy-boto3-cloudsearchdomain>=1.27.0, <1.28.0",
+            "mypy-boto3-cloudtrail>=1.27.0, <1.28.0",
+            "mypy-boto3-cloudtrail-data>=1.27.0, <1.28.0",
+            "mypy-boto3-cloudwatch>=1.27.0, <1.28.0",
+            "mypy-boto3-codeartifact>=1.27.0, <1.28.0",
+            "mypy-boto3-codebuild>=1.27.0, <1.28.0",
+            "mypy-boto3-codecatalyst>=1.27.0, <1.28.0",
+            "mypy-boto3-codecommit>=1.27.0, <1.28.0",
+            "mypy-boto3-codedeploy>=1.27.0, <1.28.0",
+            "mypy-boto3-codeguru-reviewer>=1.27.0, <1.28.0",
+            "mypy-boto3-codeguru-security>=1.27.0, <1.28.0",
+            "mypy-boto3-codeguruprofiler>=1.27.0, <1.28.0",
+            "mypy-boto3-codepipeline>=1.27.0, <1.28.0",
+            "mypy-boto3-codestar>=1.27.0, <1.28.0",
+            "mypy-boto3-codestar-connections>=1.27.0, <1.28.0",
+            "mypy-boto3-codestar-notifications>=1.27.0, <1.28.0",
+            "mypy-boto3-cognito-identity>=1.27.0, <1.28.0",
+            "mypy-boto3-cognito-idp>=1.27.0, <1.28.0",
+            "mypy-boto3-cognito-sync>=1.27.0, <1.28.0",
+            "mypy-boto3-comprehend>=1.27.0, <1.28.0",
+            "mypy-boto3-comprehendmedical>=1.27.0, <1.28.0",
+            "mypy-boto3-compute-optimizer>=1.27.0, <1.28.0",
+            "mypy-boto3-config>=1.27.0, <1.28.0",
+            "mypy-boto3-connect>=1.27.0, <1.28.0",
+            "mypy-boto3-connect-contact-lens>=1.27.0, <1.28.0",
+            "mypy-boto3-connectcampaigns>=1.27.0, <1.28.0",
+            "mypy-boto3-connectcases>=1.27.0, <1.28.0",
+            "mypy-boto3-connectparticipant>=1.27.0, <1.28.0",
+            "mypy-boto3-controltower>=1.27.0, <1.28.0",
+            "mypy-boto3-cur>=1.27.0, <1.28.0",
+            "mypy-boto3-customer-profiles>=1.27.0, <1.28.0",
+            "mypy-boto3-databrew>=1.27.0, <1.28.0",
+            "mypy-boto3-dataexchange>=1.27.0, <1.28.0",
+            "mypy-boto3-datapipeline>=1.27.0, <1.28.0",
+            "mypy-boto3-datasync>=1.27.0, <1.28.0",
+            "mypy-boto3-dax>=1.27.0, <1.28.0",
+            "mypy-boto3-detective>=1.27.0, <1.28.0",
+            "mypy-boto3-devicefarm>=1.27.0, <1.28.0",
+            "mypy-boto3-devops-guru>=1.27.0, <1.28.0",
+            "mypy-boto3-directconnect>=1.27.0, <1.28.0",
+            "mypy-boto3-discovery>=1.27.0, <1.28.0",
+            "mypy-boto3-dlm>=1.27.0, <1.28.0",
+            "mypy-boto3-dms>=1.27.0, <1.28.0",
+            "mypy-boto3-docdb>=1.27.0, <1.28.0",
+            "mypy-boto3-docdb-elastic>=1.27.0, <1.28.0",
+            "mypy-boto3-drs>=1.27.0, <1.28.0",
+            "mypy-boto3-ds>=1.27.0, <1.28.0",
+            "mypy-boto3-dynamodb>=1.27.0, <1.28.0",
+            "mypy-boto3-dynamodbstreams>=1.27.0, <1.28.0",
+            "mypy-boto3-ebs>=1.27.0, <1.28.0",
+            "mypy-boto3-ec2>=1.27.0, <1.28.0",
+            "mypy-boto3-ec2-instance-connect>=1.27.0, <1.28.0",
+            "mypy-boto3-ecr>=1.27.0, <1.28.0",
+            "mypy-boto3-ecr-public>=1.27.0, <1.28.0",
+            "mypy-boto3-ecs>=1.27.0, <1.28.0",
+            "mypy-boto3-efs>=1.27.0, <1.28.0",
+            "mypy-boto3-eks>=1.27.0, <1.28.0",
+            "mypy-boto3-elastic-inference>=1.27.0, <1.28.0",
+            "mypy-boto3-elasticache>=1.27.0, <1.28.0",
+            "mypy-boto3-elasticbeanstalk>=1.27.0, <1.28.0",
+            "mypy-boto3-elastictranscoder>=1.27.0, <1.28.0",
+            "mypy-boto3-elb>=1.27.0, <1.28.0",
+            "mypy-boto3-elbv2>=1.27.0, <1.28.0",
+            "mypy-boto3-emr>=1.27.0, <1.28.0",
+            "mypy-boto3-emr-containers>=1.27.0, <1.28.0",
+            "mypy-boto3-emr-serverless>=1.27.0, <1.28.0",
+            "mypy-boto3-es>=1.27.0, <1.28.0",
+            "mypy-boto3-events>=1.27.0, <1.28.0",
+            "mypy-boto3-evidently>=1.27.0, <1.28.0",
+            "mypy-boto3-finspace>=1.27.0, <1.28.0",
+            "mypy-boto3-finspace-data>=1.27.0, <1.28.0",
+            "mypy-boto3-firehose>=1.27.0, <1.28.0",
+            "mypy-boto3-fis>=1.27.0, <1.28.0",
+            "mypy-boto3-fms>=1.27.0, <1.28.0",
+            "mypy-boto3-forecast>=1.27.0, <1.28.0",
+            "mypy-boto3-forecastquery>=1.27.0, <1.28.0",
+            "mypy-boto3-frauddetector>=1.27.0, <1.28.0",
+            "mypy-boto3-fsx>=1.27.0, <1.28.0",
+            "mypy-boto3-gamelift>=1.27.0, <1.28.0",
+            "mypy-boto3-gamesparks>=1.27.0, <1.28.0",
+            "mypy-boto3-glacier>=1.27.0, <1.28.0",
+            "mypy-boto3-globalaccelerator>=1.27.0, <1.28.0",
+            "mypy-boto3-glue>=1.27.0, <1.28.0",
+            "mypy-boto3-grafana>=1.27.0, <1.28.0",
+            "mypy-boto3-greengrass>=1.27.0, <1.28.0",
+            "mypy-boto3-greengrassv2>=1.27.0, <1.28.0",
+            "mypy-boto3-groundstation>=1.27.0, <1.28.0",
+            "mypy-boto3-guardduty>=1.27.0, <1.28.0",
+            "mypy-boto3-health>=1.27.0, <1.28.0",
+            "mypy-boto3-healthlake>=1.27.0, <1.28.0",
+            "mypy-boto3-honeycode>=1.27.0, <1.28.0",
+            "mypy-boto3-iam>=1.27.0, <1.28.0",
+            "mypy-boto3-identitystore>=1.27.0, <1.28.0",
+            "mypy-boto3-imagebuilder>=1.27.0, <1.28.0",
+            "mypy-boto3-importexport>=1.27.0, <1.28.0",
+            "mypy-boto3-inspector>=1.27.0, <1.28.0",
+            "mypy-boto3-inspector2>=1.27.0, <1.28.0",
+            "mypy-boto3-internetmonitor>=1.27.0, <1.28.0",
+            "mypy-boto3-iot>=1.27.0, <1.28.0",
+            "mypy-boto3-iot-data>=1.27.0, <1.28.0",
+            "mypy-boto3-iot-jobs-data>=1.27.0, <1.28.0",
+            "mypy-boto3-iot-roborunner>=1.27.0, <1.28.0",
+            "mypy-boto3-iot1click-devices>=1.27.0, <1.28.0",
+            "mypy-boto3-iot1click-projects>=1.27.0, <1.28.0",
+            "mypy-boto3-iotanalytics>=1.27.0, <1.28.0",
+            "mypy-boto3-iotdeviceadvisor>=1.27.0, <1.28.0",
+            "mypy-boto3-iotevents>=1.27.0, <1.28.0",
+            "mypy-boto3-iotevents-data>=1.27.0, <1.28.0",
+            "mypy-boto3-iotfleethub>=1.27.0, <1.28.0",
+            "mypy-boto3-iotfleetwise>=1.27.0, <1.28.0",
+            "mypy-boto3-iotsecuretunneling>=1.27.0, <1.28.0",
+            "mypy-boto3-iotsitewise>=1.27.0, <1.28.0",
+            "mypy-boto3-iotthingsgraph>=1.27.0, <1.28.0",
+            "mypy-boto3-iottwinmaker>=1.27.0, <1.28.0",
+            "mypy-boto3-iotwireless>=1.27.0, <1.28.0",
+            "mypy-boto3-ivs>=1.27.0, <1.28.0",
+            "mypy-boto3-ivs-realtime>=1.27.0, <1.28.0",
+            "mypy-boto3-ivschat>=1.27.0, <1.28.0",
+            "mypy-boto3-kafka>=1.27.0, <1.28.0",
+            "mypy-boto3-kafkaconnect>=1.27.0, <1.28.0",
+            "mypy-boto3-kendra>=1.27.0, <1.28.0",
+            "mypy-boto3-kendra-ranking>=1.27.0, <1.28.0",
+            "mypy-boto3-keyspaces>=1.27.0, <1.28.0",
+            "mypy-boto3-kinesis>=1.27.0, <1.28.0",
+            "mypy-boto3-kinesis-video-archived-media>=1.27.0, <1.28.0",
+            "mypy-boto3-kinesis-video-media>=1.27.0, <1.28.0",
+            "mypy-boto3-kinesis-video-signaling>=1.27.0, <1.28.0",
+            "mypy-boto3-kinesis-video-webrtc-storage>=1.27.0, <1.28.0",
+            "mypy-boto3-kinesisanalytics>=1.27.0, <1.28.0",
+            "mypy-boto3-kinesisanalyticsv2>=1.27.0, <1.28.0",
+            "mypy-boto3-kinesisvideo>=1.27.0, <1.28.0",
+            "mypy-boto3-kms>=1.27.0, <1.28.0",
+            "mypy-boto3-lakeformation>=1.27.0, <1.28.0",
+            "mypy-boto3-lambda>=1.27.0, <1.28.0",
+            "mypy-boto3-lex-models>=1.27.0, <1.28.0",
+            "mypy-boto3-lex-runtime>=1.27.0, <1.28.0",
+            "mypy-boto3-lexv2-models>=1.27.0, <1.28.0",
+            "mypy-boto3-lexv2-runtime>=1.27.0, <1.28.0",
+            "mypy-boto3-license-manager>=1.27.0, <1.28.0",
+            "mypy-boto3-license-manager-linux-subscriptions>=1.27.0, <1.28.0",
+            "mypy-boto3-license-manager-user-subscriptions>=1.27.0, <1.28.0",
+            "mypy-boto3-lightsail>=1.27.0, <1.28.0",
+            "mypy-boto3-location>=1.27.0, <1.28.0",
+            "mypy-boto3-logs>=1.27.0, <1.28.0",
+            "mypy-boto3-lookoutequipment>=1.27.0, <1.28.0",
+            "mypy-boto3-lookoutmetrics>=1.27.0, <1.28.0",
+            "mypy-boto3-lookoutvision>=1.27.0, <1.28.0",
+            "mypy-boto3-m2>=1.27.0, <1.28.0",
+            "mypy-boto3-machinelearning>=1.27.0, <1.28.0",
+            "mypy-boto3-macie>=1.27.0, <1.28.0",
+            "mypy-boto3-macie2>=1.27.0, <1.28.0",
+            "mypy-boto3-managedblockchain>=1.27.0, <1.28.0",
+            "mypy-boto3-marketplace-catalog>=1.27.0, <1.28.0",
+            "mypy-boto3-marketplace-entitlement>=1.27.0, <1.28.0",
+            "mypy-boto3-marketplacecommerceanalytics>=1.27.0, <1.28.0",
+            "mypy-boto3-mediaconnect>=1.27.0, <1.28.0",
+            "mypy-boto3-mediaconvert>=1.27.0, <1.28.0",
+            "mypy-boto3-medialive>=1.27.0, <1.28.0",
+            "mypy-boto3-mediapackage>=1.27.0, <1.28.0",
+            "mypy-boto3-mediapackage-vod>=1.27.0, <1.28.0",
+            "mypy-boto3-mediapackagev2>=1.27.0, <1.28.0",
+            "mypy-boto3-mediastore>=1.27.0, <1.28.0",
+            "mypy-boto3-mediastore-data>=1.27.0, <1.28.0",
+            "mypy-boto3-mediatailor>=1.27.0, <1.28.0",
+            "mypy-boto3-memorydb>=1.27.0, <1.28.0",
+            "mypy-boto3-meteringmarketplace>=1.27.0, <1.28.0",
+            "mypy-boto3-mgh>=1.27.0, <1.28.0",
+            "mypy-boto3-mgn>=1.27.0, <1.28.0",
+            "mypy-boto3-migration-hub-refactor-spaces>=1.27.0, <1.28.0",
+            "mypy-boto3-migrationhub-config>=1.27.0, <1.28.0",
+            "mypy-boto3-migrationhuborchestrator>=1.27.0, <1.28.0",
+            "mypy-boto3-migrationhubstrategy>=1.27.0, <1.28.0",
+            "mypy-boto3-mobile>=1.27.0, <1.28.0",
+            "mypy-boto3-mq>=1.27.0, <1.28.0",
+            "mypy-boto3-mturk>=1.27.0, <1.28.0",
+            "mypy-boto3-mwaa>=1.27.0, <1.28.0",
+            "mypy-boto3-neptune>=1.27.0, <1.28.0",
+            "mypy-boto3-network-firewall>=1.27.0, <1.28.0",
+            "mypy-boto3-networkmanager>=1.27.0, <1.28.0",
+            "mypy-boto3-nimble>=1.27.0, <1.28.0",
+            "mypy-boto3-oam>=1.27.0, <1.28.0",
+            "mypy-boto3-omics>=1.27.0, <1.28.0",
+            "mypy-boto3-opensearch>=1.27.0, <1.28.0",
+            "mypy-boto3-opensearchserverless>=1.27.0, <1.28.0",
+            "mypy-boto3-opsworks>=1.27.0, <1.28.0",
+            "mypy-boto3-opsworkscm>=1.27.0, <1.28.0",
+            "mypy-boto3-organizations>=1.27.0, <1.28.0",
+            "mypy-boto3-osis>=1.27.0, <1.28.0",
+            "mypy-boto3-outposts>=1.27.0, <1.28.0",
+            "mypy-boto3-panorama>=1.27.0, <1.28.0",
+            "mypy-boto3-payment-cryptography>=1.27.0, <1.28.0",
+            "mypy-boto3-payment-cryptography-data>=1.27.0, <1.28.0",
+            "mypy-boto3-personalize>=1.27.0, <1.28.0",
+            "mypy-boto3-personalize-events>=1.27.0, <1.28.0",
+            "mypy-boto3-personalize-runtime>=1.27.0, <1.28.0",
+            "mypy-boto3-pi>=1.27.0, <1.28.0",
+            "mypy-boto3-pinpoint>=1.27.0, <1.28.0",
+            "mypy-boto3-pinpoint-email>=1.27.0, <1.28.0",
+            "mypy-boto3-pinpoint-sms-voice>=1.27.0, <1.28.0",
+            "mypy-boto3-pinpoint-sms-voice-v2>=1.27.0, <1.28.0",
+            "mypy-boto3-pipes>=1.27.0, <1.28.0",
+            "mypy-boto3-polly>=1.27.0, <1.28.0",
+            "mypy-boto3-pricing>=1.27.0, <1.28.0",
+            "mypy-boto3-privatenetworks>=1.27.0, <1.28.0",
+            "mypy-boto3-proton>=1.27.0, <1.28.0",
+            "mypy-boto3-qldb>=1.27.0, <1.28.0",
+            "mypy-boto3-qldb-session>=1.27.0, <1.28.0",
+            "mypy-boto3-quicksight>=1.27.0, <1.28.0",
+            "mypy-boto3-ram>=1.27.0, <1.28.0",
+            "mypy-boto3-rbin>=1.27.0, <1.28.0",
+            "mypy-boto3-rds>=1.27.0, <1.28.0",
+            "mypy-boto3-rds-data>=1.27.0, <1.28.0",
+            "mypy-boto3-redshift>=1.27.0, <1.28.0",
+            "mypy-boto3-redshift-data>=1.27.0, <1.28.0",
+            "mypy-boto3-redshift-serverless>=1.27.0, <1.28.0",
+            "mypy-boto3-rekognition>=1.27.0, <1.28.0",
+            "mypy-boto3-resiliencehub>=1.27.0, <1.28.0",
+            "mypy-boto3-resource-explorer-2>=1.27.0, <1.28.0",
+            "mypy-boto3-resource-groups>=1.27.0, <1.28.0",
+            "mypy-boto3-resourcegroupstaggingapi>=1.27.0, <1.28.0",
+            "mypy-boto3-robomaker>=1.27.0, <1.28.0",
+            "mypy-boto3-rolesanywhere>=1.27.0, <1.28.0",
+            "mypy-boto3-route53>=1.27.0, <1.28.0",
+            "mypy-boto3-route53-recovery-cluster>=1.27.0, <1.28.0",
+            "mypy-boto3-route53-recovery-control-config>=1.27.0, <1.28.0",
+            "mypy-boto3-route53-recovery-readiness>=1.27.0, <1.28.0",
+            "mypy-boto3-route53domains>=1.27.0, <1.28.0",
+            "mypy-boto3-route53resolver>=1.27.0, <1.28.0",
+            "mypy-boto3-rum>=1.27.0, <1.28.0",
+            "mypy-boto3-s3>=1.27.0, <1.28.0",
+            "mypy-boto3-s3control>=1.27.0, <1.28.0",
+            "mypy-boto3-s3outposts>=1.27.0, <1.28.0",
+            "mypy-boto3-sagemaker>=1.27.0, <1.28.0",
+            "mypy-boto3-sagemaker-a2i-runtime>=1.27.0, <1.28.0",
+            "mypy-boto3-sagemaker-edge>=1.27.0, <1.28.0",
+            "mypy-boto3-sagemaker-featurestore-runtime>=1.27.0, <1.28.0",
+            "mypy-boto3-sagemaker-geospatial>=1.27.0, <1.28.0",
+            "mypy-boto3-sagemaker-metrics>=1.27.0, <1.28.0",
+            "mypy-boto3-sagemaker-runtime>=1.27.0, <1.28.0",
+            "mypy-boto3-savingsplans>=1.27.0, <1.28.0",
+            "mypy-boto3-scheduler>=1.27.0, <1.28.0",
+            "mypy-boto3-schemas>=1.27.0, <1.28.0",
+            "mypy-boto3-sdb>=1.27.0, <1.28.0",
+            "mypy-boto3-secretsmanager>=1.27.0, <1.28.0",
+            "mypy-boto3-securityhub>=1.27.0, <1.28.0",
+            "mypy-boto3-securitylake>=1.27.0, <1.28.0",
+            "mypy-boto3-serverlessrepo>=1.27.0, <1.28.0",
+            "mypy-boto3-service-quotas>=1.27.0, <1.28.0",
+            "mypy-boto3-servicecatalog>=1.27.0, <1.28.0",
+            "mypy-boto3-servicecatalog-appregistry>=1.27.0, <1.28.0",
+            "mypy-boto3-servicediscovery>=1.27.0, <1.28.0",
+            "mypy-boto3-ses>=1.27.0, <1.28.0",
+            "mypy-boto3-sesv2>=1.27.0, <1.28.0",
+            "mypy-boto3-shield>=1.27.0, <1.28.0",
+            "mypy-boto3-signer>=1.27.0, <1.28.0",
+            "mypy-boto3-simspaceweaver>=1.27.0, <1.28.0",
+            "mypy-boto3-sms>=1.27.0, <1.28.0",
+            "mypy-boto3-sms-voice>=1.27.0, <1.28.0",
+            "mypy-boto3-snow-device-management>=1.27.0, <1.28.0",
+            "mypy-boto3-snowball>=1.27.0, <1.28.0",
+            "mypy-boto3-sns>=1.27.0, <1.28.0",
+            "mypy-boto3-sqs>=1.27.0, <1.28.0",
+            "mypy-boto3-ssm>=1.27.0, <1.28.0",
+            "mypy-boto3-ssm-contacts>=1.27.0, <1.28.0",
+            "mypy-boto3-ssm-incidents>=1.27.0, <1.28.0",
+            "mypy-boto3-ssm-sap>=1.27.0, <1.28.0",
+            "mypy-boto3-sso>=1.27.0, <1.28.0",
+            "mypy-boto3-sso-admin>=1.27.0, <1.28.0",
+            "mypy-boto3-sso-oidc>=1.27.0, <1.28.0",
+            "mypy-boto3-stepfunctions>=1.27.0, <1.28.0",
+            "mypy-boto3-storagegateway>=1.27.0, <1.28.0",
+            "mypy-boto3-sts>=1.27.0, <1.28.0",
+            "mypy-boto3-support>=1.27.0, <1.28.0",
+            "mypy-boto3-support-app>=1.27.0, <1.28.0",
+            "mypy-boto3-swf>=1.27.0, <1.28.0",
+            "mypy-boto3-synthetics>=1.27.0, <1.28.0",
+            "mypy-boto3-textract>=1.27.0, <1.28.0",
+            "mypy-boto3-timestream-query>=1.27.0, <1.28.0",
+            "mypy-boto3-timestream-write>=1.27.0, <1.28.0",
+            "mypy-boto3-tnb>=1.27.0, <1.28.0",
+            "mypy-boto3-transcribe>=1.27.0, <1.28.0",
+            "mypy-boto3-transfer>=1.27.0, <1.28.0",
+            "mypy-boto3-translate>=1.27.0, <1.28.0",
+            "mypy-boto3-verifiedpermissions>=1.27.0, <1.28.0",
+            "mypy-boto3-voice-id>=1.27.0, <1.28.0",
+            "mypy-boto3-vpc-lattice>=1.27.0, <1.28.0",
+            "mypy-boto3-waf>=1.27.0, <1.28.0",
+            "mypy-boto3-waf-regional>=1.27.0, <1.28.0",
+            "mypy-boto3-wafv2>=1.27.0, <1.28.0",
+            "mypy-boto3-wellarchitected>=1.27.0, <1.28.0",
+            "mypy-boto3-wisdom>=1.27.0, <1.28.0",
+            "mypy-boto3-workdocs>=1.27.0, <1.28.0",
+            "mypy-boto3-worklink>=1.27.0, <1.28.0",
+            "mypy-boto3-workmail>=1.27.0, <1.28.0",
+            "mypy-boto3-workmailmessageflow>=1.27.0, <1.28.0",
+            "mypy-boto3-workspaces>=1.27.0, <1.28.0",
+            "mypy-boto3-workspaces-web>=1.27.0, <1.28.0",
+            "mypy-boto3-xray>=1.27.0, <1.28.0",
         ],
         "essential": [
-            "mypy-boto3-cloudformation>=1.26.0, <1.27.0",
-            "mypy-boto3-dynamodb>=1.26.0, <1.27.0",
-            "mypy-boto3-ec2>=1.26.0, <1.27.0",
-            "mypy-boto3-lambda>=1.26.0, <1.27.0",
-            "mypy-boto3-rds>=1.26.0, <1.27.0",
-            "mypy-boto3-s3>=1.26.0, <1.27.0",
-            "mypy-boto3-sqs>=1.26.0, <1.27.0",
+            "mypy-boto3-cloudformation>=1.27.0, <1.28.0",
+            "mypy-boto3-dynamodb>=1.27.0, <1.28.0",
+            "mypy-boto3-ec2>=1.27.0, <1.28.0",
+            "mypy-boto3-lambda>=1.27.0, <1.28.0",
+            "mypy-boto3-rds>=1.27.0, <1.28.0",
+            "mypy-boto3-s3>=1.27.0, <1.28.0",
+            "mypy-boto3-sqs>=1.27.0, <1.28.0",
         ],
-        "boto3": ["boto3==1.26.99", "botocore==1.29.99"],
-        "accessanalyzer": ["mypy-boto3-accessanalyzer>=1.26.0, <1.27.0"],
-        "account": ["mypy-boto3-account>=1.26.0, <1.27.0"],
-        "acm": ["mypy-boto3-acm>=1.26.0, <1.27.0"],
-        "acm-pca": ["mypy-boto3-acm-pca>=1.26.0, <1.27.0"],
-        "alexaforbusiness": ["mypy-boto3-alexaforbusiness>=1.26.0, <1.27.0"],
-        "amp": ["mypy-boto3-amp>=1.26.0, <1.27.0"],
-        "amplify": ["mypy-boto3-amplify>=1.26.0, <1.27.0"],
-        "amplifybackend": ["mypy-boto3-amplifybackend>=1.26.0, <1.27.0"],
-        "amplifyuibuilder": ["mypy-boto3-amplifyuibuilder>=1.26.0, <1.27.0"],
-        "apigateway": ["mypy-boto3-apigateway>=1.26.0, <1.27.0"],
-        "apigatewaymanagementapi": ["mypy-boto3-apigatewaymanagementapi>=1.26.0, <1.27.0"],
-        "apigatewayv2": ["mypy-boto3-apigatewayv2>=1.26.0, <1.27.0"],
-        "appconfig": ["mypy-boto3-appconfig>=1.26.0, <1.27.0"],
-        "appconfigdata": ["mypy-boto3-appconfigdata>=1.26.0, <1.27.0"],
-        "appflow": ["mypy-boto3-appflow>=1.26.0, <1.27.0"],
-        "appintegrations": ["mypy-boto3-appintegrations>=1.26.0, <1.27.0"],
-        "application-autoscaling": ["mypy-boto3-application-autoscaling>=1.26.0, <1.27.0"],
-        "application-insights": ["mypy-boto3-application-insights>=1.26.0, <1.27.0"],
-        "applicationcostprofiler": ["mypy-boto3-applicationcostprofiler>=1.26.0, <1.27.0"],
-        "appmesh": ["mypy-boto3-appmesh>=1.26.0, <1.27.0"],
-        "apprunner": ["mypy-boto3-apprunner>=1.26.0, <1.27.0"],
-        "appstream": ["mypy-boto3-appstream>=1.26.0, <1.27.0"],
-        "appsync": ["mypy-boto3-appsync>=1.26.0, <1.27.0"],
-        "arc-zonal-shift": ["mypy-boto3-arc-zonal-shift>=1.26.0, <1.27.0"],
-        "athena": ["mypy-boto3-athena>=1.26.0, <1.27.0"],
-        "auditmanager": ["mypy-boto3-auditmanager>=1.26.0, <1.27.0"],
-        "autoscaling": ["mypy-boto3-autoscaling>=1.26.0, <1.27.0"],
-        "autoscaling-plans": ["mypy-boto3-autoscaling-plans>=1.26.0, <1.27.0"],
-        "backup": ["mypy-boto3-backup>=1.26.0, <1.27.0"],
-        "backup-gateway": ["mypy-boto3-backup-gateway>=1.26.0, <1.27.0"],
-        "backupstorage": ["mypy-boto3-backupstorage>=1.26.0, <1.27.0"],
-        "batch": ["mypy-boto3-batch>=1.26.0, <1.27.0"],
-        "billingconductor": ["mypy-boto3-billingconductor>=1.26.0, <1.27.0"],
-        "braket": ["mypy-boto3-braket>=1.26.0, <1.27.0"],
-        "budgets": ["mypy-boto3-budgets>=1.26.0, <1.27.0"],
-        "ce": ["mypy-boto3-ce>=1.26.0, <1.27.0"],
-        "chime": ["mypy-boto3-chime>=1.26.0, <1.27.0"],
-        "chime-sdk-identity": ["mypy-boto3-chime-sdk-identity>=1.26.0, <1.27.0"],
-        "chime-sdk-media-pipelines": ["mypy-boto3-chime-sdk-media-pipelines>=1.26.0, <1.27.0"],
-        "chime-sdk-meetings": ["mypy-boto3-chime-sdk-meetings>=1.26.0, <1.27.0"],
-        "chime-sdk-messaging": ["mypy-boto3-chime-sdk-messaging>=1.26.0, <1.27.0"],
-        "chime-sdk-voice": ["mypy-boto3-chime-sdk-voice>=1.26.0, <1.27.0"],
-        "cleanrooms": ["mypy-boto3-cleanrooms>=1.26.0, <1.27.0"],
-        "cloud9": ["mypy-boto3-cloud9>=1.26.0, <1.27.0"],
-        "cloudcontrol": ["mypy-boto3-cloudcontrol>=1.26.0, <1.27.0"],
-        "clouddirectory": ["mypy-boto3-clouddirectory>=1.26.0, <1.27.0"],
-        "cloudformation": ["mypy-boto3-cloudformation>=1.26.0, <1.27.0"],
-        "cloudfront": ["mypy-boto3-cloudfront>=1.26.0, <1.27.0"],
-        "cloudhsm": ["mypy-boto3-cloudhsm>=1.26.0, <1.27.0"],
-        "cloudhsmv2": ["mypy-boto3-cloudhsmv2>=1.26.0, <1.27.0"],
-        "cloudsearch": ["mypy-boto3-cloudsearch>=1.26.0, <1.27.0"],
-        "cloudsearchdomain": ["mypy-boto3-cloudsearchdomain>=1.26.0, <1.27.0"],
-        "cloudtrail": ["mypy-boto3-cloudtrail>=1.26.0, <1.27.0"],
-        "cloudtrail-data": ["mypy-boto3-cloudtrail-data>=1.26.0, <1.27.0"],
-        "cloudwatch": ["mypy-boto3-cloudwatch>=1.26.0, <1.27.0"],
-        "codeartifact": ["mypy-boto3-codeartifact>=1.26.0, <1.27.0"],
-        "codebuild": ["mypy-boto3-codebuild>=1.26.0, <1.27.0"],
-        "codecatalyst": ["mypy-boto3-codecatalyst>=1.26.0, <1.27.0"],
-        "codecommit": ["mypy-boto3-codecommit>=1.26.0, <1.27.0"],
-        "codedeploy": ["mypy-boto3-codedeploy>=1.26.0, <1.27.0"],
-        "codeguru-reviewer": ["mypy-boto3-codeguru-reviewer>=1.26.0, <1.27.0"],
-        "codeguruprofiler": ["mypy-boto3-codeguruprofiler>=1.26.0, <1.27.0"],
-        "codepipeline": ["mypy-boto3-codepipeline>=1.26.0, <1.27.0"],
-        "codestar": ["mypy-boto3-codestar>=1.26.0, <1.27.0"],
-        "codestar-connections": ["mypy-boto3-codestar-connections>=1.26.0, <1.27.0"],
-        "codestar-notifications": ["mypy-boto3-codestar-notifications>=1.26.0, <1.27.0"],
-        "cognito-identity": ["mypy-boto3-cognito-identity>=1.26.0, <1.27.0"],
-        "cognito-idp": ["mypy-boto3-cognito-idp>=1.26.0, <1.27.0"],
-        "cognito-sync": ["mypy-boto3-cognito-sync>=1.26.0, <1.27.0"],
-        "comprehend": ["mypy-boto3-comprehend>=1.26.0, <1.27.0"],
-        "comprehendmedical": ["mypy-boto3-comprehendmedical>=1.26.0, <1.27.0"],
-        "compute-optimizer": ["mypy-boto3-compute-optimizer>=1.26.0, <1.27.0"],
-        "config": ["mypy-boto3-config>=1.26.0, <1.27.0"],
-        "connect": ["mypy-boto3-connect>=1.26.0, <1.27.0"],
-        "connect-contact-lens": ["mypy-boto3-connect-contact-lens>=1.26.0, <1.27.0"],
-        "connectcampaigns": ["mypy-boto3-connectcampaigns>=1.26.0, <1.27.0"],
-        "connectcases": ["mypy-boto3-connectcases>=1.26.0, <1.27.0"],
-        "connectparticipant": ["mypy-boto3-connectparticipant>=1.26.0, <1.27.0"],
-        "controltower": ["mypy-boto3-controltower>=1.26.0, <1.27.0"],
-        "cur": ["mypy-boto3-cur>=1.26.0, <1.27.0"],
-        "customer-profiles": ["mypy-boto3-customer-profiles>=1.26.0, <1.27.0"],
-        "databrew": ["mypy-boto3-databrew>=1.26.0, <1.27.0"],
-        "dataexchange": ["mypy-boto3-dataexchange>=1.26.0, <1.27.0"],
-        "datapipeline": ["mypy-boto3-datapipeline>=1.26.0, <1.27.0"],
-        "datasync": ["mypy-boto3-datasync>=1.26.0, <1.27.0"],
-        "dax": ["mypy-boto3-dax>=1.26.0, <1.27.0"],
-        "detective": ["mypy-boto3-detective>=1.26.0, <1.27.0"],
-        "devicefarm": ["mypy-boto3-devicefarm>=1.26.0, <1.27.0"],
-        "devops-guru": ["mypy-boto3-devops-guru>=1.26.0, <1.27.0"],
-        "directconnect": ["mypy-boto3-directconnect>=1.26.0, <1.27.0"],
-        "discovery": ["mypy-boto3-discovery>=1.26.0, <1.27.0"],
-        "dlm": ["mypy-boto3-dlm>=1.26.0, <1.27.0"],
-        "dms": ["mypy-boto3-dms>=1.26.0, <1.27.0"],
-        "docdb": ["mypy-boto3-docdb>=1.26.0, <1.27.0"],
-        "docdb-elastic": ["mypy-boto3-docdb-elastic>=1.26.0, <1.27.0"],
-        "drs": ["mypy-boto3-drs>=1.26.0, <1.27.0"],
-        "ds": ["mypy-boto3-ds>=1.26.0, <1.27.0"],
-        "dynamodb": ["mypy-boto3-dynamodb>=1.26.0, <1.27.0"],
-        "dynamodbstreams": ["mypy-boto3-dynamodbstreams>=1.26.0, <1.27.0"],
-        "ebs": ["mypy-boto3-ebs>=1.26.0, <1.27.0"],
-        "ec2": ["mypy-boto3-ec2>=1.26.0, <1.27.0"],
-        "ec2-instance-connect": ["mypy-boto3-ec2-instance-connect>=1.26.0, <1.27.0"],
-        "ecr": ["mypy-boto3-ecr>=1.26.0, <1.27.0"],
-        "ecr-public": ["mypy-boto3-ecr-public>=1.26.0, <1.27.0"],
-        "ecs": ["mypy-boto3-ecs>=1.26.0, <1.27.0"],
-        "efs": ["mypy-boto3-efs>=1.26.0, <1.27.0"],
-        "eks": ["mypy-boto3-eks>=1.26.0, <1.27.0"],
-        "elastic-inference": ["mypy-boto3-elastic-inference>=1.26.0, <1.27.0"],
-        "elasticache": ["mypy-boto3-elasticache>=1.26.0, <1.27.0"],
-        "elasticbeanstalk": ["mypy-boto3-elasticbeanstalk>=1.26.0, <1.27.0"],
-        "elastictranscoder": ["mypy-boto3-elastictranscoder>=1.26.0, <1.27.0"],
-        "elb": ["mypy-boto3-elb>=1.26.0, <1.27.0"],
-        "elbv2": ["mypy-boto3-elbv2>=1.26.0, <1.27.0"],
-        "emr": ["mypy-boto3-emr>=1.26.0, <1.27.0"],
-        "emr-containers": ["mypy-boto3-emr-containers>=1.26.0, <1.27.0"],
-        "emr-serverless": ["mypy-boto3-emr-serverless>=1.26.0, <1.27.0"],
-        "es": ["mypy-boto3-es>=1.26.0, <1.27.0"],
-        "events": ["mypy-boto3-events>=1.26.0, <1.27.0"],
-        "evidently": ["mypy-boto3-evidently>=1.26.0, <1.27.0"],
-        "finspace": ["mypy-boto3-finspace>=1.26.0, <1.27.0"],
-        "finspace-data": ["mypy-boto3-finspace-data>=1.26.0, <1.27.0"],
-        "firehose": ["mypy-boto3-firehose>=1.26.0, <1.27.0"],
-        "fis": ["mypy-boto3-fis>=1.26.0, <1.27.0"],
-        "fms": ["mypy-boto3-fms>=1.26.0, <1.27.0"],
-        "forecast": ["mypy-boto3-forecast>=1.26.0, <1.27.0"],
-        "forecastquery": ["mypy-boto3-forecastquery>=1.26.0, <1.27.0"],
-        "frauddetector": ["mypy-boto3-frauddetector>=1.26.0, <1.27.0"],
-        "fsx": ["mypy-boto3-fsx>=1.26.0, <1.27.0"],
-        "gamelift": ["mypy-boto3-gamelift>=1.26.0, <1.27.0"],
-        "gamesparks": ["mypy-boto3-gamesparks>=1.26.0, <1.27.0"],
-        "glacier": ["mypy-boto3-glacier>=1.26.0, <1.27.0"],
-        "globalaccelerator": ["mypy-boto3-globalaccelerator>=1.26.0, <1.27.0"],
-        "glue": ["mypy-boto3-glue>=1.26.0, <1.27.0"],
-        "grafana": ["mypy-boto3-grafana>=1.26.0, <1.27.0"],
-        "greengrass": ["mypy-boto3-greengrass>=1.26.0, <1.27.0"],
-        "greengrassv2": ["mypy-boto3-greengrassv2>=1.26.0, <1.27.0"],
-        "groundstation": ["mypy-boto3-groundstation>=1.26.0, <1.27.0"],
-        "guardduty": ["mypy-boto3-guardduty>=1.26.0, <1.27.0"],
-        "health": ["mypy-boto3-health>=1.26.0, <1.27.0"],
-        "healthlake": ["mypy-boto3-healthlake>=1.26.0, <1.27.0"],
-        "honeycode": ["mypy-boto3-honeycode>=1.26.0, <1.27.0"],
-        "iam": ["mypy-boto3-iam>=1.26.0, <1.27.0"],
-        "identitystore": ["mypy-boto3-identitystore>=1.26.0, <1.27.0"],
-        "imagebuilder": ["mypy-boto3-imagebuilder>=1.26.0, <1.27.0"],
-        "importexport": ["mypy-boto3-importexport>=1.26.0, <1.27.0"],
-        "inspector": ["mypy-boto3-inspector>=1.26.0, <1.27.0"],
-        "inspector2": ["mypy-boto3-inspector2>=1.26.0, <1.27.0"],
-        "internetmonitor": ["mypy-boto3-internetmonitor>=1.26.0, <1.27.0"],
-        "iot": ["mypy-boto3-iot>=1.26.0, <1.27.0"],
-        "iot-data": ["mypy-boto3-iot-data>=1.26.0, <1.27.0"],
-        "iot-jobs-data": ["mypy-boto3-iot-jobs-data>=1.26.0, <1.27.0"],
-        "iot-roborunner": ["mypy-boto3-iot-roborunner>=1.26.0, <1.27.0"],
-        "iot1click-devices": ["mypy-boto3-iot1click-devices>=1.26.0, <1.27.0"],
-        "iot1click-projects": ["mypy-boto3-iot1click-projects>=1.26.0, <1.27.0"],
-        "iotanalytics": ["mypy-boto3-iotanalytics>=1.26.0, <1.27.0"],
-        "iotdeviceadvisor": ["mypy-boto3-iotdeviceadvisor>=1.26.0, <1.27.0"],
-        "iotevents": ["mypy-boto3-iotevents>=1.26.0, <1.27.0"],
-        "iotevents-data": ["mypy-boto3-iotevents-data>=1.26.0, <1.27.0"],
-        "iotfleethub": ["mypy-boto3-iotfleethub>=1.26.0, <1.27.0"],
-        "iotfleetwise": ["mypy-boto3-iotfleetwise>=1.26.0, <1.27.0"],
-        "iotsecuretunneling": ["mypy-boto3-iotsecuretunneling>=1.26.0, <1.27.0"],
-        "iotsitewise": ["mypy-boto3-iotsitewise>=1.26.0, <1.27.0"],
-        "iotthingsgraph": ["mypy-boto3-iotthingsgraph>=1.26.0, <1.27.0"],
-        "iottwinmaker": ["mypy-boto3-iottwinmaker>=1.26.0, <1.27.0"],
-        "iotwireless": ["mypy-boto3-iotwireless>=1.26.0, <1.27.0"],
-        "ivs": ["mypy-boto3-ivs>=1.26.0, <1.27.0"],
-        "ivs-realtime": ["mypy-boto3-ivs-realtime>=1.26.0, <1.27.0"],
-        "ivschat": ["mypy-boto3-ivschat>=1.26.0, <1.27.0"],
-        "kafka": ["mypy-boto3-kafka>=1.26.0, <1.27.0"],
-        "kafkaconnect": ["mypy-boto3-kafkaconnect>=1.26.0, <1.27.0"],
-        "kendra": ["mypy-boto3-kendra>=1.26.0, <1.27.0"],
-        "kendra-ranking": ["mypy-boto3-kendra-ranking>=1.26.0, <1.27.0"],
-        "keyspaces": ["mypy-boto3-keyspaces>=1.26.0, <1.27.0"],
-        "kinesis": ["mypy-boto3-kinesis>=1.26.0, <1.27.0"],
+        "boto3": ["boto3==1.27.0", "botocore==1.30.0"],
+        "accessanalyzer": ["mypy-boto3-accessanalyzer>=1.27.0, <1.28.0"],
+        "account": ["mypy-boto3-account>=1.27.0, <1.28.0"],
+        "acm": ["mypy-boto3-acm>=1.27.0, <1.28.0"],
+        "acm-pca": ["mypy-boto3-acm-pca>=1.27.0, <1.28.0"],
+        "alexaforbusiness": ["mypy-boto3-alexaforbusiness>=1.27.0, <1.28.0"],
+        "amp": ["mypy-boto3-amp>=1.27.0, <1.28.0"],
+        "amplify": ["mypy-boto3-amplify>=1.27.0, <1.28.0"],
+        "amplifybackend": ["mypy-boto3-amplifybackend>=1.27.0, <1.28.0"],
+        "amplifyuibuilder": ["mypy-boto3-amplifyuibuilder>=1.27.0, <1.28.0"],
+        "apigateway": ["mypy-boto3-apigateway>=1.27.0, <1.28.0"],
+        "apigatewaymanagementapi": ["mypy-boto3-apigatewaymanagementapi>=1.27.0, <1.28.0"],
+        "apigatewayv2": ["mypy-boto3-apigatewayv2>=1.27.0, <1.28.0"],
+        "appconfig": ["mypy-boto3-appconfig>=1.27.0, <1.28.0"],
+        "appconfigdata": ["mypy-boto3-appconfigdata>=1.27.0, <1.28.0"],
+        "appfabric": ["mypy-boto3-appfabric>=1.27.0, <1.28.0"],
+        "appflow": ["mypy-boto3-appflow>=1.27.0, <1.28.0"],
+        "appintegrations": ["mypy-boto3-appintegrations>=1.27.0, <1.28.0"],
+        "application-autoscaling": ["mypy-boto3-application-autoscaling>=1.27.0, <1.28.0"],
+        "application-insights": ["mypy-boto3-application-insights>=1.27.0, <1.28.0"],
+        "applicationcostprofiler": ["mypy-boto3-applicationcostprofiler>=1.27.0, <1.28.0"],
+        "appmesh": ["mypy-boto3-appmesh>=1.27.0, <1.28.0"],
+        "apprunner": ["mypy-boto3-apprunner>=1.27.0, <1.28.0"],
+        "appstream": ["mypy-boto3-appstream>=1.27.0, <1.28.0"],
+        "appsync": ["mypy-boto3-appsync>=1.27.0, <1.28.0"],
+        "arc-zonal-shift": ["mypy-boto3-arc-zonal-shift>=1.27.0, <1.28.0"],
+        "athena": ["mypy-boto3-athena>=1.27.0, <1.28.0"],
+        "auditmanager": ["mypy-boto3-auditmanager>=1.27.0, <1.28.0"],
+        "autoscaling": ["mypy-boto3-autoscaling>=1.27.0, <1.28.0"],
+        "autoscaling-plans": ["mypy-boto3-autoscaling-plans>=1.27.0, <1.28.0"],
+        "backup": ["mypy-boto3-backup>=1.27.0, <1.28.0"],
+        "backup-gateway": ["mypy-boto3-backup-gateway>=1.27.0, <1.28.0"],
+        "backupstorage": ["mypy-boto3-backupstorage>=1.27.0, <1.28.0"],
+        "batch": ["mypy-boto3-batch>=1.27.0, <1.28.0"],
+        "billingconductor": ["mypy-boto3-billingconductor>=1.27.0, <1.28.0"],
+        "braket": ["mypy-boto3-braket>=1.27.0, <1.28.0"],
+        "budgets": ["mypy-boto3-budgets>=1.27.0, <1.28.0"],
+        "ce": ["mypy-boto3-ce>=1.27.0, <1.28.0"],
+        "chime": ["mypy-boto3-chime>=1.27.0, <1.28.0"],
+        "chime-sdk-identity": ["mypy-boto3-chime-sdk-identity>=1.27.0, <1.28.0"],
+        "chime-sdk-media-pipelines": ["mypy-boto3-chime-sdk-media-pipelines>=1.27.0, <1.28.0"],
+        "chime-sdk-meetings": ["mypy-boto3-chime-sdk-meetings>=1.27.0, <1.28.0"],
+        "chime-sdk-messaging": ["mypy-boto3-chime-sdk-messaging>=1.27.0, <1.28.0"],
+        "chime-sdk-voice": ["mypy-boto3-chime-sdk-voice>=1.27.0, <1.28.0"],
+        "cleanrooms": ["mypy-boto3-cleanrooms>=1.27.0, <1.28.0"],
+        "cloud9": ["mypy-boto3-cloud9>=1.27.0, <1.28.0"],
+        "cloudcontrol": ["mypy-boto3-cloudcontrol>=1.27.0, <1.28.0"],
+        "clouddirectory": ["mypy-boto3-clouddirectory>=1.27.0, <1.28.0"],
+        "cloudformation": ["mypy-boto3-cloudformation>=1.27.0, <1.28.0"],
+        "cloudfront": ["mypy-boto3-cloudfront>=1.27.0, <1.28.0"],
+        "cloudhsm": ["mypy-boto3-cloudhsm>=1.27.0, <1.28.0"],
+        "cloudhsmv2": ["mypy-boto3-cloudhsmv2>=1.27.0, <1.28.0"],
+        "cloudsearch": ["mypy-boto3-cloudsearch>=1.27.0, <1.28.0"],
+        "cloudsearchdomain": ["mypy-boto3-cloudsearchdomain>=1.27.0, <1.28.0"],
+        "cloudtrail": ["mypy-boto3-cloudtrail>=1.27.0, <1.28.0"],
+        "cloudtrail-data": ["mypy-boto3-cloudtrail-data>=1.27.0, <1.28.0"],
+        "cloudwatch": ["mypy-boto3-cloudwatch>=1.27.0, <1.28.0"],
+        "codeartifact": ["mypy-boto3-codeartifact>=1.27.0, <1.28.0"],
+        "codebuild": ["mypy-boto3-codebuild>=1.27.0, <1.28.0"],
+        "codecatalyst": ["mypy-boto3-codecatalyst>=1.27.0, <1.28.0"],
+        "codecommit": ["mypy-boto3-codecommit>=1.27.0, <1.28.0"],
+        "codedeploy": ["mypy-boto3-codedeploy>=1.27.0, <1.28.0"],
+        "codeguru-reviewer": ["mypy-boto3-codeguru-reviewer>=1.27.0, <1.28.0"],
+        "codeguru-security": ["mypy-boto3-codeguru-security>=1.27.0, <1.28.0"],
+        "codeguruprofiler": ["mypy-boto3-codeguruprofiler>=1.27.0, <1.28.0"],
+        "codepipeline": ["mypy-boto3-codepipeline>=1.27.0, <1.28.0"],
+        "codestar": ["mypy-boto3-codestar>=1.27.0, <1.28.0"],
+        "codestar-connections": ["mypy-boto3-codestar-connections>=1.27.0, <1.28.0"],
+        "codestar-notifications": ["mypy-boto3-codestar-notifications>=1.27.0, <1.28.0"],
+        "cognito-identity": ["mypy-boto3-cognito-identity>=1.27.0, <1.28.0"],
+        "cognito-idp": ["mypy-boto3-cognito-idp>=1.27.0, <1.28.0"],
+        "cognito-sync": ["mypy-boto3-cognito-sync>=1.27.0, <1.28.0"],
+        "comprehend": ["mypy-boto3-comprehend>=1.27.0, <1.28.0"],
+        "comprehendmedical": ["mypy-boto3-comprehendmedical>=1.27.0, <1.28.0"],
+        "compute-optimizer": ["mypy-boto3-compute-optimizer>=1.27.0, <1.28.0"],
+        "config": ["mypy-boto3-config>=1.27.0, <1.28.0"],
+        "connect": ["mypy-boto3-connect>=1.27.0, <1.28.0"],
+        "connect-contact-lens": ["mypy-boto3-connect-contact-lens>=1.27.0, <1.28.0"],
+        "connectcampaigns": ["mypy-boto3-connectcampaigns>=1.27.0, <1.28.0"],
+        "connectcases": ["mypy-boto3-connectcases>=1.27.0, <1.28.0"],
+        "connectparticipant": ["mypy-boto3-connectparticipant>=1.27.0, <1.28.0"],
+        "controltower": ["mypy-boto3-controltower>=1.27.0, <1.28.0"],
+        "cur": ["mypy-boto3-cur>=1.27.0, <1.28.0"],
+        "customer-profiles": ["mypy-boto3-customer-profiles>=1.27.0, <1.28.0"],
+        "databrew": ["mypy-boto3-databrew>=1.27.0, <1.28.0"],
+        "dataexchange": ["mypy-boto3-dataexchange>=1.27.0, <1.28.0"],
+        "datapipeline": ["mypy-boto3-datapipeline>=1.27.0, <1.28.0"],
+        "datasync": ["mypy-boto3-datasync>=1.27.0, <1.28.0"],
+        "dax": ["mypy-boto3-dax>=1.27.0, <1.28.0"],
+        "detective": ["mypy-boto3-detective>=1.27.0, <1.28.0"],
+        "devicefarm": ["mypy-boto3-devicefarm>=1.27.0, <1.28.0"],
+        "devops-guru": ["mypy-boto3-devops-guru>=1.27.0, <1.28.0"],
+        "directconnect": ["mypy-boto3-directconnect>=1.27.0, <1.28.0"],
+        "discovery": ["mypy-boto3-discovery>=1.27.0, <1.28.0"],
+        "dlm": ["mypy-boto3-dlm>=1.27.0, <1.28.0"],
+        "dms": ["mypy-boto3-dms>=1.27.0, <1.28.0"],
+        "docdb": ["mypy-boto3-docdb>=1.27.0, <1.28.0"],
+        "docdb-elastic": ["mypy-boto3-docdb-elastic>=1.27.0, <1.28.0"],
+        "drs": ["mypy-boto3-drs>=1.27.0, <1.28.0"],
+        "ds": ["mypy-boto3-ds>=1.27.0, <1.28.0"],
+        "dynamodb": ["mypy-boto3-dynamodb>=1.27.0, <1.28.0"],
+        "dynamodbstreams": ["mypy-boto3-dynamodbstreams>=1.27.0, <1.28.0"],
+        "ebs": ["mypy-boto3-ebs>=1.27.0, <1.28.0"],
+        "ec2": ["mypy-boto3-ec2>=1.27.0, <1.28.0"],
+        "ec2-instance-connect": ["mypy-boto3-ec2-instance-connect>=1.27.0, <1.28.0"],
+        "ecr": ["mypy-boto3-ecr>=1.27.0, <1.28.0"],
+        "ecr-public": ["mypy-boto3-ecr-public>=1.27.0, <1.28.0"],
+        "ecs": ["mypy-boto3-ecs>=1.27.0, <1.28.0"],
+        "efs": ["mypy-boto3-efs>=1.27.0, <1.28.0"],
+        "eks": ["mypy-boto3-eks>=1.27.0, <1.28.0"],
+        "elastic-inference": ["mypy-boto3-elastic-inference>=1.27.0, <1.28.0"],
+        "elasticache": ["mypy-boto3-elasticache>=1.27.0, <1.28.0"],
+        "elasticbeanstalk": ["mypy-boto3-elasticbeanstalk>=1.27.0, <1.28.0"],
+        "elastictranscoder": ["mypy-boto3-elastictranscoder>=1.27.0, <1.28.0"],
+        "elb": ["mypy-boto3-elb>=1.27.0, <1.28.0"],
+        "elbv2": ["mypy-boto3-elbv2>=1.27.0, <1.28.0"],
+        "emr": ["mypy-boto3-emr>=1.27.0, <1.28.0"],
+        "emr-containers": ["mypy-boto3-emr-containers>=1.27.0, <1.28.0"],
+        "emr-serverless": ["mypy-boto3-emr-serverless>=1.27.0, <1.28.0"],
+        "es": ["mypy-boto3-es>=1.27.0, <1.28.0"],
+        "events": ["mypy-boto3-events>=1.27.0, <1.28.0"],
+        "evidently": ["mypy-boto3-evidently>=1.27.0, <1.28.0"],
+        "finspace": ["mypy-boto3-finspace>=1.27.0, <1.28.0"],
+        "finspace-data": ["mypy-boto3-finspace-data>=1.27.0, <1.28.0"],
+        "firehose": ["mypy-boto3-firehose>=1.27.0, <1.28.0"],
+        "fis": ["mypy-boto3-fis>=1.27.0, <1.28.0"],
+        "fms": ["mypy-boto3-fms>=1.27.0, <1.28.0"],
+        "forecast": ["mypy-boto3-forecast>=1.27.0, <1.28.0"],
+        "forecastquery": ["mypy-boto3-forecastquery>=1.27.0, <1.28.0"],
+        "frauddetector": ["mypy-boto3-frauddetector>=1.27.0, <1.28.0"],
+        "fsx": ["mypy-boto3-fsx>=1.27.0, <1.28.0"],
+        "gamelift": ["mypy-boto3-gamelift>=1.27.0, <1.28.0"],
+        "gamesparks": ["mypy-boto3-gamesparks>=1.27.0, <1.28.0"],
+        "glacier": ["mypy-boto3-glacier>=1.27.0, <1.28.0"],
+        "globalaccelerator": ["mypy-boto3-globalaccelerator>=1.27.0, <1.28.0"],
+        "glue": ["mypy-boto3-glue>=1.27.0, <1.28.0"],
+        "grafana": ["mypy-boto3-grafana>=1.27.0, <1.28.0"],
+        "greengrass": ["mypy-boto3-greengrass>=1.27.0, <1.28.0"],
+        "greengrassv2": ["mypy-boto3-greengrassv2>=1.27.0, <1.28.0"],
+        "groundstation": ["mypy-boto3-groundstation>=1.27.0, <1.28.0"],
+        "guardduty": ["mypy-boto3-guardduty>=1.27.0, <1.28.0"],
+        "health": ["mypy-boto3-health>=1.27.0, <1.28.0"],
+        "healthlake": ["mypy-boto3-healthlake>=1.27.0, <1.28.0"],
+        "honeycode": ["mypy-boto3-honeycode>=1.27.0, <1.28.0"],
+        "iam": ["mypy-boto3-iam>=1.27.0, <1.28.0"],
+        "identitystore": ["mypy-boto3-identitystore>=1.27.0, <1.28.0"],
+        "imagebuilder": ["mypy-boto3-imagebuilder>=1.27.0, <1.28.0"],
+        "importexport": ["mypy-boto3-importexport>=1.27.0, <1.28.0"],
+        "inspector": ["mypy-boto3-inspector>=1.27.0, <1.28.0"],
+        "inspector2": ["mypy-boto3-inspector2>=1.27.0, <1.28.0"],
+        "internetmonitor": ["mypy-boto3-internetmonitor>=1.27.0, <1.28.0"],
+        "iot": ["mypy-boto3-iot>=1.27.0, <1.28.0"],
+        "iot-data": ["mypy-boto3-iot-data>=1.27.0, <1.28.0"],
+        "iot-jobs-data": ["mypy-boto3-iot-jobs-data>=1.27.0, <1.28.0"],
+        "iot-roborunner": ["mypy-boto3-iot-roborunner>=1.27.0, <1.28.0"],
+        "iot1click-devices": ["mypy-boto3-iot1click-devices>=1.27.0, <1.28.0"],
+        "iot1click-projects": ["mypy-boto3-iot1click-projects>=1.27.0, <1.28.0"],
+        "iotanalytics": ["mypy-boto3-iotanalytics>=1.27.0, <1.28.0"],
+        "iotdeviceadvisor": ["mypy-boto3-iotdeviceadvisor>=1.27.0, <1.28.0"],
+        "iotevents": ["mypy-boto3-iotevents>=1.27.0, <1.28.0"],
+        "iotevents-data": ["mypy-boto3-iotevents-data>=1.27.0, <1.28.0"],
+        "iotfleethub": ["mypy-boto3-iotfleethub>=1.27.0, <1.28.0"],
+        "iotfleetwise": ["mypy-boto3-iotfleetwise>=1.27.0, <1.28.0"],
+        "iotsecuretunneling": ["mypy-boto3-iotsecuretunneling>=1.27.0, <1.28.0"],
+        "iotsitewise": ["mypy-boto3-iotsitewise>=1.27.0, <1.28.0"],
+        "iotthingsgraph": ["mypy-boto3-iotthingsgraph>=1.27.0, <1.28.0"],
+        "iottwinmaker": ["mypy-boto3-iottwinmaker>=1.27.0, <1.28.0"],
+        "iotwireless": ["mypy-boto3-iotwireless>=1.27.0, <1.28.0"],
+        "ivs": ["mypy-boto3-ivs>=1.27.0, <1.28.0"],
+        "ivs-realtime": ["mypy-boto3-ivs-realtime>=1.27.0, <1.28.0"],
+        "ivschat": ["mypy-boto3-ivschat>=1.27.0, <1.28.0"],
+        "kafka": ["mypy-boto3-kafka>=1.27.0, <1.28.0"],
+        "kafkaconnect": ["mypy-boto3-kafkaconnect>=1.27.0, <1.28.0"],
+        "kendra": ["mypy-boto3-kendra>=1.27.0, <1.28.0"],
+        "kendra-ranking": ["mypy-boto3-kendra-ranking>=1.27.0, <1.28.0"],
+        "keyspaces": ["mypy-boto3-keyspaces>=1.27.0, <1.28.0"],
+        "kinesis": ["mypy-boto3-kinesis>=1.27.0, <1.28.0"],
         "kinesis-video-archived-media": [
-            "mypy-boto3-kinesis-video-archived-media>=1.26.0, <1.27.0"
+            "mypy-boto3-kinesis-video-archived-media>=1.27.0, <1.28.0"
         ],
-        "kinesis-video-media": ["mypy-boto3-kinesis-video-media>=1.26.0, <1.27.0"],
-        "kinesis-video-signaling": ["mypy-boto3-kinesis-video-signaling>=1.26.0, <1.27.0"],
+        "kinesis-video-media": ["mypy-boto3-kinesis-video-media>=1.27.0, <1.28.0"],
+        "kinesis-video-signaling": ["mypy-boto3-kinesis-video-signaling>=1.27.0, <1.28.0"],
         "kinesis-video-webrtc-storage": [
-            "mypy-boto3-kinesis-video-webrtc-storage>=1.26.0, <1.27.0"
+            "mypy-boto3-kinesis-video-webrtc-storage>=1.27.0, <1.28.0"
         ],
-        "kinesisanalytics": ["mypy-boto3-kinesisanalytics>=1.26.0, <1.27.0"],
-        "kinesisanalyticsv2": ["mypy-boto3-kinesisanalyticsv2>=1.26.0, <1.27.0"],
-        "kinesisvideo": ["mypy-boto3-kinesisvideo>=1.26.0, <1.27.0"],
-        "kms": ["mypy-boto3-kms>=1.26.0, <1.27.0"],
-        "lakeformation": ["mypy-boto3-lakeformation>=1.26.0, <1.27.0"],
-        "lambda": ["mypy-boto3-lambda>=1.26.0, <1.27.0"],
-        "lex-models": ["mypy-boto3-lex-models>=1.26.0, <1.27.0"],
-        "lex-runtime": ["mypy-boto3-lex-runtime>=1.26.0, <1.27.0"],
-        "lexv2-models": ["mypy-boto3-lexv2-models>=1.26.0, <1.27.0"],
-        "lexv2-runtime": ["mypy-boto3-lexv2-runtime>=1.26.0, <1.27.0"],
-        "license-manager": ["mypy-boto3-license-manager>=1.26.0, <1.27.0"],
+        "kinesisanalytics": ["mypy-boto3-kinesisanalytics>=1.27.0, <1.28.0"],
+        "kinesisanalyticsv2": ["mypy-boto3-kinesisanalyticsv2>=1.27.0, <1.28.0"],
+        "kinesisvideo": ["mypy-boto3-kinesisvideo>=1.27.0, <1.28.0"],
+        "kms": ["mypy-boto3-kms>=1.27.0, <1.28.0"],
+        "lakeformation": ["mypy-boto3-lakeformation>=1.27.0, <1.28.0"],
+        "lambda": ["mypy-boto3-lambda>=1.27.0, <1.28.0"],
+        "lex-models": ["mypy-boto3-lex-models>=1.27.0, <1.28.0"],
+        "lex-runtime": ["mypy-boto3-lex-runtime>=1.27.0, <1.28.0"],
+        "lexv2-models": ["mypy-boto3-lexv2-models>=1.27.0, <1.28.0"],
+        "lexv2-runtime": ["mypy-boto3-lexv2-runtime>=1.27.0, <1.28.0"],
+        "license-manager": ["mypy-boto3-license-manager>=1.27.0, <1.28.0"],
         "license-manager-linux-subscriptions": [
-            "mypy-boto3-license-manager-linux-subscriptions>=1.26.0, <1.27.0"
+            "mypy-boto3-license-manager-linux-subscriptions>=1.27.0, <1.28.0"
         ],
         "license-manager-user-subscriptions": [
-            "mypy-boto3-license-manager-user-subscriptions>=1.26.0, <1.27.0"
+            "mypy-boto3-license-manager-user-subscriptions>=1.27.0, <1.28.0"
         ],
-        "lightsail": ["mypy-boto3-lightsail>=1.26.0, <1.27.0"],
-        "location": ["mypy-boto3-location>=1.26.0, <1.27.0"],
-        "logs": ["mypy-boto3-logs>=1.26.0, <1.27.0"],
-        "lookoutequipment": ["mypy-boto3-lookoutequipment>=1.26.0, <1.27.0"],
-        "lookoutmetrics": ["mypy-boto3-lookoutmetrics>=1.26.0, <1.27.0"],
-        "lookoutvision": ["mypy-boto3-lookoutvision>=1.26.0, <1.27.0"],
-        "m2": ["mypy-boto3-m2>=1.26.0, <1.27.0"],
-        "machinelearning": ["mypy-boto3-machinelearning>=1.26.0, <1.27.0"],
-        "macie": ["mypy-boto3-macie>=1.26.0, <1.27.0"],
-        "macie2": ["mypy-boto3-macie2>=1.26.0, <1.27.0"],
-        "managedblockchain": ["mypy-boto3-managedblockchain>=1.26.0, <1.27.0"],
-        "marketplace-catalog": ["mypy-boto3-marketplace-catalog>=1.26.0, <1.27.0"],
-        "marketplace-entitlement": ["mypy-boto3-marketplace-entitlement>=1.26.0, <1.27.0"],
+        "lightsail": ["mypy-boto3-lightsail>=1.27.0, <1.28.0"],
+        "location": ["mypy-boto3-location>=1.27.0, <1.28.0"],
+        "logs": ["mypy-boto3-logs>=1.27.0, <1.28.0"],
+        "lookoutequipment": ["mypy-boto3-lookoutequipment>=1.27.0, <1.28.0"],
+        "lookoutmetrics": ["mypy-boto3-lookoutmetrics>=1.27.0, <1.28.0"],
+        "lookoutvision": ["mypy-boto3-lookoutvision>=1.27.0, <1.28.0"],
+        "m2": ["mypy-boto3-m2>=1.27.0, <1.28.0"],
+        "machinelearning": ["mypy-boto3-machinelearning>=1.27.0, <1.28.0"],
+        "macie": ["mypy-boto3-macie>=1.27.0, <1.28.0"],
+        "macie2": ["mypy-boto3-macie2>=1.27.0, <1.28.0"],
+        "managedblockchain": ["mypy-boto3-managedblockchain>=1.27.0, <1.28.0"],
+        "marketplace-catalog": ["mypy-boto3-marketplace-catalog>=1.27.0, <1.28.0"],
+        "marketplace-entitlement": ["mypy-boto3-marketplace-entitlement>=1.27.0, <1.28.0"],
         "marketplacecommerceanalytics": [
-            "mypy-boto3-marketplacecommerceanalytics>=1.26.0, <1.27.0"
+            "mypy-boto3-marketplacecommerceanalytics>=1.27.0, <1.28.0"
         ],
-        "mediaconnect": ["mypy-boto3-mediaconnect>=1.26.0, <1.27.0"],
-        "mediaconvert": ["mypy-boto3-mediaconvert>=1.26.0, <1.27.0"],
-        "medialive": ["mypy-boto3-medialive>=1.26.0, <1.27.0"],
-        "mediapackage": ["mypy-boto3-mediapackage>=1.26.0, <1.27.0"],
-        "mediapackage-vod": ["mypy-boto3-mediapackage-vod>=1.26.0, <1.27.0"],
-        "mediastore": ["mypy-boto3-mediastore>=1.26.0, <1.27.0"],
-        "mediastore-data": ["mypy-boto3-mediastore-data>=1.26.0, <1.27.0"],
-        "mediatailor": ["mypy-boto3-mediatailor>=1.26.0, <1.27.0"],
-        "memorydb": ["mypy-boto3-memorydb>=1.26.0, <1.27.0"],
-        "meteringmarketplace": ["mypy-boto3-meteringmarketplace>=1.26.0, <1.27.0"],
-        "mgh": ["mypy-boto3-mgh>=1.26.0, <1.27.0"],
-        "mgn": ["mypy-boto3-mgn>=1.26.0, <1.27.0"],
+        "mediaconnect": ["mypy-boto3-mediaconnect>=1.27.0, <1.28.0"],
+        "mediaconvert": ["mypy-boto3-mediaconvert>=1.27.0, <1.28.0"],
+        "medialive": ["mypy-boto3-medialive>=1.27.0, <1.28.0"],
+        "mediapackage": ["mypy-boto3-mediapackage>=1.27.0, <1.28.0"],
+        "mediapackage-vod": ["mypy-boto3-mediapackage-vod>=1.27.0, <1.28.0"],
+        "mediapackagev2": ["mypy-boto3-mediapackagev2>=1.27.0, <1.28.0"],
+        "mediastore": ["mypy-boto3-mediastore>=1.27.0, <1.28.0"],
+        "mediastore-data": ["mypy-boto3-mediastore-data>=1.27.0, <1.28.0"],
+        "mediatailor": ["mypy-boto3-mediatailor>=1.27.0, <1.28.0"],
+        "memorydb": ["mypy-boto3-memorydb>=1.27.0, <1.28.0"],
+        "meteringmarketplace": ["mypy-boto3-meteringmarketplace>=1.27.0, <1.28.0"],
+        "mgh": ["mypy-boto3-mgh>=1.27.0, <1.28.0"],
+        "mgn": ["mypy-boto3-mgn>=1.27.0, <1.28.0"],
         "migration-hub-refactor-spaces": [
-            "mypy-boto3-migration-hub-refactor-spaces>=1.26.0, <1.27.0"
+            "mypy-boto3-migration-hub-refactor-spaces>=1.27.0, <1.28.0"
         ],
-        "migrationhub-config": ["mypy-boto3-migrationhub-config>=1.26.0, <1.27.0"],
-        "migrationhuborchestrator": ["mypy-boto3-migrationhuborchestrator>=1.26.0, <1.27.0"],
-        "migrationhubstrategy": ["mypy-boto3-migrationhubstrategy>=1.26.0, <1.27.0"],
-        "mobile": ["mypy-boto3-mobile>=1.26.0, <1.27.0"],
-        "mq": ["mypy-boto3-mq>=1.26.0, <1.27.0"],
-        "mturk": ["mypy-boto3-mturk>=1.26.0, <1.27.0"],
-        "mwaa": ["mypy-boto3-mwaa>=1.26.0, <1.27.0"],
-        "neptune": ["mypy-boto3-neptune>=1.26.0, <1.27.0"],
-        "network-firewall": ["mypy-boto3-network-firewall>=1.26.0, <1.27.0"],
-        "networkmanager": ["mypy-boto3-networkmanager>=1.26.0, <1.27.0"],
-        "nimble": ["mypy-boto3-nimble>=1.26.0, <1.27.0"],
-        "oam": ["mypy-boto3-oam>=1.26.0, <1.27.0"],
-        "omics": ["mypy-boto3-omics>=1.26.0, <1.27.0"],
-        "opensearch": ["mypy-boto3-opensearch>=1.26.0, <1.27.0"],
-        "opensearchserverless": ["mypy-boto3-opensearchserverless>=1.26.0, <1.27.0"],
-        "opsworks": ["mypy-boto3-opsworks>=1.26.0, <1.27.0"],
-        "opsworkscm": ["mypy-boto3-opsworkscm>=1.26.0, <1.27.0"],
-        "organizations": ["mypy-boto3-organizations>=1.26.0, <1.27.0"],
-        "outposts": ["mypy-boto3-outposts>=1.26.0, <1.27.0"],
-        "panorama": ["mypy-boto3-panorama>=1.26.0, <1.27.0"],
-        "personalize": ["mypy-boto3-personalize>=1.26.0, <1.27.0"],
-        "personalize-events": ["mypy-boto3-personalize-events>=1.26.0, <1.27.0"],
-        "personalize-runtime": ["mypy-boto3-personalize-runtime>=1.26.0, <1.27.0"],
-        "pi": ["mypy-boto3-pi>=1.26.0, <1.27.0"],
-        "pinpoint": ["mypy-boto3-pinpoint>=1.26.0, <1.27.0"],
-        "pinpoint-email": ["mypy-boto3-pinpoint-email>=1.26.0, <1.27.0"],
-        "pinpoint-sms-voice": ["mypy-boto3-pinpoint-sms-voice>=1.26.0, <1.27.0"],
-        "pinpoint-sms-voice-v2": ["mypy-boto3-pinpoint-sms-voice-v2>=1.26.0, <1.27.0"],
-        "pipes": ["mypy-boto3-pipes>=1.26.0, <1.27.0"],
-        "polly": ["mypy-boto3-polly>=1.26.0, <1.27.0"],
-        "pricing": ["mypy-boto3-pricing>=1.26.0, <1.27.0"],
-        "privatenetworks": ["mypy-boto3-privatenetworks>=1.26.0, <1.27.0"],
-        "proton": ["mypy-boto3-proton>=1.26.0, <1.27.0"],
-        "qldb": ["mypy-boto3-qldb>=1.26.0, <1.27.0"],
-        "qldb-session": ["mypy-boto3-qldb-session>=1.26.0, <1.27.0"],
-        "quicksight": ["mypy-boto3-quicksight>=1.26.0, <1.27.0"],
-        "ram": ["mypy-boto3-ram>=1.26.0, <1.27.0"],
-        "rbin": ["mypy-boto3-rbin>=1.26.0, <1.27.0"],
-        "rds": ["mypy-boto3-rds>=1.26.0, <1.27.0"],
-        "rds-data": ["mypy-boto3-rds-data>=1.26.0, <1.27.0"],
-        "redshift": ["mypy-boto3-redshift>=1.26.0, <1.27.0"],
-        "redshift-data": ["mypy-boto3-redshift-data>=1.26.0, <1.27.0"],
-        "redshift-serverless": ["mypy-boto3-redshift-serverless>=1.26.0, <1.27.0"],
-        "rekognition": ["mypy-boto3-rekognition>=1.26.0, <1.27.0"],
-        "resiliencehub": ["mypy-boto3-resiliencehub>=1.26.0, <1.27.0"],
-        "resource-explorer-2": ["mypy-boto3-resource-explorer-2>=1.26.0, <1.27.0"],
-        "resource-groups": ["mypy-boto3-resource-groups>=1.26.0, <1.27.0"],
-        "resourcegroupstaggingapi": ["mypy-boto3-resourcegroupstaggingapi>=1.26.0, <1.27.0"],
-        "robomaker": ["mypy-boto3-robomaker>=1.26.0, <1.27.0"],
-        "rolesanywhere": ["mypy-boto3-rolesanywhere>=1.26.0, <1.27.0"],
-        "route53": ["mypy-boto3-route53>=1.26.0, <1.27.0"],
-        "route53-recovery-cluster": ["mypy-boto3-route53-recovery-cluster>=1.26.0, <1.27.0"],
+        "migrationhub-config": ["mypy-boto3-migrationhub-config>=1.27.0, <1.28.0"],
+        "migrationhuborchestrator": ["mypy-boto3-migrationhuborchestrator>=1.27.0, <1.28.0"],
+        "migrationhubstrategy": ["mypy-boto3-migrationhubstrategy>=1.27.0, <1.28.0"],
+        "mobile": ["mypy-boto3-mobile>=1.27.0, <1.28.0"],
+        "mq": ["mypy-boto3-mq>=1.27.0, <1.28.0"],
+        "mturk": ["mypy-boto3-mturk>=1.27.0, <1.28.0"],
+        "mwaa": ["mypy-boto3-mwaa>=1.27.0, <1.28.0"],
+        "neptune": ["mypy-boto3-neptune>=1.27.0, <1.28.0"],
+        "network-firewall": ["mypy-boto3-network-firewall>=1.27.0, <1.28.0"],
+        "networkmanager": ["mypy-boto3-networkmanager>=1.27.0, <1.28.0"],
+        "nimble": ["mypy-boto3-nimble>=1.27.0, <1.28.0"],
+        "oam": ["mypy-boto3-oam>=1.27.0, <1.28.0"],
+        "omics": ["mypy-boto3-omics>=1.27.0, <1.28.0"],
+        "opensearch": ["mypy-boto3-opensearch>=1.27.0, <1.28.0"],
+        "opensearchserverless": ["mypy-boto3-opensearchserverless>=1.27.0, <1.28.0"],
+        "opsworks": ["mypy-boto3-opsworks>=1.27.0, <1.28.0"],
+        "opsworkscm": ["mypy-boto3-opsworkscm>=1.27.0, <1.28.0"],
+        "organizations": ["mypy-boto3-organizations>=1.27.0, <1.28.0"],
+        "osis": ["mypy-boto3-osis>=1.27.0, <1.28.0"],
+        "outposts": ["mypy-boto3-outposts>=1.27.0, <1.28.0"],
+        "panorama": ["mypy-boto3-panorama>=1.27.0, <1.28.0"],
+        "payment-cryptography": ["mypy-boto3-payment-cryptography>=1.27.0, <1.28.0"],
+        "payment-cryptography-data": ["mypy-boto3-payment-cryptography-data>=1.27.0, <1.28.0"],
+        "personalize": ["mypy-boto3-personalize>=1.27.0, <1.28.0"],
+        "personalize-events": ["mypy-boto3-personalize-events>=1.27.0, <1.28.0"],
+        "personalize-runtime": ["mypy-boto3-personalize-runtime>=1.27.0, <1.28.0"],
+        "pi": ["mypy-boto3-pi>=1.27.0, <1.28.0"],
+        "pinpoint": ["mypy-boto3-pinpoint>=1.27.0, <1.28.0"],
+        "pinpoint-email": ["mypy-boto3-pinpoint-email>=1.27.0, <1.28.0"],
+        "pinpoint-sms-voice": ["mypy-boto3-pinpoint-sms-voice>=1.27.0, <1.28.0"],
+        "pinpoint-sms-voice-v2": ["mypy-boto3-pinpoint-sms-voice-v2>=1.27.0, <1.28.0"],
+        "pipes": ["mypy-boto3-pipes>=1.27.0, <1.28.0"],
+        "polly": ["mypy-boto3-polly>=1.27.0, <1.28.0"],
+        "pricing": ["mypy-boto3-pricing>=1.27.0, <1.28.0"],
+        "privatenetworks": ["mypy-boto3-privatenetworks>=1.27.0, <1.28.0"],
+        "proton": ["mypy-boto3-proton>=1.27.0, <1.28.0"],
+        "qldb": ["mypy-boto3-qldb>=1.27.0, <1.28.0"],
+        "qldb-session": ["mypy-boto3-qldb-session>=1.27.0, <1.28.0"],
+        "quicksight": ["mypy-boto3-quicksight>=1.27.0, <1.28.0"],
+        "ram": ["mypy-boto3-ram>=1.27.0, <1.28.0"],
+        "rbin": ["mypy-boto3-rbin>=1.27.0, <1.28.0"],
+        "rds": ["mypy-boto3-rds>=1.27.0, <1.28.0"],
+        "rds-data": ["mypy-boto3-rds-data>=1.27.0, <1.28.0"],
+        "redshift": ["mypy-boto3-redshift>=1.27.0, <1.28.0"],
+        "redshift-data": ["mypy-boto3-redshift-data>=1.27.0, <1.28.0"],
+        "redshift-serverless": ["mypy-boto3-redshift-serverless>=1.27.0, <1.28.0"],
+        "rekognition": ["mypy-boto3-rekognition>=1.27.0, <1.28.0"],
+        "resiliencehub": ["mypy-boto3-resiliencehub>=1.27.0, <1.28.0"],
+        "resource-explorer-2": ["mypy-boto3-resource-explorer-2>=1.27.0, <1.28.0"],
+        "resource-groups": ["mypy-boto3-resource-groups>=1.27.0, <1.28.0"],
+        "resourcegroupstaggingapi": ["mypy-boto3-resourcegroupstaggingapi>=1.27.0, <1.28.0"],
+        "robomaker": ["mypy-boto3-robomaker>=1.27.0, <1.28.0"],
+        "rolesanywhere": ["mypy-boto3-rolesanywhere>=1.27.0, <1.28.0"],
+        "route53": ["mypy-boto3-route53>=1.27.0, <1.28.0"],
+        "route53-recovery-cluster": ["mypy-boto3-route53-recovery-cluster>=1.27.0, <1.28.0"],
         "route53-recovery-control-config": [
-            "mypy-boto3-route53-recovery-control-config>=1.26.0, <1.27.0"
+            "mypy-boto3-route53-recovery-control-config>=1.27.0, <1.28.0"
         ],
-        "route53-recovery-readiness": ["mypy-boto3-route53-recovery-readiness>=1.26.0, <1.27.0"],
-        "route53domains": ["mypy-boto3-route53domains>=1.26.0, <1.27.0"],
-        "route53resolver": ["mypy-boto3-route53resolver>=1.26.0, <1.27.0"],
-        "rum": ["mypy-boto3-rum>=1.26.0, <1.27.0"],
-        "s3": ["mypy-boto3-s3>=1.26.0, <1.27.0"],
-        "s3control": ["mypy-boto3-s3control>=1.26.0, <1.27.0"],
-        "s3outposts": ["mypy-boto3-s3outposts>=1.26.0, <1.27.0"],
-        "sagemaker": ["mypy-boto3-sagemaker>=1.26.0, <1.27.0"],
-        "sagemaker-a2i-runtime": ["mypy-boto3-sagemaker-a2i-runtime>=1.26.0, <1.27.0"],
-        "sagemaker-edge": ["mypy-boto3-sagemaker-edge>=1.26.0, <1.27.0"],
+        "route53-recovery-readiness": ["mypy-boto3-route53-recovery-readiness>=1.27.0, <1.28.0"],
+        "route53domains": ["mypy-boto3-route53domains>=1.27.0, <1.28.0"],
+        "route53resolver": ["mypy-boto3-route53resolver>=1.27.0, <1.28.0"],
+        "rum": ["mypy-boto3-rum>=1.27.0, <1.28.0"],
+        "s3": ["mypy-boto3-s3>=1.27.0, <1.28.0"],
+        "s3control": ["mypy-boto3-s3control>=1.27.0, <1.28.0"],
+        "s3outposts": ["mypy-boto3-s3outposts>=1.27.0, <1.28.0"],
+        "sagemaker": ["mypy-boto3-sagemaker>=1.27.0, <1.28.0"],
+        "sagemaker-a2i-runtime": ["mypy-boto3-sagemaker-a2i-runtime>=1.27.0, <1.28.0"],
+        "sagemaker-edge": ["mypy-boto3-sagemaker-edge>=1.27.0, <1.28.0"],
         "sagemaker-featurestore-runtime": [
-            "mypy-boto3-sagemaker-featurestore-runtime>=1.26.0, <1.27.0"
+            "mypy-boto3-sagemaker-featurestore-runtime>=1.27.0, <1.28.0"
         ],
-        "sagemaker-geospatial": ["mypy-boto3-sagemaker-geospatial>=1.26.0, <1.27.0"],
-        "sagemaker-metrics": ["mypy-boto3-sagemaker-metrics>=1.26.0, <1.27.0"],
-        "sagemaker-runtime": ["mypy-boto3-sagemaker-runtime>=1.26.0, <1.27.0"],
-        "savingsplans": ["mypy-boto3-savingsplans>=1.26.0, <1.27.0"],
-        "scheduler": ["mypy-boto3-scheduler>=1.26.0, <1.27.0"],
-        "schemas": ["mypy-boto3-schemas>=1.26.0, <1.27.0"],
-        "sdb": ["mypy-boto3-sdb>=1.26.0, <1.27.0"],
-        "secretsmanager": ["mypy-boto3-secretsmanager>=1.26.0, <1.27.0"],
-        "securityhub": ["mypy-boto3-securityhub>=1.26.0, <1.27.0"],
-        "securitylake": ["mypy-boto3-securitylake>=1.26.0, <1.27.0"],
-        "serverlessrepo": ["mypy-boto3-serverlessrepo>=1.26.0, <1.27.0"],
-        "service-quotas": ["mypy-boto3-service-quotas>=1.26.0, <1.27.0"],
-        "servicecatalog": ["mypy-boto3-servicecatalog>=1.26.0, <1.27.0"],
-        "servicecatalog-appregistry": ["mypy-boto3-servicecatalog-appregistry>=1.26.0, <1.27.0"],
-        "servicediscovery": ["mypy-boto3-servicediscovery>=1.26.0, <1.27.0"],
-        "ses": ["mypy-boto3-ses>=1.26.0, <1.27.0"],
-        "sesv2": ["mypy-boto3-sesv2>=1.26.0, <1.27.0"],
-        "shield": ["mypy-boto3-shield>=1.26.0, <1.27.0"],
-        "signer": ["mypy-boto3-signer>=1.26.0, <1.27.0"],
-        "simspaceweaver": ["mypy-boto3-simspaceweaver>=1.26.0, <1.27.0"],
-        "sms": ["mypy-boto3-sms>=1.26.0, <1.27.0"],
-        "sms-voice": ["mypy-boto3-sms-voice>=1.26.0, <1.27.0"],
-        "snow-device-management": ["mypy-boto3-snow-device-management>=1.26.0, <1.27.0"],
-        "snowball": ["mypy-boto3-snowball>=1.26.0, <1.27.0"],
-        "sns": ["mypy-boto3-sns>=1.26.0, <1.27.0"],
-        "sqs": ["mypy-boto3-sqs>=1.26.0, <1.27.0"],
-        "ssm": ["mypy-boto3-ssm>=1.26.0, <1.27.0"],
-        "ssm-contacts": ["mypy-boto3-ssm-contacts>=1.26.0, <1.27.0"],
-        "ssm-incidents": ["mypy-boto3-ssm-incidents>=1.26.0, <1.27.0"],
-        "ssm-sap": ["mypy-boto3-ssm-sap>=1.26.0, <1.27.0"],
-        "sso": ["mypy-boto3-sso>=1.26.0, <1.27.0"],
-        "sso-admin": ["mypy-boto3-sso-admin>=1.26.0, <1.27.0"],
-        "sso-oidc": ["mypy-boto3-sso-oidc>=1.26.0, <1.27.0"],
-        "stepfunctions": ["mypy-boto3-stepfunctions>=1.26.0, <1.27.0"],
-        "storagegateway": ["mypy-boto3-storagegateway>=1.26.0, <1.27.0"],
-        "sts": ["mypy-boto3-sts>=1.26.0, <1.27.0"],
-        "support": ["mypy-boto3-support>=1.26.0, <1.27.0"],
-        "support-app": ["mypy-boto3-support-app>=1.26.0, <1.27.0"],
-        "swf": ["mypy-boto3-swf>=1.26.0, <1.27.0"],
-        "synthetics": ["mypy-boto3-synthetics>=1.26.0, <1.27.0"],
-        "textract": ["mypy-boto3-textract>=1.26.0, <1.27.0"],
-        "timestream-query": ["mypy-boto3-timestream-query>=1.26.0, <1.27.0"],
-        "timestream-write": ["mypy-boto3-timestream-write>=1.26.0, <1.27.0"],
-        "tnb": ["mypy-boto3-tnb>=1.26.0, <1.27.0"],
-        "transcribe": ["mypy-boto3-transcribe>=1.26.0, <1.27.0"],
-        "transfer": ["mypy-boto3-transfer>=1.26.0, <1.27.0"],
-        "translate": ["mypy-boto3-translate>=1.26.0, <1.27.0"],
-        "voice-id": ["mypy-boto3-voice-id>=1.26.0, <1.27.0"],
-        "waf": ["mypy-boto3-waf>=1.26.0, <1.27.0"],
-        "waf-regional": ["mypy-boto3-waf-regional>=1.26.0, <1.27.0"],
-        "wafv2": ["mypy-boto3-wafv2>=1.26.0, <1.27.0"],
-        "wellarchitected": ["mypy-boto3-wellarchitected>=1.26.0, <1.27.0"],
-        "wisdom": ["mypy-boto3-wisdom>=1.26.0, <1.27.0"],
-        "workdocs": ["mypy-boto3-workdocs>=1.26.0, <1.27.0"],
-        "worklink": ["mypy-boto3-worklink>=1.26.0, <1.27.0"],
-        "workmail": ["mypy-boto3-workmail>=1.26.0, <1.27.0"],
-        "workmailmessageflow": ["mypy-boto3-workmailmessageflow>=1.26.0, <1.27.0"],
-        "workspaces": ["mypy-boto3-workspaces>=1.26.0, <1.27.0"],
-        "workspaces-web": ["mypy-boto3-workspaces-web>=1.26.0, <1.27.0"],
-        "xray": ["mypy-boto3-xray>=1.26.0, <1.27.0"],
+        "sagemaker-geospatial": ["mypy-boto3-sagemaker-geospatial>=1.27.0, <1.28.0"],
+        "sagemaker-metrics": ["mypy-boto3-sagemaker-metrics>=1.27.0, <1.28.0"],
+        "sagemaker-runtime": ["mypy-boto3-sagemaker-runtime>=1.27.0, <1.28.0"],
+        "savingsplans": ["mypy-boto3-savingsplans>=1.27.0, <1.28.0"],
+        "scheduler": ["mypy-boto3-scheduler>=1.27.0, <1.28.0"],
+        "schemas": ["mypy-boto3-schemas>=1.27.0, <1.28.0"],
+        "sdb": ["mypy-boto3-sdb>=1.27.0, <1.28.0"],
+        "secretsmanager": ["mypy-boto3-secretsmanager>=1.27.0, <1.28.0"],
+        "securityhub": ["mypy-boto3-securityhub>=1.27.0, <1.28.0"],
+        "securitylake": ["mypy-boto3-securitylake>=1.27.0, <1.28.0"],
+        "serverlessrepo": ["mypy-boto3-serverlessrepo>=1.27.0, <1.28.0"],
+        "service-quotas": ["mypy-boto3-service-quotas>=1.27.0, <1.28.0"],
+        "servicecatalog": ["mypy-boto3-servicecatalog>=1.27.0, <1.28.0"],
+        "servicecatalog-appregistry": ["mypy-boto3-servicecatalog-appregistry>=1.27.0, <1.28.0"],
+        "servicediscovery": ["mypy-boto3-servicediscovery>=1.27.0, <1.28.0"],
+        "ses": ["mypy-boto3-ses>=1.27.0, <1.28.0"],
+        "sesv2": ["mypy-boto3-sesv2>=1.27.0, <1.28.0"],
+        "shield": ["mypy-boto3-shield>=1.27.0, <1.28.0"],
+        "signer": ["mypy-boto3-signer>=1.27.0, <1.28.0"],
+        "simspaceweaver": ["mypy-boto3-simspaceweaver>=1.27.0, <1.28.0"],
+        "sms": ["mypy-boto3-sms>=1.27.0, <1.28.0"],
+        "sms-voice": ["mypy-boto3-sms-voice>=1.27.0, <1.28.0"],
+        "snow-device-management": ["mypy-boto3-snow-device-management>=1.27.0, <1.28.0"],
+        "snowball": ["mypy-boto3-snowball>=1.27.0, <1.28.0"],
+        "sns": ["mypy-boto3-sns>=1.27.0, <1.28.0"],
+        "sqs": ["mypy-boto3-sqs>=1.27.0, <1.28.0"],
+        "ssm": ["mypy-boto3-ssm>=1.27.0, <1.28.0"],
+        "ssm-contacts": ["mypy-boto3-ssm-contacts>=1.27.0, <1.28.0"],
+        "ssm-incidents": ["mypy-boto3-ssm-incidents>=1.27.0, <1.28.0"],
+        "ssm-sap": ["mypy-boto3-ssm-sap>=1.27.0, <1.28.0"],
+        "sso": ["mypy-boto3-sso>=1.27.0, <1.28.0"],
+        "sso-admin": ["mypy-boto3-sso-admin>=1.27.0, <1.28.0"],
+        "sso-oidc": ["mypy-boto3-sso-oidc>=1.27.0, <1.28.0"],
+        "stepfunctions": ["mypy-boto3-stepfunctions>=1.27.0, <1.28.0"],
+        "storagegateway": ["mypy-boto3-storagegateway>=1.27.0, <1.28.0"],
+        "sts": ["mypy-boto3-sts>=1.27.0, <1.28.0"],
+        "support": ["mypy-boto3-support>=1.27.0, <1.28.0"],
+        "support-app": ["mypy-boto3-support-app>=1.27.0, <1.28.0"],
+        "swf": ["mypy-boto3-swf>=1.27.0, <1.28.0"],
+        "synthetics": ["mypy-boto3-synthetics>=1.27.0, <1.28.0"],
+        "textract": ["mypy-boto3-textract>=1.27.0, <1.28.0"],
+        "timestream-query": ["mypy-boto3-timestream-query>=1.27.0, <1.28.0"],
+        "timestream-write": ["mypy-boto3-timestream-write>=1.27.0, <1.28.0"],
+        "tnb": ["mypy-boto3-tnb>=1.27.0, <1.28.0"],
+        "transcribe": ["mypy-boto3-transcribe>=1.27.0, <1.28.0"],
+        "transfer": ["mypy-boto3-transfer>=1.27.0, <1.28.0"],
+        "translate": ["mypy-boto3-translate>=1.27.0, <1.28.0"],
+        "verifiedpermissions": ["mypy-boto3-verifiedpermissions>=1.27.0, <1.28.0"],
+        "voice-id": ["mypy-boto3-voice-id>=1.27.0, <1.28.0"],
+        "vpc-lattice": ["mypy-boto3-vpc-lattice>=1.27.0, <1.28.0"],
+        "waf": ["mypy-boto3-waf>=1.27.0, <1.28.0"],
+        "waf-regional": ["mypy-boto3-waf-regional>=1.27.0, <1.28.0"],
+        "wafv2": ["mypy-boto3-wafv2>=1.27.0, <1.28.0"],
+        "wellarchitected": ["mypy-boto3-wellarchitected>=1.27.0, <1.28.0"],
+        "wisdom": ["mypy-boto3-wisdom>=1.27.0, <1.28.0"],
+        "workdocs": ["mypy-boto3-workdocs>=1.27.0, <1.28.0"],
+        "worklink": ["mypy-boto3-worklink>=1.27.0, <1.28.0"],
+        "workmail": ["mypy-boto3-workmail>=1.27.0, <1.28.0"],
+        "workmailmessageflow": ["mypy-boto3-workmailmessageflow>=1.27.0, <1.28.0"],
+        "workspaces": ["mypy-boto3-workspaces>=1.27.0, <1.28.0"],
+        "workspaces-web": ["mypy-boto3-workspaces-web>=1.27.0, <1.28.0"],
+        "xray": ["mypy-boto3-xray>=1.27.0, <1.28.0"],
     },
     zip_safe=False,
 )
```

