# Comparing `tmp/spark_quality_rules_tools-0.4.2.tar.gz` & `tmp/spark_quality_rules_tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.4.2.tar", last modified: Sun Jul  2 06:29:00 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.5.0.tar", last modified: Mon Jul  3 14:59:55 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.4.2.tar` & `spark_quality_rules_tools-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 06:29:00.056382 spark_quality_rules_tools-0.4.2/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.4.2/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-07-02 06:29:00.056382 spark_quality_rules_tools-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.4.2/README.md
--rw-rw-rw-   0        0        0      685 2023-07-01 22:58:24.000000 spark_quality_rules_tools-0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-02 06:29:00.056382 spark_quality_rules_tools-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-07-02 06:28:45.000000 spark_quality_rules_tools-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 06:29:00.040756 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2550 2023-07-02 03:08:37.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 06:29:00.056382 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    49594 2023-07-02 06:28:45.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-02 06:29:00.056382 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-07-02 06:29:00.056382 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/utils/resource/resolve_edge.conf
--rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
--rw-rw-rw-   0        0        0    25817 2023-07-02 01:22:13.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-07-02 06:29:00.040756 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-07-02 06:29:00.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-07-02 06:29:00.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 06:29:00.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-02 06:29:00.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-02 06:29:00.000000 spark_quality_rules_tools-0.4.2/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 14:59:55.784552 spark_quality_rules_tools-0.5.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-07-03 14:59:55.785553 spark_quality_rules_tools-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.5.0/README.md
+-rw-rw-rw-   0        0        0      685 2023-07-01 22:58:24.000000 spark_quality_rules_tools-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-03 14:59:55.786553 spark_quality_rules_tools-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-03 14:59:45.000000 spark_quality_rules_tools-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:59:55.732541 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2550 2023-07-02 03:08:37.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:59:55.756546 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    49664 2023-07-03 14:59:45.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:59:55.775551 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:59:55.784552 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    25817 2023-07-02 01:22:13.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:59:55.755546 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-07-03 14:59:55.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-07-03 14:59:55.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 14:59:55.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-03 14:59:55.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-03 14:59:55.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.4.2/LICENSE` & `spark_quality_rules_tools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.4.2/PKG-INFO` & `spark_quality_rules_tools-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.4.2
+Version: 0.5.0
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.4.2/README.md` & `spark_quality_rules_tools-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.4.2/pyproject.toml` & `spark_quality_rules_tools-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.4.2/setup.py` & `spark_quality_rules_tools-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.4.2',
+    version='0.5.0',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/functions/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -980,14 +980,15 @@
     uuaa_name = str(table_name.split("_")[1]).upper()
     json_resource_rules = os.path.join(BASE_DIR, "utils", "resource", "rules.json")
     dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{table_name}_{rule_id}_generated.conf")
 
     if is_windows:
         json_resource_rules = json_resource_rules.replace("\\", "/")
         dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
+    os.makedirs(os.path.dirname(dir_hocons_filename), exist_ok=True)
 
     with open(json_resource_rules) as f:
         default_rules = json.load(f)
     rules_config = default_rules.get("rules_config", None)
     hamu_dict = dict()
     rs_list = list()
     rs_dict = dict()
```

### Comparing `spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/utils/resource/resolve_edge.conf` & `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf` & `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.4.2/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.4.2/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.4.2
+Version: 0.5.0
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.4.2/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

