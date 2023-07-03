# Comparing `tmp/prompton-0.0.8.tar.gz` & `tmp/prompton-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompton-0.0.8.tar", max compression
+gzip compressed data, was "prompton-0.0.9.tar", max compression
```

## Comparing `prompton-0.0.8.tar` & `prompton-0.0.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      100 2023-06-12 11:15:10.410454 prompton-0.0.8/README.md
--rw-r--r--   0        0        0     2604 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/__init__.py
--rw-r--r--   0        0        0     2572 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/client.py
--rw-r--r--   0        0        0      348 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      426 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/errors/bad_request_error.py
--rw-r--r--   0        0        0      246 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/errors/conflict_error.py
--rw-r--r--   0        0        0      246 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/errors/not_found_error.py
--rw-r--r--   0        0        0      250 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/errors/unauthorized_error.py
--rw-r--r--   0        0        0      257 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0      292 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/authentication/__init__.py
--rw-r--r--   0        0        0     6099 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/authentication/client.py
--rw-r--r--   0        0        0       65 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/feedbacks/__init__.py
--rw-r--r--   0        0        0    11981 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/feedbacks/client.py
--rw-r--r--   0        0        0       65 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/inferences/__init__.py
--rw-r--r--   0        0        0     9839 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/inferences/client.py
--rw-r--r--   0        0        0       65 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/orgs/__init__.py
--rw-r--r--   0        0        0    15505 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/orgs/client.py
--rw-r--r--   0        0        0       65 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/prompt_versions/__init__.py
--rw-r--r--   0        0        0    16783 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/prompt_versions/client.py
--rw-r--r--   0        0        0       65 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/prompts/__init__.py
--rw-r--r--   0        0        0    15927 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/server_status/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/server_status/client.py
--rw-r--r--   0        0        0       65 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/users/__init__.py
--rw-r--r--   0        0        0    13599 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/resources/users/client.py
--rw-r--r--   0        0        0     3263 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/__init__.py
--rw-r--r--   0        0        0      900 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/api_status_response.py
--rw-r--r--   0        0        0      936 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/body_get_access_token_extended_token_post.py
--rw-r--r--   0        0        0     1274 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/chat_gpt_chat_completition_config.py
--rw-r--r--   0        0        0      152 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/chat_gpt_chat_completition_config_stop.py
--rw-r--r--   0        0        0     1458 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/chat_gpt_chat_completition_request.py
--rw-r--r--   0        0        0      153 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/chat_gpt_chat_completition_request_stop.py
--rw-r--r--   0        0        0     1012 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/chat_gpt_chat_completition_response.py
--rw-r--r--   0        0        0      856 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/chat_gpt_completition_choice.py
--rw-r--r--   0        0        0      843 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/chat_gpt_message.py
--rw-r--r--   0        0        0      666 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/chat_gpt_role.py
--rw-r--r--   0        0        0      809 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/chat_gpt_token_usage.py
--rw-r--r--   0        0        0      773 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/db_status.py
--rw-r--r--   0        0        0      909 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/default_post_response.py
--rw-r--r--   0        0        0     2068 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/feedback_read.py
--rw-r--r--   0        0        0      843 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/http_validation_error.py
--rw-r--r--   0        0        0     2205 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/inference_create_by_prompt_id.py
--rw-r--r--   0        0        0     1805 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/inference_create_by_prompt_version_id.py
--rw-r--r--   0        0        0      813 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/inference_error.py
--rw-r--r--   0        0        0      926 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/inference_post_response.py
--rw-r--r--   0        0        0      293 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/inference_post_response_response.py
--rw-r--r--   0        0        0     2510 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/inference_read.py
--rw-r--r--   0        0        0      285 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/inference_read_response.py
--rw-r--r--   0        0        0      965 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/inference_request_data.py
--rw-r--r--   0        0        0     1229 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/inference_response_data.py
--rw-r--r--   0        0        0     1082 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/inference_response_error.py
--rw-r--r--   0        0        0     1049 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/inference_response_status.py
--rw-r--r--   0        0        0      330 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/new_inference_request.py
--rw-r--r--   0        0        0     1136 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/org_read.py
--rw-r--r--   0        0        0     1275 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/prompt_read.py
--rw-r--r--   0        0        0      507 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/prompt_status.py
--rw-r--r--   0        0        0      152 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/prompt_version_providers.py
--rw-r--r--   0        0        0     1810 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/prompt_version_read.py
--rw-r--r--   0        0        0      837 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/prompt_version_status.py
--rw-r--r--   0        0        0      767 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/token.py
--rw-r--r--   0        0        0     1327 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/user_read.py
--rw-r--r--   0        0        0      686 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/user_roles.py
--rw-r--r--   0        0        0      869 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-06-30 10:53:18.000000 prompton-0.0.8/prompton/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      450 2023-06-30 11:45:53.239085 prompton-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 prompton-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      100 2023-06-12 11:15:10.410454 prompton-0.0.9/README.md
+-rw-r--r--   0        0        0     2604 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/__init__.py
+-rw-r--r--   0        0        0     2572 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/client.py
+-rw-r--r--   0        0        0      348 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      426 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/errors/bad_request_error.py
+-rw-r--r--   0        0        0      246 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/errors/conflict_error.py
+-rw-r--r--   0        0        0      246 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/errors/not_found_error.py
+-rw-r--r--   0        0        0      250 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      257 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0      292 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/authentication/__init__.py
+-rw-r--r--   0        0        0     6099 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/authentication/client.py
+-rw-r--r--   0        0        0       65 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/feedbacks/__init__.py
+-rw-r--r--   0        0        0    11981 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/feedbacks/client.py
+-rw-r--r--   0        0        0       65 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/inferences/__init__.py
+-rw-r--r--   0        0        0     9839 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/inferences/client.py
+-rw-r--r--   0        0        0       65 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/orgs/__init__.py
+-rw-r--r--   0        0        0    15505 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/orgs/client.py
+-rw-r--r--   0        0        0       65 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/prompt_versions/__init__.py
+-rw-r--r--   0        0        0    16783 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/prompt_versions/client.py
+-rw-r--r--   0        0        0       65 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    15927 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/server_status/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/server_status/client.py
+-rw-r--r--   0        0        0       65 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/users/__init__.py
+-rw-r--r--   0        0        0    13599 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/resources/users/client.py
+-rw-r--r--   0        0        0     3263 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/__init__.py
+-rw-r--r--   0        0        0      900 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/api_status_response.py
+-rw-r--r--   0        0        0      936 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/body_get_access_token_extended_token_post.py
+-rw-r--r--   0        0        0     1274 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/chat_gpt_chat_completition_config.py
+-rw-r--r--   0        0        0      152 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/chat_gpt_chat_completition_config_stop.py
+-rw-r--r--   0        0        0     1458 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/chat_gpt_chat_completition_request.py
+-rw-r--r--   0        0        0      153 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/chat_gpt_chat_completition_request_stop.py
+-rw-r--r--   0        0        0     1012 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/chat_gpt_chat_completition_response.py
+-rw-r--r--   0        0        0      856 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/chat_gpt_completition_choice.py
+-rw-r--r--   0        0        0      843 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/chat_gpt_message.py
+-rw-r--r--   0        0        0      666 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/chat_gpt_role.py
+-rw-r--r--   0        0        0      809 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/chat_gpt_token_usage.py
+-rw-r--r--   0        0        0      773 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/db_status.py
+-rw-r--r--   0        0        0      909 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/default_post_response.py
+-rw-r--r--   0        0        0     2068 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/feedback_read.py
+-rw-r--r--   0        0        0      843 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/http_validation_error.py
+-rw-r--r--   0        0        0     2205 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/inference_create_by_prompt_id.py
+-rw-r--r--   0        0        0     1805 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/inference_create_by_prompt_version_id.py
+-rw-r--r--   0        0        0      813 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/inference_error.py
+-rw-r--r--   0        0        0      926 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/inference_post_response.py
+-rw-r--r--   0        0        0      293 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/inference_post_response_response.py
+-rw-r--r--   0        0        0     2510 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/inference_read.py
+-rw-r--r--   0        0        0      285 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/inference_read_response.py
+-rw-r--r--   0        0        0      965 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/inference_request_data.py
+-rw-r--r--   0        0        0     1229 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/inference_response_data.py
+-rw-r--r--   0        0        0     1082 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/inference_response_error.py
+-rw-r--r--   0        0        0     1049 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/inference_response_status.py
+-rw-r--r--   0        0        0      330 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/new_inference_request.py
+-rw-r--r--   0        0        0     1136 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/org_read.py
+-rw-r--r--   0        0        0     1275 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/prompt_read.py
+-rw-r--r--   0        0        0      507 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/prompt_status.py
+-rw-r--r--   0        0        0      152 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/prompt_version_providers.py
+-rw-r--r--   0        0        0     1810 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/prompt_version_read.py
+-rw-r--r--   0        0        0      837 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/prompt_version_status.py
+-rw-r--r--   0        0        0      767 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/token.py
+-rw-r--r--   0        0        0     1327 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/user_read.py
+-rw-r--r--   0        0        0      849 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/user_roles.py
+-rw-r--r--   0        0        0      869 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-06-30 11:31:38.000000 prompton-0.0.9/prompton/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      450 2023-06-30 12:29:08.021042 prompton-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 prompton-0.0.9/PKG-INFO
```

### Comparing `prompton-0.0.8/prompton/__init__.py` & `prompton-0.0.9/prompton/__init__.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/client.py` & `prompton-0.0.9/prompton/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/core/datetime_utils.py` & `prompton-0.0.9/prompton/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/core/jsonable_encoder.py` & `prompton-0.0.9/prompton/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/resources/authentication/client.py` & `prompton-0.0.9/prompton/resources/authentication/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/resources/feedbacks/client.py` & `prompton-0.0.9/prompton/resources/feedbacks/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/resources/inferences/client.py` & `prompton-0.0.9/prompton/resources/inferences/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/resources/orgs/client.py` & `prompton-0.0.9/prompton/resources/orgs/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/resources/prompt_versions/client.py` & `prompton-0.0.9/prompton/resources/prompt_versions/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/resources/prompts/client.py` & `prompton-0.0.9/prompton/resources/prompts/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/resources/server_status/client.py` & `prompton-0.0.9/prompton/resources/server_status/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/resources/users/client.py` & `prompton-0.0.9/prompton/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/__init__.py` & `prompton-0.0.9/prompton/types/__init__.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/api_status_response.py` & `prompton-0.0.9/prompton/types/api_status_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/body_get_access_token_extended_token_post.py` & `prompton-0.0.9/prompton/types/body_get_access_token_extended_token_post.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/chat_gpt_chat_completition_config.py` & `prompton-0.0.9/prompton/types/chat_gpt_chat_completition_config.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/chat_gpt_chat_completition_request.py` & `prompton-0.0.9/prompton/types/chat_gpt_chat_completition_request.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/chat_gpt_chat_completition_response.py` & `prompton-0.0.9/prompton/types/chat_gpt_chat_completition_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/chat_gpt_completition_choice.py` & `prompton-0.0.9/prompton/types/chat_gpt_completition_choice.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/chat_gpt_message.py` & `prompton-0.0.9/prompton/types/chat_gpt_message.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/chat_gpt_role.py` & `prompton-0.0.9/prompton/types/chat_gpt_role.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/chat_gpt_token_usage.py` & `prompton-0.0.9/prompton/types/chat_gpt_token_usage.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/db_status.py` & `prompton-0.0.9/prompton/types/db_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/default_post_response.py` & `prompton-0.0.9/prompton/types/default_post_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/feedback_read.py` & `prompton-0.0.9/prompton/types/feedback_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/http_validation_error.py` & `prompton-0.0.9/prompton/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/inference_create_by_prompt_id.py` & `prompton-0.0.9/prompton/types/inference_create_by_prompt_id.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/inference_create_by_prompt_version_id.py` & `prompton-0.0.9/prompton/types/inference_create_by_prompt_version_id.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/inference_error.py` & `prompton-0.0.9/prompton/types/inference_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/inference_post_response.py` & `prompton-0.0.9/prompton/types/inference_post_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/inference_read.py` & `prompton-0.0.9/prompton/types/inference_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/inference_request_data.py` & `prompton-0.0.9/prompton/types/inference_request_data.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/inference_response_data.py` & `prompton-0.0.9/prompton/types/inference_response_data.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/inference_response_error.py` & `prompton-0.0.9/prompton/types/inference_response_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/inference_response_status.py` & `prompton-0.0.9/prompton/types/inference_response_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/org_read.py` & `prompton-0.0.9/prompton/types/org_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/prompt_read.py` & `prompton-0.0.9/prompton/types/prompt_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/prompt_version_read.py` & `prompton-0.0.9/prompton/types/prompt_version_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/prompt_version_status.py` & `prompton-0.0.9/prompton/types/prompt_version_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/token.py` & `prompton-0.0.9/prompton/types/token.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/user_read.py` & `prompton-0.0.9/prompton/types/user_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/prompton/types/validation_error.py` & `prompton-0.0.9/prompton/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.8/PKG-INFO` & `prompton-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompton
-Version: 0.0.8
+Version: 0.0.9
 Summary: Chat prompt template evaluation and inference monitoring
 Author: PromptOn
 Author-email: hello@prompton.ai
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

