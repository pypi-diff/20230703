# Comparing `tmp/khoj_assistant-0.7.1.dev12.tar.gz` & `tmp/khoj_assistant-0.7.1.dev14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Jul  2 16:14:08 2023, max compression
+gzip compressed data, last modified: Sun Jul  2 23:08:29 2023, max compression
```

## Comparing `khoj_assistant-0.7.1.dev12.tar` & `khoj_assistant-0.7.1.dev14.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/__init__.py
--rw-r--r--   0        0        0    11412 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/configure.py
--rw-r--r--   0        0        0     5379 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1395 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     3532 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    14414 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0     6212 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     6990 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     6799 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    19296 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3644 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1813 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0   205167 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     7946 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6056 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13481 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5708 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7454 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5193 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    18153 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     4394 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7560 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11381 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11054 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2088 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2510 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2995 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6852 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4215 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1066 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/LICENSE
--rw-r--r--   0        0        0    23398 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/README.md
--rw-r--r--   0        0        0     2841 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/pyproject.toml
--rw-r--r--   0        0        0    25805 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/__init__.py
+-rw-r--r--   0        0        0    11900 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/configure.py
+-rw-r--r--   0        0        0     5379 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     3532 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    14414 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0     6212 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6990 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     6799 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    19296 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3644 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1813 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0   205167 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     7946 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6056 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13481 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5708 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7454 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5193 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    18314 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     4394 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7560 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11054 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2088 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2510 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2995 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6852 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4215 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/LICENSE
+-rw-r--r--   0        0        0    23398 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/README.md
+-rw-r--r--   0        0        0     2841 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/pyproject.toml
+-rw-r--r--   0        0        0    25805 2023-07-02 23:08:29.000000 khoj_assistant-0.7.1.dev14/PKG-INFO
```

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/configure.py` & `khoj_assistant-0.7.1.dev14/src/khoj/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,106 +89,114 @@
 
 
 def configure_search(model: SearchModels, config: FullConfig, regenerate: bool, t: Optional[state.SearchType] = None):
     if config is None or config.content_type is None or config.search_type is None:
         logger.warning("🚨 No Content or Search type is configured.")
         return
 
-    # Initialize Org Notes Search
-    if (t == state.SearchType.Org or t == None) and config.content_type.org and config.search_type.asymmetric:
-        logger.info("🦄 Setting up search for orgmode notes")
-        # Extract Entries, Generate Notes Embeddings
-        model.org_search = text_search.setup(
-            OrgToJsonl,
-            config.content_type.org,
-            search_config=config.search_type.asymmetric,
-            regenerate=regenerate,
-            filters=[DateFilter(), WordFilter(), FileFilter()],
-        )
-
-    # Initialize Org Music Search
-    if (t == state.SearchType.Music or t == None) and config.content_type.music and config.search_type.asymmetric:
-        logger.info("🎺 Setting up search for org-music")
-        # Extract Entries, Generate Music Embeddings
-        model.music_search = text_search.setup(
-            OrgToJsonl,
-            config.content_type.music,
-            search_config=config.search_type.asymmetric,
-            regenerate=regenerate,
-            filters=[DateFilter(), WordFilter()],
-        )
-
-    # Initialize Markdown Search
-    if (t == state.SearchType.Markdown or t == None) and config.content_type.markdown and config.search_type.asymmetric:
-        logger.info("💎 Setting up search for markdown notes")
-        # Extract Entries, Generate Markdown Embeddings
-        model.markdown_search = text_search.setup(
-            MarkdownToJsonl,
-            config.content_type.markdown,
-            search_config=config.search_type.asymmetric,
-            regenerate=regenerate,
-            filters=[DateFilter(), WordFilter(), FileFilter()],
-        )
-
-    # Initialize Ledger Search
-    if (t == state.SearchType.Ledger or t == None) and config.content_type.ledger and config.search_type.symmetric:
-        logger.info("💸 Setting up search for ledger")
-        # Extract Entries, Generate Ledger Embeddings
-        model.ledger_search = text_search.setup(
-            BeancountToJsonl,
-            config.content_type.ledger,
-            search_config=config.search_type.symmetric,
-            regenerate=regenerate,
-            filters=[DateFilter(), WordFilter(), FileFilter()],
-        )
-
-    # Initialize PDF Search
-    if (t == state.SearchType.Pdf or t == None) and config.content_type.pdf and config.search_type.asymmetric:
-        logger.info("🖨️ Setting up search for pdf")
-        # Extract Entries, Generate PDF Embeddings
-        model.pdf_search = text_search.setup(
-            PdfToJsonl,
-            config.content_type.pdf,
-            search_config=config.search_type.asymmetric,
-            regenerate=regenerate,
-            filters=[DateFilter(), WordFilter(), FileFilter()],
-        )
-
-    # Initialize Image Search
-    if (t == state.SearchType.Image or t == None) and config.content_type.image and config.search_type.image:
-        logger.info("🌄 Setting up search for images")
-        # Extract Entries, Generate Image Embeddings
-        model.image_search = image_search.setup(
-            config.content_type.image, search_config=config.search_type.image, regenerate=regenerate
-        )
-
-    if (t == state.SearchType.Github or t == None) and config.content_type.github and config.search_type.asymmetric:
-        logger.info("🐙 Setting up search for github")
-        # Extract Entries, Generate Github Embeddings
-        model.github_search = text_search.setup(
-            GithubToJsonl,
-            config.content_type.github,
-            search_config=config.search_type.asymmetric,
-            regenerate=regenerate,
-            filters=[DateFilter(), WordFilter(), FileFilter()],
-        )
-
-    # Initialize External Plugin Search
-    if (t == None or t in state.SearchType) and config.content_type.plugins:
-        logger.info("🔌 Setting up search for plugins")
-        model.plugin_search = {}
-        for plugin_type, plugin_config in config.content_type.plugins.items():
-            model.plugin_search[plugin_type] = text_search.setup(
-                JsonlToJsonl,
-                plugin_config,
+    try:
+        # Initialize Org Notes Search
+        if (t == state.SearchType.Org or t == None) and config.content_type.org and config.search_type.asymmetric:
+            logger.info("🦄 Setting up search for orgmode notes")
+            # Extract Entries, Generate Notes Embeddings
+            model.org_search = text_search.setup(
+                OrgToJsonl,
+                config.content_type.org,
                 search_config=config.search_type.asymmetric,
                 regenerate=regenerate,
                 filters=[DateFilter(), WordFilter(), FileFilter()],
             )
 
+        # Initialize Org Music Search
+        if (t == state.SearchType.Music or t == None) and config.content_type.music and config.search_type.asymmetric:
+            logger.info("🎺 Setting up search for org-music")
+            # Extract Entries, Generate Music Embeddings
+            model.music_search = text_search.setup(
+                OrgToJsonl,
+                config.content_type.music,
+                search_config=config.search_type.asymmetric,
+                regenerate=regenerate,
+                filters=[DateFilter(), WordFilter()],
+            )
+
+        # Initialize Markdown Search
+        if (
+            (t == state.SearchType.Markdown or t == None)
+            and config.content_type.markdown
+            and config.search_type.asymmetric
+        ):
+            logger.info("💎 Setting up search for markdown notes")
+            # Extract Entries, Generate Markdown Embeddings
+            model.markdown_search = text_search.setup(
+                MarkdownToJsonl,
+                config.content_type.markdown,
+                search_config=config.search_type.asymmetric,
+                regenerate=regenerate,
+                filters=[DateFilter(), WordFilter(), FileFilter()],
+            )
+
+        # Initialize Ledger Search
+        if (t == state.SearchType.Ledger or t == None) and config.content_type.ledger and config.search_type.symmetric:
+            logger.info("💸 Setting up search for ledger")
+            # Extract Entries, Generate Ledger Embeddings
+            model.ledger_search = text_search.setup(
+                BeancountToJsonl,
+                config.content_type.ledger,
+                search_config=config.search_type.symmetric,
+                regenerate=regenerate,
+                filters=[DateFilter(), WordFilter(), FileFilter()],
+            )
+
+        # Initialize PDF Search
+        if (t == state.SearchType.Pdf or t == None) and config.content_type.pdf and config.search_type.asymmetric:
+            logger.info("🖨️ Setting up search for pdf")
+            # Extract Entries, Generate PDF Embeddings
+            model.pdf_search = text_search.setup(
+                PdfToJsonl,
+                config.content_type.pdf,
+                search_config=config.search_type.asymmetric,
+                regenerate=regenerate,
+                filters=[DateFilter(), WordFilter(), FileFilter()],
+            )
+
+        # Initialize Image Search
+        if (t == state.SearchType.Image or t == None) and config.content_type.image and config.search_type.image:
+            logger.info("🌄 Setting up search for images")
+            # Extract Entries, Generate Image Embeddings
+            model.image_search = image_search.setup(
+                config.content_type.image, search_config=config.search_type.image, regenerate=regenerate
+            )
+
+        if (t == state.SearchType.Github or t == None) and config.content_type.github and config.search_type.asymmetric:
+            logger.info("🐙 Setting up search for github")
+            # Extract Entries, Generate Github Embeddings
+            model.github_search = text_search.setup(
+                GithubToJsonl,
+                config.content_type.github,
+                search_config=config.search_type.asymmetric,
+                regenerate=regenerate,
+                filters=[DateFilter(), WordFilter(), FileFilter()],
+            )
+
+        # Initialize External Plugin Search
+        if (t == None or t in state.SearchType) and config.content_type.plugins:
+            logger.info("🔌 Setting up search for plugins")
+            model.plugin_search = {}
+            for plugin_type, plugin_config in config.content_type.plugins.items():
+                model.plugin_search[plugin_type] = text_search.setup(
+                    JsonlToJsonl,
+                    plugin_config,
+                    search_config=config.search_type.asymmetric,
+                    regenerate=regenerate,
+                    filters=[DateFilter(), WordFilter(), FileFilter()],
+                )
+    except Exception as e:
+        logger.error("🚨 Failed to setup search")
+        raise e
+
     # Invalidate Query Cache
     state.query_cache = LRU()
 
     return model
 
 
 def configure_processor(processor_config: ProcessorConfig):
```

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/main.py` & `khoj_assistant-0.7.1.dev14/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/404.html` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/chat.html` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/config.html` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/index.html` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.7.1.dev14/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.7.1.dev14/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.7.1.dev14/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.7.1.dev14/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.7.1.dev14/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.7.1.dev14/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.7.1.dev14/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.7.1.dev14/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.7.1.dev14/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.7.1.dev14/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.7.1.dev14/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.7.1.dev14/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/routers/api.py` & `khoj_assistant-0.7.1.dev14/src/khoj/routers/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,16 +353,21 @@
     client: Optional[str] = None,
     user_agent: Optional[str] = Header(None),
     referer: Optional[str] = Header(None),
     host: Optional[str] = Header(None),
 ):
     try:
         state.search_index_lock.acquire()
-        state.model = configure_search(state.model, state.config, regenerate=force or False, t=t)
-        state.search_index_lock.release()
+        try:
+            state.model = configure_search(state.model, state.config, regenerate=force or False, t=t)
+        except Exception as e:
+            logger.error(e)
+            raise HTTPException(status_code=500, detail=str(e))
+        finally:
+            state.search_index_lock.release()
     except ValueError as e:
         logger.error(e)
         raise HTTPException(status_code=500, detail=str(e))
     else:
         logger.info("📬 Search index updated via API")
 
     try:
```

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/routers/api_beta.py` & `khoj_assistant-0.7.1.dev14/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/routers/web_client.py` & `khoj_assistant-0.7.1.dev14/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.7.1.dev14/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.7.1.dev14/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.7.1.dev14/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.7.1.dev14/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/search_type/image_search.py` & `khoj_assistant-0.7.1.dev14/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/search_type/text_search.py` & `khoj_assistant-0.7.1.dev14/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/utils/cli.py` & `khoj_assistant-0.7.1.dev14/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/utils/config.py` & `khoj_assistant-0.7.1.dev14/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/utils/constants.py` & `khoj_assistant-0.7.1.dev14/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/utils/helpers.py` & `khoj_assistant-0.7.1.dev14/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/utils/jsonl.py` & `khoj_assistant-0.7.1.dev14/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/utils/models.py` & `khoj_assistant-0.7.1.dev14/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.7.1.dev14/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/utils/state.py` & `khoj_assistant-0.7.1.dev14/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/src/khoj/utils/yaml.py` & `khoj_assistant-0.7.1.dev14/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/.gitignore` & `khoj_assistant-0.7.1.dev14/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/LICENSE` & `khoj_assistant-0.7.1.dev14/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/README.md` & `khoj_assistant-0.7.1.dev14/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/pyproject.toml` & `khoj_assistant-0.7.1.dev14/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev12/PKG-INFO` & `khoj_assistant-0.7.1.dev14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.7.1.dev12
+Version: 0.7.1.dev14
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

