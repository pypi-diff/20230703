# Comparing `tmp/QuantumPathQSOAPySDK-1.5.7.tar.gz` & `tmp/QuantumPathQSOAPySDK-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumPathQSOAPySDK-1.5.7.tar", last modified: Fri Jun 30 08:01:30 2023, max compression
+gzip compressed data, was "QuantumPathQSOAPySDK-1.5.8.tar", last modified: Mon Jul  3 09:00:51 2023, max compression
```

## Comparing `QuantumPathQSOAPySDK-1.5.7.tar` & `QuantumPathQSOAPySDK-1.5.8.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.529219 QuantumPathQSOAPySDK-1.5.7/
--rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.7/MANIFEST.in
--rw-rw-rw-   0        0        0      928 2023-06-30 08:01:30.528226 QuantumPathQSOAPySDK-1.5.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.167704 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/
--rw-rw-rw-   0        0        0    43170 2023-06-29 15:26:36.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/QSOAPlatform.py
--rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.220423 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/
--rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.234349 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/annealing/
--rw-rw-rw-   0        0        0     7907 2023-06-26 09:01:38.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
--rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
--rw-rw-rw-   0        0        0    28762 2023-06-27 08:12:21.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/annealing/components.py
-drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.315819 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/flow/
--rw-rw-rw-   0        0        0     4848 2023-06-26 09:03:51.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
--rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/flow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.349640 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/gates/
--rw-rw-rw-   0        0        0    53330 2023-06-27 11:39:45.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
--rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/gates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.415099 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/
--rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/Application.py
--rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/Asset.py
--rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/AssetManagementData.py
--rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
--rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/DeviceItem.py
--rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/Execution.py
--rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/FlowItem.py
--rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
--rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/SolutionItem.py
--rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.436709 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/
--rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/__init__.py
--rw-rw-rw-   0        0        0     9076 2023-06-09 09:56:38.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
--rw-rw-rw-   0        0        0    10099 2023-06-12 08:01:27.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
--rw-rw-rw-   0        0        0     4077 2023-06-13 11:39:31.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
-drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.460589 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/
--rw-rw-rw-   0        0        0     3542 2023-06-30 07:54:28.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/Context.py
--rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/Exception.py
--rw-rw-rw-   0        0        0      160 2023-06-22 10:01:20.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/__init__.py
--rw-rw-rw-   0        0        0     1514 2023-06-06 09:42:42.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/apiConnection.py
--rw-rw-rw-   0        0        0     3216 2023-06-22 11:57:59.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/checker.py
-drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.215449 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/
--rw-rw-rw-   0        0        0      928 2023-06-30 08:01:29.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2085 2023-06-30 08:01:30.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 08:01:29.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-30 08:01:29.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-30 08:01:29.000000 QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 08:01:30.530215 QuantumPathQSOAPySDK-1.5.7/setup.cfg
--rw-rw-rw-   0        0        0      973 2023-06-30 08:01:23.000000 QuantumPathQSOAPySDK-1.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.465557 QuantumPathQSOAPySDK-1.5.7/test/
--rw-rw-rw-   0        0        0       83 2023-06-30 08:00:25.000000 QuantumPathQSOAPySDK-1.5.7/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.495398 QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/__init__.py
--rw-rw-rw-   0        0        0     4601 2023-06-30 07:59:05.000000 QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_ContextMethods.py
--rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_DynamicMethods.py
--rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_QSOAPlatform.py
--rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_SecurityMethods.py
--rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_StaticMethods.py
-drwxrwxrwx   0        0        0        0 2023-06-30 08:01:30.523248 QuantumPathQSOAPySDK-1.5.7/test/test_circuit/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.7/test/test_circuit/__init__.py
--rw-rw-rw-   0        0        0   130207 2023-06-27 08:11:21.000000 QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitAnnealing.py
--rw-rw-rw-   0        0        0     8004 2023-06-26 10:45:48.000000 QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitFlow.py
--rw-rw-rw-   0        0        0     7331 2023-06-26 10:46:07.000000 QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitGates.py
--rw-rw-rw-   0        0        0   153999 2023-06-27 11:33:39.000000 QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitGates_gates1.py
--rw-rw-rw-   0        0        0    41572 2023-06-27 11:33:49.000000 QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitGates_gates2.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:00:51.069873 QuantumPathQSOAPySDK-1.5.8/
+-rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      928 2023-07-03 09:00:51.068875 QuantumPathQSOAPySDK-1.5.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 09:00:50.965752 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/
+-rw-rw-rw-   0        0        0    43350 2023-06-30 11:31:19.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/QSOAPlatform.py
+-rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:00:50.981108 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/
+-rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:00:50.989089 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/annealing/
+-rw-rw-rw-   0        0        0     7907 2023-06-26 09:01:38.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
+-rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
+-rw-rw-rw-   0        0        0    28762 2023-06-27 08:12:21.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/annealing/components.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:00:50.995072 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/flow/
+-rw-rw-rw-   0        0        0     4848 2023-06-26 09:03:51.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
+-rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/flow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:00:50.999061 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/gates/
+-rw-rw-rw-   0        0        0    53330 2023-06-27 11:39:45.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
+-rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/gates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:00:51.020012 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/
+-rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/Application.py
+-rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/Asset.py
+-rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/AssetManagementData.py
+-rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
+-rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/DeviceItem.py
+-rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/Execution.py
+-rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/FlowItem.py
+-rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
+-rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/SolutionItem.py
+-rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:00:51.030001 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/
+-rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/__init__.py
+-rw-rw-rw-   0        0        0     9869 2023-07-03 08:57:31.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
+-rw-rw-rw-   0        0        0    10579 2023-07-03 08:57:37.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
+-rw-rw-rw-   0        0        0     4296 2023-07-03 08:57:44.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:00:51.040950 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/
+-rw-rw-rw-   0        0        0     3682 2023-07-03 08:31:52.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/Context.py
+-rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/Exception.py
+-rw-rw-rw-   0        0        0      160 2023-06-22 10:01:20.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/__init__.py
+-rw-rw-rw-   0        0        0     1605 2023-06-30 10:05:23.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/apiConnection.py
+-rw-rw-rw-   0        0        0     3571 2023-06-30 12:03:18.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/checker.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:00:50.980112 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/
+-rw-rw-rw-   0        0        0      928 2023-07-03 09:00:50.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2085 2023-07-03 09:00:50.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 09:00:50.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-03 09:00:50.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-03 09:00:50.000000 QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 09:00:51.069873 QuantumPathQSOAPySDK-1.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      973 2023-07-03 09:00:42.000000 QuantumPathQSOAPySDK-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:00:51.042943 QuantumPathQSOAPySDK-1.5.8/test/
+-rw-rw-rw-   0        0        0       83 2023-07-03 08:57:13.000000 QuantumPathQSOAPySDK-1.5.8/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:00:51.053915 QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/__init__.py
+-rw-rw-rw-   0        0        0     4995 2023-07-03 08:37:49.000000 QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_ContextMethods.py
+-rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_DynamicMethods.py
+-rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_QSOAPlatform.py
+-rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_SecurityMethods.py
+-rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_StaticMethods.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:00:51.066880 QuantumPathQSOAPySDK-1.5.8/test/test_circuit/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.8/test/test_circuit/__init__.py
+-rw-rw-rw-   0        0        0   130207 2023-06-27 08:11:21.000000 QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitAnnealing.py
+-rw-rw-rw-   0        0        0     8004 2023-06-26 10:45:48.000000 QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitFlow.py
+-rw-rw-rw-   0        0        0     7331 2023-06-26 10:46:07.000000 QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitGates.py
+-rw-rw-rw-   0        0        0   153999 2023-06-27 11:33:39.000000 QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitGates_gates1.py
+-rw-rw-rw-   0        0        0    41572 2023-06-27 11:33:49.000000 QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitGates_gates2.py
```

### Comparing `QuantumPathQSOAPySDK-1.5.7/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5.7
+Version: 1.5.8
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/QSOAPlatform.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,42 +131,44 @@
         Output
         ----------
         tuple
         """
         return self.__context.getActiveEnvironment()
 
     # SET ACTIVE ENVIRONMENT
-    def setActiveEnvironment(self, environmentName: str, qSOATargetURL: str = None) -> tuple:
+    def setActiveEnvironment(self, environmentName: str, qSOATargetURL: str = None, validateCert: bool = True) -> tuple:
         """
         Set active QuantumPath environment.
 
         Prerequisites
         ----------
         Existing QuantumPath environment.
 
         Parameters
         ----------
         environmentName : str
             QuantumPath environment name to set as active.
         qSOATargetURL : str
             Optional argument. New qSOA target URL to add to existing environments and set as active.
+        validate : Optional argument. Check URL certificate for custom environment.
 
         Output
         ----------
         tuple
         """
         checkInputTypes(
-            ('environmentName', environmentName, (str,))
+            ('environmentName', environmentName, (str,)),
+            ('validateCert', validateCert, (bool,))
         )
         if qSOATargetURL:
             checkInputTypes(
                 ('qSOATargetURL', qSOATargetURL, (str,))
             )
 
-        return self.__context.setActiveEnvironment(environmentName, qSOATargetURL)
+        return self.__context.setActiveEnvironment(environmentName, qSOATargetURL, validateCert)
 
 
     ##################_____SECURITY METHODS_____##################
 
     # ENCODE PASSWORD
     def encodePassword(self, password: str):
         """
```

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/annealing/components.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/annealing/components.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/Application.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/Application.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/Asset.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/Asset.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/AssetManagementData.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/AssetManagementData.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/AssetManagementResult.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/AssetManagementResult.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/DeviceItem.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/DeviceItem.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/Execution.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/Execution.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/__init__.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/__init__.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/connectionPoints.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/connectionPoints.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ..utils.apiConnection import apiConnection
+from ..utils.checker import getURL
 from ..objects.SolutionItem import SolutionItem
 from ..objects.DeviceItem import DeviceItem
 from ..objects.FlowItem import FlowItem
 from ..objects.Application import Application
 from ..objects.Execution import Execution
 
 from matplotlib import pyplot as plt
@@ -21,17 +22,14 @@
     'runQuantumApplication': 'connectionPoint/runQuantumApplication/',
     'getQuantumExecutionResponse': 'connectionPoint/getQuantumExecutionResponse/',
     'getQuantumDevicesEx': 'connectionPoint/getQuantumDevicesEx/'
 }
 
 
 # PRIVATE METHODS
-def __getURL(context) -> str:
-    return context.getEnvironments()[context.getActiveEnvironment()[0]][context.getActiveEnvironment()[1]]
-
 def __plotQuantumGatesCircuit(histogramData: dict, name: str): # __plotQuantumGatesCircuit. Returns a plot
     histogramTitle = name
     histogramValues = histogramData[name]
 
     histogramValues = collections.OrderedDict(sorted(histogramValues.items())) # sort values
 
     fig, ax = plt.subplots(1, 1)
@@ -67,128 +65,152 @@
     return f'\n\n{histogramTitle}\n{tableInfo}\n{tableResults}'
 
 
 ##################_____STATIC METHODS_____##################
 
 # GET VERSION
 def getVersion(self, context) -> str:
-    url = __getURL(context) + connectionPoints['getVersion']
+    urlData = getURL(context)
+    url = urlData[0] + connectionPoints['getVersion']
+    validate = urlData[1]
 
-    return apiConnection(url, context.getHeader(), 'string')
+    return apiConnection(url, context.getHeader(), 'string', validate=validate)
     
 # GET LICENCE INFO
 def getLicenceInfo(self, context) -> dict:
-    url = __getURL(context) + connectionPoints['getLicenceInfo']
+    urlData = getURL(context)
+    url = urlData[0] + connectionPoints['getLicenceInfo']
+    validate = urlData[1]
 
-    return apiConnection(url, context.getHeader(), 'json')
+    return apiConnection(url, context.getHeader(), 'json', validate=validate)
 
 # GET QUANTUM SOLUTION LIST
 def getQuantumSolutionList(self, context) -> dict:
-    url = __getURL(context) + connectionPoints['getQuantumSolutions']
+    urlData = getURL(context)
+    url = urlData[0] + connectionPoints['getQuantumSolutions']
+    validate = urlData[1]
  
-    return apiConnection(url, context.getHeader(), 'json')
+    return apiConnection(url, context.getHeader(), 'json', validate=validate)
 
 # GET QUANTUM SOLUTIONS
 def getQuantumSolutions(self, context) -> list:
-    solutions = list()
+    urlData = getURL(context)
+    url = urlData[0] + connectionPoints['getQuantumSolutions']
+    validate = urlData[1]
 
-    url = __getURL(context) + connectionPoints['getQuantumSolutions']
+    solutions = []
 
-    solutionsDict = apiConnection(url, context.getHeader(), 'json')
+    solutionsDict = apiConnection(url, context.getHeader(), 'json', validate=validate)
 
     for idSolution in solutionsDict:
         solutions.append(SolutionItem(int(idSolution), solutionsDict[idSolution]))
 
     return solutions
 
 # GET QUANTUM SOLUTION NAME
 def getQuantumSolutionName(self, context, idSolution: int) -> str:
-    url = __getURL(context) + connectionPoints['getQuantumSolutions']
+    urlData = getURL(context)
+    url = urlData[0] + connectionPoints['getQuantumSolutions']
+    validate = urlData[1]
 
-    solutionsDict = apiConnection(url, context.getHeader(), 'json')
+    solutionsDict = apiConnection(url, context.getHeader(), 'json', validate=validate)
     
     if str(idSolution) in solutionsDict.keys():
         solutionName = solutionsDict[str(idSolution)]
     
     else:
         raise ValueError('Incorrect Solution ID')
 
     return solutionName
 
 # GET QUANTUM DEVICE LIST
 def getQuantumDeviceList(self, context, idSolution: int) -> dict:
-    url = __getURL(context) + connectionPoints['getQuantumDevices'] + str(idSolution)
+    urlData = getURL(context)
+    url = urlData[0] + connectionPoints['getQuantumDevices'] + str(idSolution)
+    validate = urlData[1]
 
-    return apiConnection(url, context.getHeader(), 'json')
+    return apiConnection(url, context.getHeader(), 'json', validate=validate)
 
 # GET QUANTUM DEVICES
 def getQuantumDevices(self, context, idSolution: int) -> list:
-    devices = list()
+    urlData = getURL(context)
+    url = urlData[0] + connectionPoints['getQuantumDevicesEx'] + str(idSolution)
+    validate = urlData[1]
 
-    url = __getURL(context) + connectionPoints['getQuantumDevicesEx'] + str(idSolution)
+    devices = []
 
-    devicesDict = apiConnection(url, context.getHeader(), 'json')
+    devicesDict = apiConnection(url, context.getHeader(), 'json', validate=validate)
 
     for device in devicesDict:
         devices.append(DeviceItem(device))
     
     return devices
 
 # GET QUANTUM DEVICE NAME
 def getQuantumDeviceName(self, context, idSolution: int, idDevice: int) -> str:
-    url = __getURL(context) + connectionPoints['getQuantumDevices'] + str(idSolution)
+    urlData = getURL(context)
+    url = urlData[0] + connectionPoints['getQuantumDevices'] + str(idSolution)
+    validate = urlData[1]
 
-    devicesDict = apiConnection(url, context.getHeader(), 'json')
+    devicesDict = apiConnection(url, context.getHeader(), 'json', validate=validate)
     
     if str(idDevice) in devicesDict.keys():
         deviceName = devicesDict[str(idDevice)]
     
     else:
         raise ValueError('Incorrect Device ID')
 
     return deviceName
 
 # GET QUANTUM FLOW LIST
 def getQuantumFlowList(self, context, idSolution: int) -> dict:
-    url = __getURL(context) + connectionPoints['getQuantumFlows'] + str(idSolution)
+    urlData = getURL(context)
+    url = urlData[0] + connectionPoints['getQuantumFlows'] + str(idSolution)
+    validate = urlData[1]
     
-    return apiConnection(url, context.getHeader(), 'json')
+    return apiConnection(url, context.getHeader(), 'json', validate=validate)
 
 # GET QUANTUM FLOWS
 def getQuantumFlows(self, context, idSolution: int) -> list:
-    flows = list()
+    urlData = getURL(context)
+    url = urlData[0] + connectionPoints['getQuantumFlows'] + str(idSolution)
+    validate = urlData[1]
 
-    url = __getURL(context) + connectionPoints['getQuantumFlows'] + str(idSolution)
+    flows = []
 
-    flowsDict = apiConnection(url, context.getHeader(), 'json')
+    flowsDict = apiConnection(url, context.getHeader(), 'json', validate=validate)
 
     for idFlow in flowsDict:
         flows.append(FlowItem(int(idFlow), flowsDict[idFlow]))
     
     return flows
 
 # GET QUANTUM FLOW NAME
 def getQuantumFlowName(self, context, idSolution: int, idFlow: int) -> str:
-    url = __getURL(context) + connectionPoints['getQuantumFlows'] + str(idSolution)
+    urlData = getURL(context)
+    url = urlData[0] + connectionPoints['getQuantumFlows'] + str(idSolution)
+    validate = urlData[1]
 
-    flowsDict = apiConnection(url, context.getHeader(), 'json')
+    flowsDict = apiConnection(url, context.getHeader(), 'json', validate=validate)
     
     if str(idFlow) in flowsDict.keys():
         flowName = flowsDict[str(idFlow)]
     
     else:
         raise ValueError('Incorrect Flow ID')
 
     return flowName
 
 # RUN QUANTUM APPLICATION
 def runQuantumApplication(self, context, applicationName: str, idSolution: int, idFlow: int, idDevice: int) -> Application:
-    url = __getURL(context) + connectionPoints['runQuantumApplication'] + str(applicationName) + '/' + str(idSolution) + '/' + str(idFlow) + '/' + str(idDevice)
+    urlData = getURL(context)
+    url = urlData[0] + connectionPoints['runQuantumApplication'] + str(applicationName) + '/' + str(idSolution) + '/' + str(idFlow) + '/' + str(idDevice)
+    validate = urlData[1]
 
-    executionToken = apiConnection(url, context.getHeader(), 'string')
+    executionToken = apiConnection(url, context.getHeader(), 'string', validate=validate)
 
     return Application(applicationName, int(idSolution), int(idFlow), int(idDevice), executionToken)
 
 # RUN QUANTUM APPLICATION SYNC
 def runQuantumApplicationSync(self, context, applicationName: str, idSolution: int, idFlow: int, idDevice: int) -> Application:
     application = runQuantumApplication(None, context, applicationName, idSolution, idFlow, idDevice)
 
@@ -208,17 +230,19 @@
         idFlow = args[0].getIdFlow()
     
     elif len(args) == 3:
         executionToken = args[0]
         idSolution = args[1]
         idFlow = args[2]
 
-    url = __getURL(context) + connectionPoints['getQuantumExecutionResponse'] + str(executionToken) + '/' + str(idSolution) + '/' + str(idFlow)
+    urlData = getURL(context)
+    url = urlData[0] + connectionPoints['getQuantumExecutionResponse'] + str(executionToken) + '/' + str(idSolution) + '/' + str(idFlow)
+    validate = urlData[1]
 
-    executionDict = apiConnection(url, context.getHeader(), 'json')
+    executionDict = apiConnection(url, context.getHeader(), 'json', validate=validate)
     
     return Execution(executionDict)
 
 # REPRESENT RESULTS
 def representResults(self, context, execution: Execution, resultIndex: int = None):
     representation = None
     histogramData = execution.getHistogram()
```

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ..utils.apiConnection import apiConnection
+from ..utils.checker import getURL
 from ..objects.Asset import Asset
 from ..objects.AssetManagementData import AssetManagementData
 from ..objects.AssetManagementResult import AssetManagementResult
 from ..objects.QuantumExecutionHistoryEntry import QuantumExecutionHistoryEntry
 from ..circuit.annealing.CircuitAnnealing import CircuitAnnealing
 from ..circuit.gates.CircuitGates import CircuitGates
 from ..circuit.flow.CircuitFlow import CircuitFlow
@@ -21,39 +22,39 @@
     'getAssetManagementResult': 'connectionPoint/getAssetManagementResult/',
     'publishFlow': 'connectionPoint/publishFlow/',
     'deleteAsset': 'connectionPoint/deleteAsset/',
     'getQuantumExecutionHistoric': 'connectionPoint/getQuantumExecutionHistoric/',
     'getQuantumExecutionHistoricResult': 'connectionPoint/getQuantumExecutionHistoricResult/'
 }
 
-# PRIVATE METHODS
-def __getURL(context) -> str:
-    return context.getEnvironments()[context.getActiveEnvironment()[0]][context.getActiveEnvironment()[1]]
-
 
 ##################_____DYNAMIC METHODS_____##################
 
 # GET ASSET CATALOG
 def getAssetCatalog(self, context, idSolution: int, assetType: str, assetLevel: str) -> list:
-    assetCatalog = list()
+    urlData = getURL(context)
+    url = urlData[0] + dynamicExtensions['getAssetCatalog'] + str(idSolution) + '/' + assetType + '/' + assetLevel
+    validate = urlData[1]
 
-    url = __getURL(context) + dynamicExtensions['getAssetCatalog'] + str(idSolution) + '/' + assetType + '/' + assetLevel
+    assetCatalog = []
 
-    assetCatalogList = apiConnection(url, context.getHeader(), 'json')
+    assetCatalogList = apiConnection(url, context.getHeader(), 'json', validate=validate)
 
     for asset in assetCatalogList:
         assetCatalog.append(Asset(asset))
 
     return assetCatalog
 
 # GET ASSET
 def getAsset(self, context, idAsset: int, assetType: str, assetLevel: str) -> Asset:
-    url = __getURL(context) + dynamicExtensions['getAsset'] + str(idAsset) + '/' + assetType + '/' + assetLevel
+    urlData = getURL(context)
+    url = urlData[0] + dynamicExtensions['getAsset'] + str(idAsset) + '/' + assetType + '/' + assetLevel
+    validate = urlData[1]
 
-    assetResponse = apiConnection(url, context.getHeader(), 'json')
+    assetResponse = apiConnection(url, context.getHeader(), 'json', validate=validate)
     
     return Asset(assetResponse)
 
 # CREATE ASSET
 def createAsset(self, context, idSolution: int, assetName: str, assetNamespace: str, assetDescription: str, assetBody, assetType: str,
                 assetLevel: str) -> AssetManagementData:
     if isinstance(assetBody, (CircuitGates, CircuitAnnealing, CircuitFlow)):
@@ -66,17 +67,19 @@
         "AssetDescription": assetDescription,
         "AssetBody": base64.b64encode(assetBody.encode('ascii')).decode('ascii'),
         "AssetType": assetType,
         "AssetLevel": assetLevel,
         "AssetLastUpdate": ''
     }
 
-    url = __getURL(context) + dynamicExtensions['createAsset'] + str(idSolution)
+    urlData = getURL(context)
+    url = urlData[0] + dynamicExtensions['createAsset'] + str(idSolution)
+    validate = urlData[1]
     
-    assetManagementDataResult = apiConnection(url, context.getHeader(), str(newAsset), 'json', 'data')
+    assetManagementDataResult = apiConnection(url, context.getHeader(), str(newAsset), 'json', 'data', validate=validate)
 
     return AssetManagementData(assetManagementDataResult)
 
 # CREATE ASSET SYNC
 def createAssetSync(self, context, idSolution: int, assetName: str, assetNamespace: str, assetDescription: str, assetBody, assetType: str,
                     assetLevel: str) -> AssetManagementResult:
 
@@ -110,17 +113,19 @@
         time.sleep(1)
         assetManagementResult = getAssetManagementResult(None, context, assetManagementData.getLifecycleToken())
 
     return assetManagementResult
 
 # PUBLISH FLOW
 def publishFlow(self, context, idFlow: int, publish: bool) -> bool:
-    url = __getURL(context) + dynamicExtensions['publishFlow'] + str(idFlow) + '/' + str(publish)
-    
-    apiConnection(url, context.getHeader(), 'string')
+    urlData = getURL(context)
+    url = urlData[0] + dynamicExtensions['publishFlow'] + str(idFlow) + '/' + str(publish)
+    validate = urlData[1]
+
+    apiConnection(url, context.getHeader(), 'string', validate=validate)
     
     return publish
 
 # UPDATE ASSET
 def updateAsset(self, context, asset: Asset, assetName: str = None, assetNamespace: str = None, assetDescription: str = None, assetBody = None,
                 assetType: str = None, assetLevel: str = None) -> AssetManagementData:
     
@@ -146,17 +151,19 @@
         "AssetDescription": asset.getDescription() if asset.getDescription() else '',
         "AssetBody": base64.b64encode(asset.getBody().encode('ascii')).decode('ascii'),
         "AssetType": asset.getType(),
         "AssetLevel": asset.getLevel(),
         "AssetLastUpdate": asset.getLastUpdate()
     }
     
-    url = __getURL(context) + dynamicExtensions['updateAsset']
+    urlData = getURL(context)
+    url = urlData[0] + dynamicExtensions['updateAsset']
+    validate = urlData[1]
 
-    assetManagementDataResult = apiConnection(url, context.getHeader(), str(newAsset), 'json', 'data')
+    assetManagementDataResult = apiConnection(url, context.getHeader(), str(newAsset), 'json', 'data', validate=validate)
     
     return AssetManagementData(assetManagementDataResult)
 
 # UPDATE ASSET SYNC
 def updateAssetSync(self, context, asset: Asset, assetName: str = None, assetNamespace: str = None, assetDescription: str = None, assetBody = None,
                     assetType: str = None, assetLevel: str = None) -> AssetManagementResult:
 
@@ -167,17 +174,19 @@
         time.sleep(1)
         assetManagementResult = getAssetManagementResult(None, context, assetManagementData.getLifecycleToken())
 
     return assetManagementResult
 
 # GET ASSET MANAGEMENT RESULT
 def getAssetManagementResult(self, context, lifecycleToken: str) -> AssetManagementResult:
-    url = __getURL(context) + dynamicExtensions['getAssetManagementResult'] + str(lifecycleToken)
+    urlData = getURL(context)
+    url = urlData[0] + dynamicExtensions['getAssetManagementResult'] + str(lifecycleToken)
+    validate = urlData[1]
 
-    assetManagementResult = apiConnection(url, context.getHeader(), 'json')
+    assetManagementResult = apiConnection(url, context.getHeader(), 'json', validate=validate)
 
     return AssetManagementResult(assetManagementResult)
 
 # DELETE ASSET
 def deleteAsset(self, context, *args) -> bool:
     if len(args) == 1:
         idAsset = str(args[0].getId())
@@ -186,40 +195,45 @@
             assetType = args[0].getType()
         else:
             assetType = 'CIRCUIT'
 
     else:
         idAsset = str(args[0])
         assetType = str(args[1])
-        
-    url = __getURL(context) + dynamicExtensions['deleteAsset'] + idAsset + '/' + assetType
 
-    return apiConnection(url, context.getHeader(), 'boolean')
+    urlData = getURL(context)
+    url = urlData[0] + dynamicExtensions['deleteAsset'] + idAsset + '/' + assetType
+    validate = urlData[1]
+
+    return apiConnection(url, context.getHeader(), 'boolean', validate=validate)
 
 # GET QUANTUM EXECUTION HISTORIC
 def getQuantumExecutionHistoric(self, context, idSolution: int = None, idFlow: int = None, idDevice: int = None, dateFrom: str = None, isSimulator: bool = None,
                                 top: int = None, resultType: bool = None) -> list:
 
     quantumExecutionHistoric = list()
 
     if dateFrom:
         t0 = datetime(1, 1, 1)
         now = datetime.strptime(dateFrom, '%Y-%m-%dT%H:%M:%S')
         seconds = (now - t0).total_seconds()
         dateFrom = int(seconds * 10**7)
-        
-    url = __getURL(context) + dynamicExtensions['getQuantumExecutionHistoric'] + str(idSolution) + '/' + str(idFlow) + '/' + str(idDevice) + '/' + str(dateFrom) + '/' + str(isSimulator) + '/' + str(top) + '/' + str(resultType)
 
-    quantumExecutionHistoricList = apiConnection(url, context.getHeader(), 'json')
+    urlData = getURL(context)
+    url = urlData[0] + dynamicExtensions['getQuantumExecutionHistoric'] + str(idSolution) + '/' + str(idFlow) + '/' + str(idDevice) + '/' + str(dateFrom) + '/' + str(isSimulator) + '/' + str(top) + '/' + str(resultType)
+    validate = urlData[1]
+
+    quantumExecutionHistoricList = apiConnection(url, context.getHeader(), 'json', validate=validate)
 
     for quantumExecutionHistoryEntry in quantumExecutionHistoricList:
         quantumExecutionHistoric.append(QuantumExecutionHistoryEntry(quantumExecutionHistoryEntry))
 
     return quantumExecutionHistoric
 
 def getQuantumExecutionHistoricResult(self, context, idResult: int) -> QuantumExecutionHistoryEntry: # getQuantumExecutionHistoricResult. Returns a QuantumExecutionHistoryEntry object
+    urlData = getURL(context)
+    url = urlData[0] + dynamicExtensions['getQuantumExecutionHistoricResult'] + str(idResult)
+    validate = urlData[1]
 
-    url = __getURL(context) + dynamicExtensions['getQuantumExecutionHistoricResult'] + str(idResult)
-
-    quantumExecutionHistoricResultList = apiConnection(url, context.getHeader(), 'json')
+    quantumExecutionHistoricResultList = apiConnection(url, context.getHeader(), 'json', validate=validate)
             
     return QuantumExecutionHistoryEntry(quantumExecutionHistoricResultList[0])
```

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ..utils.apiConnection import apiConnection
+from ..utils.checker import getURL
 from ..utils.Exception import (ConfigFileError, Base64Error)
 
 import base64
 import hashlib
 from pathlib import Path
 from configparser import ConfigParser
 
@@ -32,17 +33,14 @@
 def __decodePassword(password: str) -> str:
     try:
         return base64.b64decode(password).decode('utf-8')
     
     except:
         raise Base64Error('Invalid Base64 encoding in password')
 
-def __getURL(context) -> str:
-    return context.getEnvironments()[context.getActiveEnvironment()[0]][context.getActiveEnvironment()[1]]
-
 
 ##################_____SECURITY METHODS_____##################
 
 # ENCODE PASSWORD
 def encodePassword(self, password: str):
     encoded_bytes = base64.b64encode(password.encode('utf-8'))
     encoded_password = encoded_bytes.decode('utf-8')
@@ -53,15 +51,16 @@
 def encryptPassword(self, password: str):
     hashed_password = hashlib.sha256(password.encode('utf-8')).hexdigest()
     
     return hashed_password
 
 # AUTHENTICATE BASIC
 def authenticateBasic(self, context, username: str = None, password: str = None) -> bool:
-    url = __getURL(context) + securityEndpoints['authenticate']
+    urlData = getURL(context)
+    url = (urlData[0] + securityEndpoints['authenticate'], urlData[1])
 
     if not username and not password:
         credentials = __getCredentialsFromConfigFile(context)
         username = credentials[0]
         password = credentials[1]
 
     elif not username or not password:
@@ -69,15 +68,16 @@
 
     context.updateContext(username, password, url)
 
     return True
 
 # AUTHENTICATE
 def authenticate(self, context, username: str = None, password: str = None) -> bool:
-    url = __getURL(context) + securityEndpoints['authenticate']
+    urlData = getURL(context)
+    url = (urlData[0] + securityEndpoints['authenticate'], urlData[1])
 
     if not username and not password:
         credentials = __getCredentialsFromConfigFile(context)
         username = credentials[0]
         password = credentials[1]
         
     elif not username or not password:
@@ -88,15 +88,16 @@
 
     context.updateContext(username, password, url)
 
     return True
 
 # AUTHENTICATE EX
 def authenticateEx(self, context, username: str = None, password: str = None) -> bool:
-    url = __getURL(context) + securityEndpoints['authenticateEx']
+    urlData = getURL(context)
+    url = (urlData[0] + securityEndpoints['authenticateEx'], urlData[1])
 
     if not username and not password:
         credentials = __getCredentialsFromConfigFile(context)
         username = credentials[0]
         password = credentials[1]
 
     elif not username or not password:
@@ -104,22 +105,28 @@
 
     context.updateContext(username, password, url)
 
     return True
 
 # ECHOPING
 def echoping(self, context) -> bool:
-    url = __getURL(context) + securityEndpoints['echoping']
+    urlData = getURL(context)
+    url = urlData[0] + securityEndpoints['echoping']
+    validate = urlData[1]
     
-    return apiConnection(url, 'boolean')
+    return apiConnection(url, 'boolean', validate=validate)
 
 # ECHOSTATUS
 def echostatus(self, context) -> bool:
-    url = __getURL(context) + securityEndpoints['echostatus']
+    urlData = getURL(context)
+    url = urlData[0] + securityEndpoints['echostatus']
+    validate = urlData[1]
 
-    return apiConnection(url, context.getHeader(), 'boolean')
+    return apiConnection(url, context.getHeader(), 'boolean', validate=validate)
 
 # ECHOUSER
 def echouser(self, context) -> str:
-    url = __getURL(context) + securityEndpoints['echouser']
+    urlData = getURL(context)
+    url = urlData[0] + securityEndpoints['echouser']
+    validate = urlData[1]
 
-    return apiConnection(url, context.getHeader(), 'string')
+    return apiConnection(url, context.getHeader(), 'string', validate=validate)
```

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/Context.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/Context.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,45 +3,46 @@
 from pathlib import Path
 from configparser import ConfigParser
 
 
 class Context:
 
     # CONSTRUCTOR
-    def __init__(self, username: str = None, password: str = None, url: str = None):
-        customEnvironments = []
+    def __init__(self, username: str = None, password: str = None, url: tuple = None):
+        self.__environments = {
+            'default-environments': {
+                'pro': 'https://qsoa.quantumpath.app:8443/api/'
+            },
+            'custom-environments': {}
+        }
 
         qpathFile = ConfigParser(allow_no_value=True)
         qpathFileExists = qpathFile.read(str(Path.home()) + '\.qpath')
 
         if qpathFileExists:
             self.__activeEnvironment = eval(qpathFile.options('active-environment')[0])
+
             for key in qpathFile['custom-environments']:
-                value = qpathFile['custom-environments'][key]
+                value = eval(qpathFile['custom-environments'][key])
 
-                if value[len(value)-1] != '/':
-                    value = value + '/'
+                if value[0][len(value)-1] != '/':
+                    urlDirection = value[0] + '/'
+                else:
+                    urlDirection = value[0]
 
-                customEnvironments.append((key, value))
+                self.__environments['custom-environments'][key] = (urlDirection, value[1])
         else:
             self.__activeEnvironment = ('default-environments', 'pro')
 
-        self.__environments = {
-            'default-environments': {
-                'pro': 'https://qsoa.quantumpath.app:8443/api/'
-            },
-            'custom-environments': dict(customEnvironments)
-        }
-
         self.__credentials = {
             "Username": username,
             "Password": password
         } if username else None
 
-        self.__authToken = apiConnection(url, self.__credentials, 'string', 'data') if username else None
+        self.__authToken = apiConnection(url[0], self.__credentials, 'string', 'data', validate=url[1]) if username else None
 
         self.__header = {
             "Authorization": 'Bearer ' + str(self.__authToken)
         } if username else None
 
 
     # GETTERS
@@ -54,44 +55,44 @@
     def getHeader(self) -> dict:
         return self.__header
 
 
     ##################_____METHODS_____##################
 
     # UPDATE CONTEXT
-    def updateContext(self, username: str, password: str, url: str):
+    def updateContext(self, username: str, password: str, url: tuple):
         self.__credentials = {
             "Username": username,
             "Password": password
         }
 
-        self.__authToken = apiConnection(url, self.__credentials, 'string', 'data')
+        self.__authToken = apiConnection(url[0], self.__credentials, 'string', 'data', validate=url[1])
 
         self.__header = {
             "Authorization": 'Bearer ' + str(self.__authToken)
         }
 
     # GET ENVIRONMENTS
     def getEnvironments(self) -> dict:
         return self.__environments
 
     # GET ACTIVE ENVIRONMENT
     def getActiveEnvironment(self) -> tuple:
         return self.__activeEnvironment
 
     # SET ACTIVE ENVIRONMENT
-    def setActiveEnvironment(self, environmentName: str, qSOATargetURL: str = None) -> tuple:
+    def setActiveEnvironment(self, environmentName: str, qSOATargetURL: str, validateCert: bool) -> tuple:
         if qSOATargetURL:
             if environmentName in self.__environments['default-environments']:
                 raise ValueError(f'Environment not valid, default-environments cannot be changed. Active environment is still {self.__activeEnvironment}')
 
             if qSOATargetURL[len(qSOATargetURL)-1] != '/':
                 qSOATargetURL = qSOATargetURL + '/'
 
-            self.__environments['custom-environments'][environmentName] = qSOATargetURL
+            self.__environments['custom-environments'][environmentName] = (qSOATargetURL, validateCert)
 
         if environmentName in self.__environments['default-environments']:
             newActiveEnvironment = ('default-environments', environmentName)
         
         elif environmentName in self.__environments['custom-environments']:
             newActiveEnvironment = ('custom-environments', environmentName)
```

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/Exception.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/Exception.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/apiConnection.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/apiConnection.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,22 +20,22 @@
                 desMessage = json.loads(desMessage)
 
     else:
         raise APIConnectionError(f'Error {message.status_code} {message.reason}. {message.text}')
 
     return desMessage
 
-def apiConnection(*args): # manage api calls
+def apiConnection(*args, validate: bool = True): # manage api calls
     if len(args) == 2: # echoping
-        response = __deserialize(requests.get(args[0]), args[1])
+        response = __deserialize(requests.get(args[0], verify=validate), args[1])
     
     elif len(args) == 3: # normal get calls
-        response = __deserialize(requests.get(args[0], headers=args[1]), args[2])
+        response = __deserialize(requests.get(args[0], headers=args[1], verify=validate), args[2])
     
     elif len(args) == 4: # create context
-        response = __deserialize(requests.post(args[0], data=args[1]), args[2])
+        response = __deserialize(requests.post(args[0], data=args[1], verify=validate), args[2])
     
     elif len(args) == 5: # post asset
         args[1].update({'Content-type': 'application/json; charset=utf-8'})
-        response = __deserialize(requests.post(args[0], headers=args[1], data=args[2].encode('utf-8')), args[3])
+        response = __deserialize(requests.post(args[0], headers=args[1], data=args[2].encode('utf-8'), verify=validate), args[3])
     
     return response
```

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK/utils/checker.py` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK/utils/checker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 from ..utils.apiConnection import apiConnection
 from .Exception import AuthenticationError
 
 import math
 
-def getURL(context) -> str:
-    return context.getEnvironments()[context.getActiveEnvironment()[0]][context.getActiveEnvironment()[1]]
+def getURL(context) -> tuple:
+    if context.getActiveEnvironment()[0] == 'default-environments':
+        url = (context.getEnvironments()[context.getActiveEnvironment()[0]][context.getActiveEnvironment()[1]], True)
+
+    elif context.getActiveEnvironment()[0] == 'custom-environments':
+        url = context.getEnvironments()[context.getActiveEnvironment()[0]][context.getActiveEnvironment()[1]]
+
+    return url
 
 def depth(inputList):
     if isinstance(inputList, list):
         return 1 + max(depth(item) for item in inputList)
     else:
         return 0
 
 def checkUserSession(context):
-    url = getURL(context) + 'login/echostatus'
+    urlData = getURL(context)
+    url = urlData[0] + 'login/echostatus'
+    validate = urlData[1]
 
-    if not apiConnection(url, context.getHeader(), 'boolean'):
+    if not apiConnection(url, context.getHeader(), 'boolean', validate=validate):
         raise AuthenticationError('User not authenticated')
 
 def checkInputTypes(*args):
     for arg in args:
         name = arg[0]
         variable = arg[1]
         types = arg[2]
```

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5.7
+Version: 1.5.8
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5.7/QuantumPathQSOAPySDK.egg-info/SOURCES.txt` & `QuantumPathQSOAPySDK-1.5.8/QuantumPathQSOAPySDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/setup.py` & `QuantumPathQSOAPySDK-1.5.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   'Intended Audience :: Developers',
   'Intended Audience :: Education',
   'Intended Audience :: Information Technology'
 ]
 
 setup(
   name='QuantumPathQSOAPySDK',
-  version='1.5.7',
+  version='1.5.8',
   description='QuantumPath qSOA Python SDK',
   long_description=open('README.md').read(),
   long_description_content_type = 'text/markdown',
   url='https://core.quantumpath.app/',
   author='QuantumPath',
   classifiers=classifiers,
   keywords='quantum, quantumpath, qSOA, sdk, quantum applications, quantum software',
```

### Comparing `QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_ContextMethods.py` & `QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_ContextMethods.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,44 +56,44 @@
         self.assertIsInstance(setActiveEnvironment, tuple)
         self.assertEqual(setActiveEnvironment, ('default-environments', 'pro'))
     
     # SET ACTIVE ENVIRONMENT qSOATargetURL SLASH
     def test_setActiveEnvironment_qSOATargetURL_slash(self):
         qsoa = QSOAPlatform()
 
-        setActiveEnvironment = qsoa.setActiveEnvironment('custom', 'url/')
+        setActiveEnvironment = qsoa.setActiveEnvironment('custom', 'url/', True)
 
         customEnvironments = qsoa.getEnvironments()['custom-environments']
 
-        self.assertEqual(customEnvironments, {'custom': 'url/'})
+        self.assertEqual(customEnvironments, {'custom': ('url/', True)})
         self.assertIsInstance(setActiveEnvironment, tuple)
         self.assertEqual(setActiveEnvironment, ('custom-environments', 'custom'))
 
     # SET ACTIVE ENVIRONMENT qSOATargetURL NO SLASH
     def test_setActiveEnvironment_qSOATargetURL_noSlash(self):
         qsoa = QSOAPlatform()
 
-        setActiveEnvironment = qsoa.setActiveEnvironment('custom', 'url')
+        setActiveEnvironment = qsoa.setActiveEnvironment('custom', 'url', True)
 
         customEnvironments = qsoa.getEnvironments()['custom-environments']
 
-        self.assertEqual(customEnvironments, {'custom': 'url/'})
+        self.assertEqual(customEnvironments, {'custom': ('url/', True)})
         self.assertIsInstance(setActiveEnvironment, tuple)
         self.assertEqual(setActiveEnvironment, ('custom-environments', 'custom'))
 
     # SET ACTIVE ENVIRONMENT qSOATargetURL OVERRIDE
     def test_setActiveEnvironment_qSOATargetURL_override(self):
         qsoa = QSOAPlatform()
         qsoa.setActiveEnvironment('custom', 'url')
 
-        setActiveEnvironment = qsoa.setActiveEnvironment('custom', 'url2')
+        setActiveEnvironment = qsoa.setActiveEnvironment('custom', 'url2', True)
 
         customEnvironments = qsoa.getEnvironments()['custom-environments']
 
-        self.assertEqual(customEnvironments, {'custom': 'url2/'})
+        self.assertEqual(customEnvironments, {'custom': ('url2/', True)})
         self.assertIsInstance(setActiveEnvironment, tuple)
         self.assertEqual(setActiveEnvironment, ('custom-environments', 'custom'))
 
     # BAD ARGUMENT environmentName
     def test_setActiveEnvironment_badArgument_environmentName(self):
         qsoa = QSOAPlatform()
 
@@ -105,15 +105,15 @@
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT qSOATargetURL DEFAULT
     def test_setActiveEnvironment_badArgument_qSOATargetURL_default(self):
         qsoa = QSOAPlatform()
 
         try:
-            qsoa.setActiveEnvironment('pro', 'url')
+            qsoa.setActiveEnvironment('pro', 'url', True)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE environmentName
     def test_setActiveEnvironment_badArgumentType_environmentName(self):
@@ -122,10 +122,21 @@
         try:
             qsoa.setActiveEnvironment(0)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
+    # BAD ARGUMENT TYPE qSOATargetURL
+    def test_setActiveEnvironment_badArgumentType_qSOATargetURL(self):
+        qsoa = QSOAPlatform()
+
+        try:
+            qsoa.setActiveEnvironment('custom', 'url2', 'qSOATargetURL')
+            raise Exception
+
+        except Exception as e:
+            self.assertIsInstance(e, TypeError)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_DynamicMethods.py` & `QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_DynamicMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_QSOAPlatform.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_SecurityMethods.py` & `QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_SecurityMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/test/test_QSOAPlatform/test_StaticMethods.py` & `QuantumPathQSOAPySDK-1.5.8/test/test_QSOAPlatform/test_StaticMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitAnnealing.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitGates.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitGates_gates1.py` & `QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitGates_gates1.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.7/test/test_circuit/test_CircuitGates_gates2.py` & `QuantumPathQSOAPySDK-1.5.8/test/test_circuit/test_CircuitGates_gates2.py`

 * *Files identical despite different names*

