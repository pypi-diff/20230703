# Comparing `tmp/datagit-0.5.tar.gz` & `tmp/datagit-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagit-0.5.tar", last modified: Mon Jul  3 15:15:45 2023, max compression
+gzip compressed data, was "datagit-0.6.tar", last modified: Mon Jul  3 15:31:15 2023, max compression
```

## Comparing `datagit-0.5.tar` & `datagit-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 15:15:45.361710 datagit-0.5/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     3145 2023-07-03 15:15:45.361578 datagit-0.5/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)     2745 2023-07-03 14:48:50.000000 datagit-0.5/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 15:15:45.360694 datagit-0.5/datagit/
--rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-05-22 13:02:30.000000 datagit-0.5/datagit/__init__.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      635 2023-05-23 16:37:26.000000 datagit-0.5/datagit/dataset_helpers.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     9436 2023-07-03 14:56:00.000000 datagit-0.5/datagit/github_connector.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      721 2023-05-23 14:01:11.000000 datagit-0.5/datagit/query_builder.py
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 15:15:45.361381 datagit-0.5/datagit.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     3145 2023-07-03 15:15:45.000000 datagit-0.5/datagit.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      272 2023-07-03 15:15:45.000000 datagit-0.5/datagit.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-07-03 15:15:45.000000 datagit-0.5/datagit.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       16 2023-07-03 15:15:45.000000 datagit-0.5/datagit.egg-info/requires.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        8 2023-07-03 15:15:45.000000 datagit-0.5/datagit.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-07-03 15:15:45.361762 datagit-0.5/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      648 2023-07-03 15:15:02.000000 datagit-0.5/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 15:31:15.715847 datagit-0.6/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3145 2023-07-03 15:31:15.715722 datagit-0.6/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     2745 2023-07-03 14:48:50.000000 datagit-0.6/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 15:31:15.714716 datagit-0.6/datagit/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-05-22 13:02:30.000000 datagit-0.6/datagit/__init__.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      635 2023-05-23 16:37:26.000000 datagit-0.6/datagit/dataset_helpers.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     9486 2023-07-03 15:30:11.000000 datagit-0.6/datagit/github_connector.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      721 2023-05-23 14:01:11.000000 datagit-0.6/datagit/query_builder.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 15:31:15.715500 datagit-0.6/datagit.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3145 2023-07-03 15:31:15.000000 datagit-0.6/datagit.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      272 2023-07-03 15:31:15.000000 datagit-0.6/datagit.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-07-03 15:31:15.000000 datagit-0.6/datagit.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       16 2023-07-03 15:31:15.000000 datagit-0.6/datagit.egg-info/requires.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        8 2023-07-03 15:31:15.000000 datagit-0.6/datagit.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-07-03 15:31:15.715905 datagit-0.6/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      648 2023-07-03 15:31:02.000000 datagit-0.6/setup.py
```

### Comparing `datagit-0.5/PKG-INFO` & `datagit-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagit
-Version: 0.5
+Version: 0.6
 Summary: Git based metric store
 Home-page: https://github.com/data-drift/datagit
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datagit-0.5/README.md` & `datagit-0.6/README.md`

 * *Files identical despite different names*

### Comparing `datagit-0.5/datagit/dataset_helpers.py` & `datagit-0.6/datagit/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `datagit-0.5/datagit/github_connector.py` & `datagit-0.6/datagit/github_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             checkout_branch_from_default_branch(repo, computed_branch)
             if not old_data_with_freshdata.equals(dataframe):
                 print("Drift detected")
                 push_drift_lines(file_path, repo, computed_branch,
                                  dataframe, store_json)
                 print("Drift pushed")
                 print("Creating pull request")
-                create_pullrequest(repo, computed_branch, assignees)
+                create_pullrequest(repo, computed_branch, assignees, file_path)
 
     pass
 
 
 def assert_file_exists(repo: Repository.Repository, file_path: str, ref: str) -> Optional[ContentFile.ContentFile]:
     try:
         contents = repo.get_contents(file_path, ref=ref)
@@ -71,22 +71,22 @@
         if e.status == 404:
             return None
         else:
             raise e
 
 
 def push_new_lines(file_path: str, repo: Repository.Repository, branch: str, dataframe: pd.DataFrame, store_json: bool):
-    commit_message = "New metric: " + file_path
+    commit_message = "New data: " + file_path
     print("Commit: " + commit_message)
     update_file_with_retry(repo, file_path, commit_message,
                            dataframe.to_csv(index=False, header=True), branch)
 
     if store_json:
         json_file_path = file_path.replace(".csv", ".json")
-        json_commit_message = "New metric (json): " + json_file_path
+        json_commit_message = "New data (json): " + json_file_path
         json_data = dataframe.to_json(
             orient="records", lines=True, date_format="iso")
         update_file_with_retry(repo, json_file_path,
                                json_commit_message, json_data, branch)
 
 
 def push_drift_lines(file_path: str, repo: Repository.Repository, branch: str, dataframe: pd.DataFrame, store_json: bool):
@@ -122,29 +122,29 @@
                 time.sleep(1)  # Wait for 1 second before retrying
             else:
                 raise e
     raise Exception(f"Failed to update file after {max_retries} retries")
 
 
 def create_file_on_branch(file_path: str, repo: Repository.Repository, branch: str, dataframe: pd.DataFrame, assignees: List[str], store_json: bool):
-    commit_message = "New metric: " + file_path
+    commit_message = "New data: " + file_path
     print("Commit: " + commit_message)
     repo.create_file(file_path, commit_message, dataframe.to_csv(
         index=False, header=True), branch)
     if store_json:
         json_file_path = file_path.replace(".csv", ".json")
-        repo.create_file(json_file_path, "New metric (json): " +
+        repo.create_file(json_file_path, "New data (json): " +
                          file_path, dataframe.to_json(orient="records", lines=True, date_format="iso"), branch)
 
 
-def create_pullrequest(repo: Repository.Repository, branch: str, assignees: List[str]):
+def create_pullrequest(repo: Repository.Repository, branch: str, assignees: List[str], file_path: str):
     try:
         if len(assignees) > 0:
             pullrequest = repo.create_pull(
-                title="New data", body="New data available", head=branch, base=repo.default_branch)
+                title="New drift detected "+file_path, body="A new drift has been detecte", head=branch, base=repo.default_branch)
             print("Pull request created: " + pullrequest.html_url)
             existing_assignees = assert_assignees_exists(repo, assignees)
             pullrequest.add_to_assignees(*existing_assignees)
         else:
             print("No assignees, skipping pull request creation")
     except GithubException as e:
         if e.status == 422:
```

### Comparing `datagit-0.5/datagit/query_builder.py` & `datagit-0.6/datagit/query_builder.py`

 * *Files identical despite different names*

### Comparing `datagit-0.5/datagit.egg-info/PKG-INFO` & `datagit-0.6/datagit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagit
-Version: 0.5
+Version: 0.6
 Summary: Git based metric store
 Home-page: https://github.com/data-drift/datagit
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datagit-0.5/setup.py` & `datagit-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="datagit",
-    version="0.5",
+    version="0.6",
     packages=find_packages(),
     author="Sammy Teillet",
     author_email="sammy.teillet@gmail.com",
     description="Git based metric store",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/data-drift/datagit",
```

