# Comparing `tmp/splatnet3_scraper-0.8.1.tar.gz` & `tmp/splatnet3_scraper-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splatnet3_scraper-0.8.1.tar", max compression
+gzip compressed data, was "splatnet3_scraper-0.9.0.tar", max compression
```

## Comparing `splatnet3_scraper-0.8.1.tar` & `splatnet3_scraper-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    34915 2023-04-10 05:10:54.759478 splatnet3_scraper-0.8.1/LICENSE.md
--rw-r--r--   0        0        0    10984 2023-04-15 00:47:42.245111 splatnet3_scraper-0.8.1/README.md
--rw-r--r--   0        0        0     1916 2023-06-08 23:44:15.709425 splatnet3_scraper-0.8.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-08 23:33:41.510800 splatnet3_scraper-0.8.1/splatnet3_scraper/__init__.py
--rw-r--r--   0        0        0      271 2023-04-10 05:20:16.704543 splatnet3_scraper-0.8.1/splatnet3_scraper/auth/__init__.py
--rw-r--r--   0        0        0     3064 2023-04-10 05:20:16.704543 splatnet3_scraper-0.8.1/splatnet3_scraper/auth/environment_manager.py
--rw-r--r--   0        0        0      287 2023-04-10 05:10:54.769478 splatnet3_scraper-0.8.1/splatnet3_scraper/auth/exceptions.py
--rw-r--r--   0        0        0    10032 2023-04-14 23:55:14.106500 splatnet3_scraper-0.8.1/splatnet3_scraper/auth/graph_ql_queries.py
--rw-r--r--   0        0        0    44111 2023-05-26 03:02:35.840997 splatnet3_scraper-0.8.1/splatnet3_scraper/auth/nso.py
--rw-r--r--   0        0        0    28908 2023-04-10 05:20:16.704543 splatnet3_scraper-0.8.1/splatnet3_scraper/auth/token_manager.py
--rw-r--r--   0        0        0     7847 2023-05-26 03:02:35.840997 splatnet3_scraper-0.8.1/splatnet3_scraper/constants.py
--rw-r--r--   0        0        0      226 2023-04-10 05:20:16.704543 splatnet3_scraper-0.8.1/splatnet3_scraper/query/__init__.py
--rw-r--r--   0        0        0    13307 2023-04-10 05:20:16.704543 splatnet3_scraper-0.8.1/splatnet3_scraper/query/config.py
--rw-r--r--   0        0        0    16840 2023-04-10 05:10:54.769478 splatnet3_scraper-0.8.1/splatnet3_scraper/query/handler.py
--rw-r--r--   0        0        0    16980 2023-04-10 05:10:54.769478 splatnet3_scraper-0.8.1/splatnet3_scraper/query/json_parser.py
--rw-r--r--   0        0        0    27320 2023-06-09 05:47:10.000316 splatnet3_scraper-0.8.1/splatnet3_scraper/query/responses.py
--rw-r--r--   0        0        0      117 2023-04-10 05:10:54.769478 splatnet3_scraper-0.8.1/splatnet3_scraper/scraper/__init__.py
--rw-r--r--   0        0        0     9382 2023-04-10 05:20:16.704543 splatnet3_scraper-0.8.1/splatnet3_scraper/scraper/main.py
--rw-r--r--   0        0        0     6182 2023-04-14 04:47:23.115079 splatnet3_scraper-0.8.1/splatnet3_scraper/scraper/query_map.py
--rw-r--r--   0        0        0    18732 2023-04-16 03:44:19.509582 splatnet3_scraper-0.8.1/splatnet3_scraper/utils.py
--rw-r--r--   0        0        0    12156 1970-01-01 00:00:00.000000 splatnet3_scraper-0.8.1/setup.py
--rw-r--r--   0        0        0    11882 1970-01-01 00:00:00.000000 splatnet3_scraper-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    34915 2023-04-10 05:10:54.759478 splatnet3_scraper-0.9.0/LICENSE.md
+-rw-r--r--   0        0        0    10984 2023-04-15 00:47:42.245111 splatnet3_scraper-0.9.0/README.md
+-rw-r--r--   0        0        0     1916 2023-07-03 03:35:35.804985 splatnet3_scraper-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-03 05:52:40.454469 splatnet3_scraper-0.9.0/splatnet3_scraper/__init__.py
+-rw-r--r--   0        0        0      271 2023-04-10 05:20:16.704543 splatnet3_scraper-0.9.0/splatnet3_scraper/auth/__init__.py
+-rw-r--r--   0        0        0     3064 2023-04-10 05:20:16.704543 splatnet3_scraper-0.9.0/splatnet3_scraper/auth/environment_manager.py
+-rw-r--r--   0        0        0      287 2023-04-10 05:10:54.769478 splatnet3_scraper-0.9.0/splatnet3_scraper/auth/exceptions.py
+-rw-r--r--   0        0        0    10032 2023-04-14 23:55:14.106500 splatnet3_scraper-0.9.0/splatnet3_scraper/auth/graph_ql_queries.py
+-rw-r--r--   0        0        0    44201 2023-07-03 05:49:25.951451 splatnet3_scraper-0.9.0/splatnet3_scraper/auth/nso.py
+-rw-r--r--   0        0        0    28908 2023-04-10 05:20:16.704543 splatnet3_scraper-0.9.0/splatnet3_scraper/auth/token_manager.py
+-rw-r--r--   0        0        0     7847 2023-05-26 03:02:35.840997 splatnet3_scraper-0.9.0/splatnet3_scraper/constants.py
+-rw-r--r--   0        0        0      226 2023-04-10 05:20:16.704543 splatnet3_scraper-0.9.0/splatnet3_scraper/query/__init__.py
+-rw-r--r--   0        0        0    13307 2023-04-10 05:20:16.704543 splatnet3_scraper-0.9.0/splatnet3_scraper/query/config.py
+-rw-r--r--   0        0        0    17119 2023-07-03 05:48:09.178422 splatnet3_scraper-0.9.0/splatnet3_scraper/query/handler.py
+-rw-r--r--   0        0        0    16980 2023-04-10 05:10:54.769478 splatnet3_scraper-0.9.0/splatnet3_scraper/query/json_parser.py
+-rw-r--r--   0        0        0    27320 2023-07-02 23:51:51.516981 splatnet3_scraper-0.9.0/splatnet3_scraper/query/responses.py
+-rw-r--r--   0        0        0      117 2023-04-10 05:10:54.769478 splatnet3_scraper-0.9.0/splatnet3_scraper/scraper/__init__.py
+-rw-r--r--   0        0        0     9912 2023-07-03 05:59:46.157011 splatnet3_scraper-0.9.0/splatnet3_scraper/scraper/main.py
+-rw-r--r--   0        0        0     6182 2023-04-14 04:47:23.115079 splatnet3_scraper-0.9.0/splatnet3_scraper/scraper/query_map.py
+-rw-r--r--   0        0        0    18732 2023-07-03 05:07:37.608933 splatnet3_scraper-0.9.0/splatnet3_scraper/utils.py
+-rw-r--r--   0        0        0    12156 1970-01-01 00:00:00.000000 splatnet3_scraper-0.9.0/setup.py
+-rw-r--r--   0        0        0    11882 1970-01-01 00:00:00.000000 splatnet3_scraper-0.9.0/PKG-INFO
```

### Comparing `splatnet3_scraper-0.8.1/LICENSE.md` & `splatnet3_scraper-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.8.1/README.md` & `splatnet3_scraper-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.8.1/pyproject.toml` & `splatnet3_scraper-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splatnet3_scraper"
-version = "0.8.1"
+version = "0.9.0"
 description = "Scraper for SplatNet 3 for Splatoon 3"
 authors = ["Cesar E Garza <cesar@cegarza.com>"]
 readme = "README.md"
 packages = [{include = "splatnet3_scraper"}]
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
```

### Comparing `splatnet3_scraper-0.8.1/splatnet3_scraper/auth/environment_manager.py` & `splatnet3_scraper-0.9.0/splatnet3_scraper/auth/environment_manager.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.8.1/splatnet3_scraper/auth/graph_ql_queries.py` & `splatnet3_scraper-0.9.0/splatnet3_scraper/auth/graph_ql_queries.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.8.1/splatnet3_scraper/auth/nso.py` & `splatnet3_scraper-0.9.0/splatnet3_scraper/auth/nso.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,15 @@
         self._user_access_token: str | None = None
         self._id_token: str | None = None
         self._nintendo_account_id: str | None = None
         self._coral_user_id: str | None = None
         self._gtoken: str | None = None
         self._user_info: dict[str, str] | None = None
         self._f_token_function: FToken_Gen = self.get_ftoken
+        self.logger = logging.getLogger(__name__)
 
     @staticmethod
     def new_instance() -> "NSO":
         """Creates a new instance of the NSO class with a new requests session.
 
         This is the recommended way to create a new instance of the NSO class,
         as it ensures that the session is a fresh session, however it is not
@@ -190,15 +191,15 @@
             str: The current version of the NSO app.
         """
         # TODO: Replace the iOS app store method with a method that does not
         # require scraping a website with scraping protection.
         response = self.session.get(IOS_APP_URL)
         version = version_re.search(response.text)
         if version is None:
-            logging.warning(
+            self.logger.warning(
                 "Failed to get version from app store, using fallback"
             )
             return APP_VERSION_FALLBACK
         return version.group(0).strip()
 
     @property
     def state(self) -> bytes:
@@ -478,42 +479,42 @@
 
         Returns:
             str: The gtoken. This is used to authenticate requests to the
                 Nintendo Switch Online API. This token is valid for 2 hours.
         """
         f_token_url = f_token_url if f_token_url is not None else IMINK_URL
         # Get user access token
-        logging.info("Getting user access token")
+        self.logger.info("Getting user access token")
         user_access_response = self.get_user_access_token(session_token)
         try:
             self._user_access_token = cast(
                 str, user_access_response["access_token"]
             )
             self._id_token = cast(str, user_access_response["id_token"])
         except (KeyError, TypeError, AttributeError):
             raise NintendoException(
                 "Failed to get user access token. "
                 + f"Response: {user_access_response}"
             )
 
-        logging.info("Getting user info")
+        self.logger.info("Getting user info")
         user_info = self.get_user_info(self._user_access_token)
         self._user_info = user_info
         self._nintendo_account_id = user_info["id"]
-        logging.info("Getting Web Service Access Token")
+        self.logger.info("Getting Web Service Access Token")
         (
             web_service_access_token,
             coral_user_id,
         ) = self.g_token_generation_phase_1(
             self._id_token,
             user_info,
             self._nintendo_account_id,
             f_token_url=f_token_url,
         )
-        logging.info("Getting gtoken")
+        self.logger.info("Getting gtoken")
         self._coral_user_id = coral_user_id
         gtoken = self.g_token_generation_phase_2(
             web_service_access_token,
             self._nintendo_account_id,
             self._coral_user_id,
             f_token_url=f_token_url,
         )
@@ -554,18 +555,18 @@
                 2. The request id.
                 3. The timestamp.
 
             If this argument is not provided or is ``None``, the default
             ``f_token`` generation method will be restored.
         """
         if new_function is None:
-            logging.info("Restoring default ftoken generation method")
+            self.logger.info("Restoring default ftoken generation method")
             self._f_token_function = self.get_ftoken
         else:
-            logging.info("Setting new ftoken generation method")
+            self.logger.info("Setting new ftoken generation method")
             self._f_token_function = new_function
 
     def get_ftoken(
         self,
         f_token_url: str,
         id_token: str,
         step: Literal[1] | Literal[2],
@@ -925,15 +926,15 @@
                 the request failed silently.
 
         Returns:
             str: The bullet token. This token is required to make any requests
                 to SplatNet 3, and is valid for 6 hours and 30 minutes after it
                 is obtained.
         """
-        logging.info("Getting bullet token")
+        self.logger.info("Getting bullet token")
         user_agent = (
             user_agent if user_agent is not None else DEFAULT_USER_AGENT
         )
         header = {
             "Content-Length": "0",
             "Content-Type": "application/json",
             "Accept-Language": user_info["language"],
@@ -981,10 +982,10 @@
         if self._web_view_version is not None:
             return self._web_view_version
         try:
             web_version = get_splatnet_version()
             self._web_view_version = web_version
             return web_version
         except SplatNetException as e:
-            logging.warning(str(e))
-            logging.warning("Using fallback web view version")
+            self.logger.warning(str(e))
+            self.logger.warning("Using fallback web view version")
             return WEB_VIEW_VERSION_FALLBACK
```

### Comparing `splatnet3_scraper-0.8.1/splatnet3_scraper/auth/token_manager.py` & `splatnet3_scraper-0.9.0/splatnet3_scraper/auth/token_manager.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.8.1/splatnet3_scraper/constants.py` & `splatnet3_scraper-0.9.0/splatnet3_scraper/constants.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.8.1/splatnet3_scraper/query/config.py` & `splatnet3_scraper-0.9.0/splatnet3_scraper/query/config.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.8.1/splatnet3_scraper/query/handler.py` & `splatnet3_scraper-0.9.0/splatnet3_scraper/query/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import logging
 
 import requests
 
 from splatnet3_scraper.auth import NSO, TokenManager
 from splatnet3_scraper.auth.exceptions import SplatNetException
 from splatnet3_scraper.auth.graph_ql_queries import queries
 from splatnet3_scraper.constants import TOKENS
@@ -40,14 +41,16 @@
                 the user uses the factory methods to create a new instance of
                 the class instead of instantiating it directly, as the factory
                 methods will automatically create a Config object for the user
                 based on the instantiation method they prefer and pass it to the
                 constructor.
         """
         self.config = config
+        self.logger = logging.getLogger(__name__)
+        self.logger.info("Initialized QueryHandler.")
 
     @staticmethod
     def from_config_file(
         config_path: str | None = None,
     ) -> "QueryHandler":
         """Creates a new instance of the class using a configuration file.
 
@@ -272,14 +275,15 @@
             QueryResponse: The response from the query. This object will contain
                 the data from the query, and will also contain the query hash
                 that was used to generate the query. This is useful for
                 debugging purposes.
         """
         response = self.__query_hash(query_hash, variables)
         if response.status_code != 200:
+            self.logger.info("Query failed, regenerating tokens and retrying.")
             self.config.token_manager.generate_all_tokens()
             response = self.__query_hash(query_hash, variables)
 
         if "errors" in response.json():
             errors = response.json()["errors"]
             error_message = (
                 "Query was successful but returned at least one error."
@@ -329,14 +333,15 @@
             QueryResponse: The response from the query. This object will contain
                 the data from the query, and will also contain the query hash
                 that was used to generate the query. This is useful for
                 debugging purposes.
         """
         response = self.__query(query_name, variables)
         if response.status_code != 200:
+            self.logger.info("Query failed, regenerating tokens and retrying.")
             self.config.token_manager.generate_all_tokens()
             response = self.__query(query_name, variables)
 
         if "errors" in response.json():
             errors = response.json()["errors"]
             error_message = (
                 "Query was successful but returned at least one error."
```

### Comparing `splatnet3_scraper-0.8.1/splatnet3_scraper/query/json_parser.py` & `splatnet3_scraper-0.9.0/splatnet3_scraper/query/json_parser.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.8.1/splatnet3_scraper/query/responses.py` & `splatnet3_scraper-0.9.0/splatnet3_scraper/query/responses.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.8.1/splatnet3_scraper/scraper/main.py` & `splatnet3_scraper-0.9.0/splatnet3_scraper/scraper/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from typing import Literal, cast, overload
 
 from splatnet3_scraper.query import QueryHandler, QueryResponse
 from splatnet3_scraper.scraper.query_map import QueryMap
 
 
 class SplatNet_Scraper:
@@ -14,14 +15,15 @@
     def __init__(self, query_handler: QueryHandler) -> None:
         """Initializes a SplatNet_Scraper.
 
         Args:
             query_handler (QueryHandler): The query handler to use.
         """
         self._query_handler = query_handler
+        self.logger = logging.getLogger(__name__)
 
     @staticmethod
     def from_session_token(session_token: str) -> "SplatNet_Scraper":
         """Creates a SplatNet_Scraper instance using the given session token.
 
         Args:
             session_token (str): The session token to use.
@@ -128,45 +130,57 @@
             detail_query = QueryMap.SALMON_DETAIL
             variable_name = "coopHistoryDetailId"
         else:
             detail_query = QueryMap.VS_DETAIL
             variable_name = "vsResultId"
 
         _limit = -1 if limit is None else limit
+        self.logger.info(f"Limit set to {_limit}")
 
         # Get the list of battles
         summary_query = self.__query(query)
 
         # Top level key depends on the game mode, but there is only one.
         top_level_key = summary_query.keys()[0]
         history_groups = summary_query[top_level_key, "historyGroups", "nodes"]
         out: list[QueryResponse] = []
+        queue: list[str] = []
         idx = 0
+        break_early = False
 
         for group in history_groups:
             group = cast(QueryResponse, group)
+            if break_early:
+                break
             for game in group["historyDetails", "nodes"]:
                 game = cast(QueryResponse, game)
                 if idx == _limit:
-                    return summary_query, out
+                    break_early = True
+                    break
                 idx += 1
-                game_id = game["id"]
+                game_id = cast(str, game["id"])
 
                 if isinstance(existing_ids, str):
                     if game_id == existing_ids:
-                        return summary_query, out
+                        break_early = True
+                        break
                 elif isinstance(existing_ids, list):
                     if game_id in existing_ids:
                         idx -= 1
                         continue
 
                 variables = {variable_name: game_id}
-                detailed_game = self.__query(detail_query, variables)
-                out.append(detailed_game)
+                queue.append(game_id)
 
+        self.logger.info(f"Queue length: {len(queue)}")
+        for idx, game_id in enumerate(queue):
+            self.logger.info(f"Getting game {idx + 1} of {len(queue)}")
+            variables = {variable_name: game_id}
+            detailed_game = self.__query(detail_query, variables)
+            out.append(detailed_game)
         return summary_query, out
 
     @overload
     def get_vs_battles(
         self,
         mode: str,
         detail: Literal[False],
```

### Comparing `splatnet3_scraper-0.8.1/splatnet3_scraper/scraper/query_map.py` & `splatnet3_scraper-0.9.0/splatnet3_scraper/scraper/query_map.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.8.1/splatnet3_scraper/utils.py` & `splatnet3_scraper-0.9.0/splatnet3_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.8.1/setup.py` & `splatnet3_scraper-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {'examples': ['pandas[examples]>=1.5.3,<2.0.0',
               'sqlalchemy[examples]>=2.0.1,<3.0.0',
               'psycopg2[examples]>=2.9.5,<3.0.0'],
  'parquet': ['pyarrow[parquet]>=10.0.1,<11.0.0']}
 
 setup_kwargs = {
     'name': 'splatnet3-scraper',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': 'Scraper for SplatNet 3 for Splatoon 3',
     'long_description': '# SplatNet 3 Scraper\n\n[![Tests Status](./reports/junit/tests-badge.svg?dummy=8484744)](https://htmlpreview.github.io/?https://github.com/cesaregarza/SplatNet3_Scraper/blob/main/reports/junit/report.html) ![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744) ![Flake8 Status](./reports/flake8/flake8-badge.svg?dummy=8484744) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n**SplatNet 3 Scraper** is a Python library for scraping data from the Splatoon 3 SplatNet 3 API. It is designed to be as lightweight as possible, with minimal dependencies to make it easy to integrate into other projects.\n\n**SplatNet 3 Scraper** started as a fork of **[s3s](https://github.com/frozenpandaman/s3s)**, but has since been rewritten from scratch while incorporating much of the login flow logic of s3s. As a result, I am deeply indebted to the authors of s3s for their work. This project would not have been possible without their efforts.\n\n## Table of Contents\n\n1. [Features](#features)\n2. [Documentation](#documentation)\n3. [Installation](#installation)\n4. [Usage](#usage)\n   - [Using the `scraper` module](#using-the-scraper-module)\n   - [Using the `query` module](#using-the-query-module)\n   - [Using the `auth` module](#using-the-auth-module)\n5. [Roadmap](#roadmap)\n6. [Contributing](#contributing)\n7. [License](#license)\n\n## Features\n\n- Lightweight and minimal dependencies. Only requires the `requests` library. Requires Python 3.10 or later.\n- The `scraper` module provides a user-level API that enables a quick and easy way to get data from the SplatNet 3 API, only requiring the user to provide their session token.\n- The `query` module provides a high-level API that provides a simple way to make queries to the SplatNet 3 API. It automatically handles authentication and query handling, and provides a simple interface for accessing the response data.\n- The `auth` module provides a low level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication.\n- Compatibility with the configuration file format used by `s3s`.\n- Responses from the SplatNet 3 API can be saved and loaded from disk, currently supporting the following formats:\n  - JSON\n  - gzip-compressed JSON\n  - csv\n  - parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)\n- Heavily documented codebase, with extensive docstrings and type annotations for nearly all functions and classes. The documentation is also available on [Read the Docs](https://splatnet3-scraper.readthedocs.io/en/latest/index.html).\n\n## Documentation\n\nDetailed documentation for SplatNet 3 Scraper, including usage instructions, examples, and API reference, is available on Read the Docs:\n\n[**SplatNet 3 Scraper Documentation**](https://splatnet3-scraper.readthedocs.io/en/latest/index.html)\n\nWe highly recommend referring to the documentation to get the most out of SplatNet 3 Scraper and understand its full capabilities.\n\n## Installation\n\n**SplatNet 3 Scraper** is currently under active development but is currently available on PyPI. It can be installed using pip:\n\n```bash\npip install splatnet3_scraper\n```\n\nNote that the current versions of **SplatNet 3 Scraper** are currently `v0.x.y`, which means that the API is not guaranteed to be stable and may change at any moment. As such, it is highly recommended that you pin the version of **SplatNet 3 Scraper** that you are using until the API is stabilized with the release of `v1.0.0`.\n\n## Usage\n\nThere are three ways to use **SplatNet 3 Scraper**. The first is to use the `scraper` module, which provides a top-level API that greatly simplifies the process of retrieving commonly requested data from SplatNet 3. This module is greatly recommended for most users. The second is to use the `query` module, which provides a high-level API that provides a simple interface to make queries to the SplatNet 3 API. This module is recommended for developers who can\'t find what they need with the `scraper` module. The third is to use the `auth` module, which provides a low-level API that gives the user the most control over the scraping process. This module is recommended for advanced developers who need to have full control over the authentication process. Whichever module you choose to use, all of them require providing a session token.\n\n### Using the `scraper` module\n\nThe `scraper` module is by far the easiest way to get data from the SplatNet 3 API and the module that is recommended for most users, especially those who are not highly experienced with Python. The `scraper` module provides multiple functions that can be used to retrieve commonly requested data from the SplatNet 3 API. The `scraper` module is designed to be used by users who are not highly experienced with Python or users who do not need to have full control over the scraping process.\n\nThis module is currently under active development and is not yet complete. Please check back later for more functions.\n\n### Using the `query` module\n\nThe `query` module is an easy-to-use module that enables fast and painless querying to the SplatNet 3 API. It handles authentication and query handling automagically, and provides a simple interface for accessing the response data. The `query` module is designed to be used by advanced users who need more control over the queries they make to the SplatNet 3 API. If you are looking for a simple way to get data from the SplatNet 3 API, you should use the `scraper` module instead.\n\nThe `query` module provides the `QueryHandler` class, which is used to make queries to the SplatNet 3 API. The `QueryHandler` class can be instantiated in one of a few ways: by providing a session token, by providing the path to a configuration file, or by loading environment variables.\n\n### Using the `auth` module\n\n:warning: **Warning: The `auth` module is intended for advanced users only. Most users should use the `scraper` or `query` modules for a simpler and more convenient experience.**\n\nThe `auth` module provides a low-level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication and is designed for advanced developers who need full control over the authentication process.\n\nTo use the `auth` module, you will need to import the necessary components and handle the authentication flow manually. Please refer to the [documentation](https://splatnet3-scraper.readthedocs.io/en/latest/index.html) for detailed instructions and examples on how to use the `auth` module.\n\n#### Instantiating the `QueryHandler` class by providing a session token\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_session_token("session_token")\nhandler.query("StageScheduleQuery")\n```\n\n#### Instantiating the `QueryHandler` class by providing the path to a configuration file\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_config_file(".splatnet3_scraper")\nhandler.query("StageScheduleQuery")\n```\n\n#### Instantiating the `QueryHandler` class by loading environment variables\n\nThe following environment variables are supported:\n\n- `SN3S_SESSION_TOKEN`\n- `SN3S_GTOKEN`\n- `SN3S_BULLET_TOKEN`\n\n```python\nfrom splatnet3_scrape.query import QueryHandler\nhandler = QueryHandler.from_env()\nhandler.query("StageScheduleQuery")\n```\n\n#### Querying the SplatNet 3 API\n\nThe `QueryHandler` class provides a `query` method that can be used to make queries to the SplatNet 3 API. The `query` method takes a single argument, which is the name of the query to make. The `query` method returns a `QueryResponse` object, which contains the response data from the SplatNet 3 API. The `QueryResponse` object provides a `data` property that can be used to access the response data. The `QueryResponse` module also supports numpy-style indexing, which can be used to quickly and clearly access specific parts of the response data. For example, the following code will print the game mode name of the the current stage rotation schedule:\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_env()\nresponse = handler.query("StageScheduleQuery")\nprint(response["xSchedules", "nodes", 0, "vsRule", "name"])\n```\n\n#### Saving and loading responses\n\nThe `QueryResponse` class provides a `parsed_json` method that can be used to generate a `JSONParser` object from the response data. The `JSONParser` class provides multiple ways of interacting with the given data, including the ability to save the data to disk in a variety of formats. There are currently four different formats that are supported and can be used by passing the desired format to a `to_*` method such as `to_json`. The following formats are supported:\n\n- JSON\n- gzip-compressed JSON\n- csv\n- parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)\n\nNote: csv and parquet formats work by converting the response data from a nested dictionary to a columnar format. This is not recommended for single queries, but can be useful for interacting with large amounts of data as it deduplicates the JSON structure and allows for more efficient storage and querying.\n\nThe following code will save the response data to a file named `response.json` in the current directory:\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_env()\nresponse = handler.query("StageScheduleQuery")\nresponse.parsed_json().to_json("response.json")\n```\n\nAdditionally, the `JSONParser` class provides a `from_*` method that can be used to load data from a file. The following code will load the response data from the file `response.json` in the current directory:\n\n```python\nfrom splatnet3_scraper.query import JSONParser\nparser = JSONParser.from_json("response.json")\n```\n\n## Symbols\n\n| Symbol | Meaning |\n| ------ | ------- |\n| :white_check_mark: | Implemented |\n| :construction: | In progress |\n| :world_map: | Planned |\n| :x: | Not planned |\n\n## Roadmap\n\n| Feature | Status |\n| ------- | ------ |\n| Support for the SplatNet 3 API | :white_check_mark: |\n| Full support for the SplatNet 3 API | :white_check_mark: |\n| Support for the SplatNet 2 API | :x: |\n| Obtaining session tokens | :white_check_mark: |\n| Full documentation | :white_check_mark: |\n| Full unit test coverage | :white_check_mark: |\n| Columnar data format support | :construction: |\n| CLI interface | :x: |\n| Integration with stat.ink | :x: |\n| PyPI package | :white_check_mark: |\n| Docker image | :world_map: |\n| Executable binary | :x: |\n\n## Contributing\n\nWe welcome contributions to SplatNet 3 Scraper! For detailed information on how to contribute, please refer to our [CONTRIBUTING.md](./CONTRIBUTING.md) file.\n\nTo report issues or request new features, please open an issue on the GitHub repository.\n\n## License\n\nSplatNet 3 Scraper is licensed under the GPLv3. See the [LICENSE](./LICENSE) file for more details.\n',
     'author': 'Cesar E Garza',
     'author_email': 'cesar@cegarza.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `splatnet3_scraper-0.8.1/PKG-INFO` & `splatnet3_scraper-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splatnet3-scraper
-Version: 0.8.1
+Version: 0.9.0
 Summary: Scraper for SplatNet 3 for Splatoon 3
 License: GPL-3.0-or-later
 Author: Cesar E Garza
 Author-email: cesar@cegarza.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

