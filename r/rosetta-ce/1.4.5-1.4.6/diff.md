# Comparing `tmp/rosetta-ce-1.4.5.tar.gz` & `tmp/rosetta-ce-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.4.5.tar", last modified: Mon Jul  3 09:36:35 2023, max compression
+gzip compressed data, was "rosetta-ce-1.4.6.tar", last modified: Mon Jul  3 09:41:03 2023, max compression
```

## Comparing `rosetta-ce-1.4.5.tar` & `rosetta-ce-1.4.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:36:35.517491 rosetta-ce-1.4.5/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.4.5/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-03 09:36:35.517140 rosetta-ce-1.4.5/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.4.5/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:36:35.511053 rosetta-ce-1.4.5/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.4.5/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:36:35.512855 rosetta-ce-1.4.5/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.4.5/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.4.5/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.4.5/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.4.5/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.4.5/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    44026 2023-07-03 09:35:55.000000 rosetta-ce-1.4.5/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.4.5/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:36:35.515113 rosetta-ce-1.4.5/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-03 09:36:35.000000 rosetta-ce-1.4.5/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-03 09:36:35.000000 rosetta-ce-1.4.5/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-03 09:36:35.000000 rosetta-ce-1.4.5/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-03 09:36:35.000000 rosetta-ce-1.4.5/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-03 09:36:35.000000 rosetta-ce-1.4.5/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-03 09:36:35.517540 rosetta-ce-1.4.5/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-03 09:36:07.000000 rosetta-ce-1.4.5/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:36:35.516606 rosetta-ce-1.4.5/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.4.5/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.4.5/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.4.5/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:41:03.988906 rosetta-ce-1.4.6/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.4.6/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-03 09:41:03.988563 rosetta-ce-1.4.6/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.4.6/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:41:03.981701 rosetta-ce-1.4.6/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.4.6/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:41:03.984039 rosetta-ce-1.4.6/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.4.6/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.4.6/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.4.6/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.4.6/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.4.6/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    44071 2023-07-03 09:40:20.000000 rosetta-ce-1.4.6/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.4.6/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:41:03.986444 rosetta-ce-1.4.6/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-03 09:41:03.000000 rosetta-ce-1.4.6/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-03 09:41:03.000000 rosetta-ce-1.4.6/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-03 09:41:03.000000 rosetta-ce-1.4.6/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-03 09:41:03.000000 rosetta-ce-1.4.6/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-03 09:41:03.000000 rosetta-ce-1.4.6/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-03 09:41:03.988947 rosetta-ce-1.4.6/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-03 09:40:26.000000 rosetta-ce-1.4.6/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-03 09:41:03.987982 rosetta-ce-1.4.6/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.4.6/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.4.6/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.4.6/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.4.5/LICENSE` & `rosetta-ce-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.5/PKG-INFO` & `rosetta-ce-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.4.5
+Version: 1.4.6
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.4.5/README.md` & `rosetta-ce-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.5/rosetta/constants/sensors.py` & `rosetta-ce-1.4.6/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.5/rosetta/constants/sources.py` & `rosetta-ce-1.4.6/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.5/rosetta/constants/systems.py` & `rosetta-ce-1.4.6/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.5/rosetta/rconverter.py` & `rosetta-ce-1.4.6/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.5/rosetta/rfaker.py` & `rosetta-ce-1.4.6/rosetta/rfaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -415,25 +415,25 @@
             field_value = random.choice(observables.cve) if observables and observables.cve \
                     else Observables.generator(observable_type=ObservableType.CVE, count=1)
         if field == "file_hash":
             field_value = random.choice(observables.file_hash) if observables and observables.file_hash \
                     else Observables.generator(observable_type=ObservableType.SHA256, known=ObservableKnown.BAD,
                                                count=1)
         if field == "incident_types":
-            field_value = observables.incident_types if observables and observables.incident_types \
+            field_value = random.choice(observables.incident_types) if observables and observables.incident_types \
                 else INCIDENTS_TYPES
         if field == "analysts":
-            field_value = observables.analysts if observables and observables.analysts \
+            field_value = random.choice(observables.analysts) if observables and observables.analysts \
                 else [faker.unique.first_name() for _ in range(10)]
         if field == "duration":
             field_value = random.randint(1, 5)
         if field == "log_id":
             field_value = faker.uuid4()
         if field == "alert_name":
-            field_value = observables.alert_name if observables and observables.alert_name \
+            field_value = random.choice(observables.alert_name) if observables and observables.alert_name \
                 else faker.sentence(nb_words=4)
         return field_value
 
     @classmethod
     def syslog(cls, count: int, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None,
                required_fields: Optional[str] = None) -> List[str]:
         """
```

### Comparing `rosetta-ce-1.4.5/rosetta/rsender.py` & `rosetta-ce-1.4.6/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.5/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.4.6/rosetta_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.4.5
+Version: 1.4.6
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.4.5/setup.py` & `rosetta-ce-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.4.5",
+    version="1.4.6",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.4.5/tests/test_rconverter.py` & `rosetta-ce-1.4.6/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.5/tests/test_rfaker.py` & `rosetta-ce-1.4.6/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.5/tests/test_rsender.py` & `rosetta-ce-1.4.6/tests/test_rsender.py`

 * *Files identical despite different names*

