# Comparing `tmp/zhmcclient-1.8.1.tar.gz` & `tmp/zhmcclient-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhmcclient-1.8.1.tar", last modified: Fri May 26 15:03:24 2023, max compression
+gzip compressed data, was "zhmcclient-1.8.2.tar", last modified: Mon Jul  3 17:23:31 2023, max compression
```

## Comparing `zhmcclient-1.8.1.tar` & `zhmcclient-1.8.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:03:24.336064 zhmcclient-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-26 15:03:20.000000 zhmcclient-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-26 15:03:24.332064 zhmcclient-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/extra-testutils-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:03:24.336064 zhmcclient-1.8.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5458 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:03:24.328064 zhmcclient-1.8.1/zhmcclient/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_activation_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    27187 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_capacity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32528 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    94301 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_debug_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    46440 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_hba.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_ldap_server_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    78470 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_lpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    33251 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    36561 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_nic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15902 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_password_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_port.py
--rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_resource_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    69538 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    33564 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_storage_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_storage_group_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    25230 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_storage_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_storage_volume_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_timestats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_unmanaged_cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_user_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_virtual_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_virtual_storage_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_virtual_switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:03:24.332064 zhmcclient-1.8.1/zhmcclient/testutils/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/testutils/_cpc_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/testutils/_hmc_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/testutils/_hmc_definition_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/testutils/_hmc_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/testutils/_hmc_inventory_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/testutils/_hmc_vault_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:03:24.332064 zhmcclient-1.8.1/zhmcclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-26 15:03:24.000000 zhmcclient-1.8.1/zhmcclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-26 15:03:24.000000 zhmcclient-1.8.1/zhmcclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:03:24.000000 zhmcclient-1.8.1/zhmcclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-26 15:03:24.000000 zhmcclient-1.8.1/zhmcclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 15:03:24.000000 zhmcclient-1.8.1/zhmcclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:02:39.000000 zhmcclient-1.8.1/zhmcclient.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:03:24.332064 zhmcclient-1.8.1/zhmcclient_mock/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   134108 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient_mock/_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient_mock/_idpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    42583 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient_mock/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)   201548 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient_mock/_urihandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:23:31.914493 zhmcclient-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-03 17:23:27.000000 zhmcclient-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-07-03 17:23:31.914493 zhmcclient-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/extra-testutils-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:23:31.914493 zhmcclient-1.8.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5458 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:23:31.910493 zhmcclient-1.8.2/zhmcclient/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_activation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27187 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_capacity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32528 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94301 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46440 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_hba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_ldap_server_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78470 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_lpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33251 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36561 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_nic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15902 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_password_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_resource_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69684 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33564 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_storage_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_storage_group_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25230 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_storage_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_storage_volume_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_timestats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_unmanaged_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_user_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_virtual_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_virtual_storage_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/_virtual_switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:23:31.914493 zhmcclient-1.8.2/zhmcclient/testutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/testutils/_cpc_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/testutils/_hmc_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/testutils/_hmc_definition_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/testutils/_hmc_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/testutils/_hmc_inventory_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient/testutils/_hmc_vault_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:23:31.910493 zhmcclient-1.8.2/zhmcclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-07-03 17:23:31.000000 zhmcclient-1.8.2/zhmcclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-03 17:23:31.000000 zhmcclient-1.8.2/zhmcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:23:31.000000 zhmcclient-1.8.2/zhmcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-03 17:23:31.000000 zhmcclient-1.8.2/zhmcclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 17:23:31.000000 zhmcclient-1.8.2/zhmcclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:22:48.000000 zhmcclient-1.8.2/zhmcclient.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:23:31.914493 zhmcclient-1.8.2/zhmcclient_mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134108 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient_mock/_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient_mock/_idpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42583 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient_mock/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)   201548 2023-07-03 17:22:37.000000 zhmcclient-1.8.2/zhmcclient_mock/_urihandler.py
```

### Comparing `zhmcclient-1.8.1/LICENSE` & `zhmcclient-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/MANIFEST.in` & `zhmcclient-1.8.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/PKG-INFO` & `zhmcclient-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmcclient
-Version: 1.8.1
+Version: 1.8.2
 Summary: A pure Python client library for the IBM Z HMC Web Services API.
 Home-page: https://github.com/zhmcclient/python-zhmcclient
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmcclient-1.8.1/README.rst` & `zhmcclient-1.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/extra-testutils-requirements.txt` & `zhmcclient-1.8.2/extra-testutils-requirements.txt`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/requirements.txt` & `zhmcclient-1.8.2/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 # pytz 2019.1 fixes an ImportError for collections.Mapping on Python 3.10
 pytz>=2016.10; python_version <= '3.9'  # MIT
 pytz>=2019.1; python_version >= '3.10'  # MIT
 
 # requests 2.25.0 tolerates urllib3 1.26.5 which is needed on Python 3.10 to
 #   remove ImportWarning in six
-requests>=2.25.0  # Apache-2.0
+requests>=2.25.0; python_version <= '3.6'
+requests>=2.31.0; python_version >= '3.7'
 
 # six 1.16.0 removes the ImportWarning raised by Python 3.10
 six>=1.14.0; python_version <= '3.9'  # MIT
 six>=1.16.0; python_version >= '3.10'  # MIT
 
 # stomp.py 5.0.0 (now deleted) and 6.0.0 removed support for Python 2.7, 3.4 and 3.5
 # stomp.py 6.1.0 on Pypi contained older code than v6.1.0 in the repo -> will be yanked on Pypi
```

### Comparing `zhmcclient-1.8.1/setup.py` & `zhmcclient-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/__init__.py` & `zhmcclient-1.8.2/zhmcclient/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_activation_profile.py` & `zhmcclient-1.8.2/zhmcclient/_activation_profile.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_adapter.py` & `zhmcclient-1.8.2/zhmcclient/_adapter.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_capacity_group.py` & `zhmcclient-1.8.2/zhmcclient/_capacity_group.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_certificates.py` & `zhmcclient-1.8.2/zhmcclient/_certificates.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_client.py` & `zhmcclient-1.8.2/zhmcclient/_client.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_console.py` & `zhmcclient-1.8.2/zhmcclient/_console.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_constants.py` & `zhmcclient-1.8.2/zhmcclient/_constants.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_cpc.py` & `zhmcclient-1.8.2/zhmcclient/_cpc.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_debug_info.py` & `zhmcclient-1.8.2/zhmcclient/_debug_info.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_exceptions.py` & `zhmcclient-1.8.2/zhmcclient/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_group.py` & `zhmcclient-1.8.2/zhmcclient/_group.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_hba.py` & `zhmcclient-1.8.2/zhmcclient/_hba.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_ldap_server_definition.py` & `zhmcclient-1.8.2/zhmcclient/_ldap_server_definition.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_logging.py` & `zhmcclient-1.8.2/zhmcclient/_logging.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_lpar.py` & `zhmcclient-1.8.2/zhmcclient/_lpar.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_manager.py` & `zhmcclient-1.8.2/zhmcclient/_manager.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_metrics.py` & `zhmcclient-1.8.2/zhmcclient/_metrics.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_nic.py` & `zhmcclient-1.8.2/zhmcclient/_nic.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_notification.py` & `zhmcclient-1.8.2/zhmcclient/_notification.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_partition.py` & `zhmcclient-1.8.2/zhmcclient/_partition.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_password_rule.py` & `zhmcclient-1.8.2/zhmcclient/_password_rule.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_port.py` & `zhmcclient-1.8.2/zhmcclient/_port.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_resource.py` & `zhmcclient-1.8.2/zhmcclient/_resource.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_resource_updater.py` & `zhmcclient-1.8.2/zhmcclient/_resource_updater.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_session.py` & `zhmcclient-1.8.2/zhmcclient/_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -798,15 +798,17 @@
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.ConnectionError`
         """
         session_uri = '/api/sessions/this-session'
         try:
             self.delete(session_uri, logon_required=False, renew_session=False)
-        except ServerAuthError:
+        except (ServerAuthError, ConnectionError):
+            # HMC shutdown or broken network causes ConnectionError.
+            # Invalid credentials cause ServerAuthError.
             pass
         self._session_id = None
         self._session = None
         self._headers.pop('X-API-Session', None)
         self._object_topic = None
         self._job_topic = None
 
@@ -1219,15 +1221,15 @@
                 return _result_object(result)
 
             if result.status_code == 204:
                 # No content
                 return None
 
             if result.status_code == 202:
-                if result.content == '':
+                if result.content == b'':
                     # Some operations (e.g. "Restart Console",
                     # "Shutdown Console" or "Cancel Job") return 202
                     # with no response content.
                     return None
 
                 # This is the most common case to return 202: An
                 # asynchronous job has been started.
```

### Comparing `zhmcclient-1.8.1/zhmcclient/_storage_group.py` & `zhmcclient-1.8.2/zhmcclient/_storage_group.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_storage_group_template.py` & `zhmcclient-1.8.2/zhmcclient/_storage_group_template.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_storage_volume.py` & `zhmcclient-1.8.2/zhmcclient/_storage_volume.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_storage_volume_template.py` & `zhmcclient-1.8.2/zhmcclient/_storage_volume_template.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_task.py` & `zhmcclient-1.8.2/zhmcclient/_task.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_timestats.py` & `zhmcclient-1.8.2/zhmcclient/_timestats.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_unmanaged_cpc.py` & `zhmcclient-1.8.2/zhmcclient/_unmanaged_cpc.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_user.py` & `zhmcclient-1.8.2/zhmcclient/_user.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_user_pattern.py` & `zhmcclient-1.8.2/zhmcclient/_user_pattern.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_user_role.py` & `zhmcclient-1.8.2/zhmcclient/_user_role.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_utils.py` & `zhmcclient-1.8.2/zhmcclient/_utils.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_version.py` & `zhmcclient-1.8.2/zhmcclient/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.P.dev1": A not yet released version M.N.P
 #: * "M.N.P": A released version M.N.P
-__version__ = '1.8.1'
+__version__ = '1.8.2'
 
 # Check supported Python versions
 # Keep these Python versions in sync with:
 # - python_requires and classifiers in setup.py
 # - Section "Supported environments" in docs/intro.rst
 _PYTHON_M = sys.version_info[0]
 _PYTHON_N = sys.version_info[1]
```

### Comparing `zhmcclient-1.8.1/zhmcclient/_virtual_function.py` & `zhmcclient-1.8.2/zhmcclient/_virtual_function.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_virtual_storage_resource.py` & `zhmcclient-1.8.2/zhmcclient/_virtual_storage_resource.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/_virtual_switch.py` & `zhmcclient-1.8.2/zhmcclient/_virtual_switch.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/testutils/__init__.py` & `zhmcclient-1.8.2/zhmcclient/testutils/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/testutils/_cpc_fixtures.py` & `zhmcclient-1.8.2/zhmcclient/testutils/_cpc_fixtures.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/testutils/_hmc_definition.py` & `zhmcclient-1.8.2/zhmcclient/testutils/_hmc_definition.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/testutils/_hmc_definition_fixtures.py` & `zhmcclient-1.8.2/zhmcclient/testutils/_hmc_definition_fixtures.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/testutils/_hmc_definitions.py` & `zhmcclient-1.8.2/zhmcclient/testutils/_hmc_definitions.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/testutils/_hmc_inventory_file.py` & `zhmcclient-1.8.2/zhmcclient/testutils/_hmc_inventory_file.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient/testutils/_hmc_vault_file.py` & `zhmcclient-1.8.2/zhmcclient/testutils/_hmc_vault_file.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient.egg-info/PKG-INFO` & `zhmcclient-1.8.2/zhmcclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmcclient
-Version: 1.8.1
+Version: 1.8.2
 Summary: A pure Python client library for the IBM Z HMC Web Services API.
 Home-page: https://github.com/zhmcclient/python-zhmcclient
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmcclient-1.8.1/zhmcclient.egg-info/SOURCES.txt` & `zhmcclient-1.8.2/zhmcclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient_mock/__init__.py` & `zhmcclient-1.8.2/zhmcclient_mock/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient_mock/_hmc.py` & `zhmcclient-1.8.2/zhmcclient_mock/_hmc.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient_mock/_idpool.py` & `zhmcclient-1.8.2/zhmcclient_mock/_idpool.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient_mock/_session.py` & `zhmcclient-1.8.2/zhmcclient_mock/_session.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.1/zhmcclient_mock/_urihandler.py` & `zhmcclient-1.8.2/zhmcclient_mock/_urihandler.py`

 * *Files identical despite different names*

