# Comparing `tmp/servifai-0.1.0.tar.gz` & `tmp/servifai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servifai-0.1.0.tar", max compression
+gzip compressed data, was "servifai-0.1.1.tar", max compression
```

## Comparing `servifai-0.1.0.tar` & `servifai-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1067 2023-06-29 08:21:05.500102 servifai-0.1.0/LICENSE
--rw-r--r--   0        0        0     3544 2023-06-30 06:16:35.092259 servifai-0.1.0/README.md
--rw-r--r--   0        0        0      667 2023-06-30 06:13:02.180259 servifai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       53 2023-06-30 06:13:02.180259 servifai-0.1.0/servifai/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 08:25:16.344102 servifai-0.1.0/servifai/agents/__init__.py
--rw-r--r--   0        0        0     1063 2023-06-30 06:16:35.092259 servifai-0.1.0/servifai/agents/react.py
--rw-r--r--   0        0        0      113 2023-06-30 05:42:21.396259 servifai-0.1.0/servifai/default_config.yaml
--rw-r--r--   0        0        0        0 2023-06-29 08:25:16.344102 servifai-0.1.0/servifai/llms/__init__.py
--rw-r--r--   0        0        0      849 2023-06-30 06:16:35.092259 servifai-0.1.0/servifai/llms/openai.py
--rw-r--r--   0        0        0        0 2023-06-29 08:25:16.344102 servifai-0.1.0/servifai/memory/__init__.py
--rw-r--r--   0        0        0     1467 2023-06-29 18:08:26.490413 servifai-0.1.0/servifai/memory/chroma.py
--rw-r--r--   0        0        0     2317 2023-06-30 06:18:20.392259 servifai-0.1.0/servifai/servifai.py
--rw-r--r--   0        0        0        0 2023-06-29 08:25:16.344102 servifai-0.1.0/servifai/tools/__init__.py
--rw-r--r--   0        0        0     1291 2023-06-30 06:16:35.092259 servifai-0.1.0/servifai/tools/default.py
--rw-r--r--   0        0        0     6690 2023-06-30 06:16:35.092259 servifai-0.1.0/servifai/tools/knowledge_base.py
--rw-r--r--   0        0        0     4442 1970-01-01 00:00:00.000000 servifai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-29 08:21:05.500102 servifai-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4372 2023-07-03 04:05:52.164398 servifai-0.1.1/README.md
+-rw-r--r--   0        0        0      751 2023-07-03 04:14:35.980398 servifai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-07-03 04:11:23.100398 servifai-0.1.1/servifai/__init__.py
+-rw-r--r--   0        0        0      113 2023-06-30 05:42:21.396259 servifai-0.1.1/servifai/default_config.yaml
+-rw-r--r--   0        0        0        0 2023-06-29 08:25:16.344102 servifai-0.1.1/servifai/llm/__init__.py
+-rw-r--r--   0        0        0      849 2023-07-03 04:12:13.788398 servifai-0.1.1/servifai/llm/openai.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:25:16.344102 servifai-0.1.1/servifai/memory/__init__.py
+-rw-r--r--   0        0        0     1467 2023-06-29 18:08:26.490413 servifai-0.1.1/servifai/memory/chroma.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:25:16.344102 servifai-0.1.1/servifai/planning/__init__.py
+-rw-r--r--   0        0        0     1065 2023-07-03 03:50:52.248398 servifai-0.1.1/servifai/planning/react.py
+-rw-r--r--   0        0        0     2437 2023-07-03 04:12:13.796398 servifai-0.1.1/servifai/servifai.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:25:16.344102 servifai-0.1.1/servifai/toolbox/__init__.py
+-rw-r--r--   0        0        0     1291 2023-06-30 06:16:35.092259 servifai-0.1.1/servifai/toolbox/default.py
+-rw-r--r--   0        0        0     6689 2023-07-03 03:50:40.432398 servifai-0.1.1/servifai/toolbox/knowledge_base.py
+-rw-r--r--   0        0        0     5292 1970-01-01 00:00:00.000000 servifai-0.1.1/PKG-INFO
```

### Comparing `servifai-0.1.0/LICENSE` & `servifai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `servifai-0.1.0/pyproject.toml` & `servifai-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "servifai"
-version = "0.1.0"
-description = "A mini framework built on top of Langchain and Llamaindex to simplify creation of LLM powered Autonomous Agents"
+version = "0.1.1"
+description = "A mini framework built on top of Langchain and Llamaindex to provide LLM powered Autonomous Agents as a simplified service to assist users with their tasks"
 authors = ["Zoheb Abai <zohebabai@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
-langchain = "^0.0.216"
-llama-index = "^0.6.34.post1"
+langchain = "0.0.220"
+llama-index = "0.6.38"
 python-dotenv = "^1.0.0"
 chromadb = "^0.3.26"
 pypdf = "^3.11.0"
 pyyaml = "^6.0"
 nltk = "^3.8.1"
 duckduckgo-search = "^3.8.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pre-commit = "^3.3.3"
+scriv = {extras = ["toml"], version = "^1.3.1"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `servifai-0.1.0/servifai/agents/react.py` & `servifai-0.1.1/servifai/planning/react.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from langchain.agents import initialize_agent
 from langchain.chains.conversation.memory import ConversationBufferMemory
 
-from servifai.tools.default import DefaultTools
+from servifai.toolbox.default import DefaultTools
 
 
 class ReactChatAgent:
     def __init__(self, task, knowledge_base, llm):
         self.task = task
         self.llm = llm
         self.default_tool = DefaultTools(self.llm)
```

### Comparing `servifai-0.1.0/servifai/llms/openai.py` & `servifai-0.1.1/servifai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `servifai-0.1.0/servifai/memory/chroma.py` & `servifai-0.1.1/servifai/memory/chroma.py`

 * *Files identical despite different names*

### Comparing `servifai-0.1.0/servifai/servifai.py` & `servifai-0.1.1/servifai/servifai.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # Import Libraries
 import logging
 import sys
 from pathlib import Path
 
 import yaml
 
-from servifai.agents.react import ReactChatAgent
-from servifai.llms.openai import OpenAILLM
-from servifai.tools.knowledge_base import KnowledgeBase
+from servifai.llm.openai import OpenAILLM
+from servifai.planning.react import ReactChatAgent
+from servifai.toolbox.knowledge_base import KnowledgeBase
 
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 logging.getLogger().addHandler(logging.StreamHandler(stream=sys.stdout))
 
 BASE_DIR = Path(__file__).parent.parent.absolute()
 LOGS_DIR = Path(BASE_DIR, "logs")
 DEFAULT_CONFIG = Path(BASE_DIR, "servifai/default_config.yaml")
 
 
 class ServifAI:
     def __init__(self, config_file=None):
-        """Initializes a Assistify instance with specific config for a particular data
+        """Initializes a ServifAI instance with specific config for a given task
 
         Args:
             cfg (DictConfig): specific constants for a particular data
         """
         self.cfg = self._load_config(config_file)
         self.task = self.cfg["task"]
         self.oaillm = OpenAILLM(
@@ -61,11 +61,14 @@
         Args:
             question (str): user query
 
         Returns:
             str: Response
         """
         try:
-            logging.info("Generating response:")
-            return self.agent.chat(question)
+            if question != "":
+                logging.info("Generating response:")
+                return self.agent.chat(question)
+            else:
+                logging.warning("No input text provided by user")
         except Exception as e:
             logging.error(f"Error {e} occured")
```

### Comparing `servifai-0.1.0/servifai/tools/default.py` & `servifai-0.1.1/servifai/toolbox/default.py`

 * *Files identical despite different names*

### Comparing `servifai-0.1.0/servifai/tools/knowledge_base.py` & `servifai-0.1.1/servifai/toolbox/knowledge_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 from llama_index.indices.composability import ComposableGraph
 from llama_index.indices.keyword_table import SimpleKeywordTableIndex
 from llama_index.indices.query.query_transform.base import DecomposeQueryTransform
 from llama_index.query_engine.transform_query_engine import TransformQueryEngine
 from llama_index.vector_stores import ChromaVectorStore
 
-from servifai.llms.openai import OpenAILLM
+from servifai.llm.openai import OpenAILLM
 from servifai.memory.chroma import ChromaDB
 
 
 class VectorKnowledgeBase:
     def __init__(self, vector_indices, index_summaries, service_context):
         self._indices = vector_indices
         self._summaries = index_summaries
```

### Comparing `servifai-0.1.0/PKG-INFO` & `servifai-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,64 @@
 Metadata-Version: 2.1
 Name: servifai
-Version: 0.1.0
-Summary: A mini framework built on top of Langchain and Llamaindex to simplify creation of LLM powered Autonomous Agents
+Version: 0.1.1
+Summary: A mini framework built on top of Langchain and Llamaindex to provide LLM powered Autonomous Agents as a simplified service to assist users with their tasks
 License: MIT
 Author: Zoheb Abai
 Author-email: zohebabai@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chromadb (>=0.3.26,<0.4.0)
 Requires-Dist: duckduckgo-search (>=3.8.3,<4.0.0)
-Requires-Dist: langchain (>=0.0.216,<0.0.217)
-Requires-Dist: llama-index (>=0.6.34.post1,<0.7.0)
+Requires-Dist: langchain (==0.0.220)
+Requires-Dist: llama-index (==0.6.38)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pypdf (>=3.11.0,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 # ServifAI
+
 *A mini framework built on top of Langchain and Llamaindex to provide LLM powered Autonomous Agents as a simplified service to assist users with their tasks.*
 
-**Agent = LLM + memory + planning skills + tool use**
+![PyPI](https://img.shields.io/github/license/zohebabai/servifai)
+![PyPI](https://img.shields.io/pypi/v/servifai)
+
+## Overview
+
+**ServifAI (Task-based Agent) = LLM + Memory + Planning + Toolbox**
 
 ![agent_pic](https://lilianweng.github.io/posts/2023-06-23-agent/agent-overview.png)
 
+Instead of feeding all kinds of tools to a single agent and confusing it while selection, **ServifAI** narrows down the selection by combining only necessary tools on basis of the task at hand.
+
+Read [this article to understand How Agents works](https://lilianweng.github.io/posts/2023-06-23-agent/). 
+
 By default, **ServifAI** can chat while browsing internet and solving common math problems.
 
-# Installation
-```python
+### Current Toolbox Status:
+- Default (DuckDuckgo + LLM Math + PAL Math)
+- QA Knowledge Base (Vector Index + Knowledge Graphs)
+
+## Installation
+Works best with [Poetry](https://python-poetry.org/docs/)
+```bash
+poetry add servifai
+```
+With pip, you might have to install dependencies manually
+```bash
 pip install servifai
 ```
 
-# Usage
+## Usage
 Create a `.env` file
 ```env
 OPENAI_API_KEY='sk-...'
 ```
 
 Run Python Code
 ```python
@@ -56,16 +75,16 @@
 Me: Hi, How are you?
 ServifAI: Hi, I'm an AI language model, so I don't have feelings, but I'm here to help you with any questions or tasks you have!
 
 Me: What is the current weather of Bengaluru?
 ServifAI: The current weather in Bengaluru is mostly cloudy with a temperature of 81°F (27°C). The wind is coming from the north at 3 mph (5 km/h). Tomorrow's temperature is expected to be nearly the same as today.
 
 ```
-# Data Creation Recipe for Local Knowledge Extraction Tasks
-Consider the example of Uber 10Q filings. 
+## Data Creation Recipe for Local Knowledge Extraction Tasks
+Consider the example of [Uber 10Q filings](https://investor.uber.com/financials/default.aspx). 
 - Download the quaterly reports for year 2022 and 2023 as pdf and save it locally in a directory (here `reports`).
 - Create a config YAML file `uber_10q.yaml` inside a `configs` dir and fill details as:
 ```yaml
 task: 'qa_knowledge_base'
 
 vectordb:
   dir: "uber_10q"
@@ -111,12 +130,14 @@
 
 Me: How much cash did Uber have in last quarter of 2022?
 ServifAI: Based on the provided context, the cash balance for Uber at the end of Q4 2022 was $4.3 billion.
 
 ```
 
 # TODO:
+- [ ] Add other task based tools
 - [ ] Add support for Local LLMs
 - [ ] Add support for other VectorDBs
 - [ ] Add support for other unstructured data
 - [ ] Add support for structured data 
+- [ ] OpenAI funcs
```

