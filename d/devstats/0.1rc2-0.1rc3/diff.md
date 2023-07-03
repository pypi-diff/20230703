# Comparing `tmp/devstats-0.1rc2.tar.gz` & `tmp/devstats-0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devstats-0.1rc2.tar", last modified: Fri May 26 16:02:59 2023, max compression
+gzip compressed data, was "devstats-0.1rc3.tar", last modified: Mon Jul  3 19:43:08 2023, max compression
```

## Comparing `devstats-0.1rc2.tar` & `devstats-0.1rc3.tar`

### file list

```diff
@@ -1,34 +1,46 @@
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-26 16:02:59.910227 devstats-0.1rc2/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1504 2023-05-22 22:53:17.000000 devstats-0.1rc2/LICENSE
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2146 2023-05-26 16:02:59.910227 devstats-0.1rc2/PKG-INFO
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2146 2023-05-24 23:45:39.000000 devstats-0.1rc2/README.md
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-26 16:02:59.906227 devstats-0.1rc2/devstats/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 00:27:42.000000 devstats-0.1rc2/devstats/__init__.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1764 2023-05-26 15:53:46.000000 devstats-0.1rc2/devstats/__main__.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      999 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/publish.py
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-26 16:02:59.908228 devstats-0.1rc2/devstats/queries/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1453 2023-05-24 00:22:14.000000 devstats-0.1rc2/devstats/queries/issue_activity_since_date.gql
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      582 2023-05-24 00:22:14.000000 devstats-0.1rc2/devstats/queries/pr_data_query.gql
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6364 2023-05-24 16:58:50.000000 devstats-0.1rc2/devstats/query.py
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-26 16:02:59.904228 devstats-0.1rc2/devstats/reports/
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-26 16:02:59.908228 devstats-0.1rc2/devstats/reports/issues/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      445 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/issues/first_responders.md
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1786 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/issues/new_issues.md
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     3079 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/issues/time_to_response.md
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-26 16:02:59.910227 devstats-0.1rc2/devstats/reports/pull_requests/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1078 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/pull_requests/mergeability_of_open_prs.md
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2080 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/pull_requests/merged_prs_over_time.md
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      824 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/pull_requests/number_of_pr_participants.md
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1695 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/pull_requests/pony_factor.md
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2424 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/pull_requests/pr_lifetime.md
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1669 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/reports/pull_requests/where_contributions_come_from.md
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2881 2023-05-26 15:58:53.000000 devstats-0.1rc2/devstats/template.md
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-05-26 16:02:59.907227 devstats-0.1rc2/devstats.egg-info/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2146 2023-05-26 16:02:59.000000 devstats-0.1rc2/devstats.egg-info/PKG-INFO
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      865 2023-05-26 16:02:59.000000 devstats-0.1rc2/devstats.egg-info/SOURCES.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)        1 2023-05-26 16:02:59.000000 devstats-0.1rc2/devstats.egg-info/dependency_links.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       51 2023-05-26 16:02:59.000000 devstats-0.1rc2/devstats.egg-info/entry_points.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       73 2023-05-26 16:02:59.000000 devstats-0.1rc2/devstats.egg-info/requires.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)        9 2023-05-26 16:02:59.000000 devstats-0.1rc2/devstats.egg-info/top_level.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      847 2023-05-26 15:59:15.000000 devstats-0.1rc2/pyproject.toml
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       38 2023-05-26 16:02:59.911228 devstats-0.1rc2/setup.cfg
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-03 19:43:08.472243 devstats-0.1rc3/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       12 2023-07-03 18:30:07.000000 devstats-0.1rc3/CHANGELOG.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1504 2023-05-22 22:53:17.000000 devstats-0.1rc3/LICENSE
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       21 2023-07-03 18:30:07.000000 devstats-0.1rc3/MANIFEST.in
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2166 2023-07-03 19:43:08.472243 devstats-0.1rc3/PKG-INFO
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2146 2023-05-26 17:10:32.000000 devstats-0.1rc3/README.md
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-03 19:43:08.464243 devstats-0.1rc3/devstats/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        0 2023-05-24 00:27:42.000000 devstats-0.1rc3/devstats/__init__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2150 2023-07-03 19:34:52.000000 devstats-0.1rc3/devstats/__main__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2547 2023-07-03 19:34:52.000000 devstats-0.1rc3/devstats/publish.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-03 19:43:08.466243 devstats-0.1rc3/devstats/queries/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1453 2023-05-24 00:22:14.000000 devstats-0.1rc3/devstats/queries/issue_activity_since_date.gql
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      582 2023-05-24 00:22:14.000000 devstats-0.1rc3/devstats/queries/pr_data_query.gql
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6364 2023-05-24 16:58:50.000000 devstats-0.1rc3/devstats/query.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-03 19:43:08.468243 devstats-0.1rc3/devstats/reports/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2244 2023-07-03 19:34:52.000000 devstats-0.1rc3/devstats/reports/index.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      428 2023-07-03 19:34:52.000000 devstats-0.1rc3/devstats/reports/issue_first_responders.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     3062 2023-07-03 19:34:52.000000 devstats-0.1rc3/devstats/reports/issue_time_to_response.md
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-03 19:43:08.469243 devstats-0.1rc3/devstats/reports/issues/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      445 2023-07-03 18:30:07.000000 devstats-0.1rc3/devstats/reports/issues/first_responders.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1786 2023-07-03 18:30:07.000000 devstats-0.1rc3/devstats/reports/issues/new_issues.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     3079 2023-07-03 18:30:07.000000 devstats-0.1rc3/devstats/reports/issues/time_to_response.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2161 2023-07-03 19:34:52.000000 devstats-0.1rc3/devstats/reports/new_issues.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      650 2023-07-03 19:34:52.000000 devstats-0.1rc3/devstats/reports/preamble.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1651 2023-07-03 19:34:52.000000 devstats-0.1rc3/devstats/reports/prs_contributor_origin.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2415 2023-07-03 19:34:52.000000 devstats-0.1rc3/devstats/reports/prs_lifetime.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1069 2023-07-03 19:34:52.000000 devstats-0.1rc3/devstats/reports/prs_mergeability.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2071 2023-07-03 19:34:52.000000 devstats-0.1rc3/devstats/reports/prs_merged_over_time.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      815 2023-07-03 19:34:52.000000 devstats-0.1rc3/devstats/reports/prs_participants.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1687 2023-07-03 19:34:52.000000 devstats-0.1rc3/devstats/reports/prs_pony_factor.md
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-03 19:43:08.471243 devstats-0.1rc3/devstats/reports/pull_requests/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1078 2023-07-03 18:30:07.000000 devstats-0.1rc3/devstats/reports/pull_requests/mergeability_of_open_prs.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2080 2023-07-03 18:30:07.000000 devstats-0.1rc3/devstats/reports/pull_requests/merged_prs_over_time.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      824 2023-07-03 18:30:07.000000 devstats-0.1rc3/devstats/reports/pull_requests/number_of_pr_participants.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1695 2023-07-03 18:30:07.000000 devstats-0.1rc3/devstats/reports/pull_requests/pony_factor.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2424 2023-07-03 18:30:07.000000 devstats-0.1rc3/devstats/reports/pull_requests/pr_lifetime.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1669 2023-07-03 18:30:07.000000 devstats-0.1rc3/devstats/reports/pull_requests/where_contributions_come_from.md
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-03 19:43:08.465243 devstats-0.1rc3/devstats.egg-info/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2166 2023-07-03 19:43:08.000000 devstats-0.1rc3/devstats.egg-info/PKG-INFO
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1268 2023-07-03 19:43:08.000000 devstats-0.1rc3/devstats.egg-info/SOURCES.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        1 2023-07-03 19:43:08.000000 devstats-0.1rc3/devstats.egg-info/dependency_links.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       51 2023-07-03 19:43:08.000000 devstats-0.1rc3/devstats.egg-info/entry_points.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       96 2023-07-03 19:43:08.000000 devstats-0.1rc3/devstats.egg-info/requires.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        9 2023-07-03 19:43:08.000000 devstats-0.1rc3/devstats.egg-info/top_level.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      872 2023-07-03 19:35:56.000000 devstats-0.1rc3/pyproject.toml
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       38 2023-07-03 19:43:08.472243 devstats-0.1rc3/setup.cfg
```

### Comparing `devstats-0.1rc2/LICENSE` & `devstats-0.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc2/PKG-INFO` & `devstats-0.1rc3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devstats
-Version: 0.1rc2
+Version: 0.1rc3
 Summary: Developer tool for scientific Python libraries
 Maintainer-email: Scientific Python <devstats@discuss.scientific-python.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scientific Python
         
         Redistribution and use in source and binary forms, with or without
@@ -33,8 +33,9 @@
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: homepage, https://github.com/scientific-python/devstats
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Provides-Extra: lint
+Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `devstats-0.1rc2/README.md` & `devstats-0.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc2/devstats/__main__.py` & `devstats-0.1rc3/devstats/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,48 @@
 import json
 import os
 import re
 import sys
 from glob import glob
+import collections
 
 import click
 import requests
 
 from .query import GithubGrabber
-from .publish import publisher
+from .publish import template, publish
 
 
-@click.group()
+class OrderedGroup(click.Group):
+    def __init__(self, name=None, commands=None, **attrs):
+        super().__init__(name, commands, **attrs)
+        self.commands = commands or collections.OrderedDict()
+
+    def list_commands(self, ctx):
+        return self.commands
+
+
+@click.group(cls=OrderedGroup)
 def cli():
     pass
 
 
 @cli.command("query")
 @click.argument("repo_owner")
 @click.argument("repo_name")
-def query(repo_owner, repo_name):
-    """Download and save issue and pr data for `repo_owner`/`repo_name`."""
+@click.option(
+    "-o",
+    "--outdir",
+    default="devstats-data",
+    help="Output directory",
+    show_default=True,
+)
+def query(repo_owner, repo_name, outdir):
+    """Download and save issue and pr data for `repo_owner`/`repo_name`"""
+    os.makedirs(outdir, exist_ok=True)
 
     try:
         token = os.environ["GRAPH_API_KEY"]
     except KeyError:
         print("You need to set GRAPH_API_KEY")
         sys.exit()
 
@@ -55,15 +73,12 @@
             qtype,
             headers,
             repo_owner=repo_owner,
             repo_name=repo_name,
         )
         data.get()
         ftype = {"issues": "issues", "pullRequests": "PRs"}
-        data.dump(f"{repo_name}_{ftype.get(qtype, qtype)}.json")
+        data.dump(f"{outdir}/{repo_name}_{ftype.get(qtype, qtype)}.json")
 
 
-@cli.command("publish")
-@click.argument("project")
-def publish(project):
-    """Generate myst report for `repo_owner`/`repo_name`."""
-    publisher(project)
+cli.add_command(template)
+cli.add_command(publish)
```

### Comparing `devstats-0.1rc2/devstats/queries/issue_activity_since_date.gql` & `devstats-0.1rc3/devstats/queries/issue_activity_since_date.gql`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc2/devstats/queries/pr_data_query.gql` & `devstats-0.1rc3/devstats/queries/pr_data_query.gql`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc2/devstats/query.py` & `devstats-0.1rc3/devstats/query.py`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc2/devstats/reports/issues/new_issues.md` & `devstats-0.1rc3/devstats/reports/issues/new_issues.md`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc2/devstats/reports/issues/time_to_response.md` & `devstats-0.1rc3/devstats/reports/issues/time_to_response.md`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc2/devstats/reports/pull_requests/mergeability_of_open_prs.md` & `devstats-0.1rc3/devstats/reports/pull_requests/mergeability_of_open_prs.md`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc2/devstats/reports/pull_requests/merged_prs_over_time.md` & `devstats-0.1rc3/devstats/reports/pull_requests/merged_prs_over_time.md`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc2/devstats/reports/pull_requests/number_of_pr_participants.md` & `devstats-0.1rc3/devstats/reports/pull_requests/number_of_pr_participants.md`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc2/devstats/reports/pull_requests/pony_factor.md` & `devstats-0.1rc3/devstats/reports/pull_requests/pony_factor.md`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc2/devstats/reports/pull_requests/pr_lifetime.md` & `devstats-0.1rc3/devstats/reports/pull_requests/pr_lifetime.md`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc2/devstats/reports/pull_requests/where_contributions_come_from.md` & `devstats-0.1rc3/devstats/reports/pull_requests/where_contributions_come_from.md`

 * *Files identical despite different names*

### Comparing `devstats-0.1rc2/devstats.egg-info/PKG-INFO` & `devstats-0.1rc3/devstats.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devstats
-Version: 0.1rc2
+Version: 0.1rc3
 Summary: Developer tool for scientific Python libraries
 Maintainer-email: Scientific Python <devstats@discuss.scientific-python.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scientific Python
         
         Redistribution and use in source and binary forms, with or without
@@ -33,8 +33,9 @@
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: homepage, https://github.com/scientific-python/devstats
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Provides-Extra: lint
+Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `devstats-0.1rc2/pyproject.toml` & `devstats-0.1rc3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=61.2"]
 
 [project]
 name = "devstats"
-version = "0.1rc2"
+version = "0.1rc3"
 requires-python = ">=3.8"
 description = "Developer tool for scientific Python libraries"
 license = {file = "LICENSE"}
 maintainers = [
   {name = "Scientific Python", email = "devstats@discuss.scientific-python.org"}
 ]
 classifiers = [
@@ -24,15 +24,16 @@
   "networkx",
 ]
 
 [project.scripts]
 devstats = "devstats.__main__:cli"
 
 [project.optional-dependencies]
-lint = ["pre-commit >= 3.3.2"]
+lint = ["pre-commit == 3.3.3"]
+dev = ["changelist == 0.1"]
 
 [project.urls]
 homepage = "https://github.com/scientific-python/devstats"
 
 [tool.setuptools.packages.find]
 include = ["devstats*"]
```

