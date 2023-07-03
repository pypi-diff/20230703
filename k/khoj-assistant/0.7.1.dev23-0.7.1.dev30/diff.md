# Comparing `tmp/khoj_assistant-0.7.1.dev23.tar.gz` & `tmp/khoj_assistant-0.7.1.dev30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jul  3 00:48:29 2023, max compression
+gzip compressed data, last modified: Mon Jul  3 07:16:51 2023, max compression
```

## Comparing `khoj_assistant-0.7.1.dev23.tar` & `khoj_assistant-0.7.1.dev30.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/__init__.py
--rw-r--r--   0        0        0    10673 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/configure.py
--rw-r--r--   0        0        0     5379 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1395 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     3532 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    14414 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0     6212 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     6990 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     6799 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    18662 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3644 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1813 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0   205167 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     7946 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6056 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4065 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13481 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7454 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5193 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    17216 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     4394 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7560 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11381 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11054 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2040 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2385 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2500 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6852 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4136 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1066 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/LICENSE
--rw-r--r--   0        0        0    23342 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/README.md
--rw-r--r--   0        0        0     2790 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/pyproject.toml
--rw-r--r--   0        0        0    25705 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10673 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/configure.py
+-rw-r--r--   0        0        0     5379 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     3910 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    14414 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    13551 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6930 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     6739 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    18662 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3583 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1813 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0      549 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0   205167 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     7946 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6056 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4065 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13481 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7454 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5193 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    18352 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     4646 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7560 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11054 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2040 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2385 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2500 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6852 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4136 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/LICENSE
+-rw-r--r--   0        0        0    23342 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/README.md
+-rw-r--r--   0        0        0     2790 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/pyproject.toml
+-rw-r--r--   0        0        0    25705 2023-07-03 07:16:51.000000 khoj_assistant-0.7.1.dev30/PKG-INFO
```

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/configure.py` & `khoj_assistant-0.7.1.dev30/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/main.py` & `khoj_assistant-0.7.1.dev30/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/404.html` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/base_config.html`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         }
         .card {
             display: grid;
             grid-template-rows: repeat(3, 1fr);
             gap: 8px;
             padding: 24px 16px;
             width: 320px;
-            height: 160px;
+            height: 180px;
             background: white;
             border: 1px solid rgb(229, 229, 229);
             border-radius: 4px;
             box-shadow: 0px 1px 3px 0px rgba(0,0,0,0.1),0px 1px 2px -1px rgba(0,0,0,0.1);
             overflow: hidden;
         }
         .card-title-row {
@@ -110,14 +110,30 @@
             padding: 15px 32px;
             text-align: center;
             text-decoration: none;
             display: inline-block;
             font-size: 16px;
         }
 
+        button.card-button {
+            color: rgb(255, 136, 136);
+            background: transparent;
+            font-size: 16px;
+            cursor: pointer;
+            margin: 0;
+            padding: 0;
+            height: 32px;
+            text-align: right;
+            text-align: left;
+        }
+
+        img.configured-icon {
+            max-width: 16px;
+        }
+
         @media screen and (max-width: 600px) {
             .section-cards {
                 grid-template-columns: 1fr;
             }
         }
     </style>
 </html>
```

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/chat.html` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/content_type_github_input.html`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,15 @@
                             class="remove-repo-button"
                             onclick="remove_repo({{loop.index}})"
                             id="remove-repo-button-{{loop.index}}">Remove Repository</button>
                 </div>
                 {% endfor %}
             </div>
             <button type="button" id="add-repository-button">Add Repository</button>
-            <h4>You probably don't need to edit these.</h4>
-
-            <table>
+            <table style="display: none;" >
                 <tr>
                     <td>
                         <label for="compressed-jsonl">Compressed JSONL (Output)</label>
                     </td>
                     <td>
                         <input type="text" id="compressed-jsonl" name="compressed-jsonl" value="{{ current_config['compressed_jsonl'] }}">
                     </td>
@@ -156,15 +154,15 @@
                 "compressed_jsonl": compressed_jsonl,
                 "embeddings_file": embeddings_file,
             })
         })
         .then(response => response.json())
         .then(data => {
             if (data["status"] == "ok") {
-                document.getElementById("success").innerHTML = "✅ Successfully updated. Click Configure on your <a href='/config'>settings page</a> to complete your Khoj setup.";
+                document.getElementById("success").innerHTML = "✅ Successfully updated. Go to your <a href='/config'>settings page</a> to complete setup.";
                 document.getElementById("success").style.display = "block";
             } else {
                 document.getElementById("success").innerHTML = "⚠️ Failed to update settings.";
                 document.getElementById("success").style.display = "block";
             }
         })
     });
```

#### html2text {}

```diff
@@ -3,12 +3,11 @@
 Personal Access Token [{{ current_config['pat_token'] }}]
 *** Repositories ***
 {% for repo in current_config['repos'] %}
 Repository Owner [{{ repo.owner }}    ] Repository Name [{{ repo.name}}      ]
 Repository Branch [{{ repo.branch }}   ] Remove Repository
 {% endfor %}
 Add Repository
-*** You probably don't need to edit these. ***
 Compressed JSONL (Output) [{{ current_config['compressed_jsonl'] }}]
 Embeddings File (Output)  [{{ current_config['embeddings_file'] }}]
 Save
  {% endblock %}
```

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/content_type_input.html`

 * *Files 3% similar despite different names*

```diff
@@ -40,17 +40,15 @@
                     </td>
                     <td>
                         <button type="button" id="input-filter-button">Add</button>
                     </td>
                 </tr>
             </table>
 
-            <h4>You probably don't need to edit these.</h4>
-
-            <table>
+            <table style="display: none;" >
                 <tr>
                     <td>
                         <label for="compressed-jsonl">Compressed JSONL (Output)</label>
                     </td>
                     <td>
                         <input type="text" id="compressed-jsonl" name="compressed-jsonl" value="{{ current_config['compressed_jsonl'] }}">
                     </td>
@@ -145,15 +143,15 @@
                 "embeddings_file": embeddings_file,
                 "index_heading_entries": index_heading_entries
             })
         })
         .then(response => response.json())
         .then(data => {
             if (data["status"] == "ok") {
-                document.getElementById("success").innerHTML = "✅ Successfully updated. Click Configure on your <a href='/config'>settings page</a> to complete your Khoj setup.";
+                document.getElementById("success").innerHTML = "✅ Successfully updated. Go to your <a href='/config'>settings page</a> to complete setup.";
                 document.getElementById("success").style.display = "block";
             } else {
                 document.getElementById("success").innerHTML = "⚠️ Failed to update settings.";
                 document.getElementById("success").style.display = "block";
             }
         })
     });
```

#### html2text {}

```diff
@@ -4,13 +4,12 @@
 Input Files  ] {% else %} {% for input_file in current_config              Add
              ['input_files'] %} [{{ input_file }}    ] {% endfor %} {%
              endif %}
              {% if current_config['input_filter'] is none %} [input-filter
 Input Filter ] {% else %} {% for input_filter in current_config            Add
              ['input_filter'] %} [{{ input_filter }}  ] {% endfor %} {%
              endif %}
-*** You probably don't need to edit these. ***
 Compressed JSONL (Output) [{{ current_config['compressed_jsonl'] }}]
 Embeddings File (Output)  [{{ current_config['embeddings_file'] }}]
 Index Heading Entries     [{{ current_config['index_heading_entries'] }}]
 Save
  {% endblock %}
```

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/index.html` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/processor_conversation_input.html`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,16 @@
                         <label for="openai-api-key">OpenAI API key</label>
                     </td>
                     <td>
                         <input type="text" id="openai-api-key" name="openai-api-key" value="{{ current_config['openai_api_key'] }}">
                     </td>
                 </tr>
             </table>
-
-            <h4>You probably don't need to edit these.</h4>
-
-            <table>
-                <tr>
+            <table >
+                <tr style="display: none;">
                     <td>
                         <label for="conversation-logfile">Conversation Logfile</label>
                     </td>
                     <td>
                         <input type="text" id="conversation-logfile" name="conversation-logfile" value="{{ current_config['conversation_logfile'] }}">
                     </td>
                 </tr>
@@ -74,15 +71,15 @@
                 "model": model,
                 "chat_model": chat_model
             })
         })
         .then(response => response.json())
         .then(data => {
             if (data["status"] == "ok") {
-                document.getElementById("success").innerHTML = "✅ Successfully updated. Click Configure on your <a href='/config'>settings page</a> to complete your Khoj setup.";
+                document.getElementById("success").innerHTML = "✅ Successfully updated. Go to your <a href='/config'>settings page</a> to complete setup.";
                 document.getElementById("success").style.display = "block";
             } else {
                 document.getElementById("success").innerHTML = "⚠️ Failed to update settings.";
                 document.getElementById("success").style.display = "block";
             }
         })
     });
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
 {% extends "base_config.html" %} {% block content %}
 ***** [Chat] Chat *****
 OpenAI API key [{{ current_config['openai_api_key'] }}]
-*** You probably don't need to edit these. ***
 Conversation Logfile [{{ current_config['conversation_logfile'] }}]
 Model                [{{ current_config['model'] }}]
 Chat Model           [{{ current_config['chat_model'] }}]
 Save
  {% endblock %}
```

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.7.1.dev30/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.7.1.dev30/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.7.1.dev30/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.7.1.dev30/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.7.1.dev30/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.7.1.dev30/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.7.1.dev30/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.7.1.dev30/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.7.1.dev30/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.7.1.dev30/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.7.1.dev30/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/routers/api.py` & `khoj_assistant-0.7.1.dev30/src/khoj/routers/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         state.config = updated_config
         with open(state.config_file, "w") as outfile:
             yaml.dump(yaml.safe_load(state.config.json(by_alias=True)), outfile)
             outfile.close()
         return state.config
 
     @api.post("/config/data/content_type/github", status_code=200)
-    async def set_content_config_github_data(updated_config: GithubContentConfig):
+    async def set_content_config_github_data(updated_config: Union[GithubContentConfig, None]):
         if not state.config:
             state.config = FullConfig()
             state.config.search_type = SearchConfig.parse_obj(constants.default_config["search-type"])
 
         if not state.config.content_type:
             state.config.content_type = ContentConfig(**{"github": updated_config})
         else:
@@ -66,16 +66,43 @@
 
         try:
             save_config_to_file_updated_state()
             return {"status": "ok"}
         except Exception as e:
             return {"status": "error", "message": str(e)}
 
+    @api.post("/delete/config/data/content_type/{content_type}", status_code=200)
+    async def remove_content_config_data(content_type: str):
+        if not state.config or not state.config.content_type:
+            return {"status": "ok"}
+
+        if state.config.content_type:
+            state.config.content_type[content_type] = None
+
+        try:
+            save_config_to_file_updated_state()
+            return {"status": "ok"}
+        except Exception as e:
+            return {"status": "error", "message": str(e)}
+
+    @api.post("/delete/config/data/processor/conversation", status_code=200)
+    async def remove_processor_conversation_config_data():
+        if not state.config or not state.config.processor or not state.config.processor.conversation:
+            return {"status": "ok"}
+
+        state.config.processor.conversation = None
+
+        try:
+            save_config_to_file_updated_state()
+            return {"status": "ok"}
+        except Exception as e:
+            return {"status": "error", "message": str(e)}
+
     @api.post("/config/data/content_type/{content_type}", status_code=200)
-    async def set_content_config_data(content_type: str, updated_config: TextContentConfig):
+    async def set_content_config_data(content_type: str, updated_config: Union[TextContentConfig, None]):
         if not state.config:
             state.config = FullConfig()
             state.config.search_type = SearchConfig.parse_obj(constants.default_config["search-type"])
 
         if not state.config.content_type:
             state.config.content_type = ContentConfig(**{content_type: updated_config})
         else:
@@ -84,15 +111,15 @@
         try:
             save_config_to_file_updated_state()
             return {"status": "ok"}
         except Exception as e:
             return {"status": "error", "message": str(e)}
 
     @api.post("/config/data/processor/conversation", status_code=200)
-    async def set_processor_conversation_config_data(updated_config: ConversationProcessorConfig):
+    async def set_processor_conversation_config_data(updated_config: Union[ConversationProcessorConfig, None]):
         if not state.config:
             state.config = FullConfig()
             state.config.search_type = SearchConfig.parse_obj(constants.default_config["search-type"])
         state.config.processor = ProcessorConfig(conversation=updated_config)
         try:
             save_config_to_file_updated_state()
             return {"status": "ok"}
@@ -338,15 +365,16 @@
     except ValueError as e:
         logger.error(e)
         raise HTTPException(status_code=500, detail=str(e))
     else:
         logger.info("📬 Search index updated via API")
 
     try:
-        state.processor_config = configure_processor(state.config.processor)
+        if state.config and state.config.processor:
+            state.processor_config = configure_processor(state.config.processor)
     except ValueError as e:
         logger.error(e)
         raise HTTPException(status_code=500, detail=str(e))
     else:
         logger.info("📬 Processor reconfigured via API")
 
     user_state = {
```

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/routers/api_beta.py` & `khoj_assistant-0.7.1.dev30/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/routers/web_client.py` & `khoj_assistant-0.7.1.dev30/src/khoj/routers/web_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # External Packages
 from fastapi import APIRouter
 from fastapi import Request
 from fastapi.responses import HTMLResponse, FileResponse
 from fastapi.templating import Jinja2Templates
-from khoj.utils.rawconfig import TextContentConfig, ConversationProcessorConfig
+from khoj.utils.rawconfig import TextContentConfig, ConversationProcessorConfig, FullConfig
 
 # Internal Packages
 from khoj.utils import constants, state
 
-import logging
 import json
 
 
 # Initialize Router
 web_client = APIRouter()
 templates = Jinja2Templates(directory=constants.web_directory)
 
@@ -30,15 +29,21 @@
     return templates.TemplateResponse("chat.html", context={"request": request, "demo": state.demo})
 
 
 if not state.demo:
 
     @web_client.get("/config", response_class=HTMLResponse)
     def config_page(request: Request):
-        return templates.TemplateResponse("config.html", context={"request": request})
+        default_full_config = FullConfig(
+            content_type=None,
+            search_type=None,
+            processor=None,
+        )
+        current_config = state.config or json.loads(default_full_config.json())
+        return templates.TemplateResponse("config.html", context={"request": request, "current_config": current_config})
 
     @web_client.get("/config/content_type/github", response_class=HTMLResponse)
     def github_config_page(request: Request):
         default_copy = constants.default_config.copy()
         default_github = default_copy["content-type"]["github"]  # type: ignore
 
         default_config = TextContentConfig(
```

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.7.1.dev30/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.7.1.dev30/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.7.1.dev30/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.7.1.dev30/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/search_type/image_search.py` & `khoj_assistant-0.7.1.dev30/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/search_type/text_search.py` & `khoj_assistant-0.7.1.dev30/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/utils/cli.py` & `khoj_assistant-0.7.1.dev30/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/utils/config.py` & `khoj_assistant-0.7.1.dev30/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/utils/constants.py` & `khoj_assistant-0.7.1.dev30/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/utils/helpers.py` & `khoj_assistant-0.7.1.dev30/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/utils/jsonl.py` & `khoj_assistant-0.7.1.dev30/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/utils/models.py` & `khoj_assistant-0.7.1.dev30/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.7.1.dev30/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/utils/state.py` & `khoj_assistant-0.7.1.dev30/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/src/khoj/utils/yaml.py` & `khoj_assistant-0.7.1.dev30/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/.gitignore` & `khoj_assistant-0.7.1.dev30/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/LICENSE` & `khoj_assistant-0.7.1.dev30/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/README.md` & `khoj_assistant-0.7.1.dev30/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/pyproject.toml` & `khoj_assistant-0.7.1.dev30/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev23/PKG-INFO` & `khoj_assistant-0.7.1.dev30/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.7.1.dev23
+Version: 0.7.1.dev30
 Summary: An AI personal assistant for your Digital Brain
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

