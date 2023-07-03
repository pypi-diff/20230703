# Comparing `tmp/khoj_assistant-0.7.1.dev15.tar.gz` & `tmp/khoj_assistant-0.7.1.dev23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Jul  2 23:09:07 2023, max compression
+gzip compressed data, last modified: Mon Jul  3 00:48:29 2023, max compression
```

## Comparing `khoj_assistant-0.7.1.dev15.tar` & `khoj_assistant-0.7.1.dev23.tar`

### file list

```diff
@@ -1,78 +1,76 @@
--rw-r--r--   0        0        0        0 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/__init__.py
--rw-r--r--   0        0        0    11900 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/configure.py
--rw-r--r--   0        0        0     5379 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1395 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     3532 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    14414 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0     6212 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     6990 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     6799 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    19296 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3644 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1813 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0   205167 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     7946 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6056 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13481 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5708 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7454 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5193 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    18314 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     4394 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7560 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11381 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11054 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2040 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2510 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2995 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6852 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4215 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1066 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/LICENSE
--rw-r--r--   0        0        0    23398 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/README.md
--rw-r--r--   0        0        0     2807 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/pyproject.toml
--rw-r--r--   0        0        0    25771 2023-07-02 23:09:07.000000 khoj_assistant-0.7.1.dev15/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10673 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/configure.py
+-rw-r--r--   0        0        0     5379 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     3532 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    14414 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0     6212 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6990 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     6799 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    18662 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3644 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1813 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0   205167 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     7946 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6056 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4065 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13481 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7454 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5193 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    17216 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     4394 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7560 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11054 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2040 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2385 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2500 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6852 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4136 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/LICENSE
+-rw-r--r--   0        0        0    23342 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/README.md
+-rw-r--r--   0        0        0     2790 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/pyproject.toml
+-rw-r--r--   0        0        0    25705 2023-07-03 00:48:29.000000 khoj_assistant-0.7.1.dev23/PKG-INFO
```

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/configure.py` & `khoj_assistant-0.7.1.dev23/src/khoj/configure.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 # External Packages
 import schedule
 from fastapi.staticfiles import StaticFiles
 
 # Internal Packages
 from khoj.processor.conversation.gpt import summarize
-from khoj.processor.ledger.beancount_to_jsonl import BeancountToJsonl
 from khoj.processor.jsonl.jsonl_to_jsonl import JsonlToJsonl
 from khoj.processor.markdown.markdown_to_jsonl import MarkdownToJsonl
 from khoj.processor.org_mode.org_to_jsonl import OrgToJsonl
 from khoj.processor.pdf.pdf_to_jsonl import PdfToJsonl
 from khoj.processor.github.github_to_jsonl import GithubToJsonl
 from khoj.search_type import image_search, text_search
 from khoj.utils import constants, state
@@ -102,26 +101,14 @@
                 OrgToJsonl,
                 config.content_type.org,
                 search_config=config.search_type.asymmetric,
                 regenerate=regenerate,
                 filters=[DateFilter(), WordFilter(), FileFilter()],
             )
 
-        # Initialize Org Music Search
-        if (t == state.SearchType.Music or t == None) and config.content_type.music and config.search_type.asymmetric:
-            logger.info("🎺 Setting up search for org-music")
-            # Extract Entries, Generate Music Embeddings
-            model.music_search = text_search.setup(
-                OrgToJsonl,
-                config.content_type.music,
-                search_config=config.search_type.asymmetric,
-                regenerate=regenerate,
-                filters=[DateFilter(), WordFilter()],
-            )
-
         # Initialize Markdown Search
         if (
             (t == state.SearchType.Markdown or t == None)
             and config.content_type.markdown
             and config.search_type.asymmetric
         ):
             logger.info("💎 Setting up search for markdown notes")
@@ -130,26 +117,14 @@
                 MarkdownToJsonl,
                 config.content_type.markdown,
                 search_config=config.search_type.asymmetric,
                 regenerate=regenerate,
                 filters=[DateFilter(), WordFilter(), FileFilter()],
             )
 
-        # Initialize Ledger Search
-        if (t == state.SearchType.Ledger or t == None) and config.content_type.ledger and config.search_type.symmetric:
-            logger.info("💸 Setting up search for ledger")
-            # Extract Entries, Generate Ledger Embeddings
-            model.ledger_search = text_search.setup(
-                BeancountToJsonl,
-                config.content_type.ledger,
-                search_config=config.search_type.symmetric,
-                regenerate=regenerate,
-                filters=[DateFilter(), WordFilter(), FileFilter()],
-            )
-
         # Initialize PDF Search
         if (t == state.SearchType.Pdf or t == None) and config.content_type.pdf and config.search_type.asymmetric:
             logger.info("🖨️ Setting up search for pdf")
             # Extract Entries, Generate PDF Embeddings
             model.pdf_search = text_search.setup(
                 PdfToJsonl,
                 config.content_type.pdf,
```

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/main.py` & `khoj_assistant-0.7.1.dev23/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/404.html` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/chat.html` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/config.html` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/index.html` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,14 @@
                 else {
                     rendered = md.render(`${item.entry}`);
                 }
                 return `<div class="results-markdown">` + rendered + `</div>`;
             }).join("\n");
         }
 
-        function render_ledger(query, data) {
-            return data.map(function (item) {
-                return `<div class="results-ledger">` + `<p>${item.entry}</p>` + `</div>`;
-            }).join("\n");
-        }
-
         function render_pdf(query, data) {
             return data.map(function (item) {
                 let compiled_lines = item.additional.compiled.split("\n");
                 let filename = compiled_lines.shift();
                 let text_match = compiled_lines.join("\n")
                 return `<div class="results-pdf">` + `<h2>${filename}</h2>\n<p>${text_match}</p>` + `</div>`;
             }).join("\n");
@@ -84,20 +78,16 @@
 
         function render_results(data, query, type) {
             let results = "";
             if (type === "markdown") {
                 results = render_markdown(query, data);
             } else if (type === "org") {
                 results = render_org(query, data, "org-");
-            } else if (type === "music") {
-                results = render_org(query, data, "music-");
             } else if (type === "image") {
                 results = data.map(render_image).join('');
-            } else if (type === "ledger") {
-                results = render_ledger(query, data);
             } else if (type === "pdf") {
                 results = render_pdf(query, data);
             } else if (type === "github" || type === "all") {
                 results = render_multiple(query, data, type);
             } else {
                 results = data.map((item) => `<div class="results-plugin">` + `<p>${item.entry}</p>` + `</div>`).join("\n")
             }
@@ -358,51 +348,44 @@
             border-radius: 10px;
             border: 1px solid #475569;
         }
         #json {
             white-space: pre-wrap;
         }
         .results-pdf,
-        .results-plugin,
-        .results-ledger {
+        .results-plugin {
             text-align: left;
             white-space: pre-line;
         }
         .results-markdown,
         .results-github {
             text-align: left;
         }
-        .results-music,
         .results-org {
             text-align: left;
             white-space: pre-line;
         }
-        .results-music h3,
         .results-org h3 {
             margin: 20px 0 0 0;
             font-size: larger;
         }
-        span.music-task-status,
         span.org-task-status {
             color: white;
             padding: 3.5px 3.5px 0;
             margin-right: 5px;
             border-radius: 5px;
             background-color: #eab308;
             font-size: medium;
         }
-        span.music-task-status.todo,
         span.org-task-status.todo {
             background-color: #3b82f6
         }
-        span.music-task-status.done,
         span.org-task-status.done {
             background-color: #22c55e;
         }
-        span.music-task-tag,
         span.org-task-tag {
             color: white;
             padding: 3.5px 3.5px 0;
             margin-right: 5px;
             border-radius: 5px;
             border: 1px solid #475569;
             background-color: #ef4444;
```

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.7.1.dev23/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.7.1.dev23/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.7.1.dev23/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.7.1.dev23/src/khoj/processor/conversation/prompts.py`

 * *Files 8% similar despite different names*

```diff
@@ -139,27 +139,19 @@
 
 ## Extract Search Type
 ## --
 search_type = """
 Objective: Extract search type from user query and return information as JSON
 
 Allowed search types are listed below:
-  - search-type=["notes","ledger","image","music", "pdf"]
+  - search-type=["notes", "image", "pdf"]
 
 Some examples are given below for reference:
 Q:What fiction book was I reading last week about AI starship?
 A:{ "search-type": "notes" }
 Q: What did the lease say about early termination
 A: { "search-type": "pdf" }
-Q:Play some calm classical music?
-A:{ "search-type": "music" }
-Q:How much did I spend at Subway for dinner last time?
-A:{ "search-type": "ledger" }
-Q:What was that popular Sri lankan song that Alex had mentioned?
-A:{ "search-type": "music" }
 Q:Can you recommend a movie to watch from my notes?
 A:{ "search-type": "notes" }
-Q:When did I buy Groceries last?
-A:{ "search-type": "ledger" }
 Q:When did I go surfing last?
 A:{ "search-type": "notes" }
 Q:"""
```

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.7.1.dev23/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.7.1.dev23/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.7.1.dev23/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.7.1.dev23/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,133 +1,133 @@
 # Standard Packages
 import glob
-import re
 import logging
+from pathlib import Path
 from typing import List
 
+# External Packages
+from langchain.document_loaders import PyPDFLoader
+
 # Internal Packages
 from khoj.processor.text_to_jsonl import TextToJsonl
 from khoj.utils.helpers import get_absolute_path, is_none_or_empty, timer
-from khoj.utils.constants import empty_escape_sequences
 from khoj.utils.jsonl import dump_jsonl, compress_jsonl_data
 from khoj.utils.rawconfig import Entry
 
 
 logger = logging.getLogger(__name__)
 
 
-class BeancountToJsonl(TextToJsonl):
+class PdfToJsonl(TextToJsonl):
     # Define Functions
     def process(self, previous_entries=None):
         # Extract required fields from config
-        beancount_files, beancount_file_filter, output_file = (
+        pdf_files, pdf_file_filter, output_file = (
             self.config.input_files,
             self.config.input_filter,
             self.config.compressed_jsonl,
         )
 
         # Input Validation
-        if is_none_or_empty(beancount_files) and is_none_or_empty(beancount_file_filter):
-            print("At least one of beancount-files or beancount-file-filter is required to be specified")
+        if is_none_or_empty(pdf_files) and is_none_or_empty(pdf_file_filter):
+            print("At least one of pdf-files or pdf-file-filter is required to be specified")
             exit(1)
 
-        # Get Beancount Files to Process
-        beancount_files = BeancountToJsonl.get_beancount_files(beancount_files, beancount_file_filter)
+        # Get Pdf Files to Process
+        pdf_files = PdfToJsonl.get_pdf_files(pdf_files, pdf_file_filter)
 
-        # Extract Entries from specified Beancount files
-        with timer("Parse transactions from Beancount files into dictionaries", logger):
-            current_entries = BeancountToJsonl.convert_transactions_to_maps(
-                *BeancountToJsonl.extract_beancount_transactions(beancount_files)
-            )
+        # Extract Entries from specified Pdf files
+        with timer("Parse entries from PDF files into dictionaries", logger):
+            current_entries = PdfToJsonl.convert_pdf_entries_to_maps(*PdfToJsonl.extract_pdf_entries(pdf_files))
 
         # Split entries by max tokens supported by model
         with timer("Split entries by max token size supported by model", logger):
             current_entries = self.split_entries_by_max_tokens(current_entries, max_tokens=256)
 
         # Identify, mark and merge any new entries with previous entries
-        with timer("Identify new or updated transaction", logger):
+        with timer("Identify new or updated entries", logger):
             if not previous_entries:
                 entries_with_ids = list(enumerate(current_entries))
             else:
                 entries_with_ids = TextToJsonl.mark_entries_for_update(
                     current_entries, previous_entries, key="compiled", logger=logger
                 )
 
-        with timer("Write transactions to JSONL file", logger):
+        with timer("Write PDF entries to JSONL file", logger):
             # Process Each Entry from All Notes Files
             entries = list(map(lambda entry: entry[1], entries_with_ids))
-            jsonl_data = BeancountToJsonl.convert_transaction_maps_to_jsonl(entries)
+            jsonl_data = PdfToJsonl.convert_pdf_maps_to_jsonl(entries)
 
             # Compress JSONL formatted Data
             if output_file.suffix == ".gz":
                 compress_jsonl_data(jsonl_data, output_file)
             elif output_file.suffix == ".jsonl":
                 dump_jsonl(jsonl_data, output_file)
 
         return entries_with_ids
 
     @staticmethod
-    def get_beancount_files(beancount_files=None, beancount_file_filters=None):
-        "Get Beancount files to process"
-        absolute_beancount_files, filtered_beancount_files = set(), set()
-        if beancount_files:
-            absolute_beancount_files = {get_absolute_path(beancount_file) for beancount_file in beancount_files}
-        if beancount_file_filters:
-            filtered_beancount_files = {
+    def get_pdf_files(pdf_files=None, pdf_file_filters=None):
+        "Get PDF files to process"
+        absolute_pdf_files, filtered_pdf_files = set(), set()
+        if pdf_files:
+            absolute_pdf_files = {get_absolute_path(pdf_file) for pdf_file in pdf_files}
+        if pdf_file_filters:
+            filtered_pdf_files = {
                 filtered_file
-                for beancount_file_filter in beancount_file_filters
-                for filtered_file in glob.glob(get_absolute_path(beancount_file_filter), recursive=True)
+                for pdf_file_filter in pdf_file_filters
+                for filtered_file in glob.glob(get_absolute_path(pdf_file_filter), recursive=True)
             }
 
-        all_beancount_files = sorted(absolute_beancount_files | filtered_beancount_files)
+        all_pdf_files = sorted(absolute_pdf_files | filtered_pdf_files)
 
-        files_with_non_beancount_extensions = {
-            beancount_file
-            for beancount_file in all_beancount_files
-            if not beancount_file.endswith(".bean") and not beancount_file.endswith(".beancount")
-        }
-        if any(files_with_non_beancount_extensions):
-            print(f"[Warning] There maybe non beancount files in the input set: {files_with_non_beancount_extensions}")
+        files_with_non_pdf_extensions = {pdf_file for pdf_file in all_pdf_files if not pdf_file.endswith(".pdf")}
 
-        logger.debug(f"Processing files: {all_beancount_files}")
+        if any(files_with_non_pdf_extensions):
+            logger.warning(
+                f"[Warning] There maybe non pdf-mode files in the input set: {files_with_non_pdf_extensions}"
+            )
 
-        return all_beancount_files
+        logger.debug(f"Processing files: {all_pdf_files}")
 
-    @staticmethod
-    def extract_beancount_transactions(beancount_files):
-        "Extract entries from specified Beancount files"
+        return all_pdf_files
 
-        # Initialize Regex for extracting Beancount Entries
-        transaction_regex = r"^\n?\d{4}-\d{2}-\d{2} [\*|\!] "
-        empty_newline = f"^[\n\r\t\ ]*$"
+    @staticmethod
+    def extract_pdf_entries(pdf_files):
+        """Extract entries by page from specified PDF files"""
 
         entries = []
-        transaction_to_file_map = []
-        for beancount_file in beancount_files:
-            with open(beancount_file) as f:
-                ledger_content = f.read()
-                transactions_per_file = [
-                    entry.strip(empty_escape_sequences)
-                    for entry in re.split(empty_newline, ledger_content, flags=re.MULTILINE)
-                    if re.match(transaction_regex, entry)
-                ]
-                transaction_to_file_map += zip(transactions_per_file, [beancount_file] * len(transactions_per_file))
-                entries.extend(transactions_per_file)
-        return entries, dict(transaction_to_file_map)
+        entry_to_location_map = []
+        for pdf_file in pdf_files:
+            loader = PyPDFLoader(pdf_file)
+            pdf_entries_per_file = [page.page_content for page in loader.load()]
+            entry_to_location_map += zip(pdf_entries_per_file, [pdf_file] * len(pdf_entries_per_file))
+            entries.extend(pdf_entries_per_file)
+
+        return entries, dict(entry_to_location_map)
 
     @staticmethod
-    def convert_transactions_to_maps(parsed_entries: List[str], transaction_to_file_map) -> List[Entry]:
-        "Convert each parsed Beancount transaction into a Entry"
+    def convert_pdf_entries_to_maps(parsed_entries: List[str], entry_to_file_map) -> List[Entry]:
+        "Convert each PDF entries into a dictionary"
         entries = []
         for parsed_entry in parsed_entries:
+            entry_filename = Path(entry_to_file_map[parsed_entry])
+            # Append base filename to compiled entry for context to model
+            heading = f"{entry_filename.stem}\n"
+            compiled_entry = f"{heading}{parsed_entry}"
             entries.append(
-                Entry(compiled=parsed_entry, raw=parsed_entry, file=f"{transaction_to_file_map[parsed_entry]}")
+                Entry(
+                    compiled=compiled_entry,
+                    raw=parsed_entry,
+                    heading=heading,
+                    file=f"{entry_filename}",
+                )
             )
 
-        logger.debug(f"Converted {len(parsed_entries)} transactions to dictionaries")
+        logger.debug(f"Converted {len(parsed_entries)} PDF entries to dictionaries")
 
         return entries
 
     @staticmethod
-    def convert_transaction_maps_to_jsonl(entries: List[Entry]) -> str:
-        "Convert each Beancount transaction entry to JSON and collate as JSONL"
+    def convert_pdf_maps_to_jsonl(entries: List[Entry]):
+        "Convert each PDF entry to JSON and collate as JSONL"
         return "".join([f"{entry.to_json()}\n" for entry in entries])
```

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.7.1.dev23/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.7.1.dev23/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.7.1.dev23/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/routers/api.py` & `khoj_assistant-0.7.1.dev23/src/khoj/routers/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,19 +167,17 @@
 
     # Encode query with filter terms removed
     defiltered_query = user_query
     for filter in [DateFilter(), WordFilter(), FileFilter()]:
         defiltered_query = filter.defilter(user_query)
 
     encoded_asymmetric_query = None
-    if t == SearchType.All or (t != SearchType.Ledger and t != SearchType.Image):
+    if t == SearchType.All or t != SearchType.Image:
         text_search_models: List[TextSearchModel] = [
-            model
-            for model_name, model in state.model.__dict__.items()
-            if isinstance(model, TextSearchModel) and model_name != "ledger_search"
+            model for model in state.model.__dict__.values() if isinstance(model, TextSearchModel)
         ]
         if text_search_models:
             with timer("Encoding query took", logger=logger):
                 encoded_asymmetric_query = util.normalize_embeddings(
                     text_search_models[0].bi_encoder.encode(
                         [defiltered_query],
                         convert_to_tensor=True,
@@ -240,41 +238,14 @@
                     question_embedding=encoded_asymmetric_query,
                     rank_results=r or False,
                     score_threshold=score_threshold,
                     dedupe=dedupe or True,
                 )
             ]
 
-        if (t == SearchType.Ledger) and state.model.ledger_search:
-            # query transactions
-            search_futures += [
-                executor.submit(
-                    text_search.query,
-                    user_query,
-                    state.model.ledger_search,
-                    rank_results=r or False,
-                    score_threshold=score_threshold,
-                    dedupe=dedupe or True,
-                )
-            ]
-
-        if (t == SearchType.Music or t == SearchType.All) and state.model.music_search:
-            # query music library
-            search_futures += [
-                executor.submit(
-                    text_search.query,
-                    user_query,
-                    state.model.music_search,
-                    question_embedding=encoded_asymmetric_query,
-                    rank_results=r or False,
-                    score_threshold=score_threshold,
-                    dedupe=dedupe or True,
-                )
-            ]
-
         if (t == SearchType.Image) and state.model.image_search:
             # query images
             search_futures += [
                 executor.submit(
                     image_search.query,
                     user_query,
                     results_count,
```

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/routers/api_beta.py` & `khoj_assistant-0.7.1.dev23/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/routers/web_client.py` & `khoj_assistant-0.7.1.dev23/src/khoj/routers/web_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import json
 
 
 # Initialize Router
 web_client = APIRouter()
 templates = Jinja2Templates(directory=constants.web_directory)
 
-VALID_CONTENT_TYPES = ["org", "ledger", "markdown", "pdf"]
+VALID_TEXT_CONTENT_TYPES = ["org", "markdown", "pdf"]
 
 
 # Create Routes
 @web_client.get("/", response_class=FileResponse)
 def index(request: Request):
     return templates.TemplateResponse("index.html", context={"request": request, "demo": state.demo})
 
@@ -56,15 +56,15 @@
 
         return templates.TemplateResponse(
             "content_type_github_input.html", context={"request": request, "current_config": current_config}
         )
 
     @web_client.get("/config/content_type/{content_type}", response_class=HTMLResponse)
     def content_config_page(request: Request, content_type: str):
-        if content_type not in VALID_CONTENT_TYPES:
+        if content_type not in VALID_TEXT_CONTENT_TYPES:
             return templates.TemplateResponse("config.html", context={"request": request})
 
         default_copy = constants.default_config.copy()
         default_content_type = default_copy["content-type"][content_type]  # type: ignore
 
         default_config = TextContentConfig(
             compressed_jsonl=default_content_type["compressed-jsonl"],
```

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.7.1.dev23/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.7.1.dev23/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.7.1.dev23/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.7.1.dev23/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/search_type/image_search.py` & `khoj_assistant-0.7.1.dev23/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/search_type/text_search.py` & `khoj_assistant-0.7.1.dev23/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/utils/cli.py` & `khoj_assistant-0.7.1.dev23/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/utils/config.py` & `khoj_assistant-0.7.1.dev23/src/khoj/utils/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     from khoj.utils.models import BaseEncoder
     from khoj.utils.rawconfig import ConversationProcessorConfig, Entry
 
 
 class SearchType(str, Enum):
     All = "all"
     Org = "org"
-    Ledger = "ledger"
-    Music = "music"
     Markdown = "markdown"
     Image = "image"
     Pdf = "pdf"
     Github = "github"
 
 
 class ProcessorType(str, Enum):
@@ -57,16 +55,14 @@
         self.image_metadata_embeddings = image_metadata_embeddings
         self.image_encoder = image_encoder
 
 
 @dataclass
 class SearchModels:
     org_search: TextSearchModel = None
-    ledger_search: TextSearchModel = None
-    music_search: TextSearchModel = None
     markdown_search: TextSearchModel = None
     pdf_search: TextSearchModel = None
     image_search: ImageSearchModel = None
     github_search: TextSearchModel = None
     plugin_search: Dict[str, TextSearchModel] = None
```

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/utils/constants.py` & `khoj_assistant-0.7.1.dev23/src/khoj/utils/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,39 +18,27 @@
         },
         "markdown": {
             "input-files": None,
             "input-filter": None,
             "compressed-jsonl": "~/.khoj/content/markdown/markdown.jsonl.gz",
             "embeddings-file": "~/.khoj/content/markdown/markdown_embeddings.pt",
         },
-        "ledger": {
-            "input-files": None,
-            "input-filter": None,
-            "compressed-jsonl": "~/.khoj/content/ledger/ledger.jsonl.gz",
-            "embeddings-file": "~/.khoj/content/ledger/ledger_embeddings.pt",
-        },
         "pdf": {
             "input-files": None,
             "input-filter": None,
             "compressed-jsonl": "~/.khoj/content/pdf/pdf.jsonl.gz",
             "embeddings-file": "~/.khoj/content/pdf/pdf_embeddings.pt",
         },
         "image": {
             "input-directories": None,
             "input-filter": None,
             "embeddings-file": "~/.khoj/content/image/image_embeddings.pt",
             "batch-size": 50,
             "use-xmp-metadata": False,
         },
-        "music": {
-            "input-files": None,
-            "input-filter": None,
-            "compressed-jsonl": "~/.khoj/content/music/music.jsonl.gz",
-            "embeddings-file": "~/.khoj/content/music/music_embeddings.pt",
-        },
         "github": {
             "pat-token": None,
             "repos": [],
             "compressed-jsonl": "~/.khoj/content/github/github.jsonl.gz",
             "embeddings-file": "~/.khoj/content/github/github_embeddings.pt",
         },
     },
```

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/utils/helpers.py` & `khoj_assistant-0.7.1.dev23/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/utils/jsonl.py` & `khoj_assistant-0.7.1.dev23/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/utils/models.py` & `khoj_assistant-0.7.1.dev23/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.7.1.dev23/src/khoj/utils/rawconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,17 +68,15 @@
                 "Either input_filter or input_directories required in all content-type.image section of Khoj config file"
             )
         return input_filter
 
 
 class ContentConfig(ConfigBase):
     org: Optional[TextContentConfig]
-    ledger: Optional[TextContentConfig]
     image: Optional[ImageContentConfig]
-    music: Optional[TextContentConfig]
     markdown: Optional[TextContentConfig]
     pdf: Optional[TextContentConfig]
     github: Optional[GithubContentConfig]
     plugins: Optional[Dict[str, TextContentConfig]]
 
 
 class TextSearchConfig(ConfigBase):
```

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/utils/state.py` & `khoj_assistant-0.7.1.dev23/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/src/khoj/utils/yaml.py` & `khoj_assistant-0.7.1.dev23/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/.gitignore` & `khoj_assistant-0.7.1.dev23/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/LICENSE` & `khoj_assistant-0.7.1.dev23/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev15/README.md` & `khoj_assistant-0.7.1.dev23/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 - **Chat**
   - **Faster answers**: Find answers faster, smoother than search. No need to manually scan through your notes to find answers.
   - **Iterative discovery**: Iteratively explore and (re-)discover your notes
   - **Assisted creativity**: Smoothly weave across answers retrieval and content generation
 - **General**
   - **Natural**: Advanced natural language understanding using Transformer based ML Models
   - **Pluggable**: Modular architecture makes it easy to plug in new data sources, frontends and ML models
-  - **Multiple Sources**: Index your Org-mode and Markdown notes, Beancount transactions, PDF files, Github repositories, and Photos
+  - **Multiple Sources**: Index your Org-mode and Markdown notes, PDF files, Github repositories, and Photos
   - **Multiple Interfaces**: Interact from your [Web Browser](./src/khoj/interface/web/index.html), [Emacs](./src/interface/emacs/khoj.el) or [Obsidian](./src/interface/obsidian/)
 
 ## Demos
 ### Khoj in Obsidian
 https://github.com/khoj-ai/khoj/assets/6413477/3e33d8ea-25bb-46c8-a3bf-c92f78d0f56b
 
 <details><summary>Description</summary>
@@ -263,15 +263,15 @@
 
 ## Advanced Usage
 ### Access Khoj on Mobile
 1. [Setup Khoj](#Setup) on your personal server. This can be any always-on machine, i.e an old computer, RaspberryPi(?) etc
 2. [Install](https://tailscale.com/kb/installation/) [Tailscale](tailscale.com/) on your personal server and phone
 3. Open the Khoj web interface of the server from your phone browser.<br /> It should be `http://tailscale-ip-of-server:8000` or `http://name-of-server:8000` if you've setup [MagicDNS](https://tailscale.com/kb/1081/magicdns/)
 4. Click the [Add to Homescreen](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Add_to_home_screen) button
-5. Enjoy exploring your notes, transactions and images from your phone!
+5. Enjoy exploring your notes, documents and images from your phone!
 
 ![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_pwa_android.png?)
 
 ### Use OpenAI Models for Search
 #### Setup
 1. Set `encoder-type`, `encoder` and `model-directory` under `asymmetric` and/or `symmetric` `search-type` in your `khoj.yml`[^1]:
    ```diff
@@ -395,26 +395,26 @@
    - **Manually**:
      - Copy the `config/khoj_sample.yml` to `~/.khoj/khoj.yml`
      - Set `input-files` or `input-filter` in each relevant `content-type` section of `~/.khoj/khoj.yml`
        - Set `input-directories` field in `image` `content-type` section
      - Delete `content-type` and `processor` sub-section(s) irrelevant for your use-case
      - Restart khoj
 
-  Note: Wait after configuration for khoj to Load ML model, generate embeddings and expose API to query notes, images, transactions etc specified in config YAML
+  Note: Wait after configuration for khoj to Load ML model, generate embeddings and expose API to query notes, images, documents etc specified in config YAML
 
 #### Using Docker
 ##### 1. Clone
 
 ```shell
 git clone https://github.com/khoj-ai/khoj && cd khoj
 ```
 
 ##### 2. Configure
 
-- **Required**: Update [docker-compose.yml](./docker-compose.yml) to mount your images, (org-mode or markdown) notes, pdf, Github repositories, and beancount directories
+- **Required**: Update [docker-compose.yml](./docker-compose.yml) to mount your images, (org-mode or markdown) notes, PDFs and Github repositories
 - **Optional**: Edit application configuration in [khoj_docker.yml](./config/khoj_docker.yml)
 
 ##### 3. Run
 
 ```shell
 docker-compose up -d
 ```
@@ -445,15 +445,15 @@
   - Set `input-directories` field in `image` `content-type` section
 - Delete `content-type`, `processor` sub-sections irrelevant for your use-case
 
 ##### 4. Run
 ```shell
 python3 -m src.khoj.main -vv
 ```
-  Load ML model, generate embeddings and expose API to query notes, images, transactions etc specified in config YAML
+  Load ML model, generate embeddings and expose API to query notes, images, documents etc specified in config YAML
 
 ##### 5. Upgrade
 ```shell
 cd khoj
 git pull origin master
 conda deactivate khoj
 conda env update -f config/environment.yml
```

### Comparing `khoj_assistant-0.7.1.dev15/pyproject.toml` & `khoj_assistant-0.7.1.dev23/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     "search",
     "semantic-search",
     "productivity",
     "NLP",
     "AI",
     "org-mode",
     "markdown",
-    "beancount",
     "images",
     "pdf",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

### Comparing `khoj_assistant-0.7.1.dev15/PKG-INFO` & `khoj_assistant-0.7.1.dev23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.7.1.dev15
+Version: 0.7.1.dev23
 Summary: An AI personal assistant for your Digital Brain
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
-Keywords: AI,NLP,beancount,images,markdown,org-mode,pdf,productivity,search,semantic-search
+Keywords: AI,NLP,images,markdown,org-mode,pdf,productivity,search,semantic-search
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -118,15 +118,15 @@
 - **Chat**
   - **Faster answers**: Find answers faster, smoother than search. No need to manually scan through your notes to find answers.
   - **Iterative discovery**: Iteratively explore and (re-)discover your notes
   - **Assisted creativity**: Smoothly weave across answers retrieval and content generation
 - **General**
   - **Natural**: Advanced natural language understanding using Transformer based ML Models
   - **Pluggable**: Modular architecture makes it easy to plug in new data sources, frontends and ML models
-  - **Multiple Sources**: Index your Org-mode and Markdown notes, Beancount transactions, PDF files, Github repositories, and Photos
+  - **Multiple Sources**: Index your Org-mode and Markdown notes, PDF files, Github repositories, and Photos
   - **Multiple Interfaces**: Interact from your [Web Browser](./src/khoj/interface/web/index.html), [Emacs](./src/interface/emacs/khoj.el) or [Obsidian](./src/interface/obsidian/)
 
 ## Demos
 ### Khoj in Obsidian
 https://github.com/khoj-ai/khoj/assets/6413477/3e33d8ea-25bb-46c8-a3bf-c92f78d0f56b
 
 <details><summary>Description</summary>
@@ -321,15 +321,15 @@
 
 ## Advanced Usage
 ### Access Khoj on Mobile
 1. [Setup Khoj](#Setup) on your personal server. This can be any always-on machine, i.e an old computer, RaspberryPi(?) etc
 2. [Install](https://tailscale.com/kb/installation/) [Tailscale](tailscale.com/) on your personal server and phone
 3. Open the Khoj web interface of the server from your phone browser.<br /> It should be `http://tailscale-ip-of-server:8000` or `http://name-of-server:8000` if you've setup [MagicDNS](https://tailscale.com/kb/1081/magicdns/)
 4. Click the [Add to Homescreen](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Add_to_home_screen) button
-5. Enjoy exploring your notes, transactions and images from your phone!
+5. Enjoy exploring your notes, documents and images from your phone!
 
 ![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_pwa_android.png?)
 
 ### Use OpenAI Models for Search
 #### Setup
 1. Set `encoder-type`, `encoder` and `model-directory` under `asymmetric` and/or `symmetric` `search-type` in your `khoj.yml`[^1]:
    ```diff
@@ -453,26 +453,26 @@
    - **Manually**:
      - Copy the `config/khoj_sample.yml` to `~/.khoj/khoj.yml`
      - Set `input-files` or `input-filter` in each relevant `content-type` section of `~/.khoj/khoj.yml`
        - Set `input-directories` field in `image` `content-type` section
      - Delete `content-type` and `processor` sub-section(s) irrelevant for your use-case
      - Restart khoj
 
-  Note: Wait after configuration for khoj to Load ML model, generate embeddings and expose API to query notes, images, transactions etc specified in config YAML
+  Note: Wait after configuration for khoj to Load ML model, generate embeddings and expose API to query notes, images, documents etc specified in config YAML
 
 #### Using Docker
 ##### 1. Clone
 
 ```shell
 git clone https://github.com/khoj-ai/khoj && cd khoj
 ```
 
 ##### 2. Configure
 
-- **Required**: Update [docker-compose.yml](./docker-compose.yml) to mount your images, (org-mode or markdown) notes, pdf, Github repositories, and beancount directories
+- **Required**: Update [docker-compose.yml](./docker-compose.yml) to mount your images, (org-mode or markdown) notes, PDFs and Github repositories
 - **Optional**: Edit application configuration in [khoj_docker.yml](./config/khoj_docker.yml)
 
 ##### 3. Run
 
 ```shell
 docker-compose up -d
 ```
@@ -503,15 +503,15 @@
   - Set `input-directories` field in `image` `content-type` section
 - Delete `content-type`, `processor` sub-sections irrelevant for your use-case
 
 ##### 4. Run
 ```shell
 python3 -m src.khoj.main -vv
 ```
-  Load ML model, generate embeddings and expose API to query notes, images, transactions etc specified in config YAML
+  Load ML model, generate embeddings and expose API to query notes, images, documents etc specified in config YAML
 
 ##### 5. Upgrade
 ```shell
 cd khoj
 git pull origin master
 conda deactivate khoj
 conda env update -f config/environment.yml
```

