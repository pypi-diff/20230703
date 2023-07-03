# Comparing `tmp/aicodebot-0.7.0.tar.gz` & `tmp/aicodebot-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.7.0.tar", last modified: Sun Jul  2 04:30:34 2023, max compression
+gzip compressed data, was "aicodebot-0.7.1.tar", last modified: Mon Jul  3 00:21:17 2023, max compression
```

## Comparing `aicodebot-0.7.0.tar` & `aicodebot-0.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:30:34.282827 aicodebot-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-02 04:30:10.000000 aicodebot-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-07-02 04:30:34.278828 aicodebot-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-07-02 04:30:10.000000 aicodebot-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:30:34.278828 aicodebot-0.7.0/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/.aicodebot.template
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:30:34.278828 aicodebot-0.7.0/aicodebot/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/prompts/alignment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/prompts/commit_message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/prompts/debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/prompts/fun_fact.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-02 04:30:10.000000 aicodebot-0.7.0/aicodebot/prompts/review.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:30:34.278828 aicodebot-0.7.0/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-07-02 04:30:34.000000 aicodebot-0.7.0/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-02 04:30:34.000000 aicodebot-0.7.0/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:30:34.000000 aicodebot-0.7.0/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-02 04:30:34.000000 aicodebot-0.7.0/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-02 04:30:34.000000 aicodebot-0.7.0/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-02 04:30:34.000000 aicodebot-0.7.0/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-02 04:30:10.000000 aicodebot-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 04:30:34.282827 aicodebot-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-02 04:30:10.000000 aicodebot-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:21:17.648448 aicodebot-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-03 00:20:53.000000 aicodebot-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-07-03 00:21:17.648448 aicodebot-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-07-03 00:20:53.000000 aicodebot-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:21:17.648448 aicodebot-0.7.1/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 00:20:53.000000 aicodebot-0.7.1/aicodebot/.aicodebot.template
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 00:20:53.000000 aicodebot-0.7.1/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-03 00:20:53.000000 aicodebot-0.7.1/aicodebot/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14574 2023-07-03 00:20:53.000000 aicodebot-0.7.1/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-03 00:20:53.000000 aicodebot-0.7.1/aicodebot/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:21:17.648448 aicodebot-0.7.1/aicodebot/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:20:53.000000 aicodebot-0.7.1/aicodebot/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-03 00:20:53.000000 aicodebot-0.7.1/aicodebot/prompts/alignment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-03 00:20:53.000000 aicodebot-0.7.1/aicodebot/prompts/commit_message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 00:20:53.000000 aicodebot-0.7.1/aicodebot/prompts/debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-03 00:20:53.000000 aicodebot-0.7.1/aicodebot/prompts/fun_fact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-03 00:20:53.000000 aicodebot-0.7.1/aicodebot/prompts/review.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:21:17.648448 aicodebot-0.7.1/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-07-03 00:21:17.000000 aicodebot-0.7.1/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 00:21:17.000000 aicodebot-0.7.1/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 00:21:17.000000 aicodebot-0.7.1/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 00:21:17.000000 aicodebot-0.7.1/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-03 00:21:17.000000 aicodebot-0.7.1/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 00:21:17.000000 aicodebot-0.7.1/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-03 00:20:53.000000 aicodebot-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 00:21:17.648448 aicodebot-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-03 00:20:53.000000 aicodebot-0.7.1/setup.py
```

### Comparing `aicodebot-0.7.0/LICENSE` & `aicodebot-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.0/PKG-INFO` & `aicodebot-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.7.0
+Version: 0.7.1
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aicodebot-0.7.0/README.md` & `aicodebot-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.0/aicodebot/agents.py` & `aicodebot-0.7.1/aicodebot/agents.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.0/aicodebot/cli.py` & `aicodebot-0.7.1/aicodebot/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 DEFAULT_MAX_TOKENS = 512
 DEFAULT_TEMPERATURE = 0.1
 DEFAULT_SPINNER = "point"
 
 # ----------------------- Setup for rich console output ---------------------- #
 console = Console()
 bot_style = Style(color="#30D5C8")
+error_style = Style(color="#FF0000")
+warning_style = Style(color="#FFA500")
 
 
 # -------------------------- Top level command group ------------------------- #
 
 
 @click.group()
 @click.version_option(aicodebot_version, "--version", "-V")
@@ -233,15 +235,24 @@
         console.print(response, style=bot_style)
 
 
 @cli.command
 @click.option("--task", "-t", help="The task you want to perform - a description of what you want to do.")
 @click.option("-v", "--verbose", count=True)
 def sidekick(task, verbose):
-    """ALPHA/EXPERIMENTAL: Get help with a task from your AI sidekick."""
+    """ALPHA/EXPERIMENTAL: Get coding help from your AI sidekick."""
+    console.print(
+        "⚠️ WARNING: The 'sidekick' feature is currently experimental and, frankly, it sucks right now. "
+        "Due to the token limitations with large language models, the amount of context "
+        "that can be sent back and forth is limited, and slow. This means that sidekick will struggle with "
+        "complex tasks and will take longer than a human for simpler tasks.\n"
+        "Play with it, but don't expect too much. Do you feel like contributing? 😃",
+        style=warning_style,
+    )
+
     setup_environment()
 
     model = get_llm_model()
     llm = ChatOpenAI(model=model, temperature=DEFAULT_TEMPERATURE, max_tokens=3500, verbose=verbose)
 
     agent = get_agent("sidekick", llm, verbose)
```

### Comparing `aicodebot-0.7.0/aicodebot/helpers.py` & `aicodebot-0.7.1/aicodebot/helpers.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.0/aicodebot/prompts/alignment.yaml` & `aicodebot-0.7.1/aicodebot/prompts/alignment.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.0/aicodebot/prompts/commit_message.yaml` & `aicodebot-0.7.1/aicodebot/prompts/commit_message.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.0/aicodebot/prompts/review.yaml` & `aicodebot-0.7.1/aicodebot/prompts/review.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.0/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.7.1/aicodebot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.7.0
+Version: 0.7.1
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aicodebot-0.7.0/aicodebot.egg-info/SOURCES.txt` & `aicodebot-0.7.1/aicodebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.0/pyproject.toml` & `aicodebot-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.0/setup.py` & `aicodebot-0.7.1/setup.py`

 * *Files identical despite different names*

