# Comparing `tmp/line-bot-sdk-2.4.3.tar.gz` & `tmp/line-bot-sdk-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "line-bot-sdk-2.4.3.tar", last modified: Fri Jun 30 01:47:51 2023, max compression
+gzip compressed data, was "line-bot-sdk-3.0.2.tar", last modified: Mon Jul  3 04:58:36 2023, max compression
```

## Comparing `line-bot-sdk-2.4.3.tar` & `line-bot-sdk-3.0.2.tar`

### file list

```diff
@@ -1,123 +1,218 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.471355 line-bot-sdk-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    46220 2023-06-30 01:47:51.471355 line-bot-sdk-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    45423 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.455355 line-bot-sdk-2.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.455355 line-bot-sdk-2.4.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/docs/source/linebot.models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/docs/source/linebot.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.459355 line-bot-sdk-2.4.3/line_bot_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46220 2023-06-30 01:47:51.000000 line-bot-sdk-2.4.3/line_bot_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-30 01:47:51.000000 line-bot-sdk-2.4.3/line_bot_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 01:47:51.000000 line-bot-sdk-2.4.3/line_bot_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 01:47:51.000000 line-bot-sdk-2.4.3/line_bot_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 01:47:51.000000 line-bot-sdk-2.4.3/line_bot_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.459355 line-bot-sdk-2.4.3/linebot/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/aiohttp_async_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    86776 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    88701 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/async_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/async_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.459355 line-bot-sdk-2.4.3/linebot/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/delivery_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/emojis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    19053 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    26498 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/flex_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/imagemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/insight.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/mention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/mentionee.py
--rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)    38321 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/rich_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/send_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/things.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/unsend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/video_play_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 01:47:51.471355 line-bot-sdk-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.459355 line-bot-sdk-2.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.463355 line-bot-sdk-2.4.3/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_channel_access_token_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_error_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_bot_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_custom_aggregation_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_insight.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_member_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_member_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_message_quota.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_room.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_issue_channel_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_issue_link_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_leave.py
--rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_narrowcast_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_revoke_channel_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    17746 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_rich_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_rich_menu_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_audio_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_image_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_imagemap_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_location_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_sticker_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_template_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_text_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_text_message_with_quick_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_text_message_with_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_text_message_with_statistics_per_aggregation_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_video_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_set_webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_test_webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_validate_message_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.463355 line-bot-sdk-2.4.3/tests/async_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/async_api/test_async_error_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/async_api/test_get_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/async_api/test_get_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.463355 line-bot-sdk-2.4.3/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/serialize_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_background.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_flex_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_imagemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_send_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_text_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/test_aiohttp_async_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/test_webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.471355 line-bot-sdk-2.4.3/tests/text/
--rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/text/webhook.json
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.385014 line-bot-sdk-3.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.385014 line-bot-sdk-3.0.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/docs/source/linebot.models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/docs/source/linebot.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.389014 line-bot-sdk-3.0.2/line_bot_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-07-03 04:58:36.000000 line-bot-sdk-3.0.2/line_bot_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-07-03 04:58:36.000000 line-bot-sdk-3.0.2/line_bot_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 04:58:36.000000 line-bot-sdk-3.0.2/line_bot_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-03 04:58:36.000000 line-bot-sdk-3.0.2/line_bot_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 04:58:36.000000 line-bot-sdk-3.0.2/line_bot_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.393014 line-bot-sdk-3.0.2/linebot/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/aiohttp_async_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109752 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114831 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/async_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/async_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.401014 line-bot-sdk-3.0.2/linebot/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/delivery_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26498 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/flex_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/imagemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/mention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/mentionee.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38321 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/rich_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/send_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/things.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/unsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/video_play_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.401014 line-bot-sdk-3.0.2/linebot/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.405014 line-bot-sdk-3.0.2/linebot/v3/audience/
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30106 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30342 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14497 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.405014 line-bot-sdk-3.0.2/linebot/v3/insight/
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30118 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30354 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.409014 line-bot-sdk-3.0.2/linebot/v3/liff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30050 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30286 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.409014 line-bot-sdk-3.0.2/linebot/v3/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30112 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30348 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.409014 line-bot-sdk-3.0.2/linebot/v3/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/models/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.409014 line-bot-sdk-3.0.2/linebot/v3/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30094 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30330 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.409014 line-bot-sdk-3.0.2/linebot/v3/moduleattach/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30130 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30366 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14932 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.409014 line-bot-sdk-3.0.2/linebot/v3/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30100 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30336 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.409014 line-bot-sdk-3.0.2/linebot/v3/shop/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30091 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.413014 line-bot-sdk-3.0.2/linebot/v3/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30118 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30354 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.413014 line-bot-sdk-3.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_channel_access_token_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_error_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_bot_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_custom_aggregation_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_member_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_member_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_message_quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_issue_channel_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_issue_link_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_leave.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_narrowcast_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_revoke_channel_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17746 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_rich_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_rich_menu_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_audio_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_image_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_imagemap_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_location_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_sticker_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_template_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_text_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_text_message_with_quick_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_text_message_with_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_text_message_with_statistics_per_aggregation_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_video_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_set_webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_test_webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_validate_message_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/tests/async_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/async_api/test_async_error_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/async_api/test_get_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/async_api/test_get_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/serialize_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_flex_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_imagemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_send_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_text_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/test_aiohttp_async_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/tests/text/
+-rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/text/webhook.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/tests/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/v3/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39963 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/v3/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/tests/v3/text/
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/v3/text/webhook.json
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tox.ini
```

### Comparing `line-bot-sdk-2.4.3/LICENSE` & `line-bot-sdk-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/docs/Makefile` & `line-bot-sdk-3.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/docs/source/conf.py` & `line-bot-sdk-3.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/docs/source/linebot.models.rst` & `line-bot-sdk-3.0.2/docs/source/linebot.models.rst`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/__about__.py` & `line-bot-sdk-3.0.2/linebot/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations
 #  under the License.
 
 """Meta data of line-bot-sdk."""
 
 
-__version__ = '2.4.3'
+__version__ = '3.0.2'
 __author__ = 'LINE Corporation'
 __copyright__ = 'Copyright 2016, LINE Corporation'
 __license__ = 'Apache 2.0'
 
 __all__ = (
     '__version__'
 )
```

### Comparing `line-bot-sdk-2.4.3/linebot/__init__.py` & `line-bot-sdk-3.0.2/linebot/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,7 +35,12 @@
 )
 from .webhook import (  # noqa
     SignatureValidator,
     WebhookParser,
     WebhookHandler,
     WebhookPayload,
 )
+
+from .deprecations import (
+    LineBotSdkDeprecationWarning,
+    LineBotSdkDeprecatedIn30,
+)
```

### Comparing `line-bot-sdk-2.4.3/linebot/aiohttp_async_http_client.py` & `line-bot-sdk-3.0.2/linebot/aiohttp_async_http_client.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/async_http_client.py` & `line-bot-sdk-3.0.2/linebot/async_http_client.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/exceptions.py` & `line-bot-sdk-3.0.2/linebot/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,19 +10,24 @@
 #  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations
 #  under the License.
 
 """linebot.exceptions module."""
 
-
 from abc import ABCMeta
 
 from future.utils import with_metaclass
 
+from deprecated import deprecated
+
+from .deprecations import (
+    LineBotSdkDeprecatedIn30
+)
+
 
 class BaseError(with_metaclass(ABCMeta, Exception)):
     """Base Exception class."""
 
     def __init__(self, message='-'):
         """__init__ method.
 
@@ -39,14 +44,15 @@
 
         :rtype: str
         """
         return '<{0} [{1}]>'.format(
             self.__class__.__name__, self.message)
 
 
+@deprecated(reason="Use 'from linebot.v3.exceptions import InvalidSignatureError' and v3 webhook handlers instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class InvalidSignatureError(BaseError):
     """When Webhook signature does NOT match, this error will be raised."""
 
     def __init__(self, message='-'):
         """__init__ method.
 
         :param str message: Human readable message
```

### Comparing `line-bot-sdk-2.4.3/linebot/http_client.py` & `line-bot-sdk-3.0.2/linebot/http_client.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/__init__.py` & `line-bot-sdk-3.0.2/linebot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/actions.py` & `line-bot-sdk-3.0.2/linebot/models/actions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/background.py` & `line-bot-sdk-3.0.2/linebot/models/background.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/base.py` & `line-bot-sdk-3.0.2/linebot/models/base.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/delivery_context.py` & `line-bot-sdk-3.0.2/linebot/v3/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,22 @@
+# -*- coding: utf-8 -*-
+
 #  Licensed under the Apache License, Version 2.0 (the "License"); you may
 #  not use this file except in compliance with the License. You may obtain
 #  a copy of the License at
 #
 #       https://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations
 #  under the License.
 
-"""linebot.models.delivery_context module."""
-
-
-from abc import ABCMeta
-
-from future.utils import with_metaclass
-
-from .base import Base
-
-
-class DeliveryContext(with_metaclass(ABCMeta, Base)):
-    """Abstract Base Class of DeliveryContext."""
-
-    def __init__(self, is_redelivery=None, **kwargs):
-        """__init__ method.
-
-        :param bool is_redelivery: Whether the webhook event is a redelivered one or not
-        :param kwargs:
-        """
-        super(DeliveryContext, self).__init__(**kwargs)
+"""linebot.v3 package."""
 
-        self.is_redelivery = is_redelivery
+from .webhook import (  # noqa
+    SignatureValidator,
+    WebhookParser,
+    WebhookHandler,
+    WebhookPayload,
+)
```

### Comparing `line-bot-sdk-2.4.3/linebot/models/emojis.py` & `line-bot-sdk-3.0.2/linebot/models/emojis.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/error.py` & `line-bot-sdk-3.0.2/linebot/models/error.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/events.py` & `line-bot-sdk-3.0.2/linebot/models/events.py`

 * *Files 25% similar despite different names*

```diff
@@ -36,15 +36,24 @@
     DeviceLink,
     ScenarioResult,
 )
 from linebot.models.things import Things  # noqa, backward compatibility
 from linebot.models.unsend import Unsend
 from linebot.models.video_play_complete import VideoPlayComplete
 
+from deprecated import deprecated
 
+from deprecated import deprecated
+
+from linebot.deprecations import (
+    LineBotSdkDeprecatedIn30
+)
+
+
+@deprecated(reason="Use 'from linebot.v3.webhooks import VideoPlayComplete' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class Event(with_metaclass(ABCMeta, Base)):
     """Abstract Base Class of Webhook Event.
 
     https://developers.line.biz/en/reference/messaging-api/#webhook-event-objects
     """
 
     def __init__(
@@ -78,14 +87,15 @@
         )
         self.webhook_event_id = webhook_event_id
         self.delivery_context = self.get_or_new_from_json_dict(
             delivery_context, DeliveryContext
         )
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import MessageEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class MessageEvent(Event):
     """Webhook MessageEvent.
 
     https://developers.line.biz/en/reference/messaging-api/#message-event
 
     Event object which contains the sent message.
     The message field contains a message object which corresponds with the message type.
@@ -120,14 +130,15 @@
                 'location': LocationMessage,
                 'sticker': StickerMessage,
                 'file': FileMessage
             }
         )
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import FollowEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class FollowEvent(Event):
     """Webhook FollowEvent.
 
     https://developers.line.biz/en/reference/messaging-api/#follow-event
 
     Event object for when your account is added as a friend (or unblocked).
     You can reply to follow events.
@@ -147,14 +158,15 @@
             mode=mode, timestamp=timestamp, source=source, **kwargs
         )
 
         self.type = 'follow'
         self.reply_token = reply_token
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import UnfollowEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class UnfollowEvent(Event):
     """Webhook UnfollowEvent.
 
     https://developers.line.biz/en/reference/messaging-api/#unfollow-event
 
     Event object for when your account is blocked.
     """
@@ -171,14 +183,15 @@
         super(UnfollowEvent, self).__init__(
             mode=mode, timestamp=timestamp, source=source, **kwargs
         )
 
         self.type = 'unfollow'
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import JoinEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class JoinEvent(Event):
     """Webhook JoinEvent.
 
     https://developers.line.biz/en/reference/messaging-api/#join-event
 
     Event object for when your account joins a group or talk room.
     You can reply to join events.
@@ -198,14 +211,15 @@
             mode=mode, timestamp=timestamp, source=source, **kwargs
         )
 
         self.type = 'join'
         self.reply_token = reply_token
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import LeaveEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class LeaveEvent(Event):
     """Webhook LeaveEvent.
 
     https://developers.line.biz/en/reference/messaging-api/#leave-event
 
     Event object for when your account leaves a group.
     """
@@ -222,14 +236,15 @@
         super(LeaveEvent, self).__init__(
             mode=mode, timestamp=timestamp, source=source, **kwargs
         )
 
         self.type = 'leave'
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import PostbackEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class PostbackEvent(Event):
     """Webhook PostbackEvent.
 
     https://developers.line.biz/en/reference/messaging-api/#postback-event
 
     Event object for when a user performs an action on
     a template message which initiates a postback.
@@ -256,14 +271,15 @@
         self.type = 'postback'
         self.reply_token = reply_token
         self.postback = self.get_or_new_from_json_dict(
             postback, Postback
         )
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import BeaconEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class BeaconEvent(Event):
     """Webhook BeaconEvent.
 
     https://developers.line.biz/en/reference/messaging-api/#beacon-event
 
     Event object for when a user detects a LINE Beacon. You can reply to beacon events.
     """
@@ -288,14 +304,15 @@
         self.type = 'beacon'
         self.reply_token = reply_token
         self.beacon = self.get_or_new_from_json_dict(
             beacon, Beacon
         )
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import MemberJoinedEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class MemberJoinedEvent(Event):
     """Webhook MemberJoinedEvent.
 
     https://developers.line.biz/en/reference/messaging-api/#member-joined-event
 
     Event object for when a user joins a group or room that the bot is in.
 
@@ -321,14 +338,15 @@
         self.type = 'memberJoined'
         self.reply_token = reply_token
         self.joined = self.get_or_new_from_json_dict(
             joined, Joined
         )
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import MemberLeftEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class MemberLeftEvent(Event):
     """Webhook MemberLeftEvent.
 
     https://developers.line.biz/en/reference/messaging-api/#member-left-event
 
     Event object for when a user leaves a group or room that the bot is in.
 
@@ -351,14 +369,15 @@
 
         self.type = 'memberLeft'
         self.left = self.get_or_new_from_json_dict(
             left, Left
         )
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import AccountLinkEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class AccountLinkEvent(Event):
     """Webhook AccountLinkEvent.
 
     https://developers.line.me/en/docs/messaging-api/reference/#account-link-event
 
     Event object for when a user has linked his/her LINE account with a provider's service account.
     You can reply to account link events.
@@ -386,14 +405,15 @@
         self.type = 'accountLink'
         self.reply_token = reply_token
         self.link = self.get_or_new_from_json_dict(
             link, Link
         )
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import ThingsEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class ThingsEvent(Event):
     """Webhook ThingsEvent.
 
     https://developers.line.biz/en/reference/messaging-api/#device-link-event
     https://developers.line.biz/en/reference/messaging-api/#device-unlink-event
     https://developers.line.biz/en/reference/messaging-api/#scenario-result-event
 
@@ -424,14 +444,15 @@
                 'link': DeviceLink,
                 'unlink': DeviceUnlink,
                 'scenarioResult': ScenarioResult,
             }
         )
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import UnsendEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class UnsendEvent(Event):
     """Webhook UnsendEvent.
 
     https://developers.line.biz/en/reference/messaging-api/#unsend-event
 
     Event object for when the user unsends a message in a group or room.
     """
@@ -453,14 +474,15 @@
 
         self.type = 'unsend'
         self.unsend = self.get_or_new_from_json_dict(
             unsend, Unsend
         )
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import VideoPlayCompleteEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class VideoPlayCompleteEvent(Event):
     """Webhook VideoCompleteEvent.
 
     https://developers.line.biz/en/reference/messaging-api/#video-viewing-complete
 
     Event object Event for when a user finishes viewing a video at least once.
     """
@@ -486,14 +508,15 @@
         self.type = 'videoPlayComplete'
         self.reply_token = reply_token
         self.video_play_complete = self.get_or_new_from_json_dict(
             video_play_complete, VideoPlayComplete
         )
 
 
+@deprecated(reason="Use 'from linebot.v3.models import UnknownEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class UnknownEvent(Event):
     """Unknown event.
 
     We welcome your contribution to line-bot-sdk-python!
     """
 
     def __init__(self, **kwargs):
@@ -502,14 +525,15 @@
         :param kwargs:
         """
         super(UnknownEvent, self).__init__(**kwargs)
 
         self.type = 'unknown'
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import PostbackContent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class Postback(Base):
     """Postback.
 
     https://developers.line.biz/en/reference/messaging-api/#postback-event
     """
 
     def __init__(self, data=None, params=None, **kwargs):
@@ -523,14 +547,15 @@
         """
         super(Postback, self).__init__(**kwargs)
 
         self.data = data
         self.params = params
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import BeaconContent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class Beacon(Base):
     """Beacon.
 
     https://developers.line.biz/en/reference/messaging-api/#beacon-event
     """
 
     def __init__(self, type=None, hwid=None, dm=None, **kwargs):
@@ -552,14 +577,15 @@
         """Get dm(device_message) as bytearray.
 
         :rtype: bytearray
         """
         return bytearray.fromhex(self.dm) if self.dm is not None else None
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import JoinedMembers' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class Joined(Base):
     """Joined.
 
     https://developers.line.biz/en/reference/messaging-api/#member-joined-event
     """
 
     def __init__(self, members=None, **kwargs):
@@ -574,14 +600,15 @@
 
     @property
     def members(self):
         """Get members as list of SourceUser."""
         return [SourceUser(user_id=x['userId']) for x in self._members]
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import LeftMembers' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class Left(Base):
     """Left.
 
     https://developers.line.biz/en/reference/messaging-api/#member-left-event
     """
 
     def __init__(self, members=None, **kwargs):
@@ -596,14 +623,15 @@
 
     @property
     def members(self):
         """Get members as list of SourceUser."""
         return [SourceUser(user_id=x['userId']) for x in self._members]
 
 
+@deprecated(reason="Use 'from linebot.v3.webhooks import AccountLinkEvent' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class Link(Base):
     """Link.
 
     https://developers.line.me/en/docs/messaging-api/reference/#link-object
     """
 
     def __init__(self, result=None, nonce=None, **kwargs):
```

### Comparing `line-bot-sdk-2.4.3/linebot/models/filter.py` & `line-bot-sdk-3.0.2/linebot/models/filter.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/flex_message.py` & `line-bot-sdk-3.0.2/linebot/models/flex_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/imagemap.py` & `line-bot-sdk-3.0.2/linebot/models/imagemap.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/insight.py` & `line-bot-sdk-3.0.2/linebot/models/insight.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/limit.py` & `line-bot-sdk-3.0.2/linebot/models/limit.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/mention.py` & `line-bot-sdk-3.0.2/linebot/models/mention.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,15 +17,22 @@
 
 from abc import ABCMeta
 
 from future.utils import with_metaclass
 
 from .base import Base
 
+from deprecated import deprecated
 
+from linebot.deprecations import (
+    LineBotSdkDeprecatedIn30
+)
+
+
+@deprecated(reason="Use 'from linebot.v3.webhooks import Mention' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class Mention(with_metaclass(ABCMeta, Base)):
     """Mention.
 
     https://developers.line.biz/en/reference/messaging-api/#text-message
 
     Object containing the contents of the mentioned user.
     """
```

### Comparing `line-bot-sdk-2.4.3/linebot/models/mentionee.py` & `line-bot-sdk-3.0.2/linebot/models/video_play_complete.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,38 +8,37 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations
 #  under the License.
 
-"""linebot.models.mentionee module."""
+"""linebot.models.video_play_complete module."""
 
 
 from abc import ABCMeta
 
 from future.utils import with_metaclass
 
 from .base import Base
 
+from deprecated import deprecated
 
-class Mentionee(with_metaclass(ABCMeta, Base)):
-    """Mentionee.
+from linebot.deprecations import (
+    LineBotSdkDeprecatedIn30
+)
 
-    https://developers.line.biz/en/reference/messaging-api/#text-message
 
-    Mentioned user information.
-    """
+@deprecated(reason="Use 'from linebot.v3.webhooks import VideoPlayComplete' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
+class VideoPlayComplete(with_metaclass(ABCMeta, Base)):
+    """Abstract Base Class of VideoPlayComplete."""
 
-    def __init__(self, index=None, length=None, user_id=None, **kwargs):
+    def __init__(self, tracking_id=None, **kwargs):
         """__init__ method.
 
-        :param int index: Index position of the user mention for a character
-        :param int length: Length of the text of the mentioned user
-        :param str user_id: User ID
+        :param str tracking_id: the video viewing complete event occurs
+            when the user finishes watching the video.
+            Max character limit: 100.
         :param kwargs:
         """
-        super(Mentionee, self).__init__(**kwargs)
-
-        self.index = index
-        self.length = length
-        self.user_id = user_id
+        super(VideoPlayComplete, self).__init__(**kwargs)
+        self.tracking_id = tracking_id
```

### Comparing `line-bot-sdk-2.4.3/linebot/models/messages.py` & `line-bot-sdk-3.0.2/linebot/models/send_messages.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,60 +8,61 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations
 #  under the License.
 
-"""linebot.models.messages module."""
+"""linebot.models.send_messages module."""
 
 
 from abc import ABCMeta
 
 from future.utils import with_metaclass
 
-from linebot.models.emojis import Emojis
-from .mention import Mention
-from .mentionee import Mentionee
+from .emojis import Emojis
+from .actions import get_action
 from .base import Base
 
 
-class Message(with_metaclass(ABCMeta, Base)):
-    """Abstract Base Class of Message."""
+class SendMessage(with_metaclass(ABCMeta, Base)):
+    """Abstract Base Class of SendMessage."""
 
-    def __init__(self, id=None, **kwargs):
+    def __init__(self, quick_reply=None, sender=None, **kwargs):
         """__init__ method.
 
-        :param str id: Message ID
+        :param quick_reply: QuickReply object
+        :type quick_reply: T <= :py:class:`linebot.models.send_messages.QuickReply`
+        :param sender: Sender object
+        :type sender: T <= :py:class:`linebot.models.send_messages.Sender`
         :param kwargs:
         """
-        super(Message, self).__init__(**kwargs)
+        super(SendMessage, self).__init__(**kwargs)
 
         self.type = None
-        self.id = id
+        self.quick_reply = self.get_or_new_from_json_dict(quick_reply, QuickReply)
+        self.sender = self.get_or_new_from_json_dict(sender, Sender)
 
 
-class TextMessage(Message):
-    """TextMessage.
+class TextSendMessage(SendMessage):
+    """TextSendMessage.
 
-    https://developers.line.biz/en/reference/messaging-api/#wh-text
-
-    Message object which contains the text sent from the source.
+    https://developers.line.biz/en/reference/messaging-api/#text-message
     """
 
-    def __init__(self, id=None, text=None, emojis=None, mention=None, **kwargs):
+    def __init__(self, text=None, emojis=None, quick_reply=None, sender=None, **kwargs):
         """__init__ method.
 
-        :param str id: Message ID
         :param str text: Message text
-        :param List emojis: Array of LINE emoji objects
-        :param object mention: LINE mention object
+        :param quick_reply: QuickReply object
+        :type quick_reply: T <= :py:class:`linebot.models.send_messages.QuickReply`
+        :type sender: T <= :py:class:`linebot.models.send_messages.Sender`
         :param kwargs:
         """
-        super(TextMessage, self).__init__(id=id, **kwargs)
+        super(TextSendMessage, self).__init__(quick_reply=quick_reply, sender=sender, **kwargs)
 
         self.type = 'text'
         self.text = text
         if emojis:
             new_emojis = []
             for emoji in emojis:
                 emoji_object = self.get_or_new_from_json_dict(
@@ -69,226 +70,208 @@
                 )
                 if emoji_object:
                     new_emojis.append(emoji_object)
             self.emojis = new_emojis
         else:
             self.emojis = emojis
 
-        if mention:
-            mention_object = self.get_or_new_from_json_dict(
-                mention, Mention
-            )
-            mentionees = []
-            for mentionee in mention_object.mentionees:
-                mentionee_object = self.get_or_new_from_json_dict(
-                    mentionee, Mentionee
-                )
-                if mentionee_object:
-                    mentionees.append(mentionee_object)
-            self.mention = Mention(mentionees)
-        else:
-            self.mention = mention
-
-
-class ImageMessage(Message):
-    """ImageMessage.
 
-    https://developers.line.biz/en/reference/messaging-api/#wh-image
+class ImageSendMessage(SendMessage):
+    """ImageSendMessage.
 
-    Message object which contains the image content sent from the source.
-    The binary image data can be retrieved with the Content API.
+    https://developers.line.biz/en/reference/messaging-api/#image-message
     """
 
-    def __init__(self, id=None, content_provider=None, image_set=None, **kwargs):
+    def __init__(self, original_content_url=None, preview_image_url=None,
+                 quick_reply=None, sender=None, **kwargs):
         """__init__ method.
 
-        :param str id: Message ID
-        :param content_provider: ContentProvider object
-        :type content_provider:
-            :py:class:`linebot.models.messages.ContentProvider`
-        :param image_set: ImageSet object
-        :type image_set:
-            :py:class:`linebot.models.messages.ImageSet`
+        :param str original_content_url: Image URL.
+            HTTPS
+            JPEG
+            Max: 1024 x 1024
+            Max: 1 MB
+        :param str preview_image_url: Preview image URL
+            HTTPS
+            JPEG
+            Max: 240 x 240
+            Max: 1 MB
+        :param quick_reply: QuickReply object
+        :type quick_reply: T <= :py:class:`linebot.models.send_messages.QuickReply`
+        :type sender: T <= :py:class:`linebot.models.send_messages.Sender`
         :param kwargs:
         """
-        super(ImageMessage, self).__init__(id=id, **kwargs)
+        super(ImageSendMessage, self).__init__(quick_reply=quick_reply, sender=sender, **kwargs)
 
         self.type = 'image'
-        self.content_provider = self.get_or_new_from_json_dict(
-            content_provider, ContentProvider
-        )
-        self.image_set = self.get_or_new_from_json_dict(
-            image_set, ImageSet
-        )
-
+        self.original_content_url = original_content_url
+        self.preview_image_url = preview_image_url
 
-class VideoMessage(Message):
-    """VideoMessage.
 
-    https://developers.line.biz/en/reference/messaging-api/#wh-video
+class VideoSendMessage(SendMessage):
+    """VideoSendMessage.
 
-    Message object which contains the video content sent from the source.
-    The binary video data can be retrieved with the Content API.
+    https://developers.line.biz/en/reference/messaging-api/#video-message
     """
 
-    def __init__(self, id=None, duration=None, content_provider=None, **kwargs):
+    def __init__(self, original_content_url=None, preview_image_url=None,
+                 tracking_id=None, quick_reply=None, sender=None, **kwargs):
         """__init__ method.
 
-        :param str id: Message ID
-        :param long duration: Length of video file (milliseconds)
-        :param content_provider: ContentProvider object
-        :type content_provider:
-            :py:class:`linebot.models.messages.ContentProvider`
+        :param str original_content_url: URL of video file.
+            HTTPS. mp4. Less than 1 minute. Max: 10 MB.
+        :param str preview_image_url: URL of preview image.
+            HTTPS. JPEG. Max: 240 x 240. Max: 1 MB.
+        :param str tracking_id: the video viewing complete event occurs
+            when the user finishes watching the video.
+            Max character limit: 100.
+        :param quick_reply: QuickReply object
+        :type quick_reply: T <= :py:class:`linebot.models.send_messages.QuickReply`
+        :type sender: T <= :py:class:`linebot.models.send_messages.Sender`
         :param kwargs:
         """
-        super(VideoMessage, self).__init__(id=id, **kwargs)
+        super(VideoSendMessage, self).__init__(quick_reply=quick_reply, sender=sender, **kwargs)
 
         self.type = 'video'
-        self.duration = duration
-        self.content_provider = self.get_or_new_from_json_dict(
-            content_provider, ContentProvider
-        )
-
+        self.original_content_url = original_content_url
+        self.preview_image_url = preview_image_url
+        self.tracking_id = tracking_id
 
-class AudioMessage(Message):
-    """AudioMessage.
 
-    https://developers.line.biz/en/reference/messaging-api/#wh-audio
+class AudioSendMessage(SendMessage):
+    """AudioSendMessage.
 
-    Message object which contains the audio content sent from the source.
-    The binary audio data can be retrieved with the Content API.
+    https://developers.line.biz/en/reference/messaging-api/#audio-message
     """
 
-    def __init__(self, id=None, duration=None, content_provider=None, **kwargs):
+    def __init__(self, original_content_url=None, duration=None, quick_reply=None,
+                 sender=None, **kwargs):
         """__init__ method.
 
-        :param str id: Message ID
-        :param long duration: Length of audio file (milliseconds)
-        :param content_provider: ContentProvider object
-        :type content_provider:
-            :py:class:`linebot.models.messages.ContentProvider`
+        :param str original_content_url: URL of audio file. HTTPS.
+            m4a. Less than 1 minute. Max 10 MB.
+        :param long duration: Length of audio file (milliseconds).
+        :param quick_reply: QuickReply object
+        :type quick_reply: T <= :py:class:`linebot.models.send_messages.QuickReply`
+        :type sender: T <= :py:class:`linebot.models.send_messages.Sender`
         :param kwargs:
         """
-        super(AudioMessage, self).__init__(id=id, **kwargs)
+        super(AudioSendMessage, self).__init__(quick_reply=quick_reply, sender=sender, **kwargs)
 
         self.type = 'audio'
+        self.original_content_url = original_content_url
         self.duration = duration
-        self.content_provider = self.get_or_new_from_json_dict(
-            content_provider, ContentProvider
-        )
 
 
-class LocationMessage(Message):
-    """LocationMessage.
+class LocationSendMessage(SendMessage):
+    """LocationSendMessage.
 
-    https://developers.line.biz/en/reference/messaging-api/#wh-location
+    https://developers.line.biz/en/reference/messaging-api/#location-message
     """
 
-    def __init__(self, id=None, title=None, address=None, latitude=None, longitude=None,
-                 **kwargs):
+    def __init__(self, title=None, address=None, latitude=None, longitude=None,
+                 quick_reply=None, sender=None, **kwargs):
         """__init__ method.
 
-        :param str id: Message ID
         :param str title: Title
         :param str address: Address
         :param float latitude: Latitude
         :param float longitude: Longitude
+        :param quick_reply: QuickReply object
+        :type quick_reply: T <= :py:class:`linebot.models.send_messages.QuickReply`
+        :type sender: T <= :py:class:`linebot.models.send_messages.Sender`
         :param kwargs:
         """
-        super(LocationMessage, self).__init__(id=id, **kwargs)
+        super(LocationSendMessage, self).__init__(quick_reply=quick_reply, sender=sender, **kwargs)
 
         self.type = 'location'
         self.title = title
         self.address = address
         self.latitude = latitude
         self.longitude = longitude
 
 
-class StickerMessage(Message):
-    """StickerMessage.
-
-    https://developers.line.biz/en/reference/messaging-api/#wh-sticker
+class StickerSendMessage(SendMessage):
+    """StickerSendMessage.
 
-    Message object which contains the sticker data sent from the source.
-    For a list of basic LINE stickers and sticker IDs, see sticker list.
+    https://developers.line.biz/en/reference/messaging-api/#sticker-message
     """
 
-    def __init__(self, id=None, package_id=None, sticker_id=None,
-                 sticker_resource_type=None, keywords=None, text=None, **kwargs):
+    def __init__(self, package_id=None, sticker_id=None, quick_reply=None, sender=None, **kwargs):
         """__init__ method.
 
-        :param str id: Message ID
         :param str package_id: Package ID
         :param str sticker_id: Sticker ID
-        :param str sticker_resource_type: Sticker resource type
-        :param list[str] keywords: List of up to 15 keywords describing the sticker
-        :param str text: Any text entered by the user
+        :param quick_reply: QuickReply object
+        :type quick_reply: T <= :py:class:`linebot.models.send_messages.QuickReply`
+        :type sender: T <= :py:class:`linebot.models.send_messages.Sender`
         :param kwargs:
         """
-        super(StickerMessage, self).__init__(id=id, **kwargs)
+        super(StickerSendMessage, self).__init__(quick_reply=quick_reply, sender=sender, **kwargs)
 
         self.type = 'sticker'
         self.package_id = package_id
         self.sticker_id = sticker_id
-        self.sticker_resource_type = sticker_resource_type
-        self.keywords = keywords
-        self.text = text
 
 
-class FileMessage(Message):
-    """FileMessage.
+class QuickReply(with_metaclass(ABCMeta, Base)):
+    """QuickReply.
 
-    https://developers.line.biz/en/reference/messaging-api/#wh-file
-
-    Message object which contains the file content sent from the source.
-    The binary file data can be retrieved with the Content API.
+    https://developers.line.me/en/docs/messaging-api/#quick-reply
     """
 
-    def __init__(self, id=None, file_name=None, file_size=None, **kwargs):
+    def __init__(self, items=None, **kwargs):
         """__init__ method.
 
-        :param str id: Message ID
-        :param str file_name: File Name
-        :param int file_size: File Size
+        :param items: Quick reply button objects
+        :type items: list[T <= :py:class:`linebot.models.send_messages.QuickReplyButton`]
         :param kwargs:
         """
-        super(FileMessage, self).__init__(id=id, **kwargs)
+        super(QuickReply, self).__init__(**kwargs)
+
+        new_items = []
+        if items:
+            for item in items:
+                new_items.append(self.get_or_new_from_json_dict(
+                    item, QuickReplyButton
+                ))
+        self.items = new_items
 
-        self.type = 'file'
-        self.file_size = file_size
-        self.file_name = file_name
 
+class QuickReplyButton(with_metaclass(ABCMeta, Base)):
+    """QuickReplyButton.
 
-class ContentProvider(Base):
-    """Content provider."""
+    https://developers.line.me/en/reference/messaging-api/#quick-reply-button-object
+    """
 
-    def __init__(self, type=None, original_content_url=None, preview_image_url=None, **kwargs):
+    def __init__(self, image_url=None, action=None, **kwargs):
         """__init__ method.
 
-        :param str type: Provider of the content. `line` or `external`.
-        :param str original_content_url: URL of the content.
-        :param str preview_image_url: URL of the preview image.
+        :param str image_url: URL of the icon that is displayed
+            at the beginning of the button
+        :param action: Action performed when this button is tapped
+        :type action: T <= :py:class:`linebot.models.actions.Action`
         :param kwargs:
         """
-        super(ContentProvider, self).__init__(**kwargs)
+        super(QuickReplyButton, self).__init__(**kwargs)
 
-        self.type = type
-        self.original_content_url = original_content_url
-        self.preview_image_url = preview_image_url
+        self.type = 'action'
+        self.image_url = image_url
+        self.action = get_action(action)
 
 
-class ImageSet(Base):
-    """Image Set."""
+class Sender(with_metaclass(ABCMeta, Base)):
+    """Sender.
 
-    def __init__(self, id=None, index=None, total=0, **kwargs):
+    https://developers.line.biz/en/reference/messaging-api/#icon-nickname-switch
+    """
+
+    def __init__(self, name=None, icon_url=None, **kwargs):
         """__init__ method.
 
-        :param str id: Image set ID.
-        :param int index: Image number in a set of images sent simultaneously.
-        :param int total: Total number of images sent simultaneously.
-        :param kwargs:
+        :param str name: Display name
+        :param str icon_url: Icon image URL
         """
-        super(ImageSet, self).__init__(**kwargs)
+        super(Sender, self).__init__(**kwargs)
 
-        self.id = id
-        self.index = index
-        self.total = total
+        self.name = name
+        self.icon_url = icon_url
```

### Comparing `line-bot-sdk-2.4.3/linebot/models/operator.py` & `line-bot-sdk-3.0.2/linebot/models/operator.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/recipient.py` & `line-bot-sdk-3.0.2/linebot/models/recipient.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/responses.py` & `line-bot-sdk-3.0.2/linebot/models/responses.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/rich_menu.py` & `line-bot-sdk-3.0.2/linebot/models/rich_menu.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/template.py` & `line-bot-sdk-3.0.2/linebot/models/template.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/linebot/models/unsend.py` & `line-bot-sdk-3.0.2/linebot/v3/models/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,28 +8,12 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations
 #  under the License.
 
-"""linebot.models.unsend module."""
+"""linebot.v3.models package."""
 
-
-from abc import ABCMeta
-
-from future.utils import with_metaclass
-
-from .base import Base
-
-
-class Unsend(with_metaclass(ABCMeta, Base)):
-    """Abstract Base Class of Unsend."""
-
-    def __init__(self, message_id=None, **kwargs):
-        """__init__ method.
-
-        :param str message_id: The message ID of the unsent message.
-        :param kwargs:
-        """
-        super(Unsend, self).__init__(**kwargs)
-        self.message_id = message_id
+from .events import (  # noqa
+    UnknownEvent,
+)
```

### Comparing `line-bot-sdk-2.4.3/linebot/models/video_play_complete.py` & `line-bot-sdk-3.0.2/linebot/v3/models/events.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,30 +8,28 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations
 #  under the License.
 
-"""linebot.models.video_play_complete module."""
+"""linebot.v3.models.events module."""
 
+from linebot.v3.webhooks.models.event import Event
+from linebot.v3.utils import to_snake_case
 
-from abc import ABCMeta
+class UnknownEvent(Event):
+    """Unknown event.
 
-from future.utils import with_metaclass
+    We welcome your contribution to line-bot-sdk-python!
+    """
 
-from .base import Base
+    @classmethod
+    def new_from_json_dict(cls, data):
+        """Create a new instance from a dict.
 
-
-class VideoPlayComplete(with_metaclass(ABCMeta, Base)):
-    """Abstract Base Class of VideoPlayComplete."""
-
-    def __init__(self, tracking_id=None, **kwargs):
-        """__init__ method.
-
-        :param str tracking_id: the video viewing complete event occurs
-            when the user finishes watching the video.
-            Max character limit: 100.
-        :param kwargs:
+        :param data: JSON dict
         """
-        super(VideoPlayComplete, self).__init__(**kwargs)
-        self.tracking_id = tracking_id
+        new_data = {to_snake_case(key): value
+                    for key, value in data.items()}
+
+        return cls(**new_data)
```

### Comparing `line-bot-sdk-2.4.3/linebot/utils.py` & `line-bot-sdk-3.0.2/linebot/v3/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations
 #  under the License.
 
-"""linebot.utils module."""
+"""linebot.v3.utils module."""
 
 
 import logging
 import re
 
 import sys
```

### Comparing `line-bot-sdk-2.4.3/linebot/webhook.py` & `line-bot-sdk-3.0.2/linebot/webhook.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 #  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations
 #  under the License.
 
 """linebot.webhook module."""
 
-
 import base64
 import hashlib
 import hmac
 import inspect
 import json
 
 from .exceptions import InvalidSignatureError
@@ -36,14 +35,20 @@
     ThingsEvent,
     UnsendEvent,
     VideoPlayCompleteEvent,
     UnknownEvent,
 )
 from .utils import LOGGER, PY3, safe_compare_digest
 
+from deprecated import deprecated
+
+from .deprecations import (
+    LineBotSdkDeprecatedIn30
+)
+
 if hasattr(hmac, "compare_digest"):
     def compare_digest(val1, val2):
         """compare_digest function.
 
         If hmac module has compare_digest function, use it.
         Or not, use linebot.utils.safe_compare_digest.
 
@@ -68,14 +73,15 @@
         :type val2: str | bytes
         :rtype: bool
         :return: result
         """
         return safe_compare_digest(val1, val2)
 
 
+@deprecated(reason="Use 'from linebot.v3.webhook import SignatureValidator' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class SignatureValidator(object):
     """Signature validator.
 
     https://developers.line.biz/en/reference/messaging-api/#signature-validation
     """
 
     def __init__(self, channel_secret):
@@ -99,14 +105,15 @@
         ).digest()
 
         return compare_digest(
             signature.encode('utf-8'), base64.b64encode(gen_signature)
         )
 
 
+@deprecated(reason="Use 'from linebot.v3.webhook import WebhookPayload' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class WebhookPayload(object):
     """Webhook Payload.
 
     https://developers.line.biz/en/reference/messaging-api/#request-body
     """
 
     def __init__(self, events=None, destination=None):
@@ -116,14 +123,15 @@
         :type events: list[T <= :py:class:`linebot.models.events.Event`]
         :param str destination: User ID of a bot that should receive webhook events.
         """
         self.events = events
         self.destination = destination
 
 
+@deprecated(reason="Use 'from linebot.v3.webhook import WebhookParser' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class WebhookParser(object):
     """Webhook Parser."""
 
     def __init__(self, channel_secret):
         """__init__ method.
 
         :param str channel_secret: Channel secret (as text)
@@ -180,14 +188,15 @@
 
         if as_payload:
             return WebhookPayload(events=events, destination=body_json.get('destination'))
         else:
             return events
 
 
+@deprecated(reason="Use 'from linebot.v3.webhook import WebhookHandler' instead. See https://github.com/line/line-bot-sdk-python/blob/master/README.rst for more details.", version='3.0.0', category=LineBotSdkDeprecatedIn30)  # noqa: E501
 class WebhookHandler(object):
     """Webhook Handler.
 
     Please read https://github.com/line/line-bot-sdk-python#webhookhandler
     """
 
     def __init__(self, channel_secret):
@@ -206,14 +215,15 @@
         :type event: T <= :py:class:`linebot.models.events.Event` class
         :param message: (optional) If event is MessageEvent,
             specify kind of Messages which you want to handle
         :type: message: T <= :py:class:`linebot.models.messages.Message` class
         :rtype: func
         :return: decorator
         """
+
         def decorator(func):
             if isinstance(message, (list, tuple)):
                 for it in message:
                     self.__add_handler(func, event, message=it)
             else:
                 self.__add_handler(func, event, message=message)
 
@@ -223,14 +233,15 @@
 
     def default(self):
         """Set default handler method.
 
         :rtype: func
         :return: decorator
         """
+
         def decorator(func):
             self._default = func
             return func
 
         return decorator
 
     def handle(self, body, signature):
```

### Comparing `line-bot-sdk-2.4.3/tests/__init__.py` & `line-bot-sdk-3.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/__init__.py` & `line-bot-sdk-3.0.2/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_channel_access_token_v2_1.py` & `line-bot-sdk-3.0.2/tests/api/test_channel_access_token_v2_1.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_error_handle.py` & `line-bot-sdk-3.0.2/tests/api/test_error_handle.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_get_bot_info.py` & `line-bot-sdk-3.0.2/tests/api/test_get_bot_info.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_get_content.py` & `line-bot-sdk-3.0.2/tests/api/test_get_content.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_get_custom_aggregation_units.py` & `line-bot-sdk-3.0.2/tests/api/test_get_custom_aggregation_units.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_get_delivery.py` & `line-bot-sdk-3.0.2/tests/api/test_get_delivery.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_get_group.py` & `line-bot-sdk-3.0.2/tests/api/test_get_group.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_get_insight.py` & `line-bot-sdk-3.0.2/tests/api/test_get_insight.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_get_member_ids.py` & `line-bot-sdk-3.0.2/tests/api/test_get_member_ids.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_get_member_profile.py` & `line-bot-sdk-3.0.2/tests/api/test_get_member_profile.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_get_message_quota.py` & `line-bot-sdk-3.0.2/tests/api/test_get_message_quota.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_get_profile.py` & `line-bot-sdk-3.0.2/tests/api/test_get_profile.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_get_room.py` & `line-bot-sdk-3.0.2/tests/api/test_get_room.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_get_webhook_endpoint.py` & `line-bot-sdk-3.0.2/tests/api/test_get_webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_issue_channel_token.py` & `line-bot-sdk-3.0.2/tests/api/test_issue_channel_token.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_issue_link_token.py` & `line-bot-sdk-3.0.2/tests/api/test_issue_link_token.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_leave.py` & `line-bot-sdk-3.0.2/tests/api/test_leave.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_narrowcast_message.py` & `line-bot-sdk-3.0.2/tests/api/test_narrowcast_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_revoke_channel_token.py` & `line-bot-sdk-3.0.2/tests/api/test_revoke_channel_token.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_rich_menu.py` & `line-bot-sdk-3.0.2/tests/api/test_rich_menu.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_rich_menu_alias.py` & `line-bot-sdk-3.0.2/tests/api/test_rich_menu_alias.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_send_audio_message.py` & `line-bot-sdk-3.0.2/tests/api/test_send_audio_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_send_image_message.py` & `line-bot-sdk-3.0.2/tests/api/test_send_image_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_send_imagemap_message.py` & `line-bot-sdk-3.0.2/tests/api/test_send_imagemap_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_send_location_message.py` & `line-bot-sdk-3.0.2/tests/api/test_send_location_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_send_sticker_message.py` & `line-bot-sdk-3.0.2/tests/api/test_send_sticker_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_send_template_message.py` & `line-bot-sdk-3.0.2/tests/api/test_send_template_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_send_text_message.py` & `line-bot-sdk-3.0.2/tests/api/test_send_text_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_send_text_message_with_quick_reply.py` & `line-bot-sdk-3.0.2/tests/api/test_send_text_message_with_quick_reply.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_send_text_message_with_sender.py` & `line-bot-sdk-3.0.2/tests/api/test_send_text_message_with_sender.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_send_text_message_with_statistics_per_aggregation_unit.py` & `line-bot-sdk-3.0.2/tests/api/test_send_text_message_with_statistics_per_aggregation_unit.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_send_video_message.py` & `line-bot-sdk-3.0.2/tests/api/test_send_video_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_set_webhook_endpoint.py` & `line-bot-sdk-3.0.2/tests/api/test_set_webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_test_webhook_endpoint.py` & `line-bot-sdk-3.0.2/tests/api/test_test_webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/api/test_validate_message_objects.py` & `line-bot-sdk-3.0.2/tests/api/test_validate_message_objects.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/async_api/test_async_error_handle.py` & `line-bot-sdk-3.0.2/tests/async_api/test_async_error_handle.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/async_api/test_get_message_content.py` & `line-bot-sdk-3.0.2/tests/async_api/test_get_message_content.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/async_api/test_get_profile.py` & `line-bot-sdk-3.0.2/tests/async_api/test_get_profile.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/models/__init__.py` & `line-bot-sdk-3.0.2/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/models/serialize_test_case.py` & `line-bot-sdk-3.0.2/tests/models/serialize_test_case.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/models/test_actions.py` & `line-bot-sdk-3.0.2/tests/models/test_actions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/models/test_background.py` & `line-bot-sdk-3.0.2/tests/models/test_background.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/models/test_base.py` & `line-bot-sdk-3.0.2/tests/models/test_base.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/models/test_filter.py` & `line-bot-sdk-3.0.2/tests/models/test_filter.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/models/test_flex_message.py` & `line-bot-sdk-3.0.2/tests/models/test_flex_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/models/test_imagemap.py` & `line-bot-sdk-3.0.2/tests/models/test_imagemap.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/models/test_send_messages.py` & `line-bot-sdk-3.0.2/tests/models/test_send_messages.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/models/test_template.py` & `line-bot-sdk-3.0.2/tests/models/test_template.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/models/test_text_message.py` & `line-bot-sdk-3.0.2/tests/models/test_text_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/test_aiohttp_async_http_client.py` & `line-bot-sdk-3.0.2/tests/test_aiohttp_async_http_client.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/test_exceptions.py` & `line-bot-sdk-3.0.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/test_utils.py` & `line-bot-sdk-3.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/test_webhook.py` & `line-bot-sdk-3.0.2/tests/test_webhook.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tests/text/webhook.json` & `line-bot-sdk-3.0.2/tests/text/webhook.json`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.3/tox.ini` & `line-bot-sdk-3.0.2/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py3.7, py3.8, py3.9, py3.10, py3-flake8-src, py3-flake8-other
+envlist = py3.7, py3.8, py3.9, py3.10, py3.11, py3-flake8-src, py3-flake8-other
 
 [testenv]
 deps =
     six
     -r{toxinidir}/requirements.txt
     -r{toxinidir}/requirements-test.txt
 commands = py.test -v tests/
@@ -15,15 +15,16 @@
 
 [testenv:py3-flake8-src]
 basepython = python3
 deps =
     six
     flake8
     flake8-docstrings
-commands = flake8 linebot/
+# Ignores generated files.
+commands = flake8 --filename=linebot/*.py
 
 [testenv:py3-flake8-other]
 basepython = python3
 deps =
     six
     flake8
 commands = flake8 tests/ examples/ --max-line-length=120
```

