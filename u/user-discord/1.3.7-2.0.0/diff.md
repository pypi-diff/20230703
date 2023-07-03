# Comparing `tmp/user_discord-1.3.7.tar.gz` & `tmp/user_discord-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_discord-1.3.7.tar", last modified: Sat Jul  1 21:29:17 2023, max compression
+gzip compressed data, was "user_discord-2.0.0.tar", last modified: Mon Jul  3 17:09:16 2023, max compression
```

## Comparing `user_discord-1.3.7.tar` & `user_discord-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,134 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 21:29:17.941354 user_discord-1.3.7/
--rw-rw-rw-   0        0        0      335 2023-07-01 21:29:17.942354 user_discord-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.3.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 21:29:17.944351 user_discord-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-07-01 21:29:01.000000 user_discord-1.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 21:29:17.888246 user_discord-1.3.7/user_discord/
--rw-rw-rw-   0        0        0      598 2023-07-01 21:28:54.000000 user_discord-1.3.7/user_discord/__init__.py
--rw-rw-rw-   0        0        0     2510 2023-07-01 21:28:04.000000 user_discord-1.3.7/user_discord/socket.py
--rw-rw-rw-   0        0        0     4414 2023-07-01 21:28:44.000000 user_discord-1.3.7/user_discord/user_discord.py
-drwxrwxrwx   0        0        0        0 2023-07-01 21:29:17.939354 user_discord-1.3.7/user_discord/utils/
--rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.3.7/user_discord/utils/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.3.7/user_discord/utils/objects.py
--rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.3.7/user_discord/utils/payloads.py
-drwxrwxrwx   0        0        0        0 2023-07-01 21:29:17.924363 user_discord-1.3.7/user_discord.egg-info/
--rw-rw-rw-   0        0        0      335 2023-07-01 21:29:17.000000 user_discord-1.3.7/user_discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-07-01 21:29:17.000000 user_discord-1.3.7/user_discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 21:29:17.000000 user_discord-1.3.7/user_discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-01 21:29:17.000000 user_discord-1.3.7/user_discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-01 21:29:17.000000 user_discord-1.3.7/user_discord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 17:09:16.580595 user_discord-2.0.0/
+-rw-rw-rw-   0        0        0      335 2023-07-03 17:09:16.580595 user_discord-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 17:09:16.583591 user_discord-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-07-03 17:08:32.000000 user_discord-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:09:13.681690 user_discord-2.0.0/user_discord/
+-rw-rw-rw-   0        0        0      673 2023-07-03 17:08:19.000000 user_discord-2.0.0/user_discord/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:09:15.865662 user_discord-2.0.0/user_discord/discord/
+-rw-rw-rw-   0        0        0     2436 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/__init__.py
+-rw-rw-rw-   0        0        0    10966 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/__main__.py
+-rw-rw-rw-   0        0        0    82000 2023-07-03 01:46:41.000000 user_discord-2.0.0/user_discord/discord/abc.py
+-rw-rw-rw-   0        0        0    35249 2023-07-03 01:46:41.000000 user_discord-2.0.0/user_discord/discord/activity.py
+-rw-rw-rw-   0        0        0     4272 2023-07-03 01:46:41.000000 user_discord-2.0.0/user_discord/discord/affinity.py
+-rw-rw-rw-   0        0        0   124457 2023-07-03 01:46:41.000000 user_discord-2.0.0/user_discord/discord/application.py
+-rw-rw-rw-   0        0        0    20104 2023-07-03 01:46:41.000000 user_discord-2.0.0/user_discord/discord/asset.py
+-rw-rw-rw-   0        0        0    31379 2023-07-03 01:46:41.000000 user_discord-2.0.0/user_discord/discord/audit_logs.py
+-rw-rw-rw-   0        0        0    24248 2023-07-03 01:46:41.000000 user_discord-2.0.0/user_discord/discord/automod.py
+-rw-rw-rw-   0        0        0     3859 2023-07-03 01:46:41.000000 user_discord-2.0.0/user_discord/discord/backoff.py
+-rw-rw-rw-   0        0        0    12634 2023-07-03 01:46:41.000000 user_discord-2.0.0/user_discord/discord/billing.py
+-rw-rw-rw-   0        0        0    16172 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/calls.py
+-rw-rw-rw-   0        0        0   134638 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/channel.py
+-rw-rw-rw-   0        0        0   154059 2023-07-03 16:17:19.000000 user_discord-2.0.0/user_discord/discord/client.py
+-rw-rw-rw-   0        0        0    14681 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/colour.py
+-rw-rw-rw-   0        0        0    32936 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/commands.py
+-rw-rw-rw-   0        0        0    17498 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/components.py
+-rw-rw-rw-   0        0        0    11516 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/connections.py
+-rw-rw-rw-   0        0        0     3124 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/context_managers.py
+-rw-rw-rw-   0        0        0    23041 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/embeds.py
+-rw-rw-rw-   0        0        0     9463 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/emoji.py
+-rw-rw-rw-   0        0        0    23239 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/entitlements.py
+-rw-rw-rw-   0        0        0    38120 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/enums.py
+-rw-rw-rw-   0        0        0     8247 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/errors.py
+-rw-rw-rw-   0        0        0     5816 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/file.py
+-rw-rw-rw-   0        0        0    76908 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/flags.py
+-rw-rw-rw-   0        0        0    39792 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/gateway.py
+-rw-rw-rw-   0        0        0   168357 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/guild.py
+-rw-rw-rw-   0        0        0    10816 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/guild_premium.py
+-rw-rw-rw-   0        0        0     3529 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/handlers.py
+-rw-rw-rw-   0        0        0   177638 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/http.py
+-rw-rw-rw-   0        0        0    12512 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/integrations.py
+-rw-rw-rw-   0        0        0     7790 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/interactions.py
+-rw-rw-rw-   0        0        0    26660 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/invite.py
+-rw-rw-rw-   0        0        0     9503 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/library.py
+-rw-rw-rw-   0        0        0    43467 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/member.py
+-rw-rw-rw-   0        0        0     5743 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/mentions.py
+-rw-rw-rw-   0        0        0    85298 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/message.py
+-rw-rw-rw-   0        0        0     4655 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/metadata.py
+-rw-rw-rw-   0        0        0     1531 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/mixins.py
+-rw-rw-rw-   0        0        0     4534 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/modal.py
+-rw-rw-rw-   0        0        0     3812 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/object.py
+-rw-rw-rw-   0        0        0     3763 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/oggparse.py
+-rw-rw-rw-   0        0        0    15308 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/opus.py
+-rw-rw-rw-   0        0        0     9165 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/partial_emoji.py
+-rw-rw-rw-   0        0        0    10693 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/payments.py
+-rw-rw-rw-   0        0        0    30168 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/permissions.py
+-rw-rw-rw-   0        0        0    26617 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/player.py
+-rw-rw-rw-   0        0        0    16128 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/profile.py
+-rw-rw-rw-   0        0        0    10463 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/promotions.py
+-rw-rw-rw-   0        0        0    12430 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/raw_models.py
+-rw-rw-rw-   0        0        0     8482 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/reaction.py
+-rw-rw-rw-   0        0        0    10742 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/relationship.py
+-rw-rw-rw-   0        0        0    24102 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/role.py
+-rw-rw-rw-   0        0        0    24244 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/scheduled_event.py
+-rw-rw-rw-   0        0        0    98360 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/settings.py
+-rw-rw-rw-   0        0        0     6848 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/stage_instance.py
+-rw-rw-rw-   0        0        0   120924 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/state.py
+-rw-rw-rw-   0        0        0    17642 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/sticker.py
+-rw-rw-rw-   0        0        0    93140 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/store.py
+-rw-rw-rw-   0        0        0    30116 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/subscriptions.py
+-rw-rw-rw-   0        0        0    19286 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/team.py
+-rw-rw-rw-   0        0        0     9691 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/template.py
+-rw-rw-rw-   0        0        0    34125 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/threads.py
+-rw-rw-rw-   0        0        0     7454 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/tracking.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:09:16.445571 user_discord-2.0.0/user_discord/discord/types/
+-rw-rw-rw-   0        0        0      159 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/__init__.py
+-rw-rw-rw-   0        0        0     2836 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/activity.py
+-rw-rw-rw-   0        0        0     7631 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/application.py
+-rw-rw-rw-   0        0        0     8193 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/audit_log.py
+-rw-rw-rw-   0        0        0     4141 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/automod.py
+-rw-rw-rw-   0        0        0     2493 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/billing.py
+-rw-rw-rw-   0        0        0     5126 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/channel.py
+-rw-rw-rw-   0        0        0     5805 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/command.py
+-rw-rw-rw-   0        0        0     2548 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/components.py
+-rw-rw-rw-   0        0        0     2419 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/embed.py
+-rw-rw-rw-   0        0        0     1718 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/emoji.py
+-rw-rw-rw-   0        0        0     3327 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/entitlements.py
+-rw-rw-rw-   0        0        0    12841 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/gateway.py
+-rw-rw-rw-   0        0        0     5168 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/guild.py
+-rw-rw-rw-   0        0        0     2419 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/integration.py
+-rw-rw-rw-   0        0        0     7070 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/interactions.py
+-rw-rw-rw-   0        0        0     2813 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/invite.py
+-rw-rw-rw-   0        0        0     1647 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/library.py
+-rw-rw-rw-   0        0        0     2051 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/member.py
+-rw-rw-rw-   0        0        0     4338 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/message.py
+-rw-rw-rw-   0        0        0     2285 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/payments.py
+-rw-rw-rw-   0        0        0     2668 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/profile.py
+-rw-rw-rw-   0        0        0     2526 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/promotions.py
+-rw-rw-rw-   0        0        0     1799 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/role.py
+-rw-rw-rw-   0        0        0     3412 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/scheduled_event.py
+-rw-rw-rw-   0        0        0     1210 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/snowflake.py
+-rw-rw-rw-   0        0        0     2343 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/sticker.py
+-rw-rw-rw-   0        0        0     5078 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/store.py
+-rw-rw-rw-   0        0        0     4653 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/subscriptions.py
+-rw-rw-rw-   0        0        0     2025 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/team.py
+-rw-rw-rw-   0        0        0     1658 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/template.py
+-rw-rw-rw-   0        0        0     2569 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/threads.py
+-rw-rw-rw-   0        0        0     3841 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/user.py
+-rw-rw-rw-   0        0        0     2415 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/voice.py
+-rw-rw-rw-   0        0        0     2045 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/webhook.py
+-rw-rw-rw-   0        0        0     1500 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/welcome_screen.py
+-rw-rw-rw-   0        0        0     1948 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/types/widget.py
+-rw-rw-rw-   0        0        0    35605 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/user.py
+-rw-rw-rw-   0        0        0    50402 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/utils.py
+-rw-rw-rw-   0        0        0    26084 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/voice_client.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:09:16.509938 user_discord-2.0.0/user_discord/discord/webhook/
+-rw-rw-rw-   0        0        0      195 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/webhook/__init__.py
+-rw-rw-rw-   0        0        0    61821 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/webhook/async_.py
+-rw-rw-rw-   0        0        0    43801 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/webhook/sync.py
+-rw-rw-rw-   0        0        0     7603 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/welcome_screen.py
+-rw-rw-rw-   0        0        0    10420 2023-07-03 01:46:42.000000 user_discord-2.0.0/user_discord/discord/widget.py
+-rw-rw-rw-   0        0        0     2589 2023-07-03 03:20:52.000000 user_discord-2.0.0/user_discord/socket.py
+-rw-rw-rw-   0        0        0     5845 2023-07-03 16:45:13.000000 user_discord-2.0.0/user_discord/user_discord.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:09:16.578596 user_discord-2.0.0/user_discord/utils/
+-rw-rw-rw-   0        0        0      146 2023-07-03 16:25:15.000000 user_discord-2.0.0/user_discord/utils/__init__.py
+-rw-rw-rw-   0        0        0     1484 2023-07-03 03:22:47.000000 user_discord-2.0.0/user_discord/utils/objects.py
+-rw-rw-rw-   0        0        0      818 2023-07-03 01:46:43.000000 user_discord-2.0.0/user_discord/utils/payloads.py
+-rw-rw-rw-   0        0        0      721 2023-07-03 16:24:34.000000 user_discord-2.0.0/user_discord/utils/threading.py
+-rw-rw-rw-   0        0        0     1324 2023-07-03 03:32:12.000000 user_discord-2.0.0/user_discord/utils/youtube.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:09:13.728510 user_discord-2.0.0/user_discord.egg-info/
+-rw-rw-rw-   0        0        0      335 2023-07-03 17:09:10.000000 user_discord-2.0.0/user_discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4292 2023-07-03 17:09:10.000000 user_discord-2.0.0/user_discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 17:09:10.000000 user_discord-2.0.0/user_discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-03 17:09:10.000000 user_discord-2.0.0/user_discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 17:09:10.000000 user_discord-2.0.0/user_discord.egg-info/top_level.txt
```

### Comparing `user_discord-1.3.7/README.md` & `user_discord-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.7/setup.py` & `user_discord-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 long_description ="""By: nxslayer\nInstall: pip install user_discord"""
 
 setup(
     name="user_discord",
     license="MIT",
     author="nxSlayer",
-    version="1.3.7",
+    version="2.0.0",
     author_email="princediscordslay@gmail.com",
     description="Library for discord bots.",
     url="https://github.com/nxSlayer/user-discord",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
```

### Comparing `user_discord-1.3.7/user_discord/__init__.py` & `user_discord-2.0.0/user_discord/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 nxSlayer'
 
 from .socket import SocketDiscord
 from .user_discord import ClientDiscord
 from .utils import objects
 from .utils import payloads
+from .utils import youtube
+from . import discord
+from .utils import Thread
 
 from requests import get
 from json import loads
 
 __newest__ = loads(get("https://pypi.org/pypi/user-discord/json").text)["info"]["version"]
 
-if '1.3.7' != __newest__:
+if '2.0.0' != __newest__:
     print(f"(user-discord) There is a new version, please update for better results")
```

### Comparing `user_discord-1.3.7/user_discord/socket.py` & `user_discord-2.0.0/user_discord/socket.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 class SocketDiscord:
     def __init__(self, client):
         self.events = {}
         self.ws = None
         self.token = client.token
         self.client = client
         
+        
+        self.session_id = None
+        
 
     def on(self, event):
         def event_ready(handler):
             if event not in self.events:
                 self.events[event] = []
             self.events[event].append(handler)
             return handler
@@ -29,18 +32,16 @@
 
     def trig(self, event, *args, **kwargs):
         if event in self.events:
             for handler in self.events[event]:
                 handler(*args, **kwargs)
 
     def send_json(self, payload):
-      try:
         self.ws.send(json.dumps(payload))
-      except:
-        return Exception("Start socket")
+
 
     def receive_json(self):
       response = self.ws.recv()
       if response:
         return json.loads(response)
         
     def send_and_receive_json(self, payload):
@@ -59,18 +60,21 @@
         self.send_json(payload)
 
     def start_ws(self):
       self.ws = websocket.WebSocket()
       self.ws.connect('wss://gateway.discord.gg/?encoding=json')
       self.send_json(StartSocket(self.token))
       Thread(target=self.event_manager).start()
-      self.session_id = self.receive_json()
-      self.session_id = self.session_id.get('d').get('session_id')
 
     def get_object(self, data):
+      if data['t'] == "READY":
+        self.session_id = data.get('d').get('session_id')
+        if not self.client.no_warns:
+          print(f"{self.client.var_} - Session ID: {self.session_id}")
+        
       if data['t'] == 'MESSAGE_CREATE':
         return MessageContent(data).MessageContent
 
       if data['t'] == 'GUILD_MEMBER_LIST_UPDATE':
         if data['s'] == 3:
           try:
             for item in data['d']['ops'][0]['items']:
```

### Comparing `user_discord-1.3.7/user_discord/user_discord.py` & `user_discord-2.0.0/user_discord/user_discord.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,39 +5,50 @@
 import requests
 import websocket
 from requests.structures import CaseInsensitiveDict
 from threading import Thread
 from user_discord.utils.payloads import StartSocket
 from user_discord.utils.objects import MessageContent
 from . import SocketDiscord
+from . import discord
+from .utils import youtube
+import asyncio
+from .utils import Thread
 
 
+global_variables = {}
+
 class ClientDiscord:
 
-  def __init__(self):
+  def __init__(self, no_warns: bool = False):
+    self.no_warns = no_warns
     
     self.token = None
 
-    self.username = None
+    self.Username = None
     self.email = None
     self.id = None
     self.telephone = None
 
     #Guild parameters
     self.online_members = []
-
+    
+    #Reqs
     self.headers = CaseInsensitiveDict()
+    self.var_ = "(user_discord)"
+    
 
 
   def generate_nonce(self):
-    return str(random.randint(1121966494243094528, 2121966494243094528))
+    return str(random.randint(int("1"+"0"*18), int("21"+"0"*17)))
 
   def login_token(self, token):
     # "Login" in account with token
     global requests
+    global global_variables
     api = "https://discord.com/api/users/@me"
     temp_headers = CaseInsensitiveDict()
     temp_headers['Authorization'] = token
     res = requests.get(api, headers=temp_headers)
     if res.status_code != 200:
       return Exception(res.text)
     else:
@@ -46,14 +57,17 @@
       self.web = requests.Session()
       self.web.headers = self.headers
       self.username = data['username']
       self.id = data['id']
       self.email = data['email']
       self.telephone = data['phone']
       self.token = token
+      global_variables = self
+      if not self.no_warns:
+        print(f'{self.var_} - Logged as: {self.username}')
       return data
 
   def send_message(self, channelId, message):
     #Send message in channel
     api = f"https://discord.com/api/v9/channels/{channelId}/messages"
     payload = {
       "content": message,
@@ -146,8 +160,40 @@
     else:
       return res.json()
       
   def get_members(self, socket, guild_id, channel_id):
     #Get members from channel
     socket.send_json({"op":14,"d":{"guild_id":guild_id,"channels":{channel_id:[[0,99]]}}})
     time.sleep(2)
-    return self.online_members
+    return self.online_members
+
+  def get_user(self, user_id):
+    #Get user from id
+    api = "https://discord.com/api/v9/users/@me/channels"
+    res = self.web.post(api, json={"recipients": [str(user_id)]})
+    if res.status_code != 200:
+      return Exception(res.text)
+    else:
+      return res.json()
+
+  class transmit_yt_song:
+    def __init__(self, channel_id, url):
+      self.voice_thread = None
+      self.channel_id = channel_id
+      self.url = url
+      
+    def trans_model(self, channel_id, url):
+          class VoiceClient(discord.Client):
+            async def on_ready(self):
+              self.vc = await player.get_channel(int(channel_id)).connect()
+              source = await youtube.YTDLSource.from_url(url)
+              await self.vc.play(source)
+          player = VoiceClient()
+          player.run(global_variables.token)
+        
+    def start(self):
+        self.voice_thread = Thread(target=self.trans_model, args=[self.channel_id, self.url])
+        self.voice_thread.start()
+        
+    def stop(self):
+        self.voice_thread.kill()
+        self.voice_thread.join()
```

### Comparing `user_discord-1.3.7/user_discord/utils/objects.py` & `user_discord-2.0.0/user_discord/utils/objects.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 class MessageContent:
   def __init__(self, data):
     self.json = data
     
   @property
   def MessageContent(self):
     self.Event = self.json.get('t')
-    self.Message = self.json.get('d').get('content')
+    self.Content = self.json.get('d').get('content')
     self.Author = AuthorProfile(self.json.get('d').get('author')).AuthorProfile
     self.id = self.json.get('d').get('id')
     self.timestamp = self.json.get('d').get('timestamp')
     self.MentionEveryone = self.json.get('d').get('mention_everyone')
+    self.ChannelId = self.json.get('d').get('channel_id')
 
     return self
```

### Comparing `user_discord-1.3.7/user_discord/utils/payloads.py` & `user_discord-2.0.0/user_discord/utils/payloads.py`

 * *Files identical despite different names*

