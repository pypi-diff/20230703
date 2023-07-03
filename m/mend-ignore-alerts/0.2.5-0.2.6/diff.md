# Comparing `tmp/mend_ignore_alerts-0.2.5-py3-none-any.whl.zip` & `tmp/mend_ignore_alerts-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11996 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 14:48 mend_ignore_alerts/__init__.py
--rw-r--r--  2.0 unx      107 b- defN 23-Jul-03 14:48 mend_ignore_alerts/_version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 14:48 mend_ignore_alerts/conftest.py
--rw-r--r--  2.0 unx     1554 b- defN 23-Jul-03 14:48 mend_ignore_alerts/const.py
--rw-r--r--  2.0 unx    10794 b- defN 23-Jul-03 14:48 mend_ignore_alerts/ignore_alerts.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-03 14:49 mend_ignore_alerts-0.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     5030 b- defN 23-Jul-03 14:49 mend_ignore_alerts-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 14:49 mend_ignore_alerts-0.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Jul-03 14:49 mend_ignore_alerts-0.2.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-03 14:49 mend_ignore_alerts-0.2.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      979 b- defN 23-Jul-03 14:49 mend_ignore_alerts-0.2.5.dist-info/RECORD
-11 files, 30004 bytes uncompressed, 10304 bytes compressed:  65.7%
+Zip file size: 11999 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 15:00 mend_ignore_alerts/__init__.py
+-rw-r--r--  2.0 unx      107 b- defN 23-Jul-03 15:00 mend_ignore_alerts/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 15:00 mend_ignore_alerts/conftest.py
+-rw-r--r--  2.0 unx     1554 b- defN 23-Jul-03 15:00 mend_ignore_alerts/const.py
+-rw-r--r--  2.0 unx    10820 b- defN 23-Jul-03 15:00 mend_ignore_alerts/ignore_alerts.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-03 15:00 mend_ignore_alerts-0.2.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5030 b- defN 23-Jul-03 15:00 mend_ignore_alerts-0.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 15:00 mend_ignore_alerts-0.2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jul-03 15:00 mend_ignore_alerts-0.2.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-03 15:00 mend_ignore_alerts-0.2.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      979 b- defN 23-Jul-03 15:00 mend_ignore_alerts-0.2.6.dist-info/RECORD
+11 files, 30030 bytes uncompressed, 10307 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: mend_ignore_alerts/const.py
 Comment: 
 
 Filename: mend_ignore_alerts/ignore_alerts.py
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.5.dist-info/LICENSE
+Filename: mend_ignore_alerts-0.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.5.dist-info/METADATA
+Filename: mend_ignore_alerts-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.5.dist-info/WHEEL
+Filename: mend_ignore_alerts-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.5.dist-info/entry_points.txt
+Filename: mend_ignore_alerts-0.2.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.5.dist-info/top_level.txt
+Filename: mend_ignore_alerts-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.5.dist-info/RECORD
+Filename: mend_ignore_alerts-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_ignore_alerts/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __tool_name__ = "ignore_alerts"
 __description__ = "Parse yml file and update alerts"
```

## mend_ignore_alerts/ignore_alerts.py

```diff
@@ -176,15 +176,15 @@
             })
     except Exception as err:
         pass
     return res
 
 
 def is_vuln_in_ignored(vulnerability, ign_list):
-    logger.info(f"Ignored:{ign_list}")
+    logger.info(f"Ignored:{ign_list},{vulnerability}")
     for ign_ in ign_list:
         for key, value in ign_.items():
             if vulnerability.strip() == key:
                 logger.info(f"key*{key}*, vuln*{vulnerability.strip()}*")
                 return True, value
     return False, ""
 
@@ -232,20 +232,20 @@
 
 def exec_input_yaml(input_data):
     for el_ in input_data:
         prj_token = get_token_by_prj_name(el_["name"])
         if prj_token:
             #restore_alerts(project=prj_token)
             ignored_al = get_ingnored_alerts(project=prj_token)
-            print(ignored_al)
             alerts = get_alerts_by_type(prj_token=prj_token, alert_type="SECURITY_VULNERABILITY")
             try:
                 for data_ in el_["vulns"]:
                     note = data_["note"]
                     status, note_ign = is_vuln_in_ignored(vulnerability=data_["vuln_id"],ign_list=ignored_al)
+                    logger.info(status)
                     if not status:
                         alert_uuid = ""
                         for alert_ in alerts:
                             if alert_["vulnerability"]["name"] == data_["vuln_id"] and "SNYK" not in data_["vuln_id"]:
                                 alert_uuid = alert_["alertUuid"]
                                 break
                         if alert_uuid :
```

## Comparing `mend_ignore_alerts-0.2.5.dist-info/LICENSE` & `mend_ignore_alerts-0.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_ignore_alerts-0.2.5.dist-info/METADATA` & `mend_ignore_alerts-0.2.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mend-ignore-alerts
-Version: 0.2.5
+Version: 0.2.6
 Summary: Parse yml file and update alerts
 Home-page: https://github.com/mend-toolkit/ignore-alerts
 Author: Mend Professional Services
 Author-email: ps@mend.io
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `mend_ignore_alerts-0.2.5.dist-info/RECORD` & `mend_ignore_alerts-0.2.6.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mend_ignore_alerts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mend_ignore_alerts/_version.py,sha256=s9rJBUIhAG9SQrnoyXz837qS2a_qNnlrqwOzBgp2LWM,107
+mend_ignore_alerts/_version.py,sha256=HIpfv8IwUQtjpqefN8bfXQNye1w6txDlr-TP4D7aRp4,107
 mend_ignore_alerts/conftest.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mend_ignore_alerts/const.py,sha256=aRDadkUul_6NZB_LDIZTkGf5VkWTPqfnj6eap-1Y7As,1554
-mend_ignore_alerts/ignore_alerts.py,sha256=S6joLY8o3uGHb5cVBImSoAO2UpKrGw-mhUfRCxXxsHI,10794
-mend_ignore_alerts-0.2.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mend_ignore_alerts-0.2.5.dist-info/METADATA,sha256=u3xEbePA8Z7XQY3TstvtoHHOsiCfiMhxe3EChbHBQ2M,5030
-mend_ignore_alerts-0.2.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mend_ignore_alerts-0.2.5.dist-info/entry_points.txt,sha256=b_q3jF-WbTVm6sR0BrVXts8u1OhXtD1aM2IZ5CfWmpE,72
-mend_ignore_alerts-0.2.5.dist-info/top_level.txt,sha256=ookvTXlTz4JKFzjrBd6U6MmV6RzYs9C8B2E2vMscaZ8,19
-mend_ignore_alerts-0.2.5.dist-info/RECORD,,
+mend_ignore_alerts/ignore_alerts.py,sha256=ORvJgO4SfETEBVN6MoDBF33XN6JRUTc7YTtW2SzTHlY,10820
+mend_ignore_alerts-0.2.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mend_ignore_alerts-0.2.6.dist-info/METADATA,sha256=HC90mUswpKYavgXdfbcBPT4mnXuJpD_gpCWwx0AJb-s,5030
+mend_ignore_alerts-0.2.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mend_ignore_alerts-0.2.6.dist-info/entry_points.txt,sha256=b_q3jF-WbTVm6sR0BrVXts8u1OhXtD1aM2IZ5CfWmpE,72
+mend_ignore_alerts-0.2.6.dist-info/top_level.txt,sha256=ookvTXlTz4JKFzjrBd6U6MmV6RzYs9C8B2E2vMscaZ8,19
+mend_ignore_alerts-0.2.6.dist-info/RECORD,,
```

