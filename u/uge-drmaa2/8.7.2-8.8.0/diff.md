# Comparing `tmp/uge-drmaa2-8.7.2.tar.gz` & `tmp/uge-drmaa2-8.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uge-drmaa2-8.7.2.tar", last modified: Tue Aug 23 16:13:32 2022, max compression
+gzip compressed data, was "dist/uge-drmaa2-8.8.0.tar", last modified: Mon Jul  3 09:49:28 2023, max compression
```

## Comparing `uge-drmaa2-8.7.2.tar` & `uge-drmaa2-8.8.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:13:32.000000 uge-drmaa2-8.7.2/
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:13:32.000000 uge-drmaa2-8.7.2/drmaa2/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5786 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/reservation.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4343 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/exception_mapper.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    15156 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/drmaa2_object_descriptors.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4856 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/notification.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1633 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/drmaa2_slot_info_list_descriptor.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3695 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/reservation_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4595 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/reservation_template.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2817 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/log_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    22185 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/job_session.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5392 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/machine_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2857 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/sudo.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1607 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/drmaa2_job_list_descriptor.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6222 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/drmaa2_exceptions.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4714 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/version.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5360 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/job_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     8676 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/job_array.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1741 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/singleton.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     9766 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/drmaa2_object.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1622 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/byte_string.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    26134 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/library_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3549 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/queue_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     9581 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/drmaa2_ctypes.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7394 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/job_template.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3660 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/slot_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    14749 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/job.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2298 2022-08-12 11:28:14.000000 uge-drmaa2-8.7.2/drmaa2/__init__.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3742 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/drmaa2_constants.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    12375 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/reservation_session.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     9119 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/monitoring_session.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1630 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/drmaa2/drmaa2_version_descriptor.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3607 2022-08-23 16:13:32.000000 uge-drmaa2-8.7.2/PKG-INFO
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:13:32.000000 uge-drmaa2-8.7.2/test/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1293 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_machine_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3267 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_job_array.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1770 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_reservation.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5120 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_job.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1858 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_failed.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1646 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_library_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4657 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_reservation_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    10970 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_job_template.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6688 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_job_session.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3988 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_reservation_session.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6813 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_job_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3109 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_monitoring_session.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1288 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_notification.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6023 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_reservation_template.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1268 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_queue_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2261 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_sudo.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1817 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_version.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2221 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/test/test_drmaa2_init.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2415 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/README.rst
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2022-08-23 16:13:32.000000 uge-drmaa2-8.7.2/uge_drmaa2.egg-info/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)        1 2022-08-23 16:13:31.000000 uge-drmaa2-8.7.2/uge_drmaa2.egg-info/dependency_links.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1369 2022-08-23 16:13:31.000000 uge-drmaa2-8.7.2/uge_drmaa2.egg-info/SOURCES.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3607 2022-08-23 16:13:31.000000 uge-drmaa2-8.7.2/uge_drmaa2.egg-info/PKG-INFO
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)        7 2022-08-23 16:13:31.000000 uge-drmaa2-8.7.2/uge_drmaa2.egg-info/top_level.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      240 2022-08-23 16:13:32.000000 uge-drmaa2-8.7.2/setup.cfg
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2156 2022-08-11 15:04:14.000000 uge-drmaa2-8.7.2/setup.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:49:28.000000 uge-drmaa2-8.8.0/
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:49:28.000000 uge-drmaa2-8.8.0/drmaa2/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5786 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/reservation.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4343 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/exception_mapper.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    15156 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/drmaa2_object_descriptors.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4856 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/notification.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1633 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/drmaa2_slot_info_list_descriptor.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3695 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/reservation_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4595 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/reservation_template.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2817 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/log_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    22185 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/job_session.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5392 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/machine_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2857 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/sudo.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1607 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/drmaa2_job_list_descriptor.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6222 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/drmaa2_exceptions.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4714 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/version.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5360 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/job_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     8676 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/job_array.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1741 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/singleton.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     9766 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/drmaa2_object.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1622 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/byte_string.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    26134 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/library_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3549 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/queue_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     9581 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/drmaa2_ctypes.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7394 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/job_template.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3660 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/slot_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    14749 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/job.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2298 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/__init__.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3742 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/drmaa2_constants.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    12375 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/reservation_session.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     9119 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/monitoring_session.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1630 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/drmaa2/drmaa2_version_descriptor.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3607 2023-07-03 09:49:28.000000 uge-drmaa2-8.8.0/PKG-INFO
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:49:28.000000 uge-drmaa2-8.8.0/test/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1293 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_machine_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3267 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_job_array.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1770 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_reservation.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5120 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_job.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1858 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_failed.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1646 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_library_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4657 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_reservation_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    10970 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_job_template.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6688 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_job_session.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3988 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_reservation_session.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6813 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_job_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3109 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_monitoring_session.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1288 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_notification.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6023 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_reservation_template.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1268 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_queue_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2261 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_sudo.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1817 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_version.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2221 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/test/test_drmaa2_init.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2415 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/README.rst
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-07-03 09:49:28.000000 uge-drmaa2-8.8.0/uge_drmaa2.egg-info/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)        1 2023-07-03 09:49:28.000000 uge-drmaa2-8.8.0/uge_drmaa2.egg-info/dependency_links.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1369 2023-07-03 09:49:28.000000 uge-drmaa2-8.8.0/uge_drmaa2.egg-info/SOURCES.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3607 2023-07-03 09:49:28.000000 uge-drmaa2-8.8.0/uge_drmaa2.egg-info/PKG-INFO
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)        7 2023-07-03 09:49:28.000000 uge-drmaa2-8.8.0/uge_drmaa2.egg-info/top_level.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      240 2023-07-03 09:49:28.000000 uge-drmaa2-8.8.0/setup.cfg
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2156 2023-06-28 12:36:01.000000 uge-drmaa2-8.8.0/setup.py
```

### Comparing `uge-drmaa2-8.7.2/drmaa2/reservation.py` & `uge-drmaa2-8.8.0/drmaa2/reservation.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/exception_mapper.py` & `uge-drmaa2-8.8.0/drmaa2/exception_mapper.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/drmaa2_object_descriptors.py` & `uge-drmaa2-8.8.0/drmaa2/drmaa2_object_descriptors.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/notification.py` & `uge-drmaa2-8.8.0/drmaa2/notification.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/drmaa2_slot_info_list_descriptor.py` & `uge-drmaa2-8.8.0/drmaa2/drmaa2_slot_info_list_descriptor.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/reservation_info.py` & `uge-drmaa2-8.8.0/drmaa2/reservation_info.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/reservation_template.py` & `uge-drmaa2-8.8.0/drmaa2/reservation_template.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/log_manager.py` & `uge-drmaa2-8.8.0/drmaa2/log_manager.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/job_session.py` & `uge-drmaa2-8.8.0/drmaa2/job_session.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/machine_info.py` & `uge-drmaa2-8.8.0/drmaa2/machine_info.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/sudo.py` & `uge-drmaa2-8.8.0/drmaa2/sudo.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/drmaa2_job_list_descriptor.py` & `uge-drmaa2-8.8.0/drmaa2/drmaa2_job_list_descriptor.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/drmaa2_exceptions.py` & `uge-drmaa2-8.8.0/drmaa2/drmaa2_exceptions.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/version.py` & `uge-drmaa2-8.8.0/drmaa2/version.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/job_info.py` & `uge-drmaa2-8.8.0/drmaa2/job_info.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/job_array.py` & `uge-drmaa2-8.8.0/drmaa2/job_array.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/singleton.py` & `uge-drmaa2-8.8.0/drmaa2/singleton.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/drmaa2_object.py` & `uge-drmaa2-8.8.0/drmaa2/drmaa2_object.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/byte_string.py` & `uge-drmaa2-8.8.0/drmaa2/byte_string.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/library_manager.py` & `uge-drmaa2-8.8.0/drmaa2/library_manager.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/queue_info.py` & `uge-drmaa2-8.8.0/drmaa2/queue_info.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/drmaa2_ctypes.py` & `uge-drmaa2-8.8.0/drmaa2/drmaa2_ctypes.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/job_template.py` & `uge-drmaa2-8.8.0/drmaa2/job_template.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/slot_info.py` & `uge-drmaa2-8.8.0/drmaa2/slot_info.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/job.py` & `uge-drmaa2-8.8.0/drmaa2/job.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/__init__.py` & `uge-drmaa2-8.8.0/drmaa2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,8 +46,8 @@
 get_drmaa_name = LibraryManager.get_drmaa_name
 drmaa_supports = LibraryManager.drmaa_supports 
 get_drms_version = Version.get_drms_version
 get_drmaa_version = Version.get_drmaa_version
 get_job_session_names = JobSession.list_session_names 
 get_reservation_session_names = ReservationSession.list_session_names 
  
-__version__ = '8.7.2'
+__version__ = '8.8.0'
```

### Comparing `uge-drmaa2-8.7.2/drmaa2/drmaa2_constants.py` & `uge-drmaa2-8.8.0/drmaa2/drmaa2_constants.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/reservation_session.py` & `uge-drmaa2-8.8.0/drmaa2/reservation_session.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/monitoring_session.py` & `uge-drmaa2-8.8.0/drmaa2/monitoring_session.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/drmaa2/drmaa2_version_descriptor.py` & `uge-drmaa2-8.8.0/drmaa2/drmaa2_version_descriptor.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/PKG-INFO` & `uge-drmaa2-8.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: uge-drmaa2
-Version: 8.7.2
+Version: 8.8.0
 Summary: UGE DRMAA2 Python API
 Home-page: https://www.altair.com
 Author: Altair Engineering Inc.
 Author-email: support@altair.com
 License: Apache 2.0
 Description: (c) Copyright 2008-2022 Altair Engineering Inc.
             Licensed under the Apache License, Version 2.0 (the "License"); you may not
```

### Comparing `uge-drmaa2-8.7.2/test/test_machine_info.py` & `uge-drmaa2-8.8.0/test/test_machine_info.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_job_array.py` & `uge-drmaa2-8.8.0/test/test_job_array.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_reservation.py` & `uge-drmaa2-8.8.0/test/test_reservation.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_job.py` & `uge-drmaa2-8.8.0/test/test_job.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_failed.py` & `uge-drmaa2-8.8.0/test/test_failed.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_library_manager.py` & `uge-drmaa2-8.8.0/test/test_library_manager.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_reservation_info.py` & `uge-drmaa2-8.8.0/test/test_reservation_info.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_job_template.py` & `uge-drmaa2-8.8.0/test/test_job_template.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_job_session.py` & `uge-drmaa2-8.8.0/test/test_job_session.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_reservation_session.py` & `uge-drmaa2-8.8.0/test/test_reservation_session.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_job_info.py` & `uge-drmaa2-8.8.0/test/test_job_info.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_monitoring_session.py` & `uge-drmaa2-8.8.0/test/test_monitoring_session.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_notification.py` & `uge-drmaa2-8.8.0/test/test_notification.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_reservation_template.py` & `uge-drmaa2-8.8.0/test/test_reservation_template.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_queue_info.py` & `uge-drmaa2-8.8.0/test/test_queue_info.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_sudo.py` & `uge-drmaa2-8.8.0/test/test_sudo.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_version.py` & `uge-drmaa2-8.8.0/test/test_version.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/test/test_drmaa2_init.py` & `uge-drmaa2-8.8.0/test/test_drmaa2_init.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/README.rst` & `uge-drmaa2-8.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/uge_drmaa2.egg-info/SOURCES.txt` & `uge-drmaa2-8.8.0/uge_drmaa2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.7.2/uge_drmaa2.egg-info/PKG-INFO` & `uge-drmaa2-8.8.0/uge_drmaa2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: uge-drmaa2
-Version: 8.7.2
+Version: 8.8.0
 Summary: UGE DRMAA2 Python API
 Home-page: https://www.altair.com
 Author: Altair Engineering Inc.
 Author-email: support@altair.com
 License: Apache 2.0
 Description: (c) Copyright 2008-2022 Altair Engineering Inc.
             Licensed under the Apache License, Version 2.0 (the "License"); you may not
```

### Comparing `uge-drmaa2-8.7.2/setup.py` & `uge-drmaa2-8.8.0/setup.py`

 * *Files identical despite different names*

