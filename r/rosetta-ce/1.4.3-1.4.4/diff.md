# Comparing `tmp/rosetta-ce-1.4.3.tar.gz` & `tmp/rosetta-ce-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.4.3.tar", last modified: Sun Jul  2 18:04:26 2023, max compression
+gzip compressed data, was "rosetta-ce-1.4.4.tar", last modified: Mon Jul  3 09:26:02 2023, max compression
```

## Comparing `rosetta-ce-1.4.3.tar` & `rosetta-ce-1.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 18:04:26.976531 rosetta-ce-1.4.3/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.4.3/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 18:04:26.976226 rosetta-ce-1.4.3/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.4.3/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 18:04:26.970011 rosetta-ce-1.4.3/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.4.3/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 18:04:26.971899 rosetta-ce-1.4.3/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.4.3/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.4.3/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.4.3/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.4.3/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.4.3/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    43848 2023-07-02 18:03:11.000000 rosetta-ce-1.4.3/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.4.3/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 18:04:26.974039 rosetta-ce-1.4.3/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 18:04:26.000000 rosetta-ce-1.4.3/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-02 18:04:26.000000 rosetta-ce-1.4.3/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-02 18:04:26.000000 rosetta-ce-1.4.3/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-02 18:04:26.000000 rosetta-ce-1.4.3/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-02 18:04:26.000000 rosetta-ce-1.4.3/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-02 18:04:26.976569 rosetta-ce-1.4.3/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-02 18:03:11.000000 rosetta-ce-1.4.3/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 18:04:26.975745 rosetta-ce-1.4.3/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.4.3/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.4.3/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.4.3/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:26:02.558709 rosetta-ce-1.4.4/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.4.4/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-03 09:26:02.558372 rosetta-ce-1.4.4/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.4.4/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:26:02.552339 rosetta-ce-1.4.4/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.4.4/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:26:02.554112 rosetta-ce-1.4.4/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.4.4/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.4.4/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.4.4/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.4.4/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.4.4/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    43851 2023-07-03 09:25:12.000000 rosetta-ce-1.4.4/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.4.4/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:26:02.556280 rosetta-ce-1.4.4/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-03 09:26:02.000000 rosetta-ce-1.4.4/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-03 09:26:02.000000 rosetta-ce-1.4.4/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-03 09:26:02.000000 rosetta-ce-1.4.4/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-03 09:26:02.000000 rosetta-ce-1.4.4/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-03 09:26:02.000000 rosetta-ce-1.4.4/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-03 09:26:02.558753 rosetta-ce-1.4.4/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-03 09:25:25.000000 rosetta-ce-1.4.4/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:26:02.557809 rosetta-ce-1.4.4/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.4.4/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.4.4/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.4.4/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.4.3/LICENSE` & `rosetta-ce-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.3/PKG-INFO` & `rosetta-ce-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.4.3
+Version: 1.4.4
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.4.3/README.md` & `rosetta-ce-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.3/rosetta/constants/sensors.py` & `rosetta-ce-1.4.4/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.3/rosetta/constants/sources.py` & `rosetta-ce-1.4.4/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.3/rosetta/constants/systems.py` & `rosetta-ce-1.4.4/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.3/rosetta/rconverter.py` & `rosetta-ce-1.4.4/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.3/rosetta/rfaker.py` & `rosetta-ce-1.4.4/rosetta/rfaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         if field == "local_ip":
             field_value = random.choice(observables.local_ip) if observables and observables.local_ip \
                     else faker.ipv4()
         if field == "local_port":
             field_value = faker.random_int(min=1024, max=65535)
         if field == "remote_ip":
             field_value = random.choice(observables.remote_ip) if observables and observables.remote_ip \
-                    else Observables.generator(observable_type=ObservableType.IP, known=ObservableKnown.BAD, count=1)
+                    else Observables.generator(observable_type=ObservableType.IP, known=ObservableKnown.BAD, count=1)[0]
         if field == "remote_port":
             field_value = random.choice(observables.remote_port) if observables and observables.remote_port \
                     else faker.random_int(min=1024, max=65535)
         if field == "dst_url":
             field_value = random.choice(observables.url) if observables and observables.url \
                     else Observables.generator(observable_type=ObservableType.URL, known=ObservableKnown.BAD, count=1)
         if field == "inbound_bytes":
```

### Comparing `rosetta-ce-1.4.3/rosetta/rsender.py` & `rosetta-ce-1.4.4/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.3/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.4.4/rosetta_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.4.3
+Version: 1.4.4
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.4.3/setup.py` & `rosetta-ce-1.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.4.3",
+    version="1.4.4",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.4.3/tests/test_rconverter.py` & `rosetta-ce-1.4.4/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.3/tests/test_rfaker.py` & `rosetta-ce-1.4.4/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.3/tests/test_rsender.py` & `rosetta-ce-1.4.4/tests/test_rsender.py`

 * *Files identical despite different names*

