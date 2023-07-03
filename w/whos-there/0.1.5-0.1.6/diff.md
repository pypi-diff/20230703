# Comparing `tmp/whos_there-0.1.5.tar.gz` & `tmp/whos_there-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whos_there-0.1.5.tar", max compression
+gzip compressed data, was "whos_there-0.1.6.tar", max compression
```

## Comparing `whos_there-0.1.5.tar` & `whos_there-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1061 2023-01-19 18:11:12.426103 whos_there-0.1.5/LICENSE
--rw-r--r--   0        0        0     5773 2023-01-19 18:11:12.426103 whos_there-0.1.5/README.md
--rw-r--r--   0        0        0     2384 2023-01-19 18:13:43.282770 whos_there-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       89 2023-01-19 18:11:12.426103 whos_there-0.1.5/whos_there/__init__.py
--rw-r--r--   0        0        0     4359 2023-01-19 18:11:12.426103 whos_there-0.1.5/whos_there/callback.py
--rw-r--r--   0        0        0      304 2023-01-19 18:11:12.426103 whos_there-0.1.5/whos_there/senders/__init__.py
--rw-r--r--   0        0        0      833 2023-01-19 18:11:12.426103 whos_there-0.1.5/whos_there/senders/base.py
--rw-r--r--   0        0        0      644 2023-01-19 18:11:12.426103 whos_there-0.1.5/whos_there/senders/debug.py
--rw-r--r--   0        0        0      417 2023-01-19 18:11:12.426103 whos_there-0.1.5/whos_there/senders/discord.py
--rw-r--r--   0        0        0     1492 2023-01-19 18:11:12.426103 whos_there-0.1.5/whos_there/senders/email.py
--rw-r--r--   0        0        0      889 2023-01-19 18:11:12.426103 whos_there-0.1.5/whos_there/senders/slack.py
--rw-r--r--   0        0        0      733 2023-01-19 18:11:12.426103 whos_there-0.1.5/whos_there/senders/teams.py
--rw-r--r--   0        0        0      797 2023-01-19 18:11:12.426103 whos_there-0.1.5/whos_there/senders/telegram.py
--rw-r--r--   0        0        0      720 2023-01-19 18:11:12.426103 whos_there-0.1.5/whos_there/utils/logging.py
--rw-r--r--   0        0        0     6824 1970-01-01 00:00:00.000000 whos_there-0.1.5/setup.py
--rw-r--r--   0        0        0     6902 1970-01-01 00:00:00.000000 whos_there-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-03 18:12:38.275381 whos_there-0.1.6/LICENSE
+-rw-r--r--   0        0        0     5924 2023-07-03 18:12:38.275381 whos_there-0.1.6/README.md
+-rw-r--r--   0        0        0     4959 2023-07-03 18:14:34.521284 whos_there-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-07-03 18:12:38.275381 whos_there-0.1.6/src/whos_there/__init__.py
+-rw-r--r--   0        0        0     4173 2023-07-03 18:12:38.275381 whos_there-0.1.6/src/whos_there/callback.py
+-rw-r--r--   0        0        0      310 2023-07-03 18:12:38.275381 whos_there-0.1.6/src/whos_there/senders/__init__.py
+-rw-r--r--   0        0        0      883 2023-07-03 18:12:38.275381 whos_there-0.1.6/src/whos_there/senders/base.py
+-rw-r--r--   0        0        0      667 2023-07-03 18:12:38.275381 whos_there-0.1.6/src/whos_there/senders/debug.py
+-rw-r--r--   0        0        0      432 2023-07-03 18:12:38.275381 whos_there-0.1.6/src/whos_there/senders/discord.py
+-rw-r--r--   0        0        0     1588 2023-07-03 18:12:38.275381 whos_there-0.1.6/src/whos_there/senders/email.py
+-rw-r--r--   0        0        0      991 2023-07-03 18:12:38.275381 whos_there-0.1.6/src/whos_there/senders/slack.py
+-rw-r--r--   0        0        0      831 2023-07-03 18:12:38.275381 whos_there-0.1.6/src/whos_there/senders/teams.py
+-rw-r--r--   0        0        0      826 2023-07-03 18:12:38.275381 whos_there-0.1.6/src/whos_there/senders/telegram.py
+-rw-r--r--   0        0        0      736 2023-07-03 18:12:38.275381 whos_there-0.1.6/src/whos_there/utils/logging.py
+-rw-r--r--   0        0        0     6934 1970-01-01 00:00:00.000000 whos_there-0.1.6/PKG-INFO
```

### Comparing `whos_there-0.1.5/README.md` & `whos_there-0.1.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-# Who's there?
-
-<div align="center">
-
-<!--- BADGES: START --->
-[![PyPI - Package Version](https://img.shields.io/pypi/v/whos-there?logo=pypi&style=flat&color=orange)][#pypi-package]
-[![Conda - Platform](https://img.shields.io/conda/pn/conda-forge/whos-there?logo=anaconda&style=flat)][#conda-forge-package]
-[![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/whos-there?logo=anaconda&style=flat&color=orange)][#conda-forge-package]
-
-[![Build](https://github.com/twsl/whos-there/actions/workflows/build.yml/badge.svg)][#github-workflows-build]
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/whos-there?logo=pypi&style=flat&color=blue)][#pypi-package]
-[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/twsl/whos-there/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
-
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
-[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][#github-pre-commit]
-[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)][#github-releases]
-[![GitHub - License](https://img.shields.io/github/license/twsl/whos-there?logo=github&style=flat&color=green)][#github-license]
-
-[#github-license]: https://github.com/twsl/whos-there/blob/main/LICENSE
-[#pypi-package]: https://pypi.org/project/whos-there/
-[#conda-forge-package]: https://anaconda.org/conda-forge/whos-there
-[#github-pre-commit]: https://github.com/twsl/whos-there/blob/master/.pre-commit-config.yaml
-[#github-releases]: https://github.com/twsl/whos-there/releases
-[#github-workflows-build]: https://github.com/twsl/whos-there/actions/workflows/build.yml
-<!--- BADGES: END --->
-    
-The spiritual successor to [knockknock](https://github.com/huggingface/knockknock) for [PyTorch Lightning](https://github.com/PyTorchLightning/pytorch-lightning), to get a notification when your training is complete or when it crashes during the process with a single callback.
-
-</div>
-
-## 🚀 Features
-
-- Supports E-Mail, Discord, Slack, Teams, Telegram
-
-## 🎯 Installation
-
-You can install `whos-there` with `pip` or `poetry` or `conda`.
-
-**with pip**
-
-```bash
-pip install -U whos-there
-```
-
-**with poetry**
-
-```bash
-poetry add whos-there
-```
-
-**with conda**
-
-```sh
-conda install -c conda-forge whos-there
-```
-
-## 🤯 How to use it
-
-```python
-from whos_there.callback import NotificationCallback
-from whos_there.senders.debug import DebugSender
-
-trainer = pl.Trainer(
-    callbacks=[
-        NotificationCallback(senders=[
-            # Add your senders here
-            DebugSender(),
-        ])
-    ]
-)
-```
-
-### E-Mail
-Requires your e-mail provider specific SMTP settings.
-
-```python
-from whos_there.senders.email import EmailSender
-# ...
-EmailSender(
-    host="smtp.example.de",
-    port=587,
-    sender_email="from@example.com",
-    password="*********",
-    recipient_emails=[
-        "to1@example.com",
-        "to2@example.com",
-    ]
-)
-```
-
-### Discord
-Requires your Discord channel's [webhook URL](https://support.discordapp.com/hc/en-us/articles/228383668-Intro-to-Webhooks).
-
-```python
-from whos_there.senders.discord import DiscordSender
-# ...
-DiscordSender(
-    webhook_url="https://discord.com/api/webhooks/XXXXXXXXXXXXXX/XXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
-)
-```
-
-### Slack
-Requires your Slack room [webhook URL](https://api.slack.com/incoming-webhooks#create_a_webhook) and optionally your [user id](https://api.slack.com/methods/users.identity) (if you want to tag yourself or someone else).
-
-```python
-from whos_there.senders.slack import SlackSender
-# ...
-SlackSender(
-    webhook_url="https://hooks.slack.com/services/T00000000/B00000000/XXXXXXXXXXXXXXXXXXXXXXXX",
-    channel="channel_name",
-    user_mentions=[
-        "XXXXXXXX"
-    ]
-)
-```
-
-### Teams
-Requires your Team Channel [webhook URL](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/connectors/connectors-using).
-
-```python
-from whos_there.senders.teams import TeamsSender
-# ...
-TeamsSender(
-    webhook_url="https://XXXXX.webhook.office.com/",
-    user_mentions=[
-        "twsl"
-    ]
-)
-```
-
-### Telegram
-You can also use Telegram Messenger to get notifications. You'll first have to create your own notification bot by following the three steps provided by Telegram [here](https://core.telegram.org/bots#6-botfather) and save your API access `TOKEN`.
-Telegram bots are shy and can't send the first message so you'll have to do the first step. By sending the first message, you'll be able to get the `chat_id` required (identification of your messaging room) by visiting `https://api.telegram.org/bot<YourBOTToken>/getUpdates` and get the `int` under the key `message['chat']['id']`.
-
-```python
-from whos_there.senders.telegram import TelegramSender
-# ...
-TelegramSender(
-    chat_id=1234567890,
-    token="XXXXXXX:XXXXXXXXXXXXXXXXXXXXXXXXXXX"
-)
-```
-
-## 🛡 License
-
-[![License](https://img.shields.io/github/license/twsl/whos-there)](https://github.com/twsl/whos-there/blob/master/LICENSE)
-
-This project is licensed under the terms of the MIT license. See [LICENSE](https://github.com/twsl/whos-there/blob/master/LICENSE) for more details.
-
-## 🏅 Credits
-
-This project was generated with [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)
-
-Big thanks to [knockknock](https://github.com/huggingface/knockknock) for the idea and code snippets.
+# Who's there?
+
+<div align="center">
+
+<!--- BADGES: START --->
+[![PyPI - Package Version](https://img.shields.io/pypi/v/whos-there?logo=pypi&style=flat&color=orange)][#pypi-package]
+[![Conda - Platform](https://img.shields.io/conda/pn/conda-forge/whos-there?logo=anaconda&style=flat)][#conda-forge-package]
+[![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/whos-there?logo=anaconda&style=flat&color=orange)][#conda-forge-package]
+
+[![Build](https://github.com/twsl/whos-there/actions/workflows/build.yml/badge.svg)][#github-workflows-build]
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/whos-there?logo=pypi&style=flat&color=blue)][#pypi-package]
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/twsl/whos-there/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][#github-pre-commit]
+[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)][#github-releases]
+[![GitHub - License](https://img.shields.io/github/license/twsl/whos-there?logo=github&style=flat&color=green)][#github-license]
+
+[#github-license]: https://github.com/twsl/whos-there/blob/main/LICENSE
+[#pypi-package]: https://pypi.org/project/whos-there/
+[#conda-forge-package]: https://anaconda.org/conda-forge/whos-there
+[#github-pre-commit]: https://github.com/twsl/whos-there/blob/master/.pre-commit-config.yaml
+[#github-releases]: https://github.com/twsl/whos-there/releases
+[#github-workflows-build]: https://github.com/twsl/whos-there/actions/workflows/build.yml
+<!--- BADGES: END --->
+
+The spiritual successor to [knockknock](https://github.com/huggingface/knockknock) for [PyTorch Lightning](https://github.com/PyTorchLightning/pytorch-lightning), to get a notification when your training is complete or when it crashes during the process with a single callback.
+
+</div>
+
+## 🚀 Features
+
+- Supports E-Mail, Discord, Slack, Teams, Telegram
+
+## 🎯 Installation
+
+You can install `whos-there` with `pip` or `poetry` or `conda`.
+
+**with pip**
+
+```bash
+pip install -U whos-there
+```
+
+**with poetry**
+
+```bash
+poetry add whos-there
+```
+
+**with conda**
+
+```sh
+conda install -c conda-forge whos-there
+```
+
+## 🤯 How to use it
+
+```python
+from whos_there.callback import NotificationCallback
+from whos_there.senders.debug import DebugSender
+
+trainer = pl.Trainer(
+    callbacks=[
+        NotificationCallback(senders=[
+            # Add your senders here
+            DebugSender(),
+        ])
+    ]
+)
+```
+
+### E-Mail
+Requires your e-mail provider specific SMTP settings.
+
+```python
+from whos_there.senders.email import EmailSender
+# ...
+EmailSender(
+    host="smtp.example.de",
+    port=587,
+    sender_email="from@example.com",
+    password="*********",
+    recipient_emails=[
+        "to1@example.com",
+        "to2@example.com",
+    ]
+)
+```
+
+### Discord
+Requires your Discord channel's [webhook URL](https://support.discordapp.com/hc/en-us/articles/228383668-Intro-to-Webhooks).
+
+```python
+from whos_there.senders.discord import DiscordSender
+# ...
+DiscordSender(
+    webhook_url="https://discord.com/api/webhooks/XXXXXXXXXXXXXX/XXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
+)
+```
+
+### Slack
+Requires your Slack room [webhook URL](https://api.slack.com/incoming-webhooks#create_a_webhook) and optionally your [user id](https://api.slack.com/methods/users.identity) (if you want to tag yourself or someone else).
+
+```python
+from whos_there.senders.slack import SlackSender
+# ...
+SlackSender(
+    webhook_url="https://hooks.slack.com/services/T00000000/B00000000/XXXXXXXXXXXXXXXXXXXXXXXX",
+    channel="channel_name",
+    user_mentions=[
+        "XXXXXXXX"
+    ]
+)
+```
+
+### Teams
+Requires your Team Channel [webhook URL](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/connectors/connectors-using).
+
+```python
+from whos_there.senders.teams import TeamsSender
+# ...
+TeamsSender(
+    webhook_url="https://XXXXX.webhook.office.com/",
+    user_mentions=[
+        "twsl"
+    ]
+)
+```
+
+### Telegram
+You can also use Telegram Messenger to get notifications. You'll first have to create your own notification bot by following the three steps provided by Telegram [here](https://core.telegram.org/bots#6-botfather) and save your API access `TOKEN`.
+Telegram bots are shy and can't send the first message so you'll have to do the first step. By sending the first message, you'll be able to get the `chat_id` required (identification of your messaging room) by visiting `https://api.telegram.org/bot<YourBOTToken>/getUpdates` and get the `int` under the key `message['chat']['id']`.
+
+```python
+from whos_there.senders.telegram import TelegramSender
+# ...
+TelegramSender(
+    chat_id=1234567890,
+    token="XXXXXXX:XXXXXXXXXXXXXXXXXXXXXXXXXXX"
+)
+```
+
+## 🛡 License
+
+[![License](https://img.shields.io/github/license/twsl/whos-there)](https://github.com/twsl/whos-there/blob/master/LICENSE)
+
+This project is licensed under the terms of the MIT license. See [LICENSE](https://github.com/twsl/whos-there/blob/master/LICENSE) for more details.
+
+## 🏅 Credits
+
+This project was generated with [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)
+
+Big thanks to [knockknock](https://github.com/huggingface/knockknock) for the idea and code snippets.
```

### Comparing `whos_there-0.1.5/whos_there/callback.py` & `whos_there-0.1.6/src/whos_there/callback.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,101 @@
-import socket
-import textwrap
-from typing import Any, Dict, List, Optional
-
-from pytorch_lightning import Callback, LightningModule, Trainer
-from pytorch_lightning.trainer.states import TrainerFn
-
-from whos_there.senders.base import Sender
-from whos_there.senders.debug import DebugSender
-from whos_there.utils.logging import get_logger
-
-logger = get_logger(__name__)
-
-
-class NotificationCallback(Callback):
-    def __init__(self, senders: List[Sender] = [DebugSender()]) -> None:
-        """Initialize the notification callback.
-
-        Args:
-            senders: List of instances of senders.
-        """
-        super().__init__()
-        self.senders = senders
-        self._current_stage: str = None
-
-    def _send(self, text: str) -> None:
-        for sender in self.senders:
-            try:
-                sender.send(text)
-            except Exception as e:
-                logger.exception(f"An exception using {sender} occurred: {e}")
-
-    def setup(self, trainer: Trainer, pl_module: LightningModule, stage: Optional[str] = None) -> None:
-        """Called when fit, validate, test, predict, or tune begins.
-        Args:
-            trainer: The current :class:`~pytorch_lightning.trainer.Trainer` instance.
-            pl_module: The current :class:`~pytorch_lightning.core.lightning.LightningModule` instance.
-            stage: The stage the trainer is currently in.
-        """
-        if trainer.global_rank == 0:
-            self._current_stage = stage
-
-    def teardown(self, trainer: Trainer, pl_module: LightningModule, stage: Optional[str] = None) -> None:
-        """Called when fit, validate, test, predict, or tune ends.
-        Args:
-            trainer: The current :class:`~pytorch_lightning.trainer.Trainer` instance.
-            pl_module: The current :class:`~pytorch_lightning.core.lightning.LightningModule` instance.
-            stage: The stage the trainer is currently in.
-        """
-        if trainer.global_rank == 0:
-            if stage == TrainerFn.FITTING:
-                contents = f"🎉 Your training of {pl_module._get_name()} on {socket.gethostname()} is complete."
-                self._send(contents)
-            if stage == TrainerFn.TESTING:
-                contents = f"🧪 Your testing of {pl_module._get_name()} on {socket.gethostname()} is complete."
-                self._send(contents)
-
-    def on_exception(self, trainer: Trainer, pl_module: LightningModule, exception: BaseException) -> None:
-        """Called when any trainer execution is interrupted by an exception.
-        Args:
-            trainer: The current :class:`~pytorch_lightning.trainer.Trainer` instance.
-            pl_module: The current :class:`~pytorch_lightning.core.lightning.LightningModule` instance.
-            exception: The exception raised.
-        """
-        contents = f"""💥 {exception} during {self._current_stage} of {pl_module._get_name()}.
-        Stage failed on {socket.gethostname()} (global rank {trainer.global_rank}).
-        """
-        self._send(textwrap.dedent(contents))
-
-    def state_dict(self) -> dict:
-        """Called when saving a model checkpoint, use to persist state.
-        Args:
-            trainer: the current :class:`~pytorch_lightning.trainer.Trainer` instance.
-            pl_module: the current :class:`~pytorch_lightning.core.lightning.LightningModule` instance.
-            checkpoint: the checkpoint dictionary that will be saved.
-        Returns:
-            The callback state.
-        """
-        return {"current_stage": self._current_stage}
-
-    def on_load_checkpoint(self, trainer: Trainer, pl_module: LightningModule, checkpoint: Dict[str, Any]) -> None:
-        """Called when loading a model checkpoint, use to reload state.
-        Args:
-            trainer: the current :class:`~pytorch_lightning.trainer.Trainer` instance.
-            pl_module: the current :class:`~pytorch_lightning.core.lightning.LightningModule` instance.
-            checkpoint: the callback state returned by ``on_save_checkpoint``.
-        Note:
-            The ``on_load_checkpoint`` won't be called with an undefined state.
-            If your ``on_load_checkpoint`` hook behavior doesn't rely on a state,
-            you will still need to override ``on_save_checkpoint`` to return a ``dummy state``.
-        """
-        self._current_stage = checkpoint.get("current_stage", None)
+from __future__ import annotations  # remove when dropping 3.8 support
+
+import socket
+import textwrap
+from typing import Any
+
+import pytorch_lightning as pl
+from pytorch_lightning.trainer.states import TrainerFn
+
+from whos_there.senders.base import Sender
+from whos_there.senders.debug import DebugSender
+from whos_there.utils.logging import get_logger
+
+logger = get_logger(__name__)
+
+
+class NotificationCallback(pl.Callback):
+    """Notification callback."""
+
+    def __init__(self, senders: list[Sender] = None) -> None:
+        """Initialize the notification callback.
+
+        Args:
+            senders: List of instances of senders.
+        """
+        super().__init__()
+        self.senders: list[Sender] = senders if senders else [DebugSender()]
+        self._current_stage: str = None
+
+    def _send(self, text: str) -> None:
+        for sender in self.senders:
+            try:
+                sender.send(text)
+            except Exception:
+                logger.exception(f"An exception using {sender} occurred.")
+
+    def setup(self, trainer: pl.Trainer, pl_module: pl.LightningModule, stage: str) -> None:
+        """Called when fit, validate, test, predict, or tune begins.
+
+        Args:
+            trainer: The current :class:`~pytorch_lightning.trainer.Trainer` instance.
+            pl_module: The current :class:`~pytorch_lightning.core.lightning.LightningModule` instance.
+            stage: The stage the trainer is currently in.
+        """
+        if trainer.global_rank == 0:
+            self._current_stage = stage
+
+    def teardown(self, trainer: pl.Trainer, pl_module: pl.LightningModule, stage: str) -> None:
+        """Called when fit, validate, test, predict, or tune ends.
+
+        Args:
+            trainer: The current :class:`~pytorch_lightning.trainer.Trainer` instance.
+            pl_module: The current :class:`~pytorch_lightning.core.lightning.LightningModule` instance.
+            stage: The stage the trainer is currently in.
+        """
+        if trainer.global_rank == 0:
+            icon = None
+            if stage == "tune":
+                icon = "🧪"
+            if stage == TrainerFn.FITTING:
+                icon = "✨"
+            if stage == TrainerFn.TESTING:
+                icon = "🎉"
+            if icon is not None:
+                name = pl_module._get_name()
+                contents = f"{icon} {stage.capitalize()} stage of {name} on {socket.gethostname()} is complete."
+                self._send(contents)
+
+    def on_exception(self, trainer: pl.Trainer, pl_module: pl.LightningModule, exception: BaseException) -> None:
+        """Called when any trainer execution is interrupted by an exception.
+
+        Args:
+            trainer: The current :class:`~pytorch_lightning.trainer.Trainer` instance.
+            pl_module: The current :class:`~pytorch_lightning.core.lightning.LightningModule` instance.
+            exception: The exception raised.
+        """
+        name = pl_module._get_name()
+        contents = f"""💥 Failed during {self._current_stage.capitalize()} stage of {name} on {socket.gethostname()}.
+        Exception (global rank {trainer.global_rank}): '{exception}'
+        """
+        self._send(textwrap.dedent(contents))
+
+    def state_dict(self) -> dict[str, Any]:
+        """Called when saving a checkpoint, implement to generate callback's ``state_dict``.
+
+        Returns:
+            A dictionary containing callback state.
+        """
+        return {"current_stage": self._current_stage}
+
+    def on_load_checkpoint(
+        self, trainer: pl.Trainer, pl_module: pl.LightningModule, checkpoint: dict[str, Any]
+    ) -> None:
+        r"""Called when loading a model checkpoint, use to reload state.
+
+        Args:
+            trainer: the current :class:`~pytorch_lightning.trainer.Trainer` instance.
+            pl_module: the current :class:`~pytorch_lightning.core.module.LightningModule` instance.
+            checkpoint: the full checkpoint dictionary that got loaded by the Trainer.
+        """
+        self._current_stage = checkpoint.get("current_stage", None)
```

### Comparing `whos_there-0.1.5/whos_there/senders/base.py` & `whos_there-0.1.6/src/whos_there/senders/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import abc
-import json
-from typing import Any
-
-import requests
-
-
-class Sender(abc.ABC):
-    def __init__(self) -> None:
-        super().__init__()
-
-    @abc.abstractmethod
-    def send(self, text: str) -> Any:
-        """Actually send the text to the desired output method.
-
-        Args:
-            text: Message to send.
-
-        Returns:
-            Optional return value.
-        """
-        pass
-
-    def _send_json(self, url: str, data: Any) -> requests.Response:
-        """Send JSON data to URL.
-
-        Args:
-            url: URL to send the data payload to.
-            data: Payload data.
-
-        Returns:
-            Response of the HTTP request.
-        """
-        headers = {"Content-Type": "application/json"}
-        payload = json.dumps(data)
-        return requests.post(url=url, data=payload, headers=headers)
+import abc
+import json
+from typing import Any
+
+import requests
+
+
+class Sender(abc.ABC):
+    def __init__(self) -> None:
+        super().__init__()
+
+    @abc.abstractmethod
+    def send(self, text: str) -> Any:
+        """Actually send the text to the desired output method.
+
+        Args:
+            text: Message to send.
+
+        Returns:
+            Optional return value.
+        """
+        pass
+
+    def _send_json(self, url: str, data: Any) -> requests.Response:
+        """Send JSON data to URL.
+
+        Args:
+            url: URL to send the data payload to.
+            data: Payload data.
+
+        Returns:
+            Response of the HTTP request.
+        """
+        headers = {"Content-Type": "application/json"}
+        payload = json.dumps(data)
+        return requests.post(url=url, data=payload, headers=headers, timeout=5000)
```

### Comparing `whos_there-0.1.5/whos_there/senders/email.py` & `whos_there-0.1.6/src/whos_there/senders/email.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-import smtplib
-from email.message import EmailMessage
-from typing import List
-
-from whos_there.senders.base import Sender
-
-
-class EmailSender(Sender):
-    def __init__(self, host: str, port: int, sender_email: str, password: str, recipient_emails: List[str]) -> None:
-        """Initialize the Email sender.
-
-        Args:
-            host: The SMTP host.
-            port: The SMTP port.
-            sender_email: The senders email adress.
-            password: The email password.
-            recipient_emails: The recipients emails.
-        """
-        super().__init__()
-        self.host = host
-        self.port = port
-        self.sender_email = sender_email
-        self.password = password
-        self.recipient_emails = recipient_emails
-        self._server: smtplib.SMTP = None
-
-    @property
-    def server(self) -> smtplib.SMTP:
-        """SMTP server instance.
-
-        Returns:
-            The SMTP instance.
-        """
-        if not self._server:
-            self._server = smtplib.SMTP(self.host, self.port)
-            self._server.starttls()
-            self._server.login(self.sender_email, self.password)
-        return self._server
-
-    def send(self, text: str) -> None:
-        msg = EmailMessage()
-        msg.set_content(text)
-        msg["Subject"] = "Knock Knock"
-        msg["From"] = self.sender_email
-        msg["To"] = self.recipient_emails
-        self.server.sendmail(self.sender_email, self.recipient_emails, msg.as_string())
-        self.server.quit()
+from __future__ import annotations  # remove when dropping 3.8 support
+
+from email.message import EmailMessage
+import smtplib
+
+from whos_there.senders.base import Sender
+
+
+class EmailSender(Sender):
+    def __init__(self, host: str, port: int, sender_email: str, password: str, recipient_emails: list[str]) -> None:
+        """Initialize the Email sender.
+
+        Args:
+            host: The SMTP host.
+            port: The SMTP port.
+            sender_email: The senders email adress.
+            password: The email password.
+            recipient_emails: The recipients emails.
+        """
+        super().__init__()
+        self.host = host
+        self.port = port
+        self.sender_email = sender_email
+        self.password = password
+        self.recipient_emails = recipient_emails
+        self._server: smtplib.SMTP = None
+
+    @property
+    def server(self) -> smtplib.SMTP:
+        """SMTP server instance.
+
+        Returns:
+            The SMTP instance.
+        """
+        if not self._server:
+            self._server = smtplib.SMTP(self.host, self.port)
+            self._server.starttls()
+            self._server.login(self.sender_email, self.password)
+        return self._server
+
+    def send(self, text: str) -> None:
+        msg = EmailMessage()
+        msg.set_content(text)
+        msg["Subject"] = "Knock Knock"
+        msg["From"] = self.sender_email
+        msg["To"] = self.recipient_emails
+        self.server.sendmail(self.sender_email, self.recipient_emails, msg.as_string())
+        self.server.quit()
```

### Comparing `whos_there-0.1.5/whos_there/senders/slack.py` & `whos_there-0.1.6/src/whos_there/senders/slack.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import List
-
-from whos_there.senders.base import Sender
-
-
-class SlackSender(Sender):
-    def __init__(self, webhook_url: str, channel: str, user_mentions: List[str] = []) -> None:
-        """Initialize the Slack sender.
-
-        Args:
-            webhook_url: The Slack webhook URL.
-            channel: The Slack channel name.
-            user_mentions: The list of users to mention.
-        """
-        super().__init__()
-        self.webhook_url = webhook_url
-        self.channel = channel
-        self.user_mentions = " ".join(user_mentions)
-
-    def send(self, text: str) -> None:
-        data = {
-            "username": "Knock Knock",
-            "channel": self.channel,
-            "link_names": 1,
-            "icon_emoji": ":clapper:",  # ":tada:"
-            "text": f"{text} {self.user_mentions}",
-        }
-        return self._send_json(self.webhook_url, data)
+from __future__ import annotations  # remove when dropping 3.8 support
+
+from whos_there.senders.base import Sender
+
+
+class SlackSender(Sender):
+    def __init__(self, webhook_url: str, channel: str, user_mentions: list[str] = None) -> None:
+        """Initialize the Slack sender.
+
+        Args:
+            webhook_url: The Slack webhook URL.
+            channel: The Slack channel name.
+            user_mentions: The list of users to mention.
+        """
+        super().__init__()
+        self.webhook_url = webhook_url
+        self.channel = channel
+        self.user_mentions = " ".join(user_mentions) if user_mentions else []
+
+    def send(self, text: str) -> None:
+        data = {
+            "username": "Knock Knock",
+            "channel": self.channel,
+            "link_names": 1,
+            "icon_emoji": ":clapper:",  # ":tada:"
+            "text": f"{text} {self.user_mentions}",
+        }
+        return self._send_json(self.webhook_url, data)
```

### Comparing `whos_there-0.1.5/whos_there/senders/teams.py` & `whos_there-0.1.6/src/whos_there/senders/teams.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import List
-
-from whos_there.senders.base import Sender
-
-
-class TeamsSender(Sender):
-    def __init__(self, webhook_url: str, user_mentions: List[str] = []) -> None:
-        """Initialize the Teams sender.
-
-        Args:
-            webhook_url: The Teams webhook URL.
-            user_mentions: The list of users to mention.
-        """
-        super().__init__()
-        self.webhook_url = webhook_url
-        self.user_mentions = " ".join(user_mentions)
-
-    def send(self, text: str) -> None:
-        data = {
-            "username": "Knock Knock",
-            "icon_emoji": ":clapper:",  # ":tada:"
-            "text": f"{text} {self.user_mentions}",
-        }
-        return self._send_json(self.webhook_url, data)
+from __future__ import annotations  # remove when dropping 3.8 support
+
+from whos_there.senders.base import Sender
+
+
+class TeamsSender(Sender):
+    def __init__(self, webhook_url: str, user_mentions: list[str] = None) -> None:
+        """Initialize the Teams sender.
+
+        Args:
+            webhook_url: The Teams webhook URL.
+            user_mentions: The list of users to mention.
+        """
+        super().__init__()
+        self.webhook_url = webhook_url
+        self.user_mentions = " ".join(user_mentions) if user_mentions else []
+
+    def send(self, text: str) -> None:
+        data = {
+            "username": "Knock Knock",
+            "icon_emoji": ":clapper:",  # ":tada:"
+            "text": f"{text} {self.user_mentions}",
+        }
+        return self._send_json(self.webhook_url, data)
```

### Comparing `whos_there-0.1.5/setup.py` & `whos_there-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,183 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: whos-there
+Version: 0.1.6
+Summary: The spiritual successor to knockknock for PyTorch Lightning, get notified when your training ends
+Home-page: https://github.com/twsl/whos-there
+License: MIT
+Keywords: python,pytorch,pytorch-lightning,machine-learning,deep-learning
+Author: twsl
+Author-email: 45483159+twsl@users.noreply.github.com
+Maintainer: twsl
+Maintainer-email: 45483159+twsl@users.noreply.github.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Requires-Dist: python-telegram-bot (>=20.0,<21.0)
+Requires-Dist: pytorch-lightning (>=2.0,<3.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: torch (>=1.11.0,!=2.0.1)
+Project-URL: Documentation, https://github.com/twsl/whos-there
+Project-URL: Repository, https://github.com/twsl/whos-there
+Project-URL: issues, https://github.com/twsl/whos-there/issues
+Description-Content-Type: text/markdown
+
+# Who's there?
+
+<div align="center">
+
+<!--- BADGES: START --->
+[![PyPI - Package Version](https://img.shields.io/pypi/v/whos-there?logo=pypi&style=flat&color=orange)][#pypi-package]
+[![Conda - Platform](https://img.shields.io/conda/pn/conda-forge/whos-there?logo=anaconda&style=flat)][#conda-forge-package]
+[![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/whos-there?logo=anaconda&style=flat&color=orange)][#conda-forge-package]
+
+[![Build](https://github.com/twsl/whos-there/actions/workflows/build.yml/badge.svg)][#github-workflows-build]
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/whos-there?logo=pypi&style=flat&color=blue)][#pypi-package]
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/twsl/whos-there/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][#github-pre-commit]
+[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)][#github-releases]
+[![GitHub - License](https://img.shields.io/github/license/twsl/whos-there?logo=github&style=flat&color=green)][#github-license]
+
+[#github-license]: https://github.com/twsl/whos-there/blob/main/LICENSE
+[#pypi-package]: https://pypi.org/project/whos-there/
+[#conda-forge-package]: https://anaconda.org/conda-forge/whos-there
+[#github-pre-commit]: https://github.com/twsl/whos-there/blob/master/.pre-commit-config.yaml
+[#github-releases]: https://github.com/twsl/whos-there/releases
+[#github-workflows-build]: https://github.com/twsl/whos-there/actions/workflows/build.yml
+<!--- BADGES: END --->
+
+The spiritual successor to [knockknock](https://github.com/huggingface/knockknock) for [PyTorch Lightning](https://github.com/PyTorchLightning/pytorch-lightning), to get a notification when your training is complete or when it crashes during the process with a single callback.
+
+</div>
+
+## 🚀 Features
+
+- Supports E-Mail, Discord, Slack, Teams, Telegram
+
+## 🎯 Installation
+
+You can install `whos-there` with `pip` or `poetry` or `conda`.
+
+**with pip**
+
+```bash
+pip install -U whos-there
+```
+
+**with poetry**
+
+```bash
+poetry add whos-there
+```
+
+**with conda**
+
+```sh
+conda install -c conda-forge whos-there
+```
+
+## 🤯 How to use it
+
+```python
+from whos_there.callback import NotificationCallback
+from whos_there.senders.debug import DebugSender
+
+trainer = pl.Trainer(
+    callbacks=[
+        NotificationCallback(senders=[
+            # Add your senders here
+            DebugSender(),
+        ])
+    ]
+)
+```
+
+### E-Mail
+Requires your e-mail provider specific SMTP settings.
+
+```python
+from whos_there.senders.email import EmailSender
+# ...
+EmailSender(
+    host="smtp.example.de",
+    port=587,
+    sender_email="from@example.com",
+    password="*********",
+    recipient_emails=[
+        "to1@example.com",
+        "to2@example.com",
+    ]
+)
+```
+
+### Discord
+Requires your Discord channel's [webhook URL](https://support.discordapp.com/hc/en-us/articles/228383668-Intro-to-Webhooks).
+
+```python
+from whos_there.senders.discord import DiscordSender
+# ...
+DiscordSender(
+    webhook_url="https://discord.com/api/webhooks/XXXXXXXXXXXXXX/XXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
+)
+```
+
+### Slack
+Requires your Slack room [webhook URL](https://api.slack.com/incoming-webhooks#create_a_webhook) and optionally your [user id](https://api.slack.com/methods/users.identity) (if you want to tag yourself or someone else).
+
+```python
+from whos_there.senders.slack import SlackSender
+# ...
+SlackSender(
+    webhook_url="https://hooks.slack.com/services/T00000000/B00000000/XXXXXXXXXXXXXXXXXXXXXXXX",
+    channel="channel_name",
+    user_mentions=[
+        "XXXXXXXX"
+    ]
+)
+```
+
+### Teams
+Requires your Team Channel [webhook URL](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/connectors/connectors-using).
+
+```python
+from whos_there.senders.teams import TeamsSender
+# ...
+TeamsSender(
+    webhook_url="https://XXXXX.webhook.office.com/",
+    user_mentions=[
+        "twsl"
+    ]
+)
+```
+
+### Telegram
+You can also use Telegram Messenger to get notifications. You'll first have to create your own notification bot by following the three steps provided by Telegram [here](https://core.telegram.org/bots#6-botfather) and save your API access `TOKEN`.
+Telegram bots are shy and can't send the first message so you'll have to do the first step. By sending the first message, you'll be able to get the `chat_id` required (identification of your messaging room) by visiting `https://api.telegram.org/bot<YourBOTToken>/getUpdates` and get the `int` under the key `message['chat']['id']`.
+
+```python
+from whos_there.senders.telegram import TelegramSender
+# ...
+TelegramSender(
+    chat_id=1234567890,
+    token="XXXXXXX:XXXXXXXXXXXXXXXXXXXXXXXXXXX"
+)
+```
+
+## 🛡 License
+
+[![License](https://img.shields.io/github/license/twsl/whos-there)](https://github.com/twsl/whos-there/blob/master/LICENSE)
 
-packages = \
-['whos_there', 'whos_there.senders', 'whos_there.utils']
+This project is licensed under the terms of the MIT license. See [LICENSE](https://github.com/twsl/whos-there/blob/master/LICENSE) for more details.
 
-package_data = \
-{'': ['*']}
+## 🏅 Credits
 
-install_requires = \
-['python-telegram-bot>=20.0,<21.0',
- 'pytorch-lightning>=1.8.0,<2.0.0',
- 'requests>=2.28.2,<3.0.0']
-
-setup_kwargs = {
-    'name': 'whos-there',
-    'version': '0.1.5',
-    'description': 'The spiritual successor to knockknock for PyTorch Lightning, get notified when your training ends',
-    'long_description': '# Who\'s there?\n\n<div align="center">\n\n<!--- BADGES: START --->\n[![PyPI - Package Version](https://img.shields.io/pypi/v/whos-there?logo=pypi&style=flat&color=orange)][#pypi-package]\n[![Conda - Platform](https://img.shields.io/conda/pn/conda-forge/whos-there?logo=anaconda&style=flat)][#conda-forge-package]\n[![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/whos-there?logo=anaconda&style=flat&color=orange)][#conda-forge-package]\n\n[![Build](https://github.com/twsl/whos-there/actions/workflows/build.yml/badge.svg)][#github-workflows-build]\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/whos-there?logo=pypi&style=flat&color=blue)][#pypi-package]\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/twsl/whos-there/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][#github-pre-commit]\n[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)][#github-releases]\n[![GitHub - License](https://img.shields.io/github/license/twsl/whos-there?logo=github&style=flat&color=green)][#github-license]\n\n[#github-license]: https://github.com/twsl/whos-there/blob/main/LICENSE\n[#pypi-package]: https://pypi.org/project/whos-there/\n[#conda-forge-package]: https://anaconda.org/conda-forge/whos-there\n[#github-pre-commit]: https://github.com/twsl/whos-there/blob/master/.pre-commit-config.yaml\n[#github-releases]: https://github.com/twsl/whos-there/releases\n[#github-workflows-build]: https://github.com/twsl/whos-there/actions/workflows/build.yml\n<!--- BADGES: END --->\n    \nThe spiritual successor to [knockknock](https://github.com/huggingface/knockknock) for [PyTorch Lightning](https://github.com/PyTorchLightning/pytorch-lightning), to get a notification when your training is complete or when it crashes during the process with a single callback.\n\n</div>\n\n## 🚀 Features\n\n- Supports E-Mail, Discord, Slack, Teams, Telegram\n\n## 🎯 Installation\n\nYou can install `whos-there` with `pip` or `poetry` or `conda`.\n\n**with pip**\n\n```bash\npip install -U whos-there\n```\n\n**with poetry**\n\n```bash\npoetry add whos-there\n```\n\n**with conda**\n\n```sh\nconda install -c conda-forge whos-there\n```\n\n## 🤯 How to use it\n\n```python\nfrom whos_there.callback import NotificationCallback\nfrom whos_there.senders.debug import DebugSender\n\ntrainer = pl.Trainer(\n    callbacks=[\n        NotificationCallback(senders=[\n            # Add your senders here\n            DebugSender(),\n        ])\n    ]\n)\n```\n\n### E-Mail\nRequires your e-mail provider specific SMTP settings.\n\n```python\nfrom whos_there.senders.email import EmailSender\n# ...\nEmailSender(\n    host="smtp.example.de",\n    port=587,\n    sender_email="from@example.com",\n    password="*********",\n    recipient_emails=[\n        "to1@example.com",\n        "to2@example.com",\n    ]\n)\n```\n\n### Discord\nRequires your Discord channel\'s [webhook URL](https://support.discordapp.com/hc/en-us/articles/228383668-Intro-to-Webhooks).\n\n```python\nfrom whos_there.senders.discord import DiscordSender\n# ...\nDiscordSender(\n    webhook_url="https://discord.com/api/webhooks/XXXXXXXXXXXXXX/XXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"\n)\n```\n\n### Slack\nRequires your Slack room [webhook URL](https://api.slack.com/incoming-webhooks#create_a_webhook) and optionally your [user id](https://api.slack.com/methods/users.identity) (if you want to tag yourself or someone else).\n\n```python\nfrom whos_there.senders.slack import SlackSender\n# ...\nSlackSender(\n    webhook_url="https://hooks.slack.com/services/T00000000/B00000000/XXXXXXXXXXXXXXXXXXXXXXXX",\n    channel="channel_name",\n    user_mentions=[\n        "XXXXXXXX"\n    ]\n)\n```\n\n### Teams\nRequires your Team Channel [webhook URL](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/connectors/connectors-using).\n\n```python\nfrom whos_there.senders.teams import TeamsSender\n# ...\nTeamsSender(\n    webhook_url="https://XXXXX.webhook.office.com/",\n    user_mentions=[\n        "twsl"\n    ]\n)\n```\n\n### Telegram\nYou can also use Telegram Messenger to get notifications. You\'ll first have to create your own notification bot by following the three steps provided by Telegram [here](https://core.telegram.org/bots#6-botfather) and save your API access `TOKEN`.\nTelegram bots are shy and can\'t send the first message so you\'ll have to do the first step. By sending the first message, you\'ll be able to get the `chat_id` required (identification of your messaging room) by visiting `https://api.telegram.org/bot<YourBOTToken>/getUpdates` and get the `int` under the key `message[\'chat\'][\'id\']`.\n\n```python\nfrom whos_there.senders.telegram import TelegramSender\n# ...\nTelegramSender(\n    chat_id=1234567890,\n    token="XXXXXXX:XXXXXXXXXXXXXXXXXXXXXXXXXXX"\n)\n```\n\n## 🛡 License\n\n[![License](https://img.shields.io/github/license/twsl/whos-there)](https://github.com/twsl/whos-there/blob/master/LICENSE)\n\nThis project is licensed under the terms of the MIT license. See [LICENSE](https://github.com/twsl/whos-there/blob/master/LICENSE) for more details.\n\n## 🏅 Credits\n\nThis project was generated with [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)\n\nBig thanks to [knockknock](https://github.com/huggingface/knockknock) for the idea and code snippets.\n',
-    'author': 'twsl',
-    'author_email': '45483159+twsl@users.noreply.github.com',
-    'maintainer': 'twsl',
-    'maintainer_email': '45483159+twsl@users.noreply.github.com',
-    'url': 'https://github.com/twsl/whos-there',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8.1,<4.0.0',
-}
+This project was generated with [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)
 
+Big thanks to [knockknock](https://github.com/huggingface/knockknock) for the idea and code snippets.
 
-setup(**setup_kwargs)
```

