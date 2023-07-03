# Comparing `tmp/gitlabx-0.2.0-py3-none-any.whl.zip` & `tmp/gitlabx-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,24 @@
-Zip file size: 8866 bytes, number of entries: 17
--rwxrwxrwx  2.0 unx      970 b- defN 23-Jul-02 21:49 gitlabx/Member.py
+Zip file size: 12446 bytes, number of entries: 22
 -rwxrwxrwx  2.0 unx        0 b- defN 23-Jun-28 23:28 gitlabx/__init__.py
 -rwxrwxrwx  2.0 unx      380 b- defN 23-Jun-29 10:14 gitlabx/abstract.py
 -rwxrwxrwx  2.0 unx      950 b- defN 23-Jun-29 23:39 gitlabx/branches.py
--rwxrwxrwx  2.0 unx      972 b- defN 23-Jun-30 00:06 gitlabx/commits.py
+-rwxrwxrwx  2.0 unx     1241 b- defN 23-Jul-02 23:24 gitlabx/commits.py
 -rwxrwxrwx  2.0 unx     1026 b- defN 23-Jun-29 11:24 gitlabx/deployments.py
 -rwxrwxrwx  2.0 unx      902 b- defN 23-Jun-29 11:24 gitlabx/events.py
--rwxrwxrwx  2.0 unx     1985 b- defN 23-Jul-02 21:49 gitlabx/factories.py
+-rwxrwxrwx  2.0 unx     2795 b- defN 23-Jul-02 23:47 gitlabx/factories.py
 -rwxrwxrwx  2.0 unx      944 b- defN 23-Jun-29 11:24 gitlabx/issues.py
+-rwxrwxrwx  2.0 unx      984 b- defN 23-Jul-02 23:37 gitlabx/jobs.py
+-rwxrwxrwx  2.0 unx      974 b- defN 23-Jul-02 22:40 gitlabx/member.py
+-rwxrwxrwx  2.0 unx     1204 b- defN 23-Jul-02 23:01 gitlabx/merge_request.py
+-rwxrwxrwx  2.0 unx     1233 b- defN 23-Jul-02 23:49 gitlabx/pipelines.py
+-rwxrwxrwx  2.0 unx     1121 b- defN 23-Jul-02 23:38 gitlabx/pipelines_schedules.py
 -rwxrwxrwx  2.0 unx      785 b- defN 23-Jun-29 11:24 gitlabx/project.py
 -rwxrwxrwx  2.0 unx      979 b- defN 23-Jun-29 11:24 gitlabx/projectLanguages.py
 -rwxrwxrwx  2.0 unx     1026 b- defN 23-Jun-29 11:24 gitlabx/repositories.py
--rwxrwxrwx  2.0 unx     1080 b- defN 23-Jun-29 11:24 gitlabx/repositoryTree.py
--rwxrwxrwx  2.0 unx     1675 b- defN 23-Jul-02 21:51 gitlabx-0.2.0.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-02 21:51 gitlabx-0.2.0.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jul-02 21:51 gitlabx-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1288 b- defN 23-Jul-02 21:51 gitlabx-0.2.0.dist-info/RECORD
-17 files, 15062 bytes uncompressed, 6774 bytes compressed:  55.0%
+-rwxrwxrwx  2.0 unx     1376 b- defN 23-Jul-02 22:55 gitlabx/repositoryTree.py
+-rwxrwxrwx  2.0 unx     1062 b- defN 23-Jul-02 23:34 gitlabx/trriggers.py
+-rwxrwxrwx  2.0 unx     1675 b- defN 23-Jul-03 00:08 gitlabx-0.3.0.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-03 00:08 gitlabx-0.3.0.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jul-03 00:08 gitlabx-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1682 b- defN 23-Jul-03 00:08 gitlabx-0.3.0.dist-info/RECORD
+22 files, 22439 bytes uncompressed, 9756 bytes compressed:  56.5%
```

## zipnote {}

```diff
@@ -1,10 +1,7 @@
-Filename: gitlabx/Member.py
-Comment: 
-
 Filename: gitlabx/__init__.py
 Comment: 
 
 Filename: gitlabx/abstract.py
 Comment: 
 
 Filename: gitlabx/branches.py
@@ -21,32 +18,50 @@
 
 Filename: gitlabx/factories.py
 Comment: 
 
 Filename: gitlabx/issues.py
 Comment: 
 
+Filename: gitlabx/jobs.py
+Comment: 
+
+Filename: gitlabx/member.py
+Comment: 
+
+Filename: gitlabx/merge_request.py
+Comment: 
+
+Filename: gitlabx/pipelines.py
+Comment: 
+
+Filename: gitlabx/pipelines_schedules.py
+Comment: 
+
 Filename: gitlabx/project.py
 Comment: 
 
 Filename: gitlabx/projectLanguages.py
 Comment: 
 
 Filename: gitlabx/repositories.py
 Comment: 
 
 Filename: gitlabx/repositoryTree.py
 Comment: 
 
-Filename: gitlabx-0.2.0.dist-info/METADATA
+Filename: gitlabx/trriggers.py
+Comment: 
+
+Filename: gitlabx-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: gitlabx-0.2.0.dist-info/WHEEL
+Filename: gitlabx-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: gitlabx-0.2.0.dist-info/top_level.txt
+Filename: gitlabx-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gitlabx-0.2.0.dist-info/RECORD
+Filename: gitlabx-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gitlabx/commits.py

```diff
@@ -15,20 +15,26 @@
 		commit_list = []
 
 		try:
 			logging.info("Start function: get_Commits")
 			result = self.gl.projects.list(owned=True, iterator=True)
 
 			for project in result:
+				logging.info("Start function: get_Commits:"+project.name )
 				commits = project.commits.list(iterator=True,all=True)
 				project = project.asdict()
 				for	commit in commits:
-					commit = commit.asdict()
-					commit['project_id'] = project['id']
-					commit_list.append(commit)
+					commitX = commit.asdict()
+					commitX['project_id'] = project['id']
+					commitX['merge_requests'] = commit.merge_requests()
+					commitX['refs'] = commit.refs() 
+					commitX['comments'] = commit.comments.list()
+					commitX['statuses '] = commit.statuses.list()
+
+					commit_list.append(commitX)
 			
 		except Exception as e: 
 			logging.error("OS error: {0}".format(e))
 			logging.error(e.__dict__) 
 
 		logging.info("Retrieve All Project Commits")
```

## gitlabx/factories.py

```diff
@@ -4,15 +4,53 @@
 from .branches import Branches
 from .commits import Commits
 from .deployments import Deployments
 from .events import Events
 from .issues import Issues
 from .repositories import Repositories
 from .projectLanguages import ProjectLanguages
-from .Member import Member
+from .member import Member
+from .merge_request import MergeRequest
+from .pipelines import Pipelines
+from .pipelines_schedules import PipelinesSchedules
+from .jobs import Job
+
+class JobFactory(factory.Factory):
+    
+    class Meta:
+        model = Job
+        
+    personal_access_token = None
+    gitlab_url = None
+
+class PipelinesSchedulesFactory(factory.Factory):
+    
+    class Meta:
+        model = PipelinesSchedules
+        
+    personal_access_token = None
+    gitlab_url = None
+
+class PipelineFactory(factory.Factory):
+    
+    class Meta:
+        model = Pipelines
+        
+    personal_access_token = None
+    gitlab_url = None
+
+
+class MergeRequestFactory(factory.Factory):
+    
+    class Meta:
+        model = MergeRequest
+        
+    personal_access_token = None
+    gitlab_url = None
+
 
 class ProjectFactory(factory.Factory):
     
     class Meta:
         model = Project
         
     personal_access_token = None
```

## gitlabx/repositoryTree.py

```diff
@@ -15,19 +15,30 @@
 
 		try:
 			logging.info("Start function: get_projects_repository_tree")
 			
 			projects = self.gl.projects.list(owned=True, iterator=True)
 
 			for project in projects:
-				project_repository_tree_return = project.repository_tree()
-				project = project.asdict()
-				for repository_tree in project_repository_tree_return:
-					repository_tree["project_id"] = project["id"]
-					project_repository_tree.append(repository_tree)
+				try:
+					logging.info("ProjectName:"+project.name)	
+					project_repository_tree_return = project.repository_tree(get_all=True, iterator=True)
+					
+					for item in project_repository_tree_return:
+						if item["type"] == 'blob':
+							file_info =  project.repository_blob(item["id"])
+							item["file_info"] = file_info
+						
+						item["project_id"] = project.id
+						project_repository_tree.append(item)
+						
+											
+				except Exception as e: 
+					logging.error("OS error: {0}".format(e))
+					logging.error(e.__dict__) 
 
 			
 		except Exception as e: 
 			logging.error("OS error: {0}".format(e))
 			logging.error(e.__dict__) 
 
 		logging.info("Retrieve All Projects Repository Tree")
```

## Comparing `gitlabx/Member.py` & `gitlabx/member.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 		member_list = []
 
 		try:
 			logging.info("Start function: get_members")
 			result = self.gl.projects.list(owned=True, iterator=True)
 
 			for project in result:
-				members = project.members.list(iterator=True,all=True)
+				members = project.members_all.list(iterator=True,all=True)
 				project = project.asdict()
 				for	member in members:
 					member = member.asdict()
 					member['project_id'] = project['id']
 					member_list.append(member)
 			
 		except Exception as e:
```

## Comparing `gitlabx-0.2.0.dist-info/METADATA` & `gitlabx-0.3.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabx
-Version: 0.2.0
+Version: 0.3.0
 Summary: Uma Lib para buscar dados do Gitlab
 Home-page: https://gitlab.com/immigrant-data-driven-development/libs/application/gitlab
 Author: Carlos Henrique Maulaz de Freitas
 Author-email: carlosmaulaz@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

