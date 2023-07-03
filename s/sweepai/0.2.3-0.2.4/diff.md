# Comparing `tmp/sweepai-0.2.3.tar.gz` & `tmp/sweepai-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.2.3.tar", max compression
+gzip compressed data, was "sweepai-0.2.4.tar", max compression
```

## Comparing `sweepai-0.2.3.tar` & `sweepai-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.3/LICENSE
--rw-r--r--   0        0        0     4221 2023-07-03 20:48:18.953249 sweepai-0.2.3/README.md
--rw-r--r--   0        0        0     1133 2023-07-03 20:48:48.779950 sweepai-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.3/sweepai/__init__.py
--rw-r--r--   0        0        0    10664 2023-07-01 23:29:41.701470 sweepai-0.2.3/sweepai/api.py
--rw-r--r--   0        0        0     5893 2023-07-02 07:30:30.847953 sweepai-0.2.3/sweepai/app/api_client.py
--rw-r--r--   0        0        0     6995 2023-07-02 07:30:30.847953 sweepai-0.2.3/sweepai/app/backend.py
--rw-r--r--   0        0        0      993 2023-07-03 20:38:42.899426 sweepai-0.2.3/sweepai/app/cli.py
--rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.3/sweepai/app/config.py
--rw-r--r--   0        0        0    10441 2023-07-03 19:27:15.637337 sweepai-0.2.3/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.3/sweepai/core/__init__.py
--rw-r--r--   0        0        0    16077 2023-07-02 07:30:30.847953 sweepai-0.2.3/sweepai/core/chat.py
--rw-r--r--   0        0        0     2306 2023-07-03 00:42:21.645402 sweepai-0.2.3/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     7286 2023-07-02 07:30:30.847953 sweepai-0.2.3/sweepai/core/entities.py
--rw-r--r--   0        0        0    13104 2023-07-03 00:42:21.645402 sweepai-0.2.3/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3509 2023-07-01 23:29:41.701470 sweepai-0.2.3/sweepai/core/react.py
--rw-r--r--   0        0        0    16496 2023-07-03 00:51:22.966350 sweepai-0.2.3/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    12030 2023-07-02 07:30:30.847953 sweepai-0.2.3/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     2536 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     3150 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    11178 2023-07-03 00:51:22.966350 sweepai-0.2.3/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0    19497 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/utils/__init__.py
--rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/utils/config.py
--rw-r--r--   0        0        0      670 2023-07-03 00:42:21.645402 sweepai-0.2.3/sweepai/utils/constants.py
--rw-r--r--   0        0        0     4072 2023-07-03 00:42:21.645402 sweepai-0.2.3/sweepai/utils/diff.py
--rw-r--r--   0        0        0      507 2023-07-03 00:42:21.645402 sweepai-0.2.3/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8166 2023-07-03 00:42:21.645402 sweepai-0.2.3/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/utils/hash.py
--rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/utils/huggingface.py
--rw-r--r--   0        0        0     5339 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      902 2023-07-02 07:30:30.851287 sweepai-0.2.3/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.3/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11266 2023-07-01 23:29:41.708137 sweepai-0.2.3/sweepai/utils/utils.py
--rw-r--r--   0        0        0     5286 2023-07-03 20:48:50.959518 sweepai-0.2.3/setup.py
--rw-r--r--   0        0        0     4769 2023-07-03 20:48:50.960638 sweepai-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4221 2023-07-03 20:48:18.953249 sweepai-0.2.4/README.md
+-rw-r--r--   0        0        0     1133 2023-07-03 21:08:33.771579 sweepai-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.4/sweepai/__init__.py
+-rw-r--r--   0        0        0    10664 2023-07-01 23:29:41.701470 sweepai-0.2.4/sweepai/api.py
+-rw-r--r--   0        0        0     5893 2023-07-02 07:30:30.847953 sweepai-0.2.4/sweepai/app/api_client.py
+-rw-r--r--   0        0        0     6995 2023-07-02 07:30:30.847953 sweepai-0.2.4/sweepai/app/backend.py
+-rw-r--r--   0        0        0      993 2023-07-03 20:38:42.899426 sweepai-0.2.4/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.4/sweepai/app/config.py
+-rw-r--r--   0        0        0    10441 2023-07-03 19:27:15.637337 sweepai-0.2.4/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.4/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    16077 2023-07-02 07:30:30.847953 sweepai-0.2.4/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2306 2023-07-03 00:42:21.645402 sweepai-0.2.4/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     7435 2023-07-03 21:07:59.718196 sweepai-0.2.4/sweepai/core/entities.py
+-rw-r--r--   0        0        0    13104 2023-07-03 00:42:21.645402 sweepai-0.2.4/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3509 2023-07-01 23:29:41.701470 sweepai-0.2.4/sweepai/core/react.py
+-rw-r--r--   0        0        0    16496 2023-07-03 00:51:22.966350 sweepai-0.2.4/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    12030 2023-07-02 07:30:30.847953 sweepai-0.2.4/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     2536 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     3150 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    11178 2023-07-03 00:51:22.966350 sweepai-0.2.4/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0    19497 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/utils/config.py
+-rw-r--r--   0        0        0      670 2023-07-03 00:42:21.645402 sweepai-0.2.4/sweepai/utils/constants.py
+-rw-r--r--   0        0        0     4072 2023-07-03 00:42:21.645402 sweepai-0.2.4/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      507 2023-07-03 00:42:21.645402 sweepai-0.2.4/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8166 2023-07-03 00:42:21.645402 sweepai-0.2.4/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/utils/huggingface.py
+-rw-r--r--   0        0        0     5339 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      902 2023-07-02 07:30:30.851287 sweepai-0.2.4/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.4/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11266 2023-07-01 23:29:41.708137 sweepai-0.2.4/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     5286 2023-07-03 21:09:00.725748 sweepai-0.2.4/setup.py
+-rw-r--r--   0        0        0     4820 2023-07-03 21:09:00.726324 sweepai-0.2.4/PKG-INFO
```

### Comparing `sweepai-0.2.3/LICENSE` & `sweepai-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/README.md` & `sweepai-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/pyproject.toml` & `sweepai-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.2.3"
+version = "0.2.4"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 PyGithub = "1.58.2"
 loguru = "^0.6.0"
 requests = "^2.28.2"
 urllib3 = "^2.0.3"
 gradio = "^3.35.2"
 config-path = "^1.0.3"
 typer = "^0.9.0"
```

### Comparing `sweepai-0.2.3/sweepai/api.py` & `sweepai-0.2.4/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/app/api_client.py` & `sweepai-0.2.4/sweepai/app/api_client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/app/backend.py` & `sweepai-0.2.4/sweepai/app/backend.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/app/cli.py` & `sweepai-0.2.4/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/app/config.py` & `sweepai-0.2.4/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/app/ui.py` & `sweepai-0.2.4/sweepai/app/ui.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/core/chat.py` & `sweepai-0.2.4/sweepai/core/chat.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/core/code_repair.py` & `sweepai-0.2.4/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/core/entities.py` & `sweepai-0.2.4/sweepai/core/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import re
-from typing import ClassVar, Literal, Self, Type
+from typing import ClassVar, Literal, Type, TypeVar
 from loguru import logger
 from pydantic import BaseModel
 
+try:   # Python 3.11+
+    from typing import Self
+except ImportError:  # Python 3.10
+    Self = TypeVar("Self", bound="RegexMatchableBaseModel")
+
 
 class Message(BaseModel):
     role: Literal["system"] | Literal["user"] | Literal["assistant"] | Literal["function"]
     content: str | None = None
     name: str | None = None
     function_call: dict | None = None
     key: str | None = None
```

### Comparing `sweepai-0.2.3/sweepai/core/prompts.py` & `sweepai-0.2.4/sweepai/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/core/react.py` & `sweepai-0.2.4/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/core/sweep_bot.py` & `sweepai-0.2.4/sweepai/core/sweep_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/core/vector_db.py` & `sweepai-0.2.4/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/events.py` & `sweepai-0.2.4/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/handlers/create_pr.py` & `sweepai-0.2.4/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/handlers/on_comment.py` & `sweepai-0.2.4/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/handlers/on_review.py` & `sweepai-0.2.4/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/handlers/on_ticket.py` & `sweepai-0.2.4/sweepai/handlers/on_ticket.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/slack.py` & `sweepai-0.2.4/sweepai/slack.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/utils/constants.py` & `sweepai-0.2.4/sweepai/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/utils/diff.py` & `sweepai-0.2.4/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/utils/file_change_functions.py` & `sweepai-0.2.4/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/utils/github_utils.py` & `sweepai-0.2.4/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/utils/huggingface.py` & `sweepai-0.2.4/sweepai/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/utils/prompt_constructor.py` & `sweepai-0.2.4/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/utils/scorer.py` & `sweepai-0.2.4/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/utils/snippets.py` & `sweepai-0.2.4/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/sweepai/utils/utils.py` & `sweepai-0.2.4/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.3/setup.py` & `sweepai-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': 'Sweep software chores',
     'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png">\n</p>\n<p align="center">\n    <i>Spend time reviewing code generated by AI, not writing it.</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev/">🌐 Website</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://docs.sweep.dev/">📚 Docs</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://discord.gg/sweep-ai">📢 Discord</a>\n</p>\n\n<b>Sweep</b> allows you to create and review GitHub issues with ease.\nSimply describe any issue and Sweep will do the rest.\nIt will plan out what needs to be done, what changes to make, and write the changes to a PR. \n\nSupported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports\n\n---\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🚀 Getting Started\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`. Note that you need python 3.11 or greater.\n\n3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. \n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\n💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need python 3.11 or greater.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. "👀" means it is taking a look, and it will generate the desired code\n4. "🚀" means the bot has finished its job and created a PR\n\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n\n## 🌠 Features\n* Automatic feature development\n* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address developer comments after PR is created\n* Code snippets embedding-based search\n* Chain-of-Thought retrieval using GPT Functions\n\n## 🗺️ Roadmap\nWe\'re currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).\n\n---\n\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.11,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['sweepai',
 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
 package_data = \ {'': ['*']} install_requires = \ ['PyGithub==1.58.2', 'config-
 path>=1.0.3,<2.0.0', 'gradio>=3.35.2,<4.0.0', 'loguru>=0.6.0,<0.7.0',
 'requests>=2.28.2,<3.0.0', 'typer>=0.9.0,<0.10.0', 'urllib3>=2.0.3,<3.0.0']
 entry_points = \ {'console_scripts': ['sweep = sweepai.app.cli:app', 'sweepai =
-sweepai.app.cli:app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.2.3',
+sweepai.app.cli:app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.2.4',
 'description': 'Sweep software chores', 'long_description': '
                   \n [https://github.com/sweepai/sweep/blob/
   856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png]\n
 \n
         \n Spend time reviewing code generated by AI, not writing it.\n
 \n\n
           \nð_Website\n  â¢  \nð_Docs\n  â¢  \nð¢_Discord\n
@@ -63,8 +63,8 @@
 \n
           \n \n_[https://contrib.rocks/image?repo=sweepai/sweep]\n\n
 \n
                           \n and, of course, Sweep!\n
 \n', 'author': 'Kevin Lu', 'author_email': None, 'maintainer': None,
 'maintainer_email': None, 'url': None, 'packages': packages, 'package_data':
 package_data, 'install_requires': install_requires, 'entry_points':
-entry_points, 'python_requires': '>=3.11,<4.0', } setup(**setup_kwargs)
+entry_points, 'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
```

### Comparing `sweepai-0.2.3/PKG-INFO` & `sweepai-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.2.3
+Version: 0.2.4
 Summary: Sweep software chores
 Author: Kevin Lu
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyGithub (==1.58.2)
 Requires-Dist: config-path (>=1.0.3,<2.0.0)
 Requires-Dist: gradio (>=3.35.2,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.2.3 Summary: Sweep software
-chores Author: Kevin Lu Requires-Python: >=3.11,<4.0 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyGithub (==1.58.2) Requires-Dist: config-path (>=1.0.3,<2.0.0)
-Requires-Dist: gradio (>=3.35.2,<4.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist: typer
-(>=0.9.0,<0.10.0) Requires-Dist: urllib3 (>=2.0.3,<3.0.0) Description-Content-
-Type: text/markdown
+Metadata-Version: 2.1 Name: sweepai Version: 0.2.4 Summary: Sweep software
+chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: PyGithub
+(==1.58.2) Requires-Dist: config-path (>=1.0.3,<2.0.0) Requires-Dist: gradio
+(>=3.35.2,<4.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0) Requires-Dist:
+requests (>=2.28.2,<3.0.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Requires-
+Dist: urllib3 (>=2.0.3,<3.0.0) Description-Content-Type: text/markdown
                     [https://github.com/sweepai/sweep/blob/
    856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/sweep-banner-github.png]
           Spend time reviewing code generated by AI, not writing it.
               ð_Website   â¢   ð_Docs   â¢   ð¢_Discord
 Sweep allows you to create and review GitHub issues with ease. Simply describe
 any issue and Sweep will do the rest. It will plan out what needs to be done,
 what changes to make, and write the changes to a PR. Supported languages:
```

