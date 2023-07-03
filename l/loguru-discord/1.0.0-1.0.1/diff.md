# Comparing `tmp/loguru_discord-1.0.0.tar.gz` & `tmp/loguru_discord-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loguru_discord-1.0.0.tar", max compression
+gzip compressed data, was "loguru_discord-1.0.1.tar", max compression
```

## Comparing `loguru_discord-1.0.0.tar` & `loguru_discord-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1062 2023-07-03 03:40:47.211349 loguru_discord-1.0.0/LICENSE
--rw-r--r--   0        0        0     1892 2023-07-03 03:40:47.211349 loguru_discord-1.0.0/README.md
--rw-r--r--   0        0        0      194 2023-07-03 03:40:47.211349 loguru_discord-1.0.0/loguru_discord/__init__.py
--rw-r--r--   0        0        0     3578 2023-07-03 03:40:47.211349 loguru_discord-1.0.0/loguru_discord/sink.py
--rw-r--r--   0        0        0     1216 2023-07-03 03:40:47.211349 loguru_discord-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 loguru_discord-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-03 04:31:28.970300 loguru_discord-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1824 2023-07-03 04:31:28.970300 loguru_discord-1.0.1/README.md
+-rw-r--r--   0        0        0      194 2023-07-03 04:31:28.970300 loguru_discord-1.0.1/loguru_discord/__init__.py
+-rw-r--r--   0        0        0     3209 2023-07-03 04:31:28.970300 loguru_discord-1.0.1/loguru_discord/sink.py
+-rw-r--r--   0        0        0     1216 2023-07-03 04:31:28.974300 loguru_discord-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2910 1970-01-01 00:00:00.000000 loguru_discord-1.0.1/PKG-INFO
```

### Comparing `loguru_discord-1.0.0/LICENSE` & `loguru_discord-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loguru_discord-1.0.0/README.md` & `loguru_discord-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -39,26 +39,25 @@
         embed=True
     ),
     level="WARNING",
 )
 
 try:
     value: float = 1 / 0
-except Exception as ex:
-    logger.error("Lorem ipsum dolor sit amet.", e=ex)
+except Exception as e:
+    logger.opt(exception=e).error("Lorem ipsum dolor sit amet.")
 ```
 
 ## Customization
 
 Upon constructing your handler, the following optional customizations are available via keyword arguments.
 
 -   **Username**: Username to use for the Discord Webhook message.
 -   **Avatar**: Image URL to use for the Discord Webhook message.
 -   **Embed**: Toggle whether to use plain codeblock formatting or rich embeds.
--   **Trace**: Toggle whether or not to include tracebacks (where available).
 
 ## Releases
 
 Loguru-Discord follows [Semantic Versioning](https://semver.org/) for tagging releases of the project.
 
 Changelogs can be found on the [Releases](https://github.com/EthanC/Loguru-Discord/releases) page in the [Keep a Changelog](https://keepachangelog.com/) format.
```

### Comparing `loguru_discord-1.0.0/loguru_discord/sink.py` & `loguru_discord-1.0.1/loguru_discord/sink.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import traceback
 from logging import Handler, LogRecord
 from typing import Optional, Self
 
 from discord_webhook import DiscordEmbed, DiscordWebhook
 
 
 class DiscordSink(Handler):
@@ -12,39 +11,35 @@
     def __init__(
         self: Self,
         webhookUrl: str,
         *,
         username: Optional[str] = None,
         avatarUrl: Optional[str] = None,
         embed: bool = False,
-        trace: bool = True,
     ) -> None:
         """
         Initialize a DiscordSink instance.
 
         Args:
             webhookUrl (str): Discord Webhook URL to write log messages to.
 
             `username` (`str`, optional): Username to use for the Webhook message.
                 Default is `None` (determined by Discord.)
             `avatarUrl` (`str`, optional): Image URL to use for the Webhook avatar.
                 Default is `None` (determined by Discord.)
             `embed` (`bool`, optional): A toggle to use the Discord Embed format.
                 Default is `False`.
-            `trace` (`bool`, optional): A toggle to include tracebacks in the log message.
-                Default is `True`.
         """
 
         super().__init__()
 
         self.webhookUrl: str = webhookUrl
         self.username: Optional[str] = username
         self.avatarUrl: Optional[str] = avatarUrl
         self.embed: bool = embed
-        self.trace: bool = trace
 
         self.webhook: DiscordWebhook = DiscordWebhook(
             self.webhookUrl,
             username=self.username,
             avatar_url=self.avatarUrl,
             rate_limit_retry=True,
         )
@@ -60,18 +55,14 @@
         - Embeds: https://discord.com/developers/docs/resources/channel#embed-object-embed-limits
 
         Ars:
             `record` (`logging.LogRecord`): Log record to send.
         """
 
         message: str = record.getMessage()
-        details: str = "".join(traceback.format_exception(*record.exc_info))
-
-        if (self.trace) and (record.exc_info):
-            message += f"\n\n{details}"
 
         if not self.embed:
             self.webhook.set_content(f"```py\n{message[:1990]}\n```")
         else:
             embed: DiscordEmbed = DiscordEmbed()
 
             match record.levelno:
```

### Comparing `loguru_discord-1.0.0/pyproject.toml` & `loguru_discord-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "loguru-discord"
-version = "1.0.0"
+version = "1.0.1"
 description = "Lightweight, easy-to-use Discord sink for Loguru."
 authors = ["EthanC <16727756+EthanC@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["loguru", "discord", "logging", "logger", "sink"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `loguru_discord-1.0.0/PKG-INFO` & `loguru_discord-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loguru-discord
-Version: 1.0.0
+Version: 1.0.1
 Summary: Lightweight, easy-to-use Discord sink for Loguru.
 License: MIT
 Keywords: loguru,discord,logging,logger,sink
 Author: EthanC
 Author-email: 16727756+EthanC@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -65,26 +65,25 @@
         embed=True
     ),
     level="WARNING",
 )
 
 try:
     value: float = 1 / 0
-except Exception as ex:
-    logger.error("Lorem ipsum dolor sit amet.", e=ex)
+except Exception as e:
+    logger.opt(exception=e).error("Lorem ipsum dolor sit amet.")
 ```
 
 ## Customization
 
 Upon constructing your handler, the following optional customizations are available via keyword arguments.
 
 -   **Username**: Username to use for the Discord Webhook message.
 -   **Avatar**: Image URL to use for the Discord Webhook message.
 -   **Embed**: Toggle whether to use plain codeblock formatting or rich embeds.
--   **Trace**: Toggle whether or not to include tracebacks (where available).
 
 ## Releases
 
 Loguru-Discord follows [Semantic Versioning](https://semver.org/) for tagging releases of the project.
 
 Changelogs can be found on the [Releases](https://github.com/EthanC/Loguru-Discord/releases) page in the [Keep a Changelog](https://keepachangelog.com/) format.
```

