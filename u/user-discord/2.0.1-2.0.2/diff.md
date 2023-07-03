# Comparing `tmp/user_discord-2.0.1.tar.gz` & `tmp/user_discord-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_discord-2.0.1.tar", last modified: Mon Jul  3 17:52:27 2023, max compression
+gzip compressed data, was "user_discord-2.0.2.tar", last modified: Mon Jul  3 18:14:33 2023, max compression
```

## Comparing `user_discord-2.0.1.tar` & `user_discord-2.0.2.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 17:52:27.928425 user_discord-2.0.1/
--rw-rw-rw-   0        0        0      335 2023-07-03 17:52:27.928425 user_discord-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-2.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 17:52:27.931422 user_discord-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-07-03 17:52:05.000000 user_discord-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:52:27.609481 user_discord-2.0.1/user_discord/
--rw-rw-rw-   0        0        0      673 2023-07-03 17:52:10.000000 user_discord-2.0.1/user_discord/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:52:27.809499 user_discord-2.0.1/user_discord/discord/
--rw-rw-rw-   0        0        0     2436 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/__init__.py
--rw-rw-rw-   0        0        0    10966 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/__main__.py
--rw-rw-rw-   0        0        0    82000 2023-07-03 01:46:41.000000 user_discord-2.0.1/user_discord/discord/abc.py
--rw-rw-rw-   0        0        0    35249 2023-07-03 01:46:41.000000 user_discord-2.0.1/user_discord/discord/activity.py
--rw-rw-rw-   0        0        0     4272 2023-07-03 01:46:41.000000 user_discord-2.0.1/user_discord/discord/affinity.py
--rw-rw-rw-   0        0        0   124457 2023-07-03 01:46:41.000000 user_discord-2.0.1/user_discord/discord/application.py
--rw-rw-rw-   0        0        0    20104 2023-07-03 01:46:41.000000 user_discord-2.0.1/user_discord/discord/asset.py
--rw-rw-rw-   0        0        0    31379 2023-07-03 01:46:41.000000 user_discord-2.0.1/user_discord/discord/audit_logs.py
--rw-rw-rw-   0        0        0    24248 2023-07-03 01:46:41.000000 user_discord-2.0.1/user_discord/discord/automod.py
--rw-rw-rw-   0        0        0     3859 2023-07-03 01:46:41.000000 user_discord-2.0.1/user_discord/discord/backoff.py
--rw-rw-rw-   0        0        0    12634 2023-07-03 01:46:41.000000 user_discord-2.0.1/user_discord/discord/billing.py
--rw-rw-rw-   0        0        0    16172 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/calls.py
--rw-rw-rw-   0        0        0   134638 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/channel.py
--rw-rw-rw-   0        0        0   154059 2023-07-03 16:17:19.000000 user_discord-2.0.1/user_discord/discord/client.py
--rw-rw-rw-   0        0        0    14681 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/colour.py
--rw-rw-rw-   0        0        0    32936 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/commands.py
--rw-rw-rw-   0        0        0    17498 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/components.py
--rw-rw-rw-   0        0        0    11516 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/connections.py
--rw-rw-rw-   0        0        0     3124 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/context_managers.py
--rw-rw-rw-   0        0        0    23041 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/embeds.py
--rw-rw-rw-   0        0        0     9463 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/emoji.py
--rw-rw-rw-   0        0        0    23239 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/entitlements.py
--rw-rw-rw-   0        0        0    38120 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/enums.py
--rw-rw-rw-   0        0        0     8247 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/errors.py
--rw-rw-rw-   0        0        0     5816 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/file.py
--rw-rw-rw-   0        0        0    76908 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/flags.py
--rw-rw-rw-   0        0        0    39792 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/gateway.py
--rw-rw-rw-   0        0        0   168357 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/guild.py
--rw-rw-rw-   0        0        0    10816 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/guild_premium.py
--rw-rw-rw-   0        0        0     3529 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/handlers.py
--rw-rw-rw-   0        0        0   177638 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/http.py
--rw-rw-rw-   0        0        0    12512 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/integrations.py
--rw-rw-rw-   0        0        0     7790 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/interactions.py
--rw-rw-rw-   0        0        0    26660 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/invite.py
--rw-rw-rw-   0        0        0     9503 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/library.py
--rw-rw-rw-   0        0        0    43467 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/member.py
--rw-rw-rw-   0        0        0     5743 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/mentions.py
--rw-rw-rw-   0        0        0    85298 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/message.py
--rw-rw-rw-   0        0        0     4655 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/metadata.py
--rw-rw-rw-   0        0        0     1531 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/mixins.py
--rw-rw-rw-   0        0        0     4534 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/modal.py
--rw-rw-rw-   0        0        0     3812 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/object.py
--rw-rw-rw-   0        0        0     3763 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/oggparse.py
--rw-rw-rw-   0        0        0    15308 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/opus.py
--rw-rw-rw-   0        0        0     9165 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/partial_emoji.py
--rw-rw-rw-   0        0        0    10693 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/payments.py
--rw-rw-rw-   0        0        0    30168 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/permissions.py
--rw-rw-rw-   0        0        0    26617 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/player.py
--rw-rw-rw-   0        0        0    16128 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/profile.py
--rw-rw-rw-   0        0        0    10463 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/promotions.py
--rw-rw-rw-   0        0        0    12430 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/raw_models.py
--rw-rw-rw-   0        0        0     8482 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/reaction.py
--rw-rw-rw-   0        0        0    10742 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/relationship.py
--rw-rw-rw-   0        0        0    24102 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/role.py
--rw-rw-rw-   0        0        0    24244 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/scheduled_event.py
--rw-rw-rw-   0        0        0    98360 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/settings.py
--rw-rw-rw-   0        0        0     6848 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/stage_instance.py
--rw-rw-rw-   0        0        0   120924 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/state.py
--rw-rw-rw-   0        0        0    17642 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/sticker.py
--rw-rw-rw-   0        0        0    93140 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/store.py
--rw-rw-rw-   0        0        0    30116 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/subscriptions.py
--rw-rw-rw-   0        0        0    19286 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/team.py
--rw-rw-rw-   0        0        0     9691 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/template.py
--rw-rw-rw-   0        0        0    34125 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/threads.py
--rw-rw-rw-   0        0        0     7454 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/tracking.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:52:27.906437 user_discord-2.0.1/user_discord/discord/types/
--rw-rw-rw-   0        0        0      159 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/__init__.py
--rw-rw-rw-   0        0        0     2836 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/activity.py
--rw-rw-rw-   0        0        0     7631 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/application.py
--rw-rw-rw-   0        0        0     8193 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/audit_log.py
--rw-rw-rw-   0        0        0     4141 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/automod.py
--rw-rw-rw-   0        0        0     2493 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/billing.py
--rw-rw-rw-   0        0        0     5126 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/channel.py
--rw-rw-rw-   0        0        0     5805 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/command.py
--rw-rw-rw-   0        0        0     2548 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/components.py
--rw-rw-rw-   0        0        0     2419 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/embed.py
--rw-rw-rw-   0        0        0     1718 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/emoji.py
--rw-rw-rw-   0        0        0     3327 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/entitlements.py
--rw-rw-rw-   0        0        0    12841 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/gateway.py
--rw-rw-rw-   0        0        0     5168 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/guild.py
--rw-rw-rw-   0        0        0     2419 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/integration.py
--rw-rw-rw-   0        0        0     7070 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/interactions.py
--rw-rw-rw-   0        0        0     2813 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/invite.py
--rw-rw-rw-   0        0        0     1647 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/library.py
--rw-rw-rw-   0        0        0     2051 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/member.py
--rw-rw-rw-   0        0        0     4338 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/message.py
--rw-rw-rw-   0        0        0     2285 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/payments.py
--rw-rw-rw-   0        0        0     2668 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/profile.py
--rw-rw-rw-   0        0        0     2526 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/promotions.py
--rw-rw-rw-   0        0        0     1799 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/role.py
--rw-rw-rw-   0        0        0     3412 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/scheduled_event.py
--rw-rw-rw-   0        0        0     1210 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/snowflake.py
--rw-rw-rw-   0        0        0     2343 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/sticker.py
--rw-rw-rw-   0        0        0     5078 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/store.py
--rw-rw-rw-   0        0        0     4653 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/subscriptions.py
--rw-rw-rw-   0        0        0     2025 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/team.py
--rw-rw-rw-   0        0        0     1658 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/template.py
--rw-rw-rw-   0        0        0     2569 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/threads.py
--rw-rw-rw-   0        0        0     3841 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/user.py
--rw-rw-rw-   0        0        0     2415 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/voice.py
--rw-rw-rw-   0        0        0     2045 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/webhook.py
--rw-rw-rw-   0        0        0     1500 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/welcome_screen.py
--rw-rw-rw-   0        0        0     1948 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/types/widget.py
--rw-rw-rw-   0        0        0    35605 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/user.py
--rw-rw-rw-   0        0        0    50402 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/utils.py
--rw-rw-rw-   0        0        0    26266 2023-07-03 17:50:20.000000 user_discord-2.0.1/user_discord/discord/voice_client.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:52:27.913432 user_discord-2.0.1/user_discord/discord/webhook/
--rw-rw-rw-   0        0        0      195 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/webhook/__init__.py
--rw-rw-rw-   0        0        0    61821 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/webhook/async_.py
--rw-rw-rw-   0        0        0    43801 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/webhook/sync.py
--rw-rw-rw-   0        0        0     7603 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/welcome_screen.py
--rw-rw-rw-   0        0        0    10420 2023-07-03 01:46:42.000000 user_discord-2.0.1/user_discord/discord/widget.py
--rw-rw-rw-   0        0        0     2589 2023-07-03 03:20:52.000000 user_discord-2.0.1/user_discord/socket.py
--rw-rw-rw-   0        0        0     5845 2023-07-03 16:45:13.000000 user_discord-2.0.1/user_discord/user_discord.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:52:27.925426 user_discord-2.0.1/user_discord/utils/
--rw-rw-rw-   0        0        0      146 2023-07-03 16:25:15.000000 user_discord-2.0.1/user_discord/utils/__init__.py
--rw-rw-rw-   0        0        0     1484 2023-07-03 03:22:47.000000 user_discord-2.0.1/user_discord/utils/objects.py
--rw-rw-rw-   0        0        0      818 2023-07-03 01:46:43.000000 user_discord-2.0.1/user_discord/utils/payloads.py
--rw-rw-rw-   0        0        0      721 2023-07-03 16:24:34.000000 user_discord-2.0.1/user_discord/utils/threading.py
--rw-rw-rw-   0        0        0     1324 2023-07-03 03:32:12.000000 user_discord-2.0.1/user_discord/utils/youtube.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:52:27.631850 user_discord-2.0.1/user_discord.egg-info/
--rw-rw-rw-   0        0        0      335 2023-07-03 17:52:26.000000 user_discord-2.0.1/user_discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4292 2023-07-03 17:52:27.000000 user_discord-2.0.1/user_discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 17:52:26.000000 user_discord-2.0.1/user_discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-03 17:52:26.000000 user_discord-2.0.1/user_discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 17:52:26.000000 user_discord-2.0.1/user_discord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 18:14:33.053273 user_discord-2.0.2/
+-rw-rw-rw-   0        0        0      335 2023-07-03 18:14:33.053273 user_discord-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-2.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 18:14:33.056271 user_discord-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      731 2023-07-03 18:13:58.000000 user_discord-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 18:14:32.678051 user_discord-2.0.2/user_discord/
+-rw-rw-rw-   0        0        0      673 2023-07-03 18:14:05.000000 user_discord-2.0.2/user_discord/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 18:14:32.937987 user_discord-2.0.2/user_discord/discord/
+-rw-rw-rw-   0        0        0     2436 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/__init__.py
+-rw-rw-rw-   0        0        0    10966 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/__main__.py
+-rw-rw-rw-   0        0        0    82000 2023-07-03 01:46:41.000000 user_discord-2.0.2/user_discord/discord/abc.py
+-rw-rw-rw-   0        0        0    35249 2023-07-03 01:46:41.000000 user_discord-2.0.2/user_discord/discord/activity.py
+-rw-rw-rw-   0        0        0     4272 2023-07-03 01:46:41.000000 user_discord-2.0.2/user_discord/discord/affinity.py
+-rw-rw-rw-   0        0        0   124457 2023-07-03 01:46:41.000000 user_discord-2.0.2/user_discord/discord/application.py
+-rw-rw-rw-   0        0        0    20104 2023-07-03 01:46:41.000000 user_discord-2.0.2/user_discord/discord/asset.py
+-rw-rw-rw-   0        0        0    31379 2023-07-03 01:46:41.000000 user_discord-2.0.2/user_discord/discord/audit_logs.py
+-rw-rw-rw-   0        0        0    24248 2023-07-03 01:46:41.000000 user_discord-2.0.2/user_discord/discord/automod.py
+-rw-rw-rw-   0        0        0     3859 2023-07-03 01:46:41.000000 user_discord-2.0.2/user_discord/discord/backoff.py
+-rw-rw-rw-   0        0        0    12634 2023-07-03 01:46:41.000000 user_discord-2.0.2/user_discord/discord/billing.py
+-rw-rw-rw-   0        0        0    16172 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/calls.py
+-rw-rw-rw-   0        0        0   134638 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/channel.py
+-rw-rw-rw-   0        0        0   154059 2023-07-03 16:17:19.000000 user_discord-2.0.2/user_discord/discord/client.py
+-rw-rw-rw-   0        0        0    14681 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/colour.py
+-rw-rw-rw-   0        0        0    32936 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/commands.py
+-rw-rw-rw-   0        0        0    17498 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/components.py
+-rw-rw-rw-   0        0        0    11516 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/connections.py
+-rw-rw-rw-   0        0        0     3124 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/context_managers.py
+-rw-rw-rw-   0        0        0    23041 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/embeds.py
+-rw-rw-rw-   0        0        0     9463 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/emoji.py
+-rw-rw-rw-   0        0        0    23239 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/entitlements.py
+-rw-rw-rw-   0        0        0    38120 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/enums.py
+-rw-rw-rw-   0        0        0     8247 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/errors.py
+-rw-rw-rw-   0        0        0     5816 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/file.py
+-rw-rw-rw-   0        0        0    76908 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/flags.py
+-rw-rw-rw-   0        0        0    39792 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/gateway.py
+-rw-rw-rw-   0        0        0   168357 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/guild.py
+-rw-rw-rw-   0        0        0    10816 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/guild_premium.py
+-rw-rw-rw-   0        0        0     3529 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/handlers.py
+-rw-rw-rw-   0        0        0   177638 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/http.py
+-rw-rw-rw-   0        0        0    12512 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/integrations.py
+-rw-rw-rw-   0        0        0     7790 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/interactions.py
+-rw-rw-rw-   0        0        0    26660 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/invite.py
+-rw-rw-rw-   0        0        0     9503 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/library.py
+-rw-rw-rw-   0        0        0    43467 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/member.py
+-rw-rw-rw-   0        0        0     5743 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/mentions.py
+-rw-rw-rw-   0        0        0    85298 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/message.py
+-rw-rw-rw-   0        0        0     4655 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/metadata.py
+-rw-rw-rw-   0        0        0     1531 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/mixins.py
+-rw-rw-rw-   0        0        0     4534 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/modal.py
+-rw-rw-rw-   0        0        0     3812 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/object.py
+-rw-rw-rw-   0        0        0     3763 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/oggparse.py
+-rw-rw-rw-   0        0        0    15308 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/opus.py
+-rw-rw-rw-   0        0        0     9165 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/partial_emoji.py
+-rw-rw-rw-   0        0        0    10693 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/payments.py
+-rw-rw-rw-   0        0        0    30168 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/permissions.py
+-rw-rw-rw-   0        0        0    26617 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/player.py
+-rw-rw-rw-   0        0        0    16128 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/profile.py
+-rw-rw-rw-   0        0        0    10463 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/promotions.py
+-rw-rw-rw-   0        0        0    12430 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/raw_models.py
+-rw-rw-rw-   0        0        0     8482 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/reaction.py
+-rw-rw-rw-   0        0        0    10742 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/relationship.py
+-rw-rw-rw-   0        0        0    24102 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/role.py
+-rw-rw-rw-   0        0        0    24244 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/scheduled_event.py
+-rw-rw-rw-   0        0        0    98360 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/settings.py
+-rw-rw-rw-   0        0        0     6848 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/stage_instance.py
+-rw-rw-rw-   0        0        0   120924 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/state.py
+-rw-rw-rw-   0        0        0    17642 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/sticker.py
+-rw-rw-rw-   0        0        0    93140 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/store.py
+-rw-rw-rw-   0        0        0    30116 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/subscriptions.py
+-rw-rw-rw-   0        0        0    19286 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/team.py
+-rw-rw-rw-   0        0        0     9691 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/template.py
+-rw-rw-rw-   0        0        0    34125 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/threads.py
+-rw-rw-rw-   0        0        0     7454 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/tracking.py
+drwxrwxrwx   0        0        0        0 2023-07-03 18:14:33.034157 user_discord-2.0.2/user_discord/discord/types/
+-rw-rw-rw-   0        0        0      159 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/__init__.py
+-rw-rw-rw-   0        0        0     2836 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/activity.py
+-rw-rw-rw-   0        0        0     7631 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/application.py
+-rw-rw-rw-   0        0        0     8193 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/audit_log.py
+-rw-rw-rw-   0        0        0     4141 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/automod.py
+-rw-rw-rw-   0        0        0     2493 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/billing.py
+-rw-rw-rw-   0        0        0     5126 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/channel.py
+-rw-rw-rw-   0        0        0     5805 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/command.py
+-rw-rw-rw-   0        0        0     2548 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/components.py
+-rw-rw-rw-   0        0        0     2419 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/embed.py
+-rw-rw-rw-   0        0        0     1718 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/emoji.py
+-rw-rw-rw-   0        0        0     3327 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/entitlements.py
+-rw-rw-rw-   0        0        0    12841 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/gateway.py
+-rw-rw-rw-   0        0        0     5168 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/guild.py
+-rw-rw-rw-   0        0        0     2419 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/integration.py
+-rw-rw-rw-   0        0        0     7070 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/interactions.py
+-rw-rw-rw-   0        0        0     2813 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/invite.py
+-rw-rw-rw-   0        0        0     1647 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/library.py
+-rw-rw-rw-   0        0        0     2051 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/member.py
+-rw-rw-rw-   0        0        0     4338 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/message.py
+-rw-rw-rw-   0        0        0     2285 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/payments.py
+-rw-rw-rw-   0        0        0     2668 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/profile.py
+-rw-rw-rw-   0        0        0     2526 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/promotions.py
+-rw-rw-rw-   0        0        0     1799 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/role.py
+-rw-rw-rw-   0        0        0     3412 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/scheduled_event.py
+-rw-rw-rw-   0        0        0     1210 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/snowflake.py
+-rw-rw-rw-   0        0        0     2343 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/sticker.py
+-rw-rw-rw-   0        0        0     5078 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/store.py
+-rw-rw-rw-   0        0        0     4653 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/subscriptions.py
+-rw-rw-rw-   0        0        0     2025 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/team.py
+-rw-rw-rw-   0        0        0     1658 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/template.py
+-rw-rw-rw-   0        0        0     2569 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/threads.py
+-rw-rw-rw-   0        0        0     3841 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/user.py
+-rw-rw-rw-   0        0        0     2415 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/voice.py
+-rw-rw-rw-   0        0        0     2045 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/webhook.py
+-rw-rw-rw-   0        0        0     1500 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/welcome_screen.py
+-rw-rw-rw-   0        0        0     1948 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/types/widget.py
+-rw-rw-rw-   0        0        0    35605 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/user.py
+-rw-rw-rw-   0        0        0    50402 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/utils.py
+-rw-rw-rw-   0        0        0    26084 2023-07-03 18:04:18.000000 user_discord-2.0.2/user_discord/discord/voice_client.py
+drwxrwxrwx   0        0        0        0 2023-07-03 18:14:33.041153 user_discord-2.0.2/user_discord/discord/webhook/
+-rw-rw-rw-   0        0        0      195 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/webhook/__init__.py
+-rw-rw-rw-   0        0        0    61821 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/webhook/async_.py
+-rw-rw-rw-   0        0        0    43801 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/webhook/sync.py
+-rw-rw-rw-   0        0        0     7603 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/welcome_screen.py
+-rw-rw-rw-   0        0        0    10420 2023-07-03 01:46:42.000000 user_discord-2.0.2/user_discord/discord/widget.py
+-rw-rw-rw-   0        0        0     2589 2023-07-03 03:20:52.000000 user_discord-2.0.2/user_discord/socket.py
+-rw-rw-rw-   0        0        0     5845 2023-07-03 16:45:13.000000 user_discord-2.0.2/user_discord/user_discord.py
+drwxrwxrwx   0        0        0        0 2023-07-03 18:14:33.051274 user_discord-2.0.2/user_discord/utils/
+-rw-rw-rw-   0        0        0      146 2023-07-03 16:25:15.000000 user_discord-2.0.2/user_discord/utils/__init__.py
+-rw-rw-rw-   0        0        0     1484 2023-07-03 03:22:47.000000 user_discord-2.0.2/user_discord/utils/objects.py
+-rw-rw-rw-   0        0        0      818 2023-07-03 01:46:43.000000 user_discord-2.0.2/user_discord/utils/payloads.py
+-rw-rw-rw-   0        0        0      721 2023-07-03 16:24:34.000000 user_discord-2.0.2/user_discord/utils/threading.py
+-rw-rw-rw-   0        0        0     1324 2023-07-03 03:32:12.000000 user_discord-2.0.2/user_discord/utils/youtube.py
+drwxrwxrwx   0        0        0        0 2023-07-03 18:14:32.711499 user_discord-2.0.2/user_discord.egg-info/
+-rw-rw-rw-   0        0        0      335 2023-07-03 18:14:32.000000 user_discord-2.0.2/user_discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4292 2023-07-03 18:14:32.000000 user_discord-2.0.2/user_discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 18:14:32.000000 user_discord-2.0.2/user_discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-03 18:14:32.000000 user_discord-2.0.2/user_discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 18:14:32.000000 user_discord-2.0.2/user_discord.egg-info/top_level.txt
```

### Comparing `user_discord-2.0.1/README.md` & `user_discord-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/setup.py` & `user_discord-2.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from setuptools import setup, find_packages
 
 requirements = [
     "requests",
-    "websocket-client"
+    "websocket-client",
+    "yt-dlp",
+    "discord-protos",
+    "PyNaCl"
 ]
 
 long_description ="""By: nxslayer\nInstall: pip install user_discord"""
 
 setup(
     name="user_discord",
     license="MIT",
     author="nxSlayer",
-    version="2.0.1",
+    version="2.0.2",
     author_email="princediscordslay@gmail.com",
     description="Library for discord bots.",
     url="https://github.com/nxSlayer/user-discord",
     packages=find_packages(),
+    include_package_data=True,
     long_description=long_description,
     install_requires=requirements,
     keywords=[
         'user_discord',
         'user-discord',
     ],
     python_requires='>=3.6',
```

### Comparing `user_discord-2.0.1/user_discord/__init__.py` & `user_discord-2.0.2/user_discord/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 from .utils import Thread
 
 from requests import get
 from json import loads
 
 __newest__ = loads(get("https://pypi.org/pypi/user-discord/json").text)["info"]["version"]
 
-if '2.0.1' != __newest__:
+if '2.0.2' != __newest__:
     print(f"(user-discord) There is a new version, please update for better results")
```

### Comparing `user_discord-2.0.1/user_discord/discord/__init__.py` & `user_discord-2.0.2/user_discord/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/__main__.py` & `user_discord-2.0.2/user_discord/discord/__main__.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/abc.py` & `user_discord-2.0.2/user_discord/discord/abc.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/activity.py` & `user_discord-2.0.2/user_discord/discord/activity.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/affinity.py` & `user_discord-2.0.2/user_discord/discord/affinity.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/application.py` & `user_discord-2.0.2/user_discord/discord/application.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/asset.py` & `user_discord-2.0.2/user_discord/discord/asset.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/audit_logs.py` & `user_discord-2.0.2/user_discord/discord/audit_logs.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/automod.py` & `user_discord-2.0.2/user_discord/discord/automod.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/backoff.py` & `user_discord-2.0.2/user_discord/discord/backoff.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/billing.py` & `user_discord-2.0.2/user_discord/discord/billing.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/calls.py` & `user_discord-2.0.2/user_discord/discord/calls.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/channel.py` & `user_discord-2.0.2/user_discord/discord/channel.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/client.py` & `user_discord-2.0.2/user_discord/discord/client.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/colour.py` & `user_discord-2.0.2/user_discord/discord/colour.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/commands.py` & `user_discord-2.0.2/user_discord/discord/commands.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/components.py` & `user_discord-2.0.2/user_discord/discord/components.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/connections.py` & `user_discord-2.0.2/user_discord/discord/connections.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/context_managers.py` & `user_discord-2.0.2/user_discord/discord/context_managers.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/embeds.py` & `user_discord-2.0.2/user_discord/discord/embeds.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/emoji.py` & `user_discord-2.0.2/user_discord/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/entitlements.py` & `user_discord-2.0.2/user_discord/discord/entitlements.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/enums.py` & `user_discord-2.0.2/user_discord/discord/enums.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/errors.py` & `user_discord-2.0.2/user_discord/discord/errors.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/file.py` & `user_discord-2.0.2/user_discord/discord/file.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/flags.py` & `user_discord-2.0.2/user_discord/discord/flags.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/gateway.py` & `user_discord-2.0.2/user_discord/discord/gateway.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/guild.py` & `user_discord-2.0.2/user_discord/discord/guild.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/guild_premium.py` & `user_discord-2.0.2/user_discord/discord/guild_premium.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/handlers.py` & `user_discord-2.0.2/user_discord/discord/handlers.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/http.py` & `user_discord-2.0.2/user_discord/discord/http.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/integrations.py` & `user_discord-2.0.2/user_discord/discord/integrations.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/interactions.py` & `user_discord-2.0.2/user_discord/discord/interactions.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/invite.py` & `user_discord-2.0.2/user_discord/discord/invite.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/library.py` & `user_discord-2.0.2/user_discord/discord/library.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/member.py` & `user_discord-2.0.2/user_discord/discord/member.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/mentions.py` & `user_discord-2.0.2/user_discord/discord/mentions.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/message.py` & `user_discord-2.0.2/user_discord/discord/message.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/metadata.py` & `user_discord-2.0.2/user_discord/discord/metadata.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/mixins.py` & `user_discord-2.0.2/user_discord/discord/mixins.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/modal.py` & `user_discord-2.0.2/user_discord/discord/modal.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/object.py` & `user_discord-2.0.2/user_discord/discord/object.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/oggparse.py` & `user_discord-2.0.2/user_discord/discord/oggparse.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/opus.py` & `user_discord-2.0.2/user_discord/discord/opus.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/partial_emoji.py` & `user_discord-2.0.2/user_discord/discord/partial_emoji.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/payments.py` & `user_discord-2.0.2/user_discord/discord/payments.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/permissions.py` & `user_discord-2.0.2/user_discord/discord/permissions.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/player.py` & `user_discord-2.0.2/user_discord/discord/player.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/profile.py` & `user_discord-2.0.2/user_discord/discord/profile.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/promotions.py` & `user_discord-2.0.2/user_discord/discord/promotions.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/raw_models.py` & `user_discord-2.0.2/user_discord/discord/raw_models.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/reaction.py` & `user_discord-2.0.2/user_discord/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/relationship.py` & `user_discord-2.0.2/user_discord/discord/relationship.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/role.py` & `user_discord-2.0.2/user_discord/discord/role.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/scheduled_event.py` & `user_discord-2.0.2/user_discord/discord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/settings.py` & `user_discord-2.0.2/user_discord/discord/settings.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/stage_instance.py` & `user_discord-2.0.2/user_discord/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/state.py` & `user_discord-2.0.2/user_discord/discord/state.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/sticker.py` & `user_discord-2.0.2/user_discord/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/store.py` & `user_discord-2.0.2/user_discord/discord/store.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/subscriptions.py` & `user_discord-2.0.2/user_discord/discord/subscriptions.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/team.py` & `user_discord-2.0.2/user_discord/discord/team.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/template.py` & `user_discord-2.0.2/user_discord/discord/template.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/threads.py` & `user_discord-2.0.2/user_discord/discord/threads.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/tracking.py` & `user_discord-2.0.2/user_discord/discord/tracking.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/activity.py` & `user_discord-2.0.2/user_discord/discord/types/activity.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/application.py` & `user_discord-2.0.2/user_discord/discord/types/application.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/audit_log.py` & `user_discord-2.0.2/user_discord/discord/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/automod.py` & `user_discord-2.0.2/user_discord/discord/types/automod.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/billing.py` & `user_discord-2.0.2/user_discord/discord/types/billing.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/channel.py` & `user_discord-2.0.2/user_discord/discord/types/channel.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/command.py` & `user_discord-2.0.2/user_discord/discord/types/command.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/components.py` & `user_discord-2.0.2/user_discord/discord/types/components.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/embed.py` & `user_discord-2.0.2/user_discord/discord/types/embed.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/emoji.py` & `user_discord-2.0.2/user_discord/discord/types/emoji.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/entitlements.py` & `user_discord-2.0.2/user_discord/discord/types/entitlements.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/gateway.py` & `user_discord-2.0.2/user_discord/discord/types/gateway.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/guild.py` & `user_discord-2.0.2/user_discord/discord/types/guild.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/integration.py` & `user_discord-2.0.2/user_discord/discord/types/integration.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/interactions.py` & `user_discord-2.0.2/user_discord/discord/types/interactions.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/invite.py` & `user_discord-2.0.2/user_discord/discord/types/invite.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/library.py` & `user_discord-2.0.2/user_discord/discord/types/library.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/member.py` & `user_discord-2.0.2/user_discord/discord/types/member.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/message.py` & `user_discord-2.0.2/user_discord/discord/types/message.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/payments.py` & `user_discord-2.0.2/user_discord/discord/types/payments.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/profile.py` & `user_discord-2.0.2/user_discord/discord/types/profile.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/promotions.py` & `user_discord-2.0.2/user_discord/discord/types/promotions.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/role.py` & `user_discord-2.0.2/user_discord/discord/types/role.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/scheduled_event.py` & `user_discord-2.0.2/user_discord/discord/types/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/snowflake.py` & `user_discord-2.0.2/user_discord/discord/types/snowflake.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/sticker.py` & `user_discord-2.0.2/user_discord/discord/types/sticker.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/store.py` & `user_discord-2.0.2/user_discord/discord/types/store.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/subscriptions.py` & `user_discord-2.0.2/user_discord/discord/types/subscriptions.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/team.py` & `user_discord-2.0.2/user_discord/discord/types/team.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/template.py` & `user_discord-2.0.2/user_discord/discord/types/template.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/threads.py` & `user_discord-2.0.2/user_discord/discord/types/threads.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/user.py` & `user_discord-2.0.2/user_discord/discord/types/user.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/voice.py` & `user_discord-2.0.2/user_discord/discord/types/voice.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/webhook.py` & `user_discord-2.0.2/user_discord/discord/types/webhook.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/welcome_screen.py` & `user_discord-2.0.2/user_discord/discord/types/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/types/widget.py` & `user_discord-2.0.2/user_discord/discord/types/widget.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/user.py` & `user_discord-2.0.2/user_discord/discord/user.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/utils.py` & `user_discord-2.0.2/user_discord/discord/utils.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/voice_client.py` & `user_discord-2.0.2/user_discord/discord/voice_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,47 +343,42 @@
         if self.guild:
             await self.guild.change_voice_state(channel=channel, self_deaf=self_deaf, self_mute=self_mute)
         else:
             await self._state.client.change_voice_state(channel=channel, self_deaf=self_deaf, self_mute=self_mute)
 
     async def voice_disconnect(self) -> None:
         guild = self.guild
-        _log.info(
-            'The voice handshake is being terminated for channel ID %s (guild ID %s).',
-            self.channel.id,
-            getattr(guild, 'id', None),
-        )
         if guild:
             await guild.change_voice_state(channel=None)
         else:
             await self._state.client.change_voice_state(channel=None)
 
     def prepare_handshake(self) -> None:
         self._voice_state_complete.clear()
         self._voice_server_complete.clear()
         self._handshaking = True
-        _log.info('Starting voice handshake (connection attempt %d)...', self._connections + 1)
+        #_log.info('Starting voice handshake (connection attempt %d)...', self._connections + 1)
         self._connections += 1
 
     def finish_handshake(self) -> None:
-        _log.info('Voice handshake complete. Endpoint found: %s.', self.endpoint)
+        #_log.info('Voice handshake complete. Endpoint found: %s.', self.endpoint)
         self._handshaking = False
         self._voice_server_complete.clear()
         self._voice_state_complete.clear()
 
     async def connect_websocket(self) -> DiscordVoiceWebSocket:
         ws = await DiscordVoiceWebSocket.from_client(self)
         self._connected.clear()
         while ws.secret_key is None:
             await ws.poll_event()
         self._connected.set()
         return ws
 
     async def connect(self, *, reconnect: bool, timeout: float, self_deaf: bool = False, self_mute: bool = False) -> None:
-        _log.info('Connecting to voice...')
+        #_log.info('Connecting to voice...')
         self.timeout = timeout
 
         for i in range(5):
             self.prepare_handshake()
 
             # This has to be created before we start the flow
             futures = [
@@ -468,33 +463,33 @@
             except (ConnectionClosed, asyncio.TimeoutError) as exc:
                 if isinstance(exc, ConnectionClosed):
                     # The following close codes are undocumented so I will document them here.
                     # 1000 - normal closure (obviously)
                     # 4014 - voice channel has been deleted.
                     # 4015 - voice server has crashed
                     if exc.code in (1000, 4015):
-                        _log.info('Disconnecting from voice normally, close code %d.', exc.code)
+                        #_log.info('Disconnecting from voice normally, close code %d.', exc.code)
                         await self.disconnect()
                         break
                     if exc.code == 4014:
-                        _log.info('Disconnected from voice by force... potentially reconnecting.')
+                        #_log.info('Disconnected from voice by force... potentially reconnecting.')
                         successful = await self.potential_reconnect()
                         if not successful:
-                            _log.info('Reconnect was unsuccessful, disconnecting from voice normally...')
+                            #_log.info('Reconnect was unsuccessful, disconnecting from voice normally...')
                             await self.disconnect()
                             break
                         else:
                             continue
 
                 if not reconnect:
                     await self.disconnect()
                     raise
 
                 retry = backoff.delay()
-                _log.exception('Disconnected from voice... Reconnecting in %.2fs.', retry)
+                #_log.exception('Disconnected from voice... Reconnecting in %.2fs.', retry)
                 self._connected.clear()
                 await asyncio.sleep(retry)
                 await self.voice_disconnect()
                 try:
                     await self.connect(reconnect=True, timeout=self.timeout)
                 except asyncio.TimeoutError:
                     # at this point we've retried 5 times... let's continue the loop.
@@ -694,8 +689,8 @@
             encoded_data = data
         packet = self._get_voice_packet(encoded_data)
         try:
             self.socket.sendto(packet, (self.endpoint_ip, self.voice_port))
         except BlockingIOError:
             _log.warning('A packet has been dropped (seq: %s, timestamp: %s)', self.sequence, self.timestamp)
 
-        self.checked_add('timestamp', opus.Encoder.SAMPLES_PER_FRAME, 4294967295)
+        self.checked_add('timestamp', opus.Encoder.SAMPLES_PER_FRAME, 4294967295)
```

### Comparing `user_discord-2.0.1/user_discord/discord/webhook/async_.py` & `user_discord-2.0.2/user_discord/discord/webhook/async_.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/webhook/sync.py` & `user_discord-2.0.2/user_discord/discord/webhook/sync.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/welcome_screen.py` & `user_discord-2.0.2/user_discord/discord/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/discord/widget.py` & `user_discord-2.0.2/user_discord/discord/widget.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/socket.py` & `user_discord-2.0.2/user_discord/socket.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/user_discord.py` & `user_discord-2.0.2/user_discord/user_discord.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/utils/objects.py` & `user_discord-2.0.2/user_discord/utils/objects.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/utils/payloads.py` & `user_discord-2.0.2/user_discord/utils/payloads.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/utils/threading.py` & `user_discord-2.0.2/user_discord/utils/threading.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord/utils/youtube.py` & `user_discord-2.0.2/user_discord/utils/youtube.py`

 * *Files identical despite different names*

### Comparing `user_discord-2.0.1/user_discord.egg-info/SOURCES.txt` & `user_discord-2.0.2/user_discord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

