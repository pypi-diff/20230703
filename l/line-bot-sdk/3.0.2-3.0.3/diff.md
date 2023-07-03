# Comparing `tmp/line-bot-sdk-3.0.2.tar.gz` & `tmp/line-bot-sdk-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "line-bot-sdk-3.0.2.tar", last modified: Mon Jul  3 04:58:36 2023, max compression
+gzip compressed data, was "line-bot-sdk-3.0.3.tar", last modified: Mon Jul  3 07:27:57 2023, max compression
```

## Comparing `line-bot-sdk-3.0.2.tar` & `line-bot-sdk-3.0.3.tar`

### file list

```diff
@@ -1,218 +1,522 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.385014 line-bot-sdk-3.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.385014 line-bot-sdk-3.0.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/docs/source/linebot.models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/docs/source/linebot.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.389014 line-bot-sdk-3.0.2/line_bot_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-07-03 04:58:36.000000 line-bot-sdk-3.0.2/line_bot_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-07-03 04:58:36.000000 line-bot-sdk-3.0.2/line_bot_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 04:58:36.000000 line-bot-sdk-3.0.2/line_bot_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-03 04:58:36.000000 line-bot-sdk-3.0.2/line_bot_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 04:58:36.000000 line-bot-sdk-3.0.2/line_bot_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.393014 line-bot-sdk-3.0.2/linebot/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/aiohttp_async_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)   109752 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/api.py
--rw-r--r--   0 runner    (1001) docker     (123)   114831 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/async_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/async_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.401014 line-bot-sdk-3.0.2/linebot/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/delivery_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/emojis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    26498 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/flex_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/imagemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/insight.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/mention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/mentionee.py
--rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)    38321 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/rich_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/send_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/things.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/unsend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/models/video_play_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.401014 line-bot-sdk-3.0.2/linebot/v3/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.405014 line-bot-sdk-3.0.2/linebot/v3/audience/
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30106 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    30342 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/async_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/async_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14497 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/audience/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.405014 line-bot-sdk-3.0.2/linebot/v3/insight/
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30118 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    30354 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/async_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/async_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/insight/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.409014 line-bot-sdk-3.0.2/linebot/v3/liff/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30050 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    30286 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/async_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/async_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/liff/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.409014 line-bot-sdk-3.0.2/linebot/v3/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30112 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    30348 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/async_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/async_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/messaging/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.409014 line-bot-sdk-3.0.2/linebot/v3/models/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/models/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.409014 line-bot-sdk-3.0.2/linebot/v3/module/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30094 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    30330 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/async_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/async_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/module/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.409014 line-bot-sdk-3.0.2/linebot/v3/moduleattach/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30130 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    30366 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/async_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/async_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14932 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/moduleattach/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.409014 line-bot-sdk-3.0.2/linebot/v3/oauth/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30100 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    30336 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/async_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/async_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/oauth/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.409014 line-bot-sdk-3.0.2/linebot/v3/shop/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30091 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/async_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/async_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/shop/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.413014 line-bot-sdk-3.0.2/linebot/v3/webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30118 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    30354 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/async_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/async_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/v3/webhooks/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/linebot/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.413014 line-bot-sdk-3.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_channel_access_token_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_error_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_bot_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_custom_aggregation_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_insight.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_member_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_member_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_message_quota.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_room.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_get_webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_issue_channel_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_issue_link_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_leave.py
--rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_narrowcast_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_revoke_channel_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    17746 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_rich_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_rich_menu_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_audio_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_image_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_imagemap_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_location_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_sticker_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_template_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_text_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_text_message_with_quick_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_text_message_with_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_text_message_with_statistics_per_aggregation_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_send_video_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_set_webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_test_webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/api/test_validate_message_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/tests/async_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/async_api/test_async_error_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/async_api/test_get_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/async_api/test_get_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/serialize_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_background.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_flex_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_imagemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_send_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/models/test_text_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/test_aiohttp_async_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/test_webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/tests/text/
--rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/text/webhook.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/tests/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/v3/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    39963 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/v3/test_webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:58:36.417014 line-bot-sdk-3.0.2/tests/v3/text/
--rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tests/v3/text/webhook.json
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-03 04:58:27.000000 line-bot-sdk-3.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.815330 line-bot-sdk-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-07-03 07:27:57.815330 line-bot-sdk-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.735329 line-bot-sdk-3.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.735329 line-bot-sdk-3.0.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/docs/source/linebot.models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/docs/source/linebot.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.739329 line-bot-sdk-3.0.3/line_bot_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-07-03 07:27:57.000000 line-bot-sdk-3.0.3/line_bot_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19949 2023-07-03 07:27:57.000000 line-bot-sdk-3.0.3/line_bot_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 07:27:57.000000 line-bot-sdk-3.0.3/line_bot_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-03 07:27:57.000000 line-bot-sdk-3.0.3/line_bot_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 07:27:57.000000 line-bot-sdk-3.0.3/line_bot_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.743329 line-bot-sdk-3.0.3/linebot/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/aiohttp_async_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109752 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114831 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/async_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/async_http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.743329 line-bot-sdk-3.0.3/linebot/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/constants/postback_input_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.747329 line-bot-sdk-3.0.3/linebot/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/delivery_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26498 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/flex_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/imagemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/mention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/mentionee.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38321 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/rich_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/send_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/things.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/unsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/models/video_play_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.747329 line-bot-sdk-3.0.3/linebot/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.751329 line-bot-sdk-3.0.3/linebot/v3/audience/
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.751329 line-bot-sdk-3.0.3/linebot/v3/audience/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88079 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/api/async_manage_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23334 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/api/async_manage_audience_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79129 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/api/manage_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/api/manage_audience_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30106 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30342 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14497 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.755329 line-bot-sdk-3.0.3/linebot/v3/audience/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/add_audience_to_audience_group_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/audience_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/audience_group_authority_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/audience_group_create_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/audience_group_failed_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/audience_group_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/audience_group_job_failed_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/audience_group_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/audience_group_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/audience_group_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/audience_group_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/audience_group_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/create_audience_group_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/create_audience_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/create_click_based_audience_group_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/create_click_based_audience_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/create_imp_based_audience_group_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/create_imp_based_audience_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/error_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/get_audience_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/get_audience_group_authority_level_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/get_audience_groups_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/update_audience_group_authority_level_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/models/update_audience_group_description_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/audience/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.759329 line-bot-sdk-3.0.3/linebot/v3/insight/
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.759329 line-bot-sdk-3.0.3/linebot/v3/insight/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42240 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/api/async_insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37178 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/api/insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30118 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30354 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.763329 line-bot-sdk-3.0.3/linebot/v3/insight/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/age_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/app_type_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/area_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/error_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/gender_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/get_friends_demographics_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/get_message_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/get_message_event_response_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/get_message_event_response_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/get_message_event_response_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/get_number_of_followers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/get_number_of_message_deliveries_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/get_statistics_per_unit_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/get_statistics_per_unit_response_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/get_statistics_per_unit_response_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/get_statistics_per_unit_response_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/models/subscription_period_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/insight/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.763329 line-bot-sdk-3.0.3/linebot/v3/liff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.763329 line-bot-sdk-3.0.3/linebot/v3/liff/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28010 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/api/async_liff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25817 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/api/liff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30050 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30286 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.767329 line-bot-sdk-3.0.3/linebot/v3/liff/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/models/add_liff_app_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/models/add_liff_app_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/models/get_all_liff_apps_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/models/liff_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/models/liff_bot_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/models/liff_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/models/liff_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/models/liff_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/models/update_liff_app_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/liff/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.767329 line-bot-sdk-3.0.3/linebot/v3/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.771329 line-bot-sdk-3.0.3/linebot/v3/messaging/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   408550 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/api/async_messaging_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38288 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/api/async_messaging_api_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)   371721 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/api/messaging_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35076 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/api/messaging_api_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30112 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30348 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.795330 line-bot-sdk-3.0.3/linebot/v3/messaging/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/age_demographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/age_demographic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/alt_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/app_type_demographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/app_type_demographic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/area_demographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/area_demographic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/audience_match_messages_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/audience_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/audio_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/bot_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/broadcast_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/buttons_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/camera_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/camera_roll_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/carousel_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/carousel_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/chat_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/confirm_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/create_rich_menu_alias_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/datetime_picker_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/demographic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/error_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_block_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_box_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_box_linear_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_bubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_bubble_styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_carousel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_filler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_separator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/flex_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/gender_demographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/gender_demographic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/get_aggregation_unit_name_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/get_aggregation_unit_usage_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/get_followers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/get_message_content_transcoding_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/get_webhook_endpoint_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/group_member_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/group_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/group_user_profile_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/image_carousel_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/image_carousel_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/image_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/imagemap_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/imagemap_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/imagemap_base_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/imagemap_external_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/imagemap_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/imagemap_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/issue_link_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/location_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/location_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/mark_messages_as_read_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/members_ids_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/message_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/message_imagemap_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/message_quota_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/multicast_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/narrowcast_progress_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/narrowcast_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/number_of_messages_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/operator_demographic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/operator_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/pnp_messages_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/postback_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/push_message_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/quick_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/quick_reply_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/quota_consumption_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/quota_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/redelivery_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/reply_message_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/rich_menu_alias_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/rich_menu_alias_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/rich_menu_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/rich_menu_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/rich_menu_bulk_link_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/rich_menu_bulk_unlink_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/rich_menu_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/rich_menu_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/rich_menu_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/rich_menu_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/rich_menu_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/rich_menu_switch_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/room_member_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/room_user_profile_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/set_webhook_endpoint_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/sticker_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/subscription_period_demographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/subscription_period_demographic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/template_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/test_webhook_endpoint_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/test_webhook_endpoint_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/text_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/update_rich_menu_alias_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/uri_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/uri_imagemap_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/user_profile_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/validate_message_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/models/video_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/messaging/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.795330 line-bot-sdk-3.0.3/linebot/v3/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/models/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.795330 line-bot-sdk-3.0.3/linebot/v3/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.795330 line-bot-sdk-3.0.3/linebot/v3/module/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31565 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/api/async_line_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28364 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/api/line_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30094 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30330 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.795330 line-bot-sdk-3.0.3/linebot/v3/module/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/models/acquire_chat_control_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/models/detach_module_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/models/get_modules_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/models/module_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/module/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.799330 line-bot-sdk-3.0.3/linebot/v3/moduleattach/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/moduleattach/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.799330 line-bot-sdk-3.0.3/linebot/v3/moduleattach/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/moduleattach/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20296 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/moduleattach/api/async_line_module_attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/moduleattach/api/line_module_attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30130 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/moduleattach/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/moduleattach/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30366 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/moduleattach/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/moduleattach/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14932 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/moduleattach/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/moduleattach/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.799330 line-bot-sdk-3.0.3/linebot/v3/moduleattach/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/moduleattach/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/moduleattach/models/attach_module_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/moduleattach/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.799330 line-bot-sdk-3.0.3/linebot/v3/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.799330 line-bot-sdk-3.0.3/linebot/v3/oauth/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58182 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/api/async_channel_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51767 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/api/channel_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30100 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30336 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.799330 line-bot-sdk-3.0.3/linebot/v3/oauth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/models/channel_access_token_key_ids_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/models/issue_channel_access_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/models/issue_short_lived_channel_access_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/models/verify_channel_access_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/oauth/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.799330 line-bot-sdk-3.0.3/linebot/v3/shop/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/shop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.799330 line-bot-sdk-3.0.3/linebot/v3/shop/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/shop/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/shop/api/async_shop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/shop/api/shop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30091 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/shop/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/shop/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30327 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/shop/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/shop/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/shop/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/shop/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.799330 line-bot-sdk-3.0.3/linebot/v3/shop/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/shop/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/shop/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/shop/models/mission_sticker_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/shop/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.803330 line-bot-sdk-3.0.3/linebot/v3/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.803330 line-bot-sdk-3.0.3/linebot/v3/webhooks/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/api/async_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/api/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30118 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30354 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/async_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/async_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.811330 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/account_link_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/action_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/activated_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/all_mentionee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/attached_module_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/audio_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/beacon_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/beacon_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/bot_resumed_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/bot_suspended_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/callback_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/chat_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/deactivated_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/delivery_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/detached_module_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/event_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/file_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/follow_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/group_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/image_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/image_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/join_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/joined_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/leave_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/left_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/link_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/link_things_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/location_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/member_joined_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/member_left_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/mention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/mentionee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/message_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/module_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/module_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/postback_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/postback_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/room_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/scenario_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/scenario_result_things_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/sticker_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/text_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/things_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/things_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/unfollow_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/unlink_things_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/unsend_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/unsend_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/user_mentionee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/user_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/video_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/video_play_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/models/video_play_complete_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/v3/webhooks/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/linebot/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-03 07:27:57.819330 line-bot-sdk-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.811330 line-bot-sdk-3.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.815330 line-bot-sdk-3.0.3/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_channel_access_token_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_error_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_get_bot_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_get_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_get_custom_aggregation_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_get_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_get_insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_get_member_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_get_member_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_get_message_quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_get_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_get_room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_get_webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_issue_channel_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_issue_link_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_leave.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_narrowcast_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_revoke_channel_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17746 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_rich_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_rich_menu_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_send_audio_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_send_image_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_send_imagemap_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_send_location_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_send_sticker_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_send_template_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_send_text_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_send_text_message_with_quick_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_send_text_message_with_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_send_text_message_with_statistics_per_aggregation_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_send_video_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_set_webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_test_webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/api/test_validate_message_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.815330 line-bot-sdk-3.0.3/tests/async_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/async_api/test_async_error_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/async_api/test_get_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/async_api/test_get_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.815330 line-bot-sdk-3.0.3/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/models/serialize_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/models/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/models/test_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/models/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/models/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/models/test_flex_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/models/test_imagemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/models/test_send_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/models/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/models/test_text_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/test_aiohttp_async_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.815330 line-bot-sdk-3.0.3/tests/text/
+-rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/text/webhook.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.815330 line-bot-sdk-3.0.3/tests/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/v3/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39963 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/v3/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:27:57.815330 line-bot-sdk-3.0.3/tests/v3/text/
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-03 07:27:47.000000 line-bot-sdk-3.0.3/tests/v3/text/webhook.json
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-03 07:27:48.000000 line-bot-sdk-3.0.3/tox.ini
```

### Comparing `line-bot-sdk-3.0.2/LICENSE` & `line-bot-sdk-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/PKG-INFO` & `line-bot-sdk-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: line-bot-sdk
-Version: 3.0.2
+Version: 3.0.3
 Summary: LINE Messaging API SDK for Python
 Home-page: https://github.com/line/line-bot-sdk-python
 Author: RyosukeHasebe
 Author-email: hsb.1014@gmail.com
 Maintainer: RyosukeHasebe
 Maintainer-email: hsb.1014@gmail.com
 License: Apache License 2.0
```

### Comparing `line-bot-sdk-3.0.2/README.rst` & `line-bot-sdk-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/docs/Makefile` & `line-bot-sdk-3.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/docs/source/conf.py` & `line-bot-sdk-3.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/docs/source/linebot.models.rst` & `line-bot-sdk-3.0.3/docs/source/linebot.models.rst`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/line_bot_sdk.egg-info/PKG-INFO` & `line-bot-sdk-3.0.3/line_bot_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: line-bot-sdk
-Version: 3.0.2
+Version: 3.0.3
 Summary: LINE Messaging API SDK for Python
 Home-page: https://github.com/line/line-bot-sdk-python
 Author: RyosukeHasebe
 Author-email: hsb.1014@gmail.com
 Maintainer: RyosukeHasebe
 Maintainer-email: hsb.1014@gmail.com
 License: Apache License 2.0
```

### Comparing `line-bot-sdk-3.0.2/linebot/__about__.py` & `line-bot-sdk-3.0.3/linebot/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations
 #  under the License.
 
 """Meta data of line-bot-sdk."""
 
 
-__version__ = '3.0.2'
+__version__ = '3.0.3'
 __author__ = 'LINE Corporation'
 __copyright__ = 'Copyright 2016, LINE Corporation'
 __license__ = 'Apache 2.0'
 
 __all__ = (
     '__version__'
 )
```

### Comparing `line-bot-sdk-3.0.2/linebot/__init__.py` & `line-bot-sdk-3.0.3/linebot/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/aiohttp_async_http_client.py` & `line-bot-sdk-3.0.3/linebot/aiohttp_async_http_client.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/api.py` & `line-bot-sdk-3.0.3/linebot/api.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/async_api.py` & `line-bot-sdk-3.0.3/linebot/async_api.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/async_http_client.py` & `line-bot-sdk-3.0.3/linebot/async_http_client.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/deprecations.py` & `line-bot-sdk-3.0.3/linebot/deprecations.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/exceptions.py` & `line-bot-sdk-3.0.3/linebot/exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/http_client.py` & `line-bot-sdk-3.0.3/linebot/http_client.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/__init__.py` & `line-bot-sdk-3.0.3/linebot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/actions.py` & `line-bot-sdk-3.0.3/linebot/models/actions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/background.py` & `line-bot-sdk-3.0.3/linebot/models/background.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/base.py` & `line-bot-sdk-3.0.3/linebot/models/base.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/delivery_context.py` & `line-bot-sdk-3.0.3/linebot/models/delivery_context.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/emojis.py` & `line-bot-sdk-3.0.3/linebot/models/emojis.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/error.py` & `line-bot-sdk-3.0.3/linebot/models/error.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/events.py` & `line-bot-sdk-3.0.3/linebot/models/events.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/filter.py` & `line-bot-sdk-3.0.3/linebot/models/filter.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/flex_message.py` & `line-bot-sdk-3.0.3/linebot/models/flex_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/imagemap.py` & `line-bot-sdk-3.0.3/linebot/models/imagemap.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/insight.py` & `line-bot-sdk-3.0.3/linebot/models/insight.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/limit.py` & `line-bot-sdk-3.0.3/linebot/models/limit.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/mention.py` & `line-bot-sdk-3.0.3/linebot/models/mention.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/mentionee.py` & `line-bot-sdk-3.0.3/linebot/models/mentionee.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/messages.py` & `line-bot-sdk-3.0.3/linebot/models/messages.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/operator.py` & `line-bot-sdk-3.0.3/linebot/models/operator.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/recipient.py` & `line-bot-sdk-3.0.3/linebot/models/recipient.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/responses.py` & `line-bot-sdk-3.0.3/linebot/models/responses.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/rich_menu.py` & `line-bot-sdk-3.0.3/linebot/models/rich_menu.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/send_messages.py` & `line-bot-sdk-3.0.3/linebot/models/send_messages.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/sources.py` & `line-bot-sdk-3.0.3/linebot/models/sources.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/template.py` & `line-bot-sdk-3.0.3/linebot/models/template.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/things.py` & `line-bot-sdk-3.0.3/linebot/models/things.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/unsend.py` & `line-bot-sdk-3.0.3/linebot/models/unsend.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/models/video_play_complete.py` & `line-bot-sdk-3.0.3/linebot/models/video_play_complete.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/utils.py` & `line-bot-sdk-3.0.3/linebot/utils.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/__init__.py` & `line-bot-sdk-3.0.3/linebot/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/audience/__init__.py` & `line-bot-sdk-3.0.3/linebot/v3/audience/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.0.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 
 # import apis into sdk package
 from linebot.v3.audience.api.manage_audience import ManageAudience
 from linebot.v3.audience.api.manage_audience_blob import ManageAudienceBlob
 
 from linebot.v3.audience.api.async_manage_audience import AsyncManageAudience
 from linebot.v3.audience.api.async_manage_audience_blob import AsyncManageAudienceBlob
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/audience/api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/audience/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python/3.0.2'
+        self.user_agent = 'line-bot-sdk-python/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/audience/api_response.py` & `line-bot-sdk-3.0.3/linebot/v3/audience/api_response.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/audience/async_api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/audience/async_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = async_rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python-async/3.0.2'
+        self.user_agent = 'line-bot-sdk-python-async/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/audience/async_rest.py` & `line-bot-sdk-3.0.3/linebot/v3/audience/async_rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/audience/configuration.py` & `line-bot-sdk-3.0.3/linebot/v3/liff/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # coding: utf-8
 
 """
-    LINE Messaging API
+    LIFF server API
 
-    This document describes LINE Messaging API.  # noqa: E501
+    LIFF Server API.  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 1.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
 import http.client as httplib
-from linebot.v3.audience.exceptions import ApiValueError
+from linebot.v3.liff.exceptions import ApiValueError
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
@@ -104,15 +104,15 @@
         """
         self.access_token = access_token
         """Access token
         """
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("linebot.v3.audience")
+        self.logger["package_logger"] = logging.getLogger("linebot.v3.liff")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
@@ -367,16 +367,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.1\n"\
-               "SDK Package Version: 3.0.2".\
+               "Version of the API: 1.0\n"\
+               "SDK Package Version: 3.0.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/audience/exceptions.py` & `line-bot-sdk-3.0.3/linebot/v3/audience/exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/audience/rest.py` & `line-bot-sdk-3.0.3/linebot/v3/audience/rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/exceptions.py` & `line-bot-sdk-3.0.3/linebot/v3/exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/insight/__init__.py` & `line-bot-sdk-3.0.3/linebot/v3/insight/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.0.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 
 # import apis into sdk package
 from linebot.v3.insight.api.insight import Insight
 
 from linebot.v3.insight.api.async_insight import AsyncInsight
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/insight/api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/insight/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python/3.0.2'
+        self.user_agent = 'line-bot-sdk-python/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/insight/api_response.py` & `line-bot-sdk-3.0.3/linebot/v3/insight/api_response.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/insight/async_api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/insight/async_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = async_rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python-async/3.0.2'
+        self.user_agent = 'line-bot-sdk-python-async/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/insight/async_rest.py` & `line-bot-sdk-3.0.3/linebot/v3/insight/async_rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/insight/configuration.py` & `line-bot-sdk-3.0.3/linebot/v3/insight/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.0.1\n"\
-               "SDK Package Version: 3.0.2".\
+               "SDK Package Version: 3.0.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/insight/exceptions.py` & `line-bot-sdk-3.0.3/linebot/v3/insight/exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/insight/rest.py` & `line-bot-sdk-3.0.3/linebot/v3/insight/rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/liff/__init__.py` & `line-bot-sdk-3.0.3/linebot/v3/liff/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 1.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 
 # import apis into sdk package
 from linebot.v3.liff.api.liff import Liff
 
 from linebot.v3.liff.api.async_liff import AsyncLiff
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/liff/api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/liff/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python/3.0.2'
+        self.user_agent = 'line-bot-sdk-python/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/liff/api_response.py` & `line-bot-sdk-3.0.3/linebot/v3/liff/api_response.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/liff/async_api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/liff/async_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = async_rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python-async/3.0.2'
+        self.user_agent = 'line-bot-sdk-python-async/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/liff/async_rest.py` & `line-bot-sdk-3.0.3/linebot/v3/liff/async_rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/liff/configuration.py` & `line-bot-sdk-3.0.3/linebot/v3/shop/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # coding: utf-8
 
 """
-    LIFF server API
+    Mission Stickers API
 
-    LIFF Server API.  # noqa: E501
+    This document describes LINE Mission Stickers API.  # noqa: E501
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 0.0.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
 import http.client as httplib
-from linebot.v3.liff.exceptions import ApiValueError
+from linebot.v3.shop.exceptions import ApiValueError
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
@@ -104,15 +104,15 @@
         """
         self.access_token = access_token
         """Access token
         """
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("linebot.v3.liff")
+        self.logger["package_logger"] = logging.getLogger("linebot.v3.shop")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
@@ -367,16 +367,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0\n"\
-               "SDK Package Version: 3.0.2".\
+               "Version of the API: 0.0.1\n"\
+               "SDK Package Version: 3.0.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/liff/exceptions.py` & `line-bot-sdk-3.0.3/linebot/v3/liff/exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/liff/rest.py` & `line-bot-sdk-3.0.3/linebot/v3/liff/rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/messaging/__init__.py` & `line-bot-sdk-3.0.3/linebot/v3/messaging/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.0.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 
 # import apis into sdk package
 from linebot.v3.messaging.api.messaging_api import MessagingApi
 from linebot.v3.messaging.api.messaging_api_blob import MessagingApiBlob
 
 from linebot.v3.messaging.api.async_messaging_api import AsyncMessagingApi
 from linebot.v3.messaging.api.async_messaging_api_blob import AsyncMessagingApiBlob
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/messaging/api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/messaging/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python/3.0.2'
+        self.user_agent = 'line-bot-sdk-python/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/messaging/api_response.py` & `line-bot-sdk-3.0.3/linebot/v3/messaging/api_response.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/messaging/async_api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/messaging/async_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = async_rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python-async/3.0.2'
+        self.user_agent = 'line-bot-sdk-python-async/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/messaging/async_rest.py` & `line-bot-sdk-3.0.3/linebot/v3/messaging/async_rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/messaging/configuration.py` & `line-bot-sdk-3.0.3/linebot/v3/messaging/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.0.1\n"\
-               "SDK Package Version: 3.0.2".\
+               "SDK Package Version: 3.0.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/messaging/exceptions.py` & `line-bot-sdk-3.0.3/linebot/v3/messaging/exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/messaging/rest.py` & `line-bot-sdk-3.0.3/linebot/v3/messaging/rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/models/__init__.py` & `line-bot-sdk-3.0.3/linebot/v3/models/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/models/events.py` & `line-bot-sdk-3.0.3/linebot/v3/models/events.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/module/__init__.py` & `line-bot-sdk-3.0.3/linebot/v3/module/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.0.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 
 # import apis into sdk package
 from linebot.v3.module.api.line_module import LineModule
 
 from linebot.v3.module.api.async_line_module import AsyncLineModule
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/module/api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/module/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python/3.0.2'
+        self.user_agent = 'line-bot-sdk-python/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/module/api_response.py` & `line-bot-sdk-3.0.3/linebot/v3/module/api_response.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/module/async_api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/module/async_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = async_rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python-async/3.0.2'
+        self.user_agent = 'line-bot-sdk-python-async/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/module/async_rest.py` & `line-bot-sdk-3.0.3/linebot/v3/module/async_rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/module/configuration.py` & `line-bot-sdk-3.0.3/linebot/v3/module/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.0.1\n"\
-               "SDK Package Version: 3.0.2".\
+               "SDK Package Version: 3.0.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/module/exceptions.py` & `line-bot-sdk-3.0.3/linebot/v3/module/exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/module/rest.py` & `line-bot-sdk-3.0.3/linebot/v3/module/rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/moduleattach/__init__.py` & `line-bot-sdk-3.0.3/linebot/v3/moduleattach/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.0.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 
 # import apis into sdk package
 from linebot.v3.moduleattach.api.line_module_attach import LineModuleAttach
 
 from linebot.v3.moduleattach.api.async_line_module_attach import AsyncLineModuleAttach
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/moduleattach/api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/moduleattach/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python/3.0.2'
+        self.user_agent = 'line-bot-sdk-python/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/moduleattach/api_response.py` & `line-bot-sdk-3.0.3/linebot/v3/moduleattach/api_response.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/moduleattach/async_api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/moduleattach/async_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = async_rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python-async/3.0.2'
+        self.user_agent = 'line-bot-sdk-python-async/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/moduleattach/async_rest.py` & `line-bot-sdk-3.0.3/linebot/v3/moduleattach/async_rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/moduleattach/configuration.py` & `line-bot-sdk-3.0.3/linebot/v3/moduleattach/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.0.1\n"\
-               "SDK Package Version: 3.0.2".\
+               "SDK Package Version: 3.0.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/moduleattach/exceptions.py` & `line-bot-sdk-3.0.3/linebot/v3/moduleattach/exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/moduleattach/rest.py` & `line-bot-sdk-3.0.3/linebot/v3/moduleattach/rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/oauth/__init__.py` & `line-bot-sdk-3.0.3/linebot/v3/oauth/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.0.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 
 # import apis into sdk package
 from linebot.v3.oauth.api.channel_access_token import ChannelAccessToken
 
 from linebot.v3.oauth.api.async_channel_access_token import AsyncChannelAccessToken
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/oauth/api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/oauth/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python/3.0.2'
+        self.user_agent = 'line-bot-sdk-python/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/oauth/api_response.py` & `line-bot-sdk-3.0.3/linebot/v3/oauth/api_response.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/oauth/async_api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/oauth/async_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = async_rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python-async/3.0.2'
+        self.user_agent = 'line-bot-sdk-python-async/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/oauth/async_rest.py` & `line-bot-sdk-3.0.3/linebot/v3/oauth/async_rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/oauth/configuration.py` & `line-bot-sdk-3.0.3/linebot/v3/oauth/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.0.1\n"\
-               "SDK Package Version: 3.0.2".\
+               "SDK Package Version: 3.0.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/oauth/exceptions.py` & `line-bot-sdk-3.0.3/linebot/v3/oauth/exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/oauth/rest.py` & `line-bot-sdk-3.0.3/linebot/v3/oauth/rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/shop/__init__.py` & `line-bot-sdk-3.0.3/linebot/v3/shop/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.0.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 
 # import apis into sdk package
 from linebot.v3.shop.api.shop import Shop
 
 from linebot.v3.shop.api.async_shop import AsyncShop
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/shop/api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/shop/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python/3.0.2'
+        self.user_agent = 'line-bot-sdk-python/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/shop/api_response.py` & `line-bot-sdk-3.0.3/linebot/v3/shop/api_response.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/shop/async_api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/shop/async_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.rest_client = async_rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.default_headers['Authorization'] = 'Bearer ' + configuration.access_token
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'line-bot-sdk-python-async/3.0.2'
+        self.user_agent = 'line-bot-sdk-python-async/3.0.3'
         self.client_side_validation = configuration.client_side_validation
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/shop/async_rest.py` & `line-bot-sdk-3.0.3/linebot/v3/shop/async_rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/shop/configuration.py` & `line-bot-sdk-3.0.3/linebot/v3/audience/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Mission Stickers API
+    LINE Messaging API
 
-    This document describes LINE Mission Stickers API.  # noqa: E501
+    This document describes LINE Messaging API.  # noqa: E501
 
     The version of the OpenAPI document: 0.0.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
@@ -15,15 +15,15 @@
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
 import http.client as httplib
-from linebot.v3.shop.exceptions import ApiValueError
+from linebot.v3.audience.exceptions import ApiValueError
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
@@ -104,15 +104,15 @@
         """
         self.access_token = access_token
         """Access token
         """
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("linebot.v3.shop")
+        self.logger["package_logger"] = logging.getLogger("linebot.v3.audience")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
@@ -368,15 +368,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.0.1\n"\
-               "SDK Package Version: 3.0.2".\
+               "SDK Package Version: 3.0.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `line-bot-sdk-3.0.2/linebot/v3/shop/exceptions.py` & `line-bot-sdk-3.0.3/linebot/v3/shop/exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/shop/rest.py` & `line-bot-sdk-3.0.3/linebot/v3/shop/rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/utils.py` & `line-bot-sdk-3.0.3/linebot/v3/utils.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/webhook.py` & `line-bot-sdk-3.0.3/linebot/v3/webhook.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/webhooks/__init__.py` & `line-bot-sdk-3.0.3/linebot/v3/webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/webhooks/api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/webhooks/api_client.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/webhooks/api_response.py` & `line-bot-sdk-3.0.3/linebot/v3/webhooks/api_response.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/webhooks/async_api_client.py` & `line-bot-sdk-3.0.3/linebot/v3/webhooks/async_api_client.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/webhooks/async_rest.py` & `line-bot-sdk-3.0.3/linebot/v3/webhooks/async_rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/webhooks/configuration.py` & `line-bot-sdk-3.0.3/linebot/v3/webhooks/configuration.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/webhooks/exceptions.py` & `line-bot-sdk-3.0.3/linebot/v3/webhooks/exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/v3/webhooks/rest.py` & `line-bot-sdk-3.0.3/linebot/v3/webhooks/rest.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/linebot/webhook.py` & `line-bot-sdk-3.0.3/linebot/webhook.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/setup.py` & `line-bot-sdk-3.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 import os
 import re
 import sys
 import subprocess
 
-from setuptools import setup, Command
+from setuptools import setup, Command, find_packages
 from setuptools.command.test import test as TestCommand
 
 __version__ = ''
 with open('linebot/__about__.py', 'r') as fd:
     reg = re.compile(r'__version__ = [\'"]([^\'"]*)[\'"]')
     for line in fd:
         m = reg.match(line)
@@ -183,29 +183,15 @@
     author_email="hsb.1014@gmail.com",
     maintainer="RyosukeHasebe",
     maintainer_email="hsb.1014@gmail.com",
     url="https://github.com/line/line-bot-sdk-python",
     description="LINE Messaging API SDK for Python",
     long_description=long_description,
     license='Apache License 2.0',
-    packages=[
-        "linebot",
-        "linebot.models",
-        "linebot.v3",
-        "linebot.v3.audience",
-        "linebot.v3.insight",
-        "linebot.v3.liff",
-        "linebot.v3.messaging",
-        "linebot.v3.models",
-        "linebot.v3.module",
-        "linebot.v3.moduleattach",
-        "linebot.v3.oauth",
-        "linebot.v3.shop",
-        "linebot.v3.webhooks",
-    ],
+    packages=find_packages(include=["linebot*"]),
     python_requires=">=3.7.0",
     install_requires=_requirements(),
     tests_require=_requirements_test(),
     cmdclass={
         'test': PyTest,
         'codegen': CodegenCommand
     },
```

### Comparing `line-bot-sdk-3.0.2/tests/__init__.py` & `line-bot-sdk-3.0.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/__init__.py` & `line-bot-sdk-3.0.3/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_channel_access_token_v2_1.py` & `line-bot-sdk-3.0.3/tests/api/test_channel_access_token_v2_1.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_error_handle.py` & `line-bot-sdk-3.0.3/tests/api/test_error_handle.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_get_bot_info.py` & `line-bot-sdk-3.0.3/tests/api/test_get_bot_info.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_get_content.py` & `line-bot-sdk-3.0.3/tests/api/test_get_content.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_get_custom_aggregation_units.py` & `line-bot-sdk-3.0.3/tests/api/test_get_custom_aggregation_units.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_get_delivery.py` & `line-bot-sdk-3.0.3/tests/api/test_get_delivery.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_get_group.py` & `line-bot-sdk-3.0.3/tests/api/test_get_group.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_get_insight.py` & `line-bot-sdk-3.0.3/tests/api/test_get_insight.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_get_member_ids.py` & `line-bot-sdk-3.0.3/tests/api/test_get_member_ids.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_get_member_profile.py` & `line-bot-sdk-3.0.3/tests/api/test_get_member_profile.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_get_message_quota.py` & `line-bot-sdk-3.0.3/tests/api/test_get_message_quota.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_get_profile.py` & `line-bot-sdk-3.0.3/tests/api/test_get_profile.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_get_room.py` & `line-bot-sdk-3.0.3/tests/api/test_get_room.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_get_webhook_endpoint.py` & `line-bot-sdk-3.0.3/tests/api/test_get_webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_issue_channel_token.py` & `line-bot-sdk-3.0.3/tests/api/test_issue_channel_token.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_issue_link_token.py` & `line-bot-sdk-3.0.3/tests/api/test_issue_link_token.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_leave.py` & `line-bot-sdk-3.0.3/tests/api/test_leave.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_narrowcast_message.py` & `line-bot-sdk-3.0.3/tests/api/test_narrowcast_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_revoke_channel_token.py` & `line-bot-sdk-3.0.3/tests/api/test_revoke_channel_token.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_rich_menu.py` & `line-bot-sdk-3.0.3/tests/api/test_rich_menu.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_rich_menu_alias.py` & `line-bot-sdk-3.0.3/tests/api/test_rich_menu_alias.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_send_audio_message.py` & `line-bot-sdk-3.0.3/tests/api/test_send_audio_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_send_image_message.py` & `line-bot-sdk-3.0.3/tests/api/test_send_image_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_send_imagemap_message.py` & `line-bot-sdk-3.0.3/tests/api/test_send_imagemap_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_send_location_message.py` & `line-bot-sdk-3.0.3/tests/api/test_send_location_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_send_sticker_message.py` & `line-bot-sdk-3.0.3/tests/api/test_send_sticker_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_send_template_message.py` & `line-bot-sdk-3.0.3/tests/api/test_send_template_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_send_text_message.py` & `line-bot-sdk-3.0.3/tests/api/test_send_text_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_send_text_message_with_quick_reply.py` & `line-bot-sdk-3.0.3/tests/api/test_send_text_message_with_quick_reply.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_send_text_message_with_sender.py` & `line-bot-sdk-3.0.3/tests/api/test_send_text_message_with_sender.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_send_text_message_with_statistics_per_aggregation_unit.py` & `line-bot-sdk-3.0.3/tests/api/test_send_text_message_with_statistics_per_aggregation_unit.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_send_video_message.py` & `line-bot-sdk-3.0.3/tests/api/test_send_video_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_set_webhook_endpoint.py` & `line-bot-sdk-3.0.3/tests/api/test_set_webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_test_webhook_endpoint.py` & `line-bot-sdk-3.0.3/tests/api/test_test_webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/api/test_validate_message_objects.py` & `line-bot-sdk-3.0.3/tests/api/test_validate_message_objects.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/async_api/test_async_error_handle.py` & `line-bot-sdk-3.0.3/tests/async_api/test_async_error_handle.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/async_api/test_get_message_content.py` & `line-bot-sdk-3.0.3/tests/async_api/test_get_message_content.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/async_api/test_get_profile.py` & `line-bot-sdk-3.0.3/tests/async_api/test_get_profile.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/models/__init__.py` & `line-bot-sdk-3.0.3/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/models/serialize_test_case.py` & `line-bot-sdk-3.0.3/tests/models/serialize_test_case.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/models/test_actions.py` & `line-bot-sdk-3.0.3/tests/models/test_actions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/models/test_background.py` & `line-bot-sdk-3.0.3/tests/models/test_background.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/models/test_base.py` & `line-bot-sdk-3.0.3/tests/models/test_base.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/models/test_filter.py` & `line-bot-sdk-3.0.3/tests/models/test_filter.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/models/test_flex_message.py` & `line-bot-sdk-3.0.3/tests/models/test_flex_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/models/test_imagemap.py` & `line-bot-sdk-3.0.3/tests/models/test_imagemap.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/models/test_send_messages.py` & `line-bot-sdk-3.0.3/tests/models/test_send_messages.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/models/test_template.py` & `line-bot-sdk-3.0.3/tests/models/test_template.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/models/test_text_message.py` & `line-bot-sdk-3.0.3/tests/models/test_text_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/test_aiohttp_async_http_client.py` & `line-bot-sdk-3.0.3/tests/test_aiohttp_async_http_client.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/test_exceptions.py` & `line-bot-sdk-3.0.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/test_utils.py` & `line-bot-sdk-3.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/test_webhook.py` & `line-bot-sdk-3.0.3/tests/test_webhook.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/text/webhook.json` & `line-bot-sdk-3.0.3/tests/text/webhook.json`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/v3/test_utils.py` & `line-bot-sdk-3.0.3/tests/v3/test_utils.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/v3/test_webhook.py` & `line-bot-sdk-3.0.3/tests/v3/test_webhook.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tests/v3/text/webhook.json` & `line-bot-sdk-3.0.3/tests/v3/text/webhook.json`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-3.0.2/tox.ini` & `line-bot-sdk-3.0.3/tox.ini`

 * *Files identical despite different names*

