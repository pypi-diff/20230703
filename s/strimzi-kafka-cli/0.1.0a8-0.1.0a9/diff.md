# Comparing `tmp/strimzi-kafka-cli-0.1.0a8.tar.gz` & `tmp/strimzi-kafka-cli-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/strimzi-kafka-cli-0.1.0a8.tar", last modified: Fri Jun 12 08:36:18 2020, max compression
+gzip compressed data, was "dist/strimzi-kafka-cli-0.1.0a9.tar", last modified: Fri Jun 12 10:14:07 2020, max compression
```

## Comparing `strimzi-kafka-cli-0.1.0a8.tar` & `strimzi-kafka-cli-0.1.0a9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 08:36:18.697929 strimzi-kafka-cli-0.1.0a8/
--rw-r--r--   0 runner    (1001) docker     (116)     2984 2020-06-12 08:36:18.697929 strimzi-kafka-cli-0.1.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2270 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 08:36:18.693929 strimzi-kafka-cli-0.1.0a8/kfk/
--rw-r--r--   0 runner    (1001) docker     (116)     1332 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/kfk/clusters_command.py
--rw-r--r--   0 runner    (1001) docker     (116)      221 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/kfk/command.py
--rw-r--r--   0 runner    (1001) docker     (116)     1782 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/kfk/commons.py
--rw-r--r--   0 runner    (1001) docker     (116)      159 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/kfk/configs_command.py
--rw-r--r--   0 runner    (1001) docker     (116)     1663 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/kfk/console_command.py
--rw-r--r--   0 runner    (1001) docker     (116)      800 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/kfk/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)     1499 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/kfk/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (116)     1956 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/kfk/kubectl_command_builder.py
--rw-r--r--   0 runner    (1001) docker     (116)      251 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/kfk/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     1848 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/kfk/option_extensions.py
--rw-r--r--   0 runner    (1001) docker     (116)     5447 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/kfk/topics_command.py
--rw-r--r--   0 runner    (1001) docker     (116)     4364 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/kfk/users_command.py
--rw-r--r--   0 runner    (1001) docker     (116)      647 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/kfk/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-06-12 08:36:18.697929 strimzi-kafka-cli-0.1.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      639 2020-06-12 08:36:07.000000 strimzi-kafka-cli-0.1.0a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 08:36:18.697929 strimzi-kafka-cli-0.1.0a8/strimzi_kafka_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2984 2020-06-12 08:36:18.000000 strimzi-kafka-cli-0.1.0a8/strimzi_kafka_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      527 2020-06-12 08:36:18.000000 strimzi-kafka-cli-0.1.0a8/strimzi_kafka_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-12 08:36:18.000000 strimzi-kafka-cli-0.1.0a8/strimzi_kafka_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       56 2020-06-12 08:36:18.000000 strimzi-kafka-cli-0.1.0a8/strimzi_kafka_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       18 2020-06-12 08:36:18.000000 strimzi-kafka-cli-0.1.0a8/strimzi_kafka_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        4 2020-06-12 08:36:18.000000 strimzi-kafka-cli-0.1.0a8/strimzi_kafka_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 10:14:07.220861 strimzi-kafka-cli-0.1.0a9/
+-rw-r--r--   0 runner    (1001) docker     (116)     2984 2020-06-12 10:14:07.220861 strimzi-kafka-cli-0.1.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2270 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 10:14:07.220861 strimzi-kafka-cli-0.1.0a9/kfk/
+-rw-r--r--   0 runner    (1001) docker     (116)     1332 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/kfk/clusters_command.py
+-rw-r--r--   0 runner    (1001) docker     (116)      221 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/kfk/command.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1859 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/kfk/commons.py
+-rw-r--r--   0 runner    (1001) docker     (116)      159 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/kfk/configs_command.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1663 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/kfk/console_command.py
+-rw-r--r--   0 runner    (1001) docker     (116)      800 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/kfk/constants.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1499 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/kfk/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1956 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/kfk/kubectl_command_builder.py
+-rw-r--r--   0 runner    (1001) docker     (116)      251 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/kfk/main.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1848 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/kfk/option_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5447 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/kfk/topics_command.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4364 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/kfk/users_command.py
+-rw-r--r--   0 runner    (1001) docker     (116)      647 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/kfk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-06-12 10:14:07.220861 strimzi-kafka-cli-0.1.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      639 2020-06-12 10:13:58.000000 strimzi-kafka-cli-0.1.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-12 10:14:07.220861 strimzi-kafka-cli-0.1.0a9/strimzi_kafka_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     2984 2020-06-12 10:14:07.000000 strimzi-kafka-cli-0.1.0a9/strimzi_kafka_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      527 2020-06-12 10:14:07.000000 strimzi-kafka-cli-0.1.0a9/strimzi_kafka_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-12 10:14:07.000000 strimzi-kafka-cli-0.1.0a9/strimzi_kafka_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       56 2020-06-12 10:14:07.000000 strimzi-kafka-cli-0.1.0a9/strimzi_kafka_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       18 2020-06-12 10:14:07.000000 strimzi-kafka-cli-0.1.0a9/strimzi_kafka_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        4 2020-06-12 10:14:07.000000 strimzi-kafka-cli-0.1.0a9/strimzi_kafka_cli.egg-info/top_level.txt
```

### Comparing `strimzi-kafka-cli-0.1.0a8/PKG-INFO` & `strimzi-kafka-cli-0.1.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strimzi-kafka-cli
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: Command Line Interface for Strimzi Kafka Operator
 Home-page: https://github.com/systemcraftsman/strimzi-kafka-cli
 License: UNKNOWN
 Description: ![badge](https://github.com/systemcraftsman/strimzi-kafka-cli/workflows/Build/badge.svg) ![badge](https://github.com/systemcraftsman/strimzi-kafka-cli/workflows/Deploy/badge.svg)
         
         ![strimzi cli](https://raw.githubusercontent.com/systemcraftsman/strimzi-kafka-cli/master/documentation/logo/strimzi_cli.png)
```

### Comparing `strimzi-kafka-cli-0.1.0a8/README.md` & `strimzi-kafka-cli-0.1.0a9/README.md`

 * *Files identical despite different names*

### Comparing `strimzi-kafka-cli-0.1.0a8/kfk/clusters_command.py` & `strimzi-kafka-cli-0.1.0a9/kfk/clusters_command.py`

 * *Files identical despite different names*

### Comparing `strimzi-kafka-cli-0.1.0a8/kfk/commons.py` & `strimzi-kafka-cli-0.1.0a9/kfk/commons.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,8 +44,9 @@
 def get_resource_yaml(resource_type, resource_name, namespace):
     return os.popen(
         Kubectl().get().resource(resource_type, resource_name).namespace(namespace).output("yaml").build()).read()
 
 
 def get_resource_as_file(resource_type, resource_name, namespace):
     topic_yaml = get_resource_yaml(resource_type, resource_name, namespace)
-    return io.StringIO(topic_yaml)
+    in_stream = io.BytesIO(topic_yaml.encode('utf-8'))
+    return io.TextIOWrapper(in_stream, encoding='utf-8')
```

### Comparing `strimzi-kafka-cli-0.1.0a8/kfk/console_command.py` & `strimzi-kafka-cli-0.1.0a9/kfk/console_command.py`

 * *Files identical despite different names*

### Comparing `strimzi-kafka-cli-0.1.0a8/kfk/constants.py` & `strimzi-kafka-cli-0.1.0a9/kfk/constants.py`

 * *Files identical despite different names*

### Comparing `strimzi-kafka-cli-0.1.0a8/kfk/dependencies.py` & `strimzi-kafka-cli-0.1.0a9/kfk/dependencies.py`

 * *Files identical despite different names*

### Comparing `strimzi-kafka-cli-0.1.0a8/kfk/kubectl_command_builder.py` & `strimzi-kafka-cli-0.1.0a9/kfk/kubectl_command_builder.py`

 * *Files identical despite different names*

### Comparing `strimzi-kafka-cli-0.1.0a8/kfk/option_extensions.py` & `strimzi-kafka-cli-0.1.0a9/kfk/option_extensions.py`

 * *Files identical despite different names*

### Comparing `strimzi-kafka-cli-0.1.0a8/kfk/topics_command.py` & `strimzi-kafka-cli-0.1.0a9/kfk/topics_command.py`

 * *Files identical despite different names*

### Comparing `strimzi-kafka-cli-0.1.0a8/kfk/users_command.py` & `strimzi-kafka-cli-0.1.0a9/kfk/users_command.py`

 * *Files identical despite different names*

### Comparing `strimzi-kafka-cli-0.1.0a8/kfk/utils.py` & `strimzi-kafka-cli-0.1.0a9/kfk/utils.py`

 * *Files identical despite different names*

### Comparing `strimzi-kafka-cli-0.1.0a8/setup.py` & `strimzi-kafka-cli-0.1.0a9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name='strimzi-kafka-cli',
-    version='0.1.0-alpha8',
+    version='0.1.0-alpha9',
     description="Command Line Interface for Strimzi Kafka Operator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['kfk'],
     package_dir={'kfk': 'kfk'},
     install_requires=[
         'Click',
```

### Comparing `strimzi-kafka-cli-0.1.0a8/strimzi_kafka_cli.egg-info/PKG-INFO` & `strimzi-kafka-cli-0.1.0a9/strimzi_kafka_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strimzi-kafka-cli
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: Command Line Interface for Strimzi Kafka Operator
 Home-page: https://github.com/systemcraftsman/strimzi-kafka-cli
 License: UNKNOWN
 Description: ![badge](https://github.com/systemcraftsman/strimzi-kafka-cli/workflows/Build/badge.svg) ![badge](https://github.com/systemcraftsman/strimzi-kafka-cli/workflows/Deploy/badge.svg)
         
         ![strimzi cli](https://raw.githubusercontent.com/systemcraftsman/strimzi-kafka-cli/master/documentation/logo/strimzi_cli.png)
```

### Comparing `strimzi-kafka-cli-0.1.0a8/strimzi_kafka_cli.egg-info/SOURCES.txt` & `strimzi-kafka-cli-0.1.0a9/strimzi_kafka_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

