# Comparing `tmp/automation-utilities-1.3.5.tar.gz` & `tmp/automation-utilities-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-utilities-1.3.5.tar", last modified: Sun Jul  2 20:39:26 2023, max compression
+gzip compressed data, was "automation-utilities-1.3.6.tar", last modified: Mon Jul  3 21:44:28 2023, max compression
```

## Comparing `automation-utilities-1.3.5.tar` & `automation-utilities-1.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 20:39:26.719367 automation-utilities-1.3.5/
-drwxrwxrwx   0        0        0        0 2023-07-02 20:39:26.718360 automation-utilities-1.3.5/Automation_Utilities.egg-info/
--rw-rw-rw-   0        0        0      134 2023-07-02 20:39:26.000000 automation-utilities-1.3.5/Automation_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2023-07-02 20:39:26.000000 automation-utilities-1.3.5/Automation_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 20:39:26.000000 automation-utilities-1.3.5/Automation_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-02 20:39:26.000000 automation-utilities-1.3.5/Automation_Utilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-02 20:39:26.000000 automation-utilities-1.3.5/Automation_Utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-07-02 20:39:26.718360 automation-utilities-1.3.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-02 20:39:26.716389 automation-utilities-1.3.5/automation_utilities/
--rw-rw-rw-   0        0        0     1358 2023-07-02 20:29:10.000000 automation-utilities-1.3.5/automation_utilities/Data.py
--rw-rw-rw-   0        0        0      669 2023-07-02 12:40:51.000000 automation-utilities-1.3.5/automation_utilities/Files.py
--rw-rw-rw-   0        0        0      147 2023-07-02 15:43:12.000000 automation-utilities-1.3.5/automation_utilities/Input.py
--rw-rw-rw-   0        0        0      835 2023-06-27 20:34:27.000000 automation-utilities-1.3.5/automation_utilities/PhoneNumbers.py
--rw-rw-rw-   0        0        0        0 2023-06-26 15:36:31.000000 automation-utilities-1.3.5/automation_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-02 20:39:26.719367 automation-utilities-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0      262 2023-07-02 20:39:24.000000 automation-utilities-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:44:28.192766 automation-utilities-1.3.6/
+drwxrwxrwx   0        0        0        0 2023-07-03 21:44:28.186727 automation-utilities-1.3.6/Automation_Utilities.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-07-03 21:44:27.000000 automation-utilities-1.3.6/Automation_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2023-07-03 21:44:27.000000 automation-utilities-1.3.6/Automation_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 21:44:27.000000 automation-utilities-1.3.6/Automation_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 21:44:27.000000 automation-utilities-1.3.6/Automation_Utilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-03 21:44:27.000000 automation-utilities-1.3.6/Automation_Utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-07-03 21:44:28.190772 automation-utilities-1.3.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 21:44:28.160701 automation-utilities-1.3.6/automation_utilities/
+-rw-rw-rw-   0        0        0     1358 2023-07-02 20:29:10.000000 automation-utilities-1.3.6/automation_utilities/Data.py
+-rw-rw-rw-   0        0        0      700 2023-07-03 15:16:47.000000 automation-utilities-1.3.6/automation_utilities/Files.py
+-rw-rw-rw-   0        0        0      147 2023-07-02 15:43:12.000000 automation-utilities-1.3.6/automation_utilities/Input.py
+-rw-rw-rw-   0        0        0      835 2023-06-27 20:34:27.000000 automation-utilities-1.3.6/automation_utilities/PhoneNumbers.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 15:36:31.000000 automation-utilities-1.3.6/automation_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-03 21:44:28.193752 automation-utilities-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      262 2023-07-03 21:44:20.000000 automation-utilities-1.3.6/setup.py
```

### Comparing `automation-utilities-1.3.5/Automation_Utilities.egg-info/SOURCES.txt` & `automation-utilities-1.3.6/Automation_Utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation-utilities-1.3.5/automation_utilities/Data.py` & `automation-utilities-1.3.6/automation_utilities/Data.py`

 * *Files identical despite different names*

### Comparing `automation-utilities-1.3.5/automation_utilities/PhoneNumbers.py` & `automation-utilities-1.3.6/automation_utilities/PhoneNumbers.py`

 * *Files identical despite different names*

