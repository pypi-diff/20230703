# Comparing `tmp/aws_lambda_layer-0.2.4.tar.gz` & `tmp/aws_lambda_layer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_lambda_layer-0.2.4.tar", last modified: Sat May 27 20:03:08 2023, max compression
+gzip compressed data, was "aws_lambda_layer-0.3.1.tar", last modified: Mon Jul  3 14:43:41 2023, max compression
```

## Comparing `aws_lambda_layer-0.2.4.tar` & `aws_lambda_layer-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 20:03:08.059133 aws_lambda_layer-0.2.4/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.4/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.4/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-05-13 04:31:27.000000 aws_lambda_layer-0.2.4/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-27 20:03:08.058991 aws_lambda_layer-0.2.4/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3045 2023-05-26 18:33:40.000000 aws_lambda_layer-0.2.4/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 20:03:08.056888 aws_lambda_layer-0.2.4/aws_lambda_layer/
--rw-r--r--   0 sanhehu    (501) staff       (20)      427 2023-05-26 15:58:40.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-27 19:59:46.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      412 2023-05-27 20:00:42.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4224 2023-05-26 18:14:42.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/context.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    13795 2023-05-27 19:54:58.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/layer.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    13006 2023-05-27 19:55:28.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/source.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      184 2023-05-27 19:51:13.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 20:03:08.058397 aws_lambda_layer-0.2.4/aws_lambda_layer/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:46:28.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      650 2023-05-27 19:47:26.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/vendor/better_pathlib.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3225 2023-05-26 17:28:21.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/vendor/build_dist.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7590 2023-05-27 19:48:17.000000 aws_lambda_layer-0.2.4/aws_lambda_layer/vendor/hashes.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 20:03:08.057617 aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-27 20:03:08.000000 aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      688 2023-05-27 20:03:08.000000 aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-27 20:03:08.000000 aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      169 2023-05-27 20:03:08.000000 aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       17 2023-05-27 20:03:08.000000 aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      989 2023-05-26 20:20:04.000000 aws_lambda_layer-0.2.4/pyproject.toml
--rw-r--r--   0 sanhehu    (501) staff       (20)     2239 2023-05-27 20:01:07.000000 aws_lambda_layer-0.2.4/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.4/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       30 2023-05-16 01:23:43.000000 aws_lambda_layer-0.2.4/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-27 20:03:08.059172 aws_lambda_layer-0.2.4/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7662 2023-05-26 15:59:24.000000 aws_lambda_layer-0.2.4/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 20:03:08.058740 aws_lambda_layer-0.2.4/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      634 2023-05-27 20:02:07.000000 aws_lambda_layer-0.2.4/tests/test_import.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 14:43:41.166959 aws_lambda_layer-0.3.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 19:08:25.000000 aws_lambda_layer-0.3.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2023-05-12 19:08:25.000000 aws_lambda_layer-0.3.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-05-13 04:31:27.000000 aws_lambda_layer-0.3.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-07-03 14:43:41.166805 aws_lambda_layer-0.3.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3045 2023-05-26 18:33:40.000000 aws_lambda_layer-0.3.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 14:43:41.164663 aws_lambda_layer-0.3.1/aws_lambda_layer/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      427 2023-05-26 15:58:40.000000 aws_lambda_layer-0.3.1/aws_lambda_layer/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-03 14:41:04.000000 aws_lambda_layer-0.3.1/aws_lambda_layer/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      601 2023-07-03 14:40:36.000000 aws_lambda_layer-0.3.1/aws_lambda_layer/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4224 2023-05-26 18:14:42.000000 aws_lambda_layer-0.3.1/aws_lambda_layer/context.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    13795 2023-05-27 19:54:58.000000 aws_lambda_layer-0.3.1/aws_lambda_layer/layer.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    15937 2023-07-03 14:39:38.000000 aws_lambda_layer-0.3.1/aws_lambda_layer/source.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)        5 2023-07-03 14:11:23.000000 aws_lambda_layer-0.3.1/aws_lambda_layer/test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      184 2023-05-27 19:51:13.000000 aws_lambda_layer-0.3.1/aws_lambda_layer/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 14:43:41.166234 aws_lambda_layer-0.3.1/aws_lambda_layer/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:46:28.000000 aws_lambda_layer-0.3.1/aws_lambda_layer/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      650 2023-05-27 19:47:26.000000 aws_lambda_layer-0.3.1/aws_lambda_layer/vendor/better_pathlib.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3225 2023-05-26 17:28:21.000000 aws_lambda_layer-0.3.1/aws_lambda_layer/vendor/build_dist.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7590 2023-05-27 19:48:17.000000 aws_lambda_layer-0.3.1/aws_lambda_layer/vendor/hashes.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 14:43:41.165411 aws_lambda_layer-0.3.1/aws_lambda_layer.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-07-03 14:43:41.000000 aws_lambda_layer-0.3.1/aws_lambda_layer.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      714 2023-07-03 14:43:41.000000 aws_lambda_layer-0.3.1/aws_lambda_layer.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-03 14:43:41.000000 aws_lambda_layer-0.3.1/aws_lambda_layer.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      169 2023-07-03 14:43:41.000000 aws_lambda_layer-0.3.1/aws_lambda_layer.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       17 2023-07-03 14:43:41.000000 aws_lambda_layer-0.3.1/aws_lambda_layer.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      989 2023-05-26 20:20:04.000000 aws_lambda_layer-0.3.1/pyproject.toml
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2502 2023-07-03 14:41:57.000000 aws_lambda_layer-0.3.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-12 19:08:25.000000 aws_lambda_layer-0.3.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       30 2023-05-16 01:23:43.000000 aws_lambda_layer-0.3.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-03 14:43:41.167001 aws_lambda_layer-0.3.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7662 2023-05-26 15:59:24.000000 aws_lambda_layer-0.3.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-03 14:43:41.166512 aws_lambda_layer-0.3.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      696 2023-07-03 14:40:55.000000 aws_lambda_layer-0.3.1/tests/test_import.py
```

### Comparing `aws_lambda_layer-0.2.4/LICENSE.txt` & `aws_lambda_layer-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.4/PKG-INFO` & `aws_lambda_layer-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws_lambda_layer
-Version: 0.2.4
+Version: 0.3.1
 Summary: A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts.
 Home-page: https://github.com/MacHu-GWU/aws_lambda_layer-project
-Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.4#downloads
+Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_lambda_layer-0.2.4/README.rst` & `aws_lambda_layer-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.4/aws_lambda_layer/context.py` & `aws_lambda_layer-0.3.1/aws_lambda_layer/context.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.4/aws_lambda_layer/layer.py` & `aws_lambda_layer-0.3.1/aws_lambda_layer/layer.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.4/aws_lambda_layer/source.py` & `aws_lambda_layer-0.3.1/aws_lambda_layer/source.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,14 +72,90 @@
     before_dir = dir_extracted_folder / package_name
     after_dir = dir_deploy / package_name
     dir_deploy.mkdir(parents=True, exist_ok=True)
     shutil.rmtree(after_dir, ignore_errors=True)
     shutil.move(f"{before_dir}", f"{after_dir}")
 
 
+def do_we_include(
+    relpath: Path,
+    include: T.List[str],
+    exclude: T.List[str],
+) -> bool:
+    """
+    Based on the include and exclude pattern, do we ignore this file?
+
+    explicit exclude > explicit include > implicit include
+    """
+    if len(include) == 0 and len(exclude) == 0:
+        return True
+    elif len(include) > 0 and len(exclude) > 0:
+        match_any_include = any([relpath.match(pattern) for pattern in include])
+        match_any_exclude = any([relpath.match(pattern) for pattern in exclude])
+        if match_any_exclude:
+            return False
+        else:
+            return match_any_include
+    elif len(include) > 0 and len(exclude) == 0:
+        return any([relpath.match(pattern) for pattern in include])
+    elif len(include) == 0 and len(exclude) > 0:
+        return not any([relpath.match(pattern) for pattern in exclude])
+    else:  # pragma: no cover
+        raise NotImplementedError
+
+
+def build_source_python_lib(
+    dir_python_lib_source: T.Union[str, Path],
+    dir_python_lib_target: T.Union[str, Path],
+    include: T.Optional[T.Union[str, T.List[str]]] = None,
+    exclude: T.Optional[T.Union[str, T.List[str]]] = None,
+):
+    """
+    This function build python library source code distribution. It walks through
+    the python library source code directory, include and exclude files based on
+    definition, and copy the files to the target directory.
+
+    :param dir_python_lib_source: where your python library source code is.
+    :param dir_python_lib_target: where you want to copy the source code to.
+    :param include: list of glob patterns to include.
+    :param exclude: list of glob patterns to exclude.
+    """
+    dir_python_lib_source = Path(dir_python_lib_source).absolute()
+    dir_python_lib_target = Path(dir_python_lib_target).absolute()
+    if include is None:  # pragma: no cover
+        include = []
+    elif isinstance(include, str):  # pragma: no cover
+        include = [include]
+    else:  # pragma: no cover
+        include = include
+    if exclude is None:  # pragma: no cover
+        exclude = []
+    elif isinstance(exclude, str):  # pragma: no cover
+        exclude = [exclude]
+    else:  # pragma: no cover
+        exclude = exclude
+    exclude.extend(["__pycache__", "*.pyc", "*.pyo"])
+
+    if dir_python_lib_target.exists():
+        shutil.rmtree(dir_python_lib_target)
+
+    for path in dir_python_lib_source.glob("**/*"):
+        if path.is_file():
+            relpath = path.relative_to(dir_python_lib_source)
+            if do_we_include(relpath, include=include, exclude=exclude):
+                path_new = dir_python_lib_target.joinpath(relpath)
+                try:
+                    path_new.write_bytes(path.read_bytes())
+                except FileNotFoundError:
+                    path_new.parent.mkdir(parents=True, exist_ok=True)
+                    path_new.write_bytes(path.read_bytes())
+        else:
+            pass
+
+
 def build_source_artifacts(
     path_setup_py_or_pyproject_toml: T.Union[str, Path],
     package_name: str,
     path_lambda_function: T.Union[str, Path],
     dir_build: T.Union[str, Path],
     path_bin_python: T.Optional[T.Union[str, Path]] = None,
     path_bin_poetry: T.Optional[T.Union[str, Path]] = None,
@@ -270,14 +346,15 @@
     """
     Source artifacts deployment information.
 
     :param source_sha256: code sha256 hash of the source artifacts
     :param path_source_zip: path to the source.zip file on local
     :param s3path_source_zip: S3Path object of the source.zip file
     """
+
     source_sha256: str = dataclasses.field()
     path_source_zip: Path = dataclasses.field()
     s3path_source_zip: S3Path = dataclasses.field()
 
 
 def publish_source_artifacts(
     bsm: "BotoSesManager",
```

### Comparing `aws_lambda_layer-0.2.4/aws_lambda_layer/vendor/better_pathlib.py` & `aws_lambda_layer-0.3.1/aws_lambda_layer/vendor/better_pathlib.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.4/aws_lambda_layer/vendor/build_dist.py` & `aws_lambda_layer-0.3.1/aws_lambda_layer/vendor/build_dist.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.4/aws_lambda_layer/vendor/hashes.py` & `aws_lambda_layer-0.3.1/aws_lambda_layer/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/PKG-INFO` & `aws_lambda_layer-0.3.1/aws_lambda_layer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws-lambda-layer
-Version: 0.2.4
+Version: 0.3.1
 Summary: A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts.
 Home-page: https://github.com/MacHu-GWU/aws_lambda_layer-project
-Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.4#downloads
+Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_lambda_layer-0.2.4/aws_lambda_layer.egg-info/SOURCES.txt` & `aws_lambda_layer-0.3.1/aws_lambda_layer.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 setup.py
 aws_lambda_layer/__init__.py
 aws_lambda_layer/_version.py
 aws_lambda_layer/api.py
 aws_lambda_layer/context.py
 aws_lambda_layer/layer.py
 aws_lambda_layer/source.py
+aws_lambda_layer/test.txt
 aws_lambda_layer/utils.py
 aws_lambda_layer.egg-info/PKG-INFO
 aws_lambda_layer.egg-info/SOURCES.txt
 aws_lambda_layer.egg-info/dependency_links.txt
 aws_lambda_layer.egg-info/requires.txt
 aws_lambda_layer.egg-info/top_level.txt
 aws_lambda_layer/vendor/__init__.py
```

### Comparing `aws_lambda_layer-0.2.4/pyproject.toml` & `aws_lambda_layer-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.4/release-history.rst` & `aws_lambda_layer-0.3.1/release-history.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.1 (2023-07-03)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add the following public api:
+    - ``aws_lambda_layer.api.do_we_include``
+    - ``aws_lambda_layer.api.build_source_python_lib``
+
+
 0.2.4 (2023-05-27)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Minor Improvements**
 
 - now the ``deploy_layer`` method returns a ``LayerDeployment`` object.
 - now the ``publish_source_artifacts`` method returns a ``SourceArtifactsDeployment`` object.
```

### Comparing `aws_lambda_layer-0.2.4/setup.py` & `aws_lambda_layer-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.4/tests/test_import.py` & `aws_lambda_layer-0.3.1/tests/test_import.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     _ = api.get_latest_layer_version
     _ = api.is_current_layer_the_same_as_latest_one
     _ = api.build_layer_artifacts
     _ = api.upload_layer_artifacts
     _ = api.publish_layer
     _ = api.deploy_layer
     _ = api.LayerDeployment
+    _ = api.do_we_include
+    _ = api.build_source_python_lib
     _ = api.build_source_artifacts
     _ = api.upload_source_artifacts
     _ = api.publish_source_artifacts
     _ = api.SourceArtifactsDeployment
 
 
 if __name__ == "__main__":
```

