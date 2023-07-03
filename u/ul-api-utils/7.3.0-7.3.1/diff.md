# Comparing `tmp/ul-api-utils-7.3.0.tar.gz` & `tmp/ul-api-utils-7.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-api-utils-7.3.0.tar", last modified: Wed Jun 28 12:08:17 2023, max compression
+gzip compressed data, was "ul-api-utils-7.3.1.tar", last modified: Mon Jul  3 18:46:26 2023, max compression
```

## Comparing `ul-api-utils-7.3.0.tar` & `ul-api-utils-7.3.1.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.949605 ul-api-utils-7.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2022-02-08 08:28:45.000000 ul-api-utils-7.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13527 2023-06-28 12:08:17.949605 ul-api-utils-7.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12938 2023-04-11 10:27:02.000000 ul-api-utils-7.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.929604 ul-api-utils-7.3.0/example/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-15 22:48:45.000000 ul-api-utils-7.3.0/example/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-06-28 12:08:16.000000 ul-api-utils-7.3.0/example/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/example/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.929604 ul-api-utils-7.3.0/example/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-01 08:27:51.000000 ul-api-utils-7.3.0/example/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/example/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1329 2022-08-15 22:48:45.000000 ul-api-utils-7.3.0/example/pure_flask_example.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-08-15 22:48:45.000000 ul-api-utils-7.3.0/example/rate_limit_load.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.929604 ul-api-utils-7.3.0/example/routes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-08 14:57:28.000000 ul-api-utils-7.3.0/example/routes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11237 2023-06-28 12:08:16.000000 ul-api-utils-7.3.0/example/routes/api_some.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.929604 ul-api-utils-7.3.0/example/workers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-18 20:31:49.000000 ul-api-utils-7.3.0/example/workers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/example/workers/worker.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 12:08:17.949605 ul-api-utils-7.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2548 2023-06-28 12:08:16.000000 ul-api-utils-7.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.929604 ul-api-utils-7.3.0/ul_api_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.933605 ul-api-utils-7.3.0/ul_api_utils/access/
--rw-rw-rw-   0 root         (0) root         (0)     4274 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.933605 ul-api-utils-7.3.0/ul_api_utils/api_resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/api_resource/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3279 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/api_resource/api_request.py
--rw-rw-rw-   0 root         (0) root         (0)    17185 2023-06-28 12:08:16.000000 ul-api-utils-7.3.0/ul_api_utils/api_resource/api_resource.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/api_resource/api_resource_config.py
--rw-rw-rw-   0 root         (0) root         (0)    17241 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/api_resource/api_resource_fn_typing.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/api_resource/api_resource_type.py
--rw-rw-rw-   0 root         (0) root         (0)     9676 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/api_resource/api_response.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/api_resource/api_response_db.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/api_resource/api_response_payload_alias.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-06-28 12:08:16.000000 ul-api-utils-7.3.0/ul_api_utils/api_resource/db_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/api_resource/signature_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.933605 ul-api-utils-7.3.0/ul_api_utils/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8453 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/commands/cmd_enc_keys.py
--rw-rw-rw-   0 root         (0) root         (0)     2732 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/commands/cmd_gen_api_user_token.py
--rw-rw-rw-   0 root         (0) root         (0)     4549 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/commands/cmd_gen_new_api_user.py
--rw-rw-rw-   0 root         (0) root         (0)     4453 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/commands/cmd_start.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/commands/cmd_worker_start.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.937605 ul-api-utils-7.3.0/ul_api_utils/commands/start/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/commands/start/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/commands/start/gunicorn.conf.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/commands/start/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.937605 ul-api-utils-7.3.0/ul_api_utils/conf/
--rw-rw-rw-   0 root         (0) root         (0)   999747 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/conf/ul-debugger-main.js
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/conf/ul-debugger-ui.js
--rw-rw-rw-   0 root         (0) root         (0)     3008 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.937605 ul-api-utils-7.3.0/ul_api_utils/debug/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/debug/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/debug/debugger.py
--rw-rw-rw-   0 root         (0) root         (0)     3274 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/debug/malloc.py
--rw-rw-rw-   0 root         (0) root         (0)    14591 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/debug/stat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.937605 ul-api-utils-7.3.0/ul_api_utils/encrypt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/encrypt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/encrypt/encrypt_decrypt_abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     2356 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py
--rw-rw-rw-   0 root         (0) root         (0)     8137 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.941605 ul-api-utils-7.3.0/ul_api_utils/internal_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/internal_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.941605 ul-api-utils-7.3.0/ul_api_utils/internal_api/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/internal_api/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/internal_api/__tests__/internal_api.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/internal_api/__tests__/internal_api_content_type.py
--rw-rw-rw-   0 root         (0) root         (0)    14067 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/internal_api/internal_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/internal_api/internal_api_check_context.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/internal_api/internal_api_error.py
--rw-rw-rw-   0 root         (0) root         (0)    11583 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/internal_api/internal_api_response.py
--rw-rw-rw-   0 root         (0) root         (0)      779 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.941605 ul-api-utils-7.3.0/ul_api_utils/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.941605 ul-api-utils-7.3.0/ul_api_utils/modules/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/modules/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10719 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py
--rw-rw-rw-   0 root         (0) root         (0)    20862 2023-06-28 12:08:16.000000 ul-api-utils-7.3.0/ul_api_utils/modules/api_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)     1761 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/modules/api_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15112 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/modules/api_sdk_jwt.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/modules/intermediate_state.py
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/modules/worker_context.py
--rw-rw-rw-   0 root         (0) root         (0)     4620 2023-06-28 12:08:16.000000 ul-api-utils-7.3.0/ul_api_utils/modules/worker_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/modules/worker_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.941605 ul-api-utils-7.3.0/ul_api_utils/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5077 2023-06-28 12:08:16.000000 ul-api-utils-7.3.0/ul_api_utils/resources/debugger_scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.945605 ul-api-utils-7.3.0/ul_api_utils/resources/health_check/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/resources/health_check/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/resources/health_check/const.py
--rw-rw-rw-   0 root         (0) root         (0)    18739 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/resources/health_check/health_check.py
--rw-rw-rw-   0 root         (0) root         (0)     2572 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/resources/health_check/health_check_template.py
--rw-rw-rw-   0 root         (0) root         (0)     4199 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/resources/health_check/resource.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/resources/not_implemented.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/resources/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     3358 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/resources/rate_limitter.py
--rw-rw-rw-   0 root         (0) root         (0)     5142 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/resources/swagger.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/sentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.945605 ul-api-utils-7.3.0/ul_api_utils/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.949605 ul-api-utils-7.3.0/ul_api_utils/utils/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/__tests__/api_path_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2487 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/__tests__/unwrap_typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/api_encoding.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/api_format.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/api_method.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/api_pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/api_path_version.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/api_request_info.py
--rw-rw-rw-   0 root         (0) root         (0)     5021 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/avro.py
--rw-rw-rw-   0 root         (0) root         (0)      670 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/cached_per_request.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/colors.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/decode_base64.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/deprecated.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.949605 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.949605 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/specifiers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/specifiers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py
--rw-rw-rw-   0 root         (0) root         (0)    28921 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.949605 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2603 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/utils/schema_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/imports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.949605 ul-api-utils-7.3.0/ul_api_utils/utils/jinja/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/jinja/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/jinja/t_url_for.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/jinja/to_pretty_json.py
--rw-rw-rw-   0 root         (0) root         (0)     4123 2023-06-28 12:08:16.000000 ul-api-utils-7.3.0/ul_api_utils/utils/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/load_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-06-28 12:08:16.000000 ul-api-utils-7.3.0/ul_api_utils/utils/token_check.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/token_check_through_request.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/unwrap_typing.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/utils/uuid_converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.949605 ul-api-utils-7.3.0/ul_api_utils/validators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/validators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.949605 ul-api-utils-7.3.0/ul_api_utils/validators/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/validators/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/validators/__tests__/test_custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     4023 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/validators/custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/validators/validate_empty_object.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-22 12:49:56.000000 ul-api-utils-7.3.0/ul_api_utils/validators/validate_uuid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 12:08:17.933605 ul-api-utils-7.3.0/ul_api_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13527 2023-06-28 12:08:17.000000 ul-api-utils-7.3.0/ul_api_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5370 2023-06-28 12:08:17.000000 ul-api-utils-7.3.0/ul_api_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 12:08:17.000000 ul-api-utils-7.3.0/ul_api_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-28 12:08:17.000000 ul-api-utils-7.3.0/ul_api_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      430 2023-06-28 12:08:17.000000 ul-api-utils-7.3.0/ul_api_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-28 12:08:17.000000 ul-api-utils-7.3.0/ul_api_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.195166 ul-api-utils-7.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13527 2023-07-03 18:46:26.191166 ul-api-utils-7.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12938 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.119164 ul-api-utils-7.3.1/example/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/example/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/example/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/example/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.119164 ul-api-utils-7.3.1/example/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/example/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/example/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/example/pure_flask_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/example/rate_limit_load.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.127164 ul-api-utils-7.3.1/example/routes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/example/routes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11237 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/example/routes/api_some.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.127164 ul-api-utils-7.3.1/example/workers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/example/workers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/example/workers/worker.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 18:46:26.195166 ul-api-utils-7.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2548 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.131164 ul-api-utils-7.3.1/ul_api_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.131164 ul-api-utils-7.3.1/ul_api_utils/access/
+-rw-rw-rw-   0 root         (0) root         (0)     4274 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.155165 ul-api-utils-7.3.1/ul_api_utils/api_resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    17185 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_resource_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    17241 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_resource_fn_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_resource_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     9676 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_response_db.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_response_payload_alias.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/db_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/signature_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.159165 ul-api-utils-7.3.1/ul_api_utils/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8453 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/cmd_enc_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)     2732 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/cmd_gen_api_user_token.py
+-rw-rw-rw-   0 root         (0) root         (0)     4549 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/cmd_gen_new_api_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     4453 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/cmd_start.py
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/cmd_worker_start.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.159165 ul-api-utils-7.3.1/ul_api_utils/commands/start/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/start/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/start/gunicorn.conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/start/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.159165 ul-api-utils-7.3.1/ul_api_utils/conf/
+-rw-rw-rw-   0 root         (0) root         (0)   999747 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/conf/ul-debugger-main.js
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/conf/ul-debugger-ui.js
+-rw-rw-rw-   0 root         (0) root         (0)     3008 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.163165 ul-api-utils-7.3.1/ul_api_utils/debug/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/debug/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/debug/debugger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3274 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/debug/malloc.py
+-rw-rw-rw-   0 root         (0) root         (0)    14591 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/debug/stat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.163165 ul-api-utils-7.3.1/ul_api_utils/encrypt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/encrypt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/encrypt/encrypt_decrypt_abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py
+-rw-rw-rw-   0 root         (0) root         (0)     8137 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.167165 ul-api-utils-7.3.1/ul_api_utils/internal_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.167165 ul-api-utils-7.3.1/ul_api_utils/internal_api/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/__tests__/internal_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/__tests__/internal_api_content_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    14067 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/internal_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/internal_api_check_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/internal_api_error.py
+-rw-rw-rw-   0 root         (0) root         (0)    11583 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/internal_api_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      779 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.171165 ul-api-utils-7.3.1/ul_api_utils/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.171165 ul-api-utils-7.3.1/ul_api_utils/modules/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10719 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)    20862 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/api_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)     1761 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/api_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15112 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/api_sdk_jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/intermediate_state.py
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/worker_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     4620 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/worker_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/worker_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.175166 ul-api-utils-7.3.1/ul_api_utils/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5077 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/debugger_scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.175166 ul-api-utils-7.3.1/ul_api_utils/resources/health_check/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/health_check/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/health_check/const.py
+-rw-rw-rw-   0 root         (0) root         (0)    18739 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/health_check/health_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     2572 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/health_check/health_check_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     4199 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/health_check/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/not_implemented.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3358 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/rate_limitter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5142 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/swagger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/sentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.183166 ul-api-utils-7.3.1/ul_api_utils/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.183166 ul-api-utils-7.3.1/ul_api_utils/utils/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/__tests__/api_path_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/__tests__/unwrap_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/api_encoding.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/api_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/api_method.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/api_pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/api_path_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/api_request_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     5021 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/avro.py
+-rw-rw-rw-   0 root         (0) root         (0)      670 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/cached_per_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/decode_base64.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/deprecated.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.187166 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.187166 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    28921 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.191166 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/schema_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/imports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.191166 ul-api-utils-7.3.1/ul_api_utils/utils/jinja/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/jinja/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/jinja/t_url_for.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/jinja/to_pretty_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     4123 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/load_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/token_check.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/token_check_through_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/unwrap_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/uuid_converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.191166 ul-api-utils-7.3.1/ul_api_utils/validators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/validators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.191166 ul-api-utils-7.3.1/ul_api_utils/validators/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/validators/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/validators/__tests__/test_custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     4023 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/validators/custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/validators/validate_empty_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/validators/validate_uuid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.131164 ul-api-utils-7.3.1/ul_api_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13527 2023-07-03 18:46:25.000000 ul-api-utils-7.3.1/ul_api_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-07-03 18:46:25.000000 ul-api-utils-7.3.1/ul_api_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 18:46:25.000000 ul-api-utils-7.3.1/ul_api_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-03 18:46:25.000000 ul-api-utils-7.3.1/ul_api_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      430 2023-07-03 18:46:25.000000 ul-api-utils-7.3.1/ul_api_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-03 18:46:25.000000 ul-api-utils-7.3.1/ul_api_utils.egg-info/top_level.txt
```

### Comparing `ul-api-utils-7.3.0/LICENSE` & `ul-api-utils-7.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/PKG-INFO` & `ul-api-utils-7.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-api-utils
-Version: 7.3.0
+Version: 7.3.1
 Summary: Python api utils
 Author: Unic-lab
 Author-email: 
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-api-utils-7.3.0/README.md` & `ul-api-utils-7.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/example/conf.py` & `ul-api-utils-7.3.1/example/conf.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/example/pure_flask_example.py` & `ul-api-utils-7.3.1/example/pure_flask_example.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/example/routes/api_some.py` & `ul-api-utils-7.3.1/example/routes/api_some.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/example/workers/worker.py` & `ul-api-utils-7.3.1/example/workers/worker.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/setup.py` & `ul-api-utils-7.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-api-utils',
-    version='7.3.0',
+    version='7.3.1',
     description='Python api utils',
     author='Unic-lab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='',
     packages=find_packages(),
     package_data={
```

### Comparing `ul-api-utils-7.3.0/ul_api_utils/access/__init__.py` & `ul-api-utils-7.3.1/ul_api_utils/access/__init__.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/api_resource/api_request.py` & `ul-api-utils-7.3.1/ul_api_utils/api_resource/api_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/api_resource/api_resource.py` & `ul-api-utils-7.3.1/ul_api_utils/api_resource/api_resource.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/api_resource/api_resource_config.py` & `ul-api-utils-7.3.1/ul_api_utils/api_resource/api_resource_config.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/api_resource/api_resource_fn_typing.py` & `ul-api-utils-7.3.1/ul_api_utils/api_resource/api_resource_fn_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/api_resource/api_response.py` & `ul-api-utils-7.3.1/ul_api_utils/api_resource/api_response.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/api_resource/api_response_db.py` & `ul-api-utils-7.3.1/ul_api_utils/api_resource/api_response_db.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/api_resource/api_response_payload_alias.py` & `ul-api-utils-7.3.1/ul_api_utils/api_resource/api_response_payload_alias.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/api_resource/signature_check.py` & `ul-api-utils-7.3.1/ul_api_utils/api_resource/signature_check.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/commands/cmd_enc_keys.py` & `ul-api-utils-7.3.1/ul_api_utils/commands/cmd_enc_keys.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/commands/cmd_gen_api_user_token.py` & `ul-api-utils-7.3.1/ul_api_utils/commands/cmd_gen_api_user_token.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/commands/cmd_gen_new_api_user.py` & `ul-api-utils-7.3.1/ul_api_utils/commands/cmd_gen_new_api_user.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/commands/cmd_start.py` & `ul-api-utils-7.3.1/ul_api_utils/commands/cmd_start.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/commands/cmd_worker_start.py` & `ul-api-utils-7.3.1/ul_api_utils/commands/cmd_worker_start.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/commands/start/wsgi.py` & `ul-api-utils-7.3.1/ul_api_utils/commands/start/wsgi.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/conf/ul-debugger-main.js` & `ul-api-utils-7.3.1/ul_api_utils/conf/ul-debugger-main.js`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/conf/ul-debugger-ui.js` & `ul-api-utils-7.3.1/ul_api_utils/conf/ul-debugger-ui.js`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/conf.py` & `ul-api-utils-7.3.1/ul_api_utils/conf.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/const.py` & `ul-api-utils-7.3.1/ul_api_utils/const.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/debug/debugger.py` & `ul-api-utils-7.3.1/ul_api_utils/debug/debugger.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/debug/malloc.py` & `ul-api-utils-7.3.1/ul_api_utils/debug/malloc.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/debug/stat.py` & `ul-api-utils-7.3.1/ul_api_utils/debug/stat.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py` & `ul-api-utils-7.3.1/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/errors.py` & `ul-api-utils-7.3.1/ul_api_utils/errors.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/internal_api/__tests__/internal_api.py` & `ul-api-utils-7.3.1/ul_api_utils/internal_api/__tests__/internal_api.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/internal_api/__tests__/internal_api_content_type.py` & `ul-api-utils-7.3.1/ul_api_utils/internal_api/__tests__/internal_api_content_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/internal_api/internal_api.py` & `ul-api-utils-7.3.1/ul_api_utils/internal_api/internal_api.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/internal_api/internal_api_check_context.py` & `ul-api-utils-7.3.1/ul_api_utils/internal_api/internal_api_check_context.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/internal_api/internal_api_response.py` & `ul-api-utils-7.3.1/ul_api_utils/internal_api/internal_api_response.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/main.py` & `ul-api-utils-7.3.1/ul_api_utils/main.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py` & `ul-api-utils-7.3.1/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/modules/api_sdk.py` & `ul-api-utils-7.3.1/ul_api_utils/modules/api_sdk.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/modules/api_sdk_config.py` & `ul-api-utils-7.3.1/ul_api_utils/modules/api_sdk_config.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/modules/api_sdk_jwt.py` & `ul-api-utils-7.3.1/ul_api_utils/modules/api_sdk_jwt.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/modules/intermediate_state.py` & `ul-api-utils-7.3.1/ul_api_utils/modules/intermediate_state.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/modules/worker_context.py` & `ul-api-utils-7.3.1/ul_api_utils/modules/worker_context.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/modules/worker_sdk.py` & `ul-api-utils-7.3.1/ul_api_utils/modules/worker_sdk.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/resources/debugger_scripts.py` & `ul-api-utils-7.3.1/ul_api_utils/resources/debugger_scripts.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/resources/health_check/health_check.py` & `ul-api-utils-7.3.1/ul_api_utils/resources/health_check/health_check.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/resources/health_check/health_check_template.py` & `ul-api-utils-7.3.1/ul_api_utils/resources/health_check/health_check_template.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/resources/health_check/resource.py` & `ul-api-utils-7.3.1/ul_api_utils/resources/health_check/resource.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/resources/not_implemented.py` & `ul-api-utils-7.3.1/ul_api_utils/resources/not_implemented.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/resources/permissions.py` & `ul-api-utils-7.3.1/ul_api_utils/resources/permissions.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/resources/rate_limitter.py` & `ul-api-utils-7.3.1/ul_api_utils/resources/rate_limitter.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/resources/swagger.py` & `ul-api-utils-7.3.1/ul_api_utils/resources/swagger.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/sentry.py` & `ul-api-utils-7.3.1/ul_api_utils/sentry.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/__tests__/api_path_version.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/__tests__/api_path_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/__tests__/unwrap_typing.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/__tests__/unwrap_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/api_encoding.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/api_encoding.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/api_format.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/api_format.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/api_method.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/api_method.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/api_pagination.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/api_pagination.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/api_path_version.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/api_path_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/avro.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/avro.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/cached_per_request.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/cached_per_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/colors.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/deprecated.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,37 +20,32 @@
     UUID = 'uuid'
 
     def __repr__(self) -> str:
         return f'{type(self).__name__}.{self.name}'
 
     @staticmethod
     def from_string(value: str) -> 'InputType':
+        type_map = {
+            "integer": InputType.INTEGER, "int": InputType.INTEGER,
+            "number": InputType.NUMBER, "num": InputType.NUMBER,
+            "boolean": InputType.BOOLEAN, "bool": InputType.BOOLEAN,
+            "string": InputType.STRING, "str": InputType.STRING,
+            "array": InputType.ARRAY, "object": InputType.OBJECT,
+            "nested": InputType.NESTED, "datetime": InputType.STRING,
+            "uuid": InputType.UUID,
+        }
 
         if isinstance(value, str):
-
-            if value.lower() in ['integer', 'int']:
-                return InputType.INTEGER
-            elif value.lower() in ['number', 'num']:
-                return InputType.NUMBER
-            elif value.lower() in ['boolean', 'bool']:
-                return InputType.BOOLEAN
-            elif value.lower() in ['string', 'str']:
-                return InputType.STRING
-            elif value.lower() == 'array':
-                return InputType.ARRAY
-            elif value.lower() == 'object':
-                return InputType.OBJECT
-            elif value.lower() == 'nested':
-                return InputType.NESTED
-            elif value.lower() == 'datetime':
-                return InputType.STRING
-            elif value.lower() == 'uuid':
-                return InputType.UUID
-            else:
-                raise SwaggerGeneratorError('Could not convert value {} to a input type'.format(value))
+            route_with_arguments_parenthesis = '('
+            if route_with_arguments_parenthesis in value:
+                value = value.lower().split(route_with_arguments_parenthesis)[0]
+            try:
+                return type_map[value.lower()]
+            except KeyError:
+                raise SwaggerGeneratorError(f'Could not convert {value=} to a input type')
         else:
             raise SwaggerGeneratorError("Could not convert non string value to a parameter type")
 
     def equals(self, other):  # type: ignore
 
         if isinstance(other, Enum):
             return self.value == other.value
```

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/json_encoder.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/load_modules.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/load_modules.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/token_check_through_request.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/token_check_through_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/unwrap_typing.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/unwrap_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/utils/uuid_converter.py` & `ul-api-utils-7.3.1/ul_api_utils/utils/uuid_converter.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/validators/__tests__/test_custom_fields.py` & `ul-api-utils-7.3.1/ul_api_utils/validators/__tests__/test_custom_fields.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils/validators/custom_fields.py` & `ul-api-utils-7.3.1/ul_api_utils/validators/custom_fields.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.0/ul_api_utils.egg-info/PKG-INFO` & `ul-api-utils-7.3.1/ul_api_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-api-utils
-Version: 7.3.0
+Version: 7.3.1
 Summary: Python api utils
 Author: Unic-lab
 Author-email: 
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-api-utils-7.3.0/ul_api_utils.egg-info/SOURCES.txt` & `ul-api-utils-7.3.1/ul_api_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

