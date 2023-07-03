# Comparing `tmp/mgmt-0.6.0.tar.gz` & `tmp/mgmt-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgmt-0.6.0.tar", max compression
+gzip compressed data, was "mgmt-0.6.1.tar", max compression
```

## Comparing `mgmt-0.6.0.tar` & `mgmt-0.6.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-07-01 10:53:14.039322 mgmt-0.6.0/LICENSE
--rw-r--r--   0        0        0     3511 2023-07-01 10:53:14.039322 mgmt-0.6.0/README.md
--rw-r--r--   0        0        0     1156 2023-07-01 10:53:14.039322 mgmt-0.6.0/mgmt/__init__.py
--rw-r--r--   0        0        0       44 2023-07-01 10:53:14.039322 mgmt-0.6.0/mgmt/__main__.py
--rw-r--r--   0        0        0     6751 2023-07-01 10:53:14.039322 mgmt-0.6.0/mgmt/app.py
--rw-r--r--   0        0        0     6090 2023-07-01 10:53:14.039322 mgmt-0.6.0/mgmt/aws.py
--rw-r--r--   0        0        0     1763 2023-07-01 10:53:14.043322 mgmt-0.6.0/mgmt/config.py
--rw-r--r--   0        0        0     2945 2023-07-01 10:53:14.043322 mgmt-0.6.0/mgmt/files.py
--rw-r--r--   0        0        0      957 2023-07-01 10:53:14.043322 mgmt-0.6.0/mgmt/log.py
--rw-r--r--   0        0        0     2276 2023-07-01 10:53:14.043322 mgmt-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4990 1970-01-01 00:00:00.000000 mgmt-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-03 05:37:03.674832 mgmt-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3511 2023-07-03 05:37:03.674832 mgmt-0.6.1/README.md
+-rw-r--r--   0        0        0     1156 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/__init__.py
+-rw-r--r--   0        0        0       44 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/__main__.py
+-rw-r--r--   0        0        0     6721 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/app.py
+-rw-r--r--   0        0        0     6652 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/aws.py
+-rw-r--r--   0        0        0     1763 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/config.py
+-rw-r--r--   0        0        0     2945 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/files.py
+-rw-r--r--   0        0        0     1648 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/log.py
+-rw-r--r--   0        0        0      656 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/utils.py
+-rw-r--r--   0        0        0     2276 2023-07-03 05:37:03.674832 mgmt-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4990 1970-01-01 00:00:00.000000 mgmt-0.6.1/PKG-INFO
```

### Comparing `mgmt-0.6.0/LICENSE` & `mgmt-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mgmt-0.6.0/README.md` & `mgmt-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mgmt-0.6.0/mgmt/__init__.py` & `mgmt-0.6.1/mgmt/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .app import entry_point as cli  # noqa: F401
 from .aws import AwsStorageMgmt
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 __docformat__ = "restructuredtext"
 
 """
 As per PEP 287, example:
 
 This is a reST style.
```

### Comparing `mgmt-0.6.0/mgmt/app.py` & `mgmt-0.6.1/mgmt/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,53 +7,37 @@
 from typer import echo
 from rich.table import Table
 from rich.console import Console
 
 from mgmt.aws import AwsStorageMgmt
 from mgmt.log import Log
 from mgmt.files import FileManager
+from mgmt.utils import check_selection
 from mgmt.config import Config
 
 app = typer.Typer(add_completion=False)
 aws = AwsStorageMgmt()
 logger = Log(debug=False)
 file_mgmt = FileManager()
 
 
-def echo_dict(input_dict: dict) -> None:
-    """
-    Prints a dictionary with its keys and values
-
-    Args:
-        input_dict (dict): The dictionary to be printed.
-    """
-    for key, val in input_dict.items():
-        echo(f"{key[:18]+'..' if len(key)>17 else key}{(20-int(len(key)))*'.'}{val}")
-
-
 @app.command()
 def upload(filename: str, compression: Optional[str] = "gzip") -> None:
     """
     Uploads the specified file to S3
 
     Args:
         filename (str): The name of the file or directory to upload. Use 'all' to upload all files in the directory.
         compression (Optional[str]): The compression algorithm to use. Defaults to 'gzip'.
     """
     target = filename
     cwd = Path(".").resolve()
     target_path = cwd / target
-    # localfiles = os.listdir(p)
     files_created = []
 
-    # if not target:
-    #     echo("invalid target command")
-    #     return
-    # print(str(target_path)," in ",str(os.listdir(cwd)))
-
     try:
         if target == "all":
             echo("uploading all media objects to S3")
             for _file_or_dir in cwd.iterdir():
                 echo()
                 echo("compressing...")
                 echo(str(_file_or_dir))
@@ -68,14 +52,15 @@
             return False
     except Exception as e:
         logger.error(f"An error occurred while uploading: {e}")
     finally:
         if files_created:
             for file in files_created:
                 os.remove(file)
+    return
 
 
 @app.command()
 def search(keyword: str, location: Optional[str] = "global") -> None:
     """
     Searches for files that contain the specified keyword in their names
 
@@ -96,61 +81,78 @@
 
         console = Console()
         table = Table(title="AWS S3 Search Matches")
         table.add_column("Option #")
         table.add_column("Storage Tier")
         table.add_column("Last Modified")
         table.add_column("Object Key")
+        table.add_column("Restored Status")
         doptions = {}
         for i, file_name in enumerate(s3_matches):
             try:
                 resp = aws.get_obj_head(file_name)
                 storage_class = resp.get("StorageClass", "STANDARD")
                 last_modified = resp.get("LastModified", "")
-                table.add_row(storage_class, str(last_modified), file_name)
+                restored_status = resp.get("Restore")
+                if restored_status:
+                    restored_status = str(restored_status).split("expiry-date=")[-1].replace('"', "")
+                table.add_row(str(i), storage_class, str(last_modified), file_name, str(restored_status))
                 doptions[i] = file_name
             except Exception as e:
                 logger.error(f"An error occurred while getting metadata: {e}")
 
         console.print(table)
         if not typer.confirm("Download?", default=False):
             echo("Aborted.")
-            return
         else:
             resp = typer.prompt("Which file? [option #]", type=int)
-            aws.download_file(doptions[resp])
-            return
-    else:
-        echo("no matches found\n")
-        return
+            if check_selection(resp, list(doptions)):
+                aws.download_file(object_name=doptions[resp])
+                return
+            else:
+                return
+
+        if not typer.confirm("Check Status?", default=False):
+            echo("Aborted.")
+        else:
+            resp = typer.prompt("Which file? [option #]", type=int)
+            if check_selection(resp, list(doptions)):
+                aws.get_obj_head(object_name=doptions[resp])
+                echo(json.dumps(aws.obj_head, indent=4, sort_keys=True, default=str))
+                return
+            else:
+                return
+    return
 
 
 @app.command()
 def download(filename: str, bucket_name: Optional[str] = None) -> None:
     """
     Downloads the specified file from S3
 
     Args:
         filename (str): The name of the file to download.
         bucket_name (Optional[str]): The name of the bucket from which to download the file. If not provided, the default bucket is used.
     """
     echo(f"Downloading {filename} from S3...")
     aws.download_file(object_name=filename, bucket_name=bucket_name)
+    return
 
 
 @app.command()
 def status(filename: str) -> None:
     """
     Retrieves and prints the metadata of the specified file
 
     Args:
         filename (str): The name of the file to get the metadata for.
     """
     aws.get_obj_head(object_name=filename)
     echo(json.dumps(aws.obj_head, indent=4, sort_keys=True, default=str))
+    return
 
 
 @app.command()
 def delete(filename: str) -> None:
     """
     Deletes the specified file from S3; requires confirmation
 
@@ -164,40 +166,31 @@
         return
     else:
         try:
             aws.delete_file(filename)
             echo(f"{filename} successfully deleted from S3")
         except Exception as e:
             logger.error(f"An error occurred while deleting {filename}: {e}")
+    return
 
 
 @app.command()
-def list(location: Optional[str] = "global", bucket_name: Optional[str] = None) -> None:
+def ls(location: Optional[str] = "global") -> None:
     """
     Lists the files in the specified location
 
     Args:
         location (Optional[str]): The location to list files in. Defaults to 'global'.
         bucket_name (Optional[str]): The name of the bucket to list files in. If not provided, the default bucket is used.
     """
-    if bucket_name:
-        files = aws.get_bucket_obj_keys(bucket_name=bucket_name)
-    else:
-        if location in ("local", "s3", "global"):
-            if location == "global":
-                local_files, s3_keys = aws.get_files(location=location)
-                files = local_files + s3_keys
-        elif location == "here":
-            p = Path(".")
-            files = os.listdir(p)
-        else:
-            echo(f"invalid location input: {location}")
-
-    for file in files:
-        echo(file)
+    local_files, s3_keys = aws.get_files(location=location)
+    obj_list = local_files + s3_keys
+    for obj in obj_list:
+        echo(obj)
+    return
 
 
 @app.command()
 def config() -> None:
     """
     Configures the application
     """
```

### Comparing `mgmt-0.6.0/mgmt/aws.py` & `mgmt-0.6.1/mgmt/aws.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from time import sleep
+from pathlib import Path
 
 import boto3
 from botocore.exceptions import ClientError
 
 from mgmt.log import Log
 from mgmt.files import FileManager
 from mgmt.config import Config
@@ -11,15 +12,15 @@
 
 class AwsStorageMgmt:
     def __init__(self):
         self.s3_resource = boto3.resource("s3")
         self.s3_client = boto3.client("s3")
         self.config = Config()
         self.load_config_file()
-        self.logger = Log(debug=False)
+        self.logger = Log(debug=True)
 
     def load_config_file(self):
         if self.config.check_exists():
             self.configs = self.config.get_configs()
             self.bucket = self.configs.get("BUCKET")
             self.object_prefix = self.configs.get("OBJECT_PREFIX")
             self.local_dir = self.configs.get("LOCAL_DIR")
@@ -42,15 +43,15 @@
             self.logger.error(e)
             return False
         return True
 
     def download_file(self, object_name: str, bucket_name: str = None) -> bool:
         if not bucket_name:
             bucket_name = self.bucket
-        self.logger.debug(f"Downloading `{object_name}` from `{bucket_name}`")
+        self.logger.info(f"Downloading `{object_name}` from `{bucket_name}`")
         file_name = object_name.split("/")[-1]
         try:
             with open(file_name, "wb") as data:
                 self.s3_client.download_fileobj(bucket_name, object_name, data)
         except ClientError as e:
             self.logger.error(f"-- ClientError --\n{str(e)}")
             os.remove(file_name)
@@ -69,14 +70,15 @@
         return [obj.key for obj in self.get_bucket_objs()]
 
     def get_obj_head(self, object_name: str):
         response = self.s3_client.head_object(
             Bucket=self.bucket,
             Key=object_name,
         )
+        self.obj_head = response
         return response
 
     def get_obj_restore_status(self, object_name):
         response = self.get_obj_head(object_name)
         try:
             resp_string = response["Restore"]
             self.logger.debug(resp_string)
@@ -155,7 +157,21 @@
             return self.get_bucket_obj_keys()
         elif location == "global" and self.local_dir:
             return self.file_mgmt.files_in_media_dir(), self.get_bucket_obj_keys()
         else:
             self.logger.error("invalid location")
             self.logger.error(self.local_dir)
             return False
+
+    def list_func(self, location: str):
+        file_list = []
+        if location in ("local", "s3", "global"):
+            if location == "global":
+                local_files, s3_keys = self.get_files(location=location)
+                file_list = local_files + s3_keys
+        elif location == "here":
+            p = Path(".")
+            file_list = os.listdir(p)
+        else:
+            self.logger.error("invalid location input")
+            self.logger.error(location)
+        return file_list
```

### Comparing `mgmt-0.6.0/mgmt/config.py` & `mgmt-0.6.1/mgmt/config.py`

 * *Files identical despite different names*

### Comparing `mgmt-0.6.0/mgmt/files.py` & `mgmt-0.6.1/mgmt/files.py`

 * *Files identical despite different names*

### Comparing `mgmt-0.6.0/pyproject.toml` & `mgmt-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "mgmt"
-version = "0.6.0"
+version = "0.6.1"
 description = ""
 readme = "README.md"
 authors = ["Will Wright <willwright@example.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/will-wright-eng/media-mgmt-cli"
 homepage = "https://github.com/will-wright-eng/media-mgmt-cli"
```

### Comparing `mgmt-0.6.0/PKG-INFO` & `mgmt-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgmt
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 Home-page: https://github.com/will-wright-eng/media-mgmt-cli
 License: GNU GPL v3.0
 Author: Will Wright
 Author-email: willwright@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

