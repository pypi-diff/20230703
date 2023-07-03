# Comparing `tmp/twitchify-1.1.2.tar.gz` & `tmp/twitchify-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitchify-1.1.2.tar", last modified: Fri Jun 23 20:11:24 2023, max compression
+gzip compressed data, was "twitchify-1.2.0.tar", last modified: Mon Jul  3 17:33:31 2023, max compression
```

## Comparing `twitchify-1.1.2.tar` & `twitchify-1.2.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:11:24.562590 twitchify-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-23 20:11:10.000000 twitchify-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 20:11:24.562590 twitchify-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-23 20:11:10.000000 twitchify-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 20:11:24.562590 twitchify-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-23 20:11:10.000000 twitchify-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:11:24.558590 twitchify-1.1.2/twitch/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/broadcaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/goals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/survey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:11:24.562590 twitchify-1.1.2/twitch/types/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:11:24.562590 twitchify-1.1.2/twitch/types/eventsub/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/charity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/hypertrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:11:24.562590 twitchify-1.1.2/twitchify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 20:11:24.000000 twitchify-1.1.2/twitchify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-23 20:11:24.000000 twitchify-1.1.2/twitchify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 20:11:24.000000 twitchify-1.1.2/twitchify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 20:11:24.000000 twitchify-1.1.2/twitchify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 20:11:24.000000 twitchify-1.1.2/twitchify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:33:31.479354 twitchify-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-03 17:33:15.000000 twitchify-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-03 17:33:31.479354 twitchify-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-03 17:33:15.000000 twitchify-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:33:31.479354 twitchify-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-03 17:33:15.000000 twitchify-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:33:31.475354 twitchify-1.2.0/twitch/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/broadcaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/goals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15988 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/survey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:33:31.475354 twitchify-1.2.0/twitch/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:33:31.479354 twitchify-1.2.0/twitch/types/eventsub/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/charity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/hypertrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10869 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:33:31.479354 twitchify-1.2.0/twitchify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-03 17:33:31.000000 twitchify-1.2.0/twitchify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-03 17:33:31.000000 twitchify-1.2.0/twitchify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:33:31.000000 twitchify-1.2.0/twitchify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 17:33:31.000000 twitchify-1.2.0/twitchify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 17:33:31.000000 twitchify-1.2.0/twitchify.egg-info/top_level.txt
```

### Comparing `twitchify-1.1.2/LICENSE` & `twitchify-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/PKG-INFO` & `twitchify-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitchify
-Version: 1.1.2
+Version: 1.2.0
 Summary: A Python library for Twitch's WebSocket EventSub integration.
 Home-page: https://github.com/mrsnifo/twitchify
 Author: Snifo
 Author-email: Snifo@mail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/mrsnifo/twitchify/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `twitchify-1.1.2/README.md` & `twitchify-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/setup.py` & `twitchify-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/__init__.py` & `twitchify-1.2.0/twitch/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 A Python library for Twitch's WebSocket EventSub integration.
 
 :copyright: (c) 2023-present Snifo
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = 'Twitchify'
-__version__ = '1.1.2'
+__version__ = '1.2.0'
 __license__ = 'MIT License'
 __author__ = 'Snifo'
 __email__ = 'Snifo@mail.com'
 __github__ = 'https://github.com/mrsnifo/twitchify'
 
 from .client import *
 from .user import *
 from .broadcaster import *
 from .channel import *
 from .stream import *
 from .moderation import *
 from .reward import *
 from .goals import *
 from .survey import *
+from .guest import *
```

### Comparing `twitchify-1.1.2/twitch/broadcaster.py` & `twitchify-1.2.0/twitch/broadcaster.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     :param user: The user's image data.
     """
     def __init__(self, *, user: UserImages) -> None:
         self.profile = user['profile_image_url']
         self.offline = user['offline_image_url']
 
     def __repr__(self) -> str:
-        return f'<Images profile={self.profile} offline={self.profile}>'
+        return f'<Images profile={self.profile} offline={self.offline}>'
 
 
 class Broadcaster:
     """
     Represents a Twitch broadcaster.
 
     :param http: The HTTPClient instance for making HTTP requests.
@@ -72,27 +72,30 @@
         self.tier: Tier = user['broadcaster_type'] if user['broadcaster_type'] else 'regular'
         # Set the user type.
         self.type: Types = user['type'] if user['type'] else 'regular'
         self.joined_at: datetime = parse_rfc3339_timestamp(user['created_at'])
         # Updating the channel description from the user.
         self.bio = empty_to_none(text=user['description'])
 
-    @cache_decorator(expiry_seconds=20)
+    def __repr__(self) -> str:
+        return f'<Broadcaster id={self.id} name={self.name}>'
+
+    @cache_decorator(expiry_seconds=14)
     async def get_channel(self) -> Channel:
         """
         Retrieve the channel associated with the broadcaster.
 
         :return: An instance of the Channel class representing the channel.
         """
         data: ch.Channel = await self.__http.get_channel(broadcaster_id=self.id)
         _channel = Channel(channel=data)
         _channel.description = self.bio
         return _channel
 
-    @cache_decorator(expiry_seconds=12)
+    @cache_decorator(expiry_seconds=8)
     async def get_stream(self) -> Optional[Stream]:
         """
         Retrieve the stream of the broadcaster if currently live.
 
         :return: An instance of the Stream class representing the stream if live, otherwise None.
         """
         data: Optional[stm.Stream] = await self.__http.get_stream(user_id=self.id)
```

### Comparing `twitchify-1.1.2/twitch/channel.py` & `twitchify-1.2.0/twitch/channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types.eventsub import channel as chl
     from .types import channel as ch
     from typing import Optional, List, Union
 
-__all__ = ('Channel', 'Update', 'Subscription', 'SubscriptionGift', 'SubscriptionMessage', 'Cheer', 'Raid')
+__all__ = ('Channel', 'ChannelUpdate', 'Subscription', 'SubscriptionGift', 'SubscriptionMessage',
+           'Cheer', 'Raid')
 
 
 class Category:
     """
     Represents a category for a channel.
 
     :param channel: The channel data.
@@ -73,26 +74,26 @@
         return f'<Channel title={self.title} description={self.description}>'
 
 
 # -------------------------------------------
 #                  EventSub
 # -------------------------------------------
 
-class Update:
+class ChannelUpdate:
     """
     Represents when a channel updates their information.
 
     :param channel: The channel update data.
     """
-    __slots__ = ('title', 'language', 'is_mature', 'category')
+    __slots__ = ('title', 'language', 'classification', 'category')
 
     def __init__(self, channel: chl.Update) -> None:
         self.title: str = channel['title']
         self.language: str = channel['language']
-        self.is_mature: bool = channel['is_mature']
+        self.classification: List[str] = channel['content_classification_labels']
         # Category.
         _c = Category(channel=channel) if channel['category_id'] != '' else None
         self.category: Optional[Category] = _c
 
     def __repr__(self) -> str:
         return f'<Update title={self.title} language={self.language}>'
```

### Comparing `twitchify-1.1.2/twitch/client.py` & `twitchify-1.2.0/twitch/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,31 +59,31 @@
         self._connection: ConnectionState = ConnectionState(dispatcher=self.dispatch,
                                                             http=self._http,
                                                             events=self._sub_events)
 
     @property
     def user(self) -> Broadcaster:
         """
-        Retrieve the Broadcaster.
+        Retrieves the Broadcaster.
 
         :return: An instance of the Broadcaster class representing the user.
         """
         return self._connection.broadcaster
 
     async def get_channel(self) -> Channel:
         """
-       Retrieve the channel associated with the broadcaster.
+        Retrieves the channel associated with the broadcaster.
 
-       :return: An instance of the Channel class representing the channel.
-       """
+        :return: An instance of the Channel class representing the channel.
+        """
         return await self._connection.broadcaster.get_channel()
 
-    async def get_stream(self) -> Stream:
+    async def get_stream(self) -> Optional[Stream]:
         """
-        Retrieve the stream of the broadcaster if currently live.
+        Retrieves the stream of the broadcaster if currently live.
 
         :return: An instance of the Stream class representing the stream if live, otherwise None.
         """
         return await self._connection.broadcaster.get_stream()
 
     @property
     def _sub_events(self) -> List[str]:
@@ -171,12 +171,12 @@
         except Exception as error:
             if self._http is not None and self._http.is_open:
                 await self._http.close()
             raise error
 
     def run(self, access_token: str, refresh_token: Optional[str] = None) -> None:
         """
-        Runs the Twitch client by establishing a connection and initiating the event loop.
+        Runs the Twitch client without establishing a connection and initiating the event loop.
         """
         async def runner():
             await self.start(access_token, refresh_token)
         asyncio.run(runner())
```

### Comparing `twitchify-1.1.2/twitch/errors.py` & `twitchify-1.2.0/twitch/errors.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/gateway.py` & `twitchify-1.2.0/twitch/gateway.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/goals.py` & `twitchify-1.2.0/twitch/goals.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/http.py` & `twitchify-1.2.0/twitch/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,33 +20,32 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-from . import __version__, __github__
-from aiohttp import ClientSession, helpers
-from asyncio import Lock, sleep, Task
-from time import time
-from typing import TYPE_CHECKING, Optional, List, Callable, Any
-
 from .errors import (
     UnknownError, TwitchServerError, BadRequest, Unauthorized,
     Forbidden, HTTPException, SubscriptionError, NotFound)
+from aiohttp import ClientSession, helpers
+from . import __version__, __github__
+from asyncio import Lock, sleep, Task
 from .utils import format_seconds
+from time import time
 
-
+from typing import TYPE_CHECKING
 if TYPE_CHECKING:
-    from .types.stream import Stream
-    from .types.user import UserType
-    from .types.channel import Channel
     from .types.eventsub.subscriptions import SubscriptionInfo
+    from typing import Optional, List, Callable, Any
     from aiohttp import ClientWebSocketResponse
     from .types.http import Validate, Refresh
+    from .types.stream import Stream
+    from .types.user import UserType
+    from .types.channel import Channel
 
 import logging
 _logger = logging.getLogger(__name__)
 
 
 class Route:
     BASE_ROUTE: str = 'https://api.twitch.tv/helix/'
```

### Comparing `twitchify-1.1.2/twitch/message.py` & `twitchify-1.2.0/twitch/message.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/moderation.py` & `twitchify-1.2.0/twitch/moderation.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/reward.py` & `twitchify-1.2.0/twitch/reward.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/state.py` & `twitchify-1.2.0/twitch/state.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,45 +20,43 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-# Core
-from .channel import Update, Subscription, SubscriptionGift, SubscriptionMessage, Cheer, Raid
+from .channel import ChannelUpdate, Subscription, SubscriptionGift, SubscriptionMessage, Cheer, Raid
+from .guest import GuestStar, GuestStarUpdate, GuestStarSlotUpdate, GuestStarSettingsUpdate
 from .goals import Donation, Charity, Goal, HyperTrain
-from .user import Follower, User, UserUpdate
-from .broadcaster import Broadcaster
 from .moderation import Ban, UnBan, ShieldMode
 from .stream import Online, Offline, Shoutout
+from .user import Follower, User, UserUpdate
 from .reward import Reward, Redemption
 from .survey import Poll, Prediction
+from .broadcaster import Broadcaster
 from asyncio import Task
 
 from typing import TYPE_CHECKING
-
 if TYPE_CHECKING:
     from typing import Optional, Dict, Callable, Any, List
     from .http import HTTPClient
-    from .types.eventsub.reward import Redemption as Rp
     from .types.eventsub import (
         channel as chl,
         moderation as md,
         reward as rd,
         poll as pl,
         prediction as pd,
         charity as ch,
         goal as gl,
         hypertrain as ht,
         stream as sm,
-        user as us)
+        user as us,
+        guest as gt)
 
 import logging
-
 _logger = logging.getLogger(__name__)
 
 
 class ConnectionState:
     """
     Represents the state of the connection.
     """
@@ -97,15 +95,15 @@
         """
         self._dispatch('ready')
 
     async def parse_channel_update(self, data: chl.Update) -> None:
         """
         Parse a channel update event.
         """
-        _channel = Update(channel=data)
+        _channel = ChannelUpdate(channel=data)
         self._dispatch('channel_update', _channel)
 
     async def parse_channel_follow(self, data: chl.Follow) -> None:
         """
         Parse a channel follow event.
         """
         _user = Follower(channel=data)
@@ -200,26 +198,26 @@
     async def parse_channel_channel_points_custom_reward_remove(self, data: rd.Reward):
         """
         Parse a channel custom reward remove event for channel points.
         """
         _reward = Reward(reward=data)
         self._dispatch('points_reward_remove', _reward)
 
-    async def parse_channel_channel_points_custom_reward_redemption_add(self, data: Rp) -> None:
+    async def parse_channel_channel_points_custom_reward_redemption_add(self, d: rd.Redemption) -> None:
         """
         Parse a channel custom reward redemption add event for channel points.
         """
-        _redemption = Redemption(redemption=data)
+        _redemption = Redemption(redemption=d)
         self._dispatch('points_reward_redemption', _redemption)
 
-    async def parse_channel_channel_points_custom_reward_redemption_update(self, data: Rp) -> None:
+    async def parse_channel_channel_points_custom_reward_redemption_update(self, d: rd.Redemption) -> None:
         """
         Parse a channel custom reward redemption update event for channel points.
         """
-        _redemption = Redemption(redemption=data)
+        _redemption = Redemption(redemption=d)
         self._dispatch('points_reward_redemption_update', _redemption)
 
     # ========================> Survey <========================
     # Poll
     async def parse_channel_poll_begin(self, data: pl.Begin) -> None:
         """
         Parse a channel poll begin event.
@@ -394,7 +392,42 @@
         # Updating the broadcaster
         self.broadcaster.name = _update.name
         self.broadcaster.display_name = _update.display_name
         self.broadcaster.description = _update.description
         self.broadcaster.email = _update.email
         if 'user_update' in self.events:
             self._dispatch('user_update', _update)
+
+    async def parse_beta_channel_guest_star_session_begin(self, data: gt.Begin):
+        """
+        Parse channel guest star session begin event.
+        """
+        _guest_star = GuestStar(session=data)
+        self._dispatch('guest_star_session_begin', _guest_star)
+
+    async def parse_beta_channel_guest_star_session_end(self, data: gt.End):
+        """
+        Parse channel guest star session end event.
+        """
+        _guest_star = GuestStar(session=data)
+        self._dispatch('guest_star_session_end', _guest_star)
+
+    async def parse_beta_channel_guest_star_guest_update(self, data: gt.Update):
+        """
+        Parse channel guest star guest update event.
+        """
+        _guest_star = GuestStarUpdate(session=data)
+        self._dispatch('guest_star_guest_update', _guest_star)
+
+    async def parse_beta_channel_guest_star_slot_update(self, data: gt.SlotUpdate):
+        """
+        Parse channel guest star slot update event.
+        """
+        _guest_star = GuestStarSlotUpdate(slot=data)
+        self._dispatch('guest_star_slot_update', _guest_star)
+
+    async def parse_beta_channel_guest_star_settings_update(self, data: gt.SettingsUpdate):
+        """
+        Parse channel guest star settings update event.
+        """
+        _guest_star = GuestStarSettingsUpdate(settings=data)
+        self._dispatch('guest_star_settings_update', _guest_star)
```

### Comparing `twitchify-1.1.2/twitch/stream.py` & `twitchify-1.2.0/twitch/stream.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 class Stream:
     """
     Represents a stream.
 
     :param stream: The stream data.
     """
+    __slots__ = ('id', 'language', 'viewers', 'thumbnail_url', 'is_mature', 'started_at')
 
     def __init__(self, stream: mst.Stream) -> None:
         self.id: str = stream['id']
         self.language: str = stream['language']
         self.viewers: int = stream['viewer_count']
         self.thumbnail_url: str = stream['thumbnail_url']
         self.is_mature: bool = stream['is_mature']
@@ -58,14 +59,16 @@
 
 class Shoutout:
     """
     Represents a stream shoutout.
 
     :param shoutout: The shoutout data.
     """
+    __slots__ = ('__shoutout', 'viewer_count', 'started_at', '_cooldown_ends_at',
+                 '_target_cooldown_ends_at')
 
     def __init__(self, shoutout: Union[sm.ShoutoutCreate, sm.ShoutoutReceived]) -> None:
         self.__shoutout = shoutout
         self.viewer_count: int = shoutout['viewer_count']
         self.started_at: datetime = parse_rfc3339_timestamp(timestamp=shoutout['started_at'])
         self._cooldown_ends_at: Optional[str] = shoutout.get('cooldown_ends_at')
         self._target_cooldown_ends_at: Optional[str] = shoutout.get('target_cooldown_ends_at')
@@ -81,15 +84,15 @@
         :return: The sender User object.
         """
         if self._cooldown_ends_at:
             return User(user=self.__shoutout, prefix='broadcaster_user')
         return User(user=self.__shoutout, prefix='from_broadcaster_user')
 
     @property
-    def receiver(self):
+    def receiver(self) -> User:
         """
         Get the receiver of the shoutout.
 
         :return: The receiver User object.
         """
         if self._cooldown_ends_at is None:
             return User(user=self.__shoutout, prefix='broadcaster_user')
@@ -120,14 +123,15 @@
 
 class Online:
     """
     Represents an online stream.
 
     :param stream: The online stream data.
     """
+    __slots__ = ('user', 'id', 'type', 'started_at')
 
     def __init__(self, stream: sm.Online) -> None:
         self.user: User = User(user=stream, prefix='broadcaster_user')
         self.id: str = stream['id']
         self.type: str = stream['type']
         self.started_at: datetime = parse_rfc3339_timestamp(timestamp=stream['started_at'])
 
@@ -137,13 +141,14 @@
 
 class Offline:
     """
     Represents an offline stream.
 
     :param stream: The offline stream data.
     """
+    __slots__ = ('user',)
 
     def __init__(self, stream: sm.Offline) -> None:
         self.user: User = User(user=stream, prefix='broadcaster_user')
 
     def __repr__(self) -> str:
         return f'<Offline user={self.user}>'
```

### Comparing `twitchify-1.1.2/twitch/types/channel.py` & `twitchify-1.2.0/twitch/types/channel.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/types/eventsub/channel.py` & `twitchify-1.2.0/twitch/types/eventsub/channel.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from ..user import (SpecificBroadcaster, SpecificUser, SpecificAnonymous,
                     ToSpecificBroadcaster, FromSpecificBroadcaster)
 from ..message import Message
-from typing import Optional
+from typing import Optional, List
 
 
 class Update(SpecificBroadcaster):
     """
     Type: Channel Update
     Name: `channel.update`
-    Version: 1
+    Version: beta
     """
     title: str
     language: str
     category_id: str
     category_name: str
-    is_mature: bool
+    content_classification_labels: List[str]
 
 
 class Follow(SpecificBroadcaster, SpecificUser):
     """
     Type: Channel Follow
     Name: `channel.follow`
     Version: 2
```

### Comparing `twitchify-1.1.2/twitch/types/eventsub/charity.py` & `twitchify-1.2.0/twitch/types/eventsub/charity.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/types/eventsub/goal.py` & `twitchify-1.2.0/twitch/types/eventsub/goal.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/types/eventsub/hypertrain.py` & `twitchify-1.2.0/twitch/types/eventsub/hypertrain.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/types/eventsub/moderation.py` & `twitchify-1.2.0/twitch/types/eventsub/moderation.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/types/eventsub/poll.py` & `twitchify-1.2.0/twitch/types/eventsub/poll.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-# Core
 from ..user import SpecificBroadcaster
-# Libraries
 from typing import TypedDict, List, Literal
 
 
 class Voting(TypedDict):
     is_enabled: bool
     amount_per_vote: int
```

### Comparing `twitchify-1.1.2/twitch/types/eventsub/prediction.py` & `twitchify-1.2.0/twitch/types/eventsub/prediction.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/types/eventsub/reward.py` & `twitchify-1.2.0/twitch/types/eventsub/reward.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/types/eventsub/stream.py` & `twitchify-1.2.0/twitch/types/eventsub/stream.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/types/eventsub/subscriptions.py` & `twitchify-1.2.0/twitch/types/eventsub/subscriptions.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/types/eventsub/user.py` & `twitchify-1.2.0/twitch/types/eventsub/user.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/types/gateway.py` & `twitchify-1.2.0/twitch/types/gateway.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/types/http.py` & `twitchify-1.2.0/twitch/types/http.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/types/message.py` & `twitchify-1.2.0/twitch/types/message.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/types/stream.py` & `twitchify-1.2.0/twitch/types/stream.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/types/user.py` & `twitchify-1.2.0/twitch/types/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,23 +64,41 @@
 
 class SpecificBroadcaster(TypedDict):
     broadcaster_user_id: str
     broadcaster_user_login: str
     broadcaster_user_name: str
 
 
-class SpecificModerator(TypedDict):
-    moderator_user_id: str
-    moderator_user_login: str
-    moderator_user_name: str
-
-
 class SpecificAnonymous(TypedDict):
     user_id: Optional[str]
     user_login: Optional[str]
     user_name: Optional[str]
 
 
 class SpecificUser(TypedDict):
     user_id: str
     user_login: str
     user_name: str
+
+
+class SpecificModerator(TypedDict):
+    moderator_user_id: str
+    moderator_user_login: str
+    moderator_user_name: str
+
+
+class SpecificOpModerator(TypedDict):
+    moderator_user_id: Optional[str]
+    moderator_user_login: Optional[str]
+    moderator_user_name: Optional[str]
+
+
+class SpecificGuest(TypedDict):
+    guest_user_id: str
+    guest_user_name: str
+    guest_user_login: str
+
+
+class SpecificOpGuest(TypedDict):
+    guest_user_id: Optional[str]
+    guest_user_name: Optional[str]
+    guest_user_login: Optional[str]
```

### Comparing `twitchify-1.1.2/twitch/user.py` & `twitchify-1.2.0/twitch/user.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.2/twitch/utils.py` & `twitchify-1.2.0/twitch/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,25 +27,128 @@
 from datetime import datetime
 from functools import wraps
 import logging
 import json
 import time
 
 from typing import TYPE_CHECKING
-
 if TYPE_CHECKING:
     from .types.eventsub.subscriptions import SubscriptionInfo
     from typing import Optional, List, Callable, Awaitable, Any, Dict
 try:
     # noinspection PyPackageRequirements
     import orjson
 except ImportError:
     orjson = None
 
 
+# -------------------------------------------
+#     Documentation Changelog last check
+#     Date: 2023‑06‑29
+# -------------------------------------------
+Subscriptions: Dict[str, SubscriptionInfo] = {
+    'channel_update':
+        {'name': 'channel.update', 'version': 'beta'},
+    'follow':
+        {'name': 'channel.follow', 'version': '2'},
+    'subscribe':
+        {'name': 'channel.subscribe', 'version': '1'},
+    'subscription_end':
+        {'name': 'channel.subscription.end', 'version': '1'},
+    'subscription_gift':
+        {'name': 'channel.subscription.gift', 'version': '1'},
+    'subscription_message':
+        {'name': 'channel.subscription.message', 'version': '1'},
+    'cheer':
+        {'name': 'channel.cheer', 'version': '1'},
+    'raid':
+        {'name': 'channel.raid', 'version': '1'},
+    'ban':
+        {'name': 'channel.ban', 'version': '1'},
+    'unban':
+        {'name': 'channel.unban', 'version': '1'},
+    'moderator_add':
+        {'name': 'channel.moderator.add', 'version': '1'},
+    'moderator_remove':
+        {'name': 'channel.moderator.remove', 'version': '1'},
+    'points_reward_add':
+        {'name': 'channel.channel_points_custom_reward.add', 'version': '1'},
+    'points_reward_update':
+        {'name': 'channel.channel_points_custom_reward.update', 'version': '1'},
+    'points_reward_remove':
+        {'name': 'channel.channel_points_custom_reward.remove', 'version': '1'},
+    'points_reward_redemption':
+        {'name': 'channel.channel_points_custom_reward_redemption.add', 'version': '1'},
+    'points_reward_redemption_update':
+        {'name': 'channel.channel_points_custom_reward_redemption.update', 'version': '1'},
+    'poll_begin':
+        {'name': 'channel.poll.begin', 'version': '1'},
+    'poll_progress':
+        {'name': 'channel.poll.progress', 'version': '1'},
+    'poll_end':
+        {'name': 'channel.poll.end', 'version': '1'},
+    'prediction_begin':
+        {'name': 'channel.prediction.begin', 'version': '1'},
+    'prediction_progress':
+        {'name': 'channel.prediction.progress', 'version': '1'},
+    'prediction_lock':
+        {'name': 'channel.prediction.lock', 'version': '1'},
+    'prediction_end':
+        {'name': 'channel.prediction.end', 'version': '1'},
+    'charity_campaign_donate':
+        {'name': 'channel.charity_campaign.donate', 'version': '1'},
+    'charity_campaign_start':
+        {'name': 'channel.charity_campaign.start', 'version': '1'},
+    'charity_campaign_progress':
+        {'name': 'channel.charity_campaign.progress', 'version': '1'},
+    'charity_campaign_stop':
+        {'name': 'channel.charity_campaign.stop', 'version': '1'},
+    'goal_begin':
+        {'name': 'channel.goal.begin', 'version': '1'},
+    'goal_progress':
+        {'name': 'channel.goal.progress', 'version': '1'},
+    'goal_end':
+        {'name': 'channel.goal.end', 'version': '1'},
+    'hype_train_begin':
+        {'name': 'channel.hype_train.begin', 'version': '1'},
+    'hype_train_progress':
+        {'name': 'channel.hype_train.progress', 'version': '1'},
+    'hype_train_end':
+        {'name': 'channel.hype_train.end', 'version': '1'},
+    'shield_mode_begin':
+        {'name': 'channel.shield_mode.begin', 'version': '1'},
+    'shield_mode_end':
+        {'name': 'channel.shield_mode.end', 'version': '1'},
+    'shoutout_create':
+        {'name': 'channel.shoutout.create', 'version': '1'},
+    'shoutout_receive':
+        {'name': 'channel.shoutout.receive', 'version': '1'},
+    'stream_online':
+        {'name': 'stream.online', 'version': '1'},
+    'stream_offline':
+        {'name': 'stream.offline', 'version': '1'},
+    'guest_star_session_begin':
+        {'name': 'channel.guest_star_session.begin', 'version': 'beta'},
+    'guest_star_session_end':
+        {'name': 'channel.guest_star_session.end', 'version': 'beta'},
+    'guest_star_guest_update':
+        {'name': 'channel.guest_star_guest.update', 'version': 'beta'},
+    'guest_star_slot_update':
+        {'name': 'channel.guest_star_slot.update', 'version': 'beta'},
+    'guest_star_settings_update':
+        {'name': 'channel.guest_star_settings.update', 'version': 'beta'}}
+
+
+def get_subscriptions(*, events: List[str]) -> List[SubscriptionInfo]:
+    """
+    Retrieve a list of subscriptions that needed for subscribing to event.
+    """
+    return [Subscriptions[sub] for sub in events if Subscriptions.get(sub) is not None]
+
+
 def cache_decorator(expiry_seconds: int) -> Callable:
     """
     Cache decorator that caches the result of a function with a specified expiry time.
 
     :param expiry_seconds: The number of seconds to cache the result.
     :return: The decorated function.
     """
@@ -192,101 +295,7 @@
     formatter = ColoredFormatter('%(message)s')
     handler = logging.StreamHandler()
     handler.setFormatter(formatter)
     logger = logging.getLogger()
     logger.addHandler(handler)
     logger.setLevel(logging.INFO)
     return logger
-
-
-# -------------------------------------------
-#     Documentation Changelog last check
-#              Date: 2023‑06‑15
-# -------------------------------------------
-Subscriptions: Dict[str, SubscriptionInfo] = {
-    'channel_update':
-        {'name': 'channel.update', 'version': '1'},
-    'follow':
-        {'name': 'channel.follow', 'version': '2'},
-    'subscribe':
-        {'name': 'channel.subscribe', 'version': '1'},
-    'subscription_end':
-        {'name': 'channel.subscription.end', 'version': '1'},
-    'subscription_gift':
-        {'name': 'channel.subscription.gift', 'version': '1'},
-    'subscription_message':
-        {'name': 'channel.subscription.message', 'version': '1'},
-    'cheer':
-        {'name': 'channel.cheer', 'version': '1'},
-    'raid':
-        {'name': 'channel.raid', 'version': '1'},
-    'ban':
-        {'name': 'channel.ban', 'version': '1'},
-    'unban':
-        {'name': 'channel.unban', 'version': '1'},
-    'moderator_add':
-        {'name': 'channel.moderator.add', 'version': '1'},
-    'moderator_remove':
-        {'name': 'channel.moderator.remove', 'version': '1'},
-    'points_reward_add':
-        {'name': 'channel.channel_points_custom_reward.add', 'version': '1'},
-    'points_reward_update':
-        {'name': 'channel.channel_points_custom_reward.update', 'version': '1'},
-    'points_reward_remove':
-        {'name': 'channel.channel_points_custom_reward.remove', 'version': '1'},
-    'points_reward_redemption':
-        {'name': 'channel.channel_points_custom_reward_redemption.add', 'version': '1'},
-    'points_reward_redemption_update':
-        {'name': 'channel.channel_points_custom_reward_redemption.update', 'version': '1'},
-    'poll_begin':
-        {'name': 'channel.poll.begin', 'version': '1'},
-    'poll_progress':
-        {'name': 'channel.poll.progress', 'version': '1'},
-    'poll_end':
-        {'name': 'channel.poll.end', 'version': '1'},
-    'prediction_begin':
-        {'name': 'channel.prediction.begin', 'version': '1'},
-    'prediction_progress':
-        {'name': 'channel.prediction.progress', 'version': '1'},
-    'prediction_lock':
-        {'name': 'channel.prediction.lock', 'version': '1'},
-    'prediction_end':
-        {'name': 'channel.prediction.end', 'version': '1'},
-    'charity_campaign_donate':
-        {'name': 'channel.charity_campaign.donate', 'version': '1'},
-    'charity_campaign_start':
-        {'name': 'channel.charity_campaign.start', 'version': '1'},
-    'charity_campaign_progress':
-        {'name': 'channel.charity_campaign.progress', 'version': '1'},
-    'charity_campaign_stop':
-        {'name': 'channel.charity_campaign.stop', 'version': '1'},
-    'goal_begin':
-        {'name': 'channel.goal.begin', 'version': '1'},
-    'goal_progress':
-        {'name': 'channel.goal.progress', 'version': '1'},
-    'goal_end':
-        {'name': 'channel.goal.end', 'version': '1'},
-    'hype_train_begin':
-        {'name': 'channel.hype_train.begin', 'version': '1'},
-    'hype_train_progress':
-        {'name': 'channel.hype_train.progress', 'version': '1'},
-    'hype_train_end':
-        {'name': 'channel.hype_train.end', 'version': '1'},
-    'shield_mode_begin':
-        {'name': 'channel.shield_mode.begin', 'version': '1'},
-    'shield_mode_end':
-        {'name': 'channel.shield_mode.end', 'version': '1'},
-    'shoutout_create':
-        {'name': 'channel.shoutout.create', 'version': '1'},
-    'shoutout_receive':
-        {'name': 'channel.shoutout.receive', 'version': '1'},
-    'stream_online':
-        {'name': 'stream.online', 'version': '1'},
-    'stream_offline':
-        {'name': 'stream.offline', 'version': '1'}}
-
-
-def get_subscriptions(*, events: List[str]) -> List[SubscriptionInfo]:
-    """
-    Retrieve a list of subscriptions that needed for subscribing to event.
-    """
-    return [Subscriptions[sub] for sub in events if Subscriptions.get(sub) is not None]
```

### Comparing `twitchify-1.1.2/twitchify.egg-info/PKG-INFO` & `twitchify-1.2.0/twitchify.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitchify
-Version: 1.1.2
+Version: 1.2.0
 Summary: A Python library for Twitch's WebSocket EventSub integration.
 Home-page: https://github.com/mrsnifo/twitchify
 Author: Snifo
 Author-email: Snifo@mail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/mrsnifo/twitchify/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `twitchify-1.1.2/twitchify.egg-info/SOURCES.txt` & `twitchify-1.2.0/twitchify.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 twitch/__init__.py
 twitch/broadcaster.py
 twitch/channel.py
 twitch/client.py
 twitch/errors.py
 twitch/gateway.py
 twitch/goals.py
+twitch/guest.py
 twitch/http.py
 twitch/message.py
 twitch/moderation.py
 twitch/reward.py
 twitch/state.py
 twitch/stream.py
 twitch/survey.py
@@ -24,14 +25,15 @@
 twitch/types/message.py
 twitch/types/stream.py
 twitch/types/user.py
 twitch/types/eventsub/__init__.py
 twitch/types/eventsub/channel.py
 twitch/types/eventsub/charity.py
 twitch/types/eventsub/goal.py
+twitch/types/eventsub/guest.py
 twitch/types/eventsub/hypertrain.py
 twitch/types/eventsub/moderation.py
 twitch/types/eventsub/poll.py
 twitch/types/eventsub/prediction.py
 twitch/types/eventsub/reward.py
 twitch/types/eventsub/stream.py
 twitch/types/eventsub/subscriptions.py
```

