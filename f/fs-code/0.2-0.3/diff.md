# Comparing `tmp/fs_code-0.2.tar.gz` & `tmp/fs_code-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs_code-0.2.tar", max compression
+gzip compressed data, was "fs_code-0.3.tar", max compression
```

## Comparing `fs_code-0.2.tar` & `fs_code-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-05-20 14:36:18.364352 fs_code-0.2/LICENSE
--rw-r--r--   0        0        0     1657 2023-05-20 14:36:18.364352 fs_code-0.2/README.md
--rw-r--r--   0        0        0     2245 2023-05-20 14:36:18.365352 fs_code-0.2/pyproject.toml
--rw-r--r--   0        0        0       37 2023-05-20 14:36:18.365352 fs_code-0.2/src/codefs/__init__.py
--rw-r--r--   0        0        0     3932 2023-05-20 14:36:18.365352 fs_code-0.2/src/codefs/_core.py
--rw-r--r--   0        0        0     4344 2023-05-20 14:36:18.365352 fs_code-0.2/src/codefs/gitfs/__init__.py
--rw-r--r--   0        0        0      723 2023-05-20 14:36:18.365352 fs_code-0.2/src/codefs/gitfs/opener.py
--rw-r--r--   0        0        0     4475 2023-05-20 14:36:18.366352 fs_code-0.2/src/codefs/githubfs/__init__.py
--rw-r--r--   0        0        0     2402 2023-05-20 14:36:18.366352 fs_code-0.2/src/codefs/githubfs/opener.py
--rw-r--r--   0        0        0     4785 2023-05-20 14:36:18.366352 fs_code-0.2/src/codefs/gitlabfs/__init__.py
--rw-r--r--   0        0        0     2697 2023-05-20 14:36:18.366352 fs_code-0.2/src/codefs/gitlabfs/opener.py
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 fs_code-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-03 19:04:20.909507 fs_code-0.3/LICENSE
+-rw-r--r--   0        0        0     1657 2023-07-03 19:04:20.909507 fs_code-0.3/README.md
+-rw-r--r--   0        0        0     2283 2023-07-03 19:04:20.910507 fs_code-0.3/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/__init__.py
+-rw-r--r--   0        0        0     3932 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/_core.py
+-rw-r--r--   0        0        0     4015 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/gitfs/__init__.py
+-rw-r--r--   0        0        0      723 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/gitfs/opener.py
+-rw-r--r--   0        0        0     4566 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/githubfs/__init__.py
+-rw-r--r--   0        0        0     2402 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/githubfs/opener.py
+-rw-r--r--   0        0        0     4855 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/gitlabfs/__init__.py
+-rw-r--r--   0        0        0     2697 2023-07-03 19:04:20.911507 fs_code-0.3/src/codefs/gitlabfs/opener.py
+-rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 fs_code-0.3/PKG-INFO
```

### Comparing `fs_code-0.2/LICENSE` & `fs_code-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fs_code-0.2/README.md` & `fs_code-0.3/README.md`

 * *Files identical despite different names*

### Comparing `fs_code-0.2/pyproject.toml` & `fs_code-0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fs-code"
-version = "0.2"
+version = "0.3"
 description = "PyFilesystems for GitLab, GitHub, and Git"
 license = "MIT"
 authors = [
     "Max Ludwig <mail@danjou.dev>",
 ]
 readme = "README.md"
 homepage = "https://danjou.gitlab.io/fs-code"
@@ -21,18 +21,18 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fs = "^2.4"
 schema = "~0.7"
 
 dulwich = { optional = true, version = "0.21.5" }
-python-gitlab = { optional = true, version = "^3.0" }
-werkzeug = { optional = true, version = "^2.0" }
-PyGithub = { optional = true, version = "^1.55" }
-requests = { optional = true, version = "^2.26" }
+python-gitlab = { optional = true, version = "^3.15" }
+werkzeug = { optional = true, version = "^2.3" }
+PyGithub = { optional = true, version = "^1.59" }
+requests = { optional = true, version = "^2.31" }
 
 [tool.poetry.extras]
 gitfs = [
     "dulwich",
 ]
 gitlabfs = [
     "python-gitlab",
@@ -56,15 +56,15 @@
 "github" = "codefs.githubfs.opener:Opener [githubfs]"
 "gitfs" = "codefs.gitfs.opener:Opener [gitfs]"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 dulwich = "*"
 mypy = "*"
-pdoc = "*"
+pdoc = "^13.1"  # taking care of the docs later
 pytest = "*"
 pytest-cov = "*"
 pytest-dotenv = "*"
 pytest-mock = "*"
 types-pytz = "*"
 types-PyYAML = "*"
 types-requests = "*"
```

### Comparing `fs_code-0.2/src/codefs/_core.py` & `fs_code-0.3/src/codefs/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from pathlib import PurePosixPath
 from typing import TypeVar, Callable, Generic, Mapping, List, Tuple, Protocol, Union
 
 from fs.base import FS
-from fs.errors import Unsupported, ResourceNotFound
+from fs.errors import ResourceNotFound
 from fs.memoryfs import MemoryFS
 from fs.mountfs import MountFS
 from fs.path import abspath, normpath
 from fs.subfs import SubFS
 from fs.wrap import read_only, WrapReadOnly
 from schema import And, Use  # type: ignore
 
@@ -26,14 +26,16 @@
         ...
 
     def get_repos(self) -> Mapping[str, Repository]:
         ...
 
 
 class AbstractArchiveFetcher(Protocol):
+    DEFAULT_BRANCH: str = "~"
+
     def __call__(self, ref: str) -> FS:
         ...
 
 
 class NamespaceFS(SubFS[WrapReadOnly[MountFS]]):
     def __init__(
         self,
@@ -103,15 +105,15 @@
         fs, path = super()._delegate(path)
         if fs is not self.default_fs:
             self._reset()
         return fs, path
 
     def listdir(self, path: str) -> List[str]:
         if _is_root(path):
-            raise Unsupported(path, msg="listing refs is too expensive")
+            return [self.fetch_archive.DEFAULT_BRANCH]
         return super().listdir(path)
 
 
 def Str() -> And:
     return And(str, len, error="must be non-empty string")
```

### Comparing `fs_code-0.2/src/codefs/gitfs/__init__.py` & `fs_code-0.3/src/codefs/gitfs/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -79,39 +79,38 @@
             return branch
         if tag and not branch:
             return tag
         raise RuntimeError(f"{ref!r} is both, a branch and a tag")
 
     def __call__(self, ref: str) -> FS:
         if not self._cache:
-            fs, repo, result = self._fetch()
+            fs, repo = self._fetch()
             with closing(fs):
-                committish = self.get_ref(result.refs, ref.encode())
+                if ref == self.DEFAULT_BRANCH:
+                    committish = porcelain.active_branch(repo)  # type: ignore
+                else:
+                    refs = repo.refs.as_dict()  # type: ignore
+                    committish = self.get_ref(refs, ref.encode())
                 data = BytesIO()
                 porcelain.archive(repo, committish=committish, outstream=data, errstream=NoneStream())  # type: ignore
                 data.seek(0)
                 self._cache = data.getvalue()
         return ReadTarFS(BytesIO(self._cache))  # type: ignore
 
-    def _fetch(self) -> Tuple[FS, Repo, FetchPackResult]:
+    def _fetch(self) -> Tuple[FS, Repo]:
         options = [
-            # 1st: in-memory and shallow, latter might fail because "depth not supported yet"
-            (MemoryFS, lambda _: MemoryRepo(), dict(depth=1)),  # type: ignore
-            # 2nd: in-memory, might fail because of https://github.com/jelmer/dulwich/issues/1179
-            (MemoryFS, lambda _: MemoryRepo(), {}),  # type: ignore
-            # 3rd: shallow, might fail because "depth not supported yet"
-            (TempFS, lambda fs: Repo.init(fs.root_path), dict(depth=1)),
-            # 4th: ultimate fallback -.-"
-            (TempFS, lambda fs: Repo.init(fs.root_path), {}),
+            # 1st: shallow, might fail because "depth not supported yet"
+            (TempFS, dict(depth=1)),
+            # 2nd: fallback -.-"
+            (TempFS, {}),
         ]
-        for fs_class, create_repo, args in options:
+        for fs_class, args in options:
             fs = fs_class()
-            repo = create_repo(fs)  # type: ignore
             try:
-                return fs, repo, self._client.fetch(self._path, repo, **args)  # type: ignore
+                return fs, self._client.clone(self._path, fs.root_path, mkdir=False, **args)  # type: ignore
             except (NotImplementedError, AssertionError) as e:
-                logging.warning("Failed to fetch into %s using %s", repo, fs_class, exc_info=e)
+                logging.warning("Failed to clone", exc_info=e)
                 fs.close()
                 continue
         raise Exception(
-            f"Failed to fetch into repo using {self._client} and {self._path}"
+            f"Failed to clone using {self._client} and {self._path}"
         )  # pragma: no cover, because this case of the workaround should never happen
```

### Comparing `fs_code-0.2/src/codefs/gitfs/opener.py` & `fs_code-0.3/src/codefs/gitfs/opener.py`

 * *Files identical despite different names*

### Comparing `fs_code-0.2/src/codefs/githubfs/__init__.py` & `fs_code-0.3/src/codefs/githubfs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,12 +129,14 @@
 class ArchiveFetcher(AbstractArchiveFetcher):
     def __init__(self, repo: Repository) -> None:
         self._repo = repo
         self._cache: Optional[bytes] = None
 
     def __call__(self, ref: str) -> FS:
         if not self._cache:
+            if ref == self.DEFAULT_BRANCH:
+                ref = self._repo.default_branch
             archive_link = self._repo.get_archive_link("zipball", ref)
             response = requests.get(archive_link)
             self._cache = response.content
         fs = ReadZipFS(BytesIO(self._cache))
         return cast(FS, fs.opendir(fs.listdir("/")[0]))
```

### Comparing `fs_code-0.2/src/codefs/githubfs/opener.py` & `fs_code-0.3/src/codefs/githubfs/opener.py`

 * *Files identical despite different names*

### Comparing `fs_code-0.2/src/codefs/gitlabfs/__init__.py` & `fs_code-0.3/src/codefs/gitlabfs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,10 +138,12 @@
 class ArchiveFetcher(AbstractArchiveFetcher):
     def __init__(self, project: Project) -> None:
         self._project = project
         self._cache: Optional[bytes] = None
 
     def __call__(self, ref: str) -> FS:
         if not self._cache:
-            self._cache = cast(bytes, self._project.repository_archive(ref, format="zip"))
+            self._cache = cast(
+                bytes, self._project.repository_archive(ref if ref != self.DEFAULT_BRANCH else None, format="zip")
+            )
         fs = ReadZipFS(BytesIO(self._cache or b""))
         return cast(FS, fs.opendir(fs.listdir("/")[0]))
```

### Comparing `fs_code-0.2/src/codefs/gitlabfs/opener.py` & `fs_code-0.3/src/codefs/gitlabfs/opener.py`

 * *Files identical despite different names*

### Comparing `fs_code-0.2/PKG-INFO` & `fs_code-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs-code
-Version: 0.2
+Version: 0.3
 Summary: PyFilesystems for GitLab, GitHub, and Git
 Home-page: https://danjou.gitlab.io/fs-code
 License: MIT
 Author: Max Ludwig
 Author-email: mail@danjou.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,21 +13,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: gitfs
 Provides-Extra: githubfs
 Provides-Extra: gitlabfs
-Requires-Dist: PyGithub (>=1.55,<2.0) ; extra == "githubfs" or extra == "all"
+Requires-Dist: PyGithub (>=1.59,<2.0) ; extra == "githubfs" or extra == "all"
 Requires-Dist: dulwich (==0.21.5) ; extra == "gitfs" or extra == "all"
 Requires-Dist: fs (>=2.4,<3.0)
-Requires-Dist: python-gitlab (>=3.0,<4.0) ; extra == "gitlabfs" or extra == "all"
-Requires-Dist: requests (>=2.26,<3.0) ; extra == "githubfs" or extra == "all"
+Requires-Dist: python-gitlab (>=3.15,<4.0) ; extra == "gitlabfs" or extra == "all"
+Requires-Dist: requests (>=2.31,<3.0) ; extra == "githubfs" or extra == "all"
 Requires-Dist: schema (>=0.7,<0.8)
-Requires-Dist: werkzeug (>=2.0,<3.0) ; extra == "gitlabfs" or extra == "githubfs" or extra == "all"
+Requires-Dist: werkzeug (>=2.3,<3.0) ; extra == "gitlabfs" or extra == "githubfs" or extra == "all"
 Project-URL: Documentation, https://danjou.gitlab.io/fs-code
 Project-URL: Repository, https://gitlab.com/dAnjou/fs-code
 Description-Content-Type: text/markdown
 
 # fs-code
 
 [![Documentation][docs badge]][docs link]
```

