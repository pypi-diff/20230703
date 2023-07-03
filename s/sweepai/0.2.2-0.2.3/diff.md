# Comparing `tmp/sweepai-0.2.2.tar.gz` & `tmp/sweepai-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.2.2.tar", max compression
+gzip compressed data, was "sweepai-0.2.3.tar", max compression
```

## Comparing `sweepai-0.2.2.tar` & `sweepai-0.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.2/LICENSE
--rw-r--r--   0        0        0     3867 2023-07-02 22:43:45.228580 sweepai-0.2.2/README.md
--rw-r--r--   0        0        0     1133 2023-07-02 22:42:20.755091 sweepai-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.2/sweepai/__init__.py
--rw-r--r--   0        0        0    10664 2023-07-01 23:29:41.701470 sweepai-0.2.2/sweepai/api.py
--rw-r--r--   0        0        0     5893 2023-07-02 07:30:30.847953 sweepai-0.2.2/sweepai/app/api_client.py
--rw-r--r--   0        0        0     6995 2023-07-02 07:30:30.847953 sweepai-0.2.2/sweepai/app/backend.py
--rw-r--r--   0        0        0      741 2023-07-02 07:30:30.847953 sweepai-0.2.2/sweepai/app/cli.py
--rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.2/sweepai/app/config.py
--rw-r--r--   0        0        0     9761 2023-07-02 22:43:45.228580 sweepai-0.2.2/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.2/sweepai/core/__init__.py
--rw-r--r--   0        0        0    16077 2023-07-02 07:30:30.847953 sweepai-0.2.2/sweepai/core/chat.py
--rw-r--r--   0        0        0     2553 2023-07-01 23:29:41.701470 sweepai-0.2.2/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     7286 2023-07-02 07:30:30.847953 sweepai-0.2.2/sweepai/core/entities.py
--rw-r--r--   0        0        0    13033 2023-07-01 23:29:41.701470 sweepai-0.2.2/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3509 2023-07-01 23:29:41.701470 sweepai-0.2.2/sweepai/core/react.py
--rw-r--r--   0        0        0    15487 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    12030 2023-07-02 07:30:30.847953 sweepai-0.2.2/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     2536 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     3150 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    11177 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0    19497 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/utils/__init__.py
--rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/utils/config.py
--rw-r--r--   0        0        0      670 2023-07-02 22:42:08.445068 sweepai-0.2.2/sweepai/utils/constants.py
--rw-r--r--   0        0        0     3633 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/utils/diff.py
--rw-r--r--   0        0        0      507 2023-07-02 21:36:52.379851 sweepai-0.2.2/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8166 2023-07-02 21:45:23.803536 sweepai-0.2.2/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/utils/hash.py
--rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/utils/huggingface.py
--rw-r--r--   0        0        0     5339 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      902 2023-07-02 07:30:30.851287 sweepai-0.2.2/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.2/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11266 2023-07-01 23:29:41.708137 sweepai-0.2.2/sweepai/utils/utils.py
--rw-r--r--   0        0        0     4931 2023-07-02 22:43:50.108748 sweepai-0.2.2/setup.py
--rw-r--r--   0        0        0     4415 2023-07-02 22:43:50.109315 sweepai-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4221 2023-07-03 20:48:18.953249 sweepai-0.2.3/README.md
+-rw-r--r--   0        0        0     1133 2023-07-03 20:48:48.779950 sweepai-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.3/sweepai/__init__.py
+-rw-r--r--   0        0        0    10664 2023-07-01 23:29:41.701470 sweepai-0.2.3/sweepai/api.py
+-rw-r--r--   0        0        0     5893 2023-07-02 07:30:30.847953 sweepai-0.2.3/sweepai/app/api_client.py
+-rw-r--r--   0        0        0     6995 2023-07-02 07:30:30.847953 sweepai-0.2.3/sweepai/app/backend.py
+-rw-r--r--   0        0        0      993 2023-07-03 20:38:42.899426 sweepai-0.2.3/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.3/sweepai/app/config.py
+-rw-r--r--   0        0        0    10441 2023-07-03 19:27:15.637337 sweepai-0.2.3/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.3/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    16077 2023-07-02 07:30:30.847953 sweepai-0.2.3/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2306 2023-07-03 00:42:21.645402 sweepai-0.2.3/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     7286 2023-07-02 07:30:30.847953 sweepai-0.2.3/sweepai/core/entities.py
+-rw-r--r--   0        0        0    13104 2023-07-03 00:42:21.645402 sweepai-0.2.3/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3509 2023-07-01 23:29:41.701470 sweepai-0.2.3/sweepai/core/react.py
+-rw-r--r--   0        0        0    16496 2023-07-03 00:51:22.966350 sweepai-0.2.3/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    12030 2023-07-02 07:30:30.847953 sweepai-0.2.3/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     2536 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     3150 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    11178 2023-07-03 00:51:22.966350 sweepai-0.2.3/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0    19497 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/utils/config.py
+-rw-r--r--   0        0        0      670 2023-07-03 00:42:21.645402 sweepai-0.2.3/sweepai/utils/constants.py
+-rw-r--r--   0        0        0     4072 2023-07-03 00:42:21.645402 sweepai-0.2.3/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      507 2023-07-03 00:42:21.645402 sweepai-0.2.3/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8166 2023-07-03 00:42:21.645402 sweepai-0.2.3/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/utils/huggingface.py
+-rw-r--r--   0        0        0     5339 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      902 2023-07-02 07:30:30.851287 sweepai-0.2.3/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11266 2023-07-01 23:29:41.708137 sweepai-0.2.3/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     5286 2023-07-03 20:48:50.959518 sweepai-0.2.3/setup.py
+-rw-r--r--   0        0        0     4769 2023-07-03 20:48:50.960638 sweepai-0.2.3/PKG-INFO
```

### Comparing `sweepai-0.2.2/LICENSE` & `sweepai-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/README.md` & `sweepai-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 <p align="center">
-    <img src=".assets/sweep-banner-github.png">
+    <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png">
 </p>
 <p align="center">
     <i>Spend time reviewing code generated by AI, not writing it.</i>
 </p>
 
 <p align="center">
 <a href="https://sweep.dev/">🌐 Website</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://docs.sweep.dev/">📚 Docs</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://discord.gg/sweep-ai">📢 Discord</a>
 </p>
 
-<b>Sweep</b> allows you to create and review GitHub issues with easy.
+<b>Sweep</b> allows you to create and review GitHub issues with ease.
 Simply describe any issue and Sweep will do the rest.
 It will plan out what needs to be done, what changes to make, and write the changes to a PR. 
 
+Supported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports
+
 ---
 
 ## ✨ Demo
 For the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.
 
 [Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)
 
 ## 🚀 Getting Started
 
 ### 🖥️ Sweep Chat
 Sweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. 
 
 1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
 
-2. Run `pip install sweepai && sweep`
+2. Run `pip install sweepai && sweep`. Note that you need python 3.11 or greater.
 
 3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.
 
 4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. 
-<img src=".assets/gradio-screenshot.png">
+<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">
 
 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
 
 #### From Source
 If you want the nightly build and or if the latest build has issues.
 
 1. `git clone https://github.com/sweepai/sweep && poetry install`
-2. `python sweepai/app/cli.py`
+2. `python sweepai/app/cli.py`. Note that you need python 3.11 or greater.
 
 ### ✨ Sweep Github App
 Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.
 
 1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
 2. Create new issue in repo, like "Sweep: Write tests"
 3. "👀" means it is taking a look, and it will generate the desired code
@@ -77,15 +79,14 @@
 * Chain-of-Thought retrieval using GPT Functions
 
 ## 🗺️ Roadmap
 We're currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).
 
 ---
 
-
 <h2 align="center">
     Contributors
 </h2>
 <p align="center">
     Thank you for your contribution!
 </p>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,32 +1,37 @@
-                       [.assets/sweep-banner-github.png]
+                    [https://github.com/sweepai/sweep/blob/
+   856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png]
           Spend time reviewing code generated by AI, not writing it.
               ð_Website   â¢   ð_Docs   â¢   ð¢_Discord
-Sweep allows you to create and review GitHub issues with easy. Simply describe
+Sweep allows you to create and review GitHub issues with ease. Simply describe
 any issue and Sweep will do the rest. It will plan out what needs to be done,
-what changes to make, and write the changes to a PR. --- ## â¨ Demo For the
-best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of
-your repos and see the magic happen. [Demo](https://github.com/sweepai/sweep/
-assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47) ## ð Getting Started
-### ð¥ï¸ Sweep Chat Sweep Chat allows you to interact with Sweep locally and
-will sync with GitHub. You can plan out your changes with Sweep, and then Sweep
-can create a pull request for you. 1. Install [Sweep GitHub app](https://
-github.com/apps/sweep-ai) to desired repos 2. Run `pip install sweepai &&
-sweep` 3. This should spin up a GitHub auth flow in your browser. Copy-paste
+what changes to make, and write the changes to a PR. Supported languages:
+Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-
+4 supports --- ## â¨ Demo For the best experience, [install Sweep](https://
+github.com/apps/sweep-ai) to one of your repos and see the magic happen. [Demo]
+(https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-
+0af02f2b0e47) ## ð Getting Started ### ð¥ï¸ Sweep Chat Sweep Chat allows
+you to interact with Sweep locally and will sync with GitHub. You can plan out
+your changes with Sweep, and then Sweep can create a pull request for you. 1.
+Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
+2. Run `pip install sweepai && sweep`. Note that you need python 3.11 or
+greater. 3. This should spin up a GitHub auth flow in your browser. Copy-paste
 the ðµ blue 8-digit code from your terminal into the page. Then wait a few
 seconds and it should spin up Sweep Chat. You should only need to do the auth
 once. 4. Pick a repo from the dropdown at the top (the Github app must be
 installed on this repo). Then start chatting with Sweep Chat. Relevant searched
 files will show up on the right. Sweep Chat can make PRs if you ask it to
-create a PR. [.assets/gradio-screenshot.png] ð¡ You can force dark mode by
-going to http://127.0.0.1:7861/?__theme=dark. #### From Source If you want the
-nightly build and or if the latest build has issues. 1. `git clone https://
-github.com/sweepai/sweep && poetry install` 2. `python sweepai/app/cli.py` ###
-â¨ Sweep Github App Setting up Sweep is as simple as adding the GitHub bot to
-a repo, then creating an issue for the bot to address. 1. Add the [Sweep GitHub
+create a PR. [https://github.com/sweepai/sweep/blob/
+856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png] ð¡
+You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark. ####
+From Source If you want the nightly build and or if the latest build has
+issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
+`python sweepai/app/cli.py`. Note that you need python 3.11 or greater. ### â¨
+Sweep Github App Setting up Sweep is as simple as adding the GitHub bot to a
+repo, then creating an issue for the bot to address. 1. Add the [Sweep GitHub
 app](https://github.com/apps/sweep-ai) to desired repos 2. Create new issue in
 repo, like "Sweep: Write tests" 3. "ð" means it is taking a look, and it
 will generate the desired code 4. "ð" means the bot has finished its job and
 created a PR For more detailed docs, see [ð Quickstart](https://
 docs.sweep.dev/start). --- ## ð Story We were frustrated by small tickets,
 like simple bug fixes, annoying refactors, and small features, each task
 requiring us to open our IDE to fix simple bugs. So, we decided to leverage the
```

### Comparing `sweepai-0.2.2/pyproject.toml` & `sweepai-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.2.2"
+version = "0.2.3"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `sweepai-0.2.2/sweepai/api.py` & `sweepai-0.2.3/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/app/api_client.py` & `sweepai-0.2.3/sweepai/app/api_client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/app/backend.py` & `sweepai-0.2.3/sweepai/app/backend.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/app/config.py` & `sweepai-0.2.3/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/app/ui.py` & `sweepai-0.2.3/sweepai/app/ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 import json
 from github import Github
 import gradio as gr
 from loguru import logger
 import webbrowser
-
 from sweepai.app.api_client import APIClient, create_pr_function, create_pr_function_call
 from sweepai.app.config import SweepChatConfig
 from sweepai.core.entities import Snippet
 
 config = SweepChatConfig.load()
 
 api_client = APIClient(config=config)
 
-pr_summary_template = """💡 I'll create the following PR:
+pr_summary_template = '''💡 I'll create the following PR:
 
 **{title}**
 {summary}
 
 Here is my plan:
 {plan}
 
-Reply with "ok" to create the PR or anything else to propose changes."""
+Reply with "ok" to create the PR or anything else to propose changes.'''
 
 github_client = Github(config.github_pat)
 repos = list(github_client.get_user().get_repos())
 
-css = """
+css = '''
 footer {
     visibility: hidden;
 }
 pre, code {
     white-space: pre-wrap !important;
     word-break: break-all !important;
 }
 #snippets {
     height: 750px;
     overflow-y: scroll;
 }
-"""
+'''
 
 def get_files_recursively(repo, path=''):
     path_to_contents = {}
     try:
         contents = repo.get_contents(path)
         files = []
         while contents:
@@ -57,25 +56,54 @@
                     path_to_contents[file_content.path] = file_content.decoded_content.decode("utf-8")
                     files.append(file_content.path)
         return sorted(files), path_to_contents
     except Exception as e:
         logger.error(e)
         return [], path_to_contents
 
+def get_installation_id(repo_full_name):
+    config.repo_full_name = repo_full_name
+    api_client.config = config
+    installation_id = api_client.get_installation_id()
+    return installation_id
+
+path_to_contents = {}
+def get_files(name):
+    global path_to_contents
+    global repo
+    if name is None:
+        all_files = []
+    else:
+        # Make sure repo is added to Sweep before checking all recursive files
+        try:
+            installation_id = get_installation_id(name)
+            assert installation_id
+        except:
+            return []
+        repo = github_client.get_repo(name)
+        all_files, path_to_contents = get_files_recursively(repo)
+    return all_files
+
+def get_files_update(*args):
+    global repo
+    if len(args) > 0:
+        repo = args[0]
+    else:
+        repo = config.repo_full_name
+    return gr.Dropdown.update(choices=get_files(repo))
+
+
 with gr.Blocks(theme=gr.themes.Soft(), title="Sweep Chat", css=css) as demo:
     with gr.Row():
         with gr.Column():
             repo_full_name = gr.Dropdown(choices=[repo.full_name for repo in repos], label="Repo full name", value=config.repo_full_name or "")
         with gr.Column(scale=2):
-            if config.repo_full_name is None:
-                all_files = []
-            else:
-                repo = github_client.get_repo(config.repo_full_name)
-                all_files, path_to_contents = get_files_recursively(repo)
-            file_names = gr.Dropdown(choices=all_files, multiselect=True, label="Files")
+            file_names = gr.Dropdown(choices=get_files(config.repo_full_name), multiselect=True, label="Files")
+        repo_full_name.change(get_files_update, repo_full_name, file_names)
+
     with gr.Row():
         with gr.Column(scale=2):
             chatbot = gr.Chatbot(height=750)
         with gr.Column():
             snippets_text = gr.Markdown(value="### Relevant snippets", elem_id="snippets")
     msg = gr.Textbox(label="Message to Sweep", placeholder="Write unit tests for OpenAI calls")
     # clear = gr.ClearButton([msg, chatbot, snippets_text])
@@ -84,17 +112,15 @@
     searched = False
     selected_snippets = []
     file_to_str = {}
 
     def repo_name_change(repo_full_name):
         global installation_id
         try:
-            config.repo_full_name = repo_full_name
-            api_client.config = config
-            installation_id = api_client.get_installation_id()
+            installation_id = get_installation_id(repo_full_name)
             assert installation_id
             config.installation_id = installation_id
             api_client.config = config
             config.save()
             return ""
         except Exception as e:
             webbrowser.open_new_tab("https://github.com/apps/sweep-ai")
@@ -115,14 +141,15 @@
                 add_file_to_dict(file_name)
         snippets_text = "### Relevant snippets:\n" + "\n\n".join([file_to_str[snippet.file_path] for snippet in selected_snippets])
         return snippets_text
 
     def add_file_to_dict(file_name):
         global file_to_str
         global path_to_contents
+        global repo
         if file_name in path_to_contents:
             file_contents = path_to_contents[file_name]
         else:
             file_contents = repo.get_contents(file_name).decoded_content.decode('utf-8')
         file_contents_split = file_contents.split("\n")
         length = len(file_contents_split)
         backtick, escaped_backtick = "`", "\\`"
```

### Comparing `sweepai-0.2.2/sweepai/core/chat.py` & `sweepai-0.2.3/sweepai/core/chat.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/core/code_repair.py` & `sweepai-0.2.3/sweepai/core/code_repair.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,16 +45,9 @@
 
 
     def repair_code(self, diff: str, user_code: str, feature:str) -> str:
         self.messages = [Message(role="system", content=code_repair_system_prompt.format(feature=feature))]
         self.model = "gpt-3.5-turbo-16k-0613" # can be optimized
         response = self.chat(code_repair_prompt.format(diff=diff, user_code=user_code))
         self.undo()
-        try:
-            match = re.search(response_regex, response, flags=re.DOTALL)
-        except:
-            return response.strip() + "\n"
-        if match is None:
-            return response.strip() + "\n"
-        else:
-            return match.group("response").strip() + "\n"
+        return response.strip() + "\n"
```

### Comparing `sweepai-0.2.2/sweepai/core/entities.py` & `sweepai-0.2.3/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/core/prompts.py` & `sweepai-0.2.3/sweepai/core/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,16 +258,17 @@
 """
 
 modify_file_prompt = """
 Generate a new_file based on the given plan, ensuring that you:
 1. Do not write "pass" statements.
 2. Provide complete functions with actual business logic. It is imperative that we do not leave any work to the user/future readers of this code.
 3. Do not write new "todo" comments.
-4. Do not write incomplete functions or line numbers.
-5. Make sure code follows programming language conventions in repo
+4. Do not write incomplete functions.
+5. Do not write the original line numbers with the new code.
+6. Make sure the new code follows the same programming language conventions as the old code.
 
 Instead of writing "# Rest of Code", specify the lines to copy from the old file using an XML tag, inclusive (e.g., "<copied>0-25</copied>"). Make sure to use this exact format.
 Copy the correct line numbers and copy as long of a prefix and suffix as possible. For instance, if you want to insert code after line 50, start with "<copied>0-50</copied>".
 
 Example: New file:
 print("new file")
 </new_file>
```

### Comparing `sweepai-0.2.2/sweepai/core/react.py` & `sweepai-0.2.3/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/core/sweep_bot.py` & `sweepai-0.2.3/sweepai/core/sweep_bot.py`

 * *Files 13% similar despite different names*

```diff
@@ -51,14 +51,24 @@
                     logger.debug(file_change_request)
                     logger.debug(change_type)
                     file_change_requests.append(
                         FileChangeRequest.from_string(
                             file_change_request, change_type=change_type
                         )
                     )
+                # Create a dictionary to hold file names and their corresponding instructions
+                file_instructions_dict = {}
+                for file_change_request in file_change_requests:
+                # If the file name is already in the dictionary, append the new instructions
+                    if file_change_request.filename in file_instructions_dict:
+                        instructions, change_type = file_instructions_dict[file_change_request.filename]
+                        file_instructions_dict[file_change_request.filename] = (instructions + " " + file_change_request.instructions, change_type)
+                    else:
+                        file_instructions_dict[file_change_request.filename] = (file_change_request.instructions, file_change_request.change_type)
+                file_change_requests = [FileChangeRequest(filename=file_name, instructions=instructions, change_type=change_type) for file_name, (instructions, change_type) in file_instructions_dict.items()]
                 if file_change_requests:
                     return file_change_requests
             except RegexMatchError:
                 logger.warning("Failed to parse! Retrying...")
                 self.delete_messages_from_chat("files_to_change")
                 continue
         raise Exception("Could not generate files to change")
```

### Comparing `sweepai-0.2.2/sweepai/core/vector_db.py` & `sweepai-0.2.3/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/events.py` & `sweepai-0.2.3/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/handlers/create_pr.py` & `sweepai-0.2.3/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/handlers/on_comment.py` & `sweepai-0.2.3/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/handlers/on_review.py` & `sweepai-0.2.3/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/handlers/on_ticket.py` & `sweepai-0.2.3/sweepai/handlers/on_ticket.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""
+'''
 On Github ticket, get ChatGPT to deal with it
-"""
+'''
 
 # TODO: Add file validation
 
 import os
 import openai
 
 from loguru import logger
@@ -28,21 +28,21 @@
 openai.api_key = os.environ.get("OPENAI_API_KEY")
 
 update_index = modal.Function.lookup(DB_NAME, "update_index")
 
 bot_suffix = "I'm a bot that handles simple bugs and feature requests \
 but I might make mistakes. Please be kind!"
 
-collapsible_template = """
+collapsible_template = '''
 <details>
   <summary>{summary}</summary>
 
   {body}
 </details>
-"""
+'''
 
 chunker = modal.Function.lookup(UTILS_NAME, "Chunking.chunk")
 
 num_of_snippets_to_query = 30
 max_num_of_snippets = 5
 
 def on_ticket(
@@ -298,7 +298,8 @@
         except:
             pass
         item_to_react_to.create_reaction("rocket")
 
     posthog.capture(username, "success", properties={**metadata})
     logger.info("on_ticket success")
     return {"success": True}
+
```

### Comparing `sweepai-0.2.2/sweepai/slack.py` & `sweepai-0.2.3/sweepai/slack.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/utils/constants.py` & `sweepai-0.2.3/sweepai/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/utils/diff.py` & `sweepai-0.2.3/sweepai/utils/diff.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,38 +9,48 @@
     return ''.join(diff)
 
 def format_contents(file_contents, is_markdown=False):
     """
     Add arbitrary postprocessing here, this affects files and diffs
     """
     lines = file_contents.split('\n')
-    code_lines = []
-    in_code_block = True
 
     if is_markdown:
         return '\n'.join(lines) + '\n'
-    for line in lines:
-        stripped_line = line.strip()
+    
+    # Handle small files
+    if len(lines) <= 5:
+        final_lines = []
+        start_idx = 0
+        end_idx = len(lines)
+        for idx, line in enumerate(lines):
+            if start_idx == 0 and line.strip().startswith('```'):
+                start_idx = idx
+            if start_idx != 0 and line.strip().endswith('```'):
+                end_idx = idx
+        lines = lines[start_idx + 1:end_idx]
+        return '\n'.join(lines) + '\n'
 
-        # Check if line starts a code block
-        if stripped_line.startswith('```') and not in_code_block:
-            in_code_block = True
-            continue
-
-        # Check if line ends a code block
-        if stripped_line.endswith('```') and in_code_block:
-            in_code_block = False
-            continue
-
-        # Append line if it's inside a code block or if it's not an empty line
-        if not in_code_block:
-            continue
-        code_lines.append(line)
+    first_three_lines = lines[:3]
+    last_three_lines = lines[-3:]
+    first_line_idx = 0
+    last_line_idx = 3
+    for idx, line in enumerate(first_three_lines):
+        line = line.strip()
+        if line.startswith('```'):
+            first_line_idx = idx + 1
+    for idx, line in enumerate(last_three_lines):
+        line = line.strip()
+        if line.endswith('```'):
+            last_line_idx = idx
+    first_three_lines = first_three_lines[first_line_idx:]
+    last_three_lines = last_three_lines[:last_line_idx]
 
-    return '\n'.join(code_lines) + '\n'
+    lines = first_three_lines + lines[3:-3] + last_three_lines
+    return '\n'.join(lines) + '\n'
 
 
 def generate_new_file(modify_file_response: str, old_file_content: str) -> str:
     import re
 
     result_file = ""
     old_file_lines = old_file_content.splitlines()
```

### Comparing `sweepai-0.2.2/sweepai/utils/file_change_functions.py` & `sweepai-0.2.3/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/utils/github_utils.py` & `sweepai-0.2.3/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/utils/huggingface.py` & `sweepai-0.2.3/sweepai/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/utils/prompt_constructor.py` & `sweepai-0.2.3/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/utils/scorer.py` & `sweepai-0.2.3/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/utils/snippets.py` & `sweepai-0.2.3/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/sweepai/utils/utils.py` & `sweepai-0.2.3/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.2/setup.py` & `sweepai-0.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Sweep software chores',
-    'long_description': '<p align="center">\n    <img src=".assets/sweep-banner-github.png">\n</p>\n<p align="center">\n    <i>Spend time reviewing code generated by AI, not writing it.</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev/">🌐 Website</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://docs.sweep.dev/">📚 Docs</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://discord.gg/sweep-ai">📢 Discord</a>\n</p>\n\n<b>Sweep</b> allows you to create and review GitHub issues with easy.\nSimply describe any issue and Sweep will do the rest.\nIt will plan out what needs to be done, what changes to make, and write the changes to a PR. \n\n---\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🚀 Getting Started\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`\n\n3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. \n<img src=".assets/gradio-screenshot.png">\n\n💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. "👀" means it is taking a look, and it will generate the desired code\n4. "🚀" means the bot has finished its job and created a PR\n\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n\n## 🌠 Features\n* Automatic feature development\n* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address developer comments after PR is created\n* Code snippets embedding-based search\n* Chain-of-Thought retrieval using GPT Functions\n\n## 🗺️ Roadmap\nWe\'re currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).\n\n---\n\n\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
+    'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png">\n</p>\n<p align="center">\n    <i>Spend time reviewing code generated by AI, not writing it.</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev/">🌐 Website</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://docs.sweep.dev/">📚 Docs</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://discord.gg/sweep-ai">📢 Discord</a>\n</p>\n\n<b>Sweep</b> allows you to create and review GitHub issues with ease.\nSimply describe any issue and Sweep will do the rest.\nIt will plan out what needs to be done, what changes to make, and write the changes to a PR. \n\nSupported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports\n\n---\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🚀 Getting Started\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`. Note that you need python 3.11 or greater.\n\n3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. \n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\n💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need python 3.11 or greater.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. "👀" means it is taking a look, and it will generate the desired code\n4. "🚀" means the bot has finished its job and created a PR\n\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n\n## 🌠 Features\n* Automatic feature development\n* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address developer comments after PR is created\n* Code snippets embedding-based search\n* Chain-of-Thought retrieval using GPT Functions\n\n## 🗺️ Roadmap\nWe\'re currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).\n\n---\n\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,62 +1,66 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['sweepai',
 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
 package_data = \ {'': ['*']} install_requires = \ ['PyGithub==1.58.2', 'config-
 path>=1.0.3,<2.0.0', 'gradio>=3.35.2,<4.0.0', 'loguru>=0.6.0,<0.7.0',
 'requests>=2.28.2,<3.0.0', 'typer>=0.9.0,<0.10.0', 'urllib3>=2.0.3,<3.0.0']
 entry_points = \ {'console_scripts': ['sweep = sweepai.app.cli:app', 'sweepai =
-sweepai.app.cli:app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.2.2',
+sweepai.app.cli:app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.2.3',
 'description': 'Sweep software chores', 'long_description': '
-                    \n [.assets/sweep-banner-github.png]\n
+                  \n [https://github.com/sweepai/sweep/blob/
+  856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png]\n
 \n
         \n Spend time reviewing code generated by AI, not writing it.\n
 \n\n
           \nð_Website\n  â¢  \nð_Docs\n  â¢  \nð¢_Discord\n
-\n\nSweep allows you to create and review GitHub issues with easy.\nSimply
+\n\nSweep allows you to create and review GitHub issues with ease.\nSimply
 describe any issue and Sweep will do the rest.\nIt will plan out what needs to
-be done, what changes to make, and write the changes to a PR. \n\n---\n\n## â¨
-Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-
-ai) to one of your repos and see the magic happen.\n\n[Demo](https://
-github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-
-0af02f2b0e47)\n\n## ð Getting Started\n\n### ð¥ï¸ Sweep Chat\nSweep Chat
-allows you to interact with Sweep locally and will sync with GitHub. You can
-plan out your changes with Sweep, and then Sweep can create a pull request for
-you. \n\n1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to
-desired repos\n\n2. Run `pip install sweepai && sweep`\n\n3. This should spin
-up a GitHub auth flow in your browser. Copy-paste the ðµ blue 8-digit code
-from your terminal into the page. Then wait a few seconds and it should spin up
-Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo from
-the dropdown at the top (the Github app must be installed on this repo). Then
-start chatting with Sweep Chat. Relevant searched files will show up on the
-right. Sweep Chat can make PRs if you ask it to create a PR. \n[.assets/gradio-
+be done, what changes to make, and write the changes to a PR. \n\nSupported
+languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything
+else GPT-4 supports\n\n---\n\n## â¨ Demo\nFor the best experience, [install
+Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic
+happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-
+7317-40a7-9b5e-0af02f2b0e47)\n\n## ð Getting Started\n\n### ð¥ï¸ Sweep
+Chat\nSweep Chat allows you to interact with Sweep locally and will sync with
+GitHub. You can plan out your changes with Sweep, and then Sweep can create a
+pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/
+apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`. Note
+that you need python 3.11 or greater.\n\n3. This should spin up a GitHub auth
+flow in your browser. Copy-paste the ðµ blue 8-digit code from your terminal
+into the page. Then wait a few seconds and it should spin up Sweep Chat. You
+should only need to do the auth once.\n\n4. Pick a repo from the dropdown at
+the top (the Github app must be installed on this repo). Then start chatting
+with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat
+can make PRs if you ask it to create a PR. \n[https://github.com/sweepai/sweep/
+blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-
 screenshot.png]\n\nð¡ You can force dark mode by going to http://127.0.0.1:
 7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or
 if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/
-sweep && poetry install`\n2. `python sweepai/app/cli.py`\n\n### â¨ Sweep
-Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo,
-then creating an issue for the bot to address.\n\n1. Add the [Sweep GitHub app]
-(https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in
-repo, like "Sweep: Write tests"\n3. "ð" means it is taking a look, and it
-will generate the desired code\n4. "ð" means the bot has finished its job
-and created a PR\n\nFor more detailed docs, see [ð Quickstart](https://
-docs.sweep.dev/start).\n\n---\n\n## ð Story\n\nWe were frustrated by small
-tickets, like simple bug fixes, annoying refactors, and small features, each
-task requiring us to open our IDE to fix simple bugs. So, we decided to
-leverage the capabilities of ChatGPT to address this directly in
-GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can
-be parallelized: developers can spin up 10 tickets and Sweep will address them
-all at once.\n\n## ð The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3
-100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings
-model\n- Modal Labs for infra + deployment\n\n## ð  Features\n* Automatic
-feature development\n* PR auto self-review + comment handling (effectively
-[Reflexion](https://arxiv.org/abs/2303.11366))\n* Address developer comments
-after PR is created\n* Code snippets embedding-based search\n* Chain-of-Thought
-retrieval using GPT Functions\n\n## ðºï¸ Roadmap\nWe\'re currently working
-on responding to linters and external search. For more, see [ðºï¸ Roadmap]
-(https://docs.sweep.dev/roadmap).\n\n---\n\n\n
+sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need
+python 3.11 or greater.\n\n### â¨ Sweep Github App\nSetting up Sweep is as
+simple as adding the GitHub bot to a repo, then creating an issue for the bot
+to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai)
+to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3.
+"ð" means it is taking a look, and it will generate the desired code\n4.
+"ð" means the bot has finished its job and created a PR\n\nFor more detailed
+docs, see [ð Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## ð
+Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying
+refactors, and small features, each task requiring us to open our IDE to fix
+simple bugs. So, we decided to leverage the capabilities of ChatGPT to address
+this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire
+tickets and can be parallelized: developers can spin up 10 tickets and Sweep
+will address them all at once.\n\n## ð The Stack\n- GPT-4 32k 0613 (default)
+/ Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our
+embeddings model\n- Modal Labs for infra + deployment\n\n## ð  Features\n*
+Automatic feature development\n* PR auto self-review + comment handling
+(effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address
+developer comments after PR is created\n* Code snippets embedding-based
+search\n* Chain-of-Thought retrieval using GPT Functions\n\n## ðºï¸
+Roadmap\nWe\'re currently working on responding to linters and external search.
+For more, see [ðºï¸ Roadmap](https://docs.sweep.dev/roadmap).\n\n---\n\n
                          ***** \n Contributors\n *****
 \n
                      \n Thank you for your contribution!\n
 \n
           \n \n_[https://contrib.rocks/image?repo=sweepai/sweep]\n\n
 \n
                           \n and, of course, Sweep!\n
```

### Comparing `sweepai-0.2.2/PKG-INFO` & `sweepai-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.2.2
+Version: 0.2.3
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyGithub (==1.58.2)
 Requires-Dist: config-path (>=1.0.3,<2.0.0)
@@ -12,60 +12,62 @@
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
-    <img src=".assets/sweep-banner-github.png">
+    <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png">
 </p>
 <p align="center">
     <i>Spend time reviewing code generated by AI, not writing it.</i>
 </p>
 
 <p align="center">
 <a href="https://sweep.dev/">🌐 Website</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://docs.sweep.dev/">📚 Docs</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://discord.gg/sweep-ai">📢 Discord</a>
 </p>
 
-<b>Sweep</b> allows you to create and review GitHub issues with easy.
+<b>Sweep</b> allows you to create and review GitHub issues with ease.
 Simply describe any issue and Sweep will do the rest.
 It will plan out what needs to be done, what changes to make, and write the changes to a PR. 
 
+Supported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports
+
 ---
 
 ## ✨ Demo
 For the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.
 
 [Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)
 
 ## 🚀 Getting Started
 
 ### 🖥️ Sweep Chat
 Sweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. 
 
 1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
 
-2. Run `pip install sweepai && sweep`
+2. Run `pip install sweepai && sweep`. Note that you need python 3.11 or greater.
 
 3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.
 
 4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. 
-<img src=".assets/gradio-screenshot.png">
+<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">
 
 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
 
 #### From Source
 If you want the nightly build and or if the latest build has issues.
 
 1. `git clone https://github.com/sweepai/sweep && poetry install`
-2. `python sweepai/app/cli.py`
+2. `python sweepai/app/cli.py`. Note that you need python 3.11 or greater.
 
 ### ✨ Sweep Github App
 Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.
 
 1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
 2. Create new issue in repo, like "Sweep: Write tests"
 3. "👀" means it is taking a look, and it will generate the desired code
@@ -94,15 +96,14 @@
 * Chain-of-Thought retrieval using GPT Functions
 
 ## 🗺️ Roadmap
 We're currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).
 
 ---
 
-
 <h2 align="center">
     Contributors
 </h2>
 <p align="center">
     Thank you for your contribution!
 </p>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,40 +1,45 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.2.2 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.2.3 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.11,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyGithub (==1.58.2) Requires-Dist: config-path (>=1.0.3,<2.0.0)
 Requires-Dist: gradio (>=3.35.2,<4.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist: typer
 (>=0.9.0,<0.10.0) Requires-Dist: urllib3 (>=2.0.3,<3.0.0) Description-Content-
 Type: text/markdown
-                       [.assets/sweep-banner-github.png]
+                    [https://github.com/sweepai/sweep/blob/
+   856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png]
           Spend time reviewing code generated by AI, not writing it.
               ð_Website   â¢   ð_Docs   â¢   ð¢_Discord
-Sweep allows you to create and review GitHub issues with easy. Simply describe
+Sweep allows you to create and review GitHub issues with ease. Simply describe
 any issue and Sweep will do the rest. It will plan out what needs to be done,
-what changes to make, and write the changes to a PR. --- ## â¨ Demo For the
-best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of
-your repos and see the magic happen. [Demo](https://github.com/sweepai/sweep/
-assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47) ## ð Getting Started
-### ð¥ï¸ Sweep Chat Sweep Chat allows you to interact with Sweep locally and
-will sync with GitHub. You can plan out your changes with Sweep, and then Sweep
-can create a pull request for you. 1. Install [Sweep GitHub app](https://
-github.com/apps/sweep-ai) to desired repos 2. Run `pip install sweepai &&
-sweep` 3. This should spin up a GitHub auth flow in your browser. Copy-paste
+what changes to make, and write the changes to a PR. Supported languages:
+Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-
+4 supports --- ## â¨ Demo For the best experience, [install Sweep](https://
+github.com/apps/sweep-ai) to one of your repos and see the magic happen. [Demo]
+(https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-
+0af02f2b0e47) ## ð Getting Started ### ð¥ï¸ Sweep Chat Sweep Chat allows
+you to interact with Sweep locally and will sync with GitHub. You can plan out
+your changes with Sweep, and then Sweep can create a pull request for you. 1.
+Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
+2. Run `pip install sweepai && sweep`. Note that you need python 3.11 or
+greater. 3. This should spin up a GitHub auth flow in your browser. Copy-paste
 the ðµ blue 8-digit code from your terminal into the page. Then wait a few
 seconds and it should spin up Sweep Chat. You should only need to do the auth
 once. 4. Pick a repo from the dropdown at the top (the Github app must be
 installed on this repo). Then start chatting with Sweep Chat. Relevant searched
 files will show up on the right. Sweep Chat can make PRs if you ask it to
-create a PR. [.assets/gradio-screenshot.png] ð¡ You can force dark mode by
-going to http://127.0.0.1:7861/?__theme=dark. #### From Source If you want the
-nightly build and or if the latest build has issues. 1. `git clone https://
-github.com/sweepai/sweep && poetry install` 2. `python sweepai/app/cli.py` ###
-â¨ Sweep Github App Setting up Sweep is as simple as adding the GitHub bot to
-a repo, then creating an issue for the bot to address. 1. Add the [Sweep GitHub
+create a PR. [https://github.com/sweepai/sweep/blob/
+856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png] ð¡
+You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark. ####
+From Source If you want the nightly build and or if the latest build has
+issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
+`python sweepai/app/cli.py`. Note that you need python 3.11 or greater. ### â¨
+Sweep Github App Setting up Sweep is as simple as adding the GitHub bot to a
+repo, then creating an issue for the bot to address. 1. Add the [Sweep GitHub
 app](https://github.com/apps/sweep-ai) to desired repos 2. Create new issue in
 repo, like "Sweep: Write tests" 3. "ð" means it is taking a look, and it
 will generate the desired code 4. "ð" means the bot has finished its job and
 created a PR For more detailed docs, see [ð Quickstart](https://
 docs.sweep.dev/start). --- ## ð Story We were frustrated by small tickets,
 like simple bug fixes, annoying refactors, and small features, each task
 requiring us to open our IDE to fix simple bugs. So, we decided to leverage the
```

