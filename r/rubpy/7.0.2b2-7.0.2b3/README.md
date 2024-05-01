# Comparing `tmp/rubpy-7.0.2b2.tar.gz` & `tmp/rubpy-7.0.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-7.0.2b2.tar", last modified: Sun Apr 28 23:22:40 2024, max compression
+gzip compressed data, was "rubpy-7.0.2b3.tar", last modified: Wed May  1 22:37:48 2024, max compression
```

## Comparing `rubpy-7.0.2b2.tar` & `rubpy-7.0.2b3.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.785146 rubpy-7.0.2b2/
--rw-rw-rw-   0        0        0     3723 2024-04-28 23:22:40.785146 rubpy-7.0.2b2/PKG-INFO
--rw-rw-rw-   0        0        0     2472 2024-03-14 02:30:28.000000 rubpy-7.0.2b2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.266788 rubpy-7.0.2b2/rubpy/
--rw-rw-rw-   0        0        0      490 2024-04-28 23:21:47.000000 rubpy-7.0.2b2/rubpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.316146 rubpy-7.0.2b2/rubpy/bots/
--rw-rw-rw-   0        0        0        0 2024-01-08 21:58:47.000000 rubpy-7.0.2b2/rubpy/bots/__init__.py
--rw-rw-rw-   0        0        0    11161 2024-01-08 22:59:16.000000 rubpy-7.0.2b2/rubpy/bots/client.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.506111 rubpy-7.0.2b2/rubpy/bots/types/
--rw-rw-rw-   0        0        0     1077 2024-01-08 22:47:11.000000 rubpy-7.0.2b2/rubpy/bots/types/__init__.py
--rw-rw-rw-   0        0        0      163 2024-01-08 22:26:46.000000 rubpy-7.0.2b2/rubpy/bots/types/aux_data.py
--rw-rw-rw-   0        0        0      255 2024-01-08 22:11:16.000000 rubpy-7.0.2b2/rubpy/bots/types/bot.py
--rw-rw-rw-   0        0        0      102 2024-01-08 22:11:52.000000 rubpy-7.0.2b2/rubpy/bots/types/bot_command.py
--rw-rw-rw-   0        0        0     1093 2024-01-08 22:29:20.000000 rubpy-7.0.2b2/rubpy/bots/types/button.py
--rw-rw-rw-   0        0        0      225 2024-01-08 22:20:24.000000 rubpy-7.0.2b2/rubpy/bots/types/button_calendar.py
--rw-rw-rw-   0        0        0      286 2024-01-08 22:25:55.000000 rubpy-7.0.2b2/rubpy/bots/types/button_location.py
--rw-rw-rw-   0        0        0      191 2024-01-08 22:21:11.000000 rubpy-7.0.2b2/rubpy/bots/types/button_number_picker.py
--rw-rw-rw-   0        0        0      377 2024-01-08 22:19:28.000000 rubpy-7.0.2b2/rubpy/bots/types/button_selection.py
--rw-rw-rw-   0        0        0      195 2024-01-08 22:18:19.000000 rubpy-7.0.2b2/rubpy/bots/types/button_selection_item.py
--rw-rw-rw-   0        0        0      159 2024-01-08 22:22:12.000000 rubpy-7.0.2b2/rubpy/bots/types/button_string_picker.py
--rw-rw-rw-   0        0        0      255 2024-01-08 22:24:13.000000 rubpy-7.0.2b2/rubpy/bots/types/button_textbox.py
--rw-rw-rw-   0        0        0      257 2024-01-08 22:02:54.000000 rubpy-7.0.2b2/rubpy/bots/types/chat.py
--rw-rw-rw-   0        0        0      132 2024-01-08 22:13:08.000000 rubpy-7.0.2b2/rubpy/bots/types/contact_message.py
--rw-rw-rw-   0        0        0      111 2024-01-08 22:02:20.000000 rubpy-7.0.2b2/rubpy/bots/types/file.py
--rw-rw-rw-   0        0        0      214 2024-01-08 22:03:18.000000 rubpy-7.0.2b2/rubpy/bots/types/forwarded_from.py
--rw-rw-rw-   0        0        0      340 2024-01-08 22:36:23.000000 rubpy-7.0.2b2/rubpy/bots/types/inline_message.py
--rw-rw-rw-   0        0        0      232 2024-01-08 22:30:58.000000 rubpy-7.0.2b2/rubpy/bots/types/keypad.py
--rw-rw-rw-   0        0        0      141 2024-01-08 22:30:09.000000 rubpy-7.0.2b2/rubpy/bots/types/keypad_row.py
--rw-rw-rw-   0        0        0      340 2024-01-08 22:17:29.000000 rubpy-7.0.2b2/rubpy/bots/types/live_location.py
--rw-rw-rw-   0        0        0       99 2024-01-08 22:15:36.000000 rubpy-7.0.2b2/rubpy/bots/types/location.py
--rw-rw-rw-   0        0        0      107 2024-01-08 22:09:39.000000 rubpy-7.0.2b2/rubpy/bots/types/messaage_text_update.py
--rw-rw-rw-   0        0        0      887 2024-01-08 22:34:09.000000 rubpy-7.0.2b2/rubpy/bots/types/message.py
--rw-rw-rw-   0        0        0      149 2024-01-08 22:31:58.000000 rubpy-7.0.2b2/rubpy/bots/types/message_keypad_update.py
--rw-rw-rw-   0        0        0      156 2024-01-08 22:03:44.000000 rubpy-7.0.2b2/rubpy/bots/types/payment_status.py
--rw-rw-rw-   0        0        0      192 2024-01-08 22:14:43.000000 rubpy-7.0.2b2/rubpy/bots/types/poll.py
--rw-rw-rw-   0        0        0      248 2024-01-08 22:13:58.000000 rubpy-7.0.2b2/rubpy/bots/types/poll_status.py
--rw-rw-rw-   0        0        0      148 2024-01-08 22:12:28.000000 rubpy-7.0.2b2/rubpy/bots/types/sticker.py
--rw-rw-rw-   0        0        0      455 2024-01-08 22:35:18.000000 rubpy-7.0.2b2/rubpy/bots/types/update.py
--rw-rw-rw-   0        0        0     5768 2024-03-14 02:20:07.000000 rubpy-7.0.2b2/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.520915 rubpy-7.0.2b2/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-7.0.2b2/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     5386 2024-04-24 22:40:45.000000 rubpy-7.0.2b2/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.563140 rubpy-7.0.2b2/rubpy/enums/
--rw-rw-rw-   0        0        0      320 2024-04-24 21:33:03.000000 rubpy-7.0.2b2/rubpy/enums/__init__.py
--rw-rw-rw-   0        0        0      633 2024-02-03 10:53:26.000000 rubpy-7.0.2b2/rubpy/enums/chat_access_type.py
--rw-rw-rw-   0        0        0      214 2024-02-03 10:54:38.000000 rubpy-7.0.2b2/rubpy/enums/chat_action.py
--rw-rw-rw-   0        0        0      370 2024-01-11 13:02:06.000000 rubpy-7.0.2b2/rubpy/enums/chat_type.py
--rw-rw-rw-   0        0        0      568 2024-04-06 22:47:37.000000 rubpy-7.0.2b2/rubpy/enums/message_media_type.py
--rw-rw-rw-   0        0        0      100 2024-02-10 16:11:46.000000 rubpy-7.0.2b2/rubpy/enums/parse_mode.py
--rw-rw-rw-   0        0        0      133 2024-01-11 13:07:44.000000 rubpy-7.0.2b2/rubpy/enums/poll_type.py
--rw-rw-rw-   0        0        0     1767 2024-01-16 12:03:08.000000 rubpy-7.0.2b2/rubpy/enums/reaction_type.py
--rw-rw-rw-   0        0        0      280 2024-04-24 21:38:53.000000 rubpy-7.0.2b2/rubpy/enums/report_type.py
--rw-rw-rw-   0        0        0     1942 2024-01-08 22:38:06.000000 rubpy-7.0.2b2/rubpy/exceptions.py
--rw-rw-rw-   0        0        0    12877 2024-04-06 22:45:04.000000 rubpy-7.0.2b2/rubpy/filters.py
--rw-rw-rw-   0        0        0     4886 2024-02-24 22:37:29.000000 rubpy-7.0.2b2/rubpy/handlers.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.564117 rubpy-7.0.2b2/rubpy/methods/
--rw-rw-rw-   0        0        0      697 2024-02-23 15:20:39.000000 rubpy-7.0.2b2/rubpy/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.568501 rubpy-7.0.2b2/rubpy/methods/advanced/
--rw-rw-rw-   0        0        0      143 2024-02-22 17:41:57.000000 rubpy-7.0.2b2/rubpy/methods/advanced/__init__.py
--rw-rw-rw-   0        0        0     2312 2024-03-14 01:56:23.000000 rubpy-7.0.2b2/rubpy/methods/advanced/build.py
--rw-rw-rw-   0        0        0     4483 2024-02-25 17:08:53.000000 rubpy-7.0.2b2/rubpy/methods/advanced/voice_chat_player.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.570964 rubpy-7.0.2b2/rubpy/methods/auth/
--rw-rw-rw-   0        0        0      185 2023-12-15 18:54:26.000000 rubpy-7.0.2b2/rubpy/methods/auth/__init__.py
--rw-rw-rw-   0        0        0     2007 2024-03-09 18:53:42.000000 rubpy-7.0.2b2/rubpy/methods/auth/register_device.py
--rw-rw-rw-   0        0        0      798 2024-02-24 22:49:22.000000 rubpy-7.0.2b2/rubpy/methods/auth/send_code.py
--rw-rw-rw-   0        0        0      576 2024-02-24 22:51:51.000000 rubpy-7.0.2b2/rubpy/methods/auth/sign_in.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.595154 rubpy-7.0.2b2/rubpy/methods/channels/
--rw-rw-rw-   0        0        0     1826 2024-01-22 20:05:38.000000 rubpy-7.0.2b2/rubpy/methods/channels/__init__.py
--rw-rw-rw-   0        0        0     1042 2024-02-24 22:53:48.000000 rubpy-7.0.2b2/rubpy/methods/channels/add_channel.py
--rw-rw-rw-   0        0        0      882 2024-02-24 22:53:29.000000 rubpy-7.0.2b2/rubpy/methods/channels/add_channel_members.py
--rw-rw-rw-   0        0        0     1065 2024-02-24 22:54:12.000000 rubpy-7.0.2b2/rubpy/methods/channels/ban_channel_member.py
--rw-rw-rw-   0        0        0      613 2024-02-24 22:54:34.000000 rubpy-7.0.2b2/rubpy/methods/channels/channel_preview_by_join_link.py
--rw-rw-rw-   0        0        0      574 2024-02-24 22:54:51.000000 rubpy-7.0.2b2/rubpy/methods/channels/check_channel_username.py
--rw-rw-rw-   0        0        0      523 2024-02-24 22:55:07.000000 rubpy-7.0.2b2/rubpy/methods/channels/create_channel_voice_chat.py
--rw-rw-rw-   0        0        0      748 2024-02-24 22:55:21.000000 rubpy-7.0.2b2/rubpy/methods/channels/discard_channel_voice_chat.py
--rw-rw-rw-   0        0        0     2601 2024-02-24 22:55:49.000000 rubpy-7.0.2b2/rubpy/methods/channels/edit_channel_info.py
--rw-rw-rw-   0        0        0      705 2024-02-24 22:56:18.000000 rubpy-7.0.2b2/rubpy/methods/channels/get_banned_group_members.py
--rw-rw-rw-   0        0        0      681 2024-02-24 22:56:34.000000 rubpy-7.0.2b2/rubpy/methods/channels/get_channel_admin_access_list.py
--rw-rw-rw-   0        0        0      681 2024-02-24 22:56:52.000000 rubpy-7.0.2b2/rubpy/methods/channels/get_channel_admin_members.py
--rw-rw-rw-   0        0        0      819 2024-02-24 22:58:08.000000 rubpy-7.0.2b2/rubpy/methods/channels/get_channel_all_members.py
--rw-rw-rw-   0        0        0      504 2024-02-24 22:58:25.000000 rubpy-7.0.2b2/rubpy/methods/channels/get_channel_info.py
--rw-rw-rw-   0        0        0      503 2024-02-24 22:58:39.000000 rubpy-7.0.2b2/rubpy/methods/channels/get_channel_link.py
--rw-rw-rw-   0        0        0      996 2024-02-24 22:58:58.000000 rubpy-7.0.2b2/rubpy/methods/channels/join_channel_action.py
--rw-rw-rw-   0        0        0      609 2024-02-24 22:59:21.000000 rubpy-7.0.2b2/rubpy/methods/channels/join_channel_by_link.py
--rw-rw-rw-   0        0        0      610 2024-02-24 22:59:38.000000 rubpy-7.0.2b2/rubpy/methods/channels/remove_channel.py
--rw-rw-rw-   0        0        0      956 2024-02-24 23:00:34.000000 rubpy-7.0.2b2/rubpy/methods/channels/seen_channel_messages.py
--rw-rw-rw-   0        0        0      631 2024-02-24 23:00:59.000000 rubpy-7.0.2b2/rubpy/methods/channels/set_channel_link.py
--rw-rw-rw-   0        0        0     1051 2024-02-24 23:01:17.000000 rubpy-7.0.2b2/rubpy/methods/channels/set_channel_voice_chat_setting.py
--rw-rw-rw-   0        0        0      772 2024-02-24 23:01:35.000000 rubpy-7.0.2b2/rubpy/methods/channels/update_channel_username.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.606253 rubpy-7.0.2b2/rubpy/methods/chats/
--rw-rw-rw-   0        0        0      807 2023-12-20 14:35:52.000000 rubpy-7.0.2b2/rubpy/methods/chats/__init__.py
--rw-rw-rw-   0        0        0      806 2024-02-24 23:02:06.000000 rubpy-7.0.2b2/rubpy/methods/chats/delete_avatar.py
--rw-rw-rw-   0        0        0      966 2024-02-24 23:02:35.000000 rubpy-7.0.2b2/rubpy/methods/chats/delete_chat_history.py
--rw-rw-rw-   0        0        0      790 2024-02-24 23:02:59.000000 rubpy-7.0.2b2/rubpy/methods/chats/get_abs_objects.py
--rw-rw-rw-   0        0        0      636 2024-02-24 23:03:23.000000 rubpy-7.0.2b2/rubpy/methods/chats/get_avatars.py
--rw-rw-rw-   0        0        0      601 2024-02-24 23:05:28.000000 rubpy-7.0.2b2/rubpy/methods/chats/get_chats.py
--rw-rw-rw-   0        0        0      745 2024-02-24 23:04:22.000000 rubpy-7.0.2b2/rubpy/methods/chats/get_chats_updates.py
--rw-rw-rw-   0        0        0      599 2024-02-24 23:08:10.000000 rubpy-7.0.2b2/rubpy/methods/chats/get_link_from_app_url.py
--rw-rw-rw-   0        0        0     1265 2024-02-24 23:08:43.000000 rubpy-7.0.2b2/rubpy/methods/chats/search_chat_messages.py
--rw-rw-rw-   0        0        0      611 2024-02-24 23:10:47.000000 rubpy-7.0.2b2/rubpy/methods/chats/seen_chats.py
--rw-rw-rw-   0        0        0     1110 2024-02-24 23:11:34.000000 rubpy-7.0.2b2/rubpy/methods/chats/send_chat_activity.py
--rw-rw-rw-   0        0        0     1014 2024-02-24 23:12:16.000000 rubpy-7.0.2b2/rubpy/methods/chats/set_action_chat.py
--rw-rw-rw-   0        0        0     1818 2024-02-24 23:13:42.000000 rubpy-7.0.2b2/rubpy/methods/chats/upload_avatar.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.610250 rubpy-7.0.2b2/rubpy/methods/contacts/
--rw-rw-rw-   0        0        0      299 2023-12-22 14:16:01.000000 rubpy-7.0.2b2/rubpy/methods/contacts/__init__.py
--rw-rw-rw-   0        0        0     1247 2024-02-24 23:15:53.000000 rubpy-7.0.2b2/rubpy/methods/contacts/add_address_book.py
--rw-rw-rw-   0        0        0      753 2024-02-24 23:16:17.000000 rubpy-7.0.2b2/rubpy/methods/contacts/delete_contact.py
--rw-rw-rw-   0        0        0      622 2024-02-24 23:18:12.000000 rubpy-7.0.2b2/rubpy/methods/contacts/get_contacts.py
--rw-rw-rw-   0        0        0      770 2024-02-24 23:17:44.000000 rubpy-7.0.2b2/rubpy/methods/contacts/get_contacts_updates.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.615161 rubpy-7.0.2b2/rubpy/methods/decorators/
--rw-rw-rw-   0        0        0      415 2023-12-25 13:18:28.000000 rubpy-7.0.2b2/rubpy/methods/decorators/__init__.py
--rw-rw-rw-   0        0        0      592 2024-02-24 23:18:27.000000 rubpy-7.0.2b2/rubpy/methods/decorators/on_chat_updates.py
--rw-rw-rw-   0        0        0      604 2024-02-24 23:18:42.000000 rubpy-7.0.2b2/rubpy/methods/decorators/on_message_updates.py
--rw-rw-rw-   0        0        0      624 2024-02-24 23:18:56.000000 rubpy-7.0.2b2/rubpy/methods/decorators/on_remove_notifications.py
--rw-rw-rw-   0        0        0      604 2024-02-24 23:19:09.000000 rubpy-7.0.2b2/rubpy/methods/decorators/on_show_activities.py
--rw-rw-rw-   0        0        0      616 2024-02-24 23:19:21.000000 rubpy-7.0.2b2/rubpy/methods/decorators/on_show_notifications.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.631824 rubpy-7.0.2b2/rubpy/methods/extras/
--rw-rw-rw-   0        0        0      745 2024-02-15 12:50:33.000000 rubpy-7.0.2b2/rubpy/methods/extras/__init__.py
--rw-rw-rw-   0        0        0      739 2024-02-24 23:19:55.000000 rubpy-7.0.2b2/rubpy/methods/extras/ban_member.py
--rw-rw-rw-   0        0        0     1039 2024-02-24 23:20:10.000000 rubpy-7.0.2b2/rubpy/methods/extras/get_info.py
--rw-rw-rw-   0        0        0      693 2024-02-24 23:20:43.000000 rubpy-7.0.2b2/rubpy/methods/extras/get_object_by_username.py
--rw-rw-rw-   0        0        0      538 2024-02-24 23:21:03.000000 rubpy-7.0.2b2/rubpy/methods/extras/get_profile_link_items.py
--rw-rw-rw-   0        0        0      530 2024-02-24 23:21:19.000000 rubpy-7.0.2b2/rubpy/methods/extras/get_related_objects.py
--rw-rw-rw-   0        0        0      770 2024-02-24 23:22:06.000000 rubpy-7.0.2b2/rubpy/methods/extras/get_transcription.py
--rw-rw-rw-   0        0        0      690 2024-02-24 23:22:29.000000 rubpy-7.0.2b2/rubpy/methods/extras/join.py
--rw-rw-rw-   0        0        0      648 2024-02-24 23:22:49.000000 rubpy-7.0.2b2/rubpy/methods/extras/leave_chat.py
--rw-rw-rw-   0        0        0     1305 2024-04-24 21:38:46.000000 rubpy-7.0.2b2/rubpy/methods/extras/report_object.py
--rw-rw-rw-   0        0        0      665 2024-02-24 23:24:05.000000 rubpy-7.0.2b2/rubpy/methods/extras/search_global_objects.py
--rw-rw-rw-   0        0        0      695 2024-02-24 23:25:58.000000 rubpy-7.0.2b2/rubpy/methods/extras/transcribe_voice.py
--rw-rw-rw-   0        0        0     1019 2024-02-24 23:26:53.000000 rubpy-7.0.2b2/rubpy/methods/extras/user_is_admin.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.635282 rubpy-7.0.2b2/rubpy/methods/gif/
--rw-rw-rw-   0        0        0      235 2024-01-09 12:00:36.000000 rubpy-7.0.2b2/rubpy/methods/gif/__init__.py
--rw-rw-rw-   0        0        0      611 2024-02-24 23:27:54.000000 rubpy-7.0.2b2/rubpy/methods/gif/add_to_my_gif_set.py
--rw-rw-rw-   0        0        0      341 2024-02-24 23:28:10.000000 rubpy-7.0.2b2/rubpy/methods/gif/get_my_gif_set.py
--rw-rw-rw-   0        0        0      430 2024-02-24 23:28:39.000000 rubpy-7.0.2b2/rubpy/methods/gif/remove_from_my_gif_set.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.656935 rubpy-7.0.2b2/rubpy/methods/groups/
--rw-rw-rw-   0        0        0     1857 2023-12-22 17:47:50.000000 rubpy-7.0.2b2/rubpy/methods/groups/__init__.py
--rw-rw-rw-   0        0        0      987 2024-02-24 23:33:24.000000 rubpy-7.0.2b2/rubpy/methods/groups/add_group.py
--rw-rw-rw-   0        0        0      958 2024-02-24 23:29:42.000000 rubpy-7.0.2b2/rubpy/methods/groups/add_group_members.py
--rw-rw-rw-   0        0        0     1229 2024-02-24 23:33:49.000000 rubpy-7.0.2b2/rubpy/methods/groups/ban_group_member.py
--rw-rw-rw-   0        0        0      600 2024-02-24 23:34:06.000000 rubpy-7.0.2b2/rubpy/methods/groups/create_group_voice_chat.py
--rw-rw-rw-   0        0        0      618 2024-02-24 23:34:23.000000 rubpy-7.0.2b2/rubpy/methods/groups/delete_no_access_group_chat.py
--rw-rw-rw-   0        0        0     2648 2024-02-24 23:34:53.000000 rubpy-7.0.2b2/rubpy/methods/groups/edit_group_info.py
--rw-rw-rw-   0        0        0      785 2024-02-24 23:35:11.000000 rubpy-7.0.2b2/rubpy/methods/groups/get_banned_group_members.py
--rw-rw-rw-   0        0        0      820 2024-02-24 23:35:36.000000 rubpy-7.0.2b2/rubpy/methods/groups/get_group_admin_access_list.py
--rw-rw-rw-   0        0        0      791 2024-02-24 23:35:53.000000 rubpy-7.0.2b2/rubpy/methods/groups/get_group_admin_members.py
--rw-rw-rw-   0        0        0     1003 2024-02-25 13:45:13.000000 rubpy-7.0.2b2/rubpy/methods/groups/get_group_all_members.py
--rw-rw-rw-   0        0        0      644 2024-02-24 23:36:57.000000 rubpy-7.0.2b2/rubpy/methods/groups/get_group_default_access.py
--rw-rw-rw-   0        0        0      584 2024-02-24 23:37:09.000000 rubpy-7.0.2b2/rubpy/methods/groups/get_group_info.py
--rw-rw-rw-   0        0        0      578 2024-02-24 23:37:26.000000 rubpy-7.0.2b2/rubpy/methods/groups/get_group_link.py
--rw-rw-rw-   0        0        0      787 2024-02-24 23:37:39.000000 rubpy-7.0.2b2/rubpy/methods/groups/get_group_mention_list.py
--rw-rw-rw-   0        0        0     1096 2024-02-24 23:38:09.000000 rubpy-7.0.2b2/rubpy/methods/groups/get_group_voice_chat_updates.py
--rw-rw-rw-   0        0        0      688 2024-02-24 23:38:23.000000 rubpy-7.0.2b2/rubpy/methods/groups/group_preview_by_join_link.py
--rw-rw-rw-   0        0        0      645 2024-02-24 23:38:40.000000 rubpy-7.0.2b2/rubpy/methods/groups/join_group.py
--rw-rw-rw-   0        0        0      460 2024-02-24 23:39:16.000000 rubpy-7.0.2b2/rubpy/methods/groups/leave_group.py
--rw-rw-rw-   0        0        0      784 2024-02-24 23:38:58.000000 rubpy-7.0.2b2/rubpy/methods/groups/leave_group_voice_chat.py
--rw-rw-rw-   0        0        0      466 2024-02-24 23:39:33.000000 rubpy-7.0.2b2/rubpy/methods/groups/remove_group.py
--rw-rw-rw-   0        0        0     1549 2024-02-24 23:40:14.000000 rubpy-7.0.2b2/rubpy/methods/groups/set_group_admin.py
--rw-rw-rw-   0        0        0      920 2024-02-24 23:42:43.000000 rubpy-7.0.2b2/rubpy/methods/groups/set_group_default_access.py
--rw-rw-rw-   0        0        0      596 2024-02-24 23:45:52.000000 rubpy-7.0.2b2/rubpy/methods/groups/set_group_link.py
--rw-rw-rw-   0        0        0      980 2024-02-24 23:49:50.000000 rubpy-7.0.2b2/rubpy/methods/groups/set_group_voice_chat_setting.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.682248 rubpy-7.0.2b2/rubpy/methods/messages/
--rw-rw-rw-   0        0        0     1808 2024-02-25 13:57:52.000000 rubpy-7.0.2b2/rubpy/methods/messages/__init__.py
--rw-rw-rw-   0        0        0     1431 2024-02-25 13:21:28.000000 rubpy-7.0.2b2/rubpy/methods/messages/action_on_message_reaction.py
--rw-rw-rw-   0        0        0     1148 2024-02-25 13:22:34.000000 rubpy-7.0.2b2/rubpy/methods/messages/auto_delete_message.py
--rw-rw-rw-   0        0        0     2603 2024-02-25 13:23:17.000000 rubpy-7.0.2b2/rubpy/methods/messages/create_poll.py
--rw-rw-rw-   0        0        0     1550 2024-02-25 13:24:10.000000 rubpy-7.0.2b2/rubpy/methods/messages/delete_messages.py
--rw-rw-rw-   0        0        0     1633 2024-02-25 13:25:45.000000 rubpy-7.0.2b2/rubpy/methods/messages/edit_message.py
--rw-rw-rw-   0        0        0     1635 2024-02-25 13:27:51.000000 rubpy-7.0.2b2/rubpy/methods/messages/forward_messages.py
--rw-rw-rw-   0        0        0     1044 2024-03-14 20:52:58.000000 rubpy-7.0.2b2/rubpy/methods/messages/get_message_share_url.py
--rw-rw-rw-   0        0        0     1193 2024-02-25 13:28:35.000000 rubpy-7.0.2b2/rubpy/methods/messages/get_messages_by_id.py
--rw-rw-rw-   0        0        0     1245 2024-02-25 13:28:56.000000 rubpy-7.0.2b2/rubpy/methods/messages/get_messages_interval.py
--rw-rw-rw-   0        0        0     1165 2024-02-25 13:29:20.000000 rubpy-7.0.2b2/rubpy/methods/messages/get_messages_updates.py
--rw-rw-rw-   0        0        0     1250 2024-02-25 13:31:15.000000 rubpy-7.0.2b2/rubpy/methods/messages/get_poll_option_voters.py
--rw-rw-rw-   0        0        0      823 2024-02-25 13:31:35.000000 rubpy-7.0.2b2/rubpy/methods/messages/get_poll_status.py
--rw-rw-rw-   0        0        0     1090 2024-02-25 13:31:55.000000 rubpy-7.0.2b2/rubpy/methods/messages/reaction.py
--rw-rw-rw-   0        0        0     1136 2024-02-25 13:32:18.000000 rubpy-7.0.2b2/rubpy/methods/messages/remove_reaction.py
--rw-rw-rw-   0        0        0     1156 2024-02-25 13:32:38.000000 rubpy-7.0.2b2/rubpy/methods/messages/request_send_file.py
--rw-rw-rw-   0        0        0     1515 2024-02-25 13:32:59.000000 rubpy-7.0.2b2/rubpy/methods/messages/send_document.py
--rw-rw-rw-   0        0        0     1248 2024-02-25 13:35:35.000000 rubpy-7.0.2b2/rubpy/methods/messages/send_gif.py
--rw-rw-rw-   0        0        0     7391 2024-04-06 23:02:59.000000 rubpy-7.0.2b2/rubpy/methods/messages/send_message.py
--rw-rw-rw-   0        0        0     1266 2024-02-25 13:35:46.000000 rubpy-7.0.2b2/rubpy/methods/messages/send_music.py
--rw-rw-rw-   0        0        0     1492 2024-02-25 13:35:55.000000 rubpy-7.0.2b2/rubpy/methods/messages/send_photo.py
--rw-rw-rw-   0        0        0     1785 2024-02-25 13:45:22.000000 rubpy-7.0.2b2/rubpy/methods/messages/send_sticker.py
--rw-rw-rw-   0        0        0     1236 2024-02-25 13:45:25.000000 rubpy-7.0.2b2/rubpy/methods/messages/send_video.py
--rw-rw-rw-   0        0        0     1374 2024-02-25 13:45:23.000000 rubpy-7.0.2b2/rubpy/methods/messages/send_video_message.py
--rw-rw-rw-   0        0        0     1384 2024-02-25 13:44:36.000000 rubpy-7.0.2b2/rubpy/methods/messages/send_voice.py
--rw-rw-rw-   0        0        0     2422 2024-02-25 13:43:55.000000 rubpy-7.0.2b2/rubpy/methods/messages/set_pin_message.py
--rw-rw-rw-   0        0        0      799 2024-02-25 13:44:20.000000 rubpy-7.0.2b2/rubpy/methods/messages/vote_poll.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.694280 rubpy-7.0.2b2/rubpy/methods/settings/
--rw-rw-rw-   0        0        0      878 2023-12-22 15:33:50.000000 rubpy-7.0.2b2/rubpy/methods/settings/__init__.py
--rw-rw-rw-   0        0        0      746 2024-02-25 13:16:01.000000 rubpy-7.0.2b2/rubpy/methods/settings/delete_folder.py
--rw-rw-rw-   0        0        0      586 2024-02-25 13:17:26.000000 rubpy-7.0.2b2/rubpy/methods/settings/get_blocked_users.py
--rw-rw-rw-   0        0        0      832 2024-02-25 13:17:43.000000 rubpy-7.0.2b2/rubpy/methods/settings/get_folders.py
--rw-rw-rw-   0        0        0      660 2024-02-25 13:18:03.000000 rubpy-7.0.2b2/rubpy/methods/settings/get_my_sessions.py
--rw-rw-rw-   0        0        0      640 2024-02-25 13:18:19.000000 rubpy-7.0.2b2/rubpy/methods/settings/get_privacy_setting.py
--rw-rw-rw-   0        0        0      648 2024-02-25 13:18:36.000000 rubpy-7.0.2b2/rubpy/methods/settings/get_suggested_folders.py
--rw-rw-rw-   0        0        0      662 2024-02-25 13:18:52.000000 rubpy-7.0.2b2/rubpy/methods/settings/get_two_passcode_status.py
--rw-rw-rw-   0        0        0     3312 2024-02-25 13:19:21.000000 rubpy-7.0.2b2/rubpy/methods/settings/set_setting.py
--rw-rw-rw-   0        0        0     1267 2024-02-25 13:20:00.000000 rubpy-7.0.2b2/rubpy/methods/settings/setup_two_step_verification.py
--rw-rw-rw-   0        0        0      801 2024-02-25 13:20:16.000000 rubpy-7.0.2b2/rubpy/methods/settings/terminate_session.py
--rw-rw-rw-   0        0        0     1663 2024-02-25 13:20:39.000000 rubpy-7.0.2b2/rubpy/methods/settings/update_profile.py
--rw-rw-rw-   0        0        0      745 2024-02-25 13:20:56.000000 rubpy-7.0.2b2/rubpy/methods/settings/update_username.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.701530 rubpy-7.0.2b2/rubpy/methods/stickers/
--rw-rw-rw-   0        0        0      578 2023-12-22 16:07:24.000000 rubpy-7.0.2b2/rubpy/methods/stickers/__init__.py
--rw-rw-rw-   0        0        0     1283 2024-02-25 13:08:37.000000 rubpy-7.0.2b2/rubpy/methods/stickers/action_on_sticker_set.py
--rw-rw-rw-   0        0        0      564 2024-02-25 13:09:11.000000 rubpy-7.0.2b2/rubpy/methods/stickers/get_my_sticker_sets.py
--rw-rw-rw-   0        0        0      778 2024-02-25 13:09:47.000000 rubpy-7.0.2b2/rubpy/methods/stickers/get_sticker_set_by_id.py
--rw-rw-rw-   0        0        0      877 2024-02-25 13:45:26.000000 rubpy-7.0.2b2/rubpy/methods/stickers/get_stickers_by_emoji.py
--rw-rw-rw-   0        0        0      941 2024-02-25 13:14:21.000000 rubpy-7.0.2b2/rubpy/methods/stickers/get_stickers_by_set_ids.py
--rw-rw-rw-   0        0        0      766 2024-02-25 13:14:11.000000 rubpy-7.0.2b2/rubpy/methods/stickers/get_trend_sticker_sets.py
--rw-rw-rw-   0        0        0      929 2024-02-25 13:14:28.000000 rubpy-7.0.2b2/rubpy/methods/stickers/search_stickers.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.707216 rubpy-7.0.2b2/rubpy/methods/users/
--rw-rw-rw-   0        0        0      331 2023-12-19 22:35:32.000000 rubpy-7.0.2b2/rubpy/methods/users/__init__.py
--rw-rw-rw-   0        0        0      713 2024-02-25 13:03:33.000000 rubpy-7.0.2b2/rubpy/methods/users/check_user_username.py
--rw-rw-rw-   0        0        0     1042 2024-02-25 13:04:30.000000 rubpy-7.0.2b2/rubpy/methods/users/delete_user_chat.py
--rw-rw-rw-   0        0        0      539 2024-02-25 13:05:08.000000 rubpy-7.0.2b2/rubpy/methods/users/get_me.py
--rw-rw-rw-   0        0        0      881 2024-02-26 15:47:56.000000 rubpy-7.0.2b2/rubpy/methods/users/get_user_info.py
--rw-rw-rw-   0        0        0     1265 2024-02-25 13:06:50.000000 rubpy-7.0.2b2/rubpy/methods/users/set_block_user.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.737176 rubpy-7.0.2b2/rubpy/methods/utilities/
--rw-rw-rw-   0        0        0      613 2024-01-12 14:48:33.000000 rubpy-7.0.2b2/rubpy/methods/utilities/__init__.py
--rw-rw-rw-   0        0        0      762 2024-02-25 12:47:55.000000 rubpy-7.0.2b2/rubpy/methods/utilities/add_handler.py
--rw-rw-rw-   0        0        0      741 2024-04-01 23:10:22.000000 rubpy-7.0.2b2/rubpy/methods/utilities/audio.py
--rw-rw-rw-   0        0        0      708 2024-02-26 14:31:15.000000 rubpy-7.0.2b2/rubpy/methods/utilities/connect.py
--rw-rw-rw-   0        0        0      574 2024-02-25 12:48:51.000000 rubpy-7.0.2b2/rubpy/methods/utilities/disconnect.py
--rw-rw-rw-   0        0        0     1756 2024-04-24 22:13:20.000000 rubpy-7.0.2b2/rubpy/methods/utilities/download.py
--rw-rw-rw-   0        0        0     1080 2024-03-20 23:17:03.000000 rubpy-7.0.2b2/rubpy/methods/utilities/download_profile_picture.py
--rw-rw-rw-   0        0        0     1419 2024-02-25 12:52:55.000000 rubpy-7.0.2b2/rubpy/methods/utilities/get_members.py
--rw-rw-rw-   0        0        0      337 2024-02-25 12:53:13.000000 rubpy-7.0.2b2/rubpy/methods/utilities/get_updates.py
--rw-rw-rw-   0        0        0      326 2024-02-25 12:54:09.000000 rubpy-7.0.2b2/rubpy/methods/utilities/remove_handler.py
--rw-rw-rw-   0        0        0      967 2024-02-25 12:54:38.000000 rubpy-7.0.2b2/rubpy/methods/utilities/run.py
--rw-rw-rw-   0        0        0     3646 2024-03-09 18:54:30.000000 rubpy-7.0.2b2/rubpy/methods/utilities/start.py
--rw-rw-rw-   0        0        0     6614 2024-04-06 23:05:13.000000 rubpy-7.0.2b2/rubpy/methods/utilities/thumbnail.py
--rw-rw-rw-   0        0        0      671 2024-02-25 13:02:33.000000 rubpy-7.0.2b2/rubpy/methods/utilities/upload.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.742075 rubpy-7.0.2b2/rubpy/methods/voice_chat/
--rw-rw-rw-   0        0        0      278 2024-02-25 16:36:44.000000 rubpy-7.0.2b2/rubpy/methods/voice_chat/__init__.py
--rw-rw-rw-   0        0        0      918 2024-02-24 23:57:22.000000 rubpy-7.0.2b2/rubpy/methods/voice_chat/join_voice_chat.py
--rw-rw-rw-   0        0        0     1077 2024-02-24 23:55:36.000000 rubpy-7.0.2b2/rubpy/methods/voice_chat/send_group_voice_chat_activity.py
--rw-rw-rw-   0        0        0     1181 2024-02-25 16:36:50.000000 rubpy-7.0.2b2/rubpy/methods/voice_chat/set_voice_chat_state.py
--rw-rw-rw-   0        0        0    15225 2024-04-28 20:06:28.000000 rubpy-7.0.2b2/rubpy/network.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.759165 rubpy-7.0.2b2/rubpy/parser/
--rw-rw-rw-   0        0        0       30 2024-01-09 13:49:12.000000 rubpy-7.0.2b2/rubpy/parser/__init__.py
--rw-rw-rw-   0        0        0     4847 2024-02-25 13:49:56.000000 rubpy-7.0.2b2/rubpy/parser/markdown.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.770900 rubpy-7.0.2b2/rubpy/rubino/
--rw-rw-rw-   0        0        0       26 2024-01-08 21:17:13.000000 rubpy-7.0.2b2/rubpy/rubino/__init__.py
--rw-rw-rw-   0        0        0    16027 2024-03-14 00:36:15.000000 rubpy-7.0.2b2/rubpy/rubino/client.py
--rw-rw-rw-   0        0        0     7124 2024-03-13 13:52:56.000000 rubpy-7.0.2b2/rubpy/rubino/thumbnail.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.773828 rubpy-7.0.2b2/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-7.0.2b2/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2294 2023-12-19 12:35:20.000000 rubpy-7.0.2b2/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-7.0.2b2/rubpy/sessions/stringSession.py
--rw-rw-rw-   0        0        0     3430 2024-03-14 02:26:10.000000 rubpy-7.0.2b2/rubpy/sync.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.783640 rubpy-7.0.2b2/rubpy/types/
--rw-rw-rw-   0        0        0       65 2024-02-24 22:46:34.000000 rubpy-7.0.2b2/rubpy/types/__init__.py
--rw-rw-rw-   0        0        0    30721 2024-04-24 22:04:33.000000 rubpy-7.0.2b2/rubpy/types/update.py
--rw-rw-rw-   0        0        0     4530 2024-02-24 22:36:34.000000 rubpy-7.0.2b2/rubpy/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-28 23:22:40.301473 rubpy-7.0.2b2/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3723 2024-04-28 23:22:40.000000 rubpy-7.0.2b2/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8875 2024-04-28 23:22:40.000000 rubpy-7.0.2b2/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 23:22:40.000000 rubpy-7.0.2b2/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2024-04-28 23:22:40.000000 rubpy-7.0.2b2/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-28 23:22:40.000000 rubpy-7.0.2b2/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 23:22:40.785146 rubpy-7.0.2b2/setup.cfg
--rw-rw-rw-   0        0        0     1840 2024-04-28 23:21:36.000000 rubpy-7.0.2b2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:48.266779 rubpy-7.0.2b3/
+-rw-rw-rw-   0        0        0     3723 2024-05-01 22:37:48.265798 rubpy-7.0.2b3/PKG-INFO
+-rw-rw-rw-   0        0        0     2472 2024-03-14 02:30:28.000000 rubpy-7.0.2b3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.217710 rubpy-7.0.2b3/rubpy/
+-rw-rw-rw-   0        0        0      490 2024-05-01 22:35:58.000000 rubpy-7.0.2b3/rubpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.276796 rubpy-7.0.2b3/rubpy/bots/
+-rw-rw-rw-   0        0        0        0 2024-01-08 21:58:47.000000 rubpy-7.0.2b3/rubpy/bots/__init__.py
+-rw-rw-rw-   0        0        0    11161 2024-01-08 22:59:16.000000 rubpy-7.0.2b3/rubpy/bots/client.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.472678 rubpy-7.0.2b3/rubpy/bots/types/
+-rw-rw-rw-   0        0        0     1077 2024-01-08 22:47:11.000000 rubpy-7.0.2b3/rubpy/bots/types/__init__.py
+-rw-rw-rw-   0        0        0      163 2024-01-08 22:26:46.000000 rubpy-7.0.2b3/rubpy/bots/types/aux_data.py
+-rw-rw-rw-   0        0        0      255 2024-01-08 22:11:16.000000 rubpy-7.0.2b3/rubpy/bots/types/bot.py
+-rw-rw-rw-   0        0        0      102 2024-01-08 22:11:52.000000 rubpy-7.0.2b3/rubpy/bots/types/bot_command.py
+-rw-rw-rw-   0        0        0     1093 2024-01-08 22:29:20.000000 rubpy-7.0.2b3/rubpy/bots/types/button.py
+-rw-rw-rw-   0        0        0      225 2024-01-08 22:20:24.000000 rubpy-7.0.2b3/rubpy/bots/types/button_calendar.py
+-rw-rw-rw-   0        0        0      286 2024-01-08 22:25:55.000000 rubpy-7.0.2b3/rubpy/bots/types/button_location.py
+-rw-rw-rw-   0        0        0      191 2024-01-08 22:21:11.000000 rubpy-7.0.2b3/rubpy/bots/types/button_number_picker.py
+-rw-rw-rw-   0        0        0      377 2024-01-08 22:19:28.000000 rubpy-7.0.2b3/rubpy/bots/types/button_selection.py
+-rw-rw-rw-   0        0        0      195 2024-01-08 22:18:19.000000 rubpy-7.0.2b3/rubpy/bots/types/button_selection_item.py
+-rw-rw-rw-   0        0        0      159 2024-01-08 22:22:12.000000 rubpy-7.0.2b3/rubpy/bots/types/button_string_picker.py
+-rw-rw-rw-   0        0        0      255 2024-01-08 22:24:13.000000 rubpy-7.0.2b3/rubpy/bots/types/button_textbox.py
+-rw-rw-rw-   0        0        0      257 2024-01-08 22:02:54.000000 rubpy-7.0.2b3/rubpy/bots/types/chat.py
+-rw-rw-rw-   0        0        0      132 2024-01-08 22:13:08.000000 rubpy-7.0.2b3/rubpy/bots/types/contact_message.py
+-rw-rw-rw-   0        0        0      111 2024-01-08 22:02:20.000000 rubpy-7.0.2b3/rubpy/bots/types/file.py
+-rw-rw-rw-   0        0        0      214 2024-01-08 22:03:18.000000 rubpy-7.0.2b3/rubpy/bots/types/forwarded_from.py
+-rw-rw-rw-   0        0        0      340 2024-01-08 22:36:23.000000 rubpy-7.0.2b3/rubpy/bots/types/inline_message.py
+-rw-rw-rw-   0        0        0      232 2024-01-08 22:30:58.000000 rubpy-7.0.2b3/rubpy/bots/types/keypad.py
+-rw-rw-rw-   0        0        0      141 2024-01-08 22:30:09.000000 rubpy-7.0.2b3/rubpy/bots/types/keypad_row.py
+-rw-rw-rw-   0        0        0      340 2024-01-08 22:17:29.000000 rubpy-7.0.2b3/rubpy/bots/types/live_location.py
+-rw-rw-rw-   0        0        0       99 2024-01-08 22:15:36.000000 rubpy-7.0.2b3/rubpy/bots/types/location.py
+-rw-rw-rw-   0        0        0      107 2024-01-08 22:09:39.000000 rubpy-7.0.2b3/rubpy/bots/types/messaage_text_update.py
+-rw-rw-rw-   0        0        0      887 2024-01-08 22:34:09.000000 rubpy-7.0.2b3/rubpy/bots/types/message.py
+-rw-rw-rw-   0        0        0      149 2024-01-08 22:31:58.000000 rubpy-7.0.2b3/rubpy/bots/types/message_keypad_update.py
+-rw-rw-rw-   0        0        0      156 2024-01-08 22:03:44.000000 rubpy-7.0.2b3/rubpy/bots/types/payment_status.py
+-rw-rw-rw-   0        0        0      192 2024-01-08 22:14:43.000000 rubpy-7.0.2b3/rubpy/bots/types/poll.py
+-rw-rw-rw-   0        0        0      248 2024-01-08 22:13:58.000000 rubpy-7.0.2b3/rubpy/bots/types/poll_status.py
+-rw-rw-rw-   0        0        0      148 2024-01-08 22:12:28.000000 rubpy-7.0.2b3/rubpy/bots/types/sticker.py
+-rw-rw-rw-   0        0        0      455 2024-01-08 22:35:18.000000 rubpy-7.0.2b3/rubpy/bots/types/update.py
+-rw-rw-rw-   0        0        0     5768 2024-03-14 02:20:07.000000 rubpy-7.0.2b3/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.488459 rubpy-7.0.2b3/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-7.0.2b3/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     5386 2024-04-24 22:40:45.000000 rubpy-7.0.2b3/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.548063 rubpy-7.0.2b3/rubpy/enums/
+-rw-rw-rw-   0        0        0      320 2024-04-24 21:33:03.000000 rubpy-7.0.2b3/rubpy/enums/__init__.py
+-rw-rw-rw-   0        0        0      633 2024-02-03 10:53:26.000000 rubpy-7.0.2b3/rubpy/enums/chat_access_type.py
+-rw-rw-rw-   0        0        0      214 2024-02-03 10:54:38.000000 rubpy-7.0.2b3/rubpy/enums/chat_action.py
+-rw-rw-rw-   0        0        0      370 2024-01-11 13:02:06.000000 rubpy-7.0.2b3/rubpy/enums/chat_type.py
+-rw-rw-rw-   0        0        0      568 2024-04-06 22:47:37.000000 rubpy-7.0.2b3/rubpy/enums/message_media_type.py
+-rw-rw-rw-   0        0        0      100 2024-02-10 16:11:46.000000 rubpy-7.0.2b3/rubpy/enums/parse_mode.py
+-rw-rw-rw-   0        0        0      133 2024-01-11 13:07:44.000000 rubpy-7.0.2b3/rubpy/enums/poll_type.py
+-rw-rw-rw-   0        0        0     1767 2024-01-16 12:03:08.000000 rubpy-7.0.2b3/rubpy/enums/reaction_type.py
+-rw-rw-rw-   0        0        0      280 2024-04-24 21:38:53.000000 rubpy-7.0.2b3/rubpy/enums/report_type.py
+-rw-rw-rw-   0        0        0     1942 2024-01-08 22:38:06.000000 rubpy-7.0.2b3/rubpy/exceptions.py
+-rw-rw-rw-   0        0        0    12916 2024-05-01 22:34:27.000000 rubpy-7.0.2b3/rubpy/filters.py
+-rw-rw-rw-   0        0        0     4886 2024-02-24 22:37:29.000000 rubpy-7.0.2b3/rubpy/handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.549040 rubpy-7.0.2b3/rubpy/methods/
+-rw-rw-rw-   0        0        0      697 2024-02-23 15:20:39.000000 rubpy-7.0.2b3/rubpy/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.559394 rubpy-7.0.2b3/rubpy/methods/advanced/
+-rw-rw-rw-   0        0        0      143 2024-02-22 17:41:57.000000 rubpy-7.0.2b3/rubpy/methods/advanced/__init__.py
+-rw-rw-rw-   0        0        0     2312 2024-03-14 01:56:23.000000 rubpy-7.0.2b3/rubpy/methods/advanced/build.py
+-rw-rw-rw-   0        0        0     4483 2024-02-25 17:08:53.000000 rubpy-7.0.2b3/rubpy/methods/advanced/voice_chat_player.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.581479 rubpy-7.0.2b3/rubpy/methods/auth/
+-rw-rw-rw-   0        0        0      185 2023-12-15 18:54:26.000000 rubpy-7.0.2b3/rubpy/methods/auth/__init__.py
+-rw-rw-rw-   0        0        0     2007 2024-03-09 18:53:42.000000 rubpy-7.0.2b3/rubpy/methods/auth/register_device.py
+-rw-rw-rw-   0        0        0      798 2024-02-24 22:49:22.000000 rubpy-7.0.2b3/rubpy/methods/auth/send_code.py
+-rw-rw-rw-   0        0        0      576 2024-02-24 22:51:51.000000 rubpy-7.0.2b3/rubpy/methods/auth/sign_in.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.635827 rubpy-7.0.2b3/rubpy/methods/channels/
+-rw-rw-rw-   0        0        0     1826 2024-01-22 20:05:38.000000 rubpy-7.0.2b3/rubpy/methods/channels/__init__.py
+-rw-rw-rw-   0        0        0     1042 2024-02-24 22:53:48.000000 rubpy-7.0.2b3/rubpy/methods/channels/add_channel.py
+-rw-rw-rw-   0        0        0      882 2024-02-24 22:53:29.000000 rubpy-7.0.2b3/rubpy/methods/channels/add_channel_members.py
+-rw-rw-rw-   0        0        0     1065 2024-02-24 22:54:12.000000 rubpy-7.0.2b3/rubpy/methods/channels/ban_channel_member.py
+-rw-rw-rw-   0        0        0      613 2024-02-24 22:54:34.000000 rubpy-7.0.2b3/rubpy/methods/channels/channel_preview_by_join_link.py
+-rw-rw-rw-   0        0        0      574 2024-02-24 22:54:51.000000 rubpy-7.0.2b3/rubpy/methods/channels/check_channel_username.py
+-rw-rw-rw-   0        0        0      523 2024-02-24 22:55:07.000000 rubpy-7.0.2b3/rubpy/methods/channels/create_channel_voice_chat.py
+-rw-rw-rw-   0        0        0      748 2024-02-24 22:55:21.000000 rubpy-7.0.2b3/rubpy/methods/channels/discard_channel_voice_chat.py
+-rw-rw-rw-   0        0        0     2601 2024-02-24 22:55:49.000000 rubpy-7.0.2b3/rubpy/methods/channels/edit_channel_info.py
+-rw-rw-rw-   0        0        0      705 2024-02-24 22:56:18.000000 rubpy-7.0.2b3/rubpy/methods/channels/get_banned_group_members.py
+-rw-rw-rw-   0        0        0      681 2024-02-24 22:56:34.000000 rubpy-7.0.2b3/rubpy/methods/channels/get_channel_admin_access_list.py
+-rw-rw-rw-   0        0        0      681 2024-02-24 22:56:52.000000 rubpy-7.0.2b3/rubpy/methods/channels/get_channel_admin_members.py
+-rw-rw-rw-   0        0        0      819 2024-02-24 22:58:08.000000 rubpy-7.0.2b3/rubpy/methods/channels/get_channel_all_members.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 22:58:25.000000 rubpy-7.0.2b3/rubpy/methods/channels/get_channel_info.py
+-rw-rw-rw-   0        0        0      503 2024-02-24 22:58:39.000000 rubpy-7.0.2b3/rubpy/methods/channels/get_channel_link.py
+-rw-rw-rw-   0        0        0      996 2024-02-24 22:58:58.000000 rubpy-7.0.2b3/rubpy/methods/channels/join_channel_action.py
+-rw-rw-rw-   0        0        0      609 2024-02-24 22:59:21.000000 rubpy-7.0.2b3/rubpy/methods/channels/join_channel_by_link.py
+-rw-rw-rw-   0        0        0      610 2024-02-24 22:59:38.000000 rubpy-7.0.2b3/rubpy/methods/channels/remove_channel.py
+-rw-rw-rw-   0        0        0      956 2024-02-24 23:00:34.000000 rubpy-7.0.2b3/rubpy/methods/channels/seen_channel_messages.py
+-rw-rw-rw-   0        0        0      631 2024-02-24 23:00:59.000000 rubpy-7.0.2b3/rubpy/methods/channels/set_channel_link.py
+-rw-rw-rw-   0        0        0     1051 2024-02-24 23:01:17.000000 rubpy-7.0.2b3/rubpy/methods/channels/set_channel_voice_chat_setting.py
+-rw-rw-rw-   0        0        0      772 2024-02-24 23:01:35.000000 rubpy-7.0.2b3/rubpy/methods/channels/update_channel_username.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.674664 rubpy-7.0.2b3/rubpy/methods/chats/
+-rw-rw-rw-   0        0        0      807 2023-12-20 14:35:52.000000 rubpy-7.0.2b3/rubpy/methods/chats/__init__.py
+-rw-rw-rw-   0        0        0      806 2024-02-24 23:02:06.000000 rubpy-7.0.2b3/rubpy/methods/chats/delete_avatar.py
+-rw-rw-rw-   0        0        0      966 2024-02-24 23:02:35.000000 rubpy-7.0.2b3/rubpy/methods/chats/delete_chat_history.py
+-rw-rw-rw-   0        0        0      790 2024-02-24 23:02:59.000000 rubpy-7.0.2b3/rubpy/methods/chats/get_abs_objects.py
+-rw-rw-rw-   0        0        0      636 2024-02-24 23:03:23.000000 rubpy-7.0.2b3/rubpy/methods/chats/get_avatars.py
+-rw-rw-rw-   0        0        0      601 2024-02-24 23:05:28.000000 rubpy-7.0.2b3/rubpy/methods/chats/get_chats.py
+-rw-rw-rw-   0        0        0      745 2024-02-24 23:04:22.000000 rubpy-7.0.2b3/rubpy/methods/chats/get_chats_updates.py
+-rw-rw-rw-   0        0        0      599 2024-02-24 23:08:10.000000 rubpy-7.0.2b3/rubpy/methods/chats/get_link_from_app_url.py
+-rw-rw-rw-   0        0        0     1265 2024-02-24 23:08:43.000000 rubpy-7.0.2b3/rubpy/methods/chats/search_chat_messages.py
+-rw-rw-rw-   0        0        0      611 2024-02-24 23:10:47.000000 rubpy-7.0.2b3/rubpy/methods/chats/seen_chats.py
+-rw-rw-rw-   0        0        0     1110 2024-02-24 23:11:34.000000 rubpy-7.0.2b3/rubpy/methods/chats/send_chat_activity.py
+-rw-rw-rw-   0        0        0     1014 2024-02-24 23:12:16.000000 rubpy-7.0.2b3/rubpy/methods/chats/set_action_chat.py
+-rw-rw-rw-   0        0        0     1818 2024-02-24 23:13:42.000000 rubpy-7.0.2b3/rubpy/methods/chats/upload_avatar.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.691648 rubpy-7.0.2b3/rubpy/methods/contacts/
+-rw-rw-rw-   0        0        0      299 2023-12-22 14:16:01.000000 rubpy-7.0.2b3/rubpy/methods/contacts/__init__.py
+-rw-rw-rw-   0        0        0     1247 2024-02-24 23:15:53.000000 rubpy-7.0.2b3/rubpy/methods/contacts/add_address_book.py
+-rw-rw-rw-   0        0        0      753 2024-02-24 23:16:17.000000 rubpy-7.0.2b3/rubpy/methods/contacts/delete_contact.py
+-rw-rw-rw-   0        0        0      622 2024-02-24 23:18:12.000000 rubpy-7.0.2b3/rubpy/methods/contacts/get_contacts.py
+-rw-rw-rw-   0        0        0      770 2024-02-24 23:17:44.000000 rubpy-7.0.2b3/rubpy/methods/contacts/get_contacts_updates.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.703485 rubpy-7.0.2b3/rubpy/methods/decorators/
+-rw-rw-rw-   0        0        0      415 2023-12-25 13:18:28.000000 rubpy-7.0.2b3/rubpy/methods/decorators/__init__.py
+-rw-rw-rw-   0        0        0      592 2024-02-24 23:18:27.000000 rubpy-7.0.2b3/rubpy/methods/decorators/on_chat_updates.py
+-rw-rw-rw-   0        0        0      604 2024-02-24 23:18:42.000000 rubpy-7.0.2b3/rubpy/methods/decorators/on_message_updates.py
+-rw-rw-rw-   0        0        0      624 2024-02-24 23:18:56.000000 rubpy-7.0.2b3/rubpy/methods/decorators/on_remove_notifications.py
+-rw-rw-rw-   0        0        0      604 2024-02-24 23:19:09.000000 rubpy-7.0.2b3/rubpy/methods/decorators/on_show_activities.py
+-rw-rw-rw-   0        0        0      616 2024-02-24 23:19:21.000000 rubpy-7.0.2b3/rubpy/methods/decorators/on_show_notifications.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.756352 rubpy-7.0.2b3/rubpy/methods/extras/
+-rw-rw-rw-   0        0        0      745 2024-02-15 12:50:33.000000 rubpy-7.0.2b3/rubpy/methods/extras/__init__.py
+-rw-rw-rw-   0        0        0      739 2024-02-24 23:19:55.000000 rubpy-7.0.2b3/rubpy/methods/extras/ban_member.py
+-rw-rw-rw-   0        0        0     1039 2024-02-24 23:20:10.000000 rubpy-7.0.2b3/rubpy/methods/extras/get_info.py
+-rw-rw-rw-   0        0        0      693 2024-02-24 23:20:43.000000 rubpy-7.0.2b3/rubpy/methods/extras/get_object_by_username.py
+-rw-rw-rw-   0        0        0      538 2024-02-24 23:21:03.000000 rubpy-7.0.2b3/rubpy/methods/extras/get_profile_link_items.py
+-rw-rw-rw-   0        0        0      530 2024-02-24 23:21:19.000000 rubpy-7.0.2b3/rubpy/methods/extras/get_related_objects.py
+-rw-rw-rw-   0        0        0      770 2024-02-24 23:22:06.000000 rubpy-7.0.2b3/rubpy/methods/extras/get_transcription.py
+-rw-rw-rw-   0        0        0      690 2024-02-24 23:22:29.000000 rubpy-7.0.2b3/rubpy/methods/extras/join.py
+-rw-rw-rw-   0        0        0      648 2024-02-24 23:22:49.000000 rubpy-7.0.2b3/rubpy/methods/extras/leave_chat.py
+-rw-rw-rw-   0        0        0     1305 2024-04-24 21:38:46.000000 rubpy-7.0.2b3/rubpy/methods/extras/report_object.py
+-rw-rw-rw-   0        0        0      665 2024-02-24 23:24:05.000000 rubpy-7.0.2b3/rubpy/methods/extras/search_global_objects.py
+-rw-rw-rw-   0        0        0      695 2024-02-24 23:25:58.000000 rubpy-7.0.2b3/rubpy/methods/extras/transcribe_voice.py
+-rw-rw-rw-   0        0        0     1019 2024-02-24 23:26:53.000000 rubpy-7.0.2b3/rubpy/methods/extras/user_is_admin.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.767760 rubpy-7.0.2b3/rubpy/methods/gif/
+-rw-rw-rw-   0        0        0      235 2024-01-09 12:00:36.000000 rubpy-7.0.2b3/rubpy/methods/gif/__init__.py
+-rw-rw-rw-   0        0        0      611 2024-02-24 23:27:54.000000 rubpy-7.0.2b3/rubpy/methods/gif/add_to_my_gif_set.py
+-rw-rw-rw-   0        0        0      341 2024-02-24 23:28:10.000000 rubpy-7.0.2b3/rubpy/methods/gif/get_my_gif_set.py
+-rw-rw-rw-   0        0        0      430 2024-02-24 23:28:39.000000 rubpy-7.0.2b3/rubpy/methods/gif/remove_from_my_gif_set.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.855003 rubpy-7.0.2b3/rubpy/methods/groups/
+-rw-rw-rw-   0        0        0     1857 2023-12-22 17:47:50.000000 rubpy-7.0.2b3/rubpy/methods/groups/__init__.py
+-rw-rw-rw-   0        0        0      987 2024-02-24 23:33:24.000000 rubpy-7.0.2b3/rubpy/methods/groups/add_group.py
+-rw-rw-rw-   0        0        0      958 2024-02-24 23:29:42.000000 rubpy-7.0.2b3/rubpy/methods/groups/add_group_members.py
+-rw-rw-rw-   0        0        0     1229 2024-02-24 23:33:49.000000 rubpy-7.0.2b3/rubpy/methods/groups/ban_group_member.py
+-rw-rw-rw-   0        0        0      600 2024-02-24 23:34:06.000000 rubpy-7.0.2b3/rubpy/methods/groups/create_group_voice_chat.py
+-rw-rw-rw-   0        0        0      618 2024-02-24 23:34:23.000000 rubpy-7.0.2b3/rubpy/methods/groups/delete_no_access_group_chat.py
+-rw-rw-rw-   0        0        0     2648 2024-02-24 23:34:53.000000 rubpy-7.0.2b3/rubpy/methods/groups/edit_group_info.py
+-rw-rw-rw-   0        0        0      785 2024-02-24 23:35:11.000000 rubpy-7.0.2b3/rubpy/methods/groups/get_banned_group_members.py
+-rw-rw-rw-   0        0        0      820 2024-02-24 23:35:36.000000 rubpy-7.0.2b3/rubpy/methods/groups/get_group_admin_access_list.py
+-rw-rw-rw-   0        0        0      791 2024-02-24 23:35:53.000000 rubpy-7.0.2b3/rubpy/methods/groups/get_group_admin_members.py
+-rw-rw-rw-   0        0        0     1003 2024-02-25 13:45:13.000000 rubpy-7.0.2b3/rubpy/methods/groups/get_group_all_members.py
+-rw-rw-rw-   0        0        0      644 2024-02-24 23:36:57.000000 rubpy-7.0.2b3/rubpy/methods/groups/get_group_default_access.py
+-rw-rw-rw-   0        0        0      584 2024-02-24 23:37:09.000000 rubpy-7.0.2b3/rubpy/methods/groups/get_group_info.py
+-rw-rw-rw-   0        0        0      578 2024-02-24 23:37:26.000000 rubpy-7.0.2b3/rubpy/methods/groups/get_group_link.py
+-rw-rw-rw-   0        0        0      787 2024-02-24 23:37:39.000000 rubpy-7.0.2b3/rubpy/methods/groups/get_group_mention_list.py
+-rw-rw-rw-   0        0        0     1096 2024-02-24 23:38:09.000000 rubpy-7.0.2b3/rubpy/methods/groups/get_group_voice_chat_updates.py
+-rw-rw-rw-   0        0        0      688 2024-02-24 23:38:23.000000 rubpy-7.0.2b3/rubpy/methods/groups/group_preview_by_join_link.py
+-rw-rw-rw-   0        0        0      645 2024-02-24 23:38:40.000000 rubpy-7.0.2b3/rubpy/methods/groups/join_group.py
+-rw-rw-rw-   0        0        0      460 2024-02-24 23:39:16.000000 rubpy-7.0.2b3/rubpy/methods/groups/leave_group.py
+-rw-rw-rw-   0        0        0      784 2024-02-24 23:38:58.000000 rubpy-7.0.2b3/rubpy/methods/groups/leave_group_voice_chat.py
+-rw-rw-rw-   0        0        0      466 2024-02-24 23:39:33.000000 rubpy-7.0.2b3/rubpy/methods/groups/remove_group.py
+-rw-rw-rw-   0        0        0     1549 2024-02-24 23:40:14.000000 rubpy-7.0.2b3/rubpy/methods/groups/set_group_admin.py
+-rw-rw-rw-   0        0        0      920 2024-02-24 23:42:43.000000 rubpy-7.0.2b3/rubpy/methods/groups/set_group_default_access.py
+-rw-rw-rw-   0        0        0      596 2024-02-24 23:45:52.000000 rubpy-7.0.2b3/rubpy/methods/groups/set_group_link.py
+-rw-rw-rw-   0        0        0      980 2024-02-24 23:49:50.000000 rubpy-7.0.2b3/rubpy/methods/groups/set_group_voice_chat_setting.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.963809 rubpy-7.0.2b3/rubpy/methods/messages/
+-rw-rw-rw-   0        0        0     1808 2024-02-25 13:57:52.000000 rubpy-7.0.2b3/rubpy/methods/messages/__init__.py
+-rw-rw-rw-   0        0        0     1431 2024-02-25 13:21:28.000000 rubpy-7.0.2b3/rubpy/methods/messages/action_on_message_reaction.py
+-rw-rw-rw-   0        0        0     1148 2024-02-25 13:22:34.000000 rubpy-7.0.2b3/rubpy/methods/messages/auto_delete_message.py
+-rw-rw-rw-   0        0        0     2603 2024-02-25 13:23:17.000000 rubpy-7.0.2b3/rubpy/methods/messages/create_poll.py
+-rw-rw-rw-   0        0        0     1550 2024-02-25 13:24:10.000000 rubpy-7.0.2b3/rubpy/methods/messages/delete_messages.py
+-rw-rw-rw-   0        0        0     1633 2024-02-25 13:25:45.000000 rubpy-7.0.2b3/rubpy/methods/messages/edit_message.py
+-rw-rw-rw-   0        0        0     1635 2024-02-25 13:27:51.000000 rubpy-7.0.2b3/rubpy/methods/messages/forward_messages.py
+-rw-rw-rw-   0        0        0     1044 2024-03-14 20:52:58.000000 rubpy-7.0.2b3/rubpy/methods/messages/get_message_share_url.py
+-rw-rw-rw-   0        0        0     1193 2024-02-25 13:28:35.000000 rubpy-7.0.2b3/rubpy/methods/messages/get_messages_by_id.py
+-rw-rw-rw-   0        0        0     1245 2024-02-25 13:28:56.000000 rubpy-7.0.2b3/rubpy/methods/messages/get_messages_interval.py
+-rw-rw-rw-   0        0        0     1165 2024-02-25 13:29:20.000000 rubpy-7.0.2b3/rubpy/methods/messages/get_messages_updates.py
+-rw-rw-rw-   0        0        0     1250 2024-02-25 13:31:15.000000 rubpy-7.0.2b3/rubpy/methods/messages/get_poll_option_voters.py
+-rw-rw-rw-   0        0        0      823 2024-02-25 13:31:35.000000 rubpy-7.0.2b3/rubpy/methods/messages/get_poll_status.py
+-rw-rw-rw-   0        0        0     1090 2024-02-25 13:31:55.000000 rubpy-7.0.2b3/rubpy/methods/messages/reaction.py
+-rw-rw-rw-   0        0        0     1136 2024-02-25 13:32:18.000000 rubpy-7.0.2b3/rubpy/methods/messages/remove_reaction.py
+-rw-rw-rw-   0        0        0     1156 2024-02-25 13:32:38.000000 rubpy-7.0.2b3/rubpy/methods/messages/request_send_file.py
+-rw-rw-rw-   0        0        0     1515 2024-02-25 13:32:59.000000 rubpy-7.0.2b3/rubpy/methods/messages/send_document.py
+-rw-rw-rw-   0        0        0     1248 2024-02-25 13:35:35.000000 rubpy-7.0.2b3/rubpy/methods/messages/send_gif.py
+-rw-rw-rw-   0        0        0     7391 2024-04-06 23:02:59.000000 rubpy-7.0.2b3/rubpy/methods/messages/send_message.py
+-rw-rw-rw-   0        0        0     1266 2024-02-25 13:35:46.000000 rubpy-7.0.2b3/rubpy/methods/messages/send_music.py
+-rw-rw-rw-   0        0        0     1492 2024-02-25 13:35:55.000000 rubpy-7.0.2b3/rubpy/methods/messages/send_photo.py
+-rw-rw-rw-   0        0        0     1785 2024-02-25 13:45:22.000000 rubpy-7.0.2b3/rubpy/methods/messages/send_sticker.py
+-rw-rw-rw-   0        0        0     1236 2024-02-25 13:45:25.000000 rubpy-7.0.2b3/rubpy/methods/messages/send_video.py
+-rw-rw-rw-   0        0        0     1374 2024-02-25 13:45:23.000000 rubpy-7.0.2b3/rubpy/methods/messages/send_video_message.py
+-rw-rw-rw-   0        0        0     1384 2024-02-25 13:44:36.000000 rubpy-7.0.2b3/rubpy/methods/messages/send_voice.py
+-rw-rw-rw-   0        0        0     2422 2024-02-25 13:43:55.000000 rubpy-7.0.2b3/rubpy/methods/messages/set_pin_message.py
+-rw-rw-rw-   0        0        0      799 2024-02-25 13:44:20.000000 rubpy-7.0.2b3/rubpy/methods/messages/vote_poll.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:48.014516 rubpy-7.0.2b3/rubpy/methods/settings/
+-rw-rw-rw-   0        0        0      878 2023-12-22 15:33:50.000000 rubpy-7.0.2b3/rubpy/methods/settings/__init__.py
+-rw-rw-rw-   0        0        0      746 2024-02-25 13:16:01.000000 rubpy-7.0.2b3/rubpy/methods/settings/delete_folder.py
+-rw-rw-rw-   0        0        0      586 2024-02-25 13:17:26.000000 rubpy-7.0.2b3/rubpy/methods/settings/get_blocked_users.py
+-rw-rw-rw-   0        0        0      832 2024-02-25 13:17:43.000000 rubpy-7.0.2b3/rubpy/methods/settings/get_folders.py
+-rw-rw-rw-   0        0        0      660 2024-02-25 13:18:03.000000 rubpy-7.0.2b3/rubpy/methods/settings/get_my_sessions.py
+-rw-rw-rw-   0        0        0      640 2024-02-25 13:18:19.000000 rubpy-7.0.2b3/rubpy/methods/settings/get_privacy_setting.py
+-rw-rw-rw-   0        0        0      648 2024-02-25 13:18:36.000000 rubpy-7.0.2b3/rubpy/methods/settings/get_suggested_folders.py
+-rw-rw-rw-   0        0        0      662 2024-02-25 13:18:52.000000 rubpy-7.0.2b3/rubpy/methods/settings/get_two_passcode_status.py
+-rw-rw-rw-   0        0        0     3312 2024-02-25 13:19:21.000000 rubpy-7.0.2b3/rubpy/methods/settings/set_setting.py
+-rw-rw-rw-   0        0        0     1267 2024-02-25 13:20:00.000000 rubpy-7.0.2b3/rubpy/methods/settings/setup_two_step_verification.py
+-rw-rw-rw-   0        0        0      801 2024-02-25 13:20:16.000000 rubpy-7.0.2b3/rubpy/methods/settings/terminate_session.py
+-rw-rw-rw-   0        0        0     1663 2024-02-25 13:20:39.000000 rubpy-7.0.2b3/rubpy/methods/settings/update_profile.py
+-rw-rw-rw-   0        0        0      745 2024-02-25 13:20:56.000000 rubpy-7.0.2b3/rubpy/methods/settings/update_username.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:48.053643 rubpy-7.0.2b3/rubpy/methods/stickers/
+-rw-rw-rw-   0        0        0      578 2023-12-22 16:07:24.000000 rubpy-7.0.2b3/rubpy/methods/stickers/__init__.py
+-rw-rw-rw-   0        0        0     1283 2024-02-25 13:08:37.000000 rubpy-7.0.2b3/rubpy/methods/stickers/action_on_sticker_set.py
+-rw-rw-rw-   0        0        0      564 2024-02-25 13:09:11.000000 rubpy-7.0.2b3/rubpy/methods/stickers/get_my_sticker_sets.py
+-rw-rw-rw-   0        0        0      778 2024-02-25 13:09:47.000000 rubpy-7.0.2b3/rubpy/methods/stickers/get_sticker_set_by_id.py
+-rw-rw-rw-   0        0        0      877 2024-02-25 13:45:26.000000 rubpy-7.0.2b3/rubpy/methods/stickers/get_stickers_by_emoji.py
+-rw-rw-rw-   0        0        0      941 2024-02-25 13:14:21.000000 rubpy-7.0.2b3/rubpy/methods/stickers/get_stickers_by_set_ids.py
+-rw-rw-rw-   0        0        0      766 2024-02-25 13:14:11.000000 rubpy-7.0.2b3/rubpy/methods/stickers/get_trend_sticker_sets.py
+-rw-rw-rw-   0        0        0      929 2024-02-25 13:14:28.000000 rubpy-7.0.2b3/rubpy/methods/stickers/search_stickers.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:48.097608 rubpy-7.0.2b3/rubpy/methods/users/
+-rw-rw-rw-   0        0        0      331 2023-12-19 22:35:32.000000 rubpy-7.0.2b3/rubpy/methods/users/__init__.py
+-rw-rw-rw-   0        0        0      713 2024-02-25 13:03:33.000000 rubpy-7.0.2b3/rubpy/methods/users/check_user_username.py
+-rw-rw-rw-   0        0        0     1042 2024-02-25 13:04:30.000000 rubpy-7.0.2b3/rubpy/methods/users/delete_user_chat.py
+-rw-rw-rw-   0        0        0      539 2024-02-25 13:05:08.000000 rubpy-7.0.2b3/rubpy/methods/users/get_me.py
+-rw-rw-rw-   0        0        0      881 2024-02-26 15:47:56.000000 rubpy-7.0.2b3/rubpy/methods/users/get_user_info.py
+-rw-rw-rw-   0        0        0     1265 2024-02-25 13:06:50.000000 rubpy-7.0.2b3/rubpy/methods/users/set_block_user.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:48.161367 rubpy-7.0.2b3/rubpy/methods/utilities/
+-rw-rw-rw-   0        0        0      613 2024-01-12 14:48:33.000000 rubpy-7.0.2b3/rubpy/methods/utilities/__init__.py
+-rw-rw-rw-   0        0        0      762 2024-02-25 12:47:55.000000 rubpy-7.0.2b3/rubpy/methods/utilities/add_handler.py
+-rw-rw-rw-   0        0        0      741 2024-04-01 23:10:22.000000 rubpy-7.0.2b3/rubpy/methods/utilities/audio.py
+-rw-rw-rw-   0        0        0      708 2024-02-26 14:31:15.000000 rubpy-7.0.2b3/rubpy/methods/utilities/connect.py
+-rw-rw-rw-   0        0        0      574 2024-02-25 12:48:51.000000 rubpy-7.0.2b3/rubpy/methods/utilities/disconnect.py
+-rw-rw-rw-   0        0        0     1756 2024-04-24 22:13:20.000000 rubpy-7.0.2b3/rubpy/methods/utilities/download.py
+-rw-rw-rw-   0        0        0     1080 2024-03-20 23:17:03.000000 rubpy-7.0.2b3/rubpy/methods/utilities/download_profile_picture.py
+-rw-rw-rw-   0        0        0     1419 2024-02-25 12:52:55.000000 rubpy-7.0.2b3/rubpy/methods/utilities/get_members.py
+-rw-rw-rw-   0        0        0      337 2024-02-25 12:53:13.000000 rubpy-7.0.2b3/rubpy/methods/utilities/get_updates.py
+-rw-rw-rw-   0        0        0      326 2024-02-25 12:54:09.000000 rubpy-7.0.2b3/rubpy/methods/utilities/remove_handler.py
+-rw-rw-rw-   0        0        0      967 2024-02-25 12:54:38.000000 rubpy-7.0.2b3/rubpy/methods/utilities/run.py
+-rw-rw-rw-   0        0        0     3646 2024-03-09 18:54:30.000000 rubpy-7.0.2b3/rubpy/methods/utilities/start.py
+-rw-rw-rw-   0        0        0     6614 2024-04-06 23:05:13.000000 rubpy-7.0.2b3/rubpy/methods/utilities/thumbnail.py
+-rw-rw-rw-   0        0        0      671 2024-02-25 13:02:33.000000 rubpy-7.0.2b3/rubpy/methods/utilities/upload.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:48.177657 rubpy-7.0.2b3/rubpy/methods/voice_chat/
+-rw-rw-rw-   0        0        0      278 2024-02-25 16:36:44.000000 rubpy-7.0.2b3/rubpy/methods/voice_chat/__init__.py
+-rw-rw-rw-   0        0        0      918 2024-02-24 23:57:22.000000 rubpy-7.0.2b3/rubpy/methods/voice_chat/join_voice_chat.py
+-rw-rw-rw-   0        0        0     1077 2024-02-24 23:55:36.000000 rubpy-7.0.2b3/rubpy/methods/voice_chat/send_group_voice_chat_activity.py
+-rw-rw-rw-   0        0        0     1181 2024-02-25 16:36:50.000000 rubpy-7.0.2b3/rubpy/methods/voice_chat/set_voice_chat_state.py
+-rw-rw-rw-   0        0        0    15334 2024-05-01 22:20:07.000000 rubpy-7.0.2b3/rubpy/network.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:48.196850 rubpy-7.0.2b3/rubpy/parser/
+-rw-rw-rw-   0        0        0       30 2024-01-09 13:49:12.000000 rubpy-7.0.2b3/rubpy/parser/__init__.py
+-rw-rw-rw-   0        0        0     3941 2024-05-01 21:46:53.000000 rubpy-7.0.2b3/rubpy/parser/markdown.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:48.231319 rubpy-7.0.2b3/rubpy/rubino/
+-rw-rw-rw-   0        0        0       26 2024-01-08 21:17:13.000000 rubpy-7.0.2b3/rubpy/rubino/__init__.py
+-rw-rw-rw-   0        0        0    16027 2024-03-14 00:36:15.000000 rubpy-7.0.2b3/rubpy/rubino/client.py
+-rw-rw-rw-   0        0        0     7124 2024-03-13 13:52:56.000000 rubpy-7.0.2b3/rubpy/rubino/thumbnail.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:48.244583 rubpy-7.0.2b3/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-7.0.2b3/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2294 2023-12-19 12:35:20.000000 rubpy-7.0.2b3/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-7.0.2b3/rubpy/sessions/stringSession.py
+-rw-rw-rw-   0        0        0     3430 2024-03-14 02:26:10.000000 rubpy-7.0.2b3/rubpy/sync.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:48.264824 rubpy-7.0.2b3/rubpy/types/
+-rw-rw-rw-   0        0        0       65 2024-02-24 22:46:34.000000 rubpy-7.0.2b3/rubpy/types/__init__.py
+-rw-rw-rw-   0        0        0    30721 2024-04-24 22:04:33.000000 rubpy-7.0.2b3/rubpy/types/update.py
+-rw-rw-rw-   0        0        0     4530 2024-02-24 22:36:34.000000 rubpy-7.0.2b3/rubpy/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:37:47.261375 rubpy-7.0.2b3/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3723 2024-05-01 22:37:46.000000 rubpy-7.0.2b3/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8875 2024-05-01 22:37:47.000000 rubpy-7.0.2b3/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 22:37:46.000000 rubpy-7.0.2b3/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2024-05-01 22:37:46.000000 rubpy-7.0.2b3/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-01 22:37:46.000000 rubpy-7.0.2b3/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 22:37:48.266779 rubpy-7.0.2b3/setup.cfg
+-rw-rw-rw-   0        0        0     1840 2024-05-01 22:36:12.000000 rubpy-7.0.2b3/setup.py
```

### Comparing `rubpy-7.0.2b2/PKG-INFO` & `rubpy-7.0.2b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 7.0.2b2
+Version: 7.0.2b3
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
-Metadata-Version: 2.1 Name: rubpy Version: 7.0.2b2 Summary: A powerful, fast
+Metadata-Version: 2.1 Name: rubpy Version: 7.0.2b3 Summary: A powerful, fast
 and optimal library for making robots in Rubika with sync and async support.
 Home-page: https://github.com/shayanheidari01/rubika Author: Shayan Heidari
 Author-email: contact@shayanheidari.info Keywords:
 rubika,rubpy,chat,bot,robot,asyncio Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `rubpy-7.0.2b2/README.md` & `rubpy-7.0.2b3/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/bots/client.py` & `rubpy-7.0.2b3/rubpy/bots/client.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/bots/types/__init__.py` & `rubpy-7.0.2b3/rubpy/bots/types/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/bots/types/button.py` & `rubpy-7.0.2b3/rubpy/bots/types/button.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/bots/types/message.py` & `rubpy-7.0.2b3/rubpy/bots/types/message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/client.py` & `rubpy-7.0.2b3/rubpy/client.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/crypto/crypto.py` & `rubpy-7.0.2b3/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/enums/chat_access_type.py` & `rubpy-7.0.2b3/rubpy/enums/chat_access_type.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/enums/message_media_type.py` & `rubpy-7.0.2b3/rubpy/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/enums/reaction_type.py` & `rubpy-7.0.2b3/rubpy/enums/reaction_type.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/exceptions.py` & `rubpy-7.0.2b3/rubpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/filters.py` & `rubpy-7.0.2b3/rubpy/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # List of models for internal use
 __models__ = [
     'is_pinned', 'is_mute', 'count_unseen', 'message_id',
     'is_group', 'is_private', 'is_channel', 'is_in_contact',
     'text', 'original_update', 'object_guid', 'author_guid',
     'time', 'reply_message_id', 'is_me', 'is_forward', 'is_text',
     'music', 'file', 'photo', 'sticker', 'video', 'voice',
-    'contact', 'location', 'poll', 'gif']
+    'contact', 'location', 'poll', 'gif', 'is_event']
 
 def create_model(name, base, authorize: list = [], exception: bool = True, *args, **kwargs):
     """
     Create a model dynamically based on the given name and base class.
 
     :param name: Name of the model.
     :param base: Base class for the model.
@@ -371,8 +371,9 @@
 photo: Type[BaseModel]
 video: Type[BaseModel]
 voice: Type[BaseModel]
 contact: Type[BaseModel]
 location: Type[BaseModel]
 poll: Type[BaseModel]
 gif: Type[BaseModel]
-sticker: Type[BaseModel]
+sticker: Type[BaseModel]
+is_event: Type[BaseModel]
```

### Comparing `rubpy-7.0.2b2/rubpy/handlers.py` & `rubpy-7.0.2b3/rubpy/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/__init__.py` & `rubpy-7.0.2b3/rubpy/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/advanced/build.py` & `rubpy-7.0.2b3/rubpy/methods/advanced/build.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/advanced/voice_chat_player.py` & `rubpy-7.0.2b3/rubpy/methods/advanced/voice_chat_player.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/auth/register_device.py` & `rubpy-7.0.2b3/rubpy/methods/auth/register_device.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/auth/send_code.py` & `rubpy-7.0.2b3/rubpy/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/auth/sign_in.py` & `rubpy-7.0.2b3/rubpy/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/__init__.py` & `rubpy-7.0.2b3/rubpy/methods/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/add_channel.py` & `rubpy-7.0.2b3/rubpy/methods/channels/add_channel.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/add_channel_members.py` & `rubpy-7.0.2b3/rubpy/methods/channels/add_channel_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/ban_channel_member.py` & `rubpy-7.0.2b3/rubpy/methods/channels/ban_channel_member.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/channel_preview_by_join_link.py` & `rubpy-7.0.2b3/rubpy/methods/channels/channel_preview_by_join_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/check_channel_username.py` & `rubpy-7.0.2b3/rubpy/methods/channels/check_channel_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/create_channel_voice_chat.py` & `rubpy-7.0.2b3/rubpy/methods/channels/create_channel_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/discard_channel_voice_chat.py` & `rubpy-7.0.2b3/rubpy/methods/channels/discard_channel_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/edit_channel_info.py` & `rubpy-7.0.2b3/rubpy/methods/channels/edit_channel_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/get_banned_group_members.py` & `rubpy-7.0.2b3/rubpy/methods/channels/get_banned_group_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/get_channel_admin_access_list.py` & `rubpy-7.0.2b3/rubpy/methods/channels/get_channel_admin_access_list.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/get_channel_admin_members.py` & `rubpy-7.0.2b3/rubpy/methods/channels/get_channel_admin_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/get_channel_all_members.py` & `rubpy-7.0.2b3/rubpy/methods/channels/get_channel_all_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/join_channel_action.py` & `rubpy-7.0.2b3/rubpy/methods/channels/join_channel_action.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/join_channel_by_link.py` & `rubpy-7.0.2b3/rubpy/methods/channels/join_channel_by_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/remove_channel.py` & `rubpy-7.0.2b3/rubpy/methods/channels/remove_channel.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/seen_channel_messages.py` & `rubpy-7.0.2b3/rubpy/methods/channels/seen_channel_messages.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/set_channel_link.py` & `rubpy-7.0.2b3/rubpy/methods/channels/set_channel_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/set_channel_voice_chat_setting.py` & `rubpy-7.0.2b3/rubpy/methods/channels/set_channel_voice_chat_setting.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/channels/update_channel_username.py` & `rubpy-7.0.2b3/rubpy/methods/channels/update_channel_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/chats/__init__.py` & `rubpy-7.0.2b3/rubpy/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/chats/delete_avatar.py` & `rubpy-7.0.2b3/rubpy/methods/chats/delete_avatar.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/chats/delete_chat_history.py` & `rubpy-7.0.2b3/rubpy/methods/chats/delete_chat_history.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/chats/get_abs_objects.py` & `rubpy-7.0.2b3/rubpy/methods/chats/get_abs_objects.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/chats/get_avatars.py` & `rubpy-7.0.2b3/rubpy/methods/chats/get_avatars.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/chats/get_chats.py` & `rubpy-7.0.2b3/rubpy/methods/chats/get_chats.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/chats/get_chats_updates.py` & `rubpy-7.0.2b3/rubpy/methods/chats/get_chats_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/chats/get_link_from_app_url.py` & `rubpy-7.0.2b3/rubpy/methods/chats/get_link_from_app_url.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/chats/search_chat_messages.py` & `rubpy-7.0.2b3/rubpy/methods/chats/search_chat_messages.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/chats/seen_chats.py` & `rubpy-7.0.2b3/rubpy/methods/chats/seen_chats.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/chats/send_chat_activity.py` & `rubpy-7.0.2b3/rubpy/methods/chats/send_chat_activity.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/chats/set_action_chat.py` & `rubpy-7.0.2b3/rubpy/methods/chats/set_action_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/chats/upload_avatar.py` & `rubpy-7.0.2b3/rubpy/methods/chats/upload_avatar.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/contacts/add_address_book.py` & `rubpy-7.0.2b3/rubpy/methods/contacts/add_address_book.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/contacts/delete_contact.py` & `rubpy-7.0.2b3/rubpy/methods/contacts/delete_contact.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/contacts/get_contacts.py` & `rubpy-7.0.2b3/rubpy/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/contacts/get_contacts_updates.py` & `rubpy-7.0.2b3/rubpy/methods/contacts/get_contacts_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/decorators/on_chat_updates.py` & `rubpy-7.0.2b3/rubpy/methods/decorators/on_chat_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/decorators/on_message_updates.py` & `rubpy-7.0.2b3/rubpy/methods/decorators/on_message_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/decorators/on_remove_notifications.py` & `rubpy-7.0.2b3/rubpy/methods/decorators/on_remove_notifications.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/decorators/on_show_activities.py` & `rubpy-7.0.2b3/rubpy/methods/decorators/on_show_activities.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/decorators/on_show_notifications.py` & `rubpy-7.0.2b3/rubpy/methods/decorators/on_show_notifications.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/extras/__init__.py` & `rubpy-7.0.2b3/rubpy/methods/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/extras/ban_member.py` & `rubpy-7.0.2b3/rubpy/methods/extras/ban_member.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/extras/get_info.py` & `rubpy-7.0.2b3/rubpy/methods/extras/get_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/extras/get_object_by_username.py` & `rubpy-7.0.2b3/rubpy/methods/extras/get_object_by_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/extras/get_profile_link_items.py` & `rubpy-7.0.2b3/rubpy/methods/extras/get_profile_link_items.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/extras/get_related_objects.py` & `rubpy-7.0.2b3/rubpy/methods/extras/get_related_objects.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/extras/get_transcription.py` & `rubpy-7.0.2b3/rubpy/methods/extras/get_transcription.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/extras/join.py` & `rubpy-7.0.2b3/rubpy/methods/extras/join.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/extras/leave_chat.py` & `rubpy-7.0.2b3/rubpy/methods/extras/leave_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/extras/report_object.py` & `rubpy-7.0.2b3/rubpy/methods/extras/report_object.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/extras/search_global_objects.py` & `rubpy-7.0.2b3/rubpy/methods/extras/search_global_objects.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/extras/transcribe_voice.py` & `rubpy-7.0.2b3/rubpy/methods/extras/transcribe_voice.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/extras/user_is_admin.py` & `rubpy-7.0.2b3/rubpy/methods/extras/user_is_admin.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/gif/add_to_my_gif_set.py` & `rubpy-7.0.2b3/rubpy/methods/gif/add_to_my_gif_set.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/__init__.py` & `rubpy-7.0.2b3/rubpy/methods/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/add_group.py` & `rubpy-7.0.2b3/rubpy/methods/groups/add_group.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/add_group_members.py` & `rubpy-7.0.2b3/rubpy/methods/groups/add_group_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/ban_group_member.py` & `rubpy-7.0.2b3/rubpy/methods/groups/ban_group_member.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/create_group_voice_chat.py` & `rubpy-7.0.2b3/rubpy/methods/groups/create_group_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/delete_no_access_group_chat.py` & `rubpy-7.0.2b3/rubpy/methods/groups/delete_no_access_group_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/edit_group_info.py` & `rubpy-7.0.2b3/rubpy/methods/groups/edit_group_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/get_banned_group_members.py` & `rubpy-7.0.2b3/rubpy/methods/groups/get_banned_group_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/get_group_admin_access_list.py` & `rubpy-7.0.2b3/rubpy/methods/groups/get_group_admin_access_list.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/get_group_admin_members.py` & `rubpy-7.0.2b3/rubpy/methods/groups/get_group_admin_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/get_group_all_members.py` & `rubpy-7.0.2b3/rubpy/methods/groups/get_group_all_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/get_group_default_access.py` & `rubpy-7.0.2b3/rubpy/methods/groups/get_group_default_access.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/get_group_info.py` & `rubpy-7.0.2b3/rubpy/methods/groups/get_group_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/get_group_link.py` & `rubpy-7.0.2b3/rubpy/methods/groups/get_group_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/get_group_mention_list.py` & `rubpy-7.0.2b3/rubpy/methods/groups/get_group_mention_list.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/get_group_voice_chat_updates.py` & `rubpy-7.0.2b3/rubpy/methods/groups/get_group_voice_chat_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/group_preview_by_join_link.py` & `rubpy-7.0.2b3/rubpy/methods/groups/group_preview_by_join_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/join_group.py` & `rubpy-7.0.2b3/rubpy/methods/groups/join_group.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/leave_group_voice_chat.py` & `rubpy-7.0.2b3/rubpy/methods/groups/leave_group_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/set_group_admin.py` & `rubpy-7.0.2b3/rubpy/methods/groups/set_group_admin.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/set_group_default_access.py` & `rubpy-7.0.2b3/rubpy/methods/groups/set_group_default_access.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/set_group_link.py` & `rubpy-7.0.2b3/rubpy/methods/groups/set_group_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/groups/set_group_voice_chat_setting.py` & `rubpy-7.0.2b3/rubpy/methods/groups/set_group_voice_chat_setting.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/__init__.py` & `rubpy-7.0.2b3/rubpy/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/action_on_message_reaction.py` & `rubpy-7.0.2b3/rubpy/methods/messages/action_on_message_reaction.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/auto_delete_message.py` & `rubpy-7.0.2b3/rubpy/methods/messages/auto_delete_message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/create_poll.py` & `rubpy-7.0.2b3/rubpy/methods/messages/create_poll.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/delete_messages.py` & `rubpy-7.0.2b3/rubpy/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/edit_message.py` & `rubpy-7.0.2b3/rubpy/methods/messages/edit_message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/forward_messages.py` & `rubpy-7.0.2b3/rubpy/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/get_message_share_url.py` & `rubpy-7.0.2b3/rubpy/methods/messages/get_message_share_url.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/get_messages_by_id.py` & `rubpy-7.0.2b3/rubpy/methods/messages/get_messages_by_id.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/get_messages_interval.py` & `rubpy-7.0.2b3/rubpy/methods/messages/get_messages_interval.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/get_messages_updates.py` & `rubpy-7.0.2b3/rubpy/methods/messages/get_messages_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/get_poll_option_voters.py` & `rubpy-7.0.2b3/rubpy/methods/messages/get_poll_option_voters.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/get_poll_status.py` & `rubpy-7.0.2b3/rubpy/methods/messages/get_poll_status.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/reaction.py` & `rubpy-7.0.2b3/rubpy/methods/messages/reaction.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/remove_reaction.py` & `rubpy-7.0.2b3/rubpy/methods/messages/remove_reaction.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/request_send_file.py` & `rubpy-7.0.2b3/rubpy/methods/messages/request_send_file.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/send_document.py` & `rubpy-7.0.2b3/rubpy/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/send_gif.py` & `rubpy-7.0.2b3/rubpy/methods/messages/send_gif.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/send_message.py` & `rubpy-7.0.2b3/rubpy/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/send_music.py` & `rubpy-7.0.2b3/rubpy/methods/messages/send_music.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/send_photo.py` & `rubpy-7.0.2b3/rubpy/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/send_sticker.py` & `rubpy-7.0.2b3/rubpy/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/send_video.py` & `rubpy-7.0.2b3/rubpy/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/send_video_message.py` & `rubpy-7.0.2b3/rubpy/methods/messages/send_video_message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/send_voice.py` & `rubpy-7.0.2b3/rubpy/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/set_pin_message.py` & `rubpy-7.0.2b3/rubpy/methods/messages/set_pin_message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/messages/vote_poll.py` & `rubpy-7.0.2b3/rubpy/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/settings/__init__.py` & `rubpy-7.0.2b3/rubpy/methods/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/settings/delete_folder.py` & `rubpy-7.0.2b3/rubpy/methods/settings/delete_folder.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/settings/get_blocked_users.py` & `rubpy-7.0.2b3/rubpy/methods/settings/get_blocked_users.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/settings/get_folders.py` & `rubpy-7.0.2b3/rubpy/methods/settings/get_folders.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/settings/get_my_sessions.py` & `rubpy-7.0.2b3/rubpy/methods/settings/get_my_sessions.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/settings/get_privacy_setting.py` & `rubpy-7.0.2b3/rubpy/methods/settings/get_privacy_setting.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/settings/get_suggested_folders.py` & `rubpy-7.0.2b3/rubpy/methods/settings/get_suggested_folders.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/settings/get_two_passcode_status.py` & `rubpy-7.0.2b3/rubpy/methods/settings/get_two_passcode_status.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/settings/set_setting.py` & `rubpy-7.0.2b3/rubpy/methods/settings/set_setting.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/settings/setup_two_step_verification.py` & `rubpy-7.0.2b3/rubpy/methods/settings/setup_two_step_verification.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/settings/terminate_session.py` & `rubpy-7.0.2b3/rubpy/methods/settings/terminate_session.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/settings/update_profile.py` & `rubpy-7.0.2b3/rubpy/methods/settings/update_profile.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/settings/update_username.py` & `rubpy-7.0.2b3/rubpy/methods/settings/update_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/stickers/__init__.py` & `rubpy-7.0.2b3/rubpy/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/stickers/action_on_sticker_set.py` & `rubpy-7.0.2b3/rubpy/methods/stickers/action_on_sticker_set.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/stickers/get_my_sticker_sets.py` & `rubpy-7.0.2b3/rubpy/methods/stickers/get_my_sticker_sets.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/stickers/get_sticker_set_by_id.py` & `rubpy-7.0.2b3/rubpy/methods/stickers/get_sticker_set_by_id.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/stickers/get_stickers_by_emoji.py` & `rubpy-7.0.2b3/rubpy/methods/stickers/get_stickers_by_emoji.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/stickers/get_stickers_by_set_ids.py` & `rubpy-7.0.2b3/rubpy/methods/stickers/get_stickers_by_set_ids.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/stickers/get_trend_sticker_sets.py` & `rubpy-7.0.2b3/rubpy/methods/stickers/get_trend_sticker_sets.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/stickers/search_stickers.py` & `rubpy-7.0.2b3/rubpy/methods/stickers/search_stickers.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/users/check_user_username.py` & `rubpy-7.0.2b3/rubpy/methods/users/check_user_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/users/delete_user_chat.py` & `rubpy-7.0.2b3/rubpy/methods/users/delete_user_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/users/get_me.py` & `rubpy-7.0.2b3/rubpy/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/users/get_user_info.py` & `rubpy-7.0.2b3/rubpy/methods/users/get_user_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/users/set_block_user.py` & `rubpy-7.0.2b3/rubpy/methods/users/set_block_user.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/utilities/__init__.py` & `rubpy-7.0.2b3/rubpy/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/utilities/add_handler.py` & `rubpy-7.0.2b3/rubpy/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/utilities/audio.py` & `rubpy-7.0.2b3/rubpy/methods/utilities/audio.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/utilities/connect.py` & `rubpy-7.0.2b3/rubpy/methods/utilities/connect.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/utilities/disconnect.py` & `rubpy-7.0.2b3/rubpy/methods/utilities/disconnect.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/utilities/download.py` & `rubpy-7.0.2b3/rubpy/methods/utilities/download.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/utilities/download_profile_picture.py` & `rubpy-7.0.2b3/rubpy/methods/utilities/download_profile_picture.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/utilities/get_members.py` & `rubpy-7.0.2b3/rubpy/methods/utilities/get_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/utilities/run.py` & `rubpy-7.0.2b3/rubpy/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/utilities/start.py` & `rubpy-7.0.2b3/rubpy/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/utilities/thumbnail.py` & `rubpy-7.0.2b3/rubpy/methods/utilities/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/utilities/upload.py` & `rubpy-7.0.2b3/rubpy/methods/utilities/upload.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/voice_chat/join_voice_chat.py` & `rubpy-7.0.2b3/rubpy/methods/voice_chat/join_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/voice_chat/send_group_voice_chat_activity.py` & `rubpy-7.0.2b3/rubpy/methods/voice_chat/send_group_voice_chat_activity.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/methods/voice_chat/set_voice_chat_state.py` & `rubpy-7.0.2b3/rubpy/methods/voice_chat/set_voice_chat_state.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/network.py` & `rubpy-7.0.2b3/rubpy/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         )
 
         if client.bot_token is not None:
             self.bot_api_url = f'https://messengerg2b1.iranlms.ir/v3/{client.bot_token}/'
 
         self.api_url = None
         self.wss_url = None
+        self.ws = None
 
     async def close(self):
         """
         Close the aiohttp ClientSession.
         """
         await self.session.close()
 
@@ -183,17 +184,19 @@
                     'handler raised an exception',
                     extra={'data': update}, exc_info=True)
 
     async def get_updates(self):
         """
         Receive updates from the Rubika WebSocket.
         """
+        asyncio.create_task(self.keep_socket())
         while True:
             try:
                 async with self.session.ws_connect(self.wss_url, verify_ssl=False, proxy=self.client.proxy, receive_timeout=5) as ws:
+                    self.ws = ws
                     await ws.send_json(dict(method='handShake', auth=self.client.auth, api_version='6', data=''))
 
                     async for msg in ws:
                         if msg.type == aiohttp.WSMsgType.TEXT:
                             asyncio.create_task(self.handle_text_message(msg.json()))
                         elif msg.type == aiohttp.WSMsgType.CLOSED:
                             break
@@ -208,19 +211,19 @@
                 print("Websocket connection lost. Reconnecting...")
                 await asyncio.sleep(5)  # wait before reconnecting
 
             except aiohttp.ClientError:
                 print("Websocket connection lost. Reconnecting...")
                 await asyncio.sleep(5)  # wait before reconnecting
 
-    async def keep_socket(self, ws):
+    async def keep_socket(self):
         while True:
             try:
-                await asyncio.sleep(5)
-                await ws.send_json({})
+                await asyncio.sleep(10)
+                await self.ws.send_json({})
                 await self.client.get_chats_updates()
 
             except Exception:
                 continue
 
     async def handle_text_message(self, msg_data: dict):
         """
```

### Comparing `rubpy-7.0.2b2/rubpy/rubino/client.py` & `rubpy-7.0.2b3/rubpy/rubino/client.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/rubino/thumbnail.py` & `rubpy-7.0.2b3/rubpy/rubino/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/sessions/sqliteSession.py` & `rubpy-7.0.2b3/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/sessions/stringSession.py` & `rubpy-7.0.2b3/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/sync.py` & `rubpy-7.0.2b3/rubpy/sync.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/types/update.py` & `rubpy-7.0.2b3/rubpy/types/update.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy/utils.py` & `rubpy-7.0.2b3/rubpy/utils.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/rubpy.egg-info/PKG-INFO` & `rubpy-7.0.2b3/rubpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 7.0.2b2
+Version: 7.0.2b3
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
-Metadata-Version: 2.1 Name: rubpy Version: 7.0.2b2 Summary: A powerful, fast
+Metadata-Version: 2.1 Name: rubpy Version: 7.0.2b3 Summary: A powerful, fast
 and optimal library for making robots in Rubika with sync and async support.
 Home-page: https://github.com/shayanheidari01/rubika Author: Shayan Heidari
 Author-email: contact@shayanheidari.info Keywords:
 rubika,rubpy,chat,bot,robot,asyncio Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `rubpy-7.0.2b2/rubpy.egg-info/SOURCES.txt` & `rubpy-7.0.2b3/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.2b2/setup.py` & `rubpy-7.0.2b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 
 with open('README.md', encoding='UTF-8') as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '7.0.2b2',
+    version = '7.0.2b3',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'A powerful, fast and optimal library for making robots in Rubika with sync and async support.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires='~=3.7',
     long_description_content_type = 'text/markdown',
```

