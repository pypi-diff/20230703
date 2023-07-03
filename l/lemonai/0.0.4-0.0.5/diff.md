# Comparing `tmp/lemonai-0.0.4.tar.gz` & `tmp/lemonai-0.0.5.tar.gz`

## Comparing `lemonai-0.0.4.tar` & `lemonai-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     6344 2020-02-02 00:00:00.000000 lemonai-0.0.4/heatmap.ipynb
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.0.4/src/lemonai/__init__.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 lemonai-0.0.4/src/lemonai/api_wrapper.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 lemonai-0.0.4/src/lemonai/execute_workflow.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 lemonai-0.0.4/src/lemonai/filter_tools.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 lemonai-0.0.4/src/lemonai/get_integrations.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 lemonai-0.0.4/src/lemonai/tool.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.0.4/src/lemonai/toolkit.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 lemonai-0.0.4/src/lemonai/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.0.4/tests/.gitkeep
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 lemonai-0.0.4/LICENSE
--rw-r--r--   0        0        0    10317 2020-02-02 00:00:00.000000 lemonai-0.0.4/README.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 lemonai-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 lemonai-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0   136529 2020-02-02 00:00:00.000000 lemonai-0.0.5/heatmap-example.png
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/__init__.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/api_wrapper.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/execute_workflow.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/filter_tools.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/get_integrations.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/tool.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/toolkit.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 lemonai-0.0.5/src/lemonai/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.0.5/tests/.gitkeep
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 lemonai-0.0.5/LICENSE
+-rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 lemonai-0.0.5/README.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    12726 2020-02-02 00:00:00.000000 lemonai-0.0.5/PKG-INFO
```

### Comparing `lemonai-0.0.4/src/lemonai/api_wrapper.py` & `lemonai-0.0.5/src/lemonai/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.4/src/lemonai/execute_workflow.py` & `lemonai-0.0.5/src/lemonai/execute_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from lemonai.get_integrations import get_apis_from_env
 from lemonai.api_wrapper import APIWrapper
 from lemonai.toolkit import Toolkit
 from lemonai.filter_tools import filter_tools
 
 def execute_workflow(llm: BaseLLM, prompt_string: str):
 
-    logfile_path = "output.log"
+    logfile_path = "lemonai.log"
     logger.remove(handler_id=None)
     logger.add(logfile_path, format="{time} - {extra[session_id]} - {extra[operation_name]}")
 
     api_keys_dict, access_tokens_dict = get_apis_from_env()
     session_id = uuid.uuid4()
 
     _wrapper = APIWrapper()
```

### Comparing `lemonai-0.0.4/src/lemonai/filter_tools.py` & `lemonai-0.0.5/src/lemonai/filter_tools.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.4/src/lemonai/get_integrations.py` & `lemonai-0.0.5/src/lemonai/get_integrations.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.4/src/lemonai/tool.py` & `lemonai-0.0.5/src/lemonai/tool.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.4/src/lemonai/toolkit.py` & `lemonai-0.0.5/src/lemonai/toolkit.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.4/.gitignore` & `lemonai-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.4/LICENSE` & `lemonai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.4/README.md` & `lemonai-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-# 🍋 Lemon AI Python Client
+# 🍋 Lemon AI
 
 ## About
 
-**Build powerful copilots in minutes and execute highly efficient workflow automations by accessing internal tools like Airtable, Hubspot, Notion and Salesforce. With Lemon AI, it is possible to seamlessly grant access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs.**
+**Lemon AI Python client to build powerful AI assistants in minutes and execute highly efficient workflow automations by accessing tools like Airtable, Hubspot, Slack and Github. Most connectors available today are focused on read-only operations, limiting the potential of LLMs. Agents, on the other hand, have a tendency to hallucinate from time to time due to missing context or instructions. With Lemon AI, it is possible to give your agents access to well-defined APIs for more reliable read-and-write operations. In addition, Lemon AI functions allow you to reduce the risk of hallucinations even more by providing a way to statically define workflows that the model can rely on in case of insecurity.**
 
-## Getting Started
+## 🖲️ Getting Started
+
+### Install the Lemon AI Client
 
 To use Lemon AI in your Python project just run:
 
 ```bash
 pip install lemonai
 ```
 
@@ -16,14 +18,18 @@
 
 The tool uses Python packages `langchain` and `loguru`. In the case of any installation errors with Lemon AI, install both packages first and then install the Lemon AI package.
 
 Requires Python 3.8.1 and above.
 
 To use tools that require authentication, you have to store the corresponding access credentials in your environment in the format "{tool name}\_{authentication string}" where the authentication string is one of ["API_KEY", "SECRET_KEY", "SUBSCRIPTION_KEY", "ACCESS_KEY"] for API keys or ["ACCESS_TOKEN", "SECRET_TOKEN"] for authentication tokens. Examples are "OPENAI_API_KEY", "BING_SUBSCRIPTION_KEY", "AIRTABLE_ACCESS_TOKEN".
 
+### Spin Up the Lemon AI Server
+
+The interaction of your agents and all tools provided by Lemon AI is handled by the [Lemon AI Server](https://github.com/felixbrock/lemonai-server). To use Lemon AI you need to run the server on your local machine so the Lemon AI Python client can connect to it.
+
 ## Features
 
 ### Lemon AI Out-Of-The-Box Workflow Automation
 
 Get started in minutes by giving access to relevant tools and defining a task. Lemon AI handles the rest by finding a combination of relevant tools to solve the given task. Example of retrieving user data from Hackernews and writing it to a table in Airtable:
 
 ```python
@@ -96,41 +102,45 @@
 model = OpenAI(temperature=0)
 
 execute_workflow(llm=model, prompt_string=prompt)
 ```
 
 ## Traceability
 
-To allow you to gain full transparency on how your model interacted with your Lemon AI tools to solve the given task, we are writing all decisions made, tools used and operations performed to a local output.log file.
+To give full transparency on how your model interacts with Lemon AI tools to solve a given task, all decisions made, tools used and operations performed are written to a local lemonai.log file. Every time your LLM agent is interacting with the Lemon AI tool stack a corresponding log entry is created.
 
 ```log
 2023-06-26T11:50:27.708785+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - HackerNews: Get User
 2023-06-26T11:50:39.624035+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - Airtable: Append the data to a table
 2023-06-26T11:58:32.925228+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - HackerNews: Get User
 2023-06-26T11:58:43.988788+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - Airtable: Append the data to a table
 ```
 
+By using the [Lemon AI Analytics Notebook](https://github.com/felixbrock/lemonai-analytics) you can easily gain a better understanding of how frequently and in which workflow combination tools are used. As a result you can identify weak spots in your agent’s decision making capabilities and move to a more deterministic behaviour by defining [Lemon AI functions](#lemon-ai-functions---solve-tasks-based-on-predefined-workflows):
+
+![Heatmap Example](heatmap-example.png)
+
 ## Supported Tools
 
 Below is a list of all supported tools by Lemon AI and their ids (for use in the lemonai.json workflow file):
 
-#### HackerNews:
+### HackerNews
 
 - Get User: hackernews-get-user
 - Get Article: hackernews-get-article
 
-#### Airtable:
+### Airtable
 
 - Append data to a table: airtable-append-data
 - Delete data from a table: airtable-delete-data
 - List all data from a table: airtable-list-data
 - Read data from a table: airtable-read-data
 - Update data in a table: airtable-update-data
 
-#### Slack:
+### Slack
 
 - Archive channel: slack-channel-archive
 - Close channel: slack-channel-close
 - Create channel: slack-channel-create
 - Get channel: slack-channel-get
 - Get many channels: slack-channel-get-many
 - Get channel history: slack-channel-history
@@ -164,15 +174,15 @@
 - Update user's profile: slack-user-update-profile
 - Create user group: slack-user-group-create
 - Disable user group: slack-user-group-disable
 - Enable user group: slack-user-group-enable
 - Get many user groups: slack-user-group-get-many
 - Update user group: slack-user-group-update
 
-#### HubSpot:
+### HubSpot
 
 - Create/Update a contact: hubspot-create-update-contact
 - Delete a contact: hubspot-delete-contact
 - Get a contact: hubspot-get-contact
 - Get all contacts: hubspot-get-all-contacts
 - Get recently created/updated contacts: hubspot-get-recently-created-updated-contacts
 - Search contacts: hubspot-search-contacts
@@ -199,15 +209,15 @@
 - Get all fields from a form: hubspot-get-fields-form
 - Create a ticket: hubspot-create-ticket
 - Delete a ticket: hubspot-delete-ticket
 - Get a ticket: hubspot-get-ticket
 - Get all tickets: hubspot-get-all-tickets
 - Update a ticket: hubspot-update-ticket
 
-#### Github:
+### Github
 
 - Create a new file in repository: github-file-create
 - Delete a file in repository: github-file-delete
 - Edit a file in repository: github-file-edit
 - Get the data of a single file: github-file-get
 - Create a new issue: github-issue-create
 - Create a new comment on an issue: github-issue-comment
@@ -227,7 +237,26 @@
 - Create a new review: github-review-create
 - Get a review for a pull request: github-review-get
 - Get all reviews for a pull request: github-review-get-all
 - Update a review: github-review-update
 - Return the repositories of a user: github-user-repos
 - Invite a user to an organisation: github-user-org-invite
 - Return the repositories of an organisation: github-org-repos-get
+
+## ❤️‍🔥 Next Up
+
+- [x] Github
+- [ ] Kafka
+- [ ] Pipedrive
+- [ ] Monday.com
+- [ ] Stripe
+- [ ] Medium
+- [ ] Discord
+- [ ] Gmail
+- [ ] Google Calendar
+- [ ] Google Cloud Realtime Database
+- [ ] Salesforce
+- [ ] Notion
+
+## Contributing
+
+Do you have a connector you want to see included in Lemon AI or do you want to contribute in any other way? That's amazing 🥳 Just reach out, we are extremely open to contributions!
```

### Comparing `lemonai-0.0.4/pyproject.toml` & `lemonai-0.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lemonai"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Felix Brockmeier", email="fe.brockmeier@gmail.com" },
 ]
 description = "Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs."
 readme = "README.md"
 requires-python = ">=3.8.1"
 classifiers = [
@@ -18,9 +18,9 @@
 ]
 dependencies = [
   "langchain",
   "loguru"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/feliciori/lemonai-py-client"
-"Bug Tracker" = "https://github.com/feliciori/lemonai-py-client/issues"
+"Homepage" = "https://github.com/felixbrock/lemonai-py-client"
+"Bug Tracker" = "https://github.com/felixbrock/lemonai-py-client/issues"
```

### Comparing `lemonai-0.0.4/PKG-INFO` & `lemonai-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: lemonai
-Version: 0.0.4
+Version: 0.0.5
 Summary: Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs.
-Project-URL: Homepage, https://github.com/feliciori/lemonai-py-client
-Project-URL: Bug Tracker, https://github.com/feliciori/lemonai-py-client/issues
+Project-URL: Homepage, https://github.com/felixbrock/lemonai-py-client
+Project-URL: Bug Tracker, https://github.com/felixbrock/lemonai-py-client/issues
 Author-email: Felix Brockmeier <fe.brockmeier@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8.1
 Requires-Dist: langchain
 Requires-Dist: loguru
 Description-Content-Type: text/markdown
 
-# 🍋 Lemon AI Python Client
+# 🍋 Lemon AI
 
 ## About
 
-**Build powerful copilots in minutes and execute highly efficient workflow automations by accessing internal tools like Airtable, Hubspot, Notion and Salesforce. With Lemon AI, it is possible to seamlessly grant access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs.**
+**Lemon AI Python client to build powerful AI assistants in minutes and execute highly efficient workflow automations by accessing tools like Airtable, Hubspot, Slack and Github. Most connectors available today are focused on read-only operations, limiting the potential of LLMs. Agents, on the other hand, have a tendency to hallucinate from time to time due to missing context or instructions. With Lemon AI, it is possible to give your agents access to well-defined APIs for more reliable read-and-write operations. In addition, Lemon AI functions allow you to reduce the risk of hallucinations even more by providing a way to statically define workflows that the model can rely on in case of insecurity.**
 
-## Getting Started
+## 🖲️ Getting Started
+
+### Install the Lemon AI Client
 
 To use Lemon AI in your Python project just run:
 
 ```bash
 pip install lemonai
 ```
 
@@ -32,14 +34,18 @@
 
 The tool uses Python packages `langchain` and `loguru`. In the case of any installation errors with Lemon AI, install both packages first and then install the Lemon AI package.
 
 Requires Python 3.8.1 and above.
 
 To use tools that require authentication, you have to store the corresponding access credentials in your environment in the format "{tool name}\_{authentication string}" where the authentication string is one of ["API_KEY", "SECRET_KEY", "SUBSCRIPTION_KEY", "ACCESS_KEY"] for API keys or ["ACCESS_TOKEN", "SECRET_TOKEN"] for authentication tokens. Examples are "OPENAI_API_KEY", "BING_SUBSCRIPTION_KEY", "AIRTABLE_ACCESS_TOKEN".
 
+### Spin Up the Lemon AI Server
+
+The interaction of your agents and all tools provided by Lemon AI is handled by the [Lemon AI Server](https://github.com/felixbrock/lemonai-server). To use Lemon AI you need to run the server on your local machine so the Lemon AI Python client can connect to it.
+
 ## Features
 
 ### Lemon AI Out-Of-The-Box Workflow Automation
 
 Get started in minutes by giving access to relevant tools and defining a task. Lemon AI handles the rest by finding a combination of relevant tools to solve the given task. Example of retrieving user data from Hackernews and writing it to a table in Airtable:
 
 ```python
@@ -112,41 +118,45 @@
 model = OpenAI(temperature=0)
 
 execute_workflow(llm=model, prompt_string=prompt)
 ```
 
 ## Traceability
 
-To allow you to gain full transparency on how your model interacted with your Lemon AI tools to solve the given task, we are writing all decisions made, tools used and operations performed to a local output.log file.
+To give full transparency on how your model interacts with Lemon AI tools to solve a given task, all decisions made, tools used and operations performed are written to a local lemonai.log file. Every time your LLM agent is interacting with the Lemon AI tool stack a corresponding log entry is created.
 
 ```log
 2023-06-26T11:50:27.708785+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - HackerNews: Get User
 2023-06-26T11:50:39.624035+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - Airtable: Append the data to a table
 2023-06-26T11:58:32.925228+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - HackerNews: Get User
 2023-06-26T11:58:43.988788+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - Airtable: Append the data to a table
 ```
 
+By using the [Lemon AI Analytics Notebook](https://github.com/felixbrock/lemonai-analytics) you can easily gain a better understanding of how frequently and in which workflow combination tools are used. As a result you can identify weak spots in your agent’s decision making capabilities and move to a more deterministic behaviour by defining [Lemon AI functions](#lemon-ai-functions---solve-tasks-based-on-predefined-workflows):
+
+![Heatmap Example](heatmap-example.png)
+
 ## Supported Tools
 
 Below is a list of all supported tools by Lemon AI and their ids (for use in the lemonai.json workflow file):
 
-#### HackerNews:
+### HackerNews
 
 - Get User: hackernews-get-user
 - Get Article: hackernews-get-article
 
-#### Airtable:
+### Airtable
 
 - Append data to a table: airtable-append-data
 - Delete data from a table: airtable-delete-data
 - List all data from a table: airtable-list-data
 - Read data from a table: airtable-read-data
 - Update data in a table: airtable-update-data
 
-#### Slack:
+### Slack
 
 - Archive channel: slack-channel-archive
 - Close channel: slack-channel-close
 - Create channel: slack-channel-create
 - Get channel: slack-channel-get
 - Get many channels: slack-channel-get-many
 - Get channel history: slack-channel-history
@@ -180,15 +190,15 @@
 - Update user's profile: slack-user-update-profile
 - Create user group: slack-user-group-create
 - Disable user group: slack-user-group-disable
 - Enable user group: slack-user-group-enable
 - Get many user groups: slack-user-group-get-many
 - Update user group: slack-user-group-update
 
-#### HubSpot:
+### HubSpot
 
 - Create/Update a contact: hubspot-create-update-contact
 - Delete a contact: hubspot-delete-contact
 - Get a contact: hubspot-get-contact
 - Get all contacts: hubspot-get-all-contacts
 - Get recently created/updated contacts: hubspot-get-recently-created-updated-contacts
 - Search contacts: hubspot-search-contacts
@@ -215,15 +225,15 @@
 - Get all fields from a form: hubspot-get-fields-form
 - Create a ticket: hubspot-create-ticket
 - Delete a ticket: hubspot-delete-ticket
 - Get a ticket: hubspot-get-ticket
 - Get all tickets: hubspot-get-all-tickets
 - Update a ticket: hubspot-update-ticket
 
-#### Github:
+### Github
 
 - Create a new file in repository: github-file-create
 - Delete a file in repository: github-file-delete
 - Edit a file in repository: github-file-edit
 - Get the data of a single file: github-file-get
 - Create a new issue: github-issue-create
 - Create a new comment on an issue: github-issue-comment
@@ -243,7 +253,26 @@
 - Create a new review: github-review-create
 - Get a review for a pull request: github-review-get
 - Get all reviews for a pull request: github-review-get-all
 - Update a review: github-review-update
 - Return the repositories of a user: github-user-repos
 - Invite a user to an organisation: github-user-org-invite
 - Return the repositories of an organisation: github-org-repos-get
+
+## ❤️‍🔥 Next Up
+
+- [x] Github
+- [ ] Kafka
+- [ ] Pipedrive
+- [ ] Monday.com
+- [ ] Stripe
+- [ ] Medium
+- [ ] Discord
+- [ ] Gmail
+- [ ] Google Calendar
+- [ ] Google Cloud Realtime Database
+- [ ] Salesforce
+- [ ] Notion
+
+## Contributing
+
+Do you have a connector you want to see included in Lemon AI or do you want to contribute in any other way? That's amazing 🥳 Just reach out, we are extremely open to contributions!
```

