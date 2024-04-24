# Comparing `tmp/rubpy-7.0.1b0.tar.gz` & `tmp/rubpy-7.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-7.0.1b0.tar", last modified: Mon Apr  1 23:53:30 2024, max compression
+gzip compressed data, was "rubpy-7.0.2b0.tar", last modified: Wed Apr 24 22:44:15 2024, max compression
```

## Comparing `rubpy-7.0.1b0.tar` & `rubpy-7.0.2b0.tar`

### file list

```diff
@@ -1,265 +1,264 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.241446 rubpy-7.0.1b0/
--rw-rw-rw-   0        0        0     3723 2024-04-01 23:53:30.240470 rubpy-7.0.1b0/PKG-INFO
--rw-rw-rw-   0        0        0     2472 2024-03-14 02:30:28.000000 rubpy-7.0.1b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:29.720481 rubpy-7.0.1b0/rubpy/
--rw-rw-rw-   0        0        0      490 2024-04-01 23:53:15.000000 rubpy-7.0.1b0/rubpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:29.766376 rubpy-7.0.1b0/rubpy/bots/
--rw-rw-rw-   0        0        0        0 2024-01-08 21:58:47.000000 rubpy-7.0.1b0/rubpy/bots/__init__.py
--rw-rw-rw-   0        0        0    11161 2024-01-08 22:59:16.000000 rubpy-7.0.1b0/rubpy/bots/client.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:29.987020 rubpy-7.0.1b0/rubpy/bots/types/
--rw-rw-rw-   0        0        0     1077 2024-01-08 22:47:11.000000 rubpy-7.0.1b0/rubpy/bots/types/__init__.py
--rw-rw-rw-   0        0        0      163 2024-01-08 22:26:46.000000 rubpy-7.0.1b0/rubpy/bots/types/aux_data.py
--rw-rw-rw-   0        0        0      255 2024-01-08 22:11:16.000000 rubpy-7.0.1b0/rubpy/bots/types/bot.py
--rw-rw-rw-   0        0        0      102 2024-01-08 22:11:52.000000 rubpy-7.0.1b0/rubpy/bots/types/bot_command.py
--rw-rw-rw-   0        0        0     1093 2024-01-08 22:29:20.000000 rubpy-7.0.1b0/rubpy/bots/types/button.py
--rw-rw-rw-   0        0        0      225 2024-01-08 22:20:24.000000 rubpy-7.0.1b0/rubpy/bots/types/button_calendar.py
--rw-rw-rw-   0        0        0      286 2024-01-08 22:25:55.000000 rubpy-7.0.1b0/rubpy/bots/types/button_location.py
--rw-rw-rw-   0        0        0      191 2024-01-08 22:21:11.000000 rubpy-7.0.1b0/rubpy/bots/types/button_number_picker.py
--rw-rw-rw-   0        0        0      377 2024-01-08 22:19:28.000000 rubpy-7.0.1b0/rubpy/bots/types/button_selection.py
--rw-rw-rw-   0        0        0      195 2024-01-08 22:18:19.000000 rubpy-7.0.1b0/rubpy/bots/types/button_selection_item.py
--rw-rw-rw-   0        0        0      159 2024-01-08 22:22:12.000000 rubpy-7.0.1b0/rubpy/bots/types/button_string_picker.py
--rw-rw-rw-   0        0        0      255 2024-01-08 22:24:13.000000 rubpy-7.0.1b0/rubpy/bots/types/button_textbox.py
--rw-rw-rw-   0        0        0      257 2024-01-08 22:02:54.000000 rubpy-7.0.1b0/rubpy/bots/types/chat.py
--rw-rw-rw-   0        0        0      132 2024-01-08 22:13:08.000000 rubpy-7.0.1b0/rubpy/bots/types/contact_message.py
--rw-rw-rw-   0        0        0      111 2024-01-08 22:02:20.000000 rubpy-7.0.1b0/rubpy/bots/types/file.py
--rw-rw-rw-   0        0        0      214 2024-01-08 22:03:18.000000 rubpy-7.0.1b0/rubpy/bots/types/forwarded_from.py
--rw-rw-rw-   0        0        0      340 2024-01-08 22:36:23.000000 rubpy-7.0.1b0/rubpy/bots/types/inline_message.py
--rw-rw-rw-   0        0        0      232 2024-01-08 22:30:58.000000 rubpy-7.0.1b0/rubpy/bots/types/keypad.py
--rw-rw-rw-   0        0        0      141 2024-01-08 22:30:09.000000 rubpy-7.0.1b0/rubpy/bots/types/keypad_row.py
--rw-rw-rw-   0        0        0      340 2024-01-08 22:17:29.000000 rubpy-7.0.1b0/rubpy/bots/types/live_location.py
--rw-rw-rw-   0        0        0       99 2024-01-08 22:15:36.000000 rubpy-7.0.1b0/rubpy/bots/types/location.py
--rw-rw-rw-   0        0        0      107 2024-01-08 22:09:39.000000 rubpy-7.0.1b0/rubpy/bots/types/messaage_text_update.py
--rw-rw-rw-   0        0        0      887 2024-01-08 22:34:09.000000 rubpy-7.0.1b0/rubpy/bots/types/message.py
--rw-rw-rw-   0        0        0      149 2024-01-08 22:31:58.000000 rubpy-7.0.1b0/rubpy/bots/types/message_keypad_update.py
--rw-rw-rw-   0        0        0      156 2024-01-08 22:03:44.000000 rubpy-7.0.1b0/rubpy/bots/types/payment_status.py
--rw-rw-rw-   0        0        0      192 2024-01-08 22:14:43.000000 rubpy-7.0.1b0/rubpy/bots/types/poll.py
--rw-rw-rw-   0        0        0      248 2024-01-08 22:13:58.000000 rubpy-7.0.1b0/rubpy/bots/types/poll_status.py
--rw-rw-rw-   0        0        0      148 2024-01-08 22:12:28.000000 rubpy-7.0.1b0/rubpy/bots/types/sticker.py
--rw-rw-rw-   0        0        0      455 2024-01-08 22:35:18.000000 rubpy-7.0.1b0/rubpy/bots/types/update.py
--rw-rw-rw-   0        0        0     5768 2024-03-14 02:20:07.000000 rubpy-7.0.1b0/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:29.989947 rubpy-7.0.1b0/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-7.0.1b0/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     5386 2024-02-19 23:09:00.000000 rubpy-7.0.1b0/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.041241 rubpy-7.0.1b0/rubpy/enums/
--rw-rw-rw-   0        0        0      302 2024-02-15 11:07:37.000000 rubpy-7.0.1b0/rubpy/enums/__init__.py
--rw-rw-rw-   0        0        0      633 2024-02-03 10:53:26.000000 rubpy-7.0.1b0/rubpy/enums/chat_access_type.py
--rw-rw-rw-   0        0        0      214 2024-02-03 10:54:38.000000 rubpy-7.0.1b0/rubpy/enums/chat_action.py
--rw-rw-rw-   0        0        0      370 2024-01-11 13:02:06.000000 rubpy-7.0.1b0/rubpy/enums/chat_type.py
--rw-rw-rw-   0        0        0      496 2024-01-11 13:05:56.000000 rubpy-7.0.1b0/rubpy/enums/message_media_type.py
--rw-rw-rw-   0        0        0      100 2024-02-10 16:11:46.000000 rubpy-7.0.1b0/rubpy/enums/parse_mode.py
--rw-rw-rw-   0        0        0      133 2024-01-11 13:07:44.000000 rubpy-7.0.1b0/rubpy/enums/poll_type.py
--rw-rw-rw-   0        0        0     1767 2024-01-16 12:03:08.000000 rubpy-7.0.1b0/rubpy/enums/reaction_type.py
--rw-rw-rw-   0        0        0      192 2024-02-15 11:07:26.000000 rubpy-7.0.1b0/rubpy/enums/report_type.py
--rw-rw-rw-   0        0        0     1942 2024-01-08 22:38:06.000000 rubpy-7.0.1b0/rubpy/exceptions.py
--rw-rw-rw-   0        0        0    15828 2024-03-29 05:15:18.000000 rubpy-7.0.1b0/rubpy/filters.py
--rw-rw-rw-   0        0        0     4886 2024-02-24 22:37:29.000000 rubpy-7.0.1b0/rubpy/handlers.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.042218 rubpy-7.0.1b0/rubpy/methods/
--rw-rw-rw-   0        0        0      697 2024-02-23 15:20:39.000000 rubpy-7.0.1b0/rubpy/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.045147 rubpy-7.0.1b0/rubpy/methods/advanced/
--rw-rw-rw-   0        0        0      143 2024-02-22 17:41:57.000000 rubpy-7.0.1b0/rubpy/methods/advanced/__init__.py
--rw-rw-rw-   0        0        0     2312 2024-03-14 01:56:23.000000 rubpy-7.0.1b0/rubpy/methods/advanced/build.py
--rw-rw-rw-   0        0        0     4483 2024-02-25 17:08:53.000000 rubpy-7.0.1b0/rubpy/methods/advanced/voice_chat_player.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.048073 rubpy-7.0.1b0/rubpy/methods/auth/
--rw-rw-rw-   0        0        0      185 2023-12-15 18:54:26.000000 rubpy-7.0.1b0/rubpy/methods/auth/__init__.py
--rw-rw-rw-   0        0        0     2007 2024-03-09 18:53:42.000000 rubpy-7.0.1b0/rubpy/methods/auth/register_device.py
--rw-rw-rw-   0        0        0      798 2024-02-24 22:49:22.000000 rubpy-7.0.1b0/rubpy/methods/auth/send_code.py
--rw-rw-rw-   0        0        0      576 2024-02-24 22:51:51.000000 rubpy-7.0.1b0/rubpy/methods/auth/sign_in.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.067593 rubpy-7.0.1b0/rubpy/methods/channels/
--rw-rw-rw-   0        0        0     1826 2024-01-22 20:05:38.000000 rubpy-7.0.1b0/rubpy/methods/channels/__init__.py
--rw-rw-rw-   0        0        0     1042 2024-02-24 22:53:48.000000 rubpy-7.0.1b0/rubpy/methods/channels/add_channel.py
--rw-rw-rw-   0        0        0      882 2024-02-24 22:53:29.000000 rubpy-7.0.1b0/rubpy/methods/channels/add_channel_members.py
--rw-rw-rw-   0        0        0     1065 2024-02-24 22:54:12.000000 rubpy-7.0.1b0/rubpy/methods/channels/ban_channel_member.py
--rw-rw-rw-   0        0        0      613 2024-02-24 22:54:34.000000 rubpy-7.0.1b0/rubpy/methods/channels/channel_preview_by_join_link.py
--rw-rw-rw-   0        0        0      574 2024-02-24 22:54:51.000000 rubpy-7.0.1b0/rubpy/methods/channels/check_channel_username.py
--rw-rw-rw-   0        0        0      523 2024-02-24 22:55:07.000000 rubpy-7.0.1b0/rubpy/methods/channels/create_channel_voice_chat.py
--rw-rw-rw-   0        0        0      748 2024-02-24 22:55:21.000000 rubpy-7.0.1b0/rubpy/methods/channels/discard_channel_voice_chat.py
--rw-rw-rw-   0        0        0     2601 2024-02-24 22:55:49.000000 rubpy-7.0.1b0/rubpy/methods/channels/edit_channel_info.py
--rw-rw-rw-   0        0        0      705 2024-02-24 22:56:18.000000 rubpy-7.0.1b0/rubpy/methods/channels/get_banned_group_members.py
--rw-rw-rw-   0        0        0      681 2024-02-24 22:56:34.000000 rubpy-7.0.1b0/rubpy/methods/channels/get_channel_admin_access_list.py
--rw-rw-rw-   0        0        0      681 2024-02-24 22:56:52.000000 rubpy-7.0.1b0/rubpy/methods/channels/get_channel_admin_members.py
--rw-rw-rw-   0        0        0      819 2024-02-24 22:58:08.000000 rubpy-7.0.1b0/rubpy/methods/channels/get_channel_all_members.py
--rw-rw-rw-   0        0        0      504 2024-02-24 22:58:25.000000 rubpy-7.0.1b0/rubpy/methods/channels/get_channel_info.py
--rw-rw-rw-   0        0        0      503 2024-02-24 22:58:39.000000 rubpy-7.0.1b0/rubpy/methods/channels/get_channel_link.py
--rw-rw-rw-   0        0        0      996 2024-02-24 22:58:58.000000 rubpy-7.0.1b0/rubpy/methods/channels/join_channel_action.py
--rw-rw-rw-   0        0        0      609 2024-02-24 22:59:21.000000 rubpy-7.0.1b0/rubpy/methods/channels/join_channel_by_link.py
--rw-rw-rw-   0        0        0      610 2024-02-24 22:59:38.000000 rubpy-7.0.1b0/rubpy/methods/channels/remove_channel.py
--rw-rw-rw-   0        0        0      956 2024-02-24 23:00:34.000000 rubpy-7.0.1b0/rubpy/methods/channels/seen_channel_messages.py
--rw-rw-rw-   0        0        0      631 2024-02-24 23:00:59.000000 rubpy-7.0.1b0/rubpy/methods/channels/set_channel_link.py
--rw-rw-rw-   0        0        0     1051 2024-02-24 23:01:17.000000 rubpy-7.0.1b0/rubpy/methods/channels/set_channel_voice_chat_setting.py
--rw-rw-rw-   0        0        0      772 2024-02-24 23:01:35.000000 rubpy-7.0.1b0/rubpy/methods/channels/update_channel_username.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.080281 rubpy-7.0.1b0/rubpy/methods/chats/
--rw-rw-rw-   0        0        0      807 2023-12-20 14:35:52.000000 rubpy-7.0.1b0/rubpy/methods/chats/__init__.py
--rw-rw-rw-   0        0        0      806 2024-02-24 23:02:06.000000 rubpy-7.0.1b0/rubpy/methods/chats/delete_avatar.py
--rw-rw-rw-   0        0        0      966 2024-02-24 23:02:35.000000 rubpy-7.0.1b0/rubpy/methods/chats/delete_chat_history.py
--rw-rw-rw-   0        0        0      790 2024-02-24 23:02:59.000000 rubpy-7.0.1b0/rubpy/methods/chats/get_abs_objects.py
--rw-rw-rw-   0        0        0      636 2024-02-24 23:03:23.000000 rubpy-7.0.1b0/rubpy/methods/chats/get_avatars.py
--rw-rw-rw-   0        0        0      601 2024-02-24 23:05:28.000000 rubpy-7.0.1b0/rubpy/methods/chats/get_chats.py
--rw-rw-rw-   0        0        0      745 2024-02-24 23:04:22.000000 rubpy-7.0.1b0/rubpy/methods/chats/get_chats_updates.py
--rw-rw-rw-   0        0        0      599 2024-02-24 23:08:10.000000 rubpy-7.0.1b0/rubpy/methods/chats/get_link_from_app_url.py
--rw-rw-rw-   0        0        0     1265 2024-02-24 23:08:43.000000 rubpy-7.0.1b0/rubpy/methods/chats/search_chat_messages.py
--rw-rw-rw-   0        0        0      611 2024-02-24 23:10:47.000000 rubpy-7.0.1b0/rubpy/methods/chats/seen_chats.py
--rw-rw-rw-   0        0        0     1110 2024-02-24 23:11:34.000000 rubpy-7.0.1b0/rubpy/methods/chats/send_chat_activity.py
--rw-rw-rw-   0        0        0     1014 2024-02-24 23:12:16.000000 rubpy-7.0.1b0/rubpy/methods/chats/set_action_chat.py
--rw-rw-rw-   0        0        0     1818 2024-02-24 23:13:42.000000 rubpy-7.0.1b0/rubpy/methods/chats/upload_avatar.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.083210 rubpy-7.0.1b0/rubpy/methods/contacts/
--rw-rw-rw-   0        0        0      299 2023-12-22 14:16:01.000000 rubpy-7.0.1b0/rubpy/methods/contacts/__init__.py
--rw-rw-rw-   0        0        0     1247 2024-02-24 23:15:53.000000 rubpy-7.0.1b0/rubpy/methods/contacts/add_address_book.py
--rw-rw-rw-   0        0        0      753 2024-02-24 23:16:17.000000 rubpy-7.0.1b0/rubpy/methods/contacts/delete_contact.py
--rw-rw-rw-   0        0        0      622 2024-02-24 23:18:12.000000 rubpy-7.0.1b0/rubpy/methods/contacts/get_contacts.py
--rw-rw-rw-   0        0        0      770 2024-02-24 23:17:44.000000 rubpy-7.0.1b0/rubpy/methods/contacts/get_contacts_updates.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.089065 rubpy-7.0.1b0/rubpy/methods/decorators/
--rw-rw-rw-   0        0        0      415 2023-12-25 13:18:28.000000 rubpy-7.0.1b0/rubpy/methods/decorators/__init__.py
--rw-rw-rw-   0        0        0      592 2024-02-24 23:18:27.000000 rubpy-7.0.1b0/rubpy/methods/decorators/on_chat_updates.py
--rw-rw-rw-   0        0        0      604 2024-02-24 23:18:42.000000 rubpy-7.0.1b0/rubpy/methods/decorators/on_message_updates.py
--rw-rw-rw-   0        0        0      624 2024-02-24 23:18:56.000000 rubpy-7.0.1b0/rubpy/methods/decorators/on_remove_notifications.py
--rw-rw-rw-   0        0        0      604 2024-02-24 23:19:09.000000 rubpy-7.0.1b0/rubpy/methods/decorators/on_show_activities.py
--rw-rw-rw-   0        0        0      616 2024-02-24 23:19:21.000000 rubpy-7.0.1b0/rubpy/methods/decorators/on_show_notifications.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.107613 rubpy-7.0.1b0/rubpy/methods/extras/
--rw-rw-rw-   0        0        0      745 2024-02-15 12:50:33.000000 rubpy-7.0.1b0/rubpy/methods/extras/__init__.py
--rw-rw-rw-   0        0        0      739 2024-02-24 23:19:55.000000 rubpy-7.0.1b0/rubpy/methods/extras/ban_member.py
--rw-rw-rw-   0        0        0     1039 2024-02-24 23:20:10.000000 rubpy-7.0.1b0/rubpy/methods/extras/get_info.py
--rw-rw-rw-   0        0        0      693 2024-02-24 23:20:43.000000 rubpy-7.0.1b0/rubpy/methods/extras/get_object_by_username.py
--rw-rw-rw-   0        0        0      538 2024-02-24 23:21:03.000000 rubpy-7.0.1b0/rubpy/methods/extras/get_profile_link_items.py
--rw-rw-rw-   0        0        0      530 2024-02-24 23:21:19.000000 rubpy-7.0.1b0/rubpy/methods/extras/get_related_objects.py
--rw-rw-rw-   0        0        0      770 2024-02-24 23:22:06.000000 rubpy-7.0.1b0/rubpy/methods/extras/get_transcription.py
--rw-rw-rw-   0        0        0      690 2024-02-24 23:22:29.000000 rubpy-7.0.1b0/rubpy/methods/extras/join.py
--rw-rw-rw-   0        0        0      648 2024-02-24 23:22:49.000000 rubpy-7.0.1b0/rubpy/methods/extras/leave_chat.py
--rw-rw-rw-   0        0        0     1155 2024-02-24 23:23:31.000000 rubpy-7.0.1b0/rubpy/methods/extras/report_object.py
--rw-rw-rw-   0        0        0      665 2024-02-24 23:24:05.000000 rubpy-7.0.1b0/rubpy/methods/extras/search_global_objects.py
--rw-rw-rw-   0        0        0      695 2024-02-24 23:25:58.000000 rubpy-7.0.1b0/rubpy/methods/extras/transcribe_voice.py
--rw-rw-rw-   0        0        0     1019 2024-02-24 23:26:53.000000 rubpy-7.0.1b0/rubpy/methods/extras/user_is_admin.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.110095 rubpy-7.0.1b0/rubpy/methods/gif/
--rw-rw-rw-   0        0        0      235 2024-01-09 12:00:36.000000 rubpy-7.0.1b0/rubpy/methods/gif/__init__.py
--rw-rw-rw-   0        0        0      611 2024-02-24 23:27:54.000000 rubpy-7.0.1b0/rubpy/methods/gif/add_to_my_gif_set.py
--rw-rw-rw-   0        0        0      341 2024-02-24 23:28:10.000000 rubpy-7.0.1b0/rubpy/methods/gif/get_my_gif_set.py
--rw-rw-rw-   0        0        0      430 2024-02-24 23:28:39.000000 rubpy-7.0.1b0/rubpy/methods/gif/remove_from_my_gif_set.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.132547 rubpy-7.0.1b0/rubpy/methods/groups/
--rw-rw-rw-   0        0        0     1857 2023-12-22 17:47:50.000000 rubpy-7.0.1b0/rubpy/methods/groups/__init__.py
--rw-rw-rw-   0        0        0      987 2024-02-24 23:33:24.000000 rubpy-7.0.1b0/rubpy/methods/groups/add_group.py
--rw-rw-rw-   0        0        0      958 2024-02-24 23:29:42.000000 rubpy-7.0.1b0/rubpy/methods/groups/add_group_members.py
--rw-rw-rw-   0        0        0     1229 2024-02-24 23:33:49.000000 rubpy-7.0.1b0/rubpy/methods/groups/ban_group_member.py
--rw-rw-rw-   0        0        0      600 2024-02-24 23:34:06.000000 rubpy-7.0.1b0/rubpy/methods/groups/create_group_voice_chat.py
--rw-rw-rw-   0        0        0      618 2024-02-24 23:34:23.000000 rubpy-7.0.1b0/rubpy/methods/groups/delete_no_access_group_chat.py
--rw-rw-rw-   0        0        0     2648 2024-02-24 23:34:53.000000 rubpy-7.0.1b0/rubpy/methods/groups/edit_group_info.py
--rw-rw-rw-   0        0        0      785 2024-02-24 23:35:11.000000 rubpy-7.0.1b0/rubpy/methods/groups/get_banned_group_members.py
--rw-rw-rw-   0        0        0      820 2024-02-24 23:35:36.000000 rubpy-7.0.1b0/rubpy/methods/groups/get_group_admin_access_list.py
--rw-rw-rw-   0        0        0      791 2024-02-24 23:35:53.000000 rubpy-7.0.1b0/rubpy/methods/groups/get_group_admin_members.py
--rw-rw-rw-   0        0        0     1003 2024-02-25 13:45:13.000000 rubpy-7.0.1b0/rubpy/methods/groups/get_group_all_members.py
--rw-rw-rw-   0        0        0      644 2024-02-24 23:36:57.000000 rubpy-7.0.1b0/rubpy/methods/groups/get_group_default_access.py
--rw-rw-rw-   0        0        0      584 2024-02-24 23:37:09.000000 rubpy-7.0.1b0/rubpy/methods/groups/get_group_info.py
--rw-rw-rw-   0        0        0      578 2024-02-24 23:37:26.000000 rubpy-7.0.1b0/rubpy/methods/groups/get_group_link.py
--rw-rw-rw-   0        0        0      787 2024-02-24 23:37:39.000000 rubpy-7.0.1b0/rubpy/methods/groups/get_group_mention_list.py
--rw-rw-rw-   0        0        0     1096 2024-02-24 23:38:09.000000 rubpy-7.0.1b0/rubpy/methods/groups/get_group_voice_chat_updates.py
--rw-rw-rw-   0        0        0      688 2024-02-24 23:38:23.000000 rubpy-7.0.1b0/rubpy/methods/groups/group_preview_by_join_link.py
--rw-rw-rw-   0        0        0      645 2024-02-24 23:38:40.000000 rubpy-7.0.1b0/rubpy/methods/groups/join_group.py
--rw-rw-rw-   0        0        0      460 2024-02-24 23:39:16.000000 rubpy-7.0.1b0/rubpy/methods/groups/leave_group.py
--rw-rw-rw-   0        0        0      784 2024-02-24 23:38:58.000000 rubpy-7.0.1b0/rubpy/methods/groups/leave_group_voice_chat.py
--rw-rw-rw-   0        0        0      466 2024-02-24 23:39:33.000000 rubpy-7.0.1b0/rubpy/methods/groups/remove_group.py
--rw-rw-rw-   0        0        0     1549 2024-02-24 23:40:14.000000 rubpy-7.0.1b0/rubpy/methods/groups/set_group_admin.py
--rw-rw-rw-   0        0        0      920 2024-02-24 23:42:43.000000 rubpy-7.0.1b0/rubpy/methods/groups/set_group_default_access.py
--rw-rw-rw-   0        0        0      596 2024-02-24 23:45:52.000000 rubpy-7.0.1b0/rubpy/methods/groups/set_group_link.py
--rw-rw-rw-   0        0        0      980 2024-02-24 23:49:50.000000 rubpy-7.0.1b0/rubpy/methods/groups/set_group_voice_chat_setting.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.157922 rubpy-7.0.1b0/rubpy/methods/messages/
--rw-rw-rw-   0        0        0     1808 2024-02-25 13:57:52.000000 rubpy-7.0.1b0/rubpy/methods/messages/__init__.py
--rw-rw-rw-   0        0        0     1431 2024-02-25 13:21:28.000000 rubpy-7.0.1b0/rubpy/methods/messages/action_on_message_reaction.py
--rw-rw-rw-   0        0        0     1148 2024-02-25 13:22:34.000000 rubpy-7.0.1b0/rubpy/methods/messages/auto_delete_message.py
--rw-rw-rw-   0        0        0     2603 2024-02-25 13:23:17.000000 rubpy-7.0.1b0/rubpy/methods/messages/create_poll.py
--rw-rw-rw-   0        0        0     1550 2024-02-25 13:24:10.000000 rubpy-7.0.1b0/rubpy/methods/messages/delete_messages.py
--rw-rw-rw-   0        0        0     1633 2024-02-25 13:25:45.000000 rubpy-7.0.1b0/rubpy/methods/messages/edit_message.py
--rw-rw-rw-   0        0        0     1635 2024-02-25 13:27:51.000000 rubpy-7.0.1b0/rubpy/methods/messages/forward_messages.py
--rw-rw-rw-   0        0        0     1044 2024-03-14 20:52:58.000000 rubpy-7.0.1b0/rubpy/methods/messages/get_message_share_url.py
--rw-rw-rw-   0        0        0     1193 2024-02-25 13:28:35.000000 rubpy-7.0.1b0/rubpy/methods/messages/get_messages_by_id.py
--rw-rw-rw-   0        0        0     1245 2024-02-25 13:28:56.000000 rubpy-7.0.1b0/rubpy/methods/messages/get_messages_interval.py
--rw-rw-rw-   0        0        0     1165 2024-02-25 13:29:20.000000 rubpy-7.0.1b0/rubpy/methods/messages/get_messages_updates.py
--rw-rw-rw-   0        0        0     1250 2024-02-25 13:31:15.000000 rubpy-7.0.1b0/rubpy/methods/messages/get_poll_option_voters.py
--rw-rw-rw-   0        0        0      823 2024-02-25 13:31:35.000000 rubpy-7.0.1b0/rubpy/methods/messages/get_poll_status.py
--rw-rw-rw-   0        0        0     1090 2024-02-25 13:31:55.000000 rubpy-7.0.1b0/rubpy/methods/messages/reaction.py
--rw-rw-rw-   0        0        0     1136 2024-02-25 13:32:18.000000 rubpy-7.0.1b0/rubpy/methods/messages/remove_reaction.py
--rw-rw-rw-   0        0        0     1156 2024-02-25 13:32:38.000000 rubpy-7.0.1b0/rubpy/methods/messages/request_send_file.py
--rw-rw-rw-   0        0        0     1515 2024-02-25 13:32:59.000000 rubpy-7.0.1b0/rubpy/methods/messages/send_document.py
--rw-rw-rw-   0        0        0     1248 2024-02-25 13:35:35.000000 rubpy-7.0.1b0/rubpy/methods/messages/send_gif.py
--rw-rw-rw-   0        0        0     7353 2024-04-01 22:55:47.000000 rubpy-7.0.1b0/rubpy/methods/messages/send_message.py
--rw-rw-rw-   0        0        0     1266 2024-02-25 13:35:46.000000 rubpy-7.0.1b0/rubpy/methods/messages/send_music.py
--rw-rw-rw-   0        0        0     1492 2024-02-25 13:35:55.000000 rubpy-7.0.1b0/rubpy/methods/messages/send_photo.py
--rw-rw-rw-   0        0        0     1785 2024-02-25 13:45:22.000000 rubpy-7.0.1b0/rubpy/methods/messages/send_sticker.py
--rw-rw-rw-   0        0        0     1236 2024-02-25 13:45:25.000000 rubpy-7.0.1b0/rubpy/methods/messages/send_video.py
--rw-rw-rw-   0        0        0     1374 2024-02-25 13:45:23.000000 rubpy-7.0.1b0/rubpy/methods/messages/send_video_message.py
--rw-rw-rw-   0        0        0     1384 2024-02-25 13:44:36.000000 rubpy-7.0.1b0/rubpy/methods/messages/send_voice.py
--rw-rw-rw-   0        0        0     2422 2024-02-25 13:43:55.000000 rubpy-7.0.1b0/rubpy/methods/messages/set_pin_message.py
--rw-rw-rw-   0        0        0      799 2024-02-25 13:44:20.000000 rubpy-7.0.1b0/rubpy/methods/messages/vote_poll.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.169635 rubpy-7.0.1b0/rubpy/methods/settings/
--rw-rw-rw-   0        0        0      878 2023-12-22 15:33:50.000000 rubpy-7.0.1b0/rubpy/methods/settings/__init__.py
--rw-rw-rw-   0        0        0      746 2024-02-25 13:16:01.000000 rubpy-7.0.1b0/rubpy/methods/settings/delete_folder.py
--rw-rw-rw-   0        0        0      586 2024-02-25 13:17:26.000000 rubpy-7.0.1b0/rubpy/methods/settings/get_blocked_users.py
--rw-rw-rw-   0        0        0      832 2024-02-25 13:17:43.000000 rubpy-7.0.1b0/rubpy/methods/settings/get_folders.py
--rw-rw-rw-   0        0        0      660 2024-02-25 13:18:03.000000 rubpy-7.0.1b0/rubpy/methods/settings/get_my_sessions.py
--rw-rw-rw-   0        0        0      640 2024-02-25 13:18:19.000000 rubpy-7.0.1b0/rubpy/methods/settings/get_privacy_setting.py
--rw-rw-rw-   0        0        0      648 2024-02-25 13:18:36.000000 rubpy-7.0.1b0/rubpy/methods/settings/get_suggested_folders.py
--rw-rw-rw-   0        0        0      662 2024-02-25 13:18:52.000000 rubpy-7.0.1b0/rubpy/methods/settings/get_two_passcode_status.py
--rw-rw-rw-   0        0        0     3312 2024-02-25 13:19:21.000000 rubpy-7.0.1b0/rubpy/methods/settings/set_setting.py
--rw-rw-rw-   0        0        0     1267 2024-02-25 13:20:00.000000 rubpy-7.0.1b0/rubpy/methods/settings/setup_two_step_verification.py
--rw-rw-rw-   0        0        0      801 2024-02-25 13:20:16.000000 rubpy-7.0.1b0/rubpy/methods/settings/terminate_session.py
--rw-rw-rw-   0        0        0     1663 2024-02-25 13:20:39.000000 rubpy-7.0.1b0/rubpy/methods/settings/update_profile.py
--rw-rw-rw-   0        0        0      745 2024-02-25 13:20:56.000000 rubpy-7.0.1b0/rubpy/methods/settings/update_username.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.177443 rubpy-7.0.1b0/rubpy/methods/stickers/
--rw-rw-rw-   0        0        0      578 2023-12-22 16:07:24.000000 rubpy-7.0.1b0/rubpy/methods/stickers/__init__.py
--rw-rw-rw-   0        0        0     1283 2024-02-25 13:08:37.000000 rubpy-7.0.1b0/rubpy/methods/stickers/action_on_sticker_set.py
--rw-rw-rw-   0        0        0      564 2024-02-25 13:09:11.000000 rubpy-7.0.1b0/rubpy/methods/stickers/get_my_sticker_sets.py
--rw-rw-rw-   0        0        0      778 2024-02-25 13:09:47.000000 rubpy-7.0.1b0/rubpy/methods/stickers/get_sticker_set_by_id.py
--rw-rw-rw-   0        0        0      877 2024-02-25 13:45:26.000000 rubpy-7.0.1b0/rubpy/methods/stickers/get_stickers_by_emoji.py
--rw-rw-rw-   0        0        0      941 2024-02-25 13:14:21.000000 rubpy-7.0.1b0/rubpy/methods/stickers/get_stickers_by_set_ids.py
--rw-rw-rw-   0        0        0      766 2024-02-25 13:14:11.000000 rubpy-7.0.1b0/rubpy/methods/stickers/get_trend_sticker_sets.py
--rw-rw-rw-   0        0        0      929 2024-02-25 13:14:28.000000 rubpy-7.0.1b0/rubpy/methods/stickers/search_stickers.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.183298 rubpy-7.0.1b0/rubpy/methods/users/
--rw-rw-rw-   0        0        0      331 2023-12-19 22:35:32.000000 rubpy-7.0.1b0/rubpy/methods/users/__init__.py
--rw-rw-rw-   0        0        0      713 2024-02-25 13:03:33.000000 rubpy-7.0.1b0/rubpy/methods/users/check_user_username.py
--rw-rw-rw-   0        0        0     1042 2024-02-25 13:04:30.000000 rubpy-7.0.1b0/rubpy/methods/users/delete_user_chat.py
--rw-rw-rw-   0        0        0      539 2024-02-25 13:05:08.000000 rubpy-7.0.1b0/rubpy/methods/users/get_me.py
--rw-rw-rw-   0        0        0      881 2024-02-26 15:47:56.000000 rubpy-7.0.1b0/rubpy/methods/users/get_user_info.py
--rw-rw-rw-   0        0        0     1265 2024-02-25 13:06:50.000000 rubpy-7.0.1b0/rubpy/methods/users/set_block_user.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.197946 rubpy-7.0.1b0/rubpy/methods/utilities/
--rw-rw-rw-   0        0        0      613 2024-01-12 14:48:33.000000 rubpy-7.0.1b0/rubpy/methods/utilities/__init__.py
--rw-rw-rw-   0        0        0      762 2024-02-25 12:47:55.000000 rubpy-7.0.1b0/rubpy/methods/utilities/add_handler.py
--rw-rw-rw-   0        0        0      741 2024-04-01 23:10:22.000000 rubpy-7.0.1b0/rubpy/methods/utilities/audio.py
--rw-rw-rw-   0        0        0      708 2024-02-26 14:31:15.000000 rubpy-7.0.1b0/rubpy/methods/utilities/connect.py
--rw-rw-rw-   0        0        0      574 2024-02-25 12:48:51.000000 rubpy-7.0.1b0/rubpy/methods/utilities/disconnect.py
--rw-rw-rw-   0        0        0     1755 2024-02-25 12:52:01.000000 rubpy-7.0.1b0/rubpy/methods/utilities/download.py
--rw-rw-rw-   0        0        0     1080 2024-03-20 23:17:03.000000 rubpy-7.0.1b0/rubpy/methods/utilities/download_profile_picture.py
--rw-rw-rw-   0        0        0     1419 2024-02-25 12:52:55.000000 rubpy-7.0.1b0/rubpy/methods/utilities/get_members.py
--rw-rw-rw-   0        0        0      337 2024-02-25 12:53:13.000000 rubpy-7.0.1b0/rubpy/methods/utilities/get_updates.py
--rw-rw-rw-   0        0        0      326 2024-02-25 12:54:09.000000 rubpy-7.0.1b0/rubpy/methods/utilities/remove_handler.py
--rw-rw-rw-   0        0        0      967 2024-02-25 12:54:38.000000 rubpy-7.0.1b0/rubpy/methods/utilities/run.py
--rw-rw-rw-   0        0        0     3646 2024-03-09 18:54:30.000000 rubpy-7.0.1b0/rubpy/methods/utilities/start.py
--rw-rw-rw-   0        0        0     6607 2024-03-12 12:37:06.000000 rubpy-7.0.1b0/rubpy/methods/utilities/thumbnail.py
--rw-rw-rw-   0        0        0      671 2024-02-25 13:02:33.000000 rubpy-7.0.1b0/rubpy/methods/utilities/upload.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.201847 rubpy-7.0.1b0/rubpy/methods/voice_chat/
--rw-rw-rw-   0        0        0      278 2024-02-25 16:36:44.000000 rubpy-7.0.1b0/rubpy/methods/voice_chat/__init__.py
--rw-rw-rw-   0        0        0      918 2024-02-24 23:57:22.000000 rubpy-7.0.1b0/rubpy/methods/voice_chat/join_voice_chat.py
--rw-rw-rw-   0        0        0     1077 2024-02-24 23:55:36.000000 rubpy-7.0.1b0/rubpy/methods/voice_chat/send_group_voice_chat_activity.py
--rw-rw-rw-   0        0        0     1181 2024-02-25 16:36:50.000000 rubpy-7.0.1b0/rubpy/methods/voice_chat/set_voice_chat_state.py
--rw-rw-rw-   0        0        0    15562 2024-04-01 23:19:14.000000 rubpy-7.0.1b0/rubpy/network.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.208678 rubpy-7.0.1b0/rubpy/parser/
--rw-rw-rw-   0        0        0       30 2024-01-09 13:49:12.000000 rubpy-7.0.1b0/rubpy/parser/__init__.py
--rw-rw-rw-   0        0        0     4847 2024-02-25 13:49:56.000000 rubpy-7.0.1b0/rubpy/parser/markdown.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.221926 rubpy-7.0.1b0/rubpy/rubino/
--rw-rw-rw-   0        0        0       26 2024-01-08 21:17:13.000000 rubpy-7.0.1b0/rubpy/rubino/__init__.py
--rw-rw-rw-   0        0        0    16027 2024-03-14 00:36:15.000000 rubpy-7.0.1b0/rubpy/rubino/client.py
--rw-rw-rw-   0        0        0     7124 2024-03-13 13:52:56.000000 rubpy-7.0.1b0/rubpy/rubino/thumbnail.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.225832 rubpy-7.0.1b0/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-7.0.1b0/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2294 2023-12-19 12:35:20.000000 rubpy-7.0.1b0/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-7.0.1b0/rubpy/sessions/stringSession.py
--rw-rw-rw-   0        0        0     3430 2024-03-14 02:26:10.000000 rubpy-7.0.1b0/rubpy/sync.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:30.239494 rubpy-7.0.1b0/rubpy/types/
--rw-rw-rw-   0        0        0       65 2024-02-24 22:46:34.000000 rubpy-7.0.1b0/rubpy/types/__init__.py
--rw-rw-rw-   0        0        0    28754 2024-03-22 13:57:52.000000 rubpy-7.0.1b0/rubpy/types/result.py
--rw-rw-rw-   0        0        0    29226 2024-03-29 05:13:04.000000 rubpy-7.0.1b0/rubpy/types/update.py
--rw-rw-rw-   0        0        0     4530 2024-02-24 22:36:34.000000 rubpy-7.0.1b0/rubpy/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-01 23:53:29.751723 rubpy-7.0.1b0/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3723 2024-04-01 23:53:29.000000 rubpy-7.0.1b0/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8897 2024-04-01 23:53:29.000000 rubpy-7.0.1b0/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 23:53:29.000000 rubpy-7.0.1b0/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2024-04-01 23:53:29.000000 rubpy-7.0.1b0/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-01 23:53:29.000000 rubpy-7.0.1b0/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 23:53:30.241446 rubpy-7.0.1b0/setup.cfg
--rw-rw-rw-   0        0        0     1825 2024-04-01 23:52:57.000000 rubpy-7.0.1b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:15.004871 rubpy-7.0.2b0/
+-rw-rw-rw-   0        0        0     3723 2024-04-24 22:44:15.004871 rubpy-7.0.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0     2472 2024-03-14 02:30:28.000000 rubpy-7.0.2b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.559604 rubpy-7.0.2b0/rubpy/
+-rw-rw-rw-   0        0        0      490 2024-04-24 22:43:23.000000 rubpy-7.0.2b0/rubpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.602585 rubpy-7.0.2b0/rubpy/bots/
+-rw-rw-rw-   0        0        0        0 2024-01-08 21:58:47.000000 rubpy-7.0.2b0/rubpy/bots/__init__.py
+-rw-rw-rw-   0        0        0    11161 2024-01-08 22:59:16.000000 rubpy-7.0.2b0/rubpy/bots/client.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.783321 rubpy-7.0.2b0/rubpy/bots/types/
+-rw-rw-rw-   0        0        0     1077 2024-01-08 22:47:11.000000 rubpy-7.0.2b0/rubpy/bots/types/__init__.py
+-rw-rw-rw-   0        0        0      163 2024-01-08 22:26:46.000000 rubpy-7.0.2b0/rubpy/bots/types/aux_data.py
+-rw-rw-rw-   0        0        0      255 2024-01-08 22:11:16.000000 rubpy-7.0.2b0/rubpy/bots/types/bot.py
+-rw-rw-rw-   0        0        0      102 2024-01-08 22:11:52.000000 rubpy-7.0.2b0/rubpy/bots/types/bot_command.py
+-rw-rw-rw-   0        0        0     1093 2024-01-08 22:29:20.000000 rubpy-7.0.2b0/rubpy/bots/types/button.py
+-rw-rw-rw-   0        0        0      225 2024-01-08 22:20:24.000000 rubpy-7.0.2b0/rubpy/bots/types/button_calendar.py
+-rw-rw-rw-   0        0        0      286 2024-01-08 22:25:55.000000 rubpy-7.0.2b0/rubpy/bots/types/button_location.py
+-rw-rw-rw-   0        0        0      191 2024-01-08 22:21:11.000000 rubpy-7.0.2b0/rubpy/bots/types/button_number_picker.py
+-rw-rw-rw-   0        0        0      377 2024-01-08 22:19:28.000000 rubpy-7.0.2b0/rubpy/bots/types/button_selection.py
+-rw-rw-rw-   0        0        0      195 2024-01-08 22:18:19.000000 rubpy-7.0.2b0/rubpy/bots/types/button_selection_item.py
+-rw-rw-rw-   0        0        0      159 2024-01-08 22:22:12.000000 rubpy-7.0.2b0/rubpy/bots/types/button_string_picker.py
+-rw-rw-rw-   0        0        0      255 2024-01-08 22:24:13.000000 rubpy-7.0.2b0/rubpy/bots/types/button_textbox.py
+-rw-rw-rw-   0        0        0      257 2024-01-08 22:02:54.000000 rubpy-7.0.2b0/rubpy/bots/types/chat.py
+-rw-rw-rw-   0        0        0      132 2024-01-08 22:13:08.000000 rubpy-7.0.2b0/rubpy/bots/types/contact_message.py
+-rw-rw-rw-   0        0        0      111 2024-01-08 22:02:20.000000 rubpy-7.0.2b0/rubpy/bots/types/file.py
+-rw-rw-rw-   0        0        0      214 2024-01-08 22:03:18.000000 rubpy-7.0.2b0/rubpy/bots/types/forwarded_from.py
+-rw-rw-rw-   0        0        0      340 2024-01-08 22:36:23.000000 rubpy-7.0.2b0/rubpy/bots/types/inline_message.py
+-rw-rw-rw-   0        0        0      232 2024-01-08 22:30:58.000000 rubpy-7.0.2b0/rubpy/bots/types/keypad.py
+-rw-rw-rw-   0        0        0      141 2024-01-08 22:30:09.000000 rubpy-7.0.2b0/rubpy/bots/types/keypad_row.py
+-rw-rw-rw-   0        0        0      340 2024-01-08 22:17:29.000000 rubpy-7.0.2b0/rubpy/bots/types/live_location.py
+-rw-rw-rw-   0        0        0       99 2024-01-08 22:15:36.000000 rubpy-7.0.2b0/rubpy/bots/types/location.py
+-rw-rw-rw-   0        0        0      107 2024-01-08 22:09:39.000000 rubpy-7.0.2b0/rubpy/bots/types/messaage_text_update.py
+-rw-rw-rw-   0        0        0      887 2024-01-08 22:34:09.000000 rubpy-7.0.2b0/rubpy/bots/types/message.py
+-rw-rw-rw-   0        0        0      149 2024-01-08 22:31:58.000000 rubpy-7.0.2b0/rubpy/bots/types/message_keypad_update.py
+-rw-rw-rw-   0        0        0      156 2024-01-08 22:03:44.000000 rubpy-7.0.2b0/rubpy/bots/types/payment_status.py
+-rw-rw-rw-   0        0        0      192 2024-01-08 22:14:43.000000 rubpy-7.0.2b0/rubpy/bots/types/poll.py
+-rw-rw-rw-   0        0        0      248 2024-01-08 22:13:58.000000 rubpy-7.0.2b0/rubpy/bots/types/poll_status.py
+-rw-rw-rw-   0        0        0      148 2024-01-08 22:12:28.000000 rubpy-7.0.2b0/rubpy/bots/types/sticker.py
+-rw-rw-rw-   0        0        0      455 2024-01-08 22:35:18.000000 rubpy-7.0.2b0/rubpy/bots/types/update.py
+-rw-rw-rw-   0        0        0     5768 2024-03-14 02:20:07.000000 rubpy-7.0.2b0/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.784301 rubpy-7.0.2b0/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-7.0.2b0/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     5386 2024-04-24 22:40:45.000000 rubpy-7.0.2b0/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.836024 rubpy-7.0.2b0/rubpy/enums/
+-rw-rw-rw-   0        0        0      320 2024-04-24 21:33:03.000000 rubpy-7.0.2b0/rubpy/enums/__init__.py
+-rw-rw-rw-   0        0        0      633 2024-02-03 10:53:26.000000 rubpy-7.0.2b0/rubpy/enums/chat_access_type.py
+-rw-rw-rw-   0        0        0      214 2024-02-03 10:54:38.000000 rubpy-7.0.2b0/rubpy/enums/chat_action.py
+-rw-rw-rw-   0        0        0      370 2024-01-11 13:02:06.000000 rubpy-7.0.2b0/rubpy/enums/chat_type.py
+-rw-rw-rw-   0        0        0      568 2024-04-06 22:47:37.000000 rubpy-7.0.2b0/rubpy/enums/message_media_type.py
+-rw-rw-rw-   0        0        0      100 2024-02-10 16:11:46.000000 rubpy-7.0.2b0/rubpy/enums/parse_mode.py
+-rw-rw-rw-   0        0        0      133 2024-01-11 13:07:44.000000 rubpy-7.0.2b0/rubpy/enums/poll_type.py
+-rw-rw-rw-   0        0        0     1767 2024-01-16 12:03:08.000000 rubpy-7.0.2b0/rubpy/enums/reaction_type.py
+-rw-rw-rw-   0        0        0      280 2024-04-24 21:38:53.000000 rubpy-7.0.2b0/rubpy/enums/report_type.py
+-rw-rw-rw-   0        0        0     1942 2024-01-08 22:38:06.000000 rubpy-7.0.2b0/rubpy/exceptions.py
+-rw-rw-rw-   0        0        0    12877 2024-04-06 22:45:04.000000 rubpy-7.0.2b0/rubpy/filters.py
+-rw-rw-rw-   0        0        0     4886 2024-02-24 22:37:29.000000 rubpy-7.0.2b0/rubpy/handlers.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.837001 rubpy-7.0.2b0/rubpy/methods/
+-rw-rw-rw-   0        0        0      697 2024-02-23 15:20:39.000000 rubpy-7.0.2b0/rubpy/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.837976 rubpy-7.0.2b0/rubpy/methods/advanced/
+-rw-rw-rw-   0        0        0      143 2024-02-22 17:41:57.000000 rubpy-7.0.2b0/rubpy/methods/advanced/__init__.py
+-rw-rw-rw-   0        0        0     2312 2024-03-14 01:56:23.000000 rubpy-7.0.2b0/rubpy/methods/advanced/build.py
+-rw-rw-rw-   0        0        0     4483 2024-02-25 17:08:53.000000 rubpy-7.0.2b0/rubpy/methods/advanced/voice_chat_player.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.841880 rubpy-7.0.2b0/rubpy/methods/auth/
+-rw-rw-rw-   0        0        0      185 2023-12-15 18:54:26.000000 rubpy-7.0.2b0/rubpy/methods/auth/__init__.py
+-rw-rw-rw-   0        0        0     2007 2024-03-09 18:53:42.000000 rubpy-7.0.2b0/rubpy/methods/auth/register_device.py
+-rw-rw-rw-   0        0        0      798 2024-02-24 22:49:22.000000 rubpy-7.0.2b0/rubpy/methods/auth/send_code.py
+-rw-rw-rw-   0        0        0      576 2024-02-24 22:51:51.000000 rubpy-7.0.2b0/rubpy/methods/auth/sign_in.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.859448 rubpy-7.0.2b0/rubpy/methods/channels/
+-rw-rw-rw-   0        0        0     1826 2024-01-22 20:05:38.000000 rubpy-7.0.2b0/rubpy/methods/channels/__init__.py
+-rw-rw-rw-   0        0        0     1042 2024-02-24 22:53:48.000000 rubpy-7.0.2b0/rubpy/methods/channels/add_channel.py
+-rw-rw-rw-   0        0        0      882 2024-02-24 22:53:29.000000 rubpy-7.0.2b0/rubpy/methods/channels/add_channel_members.py
+-rw-rw-rw-   0        0        0     1065 2024-02-24 22:54:12.000000 rubpy-7.0.2b0/rubpy/methods/channels/ban_channel_member.py
+-rw-rw-rw-   0        0        0      613 2024-02-24 22:54:34.000000 rubpy-7.0.2b0/rubpy/methods/channels/channel_preview_by_join_link.py
+-rw-rw-rw-   0        0        0      574 2024-02-24 22:54:51.000000 rubpy-7.0.2b0/rubpy/methods/channels/check_channel_username.py
+-rw-rw-rw-   0        0        0      523 2024-02-24 22:55:07.000000 rubpy-7.0.2b0/rubpy/methods/channels/create_channel_voice_chat.py
+-rw-rw-rw-   0        0        0      748 2024-02-24 22:55:21.000000 rubpy-7.0.2b0/rubpy/methods/channels/discard_channel_voice_chat.py
+-rw-rw-rw-   0        0        0     2601 2024-02-24 22:55:49.000000 rubpy-7.0.2b0/rubpy/methods/channels/edit_channel_info.py
+-rw-rw-rw-   0        0        0      705 2024-02-24 22:56:18.000000 rubpy-7.0.2b0/rubpy/methods/channels/get_banned_group_members.py
+-rw-rw-rw-   0        0        0      681 2024-02-24 22:56:34.000000 rubpy-7.0.2b0/rubpy/methods/channels/get_channel_admin_access_list.py
+-rw-rw-rw-   0        0        0      681 2024-02-24 22:56:52.000000 rubpy-7.0.2b0/rubpy/methods/channels/get_channel_admin_members.py
+-rw-rw-rw-   0        0        0      819 2024-02-24 22:58:08.000000 rubpy-7.0.2b0/rubpy/methods/channels/get_channel_all_members.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 22:58:25.000000 rubpy-7.0.2b0/rubpy/methods/channels/get_channel_info.py
+-rw-rw-rw-   0        0        0      503 2024-02-24 22:58:39.000000 rubpy-7.0.2b0/rubpy/methods/channels/get_channel_link.py
+-rw-rw-rw-   0        0        0      996 2024-02-24 22:58:58.000000 rubpy-7.0.2b0/rubpy/methods/channels/join_channel_action.py
+-rw-rw-rw-   0        0        0      609 2024-02-24 22:59:21.000000 rubpy-7.0.2b0/rubpy/methods/channels/join_channel_by_link.py
+-rw-rw-rw-   0        0        0      610 2024-02-24 22:59:38.000000 rubpy-7.0.2b0/rubpy/methods/channels/remove_channel.py
+-rw-rw-rw-   0        0        0      956 2024-02-24 23:00:34.000000 rubpy-7.0.2b0/rubpy/methods/channels/seen_channel_messages.py
+-rw-rw-rw-   0        0        0      631 2024-02-24 23:00:59.000000 rubpy-7.0.2b0/rubpy/methods/channels/set_channel_link.py
+-rw-rw-rw-   0        0        0     1051 2024-02-24 23:01:17.000000 rubpy-7.0.2b0/rubpy/methods/channels/set_channel_voice_chat_setting.py
+-rw-rw-rw-   0        0        0      772 2024-02-24 23:01:35.000000 rubpy-7.0.2b0/rubpy/methods/channels/update_channel_username.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.870190 rubpy-7.0.2b0/rubpy/methods/chats/
+-rw-rw-rw-   0        0        0      807 2023-12-20 14:35:52.000000 rubpy-7.0.2b0/rubpy/methods/chats/__init__.py
+-rw-rw-rw-   0        0        0      806 2024-02-24 23:02:06.000000 rubpy-7.0.2b0/rubpy/methods/chats/delete_avatar.py
+-rw-rw-rw-   0        0        0      966 2024-02-24 23:02:35.000000 rubpy-7.0.2b0/rubpy/methods/chats/delete_chat_history.py
+-rw-rw-rw-   0        0        0      790 2024-02-24 23:02:59.000000 rubpy-7.0.2b0/rubpy/methods/chats/get_abs_objects.py
+-rw-rw-rw-   0        0        0      636 2024-02-24 23:03:23.000000 rubpy-7.0.2b0/rubpy/methods/chats/get_avatars.py
+-rw-rw-rw-   0        0        0      601 2024-02-24 23:05:28.000000 rubpy-7.0.2b0/rubpy/methods/chats/get_chats.py
+-rw-rw-rw-   0        0        0      745 2024-02-24 23:04:22.000000 rubpy-7.0.2b0/rubpy/methods/chats/get_chats_updates.py
+-rw-rw-rw-   0        0        0      599 2024-02-24 23:08:10.000000 rubpy-7.0.2b0/rubpy/methods/chats/get_link_from_app_url.py
+-rw-rw-rw-   0        0        0     1265 2024-02-24 23:08:43.000000 rubpy-7.0.2b0/rubpy/methods/chats/search_chat_messages.py
+-rw-rw-rw-   0        0        0      611 2024-02-24 23:10:47.000000 rubpy-7.0.2b0/rubpy/methods/chats/seen_chats.py
+-rw-rw-rw-   0        0        0     1110 2024-02-24 23:11:34.000000 rubpy-7.0.2b0/rubpy/methods/chats/send_chat_activity.py
+-rw-rw-rw-   0        0        0     1014 2024-02-24 23:12:16.000000 rubpy-7.0.2b0/rubpy/methods/chats/set_action_chat.py
+-rw-rw-rw-   0        0        0     1818 2024-02-24 23:13:42.000000 rubpy-7.0.2b0/rubpy/methods/chats/upload_avatar.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.874088 rubpy-7.0.2b0/rubpy/methods/contacts/
+-rw-rw-rw-   0        0        0      299 2023-12-22 14:16:01.000000 rubpy-7.0.2b0/rubpy/methods/contacts/__init__.py
+-rw-rw-rw-   0        0        0     1247 2024-02-24 23:15:53.000000 rubpy-7.0.2b0/rubpy/methods/contacts/add_address_book.py
+-rw-rw-rw-   0        0        0      753 2024-02-24 23:16:17.000000 rubpy-7.0.2b0/rubpy/methods/contacts/delete_contact.py
+-rw-rw-rw-   0        0        0      622 2024-02-24 23:18:12.000000 rubpy-7.0.2b0/rubpy/methods/contacts/get_contacts.py
+-rw-rw-rw-   0        0        0      770 2024-02-24 23:17:44.000000 rubpy-7.0.2b0/rubpy/methods/contacts/get_contacts_updates.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.878968 rubpy-7.0.2b0/rubpy/methods/decorators/
+-rw-rw-rw-   0        0        0      415 2023-12-25 13:18:28.000000 rubpy-7.0.2b0/rubpy/methods/decorators/__init__.py
+-rw-rw-rw-   0        0        0      592 2024-02-24 23:18:27.000000 rubpy-7.0.2b0/rubpy/methods/decorators/on_chat_updates.py
+-rw-rw-rw-   0        0        0      604 2024-02-24 23:18:42.000000 rubpy-7.0.2b0/rubpy/methods/decorators/on_message_updates.py
+-rw-rw-rw-   0        0        0      624 2024-02-24 23:18:56.000000 rubpy-7.0.2b0/rubpy/methods/decorators/on_remove_notifications.py
+-rw-rw-rw-   0        0        0      604 2024-02-24 23:19:09.000000 rubpy-7.0.2b0/rubpy/methods/decorators/on_show_activities.py
+-rw-rw-rw-   0        0        0      616 2024-02-24 23:19:21.000000 rubpy-7.0.2b0/rubpy/methods/decorators/on_show_notifications.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.893608 rubpy-7.0.2b0/rubpy/methods/extras/
+-rw-rw-rw-   0        0        0      745 2024-02-15 12:50:33.000000 rubpy-7.0.2b0/rubpy/methods/extras/__init__.py
+-rw-rw-rw-   0        0        0      739 2024-02-24 23:19:55.000000 rubpy-7.0.2b0/rubpy/methods/extras/ban_member.py
+-rw-rw-rw-   0        0        0     1039 2024-02-24 23:20:10.000000 rubpy-7.0.2b0/rubpy/methods/extras/get_info.py
+-rw-rw-rw-   0        0        0      693 2024-02-24 23:20:43.000000 rubpy-7.0.2b0/rubpy/methods/extras/get_object_by_username.py
+-rw-rw-rw-   0        0        0      538 2024-02-24 23:21:03.000000 rubpy-7.0.2b0/rubpy/methods/extras/get_profile_link_items.py
+-rw-rw-rw-   0        0        0      530 2024-02-24 23:21:19.000000 rubpy-7.0.2b0/rubpy/methods/extras/get_related_objects.py
+-rw-rw-rw-   0        0        0      770 2024-02-24 23:22:06.000000 rubpy-7.0.2b0/rubpy/methods/extras/get_transcription.py
+-rw-rw-rw-   0        0        0      690 2024-02-24 23:22:29.000000 rubpy-7.0.2b0/rubpy/methods/extras/join.py
+-rw-rw-rw-   0        0        0      648 2024-02-24 23:22:49.000000 rubpy-7.0.2b0/rubpy/methods/extras/leave_chat.py
+-rw-rw-rw-   0        0        0     1305 2024-04-24 21:38:46.000000 rubpy-7.0.2b0/rubpy/methods/extras/report_object.py
+-rw-rw-rw-   0        0        0      665 2024-02-24 23:24:05.000000 rubpy-7.0.2b0/rubpy/methods/extras/search_global_objects.py
+-rw-rw-rw-   0        0        0      695 2024-02-24 23:25:58.000000 rubpy-7.0.2b0/rubpy/methods/extras/transcribe_voice.py
+-rw-rw-rw-   0        0        0     1019 2024-02-24 23:26:53.000000 rubpy-7.0.2b0/rubpy/methods/extras/user_is_admin.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.897520 rubpy-7.0.2b0/rubpy/methods/gif/
+-rw-rw-rw-   0        0        0      235 2024-01-09 12:00:36.000000 rubpy-7.0.2b0/rubpy/methods/gif/__init__.py
+-rw-rw-rw-   0        0        0      611 2024-02-24 23:27:54.000000 rubpy-7.0.2b0/rubpy/methods/gif/add_to_my_gif_set.py
+-rw-rw-rw-   0        0        0      341 2024-02-24 23:28:10.000000 rubpy-7.0.2b0/rubpy/methods/gif/get_my_gif_set.py
+-rw-rw-rw-   0        0        0      430 2024-02-24 23:28:39.000000 rubpy-7.0.2b0/rubpy/methods/gif/remove_from_my_gif_set.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.917033 rubpy-7.0.2b0/rubpy/methods/groups/
+-rw-rw-rw-   0        0        0     1857 2023-12-22 17:47:50.000000 rubpy-7.0.2b0/rubpy/methods/groups/__init__.py
+-rw-rw-rw-   0        0        0      987 2024-02-24 23:33:24.000000 rubpy-7.0.2b0/rubpy/methods/groups/add_group.py
+-rw-rw-rw-   0        0        0      958 2024-02-24 23:29:42.000000 rubpy-7.0.2b0/rubpy/methods/groups/add_group_members.py
+-rw-rw-rw-   0        0        0     1229 2024-02-24 23:33:49.000000 rubpy-7.0.2b0/rubpy/methods/groups/ban_group_member.py
+-rw-rw-rw-   0        0        0      600 2024-02-24 23:34:06.000000 rubpy-7.0.2b0/rubpy/methods/groups/create_group_voice_chat.py
+-rw-rw-rw-   0        0        0      618 2024-02-24 23:34:23.000000 rubpy-7.0.2b0/rubpy/methods/groups/delete_no_access_group_chat.py
+-rw-rw-rw-   0        0        0     2648 2024-02-24 23:34:53.000000 rubpy-7.0.2b0/rubpy/methods/groups/edit_group_info.py
+-rw-rw-rw-   0        0        0      785 2024-02-24 23:35:11.000000 rubpy-7.0.2b0/rubpy/methods/groups/get_banned_group_members.py
+-rw-rw-rw-   0        0        0      820 2024-02-24 23:35:36.000000 rubpy-7.0.2b0/rubpy/methods/groups/get_group_admin_access_list.py
+-rw-rw-rw-   0        0        0      791 2024-02-24 23:35:53.000000 rubpy-7.0.2b0/rubpy/methods/groups/get_group_admin_members.py
+-rw-rw-rw-   0        0        0     1003 2024-02-25 13:45:13.000000 rubpy-7.0.2b0/rubpy/methods/groups/get_group_all_members.py
+-rw-rw-rw-   0        0        0      644 2024-02-24 23:36:57.000000 rubpy-7.0.2b0/rubpy/methods/groups/get_group_default_access.py
+-rw-rw-rw-   0        0        0      584 2024-02-24 23:37:09.000000 rubpy-7.0.2b0/rubpy/methods/groups/get_group_info.py
+-rw-rw-rw-   0        0        0      578 2024-02-24 23:37:26.000000 rubpy-7.0.2b0/rubpy/methods/groups/get_group_link.py
+-rw-rw-rw-   0        0        0      787 2024-02-24 23:37:39.000000 rubpy-7.0.2b0/rubpy/methods/groups/get_group_mention_list.py
+-rw-rw-rw-   0        0        0     1096 2024-02-24 23:38:09.000000 rubpy-7.0.2b0/rubpy/methods/groups/get_group_voice_chat_updates.py
+-rw-rw-rw-   0        0        0      688 2024-02-24 23:38:23.000000 rubpy-7.0.2b0/rubpy/methods/groups/group_preview_by_join_link.py
+-rw-rw-rw-   0        0        0      645 2024-02-24 23:38:40.000000 rubpy-7.0.2b0/rubpy/methods/groups/join_group.py
+-rw-rw-rw-   0        0        0      460 2024-02-24 23:39:16.000000 rubpy-7.0.2b0/rubpy/methods/groups/leave_group.py
+-rw-rw-rw-   0        0        0      784 2024-02-24 23:38:58.000000 rubpy-7.0.2b0/rubpy/methods/groups/leave_group_voice_chat.py
+-rw-rw-rw-   0        0        0      466 2024-02-24 23:39:33.000000 rubpy-7.0.2b0/rubpy/methods/groups/remove_group.py
+-rw-rw-rw-   0        0        0     1549 2024-02-24 23:40:14.000000 rubpy-7.0.2b0/rubpy/methods/groups/set_group_admin.py
+-rw-rw-rw-   0        0        0      920 2024-02-24 23:42:43.000000 rubpy-7.0.2b0/rubpy/methods/groups/set_group_default_access.py
+-rw-rw-rw-   0        0        0      596 2024-02-24 23:45:52.000000 rubpy-7.0.2b0/rubpy/methods/groups/set_group_link.py
+-rw-rw-rw-   0        0        0      980 2024-02-24 23:49:50.000000 rubpy-7.0.2b0/rubpy/methods/groups/set_group_voice_chat_setting.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.938511 rubpy-7.0.2b0/rubpy/methods/messages/
+-rw-rw-rw-   0        0        0     1808 2024-02-25 13:57:52.000000 rubpy-7.0.2b0/rubpy/methods/messages/__init__.py
+-rw-rw-rw-   0        0        0     1431 2024-02-25 13:21:28.000000 rubpy-7.0.2b0/rubpy/methods/messages/action_on_message_reaction.py
+-rw-rw-rw-   0        0        0     1148 2024-02-25 13:22:34.000000 rubpy-7.0.2b0/rubpy/methods/messages/auto_delete_message.py
+-rw-rw-rw-   0        0        0     2603 2024-02-25 13:23:17.000000 rubpy-7.0.2b0/rubpy/methods/messages/create_poll.py
+-rw-rw-rw-   0        0        0     1550 2024-02-25 13:24:10.000000 rubpy-7.0.2b0/rubpy/methods/messages/delete_messages.py
+-rw-rw-rw-   0        0        0     1633 2024-02-25 13:25:45.000000 rubpy-7.0.2b0/rubpy/methods/messages/edit_message.py
+-rw-rw-rw-   0        0        0     1635 2024-02-25 13:27:51.000000 rubpy-7.0.2b0/rubpy/methods/messages/forward_messages.py
+-rw-rw-rw-   0        0        0     1044 2024-03-14 20:52:58.000000 rubpy-7.0.2b0/rubpy/methods/messages/get_message_share_url.py
+-rw-rw-rw-   0        0        0     1193 2024-02-25 13:28:35.000000 rubpy-7.0.2b0/rubpy/methods/messages/get_messages_by_id.py
+-rw-rw-rw-   0        0        0     1245 2024-02-25 13:28:56.000000 rubpy-7.0.2b0/rubpy/methods/messages/get_messages_interval.py
+-rw-rw-rw-   0        0        0     1165 2024-02-25 13:29:20.000000 rubpy-7.0.2b0/rubpy/methods/messages/get_messages_updates.py
+-rw-rw-rw-   0        0        0     1250 2024-02-25 13:31:15.000000 rubpy-7.0.2b0/rubpy/methods/messages/get_poll_option_voters.py
+-rw-rw-rw-   0        0        0      823 2024-02-25 13:31:35.000000 rubpy-7.0.2b0/rubpy/methods/messages/get_poll_status.py
+-rw-rw-rw-   0        0        0     1090 2024-02-25 13:31:55.000000 rubpy-7.0.2b0/rubpy/methods/messages/reaction.py
+-rw-rw-rw-   0        0        0     1136 2024-02-25 13:32:18.000000 rubpy-7.0.2b0/rubpy/methods/messages/remove_reaction.py
+-rw-rw-rw-   0        0        0     1156 2024-02-25 13:32:38.000000 rubpy-7.0.2b0/rubpy/methods/messages/request_send_file.py
+-rw-rw-rw-   0        0        0     1515 2024-02-25 13:32:59.000000 rubpy-7.0.2b0/rubpy/methods/messages/send_document.py
+-rw-rw-rw-   0        0        0     1248 2024-02-25 13:35:35.000000 rubpy-7.0.2b0/rubpy/methods/messages/send_gif.py
+-rw-rw-rw-   0        0        0     7391 2024-04-06 23:02:59.000000 rubpy-7.0.2b0/rubpy/methods/messages/send_message.py
+-rw-rw-rw-   0        0        0     1266 2024-02-25 13:35:46.000000 rubpy-7.0.2b0/rubpy/methods/messages/send_music.py
+-rw-rw-rw-   0        0        0     1492 2024-02-25 13:35:55.000000 rubpy-7.0.2b0/rubpy/methods/messages/send_photo.py
+-rw-rw-rw-   0        0        0     1785 2024-02-25 13:45:22.000000 rubpy-7.0.2b0/rubpy/methods/messages/send_sticker.py
+-rw-rw-rw-   0        0        0     1236 2024-02-25 13:45:25.000000 rubpy-7.0.2b0/rubpy/methods/messages/send_video.py
+-rw-rw-rw-   0        0        0     1374 2024-02-25 13:45:23.000000 rubpy-7.0.2b0/rubpy/methods/messages/send_video_message.py
+-rw-rw-rw-   0        0        0     1384 2024-02-25 13:44:36.000000 rubpy-7.0.2b0/rubpy/methods/messages/send_voice.py
+-rw-rw-rw-   0        0        0     2422 2024-02-25 13:43:55.000000 rubpy-7.0.2b0/rubpy/methods/messages/set_pin_message.py
+-rw-rw-rw-   0        0        0      799 2024-02-25 13:44:20.000000 rubpy-7.0.2b0/rubpy/methods/messages/vote_poll.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.948264 rubpy-7.0.2b0/rubpy/methods/settings/
+-rw-rw-rw-   0        0        0      878 2023-12-22 15:33:50.000000 rubpy-7.0.2b0/rubpy/methods/settings/__init__.py
+-rw-rw-rw-   0        0        0      746 2024-02-25 13:16:01.000000 rubpy-7.0.2b0/rubpy/methods/settings/delete_folder.py
+-rw-rw-rw-   0        0        0      586 2024-02-25 13:17:26.000000 rubpy-7.0.2b0/rubpy/methods/settings/get_blocked_users.py
+-rw-rw-rw-   0        0        0      832 2024-02-25 13:17:43.000000 rubpy-7.0.2b0/rubpy/methods/settings/get_folders.py
+-rw-rw-rw-   0        0        0      660 2024-02-25 13:18:03.000000 rubpy-7.0.2b0/rubpy/methods/settings/get_my_sessions.py
+-rw-rw-rw-   0        0        0      640 2024-02-25 13:18:19.000000 rubpy-7.0.2b0/rubpy/methods/settings/get_privacy_setting.py
+-rw-rw-rw-   0        0        0      648 2024-02-25 13:18:36.000000 rubpy-7.0.2b0/rubpy/methods/settings/get_suggested_folders.py
+-rw-rw-rw-   0        0        0      662 2024-02-25 13:18:52.000000 rubpy-7.0.2b0/rubpy/methods/settings/get_two_passcode_status.py
+-rw-rw-rw-   0        0        0     3312 2024-02-25 13:19:21.000000 rubpy-7.0.2b0/rubpy/methods/settings/set_setting.py
+-rw-rw-rw-   0        0        0     1267 2024-02-25 13:20:00.000000 rubpy-7.0.2b0/rubpy/methods/settings/setup_two_step_verification.py
+-rw-rw-rw-   0        0        0      801 2024-02-25 13:20:16.000000 rubpy-7.0.2b0/rubpy/methods/settings/terminate_session.py
+-rw-rw-rw-   0        0        0     1663 2024-02-25 13:20:39.000000 rubpy-7.0.2b0/rubpy/methods/settings/update_profile.py
+-rw-rw-rw-   0        0        0      745 2024-02-25 13:20:56.000000 rubpy-7.0.2b0/rubpy/methods/settings/update_username.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.954120 rubpy-7.0.2b0/rubpy/methods/stickers/
+-rw-rw-rw-   0        0        0      578 2023-12-22 16:07:24.000000 rubpy-7.0.2b0/rubpy/methods/stickers/__init__.py
+-rw-rw-rw-   0        0        0     1283 2024-02-25 13:08:37.000000 rubpy-7.0.2b0/rubpy/methods/stickers/action_on_sticker_set.py
+-rw-rw-rw-   0        0        0      564 2024-02-25 13:09:11.000000 rubpy-7.0.2b0/rubpy/methods/stickers/get_my_sticker_sets.py
+-rw-rw-rw-   0        0        0      778 2024-02-25 13:09:47.000000 rubpy-7.0.2b0/rubpy/methods/stickers/get_sticker_set_by_id.py
+-rw-rw-rw-   0        0        0      877 2024-02-25 13:45:26.000000 rubpy-7.0.2b0/rubpy/methods/stickers/get_stickers_by_emoji.py
+-rw-rw-rw-   0        0        0      941 2024-02-25 13:14:21.000000 rubpy-7.0.2b0/rubpy/methods/stickers/get_stickers_by_set_ids.py
+-rw-rw-rw-   0        0        0      766 2024-02-25 13:14:11.000000 rubpy-7.0.2b0/rubpy/methods/stickers/get_trend_sticker_sets.py
+-rw-rw-rw-   0        0        0      929 2024-02-25 13:14:28.000000 rubpy-7.0.2b0/rubpy/methods/stickers/search_stickers.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.959980 rubpy-7.0.2b0/rubpy/methods/users/
+-rw-rw-rw-   0        0        0      331 2023-12-19 22:35:32.000000 rubpy-7.0.2b0/rubpy/methods/users/__init__.py
+-rw-rw-rw-   0        0        0      713 2024-02-25 13:03:33.000000 rubpy-7.0.2b0/rubpy/methods/users/check_user_username.py
+-rw-rw-rw-   0        0        0     1042 2024-02-25 13:04:30.000000 rubpy-7.0.2b0/rubpy/methods/users/delete_user_chat.py
+-rw-rw-rw-   0        0        0      539 2024-02-25 13:05:08.000000 rubpy-7.0.2b0/rubpy/methods/users/get_me.py
+-rw-rw-rw-   0        0        0      881 2024-02-26 15:47:56.000000 rubpy-7.0.2b0/rubpy/methods/users/get_user_info.py
+-rw-rw-rw-   0        0        0     1265 2024-02-25 13:06:50.000000 rubpy-7.0.2b0/rubpy/methods/users/set_block_user.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.984375 rubpy-7.0.2b0/rubpy/methods/utilities/
+-rw-rw-rw-   0        0        0      613 2024-01-12 14:48:33.000000 rubpy-7.0.2b0/rubpy/methods/utilities/__init__.py
+-rw-rw-rw-   0        0        0      762 2024-02-25 12:47:55.000000 rubpy-7.0.2b0/rubpy/methods/utilities/add_handler.py
+-rw-rw-rw-   0        0        0      741 2024-04-01 23:10:22.000000 rubpy-7.0.2b0/rubpy/methods/utilities/audio.py
+-rw-rw-rw-   0        0        0      708 2024-02-26 14:31:15.000000 rubpy-7.0.2b0/rubpy/methods/utilities/connect.py
+-rw-rw-rw-   0        0        0      574 2024-02-25 12:48:51.000000 rubpy-7.0.2b0/rubpy/methods/utilities/disconnect.py
+-rw-rw-rw-   0        0        0     1756 2024-04-24 22:13:20.000000 rubpy-7.0.2b0/rubpy/methods/utilities/download.py
+-rw-rw-rw-   0        0        0     1080 2024-03-20 23:17:03.000000 rubpy-7.0.2b0/rubpy/methods/utilities/download_profile_picture.py
+-rw-rw-rw-   0        0        0     1419 2024-02-25 12:52:55.000000 rubpy-7.0.2b0/rubpy/methods/utilities/get_members.py
+-rw-rw-rw-   0        0        0      337 2024-02-25 12:53:13.000000 rubpy-7.0.2b0/rubpy/methods/utilities/get_updates.py
+-rw-rw-rw-   0        0        0      326 2024-02-25 12:54:09.000000 rubpy-7.0.2b0/rubpy/methods/utilities/remove_handler.py
+-rw-rw-rw-   0        0        0      967 2024-02-25 12:54:38.000000 rubpy-7.0.2b0/rubpy/methods/utilities/run.py
+-rw-rw-rw-   0        0        0     3646 2024-03-09 18:54:30.000000 rubpy-7.0.2b0/rubpy/methods/utilities/start.py
+-rw-rw-rw-   0        0        0     6614 2024-04-06 23:05:13.000000 rubpy-7.0.2b0/rubpy/methods/utilities/thumbnail.py
+-rw-rw-rw-   0        0        0      671 2024-02-25 13:02:33.000000 rubpy-7.0.2b0/rubpy/methods/utilities/upload.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.988281 rubpy-7.0.2b0/rubpy/methods/voice_chat/
+-rw-rw-rw-   0        0        0      278 2024-02-25 16:36:44.000000 rubpy-7.0.2b0/rubpy/methods/voice_chat/__init__.py
+-rw-rw-rw-   0        0        0      918 2024-02-24 23:57:22.000000 rubpy-7.0.2b0/rubpy/methods/voice_chat/join_voice_chat.py
+-rw-rw-rw-   0        0        0     1077 2024-02-24 23:55:36.000000 rubpy-7.0.2b0/rubpy/methods/voice_chat/send_group_voice_chat_activity.py
+-rw-rw-rw-   0        0        0     1181 2024-02-25 16:36:50.000000 rubpy-7.0.2b0/rubpy/methods/voice_chat/set_voice_chat_state.py
+-rw-rw-rw-   0        0        0    15912 2024-04-24 22:39:50.000000 rubpy-7.0.2b0/rubpy/network.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.990233 rubpy-7.0.2b0/rubpy/parser/
+-rw-rw-rw-   0        0        0       30 2024-01-09 13:49:12.000000 rubpy-7.0.2b0/rubpy/parser/__init__.py
+-rw-rw-rw-   0        0        0     4847 2024-02-25 13:49:56.000000 rubpy-7.0.2b0/rubpy/parser/markdown.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.999992 rubpy-7.0.2b0/rubpy/rubino/
+-rw-rw-rw-   0        0        0       26 2024-01-08 21:17:13.000000 rubpy-7.0.2b0/rubpy/rubino/__init__.py
+-rw-rw-rw-   0        0        0    16027 2024-03-14 00:36:15.000000 rubpy-7.0.2b0/rubpy/rubino/client.py
+-rw-rw-rw-   0        0        0     7124 2024-03-13 13:52:56.000000 rubpy-7.0.2b0/rubpy/rubino/thumbnail.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:15.002921 rubpy-7.0.2b0/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-7.0.2b0/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2294 2023-12-19 12:35:20.000000 rubpy-7.0.2b0/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-7.0.2b0/rubpy/sessions/stringSession.py
+-rw-rw-rw-   0        0        0     3430 2024-03-14 02:26:10.000000 rubpy-7.0.2b0/rubpy/sync.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:15.003897 rubpy-7.0.2b0/rubpy/types/
+-rw-rw-rw-   0        0        0       65 2024-02-24 22:46:34.000000 rubpy-7.0.2b0/rubpy/types/__init__.py
+-rw-rw-rw-   0        0        0    30721 2024-04-24 22:04:33.000000 rubpy-7.0.2b0/rubpy/types/update.py
+-rw-rw-rw-   0        0        0     4530 2024-02-24 22:36:34.000000 rubpy-7.0.2b0/rubpy/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:44:14.588884 rubpy-7.0.2b0/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3723 2024-04-24 22:44:14.000000 rubpy-7.0.2b0/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8875 2024-04-24 22:44:14.000000 rubpy-7.0.2b0/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 22:44:14.000000 rubpy-7.0.2b0/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2024-04-24 22:44:14.000000 rubpy-7.0.2b0/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-24 22:44:14.000000 rubpy-7.0.2b0/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 22:44:15.004871 rubpy-7.0.2b0/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2024-04-24 22:43:40.000000 rubpy-7.0.2b0/setup.py
```

### Comparing `rubpy-7.0.1b0/PKG-INFO` & `rubpy-7.0.2b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 7.0.1b0
+Version: 7.0.2b0
 Summary: A powerful, fast and optimal library for making robots in Rubika with sync and async support.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 7.0.1b0 Summary: A powerful, fast
+Metadata-Version: 2.1 Name: rubpy Version: 7.0.2b0 Summary: A powerful, fast
 and optimal library for making robots in Rubika with sync and async support.
 Home-page: https://github.com/shayanheidari01/rubika Author: Shayan Heidari
 Author-email: contact@shayanheidari.info Keywords:
 rubika,rubpy,chat,bot,robot,asyncio Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `rubpy-7.0.1b0/README.md` & `rubpy-7.0.2b0/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/bots/client.py` & `rubpy-7.0.2b0/rubpy/bots/client.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/bots/types/__init__.py` & `rubpy-7.0.2b0/rubpy/bots/types/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/bots/types/button.py` & `rubpy-7.0.2b0/rubpy/bots/types/button.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/bots/types/message.py` & `rubpy-7.0.2b0/rubpy/bots/types/message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/client.py` & `rubpy-7.0.2b0/rubpy/client.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/crypto/crypto.py` & `rubpy-7.0.2b0/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/enums/chat_access_type.py` & `rubpy-7.0.2b0/rubpy/enums/chat_access_type.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/enums/reaction_type.py` & `rubpy-7.0.2b0/rubpy/enums/reaction_type.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/exceptions.py` & `rubpy-7.0.2b0/rubpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/filters.py` & `rubpy-7.0.2b0/rubpy/filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 __all__ = ['Operator', 'BaseModel', 'RegexModel',
            'AuthorGuids', 'ObjectGuids', 'Commands']
 # List of models for internal use
 __models__ = [
     'is_pinned', 'is_mute', 'count_unseen', 'message_id',
     'is_group', 'is_private', 'is_channel', 'is_in_contact',
     'text', 'original_update', 'object_guid', 'author_guid',
-    'time', 'reply_message_id', 'is_me', 'is_forward', 'is_text']
+    'time', 'reply_message_id', 'is_me', 'is_forward', 'is_text',
+    'music', 'file', 'photo', 'sticker', 'video', 'voice',
+    'contact', 'location', 'poll', 'gif']
 
 def create_model(name, base, authorize: list = [], exception: bool = True, *args, **kwargs):
     """
     Create a model dynamically based on the given name and base class.
 
     :param name: Name of the model.
     :param base: Base class for the model.
@@ -145,90 +147,14 @@
                 result = result != value
 
         return bool(result)
 
     async def __call__(self, update, *args, **kwargs):
         return await self.build(update)
 
-class commands(BaseModel):
-    """
-    Filter for commands in text messages.
-    """
-    def __init__(
-            self,
-            commands: Union[str, List[str]],
-            prefixes: Union[str, List[str]] = "/",
-            case_sensitive: bool = False, *args, **kwargs,
-    ) -> None:
-        """Filter Commands, i.e.: text messages starting with "/" or any other custom prefix.
-
-        Parameters:
-            commands (``str`` | ``list``):
-                The command or list of commands as string the filter should look for.
-                Examples: "start", ["start", "help", "settings"]. When a message text containing
-                a command arrives, the command itself and its arguments will be stored in the *command*
-                field of the :obj:`~pyrogram.types.Message`.
-
-            prefixes (``str`` | ``list``, *optional*):
-                A prefix or a list of prefixes as string the filter should look for.
-                Defaults to "/" (slash). Examples: ".", "!", ["/", "!", "."], list(".:!").
-                Pass None or "" (empty string) to allow commands with no prefix at all.
-
-            case_sensitive (``bool``, *optional*):
-                Pass True if you want your command(s) to be case sensitive. Defaults to False.
-                Examples: when True, command="Start" would trigger /Start but not /start.
-        """
-
-        super().__init__(*args, **kwargs)
-        self.command_re = re.compile(r"([\"'])(.*?)(?<!\\)\1|(\S+)")
-        commands = commands if isinstance(commands, list) else [commands]
-        commands = {c if case_sensitive else c.lower() for c in commands}
-
-        prefixes = [] if prefixes is None else prefixes
-        prefixes = prefixes if isinstance(prefixes, list) else [prefixes]
-        prefixes = set(prefixes) if prefixes else {""}
-
-        self.commands = commands
-        self.prefixes = prefixes
-        self.case_sensitive = case_sensitive
-
-    async def __call__(self, update, *args, **kwargs) -> bool:
-        username = ""
-        text = update.text
-        update['command'] = None
-
-        if not text:
-            return False
-
-        for prefix in self.prefixes:
-            if not text.startswith(prefix):
-                continue
-
-            without_prefix = text[len(prefix):]
-
-            for cmd in self.commands:
-                if not re.match(rf"^(?:{cmd}(?:@?{username})?)(?:\s|$)", without_prefix,
-                                flags=re.IGNORECASE if not self.case_sensitive else 0):
-                    continue
-
-                without_command = re.sub(rf"{cmd}(?:@?{username})?\s?", "", without_prefix, count=1,
-                                         flags=re.IGNORECASE if not self.case_sensitive else 0)
-
-                # match.groups are 1-indexed, group(1) is the quote, group(2) is the text
-                # between the quotes, group(3) is unquoted, whitespace-split text
-
-                # Remove the escape character from the arguments
-                update['command'] = [cmd] + [
-                    re.sub(r"\\([\"'])", r"\1", m.group(2) or m.group(3) or "")
-                    for m in self.command_re.finditer(without_command)
-                ]
-
-                return True
-
-        return False
 
 class Commands(BaseModel):
     """
     Filter for commands in text messages.
     """
     def __init__(
             self,
@@ -435,8 +361,18 @@
 object_guid: Type[BaseModel]
 author_guid: Type[BaseModel]
 time: Type[BaseModel]
 reply_message_id: Type[BaseModel]
 is_me: Type[BaseModel]
 is_forward: Type[BaseModel]
 is_event: Type[BaseModel]
-is_text: Type[BaseModel]
+is_text: Type[BaseModel]
+music: Type[BaseModel]
+file: Type[BaseModel]
+photo: Type[BaseModel]
+video: Type[BaseModel]
+voice: Type[BaseModel]
+contact: Type[BaseModel]
+location: Type[BaseModel]
+poll: Type[BaseModel]
+gif: Type[BaseModel]
+sticker: Type[BaseModel]
```

### Comparing `rubpy-7.0.1b0/rubpy/handlers.py` & `rubpy-7.0.2b0/rubpy/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/__init__.py` & `rubpy-7.0.2b0/rubpy/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/advanced/build.py` & `rubpy-7.0.2b0/rubpy/methods/advanced/build.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/advanced/voice_chat_player.py` & `rubpy-7.0.2b0/rubpy/methods/advanced/voice_chat_player.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/auth/register_device.py` & `rubpy-7.0.2b0/rubpy/methods/auth/register_device.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/auth/send_code.py` & `rubpy-7.0.2b0/rubpy/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/auth/sign_in.py` & `rubpy-7.0.2b0/rubpy/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/__init__.py` & `rubpy-7.0.2b0/rubpy/methods/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/add_channel.py` & `rubpy-7.0.2b0/rubpy/methods/channels/add_channel.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/add_channel_members.py` & `rubpy-7.0.2b0/rubpy/methods/channels/add_channel_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/ban_channel_member.py` & `rubpy-7.0.2b0/rubpy/methods/channels/ban_channel_member.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/channel_preview_by_join_link.py` & `rubpy-7.0.2b0/rubpy/methods/channels/channel_preview_by_join_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/check_channel_username.py` & `rubpy-7.0.2b0/rubpy/methods/channels/check_channel_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/create_channel_voice_chat.py` & `rubpy-7.0.2b0/rubpy/methods/channels/create_channel_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/discard_channel_voice_chat.py` & `rubpy-7.0.2b0/rubpy/methods/channels/discard_channel_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/edit_channel_info.py` & `rubpy-7.0.2b0/rubpy/methods/channels/edit_channel_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/get_banned_group_members.py` & `rubpy-7.0.2b0/rubpy/methods/channels/get_banned_group_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/get_channel_admin_access_list.py` & `rubpy-7.0.2b0/rubpy/methods/channels/get_channel_admin_access_list.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/get_channel_admin_members.py` & `rubpy-7.0.2b0/rubpy/methods/channels/get_channel_admin_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/get_channel_all_members.py` & `rubpy-7.0.2b0/rubpy/methods/channels/get_channel_all_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/join_channel_action.py` & `rubpy-7.0.2b0/rubpy/methods/channels/join_channel_action.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/join_channel_by_link.py` & `rubpy-7.0.2b0/rubpy/methods/channels/join_channel_by_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/remove_channel.py` & `rubpy-7.0.2b0/rubpy/methods/channels/remove_channel.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/seen_channel_messages.py` & `rubpy-7.0.2b0/rubpy/methods/channels/seen_channel_messages.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/set_channel_link.py` & `rubpy-7.0.2b0/rubpy/methods/channels/set_channel_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/set_channel_voice_chat_setting.py` & `rubpy-7.0.2b0/rubpy/methods/channels/set_channel_voice_chat_setting.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/channels/update_channel_username.py` & `rubpy-7.0.2b0/rubpy/methods/channels/update_channel_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/chats/__init__.py` & `rubpy-7.0.2b0/rubpy/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/chats/delete_avatar.py` & `rubpy-7.0.2b0/rubpy/methods/chats/delete_avatar.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/chats/delete_chat_history.py` & `rubpy-7.0.2b0/rubpy/methods/chats/delete_chat_history.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/chats/get_abs_objects.py` & `rubpy-7.0.2b0/rubpy/methods/chats/get_abs_objects.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/chats/get_avatars.py` & `rubpy-7.0.2b0/rubpy/methods/chats/get_avatars.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/chats/get_chats.py` & `rubpy-7.0.2b0/rubpy/methods/chats/get_chats.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/chats/get_chats_updates.py` & `rubpy-7.0.2b0/rubpy/methods/chats/get_chats_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/chats/get_link_from_app_url.py` & `rubpy-7.0.2b0/rubpy/methods/chats/get_link_from_app_url.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/chats/search_chat_messages.py` & `rubpy-7.0.2b0/rubpy/methods/chats/search_chat_messages.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/chats/seen_chats.py` & `rubpy-7.0.2b0/rubpy/methods/chats/seen_chats.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/chats/send_chat_activity.py` & `rubpy-7.0.2b0/rubpy/methods/chats/send_chat_activity.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/chats/set_action_chat.py` & `rubpy-7.0.2b0/rubpy/methods/chats/set_action_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/chats/upload_avatar.py` & `rubpy-7.0.2b0/rubpy/methods/chats/upload_avatar.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/contacts/add_address_book.py` & `rubpy-7.0.2b0/rubpy/methods/contacts/add_address_book.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/contacts/delete_contact.py` & `rubpy-7.0.2b0/rubpy/methods/contacts/delete_contact.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/contacts/get_contacts.py` & `rubpy-7.0.2b0/rubpy/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/contacts/get_contacts_updates.py` & `rubpy-7.0.2b0/rubpy/methods/contacts/get_contacts_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/decorators/on_chat_updates.py` & `rubpy-7.0.2b0/rubpy/methods/decorators/on_chat_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/decorators/on_message_updates.py` & `rubpy-7.0.2b0/rubpy/methods/decorators/on_message_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/decorators/on_remove_notifications.py` & `rubpy-7.0.2b0/rubpy/methods/decorators/on_remove_notifications.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/decorators/on_show_activities.py` & `rubpy-7.0.2b0/rubpy/methods/decorators/on_show_activities.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/decorators/on_show_notifications.py` & `rubpy-7.0.2b0/rubpy/methods/decorators/on_show_notifications.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/extras/__init__.py` & `rubpy-7.0.2b0/rubpy/methods/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/extras/ban_member.py` & `rubpy-7.0.2b0/rubpy/methods/extras/ban_member.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/extras/get_info.py` & `rubpy-7.0.2b0/rubpy/methods/extras/get_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/extras/get_object_by_username.py` & `rubpy-7.0.2b0/rubpy/methods/extras/get_object_by_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/extras/get_profile_link_items.py` & `rubpy-7.0.2b0/rubpy/methods/extras/get_profile_link_items.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/extras/get_related_objects.py` & `rubpy-7.0.2b0/rubpy/methods/extras/get_related_objects.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/extras/get_transcription.py` & `rubpy-7.0.2b0/rubpy/methods/extras/get_transcription.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/extras/join.py` & `rubpy-7.0.2b0/rubpy/methods/extras/join.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/extras/leave_chat.py` & `rubpy-7.0.2b0/rubpy/methods/extras/leave_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/extras/report_object.py` & `rubpy-7.0.2b0/rubpy/methods/extras/report_object.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 class ReportObject:
     async def report_object(
             self: "rubpy.Client",
             object_guid: str,
             report_type: "rubpy.enums.ReportType",
             description: str = None,
-            report_type_object: str = 'Object',
+            message_id: str = None,
+            report_type_object: "rubpy.enums.ReportTypeObject" = 'Object',
     ) -> rubpy.types.Update:
         """
         Report an object (user, channel, group, etc.) for a specific reason.
 
         Args:
             object_guid (str): The identifier of the object to be reported.
             report_type (rubpy.enums.ReportType): The type of report.
@@ -22,11 +23,15 @@
         """
         input = dict(
             object_guid=object_guid,
             report_description=description,
             report_type=report_type,
             report_type_object=report_type_object,
         )
+
+        if message_id is not None:
+            input['message_id'] = message_id
+
         return await self.builder(
             name='reportObject',
             input=input,
         )
```

### Comparing `rubpy-7.0.1b0/rubpy/methods/extras/search_global_objects.py` & `rubpy-7.0.2b0/rubpy/methods/extras/search_global_objects.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/extras/transcribe_voice.py` & `rubpy-7.0.2b0/rubpy/methods/extras/transcribe_voice.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/extras/user_is_admin.py` & `rubpy-7.0.2b0/rubpy/methods/extras/user_is_admin.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/gif/add_to_my_gif_set.py` & `rubpy-7.0.2b0/rubpy/methods/gif/add_to_my_gif_set.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/__init__.py` & `rubpy-7.0.2b0/rubpy/methods/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/add_group.py` & `rubpy-7.0.2b0/rubpy/methods/groups/add_group.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/add_group_members.py` & `rubpy-7.0.2b0/rubpy/methods/groups/add_group_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/ban_group_member.py` & `rubpy-7.0.2b0/rubpy/methods/groups/ban_group_member.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/create_group_voice_chat.py` & `rubpy-7.0.2b0/rubpy/methods/groups/create_group_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/delete_no_access_group_chat.py` & `rubpy-7.0.2b0/rubpy/methods/groups/delete_no_access_group_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/edit_group_info.py` & `rubpy-7.0.2b0/rubpy/methods/groups/edit_group_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/get_banned_group_members.py` & `rubpy-7.0.2b0/rubpy/methods/groups/get_banned_group_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/get_group_admin_access_list.py` & `rubpy-7.0.2b0/rubpy/methods/groups/get_group_admin_access_list.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/get_group_admin_members.py` & `rubpy-7.0.2b0/rubpy/methods/groups/get_group_admin_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/get_group_all_members.py` & `rubpy-7.0.2b0/rubpy/methods/groups/get_group_all_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/get_group_default_access.py` & `rubpy-7.0.2b0/rubpy/methods/groups/get_group_default_access.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/get_group_info.py` & `rubpy-7.0.2b0/rubpy/methods/groups/get_group_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/get_group_link.py` & `rubpy-7.0.2b0/rubpy/methods/groups/get_group_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/get_group_mention_list.py` & `rubpy-7.0.2b0/rubpy/methods/groups/get_group_mention_list.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/get_group_voice_chat_updates.py` & `rubpy-7.0.2b0/rubpy/methods/groups/get_group_voice_chat_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/group_preview_by_join_link.py` & `rubpy-7.0.2b0/rubpy/methods/groups/group_preview_by_join_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/join_group.py` & `rubpy-7.0.2b0/rubpy/methods/groups/join_group.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/leave_group_voice_chat.py` & `rubpy-7.0.2b0/rubpy/methods/groups/leave_group_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/set_group_admin.py` & `rubpy-7.0.2b0/rubpy/methods/groups/set_group_admin.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/set_group_default_access.py` & `rubpy-7.0.2b0/rubpy/methods/groups/set_group_default_access.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/set_group_link.py` & `rubpy-7.0.2b0/rubpy/methods/groups/set_group_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/groups/set_group_voice_chat_setting.py` & `rubpy-7.0.2b0/rubpy/methods/groups/set_group_voice_chat_setting.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/__init__.py` & `rubpy-7.0.2b0/rubpy/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/action_on_message_reaction.py` & `rubpy-7.0.2b0/rubpy/methods/messages/action_on_message_reaction.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/auto_delete_message.py` & `rubpy-7.0.2b0/rubpy/methods/messages/auto_delete_message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/create_poll.py` & `rubpy-7.0.2b0/rubpy/methods/messages/create_poll.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/delete_messages.py` & `rubpy-7.0.2b0/rubpy/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/edit_message.py` & `rubpy-7.0.2b0/rubpy/methods/messages/edit_message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/forward_messages.py` & `rubpy-7.0.2b0/rubpy/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/get_message_share_url.py` & `rubpy-7.0.2b0/rubpy/methods/messages/get_message_share_url.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/get_messages_by_id.py` & `rubpy-7.0.2b0/rubpy/methods/messages/get_messages_by_id.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/get_messages_interval.py` & `rubpy-7.0.2b0/rubpy/methods/messages/get_messages_interval.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/get_messages_updates.py` & `rubpy-7.0.2b0/rubpy/methods/messages/get_messages_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/get_poll_option_voters.py` & `rubpy-7.0.2b0/rubpy/methods/messages/get_poll_option_voters.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/get_poll_status.py` & `rubpy-7.0.2b0/rubpy/methods/messages/get_poll_status.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/reaction.py` & `rubpy-7.0.2b0/rubpy/methods/messages/reaction.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/remove_reaction.py` & `rubpy-7.0.2b0/rubpy/methods/messages/remove_reaction.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/request_send_file.py` & `rubpy-7.0.2b0/rubpy/methods/messages/request_send_file.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/send_document.py` & `rubpy-7.0.2b0/rubpy/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/send_gif.py` & `rubpy-7.0.2b0/rubpy/methods/messages/send_gif.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/send_message.py` & `rubpy-7.0.2b0/rubpy/methods/messages/send_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
             file_inline['time'] = kwargs.get('time', 1)
             file_inline['width'] = kwargs.get('width', 200)
             file_inline['height'] = kwargs.get('height', 200)
             file_inline['music_performer'] = kwargs.get('performer', '')
 
             # Process thumbnail for inline display
             if isinstance(thumb, thumbnail.ResultMedia):
+                print(thumb.seconds)
                 file_inline['time'] = thumb.seconds
                 file_inline['width'] = thumb.width
                 file_inline['height'] = thumb.height
                 file_inline['thumb_inline'] = thumb.to_base64()
             
             if isinstance(audio_info, audio.AudioResult):
                 file_inline['music_performer'] = kwargs.get('performer', audio_info.performer)
```

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/send_music.py` & `rubpy-7.0.2b0/rubpy/methods/messages/send_music.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/send_photo.py` & `rubpy-7.0.2b0/rubpy/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/send_sticker.py` & `rubpy-7.0.2b0/rubpy/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/send_video.py` & `rubpy-7.0.2b0/rubpy/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/send_video_message.py` & `rubpy-7.0.2b0/rubpy/methods/messages/send_video_message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/send_voice.py` & `rubpy-7.0.2b0/rubpy/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/set_pin_message.py` & `rubpy-7.0.2b0/rubpy/methods/messages/set_pin_message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/messages/vote_poll.py` & `rubpy-7.0.2b0/rubpy/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/settings/__init__.py` & `rubpy-7.0.2b0/rubpy/methods/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/settings/delete_folder.py` & `rubpy-7.0.2b0/rubpy/methods/settings/delete_folder.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/settings/get_blocked_users.py` & `rubpy-7.0.2b0/rubpy/methods/settings/get_blocked_users.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/settings/get_folders.py` & `rubpy-7.0.2b0/rubpy/methods/settings/get_folders.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/settings/get_my_sessions.py` & `rubpy-7.0.2b0/rubpy/methods/settings/get_my_sessions.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/settings/get_privacy_setting.py` & `rubpy-7.0.2b0/rubpy/methods/settings/get_privacy_setting.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/settings/get_suggested_folders.py` & `rubpy-7.0.2b0/rubpy/methods/settings/get_suggested_folders.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/settings/get_two_passcode_status.py` & `rubpy-7.0.2b0/rubpy/methods/settings/get_two_passcode_status.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/settings/set_setting.py` & `rubpy-7.0.2b0/rubpy/methods/settings/set_setting.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/settings/setup_two_step_verification.py` & `rubpy-7.0.2b0/rubpy/methods/settings/setup_two_step_verification.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/settings/terminate_session.py` & `rubpy-7.0.2b0/rubpy/methods/settings/terminate_session.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/settings/update_profile.py` & `rubpy-7.0.2b0/rubpy/methods/settings/update_profile.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/settings/update_username.py` & `rubpy-7.0.2b0/rubpy/methods/settings/update_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/stickers/__init__.py` & `rubpy-7.0.2b0/rubpy/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/stickers/action_on_sticker_set.py` & `rubpy-7.0.2b0/rubpy/methods/stickers/action_on_sticker_set.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/stickers/get_my_sticker_sets.py` & `rubpy-7.0.2b0/rubpy/methods/stickers/get_my_sticker_sets.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/stickers/get_sticker_set_by_id.py` & `rubpy-7.0.2b0/rubpy/methods/stickers/get_sticker_set_by_id.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/stickers/get_stickers_by_emoji.py` & `rubpy-7.0.2b0/rubpy/methods/stickers/get_stickers_by_emoji.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/stickers/get_stickers_by_set_ids.py` & `rubpy-7.0.2b0/rubpy/methods/stickers/get_stickers_by_set_ids.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/stickers/get_trend_sticker_sets.py` & `rubpy-7.0.2b0/rubpy/methods/stickers/get_trend_sticker_sets.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/stickers/search_stickers.py` & `rubpy-7.0.2b0/rubpy/methods/stickers/search_stickers.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/users/check_user_username.py` & `rubpy-7.0.2b0/rubpy/methods/users/check_user_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/users/delete_user_chat.py` & `rubpy-7.0.2b0/rubpy/methods/users/delete_user_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/users/get_me.py` & `rubpy-7.0.2b0/rubpy/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/users/get_user_info.py` & `rubpy-7.0.2b0/rubpy/methods/users/get_user_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/users/set_block_user.py` & `rubpy-7.0.2b0/rubpy/methods/users/set_block_user.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/utilities/__init__.py` & `rubpy-7.0.2b0/rubpy/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/utilities/add_handler.py` & `rubpy-7.0.2b0/rubpy/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/utilities/audio.py` & `rubpy-7.0.2b0/rubpy/methods/utilities/audio.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/utilities/connect.py` & `rubpy-7.0.2b0/rubpy/methods/utilities/connect.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/utilities/disconnect.py` & `rubpy-7.0.2b0/rubpy/methods/utilities/disconnect.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/utilities/download.py` & `rubpy-7.0.2b0/rubpy/methods/utilities/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import aiofiles
 
 class Download:
     async def download(
             self: "rubpy.Client",
             file_inline: "rubpy.types.Update",
             save_as: str = None,
-            chunk_size: int = 131072,
+            chunk_size: int = 1054768,
             callback=None,
             *args,
             **kwargs,
     ) -> bytes:
         """
         Download a file using its file_inline information.
```

### Comparing `rubpy-7.0.1b0/rubpy/methods/utilities/download_profile_picture.py` & `rubpy-7.0.2b0/rubpy/methods/utilities/download_profile_picture.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/utilities/get_members.py` & `rubpy-7.0.2b0/rubpy/methods/utilities/get_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/utilities/run.py` & `rubpy-7.0.2b0/rubpy/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/utilities/start.py` & `rubpy-7.0.2b0/rubpy/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/utilities/thumbnail.py` & `rubpy-7.0.2b0/rubpy/methods/utilities/thumbnail.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 
                 capture = VideoFileClip(file_name)
                 width, height = capture.size
                 seconds = int(capture.duration)
                 image = capture.get_frame(seconds / 2)  # Extract frame from the middle of the video
                 capture.close()
                 os.remove(file_name)
-                return ResultMedia(image, width, height, seconds)
+                return ResultMedia(image, width, height, seconds * 1000)
             except Exception as e:
                 print(f"Error processing video with moviepy: {e}")
                 os.remove(file_name)
                 return None
 
         # Continue with the OpenCV approach if moviepy is not available
         if cv2 is None:
```

### Comparing `rubpy-7.0.1b0/rubpy/methods/utilities/upload.py` & `rubpy-7.0.2b0/rubpy/methods/utilities/upload.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/voice_chat/join_voice_chat.py` & `rubpy-7.0.2b0/rubpy/methods/voice_chat/join_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/voice_chat/send_group_voice_chat_activity.py` & `rubpy-7.0.2b0/rubpy/methods/voice_chat/send_group_voice_chat_activity.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/methods/voice_chat/set_voice_chat_state.py` & `rubpy-7.0.2b0/rubpy/methods/voice_chat/set_voice_chat_state.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/network.py` & `rubpy-7.0.2b0/rubpy/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,14 +225,27 @@
                         if msg.type == aiohttp.WSMsgType.TEXT:
                             asyncio.create_task(self.handle_text_message(msg.json()))
                         elif msg.type == aiohttp.WSMsgType.CLOSED:
                             break
                         elif msg.type == aiohttp.WSMsgType.ERROR:
                             break
 
+            except aiohttp.ClientError:
+                continue
+
+            except Exception:
+                continue
+
+    async def keep_socket(self, ws):
+        while True:
+            try:
+                await asyncio.sleep(10.0)
+                await ws.send_json({})
+                await self.client.get_chats_updates()
+
             except Exception:
                 continue
 
     async def handle_text_message(self, msg_data: dict):
         """
         Handle text messages received from the Rubika WebSocket.
 
@@ -353,15 +366,15 @@
                         pass
 
                 index += 1
 
             except Exception:
                 self.client.logger.error(
                     f'UploadFile({file_name}) | Messenger | raised an exception',
-                    extra={'data': self.wss_url}, exc_info=True)
+                    extra={'data': upload_url}, exc_info=True)
 
         status = result['status']
         status_det = result['status_det']
 
         if status == 'OK' and status_det == 'OK':
             result = {
                 'mime': mime,
@@ -378,30 +391,30 @@
 
     async def download(
             self,
             dc_id: int,
             file_id: int,
             access_hash: str,
             size: int,
-            chunk: int=131072,
+            chunk: int=1054768,
             callback=None,
     ) -> bytes:
         """
         Download a file from Rubika.
 
         Parameters:
         - dc_id: Data center ID.
         - file_id: File ID.
         - access_hash: Access hash of the file.
         - size: Total size of the file.
         - chunk: Chunk size for downloading.
         - callback: Progress callback.
 
         Returns:
-        Downloaded file content.
+            - Downloaded file content.
         """
         start_index = 0
         result = b''
 
         headers = {
             'auth': self.client.auth,
             'access-hash-rec': access_hash,
```

### Comparing `rubpy-7.0.1b0/rubpy/parser/markdown.py` & `rubpy-7.0.2b0/rubpy/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/rubino/client.py` & `rubpy-7.0.2b0/rubpy/rubino/client.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/rubino/thumbnail.py` & `rubpy-7.0.2b0/rubpy/rubino/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/sessions/sqliteSession.py` & `rubpy-7.0.2b0/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/sessions/stringSession.py` & `rubpy-7.0.2b0/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/sync.py` & `rubpy-7.0.2b0/rubpy/sync.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy/types/result.py` & `rubpy-7.0.2b0/rubpy/types/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-from json import dumps
-from typing import Literal, Union, Type
+from typing import Literal, Union
 from pathlib import Path
+from json import dumps
 import rubpy
-import warnings
 
 
 class Update:
-    command: Type[Union[list, None]]
-
     def __str__(self) -> str:
         return self.jsonify(indent=2)
 
     def __getattr__(self, name):
         return self.find_keys(keys=name)
 
     def __setitem__(self, key, value):
@@ -65,74 +62,128 @@
                     return self.find_keys(keys=keys, original_update=value)
                 except AttributeError:
                     return None
 
         return None
 
     @property
+    def command(self):
+        return self.find_keys('command')
+
+    @property
     def to_dict(self) -> dict:
         "Return the update as dict"
         return self.original_update
 
     @property
+    def message(self):
+        return self.find_keys('message')
+
+    @property
     def is_me(self):
-        return self.message.is_mine
+        return self.author_guid == self.client.guid
 
     @property
     def status(self):
         return self.find_keys('status')
 
     @property
     def action(self):
-        return self.find_keys('action')
+        return 'action' in self.original_update and self.original_update.get('action')
 
     @property
     def is_edited(self) -> bool:
-        return self.message.is_edited
+        return self.message is not None and self.message.is_edited
 
     @property
     def type(self):
         return self.find_keys(keys=['type', 'author_type'])
 
     @property
     def title(self) -> str:
         return self.find_keys('title')
 
     @property
     def is_forward(self) -> bool:
-        return self.find_keys('forwarded_from')
+        message = self.message
+        return message is not None and 'forwarded_from' in message.original_update
 
     @property
     def forward_type_from(self):
-        return self.find_keys('type_from')
+        return self.message.find_keys('type_from')
 
     @property
     def is_event(self) -> bool:
-        return self.find_keys('event_data')
+        return self.message is not None and self.message.type == 'Event'
+
+    @property
+    def event_data(self):
+        if self.is_event: 
+            return self.message.event_data
+
+    @property
+    def is_file_inline(self):
+        message = self.message
+        return message.type in ['FileInline', 'FileInlineCaption']
 
     @property
     def file_inline(self):
         return self.find_keys('file_inline')
 
     @property
-    def text(self) -> str:
-        return self.find_keys(keys='text')
+    def music(self):
+        return self.file_inline is not None and self.file_inline.type == 'Music'
+
+    @property
+    def file(self):
+        return self.file_inline is not None and self.file_inline.type == 'File'
+
+    @property
+    def photo(self):
+        return self.file_inline is not None and self.file_inline.type == 'Image'
 
     @property
-    def raw_text(self):
-        warnings.warn('The `raw_text` property will be removed soon, please use `text` instead')
-        return self.find_keys(keys='text')
+    def video(self):
+        return self.file_inline is not None and self.file_inline.type == 'Video'
+
+    @property
+    def voice(self):
+        return self.file_inline is not None and self.file_inline.type == 'Voice'
+
+    @property
+    def contact(self):
+        return self.file_inline is not None and self.file_inline.type == 'Contact'
+
+    @property
+    def location(self):
+        return self.file_inline is not None and self.file_inline.type == 'Location'
+
+    @property
+    def poll(self):
+        return self.file_inline is not None and self.file_inline.type == 'Poll'
+
+    @property
+    def gif(self):
+        return self.file_inline is not None and self.file_inline.type == 'Gif'
+
+    @property
+    def sticker(self):
+        return self.find_keys('sticker')
+
+    @property
+    def text(self) -> str:
+        return self.message.text
 
     @property
     def message_id(self):
         return self.find_keys(keys=['message_id', 'pinned_message_id'])
 
     @property
     def reply_message_id(self):
-        return self.find_keys(keys='reply_to_message_id')
+        return self.message.find_keys(keys='reply_to_message_id')
 
     @property
     def is_group(self):
         return self.type == 'Group'
 
     @property
     def is_channel(self):
@@ -144,19 +195,20 @@
 
     @property
     def object_guid(self):
         return self.find_keys(keys=['group_guid', 'object_guid', 'channel_guid'])
 
     @property
     def author_guid(self):
-        return self.author_object_guid
+        return self.message.author_object_guid
 
     @property
     def is_text(self):
-        return self.message.type == 'Text'
+        message = self.message
+        return message is not None and message.type == 'Text'
 
     def guid_type(self, object_guid: str = None):
         """
         Determine the type of the object based on its GUID.
 
         Args:
             - object_guid (str): The GUID of the object.
@@ -502,20 +554,25 @@
         )
 
     async def download(self, file_inline=None, save_as=None, *args, **kwargs):
         """
         Download a file.
 
         Args:
-            - file_inline (dict, optional): File information. Defaults to None.
-            - file (str, optional): Path to save the downloaded file. Defaults to None.
-            - *args, **kwargs: Additional arguments.
+        - file_inline (dict, optional): File information. Defaults to update.file_inline.
+        - save_as (str, optional): The path to save the downloaded file. If None, the file will not be saved.
+        - chunk_size (int, optional): The size of each chunk to download.
+        - callback (callable, optional): A callback function to monitor the download progress.
+        - *args, **kwargs: Additional parameters to pass to the download method.
 
         Returns:
-            - bytes: Downloaded file content.
+        - bytes: The binary data of the downloaded file.
+
+        Raises:
+        - aiofiles.errors.OSFError: If there is an issue with file I/O (when saving the file).
         """
         if isinstance(file_inline, dict):
             file_inline = Update(file_inline)
 
         return await self.client.download(file_inline or self.file_inline, save_as=save_as, *args, **kwargs)
 
     async def get_author(self, author_guid: str = None, *args, **kwargs):
```

### Comparing `rubpy-7.0.1b0/rubpy/utils.py` & `rubpy-7.0.2b0/rubpy/utils.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.1b0/rubpy.egg-info/PKG-INFO` & `rubpy-7.0.2b0/rubpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 7.0.1b0
+Version: 7.0.2b0
 Summary: A powerful, fast and optimal library for making robots in Rubika with sync and async support.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 7.0.1b0 Summary: A powerful, fast
+Metadata-Version: 2.1 Name: rubpy Version: 7.0.2b0 Summary: A powerful, fast
 and optimal library for making robots in Rubika with sync and async support.
 Home-page: https://github.com/shayanheidari01/rubika Author: Shayan Heidari
 Author-email: contact@shayanheidari.info Keywords:
 rubika,rubpy,chat,bot,robot,asyncio Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `rubpy-7.0.1b0/rubpy.egg-info/SOURCES.txt` & `rubpy-7.0.2b0/rubpy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -228,9 +228,8 @@
 rubpy/rubino/__init__.py
 rubpy/rubino/client.py
 rubpy/rubino/thumbnail.py
 rubpy/sessions/__init__.py
 rubpy/sessions/sqliteSession.py
 rubpy/sessions/stringSession.py
 rubpy/types/__init__.py
-rubpy/types/result.py
 rubpy/types/update.py
```

### Comparing `rubpy-7.0.1b0/setup.py` & `rubpy-7.0.2b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 
 with open('README.md', encoding='UTF-8') as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '7.0.1b0',
+    version = '7.0.2b0',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'A powerful, fast and optimal library for making robots in Rubika with sync and async support.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires='~=3.7',
     long_description_content_type = 'text/markdown',
```

