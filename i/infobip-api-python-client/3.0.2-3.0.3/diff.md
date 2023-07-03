# Comparing `tmp/infobip-api-python-client-3.0.2.tar.gz` & `tmp/infobip-api-python-client-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infobip-api-python-client-3.0.2.tar", last modified: Mon Jul  3 11:36:56 2023, max compression
+gzip compressed data, was "infobip-api-python-client-3.0.3.tar", last modified: Mon Jul  3 15:28:58 2023, max compression
```

## Comparing `infobip-api-python-client-3.0.2.tar` & `infobip-api-python-client-3.0.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:36:56.980473 infobip-api-python-client-3.0.2/
--rw-r--r--   0 root         (0) root         (0)     1114 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8372 2023-07-03 11:36:56.980473 infobip-api-python-client-3.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7582 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:36:56.956473 infobip-api-python-client-3.0.2/infobip_api_client/
--rw-r--r--   0 root         (0) root         (0)      854 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:36:56.958473 infobip-api-python-client-3.0.2/infobip_api_client/api/
--rw-r--r--   0 root         (0) root         (0)      225 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5279 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/api/receive_sms_api.py
--rw-r--r--   0 root         (0) root         (0)    17866 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/api/scheduled_sms_api.py
--rw-r--r--   0 root         (0) root         (0)    24996 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/api/send_sms_api.py
--rw-r--r--   0 root         (0) root         (0)    61944 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/api/tfa_api.py
--rw-r--r--   0 root         (0) root         (0)    36073 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/api_client.py
--rw-r--r--   0 root         (0) root         (0)    18140 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5078 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:36:56.978473 infobip-api-python-client-3.0.2/infobip_api_client/model/
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7862 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_advanced_binary_request.py
--rw-r--r--   0 root         (0) root         (0)     8107 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_advanced_textual_request.py
--rw-r--r--   0 root         (0) root         (0)     6713 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_api_exception.py
--rw-r--r--   0 root         (0) root         (0)     6795 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_api_request_error.py
--rw-r--r--   0 root         (0) root         (0)     6692 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_api_request_error_details.py
--rw-r--r--   0 root         (0) root         (0)     7184 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_binary_content.py
--rw-r--r--   0 root         (0) root         (0)    10671 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_binary_message.py
--rw-r--r--   0 root         (0) root         (0)     6514 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_bulk_request.py
--rw-r--r--   0 root         (0) root         (0)     6626 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_bulk_response.py
--rw-r--r--   0 root         (0) root         (0)     7143 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_bulk_status.py
--rw-r--r--   0 root         (0) root         (0)     6807 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_bulk_status_response.py
--rw-r--r--   0 root         (0) root         (0)     7193 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_delivery_day.py
--rw-r--r--   0 root         (0) root         (0)     6642 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_delivery_result.py
--rw-r--r--   0 root         (0) root         (0)     7050 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_delivery_time.py
--rw-r--r--   0 root         (0) root         (0)     7654 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_delivery_time_window.py
--rw-r--r--   0 root         (0) root         (0)     6770 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_destination.py
--rw-r--r--   0 root         (0) root         (0)     7313 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_error.py
--rw-r--r--   0 root         (0) root         (0)     8423 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_inbound_message.py
--rw-r--r--   0 root         (0) root         (0)     7062 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_inbound_message_result.py
--rw-r--r--   0 root         (0) root         (0)     6899 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_india_dlt_options.py
--rw-r--r--   0 root         (0) root         (0)     6710 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_language.py
--rw-r--r--   0 root         (0) root         (0)     7016 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_language_configuration.py
--rw-r--r--   0 root         (0) root         (0)     8920 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_log.py
--rw-r--r--   0 root         (0) root         (0)     6641 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_logs_response.py
--rw-r--r--   0 root         (0) root         (0)     7538 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_preview.py
--rw-r--r--   0 root         (0) root         (0)     7604 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_preview_request.py
--rw-r--r--   0 root         (0) root         (0)     6918 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_preview_response.py
--rw-r--r--   0 root         (0) root         (0)     6717 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_price.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_regional_options.py
--rw-r--r--   0 root         (0) root         (0)     9155 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_report.py
--rw-r--r--   0 root         (0) root         (0)     7029 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_response.py
--rw-r--r--   0 root         (0) root         (0)     7134 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_response_details.py
--rw-r--r--   0 root         (0) root         (0)     7328 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_sending_speed_limit.py
--rw-r--r--   0 root         (0) root         (0)     6947 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_speed_limit_time_unit.py
--rw-r--r--   0 root         (0) root         (0)     7324 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_status.py
--rw-r--r--   0 root         (0) root         (0)    11167 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_textual_message.py
--rw-r--r--   0 root         (0) root         (0)     7281 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_tracking.py
--rw-r--r--   0 root         (0) root         (0)     6696 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/sms_update_status_request.py
--rw-r--r--   0 root         (0) root         (0)     6713 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_api_exception.py
--rw-r--r--   0 root         (0) root         (0)     6795 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_api_request_error.py
--rw-r--r--   0 root         (0) root         (0)     6692 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_api_request_error_details.py
--rw-r--r--   0 root         (0) root         (0)     9857 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_application_configuration.py
--rw-r--r--   0 root         (0) root         (0)     7201 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_application_request.py
--rw-r--r--   0 root         (0) root         (0)     7372 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_application_response.py
--rw-r--r--   0 root         (0) root         (0)     8992 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_create_message_request.py
--rw-r--r--   0 root         (0) root         (0)     7116 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_india_dlt_options.py
--rw-r--r--   0 root         (0) root         (0)     7523 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_language.py
--rw-r--r--   0 root         (0) root         (0)     9499 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_message.py
--rw-r--r--   0 root         (0) root         (0)     7009 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_pin_type.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_regional_options.py
--rw-r--r--   0 root         (0) root         (0)     6742 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_resend_pin_request.py
--rw-r--r--   0 root         (0) root         (0)     7718 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_start_authentication_request.py
--rw-r--r--   0 root         (0) root         (0)     7635 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_start_authentication_response.py
--rw-r--r--   0 root         (0) root         (0)     8878 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_update_message_request.py
--rw-r--r--   0 root         (0) root         (0)     7236 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_verification.py
--rw-r--r--   0 root         (0) root         (0)     6743 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_verification_response.py
--rw-r--r--   0 root         (0) root         (0)     6506 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_verify_pin_request.py
--rw-r--r--   0 root         (0) root         (0)     7337 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_verify_pin_response.py
--rw-r--r--   0 root         (0) root         (0)    73713 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/model_utils.py
--rw-r--r--   0 root         (0) root         (0)    12850 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/infobip_api_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:36:56.979473 infobip-api-python-client-3.0.2/infobip_api_python_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8372 2023-07-03 11:36:56.000000 infobip-api-python-client-3.0.2/infobip_api_python_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3524 2023-07-03 11:36:56.000000 infobip-api-python-client-3.0.2/infobip_api_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 11:36:56.000000 infobip-api-python-client-3.0.2/infobip_api_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-03 11:36:56.000000 infobip-api-python-client-3.0.2/infobip_api_python_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-03 11:36:56.000000 infobip-api-python-client-3.0.2/infobip_api_python_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-03 11:36:56.981473 infobip-api-python-client-3.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1969 2023-07-03 11:36:14.000000 infobip-api-python-client-3.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:28:58.235883 infobip-api-python-client-3.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8372 2023-07-03 15:28:58.235883 infobip-api-python-client-3.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7582 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:28:58.212884 infobip-api-python-client-3.0.3/infobip_api_client/
+-rw-r--r--   0 root         (0) root         (0)      854 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:28:58.214884 infobip-api-python-client-3.0.3/infobip_api_client/api/
+-rw-r--r--   0 root         (0) root         (0)      225 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5279 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/api/receive_sms_api.py
+-rw-r--r--   0 root         (0) root         (0)    17866 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/api/scheduled_sms_api.py
+-rw-r--r--   0 root         (0) root         (0)    24996 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/api/send_sms_api.py
+-rw-r--r--   0 root         (0) root         (0)    61944 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/api/tfa_api.py
+-rw-r--r--   0 root         (0) root         (0)    36073 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    18140 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5078 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:28:58.233883 infobip-api-python-client-3.0.3/infobip_api_client/model/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7862 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_advanced_binary_request.py
+-rw-r--r--   0 root         (0) root         (0)     8107 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_advanced_textual_request.py
+-rw-r--r--   0 root         (0) root         (0)     6713 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_api_exception.py
+-rw-r--r--   0 root         (0) root         (0)     6795 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_api_request_error.py
+-rw-r--r--   0 root         (0) root         (0)     6692 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_api_request_error_details.py
+-rw-r--r--   0 root         (0) root         (0)     7184 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_binary_content.py
+-rw-r--r--   0 root         (0) root         (0)    10671 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_binary_message.py
+-rw-r--r--   0 root         (0) root         (0)     6514 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_bulk_request.py
+-rw-r--r--   0 root         (0) root         (0)     6626 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_bulk_response.py
+-rw-r--r--   0 root         (0) root         (0)     7143 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_bulk_status.py
+-rw-r--r--   0 root         (0) root         (0)     6807 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_bulk_status_response.py
+-rw-r--r--   0 root         (0) root         (0)     7193 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_delivery_day.py
+-rw-r--r--   0 root         (0) root         (0)     6642 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_delivery_result.py
+-rw-r--r--   0 root         (0) root         (0)     7050 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_delivery_time.py
+-rw-r--r--   0 root         (0) root         (0)     7654 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_delivery_time_window.py
+-rw-r--r--   0 root         (0) root         (0)     6770 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_destination.py
+-rw-r--r--   0 root         (0) root         (0)     7313 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_error.py
+-rw-r--r--   0 root         (0) root         (0)     8423 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_inbound_message.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_inbound_message_result.py
+-rw-r--r--   0 root         (0) root         (0)     6899 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_india_dlt_options.py
+-rw-r--r--   0 root         (0) root         (0)     6710 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_language.py
+-rw-r--r--   0 root         (0) root         (0)     7016 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_language_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     8920 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     6641 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_logs_response.py
+-rw-r--r--   0 root         (0) root         (0)     7538 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_preview.py
+-rw-r--r--   0 root         (0) root         (0)     7604 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_preview_request.py
+-rw-r--r--   0 root         (0) root         (0)     6918 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_preview_response.py
+-rw-r--r--   0 root         (0) root         (0)     6717 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_price.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_regional_options.py
+-rw-r--r--   0 root         (0) root         (0)     9155 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_report.py
+-rw-r--r--   0 root         (0) root         (0)     7029 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_response.py
+-rw-r--r--   0 root         (0) root         (0)     7134 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_response_details.py
+-rw-r--r--   0 root         (0) root         (0)     7328 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_sending_speed_limit.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_speed_limit_time_unit.py
+-rw-r--r--   0 root         (0) root         (0)     7324 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_status.py
+-rw-r--r--   0 root         (0) root         (0)    11167 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_textual_message.py
+-rw-r--r--   0 root         (0) root         (0)     7281 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_tracking.py
+-rw-r--r--   0 root         (0) root         (0)     6696 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/sms_update_status_request.py
+-rw-r--r--   0 root         (0) root         (0)     6713 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_api_exception.py
+-rw-r--r--   0 root         (0) root         (0)     6795 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_api_request_error.py
+-rw-r--r--   0 root         (0) root         (0)     6692 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_api_request_error_details.py
+-rw-r--r--   0 root         (0) root         (0)     9857 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_application_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     7201 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_application_request.py
+-rw-r--r--   0 root         (0) root         (0)     7372 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_application_response.py
+-rw-r--r--   0 root         (0) root         (0)     8992 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_create_message_request.py
+-rw-r--r--   0 root         (0) root         (0)     7116 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_india_dlt_options.py
+-rw-r--r--   0 root         (0) root         (0)     7523 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_language.py
+-rw-r--r--   0 root         (0) root         (0)     9499 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_message.py
+-rw-r--r--   0 root         (0) root         (0)     7009 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_pin_type.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_regional_options.py
+-rw-r--r--   0 root         (0) root         (0)     6742 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_resend_pin_request.py
+-rw-r--r--   0 root         (0) root         (0)     7718 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_start_authentication_request.py
+-rw-r--r--   0 root         (0) root         (0)     7635 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_start_authentication_response.py
+-rw-r--r--   0 root         (0) root         (0)     8878 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_update_message_request.py
+-rw-r--r--   0 root         (0) root         (0)     7236 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_verification.py
+-rw-r--r--   0 root         (0) root         (0)     6743 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_verification_response.py
+-rw-r--r--   0 root         (0) root         (0)     6506 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_verify_pin_request.py
+-rw-r--r--   0 root         (0) root         (0)     7337 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_verify_pin_response.py
+-rw-r--r--   0 root         (0) root         (0)    73713 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/model_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12850 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/infobip_api_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 15:28:58.235883 infobip-api-python-client-3.0.3/infobip_api_python_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8372 2023-07-03 15:28:58.000000 infobip-api-python-client-3.0.3/infobip_api_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-07-03 15:28:58.000000 infobip-api-python-client-3.0.3/infobip_api_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 15:28:58.000000 infobip-api-python-client-3.0.3/infobip_api_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-03 15:28:58.000000 infobip-api-python-client-3.0.3/infobip_api_python_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-03 15:28:58.000000 infobip-api-python-client-3.0.3/infobip_api_python_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-03 15:28:58.237883 infobip-api-python-client-3.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-07-03 15:28:07.000000 infobip-api-python-client-3.0.3/setup.py
```

### Comparing `infobip-api-python-client-3.0.2/LICENSE` & `infobip-api-python-client-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/PKG-INFO` & `infobip-api-python-client-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infobip-api-python-client
-Version: 3.0.2
+Version: 3.0.3
 Summary: Infobip Client API Libraries OpenAPI Specification
 Home-page: https://github.com/infobip/infobip-api-python-client
 Author: Infobip Ltd.
 Author-email: support@infobip.com
 License: MIT
 Keywords: infobip,sms,php,tfa,sdk,rest,api,msisdn,2fa,openapi
 Classifier: Intended Audience :: Telecommunications Industry
```

### Comparing `infobip-api-python-client-3.0.2/README.md` & `infobip-api-python-client-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/__init__.py` & `infobip-api-python-client-3.0.3/infobip_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/api/receive_sms_api.py` & `infobip-api-python-client-3.0.3/infobip_api_client/api/receive_sms_api.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/api/scheduled_sms_api.py` & `infobip-api-python-client-3.0.3/infobip_api_client/api/scheduled_sms_api.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/api/send_sms_api.py` & `infobip-api-python-client-3.0.3/infobip_api_client/api/send_sms_api.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/api/tfa_api.py` & `infobip-api-python-client-3.0.3/infobip_api_client/api/tfa_api.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/api_client.py` & `infobip-api-python-client-3.0.3/infobip_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/configuration.py` & `infobip-api-python-client-3.0.3/infobip_api_client/configuration.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/exceptions.py` & `infobip-api-python-client-3.0.3/infobip_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_advanced_binary_request.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_advanced_binary_request.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_advanced_textual_request.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_advanced_textual_request.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_api_exception.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_api_exception.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_api_request_error.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_api_request_error.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_api_request_error_details.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_api_request_error_details.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_binary_content.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_binary_content.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_binary_message.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_binary_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_bulk_request.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_bulk_request.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_bulk_response.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_bulk_response.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_bulk_status.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_bulk_status.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_bulk_status_response.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_bulk_status_response.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_delivery_day.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_delivery_day.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_delivery_result.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_delivery_result.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_delivery_time.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_delivery_time.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_delivery_time_window.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_delivery_time_window.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_destination.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_destination.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_error.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_error.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_inbound_message.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_inbound_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_inbound_message_result.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_inbound_message_result.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_india_dlt_options.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_india_dlt_options.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_language.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_language.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_language_configuration.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_language_configuration.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_log.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_log.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_logs_response.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_logs_response.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_preview.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_preview.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_preview_request.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_preview_request.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_preview_response.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_preview_response.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_price.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_price.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_regional_options.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_regional_options.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_report.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_report.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_response.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_response.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_response_details.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_response_details.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_sending_speed_limit.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_sending_speed_limit.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_speed_limit_time_unit.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_speed_limit_time_unit.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_status.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_status.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_textual_message.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_textual_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_tracking.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_tracking.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/sms_update_status_request.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/sms_update_status_request.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_api_exception.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_api_exception.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_api_request_error.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_api_request_error.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_api_request_error_details.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_api_request_error_details.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_application_configuration.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_application_configuration.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_application_request.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_application_request.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_application_response.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_application_response.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_create_message_request.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_create_message_request.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_india_dlt_options.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_india_dlt_options.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_language.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_language.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_message.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_pin_type.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_pin_type.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_regional_options.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_regional_options.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_resend_pin_request.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_resend_pin_request.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_start_authentication_request.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_start_authentication_request.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_start_authentication_response.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_start_authentication_response.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_update_message_request.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_update_message_request.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_verification.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_verification.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_verification_response.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_verification_response.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_verify_pin_request.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_verify_pin_request.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model/tfa_verify_pin_response.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model/tfa_verify_pin_response.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/model_utils.py` & `infobip-api-python-client-3.0.3/infobip_api_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_client/rest.py` & `infobip-api-python-client-3.0.3/infobip_api_client/rest.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/infobip_api_python_client.egg-info/PKG-INFO` & `infobip-api-python-client-3.0.3/infobip_api_python_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infobip-api-python-client
-Version: 3.0.2
+Version: 3.0.3
 Summary: Infobip Client API Libraries OpenAPI Specification
 Home-page: https://github.com/infobip/infobip-api-python-client
 Author: Infobip Ltd.
 Author-email: support@infobip.com
 License: MIT
 Keywords: infobip,sms,php,tfa,sdk,rest,api,msisdn,2fa,openapi
 Classifier: Intended Audience :: Telecommunications Industry
```

### Comparing `infobip-api-python-client-3.0.2/infobip_api_python_client.egg-info/SOURCES.txt` & `infobip-api-python-client-3.0.3/infobip_api_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infobip-api-python-client-3.0.2/setup.py` & `infobip-api-python-client-3.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "infobip-api-python-client"
-VERSION = "3.0.2"
+VERSION = "3.0.3"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -51,15 +51,15 @@
         "api",
         "msisdn",
         "2fa",
         "openapi",
     ],
     python_requires=">=3.6",
     install_requires=REQUIRES,
-    packages=find_packages(),
+    packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Intended Audience :: Telecommunications Industry",
         "Intended Audience :: Information Technology",
```

