# Comparing `tmp/cdk-cloudformation-github-teams-team-1.2.0a7.tar.gz` & `tmp/cdk-cloudformation-github-teams-team-1.4.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/github-teams-team/dist/python/cdk-cloudformation-github", last modified: Mon Mar 27 06:13:53 2023, max compression
+gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/github-teams-team/dist/python/cdk-cloudformation-github", last modified: Mon Jul  3 06:16:02 2023, max compression
```

## Comparing `cdk-cloudformation-github-teams-team-1.2.0a7.tar` & `cdk-cloudformation-github-teams-team-1.4.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:13:53.000000 cdk-cloudformation-github-teams-team-1.2.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-03-27 06:13:47.000000 cdk-cloudformation-github-teams-team-1.2.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-03-27 06:13:47.000000 cdk-cloudformation-github-teams-team-1.2.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2915 2023-03-27 06:13:53.000000 cdk-cloudformation-github-teams-team-1.2.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2007 2023-03-27 06:13:47.000000 cdk-cloudformation-github-teams-team-1.2.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-03-27 06:13:47.000000 cdk-cloudformation-github-teams-team-1.2.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-03-27 06:13:53.000000 cdk-cloudformation-github-teams-team-1.2.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1854 2023-03-27 06:13:47.000000 cdk-cloudformation-github-teams-team-1.2.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:13:53.000000 cdk-cloudformation-github-teams-team-1.2.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:13:53.000000 cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     9243 2023-03-27 06:13:47.000000 cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:13:53.000000 cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      450 2023-03-27 06:13:47.000000 cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    17894 2023-03-27 06:13:47.000000 cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team/_jsii/github-teams-team@1.2.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-03-27 06:13:47.000000 cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-03-27 06:13:53.000000 cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2915 2023-03-27 06:13:53.000000 cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      622 2023-03-27 06:13:53.000000 cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-03-27 06:13:53.000000 cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-03-27 06:13:53.000000 cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       37 2023-03-27 06:13:53.000000 cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-07-03 06:16:02.000000 cdk-cloudformation-github-teams-team-1.4.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-07-03 06:15:56.000000 cdk-cloudformation-github-teams-team-1.4.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-07-03 06:15:56.000000 cdk-cloudformation-github-teams-team-1.4.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2915 2023-07-03 06:16:02.000000 cdk-cloudformation-github-teams-team-1.4.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2007 2023-07-03 06:15:56.000000 cdk-cloudformation-github-teams-team-1.4.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-07-03 06:15:56.000000 cdk-cloudformation-github-teams-team-1.4.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-07-03 06:16:02.000000 cdk-cloudformation-github-teams-team-1.4.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1853 2023-07-03 06:15:56.000000 cdk-cloudformation-github-teams-team-1.4.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-07-03 06:16:02.000000 cdk-cloudformation-github-teams-team-1.4.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-07-03 06:16:02.000000 cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     9243 2023-07-03 06:15:56.000000 cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-07-03 06:16:02.000000 cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      450 2023-07-03 06:15:56.000000 cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    18012 2023-07-03 06:15:56.000000 cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team/_jsii/github-teams-team@1.4.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-07-03 06:15:56.000000 cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-07-03 06:16:02.000000 cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2915 2023-07-03 06:16:02.000000 cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      622 2023-07-03 06:16:02.000000 cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-07-03 06:16:02.000000 cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      112 2023-07-03 06:16:02.000000 cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       37 2023-07-03 06:16:02.000000 cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team.egg-info/top_level.txt
```

### Comparing `cdk-cloudformation-github-teams-team-1.2.0a7/LICENSE` & `cdk-cloudformation-github-teams-team-1.4.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-github-teams-team-1.2.0a7/PKG-INFO` & `cdk-cloudformation-github-teams-team-1.4.0a7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-github-teams-team
-Version: 1.2.0a7
+Version: 1.4.0a7
 Summary: Manage a team in Github
 Home-page: https://github.com/aws-ia/cloudformation-github-resource-providers
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # github-teams-team
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `GitHub::Teams::Team` v1.2.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `GitHub::Teams::Team` v1.4.0.
 
 ## Description
 
 Manage a team in Github
 
 ## References
 
@@ -56,13 +56,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `GitHub::Teams::Team`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fgithub-teams-team+v1.2.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fgithub-teams-team+v1.4.0).
 * Issues related to `GitHub::Teams::Team` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-github-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-github-teams-team-1.2.0a7/README.md` & `cdk-cloudformation-github-teams-team-1.4.0a7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # github-teams-team
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `GitHub::Teams::Team` v1.2.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `GitHub::Teams::Team` v1.4.0.
 
 ## Description
 
 Manage a team in Github
 
 ## References
 
@@ -33,13 +33,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `GitHub::Teams::Team`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fgithub-teams-team+v1.2.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fgithub-teams-team+v1.4.0).
 * Issues related to `GitHub::Teams::Team` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-github-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-github-teams-team-1.2.0a7/setup.py` & `cdk-cloudformation-github-teams-team-1.4.0a7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-github-teams-team",
-    "version": "1.2.0.a7",
+    "version": "1.4.0.a7",
     "description": "Manage a team in Github",
     "license": "Apache-2.0",
     "url": "https://github.com/aws-ia/cloudformation-github-resource-providers",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_cloudformation_github_teams_team",
         "cdk_cloudformation_github_teams_team._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_github_teams_team._jsii": [
-            "github-teams-team@1.2.0-alpha.7.jsii.tgz"
+            "github-teams-team@1.4.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_github_teams_team": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.70.0, <3.0.0",
-        "constructs>=10.1.292, <11.0.0",
-        "jsii>=1.79.0, <2.0.0",
+        "aws-cdk-lib>=2.86.0, <3.0.0",
+        "constructs>=10.2.67, <11.0.0",
+        "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team/__init__.py` & `cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # github-teams-team
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `GitHub::Teams::Team` v1.2.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `GitHub::Teams::Team` v1.4.0.
 
 ## Description
 
 Manage a team in Github
 
 ## References
 
@@ -34,15 +34,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `GitHub::Teams::Team`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fgithub-teams-team+v1.2.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fgithub-teams-team+v1.4.0).
 * Issues related to `GitHub::Teams::Team` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-github-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
```

### Comparing `cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team.egg-info/PKG-INFO` & `cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-github-teams-team
-Version: 1.2.0a7
+Version: 1.4.0a7
 Summary: Manage a team in Github
 Home-page: https://github.com/aws-ia/cloudformation-github-resource-providers
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # github-teams-team
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `GitHub::Teams::Team` v1.2.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `GitHub::Teams::Team` v1.4.0.
 
 ## Description
 
 Manage a team in Github
 
 ## References
 
@@ -56,13 +56,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `GitHub::Teams::Team`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fgithub-teams-team+v1.2.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fgithub-teams-team+v1.4.0).
 * Issues related to `GitHub::Teams::Team` should be reported to the [publisher](https://github.com/aws-ia/cloudformation-github-resource-providers).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-github-teams-team-1.2.0a7/src/cdk_cloudformation_github_teams_team.egg-info/SOURCES.txt` & `cdk-cloudformation-github-teams-team-1.4.0a7/src/cdk_cloudformation_github_teams_team.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_github_teams_team/py.typed
 src/cdk_cloudformation_github_teams_team.egg-info/PKG-INFO
 src/cdk_cloudformation_github_teams_team.egg-info/SOURCES.txt
 src/cdk_cloudformation_github_teams_team.egg-info/dependency_links.txt
 src/cdk_cloudformation_github_teams_team.egg-info/requires.txt
 src/cdk_cloudformation_github_teams_team.egg-info/top_level.txt
 src/cdk_cloudformation_github_teams_team/_jsii/__init__.py
-src/cdk_cloudformation_github_teams_team/_jsii/github-teams-team@1.2.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_github_teams_team/_jsii/github-teams-team@1.4.0-alpha.7.jsii.tgz
```

