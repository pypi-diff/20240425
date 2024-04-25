# Comparing `tmp/pyrogeram-2.0.106.tar.gz` & `tmp/pyrogeram-2.0.107.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrogeram-2.0.106.tar", last modified: Wed Apr 24 15:22:43 2024, max compression
+gzip compressed data, was "pyrogeram-2.0.107.tar", last modified: Wed Apr 24 15:34:39 2024, max compression
```

## Comparing `pyrogeram-2.0.106.tar` & `pyrogeram-2.0.107.tar`

### file list

```diff
@@ -1,588 +1,3193 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.320658 pyrogeram-2.0.106/
--rw-r--r--   0 root         (0) root         (0)      463 2024-04-24 15:22:43.320658 pyrogeram-2.0.106/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.188659 pyrogeram-2.0.106/compiler/
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/compiler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.188659 pyrogeram-2.0.106/compiler/api/
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/compiler/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22560 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/compiler/api/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.188659 pyrogeram-2.0.106/compiler/docs/
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/compiler/docs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23157 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/compiler/docs/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.188659 pyrogeram-2.0.106/compiler/errors/
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/compiler/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4992 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/compiler/errors/compiler.py
--rw-r--r--   0 root         (0) root         (0)     1338 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/compiler/errors/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.316658 pyrogeram-2.0.106/pyrogeram.egg-info/
--rw-r--r--   0 root         (0) root         (0)      463 2024-04-24 15:22:43.000000 pyrogeram-2.0.106/pyrogeram.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    23941 2024-04-24 15:22:43.000000 pyrogeram-2.0.106/pyrogeram.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 15:22:43.000000 pyrogeram-2.0.106/pyrogeram.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2024-04-24 15:22:43.000000 pyrogeram-2.0.106/pyrogeram.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-24 15:22:43.000000 pyrogeram-2.0.106/pyrogeram.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.192659 pyrogeram-2.0.106/pyrogram/
--rw-r--r--   0 root         (0) root         (0)     1517 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44003 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.192659 pyrogeram-2.0.106/pyrogram/connection/
--rw-r--r--   0 root         (0) root         (0)      929 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/connection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2676 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/connection/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.196659 pyrogeram-2.0.106/pyrogram/connection/transport/
--rw-r--r--   0 root         (0) root         (0)      913 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/connection/transport/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.196659 pyrogeram-2.0.106/pyrogram/connection/transport/tcp/
--rw-r--r--   0 root         (0) root         (0)     1119 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4164 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0 root         (0) root         (0)     1843 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 root         (0) root         (0)     2905 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 root         (0) root         (0)     1981 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 root         (0) root         (0)     1586 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 root         (0) root         (0)     2528 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.196659 pyrogeram-2.0.106/pyrogram/crypto/
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/crypto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4092 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/crypto/aes.py
--rw-r--r--   0 root         (0) root         (0)     4093 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/crypto/mtproto.py
--rw-r--r--   0 root         (0) root         (0)     2521 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/crypto/prime.py
--rw-r--r--   0 root         (0) root         (0)    13512 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/crypto/rsa.py
--rw-r--r--   0 root         (0) root         (0)    13763 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)   208096 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/emoji.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.208659 pyrogeram-2.0.106/pyrogram/enums/
--rw-r--r--   0 root         (0) root         (0)     2262 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/auto_name.py
--rw-r--r--   0 root         (0) root         (0)     1261 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/business_schedule.py
--rw-r--r--   0 root         (0) root         (0)     2382 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/chat_action.py
--rw-r--r--   0 root         (0) root         (0)     4595 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/chat_event_action.py
--rw-r--r--   0 root         (0) root         (0)     1340 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/chat_member_status.py
--rw-r--r--   0 root         (0) root         (0)     1521 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0 root         (0) root         (0)     1313 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/chat_type.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/listerner_types.py
--rw-r--r--   0 root         (0) root         (0)     2539 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/message_entity_type.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/message_media_type.py
--rw-r--r--   0 root         (0) root         (0)     2794 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/message_service_type.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/messages_filter.py
--rw-r--r--   0 root         (0) root         (0)     1596 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/next_code_type.py
--rw-r--r--   0 root         (0) root         (0)     1263 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/parse_mode.py
--rw-r--r--   0 root         (0) root         (0)     1122 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/poll_type.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/profile_color.py
--rw-r--r--   0 root         (0) root         (0)     1110 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/reaction_type.py
--rw-r--r--   0 root         (0) root         (0)     2470 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/reply_color.py
--rw-r--r--   0 root         (0) root         (0)     1798 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/sent_code_type.py
--rw-r--r--   0 root         (0) root         (0)     1308 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/stories_privacy_rules.py
--rw-r--r--   0 root         (0) root         (0)     1246 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/story_privacy.py
--rw-r--r--   0 root         (0) root         (0)     1374 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/enums/user_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.208659 pyrogeram-2.0.106/pyrogram/errors/
--rw-r--r--   0 root         (0) root         (0)     2703 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/errors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.208659 pyrogeram-2.0.106/pyrogram/errors/pyromod/
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/errors/pyromod/__init__.py
--rw-r--r--   0 root         (0) root         (0)       42 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/errors/pyromod/listener_stopped.py
--rw-r--r--   0 root         (0) root         (0)       42 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/errors/pyromod/listener_timeout.py
--rw-r--r--   0 root         (0) root         (0)     3390 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/errors/rpc_error.py
--rw-r--r--   0 root         (0) root         (0)    15229 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/file_id.py
--rw-r--r--   0 root         (0) root         (0)    27537 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.212659 pyrogeram-2.0.106/pyrogram/handlers/
--rw-r--r--   0 root         (0) root         (0)     2108 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2049 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/bot_business_connect_handler.py
--rw-r--r--   0 root         (0) root         (0)     6152 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/bot_business_message_handler.py
--rw-r--r--   0 root         (0) root         (0)     7959 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0 root         (0) root         (0)     2086 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0 root         (0) root         (0)     2176 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 root         (0) root         (0)     2514 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/conversation_handler.py
--rw-r--r--   0 root         (0) root         (0)     2655 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/deleted_bot_business_messages_handler.py
--rw-r--r--   0 root         (0) root         (0)     2618 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0 root         (0) root         (0)     1777 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0 root         (0) root         (0)     2109 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/edited_bot_business_message_handler.py
--rw-r--r--   0 root         (0) root         (0)     2054 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0 root         (0) root         (0)     1625 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/handler.py
--rw-r--r--   0 root         (0) root         (0)     2059 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0 root         (0) root         (0)     6102 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/message_handler.py
--rw-r--r--   0 root         (0) root         (0)     2217 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/message_reaction_count_updated_handler.py
--rw-r--r--   0 root         (0) root         (0)     2163 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/message_reaction_updated_handler.py
--rw-r--r--   0 root         (0) root         (0)     1989 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/poll_handler.py
--rw-r--r--   0 root         (0) root         (0)     3017 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0 root         (0) root         (0)     1926 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/story_handler.py
--rw-r--r--   0 root         (0) root         (0)     2064 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/handlers/user_status_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.212659 pyrogeram-2.0.106/pyrogram/helpers/
--rw-r--r--   0 root         (0) root         (0)      813 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3479 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/helpers/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.216659 pyrogeram-2.0.106/pyrogram/methods/
--rw-r--r--   0 root         (0) root         (0)     1482 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.216659 pyrogeram-2.0.106/pyrogram/methods/advanced/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3208 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0 root         (0) root         (0)     4733 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0 root         (0) root         (0)     8496 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/advanced/save_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.220659 pyrogeram-2.0.106/pyrogram/methods/auth/
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1543 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 root         (0) root         (0)     2017 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/check_password.py
--rw-r--r--   0 root         (0) root         (0)     1824 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/connect.py
--rw-r--r--   0 root         (0) root         (0)     1579 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0 root         (0) root         (0)     1382 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0 root         (0) root         (0)     1837 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1701 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/log_out.py
--rw-r--r--   0 root         (0) root         (0)     1906 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0 root         (0) root         (0)     2225 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0 root         (0) root         (0)     2861 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/send_code.py
--rw-r--r--   0 root         (0) root         (0)     1548 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0 root         (0) root         (0)     3160 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0 root         (0) root         (0)     2798 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0 root         (0) root         (0)     2430 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0 root         (0) root         (0)     2117 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/auth/terminate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.224659 pyrogeram-2.0.106/pyrogram/methods/bots/
--rw-r--r--   0 root         (0) root         (0)     2222 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3386 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0 root         (0) root         (0)     5065 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0 root         (0) root         (0)     2064 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0 root         (0) root         (0)     2435 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     2648 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     2126 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 root         (0) root         (0)     1811 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/get_bot_info.py
--rw-r--r--   0 root         (0) root         (0)     2493 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 root         (0) root         (0)     2960 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0 root         (0) root         (0)     3526 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0 root         (0) root         (0)     5185 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/send_game.py
--rw-r--r--   0 root         (0) root         (0)     4325 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 root         (0) root         (0)     2785 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     3261 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2146 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/set_bot_info.py
--rw-r--r--   0 root         (0) root         (0)     2123 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 root         (0) root         (0)     4108 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/bots/set_game_score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.236658 pyrogeram-2.0.106/pyrogram/methods/chats/
--rw-r--r--   0 root         (0) root         (0)     4429 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3554 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0 root         (0) root         (0)     2377 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0 root         (0) root         (0)     4913 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1943 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/close_forum_topic.py
--rw-r--r--   0 root         (0) root         (0)     1806 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/close_general_topic.py
--rw-r--r--   0 root         (0) root         (0)     1892 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0 root         (0) root         (0)     2421 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/create_forum_topic.py
--rw-r--r--   0 root         (0) root         (0)     2356 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/create_group.py
--rw-r--r--   0 root         (0) root         (0)     2030 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0 root         (0) root         (0)     1746 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0 root         (0) root         (0)     2468 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     2038 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/delete_forum_topic.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0 root         (0) root         (0)     2217 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0 root         (0) root         (0)     2272 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/edit_forum_topic.py
--rw-r--r--   0 root         (0) root         (0)     1925 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/edit_general_topic.py
--rw-r--r--   0 root         (0) root         (0)     3469 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0 root         (0) root         (0)     4193 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0 root         (0) root         (0)     3586 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     5443 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0 root         (0) root         (0)     2425 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0 root         (0) root         (0)     1884 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0 root         (0) root         (0)     3571 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0 root         (0) root         (0)     2171 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0 root         (0) root         (0)     2446 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/get_forum_topics.py
--rw-r--r--   0 root         (0) root         (0)     3306 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/get_forum_topics_by_id.py
--rw-r--r--   0 root         (0) root         (0)     2476 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0 root         (0) root         (0)     2312 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0 root         (0) root         (0)     1810 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/hide_general_topic.py
--rw-r--r--   0 root         (0) root         (0)     2790 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0 root         (0) root         (0)     2766 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0 root         (0) root         (0)     3318 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0 root         (0) root         (0)     4363 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1948 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/reopen_forum_topic.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/reopen_general_topic.py
--rw-r--r--   0 root         (0) root         (0)     9697 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     3384 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0 root         (0) root         (0)     2408 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0 root         (0) root         (0)     8713 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0 root         (0) root         (0)     4762 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     1883 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 root         (0) root         (0)     2733 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0 root         (0) root         (0)     2229 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0 root         (0) root         (0)     2239 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0 root         (0) root         (0)     2391 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0 root         (0) root         (0)     2466 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1819 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/unhide_general_topic.py
--rw-r--r--   0 root         (0) root         (0)     2101 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 root         (0) root         (0)     2300 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/unpin_chat_message.py
--rw-r--r--   0 root         (0) root         (0)     2683 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/chats/update_color.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.236658 pyrogeram-2.0.106/pyrogram/methods/contacts/
--rw-r--r--   0 root         (0) root         (0)     1229 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2728 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0 root         (0) root         (0)     2610 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1497 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0 root         (0) root         (0)     2009 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/contacts/import_contacts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.240658 pyrogeram-2.0.106/pyrogram/methods/decorators/
--rw-r--r--   0 root         (0) root         (0)     2330 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2215 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_bot_business_connect.py
--rw-r--r--   0 root         (0) root         (0)     2283 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_bot_business_message.py
--rw-r--r--   0 root         (0) root         (0)     2256 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0 root         (0) root         (0)     2244 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2265 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 root         (0) root         (0)     2292 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 root         (0) root         (0)     2328 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_deleted_bot_business_messages.py
--rw-r--r--   0 root         (0) root         (0)     2258 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 root         (0) root         (0)     1628 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0 root         (0) root         (0)     2304 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_edited_bot_business_message.py
--rw-r--r--   0 root         (0) root         (0)     2247 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0 root         (0) root         (0)     2213 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0 root         (0) root         (0)     2324 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_message_reaction_count_updated.py
--rw-r--r--   0 root         (0) root         (0)     2288 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_message_reaction_updated.py
--rw-r--r--   0 root         (0) root         (0)     2195 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0 root         (0) root         (0)     2136 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_story.py
--rw-r--r--   0 root         (0) root         (0)     2229 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/decorators/on_user_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.244658 pyrogeram-2.0.106/pyrogram/methods/invite_links/
--rw-r--r--   0 root         (0) root         (0)     2510 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2055 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     2172 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     3530 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     2056 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     2173 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2279 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     1912 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     3694 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     2743 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     3814 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     2583 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 root         (0) root         (0)     2158 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     2086 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     3089 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 root         (0) root         (0)     2090 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 root         (0) root         (0)     3108 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     2490 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.256658 pyrogeram-2.0.106/pyrogram/methods/messages/
--rw-r--r--   0 root         (0) root         (0)     4052 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6983 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0 root         (0) root         (0)     5903 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0 root         (0) root         (0)     3309 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0 root         (0) root         (0)     7693 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/download_media.py
--rw-r--r--   0 root         (0) root         (0)     2346 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0 root         (0) root         (0)    10450 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0 root         (0) root         (0)     2539 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 root         (0) root         (0)     3190 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0 root         (0) root         (0)     3139 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0 root         (0) root         (0)    13183 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0 root         (0) root         (0)     3137 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 root         (0) root         (0)     4067 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     5265 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0 root         (0) root         (0)     4662 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0 root         (0) root         (0)     2550 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0 root         (0) root         (0)     2369 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 root         (0) root         (0)     2390 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0 root         (0) root         (0)     2969 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0 root         (0) root         (0)     2111 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 root         (0) root         (0)     3107 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0 root         (0) root         (0)     4902 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0 root         (0) root         (0)     2688 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0 root         (0) root         (0)     2285 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0 root         (0) root         (0)     4235 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/search_global.py
--rw-r--r--   0 root         (0) root         (0)     2231 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0 root         (0) root         (0)     5510 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0 root         (0) root         (0)     3364 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0 root         (0) root         (0)    15042 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0 root         (0) root         (0)    13506 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0 root         (0) root         (0)     7520 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0 root         (0) root         (0)     3660 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0 root         (0) root         (0)     7244 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0 root         (0) root         (0)     7437 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0 root         (0) root         (0)    12856 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_document.py
--rw-r--r--   0 root         (0) root         (0)     6953 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_location.py
--rw-r--r--   0 root         (0) root         (0)    23444 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0 root         (0) root         (0)     9721 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_message.py
--rw-r--r--   0 root         (0) root         (0)    11874 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0 root         (0) root         (0)    10382 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0 root         (0) root         (0)     5073 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_reaction.py
--rw-r--r--   0 root         (0) root         (0)    11062 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0 root         (0) root         (0)     7754 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0 root         (0) root         (0)    14390 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_video.py
--rw-r--r--   0 root         (0) root         (0)    12476 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0 root         (0) root         (0)    11938 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0 root         (0) root         (0)     8669 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/send_web_page.py
--rw-r--r--   0 root         (0) root         (0)     2980 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0 root         (0) root         (0)     4012 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0 root         (0) root         (0)     2665 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/messages/vote_poll.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.256658 pyrogeram-2.0.106/pyrogram/methods/password/
--rw-r--r--   0 root         (0) root         (0)     1163 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2872 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0 root         (0) root         (0)     3081 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0 root         (0) root         (0)     2218 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.260658 pyrogeram-2.0.106/pyrogram/methods/pyromod/
--rw-r--r--   0 root         (0) root         (0)     1886 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/pyromod/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3851 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/pyromod/ask.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/pyromod/get_listener_matching_with_data.py
--rw-r--r--   0 root         (0) root         (0)     2504 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/pyromod/get_listener_matching_with_identifier_pattern.py
--rw-r--r--   0 root         (0) root         (0)     1884 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/pyromod/get_many_listeners_matching_with_data.py
--rw-r--r--   0 root         (0) root         (0)     2266 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/pyromod/get_many_listeners_matching_with_identifier_pattern.py
--rw-r--r--   0 root         (0) root         (0)     4546 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/pyromod/listen.py
--rw-r--r--   0 root         (0) root         (0)     3303 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/pyromod/register_next_step_handler.py
--rw-r--r--   0 root         (0) root         (0)     1454 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/pyromod/remove_listerner.py
--rw-r--r--   0 root         (0) root         (0)     2106 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/pyromod/stop_listener.py
--rw-r--r--   0 root         (0) root         (0)     2773 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/pyromod/stop_listening.py
--rw-r--r--   0 root         (0) root         (0)     2996 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/pyromod/wait_for_callback_query.py
--rw-r--r--   0 root         (0) root         (0)     2921 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/pyromod/wait_for_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.260658 pyrogeram-2.0.106/pyrogram/methods/stickers/
--rw-r--r--   0 root         (0) root         (0)     1058 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2793 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/stickers/add_sticker_to_set.py
--rw-r--r--   0 root         (0) root         (0)     4301 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/stickers/create_sticker_set.py
--rw-r--r--   0 root         (0) root         (0)     1735 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/stickers/get_sticker_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.268658 pyrogeram-2.0.106/pyrogram/methods/users/
--rw-r--r--   0 root         (0) root         (0)     2421 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1933 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/block_user.py
--rw-r--r--   0 root         (0) root         (0)     2312 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0 root         (0) root         (0)     2556 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/delete_stories.py
--rw-r--r--   0 root         (0) root         (0)    10868 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/edit_story.py
--rw-r--r--   0 root         (0) root         (0)     2381 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/export_story_link.py
--rw-r--r--   0 root         (0) root         (0)     4786 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/forward_story.py
--rw-r--r--   0 root         (0) root         (0)     1889 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/get_all_stories.py
--rw-r--r--   0 root         (0) root         (0)     4595 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0 root         (0) root         (0)     2683 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0 root         (0) root         (0)     2521 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0 root         (0) root         (0)     1739 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 root         (0) root         (0)     1640 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/get_me.py
--rw-r--r--   0 root         (0) root         (0)     2445 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/get_peer_stories.py
--rw-r--r--   0 root         (0) root         (0)     3022 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/get_stories.py
--rw-r--r--   0 root         (0) root         (0)     2620 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/get_stories_history.py
--rw-r--r--   0 root         (0) root         (0)     2724 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/get_users.py
--rw-r--r--   0 root         (0) root         (0)    11065 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/send_story.py
--rw-r--r--   0 root         (0) root         (0)     1957 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0 root         (0) root         (0)     2793 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/set_username.py
--rw-r--r--   0 root         (0) root         (0)     1943 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/update_birthday.py
--rw-r--r--   0 root         (0) root         (0)     1771 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/update_personal_chat.py
--rw-r--r--   0 root         (0) root         (0)     2455 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/users/update_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.268658 pyrogeram-2.0.106/pyrogram/methods/utilities/
--rw-r--r--   0 root         (0) root         (0)     1371 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2421 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0 root         (0) root         (0)     2307 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/utilities/compose.py
--rw-r--r--   0 root         (0) root         (0)     1632 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0 root         (0) root         (0)     2825 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/utilities/idle.py
--rw-r--r--   0 root         (0) root         (0)     2285 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0 root         (0) root         (0)     2369 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/utilities/restart.py
--rw-r--r--   0 root         (0) root         (0)     2932 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/utilities/run.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/utilities/run_sync.py
--rw-r--r--   0 root         (0) root         (0)     2439 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/utilities/start.py
--rw-r--r--   0 root         (0) root         (0)     2192 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/utilities/stop.py
--rw-r--r--   0 root         (0) root         (0)     1799 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0 root         (0) root         (0)    61990 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/mime_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.272658 pyrogeram-2.0.106/pyrogram/nav/
--rw-r--r--   0 root         (0) root         (0)      923 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/nav/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3591 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/nav/pagination.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.272658 pyrogeram-2.0.106/pyrogram/parser/
--rw-r--r--   0 root         (0) root         (0)      921 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8759 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/parser/html.py
--rw-r--r--   0 root         (0) root         (0)     7642 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/parser/markdown.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     1620 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/parser/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.272658 pyrogeram-2.0.106/pyrogram/raw/
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.272658 pyrogeram-2.0.106/pyrogram/raw/core/
--rw-r--r--   0 root         (0) root         (0)     1387 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1767 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/future_salt.py
--rw-r--r--   0 root         (0) root         (0)     1966 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/future_salts.py
--rw-r--r--   0 root         (0) root         (0)     1889 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0 root         (0) root         (0)     1123 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/list.py
--rw-r--r--   0 root         (0) root         (0)     1926 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/message.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/msg_container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.276658 pyrogeram-2.0.106/pyrogram/raw/core/primitives/
--rw-r--r--   0 root         (0) root         (0)     1087 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1572 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0 root         (0) root         (0)     1834 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0 root         (0) root         (0)     1268 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0 root         (0) root         (0)     1433 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0 root         (0) root         (0)     1269 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0 root         (0) root         (0)     2492 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0 root         (0) root         (0)     2570 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/raw/core/tl_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.276658 pyrogeram-2.0.106/pyrogram/session/
--rw-r--r--   0 root         (0) root         (0)      946 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/session/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11576 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/session/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.276658 pyrogeram-2.0.106/pyrogram/session/internals/
--rw-r--r--   0 root         (0) root         (0)      992 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/session/internals/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2564 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/session/internals/data_center.py
--rw-r--r--   0 root         (0) root         (0)     1449 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0 root         (0) root         (0)     1231 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/session/internals/msg_id.py
--rw-r--r--   0 root         (0) root         (0)     1237 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/session/internals/seq_no.py
--rw-r--r--   0 root         (0) root         (0)    14152 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/session/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.280658 pyrogeram-2.0.106/pyrogram/storage/
--rw-r--r--   0 root         (0) root         (0)     1104 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2165 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/storage/dummy_client.py
--rw-r--r--   0 root         (0) root         (0)     2034 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/storage/file_storage.py
--rw-r--r--   0 root         (0) root         (0)     2825 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/storage/memory_storage.py
--rw-r--r--   0 root         (0) root         (0)     8229 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/storage/mongo_storage.py
--rw-r--r--   0 root         (0) root         (0)     7895 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     2963 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/storage/storage.py
--rw-r--r--   0 root         (0) root         (0)     3814 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.280658 pyrogeram-2.0.106/pyrogram/types/
--rw-r--r--   0 root         (0) root         (0)     1207 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.280658 pyrogeram-2.0.106/pyrogram/types/authorization/
--rw-r--r--   0 root         (0) root         (0)     1013 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/authorization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2363 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0 root         (0) root         (0)     2005 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/authorization/terms_of_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.288658 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/
--rw-r--r--   0 root         (0) root         (0)     3296 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2659 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_business_connection.py
--rw-r--r--   0 root         (0) root         (0)     1813 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 root         (0) root         (0)     2863 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 root         (0) root         (0)     1368 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 root         (0) root         (0)     1333 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 root         (0) root         (0)     1324 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 root         (0) root         (0)     1637 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 root         (0) root         (0)     1714 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 root         (0) root         (0)     1892 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1383 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 root         (0) root         (0)     1605 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_info.py
--rw-r--r--   0 root         (0) root         (0)     1104 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 root         (0) root         (0)    12872 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 root         (0) root         (0)     2458 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 root         (0) root         (0)     8195 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 root         (0) root         (0)     2535 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 root         (0) root         (0)     7289 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 root         (0) root         (0)     3787 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 root         (0) root         (0)     1678 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 root         (0) root         (0)     1284 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 root         (0) root         (0)     1287 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 root         (0) root         (0)     1884 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 root         (0) root         (0)     4650 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 root         (0) root         (0)     2414 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 root         (0) root         (0)     1492 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/request_peer_type_channel.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/request_peer_type_chat.py
--rw-r--r--   0 root         (0) root         (0)     1383 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/request_peer_type_user.py
--rw-r--r--   0 root         (0) root         (0)     1639 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 root         (0) root         (0)     1388 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.292658 pyrogeram-2.0.106/pyrogram/types/inline_mode/
--rw-r--r--   0 root         (0) root         (0)     2830 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3737 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 root         (0) root         (0)     7373 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0 root         (0) root         (0)     2486 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0 root         (0) root         (0)     5857 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 root         (0) root         (0)     5159 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 root         (0) root         (0)     4320 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 root         (0) root         (0)     4104 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 root         (0) root         (0)     4463 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 root         (0) root         (0)     4387 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 root         (0) root         (0)     3106 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 root         (0) root         (0)     4469 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 root         (0) root         (0)     4277 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 root         (0) root         (0)     4207 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 root         (0) root         (0)     5315 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 root         (0) root         (0)     4694 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 root         (0) root         (0)     5336 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 root         (0) root         (0)     4829 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 root         (0) root         (0)     5549 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 root         (0) root         (0)     4435 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.296658 pyrogeram-2.0.106/pyrogram/types/input_media/
--rw-r--r--   0 root         (0) root         (0)     1550 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1713 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_media/input_media.py
--rw-r--r--   0 root         (0) root         (0)     3503 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0 root         (0) root         (0)     1280 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_media/input_media_area.py
--rw-r--r--   0 root         (0) root         (0)     1902 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_media/input_media_area_channel_post.py
--rw-r--r--   0 root         (0) root         (0)     3357 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0 root         (0) root         (0)     2846 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0 root         (0) root         (0)     2760 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0 root         (0) root         (0)     3695 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0 root         (0) root         (0)     1812 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.296658 pyrogeram-2.0.106/pyrogram/types/input_message_content/
--rw-r--r--   0 root         (0) root         (0)     1233 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1488 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0 root         (0) root         (0)     3179 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_message_content/input_reply_to_message.py
--rw-r--r--   0 root         (0) root         (0)     1509 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_message_content/input_reply_to_story.py
--rw-r--r--   0 root         (0) root         (0)     2713 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 root         (0) root         (0)     1168 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.304658 pyrogeram-2.0.106/pyrogram/types/messages_and_media/
--rw-r--r--   0 root         (0) root         (0)     3245 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4119 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0 root         (0) root         (0)     4144 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0 root         (0) root         (0)     2282 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0 root         (0) root         (0)     1662 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0 root         (0) root         (0)     3484 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/exported_story_link.py
--rw-r--r--   0 root         (0) root         (0)     3119 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0 root         (0) root         (0)     3739 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/giveaway.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/giveaway_launched.py
--rw-r--r--   0 root         (0) root         (0)     4575 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/giveaway_result.py
--rw-r--r--   0 root         (0) root         (0)     1735 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0 root         (0) root         (0)     1483 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/media_area.py
--rw-r--r--   0 root         (0) root         (0)     2288 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/media_area_channel_post.py
--rw-r--r--   0 root         (0) root         (0)     2546 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/media_area_coordinates.py
--rw-r--r--   0 root         (0) root         (0)   203597 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0 root         (0) root         (0)     4427 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0 root         (0) root         (0)     2923 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/message_reaction_count_updated.py
--rw-r--r--   0 root         (0) root         (0)     4299 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/message_reaction_updated.py
--rw-r--r--   0 root         (0) root         (0)     1898 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0 root         (0) root         (0)     2634 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/message_story.py
--rw-r--r--   0 root         (0) root         (0)     4384 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0 root         (0) root         (0)     8091 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0 root         (0) root         (0)     1607 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0 root         (0) root         (0)     2692 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0 root         (0) root         (0)     1941 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/reaction_count.py
--rw-r--r--   0 root         (0) root         (0)     2449 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/reaction_type.py
--rw-r--r--   0 root         (0) root         (0)     7695 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0 root         (0) root         (0)     2774 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/stickerset.py
--rw-r--r--   0 root         (0) root         (0)     1878 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/stories_privacy_rules.py
--rw-r--r--   0 root         (0) root         (0)    75413 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/story.py
--rw-r--r--   0 root         (0) root         (0)     2337 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/story_deleted.py
--rw-r--r--   0 root         (0) root         (0)     2776 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/story_forward_header.py
--rw-r--r--   0 root         (0) root         (0)     3071 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/story_skipped.py
--rw-r--r--   0 root         (0) root         (0)     1667 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/story_views.py
--rw-r--r--   0 root         (0) root         (0)     1506 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 root         (0) root         (0)     3830 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0 root         (0) root         (0)     2366 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0 root         (0) root         (0)     4464 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0 root         (0) root         (0)     3676 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0 root         (0) root         (0)     3279 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0 root         (0) root         (0)     1640 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0 root         (0) root         (0)     6426 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0 root         (0) root         (0)     1578 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/web_page_empty.py
--rw-r--r--   0 root         (0) root         (0)     2733 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/messages_and_media/web_page_preview.py
--rw-r--r--   0 root         (0) root         (0)     4053 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.308658 pyrogeram-2.0.106/pyrogram/types/pyromod/
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/pyromod/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3313 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/pyromod/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2840 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/pyromod/listener.py
--rw-r--r--   0 root         (0) root         (0)     1105 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:22:43.316658 pyrogeram-2.0.106/pyrogram/types/user_and_chats/
--rw-r--r--   0 root         (0) root         (0)     3607 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1757 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/birthday.py
--rw-r--r--   0 root         (0) root         (0)     3032 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/business_info.py
--rw-r--r--   0 root         (0) root         (0)     4303 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/business_message.py
--rw-r--r--   0 root         (0) root         (0)     2843 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/business_recipients.py
--rw-r--r--   0 root         (0) root         (0)     1564 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/business_weekly_open.py
--rw-r--r--   0 root         (0) root         (0)     2038 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/business_working_hours.py
--rw-r--r--   0 root         (0) root         (0)    43177 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0 root         (0) root         (0)     2311 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     2217 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_color.py
--rw-r--r--   0 root         (0) root         (0)    22098 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0 root         (0) root         (0)     5589 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 root         (0) root         (0)     4654 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     4320 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_joined_by_request.py
--rw-r--r--   0 root         (0) root         (0)     2639 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 root         (0) root         (0)     9519 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0 root         (0) root         (0)     3749 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 root         (0) root         (0)    10174 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 root         (0) root         (0)     4042 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     2667 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0 root         (0) root         (0)     6337 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2549 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 root         (0) root         (0)     2757 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0 root         (0) root         (0)     2497 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0 root         (0) root         (0)     4979 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/forum_topic.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/forum_topic_closed.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/forum_topic_created.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/forum_topic_edited.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/forum_topic_reopened.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
--rw-r--r--   0 root         (0) root         (0)     1060 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
--rw-r--r--   0 root         (0) root         (0)     2026 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 root         (0) root         (0)     1338 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/peer_channel.py
--rw-r--r--   0 root         (0) root         (0)     1302 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/peer_user.py
--rw-r--r--   0 root         (0) root         (0)     1738 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0 root         (0) root         (0)    17777 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0 root         (0) root         (0)     1700 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0 root         (0) root         (0)     1421 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 root         (0) root         (0)     1685 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 root         (0) root         (0)     1606 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 root         (0) root         (0)    15263 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/pyrogram/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 15:22:43.320658 pyrogeram-2.0.106/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      599 2024-04-24 15:22:13.000000 pyrogeram-2.0.106/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.278870 pyrogeram-2.0.107/
+-rw-r--r--   0 root         (0) root         (0)      463 2024-04-24 15:34:39.278870 pyrogeram-2.0.107/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.698875 pyrogeram-2.0.107/compiler/
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/compiler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.698875 pyrogeram-2.0.107/compiler/api/
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/compiler/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22560 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/compiler/api/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.698875 pyrogeram-2.0.107/compiler/docs/
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/compiler/docs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23157 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/compiler/docs/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.698875 pyrogeram-2.0.107/compiler/errors/
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/compiler/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4992 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/compiler/errors/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     1338 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/compiler/errors/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.278870 pyrogeram-2.0.107/pyrogeram.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      463 2024-04-24 15:34:38.000000 pyrogeram-2.0.107/pyrogeram.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)   142732 2024-04-24 15:34:38.000000 pyrogeram-2.0.107/pyrogeram.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 15:34:38.000000 pyrogeram-2.0.107/pyrogeram.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2024-04-24 15:34:38.000000 pyrogeram-2.0.107/pyrogeram.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-24 15:34:38.000000 pyrogeram-2.0.107/pyrogeram.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.702875 pyrogeram-2.0.107/pyrogram/
+-rw-r--r--   0 root         (0) root         (0)     1517 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44003 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.702875 pyrogeram-2.0.107/pyrogram/connection/
+-rw-r--r--   0 root         (0) root         (0)      929 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/connection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2676 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/connection/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.702875 pyrogeram-2.0.107/pyrogram/connection/transport/
+-rw-r--r--   0 root         (0) root         (0)      913 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/connection/transport/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.702875 pyrogeram-2.0.107/pyrogram/connection/transport/tcp/
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.702875 pyrogeram-2.0.107/pyrogram/crypto/
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/crypto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4092 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/crypto/aes.py
+-rw-r--r--   0 root         (0) root         (0)     4093 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/crypto/mtproto.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/crypto/prime.py
+-rw-r--r--   0 root         (0) root         (0)    13512 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/crypto/rsa.py
+-rw-r--r--   0 root         (0) root         (0)    13763 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)   208096 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/emoji.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.706874 pyrogeram-2.0.107/pyrogram/enums/
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/auto_name.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/business_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/chat_action.py
+-rw-r--r--   0 root         (0) root         (0)     4595 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0 root         (0) root         (0)     1521 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/chat_type.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/listerner_types.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/message_media_type.py
+-rw-r--r--   0 root         (0) root         (0)     2794 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/message_service_type.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/messages_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/next_code_type.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/parse_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/poll_type.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/profile_color.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/reaction_type.py
+-rw-r--r--   0 root         (0) root         (0)     2470 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/reply_color.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/stories_privacy_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/story_privacy.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/enums/user_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.706874 pyrogeram-2.0.107/pyrogram/errors/
+-rw-r--r--   0 root         (0) root         (0)     2703 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/errors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.710874 pyrogeram-2.0.107/pyrogram/errors/exceptions/
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/errors/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32751 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/errors/exceptions/all.py
+-rw-r--r--   0 root         (0) root         (0)    82731 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/errors/exceptions/bad_request_400.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/errors/exceptions/flood_420.py
+-rw-r--r--   0 root         (0) root         (0)     9351 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/errors/exceptions/forbidden_403.py
+-rw-r--r--   0 root         (0) root         (0)    11243 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/errors/exceptions/internal_server_error_500.py
+-rw-r--r--   0 root         (0) root         (0)     5536 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/errors/exceptions/not_acceptable_406.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/errors/exceptions/see_other_303.py
+-rw-r--r--   0 root         (0) root         (0)     1609 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/errors/exceptions/service_unavailable_503.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/errors/exceptions/unauthorized_401.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.710874 pyrogeram-2.0.107/pyrogram/errors/pyromod/
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/errors/pyromod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       42 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/errors/pyromod/listener_stopped.py
+-rw-r--r--   0 root         (0) root         (0)       42 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/errors/pyromod/listener_timeout.py
+-rw-r--r--   0 root         (0) root         (0)     3390 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/errors/rpc_error.py
+-rw-r--r--   0 root         (0) root         (0)    15229 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/file_id.py
+-rw-r--r--   0 root         (0) root         (0)    27537 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.714874 pyrogeram-2.0.107/pyrogram/handlers/
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/bot_business_connect_handler.py
+-rw-r--r--   0 root         (0) root         (0)     6152 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/bot_business_message_handler.py
+-rw-r--r--   0 root         (0) root         (0)     7959 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/conversation_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2655 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/deleted_bot_business_messages_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/edited_bot_business_message_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0 root         (0) root         (0)     6102 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/message_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/message_reaction_count_updated_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2163 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/message_reaction_updated_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/story_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/handlers/user_status_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.714874 pyrogeram-2.0.107/pyrogram/helpers/
+-rw-r--r--   0 root         (0) root         (0)      813 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3479 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/helpers/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.714874 pyrogeram-2.0.107/pyrogram/methods/
+-rw-r--r--   0 root         (0) root         (0)     1482 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.714874 pyrogeram-2.0.107/pyrogram/methods/advanced/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3208 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0 root         (0) root         (0)     4733 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0 root         (0) root         (0)     8496 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/advanced/save_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.718874 pyrogeram-2.0.107/pyrogram/methods/auth/
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/connect.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0 root         (0) root         (0)     2861 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0 root         (0) root         (0)     3160 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0 root         (0) root         (0)     2798 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2430 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/auth/terminate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.722874 pyrogeram-2.0.107/pyrogram/methods/bots/
+-rw-r--r--   0 root         (0) root         (0)     2222 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/get_bot_info.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0 root         (0) root         (0)     5185 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0 root         (0) root         (0)     4325 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     3261 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/set_bot_info.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     4108 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/bots/set_game_score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.730874 pyrogeram-2.0.107/pyrogram/methods/chats/
+-rw-r--r--   0 root         (0) root         (0)     4429 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3554 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0 root         (0) root         (0)     2377 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/close_forum_topic.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/close_general_topic.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/create_forum_topic.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/delete_forum_topic.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/edit_forum_topic.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/edit_general_topic.py
+-rw-r--r--   0 root         (0) root         (0)     3469 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 root         (0) root         (0)     3586 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     5443 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/get_forum_topics.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/get_forum_topics_by_id.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/hide_general_topic.py
+-rw-r--r--   0 root         (0) root         (0)     2790 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 root         (0) root         (0)     3318 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0 root         (0) root         (0)     4363 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/reopen_forum_topic.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/reopen_general_topic.py
+-rw-r--r--   0 root         (0) root         (0)     9697 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     3384 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0 root         (0) root         (0)     8713 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     4762 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2391 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/unhide_general_topic.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/unpin_chat_message.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/chats/update_color.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.730874 pyrogeram-2.0.107/pyrogram/methods/contacts/
+-rw-r--r--   0 root         (0) root         (0)     1229 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2728 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/contacts/import_contacts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.738874 pyrogeram-2.0.107/pyrogram/methods/decorators/
+-rw-r--r--   0 root         (0) root         (0)     2330 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_bot_business_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_bot_business_message.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     2328 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_deleted_bot_business_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_edited_bot_business_message.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_message_reaction_count_updated.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_message_reaction_updated.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0 root         (0) root         (0)     2136 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_story.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/decorators/on_user_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.742874 pyrogeram-2.0.107/pyrogram/methods/invite_links/
+-rw-r--r--   0 root         (0) root         (0)     2510 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     3694 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     2743 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 root         (0) root         (0)     2158 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.750874 pyrogeram-2.0.107/pyrogram/methods/messages/
+-rw-r--r--   0 root         (0) root         (0)     4052 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6983 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     5903 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0 root         (0) root         (0)     3309 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0 root         (0) root         (0)     7693 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0 root         (0) root         (0)     2346 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 root         (0) root         (0)    10450 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0 root         (0) root         (0)     3139 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0 root         (0) root         (0)    13183 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0 root         (0) root         (0)     3137 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 root         (0) root         (0)     4067 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     5265 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0 root         (0) root         (0)     4662 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0 root         (0) root         (0)     2550 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 root         (0) root         (0)     3107 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     4902 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0 root         (0) root         (0)     2285 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0 root         (0) root         (0)     4235 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0 root         (0) root         (0)     2231 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0 root         (0) root         (0)     5510 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3364 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0 root         (0) root         (0)    15042 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0 root         (0) root         (0)    13506 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0 root         (0) root         (0)     7520 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0 root         (0) root         (0)     3660 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0 root         (0) root         (0)     7244 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0 root         (0) root         (0)     7437 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0 root         (0) root         (0)    12856 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0 root         (0) root         (0)     6953 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0 root         (0) root         (0)    23444 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     9721 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0 root         (0) root         (0)    11874 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0 root         (0) root         (0)    10382 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0 root         (0) root         (0)     5073 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_reaction.py
+-rw-r--r--   0 root         (0) root         (0)    11062 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     7754 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0 root         (0) root         (0)    14390 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0 root         (0) root         (0)    12476 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0 root         (0) root         (0)    11938 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0 root         (0) root         (0)     8669 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/send_web_page.py
+-rw-r--r--   0 root         (0) root         (0)     2980 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0 root         (0) root         (0)     4012 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/messages/vote_poll.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.750874 pyrogeram-2.0.107/pyrogram/methods/password/
+-rw-r--r--   0 root         (0) root         (0)     1163 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2872 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0 root         (0) root         (0)     3081 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.754874 pyrogeram-2.0.107/pyrogram/methods/pyromod/
+-rw-r--r--   0 root         (0) root         (0)     1886 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/pyromod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3851 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/pyromod/ask.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/pyromod/get_listener_matching_with_data.py
+-rw-r--r--   0 root         (0) root         (0)     2504 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/pyromod/get_listener_matching_with_identifier_pattern.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/pyromod/get_many_listeners_matching_with_data.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/pyromod/get_many_listeners_matching_with_identifier_pattern.py
+-rw-r--r--   0 root         (0) root         (0)     4546 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/pyromod/listen.py
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/pyromod/register_next_step_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/pyromod/remove_listerner.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/pyromod/stop_listener.py
+-rw-r--r--   0 root         (0) root         (0)     2773 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/pyromod/stop_listening.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/pyromod/wait_for_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/pyromod/wait_for_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.754874 pyrogeram-2.0.107/pyrogram/methods/stickers/
+-rw-r--r--   0 root         (0) root         (0)     1058 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/stickers/add_sticker_to_set.py
+-rw-r--r--   0 root         (0) root         (0)     4301 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/stickers/create_sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/stickers/get_sticker_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.758874 pyrogeram-2.0.107/pyrogram/methods/users/
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1933 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/block_user.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/delete_stories.py
+-rw-r--r--   0 root         (0) root         (0)    10868 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/edit_story.py
+-rw-r--r--   0 root         (0) root         (0)     2381 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/export_story_link.py
+-rw-r--r--   0 root         (0) root         (0)     4786 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/forward_story.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/get_all_stories.py
+-rw-r--r--   0 root         (0) root         (0)     4595 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/get_me.py
+-rw-r--r--   0 root         (0) root         (0)     2445 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/get_peer_stories.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/get_stories.py
+-rw-r--r--   0 root         (0) root         (0)     2620 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/get_stories_history.py
+-rw-r--r--   0 root         (0) root         (0)     2724 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/get_users.py
+-rw-r--r--   0 root         (0) root         (0)    11065 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/send_story.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/set_username.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/update_birthday.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/update_personal_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/users/update_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.762874 pyrogeram-2.0.107/pyrogram/methods/utilities/
+-rw-r--r--   0 root         (0) root         (0)     1371 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0 root         (0) root         (0)     2285 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/utilities/run.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/utilities/run_sync.py
+-rw-r--r--   0 root         (0) root         (0)     2439 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/utilities/start.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0 root         (0) root         (0)    61990 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/mime_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.762874 pyrogeram-2.0.107/pyrogram/nav/
+-rw-r--r--   0 root         (0) root         (0)      923 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/nav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3591 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/nav/pagination.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.762874 pyrogeram-2.0.107/pyrogram/parser/
+-rw-r--r--   0 root         (0) root         (0)      921 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8759 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/parser/html.py
+-rw-r--r--   0 root         (0) root         (0)     7642 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/parser/markdown.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/parser/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.762874 pyrogeram-2.0.107/pyrogram/raw/
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   123357 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/all.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.830873 pyrogeram-2.0.107/pyrogram/raw/base/
+-rw-r--r--   0 root         (0) root         (0)    16535 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/access_point_rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.834873 pyrogeram-2.0.107/pyrogram/raw/base/account/
+-rw-r--r--   0 root         (0) root         (0)     2167 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/authorization_form.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/authorizations.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/auto_download_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/auto_save_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/business_chat_links.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/connected_bots.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/content_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2306 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/email_verified.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/emoji_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     2197 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/password.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/password_input_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/password_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/privacy_rules.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/reset_password_result.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/resolved_business_chat_links.py
+-rw-r--r--   0 root         (0) root         (0)     2315 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/saved_ringtone.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/saved_ringtones.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/sent_email_code.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/takeout.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/themes.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/tmp_password.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/wall_papers.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account/web_authorizations.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/account_days_ttl.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/app_web_view_result.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/attach_menu_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/attach_menu_bot_icon.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/attach_menu_bot_icon_color.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/attach_menu_bots.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/attach_menu_bots_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/attach_menu_peer_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.834873 pyrogeram-2.0.107/pyrogram/raw/base/auth/
+-rw-r--r--   0 root         (0) root         (0)     1457 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/auth/authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2264 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/auth/code_type.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/auth/exported_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2187 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/auth/logged_out.py
+-rw-r--r--   0 root         (0) root         (0)     2381 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/auth/login_token.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/auth/password_recovery.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/auth/sent_code.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/auth/sent_code_type.py
+-rw-r--r--   0 root         (0) root         (0)     2205 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/auto_download_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/auto_save_exception.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/auto_save_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/available_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     2083 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/bad_msg_notification.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/bank_card_open_url.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/base_theme.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/bind_auth_key_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/birthday.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/boost.py
+-rw-r--r--   0 root         (0) root         (0)     2018 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/bot_app.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/bot_business_connection.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/bot_command.py
+-rw-r--r--   0 root         (0) root         (0)     2442 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/bot_command_scope.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/bot_info.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/bot_inline_message.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/bot_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     2340 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/bot_menu_button.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.834873 pyrogeram-2.0.107/pyrogram/raw/base/bots/
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/bots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/bots/bot_info.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/broadcast_revenue_transaction.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/business_away_message.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/business_away_message_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/business_bot_recipients.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/business_chat_link.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/business_greeting_message.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/business_intro.py
+-rw-r--r--   0 root         (0) root         (0)     2018 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/business_location.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/business_recipients.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/business_weekly_open.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/business_work_hours.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/cdn_config.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/cdn_public_key.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/channel_admin_log_event.py
+-rw-r--r--   0 root         (0) root         (0)     7208 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/channel_admin_log_event_action.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/channel_admin_log_events_filter.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/channel_location.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/channel_messages_filter.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/channel_participant.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/channel_participants_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.838873 pyrogeram-2.0.107/pyrogram/raw/base/channels/
+-rw-r--r--   0 root         (0) root         (0)     1401 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/channels/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/channels/admin_log_results.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/channels/channel_participant.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/channels/channel_participants.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/channels/send_as_peers.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/channels/sponsored_message_report_result.py
+-rw-r--r--   0 root         (0) root         (0)     2136 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chat.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chat_admin_rights.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chat_admin_with_invites.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chat_banned_rights.py
+-rw-r--r--   0 root         (0) root         (0)     2018 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chat_full.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chat_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chat_invite_importer.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chat_onlines.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chat_participant.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chat_participants.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chat_reactions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.838873 pyrogeram-2.0.107/pyrogram/raw/base/chatlists/
+-rw-r--r--   0 root         (0) root         (0)     1332 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chatlists/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2338 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chatlists/chatlist_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chatlists/chatlist_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chatlists/exported_chatlist_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/chatlists/exported_invites.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/client_dh_inner_data.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/code_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/config.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/connected_bot.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/contact.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/contact_birthday.py
+-rw-r--r--   0 root         (0) root         (0)     2205 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/contact_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.838873 pyrogeram-2.0.107/pyrogram/raw/base/contacts/
+-rw-r--r--   0 root         (0) root         (0)     1388 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/contacts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/contacts/blocked.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/contacts/contact_birthdays.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/contacts/contacts.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/contacts/found.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/contacts/imported_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/contacts/resolved_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/contacts/top_peers.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/data_json.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/dc_option.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/default_history_ttl.py
+-rw-r--r--   0 root         (0) root         (0)     2346 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/destroy_auth_key_res.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/destroy_session_res.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/dialog.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/dialog_filter.py
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/dialog_filter_suggested.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/dialog_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/document.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/document_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/draft_message.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/email_verification.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/email_verify_purpose.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/emoji_group.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/emoji_keyword.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/emoji_keywords_difference.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/emoji_language.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/emoji_list.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     2175 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/emoji_url.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/encrypted_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/encrypted_file.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/encrypted_message.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/exported_chat_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/exported_chatlist_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/exported_contact_token.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/exported_message_link.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/exported_story_link.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/file_hash.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/folder.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/folder_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/forum_topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.838873 pyrogeram-2.0.107/pyrogram/raw/base/fragment/
+-rw-r--r--   0 root         (0) root         (0)     1181 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/fragment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/fragment/collectible_info.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/game.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/geo_point.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/global_privacy_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/group_call.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/group_call_participant.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/group_call_participant_video.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/group_call_participant_video_source_group.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/group_call_stream_channel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.842873 pyrogeram-2.0.107/pyrogram/raw/base/help/
+-rw-r--r--   0 root         (0) root         (0)     1956 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/app_config.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/app_update.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/config_simple.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/countries_list.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/country.py
+-rw-r--r--   0 root         (0) root         (0)     2003 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/country_code.py
+-rw-r--r--   0 root         (0) root         (0)     2285 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/deep_link_info.py
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/invite_text.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/passport_config.py
+-rw-r--r--   0 root         (0) root         (0)     2028 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/peer_color_option.py
+-rw-r--r--   0 root         (0) root         (0)     2084 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/peer_color_set.py
+-rw-r--r--   0 root         (0) root         (0)     2317 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/peer_colors.py
+-rw-r--r--   0 root         (0) root         (0)     2214 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/premium_promo.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/promo_data.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/recent_me_urls.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/support.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/support_name.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/terms_of_service.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/terms_of_service_update.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/timezones_list.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/help/user_info.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/high_score.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/http_wait.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/imported_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/inline_bot_switch_pm.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/inline_bot_web_view.py
+-rw-r--r--   0 root         (0) root         (0)     2430 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/inline_query_peer_type.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_app_event.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_bot_app.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_bot_inline_message.py
+-rw-r--r--   0 root         (0) root         (0)     2139 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_bot_inline_message_id.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_bot_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_business_away_message.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_business_bot_recipients.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_business_chat_link.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_business_greeting_message.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_business_intro.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_business_recipients.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_chatlist.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_check_password_srp.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_client_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_collectible.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2081 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_dialog_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_document.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_encrypted_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_encrypted_file.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_file.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_file_location.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_folder_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_game.py
+-rw-r--r--   0 root         (0) root         (0)     2063 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_geo_point.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_invoice.py
+-rw-r--r--   0 root         (0) root         (0)     2972 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_media.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_message.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_notify_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_payment_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     2349 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_peer_notify_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_phone_call.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_privacy_key.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_privacy_rule.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_quick_reply_shortcut.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_reply_to.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_secure_file.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_secure_value.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_single_media.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_sticker_set_item.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_stickered_media.py
+-rw-r--r--   0 root         (0) root         (0)     2352 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_store_payment_purpose.py
+-rw-r--r--   0 root         (0) root         (0)     2036 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_theme.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_theme_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_user.py
+-rw-r--r--   0 root         (0) root         (0)     2134 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_wall_paper.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_web_document.py
+-rw-r--r--   0 root         (0) root         (0)     2221 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/input_web_file_location.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/ip_port.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/json_object_value.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/json_value.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/keyboard_button.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/keyboard_button_row.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/labeled_price.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/lang_pack_difference.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/lang_pack_language.py
+-rw-r--r--   0 root         (0) root         (0)     2352 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/lang_pack_string.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/mask_coords.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/media_area.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/media_area_coordinates.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/message.py
+-rw-r--r--   0 root         (0) root         (0)     5292 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/message_action.py
+-rw-r--r--   0 root         (0) root         (0)     3328 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/message_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/message_extended_media.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/message_fwd_header.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/message_media.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/message_peer_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/message_peer_vote.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/message_range.py
+-rw-r--r--   0 root         (0) root         (0)     2018 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/message_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/message_replies.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/message_reply_header.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/message_views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.854873 pyrogeram-2.0.107/pyrogram/raw/base/messages/
+-rw-r--r--   0 root         (0) root         (0)     3557 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/affected_found_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/affected_history.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/affected_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/all_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/archived_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/available_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/bot_app.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/bot_callback_answer.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/bot_results.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/chat_admins_with_invites.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/chat_full.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/chat_invite_importers.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/chats.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/checked_history_import_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/dh_config.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/dialog_filters.py
+-rw-r--r--   0 root         (0) root         (0)     2341 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/discussion_message.py
+-rw-r--r--   0 root         (0) root         (0)     2402 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/emoji_groups.py
+-rw-r--r--   0 root         (0) root         (0)     2414 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/exported_chat_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/exported_chat_invites.py
+-rw-r--r--   0 root         (0) root         (0)     2329 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/faved_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2447 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/featured_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2264 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/forum_topics.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/found_sticker_sets.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/high_scores.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/history_import.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/history_import_parsed.py
+-rw-r--r--   0 root         (0) root         (0)     2240 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/inactive_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/invited_users.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/message_edit_data.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/message_reactions_list.py
+-rw-r--r--   0 root         (0) root         (0)     2231 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/message_views.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/messages.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/my_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/peer_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/peer_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/quick_replies.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2338 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/recent_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/saved_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/saved_gifs.py
+-rw-r--r--   0 root         (0) root         (0)     2366 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/saved_reaction_tags.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/search_counter.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/search_results_calendar.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/search_results_positions.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/sent_encrypted_message.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/sponsored_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2612 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/sticker_set_install_result.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/transcribed_audio.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/translated_text.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/votes_list.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages/web_page.py
+-rw-r--r--   0 root         (0) root         (0)     3260 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/messages_filter.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/missing_invitee.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/msg_detailed_info.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/msg_resend_req.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/msgs_ack.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/msgs_all_info.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/msgs_state_info.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/msgs_state_req.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/my_boost.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/nearest_dc.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/new_session.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/notification_sound.py
+-rw-r--r--   0 root         (0) root         (0)     2191 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/notify_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/outbox_read_date.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/page.py
+-rw-r--r--   0 root         (0) root         (0)     3614 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/page_block.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/page_caption.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/page_list_item.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/page_list_ordered_item.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/page_related_article.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/page_table_cell.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/page_table_row.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/password_kdf_algo.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/payment_charge.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/payment_form_method.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/payment_requested_info.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/payment_saved_credentials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.854873 pyrogeram-2.0.107/pyrogram/raw/base/payments/
+-rw-r--r--   0 root         (0) root         (0)     1528 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/payments/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2231 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/payments/bank_card_data.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/payments/checked_gift_code.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/payments/exported_invoice.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/payments/giveaway_info.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/payments/payment_form.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/payments/payment_receipt.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/payments/payment_result.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/payments/saved_info.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/payments/validated_requested_info.py
+-rw-r--r--   0 root         (0) root         (0)     2264 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/peer.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/peer_blocked.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/peer_color.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/peer_located.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/peer_notify_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/peer_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/peer_stories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.854873 pyrogeram-2.0.107/pyrogram/raw/base/phone/
+-rw-r--r--   0 root         (0) root         (0)     1483 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/phone/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/phone/exported_group_call_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2197 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/phone/group_call.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/phone/group_call_stream_channels.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/phone/group_call_stream_rtmp_url.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/phone/group_participants.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/phone/join_as_peers.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/phone/phone_call.py
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/phone_call.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/phone_call_discard_reason.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/phone_call_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/phone_connection.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/photo.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/photo_size.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.858873 pyrogeram-2.0.107/pyrogram/raw/base/photos/
+-rw-r--r--   0 root         (0) root         (0)     1187 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/photos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/photos/photo.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/photos/photos.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/poll.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/poll_answer.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/poll_answer_voters.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/poll_results.py
+-rw-r--r--   0 root         (0) root         (0)     2167 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/pong.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/popular_contact.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/post_address.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/post_interaction_counters.py
+-rw-r--r--   0 root         (0) root         (0)     2155 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/pq_inner_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.858873 pyrogeram-2.0.107/pyrogram/raw/base/premium/
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/premium/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/premium/boosts_list.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/premium/boosts_status.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/premium/my_boosts.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/premium_gift_code_option.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/premium_gift_option.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/premium_subscription_option.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/prepaid_giveaway.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/privacy_key.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/privacy_rule.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/public_forward.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/quick_reply.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/reaction.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/reaction_count.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/read_participant_date.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/received_notify_message.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/recent_me_url.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/reply_markup.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/report_reason.py
+-rw-r--r--   0 root         (0) root         (0)     2158 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/request_peer_type.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/requested_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/res_pq.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/restriction_reason.py
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/rich_text.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/rpc_drop_answer.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/rpc_error.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/rpc_result.py
+-rw-r--r--   0 root         (0) root         (0)     2206 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/saved_contact.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/saved_dialog.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/saved_reaction_tag.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/search_results_calendar_period.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/search_results_position.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/secure_credentials_encrypted.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/secure_data.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/secure_file.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/secure_password_kdf_algo.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/secure_plain_data.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/secure_required_type.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/secure_secret_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/secure_value.py
+-rw-r--r--   0 root         (0) root         (0)     2616 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/secure_value_error.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/secure_value_hash.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/secure_value_type.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/send_as_peer.py
+-rw-r--r--   0 root         (0) root         (0)     3416 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/send_message_action.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/server_dh_inner_data.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/server_dh_params.py
+-rw-r--r--   0 root         (0) root         (0)     2322 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/set_client_dh_params_answer.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/shipping_option.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/simple_web_view_result.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/sms_job.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.858873 pyrogeram-2.0.107/pyrogram/raw/base/smsjobs/
+-rw-r--r--   0 root         (0) root         (0)     1213 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/smsjobs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/smsjobs/eligibility_to_join.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/smsjobs/status.py
+-rw-r--r--   0 root         (0) root         (0)     2018 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/sponsored_message.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/sponsored_message_report_option.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/sponsored_web_page.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.858873 pyrogeram-2.0.107/pyrogram/raw/base/stats/
+-rw-r--r--   0 root         (0) root         (0)     1551 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2282 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats/broadcast_revenue_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2331 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats/broadcast_revenue_transactions.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats/broadcast_revenue_withdrawal_url.py
+-rw-r--r--   0 root         (0) root         (0)     2232 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats/broadcast_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2232 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats/megagroup_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats/message_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats/public_forwards.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats/story_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats_abs_value_and_prev.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats_date_range_days.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats_graph.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats_group_top_admin.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats_group_top_inviter.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats_group_top_poster.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats_percent_value.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stats_url.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/sticker_keyword.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/sticker_pack.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/sticker_set_covered.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.858873 pyrogeram-2.0.107/pyrogram/raw/base/stickers/
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stickers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stickers/suggested_short_name.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.858873 pyrogeram-2.0.107/pyrogram/raw/base/storage/
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/storage/file_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.862873 pyrogeram-2.0.107/pyrogram/raw/base/stories/
+-rw-r--r--   0 root         (0) root         (0)     1372 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stories/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stories/all_stories.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stories/peer_stories.py
+-rw-r--r--   0 root         (0) root         (0)     2270 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stories/stories.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stories/story_reactions_list.py
+-rw-r--r--   0 root         (0) root         (0)     2214 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stories/story_views.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stories/story_views_list.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/stories_stealth_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/story_fwd_header.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/story_item.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/story_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/story_view.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/story_views.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/text_with_entities.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/theme.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/theme_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/timezone.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/top_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2555 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/top_peer_category.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/top_peer_category_peers.py
+-rw-r--r--   0 root         (0) root         (0)    10979 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.862873 pyrogeram-2.0.107/pyrogram/raw/base/updates/
+-rw-r--r--   0 root         (0) root         (0)     1245 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/updates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/updates/channel_difference.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/updates/difference.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/updates/state.py
+-rw-r--r--   0 root         (0) root         (0)     6305 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/updates_t.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.862873 pyrogeram-2.0.107/pyrogram/raw/base/upload/
+-rw-r--r--   0 root         (0) root         (0)     1218 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/upload/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/upload/cdn_file.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/upload/file.py
+-rw-r--r--   0 root         (0) root         (0)     2187 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/upload/web_file.py
+-rw-r--r--   0 root         (0) root         (0)     2392 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/url_auth_result.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/user.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/user_full.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/user_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/user_status.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/username.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.862873 pyrogeram-2.0.107/pyrogram/raw/base/users/
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/users/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/users/user_full.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/video_size.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/wall_paper.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/wall_paper_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2018 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/web_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/web_document.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/web_page.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/web_page_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/web_view_message_sent.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/base/web_view_result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.866873 pyrogeram-2.0.107/pyrogram/raw/core/
+-rw-r--r--   0 root         (0) root         (0)     1387 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/list.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/message.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/msg_container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.866873 pyrogeram-2.0.107/pyrogram/raw/core/primitives/
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0 root         (0) root         (0)     1433 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0 root         (0) root         (0)     2570 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/raw/core/tl_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.870873 pyrogeram-2.0.107/pyrogram/raw/functions/
+-rw-r--r--   0 root         (0) root         (0)     2184 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.890873 pyrogeram-2.0.107/pyrogram/raw/functions/account/
+-rw-r--r--   0 root         (0) root         (0)     6917 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3414 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/accept_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/cancel_password_email.py
+-rw-r--r--   0 root         (0) root         (0)     3697 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/change_authorization_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/change_phone.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/check_username.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/clear_recent_emoji_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     2205 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/confirm_password_email.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/confirm_phone.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/create_business_chat_link.py
+-rw-r--r--   0 root         (0) root         (0)     3406 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/create_theme.py
+-rw-r--r--   0 root         (0) root         (0)     2063 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/decline_password_reset.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/delete_account.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/delete_auto_save_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/delete_business_chat_link.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/delete_secure_value.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/disable_peer_connected_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2555 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/edit_business_chat_link.py
+-rw-r--r--   0 root         (0) root         (0)     2328 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/finish_takeout_session.py
+-rw-r--r--   0 root         (0) root         (0)     2081 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_account_ttl.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_all_secure_values.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_authorization_form.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_authorizations.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_auto_download_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_auto_save_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2336 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_bot_business_connection.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_business_chat_links.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_channel_default_emoji_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_channel_restricted_status_emojis.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_chat_themes.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_connected_bots.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_contact_sign_up_notification.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_content_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_default_background_emojis.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_default_emoji_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_default_group_photo_emojis.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_default_profile_photo_emojis.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_global_privacy_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_multi_wall_papers.py
+-rw-r--r--   0 root         (0) root         (0)     3178 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_notify_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_notify_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_password.py
+-rw-r--r--   0 root         (0) root         (0)     2414 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_password_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_privacy.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_recent_emoji_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_saved_ringtones.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_secure_value.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_theme.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_themes.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_tmp_password.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_wall_paper.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_wall_papers.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/get_web_authorizations.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/init_takeout_session.py
+-rw-r--r--   0 root         (0) root         (0)     3521 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/install_theme.py
+-rw-r--r--   0 root         (0) root         (0)     2633 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/install_wall_paper.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/invalidate_sign_in_codes.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/register_device.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/reorder_usernames.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/report_peer.py
+-rw-r--r--   0 root         (0) root         (0)     3044 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/report_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/resend_password_email.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/reset_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/reset_notify_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/reset_password.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/reset_wall_papers.py
+-rw-r--r--   0 root         (0) root         (0)     2214 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/reset_web_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/reset_web_authorizations.py
+-rw-r--r--   0 root         (0) root         (0)     2303 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/resolve_business_chat_link.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/save_auto_download_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3570 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/save_auto_save_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/save_ringtone.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/save_secure_value.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/save_theme.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/save_wall_paper.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/send_change_phone_code.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/send_confirm_phone_code.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/send_verify_email_code.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/send_verify_phone_code.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/set_account_ttl.py
+-rw-r--r--   0 root         (0) root         (0)     2365 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/set_authorization_ttl.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/set_contact_sign_up_notification.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/set_content_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/set_global_privacy_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/set_privacy.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/toggle_connected_bot_paused.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/toggle_username.py
+-rw-r--r--   0 root         (0) root         (0)     2731 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/unregister_device.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_birthday.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_business_away_message.py
+-rw-r--r--   0 root         (0) root         (0)     2609 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_business_greeting_message.py
+-rw-r--r--   0 root         (0) root         (0)     2507 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_business_intro.py
+-rw-r--r--   0 root         (0) root         (0)     2919 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_business_location.py
+-rw-r--r--   0 root         (0) root         (0)     2673 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_business_work_hours.py
+-rw-r--r--   0 root         (0) root         (0)     3197 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_color.py
+-rw-r--r--   0 root         (0) root         (0)     3252 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_connected_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_device_locked.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_notify_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_password_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_personal_channel.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_status.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_theme.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/update_username.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/upload_ringtone.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/upload_theme.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/upload_wall_paper.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/verify_email.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/account/verify_phone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.894873 pyrogeram-2.0.107/pyrogram/raw/functions/auth/
+-rw-r--r--   0 root         (0) root         (0)     2173 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/accept_login_token.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/bind_temp_auth_key.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/cancel_code.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/check_password.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/check_recovery_password.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/drop_temp_auth_keys.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/export_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/export_login_token.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/import_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2990 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/import_bot_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/import_login_token.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/import_web_token_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/log_out.py
+-rw-r--r--   0 root         (0) root         (0)     2854 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/recover_password.py
+-rw-r--r--   0 root         (0) root         (0)     3538 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/request_firebase_sms.py
+-rw-r--r--   0 root         (0) root         (0)     2134 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/request_password_recovery.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/resend_code.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/reset_authorizations.py
+-rw-r--r--   0 root         (0) root         (0)     2588 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/reset_login_email.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/send_code.py
+-rw-r--r--   0 root         (0) root         (0)     3605 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/sign_in.py
+-rw-r--r--   0 root         (0) root         (0)     3495 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/auth/sign_up.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.898873 pyrogeram-2.0.107/pyrogram/raw/functions/bots/
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/allow_send_message.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/answer_webhook_json_query.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/can_send_message.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/get_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/get_bot_info.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/get_bot_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/invoke_web_view_custom_method.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/reorder_usernames.py
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/reset_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/send_custom_request.py
+-rw-r--r--   0 root         (0) root         (0)     2411 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/set_bot_broadcast_default_admin_rights.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/set_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2395 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/set_bot_group_default_admin_rights.py
+-rw-r--r--   0 root         (0) root         (0)     3761 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/set_bot_info.py
+-rw-r--r--   0 root         (0) root         (0)     2558 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/set_bot_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/bots/toggle_username.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.906873 pyrogeram-2.0.107/pyrogram/raw/functions/channels/
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2503 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/check_username.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/click_sponsored_message.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/convert_to_gigagroup.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/create_channel.py
+-rw-r--r--   0 root         (0) root         (0)     4100 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/create_forum_topic.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/deactivate_all_usernames.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/delete_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/delete_history.py
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/delete_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/delete_participant_history.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/delete_topic_history.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/edit_admin.py
+-rw-r--r--   0 root         (0) root         (0)     2972 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/edit_banned.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/edit_creator.py
+-rw-r--r--   0 root         (0) root         (0)     4111 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/edit_forum_topic.py
+-rw-r--r--   0 root         (0) root         (0)     2801 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/edit_location.py
+-rw-r--r--   0 root         (0) root         (0)     2575 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/edit_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/edit_title.py
+-rw-r--r--   0 root         (0) root         (0)     3095 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/export_message_link.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_admin_log.py
+-rw-r--r--   0 root         (0) root         (0)     3044 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_admined_public_channels.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_channel_recommendations.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_channels.py
+-rw-r--r--   0 root         (0) root         (0)     3648 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_forum_topics.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_forum_topics_by_id.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_full_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_groups_for_discussion.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_inactive_channels.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_left_channels.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2669 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_participant.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_participants.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_send_as.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/get_sponsored_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2629 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/invite_to_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/join_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/leave_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2479 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/read_history.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/read_message_contents.py
+-rw-r--r--   0 root         (0) root         (0)     2890 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/reorder_pinned_forum_topics.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/reorder_usernames.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/report_anti_spam_false_positive.py
+-rw-r--r--   0 root         (0) root         (0)     2792 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/report_spam.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/report_sponsored_message.py
+-rw-r--r--   0 root         (0) root         (0)     2599 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/restrict_sponsored_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/set_boosts_to_unblock_restrictions.py
+-rw-r--r--   0 root         (0) root         (0)     2587 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/set_discussion_group.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/set_emoji_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2598 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/set_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/toggle_anti_spam.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/toggle_forum.py
+-rw-r--r--   0 root         (0) root         (0)     2540 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/toggle_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/toggle_join_to_send.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/toggle_participants_hidden.py
+-rw-r--r--   0 root         (0) root         (0)     2560 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/toggle_pre_history_hidden.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/toggle_signatures.py
+-rw-r--r--   0 root         (0) root         (0)     2534 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/toggle_slow_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/toggle_username.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/toggle_view_forum_as_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3521 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/update_color.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/update_emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/update_pinned_forum_topic.py
+-rw-r--r--   0 root         (0) root         (0)     2507 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/update_username.py
+-rw-r--r--   0 root         (0) root         (0)     2541 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/channels/view_sponsored_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.910873 pyrogeram-2.0.107/pyrogram/raw/functions/chatlists/
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/chatlists/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/chatlists/check_chatlist_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/chatlists/delete_exported_invite.py
+-rw-r--r--   0 root         (0) root         (0)     3396 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/chatlists/edit_exported_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/chatlists/export_chatlist_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/chatlists/get_chatlist_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/chatlists/get_exported_invites.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/chatlists/get_leave_chatlist_suggestions.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/chatlists/hide_chatlist_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/chatlists/join_chatlist_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/chatlists/join_chatlist_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/chatlists/leave_chatlist.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.914873 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/
+-rw-r--r--   0 root         (0) root         (0)     2191 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/accept_contact.py
+-rw-r--r--   0 root         (0) root         (0)     3410 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/add_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/block.py
+-rw-r--r--   0 root         (0) root         (0)     3252 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/block_from_replies.py
+-rw-r--r--   0 root         (0) root         (0)     2240 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/delete_by_phones.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/delete_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/edit_close_friends.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/export_contact_token.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/get_birthdays.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/get_blocked.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/get_contact_i_ds.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/get_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     3094 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/get_located.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/get_saved.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/get_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     5068 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/get_top_peers.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/import_contact_token.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/import_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/reset_saved.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/reset_top_peer_rating.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/resolve_phone.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/resolve_username.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/search.py
+-rw-r--r--   0 root         (0) root         (0)     2815 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/set_blocked.py
+-rw-r--r--   0 root         (0) root         (0)     2205 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/toggle_top_peers.py
+-rw-r--r--   0 root         (0) root         (0)     2581 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contacts/unblock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.914873 pyrogeram-2.0.107/pyrogram/raw/functions/contest/
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3025 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/contest/save_developer_info.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/destroy_auth_key.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/destroy_session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.914873 pyrogeram-2.0.107/pyrogram/raw/functions/folders/
+-rw-r--r--   0 root         (0) root         (0)     1182 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/folders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/folders/edit_peer_folders.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.914873 pyrogeram-2.0.107/pyrogram/raw/functions/fragment/
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/fragment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/fragment/get_collectible_info.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/get_future_salts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.918873 pyrogeram-2.0.107/pyrogram/raw/functions/help/
+-rw-r--r--   0 root         (0) root         (0)     2280 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/accept_terms_of_service.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/dismiss_suggestion.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/edit_user_info.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_app_config.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_app_update.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_cdn_config.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_config.py
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_countries_list.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_deep_link_info.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_invite_text.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_nearest_dc.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_passport_config.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_peer_colors.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_peer_profile_colors.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_premium_promo.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_promo_data.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_recent_me_urls.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_support.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_support_name.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_terms_of_service_update.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_timezones_list.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/get_user_info.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/hide_promo_data.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/save_app_log.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/help/set_bot_updates_status.py
+-rw-r--r--   0 root         (0) root         (0)     4938 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/init_connection.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/invoke_after_msg.py
+-rw-r--r--   0 root         (0) root         (0)     2525 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/invoke_after_msgs.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/invoke_with_business_connection.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/invoke_with_layer.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/invoke_with_messages_range.py
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/invoke_with_takeout.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/invoke_without_updates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.922873 pyrogeram-2.0.107/pyrogram/raw/functions/langpack/
+-rw-r--r--   0 root         (0) root         (0)     1330 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/langpack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/langpack/get_difference.py
+-rw-r--r--   0 root         (0) root         (0)     2505 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/langpack/get_lang_pack.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/langpack/get_language.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/langpack/get_languages.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/langpack/get_strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.962872 pyrogeram-2.0.107/pyrogram/raw/functions/messages/
+-rw-r--r--   0 root         (0) root         (0)    11774 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/accept_encryption.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/accept_url_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2777 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/add_chat_user.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/check_chat_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/check_history_import.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/check_history_import_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/check_quick_reply_shortcut.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/clear_all_drafts.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/clear_recent_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/clear_recent_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2974 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/create_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/delete_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/delete_chat_user.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/delete_exported_chat_invite.py
+-rw-r--r--   0 root         (0) root         (0)     3891 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/delete_history.py
+-rw-r--r--   0 root         (0) root         (0)     2579 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/delete_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/delete_phone_call_history.py
+-rw-r--r--   0 root         (0) root         (0)     2534 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/delete_quick_reply_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/delete_quick_reply_shortcut.py
+-rw-r--r--   0 root         (0) root         (0)     2601 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/delete_revoked_exported_chat_invites.py
+-rw-r--r--   0 root         (0) root         (0)     3359 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/delete_saved_history.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/delete_scheduled_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2598 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/discard_encryption.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/edit_chat_about.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/edit_chat_admin.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/edit_chat_default_banned_rights.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/edit_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2442 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/edit_chat_title.py
+-rw-r--r--   0 root         (0) root         (0)     4497 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/edit_exported_chat_invite.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/edit_inline_bot_message.py
+-rw-r--r--   0 root         (0) root         (0)     5876 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/edit_message.py
+-rw-r--r--   0 root         (0) root         (0)     2504 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/edit_quick_reply_shortcut.py
+-rw-r--r--   0 root         (0) root         (0)     4291 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/export_chat_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/fave_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     6929 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/forward_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_admins_with_invites.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_all_drafts.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_all_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_archived_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_attach_menu_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_attach_menu_bots.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_attached_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_available_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_bot_app.py
+-rw-r--r--   0 root         (0) root         (0)     3672 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_bot_callback_answer.py
+-rw-r--r--   0 root         (0) root         (0)     4101 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_chat_invite_importers.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_common_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_custom_emoji_documents.py
+-rw-r--r--   0 root         (0) root         (0)     2118 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_default_history_ttl.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_default_tag_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2525 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_dh_config.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_dialog_filters.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_dialog_unread_marks.py
+-rw-r--r--   0 root         (0) root         (0)     4001 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_discussion_message.py
+-rw-r--r--   0 root         (0) root         (0)     2677 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_document_by_hash.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_emoji_groups.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_emoji_keywords.py
+-rw-r--r--   0 root         (0) root         (0)     2604 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_emoji_keywords_difference.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_emoji_keywords_languages.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_emoji_profile_photo_groups.py
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_emoji_status_groups.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_emoji_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_emoji_url.py
+-rw-r--r--   0 root         (0) root         (0)     2534 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_exported_chat_invite.py
+-rw-r--r--   0 root         (0) root         (0)     3991 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_exported_chat_invites.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_extended_media.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_faved_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2295 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_featured_emoji_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_featured_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_full_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_game_high_scores.py
+-rw-r--r--   0 root         (0) root         (0)     3828 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_history.py
+-rw-r--r--   0 root         (0) root         (0)     3486 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_inline_bot_results.py
+-rw-r--r--   0 root         (0) root         (0)     2650 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_inline_game_high_scores.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_mask_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_message_edit_data.py
+-rw-r--r--   0 root         (0) root         (0)     3583 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_message_reactions_list.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_message_read_participants.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_messages_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2756 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_messages_views.py
+-rw-r--r--   0 root         (0) root         (0)     2486 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_my_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_old_featured_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_onlines.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_outbox_read_date.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_peer_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_peer_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_pinned_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_pinned_saved_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2486 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_poll_results.py
+-rw-r--r--   0 root         (0) root         (0)     3440 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_poll_votes.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_quick_replies.py
+-rw-r--r--   0 root         (0) root         (0)     2926 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_quick_reply_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_recent_locations.py
+-rw-r--r--   0 root         (0) root         (0)     2459 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_recent_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_recent_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     4037 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_replies.py
+-rw-r--r--   0 root         (0) root         (0)     3631 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_saved_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_saved_gifs.py
+-rw-r--r--   0 root         (0) root         (0)     3848 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_saved_history.py
+-rw-r--r--   0 root         (0) root         (0)     2731 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_saved_reaction_tags.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_scheduled_history.py
+-rw-r--r--   0 root         (0) root         (0)     2534 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_scheduled_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3604 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_search_counters.py
+-rw-r--r--   0 root         (0) root         (0)     3688 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_search_results_calendar.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_search_results_positions.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_split_ranges.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_suggested_dialog_filters.py
+-rw-r--r--   0 root         (0) root         (0)     2447 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_top_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     3864 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_unread_mentions.py
+-rw-r--r--   0 root         (0) root         (0)     3868 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_unread_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_web_page.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/get_web_page_preview.py
+-rw-r--r--   0 root         (0) root         (0)     2977 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/hide_all_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2895 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/hide_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/hide_peer_settings_bar.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/import_chat_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2823 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/init_history_import.py
+-rw-r--r--   0 root         (0) root         (0)     2638 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/install_sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/mark_dialog_unread.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/migrate_chat.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/prolong_web_view.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/rate_transcribed_audio.py
+-rw-r--r--   0 root         (0) root         (0)     2706 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/read_discussion.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/read_encrypted_history.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/read_featured_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/read_history.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/read_mentions.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/read_message_contents.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/read_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/received_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/received_queue.py
+-rw-r--r--   0 root         (0) root         (0)     2852 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/reorder_pinned_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/reorder_pinned_saved_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/reorder_quick_replies.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/reorder_sticker_sets.py
+-rw-r--r--   0 root         (0) root         (0)     2920 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/report.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/report_encrypted_spam.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/report_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/report_spam.py
+-rw-r--r--   0 root         (0) root         (0)     4054 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/request_app_web_view.py
+-rw-r--r--   0 root         (0) root         (0)     2745 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/request_encryption.py
+-rw-r--r--   0 root         (0) root         (0)     4530 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/request_simple_web_view.py
+-rw-r--r--   0 root         (0) root         (0)     3586 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/request_url_auth.py
+-rw-r--r--   0 root         (0) root         (0)     5516 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/request_web_view.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/save_default_send_as.py
+-rw-r--r--   0 root         (0) root         (0)     4448 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/save_draft.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/save_gif.py
+-rw-r--r--   0 root         (0) root         (0)     2777 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/save_recent_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     6383 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/search.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/search_custom_emoji.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/search_emoji_sticker_sets.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/search_global.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/search_sent_media.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/search_sticker_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3117 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_bot_requested_peer.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_encrypted.py
+-rw-r--r--   0 root         (0) root         (0)     3387 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_encrypted_file.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_encrypted_service.py
+-rw-r--r--   0 root         (0) root         (0)     6099 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_inline_bot_result.py
+-rw-r--r--   0 root         (0) root         (0)     7873 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_media.py
+-rw-r--r--   0 root         (0) root         (0)     7912 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_message.py
+-rw-r--r--   0 root         (0) root         (0)     6556 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_multi_media.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_quick_reply_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3536 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_scheduled_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_screenshot_notification.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_vote.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_web_view_data.py
+-rw-r--r--   0 root         (0) root         (0)     2660 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/send_web_view_result_message.py
+-rw-r--r--   0 root         (0) root         (0)     3494 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/set_bot_callback_answer.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/set_bot_precheckout_results.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/set_bot_shipping_results.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/set_chat_available_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/set_chat_theme.py
+-rw-r--r--   0 root         (0) root         (0)     4144 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/set_chat_wall_paper.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/set_default_history_ttl.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/set_default_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/set_encrypted_typing.py
+-rw-r--r--   0 root         (0) root         (0)     3525 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/set_game_score.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/set_history_ttl.py
+-rw-r--r--   0 root         (0) root         (0)     4861 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/set_inline_bot_results.py
+-rw-r--r--   0 root         (0) root         (0)     3380 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/set_inline_game_score.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/set_typing.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/start_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/start_history_import.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/toggle_bot_in_attach_menu.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/toggle_dialog_filter_tags.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/toggle_dialog_pin.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/toggle_no_forwards.py
+-rw-r--r--   0 root         (0) root         (0)     2596 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/toggle_peer_translations.py
+-rw-r--r--   0 root         (0) root         (0)     2594 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/toggle_saved_dialog_pin.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/toggle_sticker_sets.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/transcribe_audio.py
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/translate_text.py
+-rw-r--r--   0 root         (0) root         (0)     2341 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/uninstall_sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2775 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/unpin_all_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2664 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/update_dialog_filter.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/update_dialog_filters_order.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/update_pinned_message.py
+-rw-r--r--   0 root         (0) root         (0)     2706 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/update_saved_reaction_tag.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/upload_encrypted_file.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/upload_imported_media.py
+-rw-r--r--   0 root         (0) root         (0)     3124 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/messages/upload_media.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.962872 pyrogeram-2.0.107/pyrogram/raw/functions/payments/
+-rw-r--r--   0 root         (0) root         (0)     1967 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/apply_gift_code.py
+-rw-r--r--   0 root         (0) root         (0)     2625 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/assign_app_store_transaction.py
+-rw-r--r--   0 root         (0) root         (0)     2689 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/assign_play_market_transaction.py
+-rw-r--r--   0 root         (0) root         (0)     2346 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/can_purchase_premium.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/check_gift_code.py
+-rw-r--r--   0 root         (0) root         (0)     2581 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/clear_saved_info.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/export_invoice.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/get_bank_card_data.py
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/get_giveaway_info.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/get_payment_form.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/get_payment_receipt.py
+-rw-r--r--   0 root         (0) root         (0)     2621 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/get_premium_gift_code_options.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/get_saved_info.py
+-rw-r--r--   0 root         (0) root         (0)     2899 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/launch_prepaid_giveaway.py
+-rw-r--r--   0 root         (0) root         (0)     4382 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/send_payment_form.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/payments/validate_requested_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.970872 pyrogeram-2.0.107/pyrogram/raw/functions/phone/
+-rw-r--r--   0 root         (0) root         (0)     2780 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/accept_call.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/check_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/confirm_call.py
+-rw-r--r--   0 root         (0) root         (0)     3660 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/create_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     3398 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/discard_call.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/discard_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     5183 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/edit_group_call_participant.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/edit_group_call_title.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/export_group_call_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/get_call_config.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/get_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/get_group_call_join_as.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/get_group_call_stream_channels.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/get_group_call_stream_rtmp_url.py
+-rw-r--r--   0 root         (0) root         (0)     3278 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/get_group_participants.py
+-rw-r--r--   0 root         (0) root         (0)     2587 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/invite_to_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     3866 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/join_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/join_group_call_presentation.py
+-rw-r--r--   0 root         (0) root         (0)     2503 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/leave_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/leave_group_call_presentation.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/received_call.py
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/request_call.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/save_call_debug.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/save_call_log.py
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/save_default_group_call_join_as.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/send_signaling_data.py
+-rw-r--r--   0 root         (0) root         (0)     3099 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/set_call_rating.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/start_scheduled_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/toggle_group_call_record.py
+-rw-r--r--   0 root         (0) root         (0)     3137 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/toggle_group_call_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/phone/toggle_group_call_start_subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.970872 pyrogeram-2.0.107/pyrogram/raw/functions/photos/
+-rw-r--r--   0 root         (0) root         (0)     1392 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/photos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/photos/delete_photos.py
+-rw-r--r--   0 root         (0) root         (0)     2931 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/photos/get_user_photos.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/photos/update_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     4750 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/photos/upload_contact_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     4604 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/photos/upload_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/ping.py
+-rw-r--r--   0 root         (0) root         (0)     2552 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/ping_delay_disconnect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.970872 pyrogeram-2.0.107/pyrogram/raw/functions/premium/
+-rw-r--r--   0 root         (0) root         (0)     1343 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/premium/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2714 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/premium/apply_boost.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/premium/get_boosts_list.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/premium/get_boosts_status.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/premium/get_my_boosts.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/premium/get_user_boosts.py
+-rw-r--r--   0 root         (0) root         (0)     3465 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/req_dh_params.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/req_pq.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/req_pq_multi.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/rpc_drop_answer.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/set_client_dh_params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.974872 pyrogeram-2.0.107/pyrogram/raw/functions/smsjobs/
+-rw-r--r--   0 root         (0) root         (0)     1380 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/smsjobs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/smsjobs/finish_job.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/smsjobs/get_sms_job.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/smsjobs/get_status.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/smsjobs/is_eligible_to_join.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/smsjobs/join.py
+-rw-r--r--   0 root         (0) root         (0)     2003 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/smsjobs/leave.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/smsjobs/update_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.974872 pyrogeram-2.0.107/pyrogram/raw/functions/stats/
+-rw-r--r--   0 root         (0) root         (0)     1729 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stats/get_broadcast_revenue_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stats/get_broadcast_revenue_transactions.py
+-rw-r--r--   0 root         (0) root         (0)     2775 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stats/get_broadcast_revenue_withdrawal_url.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stats/get_broadcast_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stats/get_megagroup_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stats/get_message_public_forwards.py
+-rw-r--r--   0 root         (0) root         (0)     2833 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stats/get_message_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stats/get_story_public_forwards.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stats/get_story_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2588 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stats/load_async_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.978872 pyrogeram-2.0.107/pyrogram/raw/functions/stickers/
+-rw-r--r--   0 root         (0) root         (0)     1681 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stickers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2700 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stickers/add_sticker_to_set.py
+-rw-r--r--   0 root         (0) root         (0)     3610 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stickers/change_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     2599 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stickers/change_sticker_position.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stickers/check_short_name.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stickers/create_sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2329 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stickers/delete_sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2368 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stickers/remove_sticker_from_set.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stickers/rename_sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stickers/replace_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     3361 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stickers/set_sticker_set_thumb.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stickers/suggest_short_name.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.982872 pyrogeram-2.0.107/pyrogram/raw/functions/stories/
+-rw-r--r--   0 root         (0) root         (0)     2259 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/activate_stealth_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/can_send_story.py
+-rw-r--r--   0 root         (0) root         (0)     2469 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/delete_stories.py
+-rw-r--r--   0 root         (0) root         (0)     4795 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/edit_story.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/export_story_link.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/get_all_read_peer_stories.py
+-rw-r--r--   0 root         (0) root         (0)     2941 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/get_all_stories.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/get_chats_to_send.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/get_peer_max_i_ds.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/get_peer_stories.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/get_pinned_stories.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/get_stories_archive.py
+-rw-r--r--   0 root         (0) root         (0)     2505 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/get_stories_by_id.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/get_stories_views.py
+-rw-r--r--   0 root         (0) root         (0)     3898 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/get_story_reactions_list.py
+-rw-r--r--   0 root         (0) root         (0)     4243 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/get_story_views_list.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/increment_story_views.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/read_stories.py
+-rw-r--r--   0 root         (0) root         (0)     2919 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/report.py
+-rw-r--r--   0 root         (0) root         (0)     3143 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/send_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     6705 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/send_story.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/toggle_all_stories_hidden.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/toggle_peer_stories_hidden.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/stories/toggle_pinned.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.982872 pyrogeram-2.0.107/pyrogram/raw/functions/updates/
+-rw-r--r--   0 root         (0) root         (0)     1266 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/updates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3365 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/updates/get_channel_difference.py
+-rw-r--r--   0 root         (0) root         (0)     3910 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/updates/get_difference.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/updates/get_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.982872 pyrogeram-2.0.107/pyrogram/raw/functions/upload/
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/upload/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/upload/get_cdn_file.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/upload/get_cdn_file_hashes.py
+-rw-r--r--   0 root         (0) root         (0)     3368 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/upload/get_file.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/upload/get_file_hashes.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/upload/get_web_file.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/upload/reupload_cdn_file.py
+-rw-r--r--   0 root         (0) root         (0)     2950 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/upload/save_big_file_part.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/upload/save_file_part.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:38.986872 pyrogeram-2.0.107/pyrogram/raw/functions/users/
+-rw-r--r--   0 root         (0) root         (0)     1342 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/users/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/users/get_full_user.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/users/get_is_premium_required_to_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/users/get_users.py
+-rw-r--r--   0 root         (0) root         (0)     2564 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/functions/users/set_secure_value_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.186870 pyrogeram-2.0.107/pyrogram/raw/types/
+-rw-r--r--   0 root         (0) root         (0)    63988 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/access_point_rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.194871 pyrogeram-2.0.107/pyrogram/raw/types/account/
+-rw-r--r--   0 root         (0) root         (0)     2652 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4068 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/authorization_form.py
+-rw-r--r--   0 root         (0) root         (0)     2964 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/authorizations.py
+-rw-r--r--   0 root         (0) root         (0)     3160 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/auto_download_settings.py
+-rw-r--r--   0 root         (0) root         (0)     4274 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/auto_save_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/business_chat_links.py
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/connected_bots.py
+-rw-r--r--   0 root         (0) root         (0)     3025 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/content_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/email_verified.py
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/email_verified_login.py
+-rw-r--r--   0 root         (0) root         (0)     2839 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/emoji_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/emoji_statuses_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     7365 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/password.py
+-rw-r--r--   0 root         (0) root         (0)     4371 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/password_input_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/password_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3059 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/privacy_rules.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/reset_password_failed_wait.py
+-rw-r--r--   0 root         (0) root         (0)     2285 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/reset_password_ok.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/reset_password_requested_wait.py
+-rw-r--r--   0 root         (0) root         (0)     3788 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/resolved_business_chat_links.py
+-rw-r--r--   0 root         (0) root         (0)     2270 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/saved_ringtone.py
+-rw-r--r--   0 root         (0) root         (0)     2541 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/saved_ringtone_converted.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/saved_ringtones.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/saved_ringtones_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/sent_email_code.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/takeout.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/themes.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/themes_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     2731 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/tmp_password.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/wall_papers.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/wall_papers_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account/web_authorizations.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/account_days_ttl.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/app_web_view_result_url.py
+-rw-r--r--   0 root         (0) root         (0)     5490 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/attach_menu_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/attach_menu_bot_icon.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/attach_menu_bot_icon_color.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/attach_menu_bots.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/attach_menu_bots_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/attach_menu_bots_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/attach_menu_peer_type_bot_pm.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/attach_menu_peer_type_broadcast.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/attach_menu_peer_type_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2083 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/attach_menu_peer_type_pm.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/attach_menu_peer_type_same_bot_pm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.198871 pyrogeram-2.0.107/pyrogram/raw/types/auth/
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4568 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/authorization.py
+-rw-r--r--   0 root         (0) root         (0)     3095 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/authorization_sign_up_required.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/code_type_call.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/code_type_flash_call.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/code_type_fragment_sms.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/code_type_missed_call.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/code_type_sms.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/exported_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/logged_out.py
+-rw-r--r--   0 root         (0) root         (0)     2655 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/login_token.py
+-rw-r--r--   0 root         (0) root         (0)     2671 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/login_token_migrate_to.py
+-rw-r--r--   0 root         (0) root         (0)     2633 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/login_token_success.py
+-rw-r--r--   0 root         (0) root         (0)     2510 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/password_recovery.py
+-rw-r--r--   0 root         (0) root         (0)     3835 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/sent_code.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/sent_code_success.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/sent_code_type_app.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/sent_code_type_call.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/sent_code_type_email_code.py
+-rw-r--r--   0 root         (0) root         (0)     3470 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/sent_code_type_firebase_sms.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/sent_code_type_flash_call.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/sent_code_type_fragment_sms.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/sent_code_type_missed_call.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/sent_code_type_set_up_email_required.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auth/sent_code_type_sms.py
+-rw-r--r--   0 root         (0) root         (0)     7088 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/authorization.py
+-rw-r--r--   0 root         (0) root         (0)     5929 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auto_download_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auto_save_exception.py
+-rw-r--r--   0 root         (0) root         (0)     3037 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/auto_save_settings.py
+-rw-r--r--   0 root         (0) root         (0)     5784 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/available_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bad_msg_notification.py
+-rw-r--r--   0 root         (0) root         (0)     3066 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bad_server_salt.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bank_card_open_url.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/base_theme_arctic.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/base_theme_classic.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/base_theme_day.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/base_theme_night.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/base_theme_tinted.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bind_auth_key_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/birthday.py
+-rw-r--r--   0 root         (0) root         (0)     5100 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/boost.py
+-rw-r--r--   0 root         (0) root         (0)     4019 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_app.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_app_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_business_connection.py
+-rw-r--r--   0 root         (0) root         (0)     2659 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_command.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_command_scope_chat_admins.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_command_scope_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_command_scope_default.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_command_scope_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2303 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_command_scope_peer_admins.py
+-rw-r--r--   0 root         (0) root         (0)     2570 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_command_scope_peer_user.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_command_scope_users.py
+-rw-r--r--   0 root         (0) root         (0)     4889 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_info.py
+-rw-r--r--   0 root         (0) root         (0)     4403 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_inline_media_result.py
+-rw-r--r--   0 root         (0) root         (0)     3607 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_inline_message_media_auto.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_inline_message_media_contact.py
+-rw-r--r--   0 root         (0) root         (0)     4194 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_inline_message_media_geo.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_inline_message_media_invoice.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_inline_message_media_venue.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_inline_message_media_web_page.py
+-rw-r--r--   0 root         (0) root         (0)     3881 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_inline_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     4740 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_menu_button_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bot_menu_button_default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.198871 pyrogeram-2.0.107/pyrogram/raw/types/bots/
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2821 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/bots/bot_info.py
+-rw-r--r--   0 root         (0) root         (0)     2771 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/broadcast_revenue_transaction_proceeds.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/broadcast_revenue_transaction_refund.py
+-rw-r--r--   0 root         (0) root         (0)     4252 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/broadcast_revenue_transaction_withdrawal.py
+-rw-r--r--   0 root         (0) root         (0)     3342 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/business_away_message.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/business_away_message_schedule_always.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/business_away_message_schedule_custom.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/business_away_message_schedule_outside_work_hours.py
+-rw-r--r--   0 root         (0) root         (0)     4515 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/business_bot_recipients.py
+-rw-r--r--   0 root         (0) root         (0)     3759 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/business_chat_link.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/business_greeting_message.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/business_intro.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/business_location.py
+-rw-r--r--   0 root         (0) root         (0)     4018 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/business_recipients.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/business_weekly_open.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/business_work_hours.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/cdn_config.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/cdn_public_key.py
+-rw-r--r--   0 root         (0) root         (0)    15988 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_about.py
+-rw-r--r--   0 root         (0) root         (0)     2795 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_available_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_emoji_sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_history_ttl.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_linked_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_location.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_peer_color.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2755 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_profile_peer_color.py
+-rw-r--r--   0 root         (0) root         (0)     2869 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_title.py
+-rw-r--r--   0 root         (0) root         (0)     2601 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_username.py
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_usernames.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_change_wallpaper.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_create_topic.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_default_banned_rights.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_delete_message.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_delete_topic.py
+-rw-r--r--   0 root         (0) root         (0)     2402 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_discard_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     2731 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_edit_message.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_edit_topic.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_delete.py
+-rw-r--r--   0 root         (0) root         (0)     2829 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_edit.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_revoke.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_participant_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2175 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_participant_join.py
+-rw-r--r--   0 root         (0) root         (0)     2821 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_participant_join_by_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_participant_join_by_request.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_participant_leave.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_participant_mute.py
+-rw-r--r--   0 root         (0) root         (0)     2935 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_participant_toggle_admin.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_participant_toggle_ban.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_participant_unmute.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_participant_volume.py
+-rw-r--r--   0 root         (0) root         (0)     3080 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_pin_topic.py
+-rw-r--r--   0 root         (0) root         (0)     2381 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_send_message.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_start_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_stop_poll.py
+-rw-r--r--   0 root         (0) root         (0)     2354 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_toggle_anti_spam.py
+-rw-r--r--   0 root         (0) root         (0)     2340 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_toggle_forum.py
+-rw-r--r--   0 root         (0) root         (0)     2395 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_toggle_group_call_setting.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_toggle_invites.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_toggle_no_forwards.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_toggle_pre_history_hidden.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_toggle_signatures.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_toggle_slow_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_event_action_update_pinned.py
+-rw-r--r--   0 root         (0) root         (0)     6723 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_admin_log_events_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3666 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_forbidden.py
+-rw-r--r--   0 root         (0) root         (0)    25149 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_full.py
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_location.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_location_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_messages_filter.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_messages_filter_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_participant.py
+-rw-r--r--   0 root         (0) root         (0)     4408 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_participant_admin.py
+-rw-r--r--   0 root         (0) root         (0)     3356 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_participant_banned.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_participant_creator.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_participant_left.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_participant_self.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_participants_admins.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_participants_banned.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_participants_bots.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_participants_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_participants_kicked.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_participants_mentions.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_participants_recent.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channel_participants_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.202870 pyrogeram-2.0.107/pyrogram/raw/types/channels/
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channels/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3091 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channels/admin_log_results.py
+-rw-r--r--   0 root         (0) root         (0)     3124 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channels/channel_participant.py
+-rw-r--r--   0 root         (0) root         (0)     3361 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channels/channel_participants.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channels/channel_participants_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     3020 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channels/send_as_peers.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channels/sponsored_message_report_result_ads_hidden.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channels/sponsored_message_report_result_choose_option.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/channels/sponsored_message_report_result_reported.py
+-rw-r--r--   0 root         (0) root         (0)     6739 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat.py
+-rw-r--r--   0 root         (0) root         (0)     6678 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_admin_rights.py
+-rw-r--r--   0 root         (0) root         (0)     2884 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_admin_with_invites.py
+-rw-r--r--   0 root         (0) root         (0)     8464 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_banned_rights.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2368 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_forbidden.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_full.py
+-rw-r--r--   0 root         (0) root         (0)     6223 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_invite_already.py
+-rw-r--r--   0 root         (0) root         (0)     6137 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_invite_exported.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_invite_importer.py
+-rw-r--r--   0 root         (0) root         (0)     2660 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_invite_peek.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_invite_public_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2414 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_onlines.py
+-rw-r--r--   0 root         (0) root         (0)     2673 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_participant.py
+-rw-r--r--   0 root         (0) root         (0)     2693 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_participant_admin.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_participant_creator.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_participants.py
+-rw-r--r--   0 root         (0) root         (0)     2879 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_participants_forbidden.py
+-rw-r--r--   0 root         (0) root         (0)     3197 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_photo_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2372 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_reactions_all.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_reactions_none.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chat_reactions_some.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.202870 pyrogeram-2.0.107/pyrogram/raw/types/chatlists/
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chatlists/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3654 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chatlists/chatlist_invite.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chatlists/chatlist_invite_already.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chatlists/chatlist_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2882 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chatlists/exported_chatlist_invite.py
+-rw-r--r--   0 root         (0) root         (0)     3118 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/chatlists/exported_invites.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/client_dh_inner_data.py
+-rw-r--r--   0 root         (0) root         (0)     4977 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/code_settings.py
+-rw-r--r--   0 root         (0) root         (0)    19310 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/config.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/connected_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contact.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contact_birthday.py
+-rw-r--r--   0 root         (0) root         (0)     2700 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contact_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.206870 pyrogeram-2.0.107/pyrogram/raw/types/contacts/
+-rw-r--r--   0 root         (0) root         (0)     1588 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contacts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contacts/blocked.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contacts/blocked_slice.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contacts/contact_birthdays.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contacts/contacts.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contacts/contacts_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contacts/found.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contacts/imported_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contacts/resolved_peer.py
+-rw-r--r--   0 root         (0) root         (0)     3092 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contacts/top_peers.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contacts/top_peers_disabled.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/contacts/top_peers_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/data_json.py
+-rw-r--r--   0 root         (0) root         (0)     4637 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/dc_option.py
+-rw-r--r--   0 root         (0) root         (0)     2445 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/default_history_ttl.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/destroy_auth_key_fail.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/destroy_auth_key_none.py
+-rw-r--r--   0 root         (0) root         (0)     2264 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/destroy_auth_key_ok.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/destroy_session_none.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/destroy_session_ok.py
+-rw-r--r--   0 root         (0) root         (0)     2981 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/dh_gen_fail.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/dh_gen_ok.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/dh_gen_retry.py
+-rw-r--r--   0 root         (0) root         (0)     7001 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/dialog.py
+-rw-r--r--   0 root         (0) root         (0)     6583 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/dialog_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/dialog_filter_chatlist.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/dialog_filter_default.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/dialog_filter_suggested.py
+-rw-r--r--   0 root         (0) root         (0)     4609 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/dialog_folder.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/dialog_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2461 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/dialog_peer_folder.py
+-rw-r--r--   0 root         (0) root         (0)     5188 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/document.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/document_attribute_animated.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/document_attribute_audio.py
+-rw-r--r--   0 root         (0) root         (0)     3154 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/document_attribute_custom_emoji.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/document_attribute_filename.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/document_attribute_has_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/document_attribute_image_size.py
+-rw-r--r--   0 root         (0) root         (0)     3328 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/document_attribute_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     4120 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/document_attribute_video.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/document_empty.py
+-rw-r--r--   0 root         (0) root         (0)     4414 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/draft_message.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/draft_message_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/email_verification_apple.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/email_verification_code.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/email_verification_google.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/email_verify_purpose_login_change.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/email_verify_purpose_login_setup.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/email_verify_purpose_passport.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/emoji_group.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/emoji_keyword.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/emoji_keyword_deleted.py
+-rw-r--r--   0 root         (0) root         (0)     3346 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/emoji_keywords_difference.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/emoji_language.py
+-rw-r--r--   0 root         (0) root         (0)     2881 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/emoji_list.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/emoji_list_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/emoji_status_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2470 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/emoji_status_until.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/emoji_url.py
+-rw-r--r--   0 root         (0) root         (0)     3906 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/encrypted_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2845 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/encrypted_chat_discarded.py
+-rw-r--r--   0 root         (0) root         (0)     2445 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/encrypted_chat_empty.py
+-rw-r--r--   0 root         (0) root         (0)     4049 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/encrypted_chat_requested.py
+-rw-r--r--   0 root         (0) root         (0)     3415 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/encrypted_chat_waiting.py
+-rw-r--r--   0 root         (0) root         (0)     3332 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/encrypted_file.py
+-rw-r--r--   0 root         (0) root         (0)     2282 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/encrypted_file_empty.py
+-rw-r--r--   0 root         (0) root         (0)     3131 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/encrypted_message.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/encrypted_message_service.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/exported_chatlist_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/exported_contact_token.py
+-rw-r--r--   0 root         (0) root         (0)     2621 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/exported_message_link.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/exported_story_link.py
+-rw-r--r--   0 root         (0) root         (0)     2856 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/file_hash.py
+-rw-r--r--   0 root         (0) root         (0)     4058 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/folder.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/folder_peer.py
+-rw-r--r--   0 root         (0) root         (0)     7439 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/forum_topic.py
+-rw-r--r--   0 root         (0) root         (0)     2187 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/forum_topic_deleted.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.206870 pyrogeram-2.0.107/pyrogram/raw/types/fragment/
+-rw-r--r--   0 root         (0) root         (0)     1181 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/fragment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3694 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/fragment/collectible_info.py
+-rw-r--r--   0 root         (0) root         (0)     3815 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/game.py
+-rw-r--r--   0 root         (0) root         (0)     3145 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/geo_point.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/geo_point_empty.py
+-rw-r--r--   0 root         (0) root         (0)     4540 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/global_privacy_settings.py
+-rw-r--r--   0 root         (0) root         (0)     8365 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/group_call.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/group_call_discarded.py
+-rw-r--r--   0 root         (0) root         (0)     8275 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/group_call_participant.py
+-rw-r--r--   0 root         (0) root         (0)     3485 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/group_call_participant_video.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/group_call_participant_video_source_group.py
+-rw-r--r--   0 root         (0) root         (0)     2777 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/group_call_stream_channel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.210870 pyrogeram-2.0.107/pyrogram/raw/types/help/
+-rw-r--r--   0 root         (0) root         (0)     2578 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2653 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/app_config.py
+-rw-r--r--   0 root         (0) root         (0)     2285 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/app_config_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/app_update.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/config_simple.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/countries_list.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/countries_list_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     3460 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/country.py
+-rw-r--r--   0 root         (0) root         (0)     3153 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/country_code.py
+-rw-r--r--   0 root         (0) root         (0)     3248 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/deep_link_info.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/deep_link_info_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/invite_text.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/no_app_update.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/passport_config.py
+-rw-r--r--   0 root         (0) root         (0)     2315 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/passport_config_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     4476 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/peer_color_option.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/peer_color_profile_set.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/peer_color_set.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/peer_colors.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/peer_colors_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/premium_promo.py
+-rw-r--r--   0 root         (0) root         (0)     4265 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/promo_data.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/promo_data_empty.py
+-rw-r--r--   0 root         (0) root         (0)     3012 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/recent_me_urls.py
+-rw-r--r--   0 root         (0) root         (0)     2673 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/support.py
+-rw-r--r--   0 root         (0) root         (0)     2395 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/support_name.py
+-rw-r--r--   0 root         (0) root         (0)     3519 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/terms_of_service.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/terms_of_service_update.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/terms_of_service_update_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/timezones_list.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/timezones_list_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/user_info.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/help/user_info_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/high_score.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/http_wait.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/imported_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/inline_bot_switch_pm.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/inline_bot_web_view.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/inline_query_peer_type_bot_pm.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/inline_query_peer_type_broadcast.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/inline_query_peer_type_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/inline_query_peer_type_megagroup.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/inline_query_peer_type_pm.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/inline_query_peer_type_same_bot_pm.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_app_event.py
+-rw-r--r--   0 root         (0) root         (0)     2434 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_app_id.py
+-rw-r--r--   0 root         (0) root         (0)     2540 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_app_short_name.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_inline_message_game.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_inline_message_id.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_inline_message_id64.py
+-rw-r--r--   0 root         (0) root         (0)     3632 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_inline_message_media_auto.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_inline_message_media_contact.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_inline_message_media_geo.py
+-rw-r--r--   0 root         (0) root         (0)     4565 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_inline_message_media_invoice.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_inline_message_media_venue.py
+-rw-r--r--   0 root         (0) root         (0)     4814 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_inline_message_media_web_page.py
+-rw-r--r--   0 root         (0) root         (0)     3906 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_inline_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     4825 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     3921 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_inline_result_document.py
+-rw-r--r--   0 root         (0) root         (0)     2838 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_inline_result_game.py
+-rw-r--r--   0 root         (0) root         (0)     3051 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_bot_inline_result_photo.py
+-rw-r--r--   0 root         (0) root         (0)     3387 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_business_away_message.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_business_bot_recipients.py
+-rw-r--r--   0 root         (0) root         (0)     3139 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_business_chat_link.py
+-rw-r--r--   0 root         (0) root         (0)     2989 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_business_greeting_message.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_business_intro.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_business_recipients.py
+-rw-r--r--   0 root         (0) root         (0)     2503 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_channel_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_channel_from_message.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_chat_photo_empty.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_chat_uploaded_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_chatlist_dialog_filter.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_check_password_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_check_password_srp.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_client_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_collectible_phone.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_collectible_username.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_dialog_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_dialog_peer_folder.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_document.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_document_empty.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_document_file_location.py
+-rw-r--r--   0 root         (0) root         (0)     2503 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_encrypted_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2461 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_encrypted_file.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_encrypted_file_big_uploaded.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_encrypted_file_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_encrypted_file_location.py
+-rw-r--r--   0 root         (0) root         (0)     2987 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_encrypted_file_uploaded.py
+-rw-r--r--   0 root         (0) root         (0)     2809 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_file.py
+-rw-r--r--   0 root         (0) root         (0)     2560 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_file_big.py
+-rw-r--r--   0 root         (0) root         (0)     2981 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_file_location.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_folder_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2422 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_game_id.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_game_short_name.py
+-rw-r--r--   0 root         (0) root         (0)     2913 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_geo_point.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_geo_point_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_group_call_stream.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_invoice_message.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_invoice_premium_gift_code.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_invoice_slug.py
+-rw-r--r--   0 root         (0) root         (0)     4159 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_keyboard_button_request_peer.py
+-rw-r--r--   0 root         (0) root         (0)     3482 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_keyboard_button_url_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_keyboard_button_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_area_channel_post.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_area_venue.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_dice.py
+-rw-r--r--   0 root         (0) root         (0)     3356 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_document.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_document_external.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_game.py
+-rw-r--r--   0 root         (0) root         (0)     4004 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_geo_live.py
+-rw-r--r--   0 root         (0) root         (0)     2331 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_geo_point.py
+-rw-r--r--   0 root         (0) root         (0)     4928 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_invoice.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_photo_external.py
+-rw-r--r--   0 root         (0) root         (0)     3744 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_poll.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_story.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_uploaded_document.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_uploaded_photo.py
+-rw-r--r--   0 root         (0) root         (0)     3426 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_venue.py
+-rw-r--r--   0 root         (0) root         (0)     3231 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_media_web_page.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_message_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_message_entity_mention_name.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_message_id.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_message_pinned.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_message_reply_to.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_chat_photos.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_document.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_geo.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_gif.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_music.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_my_mentions.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_phone_calls.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_photo_video.py
+-rw-r--r--   0 root         (0) root         (0)     2099 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_photos.py
+-rw-r--r--   0 root         (0) root         (0)     2099 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_pinned.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_round_video.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_round_voice.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_url.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_video.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_messages_filter_voice.py
+-rw-r--r--   0 root         (0) root         (0)     2084 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_notify_broadcasts.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_notify_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_notify_forum_topic.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_notify_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_notify_users.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_payment_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_payment_credentials_apple_pay.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_payment_credentials_google_pay.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_payment_credentials_saved.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_peer_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_peer_channel_from_message.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_peer_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_peer_empty.py
+-rw-r--r--   0 root         (0) root         (0)     5230 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_peer_notify_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2815 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_peer_photo_file_location.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_peer_self.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_peer_user.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_peer_user_from_message.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_phone_call.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_phone_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_photo_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2999 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_photo_file_location.py
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_photo_legacy_file_location.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_key_about.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_key_added_by_phone.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_key_birthday.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_key_chat_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_key_forwards.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_key_phone_call.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_key_phone_number.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_key_phone_p2_p.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_key_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_key_status_timestamp.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_key_voice_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_value_allow_all.py
+-rw-r--r--   0 root         (0) root         (0)     2349 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_value_allow_chat_participants.py
+-rw-r--r--   0 root         (0) root         (0)     2137 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_value_allow_close_friends.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_value_allow_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_value_allow_premium.py
+-rw-r--r--   0 root         (0) root         (0)     2343 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_value_allow_users.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_value_disallow_all.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_value_disallow_chat_participants.py
+-rw-r--r--   0 root         (0) root         (0)     2131 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_value_disallow_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_privacy_value_disallow_users.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_quick_reply_shortcut.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_quick_reply_shortcut_id.py
+-rw-r--r--   0 root         (0) root         (0)     4696 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_reply_to_message.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_reply_to_story.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_report_reason_child_abuse.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_report_reason_copyright.py
+-rw-r--r--   0 root         (0) root         (0)     2081 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_report_reason_fake.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_report_reason_geo_irrelevant.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_report_reason_illegal_drugs.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_report_reason_other.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_report_reason_personal_details.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_report_reason_pornography.py
+-rw-r--r--   0 root         (0) root         (0)     2081 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_report_reason_spam.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_report_reason_violence.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_secure_file.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_secure_file_location.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_secure_file_uploaded.py
+-rw-r--r--   0 root         (0) root         (0)     5672 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_secure_value.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_single_media.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_sticker_set_animated_emoji.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_sticker_set_animated_emoji_animations.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_sticker_set_dice.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_sticker_set_emoji_channel_default_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_sticker_set_emoji_default_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_sticker_set_emoji_default_topic_icons.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_sticker_set_emoji_generic_animations.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_sticker_set_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_sticker_set_id.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_sticker_set_item.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_sticker_set_premium_gifts.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_sticker_set_short_name.py
+-rw-r--r--   0 root         (0) root         (0)     2635 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_sticker_set_thumb.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_stickered_media_document.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_stickered_media_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_store_payment_gift_premium.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_store_payment_premium_gift_code.py
+-rw-r--r--   0 root         (0) root         (0)     5646 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_store_payment_premium_giveaway.py
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_store_payment_premium_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_takeout_file_location.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_theme.py
+-rw-r--r--   0 root         (0) root         (0)     5118 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_theme_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_theme_slug.py
+-rw-r--r--   0 root         (0) root         (0)     2461 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_user.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_user_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_user_from_message.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_user_self.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_wall_paper.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_wall_paper_no_file.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_wall_paper_slug.py
+-rw-r--r--   0 root         (0) root         (0)     2981 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_web_document.py
+-rw-r--r--   0 root         (0) root         (0)     3607 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_web_file_audio_album_thumb_location.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_web_file_geo_point_location.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/input_web_file_location.py
+-rw-r--r--   0 root         (0) root         (0)     6935 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/ip_port.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/ip_port_secret.py
+-rw-r--r--   0 root         (0) root         (0)     2264 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/json_array.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/json_bool.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/json_null.py
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/json_number.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/json_object.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/json_object_value.py
+-rw-r--r--   0 root         (0) root         (0)     2185 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/json_string.py
+-rw-r--r--   0 root         (0) root         (0)     2197 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button_buy.py
+-rw-r--r--   0 root         (0) root         (0)     2821 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button_callback.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button_game.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button_request_geo_location.py
+-rw-r--r--   0 root         (0) root         (0)     3059 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button_request_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button_request_phone.py
+-rw-r--r--   0 root         (0) root         (0)     2625 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button_request_poll.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button_row.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button_simple_web_view.py
+-rw-r--r--   0 root         (0) root         (0)     3300 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button_switch_inline.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button_url.py
+-rw-r--r--   0 root         (0) root         (0)     3073 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button_url_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2405 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/keyboard_button_web_view.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/labeled_price.py
+-rw-r--r--   0 root         (0) root         (0)     3302 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/lang_pack_difference.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/lang_pack_language.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/lang_pack_string.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/lang_pack_string_deleted.py
+-rw-r--r--   0 root         (0) root         (0)     4740 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/lang_pack_string_pluralized.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/mask_coords.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/media_area_channel_post.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/media_area_coordinates.py
+-rw-r--r--   0 root         (0) root         (0)     2609 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/media_area_geo_point.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/media_area_suggested_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     3704 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/media_area_venue.py
+-rw-r--r--   0 root         (0) root         (0)    15532 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_boost_apply.py
+-rw-r--r--   0 root         (0) root         (0)     3448 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_bot_allowed.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_channel_create.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_channel_migrate_from.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_chat_add_user.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_chat_create.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_chat_delete_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_chat_delete_user.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_chat_edit_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_chat_edit_title.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_chat_joined_by_link.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_chat_joined_by_request.py
+-rw-r--r--   0 root         (0) root         (0)     2303 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_chat_migrate_to.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_contact_sign_up.py
+-rw-r--r--   0 root         (0) root         (0)     2267 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_custom_action.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_game_score.py
+-rw-r--r--   0 root         (0) root         (0)     2802 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_geo_proximity_reached.py
+-rw-r--r--   0 root         (0) root         (0)     5192 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_gift_code.py
+-rw-r--r--   0 root         (0) root         (0)     3649 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_gift_premium.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_giveaway_launch.py
+-rw-r--r--   0 root         (0) root         (0)     2625 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_giveaway_results.py
+-rw-r--r--   0 root         (0) root         (0)     2743 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_group_call_scheduled.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_history_clear.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_invite_to_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     3674 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_payment_sent.py
+-rw-r--r--   0 root         (0) root         (0)     4696 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_payment_sent_me.py
+-rw-r--r--   0 root         (0) root         (0)     3420 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_phone_call.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_pin_message.py
+-rw-r--r--   0 root         (0) root         (0)     2552 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_requested_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2612 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_requested_peer_sent_me.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_screenshot_taken.py
+-rw-r--r--   0 root         (0) root         (0)     2372 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_secure_values_sent.py
+-rw-r--r--   0 root         (0) root         (0)     2754 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_secure_values_sent_me.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_set_chat_theme.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_set_chat_wall_paper.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_set_messages_ttl.py
+-rw-r--r--   0 root         (0) root         (0)     2322 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_suggest_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2980 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_topic_create.py
+-rw-r--r--   0 root         (0) root         (0)     3607 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_topic_edit.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_web_view_data_sent.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_action_web_view_data_sent_me.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_bank_card.py
+-rw-r--r--   0 root         (0) root         (0)     2459 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_blockquote.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_bold.py
+-rw-r--r--   0 root         (0) root         (0)     2461 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_bot_command.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_cashtag.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_code.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_custom_emoji.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_email.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_hashtag.py
+-rw-r--r--   0 root         (0) root         (0)     2445 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_italic.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_mention.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_mention_name.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_phone.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_pre.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_spoiler.py
+-rw-r--r--   0 root         (0) root         (0)     2445 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_strike.py
+-rw-r--r--   0 root         (0) root         (0)     2629 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_text_url.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_underline.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_unknown.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_entity_url.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_extended_media.py
+-rw-r--r--   0 root         (0) root         (0)     3604 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_extended_media_preview.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_fwd_header.py
+-rw-r--r--   0 root         (0) root         (0)     3468 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2724 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_dice.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_document.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2529 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_game.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_geo.py
+-rw-r--r--   0 root         (0) root         (0)     3800 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_geo_live.py
+-rw-r--r--   0 root         (0) root         (0)     5044 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_giveaway.py
+-rw-r--r--   0 root         (0) root         (0)     5874 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_giveaway_results.py
+-rw-r--r--   0 root         (0) root         (0)     5661 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_invoice.py
+-rw-r--r--   0 root         (0) root         (0)     3435 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2814 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_poll.py
+-rw-r--r--   0 root         (0) root         (0)     3468 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_story.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_unsupported.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_venue.py
+-rw-r--r--   0 root         (0) root         (0)     3837 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_media_web_page.py
+-rw-r--r--   0 root         (0) root         (0)     3519 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_peer_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_peer_vote.py
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_peer_vote_input_option.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_peer_vote_multiple.py
+-rw-r--r--   0 root         (0) root         (0)     2621 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_range.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     4526 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_replies.py
+-rw-r--r--   0 root         (0) root         (0)     6819 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_reply_header.py
+-rw-r--r--   0 root         (0) root         (0)     2503 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_reply_story_header.py
+-rw-r--r--   0 root         (0) root         (0)     5857 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_service.py
+-rw-r--r--   0 root         (0) root         (0)     3244 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/message_views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.226870 pyrogeram-2.0.107/pyrogram/raw/types/messages/
+-rw-r--r--   0 root         (0) root         (0)     5126 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/affected_found_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/affected_history.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/affected_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/all_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/all_stickers_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/archived_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/available_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2351 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/available_reactions_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/bot_app.py
+-rw-r--r--   0 root         (0) root         (0)     4053 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/bot_callback_answer.py
+-rw-r--r--   0 root         (0) root         (0)     5040 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/bot_results.py
+-rw-r--r--   0 root         (0) root         (0)     4995 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/channel_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2869 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/chat_admins_with_invites.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/chat_full.py
+-rw-r--r--   0 root         (0) root         (0)     3080 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/chat_invite_importers.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/chats.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/chats_slice.py
+-rw-r--r--   0 root         (0) root         (0)     2552 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/checked_history_import_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/dh_config.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/dh_config_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/dialog_filters.py
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/dialogs_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     3523 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/dialogs_slice.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/discussion_message.py
+-rw-r--r--   0 root         (0) root         (0)     2794 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/emoji_groups.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/emoji_groups_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/exported_chat_invite.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/exported_chat_invite_replaced.py
+-rw-r--r--   0 root         (0) root         (0)     3062 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/exported_chat_invites.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/faved_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/faved_stickers_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     3601 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/featured_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/featured_stickers_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/forum_topics.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/found_sticker_sets.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/found_sticker_sets_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     2813 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/high_scores.py
+-rw-r--r--   0 root         (0) root         (0)     2407 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/history_import.py
+-rw-r--r--   0 root         (0) root         (0)     3132 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/history_import_parsed.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/inactive_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2959 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/invited_users.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/message_edit_data.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/message_reactions_list.py
+-rw-r--r--   0 root         (0) root         (0)     3040 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/message_views.py
+-rw-r--r--   0 root         (0) root         (0)     3502 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/messages.py
+-rw-r--r--   0 root         (0) root         (0)     2924 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/messages_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     4911 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/messages_slice.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/my_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/peer_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     3044 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/peer_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/quick_replies.py
+-rw-r--r--   0 root         (0) root         (0)     2315 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/quick_replies_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     2801 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/reactions_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     3263 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/recent_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/recent_stickers_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/saved_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/saved_dialogs_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     3617 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/saved_dialogs_slice.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/saved_gifs.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/saved_gifs_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     2748 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/saved_reaction_tags.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/saved_reaction_tags_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     3031 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/search_counter.py
+-rw-r--r--   0 root         (0) root         (0)     4932 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/search_results_calendar.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/search_results_positions.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/sent_encrypted_file.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/sent_encrypted_message.py
+-rw-r--r--   0 root         (0) root         (0)     3601 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/sponsored_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/sponsored_messages_empty.py
+-rw-r--r--   0 root         (0) root         (0)     3697 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/sticker_set_install_result_archive.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/sticker_set_install_result_success.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/sticker_set_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/stickers_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     4100 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/transcribed_audio.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/translate_result.py
+-rw-r--r--   0 root         (0) root         (0)     3698 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/votes_list.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/messages/web_page.py
+-rw-r--r--   0 root         (0) root         (0)     3123 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/missing_invitee.py
+-rw-r--r--   0 root         (0) root         (0)     2909 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/msg_detailed_info.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/msg_new_detailed_info.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/msg_resend_ans_req.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/msg_resend_req.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/msgs_ack.py
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/msgs_all_info.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/msgs_state_info.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/msgs_state_req.py
+-rw-r--r--   0 root         (0) root         (0)     3511 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/my_boost.py
+-rw-r--r--   0 root         (0) root         (0)     2863 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/nearest_dc.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/new_session_created.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/notification_sound_default.py
+-rw-r--r--   0 root         (0) root         (0)     2430 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/notification_sound_local.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/notification_sound_none.py
+-rw-r--r--   0 root         (0) root         (0)     2231 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/notification_sound_ringtone.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/notify_broadcasts.py
+-rw-r--r--   0 root         (0) root         (0)     2039 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/notify_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/notify_forum_topic.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/notify_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2039 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/notify_users.py
+-rw-r--r--   0 root         (0) root         (0)     2409 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/outbox_read_date.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_anchor.py
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_audio.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_author_date.py
+-rw-r--r--   0 root         (0) root         (0)     2542 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_blockquote.py
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_collage.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_cover.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_details.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_divider.py
+-rw-r--r--   0 root         (0) root         (0)     4734 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_embed.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_embed_post.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_footer.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_header.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_kicker.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_list.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_map.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_ordered_list.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_paragraph.py
+-rw-r--r--   0 root         (0) root         (0)     3309 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_preformatted.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_pullquote.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_related_articles.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_slideshow.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_subheader.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_subtitle.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_table.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_title.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_unsupported.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_block_video.py
+-rw-r--r--   0 root         (0) root         (0)     2503 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_caption.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_list_item_blocks.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_list_item_text.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_list_ordered_item_blocks.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_list_ordered_item_text.py
+-rw-r--r--   0 root         (0) root         (0)     4487 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_related_article.py
+-rw-r--r--   0 root         (0) root         (0)     4718 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_table_cell.py
+-rw-r--r--   0 root         (0) root         (0)     2295 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/page_table_row.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/password_kdf_algo_sha256_sha256_pbkdf2_hmacsha512iter100000_sha256_mod_pow.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/password_kdf_algo_unknown.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payment_charge.py
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payment_form_method.py
+-rw-r--r--   0 root         (0) root         (0)     3677 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payment_requested_info.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payment_saved_credentials_card.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.226870 pyrogeram-2.0.107/pyrogram/raw/types/payments/
+-rw-r--r--   0 root         (0) root         (0)     1650 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payments/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payments/bank_card_data.py
+-rw-r--r--   0 root         (0) root         (0)     5157 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payments/checked_gift_code.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payments/exported_invoice.py
+-rw-r--r--   0 root         (0) root         (0)     4789 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payments/giveaway_info.py
+-rw-r--r--   0 root         (0) root         (0)     4341 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payments/giveaway_info_results.py
+-rw-r--r--   0 root         (0) root         (0)     7969 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payments/payment_form.py
+-rw-r--r--   0 root         (0) root         (0)     6468 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payments/payment_receipt.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payments/payment_result.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payments/payment_verification_needed.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payments/saved_info.py
+-rw-r--r--   0 root         (0) root         (0)     3219 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/payments/validated_requested_info.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/peer_blocked.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/peer_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/peer_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/peer_color.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/peer_located.py
+-rw-r--r--   0 root         (0) root         (0)     7773 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/peer_notify_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/peer_self_located.py
+-rw-r--r--   0 root         (0) root         (0)     8271 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/peer_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2989 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/peer_stories.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/peer_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.230870 pyrogeram-2.0.107/pyrogram/raw/types/phone/
+-rw-r--r--   0 root         (0) root         (0)     1483 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone/exported_group_call_invite.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone/group_call.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone/group_call_stream_channels.py
+-rw-r--r--   0 root         (0) root         (0)     2635 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone/group_call_stream_rtmp_url.py
+-rw-r--r--   0 root         (0) root         (0)     3825 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone/group_participants.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone/join_as_peers.py
+-rw-r--r--   0 root         (0) root         (0)     2821 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone/phone_call.py
+-rw-r--r--   0 root         (0) root         (0)     5701 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone_call.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone_call_accepted.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone_call_discard_reason_busy.py
+-rw-r--r--   0 root         (0) root         (0)     2135 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone_call_discard_reason_disconnect.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone_call_discard_reason_hangup.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone_call_discard_reason_missed.py
+-rw-r--r--   0 root         (0) root         (0)     3952 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone_call_discarded.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone_call_empty.py
+-rw-r--r--   0 root         (0) root         (0)     3465 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone_call_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3995 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone_call_requested.py
+-rw-r--r--   0 root         (0) root         (0)     4194 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone_call_waiting.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone_connection.py
+-rw-r--r--   0 root         (0) root         (0)     3739 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/phone_connection_webrtc.py
+-rw-r--r--   0 root         (0) root         (0)     4203 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/photo.py
+-rw-r--r--   0 root         (0) root         (0)     2721 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/photo_cached_size.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/photo_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/photo_path_size.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/photo_size.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/photo_size_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2784 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/photo_size_progressive.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/photo_stripped_size.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.230870 pyrogeram-2.0.107/pyrogram/raw/types/photos/
+-rw-r--r--   0 root         (0) root         (0)     1225 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/photos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/photos/photo.py
+-rw-r--r--   0 root         (0) root         (0)     2721 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/photos/photos.py
+-rw-r--r--   0 root         (0) root         (0)     2941 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/photos/photos_slice.py
+-rw-r--r--   0 root         (0) root         (0)     4709 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/poll.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/poll_answer.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/poll_answer_voters.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/poll_results.py
+-rw-r--r--   0 root         (0) root         (0)     2612 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/pong.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/popular_contact.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/post_address.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/post_interaction_counters_message.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/post_interaction_counters_story.py
+-rw-r--r--   0 root         (0) root         (0)     3220 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/pq_inner_data.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/pq_inner_data_dc.py
+-rw-r--r--   0 root         (0) root         (0)     3481 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/pq_inner_data_temp.py
+-rw-r--r--   0 root         (0) root         (0)     3662 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/pq_inner_data_temp_dc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.230870 pyrogeram-2.0.107/pyrogram/raw/types/premium/
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/premium/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3444 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/premium/boosts_list.py
+-rw-r--r--   0 root         (0) root         (0)     6075 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/premium/boosts_status.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/premium/my_boosts.py
+-rw-r--r--   0 root         (0) root         (0)     4049 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/premium_gift_code_option.py
+-rw-r--r--   0 root         (0) root         (0)     3372 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/premium_gift_option.py
+-rw-r--r--   0 root         (0) root         (0)     4483 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/premium_subscription_option.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/prepaid_giveaway.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_key_about.py
+-rw-r--r--   0 root         (0) root         (0)     2083 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_key_added_by_phone.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_key_birthday.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_key_chat_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_key_forwards.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_key_phone_call.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_key_phone_number.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_key_phone_p2_p.py
+-rw-r--r--   0 root         (0) root         (0)     2083 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_key_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_key_status_timestamp.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_key_voice_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_value_allow_all.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_value_allow_chat_participants.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_value_allow_close_friends.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_value_allow_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_value_allow_premium.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_value_allow_users.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_value_disallow_all.py
+-rw-r--r--   0 root         (0) root         (0)     2336 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_value_disallow_chat_participants.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_value_disallow_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/privacy_value_disallow_users.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/public_forward_message.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/public_forward_story.py
+-rw-r--r--   0 root         (0) root         (0)     2919 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/quick_reply.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/reaction_count.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/reaction_custom_emoji.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/reaction_emoji.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/reaction_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2664 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/read_participant_date.py
+-rw-r--r--   0 root         (0) root         (0)     2625 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/received_notify_message.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/recent_me_url_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/recent_me_url_chat_invite.py
+-rw-r--r--   0 root         (0) root         (0)     2486 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/recent_me_url_sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/recent_me_url_unknown.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/recent_me_url_user.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/reply_inline_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/reply_keyboard_force_reply.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/reply_keyboard_hide.py
+-rw-r--r--   0 root         (0) root         (0)     3925 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/reply_keyboard_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3917 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/request_peer_type_broadcast.py
+-rw-r--r--   0 root         (0) root         (0)     4586 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/request_peer_type_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/request_peer_type_user.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/requested_peer_channel.py
+-rw-r--r--   0 root         (0) root         (0)     3037 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/requested_peer_chat.py
+-rw-r--r--   0 root         (0) root         (0)     3877 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/requested_peer_user.py
+-rw-r--r--   0 root         (0) root         (0)     3299 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/res_pq.py
+-rw-r--r--   0 root         (0) root         (0)     2644 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/restriction_reason.py
+-rw-r--r--   0 root         (0) root         (0)     2833 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/rpc_answer_dropped.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/rpc_answer_dropped_running.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/rpc_answer_unknown.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/rpc_error.py
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/rpc_result.py
+-rw-r--r--   0 root         (0) root         (0)     2780 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/saved_dialog.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/saved_phone_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2899 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/saved_reaction_tag.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/search_result_position.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/search_results_calendar_period.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_credentials_encrypted.py
+-rw-r--r--   0 root         (0) root         (0)     2621 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_data.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_file.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_file_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_password_kdf_algo_pbkdf2_hmacsha512iter100000.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_password_kdf_algo_sha512.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_password_kdf_algo_unknown.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_plain_email.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_plain_phone.py
+-rw-r--r--   0 root         (0) root         (0)     3382 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_required_type.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_required_type_one_of.py
+-rw-r--r--   0 root         (0) root         (0)     2972 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_secret_settings.py
+-rw-r--r--   0 root         (0) root         (0)     6019 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value.py
+-rw-r--r--   0 root         (0) root         (0)     2671 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_error.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_error_data.py
+-rw-r--r--   0 root         (0) root         (0)     2732 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_error_file.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_error_files.py
+-rw-r--r--   0 root         (0) root         (0)     2748 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_error_front_side.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_error_reverse_side.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_error_selfie.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_error_translation_file.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_error_translation_files.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_hash.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_type_address.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_type_bank_statement.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_type_driver_license.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_type_email.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_type_identity_card.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_type_internal_passport.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_type_passport.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_type_passport_registration.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_type_personal_details.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_type_phone.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_type_rental_agreement.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_type_temporary_registration.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/secure_value_type_utility_bill.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_as_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_cancel_action.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_choose_contact_action.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_choose_sticker_action.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_emoji_interaction.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_emoji_interaction_seen.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_game_play_action.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_geo_location_action.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_history_import_action.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_record_audio_action.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_record_round_action.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_record_video_action.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_typing_action.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_upload_audio_action.py
+-rw-r--r--   0 root         (0) root         (0)     2306 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_upload_document_action.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_upload_photo_action.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_upload_round_action.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/send_message_upload_video_action.py
+-rw-r--r--   0 root         (0) root         (0)     3331 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/server_dh_inner_data.py
+-rw-r--r--   0 root         (0) root         (0)     2993 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/server_dh_params_fail.py
+-rw-r--r--   0 root         (0) root         (0)     2992 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/server_dh_params_ok.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/shipping_option.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/simple_web_view_result_url.py
+-rw-r--r--   0 root         (0) root         (0)     2826 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/sms_job.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.230870 pyrogeram-2.0.107/pyrogram/raw/types/smsjobs/
+-rw-r--r--   0 root         (0) root         (0)     1207 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/smsjobs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/smsjobs/eligible_to_join.py
+-rw-r--r--   0 root         (0) root         (0)     4589 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/smsjobs/status.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/speaking_in_group_call_action.py
+-rw-r--r--   0 root         (0) root         (0)     8327 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/sponsored_message.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/sponsored_message_report_option.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/sponsored_web_page.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.230870 pyrogeram-2.0.107/pyrogram/raw/types/stats/
+-rw-r--r--   0 root         (0) root         (0)     1551 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats/broadcast_revenue_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats/broadcast_revenue_transactions.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats/broadcast_revenue_withdrawal_url.py
+-rw-r--r--   0 root         (0) root         (0)    11001 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats/broadcast_stats.py
+-rw-r--r--   0 root         (0) root         (0)     8061 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats/megagroup_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats/message_stats.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats/public_forwards.py
+-rw-r--r--   0 root         (0) root         (0)     2972 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats/story_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats_abs_value_and_prev.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats_date_range_days.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats_graph.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats_graph_async.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats_graph_error.py
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats_group_top_admin.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats_group_top_inviter.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats_group_top_poster.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats_percent_value.py
+-rw-r--r--   0 root         (0) root         (0)     2158 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stats_url.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/sticker_keyword.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/sticker_pack.py
+-rw-r--r--   0 root         (0) root         (0)     7563 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/sticker_set_covered.py
+-rw-r--r--   0 root         (0) root         (0)     3426 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/sticker_set_full_covered.py
+-rw-r--r--   0 root         (0) root         (0)     2786 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/sticker_set_multi_covered.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/sticker_set_no_covered.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.234870 pyrogeram-2.0.107/pyrogram/raw/types/stickers/
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stickers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stickers/suggested_short_name.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.234870 pyrogeram-2.0.107/pyrogram/raw/types/storage/
+-rw-r--r--   0 root         (0) root         (0)     1455 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/storage/file_gif.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/storage/file_jpeg.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/storage/file_mov.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/storage/file_mp3.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/storage/file_mp4.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/storage/file_partial.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/storage/file_pdf.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/storage/file_png.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/storage/file_unknown.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/storage/file_webp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.234870 pyrogeram-2.0.107/pyrogram/raw/types/stories/
+-rw-r--r--   0 root         (0) root         (0)     1432 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stories/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4160 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stories/all_stories.py
+-rw-r--r--   0 root         (0) root         (0)     2863 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stories/all_stories_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stories/peer_stories.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stories/stories.py
+-rw-r--r--   0 root         (0) root         (0)     3777 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stories/story_reactions_list.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stories/story_views.py
+-rw-r--r--   0 root         (0) root         (0)     4526 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stories/story_views_list.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/stories_stealth_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3554 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/story_fwd_header.py
+-rw-r--r--   0 root         (0) root         (0)     9044 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/story_item.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/story_item_deleted.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/story_item_skipped.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/story_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/story_reaction_public_forward.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/story_reaction_public_repost.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/story_view.py
+-rw-r--r--   0 root         (0) root         (0)     3027 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/story_view_public_forward.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/story_view_public_repost.py
+-rw-r--r--   0 root         (0) root         (0)     4496 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/story_views.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_anchor.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_bold.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_concat.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_email.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_fixed.py
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_image.py
+-rw-r--r--   0 root         (0) root         (0)     2232 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_italic.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_marked.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_phone.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_plain.py
+-rw-r--r--   0 root         (0) root         (0)     2232 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_strike.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_subscript.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_superscript.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_underline.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_url.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/text_with_entities.py
+-rw-r--r--   0 root         (0) root         (0)     5669 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/theme.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/theme_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/timezone.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/top_peer.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/top_peer_category_bots_inline.py
+-rw-r--r--   0 root         (0) root         (0)     2084 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/top_peer_category_bots_pm.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/top_peer_category_channels.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/top_peer_category_correspondents.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/top_peer_category_forward_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/top_peer_category_forward_users.py
+-rw-r--r--   0 root         (0) root         (0)     2084 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/top_peer_category_groups.py
+-rw-r--r--   0 root         (0) root         (0)     2821 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/top_peer_category_peers.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/top_peer_category_phone_calls.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_attach_menu_bots.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_auto_save_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_business_connect.py
+-rw-r--r--   0 root         (0) root         (0)     4050 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2671 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_chat_boost.py
+-rw-r--r--   0 root         (0) root         (0)     3382 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_chat_invite_requester.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_delete_business_message.py
+-rw-r--r--   0 root         (0) root         (0)     3347 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_edit_business_message.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_inline_send.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     3789 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_message_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_message_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_new_business_message.py
+-rw-r--r--   0 root         (0) root         (0)     4192 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_precheckout_query.py
+-rw-r--r--   0 root         (0) root         (0)     3066 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_shipping_query.py
+-rw-r--r--   0 root         (0) root         (0)     2814 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_stopped.py
+-rw-r--r--   0 root         (0) root         (0)     2270 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_webhook_json.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_bot_webhook_json_query.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_channel_available_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2704 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_channel_message_forwards.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_channel_message_views.py
+-rw-r--r--   0 root         (0) root         (0)     5061 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_channel_participant.py
+-rw-r--r--   0 root         (0) root         (0)     2818 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_channel_pinned_topic.py
+-rw-r--r--   0 root         (0) root         (0)     2728 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_channel_pinned_topics.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_channel_read_messages_contents.py
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_channel_too_long.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_channel_user_typing.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_channel_view_forum_as_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2959 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_channel_web_page.py
+-rw-r--r--   0 root         (0) root         (0)     2205 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_chat_default_banned_rights.py
+-rw-r--r--   0 root         (0) root         (0)     4686 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_chat_participant.py
+-rw-r--r--   0 root         (0) root         (0)     3139 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_chat_participant_add.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_chat_participant_admin.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_chat_participant_delete.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_chat_participants.py
+-rw-r--r--   0 root         (0) root         (0)     2802 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_chat_user_typing.py
+-rw-r--r--   0 root         (0) root         (0)     2039 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_config.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_contacts_reset.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_dc_options.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_delete_channel_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_delete_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_delete_quick_reply.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_delete_quick_reply_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2557 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_delete_scheduled_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2671 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_dialog_filter.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_dialog_filter_order.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_dialog_filters.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_dialog_pinned.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_dialog_unread_mark.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_draft_message.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_edit_channel_message.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_edit_message.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_encrypted_chat_typing.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_encrypted_messages_read.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_encryption.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_faved_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_folder_peers.py
+-rw-r--r--   0 root         (0) root         (0)     2459 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_geo_live_viewed.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     2663 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_group_call_connection.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_group_call_participants.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_inline_bot_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2340 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_lang_pack.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_lang_pack_too_long.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_login_token.py
+-rw-r--r--   0 root         (0) root         (0)     2871 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_message_extended_media.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_message_id.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_message_poll.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_message_poll_vote.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_message_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_move_sticker_set_to_top.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_new_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_new_channel_message.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_new_encrypted_message.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_new_message.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_new_quick_reply.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_new_scheduled_message.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_new_sticker_set.py
+-rw-r--r--   0 root         (0) root         (0)     2663 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_notify_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2992 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_peer_blocked.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_peer_history_ttl.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_peer_located.py
+-rw-r--r--   0 root         (0) root         (0)     2544 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_peer_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3137 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_peer_wallpaper.py
+-rw-r--r--   0 root         (0) root         (0)     2924 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_pending_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_phone_call.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_phone_call_signaling_data.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_pinned_channel_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_pinned_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_pinned_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_pinned_saved_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_privacy.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_pts_changed.py
+-rw-r--r--   0 root         (0) root         (0)     2373 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_quick_replies.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_quick_reply_message.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_read_channel_discussion_inbox.py
+-rw-r--r--   0 root         (0) root         (0)     2823 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_read_channel_discussion_outbox.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_read_channel_inbox.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_read_channel_outbox.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_read_featured_emoji_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_read_featured_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     3651 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_read_history_inbox.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_read_history_outbox.py
+-rw-r--r--   0 root         (0) root         (0)     3123 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_read_messages_contents.py
+-rw-r--r--   0 root         (0) root         (0)     2451 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_read_stories.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_recent_emoji_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_recent_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_recent_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_saved_dialog_pinned.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_saved_gifs.py
+-rw-r--r--   0 root         (0) root         (0)     2083 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_saved_reaction_tags.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_saved_ringtones.py
+-rw-r--r--   0 root         (0) root         (0)     2775 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_sent_story_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     4061 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_service_notification.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_short.py
+-rw-r--r--   0 root         (0) root         (0)    10863 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_short_chat_message.py
+-rw-r--r--   0 root         (0) root         (0)    10626 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_short_message.py
+-rw-r--r--   0 root         (0) root         (0)     8398 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_short_sent_message.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_sms_job.py
+-rw-r--r--   0 root         (0) root         (0)     2564 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_sticker_sets.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_sticker_sets_order.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_stories_stealth_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_story.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_story_id.py
+-rw-r--r--   0 root         (0) root         (0)     2231 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_theme.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_transcribed_audio.py
+-rw-r--r--   0 root         (0) root         (0)     2205 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_user.py
+-rw-r--r--   0 root         (0) root         (0)     2579 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_user_emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_user_name.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_user_phone.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_user_status.py
+-rw-r--r--   0 root         (0) root         (0)     2529 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_user_typing.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_web_page.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/update_web_view_result_sent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.238870 pyrogeram-2.0.107/pyrogram/raw/types/updates/
+-rw-r--r--   0 root         (0) root         (0)     1515 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/updates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/updates/channel_difference.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/updates/channel_difference_empty.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/updates/channel_difference_too_long.py
+-rw-r--r--   0 root         (0) root         (0)     4141 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/updates/difference.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/updates/difference_empty.py
+-rw-r--r--   0 root         (0) root         (0)     4282 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/updates/difference_slice.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/updates/difference_too_long.py
+-rw-r--r--   0 root         (0) root         (0)     3179 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/updates/state.py
+-rw-r--r--   0 root         (0) root         (0)     7409 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/updates_combined.py
+-rw-r--r--   0 root         (0) root         (0)     7141 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/updates_t.py
+-rw-r--r--   0 root         (0) root         (0)     6034 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/updates_too_long.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.238870 pyrogeram-2.0.107/pyrogram/raw/types/upload/
+-rw-r--r--   0 root         (0) root         (0)     1325 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/upload/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/upload/cdn_file.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/upload/cdn_file_reupload_needed.py
+-rw-r--r--   0 root         (0) root         (0)     2845 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/upload/file.py
+-rw-r--r--   0 root         (0) root         (0)     3540 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/upload/file_cdn_redirect.py
+-rw-r--r--   0 root         (0) root         (0)     3335 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/upload/web_file.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/url_auth_result_accepted.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/url_auth_result_default.py
+-rw-r--r--   0 root         (0) root         (0)     3131 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/url_auth_result_request.py
+-rw-r--r--   0 root         (0) root         (0)    17182 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/user.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/user_empty.py
+-rw-r--r--   0 root         (0) root         (0)    20054 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/user_full.py
+-rw-r--r--   0 root         (0) root         (0)     3508 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/user_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/user_profile_photo_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/user_status_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/user_status_last_month.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/user_status_last_week.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/user_status_offline.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/user_status_online.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/user_status_recently.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/username.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.238870 pyrogeram-2.0.107/pyrogram/raw/types/users/
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/users/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/users/user_full.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/video_size.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/video_size_emoji_markup.py
+-rw-r--r--   0 root         (0) root         (0)     2957 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/video_size_sticker_markup.py
+-rw-r--r--   0 root         (0) root         (0)     4732 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/wall_paper.py
+-rw-r--r--   0 root         (0) root         (0)     3494 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/wall_paper_no_file.py
+-rw-r--r--   0 root         (0) root         (0)     5870 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/wall_paper_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/web_authorization.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/web_document.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/web_document_no_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     8912 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/web_page.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/web_page_attribute_story.py
+-rw-r--r--   0 root         (0) root         (0)     3018 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/web_page_attribute_theme.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/web_page_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2550 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/web_page_not_modified.py
+-rw-r--r--   0 root         (0) root         (0)     2745 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/web_page_pending.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/web_view_message_sent.py
+-rw-r--r--   0 root         (0) root         (0)     2630 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/pyrogram/raw/types/web_view_result_url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.238870 pyrogeram-2.0.107/pyrogram/session/
+-rw-r--r--   0 root         (0) root         (0)      946 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/session/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11576 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/session/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.238870 pyrogeram-2.0.107/pyrogram/session/internals/
+-rw-r--r--   0 root         (0) root         (0)      992 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/session/internals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2564 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/session/internals/data_center.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1231 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0 root         (0) root         (0)    14152 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/session/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.242870 pyrogeram-2.0.107/pyrogram/storage/
+-rw-r--r--   0 root         (0) root         (0)     1104 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/storage/dummy_client.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/storage/file_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/storage/memory_storage.py
+-rw-r--r--   0 root         (0) root         (0)     8229 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/storage/mongo_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7895 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/storage/storage.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.242870 pyrogeram-2.0.107/pyrogram/types/
+-rw-r--r--   0 root         (0) root         (0)     1207 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.242870 pyrogeram-2.0.107/pyrogram/types/authorization/
+-rw-r--r--   0 root         (0) root         (0)     1013 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/authorization/terms_of_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.246870 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/
+-rw-r--r--   0 root         (0) root         (0)     3296 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2659 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_business_connection.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 root         (0) root         (0)     2863 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1324 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_info.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 root         (0) root         (0)    12872 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 root         (0) root         (0)     8195 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 root         (0) root         (0)     7289 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 root         (0) root         (0)     1678 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 root         (0) root         (0)     4650 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 root         (0) root         (0)     2414 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/request_peer_type_channel.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/request_peer_type_chat.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/request_peer_type_user.py
+-rw-r--r--   0 root         (0) root         (0)     1639 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.250870 pyrogeram-2.0.107/pyrogram/types/inline_mode/
+-rw-r--r--   0 root         (0) root         (0)     2830 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3737 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     7373 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     2486 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 root         (0) root         (0)     5857 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 root         (0) root         (0)     5159 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 root         (0) root         (0)     4104 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 root         (0) root         (0)     4463 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 root         (0) root         (0)     3106 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     4469 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 root         (0) root         (0)     4277 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 root         (0) root         (0)     5315 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 root         (0) root         (0)     4694 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 root         (0) root         (0)     5336 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 root         (0) root         (0)     4829 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 root         (0) root         (0)     5549 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.258870 pyrogeram-2.0.107/pyrogram/types/input_media/
+-rw-r--r--   0 root         (0) root         (0)     1550 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0 root         (0) root         (0)     3503 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_media/input_media_area.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_media/input_media_area_channel_post.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0 root         (0) root         (0)     3695 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.258870 pyrogeram-2.0.107/pyrogram/types/input_message_content/
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0 root         (0) root         (0)     3179 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_message_content/input_reply_to_message.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_message_content/input_reply_to_story.py
+-rw-r--r--   0 root         (0) root         (0)     2713 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.270870 pyrogeram-2.0.107/pyrogram/types/messages_and_media/
+-rw-r--r--   0 root         (0) root         (0)     3245 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4119 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0 root         (0) root         (0)     4144 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0 root         (0) root         (0)     2282 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0 root         (0) root         (0)     3484 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/exported_story_link.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0 root         (0) root         (0)     3739 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/giveaway.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/giveaway_launched.py
+-rw-r--r--   0 root         (0) root         (0)     4575 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/giveaway_result.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/media_area.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/media_area_channel_post.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/media_area_coordinates.py
+-rw-r--r--   0 root         (0) root         (0)   203597 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0 root         (0) root         (0)     4427 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/message_reaction_count_updated.py
+-rw-r--r--   0 root         (0) root         (0)     4299 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/message_reaction_updated.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2634 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/message_story.py
+-rw-r--r--   0 root         (0) root         (0)     4384 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0 root         (0) root         (0)     8091 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0 root         (0) root         (0)     2692 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/reaction_count.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/reaction_type.py
+-rw-r--r--   0 root         (0) root         (0)     7695 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/stickerset.py
+-rw-r--r--   0 root         (0) root         (0)     1878 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/stories_privacy_rules.py
+-rw-r--r--   0 root         (0) root         (0)    75413 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/story.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/story_deleted.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/story_forward_header.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/story_skipped.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/story_views.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 root         (0) root         (0)     3830 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 root         (0) root         (0)     2366 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0 root         (0) root         (0)     4464 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0 root         (0) root         (0)     3676 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0 root         (0) root         (0)     3279 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 root         (0) root         (0)     6426 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/web_page_empty.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/messages_and_media/web_page_preview.py
+-rw-r--r--   0 root         (0) root         (0)     4053 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.270870 pyrogeram-2.0.107/pyrogram/types/pyromod/
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/pyromod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/pyromod/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/pyromod/listener.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:34:39.278870 pyrogeram-2.0.107/pyrogram/types/user_and_chats/
+-rw-r--r--   0 root         (0) root         (0)     3607 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/birthday.py
+-rw-r--r--   0 root         (0) root         (0)     3032 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/business_info.py
+-rw-r--r--   0 root         (0) root         (0)     4303 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/business_message.py
+-rw-r--r--   0 root         (0) root         (0)     2843 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/business_recipients.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/business_weekly_open.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/business_working_hours.py
+-rw-r--r--   0 root         (0) root         (0)    43177 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_color.py
+-rw-r--r--   0 root         (0) root         (0)    22098 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0 root         (0) root         (0)     5589 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4654 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_joined_by_request.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 root         (0) root         (0)     9519 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     3749 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 root         (0) root         (0)    10174 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     4042 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2667 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     4979 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/forum_topic.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/forum_topic_closed.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/forum_topic_created.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/forum_topic_edited.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/forum_topic_reopened.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 root         (0) root         (0)     1338 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/peer_channel.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/peer_user.py
+-rw-r--r--   0 root         (0) root         (0)     1738 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0 root         (0) root         (0)    17777 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0 root         (0) root         (0)     1700 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 root         (0) root         (0)    15263 2024-04-24 15:22:13.000000 pyrogeram-2.0.107/pyrogram/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 15:34:39.278870 pyrogeram-2.0.107/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      599 2024-04-24 15:34:32.000000 pyrogeram-2.0.107/setup.py
```

### Comparing `pyrogeram-2.0.106/compiler/__init__.py` & `pyrogeram-2.0.107/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/compiler/api/__init__.py` & `pyrogeram-2.0.107/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/compiler/api/compiler.py` & `pyrogeram-2.0.107/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/compiler/docs/__init__.py` & `pyrogeram-2.0.107/compiler/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/compiler/docs/compiler.py` & `pyrogeram-2.0.107/compiler/docs/compiler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/compiler/errors/__init__.py` & `pyrogeram-2.0.107/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/compiler/errors/compiler.py` & `pyrogeram-2.0.107/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/compiler/errors/sort.py` & `pyrogeram-2.0.107/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/__init__.py` & `pyrogeram-2.0.107/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/client.py` & `pyrogeram-2.0.107/pyrogram/client.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/connection/__init__.py` & `pyrogeram-2.0.107/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/connection/connection.py` & `pyrogeram-2.0.107/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/connection/transport/__init__.py` & `pyrogeram-2.0.107/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/connection/transport/tcp/__init__.py` & `pyrogeram-2.0.107/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/connection/transport/tcp/tcp.py` & `pyrogeram-2.0.107/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/connection/transport/tcp/tcp_abridged.py` & `pyrogeram-2.0.107/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `pyrogeram-2.0.107/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/connection/transport/tcp/tcp_full.py` & `pyrogeram-2.0.107/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `pyrogeram-2.0.107/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `pyrogeram-2.0.107/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/crypto/__init__.py` & `pyrogeram-2.0.107/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/crypto/aes.py` & `pyrogeram-2.0.107/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/crypto/mtproto.py` & `pyrogeram-2.0.107/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/crypto/prime.py` & `pyrogeram-2.0.107/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/crypto/rsa.py` & `pyrogeram-2.0.107/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/dispatcher.py` & `pyrogeram-2.0.107/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/emoji.py` & `pyrogeram-2.0.107/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/__init__.py` & `pyrogeram-2.0.107/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/auto_name.py` & `pyrogeram-2.0.107/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/business_schedule.py` & `pyrogeram-2.0.107/pyrogram/enums/business_schedule.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/chat_action.py` & `pyrogeram-2.0.107/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/chat_event_action.py` & `pyrogeram-2.0.107/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/chat_member_status.py` & `pyrogeram-2.0.107/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/chat_members_filter.py` & `pyrogeram-2.0.107/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/chat_type.py` & `pyrogeram-2.0.107/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/listerner_types.py` & `pyrogeram-2.0.107/pyrogram/enums/listerner_types.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/message_entity_type.py` & `pyrogeram-2.0.107/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/message_media_type.py` & `pyrogeram-2.0.107/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/message_service_type.py` & `pyrogeram-2.0.107/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/messages_filter.py` & `pyrogeram-2.0.107/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/next_code_type.py` & `pyrogeram-2.0.107/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/parse_mode.py` & `pyrogeram-2.0.107/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/poll_type.py` & `pyrogeram-2.0.107/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/profile_color.py` & `pyrogeram-2.0.107/pyrogram/enums/profile_color.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/reaction_type.py` & `pyrogeram-2.0.107/pyrogram/enums/reaction_type.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/reply_color.py` & `pyrogeram-2.0.107/pyrogram/enums/reply_color.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/sent_code_type.py` & `pyrogeram-2.0.107/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/stories_privacy_rules.py` & `pyrogeram-2.0.107/pyrogram/enums/stories_privacy_rules.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/story_privacy.py` & `pyrogeram-2.0.107/pyrogram/enums/story_privacy.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/enums/user_status.py` & `pyrogeram-2.0.107/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/errors/__init__.py` & `pyrogeram-2.0.107/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/errors/rpc_error.py` & `pyrogeram-2.0.107/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/file_id.py` & `pyrogeram-2.0.107/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/filters.py` & `pyrogeram-2.0.107/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/__init__.py` & `pyrogeram-2.0.107/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/bot_business_connect_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/bot_business_connect_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/bot_business_message_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/bot_business_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/callback_query_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/chat_join_request_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/chat_member_updated_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/chosen_inline_result_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/conversation_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/conversation_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/deleted_bot_business_messages_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/deleted_bot_business_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/deleted_messages_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/disconnect_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/edited_bot_business_message_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/edited_bot_business_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/edited_message_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/inline_query_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/message_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/message_reaction_count_updated_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/message_reaction_count_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/message_reaction_updated_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/message_reaction_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/poll_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/raw_update_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/story_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/story_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/handlers/user_status_handler.py` & `pyrogeram-2.0.107/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/helpers/__init__.py` & `pyrogeram-2.0.107/pyrogram/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/helpers/helpers.py` & `pyrogeram-2.0.107/pyrogram/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/__init__.py` & `pyrogeram-2.0.107/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/advanced/__init__.py` & `pyrogeram-2.0.107/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/advanced/invoke.py` & `pyrogeram-2.0.107/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/advanced/resolve_peer.py` & `pyrogeram-2.0.107/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/advanced/save_file.py` & `pyrogeram-2.0.107/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/__init__.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/accept_terms_of_service.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/check_password.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/connect.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/disconnect.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/get_password_hint.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/initialize.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/log_out.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/recover_password.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/resend_code.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/send_code.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/send_recovery_code.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/sign_in.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/sign_in_bot.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/sign_up.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/auth/terminate.py` & `pyrogeram-2.0.107/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/__init__.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/answer_callback_query.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/answer_inline_query.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/answer_web_app_query.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/delete_bot_commands.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/get_bot_commands.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/get_bot_default_privileges.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/get_bot_info.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/get_bot_info.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/get_chat_menu_button.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/get_game_high_scores.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/get_inline_bot_results.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/request_callback_answer.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/send_game.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/send_inline_bot_result.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/set_bot_commands.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/set_bot_default_privileges.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/set_bot_info.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/set_bot_info.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/set_chat_menu_button.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/bots/set_game_score.py` & `pyrogeram-2.0.107/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/__init__.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/add_chat_members.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/archive_chats.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/ban_chat_member.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/close_forum_topic.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/close_general_topic.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/close_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/create_channel.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/create_forum_topic.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/create_group.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/create_supergroup.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/delete_channel.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/delete_chat_photo.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/delete_forum_topic.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/delete_supergroup.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/delete_user_history.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/edit_forum_topic.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/edit_general_topic.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/edit_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/get_chat.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/get_chat_event_log.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/get_chat_member.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/get_chat_members.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/get_chat_members_count.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/get_chat_online_count.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/get_dialogs.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/get_dialogs_count.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/get_forum_topics.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/get_forum_topics_by_id.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/get_forum_topics_by_id.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/get_nearby_chats.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/get_send_as_chats.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/hide_general_topic.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/hide_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/join_chat.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/leave_chat.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/mark_chat_unread.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/pin_chat_message.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/promote_chat_member.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/reopen_forum_topic.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/reopen_general_topic.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/reopen_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/restrict_chat_member.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/set_administrator_title.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/set_chat_description.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/set_chat_permissions.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/set_chat_photo.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/set_chat_protected_content.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/set_chat_title.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/set_chat_username.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/set_send_as_chat.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/set_slow_mode.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/unarchive_chats.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/unban_chat_member.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/unhide_general_topic.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/unhide_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/unpin_all_chat_messages.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/unpin_chat_message.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/chats/update_color.py` & `pyrogeram-2.0.107/pyrogram/methods/chats/update_color.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/contacts/__init__.py` & `pyrogeram-2.0.107/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/contacts/add_contact.py` & `pyrogeram-2.0.107/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/contacts/delete_contacts.py` & `pyrogeram-2.0.107/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/contacts/get_contacts.py` & `pyrogeram-2.0.107/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/contacts/get_contacts_count.py` & `pyrogeram-2.0.107/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/contacts/import_contacts.py` & `pyrogeram-2.0.107/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/__init__.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_bot_business_connect.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_bot_business_connect.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_bot_business_message.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_bot_business_message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_callback_query.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_chat_join_request.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_chat_member_updated.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_chosen_inline_result.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_deleted_bot_business_messages.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_deleted_bot_business_messages.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_deleted_messages.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_disconnect.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_edited_bot_business_message.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_edited_bot_business_message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_edited_message.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_inline_query.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_message.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_message_reaction_count_updated.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_message_reaction_updated.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_poll.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_raw_update.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_story.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_story.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/decorators/on_user_status.py` & `pyrogeram-2.0.107/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/__init__.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/approve_chat_join_request.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/create_chat_invite_link.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/decline_chat_join_request.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/export_chat_invite_link.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/get_chat_invite_link.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/get_chat_join_requests.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `pyrogeram-2.0.107/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/__init__.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/copy_media_group.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/copy_message.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/delete_messages.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/download_media.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/edit_inline_caption.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/edit_inline_media.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/edit_inline_reply_markup.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/edit_inline_text.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/edit_message_caption.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/edit_message_media.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/edit_message_reply_markup.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/edit_message_text.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/forward_messages.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/get_chat_history.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/get_chat_history_count.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/get_discussion_message.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/get_discussion_replies.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/get_discussion_replies_count.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/get_media_group.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/get_messages.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/inline_session.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/read_chat_history.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/retract_vote.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/search_global.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/search_global_count.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/search_messages.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/search_messages_count.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_animation.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_audio.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_cached_media.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_chat_action.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_contact.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_dice.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_document.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_location.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_media_group.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_message.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_photo.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_poll.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_reaction.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_sticker.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_venue.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_video.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_video_note.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_voice.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/send_web_page.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/send_web_page.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/stop_poll.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/stream_media.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/messages/vote_poll.py` & `pyrogeram-2.0.107/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/password/__init__.py` & `pyrogeram-2.0.107/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/password/change_cloud_password.py` & `pyrogeram-2.0.107/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/password/enable_cloud_password.py` & `pyrogeram-2.0.107/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/password/remove_cloud_password.py` & `pyrogeram-2.0.107/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/pyromod/__init__.py` & `pyrogeram-2.0.107/pyrogram/methods/pyromod/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/pyromod/ask.py` & `pyrogeram-2.0.107/pyrogram/methods/pyromod/ask.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/pyromod/get_listener_matching_with_data.py` & `pyrogeram-2.0.107/pyrogram/methods/pyromod/get_listener_matching_with_data.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/pyromod/get_listener_matching_with_identifier_pattern.py` & `pyrogeram-2.0.107/pyrogram/methods/pyromod/get_listener_matching_with_identifier_pattern.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/pyromod/get_many_listeners_matching_with_data.py` & `pyrogeram-2.0.107/pyrogram/methods/pyromod/get_many_listeners_matching_with_data.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/pyromod/get_many_listeners_matching_with_identifier_pattern.py` & `pyrogeram-2.0.107/pyrogram/methods/pyromod/get_many_listeners_matching_with_identifier_pattern.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/pyromod/listen.py` & `pyrogeram-2.0.107/pyrogram/methods/pyromod/listen.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/pyromod/register_next_step_handler.py` & `pyrogeram-2.0.107/pyrogram/methods/pyromod/register_next_step_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/pyromod/remove_listerner.py` & `pyrogeram-2.0.107/pyrogram/methods/pyromod/remove_listerner.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/pyromod/stop_listener.py` & `pyrogeram-2.0.107/pyrogram/methods/pyromod/stop_listener.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/pyromod/stop_listening.py` & `pyrogeram-2.0.107/pyrogram/methods/pyromod/stop_listening.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/pyromod/wait_for_callback_query.py` & `pyrogeram-2.0.107/pyrogram/methods/pyromod/wait_for_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/pyromod/wait_for_message.py` & `pyrogeram-2.0.107/pyrogram/methods/pyromod/wait_for_message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/stickers/__init__.py` & `pyrogeram-2.0.107/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/stickers/add_sticker_to_set.py` & `pyrogeram-2.0.107/pyrogram/methods/stickers/add_sticker_to_set.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/stickers/create_sticker_set.py` & `pyrogeram-2.0.107/pyrogram/methods/stickers/create_sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/stickers/get_sticker_set.py` & `pyrogeram-2.0.107/pyrogram/methods/stickers/get_sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/__init__.py` & `pyrogeram-2.0.107/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/block_user.py` & `pyrogeram-2.0.107/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/delete_profile_photos.py` & `pyrogeram-2.0.107/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/delete_stories.py` & `pyrogeram-2.0.107/pyrogram/methods/users/delete_stories.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/edit_story.py` & `pyrogeram-2.0.107/pyrogram/methods/users/edit_story.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/export_story_link.py` & `pyrogeram-2.0.107/pyrogram/methods/users/export_story_link.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/forward_story.py` & `pyrogeram-2.0.107/pyrogram/methods/users/forward_story.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/get_all_stories.py` & `pyrogeram-2.0.107/pyrogram/methods/users/get_all_stories.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/get_chat_photos.py` & `pyrogeram-2.0.107/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/get_chat_photos_count.py` & `pyrogeram-2.0.107/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/get_common_chats.py` & `pyrogeram-2.0.107/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/get_default_emoji_statuses.py` & `pyrogeram-2.0.107/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/get_me.py` & `pyrogeram-2.0.107/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/get_peer_stories.py` & `pyrogeram-2.0.107/pyrogram/methods/users/get_peer_stories.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/get_stories.py` & `pyrogeram-2.0.107/pyrogram/methods/users/get_stories.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/get_stories_history.py` & `pyrogeram-2.0.107/pyrogram/methods/users/get_stories_history.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/get_users.py` & `pyrogeram-2.0.107/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/send_story.py` & `pyrogeram-2.0.107/pyrogram/methods/users/send_story.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/set_emoji_status.py` & `pyrogeram-2.0.107/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/set_profile_photo.py` & `pyrogeram-2.0.107/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/set_username.py` & `pyrogeram-2.0.107/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/unblock_user.py` & `pyrogeram-2.0.107/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/update_birthday.py` & `pyrogeram-2.0.107/pyrogram/methods/users/update_birthday.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/update_personal_chat.py` & `pyrogeram-2.0.107/pyrogram/methods/users/update_personal_chat.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/users/update_profile.py` & `pyrogeram-2.0.107/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/utilities/__init__.py` & `pyrogeram-2.0.107/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/utilities/add_handler.py` & `pyrogeram-2.0.107/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/utilities/compose.py` & `pyrogeram-2.0.107/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/utilities/export_session_string.py` & `pyrogeram-2.0.107/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/utilities/idle.py` & `pyrogeram-2.0.107/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/utilities/remove_handler.py` & `pyrogeram-2.0.107/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/utilities/restart.py` & `pyrogeram-2.0.107/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/utilities/run.py` & `pyrogeram-2.0.107/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/utilities/run_sync.py` & `pyrogeram-2.0.107/pyrogram/methods/utilities/run_sync.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/utilities/start.py` & `pyrogeram-2.0.107/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/utilities/stop.py` & `pyrogeram-2.0.107/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/methods/utilities/stop_transmission.py` & `pyrogeram-2.0.107/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/mime_types.py` & `pyrogeram-2.0.107/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/nav/__init__.py` & `pyrogeram-2.0.107/pyrogram/nav/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/nav/pagination.py` & `pyrogeram-2.0.107/pyrogram/nav/pagination.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/parser/__init__.py` & `pyrogeram-2.0.107/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/parser/html.py` & `pyrogeram-2.0.107/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/parser/markdown.py` & `pyrogeram-2.0.107/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/parser/parser.py` & `pyrogeram-2.0.107/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/parser/utils.py` & `pyrogeram-2.0.107/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/__init__.py` & `pyrogeram-2.0.107/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/__init__.py` & `pyrogeram-2.0.107/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/future_salt.py` & `pyrogeram-2.0.107/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/future_salts.py` & `pyrogeram-2.0.107/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/gzip_packed.py` & `pyrogeram-2.0.107/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/list.py` & `pyrogeram-2.0.107/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/message.py` & `pyrogeram-2.0.107/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/msg_container.py` & `pyrogeram-2.0.107/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/primitives/__init__.py` & `pyrogeram-2.0.107/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/primitives/bool.py` & `pyrogeram-2.0.107/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/primitives/bytes.py` & `pyrogeram-2.0.107/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/primitives/double.py` & `pyrogeram-2.0.107/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/primitives/int.py` & `pyrogeram-2.0.107/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/primitives/string.py` & `pyrogeram-2.0.107/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/primitives/vector.py` & `pyrogeram-2.0.107/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/raw/core/tl_object.py` & `pyrogeram-2.0.107/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/session/__init__.py` & `pyrogeram-2.0.107/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/session/auth.py` & `pyrogeram-2.0.107/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/session/internals/__init__.py` & `pyrogeram-2.0.107/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/session/internals/data_center.py` & `pyrogeram-2.0.107/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/session/internals/msg_factory.py` & `pyrogeram-2.0.107/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/session/internals/msg_id.py` & `pyrogeram-2.0.107/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/session/internals/seq_no.py` & `pyrogeram-2.0.107/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/session/session.py` & `pyrogeram-2.0.107/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/storage/__init__.py` & `pyrogeram-2.0.107/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/storage/dummy_client.py` & `pyrogeram-2.0.107/pyrogram/storage/dummy_client.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/storage/file_storage.py` & `pyrogeram-2.0.107/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/storage/memory_storage.py` & `pyrogeram-2.0.107/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/storage/mongo_storage.py` & `pyrogeram-2.0.107/pyrogram/storage/mongo_storage.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/storage/sqlite_storage.py` & `pyrogeram-2.0.107/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/storage/storage.py` & `pyrogeram-2.0.107/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/sync.py` & `pyrogeram-2.0.107/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/__init__.py` & `pyrogeram-2.0.107/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/authorization/__init__.py` & `pyrogeram-2.0.107/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/authorization/sent_code.py` & `pyrogeram-2.0.107/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/authorization/terms_of_service.py` & `pyrogeram-2.0.107/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/__init__.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_business_connection.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_business_connection.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/bot_info.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/bot_info.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/callback_game.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/callback_query.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/force_reply.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/game_high_score.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/login_url.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/menu_button.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/request_peer_type_channel.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/request_peer_type_channel.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/request_peer_type_chat.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/request_peer_type_chat.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/request_peer_type_user.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/request_peer_type_user.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/bots_and_keyboards/web_app_info.py` & `pyrogeram-2.0.107/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/__init__.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/chosen_inline_result.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_animation.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_article.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_audio.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_contact.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_document.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_location.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_photo.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_venue.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_video.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/inline_mode/inline_query_result_voice.py` & `pyrogeram-2.0.107/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_media/__init__.py` & `pyrogeram-2.0.107/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_media/input_media.py` & `pyrogeram-2.0.107/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_media/input_media_animation.py` & `pyrogeram-2.0.107/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_media/input_media_area.py` & `pyrogeram-2.0.107/pyrogram/types/input_media/input_media_area.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_media/input_media_area_channel_post.py` & `pyrogeram-2.0.107/pyrogram/types/input_media/input_media_area_channel_post.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_media/input_media_audio.py` & `pyrogeram-2.0.107/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_media/input_media_document.py` & `pyrogeram-2.0.107/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_media/input_media_photo.py` & `pyrogeram-2.0.107/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_media/input_media_video.py` & `pyrogeram-2.0.107/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_media/input_phone_contact.py` & `pyrogeram-2.0.107/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_message_content/__init__.py` & `pyrogeram-2.0.107/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_message_content/input_message_content.py` & `pyrogeram-2.0.107/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_message_content/input_reply_to_message.py` & `pyrogeram-2.0.107/pyrogram/types/input_message_content/input_reply_to_message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_message_content/input_reply_to_story.py` & `pyrogeram-2.0.107/pyrogram/types/input_message_content/input_reply_to_story.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/input_message_content/input_text_message_content.py` & `pyrogeram-2.0.107/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/list.py` & `pyrogeram-2.0.107/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/__init__.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/animation.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/audio.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/contact.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/dice.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/document.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/exported_story_link.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/exported_story_link.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/game.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/giveaway.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/giveaway.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/giveaway_launched.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/giveaway_launched.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/giveaway_result.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/giveaway_result.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/location.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/media_area.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/media_area.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/media_area_channel_post.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/media_area_channel_post.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/media_area_coordinates.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/media_area_coordinates.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/message.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/message_entity.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/message_reaction_count_updated.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/message_reaction_updated.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/message_reactions.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/message_story.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/message_story.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/photo.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/poll.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/poll_option.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/reaction.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/reaction_count.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/reaction_count.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/reaction_type.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/reaction_type.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/sticker.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/stickerset.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/stickerset.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/stories_privacy_rules.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/stories_privacy_rules.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/story.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/story.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/story_deleted.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/story_deleted.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/story_forward_header.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/story_forward_header.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/story_skipped.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/story_skipped.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/story_views.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/story_views.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/thumbnail.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/venue.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/video.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/video_note.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/voice.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/web_app_data.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/web_page.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/web_page_empty.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/web_page_empty.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/messages_and_media/web_page_preview.py` & `pyrogeram-2.0.107/pyrogram/types/messages_and_media/web_page_preview.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/object.py` & `pyrogeram-2.0.107/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/pyromod/__init__.py` & `pyrogeram-2.0.107/pyrogram/types/pyromod/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/pyromod/identifier.py` & `pyrogeram-2.0.107/pyrogram/types/pyromod/identifier.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/pyromod/listener.py` & `pyrogeram-2.0.107/pyrogram/types/pyromod/listener.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/update.py` & `pyrogeram-2.0.107/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/__init__.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/birthday.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/birthday.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/business_info.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/business_info.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/business_message.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/business_message.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/business_recipients.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/business_recipients.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/business_weekly_open.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/business_weekly_open.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/business_working_hours.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/business_working_hours.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_color.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_color.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_event.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_event_filter.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_invite_link.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_join_request.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_joined_by_request.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_joined_by_request.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_joiner.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_member.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_member_updated.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_permissions.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_photo.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_preview.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_privileges.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/chat_reactions.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/dialog.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/emoji_status.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/forum_topic.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/forum_topic_closed.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/forum_topic_created.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/forum_topic_edited.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/forum_topic_reopened.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/general_forum_topic_hidden.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/invite_link_importer.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/peer_channel.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/peer_channel.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/peer_user.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/peer_user.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/restriction.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/user.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/username.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/video_chat_ended.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/video_chat_members_invited.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/types/user_and_chats/video_chat_started.py` & `pyrogeram-2.0.107/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/pyrogram/utils.py` & `pyrogeram-2.0.107/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `pyrogeram-2.0.106/setup.py` & `pyrogeram-2.0.107/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Membaca isi dari requirements.txt
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name="pyrogeram",
-    version="2.0.106",
+    version="2.0.107",
     packages=find_packages(),
     description='Seratus Persen Clone Pyrofork',
     author="rizaldevs",
     author_email="rizaldaitona@gmail.com",
     url="https://t.me/pyrogram",
     classifiers=[
         'Programming Language :: Python :: 3.10',
```

