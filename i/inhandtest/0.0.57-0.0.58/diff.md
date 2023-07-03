# Comparing `tmp/inhandtest-0.0.57.tar.gz` & `tmp/inhandtest-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.57.tar", last modified: Wed Jun 21 05:35:38 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.58.tar", last modified: Mon Jul  3 10:26:48 2023, max compression
```

## Comparing `inhandtest-0.0.57.tar` & `inhandtest-0.0.58.tar`

### file list

```diff
@@ -1,64 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.57/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-06-21 05:35:38.000000 inhandtest-0.0.57/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.57/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/dm/
--rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.57/dm/mqtt.py
--rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.57/dm/register_v1.py
-drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.57/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/base_page/
--rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.57/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    40087 2023-06-07 07:00:46.000000 inhandtest-0.0.57/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.57/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.57/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    57431 2023-06-15 06:06:07.000000 inhandtest-0.0.57/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    23845 2023-06-15 06:06:07.000000 inhandtest-0.0.57/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.57/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3971 2023-06-16 00:48:06.000000 inhandtest-0.0.57/inhandtest/file.py
--rw-rw-rw-   0        0        0    10907 2023-06-15 06:06:07.000000 inhandtest-0.0.57/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.57/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22019 2023-06-15 06:06:07.000000 inhandtest-0.0.57/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    71913 2023-06-21 03:57:22.000000 inhandtest-0.0.57/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     8072 2023-06-20 09:32:40.000000 inhandtest-0.0.57/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    14792 2023-06-15 06:12:16.000000 inhandtest-0.0.57/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.57/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.57/inhandtest/ip.py
--rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.57/inhandtest/log.py
--rw-rw-rw-   0        0        0    13757 2023-06-15 05:47:54.000000 inhandtest-0.0.57/inhandtest/mail.py
--rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.57/inhandtest/notice_email.html
-drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/pages/
--rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.57/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0     8879 2023-06-02 05:53:59.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0     9486 2023-06-02 05:59:32.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     3057 2023-06-14 06:26:03.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0     8694 2023-06-08 08:54:15.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0    67657 2023-06-12 05:25:10.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    86112 2023-06-12 05:18:58.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/network/network_locators.py
-drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/overview/overview_locators.py
-drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/system/
--rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/system/__init__.py
--rw-rw-rw-   0        0        0    28496 2023-06-08 09:58:25.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/system/system.py
--rw-rw-rw-   0        0        0    30624 2023-06-08 09:03:50.000000 inhandtest-0.0.57/inhandtest/pages/ingateway/system/system_locators.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.57/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    34699 2023-06-20 09:30:58.000000 inhandtest-0.0.57/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    28008 2023-06-15 06:16:19.000000 inhandtest-0.0.57/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1685 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-21 05:35:38.000000 inhandtest-0.0.57/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.57/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 05:35:38.000000 inhandtest-0.0.57/setup.cfg
--rw-rw-rw-   0        0        0     1615 2023-06-21 05:35:26.000000 inhandtest-0.0.57/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.58/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-07-03 10:26:48.000000 inhandtest-0.0.58/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.58/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.58/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.58/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    43260 2023-07-03 08:13:32.000000 inhandtest-0.0.58/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.58/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.58/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    64740 2023-06-29 08:46:46.000000 inhandtest-0.0.58/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    25320 2023-06-29 01:54:01.000000 inhandtest-0.0.58/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.58/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3971 2023-06-16 00:48:06.000000 inhandtest-0.0.58/inhandtest/file.py
+-rw-rw-rw-   0        0        0    10907 2023-06-15 06:06:07.000000 inhandtest-0.0.58/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.58/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.58/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    71861 2023-07-03 01:50:04.000000 inhandtest-0.0.58/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.58/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    14831 2023-07-03 08:50:33.000000 inhandtest-0.0.58/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.58/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.58/inhandtest/ip.py
+-rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.58/inhandtest/log.py
+-rw-rw-rw-   0        0        0    13757 2023-06-15 05:47:54.000000 inhandtest-0.0.58/inhandtest/mail.py
+-rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.58/inhandtest/notice_email.html
+drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.58/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0    63438 2023-07-03 08:16:21.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0    65044 2023-07-03 07:08:34.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     3195 2023-06-30 06:11:59.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0    11128 2023-06-30 03:20:05.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0    67807 2023-06-26 05:24:31.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    86201 2023-06-26 05:24:31.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/network/network_locators.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/overview/overview_locators.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/system/
+-rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/system/__init__.py
+-rw-rw-rw-   0        0        0    28514 2023-06-26 05:24:31.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/system/system.py
+-rw-rw-rw-   0        0        0    30656 2023-06-26 05:24:31.000000 inhandtest-0.0.58/inhandtest/pages/ingateway/system/system_locators.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.58/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    34699 2023-06-20 09:30:58.000000 inhandtest-0.0.58/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    28118 2023-07-03 02:25:51.000000 inhandtest-0.0.58/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1656 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-03 10:26:48.000000 inhandtest-0.0.58/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.58/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 10:26:48.000000 inhandtest-0.0.58/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2023-07-03 10:26:35.000000 inhandtest-0.0.58/setup.py
```

### Comparing `inhandtest-0.0.57/PKG-INFO` & `inhandtest-0.0.58/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.57
+Version: 0.0.58
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.57/README.md` & `inhandtest-0.0.58/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.58/inhandtest/base_page/_ig_contents_locators.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
                                    'acl': 'ACL', 'nat': 'NAT',
                                    'status': 'Status', 'l2tp_client': 'L2TP Client',
                                    'l2tp_service': 'L2TP Service',
                                    'edge': 'Edge Computing', 'python_edge': 'Python Edge Computing',
                                    'docker_manager': 'Docker Manager', 'cloud_edge_computing': 'Cloud Edge Computing',
                                    'device_supervisor': 'Device Supervisor', 'measure_monitor': 'Measure Monitor',
                                    'monitoring_list': 'Monitoring List', 'group': 'Group',
+                                   'controller_template': 'Controller Template',
                                    'alarm': 'Alarm', 'realtime_alarms': 'Realtime Alarms', 'alarm_rules': 'Alarm Rules',
                                    'history_alarms': 'History Alarms', 'alarm_label': 'Alarm Label',
                                    'cloud': 'Cloud', 'mqtt_cloud_service': 'MQTT Cloud Service',
                                    'whitehawk_energy_manager': 'Whitehawk Energy Manager', 'protocol': 'Protocol',
                                    'parameter_settings': 'Parameter Settings',
                                    'custom_quickfunctions': 'Custom QuickFunctions',
                                    'system': 'System', 'system_time': 'System Time', 'system_log': 'Log',
@@ -51,15 +52,18 @@
                                    'system_config': 'Configuration Management', 'system_cloud': 'InHand Cloud',
                                    'system_firmware': 'Firmware Upgrade', 'system_tools': 'Access Tools',
                                    'system_user_management': 'User Management', 'system_reboot': 'Reboot',
                                    'system_network_tools': 'Network Tools',
                                    'system_3rd_party': '3rd Party Notification',
                                    'configuration': ' Configuration', 'trigger_condition': 'Trigger Condition',
                                    'gigabitethernet': 'Gigabitethernet', 'flow_usage_day': 'Flow Usage Monitoring(Day)',
-                                   'flow_usage_month': 'Flow Usage Monitoring(Month)'
+                                   'flow_usage_month': 'Flow Usage Monitoring(Month)',
+                                   'cloud_measuring_point_setting': 'Cloud Measuring Point Setting',
+                                   'cloud_measuring_point': 'Cloud Measuring Point',
+                                   'Muting_measuring_point': 'Muting Measuring Point',
                                    }
         else:
             self.__locale: dict = {'network': '网络', 'network_interface': '网络接口', 'performance': '性能与存储',
                                    'cellular': '蜂窝网', 'ethernet': '以太网',
                                    'bridge': '桥接口', 'loopback': '环回接口',
                                    'network_service': '网络服务', 'dhcp': 'DHCP服务',
                                    'dns': 'DNS服务', "gps_configure": "GPS 配置", 'gps': 'GPS',
@@ -68,28 +72,32 @@
                                    'routing': '路由', 'routing_status': '路由状态',
                                    'routing_static': '静态路由', 'firewall': '防火墙',
                                    'acl': '访问控制列表', 'nat': '网络地址转换',
                                    'status': '状态', 'l2tp_client': 'L2TP客户端', 'l2tp_service': 'L2TP服务器',
                                    'edge': '边缘计算', 'python_edge': 'Python边缘计算', 'docker_manager': 'Docker 管理',
                                    'cloud_edge_computing': '公有云边缘计算', 'device_supervisor': '设备监控',
                                    'measure_monitor': '测点监控', 'monitoring_list': '监控列表', 'group': '分组',
+                                   'controller_template': '控制器模板',
                                    'alarm': '告警', 'realtime_alarms': '实时告警', 'alarm_rules': '告警规则',
                                    'history_alarms': '历史告警', 'alarm_label': '告警标签',
                                    'cloud': '云服务', 'mqtt_cloud_service': 'MQTT云服务',
                                    'whitehawk_energy_manager': '白鹰能源管家', 'protocol': '协议转换',
                                    'parameter_settings': '参数设置', 'custom_quickfunctions': '自定义快函数',
                                    'system': '系统管理', 'system_time': '系统时间', 'system_log': '系统日志',
                                    'clear_history_log': '清除历史日志',
                                    'system_config': '配置管理', 'system_cloud': '设备云平台',
                                    'system_firmware': '固件升级', 'system_tools': '管理工具',
                                    'system_user_management': '用户管理', 'system_reboot': '重启',
                                    'system_network_tools': '工具', 'system_3rd_party': '第三方软件声明',
                                    'configuration': '配置',
                                    'trigger_condition': '触发条件', 'gigabitethernet': '千兆以太网口',
-                                   'flow_usage_day': '流量使用监测（当天）', 'flow_usage_month': '流量使用监测（当月）'
+                                   'flow_usage_day': '流量使用监测（当天）', 'flow_usage_month': '流量使用监测（当月）',
+                                   'cloud_measuring_point_setting': '上云测点设置',
+                                   'cloud_measuring_point': '上云测点',
+                                   'Muting_measuring_point': '屏蔽测点',
                                    }
 
     def content_target(self, locale) -> Locator:
         if self.__locale.get(locale):
             locale = self.__locale.get(locale)
         return self.page.locator(f'//span[@class="ant-breadcrumb-link"]/span[text()="{locale}"]')
 
@@ -513,14 +521,21 @@
                         'group': {
                             'menu': self.page.locator(f'div:text-is("{self.__locale.get("group")}")'),
                             'attributes': {
                                 self.page.locator(f'div:text-is("{self.__locale.get("group")}")'): {
                                     'aria-selected': 'true'}},
                             'wait_locator': [self.page.locator('//i[@class="anticon anticon-plus-circle"]')],
                         },
+                        'controller_template': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("controller_template")}")'),
+                            'attributes': {
+                                self.page.locator(f'div:text-is("{self.__locale.get("controller_template")}")'): {
+                                    'aria-selected': 'true'}},
+                            'wait_locator': [self.page.locator('.ant-table-header.ant-table-hide-scrollbar')],
+                        },
                     },
                     'alarm': {
                         'default': 'realtime_alarms',
                         'menu': self.alarm_menu,
                         'visible_locator': [self.content_target('alarm')],
                         'wait_locator': [self.content_target('alarm')],
                         'realtime_alarms': {
@@ -559,15 +574,42 @@
                         'visible_locator': [self.content_target('cloud')],
                         'wait_locator': [self.content_target('cloud')],
                         'mqtt_cloud_service': {
                             'menu': self.page.locator(f'div:text-is("{self.__locale.get("mqtt_cloud_service")}")'),
                             'attributes': {
                                 self.page.locator(f'div:text-is("{self.__locale.get("mqtt_cloud_service")}")'): {
                                     'aria-selected': 'true'}},
-                            'wait_locator': [self.page.locator('//label[@for="enable.form"]')]
+                            'wait_locator': [self.page.locator('//label[@for="enable.form"]')],
+                            'cloud_measuring_setting': {
+                                'menu': self.page.locator('//i[@class="anticon"]').first,
+                                'visible_locator': [self.page.locator('.ant-modal-title', has_text=self.__locale.get(
+                                    'cloud_measuring_point_setting'))],
+                                'wait_locator': [self.page.locator('.ant-modal-content').locator('.ant-table-content')],
+                                'cloud': {
+                                    'menu': self.page.locator(
+                                        f'div:text-is("{self.__locale.get("cloud_measuring_point")}")'),
+                                    'attributes': {
+                                        self.page.locator(
+                                            f'div:text-is("{self.__locale.get("cloud_measuring_point")}")'): {
+                                            'aria-selected': 'true'}},
+                                    'wait_locator': [
+                                        self.page.locator('.ant-modal-content').locator('.ant-table-content')]
+                                },
+                                'muting': {
+                                    'menu': self.page.locator(
+                                        f'div:text-is("{self.__locale.get("Muting_measuring_point")}")'),
+                                    'attributes': {
+                                        self.page.locator(
+                                            f'div:text-is("{self.__locale.get("Muting_measuring_point")}")'): {
+                                            'aria-selected': 'true'}},
+                                    'wait_locator': [
+                                        self.page.locator('.ant-modal-content').locator('.ant-table-content')]
+                                },
+
+                            }
                         },
                         'whitehawk_energy_manager': {
                             'menu': self.page.locator(
                                 f'div:text-is("{self.__locale.get("whitehawk_energy_manager")}")'),
                             'attributes': {
                                 self.page.locator(
                                     f'div:text-is("{self.__locale.get("whitehawk_energy_manager")}")'): {
@@ -608,15 +650,15 @@
                             'wait_locator': [
                                 self.page.locator(f'text=Modbus RTU Slave{self.__locale.get("configuration")}')],
                         },
                     },
                     'parameter_settings': {
                         'menu': self.parameter_settings_menu,
                         'visible_locator': [self.content_target('parameter_settings')],
-                        'wait_locator': [self.content_target('parameter_settings')]
+                        'wait_locator': [self.page.locator('.ant-table-content')]
                     },
                     'custom_quickfunctions': {
                         'menu': self.custom_quickfunctions_menu,
                         'visible_locator': [self.content_target('custom_quickfunctions')],
                         'wait_locator': [self.content_target('custom_quickfunctions')]}
                 }
             },
@@ -633,15 +675,16 @@
                 'log': {
                     'default': 'log',
                     'menu': self.system_log_menu,
                     'visible_locator': [self.content_target('system_log')],
                     'wait_locator': [self.content_target('system_log')],
                     'log': {
                         'menu': self.page.locator('.ant-tabs-tab >> nth=0'),
-                        'visible_locator': [self.page.locator('//button', has_text=self.__locale.get('clear_history_log'))],
+                        'visible_locator': [
+                            self.page.locator('//button', has_text=self.__locale.get('clear_history_log'))],
                         'attributes': {
                             self.page.locator('.ant-tabs-tab >> nth=0'): {'aria-selected': 'true'}},
                         'wait_locator': [self.page.locator('//button[@class="ant-btn"]').first],
                     },
                     'configure': {
                         'menu': self.page.locator('.ant-tabs-tab >> nth=1'),
                         'visible_locator': [self.page.locator('#log_to_remote_enable')],
```

### Comparing `inhandtest-0.0.57/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.58/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.58/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/base_page/base_page.py` & `inhandtest-0.0.58/inhandtest/base_page/base_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -349,15 +349,15 @@
                     locator.uncheck()
                 if log_desc:
                     logging.info(f'Device {self.host} {log_desc} {action}')
                 self.tip_messages(tip_messages)
         except playwright.sync_api.Error:
             pass
 
-    @allure.step('下拉选择')
+    @allure.step('下拉单项选择')
     def select_option(self, locator: Locator, value: str or int, log_desc=None) -> None:
         """ 封装公共的下拉选择操作
 
         :param locator:  元素定位
         :param value: str or int, 下拉选择option的value属性值、或label
         :param log_desc: 功能描述，用英文 如 Static Routing Destination
         :return:
@@ -430,14 +430,59 @@
             else:  # IR300 等设备的下拉选择
                 locator.select_option(value)  # value 可以为label 或者value
                 if locator.locator(f'//option[@value="{value}"]').count() == 1:
                     value = locator.locator(f'//option[@value="{value}"]').inner_text()
             if log_desc:
                 logging.info(f"Device {self.host} select {log_desc} of {value}")
 
+    @allure.step('下拉多项选择')
+    def select_more(self, locator: Locator, value: list or str, log_desc=None) -> None:
+        """下拉多项选择
+
+        :param locator: 元素定位
+        :param value: 一个或多个选项
+        :param log_desc: 功能描述，用英文 如 Static Routing Destination
+        :return:
+        """
+        if value is not None:
+            value = [value] if isinstance(value, str) else value
+            if 'IG' in self.model:
+                # 先找出现有已选择的选项， 如果不是就要取消，如果是就不管，
+                already_choices = locator.locator('//li[@class="ant-select-selection__choice"]')
+                for i in range(0, already_choices.count()):
+                    if already_choices.nth(i).locator('//div[1]').inner_text() in value:
+                        value.remove(already_choices.nth(i).locator('//div[1]').inner_text())
+                    else:
+                        self.click(already_choices.nth(i).locator('//span/i[1]'))
+                if value:
+                    locator.click()
+                    option_id = locator.locator(".ant-select-selection").get_attribute("aria-controls")
+                    for i in value:
+                        option = self.page.locator(f'//div[@id="{option_id}"]').locator(
+                            f'//ul[@role="listbox"]/li').get_by_text(i, exact=True)
+                        option.click()
+            if log_desc:
+                logging.info(f"Device {self.host} select {log_desc} more {value}")
+
+    @allure.step('下拉多层級选择')
+    def select_multi(self, locator: Locator, value: str, log_desc=None) -> None:
+        """ 封装公共的下拉多級选择, 如 IG902 设备的APP下拉多級选择
+
+        :param locator:  元素定位
+        :param value: str 多個需使用点号隔开
+        :param log_desc: 功能描述，用英文 如 Static Routing Destination
+        :return:
+        """
+        if locator.locator('//span[@class="ant-cascader-picker-label"]').inner_text() != value.split('.')[-1]:
+            locator.click()
+            for i in value.split('.'):
+                self.page.locator(f'//li[text()="{i}"]').click()
+            if log_desc:
+                logging.info(f"Device {self.host} select {log_desc} of {value}")
+
     @allure.step('切换按钮')
     def switch_button(self, locator: Locator, action: str = 'enable', log_desc=None) -> None:
         """控制通用开关按钮开关， 如拨号的开关
 
         :param locator:  开关按钮元素
         :param action: enable, disable, None, True, False 可以开启或关闭，但是并没有提交，只是点击了下
         :param log_desc:  开关功能描述
@@ -454,15 +499,15 @@
                 if locator.get_attribute('aria-checked') == 'false' or not locator.get_attribute('aria-checked'):
                     pass
                 else:
                     locator.click(force=True)
                     if log_desc:
                         logging.info(f"Device {self.host} {log_desc} disabled")
 
-    @allure.step('点选框操作')
+    @allure.step('多点选框操作')
     def radio_select(self, locator: Locator, value: str, log_desc=None) -> None:
         """ 当前只有IG和ER的设备有单选框
 
         :param locator: 在所有label元素的上级div定位
         :param value: 选项的值，注意国际化
         :param log_desc: 选项的描述
         :return:
@@ -478,14 +523,31 @@
                 else:
                     if log_desc:
                         logging.debug(f"Device {self.host} {log_desc} radio already select {value}")
             else:
                 logging.exception(f'found {value} option {option.count()} elements')
                 raise Exception(f'found {value} option {option.count()} elements')
 
+    @allure.step('单点选框操作')
+    def radio(self, locator: Locator, value: str, log_desc=None) -> None:
+        """ 当前只有IG和ER的设备有单选框
+
+        :param locator: 在所有label元素的上级div定位
+        :param value: 选项的值，注意国际化
+        :param log_desc: 选项的描述
+        :return:
+        """
+        if value is not None:
+            if value in ('check', True, 'true', 'yes'):
+                locator.check()
+            else:
+                locator.uncheck()
+            if log_desc is not None:
+                logging.debug(f"Device {self.host} {log_desc} radio {value}")
+
     @allure.step('伸缩按钮')
     def expand(self, left_text: str, action: str = 'expand') -> None:
         """ 伸缩按钮
 
         :param left_text: 伸缩按钮 左边的文本，需要注意国际化
         :param action: expand|close|None
         :return:
@@ -493,41 +555,41 @@
         text_locator = self.page.get_by_text(left_text, exact=True)
         if action is not None:
             text_locator.wait_for(state='visible')
             if text_locator.count() > 1:
                 logging.exception(f'found {left_text} {text_locator.count()} elements')
                 raise
             else:
-                if text_locator.locator('..').get_attribute('type') == 'button':  # IG 产品
-                    if 'right' in text_locator.locator('..').locator('//span/i').get_attribute('aria-label'):
+                if 'IG' in self.model:  # IG 产品
+                    if 'right' in text_locator.locator('..').locator('//i').get_attribute('aria-label'):
                         if action.lower() == 'expand':
                             self.click(text_locator.locator('..'), f'expand {left_text}')
                     else:
                         if action.lower() == 'close':
                             self.click(text_locator.locator('..'), f'closed {left_text}')
-                elif text_locator.locator('..').get_attribute('role') == 'button' or not text_locator.locator(
-                        '..').get_attribute('role'):  # ER805
+                elif 'ER' in self.model:  # ER805
                     locator = self.page.locator(f'svg[data-icon="right"]:right-of(:text-is("{left_text}"))').first
                     if action.lower() == 'expand':
                         if not locator.get_attribute('style'):
                             self.click(locator, f'expand {left_text}')
                     else:
                         if locator.get_attribute('style') == 'transform: rotate(90deg);':
                             self.click(locator, f'closed {left_text}')
                 else:
                     logging.exception(f'not support this expand')
                     raise Exception("not support this expand")
 
     @allure.step('上传文件')
-    def upload_file(self, locator: Locator, path_, dialog_massage=None) -> None:
+    def upload_file(self, locator: Locator, path_, dialog_massage=None, tip_messages=None) -> None:
         """
 
         :param locator:
         :param path_:
         :param dialog_massage
+        :param tip_messages
         :return:
         """
 
         def upload():
             if path_:
                 if os.path.isfile(path_) and os.path.exists(path_):
                     with self.page.expect_file_chooser() as fc:
@@ -538,14 +600,15 @@
                 else:
                     logging.error(f'{path_} Does Not Exist.')
 
         if dialog_massage:
             self.dialog_massage(upload, dialog_massage)
         else:
             upload()
+        self.tip_messages(tip_messages)
 
     @allure.step('下载文件')
     def download_file(self, locator: Locator, file_path, file_name=None) -> None:
         """默认为日志路径
 
         :param locator: 下载按钮元素
         :param file_path: 下载文件的路径, 不需要跟文件名，
@@ -578,14 +641,15 @@
         self.click(locator)
         if locator.get_attribute('class') == 'ant-calendar-picker':  # date
             locator_ = self.page.locator('.ant-calendar-input')
         else:
             locator_ = self.page.locator('.ant-time-picker-panel-input')
         locator_.fill(date)
         locator_.press('Enter')
+        self.page.wait_for_timeout(500)
 
     @allure.step("校验dialog message")
     def dialog_massage(self, f, message: str = '') -> None:
         """对话框提示进行校验， 使用时需要在base_locator 里面定义dialog_massage 且返回字典数据
 
         :param f:  是一个操作函数，执行后会有dialog弹窗出现
         :param message: 校验的信息, 支持模糊匹配
@@ -667,14 +731,33 @@
             else:
                 if select_locator.is_disabled():
                     self.click(select_locator.locator('..').locator('#refresh-button'), 'refresh button')
                     self.page.wait_for_timeout(500)
                 self.select_option(select_locator, refresh_time, 'refresh time select')
                 self.click(select_locator.locator('..').locator('#refresh-button'), 'refresh button ok')
 
+    def turn_page(self, father_locator: Locator = None, page_number=1):
+        """分页， 指定点到第几页  只有IG 产品拥有该方法
+
+        :param father_locator: 当同一页面存在多个分页时，需要传入父元素定位组合成链式定位，确认唯一
+        :param page_number: 第几页
+        :return: 找不到页数时返回False
+        """
+        if self.model in ('IG902', 'IG502'):
+            locator = self.page.locator(f'.ant-pagination-item-{page_number}')
+            if father_locator:
+                locator = father_locator.locator(f'.ant-pagination-item-{page_number}')
+            if locator.is_visible():
+                self.click(locator, f'turn page {page_number}', wait_for_time=500)
+                return True
+            else:
+                return False
+        else:
+            raise Exception(f'{self.model} not support turn page')
+
     @allure.step("操作表格")
     def table_tr(self, locators: dict, value: list, log_desc=None) -> List[int or None] or None:
         """
 
         :param locators: {"locator": $locator2, "param": {$key2: $value2}, "columns": list, 'unique_columns': list}
         :param value: [($action,{**kwarg})] ex: [('delete_all', )],  [('edit', $old, $new)]多个操作时使用列表 [('add',{}), ('add',{})]
         :param log_desc: 日志描述
@@ -698,15 +781,15 @@
                         exist_tr.append(tr.exist(value_[1], self.locale))
                     elif value_[0] == 'edit':
                         tr.edit(self.agg_in, value_[1], **value_[2])
                     elif value_[0] == 'connect':
                         tr.connect(value_[1])
                     elif value_[0] == 'associate_delete':
                         tr.associate_delete(value_[1])
-                    elif value_[0] in ('download_log', 'export_config'):
+                    elif value_[0] in ('download_log', 'export_config', 'export_historical_data'):
                         if isinstance(value_[2], str):
                             file_path = value_[2]
                             file_name = None
                         elif isinstance(value_[2], dict):
                             file_path = value_[2].get('file_path')
                             file_name = value_[2].get('file_name')
                         else:
@@ -721,14 +804,16 @@
                         tr.stop(value_[1])
                     elif value_[0] == 'restart':
                         tr.restart(value_[1])
                     elif value_[0] in ('check', 'enable'):
                         tr.check(self.check, value_[1], value_[2])
                     elif value_[0] == 'clear_log':
                         tr.clear_log(value_[1])
+                    elif value_[0] == 'clear_historical_data':
+                        tr.clear_historical_data(value_[1])
                 return exist_tr
         else:
             tr = Table(locators.get('columns'), locators.get('locator'),
                        locators.get('unique_columns'), locators.get('param'), log_desc)
             exist_tr = []
             if value:
                 for value_ in value:
@@ -740,45 +825,72 @@
                         tr.delete(**value[1])
                     elif value_[0] == 'exist':
                         exist_tr.append(tr.exist(**value[1]))
                     elif value_[0] == 'edit':
                         tr.edit(value[1], value[2])
                 return exist_tr
 
+    def monaco(self, locator: Locator, value: str, log_desc=None):
+        """慕尼黑编辑器输入
+
+        :param locator:
+        :param value: 换行需要使用\n
+        :param log_desc:
+        :return:
+        """
+        self.click(locator, )
+        self.page.keyboard.press('Control+A')
+        self.page.keyboard.press('Delete')
+        self.page.keyboard.type(value)
+        logging.info(f'{log_desc} monaco-editor：{value}')
+
     def agg_in(self, locators: list, action_dict: dict) -> None:
         """封装公共的整合输入操作
                 :param locators:  列表 嵌套 长度为2的元组，元组的第一项为操作项名称， 第二项为对应的一个字典
                     [($param1, {"locator": $locator1, "type": $type1, "relation": [($param2, $value2)], "param": {$key1: $value1}}),
                     ($param2, {"locator": $locator2, "type": $type2, "relation": [($param3, $value3),……], "param": {$key2: $value2}}),
                     ($param3, {"locator": $locator2, "type": 'table_tr', "relation": [($param3, $value3),……], "param": {$key2: $value2},
                                 "columns": list, 'unique_columns': list}),]
                     $param: 操作项的名称，如 'language'|'sim'|'status'
                     $locator: 操作项的元素定位， locator or [locator,locator,...]
-                    $type: 操作项的类型 text|select|button|check|upload_file|download_file|tip_messages|text_messages|title_messages|fill_date|
-                                     multi_select|multi_check|multi_fill|table_tr|switch_button|radio_select|expand|
+                    $type: 操作项的类型 text|select|select_multi|select_more|button|check|upload_file|download_file|tip_messages|text_messages|title_messages|fill_date|
+                                     multi_select|multi_check|multi_fill|table_tr|switch_button|radio_select|expand|monaco
                             select value值可以是label|Value
                             multi_select指一个参数有多个select, 对应操作项的多个locator及value用[]传入
                     "relation":[($param, $value)]: 操作项的关联项，若有多个则首个为最先操作的关联项，其中$param为关联项的名称，$value为关联项的预期值
                     "param":{$key, $value}: 参数转换，如大小写转换{"ab":"AB"} {"wan":"Wan"}等.
                 :param action_dict: 要做操作的参数名称与对应的值{$param1: $value1, $param2: $value2}
                 :return:
                 """
         relations = []
 
         def operation(param, param_locator, value):
             if param_locator.get('type') == 'text':
                 self.fill(param_locator.get('locator'), value, param)
+            elif param_locator.get('type') == 'monaco':
+                self.monaco(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'select':
                 if param_locator.get('param') and value in param_locator.get('param').keys():
                     value = param_locator.get('param').get(value)
                 self.select_option(param_locator.get('locator'), value, param)
+            elif param_locator.get('type') == 'select_more':
+                value = replace_str(value, param_locator.get('param'))
+                self.select_more(param_locator.get('locator'), value, param)
+            elif param_locator.get('type') == 'select_multi':
+                if param_locator.get('param') and value in param_locator.get('param').keys():
+                    value = param_locator.get('param').get(value)
+                self.select_multi(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'radio_select':
                 if param_locator.get('param') and value in param_locator.get('param').keys():
                     value = param_locator.get('param').get(value)
                 self.radio_select(param_locator.get('locator'), value, param)
+            elif param_locator.get('type') == 'radio':
+                if param_locator.get('param') and value in param_locator.get('param').keys():
+                    value = param_locator.get('param').get(value)
+                self.radio(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'switch_button':
                 self.switch_button(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'expand':
                 self.expand(param_locator.get('locator'), value)  # 此处获取到的locator 是一个str
             elif param_locator.get('type') == 'button':
                 if value:
                     dialog_message, tip_messages, wait_for_time, tip_messages_timeout = None, None, None, 30
@@ -829,20 +941,21 @@
                             self.fill(locator_, value_, param)
                         else:
                             logging.error(f"not support this param type {param_locator.get('type')}")
                 else:
                     logging.error('Wrong length or type of locator or value!')
             elif param_locator.get('type') == 'upload_file':
                 if value:
-                    file_path, dialog_message = value, None
+                    file_path, dialog_message, tip_message = value, None, None
                     if isinstance(value, dict):
-                        file_path, dialog_message = value.get('file_path'), value.get('dialog_message')
+                        file_path, dialog_message, tip_message = value.get('file_path'), value.get(
+                            'dialog_message'), value.get('tip_messages')
                     elif isinstance(value, str):
                         pass
-                    self.upload_file(param_locator.get('locator'), file_path, dialog_message)
+                    self.upload_file(param_locator.get('locator'), file_path, dialog_message, tip_message)
             elif param_locator.get('type') == 'download_file':
                 if value:
                     file_path, file_name = value, None
                     if isinstance(value, dict):
                         file_path, file_name = value.get('file_path'), value.get('file_name')
                     elif isinstance(value, str):
                         pass
@@ -879,26 +992,43 @@
                 for wait_for_ in wait_for:
                     if wait_for_.get('type') == 'timeout':
                         self.page.wait_for_timeout(wait_for_.get('timeout'))
                     elif wait_for_.get('type') == 'visible':
                         wait_for_.get('locator').wait_for(state='visible', timeout=wait_for_.get('timeout'))
                     elif wait_for_.get('type') == 'hidden':
                         wait_for_.get('locator').wait_for(state='hidden', timeout=wait_for_.get('timeout'))
+                    elif wait_for_.get('type') == 'tip_messages':
+                        timeout = wait_for_.get('timeout') if wait_for_.get('timeout') else 30
+                        self.tip_messages(wait_for_.get('messages'), timeout)
 
         if action_dict:
             for option in locators:
                 assert type(option) in (tuple, list) and len(option) == 2, "type of option is incorrect"
                 if option[0] in [key for key, value in action_dict.items() if value is not None]:
-                    if option[1].get("relation") and option[1].get("relation") not in relations:
-                        # 对关系项操作之前检查关系项
-                        for relation_ in option[1].get("relation"):
-                            relation_locator = [i[1] for i in locators if i[0] == relation_[0]][0]
-                            operation(relation_[0], relation_locator, relation_[1])  # 关系项操作
-                        relations.append(option[1].get("relation"))
-                    operation(option[0], option[1], action_dict.get(option[0]))  # 本身操作
+                    if isinstance(option[1], dict):
+                        if option[1].get("relation") and option[1].get("relation") not in relations:
+                            # 对关系项操作之前检查关系项
+                            for relation_ in option[1].get("relation"):
+                                relation_locator = [i[1] for i in locators if i[0] == relation_[0]][0]
+                                operation(relation_[0], relation_locator, relation_[1])  # 关系项操作
+                            relations.append(option[1].get("relation"))
+                        operation(option[0], option[1], action_dict.get(option[0]))  # 本身操作
+                    elif isinstance(option[1], list) and isinstance(action_dict.get(option[0]),
+                                                                    list):  # 当使用一个变量传多个元素的值时
+                        for option_, action_value in zip(option[1], action_dict.get(option[0])):
+                            if option_.get("relation") and option_.get("relation") not in relations:
+                                # 对关系项操作之前检查关系项
+                                for relation_ in option_.get("relation"):
+                                    relation_locator = [i[1] for i in locators if i[0] == relation_[0]][0]
+                                    operation(relation_[0], relation_locator, relation_[1])  # 关系项操作
+                                relations.append(option_.get("relation"))
+                            operation(option[0], option_, action_value)  # 本身操作
+                    else:
+                        logging.exception("type of option is incorrect")
+                        raise Exception("type of option is incorrect")
 
     @allure.step("计算元素表达式")
     def eval_locator_attribute(self, expect_: dict, locators: list) -> bool:
         """对页面特定元素值做判断
 
         :param expect_: {$status: $expressions}
                         status: 状态名称， 比如可以传定义好的 current_sim
@@ -924,14 +1054,16 @@
                     if option[1].get('type') == 'switch_button':
                         if 'ant-switch-checked' in locator.first.get_attribute('class'):
                             value = 'enable'
                         else:
                             value = 'disable'
                     elif option[1].get('type') == 'fill':
                         value = locator.first.input_value()
+                    elif option[1].get('type') == 'class':
+                        value = locator.first.get_attribute('class')
                     else:  # type is text
                         if isinstance(locator, Locator):
                             value = locator.first.inner_text() if locator.count() != 0 else 'None'
                         else:
                             value = str(locator)
                     try:
                         if '${value}' in expect_.get(key):
@@ -980,14 +1112,16 @@
                                 locator.first.click()
                                 value = self.page.evaluate('navigator.clipboard.readText()')
                             elif option[1].get('type') == 'switch_button':
                                 if 'ant-switch-checked' in locator.first.get_attribute('class'):
                                     value = 'enable'
                                 else:
                                     value = 'disable'
+                            elif option[1].get('type') == 'class':
+                                value = locator.first.get_attribute('class')
                             else:
                                 value = locator.first.inner_text()
                         else:
                             value = None
                     else:
                         value = str(locator)
                     result[key] = value
@@ -1052,8 +1186,7 @@
             self.__browser.close()
             self.__playwright.stop()
             logging.info('close browser and playwright')
 
 
 if __name__ == '__main__':
     pass
-
```

### Comparing `inhandtest-0.0.57/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.58/inhandtest/base_page/table_tr.py`

 * *Files 8% similar despite different names*

```diff
@@ -284,24 +284,28 @@
 
         :param agg_in: function, 导致该方法不能单独使用
         :param kwargs str, 待添加列 及对应值
         :return:
         """
         if ('save' not in list(kwargs.keys())) and ('cancel' not in list(kwargs.keys())):
             kwargs['save'] = True
+        try:
+            add_button = list(filter(lambda x: x[0] == 'add', self.columns))[0][1].get('locator')
+        except Exception:
+            add_button = self.table_locator.locator('//button').first
         if kwargs.get('is_exists'):
             is_exists = kwargs.pop('is_exists')
             if not self.exist(is_exists, self.locale):
-                self.table_locator.locator('//button').first.click()
+                add_button.click()
                 agg_in(self.columns, kwargs)
                 logging.debug(f'table resource {kwargs} add success')
             else:
                 logging.debug(f'table resource {kwargs} exist')
         else:
-            self.table_locator.locator('//button').first.click()
+            add_button.click()
             agg_in(self.columns, kwargs)
             if not kwargs.get('cancel'):
                 logging.debug(f'table resource {kwargs} add success')
 
     def edit(self, agg_in, old_value, **kwargs) -> None:
         """ 只能编辑匹配到的第一条记录
 
@@ -309,15 +313,18 @@
         :param old_value: str, 旧值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值
         :param kwargs str, 待添加列 及对应值
         :return:
         """
         old_value = replace_str(old_value, self.locale)
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(old_value))
         if exist_tr.count() > 0:
-            exist_tr.first.locator('//i[@class="anticon anticon-form"]').click()
+            if exist_tr.first.locator('//i[@class="anticon anticon-form"]').count() == 1:
+                exist_tr.first.locator('//i[@class="anticon anticon-form"]').click()
+            else:
+                exist_tr.first.locator('//i[@class="anticon anticon-edit"]').click()
             if ('save' not in list(kwargs.keys())) and ('cancel' not in list(kwargs.keys())):
                 kwargs['save'] = True
             agg_in(self.columns, kwargs)
             if not kwargs.get('cancel'):
                 logging.debug(f'table resource {kwargs} edit success')
         else:
             logging.debug(f'table resource {old_value} not exist')
@@ -381,17 +388,23 @@
     def check(self, action, value, check_value):
         """
         :param action: function, 导致该方法不能单独使用
         :param value str, 待check 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :param check_value: str, 待check值
         :return:
         """
-        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
-        if exist_tr.count() > 0:
-            action(exist_tr.first.locator('//input[@type="checkbox"][@class="ant-checkbox-input"]').nth(0), check_value)
+        tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr')
+        for i in range(0, tr.count()):
+            for x in range(0, tr.nth(i).locator('//td').count()):
+                if tr.nth(i).locator('//td').nth(x).inner_text() == value:
+                    return action(tr.nth(i).locator('//input[@type="checkbox"][@class="ant-checkbox-input"]').nth(0), check_value)
+        else:
+            exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+            if exist_tr.count() > 0:
+                action(exist_tr.first.locator('//input[@type="checkbox"][@class="ant-checkbox-input"]').nth(0), check_value)
         logging.debug(f'table resource {value}  {check_value}')
 
     def start(self, value: str) -> None:
         """
         :param value str, 待开始列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
@@ -425,14 +438,27 @@
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
         if exist_tr.count() > 0:
             exist_tr.first.locator('//i[@class="anticon anticon-undo"]').first.click()
             if isinstance(self.action_confirm, Locator):
                 self.action_confirm.click()  # 二次确认
         logging.debug(f'table resource {value} all restart')
 
+    def clear_historical_data(self, value: str) -> None:
+        """
+        :param value str, 待重启列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
+        :return:
+        """
+        value = replace_str(value, self.locale)
+        exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
+        if exist_tr.count() > 0:
+            exist_tr.first.locator('//i[@class="anticon"]').first.click()
+            if isinstance(self.action_confirm, Locator):
+                self.action_confirm.click()  # 二次确认
+        logging.debug(f'table resource {value} all restart')
+
     def clear_log(self, value: str) -> None:
         """
         :param value str, 待开始列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
         """
         value = replace_str(value, self.locale)
         exist_tr = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr', has_text=re.compile(value))
```

### Comparing `inhandtest-0.0.57/inhandtest/exception.py` & `inhandtest-0.0.58/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/file.py` & `inhandtest-0.0.58/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/inmodbus.py` & `inhandtest-0.0.58/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/inmongodb.py` & `inhandtest-0.0.58/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/inmqtt.py` & `inhandtest-0.0.58/inhandtest/inmqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,35 +18,39 @@
 import logging
 
 
 class MqttClient:
     __doc__ = "使用前需安装paho-mqtt  pip install paho-mqtt"
 
     def __init__(self, host: str, port: int = 1883, username=None, password=None, client_id=None, clean_session=True,
-                 reconnect_on_failure=True, keepalive=120):
+                 reconnect_on_failure=True, keepalive=120, tls=False, proxy=False):
         """MQTT客户端
 
         :param host: 服务器地址
         :param port: 服务器MQTT端口
         :param username: username
         :param password: password
         :param client_id: client_id, 如果为None时随机获取
         :param clean_session: 是否清除session， 默认为True
         :param reconnect_on_failure: 失败时重连，默认为True
+        :param tls: 是否使用tls，默认为False
+        :param proxy: 是否使用代理，默认为False
         :param keepalive: 心跳 默认120
         """
 
         self.host = host
         self.port = port
         self.username = username
         self.password = password
         self.client_id = 'inhand-' + str(uuid.uuid4()) if client_id is None else client_id
         self.keepalive = keepalive
         self.clean_session = clean_session
         self.reconnect_on_failure = reconnect_on_failure
+        self.tls = tls
+        self.proxy = proxy  # 是否使用代理
         self.connect_time = None
         self.client = self.__connect()
         self.recv_datas = []
 
     def __on_connect(self, client, userdata, flags, rc):
         """
         :param client:
@@ -89,23 +93,30 @@
         if not self.reconnect_on_failure:
             self.disconnect()
 
     def __connect(self) -> client.Client:
         """连接MQTT服务器
         """
         # 生成随机ID
+        if self.proxy:
+            import socket
+            import socks
+            socks.setdefaultproxy(socks.PROXY_TYPE_HTTP, "10.5.17.21", 8118)
+            socket.socket = socks.socksocket
         mqtt_client = client.Client(self.client_id, self.clean_session, reconnect_on_failure=self.reconnect_on_failure)
         mqtt_client.username_pw_set(self.username, self.password)
         mqtt_client.on_connect = self.__on_connect
         mqtt_client.on_message = self.__on_message
         mqtt_client.on_subscribe = self.__on_subscribe
         mqtt_client.on_publish = self.__on_publish
         mqtt_client.on_log = self.__on_log
         mqtt_client.on_disconnect = self.__on_disconnect
         logging.info(f'client {self.client_id} start connection')
+        if self.tls:
+            mqtt_client.tls_set()
         mqtt_client.connect(self.host, self.port, self.keepalive)
         mqtt_client.loop_start()
         return mqtt_client
 
     def disconnect(self) -> None:
         """断开MQTT连接
         """
@@ -202,15 +213,16 @@
                                     if len(topic_payloads) >= 2:
                                         fist_time = topic_payloads[0][2]  # 取第一条的第3个元素
                                         for time_payload in topic_payloads[1:]:
                                             if assert_payload.get('time_interval')[0] <= time_payload[2] - fist_time <= \
                                                     assert_payload.get('time_interval')[1]:
                                                 fist_time = time_payload[2]
                                             else:
-                                                logging.exception(f"current data time is  {time_payload[2]},  last data time is {fist_time}")
+                                                logging.exception(
+                                                    f"current data time is  {time_payload[2]},  last data time is {fist_time}")
                                                 raise AssertionError(
                                                     f"current data time is  {time_payload[2]},  last data time is {fist_time}")
                                 if assert_payload:
                                     def payload_verify(x):
                                         if x[0] == topic:
                                             expect_payload_ = dict_flatten(assert_payload)  # 平铺字典
                                             r_payload_ = dict_flatten(x[1])
```

### Comparing `inhandtest-0.0.57/inhandtest/inrequest.py` & `inhandtest-0.0.58/inhandtest/inrequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,20 +293,20 @@
                 'content')
             if config:
                 assert set(config.split('\n')).issubset(set(config_content.split('\n'))), f'config {config} not exist'
         else:
             logging.exception(f'the {sn} device not exist or offline')
             raise ResourceNotFoundError(f'the {sn} device not exist or offline')
 
-    def upgrade_firmware_online(self, sn: str, firmware: str, timeout=10 * 60, interval=10) -> None:
+    def upgrade_firmware_online(self, sn: str, firmware: str, timeout=20 * 60, interval=10) -> None:
         """ 升级固件， 保障升级成功不然就会报错
 
         :param sn: 设备序列号
         :param firmware: 升级的固件，本地全路径
-        :param timeout: 下发升级任务后，总体的升级超时时间， 单位秒 至少5分鐘
+        :param timeout: 下发升级任务后，总体的升级超时时间， 单位秒 至少5分鐘， 10， 20， 30
         :param interval: 升级任务检测间隔， 单位秒
         :return None or TimeOutError， 升级失败就报TimeOutError
         """
 
         def model(name):
             models = self.api.send_request('api/models', 'get',
                                            {'gateway': True, 'verbose': 100, 'limit': 0}).json().get('result')
@@ -325,15 +325,15 @@
             if os.path.isfile(firmware):  # 只要升级文件存在就升级
                 get_firmware = self.api.send_request('api/firmware', 'get', {'name': file_name}).json()
                 if get_firmware.get('total') == 0:
                     if os.path.exists(firmware):
                         param = {'filename': firmware, 'oid': 'undefined'}
                         upload_file = self.api.send_request('api/file/form', method='post', param=param,
                                                             params_type='form', file_path=firmware).json().get('result')
-                        body = {'fid': upload_file['_id'], 'jobTimeout': 30, 'model': model(file_name),
+                        body = {'fid': upload_file['_id'], 'jobTimeout': int(timeout / 60), 'model': model(file_name),
                                 'name': file_name,
                                 'version': version(file_name), 'desc': 'auto test upload firmware'}
                         firmware_id = self.api.send_request('api/firmware', 'post', body=body, ).json().get(
                             'result').get(
                             '_id')
                     else:
                         logging.exception(f'{firmware} not exist')
@@ -865,15 +865,14 @@
                     [_id.append(org.get('_id')) for org in orgs if org.get('name') == name_]
 
         if _id:
             for __id in _id:
                 self.api.send_request(f'/api/v1/orgs/{__id}', 'delete')
             logging.info(f'delete org success')
 
-
     @__only_admin
     def org_info_in_paas(self, org_email) -> DotDict:
         """ 获取org info
 
         :param org_email:
         :return:   {name: "Admin_test_new", email: "liwei@inhand.com.cn", _id: "5fb24ef9f0393a4c4fd7c8b7"}
         """
@@ -1397,9 +1396,8 @@
         return res
 
 
 if __name__ == "__main__":
     from inhandtest.log import enable_log
 
     enable_log(console_level='info')
-    my = StarInterface('liwei@inhand.com.cn', '123456', 'star.nezha.inhand.design')
-    my.delete_org('test', None, )
+    # my.delete_org('test', None, )
```

### Comparing `inhandtest-0.0.57/inhandtest/inserial.py` & `inhandtest-0.0.58/inhandtest/inserial.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,27 +114,30 @@
                 logging.debug(f"open serial {self.com} success")
                 break
             time.sleep(3)
         else:
             logging.exception(f"open serial {self.com} failed")
             raise SerialException(f'serial {self.com} already used')
 
-    def receive_log(self, timeout=20, logs_number=1):
+    def receive_log(self, recv_timeout=20, logs_number=1):
         """接收日志
 
-        :param timeout: 接收超时时间
+        :param recv_timeout: 接收超时时间
         :param logs_number
         :return:
         """
         self.serial.timeout = 1
-        for i in range(0, timeout, 1):
-            data = self.serial.readline()  # 获取串口内容
-            logging.debug(f'serial com {self.com} read str <{data.decode()}>')
+        for i in range(0, recv_timeout, 1):
+            try:
+                data = self.serial.readline()  # 获取串口内容
+            except AttributeError:
+                break
+            logging.debug(f'serial com {self.com} read str <{data.decode(errors="ignore")}>')
             if data:
-                self.logs_number.append(data.decode())
+                self.logs_number.append(data.decode(errors="ignore"))
             if logs_number == len(self.logs_number):
                 break
             else:
                 time.sleep(1)
         else:
             logging.exception(f'serial com {self.com} read log timeout')
             raise Exception('can not receive logs')
@@ -172,38 +175,44 @@
     def close(self):
         if self.serial.is_open:
             try:
                 self.serial.close()
             except SerialException:
                 logging.error(f'Serial Close {self.com} Failed')
 
-    def assert_recv_data(self, action, length, timeout=10, content=None):
+    def assert_recv_data(self, action, length, timeout=10, content=None, **kwargs):
         """
         :param action: 操作函数
         :param length: 期望接受到的数据长度
         :param timeout: 最大超时时间
         :param content: 期望校验接受到的数据的内容
         """
         serial_thread = Thread(target=self.receive_log, args=(timeout, length))
         serial_thread.daemon = True
         serial_thread.start()
         time.sleep(1)
-        action()
+        action(**kwargs)
         for x in range(0, timeout, 1):
-            if length and not content:
-                command = 'length == len(self.logs_number)'
-            elif not length and content:
-                command = "content in ','.join(self.logs_number)"
-            else:
-                command = "length == len(self.logs_number) and content in ','.join(self.logs_number)"
-            if eval(command):
-                logging.info(f"assert data {self.logs_number} ok")
+            result = True
+            if length:
+                if length != len(self.logs_number):
+                    result = False
+            if content and result:
+                if isinstance(content, str):
+                    if content not in ','.join(self.logs_number):
+                        result = False
+                else:
+                    if [c for c in content if c not in ','.join(self.logs_number)]:
+                        result = False
+            if result:
+                logging.info(f"assert data ok")
                 break
             else:
                 time.sleep(1)
+                logging.debug(f"assert data failed, try again")
         else:
-            logging.exception(f"assert data {self.logs_number} failed")
+            logging.exception(f"assert data failed finally")
             raise Exception('serial not receive data')
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `inhandtest-0.0.57/inhandtest/insocket.py` & `inhandtest-0.0.58/inhandtest/insocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,35 +6,35 @@
 insocket
 
 """
 
 import threading
 import time
 import socket
-import logging 
+import logging
 
 
 def tcp_server_data(host, port, recv_content: dict = None, connect_time=10,
-                    send_msg_to_server: str or list = None, function=None, timeout=5, **kwargs):
+                    send_msg_to_server: str or list = None, function=None, accept_timeout=5, **kwargs):
     """ 开启tcp_server, 并且接收数据，对数据做验证, 该连接为阻塞式，所以要确保客户端能正常连接过来，还要确保防火墙是关闭的
         该连接使用with，所以不管是客户端还是服务端，还是在异常状态下都会正常关闭
 
     :param host:  server地址 ex: 10.5.24.224
     :param port:  server端口 ex: 3001
     :param recv_content: {('10.5.24.224', 3002): "hello world"} 判断客户端('10.5.24.224', 3002) 在接收到的内容里面是否包含"hello world",  value可以是list，判断多个内容
                          {'content': "hello world"}, 判断连接过来的客户端在接收到的内容里面是否包含"hello world"
     :param connect_time:  服务器和客户端建立连接后，需要连接的时间
     :param send_msg_to_server: 当客户端连接成功后，已连接客户端向服务端发送的内容
     :param function: tcp_server 连接上后做的操作
-    :param timeout: 接收数据的或连接的超时时间
+    :param accept_timeout: 接收数据的或连接的超时时间
     :param kwargs:  function接入的参数
     :return: AssertionError or None
     """
     all_datas = {}
-    socket.setdefaulttimeout(timeout)
+    socket.setdefaulttimeout(accept_timeout)
 
     def client_send_msg_to_server(conn, addr, msg: str or list):
         if msg is not None:
             msg = [msg] if isinstance(msg, str) else [msg_ for msg_ in msg]
             for msg_ in msg:
                 conn.send(msg_.encode('utf-8'))
                 logging.debug(f'tcp client {addr} send msg {msg_} to server {host}: {port}')
@@ -70,15 +70,15 @@
                         datas = datas + recv_data
                         all_datas.update({__addr: datas})
                     else:
                         __conn.close()
                 if client:
                     break
         except socket.timeout:
-            logging.warning(f'tcp server {host}:{port} connect timeout or reva data timeout')
+            logging.error(f'tcp server {host}:{port} connect timeout or reva data timeout')
     # 数据校验
     if recv_content is not None:
         if all_datas:
             for k, v in recv_content.items():
                 if k == 'content':
                     datas = b''.join([v_ for v_ in all_datas.values()])
                     contents = [v.encode('utf-8')] if isinstance(v, str) else [c_.encode('utf-8') for c_ in v]
@@ -103,29 +103,29 @@
                         raise AssertionError(f'tcp server {host}:{port} client {k} not connected')
         else:
             logging.exception(f'tcp server {host}:{port} client not connected')
             raise AssertionError(f'tcp server {host}:{port} client not connected')
 
 
 def tcp_client_data(server: tuple, client: tuple = None, recv_content: str or list = None, connect_time=10,
-                    send_msg_to_server: str or list = None, function=None, timeout=5, **kwargs):
+                    send_msg_to_server: str or list = None, function=None, socket_timeout=5, **kwargs):
     """ 开启tcp_client, 并且接收数据，对数据做验证
         该连接使用with，所以不管是客户端还是服务端，还是在异常状态下都会正常关闭
 
     :param server: ($host, $port), 客户端需要连接的服务器地址和端口，使用元组，必填('192.168.2.1', 502)
     :param client:  ($host, $port) 绑定指定地址和端口，如果为None ，本机直接开启一个， 跟server参数一样
     :param recv_content: 判断客户端 在接收到的内容里面包含recv_content 也可以不做校验
     :param connect_time:  服务器和客户端建立连接后，需要连接的时间
     :param send_msg_to_server: 当客户端连接成功后，客户端向服务端发送的内容
     :param function: 当客户端 连接上后做的操作
-    :param timeout: 接收数据的或连接的超时时间
+    :param socket_timeout: 接收数据的或连接的超时时间
     :param kwargs:  function接入的参数
     :return: AssertionError or None
     """
-    socket.setdefaulttimeout(timeout)
+    socket.setdefaulttimeout(socket_timeout)
     datas = b''
 
     def client_send_msg_to_server(client_, msg: str or list):
         if msg is not None:
             msg = [msg] if isinstance(msg, str) else [msg_ for msg_ in msg]
             for msg_ in msg:
                 client_.send(msg_.encode("utf-8"))
```

### Comparing `inhandtest-0.0.57/inhandtest/inssh.py` & `inhandtest-0.0.58/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/ip.py` & `inhandtest-0.0.58/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/log.py` & `inhandtest-0.0.58/inhandtest/log.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/mail.py` & `inhandtest-0.0.58/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/pages/ingateway/ingateway.py` & `inhandtest-0.0.58/inhandtest/pages/ingateway/ingateway.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,12 +58,15 @@
         self.network: Network = Network(host, username, password, protocol, port, model, language, self.page,
                                         self.locale)
         self.edge = EdgeComputing(host, username, password, protocol, port, model, language, self.page, self.locale)
         self.system = System(host, username, password, protocol, port, model, language, self.page, self.locale)
 
 
 if __name__ == '__main__':
-    with InGateway('10.5.24.96', 'inhand', '64391099@inhand') as device:
-        device.network.cellular.config(cellular_enable=False,
-                                       submit={'tip_messages': 'cellular_configuration_changed_successful'})
+    from inhandtest.log import enable_log
 
-        # device.page.wait_for_timeout(3 * 1000)
+    enable_log(console_level='debug')
+    with InGateway('10.5.23.160', 'inhand', '64391099@inhand') as device:
+        device.edge.device_supervisor.cloud.config(
+            subscribe=[('add', {'name': 'my_publish',
+                              'topic': '/v122', 'qos': 2, 'entry_function': 'main', 'quick_function': '#import sys'})])
+        device.page.wait_for_timeout(10 * 1000)
```

### Comparing `inhandtest-0.0.57/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.58/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/pages/ingateway/network/network.py` & `inhandtest-0.0.58/inhandtest/pages/ingateway/network/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                      add parameter:
                      network_type: GSM,CDMA, ex: network_type="GSM"
                      apn: 3gnet ex: apn="3gnet"
                      access_number: *99***1# ex: access_number="*99***1#"
                      auth_method: auto,PAP,CHAP,MS-CHAP,MS-CHAPv2 ex: auth_method="auto"
                      username: gprs ex: username="gprs"
                      password: gprs ex: password="gprs"
-                     error_text: str or list
+                     text_messages: str or list
                      cancel: True, False
                  [('add', {'network_type': 'GSM', 'apn': '3gnet', 'access_number': '*99***1#',
                           'auth_method': 'auto', 'username': 'gprs', 'password': 'gprs', 'is_exists': 'GSM3gnet'})] 如果存在GSM3gnet则不添加
                  [('edit', '2GSM', {'network_type': 'GSM', 'apn': '4gnet'})]
                  多个操作时使用列表 [('add',{}), ('add',{})]
                dual_sim_enable: enable,disable ex: dual_sim_enable="enable"
                main_sim: SIM1,SIM2,Random,Sequence ex: main_sim="SIM1"
@@ -133,15 +133,15 @@
                use_default_asyncmap: enable,disable ex: use_default_asyncmap="enable"
                use_peer_dns: enable,disable ex: use_peer_dns="enable"
                lcp_interval: 10 ex: lcp_interval=10
                lcp_max_retries: 10 ex: lcp_max_retries=10
                infinitely_dial_retry: enable,disable ex: infinitely_dial_retry="enable"
                debug: enable,disable ex: debug="enable"
                expert_options: 'AT+CPIN?'
-               error_text: str or list or tuple ex: error_text="Please enter an integer for 1 ~ 604800"
+               text_messages: str or list or tuple ex: text_messages="Please enter an integer for 1 ~ 604800"
                submit: True or False ex: submit=True  or  submit={'tip_messages': 'cellular_configuration_changed_successful'}
                reset: True or False ex: reset=True
         :return:
         """
         self.access_menu('network.network_interface.cellular')
         self.agg_in(self.network_locators.cellular_locators, kwargs)
 
@@ -209,22 +209,22 @@
                     [($action, **kwarg)]
                     ex: [('delete_all', )],
                      [('delete', '192.168.2.1255.255.255.0')]
                      [('add', {'secondary_ip': '192.168.2.1', 'netmask': '255.255.255.0'})]
                      add parameter:
                         secondary_ip:
                         netmask:
-                        error_text: str or list
+                        text_messages: str or list
                         cancel: True, False
                      [('add', {'secondary_ip': '192.168.2.1', 'netmask': '255.255.255.0', 'is_exists': '192.168.2.1255.255.255.0'})]  如果存在就不加
                      [('edit', '192.168.2.1255.255.255.0', {'secondary_ip': '192.168.3.1', 'netmask': '255.255.255.0'})]
                      多个操作时使用列表 [('add',{}), ('add',{})]
                 submit: True, False ex: submit=True or submit={'tip_messages': 'submit_success'}
-                errors_text: 'ip_address_conflict' ex: errors_text='ip_address_conflict'
-                success_tip: 'submit_success' ex: success_tip='submit_success'  提交后需要验证成功的提示框
+                text_messages: 'ip_address_conflict' ex: text_messages='ip_address_conflict'
+                tip_messages: 'submit_success' ex: tip_messages='submit_success'  提交后需要验证成功的提示框
                 reset: True ex: reset=True
         :return:
         """
         self.access_menu(f'network.network_interface.ethernet.{port}')
         try:
             self.agg_in(self.network_locators.ethernet_locators, kwargs)
         except TimeoutError:
@@ -278,24 +278,24 @@
                 secondary_ip_settings:
                 [($action, **kwarg)] ex: [('delete_all', )],
                  [('delete', '192.168.2.1255.255.255.0')]
                  [('add', {'secondary_ip': '192.168.2.1', 'netmask': '255.255.255.0'})]
                     add parameter:
                     secondary_ip:
                     netmask:
-                    error_text: str or list
+                    text_messages: str or list
                     cancel: True, False
                  [('add', {'secondary_ip': '192.168.2.1', 'netmask': '255.255.255.0', 'is_exists': '192.168.2.1255.255.255.0'})]  如果存在就不加
                  [('edit', '192.168.2.1255.255.255.0', {'secondary_ip': '192.168.3.1', 'netmask': '255.255.255.0'})]
                  多个操作时使用列表 [('add',{}), ('add',{})]
                 ge_01: enable, disable ex: ge_01='enable'
                 ge_02: enable, disable ex: ge_02='enable'
                 submit: True, False ex: submit=True or submit={'tip_messages': 'submit_success'}
-                errors_text: 'ip_address_conflict' ex: errors_text='ip_address_conflict'
-                success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+                text_messages: 'ip_address_conflict' ex: text_messages='ip_address_conflict'
+                tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
                 reset: True ex: reset=True
         :return:
         """
         self.access_menu('network.network_interface.bridge')
         self.agg_in(self.network_locators.bridge_locators, kwargs)
 
 
@@ -381,16 +381,16 @@
                ap_auth_method: OPEN, SHARED, WPA-PSK, WPAPSK/WPA2PSK, ex: ap_auth_method="OPEN"
                ap_encrypt_mode: TKIP, AES, NONE, WEP40,  WEP104, ex: ap_encrypt_mode="TKIP"
                ap_wep_key: 123456, ex: ap_wep_key="123456"
                ap_wpa_psk_key: 12345678, ex: ap_wpa_psk_key="12345678"
                ap_bandwidth: 20MHz,40MHz, ex: ap_bandwidth="20MHz"
                ap_stations_limit: 1,2,3,4,5,6,7,8,9,10, ex: ap_stations_limit="1"
                submit: True,False ex: submit=True  or submit={'tip_messages': 'submit_success'}
-               errors_text: 'ip_address_conflict' ex: errors_tip='ip_address_conflict'
-               success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+               text_messages: 'ip_address_conflict' ex: errors_tip='ip_address_conflict'
+               tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
                reset: True,False ex: reset=True
         :return:
         """
         self.access_menu('network.network_interface.wlan')
         if kwargs.get('sta_connect'):
             kwargs.update({'sta_connect': [('connect', kwargs.get('sta_connect'))]})
         self.agg_in(self.network_locators.wlan_locators, kwargs)
@@ -449,22 +449,22 @@
                secondary_ip_settings:
                [($action, **kwarg)] ex: [('delete_all', )],
                  [('delete', '192.168.2.1255.255.255.0')]
                  [('add', {'secondary_ip': '192.168.2.1', 'netmask': '255.255.255.0'})]
                  add parameter:
                     secondary_ip:
                     netmask:
-                    errors_text
+                    text_messages
                     cancel: True,
                  [('add', {'secondary_ip': '192.168.2.1', 'netmask': '255.255.255.0', 'is_exists': '192.168.2.1255.255.255.0'})]  如果存在就不加
                  [('edit', '192.168.2.1255.255.255.0', {'secondary_ip': '192.168.3.1', 'netmask': '255.255.255.0'})]
                  多个操作时使用列表 [('add',{}), ('add',{})]
                submit: True,False ex: submit=True or submit={'tip_messages': 'submit_success'}
-               errors_text: 'ip_address_conflict' ex: errors_text='ip_address_conflict'
-               success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+               text_messages: 'ip_address_conflict' ex: text_messages='ip_address_conflict'
+               tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
                 reset: True,False ex: reset=True
         :return:
         """
         self.access_menu('network.network_interface.wan')
         self.agg_in(self.network_locators.wan_locators, kwargs)
 
 
@@ -512,22 +512,22 @@
                secondary_ip_settings:
                [($action, **kwarg)] ex: [('delete_all', )],
                  [('delete', '192.168.2.1255.255.255.0')]
                  [('add', {'secondary_ip': '192.168.2.1', 'netmask': '255.255.255.0'})]
                     add parameter:
                         secondary_ip:
                         netmask:
-                        errors_text: str or list
+                        text_messages: str or list
                         cancel: True,
                  [('add', {'secondary_ip': '192.168.2.1', 'netmask': '255.255.255.0', 'is_exists': '192.168.2.1255.255.255.0'})]  如果存在就不加
                  [('edit', '192.168.2.1255.255.255.0', {'secondary_ip': '192.168.3.1', 'netmask': '255.255.255.0'})]
                  多个操作时使用列表 [('add',{}), ('add',{})]
                submit: True,False ex: submit=True  or submit={'tip_messages': 'submit_success'}
-               errors_text: 'ip_address_conflict' ex: errors_text='ip_address_conflict'
-               success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+               text_messages: 'ip_address_conflict' ex: text_messages='ip_address_conflict'
+               tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
                reset: True,False ex: reset=True
         :return:
         """
         self.access_menu('network.network_interface.lan')
         self.agg_in(self.network_locators.lan_locators, kwargs)
 
 
@@ -566,22 +566,22 @@
                secondary_ip_settings:
                [($action, **kwarg)] ex: [('delete_all', )],
                  [('delete', '192.168.2.1255.255.255.0')]
                  [('add', {'secondary_ip': '192.168.2.1', 'netmask': '255.255.255.0'})]
                     add parameter:
                         secondary_ip:
                         netmask:
-                        errors_text: str or list
+                        text_messages: str or list
                         cancel: True,
                  [('add', {'secondary_ip': '192.168.2.1', 'netmask': '255.255.255.0', 'is_exists': '192.168.2.1255.255.255.0'})]  如果存在就不加
                  [('edit', '192.168.2.1255.255.255.0', {'secondary_ip': '192.168.3.1', 'netmask': '255.255.255.0'})]
                  多个操作时使用列表 [('add',{}), ('add',{})]
                submit: True,False ex: submit=True or submit={'tip_messages': 'submit_success'}
-               errors_text: 'ip_address_conflict' ex: errors_text='ip_address_conflict'
-               success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+               text_messages: 'ip_address_conflict' ex: text_messages='ip_address_conflict'
+               tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
                reset: True,False ex: reset=True
         :return:
         """
         self.access_menu('network.network_interface.loopback')
         self.agg_in(self.network_locators.loopback_locators, kwargs)
 
 
@@ -604,35 +604,35 @@
                          'start_address': '192.168.2.2', 'end_address': '192.168.2.234', 'lease': 1440})]
                    add parameters:
                         enable_dhcp_server: 'enable', 'disable'
                         interface: 'Gigabitethernet 0/1', 'Cellular 1',
                         start_address:
                         end_address:
                         lease: 30-10080
-                        error_text: str or list
+                        text_messages: str or list
                         cancel: True, False
                 [('add', {'enable_dhcp_server': 'enable', 'interface': 'Gigabitethernet 0/1',
                          'start_address': '192.168.2.2', 'end_address': '192.168.2.234', 'lease': 1440, 'is_exists': 'Gigabitethernet 0/110.5.24.97'})] 如果存在则不添加
                 [('edit', 'Gigabitethernet 0/110.5.24.97', {'enable_dhcp_server': 'enable'})]
                 多个操作时使用列表 [('add',{}), ('add',{})]
                windows_name_server: www.baidu.com ex: windows_name_server='www.baidu.com'
                static_ip_setting:
                [($action, **kwarg)] ex: [('delete_all', )],
                 [('delete', '00:00:00:00:00:0010.5.24.97')]
                 [('add', {'mac_address': '00:00:00:00:00:00', 'ip_address': '10.5.24.97'})]
                     add parameters:
                         mac_address: 00:00:00:00:00:00
                         ip_address:
-                        error_text: str or list
+                        text_messages: str or list
                         cancel: True, False
                 [('add', {'mac_address': '00:00:00:00:00:00', 'ip_address': '10.5.24.97', 'is_exists': '00:00:00:00:00:00'})] 如果存在则不添加
                 [('edit', '00:00:00:00:00:00', {'mac_address': '00:00:00:00:00:01'})]
                submit: True,False ex: submit=True  or submit={'tip_messages': 'submit_success'}
-               errors_text: 'ip_address_conflict' ex: errors_text='ip_address_conflict'
-               success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+               text_messages: 'ip_address_conflict' ex: text_messages='ip_address_conflict'
+               tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
                reset: True,False ex: reset=True
         :return:
         """
         self.access_menu('network.network_services.dhcp')
         self.agg_in(self.network_locators.dhcp_locators, kwargs)
 
 
@@ -656,21 +656,21 @@
                [($action, **kwarg)] ex: [('delete_all', )],
                 [('delete', 'ss.dc.com10.5.24.97')]
                 [('add', {'host': 'ss.dc.com', 'ip_address1': '10.5.24.97', 'ip_address2': '10.5.24.98'})]
                     add parameters:
                         host: ss.dc.com
                         ip_address1:
                         ip_address2:
-                        error_text: str or list
+                        text_messages: str or list
                         cancel: True, False
                 [('add', {'host': 'ss.dc.com', 'ip_address1': '10.5.24.97', 'ip_address2': '10.5.24.98', 'is_exists': 'ss.dc.com10.5.24.97'})] 如果存在则不添加
                 [('edit', 'ss.dc.com10.5.24.97', {'host': 'ss.db.com'})]
                submit_domain_ip_address_pair: True,False ex: submit_domain_ip_address_pair=True  or submit_domain_ip_address_pair={'tip_messages': 'submit_success'}
-               errors_text: 'ip_address_conflict' ex: errors_text='ip_address_conflict'
-               success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+               text_messages: 'ip_address_conflict' ex: text_messages='ip_address_conflict'
+               tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
                reset: True,False ex: reset=True
         :return:
         """
         self.access_menu('network.network_services.dns')
         self.agg_in(self.network_locators.dns_locators, kwargs)
 
 
@@ -701,24 +701,24 @@
         :param keys:
                gps_status, time_, location, speed
         """
         self.access_menu('network.network_services.gps.gps configure')
         return self.get_text(keys, self.network_locators.gps_status_locators)
 
     @allure.step('配置GPS')
-    def config(self, enable=True, success_tip='submit_success'):
+    def config(self, enable=True, tip_messages='submit_success'):
         """
 
         :param enable: True,False ex: enable=True
-        :param success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+        :param tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
         :return:
         """
         self.access_menu('network.network_services.gps.gps configure')
-        if success_tip:
-            self.agg_in(self.network_locators.gps_locators, {'enable': enable, 'success_tip': success_tip})
+        if tip_messages:
+            self.agg_in(self.network_locators.gps_locators, {'enable': enable, 'tip_messages': tip_messages})
         else:
             self.agg_in(self.network_locators.gps_locators, {'enable': enable})
 
     @allure.step('配置GPS IP Forwarding')
     def config_ip_forwarding(self, **kwargs):
         """ 需要注意的是，在不同的模式下，只有部分参数可用
 
@@ -744,21 +744,21 @@
                destination_ip_address:
                [($action, **kwarg)] ex: [('delete_all', )],
                 [('delete', 'ss.dc.com10.5.24.97')]
                 [('add', {'server': 'ss.dc.com', 'port': 10000})]
                     add parameter:
                         server:
                         port:
-                        errors_text: str or list
+                        text_messages: str or list
                         cancel: True, False
                 [('add', {'server': 'ss.dc.com', 'port': 10000, 'is_exists': 'ss.dc.com10000'})] 如果存在则不添加
                 [('edit', 'ss.dc.com10000', {'server': 'ss.db.com'})]
                submit: True,False ex: submit=True or submit={'tip_messages': 'submit_success'}
-               errors_text: 'ip_address_conflict' ex: errors_text='ip_address_conflict'
-               success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+               text_messages: 'ip_address_conflict' ex: text_messages='ip_address_conflict'
+               tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
                reset: True,False ex: reset=True
         :return:
         """
         self.access_menu('network.network_services.gps.gps ip forwarding')
         self.agg_in(self.network_locators.gps_ip_forwarding_locators, kwargs)
 
     @allure.step('配置GPS Serial Forwarding')
@@ -774,16 +774,16 @@
                stop_bit: 1,2 ex: stop_bits=1
                software_flow_control: enable,disable ex: software_flow_control='enable'
                include_rmc: enable,disable ex: include_rmc='enable'
                include_gsa: enable,disable ex: include_gsa='enable'
                include_gga: enable,disable ex: include_gga='enable'
                include_gsv: enable,disable ex: include_gsv='enable'
                submit: True,False ex: submit=True or submit={'tip_messages': 'submit_success'}
-               errors_text: 'ip_address_conflict' ex: errors_text='ip_address_conflict'
-               success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+               text_messages: 'ip_address_conflict' ex: text_messages='ip_address_conflict'
+               tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
                reset: True,False ex: reset=True
         :return:
         """
         self.access_menu('network.network_services.gps.gps serial forwarding')
         self.agg_in(self.network_locators.gps_serial_forwarding_locators, kwargs)
 
 
@@ -881,22 +881,22 @@
                         add parameter:
                             destination:
                             netmask:
                             interface:
                             gateway:
                             distance:
                             track_id:
-                            errors_text: str or list
+                            text_messages: str or list
                             cancel: True,False ex: cancel=True
                     [('edit', '0.0.0.0Gigabitethernet 0/1', {'destination': '1.1.1.1'})]
                     [('add', {'destination': '0.0.0.0', 'netmask': '10.5.24.97', 'interface': 'Gigabitethernet 0/1', 'is_exists': '10.5.24.97Gigabitethernet 0/1'})] 如果存在则不添加
                     [('edit', '10.5.24.97Gigabitethernet 0/1', {'destination': '1.1.1.1'})]
                 submit: True,False ex: submit=True  or submit={'tip_messages': 'submit_success'}
-                errors_text: 'ip_address_conflict' ex: errors_text='ip_address_conflict'
-                success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+                text_messages: 'ip_address_conflict' ex: text_messages='ip_address_conflict'
+                tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
                 reset: True ex: reset=True
         :return:
         """
         self.access_menu('network.routing.static routing')
         self.agg_in(self.network_locators.static_routing_locators, kwargs)
 
 
@@ -936,33 +936,33 @@
                         icmp_describe:  'all' or other
                         icmp_type_value:  str
                         icmp_code: str
                         fragments: enable, disable
                         established: enable, disable
                         log: enable, disable
                         destination: str
-                        error_text: str or list
+                        text_messages: str or list
                         cancel: True, False
                     [('add', {'acl_type': 'standard', 'id': 100, 'sequence_number': 40, 'is_exists': '10040'})] 如果存在则不添加
                     [('edit', '10040', {'sequence_number': 60})]
                access_control_list: [($action, **kwarg)] ex: [('delete_all', )],
                     [('delete', 'Cellular 1')]
                     [('add', {'interface': 'Cellular 1', 'in_acl': '100','out_acl': '102', 'admin_acl': '104'})]
                     add parameters:
                         interface: 'Cellular 1', 'Bridge 1', 'Openvpn 1', 'Gigabitethernet 0/1', 'Gigabitethernet 0/2',
                         in_acl: 100
                         out_acl: 100
                         admin_acl: 102
-                        error_text: str or list
+                        text_messages: str or list
                         cancel: True, False
                     [('add', {'interface': 'Cellular 1', 'in_acl': 100, 'out_acl': 102, 'is_exists': 'Cellular 1'})] 如果存在则不添加
                     [('edit', 'Cellular 1', {'in_acl': 102})]
               submit: True,False ex: submit=True  or submit={'tip_messages': 'submit_success'}
-              error_text: str ex: error_text='ip_address_conflict'
-              success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+              text_messages: str ex: text_messages='ip_address_conflict'
+              tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
               reset: True, False ex: reset=True
         """
         self.access_menu('network.firewall.acl')
         self.agg_in(self.network_locators.acl_locators, {'default_filter_strategy': default_filter_strategy}),
         if kwargs:
             self.agg_in(self.network_locators.acl_locators, kwargs)
 
@@ -999,31 +999,31 @@
                         translated_interface: 'Cellular 1'
                         translated_port: str
                         translated_end_port: str
                         source_ip: str
                         source_netmask: str
                         log: enable, disable
                         destination: str
-                        error_text: str or list
+                        text_messages: str or list
                         cancel: True, False
                     [('add', {'action': 'SNAT', 'source_network': 'inside', 'translation_type': 'IP to IP', 'is_exists': 'SNAT.*ACL:100'})] 如果存在则不添加
                     [('edit', 'SNAT.*ACL:100', {'action': 'SNAT'})]
                network_interface: [($action, **kwarg)] ex: [('delete_all', )],
                     [('delete', 'Cellular 1')]
                     [('add', {'interface': 'Cellular 1', 'interface_type': 'inside'})]
                     add parameters:
                         interface: 'Cellular 1', 'Bridge 1', 'Openvpn 1', 'Gigabitethernet 0/1', 'Gigabitethernet 0/2',
                         interface_type: inside, outside
-                        error_text: str or list
+                        text_messages: str or list
                         cancel: True, False
                     [('add', {'interface': 'Cellular 1', 'interface_type': 'inside', 'is_exists': 'Cellular 1'})] 如果存在则不添加
                     [('edit', 'Cellular 1', {'interface_type': 'outside'})]
               submit: True,False ex: submit=True  or submit={'tip_messages': 'submit_success'}
-              error_text: str ex: error_text='ip_address_conflict'
-              success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+              text_messages: str ex: text_messages='ip_address_conflict'
+              tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
               reset: True, False ex: reset=True
         """
         if kwargs:
             self.access_menu('network.firewall.nat')
             self.agg_in(self.network_locators.nat_locators, kwargs)
 
 
@@ -1104,30 +1104,30 @@
                 [('delete', 'nameyes')]
                 [('add', {'name': 'name', 'auth': 'yes', 'hostname': hostname, 'challenge_secret': challenge_secret})]
                     add parameter:
                         name:
                         auth: yes, no
                         hostname:
                         challenge_secret:
-                        errors_text: str or list
+                        text_messages: str or list
                         cancel: True, False
                 [('add', {'name': 'name', 'hostname': hostname, 'is_exists': 'nameyes'})] 如果存在则不添加
                 [('edit', 'nameyes', {'name': 'name1'})]
                 [('associate_delete', 'nameyes')]   # 删除关联项
             pseudowire_class:
                [($action, **kwarg)] ex: [('delete_all', )],
                 [('delete', 'namel2tp_class')]
                 [('add', {'name': 'name', 'l2tp_class': l2tp_class, 'source_interface': source_interface, 'data_encapsulation_method': data_encapsulation_method, 'tunnel_management_protocol': tunnel_management_protocol})]'})]
                     add parameter:
                         name:
                         l2tp_class: l2tp_class
                         source_interface: 'Cellular 1', 'Bridge 1'
                         data_encapsulation_method: 'L2TPv2', 'L2TPv3'
                         tunnel_management_protocol: 'L2TPv2', 'NONE', 'L2TPv3'
-                        errors_text: str or list
+                        text_messages: str or list
                         cancel: True, False
                 [('add', {'name': 'name', 'l2tp_class': l2tp_class, 'is_exists': 'namel2tp_class'})] 如果存在则不添加
                 [('edit', 'namel2tp_class', {'name': 'name1'})]
                 [('associate_delete', 'namel2tp_class')]   # 删除关联项
             l2tpv2_tunnel:
                [($action, **kwarg)] ex: [('delete_all', )],
                 [('delete', 'id')]
@@ -1138,15 +1138,15 @@
                         l2tp_server:
                         pseudowire_class:
                         auth_type: 'AUTO', 'PAP', 'CHAP'
                         username: str
                         password: str
                         local_ip_address: str
                         remote_ip_address: str
-                        errors_text: str or list
+                        text_messages: str or list
                         cancel: True, False
                 [('add', {'enable': True, 'id': id, 'is_exists': 'id'})] 如果存在则不添加
                 [('edit', 'id', {'enable': False})]
                 [('associate_delete', 'id')]   # 删除关联项
             l2tpv3_tunnel:
                [($action, **kwarg)] ex: [('delete_all', )],
                 [('delete', 'id')]
@@ -1156,36 +1156,36 @@
                         id: str or int
                         peer_id:
                         pseudowire_class:
                         protocol: 'IP', 'UDP'
                         source_port: int
                         destination_port: int
                         xconnect_interface: str
-                        errors_text: str or list
+                        text_messages: str or list
                         cancel: True, False
                 [('add', {'enable': True, 'id': id, 'is_exists': 'id'})] 如果存在则不添加
                 [('edit', 'id', {'enable': False})]
                 [('associate_delete', 'id')]   # 删除关联项
             l2tpv3_session:
                [($action, **kwarg)] ex: [('delete_all', )],
                 [('delete', 'local_session_id')]
                 [('add', {'local_session_id': local_session_id, 'remote_session_id': remote_session_id})]
                     add parameter:
                         local_session_id: str or int
                         remote_session_id: str or int
                         local_tunnel_id:
                         local_session_ip_address:
-                        errors_text: str or list
+                        text_messages: str or list
                         cancel: True, False
                 [('add', {'local_session_id': local_session_id, 'is_exists': 'local_session_id'})] 如果存在则不添加
                 [('edit', 'local_session_id', {'local_session_id': local_session_id})]
                 [('associate_delete', 'local_session_id')]   # 删除关联项
             submit: True,False ex: submit=True  or submit={'tip_messages': 'submit_success'}
-            errors_text: str or list
-            success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+            text_messages: str or list
+            tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
             reset: True,False ex: reset=True
         :return:
         """
         self.access_menu('network.vpn.l2tp.l2tp client')
         self.agg_in(self.network_locators.l2tp_client_locators, kwargs)
 
     @allure.step('配置L2tp Service')
@@ -1202,16 +1202,16 @@
             client_end_ip: str
             link_detection_interval:  int
             max_retries_for_link: int
             enable_mppe: True,False ex: enable_mppe=True
             enable_tunnel_auth: True,False ex: enable_tunnel_auth=True
             export_options: str
             submit: True,False ex: submit=True  or submit={'tip_messages': 'submit_success'}
-            errors_text: str or list
-            success_tip: submit_success ex: success_tip='submit_success' 提交后需要验证成功的提示框
+            text_messages: str or list
+            tip_messages: submit_success ex: tip_messages='submit_success' 提交后需要验证成功的提示框
             reset: True,False ex: reset=True
         :return:
         """
         self.access_menu('network.vpn.l2tp.l2tp service')
         self.agg_in(self.network_locators.l2tp_service_locators, kwargs)
```

### Comparing `inhandtest-0.0.57/inhandtest/pages/ingateway/network/network_locators.py` & `inhandtest-0.0.58/inhandtest/pages/ingateway/network/network_locators.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                     ('network_type', {'locator': self.pop_up.locator('#network_type'), 'type': 'select'}),
                     ('apn', {'locator': self.pop_up.locator('#apn'), 'type': 'text'}),
                     ('access_number', {'locator': self.pop_up.locator('#access_number'), 'type': 'text'}),
                     ('auth_method', {'locator': self.pop_up.locator('#auth_method'), 'type': 'select',
                                      'param': {'auto': self.locale.auto}}),
                     ('username', {'locator': self.pop_up.locator('#username'), 'type': 'text'}),
                     ('password', {'locator': self.pop_up.locator('#password'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr', 'relation': [('cellular_enable', 'enable')]}),
             ('dual_sim_enable', {'locator': self.page.locator('#enable_dual_sim'), 'type': 'switch_button',
@@ -179,16 +179,16 @@
             ('expert_options', {'locator': self.page.locator('#expert_options'), 'type': 'text',
                                 'relation': [('cellular_enable', 'enable'), ('advanced_settings', 'expand')]}),
             ('submit',
              {'locator': [self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
                           self.page.locator('.ant-modal-content').locator(
                               '//button[@class="ant-btn ant-btn-primary"]')],
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
 
 class EthernetLocators:
     def __init__(self, page: Page, locale: dict):
@@ -246,26 +246,26 @@
             ('description', {'locator': self.page.locator('#description'), 'type': 'text'}),
             ('secondary_ip_settings', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('secondary_ip', {'locator': self.pop_up.locator('#secondary_ip'), 'type': 'text'}),
                     ('netmask',
                      {'locator': self.pop_up.locator('#netmask'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
 
 class BridgeLocators:
     def __init__(self, page: Page, locale: dict):
@@ -303,28 +303,28 @@
             ('netmask', {'locator': self.page.locator('#netmask'), 'type': 'text'}),
             ('description', {'locator': self.page.locator('#description'), 'type': 'text'}),
             ('secondary_ip_settings', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('secondary_ip', {'locator': self.pop_up.locator('#secondary_ip'), 'type': 'text'}),
                     ('netmask', {'locator': self.pop_up.locator('#netmask'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr'}),
             ('ge_01', {'locator': self.page.locator('//button[@id="gigabitethernet 0/1"]'), 'type': 'switch_button'}),
             ('ge_02', {'locator': self.page.locator('//button[@id="gigabitethernet 0/2"]'), 'type': 'switch_button'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
 
 class WlanLocators:
     def __init__(self, page: Page, locale: dict):
@@ -439,16 +439,16 @@
             ('ap_bandwidth', {'locator': self.page.locator('#ap_bandwidth'), 'type': 'select',
                               'relation': [('enable_wifi', 'enable'), ('station_role', 'ap')]}),
             ('ap_stations_limit', {'locator': self.page.locator('#ap_max_associations'), 'type': 'text',
                                    'relation': [('enable_wifi', 'enable'), ('station_role', 'ap')]}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'text_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'text_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
 
 class WanLocators:
     def __init__(self, page: Page, locale: dict):
@@ -505,27 +505,27 @@
             ('description', {'locator': self.page.locator('#description'), 'type': 'text'}),
             ('secondary_ip_settings', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('secondary_ip', {'locator': self.page.locator('#secondary_ip'), 'type': 'text'}),
                     ('netmask',
                      {'locator': self.page.locator('.ant-modal-content').locator('#netmask'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
 
 class LanLocators:
     def __init__(self, page: Page, locale: dict):
@@ -564,27 +564,27 @@
             ('shutdown', {'locator': self.page.locator('#shutdown'), 'type': 'switch_button'}),
             ('secondary_ip_settings', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('secondary_ip', {'locator': self.page.locator('#secondary_ip'), 'type': 'text'}),
                     ('netmask',
                      {'locator': self.page.locator('.ant-modal-content').locator('#netmask'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
 
 class LoopbackLocators:
     def __init__(self, page: Page, locale: dict):
@@ -607,27 +607,27 @@
         return [
             ('secondary_ip_settings', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('secondary_ip', {'locator': self.page.locator('#secondary_ip'), 'type': 'text'}),
                     ('netmask',
                      {'locator': self.page.locator('.ant-modal-content').locator('#netmask'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
 
 class DhcpLocators:
     def __init__(self, page: Page, locale: dict):
@@ -647,40 +647,40 @@
                      {'locator': self.page.locator('.ant-modal-content').locator('#interface'), 'type': 'select'}),
                     ('start_address',
                      {'locator': self.page.locator('.ant-modal-content').locator('#start_addr'), 'type': 'text'}),
                     ('end_address',
                      {'locator': self.page.locator('.ant-modal-content').locator('#end_addr'), 'type': 'text'}),
                     ('lease',
                      {'locator': self.page.locator('.ant-modal-content').locator('#lease'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr'}),
             ('windows_name_server', {'locator': self.page.locator('#windows_name_server'), 'type': 'text'}),
             ('static_ip_setting', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox').nth(1),
                 "columns": [
                     ('mac_address', {'locator': self.pop_up.locator('#mac_addr'), 'type': 'text'}),
                     ('ip_address', {'locator': self.pop_up.locator('#ip_addr'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr', 'param': {'enable': self.locale.enable, 'not_enable': self.locale.not_enable}}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
 
 class DnsLocators:
     def __init__(self, page: Page, locale: dict):
@@ -701,27 +701,27 @@
             ('domain_ip_address_pair', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('host',
                      {'locator': self.pop_up.locator('#host'), 'type': 'text'}),
                     ('ip_address1', {'locator': self.pop_up.locator('#ip_addr1'), 'type': 'text'}),
                     ('ip_address2', {'locator': self.pop_up.locator('#ip_addr2'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr'}),
             ('submit_domain_ip_address_pair',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
                                            has_text=self.locale.submit).nth(1),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
 
 class GpsLocators:
     def __init__(self, page: Page, locale: dict):
@@ -797,27 +797,27 @@
             ('destination_ip_address', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('server',
                      {'locator': self.page.locator('.ant-modal-content').locator('#server_ip'), 'type': 'text'}),
                     ('port',
                      {'locator': self.page.locator('.ant-modal-content').locator('#server_port'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
     @property
     def gps_serial_forwarding_locators(self) -> list:
         return [
@@ -843,16 +843,16 @@
             ('include_gga', {'locator': self.page.locator('#gga'), 'type': 'switch_button',
                              'relation': [('enable', True)]}),
             ('include_gsv', {'locator': self.page.locator('#gsv'), 'type': 'switch_button',
                              'relation': [('enable', True)]}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
 
 class HostListLocators:
     def __init__(self, page: Page, locale: dict):
@@ -910,30 +910,30 @@
                                {'locator': self.page.locator('.ant-modal-content').locator('#gateway'),
                                 'type': 'text'}),
                               ('distance',
                                {'locator': self.page.locator('.ant-modal-content').locator('#distance'),
                                 'type': 'text'}),
                               ('track_id',
                                {'locator': self.page.locator('.ant-modal-content').locator('#track'), 'type': 'text'}),
-                              ('errors_text', {'type': 'text_messages'}),
+                              ('text_messages', {'type': 'text_messages'}),
                               ('cancel',
                                {'locator': self.page.locator('.ant-modal-content').locator(
                                    '//button[@class="ant-btn"]'),
                                    'type': 'button'}),
                               ('save',
                                {'locator': self.page.locator('.ant-modal-content').locator(
                                    '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'})]},
               'param': {'all': self.locale.all, 'connected_routing': self.locale.connected_routing,
                         'static_routing': self.locale.static_routing, 'ospf': 'OSPF', 'bgp': 'BGP',
                         'rip': 'RIP'}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
 
 class AclLocators:
     def __init__(self, page: Page, locale: dict):
@@ -989,15 +989,15 @@
                                     'type': 'switch_button'}),
                      ('established', {'locator': self.page.locator('.ant-modal-content').locator('#established'),
                                       'type': 'switch_button'}),
                      ('log', {'locator': self.page.locator('.ant-modal-content').locator('#log'),
                               'type': 'switch_button'}),
                      ('description', {'locator': self.page.locator('.ant-modal-content').locator('#description'),
                                       'type': 'text'}),
-                     ('errors_text', {'type': 'text_messages'}),
+                     ('text_messages', {'type': 'text_messages'}),
                      ('cancel',
                       {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                        'type': 'button'}),
                      ('save',
                       {'locator': self.page.locator('.ant-modal-content').locator(
                           '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'})]},
                  'type': 'table_tr'}),
@@ -1008,28 +1008,28 @@
                      ('interface', {'locator': self.page.locator('#interface'), 'type': 'select'}),
                      ('in_acl',
                       {'locator': self.page.locator('.ant-modal-content').locator('#inbound_acl'), 'type': 'select'}),
                      ('out_acl',
                       {'locator': self.page.locator('.ant-modal-content').locator('#outbound_acl'), 'type': 'select'}),
                      ('admin_acl',
                       {'locator': self.page.locator('.ant-modal-content').locator('#admin_acl'), 'type': 'select'}),
-                     ('errors_text', {'type': 'text_messages'}),
-                     ('success_tip', {'type': 'tip_messages'}),
+                     ('text_messages', {'type': 'text_messages'}),
+                     ('tip_messages', {'type': 'tip_messages'}),
                      ('cancel',
                       {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                        'type': 'button'}),
                      ('save',
                       {'locator': self.page.locator('.ant-modal-content').locator(
                           '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'})]},
                  'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
 
 class NatLocators:
     def __init__(self, page: Page, locale: dict):
@@ -1076,15 +1076,15 @@
                       {'locator': self.pop_up.locator('//div[@id="transmit_dest.interface"]'), 'type': 'select'}),
                      ('translated_port',
                       {'locator': self.pop_up.locator('//input[@id="transmit_dest.port"]'), 'type': 'text'}),
                      ('translated_end_port',
                       {'locator': self.pop_up.locator('//input[@id="transmit_dest.end_port"]'), 'type': 'text'}),
                      ('log', {'locator': self.pop_up.locator('#log'), 'type': 'switch_button'}),
                      ('description', {'locator': self.pop_up.locator('#description'), 'type': 'text'}),
-                     ('errors_text', {'type': 'text_messages'}),
+                     ('text_messages', {'type': 'text_messages'}),
                      ('cancel',
                       {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                        'type': 'button'}),
                      ('save',
                       {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'),
                        'type': 'button'})]},
                  'type': 'table_tr', 'param': {'inside': self.locale.inside, 'outside': self.locale.outside}}),
@@ -1092,27 +1092,27 @@
              {'locator': {
                  'locator': self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox').nth(1),
                  "columns": [
                      ('interface', {'locator': self.page.locator('#interface'), 'type': 'select'}),
                      ('interface_type',
                       {'locator': self.pop_up.locator('#type'), 'type': 'radio_select',
                        'param': {'inside': self.locale.inside, 'outside': self.locale.outside}}),
-                     ('errors_text', {'type': 'text_messages'}),
+                     ('text_messages', {'type': 'text_messages'}),
                      ('cancel',
                       {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                        'type': 'button'}),
                      ('save',
                       {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'),
                        'type': 'button'})]},
                  'type': 'table_tr', 'param': {'inside': self.locale.inside, 'outside': self.locale.outside}}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
 
 class L2tpLocators:
     def __init__(self, page: Page, locale: dict):
@@ -1143,15 +1143,15 @@
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table-index-tableBox').nth(0),
                 "columns": [
                     ('name', {'locator': self.pop_up.locator('#name'), 'type': 'text'}),
                     ('auth', {'locator': self.pop_up.locator('#authentication'), 'type': 'radio_select',
                               'param': {'yes': self.locale.yes, 'no': self.locale.no}}),
                     ('hostname', {'locator': self.pop_up.locator('#hostname'), 'type': 'text'}),
                     ('challenge_secret', {'locator': self.pop_up.locator('#challenge_secret'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr',
                 'param': {'yes': self.locale.yes, 'no': self.locale.no}}),
             ('pseudowire_class', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table-index-tableBox').nth(1),
@@ -1159,15 +1159,15 @@
                     ('name', {'locator': self.pop_up.locator('#name'), 'type': 'text'}),
                     ('l2tp_class', {'locator': self.pop_up.locator('#class'), 'type': 'select'}),
                     ('source_interface', {'locator': self.pop_up.locator('#source_interface'), 'type': 'select'}),
                     ('data_encapsulation_method',
                      {'locator': self.pop_up.locator('#data_encapsulation_method'), 'type': 'select'}),
                     ('tunnel_management_protocol',
                      {'locator': self.pop_up.locator('#tunnel_management_protocol'), 'type': 'select'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr'}),
             ('l2tpv2_tunnel', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table-index-tableBox').nth(2),
                 "columns": [
@@ -1177,15 +1177,15 @@
                     ('pseudowire_class', {'locator': self.pop_up.locator('#pseudowire_class'), 'type': 'select'}),
                     ('auth_type', {'locator': self.pop_up.locator('#authentication_type'), 'type': 'select',
                                    'param': {'AUTO': self.locale.auto}}),
                     ('username', {'locator': self.pop_up.locator('#username'), 'type': 'text'}),
                     ('password', {'locator': self.pop_up.locator('#password'), 'type': 'text'}),
                     ('local_ip_address', {'locator': self.pop_up.locator('#local_ip_address'), 'type': 'text'}),
                     ('remote_ip_address', {'locator': self.pop_up.locator('#remote_ip_address'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr'}),
             ('l2tpv3_tunnel', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table-index-tableBox').nth(3),
                 "columns": [
@@ -1193,37 +1193,37 @@
                     ('id', {'locator': self.pop_up.locator('#id'), 'type': 'text'}),
                     ('peer_id', {'locator': self.pop_up.locator('#peer_id'), 'type': 'text'}),
                     ('pseudowire_class', {'locator': self.pop_up.locator('#pseudowire_class'), 'type': 'select'}),
                     ('protocol', {'locator': self.pop_up.locator('#protocol'), 'type': 'select'}),
                     ('source_port', {'locator': self.pop_up.locator('#source_port'), 'type': 'text'}),
                     ('destination_port', {'locator': self.pop_up.locator('#destination_port'), 'type': 'text'}),
                     ('xconnect_interface', {'locator': self.pop_up.locator('#xconnect_interface'), 'type': 'select'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr'}),
             ('l2tpv3_session', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table-index-tableBox').nth(4),
                 "columns": [
                     ('local_session_id', {'locator': self.pop_up.locator('#local_session_id'), 'type': 'text'}),
                     ('remote_session_id', {'locator': self.pop_up.locator('#remote_session_id'), 'type': 'text'}),
                     ('local_tunnel_id', {'locator': self.pop_up.locator('#local_tunnel_id'), 'type': 'select'}),
                     ('local_session_ip_address',
                      {'locator': self.pop_up.locator('#local_session_ip_address'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr'}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
     @property
     def l2tp_service_locators(self) -> list:
         return [
@@ -1254,16 +1254,16 @@
             ('client_name', {'locator': self.page.locator('#client_name'), 'type': 'text',
                              'relation': [('enable', True), ('enable_tunnel_auth', True)]}),
             ('export_options',
              {'locator': self.page.locator('#export_options'), 'type': 'text', 'relation': [('enable', True)]}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
 
 
 class NetworkLocators(EthernetLocators, CellularLocators, BridgeLocators, WlanLocators, WanLocators, LanLocators,
                       LoopbackLocators, DhcpLocators, DnsLocators, GpsLocators, HostListLocators,
```

### Comparing `inhandtest-0.0.57/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.58/inhandtest/pages/ingateway/overview/overview.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.58/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/pages/ingateway/system/system.py` & `inhandtest-0.0.58/inhandtest/pages/ingateway/system/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                      error_text: str or list
                      cancel: True, False
                  [('add', {'server_address': '0.pool.ntp.org',  'is_exists': '0.pool.ntp.org'})] 如果存在0.pool.ntp.org则不添加
                  [('edit', '0.pool.ntp.org', {'server_address': '1.pool.ntp.org'})]
                  [('enable', '0.pool.ntp.org', True)] or  [('enable', '0.pool.ntp.org', False)]
                error_text: str or list or tuple
                submit_ntp: True or False ex: submit_ntp=True  or  submit_ntp={'tip_messages': 'apply_success'}
-               success_tip: True or False ex: success_tip=True or success_tip={'tip_messages': 'apply_success'}
+               tip_messages: True or False ex: tip_messages=True or tip_messages={'tip_messages': 'apply_success'}
         :return:
         """
         self.access_menu('system.system_time')
         self.agg_in(self.system_locators.system_time_locators, kwargs)
 
 
 class Log(BasePage, IgLocators):
@@ -148,15 +148,15 @@
                  [('edit', 'log.server.com', {'server_address': 'log.server.com.cn'})]
                  多个操作时使用列表 [('add',{}), ('add',{})]
                log_to_console： check, uncheck  ex log_to_console='check'
                history_log_file_size: str, int ex: history_log_file_size='100' or history_log_file_size=100
                history_log_level: debug, information, notice, warning, error, serious, alarm, emergency ex: history_log_level='debug'
                error_text: str or list or tuple
                submit: True or False ex: submit=True  or  submit={'tip_messages': 'submit_success'}
-               success_tip: True or False ex: success_tip=True or success_tip={'tip_messages': 'submit_success'}
+               tip_messages: True or False ex: tip_messages=True or tip_messages={'tip_messages': 'submit_success'}
         :return:
         """
         self.access_menu('system.log.configure')
         self.agg_in(self.system_locators.log_config_locators, kwargs)
 
 
 class Config(BasePage, IgLocators):
@@ -260,16 +260,16 @@
             iscada:
                 enable: True, False ex: enable=True
                 server_address: str custom ex: server_address='ics.inhandnetworks.com' or server_address='custom'
                 custom_address: str ex: custom_address='ics.inhandnetworks.com'
                 keepalive: int ex: keepalive=60
             all:
                 submit: True, False ex: submit=True or submit={'tip_messages': 'submit_success'}
-                errors_text:
-                success_tip:
+                text_messages:
+                tip_messages:
         :return:
         """
         if platform == 'ics':
             self.access_menu('system.inhand cloud.inhand connect service')
         elif platform == 'dm':
             self.access_menu('system.inhand cloud.inhand device manager')
         else:
@@ -398,16 +398,16 @@
                         cancel: True, False
                 [('add', {'source_network': '10.5.24.97', 'ip_wildcard': '', 'is_exists': '10.5.24.97'})] 如果存在则不添加
                 [('edit', '10.5.24.97', {'source_network': '10.5.24.98'})]
           enable_developer: True, False ex: enable_developer=True
           enable_fixed_password: True, False ex: enable_fixed_password=True
           fixed_password: str ex: fixed_password='123456'
           submit: True, False ex: submit=True or submit={'tip_messages': 'submit_success'}
-          errors_text: str or list
-          success_tip: str or list
+          text_messages: str or list
+          tip_messages: str or list
         :return:
         """
         self.access_menu('system.access tools')
         self.agg_in(self.system_locators.access_tools_locators, kwargs)
 
 
 class UserManagement(BasePage, IgLocators):
@@ -482,15 +482,15 @@
         :param lost_package: None, True, False 是否丢包
         :param kwargs:
                host: str ex: host='www.baidu.com'
                count: int ex: count=4
                size: int ex: size=32
                experts_option: str 高级选项
                ping: True, False ex: ping=True
-               errors_text: str or list
+               text_messages: str or list
         :return:
         """
         self.access_menu('system.network tools')
         if kwargs.get('ping') is None:
             kwargs.update({'ping': True})
         self.agg_in(self.system_locators.ping_locators, kwargs)
         if kwargs.get('ping'):
@@ -512,15 +512,15 @@
         :param kwargs:
                host: 地址 IP
                max_hop: 最大跳数 2-40
                timeout: 超时时间 2-10s
                protocol: UDP|ICMP 协议
                experts_option:专家选项
                trace: True|False 是否点击Trace
-               errors_text: str or list
+               text_messages: str or list
 
         :return:
         """
         self.access_menu('system.network tools')
         if kwargs.get('trace') is None:
             kwargs.update({'trace': True})
         self.agg_in(self.system_locators.trace_locators, kwargs)
@@ -539,15 +539,15 @@
     def tcp_dump(self, **kwargs):
         """抓包操作
 
         :param kwargs:
             interface: Any|Cellular 1|Gigabitethernet 0/1|Bridge 1 接口
             number:抓包个数 10-1000
             experts_option: 专家选项
-            errors_text: str or list
+            text_messages: str or list
             start_capture: True|False 是否点击开始抓包
             download: {'file_path': './', 'file_name': 'xxx.pcap'} 下载文件
         :return:
         """
         self.access_menu('system.network tools')
         if kwargs.get('start_capture') is None:
             kwargs.update({'start_capture': True})
```

### Comparing `inhandtest-0.0.57/inhandtest/pages/ingateway/system/system_locators.py` & `inhandtest-0.0.58/inhandtest/pages/ingateway/system/system_locators.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             ('sntp_interval', {'locator': self.page.locator('#update_interval'), 'type': 'text',
                                'relation': [('enable_sntp_clients', True)]}),
             ('sntp_servers', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('server_address', {'locator': self.pop_up.locator('#server_addr'), 'type': 'text'}),
                     ('port', {'locator': self.pop_up.locator('#port'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr', 'relation': [('enable_sntp_clients', True)]}),
             ('submit_sntp',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
                                            has_text=self.locale.submit).nth(0),
@@ -74,25 +74,25 @@
                            'relation': [('enable_ntp_server', True)]}),
             ('ntp_servers', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table-index-outerBox'),
                 'action_confirm': self.page.locator('.ant-popover-inner').locator(
                     '.ant-btn.ant-btn-primary.ant-btn-sm'),
                 "columns": [
                     ('server_address', {'locator': self.pop_up.locator('#server_addr'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr'}),
             ('submit_ntp',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
                                            has_text=self.locale.submit).nth(1),
               'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
         ]
 
 
 class LogLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -129,15 +129,15 @@
         return [
             ('enable_remote_server', {'locator': self.page.locator('#log_to_remote_enable'), 'type': 'check'}),
             ('remote_server', {'locator': {
                 "locator": self.page.locator('.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('server_address', {'locator': self.pop_up.locator('#server_addr'), 'type': 'text'}),
                     ('port', {'locator': self.pop_up.locator('#server_port'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'), 'type': 'button'}),
                     ('save',
                      {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr', 'relation': [('enable_remote_server', True)]}),
             ('log_to_console', {'locator': self.page.locator('#log_to_console'), 'type': 'check'}),
             ('history_log_file_size',
              {'locator': self.page.locator('//input[@class="ant-input-number-input"]'), 'type': 'text'}),
@@ -146,16 +146,16 @@
               'param': {'emergency': self.locale.emergency, 'alarm': self.locale.alarm,
                         'serious': self.locale.serious, 'error': self.locale.error, 'warning': self.locale.warning,
                         'notice': self.locale.notice, 'information': self.locale.information,
                         'debug': self.locale.debug}}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
                                            has_text=self.locale.submit), 'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
         ]
 
 
 class ConfigLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -244,16 +244,16 @@
             ('keepalive', {'locator': self.page.locator('#channel_keepalive'), 'type': 'text',
                            'relation': [('enable', True), ('advance_settings', 'expand')]}),
             ('data_upload_interval', {'locator': self.page.locator('#dataflow_upload_interval'), 'type': 'text',
                                       'relation': [('enable', True), ('advance_settings', 'expand')]}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
                                            has_text=self.locale.submit), 'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
         ]
 
 
 class FirmwareLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -323,15 +323,15 @@
                 "locator": self.page.locator('//label[@for="https.enable.form"]').locator('../../..').locator(
                     '.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('source_network',
                      {'locator': self.pop_up.locator('#source_network'), 'type': 'text'}),
                     ('ip_wildcard',
                      {'locator': self.pop_up.locator('#wildcard_mask'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr', 'relation': [('https_remote_access', 'enable')]}),
@@ -350,15 +350,15 @@
                 "locator": self.page.locator('//label[@for="telnet.enable.form"]').locator('../../..').locator(
                     '.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('source_network',
                      {'locator': self.pop_up.locator('#source_network'), 'type': 'text'}),
                     ('ip_wildcard',
                      {'locator': self.pop_up.locator('#wildcard_mask'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr',
@@ -382,15 +382,15 @@
                 "locator": self.page.locator('//label[@for="ssh.enable.form"]').locator('../../..').locator(
                     '.antd-pro-components-in-gateway-editable-table1-index-outerBox'),
                 "columns": [
                     ('source_network',
                      {'locator': self.pop_up.locator('#source_network'), 'type': 'text'}),
                     ('ip_wildcard',
                      {'locator': self.pop_up.locator('#wildcard_mask'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button'}),
                 ]}, 'type': 'table_tr',
@@ -404,16 +404,16 @@
             (
                 'fixed_password',
                 {'locator': self.page.locator('//input[@id="devlopMode.debug_password"]'), 'type': 'text',
                  'relation': [('enable_developer', 'enable'), ('enable_fixed_password', 'enable')]}),
             ('submit',
              {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]',
                                            has_text=self.locale.submit), 'type': 'button'}),
-            ('errors_text', {'type': 'text_messages'}),
-            ('success_tip', {'type': 'tip_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
+            ('tip_messages', {'type': 'tip_messages'}),
         ]
 
 
 class UserLocators:
     def __init__(self, page: Page, locale: dict):
         self.page = page
         self.locale = locale
@@ -428,15 +428,15 @@
                     '.ant-btn.ant-btn-primary.ant-btn-sm').first,
                 "columns": [
                     ('username',
                      {'locator': self.pop_up.locator('#username'), 'type': 'text'}),
                     ('permission', {'locator': self.pop_up.locator('#privilege'), 'type': 'select'}),
                     ('password', {'locator': self.pop_up.locator('#password'), 'type': 'text'}),
                     ('confirm_password', {'locator': self.pop_up.locator('#passwordConfirm'), 'type': 'text'}),
-                    ('errors_text', {'type': 'text_messages'}),
+                    ('text_messages', {'type': 'text_messages'}),
                     ('cancel',
                      {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn"]'),
                       'type': 'button'}),
                     ('save',
                      {'locator': self.page.locator('.ant-modal-content').locator(
                          '//button[@class="ant-btn ant-btn-primary"]'), 'type': 'button',
                          'wait_for': {'type': 'timeout', 'timeout': 3 * 1000}}),
@@ -476,43 +476,43 @@
     @property
     def ping_locators(self) -> list:
         return [
             ('host', {'locator': self.page.locator('#host').nth(0), 'type': 'text'}),
             ('count', {'locator': self.page.locator('#ping_count').nth(0), 'type': 'text'}),
             ('size', {'locator': self.page.locator('#packet_size').nth(0), 'type': 'text'}),
             ('expert_options', {'locator': self.page.locator('#expert_options').nth(0), 'type': 'text'}),
-            ('errors_text', {'type': 'text_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
             ('ping', {'locator': self.page.locator('//button[@type="submit"]').nth(0), 'type': 'button'}),
             ('close',
              {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn ant-btn-primary"]'),
               'type': 'button'}),
         ]
 
     @property
     def trace_locators(self) -> list:
         return [
             ('host', {'locator': self.page.locator('#host').nth(1), 'type': 'text'}),
             ('max_hop', {'locator': self.page.locator('#maximum_hops').nth(0), 'type': 'text'}),
             ('timeout', {'locator': self.page.locator('#timeout').nth(0), 'type': 'text'}),
             ('protocol', {'locator': self.page.locator('#transmit_protocol').nth(0), 'type': 'select'}),
             ('expert_options', {'locator': self.page.locator('#expert_options').nth(1), 'type': 'text'}),
-            ('errors_text', {'type': 'text_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
             ('trace', {'locator': self.page.locator('//button[@type="submit"]').nth(1), 'type': 'button'}),
             ('close',
              {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn ant-btn-primary"]'),
               'type': 'button'}),
         ]
 
     @property
     def tcpdump_locators(self) -> list:
         return [
             ('interface', {'locator': self.page.locator('#interface'), 'type': 'select'}),
             ('number', {'locator': self.page.locator('#capture_number'), 'type': 'text'}),
             ('expert_options', {'locator': self.page.locator('#expert_options').nth(2), 'type': 'text'}),
-            ('errors_text', {'type': 'text_messages'}),
+            ('text_messages', {'type': 'text_messages'}),
             ('start_capture',
              {'locator': self.page.locator('//button', has_text=self.locale.start_capture), 'type': 'button',
               'wait_for': [{'type': 'visible', 'timeout': 300 * 1000,
                            'locator': self.page.locator('//button', has_text=self.locale.start_capture)},
                            {'type': 'timeout', 'timeout': 1 * 1000}]}),
             ('download',
              {'locator': self.page.locator('//button', has_text=self.locale.download_capture_file),
```

### Comparing `inhandtest-0.0.57/inhandtest/pytest_email.html` & `inhandtest-0.0.58/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/telnet.py` & `inhandtest-0.0.58/inhandtest/telnet.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.57/inhandtest/tools.py` & `inhandtest-0.0.58/inhandtest/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,18 @@
                 conn_list = proc.connections()
             except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
                 continue
             for conn in conn_list:
                 if conn.status == psutil.CONN_LISTEN and conn.laddr.port == one_port:
                     logging.debug(f"process {proc.pid} already use port {one_port}")
                     # 终止进程
-                    proc.kill()
+                    try:
+                        proc.kill()
+                    except psutil.NoSuchProcess:
+                        pass
                     logging.info(f"kill process {proc.pid} success")
 
     def port_is_close(one_port: int):  # 杀死后要一直等到进程完全退出才能继续执行，否则会报错
         for i in range(0, 15):
             with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
                 try:
                     s.bind((ip_, one_port))
```

### Comparing `inhandtest-0.0.57/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.58/inhandtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.57
+Version: 0.0.58
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.57/inhandtest.egg-info/SOURCES.txt` & `inhandtest-0.0.58/inhandtest.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
-dm/mqtt.py
-dm/register_v1.py
 inhandtest/__init__.py
 inhandtest/exception.py
 inhandtest/file.py
 inhandtest/inmodbus.py
 inhandtest/inmongodb.py
 inhandtest/inmqtt.py
 inhandtest/inrequest.py
```

### Comparing `inhandtest-0.0.57/setup.py` & `inhandtest-0.0.58/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.57',
+    version='0.0.58',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

