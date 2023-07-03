# Comparing `tmp/mend_ignore_alerts-0.2.3-py3-none-any.whl.zip` & `tmp/mend_ignore_alerts-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11948 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 08:04 mend_ignore_alerts/__init__.py
--rw-r--r--  2.0 unx      107 b- defN 23-Jul-03 08:04 mend_ignore_alerts/_version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 08:04 mend_ignore_alerts/conftest.py
--rw-r--r--  2.0 unx     1554 b- defN 23-Jul-03 08:04 mend_ignore_alerts/const.py
--rw-r--r--  2.0 unx    10673 b- defN 23-Jul-03 08:04 mend_ignore_alerts/ignore_alerts.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-03 08:04 mend_ignore_alerts-0.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     5030 b- defN 23-Jul-03 08:04 mend_ignore_alerts-0.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 08:04 mend_ignore_alerts-0.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Jul-03 08:04 mend_ignore_alerts-0.2.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-03 08:04 mend_ignore_alerts-0.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      979 b- defN 23-Jul-03 08:04 mend_ignore_alerts-0.2.3.dist-info/RECORD
-11 files, 29883 bytes uncompressed, 10256 bytes compressed:  65.7%
+Zip file size: 11982 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 14:27 mend_ignore_alerts/__init__.py
+-rw-r--r--  2.0 unx      107 b- defN 23-Jul-03 14:27 mend_ignore_alerts/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 14:27 mend_ignore_alerts/conftest.py
+-rw-r--r--  2.0 unx     1554 b- defN 23-Jul-03 14:27 mend_ignore_alerts/const.py
+-rw-r--r--  2.0 unx    10755 b- defN 23-Jul-03 14:27 mend_ignore_alerts/ignore_alerts.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-03 14:27 mend_ignore_alerts-0.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5030 b- defN 23-Jul-03 14:27 mend_ignore_alerts-0.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 14:27 mend_ignore_alerts-0.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jul-03 14:27 mend_ignore_alerts-0.2.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-03 14:27 mend_ignore_alerts-0.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      979 b- defN 23-Jul-03 14:27 mend_ignore_alerts-0.2.4.dist-info/RECORD
+11 files, 29965 bytes uncompressed, 10290 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: mend_ignore_alerts/const.py
 Comment: 
 
 Filename: mend_ignore_alerts/ignore_alerts.py
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.3.dist-info/LICENSE
+Filename: mend_ignore_alerts-0.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.3.dist-info/METADATA
+Filename: mend_ignore_alerts-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.3.dist-info/WHEEL
+Filename: mend_ignore_alerts-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.3.dist-info/entry_points.txt
+Filename: mend_ignore_alerts-0.2.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.3.dist-info/top_level.txt
+Filename: mend_ignore_alerts-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.3.dist-info/RECORD
+Filename: mend_ignore_alerts-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_ignore_alerts/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 __tool_name__ = "ignore_alerts"
 __description__ = "Parse yml file and update alerts"
```

## mend_ignore_alerts/ignore_alerts.py

```diff
@@ -179,14 +179,15 @@
     return res
 
 
 def is_vuln_in_ignored(vulnerability, ign_list):
     for ign_ in ign_list:
         for key, value in ign_.items():
             if vulnerability.strip() == key:
+                logger.info(f"key*{key}*, vuln*{vulnerability.strip()}*")
                 return True, value
     return False, ""
 
 
 def read_yaml(yml_file):
     with open(yml_file, 'r') as file:
         data = yaml.safe_load(file)
@@ -229,16 +230,16 @@
 
 
 def exec_input_yaml(input_data):
     for el_ in input_data:
         prj_token = get_token_by_prj_name(el_["name"])
         if prj_token:
             ignored_al = get_ingnored_alerts(project=prj_token)
+            print(ignored_al)
             #restore_alerts(project=prj_token)
-            #exit(-1)
             alerts = get_alerts_by_type(prj_token=prj_token, alert_type="SECURITY_VULNERABILITY")
             try:
                 for data_ in el_["vulns"]:
                     note = data_["note"]
                     status, note_ign = is_vuln_in_ignored(vulnerability=data_["vuln_id"],ign_list=ignored_al)
                     if not status:
                         alert_uuid = ""
```

## Comparing `mend_ignore_alerts-0.2.3.dist-info/LICENSE` & `mend_ignore_alerts-0.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_ignore_alerts-0.2.3.dist-info/METADATA` & `mend_ignore_alerts-0.2.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mend-ignore-alerts
-Version: 0.2.3
+Version: 0.2.4
 Summary: Parse yml file and update alerts
 Home-page: https://github.com/mend-toolkit/ignore-alerts
 Author: Mend Professional Services
 Author-email: ps@mend.io
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

