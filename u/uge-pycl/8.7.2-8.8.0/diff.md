# Comparing `tmp/uge-pycl-8.7.2.tar.gz` & `tmp/uge-pycl-8.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uge-pycl-8.7.2.tar", last modified: Tue Aug 23 16:12:07 2022, max compression
+gzip compressed data, was "dist/uge-pycl-8.8.0.tar", last modified: Mon Jul  3 09:48:13 2023, max compression
```

## Comparing `uge-pycl-8.7.2.tar` & `uge-pycl-8.8.0.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2758 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/README.md
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      476 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test_values.json
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge/
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge/exceptions/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1502 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/exceptions/qmaster_unreachable.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1504 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/exceptions/object_already_exists.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2389 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/exceptions/command_failed.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3227 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/exceptions/ar_exception.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1490 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/exceptions/invalid_argument.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1496 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/exceptions/configuration_error.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1496 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/exceptions/authorization_error.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1486 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/exceptions/invalid_request.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3169 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/exceptions/qconf_exception.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1450 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/exceptions/__init__.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1489 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/exceptions/object_not_found.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge/utility/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4924 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/utility/uge_subprocess.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/utility/__init__.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge/api/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    11073 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/ar_api.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)   165937 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/api/qconf_api.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      912 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/__init__.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge/api/impl/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4103 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/api/impl/share_tree_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1665 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/operator_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2200 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/job_class_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2164 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/calendar_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1860 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/admin_host_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1915 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/ar_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1810 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/api/impl/submit_host_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4110 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/list_based_object_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3448 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/complex_configuration_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5375 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/api/impl/qrdel_executor.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2146 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/api/impl/user_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6500 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/dict_list_based_object_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1996 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/cluster_queue_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2644 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/execution_host_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4514 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/access_list_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1663 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/manager_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7286 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/qconf_executor.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    13007 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/dict_based_object_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2202 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/host_group_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1923 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/api/impl/resource_quota_set_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6267 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/api/impl/qrstat_executor.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2212 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/api/impl/scheduler_configuration_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/__init__.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2016 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/parallel_environment_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2028 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/checkpointing_environment_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2166 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/project_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3017 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/uge/api/impl/cluster_configuration_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5443 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/api/impl/qrsub_executor.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge/constants/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1084 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/constants/uge_status.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      820 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/constants/__init__.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge/log/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3585 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/log/logger_factory.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1666 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/log/trace_log_record.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    12739 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/log/log_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2498 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/log/trace_logger.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/log/__init__.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1581 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/log/stream_log_handler.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1780 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/log/timed_rotating_file_log_handler.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge/cli/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2806 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/cli/qconf_convert.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7353 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/cli/qconf_cli.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/cli/__init__.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge/objects/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2418 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/user_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5306 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/qconf_dict_list.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    17367 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/complex_configuration_v3_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4201 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/resource_quota_set_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5107 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/ar_object_factory.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6306 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/cluster_configuration_v2_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2711 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/qconf_name_list.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3077 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/share_tree_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2766 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/checkpointing_environment_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2629 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/advance_reservation_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2970 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/execution_host_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2500 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/host_group_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2841 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/parallel_environment_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2416 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/calendar_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4403 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/scheduler_configuration_v3_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4173 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/job_class_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    16092 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/complex_configuration_v2_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2557 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/access_list_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4271 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/job_class_v3_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4205 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/job_class_v2_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    12097 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/qconf_object_factory.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7104 2022-08-12 11:28:14.000000 uge-pycl-8.7.2/uge/objects/uge_release_object_map.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4366 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/scheduler_configuration_v2_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6276 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/cluster_configuration_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6752 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/complex_configuration_base.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2920 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/parallel_environment_v2_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4311 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/cluster_queue_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    14875 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/qconf_object.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    22217 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/complex_configuration_v4_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/__init__.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    15716 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/complex_configuration_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4373 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/cluster_queue_v2_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4200 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/scheduler_configuration_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4232 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/job_class_v4_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2531 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/objects/project_v1_0.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      846 2022-08-12 11:28:14.000000 uge-pycl-8.7.2/uge/__init__.py
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge/config/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    11839 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/config/config_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2022-08-11 15:04:14.000000 uge-pycl-8.7.2/uge/config/__init__.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)       60 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/MANIFEST.in
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge_pycl.egg-info/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)        1 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge_pycl.egg-info/dependency_links.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3972 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge_pycl.egg-info/SOURCES.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)       61 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge_pycl.egg-info/entry_points.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4273 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge_pycl.egg-info/PKG-INFO
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)       20 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge_pycl.egg-info/requires.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      105 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/uge_pycl.egg-info/top_level.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4273 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/PKG-INFO
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/test/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3240 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_ar.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4260 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_job_class.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5894 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_user.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7437 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_project.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6629 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_access_list.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5859 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_share_tree.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2665 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_admin_host.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5599 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_parallel_environment.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5764 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_cluster_queue.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2259 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_operator.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5705 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_checkpointing_environment.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2262 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_cluster_configuration.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2471 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_submit_host.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3322 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_complex_configuration.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3164 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_resource_quota_set.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2238 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2277 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_scheduler_configuration.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6386 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_host_group.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5823 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_calendar.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5303 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/test_execution_host.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4885 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/test/utils.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2886 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/README.rst
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      237 2022-08-23 16:12:07.000000 uge-pycl-8.7.2/setup.cfg
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2834 2022-08-11 15:04:13.000000 uge-pycl-8.7.2/setup.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:48:13.000000 uge-pycl-8.8.0/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2758 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/README.md
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      476 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test_values.json
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/uge/
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/uge/exceptions/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1502 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/exceptions/qmaster_unreachable.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1504 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/exceptions/object_already_exists.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2389 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/exceptions/command_failed.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3227 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/exceptions/ar_exception.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1490 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/exceptions/invalid_argument.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1496 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/exceptions/configuration_error.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1496 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/exceptions/authorization_error.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1486 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/exceptions/invalid_request.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3169 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/exceptions/qconf_exception.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1450 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/exceptions/__init__.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1489 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/exceptions/object_not_found.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:48:13.000000 uge-pycl-8.8.0/uge/utility/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4924 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/utility/uge_subprocess.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/utility/__init__.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/uge/api/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    11073 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/ar_api.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)   165937 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/qconf_api.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      912 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/__init__.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/uge/api/impl/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4103 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/share_tree_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1665 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/operator_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2200 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/job_class_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2164 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/calendar_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1860 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/admin_host_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1915 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/ar_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1810 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/submit_host_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4110 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/list_based_object_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3448 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/complex_configuration_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5375 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/qrdel_executor.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2146 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/user_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6500 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/dict_list_based_object_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1996 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/cluster_queue_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2644 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/execution_host_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4514 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/access_list_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1663 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/manager_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7286 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/qconf_executor.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    13007 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/dict_based_object_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2202 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/host_group_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1923 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/resource_quota_set_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6267 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/qrstat_executor.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2212 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/scheduler_configuration_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/__init__.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2016 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/parallel_environment_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2028 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/checkpointing_environment_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2166 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/project_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3017 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/cluster_configuration_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5443 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/api/impl/qrsub_executor.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/uge/constants/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1084 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/constants/uge_status.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      820 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/constants/__init__.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/uge/log/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3585 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/log/logger_factory.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1666 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/log/trace_log_record.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    12739 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/log/log_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2498 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/log/trace_logger.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/log/__init__.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1581 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/log/stream_log_handler.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1780 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/log/timed_rotating_file_log_handler.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/uge/cli/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2806 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/cli/qconf_convert.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7353 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/cli/qconf_cli.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/cli/__init__.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:48:13.000000 uge-pycl-8.8.0/uge/objects/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2418 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/user_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5306 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/qconf_dict_list.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    17367 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/complex_configuration_v3_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4201 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/resource_quota_set_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5107 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/ar_object_factory.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6306 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/cluster_configuration_v2_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2711 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/qconf_name_list.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3077 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/share_tree_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2766 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/checkpointing_environment_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2629 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/advance_reservation_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2970 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/execution_host_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2500 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/host_group_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2841 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/parallel_environment_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2416 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/calendar_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4403 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/scheduler_configuration_v3_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4173 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/job_class_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    16092 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/complex_configuration_v2_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2557 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/access_list_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4271 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/job_class_v3_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4205 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/job_class_v2_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    12097 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/qconf_object_factory.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7625 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/uge_release_object_map.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4366 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/scheduler_configuration_v2_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6276 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/cluster_configuration_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6752 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/complex_configuration_base.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2920 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/parallel_environment_v2_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4311 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/cluster_queue_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    14875 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/qconf_object.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    22217 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/complex_configuration_v4_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/__init__.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    15716 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/complex_configuration_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4373 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/cluster_queue_v2_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4200 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/scheduler_configuration_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4232 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/job_class_v4_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2531 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/objects/project_v1_0.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      846 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/__init__.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/uge/config/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    11839 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/config/config_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      824 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/uge/config/__init__.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)       60 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/MANIFEST.in
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:48:13.000000 uge-pycl-8.8.0/uge_pycl.egg-info/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)        1 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/uge_pycl.egg-info/dependency_links.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3972 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/uge_pycl.egg-info/SOURCES.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)       61 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/uge_pycl.egg-info/entry_points.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4273 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/uge_pycl.egg-info/PKG-INFO
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)       20 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/uge_pycl.egg-info/requires.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      105 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/uge_pycl.egg-info/top_level.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4273 2023-07-03 09:48:13.000000 uge-pycl-8.8.0/PKG-INFO
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:48:12.000000 uge-pycl-8.8.0/test/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3240 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_ar.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4260 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_job_class.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5894 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_user.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7437 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_project.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6629 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_access_list.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5859 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_share_tree.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2665 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_admin_host.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5599 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_parallel_environment.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5764 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_cluster_queue.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2259 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_operator.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5705 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_checkpointing_environment.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2262 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_cluster_configuration.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2471 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_submit_host.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3322 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_complex_configuration.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3164 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_resource_quota_set.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2238 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2277 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_scheduler_configuration.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6386 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_host_group.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5823 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_calendar.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5303 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/test_execution_host.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4885 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/test/utils.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2886 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/README.rst
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      237 2023-07-03 09:48:13.000000 uge-pycl-8.8.0/setup.cfg
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2834 2023-06-28 12:36:01.000000 uge-pycl-8.8.0/setup.py
```

### Comparing `uge-pycl-8.7.2/README.md` & `uge-pycl-8.8.0/README.md`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/exceptions/qmaster_unreachable.py` & `uge-pycl-8.8.0/uge/exceptions/qmaster_unreachable.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/exceptions/object_already_exists.py` & `uge-pycl-8.8.0/uge/exceptions/object_already_exists.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/exceptions/command_failed.py` & `uge-pycl-8.8.0/uge/exceptions/command_failed.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/exceptions/ar_exception.py` & `uge-pycl-8.8.0/uge/exceptions/ar_exception.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/exceptions/invalid_argument.py` & `uge-pycl-8.8.0/uge/exceptions/invalid_argument.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/exceptions/configuration_error.py` & `uge-pycl-8.8.0/uge/exceptions/configuration_error.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/exceptions/authorization_error.py` & `uge-pycl-8.8.0/uge/exceptions/authorization_error.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/exceptions/invalid_request.py` & `uge-pycl-8.8.0/uge/exceptions/invalid_request.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/exceptions/qconf_exception.py` & `uge-pycl-8.8.0/uge/exceptions/qconf_exception.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/exceptions/__init__.py` & `uge-pycl-8.8.0/uge/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/exceptions/object_not_found.py` & `uge-pycl-8.8.0/uge/exceptions/object_not_found.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/utility/uge_subprocess.py` & `uge-pycl-8.8.0/uge/utility/uge_subprocess.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/utility/__init__.py` & `uge-pycl-8.8.0/uge/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/ar_api.py` & `uge-pycl-8.8.0/uge/api/ar_api.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/qconf_api.py` & `uge-pycl-8.8.0/uge/api/qconf_api.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/__init__.py` & `uge-pycl-8.8.0/uge/api/__init__.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/share_tree_manager.py` & `uge-pycl-8.8.0/uge/api/impl/share_tree_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/operator_manager.py` & `uge-pycl-8.8.0/uge/api/impl/operator_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/job_class_manager.py` & `uge-pycl-8.8.0/uge/api/impl/job_class_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/calendar_manager.py` & `uge-pycl-8.8.0/uge/api/impl/calendar_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/admin_host_manager.py` & `uge-pycl-8.8.0/uge/api/impl/admin_host_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/ar_manager.py` & `uge-pycl-8.8.0/uge/api/impl/ar_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/submit_host_manager.py` & `uge-pycl-8.8.0/uge/api/impl/submit_host_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/list_based_object_manager.py` & `uge-pycl-8.8.0/uge/api/impl/list_based_object_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/complex_configuration_manager.py` & `uge-pycl-8.8.0/uge/api/impl/complex_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/qrdel_executor.py` & `uge-pycl-8.8.0/uge/api/impl/qrdel_executor.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/user_manager.py` & `uge-pycl-8.8.0/uge/api/impl/user_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/dict_list_based_object_manager.py` & `uge-pycl-8.8.0/uge/api/impl/dict_list_based_object_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/cluster_queue_manager.py` & `uge-pycl-8.8.0/uge/api/impl/cluster_queue_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/execution_host_manager.py` & `uge-pycl-8.8.0/uge/api/impl/execution_host_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/access_list_manager.py` & `uge-pycl-8.8.0/uge/api/impl/access_list_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/manager_manager.py` & `uge-pycl-8.8.0/uge/api/impl/manager_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/qconf_executor.py` & `uge-pycl-8.8.0/uge/api/impl/qconf_executor.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/dict_based_object_manager.py` & `uge-pycl-8.8.0/uge/api/impl/dict_based_object_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/host_group_manager.py` & `uge-pycl-8.8.0/uge/api/impl/host_group_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/resource_quota_set_manager.py` & `uge-pycl-8.8.0/uge/api/impl/resource_quota_set_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/qrstat_executor.py` & `uge-pycl-8.8.0/uge/api/impl/qrstat_executor.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/scheduler_configuration_manager.py` & `uge-pycl-8.8.0/uge/api/impl/scheduler_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/__init__.py` & `uge-pycl-8.8.0/uge/api/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/parallel_environment_manager.py` & `uge-pycl-8.8.0/uge/api/impl/parallel_environment_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/checkpointing_environment_manager.py` & `uge-pycl-8.8.0/uge/api/impl/checkpointing_environment_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/project_manager.py` & `uge-pycl-8.8.0/uge/api/impl/project_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/cluster_configuration_manager.py` & `uge-pycl-8.8.0/uge/api/impl/cluster_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/api/impl/qrsub_executor.py` & `uge-pycl-8.8.0/uge/api/impl/qrsub_executor.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/constants/uge_status.py` & `uge-pycl-8.8.0/uge/constants/uge_status.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/constants/__init__.py` & `uge-pycl-8.8.0/uge/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/log/logger_factory.py` & `uge-pycl-8.8.0/uge/log/logger_factory.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/log/trace_log_record.py` & `uge-pycl-8.8.0/uge/log/trace_log_record.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/log/log_manager.py` & `uge-pycl-8.8.0/uge/log/log_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/log/trace_logger.py` & `uge-pycl-8.8.0/uge/log/trace_logger.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/log/__init__.py` & `uge-pycl-8.8.0/uge/log/__init__.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/log/stream_log_handler.py` & `uge-pycl-8.8.0/uge/log/stream_log_handler.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/log/timed_rotating_file_log_handler.py` & `uge-pycl-8.8.0/uge/log/timed_rotating_file_log_handler.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/cli/qconf_convert.py` & `uge-pycl-8.8.0/uge/cli/qconf_convert.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/cli/qconf_cli.py` & `uge-pycl-8.8.0/uge/cli/qconf_cli.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/cli/__init__.py` & `uge-pycl-8.8.0/uge/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/user_v1_0.py` & `uge-pycl-8.8.0/uge/objects/user_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/qconf_dict_list.py` & `uge-pycl-8.8.0/uge/objects/qconf_dict_list.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/complex_configuration_v3_0.py` & `uge-pycl-8.8.0/uge/objects/complex_configuration_v3_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/resource_quota_set_v1_0.py` & `uge-pycl-8.8.0/uge/objects/resource_quota_set_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/ar_object_factory.py` & `uge-pycl-8.8.0/uge/objects/ar_object_factory.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/cluster_configuration_v2_0.py` & `uge-pycl-8.8.0/uge/objects/cluster_configuration_v2_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/qconf_name_list.py` & `uge-pycl-8.8.0/uge/objects/qconf_name_list.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/share_tree_v1_0.py` & `uge-pycl-8.8.0/uge/objects/share_tree_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/checkpointing_environment_v1_0.py` & `uge-pycl-8.8.0/uge/objects/checkpointing_environment_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/advance_reservation_v1_0.py` & `uge-pycl-8.8.0/uge/objects/advance_reservation_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/execution_host_v1_0.py` & `uge-pycl-8.8.0/uge/objects/execution_host_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/host_group_v1_0.py` & `uge-pycl-8.8.0/uge/objects/host_group_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/parallel_environment_v1_0.py` & `uge-pycl-8.8.0/uge/objects/parallel_environment_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/calendar_v1_0.py` & `uge-pycl-8.8.0/uge/objects/calendar_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/scheduler_configuration_v3_0.py` & `uge-pycl-8.8.0/uge/objects/scheduler_configuration_v3_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/job_class_v1_0.py` & `uge-pycl-8.8.0/uge/objects/job_class_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/complex_configuration_v2_0.py` & `uge-pycl-8.8.0/uge/objects/complex_configuration_v2_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/access_list_v1_0.py` & `uge-pycl-8.8.0/uge/objects/access_list_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/job_class_v3_0.py` & `uge-pycl-8.8.0/uge/objects/job_class_v3_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/job_class_v2_0.py` & `uge-pycl-8.8.0/uge/objects/job_class_v2_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/qconf_object_factory.py` & `uge-pycl-8.8.0/uge/objects/qconf_object_factory.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/uge_release_object_map.py` & `uge-pycl-8.8.0/uge/objects/uge_release_object_map.py`

 * *Files 12% similar despite different names*

```diff
@@ -164,14 +164,23 @@
 UGE_RELEASE_OBJECT_MAP['8.7.0'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.0beta9'])
 
 # 8.7.1
 UGE_RELEASE_OBJECT_MAP['8.7.1prealpha'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.0'])
 UGE_RELEASE_OBJECT_MAP['8.7.1'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.1prealpha'])
 
 # 8.7.2
-UGE_RELEASE_OBJECT_MAP['8.7.2prealpha3'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.0'])
+UGE_RELEASE_OBJECT_MAP['8.7.2prealpha'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.1'])
+UGE_RELEASE_OBJECT_MAP['8.7.2prealpha2'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.1'])
+UGE_RELEASE_OBJECT_MAP['8.7.2prealpha3'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.1'])
 # if new version string shall be used (see uge/api/impl/*executor.py#get_uge_version)
 # UGE_RELEASE_OBJECT_MAP['2022.1.0pre3'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.0'])
 
-UGE_RELEASE_OBJECT_MAP['8.7.2beta'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.0'])
-UGE_RELEASE_OBJECT_MAP['8.7.2'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.0'])
+UGE_RELEASE_OBJECT_MAP['8.7.2beta'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.1'])
+UGE_RELEASE_OBJECT_MAP['8.7.2'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.1'])
 
+# 8.7.3
+UGE_RELEASE_OBJECT_MAP['8.7.3prealpha'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.2'])
+
+# 8.8.0
+UGE_RELEASE_OBJECT_MAP['8.8.0prealpha'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.0'])
+UGE_RELEASE_OBJECT_MAP['8.8.0prealpha2'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.0'])
+UGE_RELEASE_OBJECT_MAP['8.8.0'] = copy.copy(UGE_RELEASE_OBJECT_MAP['8.7.0'])
```

### Comparing `uge-pycl-8.7.2/uge/objects/scheduler_configuration_v2_0.py` & `uge-pycl-8.8.0/uge/objects/scheduler_configuration_v2_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/cluster_configuration_v1_0.py` & `uge-pycl-8.8.0/uge/objects/cluster_configuration_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/complex_configuration_base.py` & `uge-pycl-8.8.0/uge/objects/complex_configuration_base.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/parallel_environment_v2_0.py` & `uge-pycl-8.8.0/uge/objects/parallel_environment_v2_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/cluster_queue_v1_0.py` & `uge-pycl-8.8.0/uge/objects/cluster_queue_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/qconf_object.py` & `uge-pycl-8.8.0/uge/objects/qconf_object.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/complex_configuration_v4_0.py` & `uge-pycl-8.8.0/uge/objects/complex_configuration_v4_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/__init__.py` & `uge-pycl-8.8.0/uge/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/complex_configuration_v1_0.py` & `uge-pycl-8.8.0/uge/objects/complex_configuration_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/cluster_queue_v2_0.py` & `uge-pycl-8.8.0/uge/objects/cluster_queue_v2_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/scheduler_configuration_v1_0.py` & `uge-pycl-8.8.0/uge/objects/scheduler_configuration_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/job_class_v4_0.py` & `uge-pycl-8.8.0/uge/objects/job_class_v4_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/objects/project_v1_0.py` & `uge-pycl-8.8.0/uge/objects/project_v1_0.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/__init__.py` & `uge-pycl-8.8.0/uge/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__ 
 # 
-__version__ = '8.7.2'
+__version__ = '8.8.0'
```

### Comparing `uge-pycl-8.7.2/uge/config/config_manager.py` & `uge-pycl-8.8.0/uge/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge/config/__init__.py` & `uge-pycl-8.8.0/uge/config/__init__.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge_pycl.egg-info/SOURCES.txt` & `uge-pycl-8.8.0/uge_pycl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/uge_pycl.egg-info/PKG-INFO` & `uge-pycl-8.8.0/uge_pycl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: uge-pycl
-Version: 8.7.2
+Version: 8.8.0
 Summary: UGE Python Configuration Library
 Home-page: https://www.altair.com
 Author: Altair Engineering Inc.
 Author-email: support@altair.com
 License: Apache 2.0
 Description: (c) Copyright 2016-2022 Altair Engineering Inc.
             Licensed under the Apache License, Version 2.0 (the "License"); you may not
```

### Comparing `uge-pycl-8.7.2/PKG-INFO` & `uge-pycl-8.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: uge-pycl
-Version: 8.7.2
+Version: 8.8.0
 Summary: UGE Python Configuration Library
 Home-page: https://www.altair.com
 Author: Altair Engineering Inc.
 Author-email: support@altair.com
 License: Apache 2.0
 Description: (c) Copyright 2016-2022 Altair Engineering Inc.
             Licensed under the Apache License, Version 2.0 (the "License"); you may not
```

### Comparing `uge-pycl-8.7.2/test/test_ar.py` & `uge-pycl-8.8.0/test/test_ar.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_job_class.py` & `uge-pycl-8.8.0/test/test_job_class.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_user.py` & `uge-pycl-8.8.0/test/test_user.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_project.py` & `uge-pycl-8.8.0/test/test_project.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_access_list.py` & `uge-pycl-8.8.0/test/test_access_list.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_share_tree.py` & `uge-pycl-8.8.0/test/test_share_tree.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_admin_host.py` & `uge-pycl-8.8.0/test/test_admin_host.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_parallel_environment.py` & `uge-pycl-8.8.0/test/test_parallel_environment.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_cluster_queue.py` & `uge-pycl-8.8.0/test/test_cluster_queue.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_operator.py` & `uge-pycl-8.8.0/test/test_operator.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_checkpointing_environment.py` & `uge-pycl-8.8.0/test/test_checkpointing_environment.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_cluster_configuration.py` & `uge-pycl-8.8.0/test/test_cluster_configuration.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_submit_host.py` & `uge-pycl-8.8.0/test/test_submit_host.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_complex_configuration.py` & `uge-pycl-8.8.0/test/test_complex_configuration.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_resource_quota_set.py` & `uge-pycl-8.8.0/test/test_resource_quota_set.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_manager.py` & `uge-pycl-8.8.0/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_scheduler_configuration.py` & `uge-pycl-8.8.0/test/test_scheduler_configuration.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_host_group.py` & `uge-pycl-8.8.0/test/test_host_group.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_calendar.py` & `uge-pycl-8.8.0/test/test_calendar.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/test_execution_host.py` & `uge-pycl-8.8.0/test/test_execution_host.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/test/utils.py` & `uge-pycl-8.8.0/test/utils.py`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/README.rst` & `uge-pycl-8.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `uge-pycl-8.7.2/setup.py` & `uge-pycl-8.8.0/setup.py`

 * *Files identical despite different names*

