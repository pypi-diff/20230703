# Comparing `tmp/datagit-0.6.tar.gz` & `tmp/datagit-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagit-0.6.tar", last modified: Mon Jul  3 15:31:15 2023, max compression
+gzip compressed data, was "datagit-0.7.tar", last modified: Mon Jul  3 17:14:34 2023, max compression
```

## Comparing `datagit-0.6.tar` & `datagit-0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 15:31:15.715847 datagit-0.6/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     3145 2023-07-03 15:31:15.715722 datagit-0.6/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)     2745 2023-07-03 14:48:50.000000 datagit-0.6/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 15:31:15.714716 datagit-0.6/datagit/
--rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-05-22 13:02:30.000000 datagit-0.6/datagit/__init__.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      635 2023-05-23 16:37:26.000000 datagit-0.6/datagit/dataset_helpers.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     9486 2023-07-03 15:30:11.000000 datagit-0.6/datagit/github_connector.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      721 2023-05-23 14:01:11.000000 datagit-0.6/datagit/query_builder.py
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 15:31:15.715500 datagit-0.6/datagit.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     3145 2023-07-03 15:31:15.000000 datagit-0.6/datagit.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      272 2023-07-03 15:31:15.000000 datagit-0.6/datagit.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-07-03 15:31:15.000000 datagit-0.6/datagit.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       16 2023-07-03 15:31:15.000000 datagit-0.6/datagit.egg-info/requires.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        8 2023-07-03 15:31:15.000000 datagit-0.6/datagit.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-07-03 15:31:15.715905 datagit-0.6/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      648 2023-07-03 15:31:02.000000 datagit-0.6/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 17:14:34.110550 datagit-0.7/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3145 2023-07-03 17:14:34.110393 datagit-0.7/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     2745 2023-07-03 14:48:50.000000 datagit-0.7/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 17:14:34.109029 datagit-0.7/datagit/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-05-22 13:02:30.000000 datagit-0.7/datagit/__init__.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     2120 2023-07-03 17:12:23.000000 datagit-0.7/datagit/dataset_helpers.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     9717 2023-07-03 17:07:17.000000 datagit-0.7/datagit/github_connector.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      721 2023-05-23 14:01:11.000000 datagit-0.7/datagit/query_builder.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 17:14:34.110116 datagit-0.7/datagit.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3145 2023-07-03 17:14:33.000000 datagit-0.7/datagit.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      272 2023-07-03 17:14:33.000000 datagit-0.7/datagit.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-07-03 17:14:33.000000 datagit-0.7/datagit.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       16 2023-07-03 17:14:33.000000 datagit-0.7/datagit.egg-info/requires.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        8 2023-07-03 17:14:33.000000 datagit-0.7/datagit.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-07-03 17:14:34.110633 datagit-0.7/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      648 2023-07-03 17:14:31.000000 datagit-0.7/setup.py
```

### Comparing `datagit-0.6/PKG-INFO` & `datagit-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagit
-Version: 0.6
+Version: 0.7
 Summary: Git based metric store
 Home-page: https://github.com/data-drift/datagit
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datagit-0.6/README.md` & `datagit-0.7/README.md`

 * *Files identical despite different names*

### Comparing `datagit-0.6/datagit/github_connector.py` & `datagit-0.7/datagit/github_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 from typing import Optional, List
 import pandas as pd
 from github import Github, Repository, ContentFile, GithubException
-from datagit.dataset_helpers import sort_dataframe_on_first_column_and_assert_is_unique
+from datagit.dataset_helpers import compare_dataframes, sort_dataframe_on_first_column_and_assert_is_unique
 import re
 import base64
 import io
 
 
 def store_metric(ghClient: Github, dataframe: pd.DataFrame, filepath: str, assignees: List[str] = [], branch: Optional[str] = None, store_json: bool = True) -> None:
     print("Storing metric...")
@@ -52,15 +52,18 @@
             checkout_branch_from_default_branch(repo, computed_branch)
             if not old_data_with_freshdata.equals(dataframe):
                 print("Drift detected")
                 push_drift_lines(file_path, repo, computed_branch,
                                  dataframe, store_json)
                 print("Drift pushed")
                 print("Creating pull request")
-                create_pullrequest(repo, computed_branch, assignees, file_path)
+                description_body = f"Drift detected:\n" + \
+                    compare_dataframes(old_data_with_freshdata, dataframe, "unique_key")
+                create_pullrequest(repo, computed_branch,
+                                   assignees, file_path, description_body)
 
     pass
 
 
 def assert_file_exists(repo: Repository.Repository, file_path: str, ref: str) -> Optional[ContentFile.ContentFile]:
     try:
         contents = repo.get_contents(file_path, ref=ref)
@@ -132,19 +135,19 @@
         index=False, header=True), branch)
     if store_json:
         json_file_path = file_path.replace(".csv", ".json")
         repo.create_file(json_file_path, "New data (json): " +
                          file_path, dataframe.to_json(orient="records", lines=True, date_format="iso"), branch)
 
 
-def create_pullrequest(repo: Repository.Repository, branch: str, assignees: List[str], file_path: str):
+def create_pullrequest(repo: Repository.Repository, branch: str, assignees: List[str], file_path: str, description_body: str):
     try:
         if len(assignees) > 0:
             pullrequest = repo.create_pull(
-                title="New drift detected "+file_path, body="A new drift has been detecte", head=branch, base=repo.default_branch)
+                title="New drift detected "+file_path, body=description_body, head=branch, base=repo.default_branch)
             print("Pull request created: " + pullrequest.html_url)
             existing_assignees = assert_assignees_exists(repo, assignees)
             pullrequest.add_to_assignees(*existing_assignees)
         else:
             print("No assignees, skipping pull request creation")
     except GithubException as e:
         if e.status == 422:
```

### Comparing `datagit-0.6/datagit/query_builder.py` & `datagit-0.7/datagit/query_builder.py`

 * *Files identical despite different names*

### Comparing `datagit-0.6/datagit.egg-info/PKG-INFO` & `datagit-0.7/datagit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagit
-Version: 0.6
+Version: 0.7
 Summary: Git based metric store
 Home-page: https://github.com/data-drift/datagit
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datagit-0.6/setup.py` & `datagit-0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="datagit",
-    version="0.6",
+    version="0.7",
     packages=find_packages(),
     author="Sammy Teillet",
     author_email="sammy.teillet@gmail.com",
     description="Git based metric store",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/data-drift/datagit",
```

