# Comparing `tmp/aicodebot-0.7.2.tar.gz` & `tmp/aicodebot-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.7.2.tar", last modified: Mon Jul  3 01:21:35 2023, max compression
+gzip compressed data, was "aicodebot-0.7.3.tar", last modified: Mon Jul  3 01:35:21 2023, max compression
```

## Comparing `aicodebot-0.7.2.tar` & `aicodebot-0.7.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:21:35.357088 aicodebot-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-03 01:21:11.000000 aicodebot-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-07-03 01:21:35.357088 aicodebot-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-03 01:21:11.000000 aicodebot-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:21:35.357088 aicodebot-0.7.2/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 01:21:11.000000 aicodebot-0.7.2/aicodebot/.aicodebot.template
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 01:21:11.000000 aicodebot-0.7.2/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-03 01:21:11.000000 aicodebot-0.7.2/aicodebot/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)    14629 2023-07-03 01:21:11.000000 aicodebot-0.7.2/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-03 01:21:11.000000 aicodebot-0.7.2/aicodebot/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:21:35.357088 aicodebot-0.7.2/aicodebot/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:21:11.000000 aicodebot-0.7.2/aicodebot/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-03 01:21:11.000000 aicodebot-0.7.2/aicodebot/prompts/alignment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-03 01:21:11.000000 aicodebot-0.7.2/aicodebot/prompts/commit_message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 01:21:11.000000 aicodebot-0.7.2/aicodebot/prompts/debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-03 01:21:11.000000 aicodebot-0.7.2/aicodebot/prompts/fun_fact.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-03 01:21:11.000000 aicodebot-0.7.2/aicodebot/prompts/review.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:21:35.357088 aicodebot-0.7.2/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-07-03 01:21:35.000000 aicodebot-0.7.2/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 01:21:35.000000 aicodebot-0.7.2/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:21:35.000000 aicodebot-0.7.2/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 01:21:35.000000 aicodebot-0.7.2/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-03 01:21:35.000000 aicodebot-0.7.2/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 01:21:35.000000 aicodebot-0.7.2/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-03 01:21:11.000000 aicodebot-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 01:21:35.357088 aicodebot-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-03 01:21:11.000000 aicodebot-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:35:21.198485 aicodebot-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-03 01:34:50.000000 aicodebot-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-03 01:35:21.198485 aicodebot-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-07-03 01:34:50.000000 aicodebot-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:35:21.194485 aicodebot-0.7.3/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/.aicodebot.template
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14629 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:35:21.198485 aicodebot-0.7.3/aicodebot/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/prompts/alignment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/prompts/commit_message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/prompts/debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/prompts/fun_fact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/prompts/review.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:35:21.198485 aicodebot-0.7.3/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-03 01:35:21.000000 aicodebot-0.7.3/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 01:35:21.000000 aicodebot-0.7.3/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:35:21.000000 aicodebot-0.7.3/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 01:35:21.000000 aicodebot-0.7.3/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-03 01:35:21.000000 aicodebot-0.7.3/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 01:35:21.000000 aicodebot-0.7.3/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-03 01:34:50.000000 aicodebot-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 01:35:21.198485 aicodebot-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-03 01:34:50.000000 aicodebot-0.7.3/setup.py
```

### Comparing `aicodebot-0.7.2/LICENSE` & `aicodebot-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.2/PKG-INFO` & `aicodebot-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.7.2
-Summary: Your AI-powered coding companion: AI Code Bot 🤖
-Home-page: https://github.com/novara_ai/aicodebot
+Version: 0.7.3
+Summary: Your AI-powered coding sidekick 🤖
+Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,15 +23,15 @@
 
 We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
 ⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features.
 
 ⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent. Much like Tesla's Full Self Driving, you have to keep your hands on the wheel.
 
-We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/novara-ai/AICodeBot/blob/main/CONTRIBUTING.md) for more.
+We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more.
 
 ### What it's not
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
 It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
@@ -131,8 +131,8 @@
 
 ## Alignment ❤️ + 🤖
 
 Technology itself is amoral, it just imbues the values of the people who create it. We believe that AI should be built-in a way that aligns with humanity, and we're building AICodeBot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
 
 ## Development / Contributing
 
-We'd love your help! If you're interested in contributing, here's how to get started. See [CONTRIBUTING](https://github.com/novara-ai/AICodeBot/blob/main/CONTRIBUTING.md) for more details.
+We'd love your help! If you're interested in contributing, here's how to get started. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more details.
```

### Comparing `aicodebot-0.7.2/README.md` & `aicodebot-0.7.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
 ⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features.
 
 ⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent. Much like Tesla's Full Self Driving, you have to keep your hands on the wheel.
 
-We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/novara-ai/AICodeBot/blob/main/CONTRIBUTING.md) for more.
+We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more.
 
 ### What it's not
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
 It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
@@ -114,8 +114,8 @@
 
 ## Alignment ❤️ + 🤖
 
 Technology itself is amoral, it just imbues the values of the people who create it. We believe that AI should be built-in a way that aligns with humanity, and we're building AICodeBot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
 
 ## Development / Contributing
 
-We'd love your help! If you're interested in contributing, here's how to get started. See [CONTRIBUTING](https://github.com/novara-ai/AICodeBot/blob/main/CONTRIBUTING.md) for more details.
+We'd love your help! If you're interested in contributing, here's how to get started. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more details.
```

### Comparing `aicodebot-0.7.2/aicodebot/agents.py` & `aicodebot-0.7.3/aicodebot/agents.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.2/aicodebot/cli.py` & `aicodebot-0.7.3/aicodebot/cli.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.2/aicodebot/helpers.py` & `aicodebot-0.7.3/aicodebot/helpers.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.2/aicodebot/prompts/alignment.yaml` & `aicodebot-0.7.3/aicodebot/prompts/alignment.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.2/aicodebot/prompts/commit_message.yaml` & `aicodebot-0.7.3/aicodebot/prompts/commit_message.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.2/aicodebot/prompts/review.yaml` & `aicodebot-0.7.3/aicodebot/prompts/review.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.2/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.7.3/aicodebot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.7.2
-Summary: Your AI-powered coding companion: AI Code Bot 🤖
-Home-page: https://github.com/novara_ai/aicodebot
+Version: 0.7.3
+Summary: Your AI-powered coding sidekick 🤖
+Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,15 +23,15 @@
 
 We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
 ⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features.
 
 ⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent. Much like Tesla's Full Self Driving, you have to keep your hands on the wheel.
 
-We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/novara-ai/AICodeBot/blob/main/CONTRIBUTING.md) for more.
+We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more.
 
 ### What it's not
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
 It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
@@ -131,8 +131,8 @@
 
 ## Alignment ❤️ + 🤖
 
 Technology itself is amoral, it just imbues the values of the people who create it. We believe that AI should be built-in a way that aligns with humanity, and we're building AICodeBot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
 
 ## Development / Contributing
 
-We'd love your help! If you're interested in contributing, here's how to get started. See [CONTRIBUTING](https://github.com/novara-ai/AICodeBot/blob/main/CONTRIBUTING.md) for more details.
+We'd love your help! If you're interested in contributing, here's how to get started. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more details.
```

### Comparing `aicodebot-0.7.2/aicodebot.egg-info/SOURCES.txt` & `aicodebot-0.7.3/aicodebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.2/pyproject.toml` & `aicodebot-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.2/setup.py` & `aicodebot-0.7.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     requirements = f.read().splitlines()
 
 if __name__ == "__main__":  # Only run setup if this is the main file (allows this file to be imported for __version__)
     setup(
         name="aicodebot",
         python_requires=">=3.9",
         version=version,
-        url="https://github.com/novara_ai/aicodebot",
+        url="https://github.com/gorillamania/AICodeBot",
         author="Nick Sullivan",
-        description="Your AI-powered coding companion: AI Code Bot 🤖",
+        description="Your AI-powered coding sidekick 🤖",
         long_description=long_description,
         long_description_content_type="text/markdown",
         install_requires=requirements,
         entry_points={
             "console_scripts": [
                 "aicodebot = aicodebot.cli:cli",
             ],
```

