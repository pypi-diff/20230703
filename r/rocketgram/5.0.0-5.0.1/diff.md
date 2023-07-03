# Comparing `tmp/rocketgram-5.0.0.tar.gz` & `tmp/rocketgram-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketgram-5.0.0.tar", last modified: Sat Mar 11 17:59:24 2023, max compression
+gzip compressed data, was "rocketgram-5.0.1.tar", last modified: Mon Jul  3 20:32:01 2023, max compression
```

## Comparing `rocketgram-5.0.0.tar` & `rocketgram-5.0.1.tar`

### file list

```diff
@@ -1,332 +1,332 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:59:24.046850 rocketgram-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-11 17:59:12.000000 rocketgram-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-03-11 17:59:24.046850 rocketgram-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-11 17:59:12.000000 rocketgram-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:59:24.018849 rocketgram-5.0.0/rocketgram/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:59:24.042849 rocketgram-5.0.0/rocketgram/api/
--rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/add_sticker_to_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/answer_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/answer_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/answer_pre_checkout_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/answer_shipping_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/answer_web_app_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/approve_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/ban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/ban_chat_sender_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/bot_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/bot_command_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/bot_command_scope_all_group_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/bot_command_scope_all_private_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/bot_command_scope_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/bot_command_scope_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/bot_command_scope_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/bot_command_scope_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/bot_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/bot_short_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/chat_action_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/chat_administrator_rights.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/chat_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/chat_member_status_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/chat_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/chat_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/close.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/close_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/close_general_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/copy_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/create_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/create_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/create_invoice_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/create_new_sticker_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/decline_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/delete_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/delete_chat_sticker_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/delete_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/delete_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/delete_my_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/delete_sticker_from_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/delete_sticker_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/delete_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/dice_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/edit_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/edit_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/edit_general_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/edit_message_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/edit_message_live_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/edit_message_media.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/edit_message_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/edit_message_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/encrypted_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/encrypted_passport_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/encrypted_passport_element_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/export_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/forum_topic_closed.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/forum_topic_created.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/forum_topic_edited.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/forum_topic_reopened.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/forward_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/game.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/game_high_score.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/general_forum_topic_hidden.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/general_forum_topic_unhidden.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_chat_member_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_custom_emoji_stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_forum_topic_icon_stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_game_high_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_me.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_my_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_my_default_administrator_rights.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_my_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_my_short_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_sticker_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_user_profile_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/get_webhook_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/hide_general_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_article.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_gif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_mpeg4_gif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_document.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_game.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_gif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_mpeg4_gif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/inline_query_result_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/input_contact_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/input_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/input_invoice_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/input_location_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/input_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/input_media_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/input_media_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/input_media_document.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/input_media_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/input_media_video.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/input_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/input_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/input_text_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/input_venue_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/keyboard_button_poll_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/keyboard_button_request_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/keyboard_button_request_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/labeled_price.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/leave_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/location.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/log_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/login_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/mask_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/mask_position_point_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/menu_button_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/menu_button_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/menu_button_web_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/message_auto_delete_timer_changed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/message_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/message_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/order_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/parse_mode_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/passport_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/passport_element_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/passport_element_error_data_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/passport_element_error_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/passport_element_error_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/passport_element_error_front_side.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/passport_element_error_reverse_side.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/passport_element_error_selfie.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/passport_element_error_translation_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/passport_element_error_translation_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/passport_element_error_unspecified.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/password_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/photo_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/pin_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/poll_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/poll_option.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/poll_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/pre_checkout_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/promote_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/proximity_alert_triggered.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/reopen_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/reopen_general_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/reply_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/reply_keyboard_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/response_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/restrict_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/revoke_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_document.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_game.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/send_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/sent_web_app_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_chat_administrator_custom_title.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_chat_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_chat_sticker_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_chat_title.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_custom_emoji_sticker_set_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_game_score.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_my_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_my_default_administrator_rights.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_my_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_my_short_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_passport_data_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_sticker_emoji_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_sticker_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_sticker_mask_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_sticker_position_in_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_sticker_set_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_sticker_set_title.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/set_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/shipping_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/shipping_option.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/shipping_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/sticker_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/sticker_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/sticker_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/stop_message_live_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/stop_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/successful_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/thumbnail_mime_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/unban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/unban_chat_sender_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/unhide_general_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/unpin_all_chat_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/unpin_all_forum_topic_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/unpin_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/update_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/upload_sticker_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/user_profile_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/user_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/video.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/video_chat_ended.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/video_chat_participants_invited.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/video_chat_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/video_chat_started.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/web_app_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/web_app_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/webhook_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/api/write_access_allowed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:59:24.042849 rocketgram-5.0.0/rocketgram/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/connectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/connectors/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:59:24.046850 rocketgram-5.0.0/rocketgram/executors/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/executors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/executors/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/executors/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/executors/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:59:24.046850 rocketgram-5.0.0/rocketgram/json_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/json_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/json_adapters/base_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/json_adapters/orjson_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/json_adapters/standard_json_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/json_adapters/ujson_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:59:24.046850 rocketgram-5.0.0/rocketgram/keyboards/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/keyboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/keyboards/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/keyboards/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/keyboards/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/keyboards/reply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:59:24.046850 rocketgram-5.0.0/rocketgram/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/middlewares/defaultvalues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/middlewares/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/middlewares/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/middlewares/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:59:24.046850 rocketgram-5.0.0/rocketgram/routers/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/routers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:59:24.046850 rocketgram-5.0.0/rocketgram/routers/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/routers/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/routers/dispatcher/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/routers/dispatcher/commonfilters.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/routers/dispatcher/commonwaiters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/routers/dispatcher/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/routers/dispatcher/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/routers/dispatcher/waiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/routers/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:59:24.046850 rocketgram-5.0.0/rocketgram/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/tools/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/tools/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-11 17:59:12.000000 rocketgram-5.0.0/rocketgram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 17:59:24.018849 rocketgram-5.0.0/rocketgram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-03-11 17:59:23.000000 rocketgram-5.0.0/rocketgram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-03-11 17:59:23.000000 rocketgram-5.0.0/rocketgram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 17:59:23.000000 rocketgram-5.0.0/rocketgram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-11 17:59:23.000000 rocketgram-5.0.0/rocketgram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-11 17:59:23.000000 rocketgram-5.0.0/rocketgram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 17:59:24.046850 rocketgram-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-11 17:59:12.000000 rocketgram-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:01.801208 rocketgram-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-03 20:31:51.000000 rocketgram-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-03 20:32:01.801208 rocketgram-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-03 20:31:51.000000 rocketgram-5.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:01.773208 rocketgram-5.0.1/rocketgram/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:01.797208 rocketgram-5.0.1/rocketgram/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/add_sticker_to_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/answer_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/answer_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/answer_pre_checkout_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/answer_shipping_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/answer_web_app_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/approve_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/ban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/ban_chat_sender_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/bot_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/bot_command_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/bot_command_scope_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/bot_command_scope_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/bot_command_scope_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/bot_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/bot_short_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/chat_action_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/chat_administrator_rights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/chat_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/chat_member_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/chat_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/chat_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/close.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/close_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/close_general_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/copy_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/create_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/create_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/create_invoice_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/create_new_sticker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/decline_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/delete_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/delete_chat_sticker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/delete_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/delete_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/delete_my_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/delete_sticker_from_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/delete_sticker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/delete_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/dice_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/edit_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/edit_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/edit_general_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/edit_message_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/edit_message_live_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/edit_message_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/edit_message_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/edit_message_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/encrypted_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/encrypted_passport_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/encrypted_passport_element_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/export_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/forum_topic_closed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/forum_topic_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/forum_topic_edited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/forum_topic_reopened.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/forward_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/game_high_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/general_forum_topic_hidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/general_forum_topic_unhidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_chat_member_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_custom_emoji_stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_forum_topic_icon_stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_game_high_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_my_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_my_default_administrator_rights.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_my_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_my_short_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_sticker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_user_profile_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/get_webhook_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/hide_general_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_article.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_gif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_mpeg4_gif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_gif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_mpeg4_gif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/inline_query_result_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/input_contact_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/input_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/input_invoice_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/input_location_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/input_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/input_media_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/input_media_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/input_media_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/input_media_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/input_media_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/input_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/input_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/input_text_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/input_venue_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/keyboard_button_poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/keyboard_button_request_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/keyboard_button_request_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/labeled_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/leave_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/log_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/login_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/mask_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/mask_position_point_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/menu_button_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/menu_button_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/menu_button_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/message_auto_delete_timer_changed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/message_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/message_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/order_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/parse_mode_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/passport_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/passport_element_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/passport_element_error_data_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/passport_element_error_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/passport_element_error_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/passport_element_error_front_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/passport_element_error_reverse_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/passport_element_error_selfie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/passport_element_error_translation_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/passport_element_error_translation_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/passport_element_error_unspecified.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/password_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/photo_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/pin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/poll_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/poll_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/pre_checkout_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/promote_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/proximity_alert_triggered.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/reopen_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/reopen_general_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/reply_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/reply_keyboard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/response_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/restrict_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/revoke_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/send_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/sent_web_app_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_chat_administrator_custom_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_chat_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_chat_sticker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_chat_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_custom_emoji_sticker_set_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_game_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_my_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_my_default_administrator_rights.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_my_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_my_short_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_passport_data_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_sticker_emoji_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_sticker_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_sticker_mask_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_sticker_position_in_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_sticker_set_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_sticker_set_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/set_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/shipping_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/shipping_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/shipping_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/sticker_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/sticker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/sticker_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/stop_message_live_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/stop_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/successful_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/thumbnail_mime_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/unban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/unban_chat_sender_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/unhide_general_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/unpin_all_chat_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/unpin_all_forum_topic_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/unpin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/update_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/upload_sticker_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/user_profile_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/user_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/video_chat_ended.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/video_chat_participants_invited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/video_chat_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/video_chat_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/web_app_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/web_app_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/webhook_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/api/write_access_allowed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:01.797208 rocketgram-5.0.1/rocketgram/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/connectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/connectors/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:01.797208 rocketgram-5.0.1/rocketgram/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/executors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/executors/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/executors/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/executors/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:01.797208 rocketgram-5.0.1/rocketgram/json_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/json_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/json_adapters/base_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/json_adapters/orjson_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/json_adapters/standard_json_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/json_adapters/ujson_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:01.797208 rocketgram-5.0.1/rocketgram/keyboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/keyboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/keyboards/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/keyboards/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/keyboards/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/keyboards/reply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:01.801208 rocketgram-5.0.1/rocketgram/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/middlewares/defaultvalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/middlewares/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/middlewares/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/middlewares/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:01.801208 rocketgram-5.0.1/rocketgram/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/routers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:01.801208 rocketgram-5.0.1/rocketgram/routers/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/routers/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/routers/dispatcher/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/routers/dispatcher/commonfilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/routers/dispatcher/commonwaiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/routers/dispatcher/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/routers/dispatcher/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/routers/dispatcher/waiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/routers/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:01.801208 rocketgram-5.0.1/rocketgram/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/tools/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/tools/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-03 20:31:51.000000 rocketgram-5.0.1/rocketgram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:32:01.773208 rocketgram-5.0.1/rocketgram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-03 20:32:01.000000 rocketgram-5.0.1/rocketgram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-07-03 20:32:01.000000 rocketgram-5.0.1/rocketgram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:32:01.000000 rocketgram-5.0.1/rocketgram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-03 20:32:01.000000 rocketgram-5.0.1/rocketgram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 20:32:01.000000 rocketgram-5.0.1/rocketgram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 20:32:01.801208 rocketgram-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-03 20:31:51.000000 rocketgram-5.0.1/setup.py
```

### Comparing `rocketgram-5.0.0/LICENSE` & `rocketgram-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/PKG-INFO` & `rocketgram-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketgram
-Version: 5.0.0
+Version: 5.0.1
 Summary: Modern and powerful asynchronous telegram bot framework.
 Home-page: https://github.com/rocketgram/rocketgram
 Author: Vd
 Author-email: vd@vd2.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rocketgram-5.0.0/README.md` & `rocketgram-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/__init__.py` & `rocketgram-5.0.1/rocketgram/__init__.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/__init__.py` & `rocketgram-5.0.1/rocketgram/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/add_sticker_to_set.py` & `rocketgram-5.0.1/rocketgram/api/add_sticker_to_set.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/animation.py` & `rocketgram-5.0.1/rocketgram/api/animation.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/answer_callback_query.py` & `rocketgram-5.0.1/rocketgram/api/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/answer_inline_query.py` & `rocketgram-5.0.1/rocketgram/api/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/answer_pre_checkout_query.py` & `rocketgram-5.0.1/rocketgram/api/answer_pre_checkout_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     """\
     Represents AnswerPreCheckoutQuery request object:
     https://core.telegram.org/bots/api#answerprecheckoutquery
     """
 
     pre_checkout_query_id: str
     ok: bool
-    error_message: Optional[str]
+    error_message: Optional[str] = None
```

### Comparing `rocketgram-5.0.0/rocketgram/api/answer_shipping_query.py` & `rocketgram-5.0.1/rocketgram/api/answer_shipping_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     """\
     Represents AnswerShippingQuery request object:
     https://core.telegram.org/bots/api#answershippingquery
     """
 
     shipping_query_id: str
     ok: bool
-    shipping_options: Optional[List[ShippingOption]]
-    error_message: Optional[str]
+    shipping_options: Optional[List[ShippingOption]] = None
+    error_message: Optional[str] = None
```

### Comparing `rocketgram-5.0.0/rocketgram/api/answer_web_app_query.py` & `rocketgram-5.0.1/rocketgram/api/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/approve_chat_join_request.py` & `rocketgram-5.0.1/rocketgram/api/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/audio.py` & `rocketgram-5.0.1/rocketgram/api/audio.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/ban_chat_member.py` & `rocketgram-5.0.1/rocketgram/api/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/ban_chat_sender_chat.py` & `rocketgram-5.0.1/rocketgram/api/ban_chat_sender_chat.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/bot_command.py` & `rocketgram-5.0.1/rocketgram/api/bot_command.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/bot_command_scope_all_chat_administrators.py` & `rocketgram-5.0.1/rocketgram/api/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/bot_command_scope_all_group_chats.py` & `rocketgram-5.0.1/rocketgram/api/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/bot_command_scope_all_private_chats.py` & `rocketgram-5.0.1/rocketgram/api/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/bot_command_scope_chat.py` & `rocketgram-5.0.1/rocketgram/api/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/bot_command_scope_chat_administrators.py` & `rocketgram-5.0.1/rocketgram/api/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/bot_command_scope_chat_member.py` & `rocketgram-5.0.1/rocketgram/api/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/bot_description.py` & `rocketgram-5.0.1/rocketgram/api/bot_description.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/bot_short_description.py` & `rocketgram-5.0.1/rocketgram/api/bot_short_description.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/callback_query.py` & `rocketgram-5.0.1/rocketgram/api/callback_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/chat.py` & `rocketgram-5.0.1/rocketgram/api/chat.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/chat_action_type.py` & `rocketgram-5.0.1/rocketgram/api/chat_action_type.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/chat_administrator_rights.py` & `rocketgram-5.0.1/rocketgram/api/chat_administrator_rights.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/chat_invite_link.py` & `rocketgram-5.0.1/rocketgram/api/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/chat_join_request.py` & `rocketgram-5.0.1/rocketgram/api/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/chat_location.py` & `rocketgram-5.0.1/rocketgram/api/chat_location.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/chat_member.py` & `rocketgram-5.0.1/rocketgram/api/chat_member.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/chat_member_updated.py` & `rocketgram-5.0.1/rocketgram/api/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/chat_permissions.py` & `rocketgram-5.0.1/rocketgram/api/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/chat_photo.py` & `rocketgram-5.0.1/rocketgram/api/chat_photo.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/chat_shared.py` & `rocketgram-5.0.1/rocketgram/api/chat_shared.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/chosen_inline_result.py` & `rocketgram-5.0.1/rocketgram/api/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/close_forum_topic.py` & `rocketgram-5.0.1/rocketgram/api/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/close_general_forum_topic.py` & `rocketgram-5.0.1/rocketgram/api/close_general_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/contact.py` & `rocketgram-5.0.1/rocketgram/api/contact.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/copy_message.py` & `rocketgram-5.0.1/rocketgram/api/copy_message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/create_chat_invite_link.py` & `rocketgram-5.0.1/rocketgram/api/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/create_forum_topic.py` & `rocketgram-5.0.1/rocketgram/api/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/create_invoice_link.py` & `rocketgram-5.0.1/rocketgram/api/create_invoice_link.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/create_new_sticker_set.py` & `rocketgram-5.0.1/rocketgram/api/create_new_sticker_set.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/decline_chat_join_request.py` & `rocketgram-5.0.1/rocketgram/api/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/delete_chat_photo.py` & `rocketgram-5.0.1/rocketgram/api/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/delete_chat_sticker_set.py` & `rocketgram-5.0.1/rocketgram/api/delete_chat_sticker_set.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/delete_forum_topic.py` & `rocketgram-5.0.1/rocketgram/api/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/delete_message.py` & `rocketgram-5.0.1/rocketgram/api/delete_message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/delete_my_commands.py` & `rocketgram-5.0.1/rocketgram/api/set_my_commands.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 # This file is part of Rocketgram, the modern Telegram bot framework.
 # Rocketgram is released under the MIT License (see LICENSE).
 
 
 from dataclasses import dataclass
 from typing import List, Optional
 
+from .bot_command import BotCommand
 from .bot_command_scope import BotCommandScope
 from .request import Request
 from .utils import BoolResultMixin
 
 
 @dataclass(frozen=True)
-class DeleteMyCommands(BoolResultMixin, Request):
+class SetMyCommands(BoolResultMixin, Request):
     """\
-    Represents DeleteMyCommands request object:
-    https://core.telegram.org/bots/api#deletemycommands
+    Represents SetMyCommands request object:
+    https://core.telegram.org/bots/api#setmycommands
     """
 
-    scope: Optional[List[BotCommandScope]]
-    language_code: Optional[str]
+    commands: List[BotCommand]
+    scope: Optional[BotCommandScope] = None
+    language_code: Optional[str] = None
```

### Comparing `rocketgram-5.0.0/rocketgram/api/delete_webhook.py` & `rocketgram-5.0.1/rocketgram/api/delete_webhook.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/dice.py` & `rocketgram-5.0.1/rocketgram/api/dice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/document.py` & `rocketgram-5.0.1/rocketgram/api/document.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/edit_chat_invite_link.py` & `rocketgram-5.0.1/rocketgram/api/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/edit_forum_topic.py` & `rocketgram-5.0.1/rocketgram/api/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/edit_general_forum_topic.py` & `rocketgram-5.0.1/rocketgram/api/edit_general_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/edit_message_caption.py` & `rocketgram-5.0.1/rocketgram/api/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/edit_message_live_location.py` & `rocketgram-5.0.1/rocketgram/api/edit_message_live_location.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/edit_message_media.py` & `rocketgram-5.0.1/rocketgram/api/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/edit_message_reply_markup.py` & `rocketgram-5.0.1/rocketgram/api/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/edit_message_text.py` & `rocketgram-5.0.1/rocketgram/api/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/encrypted_credentials.py` & `rocketgram-5.0.1/rocketgram/api/encrypted_credentials.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/encrypted_passport_element.py` & `rocketgram-5.0.1/rocketgram/api/encrypted_passport_element.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/encrypted_passport_element_type.py` & `rocketgram-5.0.1/rocketgram/api/encrypted_passport_element_type.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/entity_type.py` & `rocketgram-5.0.1/rocketgram/api/entity_type.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/export_chat_invite_link.py` & `rocketgram-5.0.1/rocketgram/api/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/file.py` & `rocketgram-5.0.1/rocketgram/api/file.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/forum_topic.py` & `rocketgram-5.0.1/rocketgram/api/forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/forum_topic_closed.py` & `rocketgram-5.0.1/rocketgram/api/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/forum_topic_created.py` & `rocketgram-5.0.1/rocketgram/api/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/forum_topic_edited.py` & `rocketgram-5.0.1/rocketgram/api/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/forum_topic_reopened.py` & `rocketgram-5.0.1/rocketgram/api/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/forward_message.py` & `rocketgram-5.0.1/rocketgram/api/forward_message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/game.py` & `rocketgram-5.0.1/rocketgram/api/game.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/game_high_score.py` & `rocketgram-5.0.1/rocketgram/api/game_high_score.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/general_forum_topic_hidden.py` & `rocketgram-5.0.1/rocketgram/api/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/general_forum_topic_unhidden.py` & `rocketgram-5.0.1/rocketgram/api/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_chat.py` & `rocketgram-5.0.1/rocketgram/api/get_chat.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_chat_administrators.py` & `rocketgram-5.0.1/rocketgram/api/get_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_chat_member.py` & `rocketgram-5.0.1/rocketgram/api/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_chat_member_count.py` & `rocketgram-5.0.1/rocketgram/api/get_chat_member_count.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_chat_menu_button.py` & `rocketgram-5.0.1/rocketgram/api/get_chat_menu_button.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 @dataclass(frozen=True)
 class GetChatMenuButton(Request):
     """\
     Represents GetChatMenuButton request object:
     https://core.telegram.org/bots/api#getchatmenubutton
     """
 
-    chat_id: Optional[Union[int, str]]
+    chat_id: Optional[Union[int, str]] = None
 
     def parse_result(self, data) -> Union[MenuButtonCommands, MenuButtonDefault, MenuButtonWebApp]:
         assert isinstance(data, dict), "Should be dict."
 
         result_type = data['type']
 
         if result_type == MenuButtonCommands.type:
```

### Comparing `rocketgram-5.0.0/rocketgram/api/get_custom_emoji_stickers.py` & `rocketgram-5.0.1/rocketgram/api/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_forum_topic_icon_stickers.py` & `rocketgram-5.0.1/rocketgram/api/get_forum_topic_icon_stickers.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_game_high_scores.py` & `rocketgram-5.0.1/rocketgram/api/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_me.py` & `rocketgram-5.0.1/rocketgram/api/get_me.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_my_commands.py` & `rocketgram-5.0.1/rocketgram/api/get_my_commands.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 @dataclass(frozen=True)
 class GetMyCommands(Request):
     """\
     Represents GetMyCommands request object:
     https://core.telegram.org/bots/api#getmycommands
     """
 
-    scope: Optional[BotCommandScope]
-    language_code: Optional[str]
+    scope: Optional[BotCommandScope] = None
+    language_code: Optional[str] = None
 
     def parse_result(self, data) -> List['api.BotCommand']:
         assert isinstance(data, list), "Should be list."
         return [api.BotCommand.parse(r) for r in data]
 
     async def send(self) -> List['api.BotCommand']:
         res = await context.bot.send(self)
```

### Comparing `rocketgram-5.0.0/rocketgram/api/get_my_default_administrator_rights.py` & `rocketgram-5.0.1/rocketgram/api/get_my_default_administrator_rights.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_my_description.py` & `rocketgram-5.0.1/rocketgram/api/get_my_description.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_my_short_description.py` & `rocketgram-5.0.1/rocketgram/api/get_my_short_description.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_sticker_set.py` & `rocketgram-5.0.1/rocketgram/api/get_sticker_set.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_updates.py` & `rocketgram-5.0.1/rocketgram/api/get_updates.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_user_profile_photos.py` & `rocketgram-5.0.1/rocketgram/api/get_user_profile_photos.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/get_webhook_info.py` & `rocketgram-5.0.1/rocketgram/api/get_webhook_info.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/hide_general_forum_topic.py` & `rocketgram-5.0.1/rocketgram/api/hide_general_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_keyboard_button.py` & `rocketgram-5.0.1/rocketgram/api/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_keyboard_markup.py` & `rocketgram-5.0.1/rocketgram/api/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query.py` & `rocketgram-5.0.1/rocketgram/api/inline_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_article.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_audio.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_audio.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_document.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_gif.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_gif.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_mpeg4_gif.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_mpeg4_gif.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_photo.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_sticker.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_video.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_cached_voice.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_contact.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_document.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_game.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_game.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_gif.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_gif.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_location.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_mpeg4_gif.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_mpeg4_gif.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_photo.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_venue.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_video.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/inline_query_result_voice.py` & `rocketgram-5.0.1/rocketgram/api/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/input_contact_message_content.py` & `rocketgram-5.0.1/rocketgram/api/input_contact_message_content.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/input_file.py` & `rocketgram-5.0.1/rocketgram/api/input_file.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/input_invoice_message_content.py` & `rocketgram-5.0.1/rocketgram/api/input_invoice_message_content.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/input_location_message_content.py` & `rocketgram-5.0.1/rocketgram/api/input_location_message_content.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/input_media_animation.py` & `rocketgram-5.0.1/rocketgram/api/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/input_media_audio.py` & `rocketgram-5.0.1/rocketgram/api/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/input_media_document.py` & `rocketgram-5.0.1/rocketgram/api/input_media_document.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/input_media_photo.py` & `rocketgram-5.0.1/rocketgram/api/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/input_media_video.py` & `rocketgram-5.0.1/rocketgram/api/input_media_video.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/input_sticker.py` & `rocketgram-5.0.1/rocketgram/api/input_sticker.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/input_text_message_content.py` & `rocketgram-5.0.1/rocketgram/api/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/input_venue_message_content.py` & `rocketgram-5.0.1/rocketgram/api/input_venue_message_content.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/invoice.py` & `rocketgram-5.0.1/rocketgram/api/invoice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/keyboard_button.py` & `rocketgram-5.0.1/rocketgram/api/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/keyboard_button_request_chat.py` & `rocketgram-5.0.1/rocketgram/api/keyboard_button_request_chat.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/keyboard_button_request_user.py` & `rocketgram-5.0.1/rocketgram/api/keyboard_button_request_user.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/location.py` & `rocketgram-5.0.1/rocketgram/api/location.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/login_url.py` & `rocketgram-5.0.1/rocketgram/api/login_url.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/mask_position.py` & `rocketgram-5.0.1/rocketgram/api/mask_position.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/menu_button_web_app.py` & `rocketgram-5.0.1/rocketgram/api/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/message.py` & `rocketgram-5.0.1/rocketgram/api/message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/message_auto_delete_timer_changed.py` & `rocketgram-5.0.1/rocketgram/api/message_auto_delete_timer_changed.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/message_entity.py` & `rocketgram-5.0.1/rocketgram/api/message_entity.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/message_id.py` & `rocketgram-5.0.1/rocketgram/api/message_id.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/message_type.py` & `rocketgram-5.0.1/rocketgram/api/message_type.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/order_info.py` & `rocketgram-5.0.1/rocketgram/api/order_info.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/passport_data.py` & `rocketgram-5.0.1/rocketgram/api/passport_data.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/passport_element_error_data_field.py` & `rocketgram-5.0.1/rocketgram/api/passport_element_error_data_field.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/passport_element_error_file.py` & `rocketgram-5.0.1/rocketgram/api/passport_element_error_file.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/passport_element_error_files.py` & `rocketgram-5.0.1/rocketgram/api/passport_element_error_files.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/passport_element_error_front_side.py` & `rocketgram-5.0.1/rocketgram/api/passport_element_error_front_side.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/passport_element_error_reverse_side.py` & `rocketgram-5.0.1/rocketgram/api/passport_element_error_reverse_side.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/passport_element_error_selfie.py` & `rocketgram-5.0.1/rocketgram/api/passport_element_error_selfie.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/passport_element_error_translation_file.py` & `rocketgram-5.0.1/rocketgram/api/passport_element_error_translation_file.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/passport_element_error_translation_files.py` & `rocketgram-5.0.1/rocketgram/api/passport_element_error_translation_files.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/passport_element_error_unspecified.py` & `rocketgram-5.0.1/rocketgram/api/passport_element_error_unspecified.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/password_file.py` & `rocketgram-5.0.1/rocketgram/api/password_file.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/photo_size.py` & `rocketgram-5.0.1/rocketgram/api/photo_size.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/pin_chat_message.py` & `rocketgram-5.0.1/rocketgram/api/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/poll.py` & `rocketgram-5.0.1/rocketgram/api/poll.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/poll_answer.py` & `rocketgram-5.0.1/rocketgram/api/poll_answer.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/poll_option.py` & `rocketgram-5.0.1/rocketgram/api/poll_option.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/pre_checkout_query.py` & `rocketgram-5.0.1/rocketgram/api/pre_checkout_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/promote_chat_member.py` & `rocketgram-5.0.1/rocketgram/api/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/proximity_alert_triggered.py` & `rocketgram-5.0.1/rocketgram/api/proximity_alert_triggered.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/reopen_forum_topic.py` & `rocketgram-5.0.1/rocketgram/api/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/reopen_general_forum_topic.py` & `rocketgram-5.0.1/rocketgram/api/reopen_general_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/reply_keyboard_markup.py` & `rocketgram-5.0.1/rocketgram/api/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/request.py` & `rocketgram-5.0.1/rocketgram/api/request.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/response.py` & `rocketgram-5.0.1/rocketgram/api/response.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/response_parameters.py` & `rocketgram-5.0.1/rocketgram/api/response_parameters.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/restrict_chat_member.py` & `rocketgram-5.0.1/rocketgram/api/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/revoke_chat_invite_link.py` & `rocketgram-5.0.1/rocketgram/api/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_animation.py` & `rocketgram-5.0.1/rocketgram/api/send_animation.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_audio.py` & `rocketgram-5.0.1/rocketgram/api/send_audio.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_chat_action.py` & `rocketgram-5.0.1/rocketgram/api/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_contact.py` & `rocketgram-5.0.1/rocketgram/api/send_contact.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_dice.py` & `rocketgram-5.0.1/rocketgram/api/send_dice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_document.py` & `rocketgram-5.0.1/rocketgram/api/send_document.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_game.py` & `rocketgram-5.0.1/rocketgram/api/send_game.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_invoice.py` & `rocketgram-5.0.1/rocketgram/api/send_invoice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_location.py` & `rocketgram-5.0.1/rocketgram/api/send_location.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_media_group.py` & `rocketgram-5.0.1/rocketgram/api/send_media_group.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_message.py` & `rocketgram-5.0.1/rocketgram/api/send_message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_photo.py` & `rocketgram-5.0.1/rocketgram/api/send_photo.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_poll.py` & `rocketgram-5.0.1/rocketgram/api/send_poll.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_sticker.py` & `rocketgram-5.0.1/rocketgram/api/send_sticker.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_venue.py` & `rocketgram-5.0.1/rocketgram/api/send_venue.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_video.py` & `rocketgram-5.0.1/rocketgram/api/send_video.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_video_note.py` & `rocketgram-5.0.1/rocketgram/api/send_video_note.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/send_voice.py` & `rocketgram-5.0.1/rocketgram/api/send_voice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/sent_web_app_message.py` & `rocketgram-5.0.1/rocketgram/api/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/set_chat_administrator_custom_title.py` & `rocketgram-5.0.1/rocketgram/api/set_chat_administrator_custom_title.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/set_chat_description.py` & `rocketgram-5.0.1/rocketgram/api/set_my_description.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Copyright (C) 2015-2022 by Vd.
 # This file is part of Rocketgram, the modern Telegram bot framework.
 # Rocketgram is released under the MIT License (see LICENSE).
 
 
 from dataclasses import dataclass
-from typing import Union, Optional
+from typing import Optional
 
 from .request import Request
 from .utils import BoolResultMixin
 
 
 @dataclass(frozen=True)
-class SetChatDescription(BoolResultMixin, Request):
+class SetMyDescription(BoolResultMixin, Request):
     """\
-    Represents SetChatDescription request object:
-    https://core.telegram.org/bots/api#setchatdescription
+    Represents SetMyDescription request object:
+    https://core.telegram.org/bots/api#setmydescription
     """
 
-    chat_id: Union[int, str]
-    description: Optional[str]
+    description: Optional[str] = None
+    language_code: Optional[str] = None
```

### Comparing `rocketgram-5.0.0/rocketgram/api/set_chat_menu_button.py` & `rocketgram-5.0.1/rocketgram/api/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/set_chat_permissions.py` & `rocketgram-5.0.1/rocketgram/api/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/set_chat_photo.py` & `rocketgram-5.0.1/rocketgram/api/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/set_chat_sticker_set.py` & `rocketgram-5.0.1/rocketgram/api/set_chat_sticker_set.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/set_chat_title.py` & `rocketgram-5.0.1/rocketgram/api/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/set_custom_emoji_sticker_set_thumbnail.py` & `rocketgram-5.0.1/rocketgram/api/set_custom_emoji_sticker_set_thumbnail.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/set_game_score.py` & `rocketgram-5.0.1/rocketgram/api/set_game_score.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/set_my_default_administrator_rights.py` & `rocketgram-5.0.1/rocketgram/api/set_my_default_administrator_rights.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/set_my_description.py` & `rocketgram-5.0.1/rocketgram/api/set_my_short_description.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Optional
 
 from .request import Request
 from .utils import BoolResultMixin
 
 
 @dataclass(frozen=True)
-class SetMyDescription(BoolResultMixin, Request):
+class SetMyShortDescription(BoolResultMixin, Request):
     """\
-    Represents SetMyDescription request object:
-    https://core.telegram.org/bots/api#setmydescription
+    Represents SetMyShortDescription request object:
+    https://core.telegram.org/bots/api#setmyshortdescription
     """
 
-    description: Optional[str]
+    short_description: Optional[str] = None
     language_code: Optional[str] = None
```

### Comparing `rocketgram-5.0.0/rocketgram/api/set_my_short_description.py` & `rocketgram-5.0.1/rocketgram/api/set_sticker_emoji_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Copyright (C) 2015-2022 by Vd.
 # This file is part of Rocketgram, the modern Telegram bot framework.
 # Rocketgram is released under the MIT License (see LICENSE).
 
 
 from dataclasses import dataclass
-from typing import Optional
+from typing import List
 
 from .request import Request
 from .utils import BoolResultMixin
 
 
 @dataclass(frozen=True)
-class SetMyShortDescription(BoolResultMixin, Request):
+class SetStickerEmojiList(BoolResultMixin, Request):
     """\
-    Represents SetMyShortDescription request object:
-    https://core.telegram.org/bots/api#setmyshortdescription
+    Represents SetStickerEmojiList request object:
+    https://core.telegram.org/bots/api#setstickeremojilist
     """
 
-    short_description: Optional[str] = None
-    language_code: Optional[str] = None
+    name: str
+    emoji_list: List[str]
```

### Comparing `rocketgram-5.0.0/rocketgram/api/set_passport_data_errors.py` & `rocketgram-5.0.1/rocketgram/api/set_passport_data_errors.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/set_sticker_emoji_list.py` & `rocketgram-5.0.1/rocketgram/api/set_sticker_keywords.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Copyright (C) 2015-2022 by Vd.
 # This file is part of Rocketgram, the modern Telegram bot framework.
 # Rocketgram is released under the MIT License (see LICENSE).
 
 
 from dataclasses import dataclass
-from typing import List
+from typing import List, Optional
 
 from .request import Request
 from .utils import BoolResultMixin
 
 
 @dataclass(frozen=True)
-class SetStickerEmojiList(BoolResultMixin, Request):
+class SetStickerKeywords(BoolResultMixin, Request):
     """\
-    Represents SetStickerEmojiList request object:
-    https://core.telegram.org/bots/api#setstickeremojilist
+    Represents SetStickerKeywords request object:
+    https://core.telegram.org/bots/api#setstickerkeywords
     """
 
     name: str
-    emoji_list: List[str]
+    keywords: Optional[List[str]] = None
```

### Comparing `rocketgram-5.0.0/rocketgram/api/set_sticker_keywords.py` & `rocketgram-5.0.1/rocketgram/api/set_sticker_mask_position.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Copyright (C) 2015-2022 by Vd.
 # This file is part of Rocketgram, the modern Telegram bot framework.
 # Rocketgram is released under the MIT License (see LICENSE).
 
 
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import Optional
 
+from .mask_position import MaskPosition
 from .request import Request
 from .utils import BoolResultMixin
 
 
 @dataclass(frozen=True)
-class SetStickerKeywords(BoolResultMixin, Request):
+class SetStickerMaskPosition(BoolResultMixin, Request):
     """\
-    Represents SetStickerKeywords request object:
-    https://core.telegram.org/bots/api#setstickerkeywords
+    Represents SetStickerMaskPosition request object:
+    https://core.telegram.org/bots/api#setstickermaskposition
     """
 
     name: str
-    keywords: Optional[List[str]] = None
+    mask_position: Optional[MaskPosition] = None
```

### Comparing `rocketgram-5.0.0/rocketgram/api/set_sticker_mask_position.py` & `rocketgram-5.0.1/rocketgram/api/unban_chat_member.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Copyright (C) 2015-2022 by Vd.
 # This file is part of Rocketgram, the modern Telegram bot framework.
 # Rocketgram is released under the MIT License (see LICENSE).
 
 
 from dataclasses import dataclass
-from typing import Optional
+from typing import Union, Optional
 
-from .mask_position import MaskPosition
 from .request import Request
 from .utils import BoolResultMixin
 
 
 @dataclass(frozen=True)
-class SetStickerMaskPosition(BoolResultMixin, Request):
+class UnbanChatMember(BoolResultMixin, Request):
     """\
-    Represents SetStickerMaskPosition request object:
-    https://core.telegram.org/bots/api#setstickermaskposition
+    Represents UnbanChatMember request object:
+    https://core.telegram.org/bots/api#unbanchatmember
     """
 
-    name: str
-    mask_position: Optional[MaskPosition] = None
+    chat_id: Union[int, str]
+    user_id: int
+    only_if_banned: Optional[bool] = None
```

### Comparing `rocketgram-5.0.0/rocketgram/api/set_sticker_position_in_set.py` & `rocketgram-5.0.1/rocketgram/api/set_sticker_position_in_set.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/set_sticker_set_thumbnail.py` & `rocketgram-5.0.1/rocketgram/api/set_sticker_set_thumbnail.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/set_webhook.py` & `rocketgram-5.0.1/rocketgram/api/set_webhook.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/shipping_address.py` & `rocketgram-5.0.1/rocketgram/api/shipping_address.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/shipping_query.py` & `rocketgram-5.0.1/rocketgram/api/shipping_query.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/sticker.py` & `rocketgram-5.0.1/rocketgram/api/sticker.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/sticker_set.py` & `rocketgram-5.0.1/rocketgram/api/sticker_set.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/stop_message_live_location.py` & `rocketgram-5.0.1/rocketgram/api/stop_message_live_location.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/stop_poll.py` & `rocketgram-5.0.1/rocketgram/api/stop_poll.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/successful_payment.py` & `rocketgram-5.0.1/rocketgram/api/successful_payment.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/unban_chat_member.py` & `rocketgram-5.0.1/rocketgram/api/user_shared.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # Copyright (C) 2015-2022 by Vd.
 # This file is part of Rocketgram, the modern Telegram bot framework.
 # Rocketgram is released under the MIT License (see LICENSE).
 
 
 from dataclasses import dataclass
-from typing import Union, Optional
-
-from .request import Request
-from .utils import BoolResultMixin
+from typing import Optional
 
 
 @dataclass(frozen=True)
-class UnbanChatMember(BoolResultMixin, Request):
+class UserShared:
     """\
-    Represents UnbanChatMember request object:
-    https://core.telegram.org/bots/api#unbanchatmember
+    Represents UserShared object:
+    https://core.telegram.org/bots/api#usershared
     """
 
-    chat_id: Union[int, str]
+    request_id: int
     user_id: int
-    only_if_banned: Optional[bool]
+
+    @classmethod
+    def parse(cls, data: dict) -> Optional['UserShared']:
+        if data is None:
+            return None
+
+        return cls(data['request_id'], data['user_id'])
```

### Comparing `rocketgram-5.0.0/rocketgram/api/unban_chat_sender_chat.py` & `rocketgram-5.0.1/rocketgram/api/unban_chat_sender_chat.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/unhide_general_forum_topic.py` & `rocketgram-5.0.1/rocketgram/api/unhide_general_forum_topic.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/unpin_all_chat_messages.py` & `rocketgram-5.0.1/rocketgram/api/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/unpin_all_forum_topic_messages.py` & `rocketgram-5.0.1/rocketgram/api/unpin_all_forum_topic_messages.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/unpin_chat_message.py` & `rocketgram-5.0.1/rocketgram/api/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/update.py` & `rocketgram-5.0.1/rocketgram/api/update.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/update_type.py` & `rocketgram-5.0.1/rocketgram/api/update_type.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/upload_sticker_file.py` & `rocketgram-5.0.1/rocketgram/api/upload_sticker_file.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/user.py` & `rocketgram-5.0.1/rocketgram/api/user.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/user_profile_photos.py` & `rocketgram-5.0.1/rocketgram/api/user_profile_photos.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/user_shared.py` & `rocketgram-5.0.1/rocketgram/api/video_chat_participants_invited.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Copyright (C) 2015-2022 by Vd.
 # This file is part of Rocketgram, the modern Telegram bot framework.
 # Rocketgram is released under the MIT License (see LICENSE).
 
 
 from dataclasses import dataclass
-from typing import Optional
+from typing import Dict, Optional, List
+
+from . import user
 
 
 @dataclass(frozen=True)
-class UserShared:
+class VideoChatParticipantsInvited:
     """\
-    Represents UserShared object:
-    https://core.telegram.org/bots/api#usershared
+    Represents VideoChatParticipantsInvited object:
+    https://core.telegram.org/bots/api#voicechatparticipantsinvited
     """
 
-    request_id: int
-    user_id: int
+    users: List['user.User']
 
     @classmethod
-    def parse(cls, data: dict) -> Optional['UserShared']:
+    def parse(cls, data: Optional[Dict]) -> Optional['VideoChatParticipantsInvited']:
         if data is None:
             return None
 
-        return cls(data['request_id'], data['user_id'])
+        return cls([user.User.parse(u) for u in data['users']])
```

### Comparing `rocketgram-5.0.0/rocketgram/api/utils.py` & `rocketgram-5.0.1/rocketgram/api/utils.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/venue.py` & `rocketgram-5.0.1/rocketgram/api/venue.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/video.py` & `rocketgram-5.0.1/rocketgram/api/video.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/video_chat_ended.py` & `rocketgram-5.0.1/rocketgram/api/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/video_chat_participants_invited.py` & `rocketgram-5.0.1/rocketgram/api/write_access_allowed.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 # Copyright (C) 2015-2022 by Vd.
 # This file is part of Rocketgram, the modern Telegram bot framework.
 # Rocketgram is released under the MIT License (see LICENSE).
 
 
 from dataclasses import dataclass
-from typing import Dict, Optional, List
-
-from . import user
+from typing import Optional
 
 
 @dataclass(frozen=True)
-class VideoChatParticipantsInvited:
+class WriteAccessAllowed:
     """\
-    Represents VideoChatParticipantsInvited object:
-    https://core.telegram.org/bots/api#voicechatparticipantsinvited
+    Represents WriteAccessAllowed object:
+    https://core.telegram.org/bots/api#writeaccessallowed
     """
 
-    users: List['user.User']
-
     @classmethod
-    def parse(cls, data: Optional[Dict]) -> Optional['VideoChatParticipantsInvited']:
+    def parse(cls, data: dict) -> Optional['WriteAccessAllowed']:
         if data is None:
             return None
 
-        return cls([user.User.parse(u) for u in data['users']])
+        return cls()
```

### Comparing `rocketgram-5.0.0/rocketgram/api/video_chat_scheduled.py` & `rocketgram-5.0.1/rocketgram/api/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/video_chat_started.py` & `rocketgram-5.0.1/rocketgram/api/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/video_note.py` & `rocketgram-5.0.1/rocketgram/api/video_note.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/voice.py` & `rocketgram-5.0.1/rocketgram/api/voice.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/web_app_data.py` & `rocketgram-5.0.1/rocketgram/api/web_app_data.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/web_app_info.py` & `rocketgram-5.0.1/rocketgram/api/web_app_info.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/api/webhook_info.py` & `rocketgram-5.0.1/rocketgram/api/webhook_info.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/bot.py` & `rocketgram-5.0.1/rocketgram/bot.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/connectors/aiohttp.py` & `rocketgram-5.0.1/rocketgram/connectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/connectors/connector.py` & `rocketgram-5.0.1/rocketgram/connectors/connector.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/context.py` & `rocketgram-5.0.1/rocketgram/context.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/errors.py` & `rocketgram-5.0.1/rocketgram/errors.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/executors/aiohttp.py` & `rocketgram-5.0.1/rocketgram/executors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/executors/executor.py` & `rocketgram-5.0.1/rocketgram/executors/executor.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/executors/updates.py` & `rocketgram-5.0.1/rocketgram/executors/updates.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/executors/webhook.py` & `rocketgram-5.0.1/rocketgram/executors/webhook.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/json_adapters/__init__.py` & `rocketgram-5.0.1/rocketgram/json_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/keyboards/inline.py` & `rocketgram-5.0.1/rocketgram/keyboards/inline.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/keyboards/keyboard.py` & `rocketgram-5.0.1/rocketgram/keyboards/keyboard.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/keyboards/reply.py` & `rocketgram-5.0.1/rocketgram/keyboards/reply.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/middlewares/defaultvalues.py` & `rocketgram-5.0.1/rocketgram/middlewares/defaultvalues.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/middlewares/limiter.py` & `rocketgram-5.0.1/rocketgram/middlewares/limiter.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/middlewares/middleware.py` & `rocketgram-5.0.1/rocketgram/middlewares/middleware.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/routers/dispatcher/base.py` & `rocketgram-5.0.1/rocketgram/routers/dispatcher/base.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/routers/dispatcher/commonfilters.py` & `rocketgram-5.0.1/rocketgram/routers/dispatcher/commonfilters.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/routers/dispatcher/commonwaiters.py` & `rocketgram-5.0.1/rocketgram/routers/dispatcher/commonwaiters.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/routers/dispatcher/dispatcher.py` & `rocketgram-5.0.1/rocketgram/routers/dispatcher/dispatcher.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/routers/dispatcher/filters.py` & `rocketgram-5.0.1/rocketgram/routers/dispatcher/filters.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/routers/dispatcher/waiters.py` & `rocketgram-5.0.1/rocketgram/routers/dispatcher/waiters.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/tools/entities.py` & `rocketgram-5.0.1/rocketgram/tools/entities.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram/tools/escape.py` & `rocketgram-5.0.1/rocketgram/tools/escape.py`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/rocketgram.egg-info/PKG-INFO` & `rocketgram-5.0.1/rocketgram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketgram
-Version: 5.0.0
+Version: 5.0.1
 Summary: Modern and powerful asynchronous telegram bot framework.
 Home-page: https://github.com/rocketgram/rocketgram
 Author: Vd
 Author-email: vd@vd2.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rocketgram-5.0.0/rocketgram.egg-info/SOURCES.txt` & `rocketgram-5.0.1/rocketgram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rocketgram-5.0.0/setup.py` & `rocketgram-5.0.1/setup.py`

 * *Files identical despite different names*

