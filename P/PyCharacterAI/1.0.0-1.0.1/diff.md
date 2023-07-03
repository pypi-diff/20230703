# Comparing `tmp/PyCharacterAI-1.0.0.tar.gz` & `tmp/PyCharacterAI-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCharacterAI-1.0.0.tar", last modified: Sun Jul  2 16:43:01 2023, max compression
+gzip compressed data, was "PyCharacterAI-1.0.1.tar", last modified: Mon Jul  3 21:06:38 2023, max compression
```

## Comparing `PyCharacterAI-1.0.0.tar` & `PyCharacterAI-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 16:43:01.105013 PyCharacterAI-1.0.0/
--rw-rw-rw-   0        0        0     1061 2023-07-02 14:01:24.000000 PyCharacterAI-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2652 2023-07-02 16:43:01.106013 PyCharacterAI-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-02 16:43:01.087952 PyCharacterAI-1.0.0/PyCharacterAI/
--rw-rw-rw-   0        0        0       62 2023-07-02 13:49:24.000000 PyCharacterAI-1.0.0/PyCharacterAI/__init__.py
--rw-rw-rw-   0        0        0    11509 2023-07-02 16:37:36.000000 PyCharacterAI-1.0.0/PyCharacterAI/chat.py
--rw-rw-rw-   0        0        0     9262 2023-07-02 16:38:01.000000 PyCharacterAI-1.0.0/PyCharacterAI/client.py
--rw-rw-rw-   0        0        0     4897 2023-07-02 16:10:18.000000 PyCharacterAI-1.0.0/PyCharacterAI/message.py
--rw-rw-rw-   0        0        0     5081 2023-07-02 16:38:01.000000 PyCharacterAI-1.0.0/PyCharacterAI/requester.py
-drwxrwxrwx   0        0        0        0 2023-07-02 16:43:01.103035 PyCharacterAI-1.0.0/PyCharacterAI.egg-info/
--rw-rw-rw-   0        0        0     2652 2023-07-02 16:43:00.000000 PyCharacterAI-1.0.0/PyCharacterAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-07-02 16:43:00.000000 PyCharacterAI-1.0.0/PyCharacterAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 16:43:00.000000 PyCharacterAI-1.0.0/PyCharacterAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-07-02 16:43:00.000000 PyCharacterAI-1.0.0/PyCharacterAI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-02 16:43:00.000000 PyCharacterAI-1.0.0/PyCharacterAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2106 2023-07-02 16:24:46.000000 PyCharacterAI-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-02 16:43:01.108011 PyCharacterAI-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-07-02 16:37:36.000000 PyCharacterAI-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:06:38.057234 PyCharacterAI-1.0.1/
+-rw-rw-rw-   0        0        0     1061 2023-07-02 14:01:24.000000 PyCharacterAI-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2947 2023-07-03 21:06:38.057234 PyCharacterAI-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 21:06:38.043220 PyCharacterAI-1.0.1/PyCharacterAI/
+-rw-rw-rw-   0        0        0       62 2023-07-02 13:49:24.000000 PyCharacterAI-1.0.1/PyCharacterAI/__init__.py
+-rw-rw-rw-   0        0        0    11738 2023-07-03 19:37:29.000000 PyCharacterAI-1.0.1/PyCharacterAI/chat.py
+-rw-rw-rw-   0        0        0     9465 2023-07-03 15:57:59.000000 PyCharacterAI-1.0.1/PyCharacterAI/client.py
+-rw-rw-rw-   0        0        0     4697 2023-07-03 20:22:52.000000 PyCharacterAI-1.0.1/PyCharacterAI/message.py
+-rw-rw-rw-   0        0        0     5081 2023-07-02 16:38:01.000000 PyCharacterAI-1.0.1/PyCharacterAI/requester.py
+drwxrwxrwx   0        0        0        0 2023-07-03 21:06:38.055220 PyCharacterAI-1.0.1/PyCharacterAI.egg-info/
+-rw-rw-rw-   0        0        0     2947 2023-07-03 21:06:37.000000 PyCharacterAI-1.0.1/PyCharacterAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-07-03 21:06:37.000000 PyCharacterAI-1.0.1/PyCharacterAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 21:06:37.000000 PyCharacterAI-1.0.1/PyCharacterAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-03 21:06:37.000000 PyCharacterAI-1.0.1/PyCharacterAI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-03 21:06:37.000000 PyCharacterAI-1.0.1/PyCharacterAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2476 2023-07-03 20:50:02.000000 PyCharacterAI-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 21:06:38.058272 PyCharacterAI-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      734 2023-07-03 21:06:25.000000 PyCharacterAI-1.0.1/setup.py
```

### Comparing `PyCharacterAI-1.0.0/LICENSE` & `PyCharacterAI-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCharacterAI-1.0.0/PKG-INFO` & `PyCharacterAI-1.0.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,17 @@
-Metadata-Version: 2.1
-Name: PyCharacterAI
-Version: 1.0.0
-Summary: An unofficial asynchronous api wrapper for Character AI
-Home-page: https://github.com/Xtr4F/PyCharacterAI
-Author: XtraF
-Author-email: igoromarov15@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyCharacterAI
 > An unofficial asynchronous api wrapper for [Character AI](https://character.ai/). For Python.
 ##
 
 This library is based on the [Character AI Unofficial Node API](https://github.com/realcoloride/node_characterai), made by [realcoloride](https://github.com/realcoloride). 
 
-If you have any questions or problems, please contact me on Discord (xtraf) or [Telegram](https://t.me/XtraF).
+If you have any questions, problems, suggestions, please contact me:
 
+[![Tag](https://img.shields.io/badge/discord-server-black?style=flat&logo=Discord)](https://discord.gg/MN7pMbH2)
+[![Tag](https://img.shields.io/badge/telegram-dm-black?style=flat&logo=Telegram)](https://t.me/XtraF)
 ## Installation
 ```bash
 pip install PyCharacterAI
 ```
 
 
 ## Getting started
@@ -32,37 +19,37 @@
 ```Python
 from PyCharacterAI import Client
 ```
 ```Python
 client = Client()
 ```
 
-This library allows you to log in in two ways.
+This library allows you to authenticate in two ways:
 
 1. As a guest (Some api features are not available):
 ```Python
 await client.authenticate_as_guest()
 ```
 
-2. Using a token.
+2. Using a token:
 ```Python
 token = 'TOKEN'
 await client.authenticate_with_token(token)
 ```
 > Instructions for getting a token:
 > 
 > 1. Open the Character AI website in your browser
 > 2. Open the developer tools `F12` and go to the `Application` tab.
 > 3. Go to the `Storage` section and click on `Local Storage`.
 > 4. Look for the `@@auth0spajs@@::dyD3gE281MqgISG7FuIXYhL2WEknqZzv::https://auth0.character.ai/::openid profile email offline_access` key.
 > 5. Open the body and copy the access token.
 
 > ![Access_Token](https://i.imgur.com/09Q9mLe.png)
 >
-> вљ пёЏ Warning! Do not share this token with anyone!
+> ⚠️ Warning! Do not share this token with anyone!
 
 
 ## Simple example
 
 ```Python
 import asyncio
 from PyCharacterAI import Client
@@ -70,15 +57,15 @@
 token = "TOKEN"
 
 
 async def main():
     client = Client()
     await client.authenticate_with_token(token)
 
-    username = (await client.fetch_user())['user']['user']['username']
+    username = (await client.fetch_user())['user']['username']
     print(f'Authenticated as {username}')
 
     character_id = "iV5qb8ttzD7Ytl69U_-ONcW2tW_lrFrOVKExyKJHlJM"  # Lily (by @landon)
     chat = await client.create_or_continue_chat(character_id)
 
     while True:
         message = input(f'{username}: ')  # In: Hi!
@@ -86,7 +73,9 @@
         answer = await chat.send_message(message)
         print(f"Character: {answer.text}")  # Out: hello there! what kind of question you gonna ask me ? i'm here to assist you :)
 
 
 asyncio.run(main())
 ```
 
+## Documentation
+The library has [documentation](https://github.com/Xtr4F/PyCharacterAI/blob/main/docs/welcome.md).
```

### Comparing `PyCharacterAI-1.0.0/PyCharacterAI/chat.py` & `PyCharacterAI-1.0.1/PyCharacterAI/chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Any
+from typing import Any, Dict, Literal, Optional, Union
 
 from PyCharacterAI.message import Message, MessageHistory, OutgoingMessage, Reply
 
 
 class Chat:
     def __init__(self, client, character_id: str, continue_body: dict):
         self.character_id = character_id
@@ -12,15 +12,15 @@
         self.client = client
 
         ai = next(participant for participant in continue_body.get('participants') if not participant['is_human'])
 
         self.ai_id = ai['user']['username']
         self.requester = client.requester
 
-    async def fetch_history(self, page_num: int = None):
+    async def fetch_history(self, page_num: int = None) -> MessageHistory:
         if not self.client.is_authenticated():
             raise Exception('You must be authenticated to do this.')
 
         page_string = f"&page_num={page_num}" if page_num else ""
         url = f"https://beta.character.ai/chat/history/msgs/user/?history_external_id={self.history_id}{page_string}"
 
         request = await self.requester.request(url, options={
@@ -42,15 +42,15 @@
             has_more = response.get("has_more", False)
             next_page = response.get("next_page", None)
 
             return MessageHistory(chat=self, messages=messages, has_more=has_more, next_page=next_page)
 
         raise Exception('Could not fetch the chat history.')
 
-    async def get_histories(self, amount: int = 50):
+    async def get_histories(self, amount: int = 50) -> list:
         if not self.client.is_authenticated():
             raise Exception('You must be authenticated to do this.')
 
         request = await self.requester.request('https://beta.character.ai/chat/character/histories/', options={
             "method": 'POST',
             "headers": self.client.get_headers(),
             "body": json.dumps({
@@ -62,15 +62,15 @@
         if request.status == 200:
             response = await request.json()
 
             return response.get('histories', {})
 
         raise Exception('Failed to fetch stories')
 
-    async def start_new_chat(self):
+    async def start_new_chat(self) -> dict:
         if not self.client.is_authenticated():
             raise Exception('You must be authenticated to do this.')
 
         request = await self.requester.request('https://beta.character.ai/chat/history/create/', options={
             "method": 'POST',
             "headers": self.client.get_headers(),
             "body": json.dumps({
@@ -83,15 +83,15 @@
 
             self.history_id = response.get('external_id', self.history_id)
 
             return response
 
         raise Exception('Failed creating new chat.')
 
-    async def send_to_character(self, options):
+    async def send_to_character(self, options: dict) -> Reply:
         if not self.client.is_authenticated():
             raise Exception('You must be authenticated to do this.')
 
         payload = OutgoingMessage(chat=self, options=options).get_payload()
 
         request = await self.requester.request('https://beta.character.ai/chat/streaming/', options={
             "method": 'POST',
@@ -112,33 +112,33 @@
 
             if len(messages) == 0:
                 return []
 
             return messages.pop()
         raise Exception('Failed sending request to character.')
 
-    async def send_message(self, text: str, primary_msg_uuid=None, image_path=None, image_description=None):
+    async def send_message(self, text: str = "", primary_msg_uuid=None, image_path=None, image_description=None) -> Reply:
         options = {
-            "text": text,
+            "text": text
         }
 
         if primary_msg_uuid:
             options['primary_msg_uuid'] = primary_msg_uuid
 
         if image_path:
             options["image_rel_path"] = image_path
             options["image_description"] = image_description or ""
             options["image_description_type"] = "HUMAN" if image_description else "AUTO_IMAGE_CAPTIONING"
 
         return await self.send_to_character(options)
 
-    async def another_response(self, parent_msg_uuid):
+    async def another_response(self, parent_msg_uuid) -> Reply:
         return await self.send_to_character(options={'parent_msg_uuid': parent_msg_uuid})
 
-    async def generate_image(self, prompt: str):
+    async def generate_image(self, prompt: str) -> str:
         if not self.client.is_authenticated():
             raise Exception('You must be authenticated to do this.')
 
         request = await self.requester.request('https://beta.character.ai/chat/generate-image/', options={
             "method": 'POST',
             "headers": self.client.get_headers(),
             "body": json.dumps({"image_description": prompt})
@@ -147,94 +147,95 @@
         if request.status == 200:
             response = await request.json()
 
             return response.get('image_rel_path', '')
 
         raise Exception('Failed generating image.')
 
-    async def change_to_conversation(self, history_id: str, force: bool = False):
+    async def change_to_conversation(self, history_id: str, force: bool = False) -> bool:
         if not self.client.is_authenticated():
             raise Exception('You must be authenticated to do this.')
 
         if force:
             self.history_id = history_id
         else:
             conversations = await self.get_histories()
 
             for i in range(len(conversations)):
                 conversation = conversations[i]
                 if conversation.get('external_id', '') == history_id:
                     self.history_id = history_id
+                    return True
 
             raise Exception("Could not switch to conversation, it either doesn't exist or is invalid.")
 
-    async def get_message(self, message_uuid: str):
+    async def get_message(self, message_uuid: str) -> Message | None:
         if not self.client.is_authenticated():
             raise Exception('You must be authenticated to do this.')
 
         history = await self.fetch_history()
         history_messages = history.messages
 
         for i in range(len(history_messages)):
             message = history_messages[i]
 
             if message.uuid == message_uuid:
                 return message
 
         return None
 
-    async def get_following_messages(self, message_uuid: str, only_uuids: bool = True) -> list[Any] | None:
+    async def get_following_messages(self, message_uuid: str, only_uuids: bool = True) -> list[Message | str] | None:
         messages = []
 
         start_message: Message = await self.get_message(message_uuid)
         if start_message is None:
             return None
 
         history = await self.fetch_history()
         history_messages = history.messages
 
         print(len(history_messages))
 
         if len(history_messages) > start_message.pos_in_history:
             for i in range(start_message.pos_in_history, len(history_messages) + 1):
                 print(i)
-                message = history_messages[i-1]
+                message = history_messages[i - 1]
                 messages.append(message)
 
         else:
             messages.append(start_message)
 
         if only_uuids:
             uuids = []
             for message in messages:
                 uuids.append(message.uuid)
             return uuids
         else:
             return messages
 
-    async def get_related_messages(self, message_uuid: str, get_previous: bool = False, only_uuids: bool = True) -> list[Any] | None:
+    async def get_related_messages(self, message_uuid: str, get_previous: bool = False, only_uuids: bool = True) -> list[Message | str] | None:
         messages = []
 
         start_message: Message = await self.get_message(message_uuid)
         if start_message is None:
             return None
 
         history = await self.fetch_history()
         history_messages = history.messages
 
         if start_message.pos_in_history > 1:
             if start_message.is_alternative:
                 for i in range(start_message.pos_in_history, 0, -1):
-                    message = history_messages[i-1]
+                    message = history_messages[i - 1]
                     if message.is_alternative:
                         messages.append(message)
                     else:
                         messages.append(message)
                         if get_previous and i > 1:
-                            message = history_messages[i-2]
+                            message = history_messages[i - 2]
                             messages.append(message)
                         break
 
             else:
                 messages.append(start_message)
 
                 if get_previous:
@@ -256,32 +257,32 @@
             uuids = []
             for message in messages:
                 uuids.append(message.uuid)
             return uuids
         else:
             return messages
 
-    async def get_parent_message(self, message_uuid: str, only_uuid: bool = True):
+    async def get_parent_message(self, message_uuid: str, only_uuid: bool = True ) -> Message | str | None:
         parent_message = None
 
         start_message: Message = await self.get_message(message_uuid)
         if start_message is None:
             return None
 
         if start_message.pos_in_history < 3:
             return None
 
         history = await self.fetch_history()
         history_messages = history.messages
 
         if start_message.is_alternative:
-            for i in range(start_message.pos_in_history-1, 0, -1):
-                message = history_messages[i-1]
+            for i in range(start_message.pos_in_history - 1, 0, -1):
+                message = history_messages[i - 1]
                 if not message.is_alternative and message.pos_in_history > 1:
-                    parent_message = history_messages[i-2]
+                    parent_message = history_messages[i - 2]
                     break
 
         else:
             prev_message: Message = history_messages[start_message.pos_in_history - 2]
             if not prev_message.is_alternative:
                 parent_message = prev_message
 
@@ -289,15 +290,15 @@
             return None
 
         if only_uuid:
             return parent_message.uuid
         else:
             return parent_message
 
-    async def delete_messages(self, message_uuids: list):
+    async def delete_messages(self, message_uuids: list) -> bool:
         if not self.client.is_authenticated():
             raise Exception('You must be authenticated to do this.')
 
         if self.client.is_guest():
             raise Exception('Guest accounts cannot delete messages.')
 
         messages_to_delete = []
@@ -327,11 +328,7 @@
             if response.get('status', '') == 'OK':
                 return True
 
         raise Exception('Failed to delete messages.')
 
     async def delete_message(self, message_uuid: str):
         await self.delete_messages([message_uuid])
-
-
-
-
```

### Comparing `PyCharacterAI-1.0.0/PyCharacterAI/client.py` & `PyCharacterAI-1.0.1/PyCharacterAI/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,115 +16,115 @@
     }
 
     requester = Requester()
 
     def __init__(self):
         pass
 
-    async def fetch_categories(self):
+    async def fetch_categories(self) -> list[dict]:
         if not self._authenticated:
             raise Exception('You must be authenticated to do this.')
 
         request = await self.requester.request('https://beta.character.ai/chat/character/categories/')
 
         if request.status == 200:
-            return await request.json()
+            return (await request.json()).get("categories", [])
         raise Exception('Failed to fetch categories.')
 
-    async def fetch_user_config(self):
+    async def fetch_user_config(self) -> dict:
         if not self._authenticated:
             raise Exception('You must be authenticated to do this.')
 
         request = await self.requester.request('https://beta.character.ai/chat/config/', options={
             "headers": self._guest_headers
         })
 
         if request.status == 200:
             return await request.json()
         raise Exception('Failed fetching user configuration.')
 
-    async def fetch_user(self):
+    async def fetch_user(self) -> dict:
         if not self._authenticated:
             raise Exception('You must be authenticated to do this.')
 
         request = await self.requester.request('https://beta.character.ai/chat/user/', options={
             "headers": dict(self.get_headers())
         })
 
         if request.status == 200:
-            return await request.json()
+            return (await request.json()).get("user", {})
         raise Exception('Failed fetching user.')
 
-    async def fetch_featured_characters(self):
+    async def fetch_featured_characters(self) -> list:
         if not self._authenticated:
             raise Exception('You must be authenticated to do this.')
 
         request = await self.requester.request('https://beta.character.ai/chat/characters/featured_v2/', options={
             "headers": self.get_headers()
         })
 
         if request.status == 200:
-            return await request.json()
+            return (await request.json()).get('characters', [])
         raise Exception('Failed fetching featured characters.')
 
-    async def fetch_characters_by_category(self, curated: bool = False):
+    async def fetch_characters_by_category(self, curated: bool = False) -> dict[str, list]:
         if not self.requester.is_initialized():
-            return print("[PyCharacterAI] Error - client is not authenticated.")
+            raise Exception('You must be authenticated to do this.')
 
         url = f"https://beta.character.ai/chat/{'curated_categories' if curated else 'categories'}/characters/"
 
         request = await self.requester.request(url, options={
             "headers": self.get_headers()
         })
 
         property_ = 'characters_by_curated_category' if curated else 'characters_by_category'
 
         if request.status == 200:
             return (await request.json())[property_]
         raise Exception('Failed fetching characters by category.')
 
-    async def fetch_character_info(self, character_id: str):
+    async def fetch_character_info(self, character_id: str) -> dict:
         if not self._authenticated:
             raise Exception('You must be authenticated to do this.')
 
         request = await self.requester.request(f"https://beta.character.ai/chat/character/info-cached/{character_id}/",options={
             "headers": self.get_headers()
         })
 
         if request.status == 200:
             return (await request.json())['character']
         raise Exception('Could not fetch character information.')
 
-    async def search_characters(self, character_name: str):
+    async def search_characters(self, character_name: str) -> list:
         if not self._authenticated:
             raise Exception('You must be authenticated to do this.')
         if self._is_guest:
             raise Exception('Guest accounts cannot use the search feature.')
 
         request = await self.requester.request(f"https://beta.character.ai/chat/characters/search/?query={character_name}", options={
             "headers": self.get_headers()
         })
 
         if request.status == 200:
-            return await request.json()
+            return (await request.json()).get('characters')
         raise Exception('Could not search for characters.')
 
-    async def get_recent_conversations(self):
+    async def get_recent_conversations(self) -> list:
         if not self._authenticated:
             raise Exception('You must be authenticated to do this.')
 
         request = await self.requester.request('https://beta.character.ai/chat/characters/recent/', options={
             "headers": self.get_headers()
         })
 
         if request.status == 200:
-            return await request.json()
+            return (await request.json()).get('characters', {})
         raise Exception('Could not get recent conversations.')
 
-    async def create_chat(self, character_id: str):
+    async def create_chat(self, character_id: str) -> Chat:
         if not self._authenticated:
             raise Exception('You must be authenticated to do this.')
 
         request = await self.requester.request('https://beta.character.ai/chat/history/create/', options={
             "method": 'POST',
             "body": json.dumps({
                 "character_external_id": character_id
@@ -134,15 +134,15 @@
 
         if request.status == 200:
             response = await request.json()
             return Chat(client=self, character_id=character_id, continue_body=response)
 
         raise Exception('Could not create a new chat.')
 
-    async def continue_chat(self, character_id: str, history_id: str):
+    async def continue_chat(self, character_id: str, history_id: str) -> Chat:
         if not self._authenticated:
             raise Exception('You must be authenticated to do this.')
 
         request = await self.requester.request('https://beta.character.ai/chat/history/continue/', options={
             "method": 'POST',
             "body": json.dumps({
                 "character_external_id": character_id,
@@ -154,15 +154,15 @@
         if (await request.text()) == "history not found.":
             raise Exception("History not found.")
 
         if request.status == 200:
             response = await request.json()
             return Chat(client=self, character_id=character_id, continue_body=response)
 
-    async def create_or_continue_chat(self, character_id: str, history_id: str = None):
+    async def create_or_continue_chat(self, character_id: str, history_id: str = None) -> Chat:
         if not self._authenticated:
             raise Exception('You must be authenticated to do this.')
 
         request = await self.requester.request('https://beta.character.ai/chat/history/continue/', options={
             "method": 'POST',
             "body": json.dumps({
                 "character_external_id": character_id,
```

### Comparing `PyCharacterAI-1.0.0/PyCharacterAI/message.py` & `PyCharacterAI-1.0.1/PyCharacterAI/message.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,24 +61,14 @@
         self.src_name = options.get("src__name", None)
         self.src_internal_id = options.get("src__user__username", None)
         self.src_is_human = options.get("src__is_human", None)
         self.src_character_avatar_file_name = options.get("src__character__avatar_file_name", None)
         self.src_character_dict = options.get("src_char", None)
         self.responsible_username = options.get("responsible_user__username", None)
 
-    def get_avatar_link(self):
-        return f"https://characterai.io/i/80/static/avatars/uploaded/{self.src_character_avatar_file_name}"
-
-    def return_message(self):
-        return self.text
-
-
-
-
-
 
 class Reply:
     def __init__(self, chat, options: dict):
         if options.get("force_login", False):
             raise Exception("Too many messages! (this might be because you use a guest account)")
 
         self.chat = chat
```

### Comparing `PyCharacterAI-1.0.0/PyCharacterAI/requester.py` & `PyCharacterAI-1.0.1/PyCharacterAI/requester.py`

 * *Files identical despite different names*

### Comparing `PyCharacterAI-1.0.0/PyCharacterAI.egg-info/PKG-INFO` & `PyCharacterAI-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCharacterAI
-Version: 1.0.0
+Version: 1.0.1
 Summary: An unofficial asynchronous api wrapper for Character AI
 Home-page: https://github.com/Xtr4F/PyCharacterAI
 Author: XtraF
 Author-email: igoromarov15@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
@@ -15,16 +15,18 @@
 
 # PyCharacterAI
 > An unofficial asynchronous api wrapper for [Character AI](https://character.ai/). For Python.
 ##
 
 This library is based on the [Character AI Unofficial Node API](https://github.com/realcoloride/node_characterai), made by [realcoloride](https://github.com/realcoloride). 
 
-If you have any questions or problems, please contact me on Discord (xtraf) or [Telegram](https://t.me/XtraF).
+If you have any questions, problems, suggestions, please contact me:
 
+[![Tag](https://img.shields.io/badge/discord-server-black?style=flat&logo=Discord)](https://discord.gg/MN7pMbH2)
+[![Tag](https://img.shields.io/badge/telegram-dm-black?style=flat&logo=Telegram)](https://t.me/XtraF)
 ## Installation
 ```bash
 pip install PyCharacterAI
 ```
 
 
 ## Getting started
@@ -32,22 +34,22 @@
 ```Python
 from PyCharacterAI import Client
 ```
 ```Python
 client = Client()
 ```
 
-This library allows you to log in in two ways.
+This library allows you to authenticate in two ways:
 
 1. As a guest (Some api features are not available):
 ```Python
 await client.authenticate_as_guest()
 ```
 
-2. Using a token.
+2. Using a token:
 ```Python
 token = 'TOKEN'
 await client.authenticate_with_token(token)
 ```
 > Instructions for getting a token:
 > 
 > 1. Open the Character AI website in your browser
@@ -70,15 +72,15 @@
 token = "TOKEN"
 
 
 async def main():
     client = Client()
     await client.authenticate_with_token(token)
 
-    username = (await client.fetch_user())['user']['user']['username']
+    username = (await client.fetch_user())['user']['username']
     print(f'Authenticated as {username}')
 
     character_id = "iV5qb8ttzD7Ytl69U_-ONcW2tW_lrFrOVKExyKJHlJM"  # Lily (by @landon)
     chat = await client.create_or_continue_chat(character_id)
 
     while True:
         message = input(f'{username}: ')  # In: Hi!
@@ -86,7 +88,11 @@
         answer = await chat.send_message(message)
         print(f"Character: {answer.text}")  # Out: hello there! what kind of question you gonna ask me ? i'm here to assist you :)
 
 
 asyncio.run(main())
 ```
 
+## Documentation
+The library has [documentation](https://github.com/Xtr4F/PyCharacterAI/blob/main/docs/welcome.md).
+
+
```

### Comparing `PyCharacterAI-1.0.0/setup.py` & `PyCharacterAI-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
+import subprocess
+
 
 
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='PyCharacterAI',
-    version='1.0.0',
+    version='1.0.1',
     author='XtraF',
     author_email='igoromarov15@gmail.com',
     description='An unofficial asynchronous api wrapper for Character AI',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/Xtr4F/PyCharacterAI',
     packages=find_packages(),
@@ -20,7 +22,8 @@
                       'uuid>=1.30'],
     classifiers=[
         'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: MIT License'
     ],
     python_requires='>=3.7'
 )
+
```

