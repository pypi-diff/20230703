# Comparing `tmp/robotframework-robotlog2db-1.3.8.tar.gz` & `tmp/robotframework-robotlog2db-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robotlog2db-1.3.8.tar", last modified: Wed Jun 21 11:40:54 2023, max compression
+gzip compressed data, was "robotframework-robotlog2db-1.3.9.tar", last modified: Mon Jul  3 13:39:19 2023, max compression
```

## Comparing `robotframework-robotlog2db-1.3.8.tar` & `robotframework-robotlog2db-1.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:54.965007 robotframework-robotlog2db-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-06-21 11:40:54.965007 robotframework-robotlog2db-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:54.965007 robotframework-robotlog2db-1.3.8/RobotLog2DB/
--rw-r--r--   0 runner    (1001) docker     (123)    41226 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/RobotLog2DB/CDataBase.py
--rw-r--r--   0 runner    (1001) docker     (123)   595489 2023-06-21 11:40:53.000000 robotframework-robotlog2db-1.3.8/RobotLog2DB/RobotLog2DB.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/RobotLog2DB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/RobotLog2DB/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43282 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/RobotLog2DB/robotlog2db.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/RobotLog2DB/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:54.965007 robotframework-robotlog2db-1.3.8/RobotLog2DB/xsd/
--rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/RobotLog2DB/xsd/robot.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:54.965007 robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-06-21 11:40:54.000000 robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-21 11:40:54.000000 robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:40:54.000000 robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 11:40:54.000000 robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 11:40:54.000000 robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 11:40:54.000000 robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 11:40:54.965007 robotframework-robotlog2db-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:39:19.210963 robotframework-robotlog2db-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-07-03 13:39:19.210963 robotframework-robotlog2db-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-07-03 13:37:13.000000 robotframework-robotlog2db-1.3.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:39:19.206963 robotframework-robotlog2db-1.3.9/RobotLog2DB/
+-rw-r--r--   0 runner    (1001) docker     (123)    41226 2023-07-03 13:37:13.000000 robotframework-robotlog2db-1.3.9/RobotLog2DB/CDataBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)   597780 2023-07-03 13:39:18.000000 robotframework-robotlog2db-1.3.9/RobotLog2DB/RobotLog2DB.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-03 13:37:13.000000 robotframework-robotlog2db-1.3.9/RobotLog2DB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-03 13:37:13.000000 robotframework-robotlog2db-1.3.9/RobotLog2DB/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46373 2023-07-03 13:37:13.000000 robotframework-robotlog2db-1.3.9/RobotLog2DB/robotlog2db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-03 13:37:13.000000 robotframework-robotlog2db-1.3.9/RobotLog2DB/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:39:19.206963 robotframework-robotlog2db-1.3.9/RobotLog2DB/xsd/
+-rw-r--r--   0 runner    (1001) docker     (123)    22349 2023-07-03 13:37:13.000000 robotframework-robotlog2db-1.3.9/RobotLog2DB/xsd/robot.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:39:19.206963 robotframework-robotlog2db-1.3.9/robotframework_robotlog2db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-07-03 13:39:19.000000 robotframework-robotlog2db-1.3.9/robotframework_robotlog2db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-03 13:39:19.000000 robotframework-robotlog2db-1.3.9/robotframework_robotlog2db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:39:19.000000 robotframework-robotlog2db-1.3.9/robotframework_robotlog2db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 13:39:19.000000 robotframework-robotlog2db-1.3.9/robotframework_robotlog2db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 13:39:19.000000 robotframework-robotlog2db-1.3.9/robotframework_robotlog2db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 13:39:19.000000 robotframework-robotlog2db-1.3.9/robotframework_robotlog2db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:39:19.210963 robotframework-robotlog2db-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-03 13:37:13.000000 robotframework-robotlog2db-1.3.9/setup.py
```

### Comparing `robotframework-robotlog2db-1.3.8/PKG-INFO` & `robotframework-robotlog2db-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robotlog2db
-Version: 1.3.8
+Version: 1.3.9
 Summary: Imports robot result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/robotframework-robotlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-robotlog2db-1.3.8/README.rst` & `robotframework-robotlog2db-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.3.8/RobotLog2DB/CDataBase.py` & `robotframework-robotlog2db-1.3.9/RobotLog2DB/CDataBase.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.3.8/RobotLog2DB/RobotLog2DB.pdf` & `robotframework-robotlog2db-1.3.9/RobotLog2DB/RobotLog2DB.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 10% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 RobotLog2DB
-v. 1.3.8
+v. 1.3.9
 Tran Duy Ngoan
-21.06.2023
+23.06.2023
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -255,72 +255,80 @@
 
 Function: format time . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 25
 
 4.8
 
-Function: process suite metadata . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+Function: retrieve result starttime . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 26
 
 4.9
 
-Function: process metadata . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+Function: retrieve result endtime . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 26
 
-4.10 Function: process suite . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+4.10 Function: process suite metadata . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 26
 
-4.11 Function: process test . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+4.11 Function: process metadata . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 27
 
-4.12 Function: process config file . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+4.12 Function: process suite . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 27
 
-4.13 Function: normalize path . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+4.13 Function: process test . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 28
 
-4.14 Function: RobotLog2DB . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+4.14 Function: process config file . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 28
 
-4.15 Class: Logger . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+4.15 Function: normalize path . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 29
 
-4.15.1 Method: config . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+4.16 Function: RobotLog2DB . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 29
 
-4.15.2 Method: log . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+4.17 Class: Logger . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 30
 
-4.15.3 Method: log warning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+4.17.1 Method: config . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 30
 
-4.15.4 Method: log error . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+4.17.2 Method: log . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 30
 
-5 Appendix
+4.17.3 Method: log warning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 31
 
-6 History
+4.17.4 Method: log error . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+
+31
+
+5 Appendix
 
 32
 
+6 History
+
+33
+
 B
 
 CHAPTER 1. INTRODUCTION
 
 Chapter 1
 
 Introduction
@@ -1806,15 +1814,47 @@
 TestResultWebApp’s time as format %Y-%m-%d %H:%M:%S.
 25
 
 CHAPTER 4. ROBOTLOG2DB.PY
 
 4.8
 
-4.8. FUNCTION: PROCESS SUITE METADATA
+4.8. FUNCTION: RETRIEVE RESULT STARTTIME
+
+Function: retrieve result starttime
+
+Retrieve starttime infomration from given result object (TestSuite or TestCase). In case the starttime in given suite
+is ’N/A’, it will try to get this information from its children suite/test.
+Arguments:
+ stime
+
+/ Condition: required / Type: TestSuite or TestCase object /
+Result object to retrieve starttime.
+Returns:
+ / Type: str /
+
+Start time of given result.
+
+Function: retrieve result endtime
+
+4.9
+
+Retrieve endtime infomration from given result object (TestSuite or TestCase). In case the endtime in given suite is
+’N/A’, it will try to get this information from its children suite/test.
+Arguments:
+ stime
+
+/ Condition: required / Type: TestSuite or TestCase object /
+Result object to retrieve endtime.
+Returns:
+ / Type: str /
+
+End time of given result.
+
+4.10
 
 Function: process suite metadata
 
 Try to find metadata information from all suite levels.
 Metadata at top suite level has a highest priority.
 Arguments:
  suite
@@ -1827,17 +1867,23 @@
 Initial Metadata information for updating.
 Returns:
  dMetadata
 
 / Type: dict /
 Dictionary of Metadata information.
 
-Function: process metadata
+26
 
-4.9
+CHAPTER 4. ROBOTLOG2DB.PY
+
+4.11
+
+4.11. FUNCTION: PROCESS METADATA
+
+Function: process metadata
 
 Extract metadata from suite result bases on DEFAULT METADATA.
 Arguments:
  metadata
 
 / Condition: required / Type: dict /
 Robot metadata object.
@@ -1847,34 +1893,27 @@
 Initial Metadata information for updating.
 Returns:
  dMetadata
 
 / Type: dict /
 Dictionary of Metadata information.
 
-4.10
+4.12
 
 Function: process suite
 
 Process to the lowest suite level (test file):
  Create new file and its header information
  Then, process all child test cases
 
 Arguments:
  db
 
 / Condition: required / Type: CDataBase object /
 CDataBase object.
-
-26
-
-CHAPTER 4. ROBOTLOG2DB.PY
-
-4.11. FUNCTION: PROCESS TEST
-
  suite
 
 / Condition: required / Type: TestSuite object /
 Robot suite object.
  tbl test result id
 
 / Condition: required / Type: str /
@@ -1886,15 +1925,21 @@
  dConfig
 
 / Condition: required / Type: dict / Default: None /
 Configuration data which is parsed from given json configuration file.
 Returns:
 (no returns)
 
-4.11
+27
+
+CHAPTER 4. ROBOTLOG2DB.PY
+
+4.13
+
+4.13. FUNCTION: PROCESS TEST
 
 Function: process test
 
 Process test case data and create new test case record.
 Arguments:
  db
 
@@ -1919,27 +1964,21 @@
  test number
 
 / Condition: required / Type: int /
 Order of test case in file.
 Returns:
 (no returns)
 
-4.12
+4.14
 
 Function: process config file
 
 Parse information from configuration file:
  component:
 
-27
-
-CHAPTER 4. ROBOTLOG2DB.PY
-
-4.13. FUNCTION: NORMALIZE PATH
-
 {
 "components" : {
 "componentA" : "componentA/path/to/testcase",
 "componentB" : "componentB/path/to/testcase",
 "componentC" : [
 "componentC1/path/to/testcase",
 "componentC2/path/to/testcase"
@@ -1947,86 +1986,93 @@
 }
 }
 Then all testcases which their paths contain componentA/path/to/testcase will be belong to
 componentA, ...
  variant, version sw: configuration file has low priority than command line.
 
 Arguments:
+
+28
+
+CHAPTER 4. ROBOTLOG2DB.PY
+
+4.15. FUNCTION: NORMALIZE PATH
+
  config file
 
 / Condition: required / Type: str /
 Path to configuration file.
 Returns:
  dConfig
 
 / Type: dict /
 Configuration object.
 
-4.13
+4.15
 
 Function: normalize path
 
 Normalize path file.
 Arguments:
  sPath
 
 / Condition: required / Type: str /
 Path file to be normalized.
  sNPath
 
 / Type: str /
 Normalized path file.
 
-4.14
+4.16
 
 Function: RobotLog2DB
 
 Import robot results from output.xml to TestResultWebApp’s database.
 Flow to import Robot results to database:
 1. Process provided arguments from command line.
 2. Parse Robot results.
 3. Connect to database.
 4. Import results into database.
 5. Disconnect from database.
 Arguments:
-28
-
-CHAPTER 4. ROBOTLOG2DB.PY
-
-4.15. CLASS: LOGGER
-
  args
 
 / Condition: required / Type: ArgumentParser object /
 Argument parser object which contains:
 – resultxmlfile : path to the xml result file or directory of result files to be imported.
 – server : server which hosts the database (IP or URL).
 – user : user for database login.
 – password : password for database login.
 – database : database name.
 – recursive : if True, then the path is searched recursively for log files to be imported.
 – dryrun : if True, then verify all input arguments (includes DB connection) and show what would be done.
 – append : if True, then allow to append new result(s) to existing execution result UUID which is provided
 by --UUID argument.
 – UUID : UUID used to identify the import and version ID on TestResultWebApp.
+29
+
+CHAPTER 4. ROBOTLOG2DB.PY
+
+4.17. CLASS: LOGGER
+
 – variant : variant name to be set for this import.
 – versions : metadata: Versions (Software;Hardware;Test) to be set for this import.
 – config : configuration json file for component mapping information.
 Returns:
 (no returns)
 
-4.15
+4.17
 
 Class: Logger
 
 Imported by:
 from RobotLog2DB.robotlog2db import Logger
 Logger class for logging message.
 
-4.15.1
+4.17.1
 
 Method: config
 
 Configure Logger class.
 Arguments:
  output console
 
@@ -2039,21 +2085,15 @@
  dryrun
 
 / Condition: optional / Type: bool / Default: True /
 If set, a prefix as ’dryrun’ is added for all messages.
 Returns:
 (no returns)
 
-29
-
-CHAPTER 4. ROBOTLOG2DB.PY
-
-4.15.2
-
-4.15. CLASS: LOGGER
+4.17.2
 
 Method: log
 
 Write log message to console/file output.
 Arguments:
  msg
 
@@ -2065,29 +2105,34 @@
 Color style for the message.
  indent
 
 / Condition: optional / Type: int / Default: 0 /
 Offset indent.
 Returns:
 (no returns)
+30
+
+CHAPTER 4. ROBOTLOG2DB.PY
 
-4.15.3
+4.17.3
+
+4.17. CLASS: LOGGER
 
 Method: log warning
 
 Write warning message to console/file output.
 Arguments:
  msg
 
 / Condition: required / Type: str /
 Warning message which is written to output.
 Returns:
 (no returns)
 
-4.15.4
+4.17.4
 
 Method: log error
 
 Write error message to console/file output.
 Arguments:
  msg
 
@@ -2096,15 +2141,15 @@
  fatal error
 
 / Condition: optional / Type: bool / Default: False /
 If set, tool will terminate after logging error message.
 Returns:
 (no returns)
 
-30
+31
 
 CHAPTER 5. APPENDIX
 
 Chapter 5
 
 Appendix
 About this package:
@@ -2115,19 +2160,19 @@
 
 Name
 
 RobotLog2DB
 
 Version
 
-1.3.8
+1.3.9
 
 Date
 
-21.06.2023
+23.06.2023
 
 Description
 
 Imports robot result(s) to TestResultWebApp database
 
 Package URL
 
@@ -2165,15 +2210,15 @@
 
 Intended Audience :: Developers
 
 Topic
 
 Topic :: Software Development
 
-31
+32
 
 CHAPTER 6. HISTORY
 
 Chapter 6
 
 History
 0.1.0
@@ -2247,24 +2292,30 @@
 - Add try/except for database access
 1.3.7
 
 14.06.2023
 
 Update README with new instruction for installation and image’s links
 
-32
+33
 
 CHAPTER 6. HISTORY
 
 1.3.8
 
 21.06.2023
 
 Fix issue with suite.starttime at root suite is N/A
+1.3.9
+
+23.06.2023
+
+- Retrieve start/end time for suite
+- Update result schema to support Robotframework Version 6.1
 
 RobotLog2DB.pdf
-Created at 21.06.2023 - 11:40:49
+Created at 03.07.2023 - 13:39:14
 by GenPackageDoc v. 0.40.3
 
-33
+34
```

### Comparing `robotframework-robotlog2db-1.3.8/RobotLog2DB/__init__.py` & `robotframework-robotlog2db-1.3.9/RobotLog2DB/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.3.8/RobotLog2DB/__main__.py` & `robotframework-robotlog2db-1.3.9/RobotLog2DB/__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.3.8/RobotLog2DB/robotlog2db.py` & `robotframework-robotlog2db-1.3.9/RobotLog2DB/robotlog2db.py`

 * *Files 7% similar despite different names*

```diff
@@ -544,14 +544,89 @@
    try:
       sFormatedTime = sTime[0:4]+"-"+sTime[4:6]+"-"+sTime[6:]
    except Exception as reason:
       Logger.log_error(f"Cannot convert given time '{sTime}' to TestResultWebApp's time format.\nReason: {reason}",
                         fatal_error=True)
    return sFormatedTime
 
+def retrieve_result_starttime(objResult):
+   """
+Retrieve starttime infomration from given result object (TestSuite or TestCase).
+In case the starttime in given suite is 'N/A', it will try to get this information from its children suite/test.
+
+**Arguments:**
+
+*  ``stime``
+
+   / *Condition*: required / *Type*: `TestSuite` or `TestCase` object /
+
+   Result object to retrieve starttime.
+
+**Returns:**
+
+*  / *Type*: str /
+
+   Start time of given result.
+   """
+   lStarttime = []
+   # Try to get starttime from root TestSuite to children TestCase
+   if type(objResult).__name__ == "TestSuite":
+      if objResult.starttime:
+         return objResult.starttime
+      elif len(objResult.suites) > 0:
+         lStarttime = [suite_starttime for suite in objResult.suites if (suite_starttime:=retrieve_result_starttime(suite)) is not None]
+      else:
+         lStarttime = [test_starttime for test in objResult.tests if (test_starttime:=retrieve_result_starttime(test)) is not None]
+   elif type(objResult).__name__ == "TestCase":
+      if objResult.starttime:
+         return objResult.starttime
+
+   if len(lStarttime):
+      return min(lStarttime)
+
+   return None
+
+def retrieve_result_endtime(objResult):
+   """
+Retrieve endtime infomration from given result object (TestSuite or TestCase).
+In case the endtime in given suite is 'N/A', it will try to get this information from its children suite/test.
+
+**Arguments:**
+
+*  ``stime``
+
+   / *Condition*: required / *Type*: `TestSuite` or `TestCase` object /
+
+   Result object to retrieve endtime.
+
+**Returns:**
+
+*  / *Type*: str /
+
+   End time of given result.
+   """
+   lEndtime = []
+   # Try to get endtime from root TestSuite to children TestCase
+   if type(objResult).__name__ == "TestSuite":
+      if objResult.endtime:
+         return objResult.endtime
+      elif len(objResult.suites) > 0:
+         lEndtime = [suite_endtime for suite in objResult.suites if (suite_endtime:=retrieve_result_endtime(suite)) is not None]
+      else:
+         lEndtime = [test_endtime for test in objResult.tests if (test_endtime:=retrieve_result_endtime(test)) is not None]
+   elif type(objResult).__name__ == "TestCase":
+      if objResult.endtime:
+         return objResult.endtime
+
+   if len(lEndtime):
+      return max(lEndtime)
+
+   return None
+
+
 def __process_commandline():
    """
 Process provided argument(s) from command line.
 
 Avalable arguments in command line:
 
    - `-v`, `--version` : tool version information.
@@ -739,16 +814,23 @@
       # File metadata
       metadata_info = process_metadata(suite.metadata, root_metadata)
       _tbl_file_name = suite.source
       _tbl_file_tester_account = metadata_info['tester']
       if dConfig != None and 'tester' in dConfig:
          _tbl_file_tester_account = dConfig['tester']
       _tbl_file_tester_machine = metadata_info['machine']
-      _tbl_file_time_start     = format_time(suite.starttime)
-      _tbl_file_time_end       = format_time(suite.endtime)
+
+      sSuiteStarttime = retrieve_result_starttime(suite)
+      sSuiteEndtime   = retrieve_result_endtime(suite)
+      if not sSuiteStarttime:
+         Logger.log_error(f"Could not retieve start time of suite '{suite.name}'.")
+      if not sSuiteEndtime:
+         Logger.log_error(f"Could not retieve end time of suite '{suite.name}'.")
+      _tbl_file_time_start     = format_time(sSuiteStarttime)
+      _tbl_file_time_end       = format_time(sSuiteEndtime)
 
       # Process component information if not provided in metadata
       if metadata_info['component'] == '':
          # assign default component name as 'unknown'
          metadata_info['component'] = 'unknown'
 
          # process component mapping if provided in config file
@@ -1204,31 +1286,36 @@
          if 'version_test' in dConfig:
             sVersionTest = dConfig['version_test']
       _tbl_result_version_sw_target = sVersionSW
       _tbl_result_version_hardware  = sVersionHW
       _tbl_result_version_sw_test   = sVersionTest
 
       # Process start/end time info
-      sSuiteStarttime = result.suite.starttime
-      sSuiteEndtime   = result.suite.endtime
-
-      # Get start and end time of suite a as min and max time incase multiple suite results
-      if (len(sources) > 1) or (len(result.suite.suites) > 0):
-         sSuiteStarttime = min([suite.starttime for suite in result.suite.suites])
-         sSuiteEndtime   = max([suite.endtime for suite in result.suite.suites])
+      sExecutionStarttime = retrieve_result_starttime(result.suite)
+      sExecutionEndtime   = retrieve_result_endtime(result.suite)
+      if not sExecutionStarttime:
+         Logger.log_error(f"Could not retieve execution start time."+
+                           "\nPlease use rebot with option '--starttime timestamp' when merging/combining result files."+
+                           "\nOr rerun Robotframework testcase(s) to get proper *.xml result file.",
+                           fatal_error=True)
+      if not sExecutionEndtime:
+         Logger.log_error(f"Could not retieve execution end time."+
+                           "\nPlease use rebot with option '--endtime timestamp' when merging/combining result files."+
+                           "\nOr rerun Robotframework testcase(s) to get proper *.xml result file",
+                           fatal_error=True)
 
-      _tbl_result_time_start = format_time(sSuiteStarttime)
-      _tbl_result_time_end   = format_time(sSuiteEndtime)
+      _tbl_result_time_start = format_time(sExecutionStarttime)
+      _tbl_result_time_end   = format_time(sExecutionEndtime)
 
       # Set version as start time of the execution if not provided in metadata
       # Format: %Y%m%d_%H%M%S
       if _tbl_result_version_sw_target=="":
          bUseDefaultVersionSW = True
          _tbl_result_version_sw_target = re.sub(r'(\d{8})\s(\d{2}):(\d{2}):(\d{2})\.\d+',
-                                                r'\1_\2\3\4', sSuiteStarttime)
+                                                r'\1_\2\3\4', sExecutionStarttime)
       if not args.append:
          Logger.log(f"Set project/variant to '{sVariant}' ({sMsgVarirantSetBy})")
          Logger.log(f"Set version_sw to '{_tbl_result_version_sw_target}' ({sMsgVersionSWSetBy})")
 
       # Process branch info from software version
       _tbl_prj_branch = get_branch_from_swversion(_tbl_result_version_sw_target)
```

### Comparing `robotframework-robotlog2db-1.3.8/RobotLog2DB/version.py` & `robotframework-robotlog2db-1.3.9/RobotLog2DB/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of RobotLog2DB
 #
-VERSION      = "1.3.8"
-VERSION_DATE = "21.06.2023"
+VERSION      = "1.3.9"
+VERSION_DATE = "23.06.2023"
```

### Comparing `robotframework-robotlog2db-1.3.8/RobotLog2DB/xsd/robot.xsd` & `robotframework-robotlog2db-1.3.9/RobotLog2DB/xsd/robot.xsd`

 * *Files 5% similar despite different names*

#### Comparing `robotframework-robotlog2db-1.3.8/RobotLog2DB/xsd/robot.xsd` & `robotframework-robotlog2db-1.3.9/RobotLog2DB/xsd/robot.xsd`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" version="3">
+<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" version="4">
   <xs:annotation>
     <xs:documentation xml:lang="en">= Robot Framework output.xml schema =
 
             Compatible with Robot Framework 5.0 and newer. For more details see:
             https://github.com/robotframework/robotframework/tree/master/doc/schema
 
             Due to XSD 1.1 not being widely adopted, this schema is XSD 1.0 compatible.
@@ -27,15 +27,15 @@
     <!-- Version of the schema output.xml is compatible with. Must match
              the `version` attribute of the `xs:schema` root element. -->
     <xs:attribute name="schemaversion" type="SpecVersion"/>
   </xs:complexType>
   <xs:simpleType name="SpecVersion">
     <xs:restriction base="xs:integer">
       <xs:minInclusive value="2"/>
-      <xs:maxInclusive value="3"/>
+      <xs:maxInclusive value="4"/>
     </xs:restriction>
   </xs:simpleType>
   <xs:complexType name="Suite">
     <xs:choice maxOccurs="unbounded">
       <!-- These keywords are possible suite setup and teardown.
                  They must have the `type` attribute set accordingly. -->
       <xs:element name="kw" type="Keyword" minOccurs="0" maxOccurs="2"/>
@@ -52,21 +52,29 @@
   <xs:complexType name="Metadata">
     <xs:simpleContent>
       <xs:extension base="xs:string">
         <xs:attribute name="name" type="xs:string" use="required"/>
       </xs:extension>
     </xs:simpleContent>
   </xs:complexType>
+  <xs:complexType name="Error">
+    <xs:choice maxOccurs="unbounded">
+      <xs:element name="value" type="xs:string" minOccurs="1" maxOccurs="unbounded"/>
+      <xs:element name="msg" type="Message"/>
+      <xs:element name="status" type="Status"/>
+    </xs:choice>
+  </xs:complexType>
   <xs:complexType name="Test">
     <xs:choice maxOccurs="unbounded">
       <xs:element name="kw" type="Keyword" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="for" type="For" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="if" type="If" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="try" type="Try" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="while" type="While" minOccurs="0" maxOccurs="unbounded"/>
+      <xs:element name="error" type="Error" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="msg" type="Message" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="doc" type="xs:string" minOccurs="0"/>
       <xs:element name="tag" type="xs:string" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="timeout" type="Timeout" minOccurs="0"/>
       <xs:element name="status" type="Status"/>
     </xs:choice>
     <xs:attribute name="name" type="xs:string"/>
@@ -78,14 +86,15 @@
   <xs:complexType name="Keyword">
     <xs:choice maxOccurs="unbounded">
       <xs:element name="kw" type="Keyword" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="for" type="For" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="if" type="If" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="try" type="Try" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="while" type="While" minOccurs="0" maxOccurs="unbounded"/>
+      <xs:element name="error" type="Error" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="return" type="Return" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="msg" type="Message" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="var" type="xs:string" minOccurs="0" maxOccurs="unbounded"/>
       <!-- Assignment -->
       <xs:element name="arg" type="xs:string" minOccurs="0" maxOccurs="unbounded"/>
       <!-- Arguments -->
       <xs:element name="doc" type="xs:string" minOccurs="0"/>
@@ -115,14 +124,20 @@
       <xs:element name="iter" type="ForIteration" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="kw" type="Keyword" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="msg" type="Message" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="doc" type="xs:string" minOccurs="0"/>
       <xs:element name="status" type="BodyItemStatus"/>
     </xs:choice>
     <xs:attribute name="flavor" type="ForFlavor"/>
+    <xs:attribute name="start" type="xs:string"/>
+    <!-- Used if IN ENUMERATE has `start`. -->
+    <xs:attribute name="mode" type="xs:string"/>
+    <!-- Used if IN ZIP has `mode`. -->
+    <xs:attribute name="fill" type="xs:string"/>
+    <!-- Used if IN ZIP has `fill`. -->
   </xs:complexType>
   <xs:simpleType name="ForFlavor">
     <xs:restriction base="xs:string">
       <xs:enumeration value="IN"/>
       <xs:enumeration value="IN RANGE"/>
       <xs:enumeration value="IN ENUMERATE"/>
       <xs:enumeration value="IN ZIP"/>
@@ -136,14 +151,15 @@
       <xs:element name="for" type="For" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="if" type="If" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="try" type="Try" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="while" type="While" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="return" type="Return" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="break" type="Break" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="continue" type="Continue" minOccurs="0" maxOccurs="unbounded"/>
+      <xs:element name="error" type="Error" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="msg" type="Message" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="doc" type="xs:string" minOccurs="0"/>
       <xs:element name="status" type="BodyItemStatus"/>
     </xs:choice>
   </xs:complexType>
   <xs:complexType name="ForIterationVariable">
     <xs:simpleContent>
@@ -166,14 +182,15 @@
       <xs:element name="for" type="For" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="if" type="If" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="try" type="Try" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="while" type="While" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="return" type="Return" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="break" type="Break" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="continue" type="Continue" minOccurs="0" maxOccurs="unbounded"/>
+      <xs:element name="error" type="Error" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="msg" type="Message" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="doc" type="xs:string" minOccurs="0"/>
       <xs:element name="status" type="BodyItemStatus"/>
     </xs:choice>
     <xs:attribute name="type" type="IfType" use="required"/>
     <xs:attribute name="condition" type="xs:string"/>
   </xs:complexType>
@@ -199,14 +216,15 @@
       <xs:element name="for" type="For" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="if" type="If" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="try" type="Try" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="while" type="While" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="return" type="Return" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="break" type="Break" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="continue" type="Continue" minOccurs="0" maxOccurs="unbounded"/>
+      <xs:element name="error" type="Error" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="msg" type="Message" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="doc" type="xs:string" minOccurs="0"/>
       <xs:element name="status" type="BodyItemStatus"/>
     </xs:choice>
     <xs:attribute name="type" type="TryType" use="required"/>
     <xs:attribute name="pattern_type" type="xs:string"/>
     <xs:attribute name="variable" type="xs:string"/>
@@ -224,25 +242,29 @@
       <xs:element name="iter" type="WhileIteration" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="kw" type="Keyword" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="msg" type="Message" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="doc" type="xs:string" minOccurs="0"/>
       <xs:element name="status" type="BodyItemStatus"/>
     </xs:choice>
     <xs:attribute name="condition" type="xs:string"/>
+    <xs:attribute name="limit" type="xs:string"/>
+    <xs:attribute name="on_limit" type="xs:string"/>
+    <xs:attribute name="on_limit_message" type="xs:string"/>
   </xs:complexType>
   <xs:complexType name="WhileIteration">
     <xs:choice maxOccurs="unbounded">
       <xs:element name="kw" type="Keyword" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="for" type="For" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="if" type="If" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="try" type="Try" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="while" type="While" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="return" type="Return" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="break" type="Break" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="continue" type="Continue" minOccurs="0" maxOccurs="unbounded"/>
+      <xs:element name="error" type="Error" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="msg" type="Message" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="doc" type="xs:string" minOccurs="0"/>
       <xs:element name="status" type="BodyItemStatus"/>
     </xs:choice>
   </xs:complexType>
   <xs:complexType name="Return">
     <xs:choice maxOccurs="unbounded">
@@ -299,14 +321,15 @@
     </xs:simpleContent>
   </xs:complexType>
   <xs:simpleType name="StatusValue">
     <xs:restriction base="xs:string">
       <xs:enumeration value="PASS"/>
       <xs:enumeration value="FAIL"/>
       <xs:enumeration value="SKIP"/>
+      <xs:enumeration value="NOT RUN"/>
       <xs:enumeration value="UNKNOWN"/>
     </xs:restriction>
   </xs:simpleType>
   <xs:complexType name="BodyItemStatus">
     <xs:simpleContent>
       <xs:extension base="xs:string">
         <xs:attribute name="status" type="BodyItemStatusValue" use="required"/>
```

### Comparing `robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/PKG-INFO` & `robotframework-robotlog2db-1.3.9/robotframework_robotlog2db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robotlog2db
-Version: 1.3.8
+Version: 1.3.9
 Summary: Imports robot result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/robotframework-robotlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-robotlog2db-1.3.8/setup.py` & `robotframework-robotlog2db-1.3.9/setup.py`

 * *Files identical despite different names*

