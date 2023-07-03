# Comparing `tmp/mona-openai-0.0.9.tar.gz` & `tmp/mona-openai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mona-openai-0.0.9.tar", last modified: Fri Jun 30 06:24:56 2023, max compression
+gzip compressed data, was "mona-openai-0.1.0.tar", last modified: Mon Jul  3 11:49:23 2023, max compression
```

## Comparing `mona-openai-0.0.9.tar` & `mona-openai-0.1.0.tar`

### file list

```diff
@@ -1,40 +1,48 @@
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-30 06:24:56.189441 mona-openai-0.0.9/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.0.9/LICENSE
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    10802 2023-06-30 06:24:56.189265 mona-openai-0.0.9/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    10208 2023-06-30 04:40:35.000000 mona-openai-0.0.9/README.md
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-30 06:24:56.185001 mona-openai-0.0.9/mona_openai/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      100 2023-06-30 04:40:35.000000 mona-openai-0.0.9/mona_openai/__init__.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-30 06:24:56.186280 mona-openai-0.0.9/mona_openai/analysis/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3613 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/analysis/privacy.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      304 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/analysis/profanity.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3100 2023-06-30 04:45:38.000000 mona-openai-0.0.9/mona_openai/analysis/textual.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-30 06:24:56.187086 mona-openai-0.0.9/mona_openai/endpoints/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     7750 2023-06-30 04:45:19.000000 mona-openai-0.0.9/mona_openai/endpoints/chat_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     5166 2023-06-30 04:45:09.000000 mona-openai-0.0.9/mona_openai/endpoints/completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     4792 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/endpoints/endpoint_wrapping.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      792 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/endpoints/wrapping_getter.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      225 2023-06-28 08:19:06.000000 mona-openai-0.0.9/mona_openai/exceptions.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1379 2023-06-30 04:40:35.000000 mona-openai-0.0.9/mona_openai/mona_client.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    17565 2023-06-30 04:40:35.000000 mona-openai-0.0.9/mona_openai/mona_openai.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-30 06:24:56.188202 mona-openai-0.0.9/mona_openai/util/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      946 2023-06-01 06:55:43.000000 mona-openai-0.0.9/mona_openai/util/async_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      675 2023-05-11 08:33:47.000000 mona-openai-0.0.9/mona_openai/util/func_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1177 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/util/oop_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      364 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/util/openai_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3788 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/util/stream_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      776 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/util/tokens_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.0.9/mona_openai/util/validation_util.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-30 06:24:56.185715 mona-openai-0.0.9/mona_openai.egg-info/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    10802 2023-06-30 06:24:56.000000 mona-openai-0.0.9/mona_openai.egg-info/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      925 2023-06-30 06:24:56.000000 mona-openai-0.0.9/mona_openai.egg-info/SOURCES.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-06-30 06:24:56.000000 mona-openai-0.0.9/mona_openai.egg-info/dependency_links.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       51 2023-06-30 06:24:56.000000 mona-openai-0.0.9/mona_openai.egg-info/requires.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-06-30 06:24:56.000000 mona-openai-0.0.9/mona_openai.egg-info/top_level.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-06-30 06:24:43.000000 mona-openai-0.0.9/pyproject.toml
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       50 2023-05-11 08:33:47.000000 mona-openai-0.0.9/requirements.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-06-30 06:24:56.189476 mona-openai-0.0.9/setup.cfg
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-30 06:24:56.188980 mona-openai-0.0.9/tests/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    17356 2023-06-30 04:45:09.000000 mona-openai-0.0.9/tests/test_chat_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    20107 2023-06-30 04:45:09.000000 mona-openai-0.0.9/tests/test_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1607 2023-05-25 05:50:33.000000 mona-openai-0.0.9/tests/test_privacy_analyzer.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      975 2023-06-29 11:44:26.000000 mona-openai-0.0.9/tests/test_textual_analyzer.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.913505 mona-openai-0.1.0/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.1.0/LICENSE
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    12386 2023-07-03 11:49:23.913279 mona-openai-0.1.0/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    11792 2023-07-03 07:58:39.000000 mona-openai-0.1.0/README.md
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.908400 mona-openai-0.1.0/mona_openai/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      238 2023-07-02 06:46:47.000000 mona-openai-0.1.0/mona_openai/__init__.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.909467 mona-openai-0.1.0/mona_openai/analysis/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3613 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/analysis/privacy.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      304 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/analysis/profanity.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3100 2023-07-02 06:46:51.000000 mona-openai-0.1.0/mona_openai/analysis/textual.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.910181 mona-openai-0.1.0/mona_openai/endpoints/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     7750 2023-07-02 06:46:51.000000 mona-openai-0.1.0/mona_openai/endpoints/chat_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     5166 2023-07-02 06:46:51.000000 mona-openai-0.1.0/mona_openai/endpoints/completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     4792 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/endpoints/endpoint_wrapping.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      792 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/endpoints/wrapping_getter.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      225 2023-06-28 08:19:06.000000 mona-openai-0.1.0/mona_openai/exceptions.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.911044 mona-openai-0.1.0/mona_openai/loggers/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      202 2023-07-03 07:53:34.000000 mona-openai-0.1.0/mona_openai/loggers/__init__.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      965 2023-07-02 06:46:47.000000 mona-openai-0.1.0/mona_openai/loggers/file_logger.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      772 2023-07-02 15:33:33.000000 mona-openai-0.1.0/mona_openai/loggers/in_memory_logging.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1411 2023-07-02 15:30:54.000000 mona-openai-0.1.0/mona_openai/loggers/logger.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.911454 mona-openai-0.1.0/mona_openai/loggers/mona_logger/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1381 2023-07-02 06:46:47.000000 mona-openai-0.1.0/mona_openai/loggers/mona_logger/mona_client.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1928 2023-07-02 07:57:33.000000 mona-openai-0.1.0/mona_openai/loggers/mona_logger/mona_logger.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1048 2023-07-02 07:46:00.000000 mona-openai-0.1.0/mona_openai/loggers/standard_logging.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    16828 2023-07-02 06:46:47.000000 mona-openai-0.1.0/mona_openai/mona_openai.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.912524 mona-openai-0.1.0/mona_openai/util/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      946 2023-06-01 06:55:43.000000 mona-openai-0.1.0/mona_openai/util/async_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      675 2023-05-11 08:33:47.000000 mona-openai-0.1.0/mona_openai/util/func_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1177 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/util/oop_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      364 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/util/openai_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3788 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/util/stream_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      776 2023-05-25 05:50:33.000000 mona-openai-0.1.0/mona_openai/util/tokens_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.1.0/mona_openai/util/validation_util.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.909068 mona-openai-0.1.0/mona_openai.egg-info/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    12386 2023-07-03 11:49:23.000000 mona-openai-0.1.0/mona_openai.egg-info/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1170 2023-07-03 11:49:23.000000 mona-openai-0.1.0/mona_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-07-03 11:49:23.000000 mona-openai-0.1.0/mona_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       51 2023-07-03 11:49:23.000000 mona-openai-0.1.0/mona_openai.egg-info/requires.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-07-03 11:49:23.000000 mona-openai-0.1.0/mona_openai.egg-info/top_level.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-07-03 11:49:02.000000 mona-openai-0.1.0/pyproject.toml
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       50 2023-05-11 08:33:47.000000 mona-openai-0.1.0/requirements.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-07-03 11:49:23.913555 mona-openai-0.1.0/setup.cfg
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-07-03 11:49:23.913083 mona-openai-0.1.0/tests/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    17356 2023-07-02 06:46:51.000000 mona-openai-0.1.0/tests/test_chat_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    20107 2023-07-02 06:46:51.000000 mona-openai-0.1.0/tests/test_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1607 2023-05-25 05:50:33.000000 mona-openai-0.1.0/tests/test_privacy_analyzer.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      975 2023-06-29 11:44:26.000000 mona-openai-0.1.0/tests/test_textual_analyzer.py
```

### Comparing `mona-openai-0.0.9/LICENSE` & `mona-openai-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/PKG-INFO` & `mona-openai-0.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: mona-openai
-Version: 0.0.9
-Summary: Integration client for monitoring OpenAI usage with Mona
-Author-email: Itai Bar Sinai <itai@monalabs.io>
-Project-URL: Homepage, https://github.com/monalabs/mona-openai
-Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
-Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Mona-OpenAI Integration Client
 <p align="center">
   <img src="https://github.com/monalabs/mona-sdk/blob/main/mona_logo.png?raw=true" alt="Mona's logo" width="180"/>
 </p>
 
 <p align="center"><a target="_blank" href="https://monalabs.wistia.com/medias/l6xmdj3cd6?wvideo=l6xmdj3cd6"><img src="https://embed-ssl.wistia.com/deliveries/c15bb616a389fa7d752968ccb3af2ab4.jpg?wistia-l6xmdj3cd6-1-l6xmdj3cd6-video-thumbnail=1&amp;image_play_button_size=2x&amp;image_crop_resized=960x540&amp;image_play_button=1&amp;image_play_button_color=66c7d1e0" width="400" height="225" style="width: 400px; height: 225px;"></a></p><p align="center"><a href="https://monalabs.wistia.com/medias/l6xmdj3cd6?wvideo=l6xmdj3cd6">OpenAI GPT Integration Tutorial</a></p>
 
@@ -27,31 +12,57 @@
 * Profanity and privacy analyses
 * Behavioral drifts and anomalies
 * LangChain support
 * Much much more
 
 ## Setting Up
 
-- TODO: Add part about Mona registration with a link to the relevant landing page where the reader can sign up.
 ```console
 $ pip install mona_openai
 ```
 
-## Quick Start and Example
+If you plan on using Mona as your monitoring service, [sign up for a free account here](https://www.monalabs.io/openai-gpt-monitoring).
+
+## Quick Start
+
+You can find boilerplate code for many use-cases under [the "examples" folder](https://github.com/monalabs/mona-openai/tree/main/examples).
 
-Example boilerplate code for both sync and async usage is given in the file "example_usage.py" and here:
 ```py
 from os import environ
 import asyncio
 import openai
+from mona_openai.loggers import StandardLogger
+from logging import WARNING
 
-from mona_openai import monitor
+from mona_openai import monitor, monitor_with_logger
 
 openai.api_key = environ.get("OPEN_AI_KEY")
 
+# When using a standard logger.
+
+monitored_completion = monitor_with_logger(
+    openai.Completion,
+    StandardLogger(WARNING),
+)
+
+response = monitored_completion.create(
+    model="text-ada-001",
+    prompt="I want to generate some text about ",
+    max_tokens=20,
+    n=1,
+    temperature=0.2,
+    # Adding additional information for monitoring purposes, unrelated to
+    # internal OpenAI call.
+    MONA_additional_data={"customer_id": "A531251"},
+)
+print(response.choices[0].text)
+
+
+# When monitoring with Mona.
+
 MONA_API_KEY = environ.get("MONA_API_KEY")
 MONA_SECRET = environ.get("MONA_SECRET")
 MONA_CREDS = {
     "key": MONA_API_KEY,
     "secret": MONA_SECRET,
 }
 CONTEXT_CLASS_NAME = "SOME_MONITORING_CONTEXT_NAME"
@@ -59,43 +70,25 @@
 
 monitored_completion = monitor(
     openai.Completion,
     MONA_CREDS,
     CONTEXT_CLASS_NAME,
 )
 
-
-prompt = "I want to generate some text about "
-model = "text-ada-001"
-temperature = 0.6
-max_tokens = 5
-n = 1
-
-# Regular (sync) usage
 response = monitored_completion.create(
-    engine=model,
-    prompt=prompt,
-    max_tokens=max_tokens,
-    n=n,
-    temperature=temperature,
+    model="text-ada-001",
+    prompt="I want to generate some text about ",
+    max_tokens=20,
+    n=1,
+    temperature=0.2,
+    # Adding additional information for monitoring purposes, unrelated to
+    # internal OpenAI call.
     MONA_additional_data={"customer_id": "A531251"},
 )
 print(response.choices[0].text)
-
-# Async usage
-response = asyncio.run(monitored_completion.acreate(
-    engine=model,
-    prompt=prompt,
-    max_tokens=max_tokens,
-    n=n,
-    temperature=temperature,
-    MONA_additional_data={"customer_id": "A531251"},
-))
-
-print(response.choices[0].text)
 ```
 ## Supported OpenAI APIs
 Currently this client supports `openai.Completion` and `openai.ChatCompletion`. Mona can support processes based on other APIs and also non-OpenAI-based apps.
 If you have a differrent use-case, we'd love to hear about it! Please email us at support@monalabs.io.
 
 ## Usage
 ### Initialization
@@ -136,14 +129,47 @@
 The specs arg allows you to configure what should be monitored. It expects a python dict with the follwoing possible keys:
 * sampling_ratio (1): A number between 0 and 1 for how often should the call be logged.
 * avoid_monitoring_exceptions (False): Whether or not to log out to Mona when there is an OpenAI exception. Default is to track exceptions - and Mona will alert you on things like a jump in number of exceptions
 * export_prompt (False): Whether Mona should export the actual prompt text. Be default set to False to avoid privacy concerns.
 * export_response_texts (False): Whether Mona should export the actual response texts. Be default set to False to avoid privacy concerns.
 * analysis: A dictionary mapping each analysis type to a boolean value telling the client whether or not to run said analysis and log it to Mona. Possible options currently are "privacy", "profanity", and "textual". By default, all analyses take place and are logged out to Mona.
 
+### Using custom loggers
+You don't have to have a Mona account to use this package. You can define specific loggers to log out the data to a file, memory, or just a given python logger. For example, to log out the relevant metrics as WARNING:
+
+```py
+from os import environ
+import openai
+from mona_openai.loggers import StandardLogger
+from logging import WARNING
+
+from mona_openai import monitor_with_logger
+
+openai.api_key = environ.get("OPEN_AI_KEY")
+
+monitored_completion = monitor_with_logger(
+    openai.Completion,
+    StandardLogger(WARNING),
+)
+
+response = monitored_completion.create(
+    model="text-ada-001",
+    prompt="I want to generate some text about ",
+    max_tokens=20,
+    n=1,
+    temperature=0.2,
+    # Adding additional information for monitoring purposes, unrelated to
+    # internal OpenAI call.
+    MONA_additional_data={"customer_id": "A531251"},
+)
+```
+
+This SDK provides a simple interface to implement your own loggers by inheriting from Logger under loggers/logger.py.
+Alternatively, by using the standard python logging library as in the example, you can create logging handlers to log the data out to any mechanism you choose (e.g., Kafka, Logstash, etc...)
+
 ### Capabilities during API calls
 
 After wrapping your endpoint with `monitor`, you really don't need to do anything else. When using `create` or `acreate` data will be tracked and monitoring will take place.
 
 There are, however, several capabilities that are added to these functions. Specifically, you can add the following arguments to any create call:
 * MONA_context_id: The unique id of the context in which the call is made. By using this ID you can export more data to Mona to the same context from other places. If not supplied, the "id" field of the OpenAI Endpoint's response will be used as the Mona context ID automatically.
 * MONA_export_timestamp: Can be used to simulate as if the current call was made in a different time, as far as Mona is concerned.
```

#### html2text {}

```diff
@@ -1,51 +1,47 @@
-Metadata-Version: 2.1 Name: mona-openai Version: 0.0.9 Summary: Integration
-client for monitoring OpenAI usage with Mona Author-email: Itai Bar Sinai
-monalabs.io> Project-URL: Homepage, https://github.com/monalabs/mona-openai
-Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
-Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI Classifier: Programming Language
-:: Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.9
-Description-Content-Type: text/markdown License-File: LICENSE # Mona-OpenAI
-Integration Client
+# Mona-OpenAI Integration Client
                                  [Mona's logo]
                    [https://embed-ssl.wistia.com/deliveries/
   c15bb616a389fa7d752968ccb3af2ab4.jpg?wistia-l6xmdj3cd6-1-l6xmdj3cd6-video-
 thumbnail=1&amp;image_play_button_size=2x&amp;image_crop_resized=960x540&amp;image_play_button=1&amp;image_play_button_color=66c7d1e0]
                         OpenAI_GPT_Integration_Tutorial
 Use one line of code to get instant live monitoring for your OpenAI usage
 including: * Tokens usage * Hallucination alerts * Profanity and privacy
 analyses * Behavioral drifts and anomalies * LangChain support * Much much more
-## Setting Up - TODO: Add part about Mona registration with a link to the
-relevant landing page where the reader can sign up. ```console $ pip install
-mona_openai ``` ## Quick Start and Example Example boilerplate code for both
-sync and async usage is given in the file "example_usage.py" and here: ```py
-from os import environ import asyncio import openai from mona_openai import
-monitor openai.api_key = environ.get("OPEN_AI_KEY") MONA_API_KEY = environ.get
-("MONA_API_KEY") MONA_SECRET = environ.get("MONA_SECRET") MONA_CREDS = { "key":
-MONA_API_KEY, "secret": MONA_SECRET, } CONTEXT_CLASS_NAME =
-"SOME_MONITORING_CONTEXT_NAME" monitored_completion = monitor
-( openai.Completion, MONA_CREDS, CONTEXT_CLASS_NAME, ) prompt = "I want to
-generate some text about " model = "text-ada-001" temperature = 0.6 max_tokens
-= 5 n = 1 # Regular (sync) usage response = monitored_completion.create
-( engine=model, prompt=prompt, max_tokens=max_tokens, n=n,
-temperature=temperature, MONA_additional_data={"customer_id": "A531251"}, )
-print(response.choices[0].text) # Async usage response = asyncio.run
-(monitored_completion.acreate( engine=model, prompt=prompt,
-max_tokens=max_tokens, n=n, temperature=temperature, MONA_additional_data=
-{"customer_id": "A531251"}, )) print(response.choices[0].text) ``` ## Supported
-OpenAI APIs Currently this client supports `openai.Completion` and
-`openai.ChatCompletion`. Mona can support processes based on other APIs and
-also non-OpenAI-based apps. If you have a differrent use-case, we'd love to
-hear about it! Please email us at support@monalabs.io. ## Usage ###
-Initialization The main and only function exposed in this package is `monitor`.
-```py import openai from mona_openai import monitor openai.api_key =
-environ.get("OPEN_AI_KEY") monitored_completion = monitor( openai.Completion,
-( environ.get("MONA_API_KEY"), environ.get("MONA_SECRET"), ),
-"SOME_MONITORING_CONTEXT_NAME", {"analysis": {"profanity": False}} ) ...
+## Setting Up ```console $ pip install mona_openai ``` If you plan on using
+Mona as your monitoring service, [sign up for a free account here](https://
+www.monalabs.io/openai-gpt-monitoring). ## Quick Start You can find boilerplate
+code for many use-cases under [the "examples" folder](https://github.com/
+monalabs/mona-openai/tree/main/examples). ```py from os import environ import
+asyncio import openai from mona_openai.loggers import StandardLogger from
+logging import WARNING from mona_openai import monitor, monitor_with_logger
+openai.api_key = environ.get("OPEN_AI_KEY") # When using a standard logger.
+monitored_completion = monitor_with_logger( openai.Completion, StandardLogger
+(WARNING), ) response = monitored_completion.create( model="text-ada-001",
+prompt="I want to generate some text about ", max_tokens=20, n=1,
+temperature=0.2, # Adding additional information for monitoring purposes,
+unrelated to # internal OpenAI call. MONA_additional_data={"customer_id":
+"A531251"}, ) print(response.choices[0].text) # When monitoring with Mona.
+MONA_API_KEY = environ.get("MONA_API_KEY") MONA_SECRET = environ.get
+("MONA_SECRET") MONA_CREDS = { "key": MONA_API_KEY, "secret": MONA_SECRET, }
+CONTEXT_CLASS_NAME = "SOME_MONITORING_CONTEXT_NAME" monitored_completion =
+monitor( openai.Completion, MONA_CREDS, CONTEXT_CLASS_NAME, ) response =
+monitored_completion.create( model="text-ada-001", prompt="I want to generate
+some text about ", max_tokens=20, n=1, temperature=0.2, # Adding additional
+information for monitoring purposes, unrelated to # internal OpenAI call.
+MONA_additional_data={"customer_id": "A531251"}, ) print(response.choices
+[0].text) ``` ## Supported OpenAI APIs Currently this client supports
+`openai.Completion` and `openai.ChatCompletion`. Mona can support processes
+based on other APIs and also non-OpenAI-based apps. If you have a differrent
+use-case, we'd love to hear about it! Please email us at support@monalabs.io.
+## Usage ### Initialization The main and only function exposed in this package
+is `monitor`. ```py import openai from mona_openai import monitor
+openai.api_key = environ.get("OPEN_AI_KEY") monitored_completion = monitor
+( openai.Completion, ( environ.get("MONA_API_KEY"), environ.get("MONA_SECRET"),
+), "SOME_MONITORING_CONTEXT_NAME", {"analysis": {"profanity": False}} ) ...
 monitored_completion.create(...) ``` The `monitor` function returns to you a
 class that wraps the original openai endpoint class you provide, with an
 equivalent API (besides some additions listed below). You can then use the
 returned class' "create" and "acreate" functions just as you would before, only
 now, besides getting the requested openAI functionality, this client will log
 out to Mona's server the parameters you used (e.g., temperature), data about
 the response from OpenAI's server, and custom analyses about the call (e.g.,
@@ -65,73 +61,88 @@
 export_prompt (False): Whether Mona should export the actual prompt text. Be
 default set to False to avoid privacy concerns. * export_response_texts
 (False): Whether Mona should export the actual response texts. Be default set
 to False to avoid privacy concerns. * analysis: A dictionary mapping each
 analysis type to a boolean value telling the client whether or not to run said
 analysis and log it to Mona. Possible options currently are "privacy",
 "profanity", and "textual". By default, all analyses take place and are logged
-out to Mona. ### Capabilities during API calls After wrapping your endpoint
-with `monitor`, you really don't need to do anything else. When using `create`
-or `acreate` data will be tracked and monitoring will take place. There are,
-however, several capabilities that are added to these functions. Specifically,
-you can add the following arguments to any create call: * MONA_context_id: The
-unique id of the context in which the call is made. By using this ID you can
-export more data to Mona to the same context from other places. If not
-supplied, the "id" field of the OpenAI Endpoint's response will be used as the
-Mona context ID automatically. * MONA_export_timestamp: Can be used to simulate
-as if the current call was made in a different time, as far as Mona is
-concerned. * MONA_additional_data: A JSON-serializable dict with any other data
-you want to add to the monitoring context. This comes in handy if you want to
-add more information to the monitoring contex that isn't part of the basic
-OpenAI API call information. For example, if you are using a specific template
-ID or if this call is being made for a specific customer ID, these are fields
-you can add there to help get full context when monitoring with Mona. Example:
-```py response = asyncio.run(monitored_completion.acreate( engine=model,
-prompt=prompt, max_tokens=max_tokens, n=n, temperature=temperature,
-MONA_additional_data={"customer_id": "A531251"}, )) print(response.choices
-[0].text) ``` ### Using OpenAI with REST calls instead of OpenAI's Python
-client In some cases you may choose to use OpenAI's API directly with REST
-calls and not using OpenAI's SDK. For these cases we allow a more direct
-approach for logging to Mona as well, by using the "get_rest_monitor" function.
-See example below. ```py # Direct REST usage, without OpenAI client import
-requests from os import environ from mona_openai import get_rest_monitor
-MONA_API_KEY = environ.get("MONA_API_KEY") MONA_SECRET = environ.get
-("MONA_SECRET") MONA_CREDS = { "key": MONA_API_KEY, "secret": MONA_SECRET, }
-CONTEXT_CLASS_NAME = "SOME_MONITORING_CONTEXT_NAME" # Get Mona logger
-mona_logger = get_rest_monitor( "Completion", MONA_CREDS, CONTEXT_CLASS_NAME, )
-# Set up the API endpoint URL and authentication headers url = "https://
-api.openai.com/v1/completions" headers = { "Content-Type": "application/json",
-"Authorization": f"Bearer {environ.get('OPEN_AI_KEY')}", } # Set up the request
-data data = { "prompt": prompt, "max_tokens": max_tokens, "temperature":
-temperature, "model": model, "n": n, } # The log_request function returns two
-other function for later logging # the response or the exception. When we later
-do that, the logger will # actually calculate all the relevant metrics and will
-send them to # Mona. response_logger, exception_logger =
-mona_logger.log_request( data, additional_data={"customer_id": "A531251"} )
-try: # Send the request to the API response = requests.post(url,
-headers=headers, json=data) # Check for HTTP errors response.raise_for_status()
-# Log response to Mona response_logger(response.json()) print(response.json()
-["choices"][0]["text"]) except Exception as err: # Log exception to Mona
-exception_logger() ``` ### Stream support OpenAI allows receiving responses as
-a stream of tokens using the "stream" parameter. When this is done, Mona will
-collect all the tokens in memory and will create the analysis and log out the
-data the moment the stream is over. You don't need to do anything to make this
-happen. Since for streaming responses OpenAI doesn't supply the full usage
-tokens summary, Mona uses the tiktoken package to calculate the tokens of the
-prompt and completion and log them for monitoring. NOTE: Stream is currently
-only supported with SDK usage, and not with using REST directly. ## LangChain
-support You can use the exported `monitor_langchain_llm` to wrap a LangChain
-OpenAI LLM (chat or normal) with Mona's monitoring capabilities: ```py from
-mona_openai import monitor_langchain_llm from langchain.llms import OpenAI #
-Wrap the LLM object with Mona monitoring. llm = monitor_langchain_llm( OpenAI
-(OPEN_AI_KEY), MONA_CREDS, CONTEXT_CLASS_NAME) ``` See full example in
-completion_langchain.py in the examples folder. ## Mona SDK This package uses
-the mona_sdk package to export the relevant data to Mona. There are several
-environment variables you can use to configure the SDK's behavior. For example,
-you can set it up to raise exceptions when exporting data to Mona fails (it
-doesn't do that by default). ## Monitoring for profanity Mona uses the alt-
-profanity-check pacakge (https://pypi.org/project/alt-profanity-check/) to
-create both boolean predictions and probabilty scores for the existence of
-profanity both in the prompt and in the responses. We use the built in package
-methods for that. If you want, for example, to use a different probability
-threshold for the boolean prediction, you can do that by changing your Mona
-config on the Mona dashboard.
+out to Mona. ### Using custom loggers You don't have to have a Mona account to
+use this package. You can define specific loggers to log out the data to a
+file, memory, or just a given python logger. For example, to log out the
+relevant metrics as WARNING: ```py from os import environ import openai from
+mona_openai.loggers import StandardLogger from logging import WARNING from
+mona_openai import monitor_with_logger openai.api_key = environ.get
+("OPEN_AI_KEY") monitored_completion = monitor_with_logger( openai.Completion,
+StandardLogger(WARNING), ) response = monitored_completion.create( model="text-
+ada-001", prompt="I want to generate some text about ", max_tokens=20, n=1,
+temperature=0.2, # Adding additional information for monitoring purposes,
+unrelated to # internal OpenAI call. MONA_additional_data={"customer_id":
+"A531251"}, ) ``` This SDK provides a simple interface to implement your own
+loggers by inheriting from Logger under loggers/logger.py. Alternatively, by
+using the standard python logging library as in the example, you can create
+logging handlers to log the data out to any mechanism you choose (e.g., Kafka,
+Logstash, etc...) ### Capabilities during API calls After wrapping your
+endpoint with `monitor`, you really don't need to do anything else. When using
+`create` or `acreate` data will be tracked and monitoring will take place.
+There are, however, several capabilities that are added to these functions.
+Specifically, you can add the following arguments to any create call: *
+MONA_context_id: The unique id of the context in which the call is made. By
+using this ID you can export more data to Mona to the same context from other
+places. If not supplied, the "id" field of the OpenAI Endpoint's response will
+be used as the Mona context ID automatically. * MONA_export_timestamp: Can be
+used to simulate as if the current call was made in a different time, as far as
+Mona is concerned. * MONA_additional_data: A JSON-serializable dict with any
+other data you want to add to the monitoring context. This comes in handy if
+you want to add more information to the monitoring contex that isn't part of
+the basic OpenAI API call information. For example, if you are using a specific
+template ID or if this call is being made for a specific customer ID, these are
+fields you can add there to help get full context when monitoring with Mona.
+Example: ```py response = asyncio.run(monitored_completion.acreate
+( engine=model, prompt=prompt, max_tokens=max_tokens, n=n,
+temperature=temperature, MONA_additional_data={"customer_id": "A531251"}, ))
+print(response.choices[0].text) ``` ### Using OpenAI with REST calls instead of
+OpenAI's Python client In some cases you may choose to use OpenAI's API
+directly with REST calls and not using OpenAI's SDK. For these cases we allow a
+more direct approach for logging to Mona as well, by using the
+"get_rest_monitor" function. See example below. ```py # Direct REST usage,
+without OpenAI client import requests from os import environ from mona_openai
+import get_rest_monitor MONA_API_KEY = environ.get("MONA_API_KEY") MONA_SECRET
+= environ.get("MONA_SECRET") MONA_CREDS = { "key": MONA_API_KEY, "secret":
+MONA_SECRET, } CONTEXT_CLASS_NAME = "SOME_MONITORING_CONTEXT_NAME" # Get Mona
+logger mona_logger = get_rest_monitor( "Completion", MONA_CREDS,
+CONTEXT_CLASS_NAME, ) # Set up the API endpoint URL and authentication headers
+url = "https://api.openai.com/v1/completions" headers = { "Content-Type":
+"application/json", "Authorization": f"Bearer {environ.get('OPEN_AI_KEY')}", }
+# Set up the request data data = { "prompt": prompt, "max_tokens": max_tokens,
+"temperature": temperature, "model": model, "n": n, } # The log_request
+function returns two other function for later logging # the response or the
+exception. When we later do that, the logger will # actually calculate all the
+relevant metrics and will send them to # Mona. response_logger,
+exception_logger = mona_logger.log_request( data, additional_data=
+{"customer_id": "A531251"} ) try: # Send the request to the API response =
+requests.post(url, headers=headers, json=data) # Check for HTTP errors
+response.raise_for_status() # Log response to Mona response_logger
+(response.json()) print(response.json()["choices"][0]["text"]) except Exception
+as err: # Log exception to Mona exception_logger() ``` ### Stream support
+OpenAI allows receiving responses as a stream of tokens using the "stream"
+parameter. When this is done, Mona will collect all the tokens in memory and
+will create the analysis and log out the data the moment the stream is over.
+You don't need to do anything to make this happen. Since for streaming
+responses OpenAI doesn't supply the full usage tokens summary, Mona uses the
+tiktoken package to calculate the tokens of the prompt and completion and log
+them for monitoring. NOTE: Stream is currently only supported with SDK usage,
+and not with using REST directly. ## LangChain support You can use the exported
+`monitor_langchain_llm` to wrap a LangChain OpenAI LLM (chat or normal) with
+Mona's monitoring capabilities: ```py from mona_openai import
+monitor_langchain_llm from langchain.llms import OpenAI # Wrap the LLM object
+with Mona monitoring. llm = monitor_langchain_llm( OpenAI(OPEN_AI_KEY),
+MONA_CREDS, CONTEXT_CLASS_NAME) ``` See full example in completion_langchain.py
+in the examples folder. ## Mona SDK This package uses the mona_sdk package to
+export the relevant data to Mona. There are several environment variables you
+can use to configure the SDK's behavior. For example, you can set it up to
+raise exceptions when exporting data to Mona fails (it doesn't do that by
+default). ## Monitoring for profanity Mona uses the alt-profanity-check pacakge
+(https://pypi.org/project/alt-profanity-check/) to create both boolean
+predictions and probabilty scores for the existence of profanity both in the
+prompt and in the responses. We use the built in package methods for that. If
+you want, for example, to use a different probability threshold for the boolean
+prediction, you can do that by changing your Mona config on the Mona dashboard.
```

### Comparing `mona-openai-0.0.9/README.md` & `mona-openai-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: mona-openai
+Version: 0.1.0
+Summary: Integration client for monitoring OpenAI usage with Mona
+Author-email: Itai Bar Sinai <itai@monalabs.io>
+Project-URL: Homepage, https://github.com/monalabs/mona-openai
+Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
+Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Mona-OpenAI Integration Client
 <p align="center">
   <img src="https://github.com/monalabs/mona-sdk/blob/main/mona_logo.png?raw=true" alt="Mona's logo" width="180"/>
 </p>
 
 <p align="center"><a target="_blank" href="https://monalabs.wistia.com/medias/l6xmdj3cd6?wvideo=l6xmdj3cd6"><img src="https://embed-ssl.wistia.com/deliveries/c15bb616a389fa7d752968ccb3af2ab4.jpg?wistia-l6xmdj3cd6-1-l6xmdj3cd6-video-thumbnail=1&amp;image_play_button_size=2x&amp;image_crop_resized=960x540&amp;image_play_button=1&amp;image_play_button_color=66c7d1e0" width="400" height="225" style="width: 400px; height: 225px;"></a></p><p align="center"><a href="https://monalabs.wistia.com/medias/l6xmdj3cd6?wvideo=l6xmdj3cd6">OpenAI GPT Integration Tutorial</a></p>
 
@@ -12,31 +27,57 @@
 * Profanity and privacy analyses
 * Behavioral drifts and anomalies
 * LangChain support
 * Much much more
 
 ## Setting Up
 
-- TODO: Add part about Mona registration with a link to the relevant landing page where the reader can sign up.
 ```console
 $ pip install mona_openai
 ```
 
-## Quick Start and Example
+If you plan on using Mona as your monitoring service, [sign up for a free account here](https://www.monalabs.io/openai-gpt-monitoring).
+
+## Quick Start
+
+You can find boilerplate code for many use-cases under [the "examples" folder](https://github.com/monalabs/mona-openai/tree/main/examples).
 
-Example boilerplate code for both sync and async usage is given in the file "example_usage.py" and here:
 ```py
 from os import environ
 import asyncio
 import openai
+from mona_openai.loggers import StandardLogger
+from logging import WARNING
 
-from mona_openai import monitor
+from mona_openai import monitor, monitor_with_logger
 
 openai.api_key = environ.get("OPEN_AI_KEY")
 
+# When using a standard logger.
+
+monitored_completion = monitor_with_logger(
+    openai.Completion,
+    StandardLogger(WARNING),
+)
+
+response = monitored_completion.create(
+    model="text-ada-001",
+    prompt="I want to generate some text about ",
+    max_tokens=20,
+    n=1,
+    temperature=0.2,
+    # Adding additional information for monitoring purposes, unrelated to
+    # internal OpenAI call.
+    MONA_additional_data={"customer_id": "A531251"},
+)
+print(response.choices[0].text)
+
+
+# When monitoring with Mona.
+
 MONA_API_KEY = environ.get("MONA_API_KEY")
 MONA_SECRET = environ.get("MONA_SECRET")
 MONA_CREDS = {
     "key": MONA_API_KEY,
     "secret": MONA_SECRET,
 }
 CONTEXT_CLASS_NAME = "SOME_MONITORING_CONTEXT_NAME"
@@ -44,43 +85,25 @@
 
 monitored_completion = monitor(
     openai.Completion,
     MONA_CREDS,
     CONTEXT_CLASS_NAME,
 )
 
-
-prompt = "I want to generate some text about "
-model = "text-ada-001"
-temperature = 0.6
-max_tokens = 5
-n = 1
-
-# Regular (sync) usage
 response = monitored_completion.create(
-    engine=model,
-    prompt=prompt,
-    max_tokens=max_tokens,
-    n=n,
-    temperature=temperature,
+    model="text-ada-001",
+    prompt="I want to generate some text about ",
+    max_tokens=20,
+    n=1,
+    temperature=0.2,
+    # Adding additional information for monitoring purposes, unrelated to
+    # internal OpenAI call.
     MONA_additional_data={"customer_id": "A531251"},
 )
 print(response.choices[0].text)
-
-# Async usage
-response = asyncio.run(monitored_completion.acreate(
-    engine=model,
-    prompt=prompt,
-    max_tokens=max_tokens,
-    n=n,
-    temperature=temperature,
-    MONA_additional_data={"customer_id": "A531251"},
-))
-
-print(response.choices[0].text)
 ```
 ## Supported OpenAI APIs
 Currently this client supports `openai.Completion` and `openai.ChatCompletion`. Mona can support processes based on other APIs and also non-OpenAI-based apps.
 If you have a differrent use-case, we'd love to hear about it! Please email us at support@monalabs.io.
 
 ## Usage
 ### Initialization
@@ -121,14 +144,47 @@
 The specs arg allows you to configure what should be monitored. It expects a python dict with the follwoing possible keys:
 * sampling_ratio (1): A number between 0 and 1 for how often should the call be logged.
 * avoid_monitoring_exceptions (False): Whether or not to log out to Mona when there is an OpenAI exception. Default is to track exceptions - and Mona will alert you on things like a jump in number of exceptions
 * export_prompt (False): Whether Mona should export the actual prompt text. Be default set to False to avoid privacy concerns.
 * export_response_texts (False): Whether Mona should export the actual response texts. Be default set to False to avoid privacy concerns.
 * analysis: A dictionary mapping each analysis type to a boolean value telling the client whether or not to run said analysis and log it to Mona. Possible options currently are "privacy", "profanity", and "textual". By default, all analyses take place and are logged out to Mona.
 
+### Using custom loggers
+You don't have to have a Mona account to use this package. You can define specific loggers to log out the data to a file, memory, or just a given python logger. For example, to log out the relevant metrics as WARNING:
+
+```py
+from os import environ
+import openai
+from mona_openai.loggers import StandardLogger
+from logging import WARNING
+
+from mona_openai import monitor_with_logger
+
+openai.api_key = environ.get("OPEN_AI_KEY")
+
+monitored_completion = monitor_with_logger(
+    openai.Completion,
+    StandardLogger(WARNING),
+)
+
+response = monitored_completion.create(
+    model="text-ada-001",
+    prompt="I want to generate some text about ",
+    max_tokens=20,
+    n=1,
+    temperature=0.2,
+    # Adding additional information for monitoring purposes, unrelated to
+    # internal OpenAI call.
+    MONA_additional_data={"customer_id": "A531251"},
+)
+```
+
+This SDK provides a simple interface to implement your own loggers by inheriting from Logger under loggers/logger.py.
+Alternatively, by using the standard python logging library as in the example, you can create logging handlers to log the data out to any mechanism you choose (e.g., Kafka, Logstash, etc...)
+
 ### Capabilities during API calls
 
 After wrapping your endpoint with `monitor`, you really don't need to do anything else. When using `create` or `acreate` data will be tracked and monitoring will take place.
 
 There are, however, several capabilities that are added to these functions. Specifically, you can add the following arguments to any create call:
 * MONA_context_id: The unique id of the context in which the call is made. By using this ID you can export more data to Mona to the same context from other places. If not supplied, the "id" field of the OpenAI Endpoint's response will be used as the Mona context ID automatically.
 * MONA_export_timestamp: Can be used to simulate as if the current call was made in a different time, as far as Mona is concerned.
```

#### html2text {}

```diff
@@ -1,43 +1,55 @@
-# Mona-OpenAI Integration Client
+Metadata-Version: 2.1 Name: mona-openai Version: 0.1.0 Summary: Integration
+client for monitoring OpenAI usage with Mona Author-email: Itai Bar Sinai
+monalabs.io> Project-URL: Homepage, https://github.com/monalabs/mona-openai
+Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
+Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI Classifier: Programming Language
+:: Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent Requires-Python: >=3.9
+Description-Content-Type: text/markdown License-File: LICENSE # Mona-OpenAI
+Integration Client
                                  [Mona's logo]
                    [https://embed-ssl.wistia.com/deliveries/
   c15bb616a389fa7d752968ccb3af2ab4.jpg?wistia-l6xmdj3cd6-1-l6xmdj3cd6-video-
 thumbnail=1&amp;image_play_button_size=2x&amp;image_crop_resized=960x540&amp;image_play_button=1&amp;image_play_button_color=66c7d1e0]
                         OpenAI_GPT_Integration_Tutorial
 Use one line of code to get instant live monitoring for your OpenAI usage
 including: * Tokens usage * Hallucination alerts * Profanity and privacy
 analyses * Behavioral drifts and anomalies * LangChain support * Much much more
-## Setting Up - TODO: Add part about Mona registration with a link to the
-relevant landing page where the reader can sign up. ```console $ pip install
-mona_openai ``` ## Quick Start and Example Example boilerplate code for both
-sync and async usage is given in the file "example_usage.py" and here: ```py
-from os import environ import asyncio import openai from mona_openai import
-monitor openai.api_key = environ.get("OPEN_AI_KEY") MONA_API_KEY = environ.get
-("MONA_API_KEY") MONA_SECRET = environ.get("MONA_SECRET") MONA_CREDS = { "key":
-MONA_API_KEY, "secret": MONA_SECRET, } CONTEXT_CLASS_NAME =
-"SOME_MONITORING_CONTEXT_NAME" monitored_completion = monitor
-( openai.Completion, MONA_CREDS, CONTEXT_CLASS_NAME, ) prompt = "I want to
-generate some text about " model = "text-ada-001" temperature = 0.6 max_tokens
-= 5 n = 1 # Regular (sync) usage response = monitored_completion.create
-( engine=model, prompt=prompt, max_tokens=max_tokens, n=n,
-temperature=temperature, MONA_additional_data={"customer_id": "A531251"}, )
-print(response.choices[0].text) # Async usage response = asyncio.run
-(monitored_completion.acreate( engine=model, prompt=prompt,
-max_tokens=max_tokens, n=n, temperature=temperature, MONA_additional_data=
-{"customer_id": "A531251"}, )) print(response.choices[0].text) ``` ## Supported
-OpenAI APIs Currently this client supports `openai.Completion` and
-`openai.ChatCompletion`. Mona can support processes based on other APIs and
-also non-OpenAI-based apps. If you have a differrent use-case, we'd love to
-hear about it! Please email us at support@monalabs.io. ## Usage ###
-Initialization The main and only function exposed in this package is `monitor`.
-```py import openai from mona_openai import monitor openai.api_key =
-environ.get("OPEN_AI_KEY") monitored_completion = monitor( openai.Completion,
-( environ.get("MONA_API_KEY"), environ.get("MONA_SECRET"), ),
-"SOME_MONITORING_CONTEXT_NAME", {"analysis": {"profanity": False}} ) ...
+## Setting Up ```console $ pip install mona_openai ``` If you plan on using
+Mona as your monitoring service, [sign up for a free account here](https://
+www.monalabs.io/openai-gpt-monitoring). ## Quick Start You can find boilerplate
+code for many use-cases under [the "examples" folder](https://github.com/
+monalabs/mona-openai/tree/main/examples). ```py from os import environ import
+asyncio import openai from mona_openai.loggers import StandardLogger from
+logging import WARNING from mona_openai import monitor, monitor_with_logger
+openai.api_key = environ.get("OPEN_AI_KEY") # When using a standard logger.
+monitored_completion = monitor_with_logger( openai.Completion, StandardLogger
+(WARNING), ) response = monitored_completion.create( model="text-ada-001",
+prompt="I want to generate some text about ", max_tokens=20, n=1,
+temperature=0.2, # Adding additional information for monitoring purposes,
+unrelated to # internal OpenAI call. MONA_additional_data={"customer_id":
+"A531251"}, ) print(response.choices[0].text) # When monitoring with Mona.
+MONA_API_KEY = environ.get("MONA_API_KEY") MONA_SECRET = environ.get
+("MONA_SECRET") MONA_CREDS = { "key": MONA_API_KEY, "secret": MONA_SECRET, }
+CONTEXT_CLASS_NAME = "SOME_MONITORING_CONTEXT_NAME" monitored_completion =
+monitor( openai.Completion, MONA_CREDS, CONTEXT_CLASS_NAME, ) response =
+monitored_completion.create( model="text-ada-001", prompt="I want to generate
+some text about ", max_tokens=20, n=1, temperature=0.2, # Adding additional
+information for monitoring purposes, unrelated to # internal OpenAI call.
+MONA_additional_data={"customer_id": "A531251"}, ) print(response.choices
+[0].text) ``` ## Supported OpenAI APIs Currently this client supports
+`openai.Completion` and `openai.ChatCompletion`. Mona can support processes
+based on other APIs and also non-OpenAI-based apps. If you have a differrent
+use-case, we'd love to hear about it! Please email us at support@monalabs.io.
+## Usage ### Initialization The main and only function exposed in this package
+is `monitor`. ```py import openai from mona_openai import monitor
+openai.api_key = environ.get("OPEN_AI_KEY") monitored_completion = monitor
+( openai.Completion, ( environ.get("MONA_API_KEY"), environ.get("MONA_SECRET"),
+), "SOME_MONITORING_CONTEXT_NAME", {"analysis": {"profanity": False}} ) ...
 monitored_completion.create(...) ``` The `monitor` function returns to you a
 class that wraps the original openai endpoint class you provide, with an
 equivalent API (besides some additions listed below). You can then use the
 returned class' "create" and "acreate" functions just as you would before, only
 now, besides getting the requested openAI functionality, this client will log
 out to Mona's server the parameters you used (e.g., temperature), data about
 the response from OpenAI's server, and custom analyses about the call (e.g.,
@@ -57,73 +69,88 @@
 export_prompt (False): Whether Mona should export the actual prompt text. Be
 default set to False to avoid privacy concerns. * export_response_texts
 (False): Whether Mona should export the actual response texts. Be default set
 to False to avoid privacy concerns. * analysis: A dictionary mapping each
 analysis type to a boolean value telling the client whether or not to run said
 analysis and log it to Mona. Possible options currently are "privacy",
 "profanity", and "textual". By default, all analyses take place and are logged
-out to Mona. ### Capabilities during API calls After wrapping your endpoint
-with `monitor`, you really don't need to do anything else. When using `create`
-or `acreate` data will be tracked and monitoring will take place. There are,
-however, several capabilities that are added to these functions. Specifically,
-you can add the following arguments to any create call: * MONA_context_id: The
-unique id of the context in which the call is made. By using this ID you can
-export more data to Mona to the same context from other places. If not
-supplied, the "id" field of the OpenAI Endpoint's response will be used as the
-Mona context ID automatically. * MONA_export_timestamp: Can be used to simulate
-as if the current call was made in a different time, as far as Mona is
-concerned. * MONA_additional_data: A JSON-serializable dict with any other data
-you want to add to the monitoring context. This comes in handy if you want to
-add more information to the monitoring contex that isn't part of the basic
-OpenAI API call information. For example, if you are using a specific template
-ID or if this call is being made for a specific customer ID, these are fields
-you can add there to help get full context when monitoring with Mona. Example:
-```py response = asyncio.run(monitored_completion.acreate( engine=model,
-prompt=prompt, max_tokens=max_tokens, n=n, temperature=temperature,
-MONA_additional_data={"customer_id": "A531251"}, )) print(response.choices
-[0].text) ``` ### Using OpenAI with REST calls instead of OpenAI's Python
-client In some cases you may choose to use OpenAI's API directly with REST
-calls and not using OpenAI's SDK. For these cases we allow a more direct
-approach for logging to Mona as well, by using the "get_rest_monitor" function.
-See example below. ```py # Direct REST usage, without OpenAI client import
-requests from os import environ from mona_openai import get_rest_monitor
-MONA_API_KEY = environ.get("MONA_API_KEY") MONA_SECRET = environ.get
-("MONA_SECRET") MONA_CREDS = { "key": MONA_API_KEY, "secret": MONA_SECRET, }
-CONTEXT_CLASS_NAME = "SOME_MONITORING_CONTEXT_NAME" # Get Mona logger
-mona_logger = get_rest_monitor( "Completion", MONA_CREDS, CONTEXT_CLASS_NAME, )
-# Set up the API endpoint URL and authentication headers url = "https://
-api.openai.com/v1/completions" headers = { "Content-Type": "application/json",
-"Authorization": f"Bearer {environ.get('OPEN_AI_KEY')}", } # Set up the request
-data data = { "prompt": prompt, "max_tokens": max_tokens, "temperature":
-temperature, "model": model, "n": n, } # The log_request function returns two
-other function for later logging # the response or the exception. When we later
-do that, the logger will # actually calculate all the relevant metrics and will
-send them to # Mona. response_logger, exception_logger =
-mona_logger.log_request( data, additional_data={"customer_id": "A531251"} )
-try: # Send the request to the API response = requests.post(url,
-headers=headers, json=data) # Check for HTTP errors response.raise_for_status()
-# Log response to Mona response_logger(response.json()) print(response.json()
-["choices"][0]["text"]) except Exception as err: # Log exception to Mona
-exception_logger() ``` ### Stream support OpenAI allows receiving responses as
-a stream of tokens using the "stream" parameter. When this is done, Mona will
-collect all the tokens in memory and will create the analysis and log out the
-data the moment the stream is over. You don't need to do anything to make this
-happen. Since for streaming responses OpenAI doesn't supply the full usage
-tokens summary, Mona uses the tiktoken package to calculate the tokens of the
-prompt and completion and log them for monitoring. NOTE: Stream is currently
-only supported with SDK usage, and not with using REST directly. ## LangChain
-support You can use the exported `monitor_langchain_llm` to wrap a LangChain
-OpenAI LLM (chat or normal) with Mona's monitoring capabilities: ```py from
-mona_openai import monitor_langchain_llm from langchain.llms import OpenAI #
-Wrap the LLM object with Mona monitoring. llm = monitor_langchain_llm( OpenAI
-(OPEN_AI_KEY), MONA_CREDS, CONTEXT_CLASS_NAME) ``` See full example in
-completion_langchain.py in the examples folder. ## Mona SDK This package uses
-the mona_sdk package to export the relevant data to Mona. There are several
-environment variables you can use to configure the SDK's behavior. For example,
-you can set it up to raise exceptions when exporting data to Mona fails (it
-doesn't do that by default). ## Monitoring for profanity Mona uses the alt-
-profanity-check pacakge (https://pypi.org/project/alt-profanity-check/) to
-create both boolean predictions and probabilty scores for the existence of
-profanity both in the prompt and in the responses. We use the built in package
-methods for that. If you want, for example, to use a different probability
-threshold for the boolean prediction, you can do that by changing your Mona
-config on the Mona dashboard.
+out to Mona. ### Using custom loggers You don't have to have a Mona account to
+use this package. You can define specific loggers to log out the data to a
+file, memory, or just a given python logger. For example, to log out the
+relevant metrics as WARNING: ```py from os import environ import openai from
+mona_openai.loggers import StandardLogger from logging import WARNING from
+mona_openai import monitor_with_logger openai.api_key = environ.get
+("OPEN_AI_KEY") monitored_completion = monitor_with_logger( openai.Completion,
+StandardLogger(WARNING), ) response = monitored_completion.create( model="text-
+ada-001", prompt="I want to generate some text about ", max_tokens=20, n=1,
+temperature=0.2, # Adding additional information for monitoring purposes,
+unrelated to # internal OpenAI call. MONA_additional_data={"customer_id":
+"A531251"}, ) ``` This SDK provides a simple interface to implement your own
+loggers by inheriting from Logger under loggers/logger.py. Alternatively, by
+using the standard python logging library as in the example, you can create
+logging handlers to log the data out to any mechanism you choose (e.g., Kafka,
+Logstash, etc...) ### Capabilities during API calls After wrapping your
+endpoint with `monitor`, you really don't need to do anything else. When using
+`create` or `acreate` data will be tracked and monitoring will take place.
+There are, however, several capabilities that are added to these functions.
+Specifically, you can add the following arguments to any create call: *
+MONA_context_id: The unique id of the context in which the call is made. By
+using this ID you can export more data to Mona to the same context from other
+places. If not supplied, the "id" field of the OpenAI Endpoint's response will
+be used as the Mona context ID automatically. * MONA_export_timestamp: Can be
+used to simulate as if the current call was made in a different time, as far as
+Mona is concerned. * MONA_additional_data: A JSON-serializable dict with any
+other data you want to add to the monitoring context. This comes in handy if
+you want to add more information to the monitoring contex that isn't part of
+the basic OpenAI API call information. For example, if you are using a specific
+template ID or if this call is being made for a specific customer ID, these are
+fields you can add there to help get full context when monitoring with Mona.
+Example: ```py response = asyncio.run(monitored_completion.acreate
+( engine=model, prompt=prompt, max_tokens=max_tokens, n=n,
+temperature=temperature, MONA_additional_data={"customer_id": "A531251"}, ))
+print(response.choices[0].text) ``` ### Using OpenAI with REST calls instead of
+OpenAI's Python client In some cases you may choose to use OpenAI's API
+directly with REST calls and not using OpenAI's SDK. For these cases we allow a
+more direct approach for logging to Mona as well, by using the
+"get_rest_monitor" function. See example below. ```py # Direct REST usage,
+without OpenAI client import requests from os import environ from mona_openai
+import get_rest_monitor MONA_API_KEY = environ.get("MONA_API_KEY") MONA_SECRET
+= environ.get("MONA_SECRET") MONA_CREDS = { "key": MONA_API_KEY, "secret":
+MONA_SECRET, } CONTEXT_CLASS_NAME = "SOME_MONITORING_CONTEXT_NAME" # Get Mona
+logger mona_logger = get_rest_monitor( "Completion", MONA_CREDS,
+CONTEXT_CLASS_NAME, ) # Set up the API endpoint URL and authentication headers
+url = "https://api.openai.com/v1/completions" headers = { "Content-Type":
+"application/json", "Authorization": f"Bearer {environ.get('OPEN_AI_KEY')}", }
+# Set up the request data data = { "prompt": prompt, "max_tokens": max_tokens,
+"temperature": temperature, "model": model, "n": n, } # The log_request
+function returns two other function for later logging # the response or the
+exception. When we later do that, the logger will # actually calculate all the
+relevant metrics and will send them to # Mona. response_logger,
+exception_logger = mona_logger.log_request( data, additional_data=
+{"customer_id": "A531251"} ) try: # Send the request to the API response =
+requests.post(url, headers=headers, json=data) # Check for HTTP errors
+response.raise_for_status() # Log response to Mona response_logger
+(response.json()) print(response.json()["choices"][0]["text"]) except Exception
+as err: # Log exception to Mona exception_logger() ``` ### Stream support
+OpenAI allows receiving responses as a stream of tokens using the "stream"
+parameter. When this is done, Mona will collect all the tokens in memory and
+will create the analysis and log out the data the moment the stream is over.
+You don't need to do anything to make this happen. Since for streaming
+responses OpenAI doesn't supply the full usage tokens summary, Mona uses the
+tiktoken package to calculate the tokens of the prompt and completion and log
+them for monitoring. NOTE: Stream is currently only supported with SDK usage,
+and not with using REST directly. ## LangChain support You can use the exported
+`monitor_langchain_llm` to wrap a LangChain OpenAI LLM (chat or normal) with
+Mona's monitoring capabilities: ```py from mona_openai import
+monitor_langchain_llm from langchain.llms import OpenAI # Wrap the LLM object
+with Mona monitoring. llm = monitor_langchain_llm( OpenAI(OPEN_AI_KEY),
+MONA_CREDS, CONTEXT_CLASS_NAME) ``` See full example in completion_langchain.py
+in the examples folder. ## Mona SDK This package uses the mona_sdk package to
+export the relevant data to Mona. There are several environment variables you
+can use to configure the SDK's behavior. For example, you can set it up to
+raise exceptions when exporting data to Mona fails (it doesn't do that by
+default). ## Monitoring for profanity Mona uses the alt-profanity-check pacakge
+(https://pypi.org/project/alt-profanity-check/) to create both boolean
+predictions and probabilty scores for the existence of profanity both in the
+prompt and in the responses. We use the built in package methods for that. If
+you want, for example, to use a different probability threshold for the boolean
+prediction, you can do that by changing your Mona config on the Mona dashboard.
```

### Comparing `mona-openai-0.0.9/mona_openai/analysis/privacy.py` & `mona-openai-0.1.0/mona_openai/analysis/privacy.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/mona_openai/analysis/textual.py` & `mona-openai-0.1.0/mona_openai/analysis/textual.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/mona_openai/endpoints/chat_completion.py` & `mona-openai-0.1.0/mona_openai/endpoints/chat_completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/mona_openai/endpoints/completion.py` & `mona-openai-0.1.0/mona_openai/endpoints/completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/mona_openai/endpoints/endpoint_wrapping.py` & `mona-openai-0.1.0/mona_openai/endpoints/endpoint_wrapping.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/mona_openai/endpoints/wrapping_getter.py` & `mona-openai-0.1.0/mona_openai/endpoints/wrapping_getter.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/mona_openai/mona_client.py` & `mona-openai-0.1.0/mona_openai/loggers/mona_logger/mona_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from mona_sdk.client import Client
 from mona_sdk.async_client import AsyncClient
 
-from .exceptions import InvalidMonaCredsException
+from ...exceptions import InvalidMonaCredsException
 
 
 MONA_API_KEY_KEY = "key"
 MONA_API_SECRET_KEY = "secret"
 
 
 def get_mona_clients(creds):
```

### Comparing `mona-openai-0.0.9/mona_openai/mona_openai.py` & `mona-openai-0.1.0/mona_openai/mona_openai.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import time
-import logging
+from .loggers.mona_logger.mona_logger import MonaLogger
 from copy import deepcopy
 from types import MappingProxyType
 
-from mona_sdk import MonaSingleMessage
-
 from .exceptions import InvalidLagnchainLLMException
 from .endpoints.wrapping_getter import get_endpoint_wrapping
-from .mona_client import get_mona_clients
+from .loggers.mona_logger.mona_client import get_mona_clients
 from .util.func_util import add_conditional_sampling
 from .util.async_util import (
     run_in_an_event_loop,
     call_non_blocking_sync_or_async,
 )
 from .util.openai_util import get_model_param
 from .util.tokens_util import get_usage
@@ -22,32 +20,29 @@
 
 MONA_ARGS_PREFIX = "MONA_"
 CONTEXT_ID_ARG_NAME = MONA_ARGS_PREFIX + "context_id"
 EXPORT_TIMESTAMP_ARG_NAME = MONA_ARGS_PREFIX + "export_timestamp"
 ADDITIONAL_DATA_ARG_NAME = MONA_ARGS_PREFIX + "additional_data"
 
 
-def _get_mona_single_message(
+def _get_logging_message(
     api_name,
     request_input,
     start_time,
     is_exception,
     is_async,
     stream_start_time,
     response,
     analysis_getter,
-    context_class,
     message_cleaner,
     additional_data,
-    context_id,
-    export_timestamp,
 ):
     """
-    Returns a MonaSingleMessage object to be used for data
-    exporting to Mona's servers by a Mona client.
+    Returns a dict object containing all the monitoring analysis to be used
+    for data logging.
     """
 
     message = {
         "input": request_input,
         "latency": time.time() - start_time,
         "stream_start_latency": stream_start_time - start_time
         if stream_start_time is not None
@@ -60,68 +55,66 @@
     if additional_data:
         message["additional_data"] = additional_data
 
     if response:
         message["response"] = response
         message["analysis"] = analysis_getter(request_input, response)
 
-    message = message_cleaner(message)
-
-    return MonaSingleMessage(
-        message=message,
-        contextClass=context_class,
-        contextId=context_id,
-        exportTimestamp=export_timestamp,
-    )
-
-
-def _init_mona_class(client, context_class_name, openai_endpoint_name):
-    response = client.create_openai_context_class(
-        context_class_name, openai_endpoint_name
-    )
-    error_message = response.get("error_message")
-    if error_message:
-        logging.warning(
-            f"Problem initializing Mona context class '{context_class_name}':"
-            f" {error_message}"
-        )
-    else:
-        logging.info(
-            f"Made sure Mona context class '{context_class_name}' "
-            "is initialised"
-        )
-    return response
+    return message_cleaner(message)
 
 
 # TODO(itai): Consider creating some sturct (as NamedTuple or dataclass) for
 #   the specs param.
 
 
 def monitor(
     openai_class,
     mona_creds,
     context_class,
     specs=EMPTY_DICT,
     mona_clients_getter=get_mona_clients,
 ):
     """
-    Returns a Wrapped version of a given OpenAI class with mona
-    monitoring logic.
-    This is the main exposed function of the mona_openai package and
-    probably the only thing you need to use from this package.
+    A simple wrapper around "monitor_with_logger" to use with a Mona logger.
+    See "monitor_with_logger" for full documentation.
+
+    Args:
+        openai_class: An OpenAI API class to wrap with monitoring
+            capabilties.
+        mona_creds: Either a dict or pair of Mona API key and secret to
+            set up Mona's clients from its SDK
+        context_class: The Mona context class name to use for
+            monitoring. Use a name of your choice.
+        specs: A dictionary of specifications such as monitoring
+            sampling ratio.
+        mona_clients_getter: Used only for testing purposes.
+    """
+    return monitor_with_logger(
+        openai_class,
+        MonaLogger(mona_creds, context_class, mona_clients_getter),
+        specs,
+    )
+
+
+def monitor_with_logger(openai_class, logger, specs=EMPTY_DICT):
+    """
+    Returns a Wrapped version of a given OpenAI class with monitoring logic.
 
     You can use the returned class' "create" and "acreate" functions
     exactly as you would the original class, and monitoring will be
     taken care of for you.
 
     This client will automatically monitor for you things like latency,
     prompt and response lengths, number of tokens, etc., along with any
     endpoint parameter usage (e.g., it tracks the "temperature" and
     "max_tokens" params you use).
 
+    The logic for what to do with the calculated analysis data is set by the
+    given logger object.
+
     You can also add other named args when calling "create" or
     "acreate" by using a new named argument called
     "MONA_additional_data" and set it to any JSON serializable
     dictionary.
     This allows you to add metadata about the call such as a prompt
     template ID, information about the context in which the API call is
     made, etc...
@@ -132,132 +125,116 @@
             is made. By using this ID you can export more data to Mona
             to the same context from other places. If not used, the
             "id" field of the OpenAI Endpoint's response will be used.
         MONA_export_timestamp: Can be used to simulate as if the
             current call was made in a different time, as far as Mona
             is concerned.
 
-    The returned monitored class also exposes a new class method called
-    "get_mona_clients", which allows you to retrieve the clients and
-    use them to export more data or communicate directly with Mona's
-    API
-
-    Read more about Mona and how to use it in Mona's docs on
-    https://docs.monalabs.io.
-
     Args:
         openai_class: An OpenAI API class to wrap with monitoring
             capabilties.
-        mona_creds: Either a dict or pair of Mona API key and secret to
-            set up Mona's clients from its SDK
-        context_class: The Mona context class name to use for
-            monitoring. Use a name of your choice.
+        logger: A logger object used to log out the calculated analysis.
         specs: A dictionary of specifications such as monitoring
             sampling ratio.
-        mona_clients_getter: Used only for testing purposes
     """
-    client, async_client = mona_clients_getter(mona_creds)
 
     sampling_ratio = validate_and_get_sampling_ratio(specs)
 
     base_class = get_endpoint_wrapping(
         openai_class.__name__, specs
     ).wrap_class(openai_class)
 
-    _init_mona_class(client, context_class, openai_class.__name__)
+    logger.start_monitoring(openai_class.__name__)
 
     # TODO(itai): Add call to Mona servers to init the context class if it
     #   isn't inited yet once we have the relevant endpoint for this.
 
     class MonitoredOpenAI(base_class):
         """
-        A mona-monitored version of an openai API class.
+        A monitored version of an openai API class.
         """
 
         @classmethod
-        def _get_mona_single_message(
+        def _get_logging_message(
             cls,
             kwargs_param,
             start_time,
             is_exception,
             is_async,
             stream_start_time,
             response,
         ):
             """
-            Returns a MonaSingleMessage object to be used for data
-            exporting to Mona's servers by a Mona client.
+            Returns a dict to be used for data logging.
             """
             # Recreate the input dict to avoid manipulating the caller's data,
             # and remove Mona-related data.
             request_input = deepcopy(
                 {
                     x: kwargs_param[x]
                     for x in kwargs_param
                     if not x.startswith(MONA_ARGS_PREFIX)
                 }
             )
 
-            return _get_mona_single_message(
+            return _get_logging_message(
                 api_name=openai_class.__name__,
                 request_input=request_input,
                 start_time=start_time,
                 is_exception=is_exception,
                 is_async=is_async,
                 stream_start_time=stream_start_time,
                 response=response,
                 analysis_getter=super()._get_full_analysis,
-                context_class=context_class,
                 message_cleaner=super()._get_clean_message,
                 additional_data=kwargs_param.get(ADDITIONAL_DATA_ARG_NAME),
-                context_id=kwargs_param.get(
-                    CONTEXT_ID_ARG_NAME, response["id"] if response else None
-                ),
-                export_timestamp=kwargs_param.get(
-                    EXPORT_TIMESTAMP_ARG_NAME, start_time
-                ),
             )
 
         @classmethod
         async def _inner_create(
             cls, export_function, super_function, args, kwargs
         ):
             """
-            The main logic for wrapping create functions with mona data
-            exporting.
+            The main logic for wrapping create functions with monitoring data
+            logging.
             This internal function porovides a template for both sync
             and async activations (helps with wrapping both "create"
             and "acreate").
             """
 
             is_stream = kwargs.get("stream", False)
             is_async = super_function.__name__ == "acreate"
 
             response = None
 
             # will be used only when stream is enabled
             stream_start_time = None
 
-            async def _inner_mona_export(is_exception):
+            async def _inner_log_message(is_exception):
                 return await call_non_blocking_sync_or_async(
                     export_function,
                     (
-                        cls._get_mona_single_message(
+                        cls._get_logging_message(
                             kwargs,
                             start_time,
                             is_exception,
                             is_async,
                             stream_start_time,
                             response,
                         ),
+                        kwargs.get(
+                            CONTEXT_ID_ARG_NAME,
+                            response["id"] if response else None,
+                        ),
+                        kwargs.get(EXPORT_TIMESTAMP_ARG_NAME, start_time),
                     ),
                 )
 
-            mona_export = add_conditional_sampling(
-                _inner_mona_export, sampling_ratio
+            log_message = add_conditional_sampling(
+                _inner_log_message, sampling_ratio
             )
 
             start_time = time.time()
 
             async def inner_super_function():
                 # Call the actual openai create function without the Mona
                 # specific arguments.
@@ -269,24 +246,24 @@
                         for x in kwargs
                         if not x.startswith(MONA_ARGS_PREFIX)
                     },
                 )
 
             async def inner_handle_exception():
                 if not specs.get("avoid_monitoring_exceptions", False):
-                    await mona_export(True)
+                    await log_message(True)
 
             if not is_stream:
                 try:
                     response = await inner_super_function()
                 except Exception:
                     await inner_handle_exception()
                     raise
 
-                await mona_export(False)
+                await log_message(False)
 
                 return response
 
             # From here it's stream handling.
 
             async def _stream_done_callback(
                 final_response, actual_stream_start_time
@@ -301,15 +278,15 @@
                         prompt_texts=base_class._get_all_prompt_texts(kwargs),
                         response_texts=base_class._get_all_response_texts(
                             final_response
                         ),
                     )
                 }
                 stream_start_time = actual_stream_start_time
-                await mona_export(False)
+                await log_message(False)
 
             try:
                 # Call the actual openai create function without the Mona
                 # specific arguments.
                 return ResponseGatheringIterator(
                     original_iterator=await inner_super_function(),
                     delta_choice_text_getter=(
@@ -322,155 +299,159 @@
             except Exception:
                 await inner_handle_exception()
                 raise
 
         @classmethod
         def create(cls, *args, **kwargs):
             """
-            A mona-monitored version of the openai base class' "create"
+            A monitored version of the openai base class' "create"
             function.
             """
             return run_in_an_event_loop(
-                cls._inner_create(client.export, super().create, args, kwargs)
+                cls._inner_create(logger.log, super().create, args, kwargs)
             )
 
         @classmethod
         async def acreate(cls, *args, **kwargs):
             """
-            An async mona-monitored version of the openai base class'
+            An async monitored version of the openai base class'
             "acreate" function.
             """
             return await cls._inner_create(
-                async_client.export_async, super().acreate, args, kwargs
+                logger.alog, super().acreate, args, kwargs
             )
 
-        @classmethod
-        def get_mona_clients(cls):
-            """
-            Returns the two Mona clients this class works with to allow
-            exporting more data or communicating directly with Mona's
-            API.
-            """
-            return (client, async_client)
-
     return type(base_class.__name__, (MonitoredOpenAI,), {})
 
 
 def get_rest_monitor(
-    # TODO(itai): Consider understanding endpoint name from complete url.
     openai_endpoint_name,
     mona_creds,
     context_class,
     specs=EMPTY_DICT,
     mona_clients_getter=get_mona_clients,
 ):
     """
+    A wrapper around get_rest_monitor_with_logger that automatically uses
+    a Mona logger.
+    """
+    return get_rest_monitor_with_logger(
+        openai_endpoint_name,
+        MonaLogger(mona_creds, context_class, mona_clients_getter),
+        specs,
+    )
+
+
+def get_rest_monitor_with_logger(
+    # TODO(itai): Consider understanding endpoint name from complete url.
+    openai_endpoint_name,
+    logger,
+    specs=EMPTY_DICT,
+):
+    """
     Returns a client class for monitoring OpenAI REST calls not done
     using the OpenAI python client (e.g., for Azure users using their
     endpoints directly). This isn't a wrapper for any http requesting
     library and doesn't call the OpenAI API for you - it's just an easy
     logging client to log requests, responses and exceptions.
     """
 
-    client, async_client = mona_clients_getter(mona_creds)
-
-    _init_mona_class(client, context_class, openai_endpoint_name)
+    logger.start_monitoring(openai_endpoint_name)
 
     sampling_ratio = validate_and_get_sampling_ratio(specs)
 
     wrapping_logic = get_endpoint_wrapping(openai_endpoint_name, specs)
 
     class RestClient:
         """
-        This will be the returned Mona logging class. We follow
+        This will be the returned monitoring class. We follow
         OpenAI's way of doing things by using a static classe with
         relevant class methods.
         """
 
         @classmethod
         def _inner_log_request(
             cls,
-            mona_export_function,
+            message_logging_function,
             request_dict,
             additional_data=None,
             context_id=None,
             export_timestamp=None,
         ):
             """
             Actual logic for logging requests, responses and exceptions.
             """
             start_time = time.time()
 
             inner_response = None
 
-            def _inner_mona_export(is_exception):
-                return mona_export_function(
-                    _get_mona_single_message(
+            def _inner_log_message(is_exception):
+                return message_logging_function(
+                    _get_logging_message(
                         api_name=openai_endpoint_name,
                         request_input=request_dict,
                         start_time=start_time,
                         is_exception=is_exception,
                         is_async=False,
                         # TODO(itai): Support stream in REST as well.
                         stream_start_time=None,
                         response=inner_response,
                         analysis_getter=wrapping_logic.get_full_analysis,
-                        context_class=context_class,
                         message_cleaner=wrapping_logic.get_clean_message,
                         additional_data=additional_data,
-                        context_id=context_id,
-                        export_timestamp=export_timestamp,
-                    )
+                    ),
+                    context_id,
+                    export_timestamp,
                 )
 
-            mona_export = add_conditional_sampling(
-                _inner_mona_export, sampling_ratio
+            log_message = add_conditional_sampling(
+                _inner_log_message, sampling_ratio
             )
 
             def log_response(response):
                 """
                 Only when this function is called, will data be logged
-                out to Mona. This function should be called with a
+                out. This function should be called with a
                 response object from the OpenAI API as close as
                 possible to when it is received to allow accurate
                 latency logging.
                 """
                 nonlocal inner_response
                 inner_response = response
-                return mona_export(False)
+                return log_message(False)
 
             def log_exception():
-                return mona_export(True)
+                return log_message(True)
 
             return log_response, log_exception
 
         @classmethod
         def log_request(
             cls,
             request_dict,
             additional_data=None,
             context_id=None,
             export_timestamp=None,
         ):
             """
-            Sets up mona logging for OpenAI request/response objects.
+            Sets up logging for OpenAI request/response objects.
 
             This function should be called with a request data dict,
             for example, what you would use as "json" when using
             "requests" to post.
 
             It returns a response logging function to be used with the
             response object, as well as an exception logging function in case
             of exceptions.
 
-            Note that this call does not log anything to Mona until one of the
+            Note that this call does not log anything until one of the
             returned callbacks is called.
             """
             return cls._inner_log_request(
-                client.export,
+                logger.log,
                 request_dict,
                 additional_data,
                 context_id,
                 export_timestamp,
             )
 
         @classmethod
@@ -482,41 +463,49 @@
             export_timestamp=None,
         ):
             """
             Async version of "log_request". See function's docstring for more
             details.
             """
             return cls._inner_log_request(
-                async_client.export_async,
+                logger.alog,
                 request_dict,
                 additional_data,
                 context_id,
                 export_timestamp,
             )
 
-        @classmethod
-        def get_mona_clients(cls):
-            """
-            Returns the two Mona client this class works with to allow
-            exporting more data or communicating directly with Mona's
-            API.
-            """
-            return client, async_client
-
     return RestClient
 
 
+def _validate_langchain_llm(llm):
+    if not hasattr(llm, "client"):
+        raise InvalidLagnchainLLMException(
+            "LLM has no client attribute - must be an OpenAI LLM"
+        )
+
+
 def monitor_langchain_llm(
     llm,
     mona_creds,
     context_class,
     specs=EMPTY_DICT,
     mona_clients_getter=get_mona_clients,
 ):
-    if not hasattr(llm, "client"):
-        raise InvalidLagnchainLLMException(
-            "LLM has no client attribute - must be an OpenAI LLM"
-        )
+    """
+    Wraps given llm with automatic mona-monitoring logic.
+    """
+    _validate_langchain_llm(llm)
     llm.client = monitor(
         llm.client, mona_creds, context_class, specs, mona_clients_getter
     )
     return llm
+
+
+def monitor_langchain_llm_with_logger(llm, logger, specs=EMPTY_DICT):
+    """
+    Wraps given llm with monitoring logic, logging the analysis with the given
+    logger.
+    """
+    _validate_langchain_llm(llm)
+    llm.client = monitor(llm.client, logger, specs)
+    return llm
```

### Comparing `mona-openai-0.0.9/mona_openai/util/async_util.py` & `mona-openai-0.1.0/mona_openai/util/async_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/mona_openai/util/func_util.py` & `mona-openai-0.1.0/mona_openai/util/func_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/mona_openai/util/oop_util.py` & `mona-openai-0.1.0/mona_openai/util/oop_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/mona_openai/util/stream_util.py` & `mona-openai-0.1.0/mona_openai/util/stream_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/mona_openai/util/tokens_util.py` & `mona-openai-0.1.0/mona_openai/util/tokens_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/mona_openai/util/validation_util.py` & `mona-openai-0.1.0/mona_openai/util/validation_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/mona_openai.egg-info/PKG-INFO` & `mona-openai-0.1.0/mona_openai.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mona-openai
-Version: 0.0.9
+Version: 0.1.0
 Summary: Integration client for monitoring OpenAI usage with Mona
 Author-email: Itai Bar Sinai <itai@monalabs.io>
 Project-URL: Homepage, https://github.com/monalabs/mona-openai
 Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
 Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -27,31 +27,57 @@
 * Profanity and privacy analyses
 * Behavioral drifts and anomalies
 * LangChain support
 * Much much more
 
 ## Setting Up
 
-- TODO: Add part about Mona registration with a link to the relevant landing page where the reader can sign up.
 ```console
 $ pip install mona_openai
 ```
 
-## Quick Start and Example
+If you plan on using Mona as your monitoring service, [sign up for a free account here](https://www.monalabs.io/openai-gpt-monitoring).
+
+## Quick Start
+
+You can find boilerplate code for many use-cases under [the "examples" folder](https://github.com/monalabs/mona-openai/tree/main/examples).
 
-Example boilerplate code for both sync and async usage is given in the file "example_usage.py" and here:
 ```py
 from os import environ
 import asyncio
 import openai
+from mona_openai.loggers import StandardLogger
+from logging import WARNING
 
-from mona_openai import monitor
+from mona_openai import monitor, monitor_with_logger
 
 openai.api_key = environ.get("OPEN_AI_KEY")
 
+# When using a standard logger.
+
+monitored_completion = monitor_with_logger(
+    openai.Completion,
+    StandardLogger(WARNING),
+)
+
+response = monitored_completion.create(
+    model="text-ada-001",
+    prompt="I want to generate some text about ",
+    max_tokens=20,
+    n=1,
+    temperature=0.2,
+    # Adding additional information for monitoring purposes, unrelated to
+    # internal OpenAI call.
+    MONA_additional_data={"customer_id": "A531251"},
+)
+print(response.choices[0].text)
+
+
+# When monitoring with Mona.
+
 MONA_API_KEY = environ.get("MONA_API_KEY")
 MONA_SECRET = environ.get("MONA_SECRET")
 MONA_CREDS = {
     "key": MONA_API_KEY,
     "secret": MONA_SECRET,
 }
 CONTEXT_CLASS_NAME = "SOME_MONITORING_CONTEXT_NAME"
@@ -59,43 +85,25 @@
 
 monitored_completion = monitor(
     openai.Completion,
     MONA_CREDS,
     CONTEXT_CLASS_NAME,
 )
 
-
-prompt = "I want to generate some text about "
-model = "text-ada-001"
-temperature = 0.6
-max_tokens = 5
-n = 1
-
-# Regular (sync) usage
 response = monitored_completion.create(
-    engine=model,
-    prompt=prompt,
-    max_tokens=max_tokens,
-    n=n,
-    temperature=temperature,
+    model="text-ada-001",
+    prompt="I want to generate some text about ",
+    max_tokens=20,
+    n=1,
+    temperature=0.2,
+    # Adding additional information for monitoring purposes, unrelated to
+    # internal OpenAI call.
     MONA_additional_data={"customer_id": "A531251"},
 )
 print(response.choices[0].text)
-
-# Async usage
-response = asyncio.run(monitored_completion.acreate(
-    engine=model,
-    prompt=prompt,
-    max_tokens=max_tokens,
-    n=n,
-    temperature=temperature,
-    MONA_additional_data={"customer_id": "A531251"},
-))
-
-print(response.choices[0].text)
 ```
 ## Supported OpenAI APIs
 Currently this client supports `openai.Completion` and `openai.ChatCompletion`. Mona can support processes based on other APIs and also non-OpenAI-based apps.
 If you have a differrent use-case, we'd love to hear about it! Please email us at support@monalabs.io.
 
 ## Usage
 ### Initialization
@@ -136,14 +144,47 @@
 The specs arg allows you to configure what should be monitored. It expects a python dict with the follwoing possible keys:
 * sampling_ratio (1): A number between 0 and 1 for how often should the call be logged.
 * avoid_monitoring_exceptions (False): Whether or not to log out to Mona when there is an OpenAI exception. Default is to track exceptions - and Mona will alert you on things like a jump in number of exceptions
 * export_prompt (False): Whether Mona should export the actual prompt text. Be default set to False to avoid privacy concerns.
 * export_response_texts (False): Whether Mona should export the actual response texts. Be default set to False to avoid privacy concerns.
 * analysis: A dictionary mapping each analysis type to a boolean value telling the client whether or not to run said analysis and log it to Mona. Possible options currently are "privacy", "profanity", and "textual". By default, all analyses take place and are logged out to Mona.
 
+### Using custom loggers
+You don't have to have a Mona account to use this package. You can define specific loggers to log out the data to a file, memory, or just a given python logger. For example, to log out the relevant metrics as WARNING:
+
+```py
+from os import environ
+import openai
+from mona_openai.loggers import StandardLogger
+from logging import WARNING
+
+from mona_openai import monitor_with_logger
+
+openai.api_key = environ.get("OPEN_AI_KEY")
+
+monitored_completion = monitor_with_logger(
+    openai.Completion,
+    StandardLogger(WARNING),
+)
+
+response = monitored_completion.create(
+    model="text-ada-001",
+    prompt="I want to generate some text about ",
+    max_tokens=20,
+    n=1,
+    temperature=0.2,
+    # Adding additional information for monitoring purposes, unrelated to
+    # internal OpenAI call.
+    MONA_additional_data={"customer_id": "A531251"},
+)
+```
+
+This SDK provides a simple interface to implement your own loggers by inheriting from Logger under loggers/logger.py.
+Alternatively, by using the standard python logging library as in the example, you can create logging handlers to log the data out to any mechanism you choose (e.g., Kafka, Logstash, etc...)
+
 ### Capabilities during API calls
 
 After wrapping your endpoint with `monitor`, you really don't need to do anything else. When using `create` or `acreate` data will be tracked and monitoring will take place.
 
 There are, however, several capabilities that are added to these functions. Specifically, you can add the following arguments to any create call:
 * MONA_context_id: The unique id of the context in which the call is made. By using this ID you can export more data to Mona to the same context from other places. If not supplied, the "id" field of the OpenAI Endpoint's response will be used as the Mona context ID automatically.
 * MONA_export_timestamp: Can be used to simulate as if the current call was made in a different time, as far as Mona is concerned.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mona-openai Version: 0.0.9 Summary: Integration
+Metadata-Version: 2.1 Name: mona-openai Version: 0.1.0 Summary: Integration
 client for monitoring OpenAI usage with Mona Author-email: Itai Bar Sinai
 monalabs.io> Project-URL: Homepage, https://github.com/monalabs/mona-openai
 Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
 Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown License-File: LICENSE # Mona-OpenAI
@@ -11,41 +11,45 @@
                    [https://embed-ssl.wistia.com/deliveries/
   c15bb616a389fa7d752968ccb3af2ab4.jpg?wistia-l6xmdj3cd6-1-l6xmdj3cd6-video-
 thumbnail=1&amp;image_play_button_size=2x&amp;image_crop_resized=960x540&amp;image_play_button=1&amp;image_play_button_color=66c7d1e0]
                         OpenAI_GPT_Integration_Tutorial
 Use one line of code to get instant live monitoring for your OpenAI usage
 including: * Tokens usage * Hallucination alerts * Profanity and privacy
 analyses * Behavioral drifts and anomalies * LangChain support * Much much more
-## Setting Up - TODO: Add part about Mona registration with a link to the
-relevant landing page where the reader can sign up. ```console $ pip install
-mona_openai ``` ## Quick Start and Example Example boilerplate code for both
-sync and async usage is given in the file "example_usage.py" and here: ```py
-from os import environ import asyncio import openai from mona_openai import
-monitor openai.api_key = environ.get("OPEN_AI_KEY") MONA_API_KEY = environ.get
-("MONA_API_KEY") MONA_SECRET = environ.get("MONA_SECRET") MONA_CREDS = { "key":
-MONA_API_KEY, "secret": MONA_SECRET, } CONTEXT_CLASS_NAME =
-"SOME_MONITORING_CONTEXT_NAME" monitored_completion = monitor
-( openai.Completion, MONA_CREDS, CONTEXT_CLASS_NAME, ) prompt = "I want to
-generate some text about " model = "text-ada-001" temperature = 0.6 max_tokens
-= 5 n = 1 # Regular (sync) usage response = monitored_completion.create
-( engine=model, prompt=prompt, max_tokens=max_tokens, n=n,
-temperature=temperature, MONA_additional_data={"customer_id": "A531251"}, )
-print(response.choices[0].text) # Async usage response = asyncio.run
-(monitored_completion.acreate( engine=model, prompt=prompt,
-max_tokens=max_tokens, n=n, temperature=temperature, MONA_additional_data=
-{"customer_id": "A531251"}, )) print(response.choices[0].text) ``` ## Supported
-OpenAI APIs Currently this client supports `openai.Completion` and
-`openai.ChatCompletion`. Mona can support processes based on other APIs and
-also non-OpenAI-based apps. If you have a differrent use-case, we'd love to
-hear about it! Please email us at support@monalabs.io. ## Usage ###
-Initialization The main and only function exposed in this package is `monitor`.
-```py import openai from mona_openai import monitor openai.api_key =
-environ.get("OPEN_AI_KEY") monitored_completion = monitor( openai.Completion,
-( environ.get("MONA_API_KEY"), environ.get("MONA_SECRET"), ),
-"SOME_MONITORING_CONTEXT_NAME", {"analysis": {"profanity": False}} ) ...
+## Setting Up ```console $ pip install mona_openai ``` If you plan on using
+Mona as your monitoring service, [sign up for a free account here](https://
+www.monalabs.io/openai-gpt-monitoring). ## Quick Start You can find boilerplate
+code for many use-cases under [the "examples" folder](https://github.com/
+monalabs/mona-openai/tree/main/examples). ```py from os import environ import
+asyncio import openai from mona_openai.loggers import StandardLogger from
+logging import WARNING from mona_openai import monitor, monitor_with_logger
+openai.api_key = environ.get("OPEN_AI_KEY") # When using a standard logger.
+monitored_completion = monitor_with_logger( openai.Completion, StandardLogger
+(WARNING), ) response = monitored_completion.create( model="text-ada-001",
+prompt="I want to generate some text about ", max_tokens=20, n=1,
+temperature=0.2, # Adding additional information for monitoring purposes,
+unrelated to # internal OpenAI call. MONA_additional_data={"customer_id":
+"A531251"}, ) print(response.choices[0].text) # When monitoring with Mona.
+MONA_API_KEY = environ.get("MONA_API_KEY") MONA_SECRET = environ.get
+("MONA_SECRET") MONA_CREDS = { "key": MONA_API_KEY, "secret": MONA_SECRET, }
+CONTEXT_CLASS_NAME = "SOME_MONITORING_CONTEXT_NAME" monitored_completion =
+monitor( openai.Completion, MONA_CREDS, CONTEXT_CLASS_NAME, ) response =
+monitored_completion.create( model="text-ada-001", prompt="I want to generate
+some text about ", max_tokens=20, n=1, temperature=0.2, # Adding additional
+information for monitoring purposes, unrelated to # internal OpenAI call.
+MONA_additional_data={"customer_id": "A531251"}, ) print(response.choices
+[0].text) ``` ## Supported OpenAI APIs Currently this client supports
+`openai.Completion` and `openai.ChatCompletion`. Mona can support processes
+based on other APIs and also non-OpenAI-based apps. If you have a differrent
+use-case, we'd love to hear about it! Please email us at support@monalabs.io.
+## Usage ### Initialization The main and only function exposed in this package
+is `monitor`. ```py import openai from mona_openai import monitor
+openai.api_key = environ.get("OPEN_AI_KEY") monitored_completion = monitor
+( openai.Completion, ( environ.get("MONA_API_KEY"), environ.get("MONA_SECRET"),
+), "SOME_MONITORING_CONTEXT_NAME", {"analysis": {"profanity": False}} ) ...
 monitored_completion.create(...) ``` The `monitor` function returns to you a
 class that wraps the original openai endpoint class you provide, with an
 equivalent API (besides some additions listed below). You can then use the
 returned class' "create" and "acreate" functions just as you would before, only
 now, besides getting the requested openAI functionality, this client will log
 out to Mona's server the parameters you used (e.g., temperature), data about
 the response from OpenAI's server, and custom analyses about the call (e.g.,
@@ -65,73 +69,88 @@
 export_prompt (False): Whether Mona should export the actual prompt text. Be
 default set to False to avoid privacy concerns. * export_response_texts
 (False): Whether Mona should export the actual response texts. Be default set
 to False to avoid privacy concerns. * analysis: A dictionary mapping each
 analysis type to a boolean value telling the client whether or not to run said
 analysis and log it to Mona. Possible options currently are "privacy",
 "profanity", and "textual". By default, all analyses take place and are logged
-out to Mona. ### Capabilities during API calls After wrapping your endpoint
-with `monitor`, you really don't need to do anything else. When using `create`
-or `acreate` data will be tracked and monitoring will take place. There are,
-however, several capabilities that are added to these functions. Specifically,
-you can add the following arguments to any create call: * MONA_context_id: The
-unique id of the context in which the call is made. By using this ID you can
-export more data to Mona to the same context from other places. If not
-supplied, the "id" field of the OpenAI Endpoint's response will be used as the
-Mona context ID automatically. * MONA_export_timestamp: Can be used to simulate
-as if the current call was made in a different time, as far as Mona is
-concerned. * MONA_additional_data: A JSON-serializable dict with any other data
-you want to add to the monitoring context. This comes in handy if you want to
-add more information to the monitoring contex that isn't part of the basic
-OpenAI API call information. For example, if you are using a specific template
-ID or if this call is being made for a specific customer ID, these are fields
-you can add there to help get full context when monitoring with Mona. Example:
-```py response = asyncio.run(monitored_completion.acreate( engine=model,
-prompt=prompt, max_tokens=max_tokens, n=n, temperature=temperature,
-MONA_additional_data={"customer_id": "A531251"}, )) print(response.choices
-[0].text) ``` ### Using OpenAI with REST calls instead of OpenAI's Python
-client In some cases you may choose to use OpenAI's API directly with REST
-calls and not using OpenAI's SDK. For these cases we allow a more direct
-approach for logging to Mona as well, by using the "get_rest_monitor" function.
-See example below. ```py # Direct REST usage, without OpenAI client import
-requests from os import environ from mona_openai import get_rest_monitor
-MONA_API_KEY = environ.get("MONA_API_KEY") MONA_SECRET = environ.get
-("MONA_SECRET") MONA_CREDS = { "key": MONA_API_KEY, "secret": MONA_SECRET, }
-CONTEXT_CLASS_NAME = "SOME_MONITORING_CONTEXT_NAME" # Get Mona logger
-mona_logger = get_rest_monitor( "Completion", MONA_CREDS, CONTEXT_CLASS_NAME, )
-# Set up the API endpoint URL and authentication headers url = "https://
-api.openai.com/v1/completions" headers = { "Content-Type": "application/json",
-"Authorization": f"Bearer {environ.get('OPEN_AI_KEY')}", } # Set up the request
-data data = { "prompt": prompt, "max_tokens": max_tokens, "temperature":
-temperature, "model": model, "n": n, } # The log_request function returns two
-other function for later logging # the response or the exception. When we later
-do that, the logger will # actually calculate all the relevant metrics and will
-send them to # Mona. response_logger, exception_logger =
-mona_logger.log_request( data, additional_data={"customer_id": "A531251"} )
-try: # Send the request to the API response = requests.post(url,
-headers=headers, json=data) # Check for HTTP errors response.raise_for_status()
-# Log response to Mona response_logger(response.json()) print(response.json()
-["choices"][0]["text"]) except Exception as err: # Log exception to Mona
-exception_logger() ``` ### Stream support OpenAI allows receiving responses as
-a stream of tokens using the "stream" parameter. When this is done, Mona will
-collect all the tokens in memory and will create the analysis and log out the
-data the moment the stream is over. You don't need to do anything to make this
-happen. Since for streaming responses OpenAI doesn't supply the full usage
-tokens summary, Mona uses the tiktoken package to calculate the tokens of the
-prompt and completion and log them for monitoring. NOTE: Stream is currently
-only supported with SDK usage, and not with using REST directly. ## LangChain
-support You can use the exported `monitor_langchain_llm` to wrap a LangChain
-OpenAI LLM (chat or normal) with Mona's monitoring capabilities: ```py from
-mona_openai import monitor_langchain_llm from langchain.llms import OpenAI #
-Wrap the LLM object with Mona monitoring. llm = monitor_langchain_llm( OpenAI
-(OPEN_AI_KEY), MONA_CREDS, CONTEXT_CLASS_NAME) ``` See full example in
-completion_langchain.py in the examples folder. ## Mona SDK This package uses
-the mona_sdk package to export the relevant data to Mona. There are several
-environment variables you can use to configure the SDK's behavior. For example,
-you can set it up to raise exceptions when exporting data to Mona fails (it
-doesn't do that by default). ## Monitoring for profanity Mona uses the alt-
-profanity-check pacakge (https://pypi.org/project/alt-profanity-check/) to
-create both boolean predictions and probabilty scores for the existence of
-profanity both in the prompt and in the responses. We use the built in package
-methods for that. If you want, for example, to use a different probability
-threshold for the boolean prediction, you can do that by changing your Mona
-config on the Mona dashboard.
+out to Mona. ### Using custom loggers You don't have to have a Mona account to
+use this package. You can define specific loggers to log out the data to a
+file, memory, or just a given python logger. For example, to log out the
+relevant metrics as WARNING: ```py from os import environ import openai from
+mona_openai.loggers import StandardLogger from logging import WARNING from
+mona_openai import monitor_with_logger openai.api_key = environ.get
+("OPEN_AI_KEY") monitored_completion = monitor_with_logger( openai.Completion,
+StandardLogger(WARNING), ) response = monitored_completion.create( model="text-
+ada-001", prompt="I want to generate some text about ", max_tokens=20, n=1,
+temperature=0.2, # Adding additional information for monitoring purposes,
+unrelated to # internal OpenAI call. MONA_additional_data={"customer_id":
+"A531251"}, ) ``` This SDK provides a simple interface to implement your own
+loggers by inheriting from Logger under loggers/logger.py. Alternatively, by
+using the standard python logging library as in the example, you can create
+logging handlers to log the data out to any mechanism you choose (e.g., Kafka,
+Logstash, etc...) ### Capabilities during API calls After wrapping your
+endpoint with `monitor`, you really don't need to do anything else. When using
+`create` or `acreate` data will be tracked and monitoring will take place.
+There are, however, several capabilities that are added to these functions.
+Specifically, you can add the following arguments to any create call: *
+MONA_context_id: The unique id of the context in which the call is made. By
+using this ID you can export more data to Mona to the same context from other
+places. If not supplied, the "id" field of the OpenAI Endpoint's response will
+be used as the Mona context ID automatically. * MONA_export_timestamp: Can be
+used to simulate as if the current call was made in a different time, as far as
+Mona is concerned. * MONA_additional_data: A JSON-serializable dict with any
+other data you want to add to the monitoring context. This comes in handy if
+you want to add more information to the monitoring contex that isn't part of
+the basic OpenAI API call information. For example, if you are using a specific
+template ID or if this call is being made for a specific customer ID, these are
+fields you can add there to help get full context when monitoring with Mona.
+Example: ```py response = asyncio.run(monitored_completion.acreate
+( engine=model, prompt=prompt, max_tokens=max_tokens, n=n,
+temperature=temperature, MONA_additional_data={"customer_id": "A531251"}, ))
+print(response.choices[0].text) ``` ### Using OpenAI with REST calls instead of
+OpenAI's Python client In some cases you may choose to use OpenAI's API
+directly with REST calls and not using OpenAI's SDK. For these cases we allow a
+more direct approach for logging to Mona as well, by using the
+"get_rest_monitor" function. See example below. ```py # Direct REST usage,
+without OpenAI client import requests from os import environ from mona_openai
+import get_rest_monitor MONA_API_KEY = environ.get("MONA_API_KEY") MONA_SECRET
+= environ.get("MONA_SECRET") MONA_CREDS = { "key": MONA_API_KEY, "secret":
+MONA_SECRET, } CONTEXT_CLASS_NAME = "SOME_MONITORING_CONTEXT_NAME" # Get Mona
+logger mona_logger = get_rest_monitor( "Completion", MONA_CREDS,
+CONTEXT_CLASS_NAME, ) # Set up the API endpoint URL and authentication headers
+url = "https://api.openai.com/v1/completions" headers = { "Content-Type":
+"application/json", "Authorization": f"Bearer {environ.get('OPEN_AI_KEY')}", }
+# Set up the request data data = { "prompt": prompt, "max_tokens": max_tokens,
+"temperature": temperature, "model": model, "n": n, } # The log_request
+function returns two other function for later logging # the response or the
+exception. When we later do that, the logger will # actually calculate all the
+relevant metrics and will send them to # Mona. response_logger,
+exception_logger = mona_logger.log_request( data, additional_data=
+{"customer_id": "A531251"} ) try: # Send the request to the API response =
+requests.post(url, headers=headers, json=data) # Check for HTTP errors
+response.raise_for_status() # Log response to Mona response_logger
+(response.json()) print(response.json()["choices"][0]["text"]) except Exception
+as err: # Log exception to Mona exception_logger() ``` ### Stream support
+OpenAI allows receiving responses as a stream of tokens using the "stream"
+parameter. When this is done, Mona will collect all the tokens in memory and
+will create the analysis and log out the data the moment the stream is over.
+You don't need to do anything to make this happen. Since for streaming
+responses OpenAI doesn't supply the full usage tokens summary, Mona uses the
+tiktoken package to calculate the tokens of the prompt and completion and log
+them for monitoring. NOTE: Stream is currently only supported with SDK usage,
+and not with using REST directly. ## LangChain support You can use the exported
+`monitor_langchain_llm` to wrap a LangChain OpenAI LLM (chat or normal) with
+Mona's monitoring capabilities: ```py from mona_openai import
+monitor_langchain_llm from langchain.llms import OpenAI # Wrap the LLM object
+with Mona monitoring. llm = monitor_langchain_llm( OpenAI(OPEN_AI_KEY),
+MONA_CREDS, CONTEXT_CLASS_NAME) ``` See full example in completion_langchain.py
+in the examples folder. ## Mona SDK This package uses the mona_sdk package to
+export the relevant data to Mona. There are several environment variables you
+can use to configure the SDK's behavior. For example, you can set it up to
+raise exceptions when exporting data to Mona fails (it doesn't do that by
+default). ## Monitoring for profanity Mona uses the alt-profanity-check pacakge
+(https://pypi.org/project/alt-profanity-check/) to create both boolean
+predictions and probabilty scores for the existence of profanity both in the
+prompt and in the responses. We use the built in package methods for that. If
+you want, for example, to use a different probability threshold for the boolean
+prediction, you can do that by changing your Mona config on the Mona dashboard.
```

### Comparing `mona-openai-0.0.9/mona_openai.egg-info/SOURCES.txt` & `mona-openai-0.1.0/mona_openai.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 mona_openai/__init__.py
 mona_openai/exceptions.py
-mona_openai/mona_client.py
 mona_openai/mona_openai.py
 mona_openai.egg-info/PKG-INFO
 mona_openai.egg-info/SOURCES.txt
 mona_openai.egg-info/dependency_links.txt
 mona_openai.egg-info/requires.txt
 mona_openai.egg-info/top_level.txt
 mona_openai/analysis/privacy.py
 mona_openai/analysis/profanity.py
 mona_openai/analysis/textual.py
 mona_openai/endpoints/chat_completion.py
 mona_openai/endpoints/completion.py
 mona_openai/endpoints/endpoint_wrapping.py
 mona_openai/endpoints/wrapping_getter.py
+mona_openai/loggers/__init__.py
+mona_openai/loggers/file_logger.py
+mona_openai/loggers/in_memory_logging.py
+mona_openai/loggers/logger.py
+mona_openai/loggers/standard_logging.py
+mona_openai/loggers/mona_logger/mona_client.py
+mona_openai/loggers/mona_logger/mona_logger.py
 mona_openai/util/async_util.py
 mona_openai/util/func_util.py
 mona_openai/util/oop_util.py
 mona_openai/util/openai_util.py
 mona_openai/util/stream_util.py
 mona_openai/util/tokens_util.py
 mona_openai/util/validation_util.py
```

### Comparing `mona-openai-0.0.9/pyproject.toml` & `mona-openai-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mona-openai"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Itai Bar Sinai", email="itai@monalabs.io" },
 ]
 description = "Integration client for monitoring OpenAI usage with Mona"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mona-openai-0.0.9/tests/test_chat_completion.py` & `mona-openai-0.1.0/tests/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/tests/test_completion.py` & `mona-openai-0.1.0/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/tests/test_privacy_analyzer.py` & `mona-openai-0.1.0/tests/test_privacy_analyzer.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.9/tests/test_textual_analyzer.py` & `mona-openai-0.1.0/tests/test_textual_analyzer.py`

 * *Files identical despite different names*

