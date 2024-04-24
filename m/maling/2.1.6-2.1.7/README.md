# Comparing `tmp/maling-2.1.6.tar.gz` & `tmp/maling-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maling-2.1.6.tar", last modified: Mon Apr 15 01:57:33 2024, max compression
+gzip compressed data, was "maling-2.1.7.tar", last modified: Tue Apr 23 16:40:17 2024, max compression
```

## Comparing `maling-2.1.6.tar` & `maling-2.1.7.tar`

### file list

```diff
@@ -1,498 +1,498 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.687065 maling-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-15 01:56:41.000000 maling-2.1.6/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-15 01:56:41.000000 maling-2.1.6/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-15 01:56:41.000000 maling-2.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-15 01:56:41.000000 maling-2.1.6/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-15 01:57:33.687065 maling-2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 01:56:41.000000 maling-2.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.587067 maling-2.1.6/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.587067 maling-2.1.6/compiler/api/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22330 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/api/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.587067 maling-2.1.6/compiler/api/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/api/source/auth_key.tl
--rw-r--r--   0 runner    (1001) docker     (127)   168867 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/api/source/main_api.tl
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.587067 maling-2.1.6/compiler/api/template/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/api/template/combinator.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/api/template/type.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.587067 maling-2.1.6/compiler/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/errors/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/errors/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.591067 maling-2.1.6/compiler/errors/source/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    22642 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.591067 maling-2.1.6/compiler/errors/template/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/errors/template/class.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 01:56:41.000000 maling-2.1.6/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.687065 maling-2.1.6/maling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-15 01:57:33.000000 maling-2.1.6/maling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17332 2024-04-15 01:57:33.000000 maling-2.1.6/maling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 01:57:33.000000 maling-2.1.6/maling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 01:57:23.000000 maling-2.1.6/maling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-15 01:57:33.000000 maling-2.1.6/maling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-15 01:57:33.000000 maling-2.1.6/maling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-15 01:56:41.000000 maling-2.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 01:57:33.687065 maling-2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-15 01:56:41.000000 maling-2.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.595067 maling-2.1.6/team/
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-15 01:56:41.000000 maling-2.1.6/team/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41896 2024-04-15 01:56:41.000000 maling-2.1.6/team/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.595067 maling-2.1.6/team/connection/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-15 01:56:41.000000 maling-2.1.6/team/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-15 01:56:41.000000 maling-2.1.6/team/connection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.595067 maling-2.1.6/team/connection/transport/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-15 01:56:41.000000 maling-2.1.6/team/connection/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.595067 maling-2.1.6/team/connection/transport/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-15 01:56:41.000000 maling-2.1.6/team/connection/transport/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-15 01:56:41.000000 maling-2.1.6/team/connection/transport/tcp/tcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-15 01:56:41.000000 maling-2.1.6/team/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-15 01:56:41.000000 maling-2.1.6/team/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-15 01:56:41.000000 maling-2.1.6/team/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-15 01:56:41.000000 maling-2.1.6/team/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-15 01:56:41.000000 maling-2.1.6/team/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.595067 maling-2.1.6/team/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-15 01:56:41.000000 maling-2.1.6/team/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-15 01:56:41.000000 maling-2.1.6/team/crypto/aes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-15 01:56:41.000000 maling-2.1.6/team/crypto/mtproto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-15 01:56:41.000000 maling-2.1.6/team/crypto/prime.py
--rw-r--r--   0 runner    (1001) docker     (127)    13437 2024-04-15 01:56:41.000000 maling-2.1.6/team/crypto/rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     9990 2024-04-15 01:56:41.000000 maling-2.1.6/team/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)   208021 2024-04-15 01:56:41.000000 maling-2.1.6/team/emoji.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.599067 maling-2.1.6/team/enums/
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/auto_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/chat_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/chat_event_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/chat_member_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/chat_members_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/chat_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/message_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/message_media_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/message_service_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/messages_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/next_code_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/parse_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/poll_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/sent_code_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-15 01:56:41.000000 maling-2.1.6/team/enums/user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.599067 maling-2.1.6/team/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-15 01:56:41.000000 maling-2.1.6/team/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-15 01:56:41.000000 maling-2.1.6/team/errors/rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    15150 2024-04-15 01:56:41.000000 maling-2.1.6/team/file_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    24704 2024-04-15 01:56:41.000000 maling-2.1.6/team/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.603067 maling-2.1.6/team/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-15 01:56:41.000000 maling-2.1.6/team/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-15 01:56:41.000000 maling-2.1.6/team/handlers/callback_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-15 01:56:41.000000 maling-2.1.6/team/handlers/chat_join_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-15 01:56:41.000000 maling-2.1.6/team/handlers/chat_member_updated_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-15 01:56:41.000000 maling-2.1.6/team/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-15 01:56:41.000000 maling-2.1.6/team/handlers/deleted_messages_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-15 01:56:41.000000 maling-2.1.6/team/handlers/disconnect_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-15 01:56:41.000000 maling-2.1.6/team/handlers/edited_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-15 01:56:41.000000 maling-2.1.6/team/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-15 01:56:41.000000 maling-2.1.6/team/handlers/inline_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-15 01:56:41.000000 maling-2.1.6/team/handlers/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 01:56:41.000000 maling-2.1.6/team/handlers/poll_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-15 01:56:41.000000 maling-2.1.6/team/handlers/raw_update_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-15 01:56:41.000000 maling-2.1.6/team/handlers/user_status_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.603067 maling-2.1.6/team/methods/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.603067 maling-2.1.6/team/methods/advanced/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/advanced/invoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/advanced/resolve_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/advanced/save_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.607066 maling-2.1.6/team/methods/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/check_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/get_password_hint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/log_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/recover_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/resend_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/send_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/send_recovery_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/sign_in.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/sign_in_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/auth/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.611066 maling-2.1.6/team/methods/bots/
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/answer_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/answer_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/answer_web_app_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/delete_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/get_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/get_game_high_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/request_callback_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/send_game.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/set_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/bots/set_game_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.615066 maling-2.1.6/team/methods/chats/
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/add_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/archive_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/ban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/create_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/create_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/create_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/delete_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/delete_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/delete_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/delete_user_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/get_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/get_chat_event_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/get_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/get_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/get_chat_members_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/get_chat_online_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/get_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/get_dialogs_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/get_nearby_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/get_send_as_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/join_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/leave_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/mark_chat_unread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/pin_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/promote_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/restrict_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/set_administrator_title.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/set_chat_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/set_chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/set_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/set_chat_title.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/set_chat_username.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/set_send_as_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/set_slow_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/unarchive_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/unban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.619066 maling-2.1.6/team/methods/contacts/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/contacts/add_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/contacts/delete_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/contacts/get_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/contacts/get_contacts_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/contacts/import_contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.619066 maling-2.1.6/team/methods/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/decorators/on_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/decorators/on_disconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/decorators/on_edited_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/decorators/on_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/decorators/on_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/decorators/on_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/decorators/on_raw_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/decorators/on_user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.627066 maling-2.1.6/team/methods/invite_links/
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.643066 maling-2.1.6/team/methods/messages/
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/copy_media_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/copy_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/delete_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/download_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/edit_inline_caption.py
--rw-r--r--   0 runner    (1001) docker     (127)    10335 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/edit_inline_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/edit_inline_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/edit_message_caption.py
--rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/edit_message_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/edit_message_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/forward_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/get_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/get_chat_history_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/get_discussion_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/get_discussion_replies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/get_media_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/get_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/inline_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/read_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/retract_vote.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/search_global.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/search_global_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/search_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/search_messages_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_animation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11050 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_cached_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_chat_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_location.py
--rw-r--r--   0 runner    (1001) docker     (127)    19858 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_media_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_sticker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_venue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_video_note.py
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/send_voice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/stop_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/stream_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/messages/vote_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.643066 maling-2.1.6/team/methods/password/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/password/change_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/password/enable_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.643066 maling-2.1.6/team/methods/users/
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/users/block_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/users/delete_profile_photos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/users/get_chat_photos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/users/get_chat_photos_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/users/get_common_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/users/get_me.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/users/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/users/set_emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/users/set_profile_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/users/set_username.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/users/unblock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/users/update_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.647066 maling-2.1.6/team/methods/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/utilities/add_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/utilities/compose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/utilities/export_session_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/utilities/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/utilities/remove_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/utilities/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/utilities/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/utilities/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/utilities/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-15 01:56:41.000000 maling-2.1.6/team/methods/utilities/stop_transmission.py
--rw-r--r--   0 runner    (1001) docker     (127)    61915 2024-04-15 01:56:41.000000 maling-2.1.6/team/mime_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.647066 maling-2.1.6/team/nandev/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-15 01:56:41.000000 maling-2.1.6/team/nandev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-15 01:56:41.000000 maling-2.1.6/team/nandev/autopilot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-15 01:56:41.000000 maling-2.1.6/team/nandev/class_emoji.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-15 01:56:41.000000 maling-2.1.6/team/nandev/class_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-15 01:56:41.000000 maling-2.1.6/team/nandev/class_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-15 01:56:41.000000 maling-2.1.6/team/nandev/class_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-15 01:56:41.000000 maling-2.1.6/team/nandev/class_mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-15 01:56:41.000000 maling-2.1.6/team/nandev/class_pytgc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16833 2024-04-15 01:56:41.000000 maling-2.1.6/team/nandev/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    26991 2024-04-15 01:56:41.000000 maling-2.1.6/team/nandev/new_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.647066 maling-2.1.6/team/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-15 01:56:41.000000 maling-2.1.6/team/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8660 2024-04-15 01:56:41.000000 maling-2.1.6/team/parser/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-15 01:56:41.000000 maling-2.1.6/team/parser/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-15 01:56:41.000000 maling-2.1.6/team/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-15 01:56:41.000000 maling-2.1.6/team/parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:56:41.000000 maling-2.1.6/team/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.647066 maling-2.1.6/team/raw/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-15 01:56:41.000000 maling-2.1.6/team/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.651066 maling-2.1.6/team/raw/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-15 01:56:41.000000 maling-2.1.6/team/raw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-15 01:56:41.000000 maling-2.1.6/team/raw/core/future_salt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-15 01:56:41.000000 maling-2.1.6/team/raw/core/future_salts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-15 01:56:41.000000 maling-2.1.6/team/raw/core/gzip_packed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-15 01:56:41.000000 maling-2.1.6/team/raw/core/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-15 01:56:41.000000 maling-2.1.6/team/raw/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-15 01:56:41.000000 maling-2.1.6/team/raw/core/msg_container.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.651066 maling-2.1.6/team/raw/core/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-15 01:56:41.000000 maling-2.1.6/team/raw/core/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-15 01:56:41.000000 maling-2.1.6/team/raw/core/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-15 01:56:42.000000 maling-2.1.6/team/raw/core/primitives/bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-15 01:56:42.000000 maling-2.1.6/team/raw/core/primitives/double.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-15 01:56:42.000000 maling-2.1.6/team/raw/core/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-15 01:56:42.000000 maling-2.1.6/team/raw/core/primitives/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-15 01:56:42.000000 maling-2.1.6/team/raw/core/primitives/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-15 01:56:42.000000 maling-2.1.6/team/raw/core/tl_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.651066 maling-2.1.6/team/session/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-15 01:56:42.000000 maling-2.1.6/team/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11418 2024-04-15 01:56:42.000000 maling-2.1.6/team/session/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.655066 maling-2.1.6/team/session/internals/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-15 01:56:42.000000 maling-2.1.6/team/session/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-15 01:56:42.000000 maling-2.1.6/team/session/internals/data_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-15 01:56:42.000000 maling-2.1.6/team/session/internals/msg_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-15 01:56:42.000000 maling-2.1.6/team/session/internals/msg_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-15 01:56:42.000000 maling-2.1.6/team/session/internals/seq_no.py
--rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-04-15 01:56:42.000000 maling-2.1.6/team/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.655066 maling-2.1.6/team/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-15 01:56:42.000000 maling-2.1.6/team/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-15 01:56:42.000000 maling-2.1.6/team/storage/file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-15 01:56:42.000000 maling-2.1.6/team/storage/memory_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-15 01:56:42.000000 maling-2.1.6/team/storage/sqlite_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-15 01:56:42.000000 maling-2.1.6/team/storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-15 01:56:42.000000 maling-2.1.6/team/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.659066 maling-2.1.6/team/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.659066 maling-2.1.6/team/types/authorization/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/authorization/sent_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/authorization/terms_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.667066 maling-2.1.6/team/types/bots_and_keyboards/
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.675066 maling-2.1.6/team/types/inline_mode/
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.675066 maling-2.1.6/team/types/input_media/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/input_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/input_media/input_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/input_media/input_media_animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/input_media/input_media_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/input_media/input_media_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/input_media/input_media_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/input_media/input_media_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.675066 maling-2.1.6/team/types/input_message_content/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/input_message_content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/input_message_content/input_message_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.679066 maling-2.1.6/team/types/messages_and_media/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/game.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/location.py
--rw-r--r--   0 runner    (1001) docker     (127)   143655 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/message_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/message_reactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/poll_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/sticker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/venue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/video_note.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/voice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/web_app_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/messages_and_media/web_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.687065 maling-2.1.6/team/types/user_and_chats/
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32339 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    19667 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/chat_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/chat_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/chat_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/restriction.py
--rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-15 01:56:42.000000 maling-2.1.6/team/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-04-15 01:56:42.000000 maling-2.1.6/team/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.687065 maling-2.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-15 01:56:42.000000 maling-2.1.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.687065 maling-2.1.6/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-15 01:56:42.000000 maling-2.1.6/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-15 01:56:42.000000 maling-2.1.6/tests/filters/test_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:57:33.687065 maling-2.1.6/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-15 01:56:42.000000 maling-2.1.6/tests/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-15 01:56:42.000000 maling-2.1.6/tests/parser/test_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-04-15 01:56:42.000000 maling-2.1.6/tests/test_file_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.061796 maling-2.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-23 16:39:29.000000 maling-2.1.7/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-23 16:39:29.000000 maling-2.1.7/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 16:39:29.000000 maling-2.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-23 16:39:29.000000 maling-2.1.7/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-23 16:40:17.061796 maling-2.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 16:39:29.000000 maling-2.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.977795 maling-2.1.7/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.977795 maling-2.1.7/compiler/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22330 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/api/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.977795 maling-2.1.7/compiler/api/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/api/source/auth_key.tl
+-rw-r--r--   0 runner    (1001) docker     (127)   168867 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/api/source/main_api.tl
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.977795 maling-2.1.7/compiler/api/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/api/template/combinator.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/api/template/type.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.977795 maling-2.1.7/compiler/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/errors/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/errors/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.977795 maling-2.1.7/compiler/errors/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    22642 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.981795 maling-2.1.7/compiler/errors/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/errors/template/class.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 16:39:29.000000 maling-2.1.7/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.061796 maling-2.1.7/maling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-23 16:40:16.000000 maling-2.1.7/maling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17332 2024-04-23 16:40:16.000000 maling-2.1.7/maling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:40:16.000000 maling-2.1.7/maling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:40:06.000000 maling-2.1.7/maling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-23 16:40:16.000000 maling-2.1.7/maling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 16:40:16.000000 maling-2.1.7/maling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-23 16:39:29.000000 maling-2.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:40:17.061796 maling-2.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-23 16:39:29.000000 maling-2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.981795 maling-2.1.7/team/
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-23 16:39:29.000000 maling-2.1.7/team/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41896 2024-04-23 16:39:29.000000 maling-2.1.7/team/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.985796 maling-2.1.7/team/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-23 16:39:29.000000 maling-2.1.7/team/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-23 16:39:29.000000 maling-2.1.7/team/connection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.985796 maling-2.1.7/team/connection/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-23 16:39:29.000000 maling-2.1.7/team/connection/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.985796 maling-2.1.7/team/connection/transport/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-23 16:39:29.000000 maling-2.1.7/team/connection/transport/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-23 16:39:29.000000 maling-2.1.7/team/connection/transport/tcp/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-23 16:39:29.000000 maling-2.1.7/team/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-23 16:39:29.000000 maling-2.1.7/team/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-23 16:39:29.000000 maling-2.1.7/team/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-23 16:39:29.000000 maling-2.1.7/team/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-23 16:39:29.000000 maling-2.1.7/team/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.985796 maling-2.1.7/team/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 16:39:29.000000 maling-2.1.7/team/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-23 16:39:29.000000 maling-2.1.7/team/crypto/aes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-23 16:39:29.000000 maling-2.1.7/team/crypto/mtproto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-23 16:39:29.000000 maling-2.1.7/team/crypto/prime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13437 2024-04-23 16:39:29.000000 maling-2.1.7/team/crypto/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9990 2024-04-23 16:39:29.000000 maling-2.1.7/team/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)   208021 2024-04-23 16:39:29.000000 maling-2.1.7/team/emoji.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.989796 maling-2.1.7/team/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/auto_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/chat_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/chat_member_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/chat_members_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/chat_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/message_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/message_media_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/message_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/messages_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/next_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/parse_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/sent_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-23 16:39:29.000000 maling-2.1.7/team/enums/user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.989796 maling-2.1.7/team/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-23 16:39:29.000000 maling-2.1.7/team/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-23 16:39:29.000000 maling-2.1.7/team/errors/rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15150 2024-04-23 16:39:29.000000 maling-2.1.7/team/file_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24704 2024-04-23 16:39:29.000000 maling-2.1.7/team/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.993795 maling-2.1.7/team/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-23 16:39:29.000000 maling-2.1.7/team/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-23 16:39:29.000000 maling-2.1.7/team/handlers/callback_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-23 16:39:29.000000 maling-2.1.7/team/handlers/chat_join_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-23 16:39:29.000000 maling-2.1.7/team/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-23 16:39:29.000000 maling-2.1.7/team/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-23 16:39:29.000000 maling-2.1.7/team/handlers/deleted_messages_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-23 16:39:29.000000 maling-2.1.7/team/handlers/disconnect_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-23 16:39:29.000000 maling-2.1.7/team/handlers/edited_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-23 16:39:29.000000 maling-2.1.7/team/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-23 16:39:29.000000 maling-2.1.7/team/handlers/inline_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-23 16:39:29.000000 maling-2.1.7/team/handlers/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-23 16:39:29.000000 maling-2.1.7/team/handlers/poll_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-23 16:39:29.000000 maling-2.1.7/team/handlers/raw_update_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-23 16:39:29.000000 maling-2.1.7/team/handlers/user_status_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.993795 maling-2.1.7/team/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.993795 maling-2.1.7/team/methods/advanced/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/advanced/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/advanced/resolve_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/advanced/save_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:16.997795 maling-2.1.7/team/methods/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/check_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/get_password_hint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/log_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/recover_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/resend_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/send_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/send_recovery_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/sign_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/sign_in_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/auth/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.001796 maling-2.1.7/team/methods/bots/
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/answer_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/answer_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/get_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/request_callback_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/send_game.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/set_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/bots/set_game_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.005796 maling-2.1.7/team/methods/chats/
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/add_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/archive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/ban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/create_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/create_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/delete_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/delete_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/delete_user_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/get_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/get_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/get_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/join_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/leave_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/pin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/promote_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/set_administrator_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/set_chat_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/set_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/set_chat_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/set_chat_username.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/set_slow_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/unarchive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/unban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.009796 maling-2.1.7/team/methods/contacts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/contacts/add_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/contacts/delete_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/contacts/get_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/contacts/import_contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.009796 maling-2.1.7/team/methods/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/decorators/on_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/decorators/on_disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/decorators/on_edited_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/decorators/on_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/decorators/on_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/decorators/on_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/decorators/on_raw_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/decorators/on_user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.013795 maling-2.1.7/team/methods/invite_links/
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.025796 maling-2.1.7/team/methods/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/copy_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/copy_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/delete_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/download_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10335 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/edit_inline_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/edit_inline_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/edit_message_caption.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/edit_message_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/edit_message_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/forward_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/get_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/get_discussion_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/get_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/inline_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/read_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/retract_vote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/search_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/search_global_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/search_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/search_messages_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11050 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_cached_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19858 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_venue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_video_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/send_voice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/stop_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/stream_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/messages/vote_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.025796 maling-2.1.7/team/methods/password/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/password/change_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/password/enable_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.025796 maling-2.1.7/team/methods/users/
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/users/block_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/users/delete_profile_photos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/users/get_chat_photos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/users/get_common_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/users/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/users/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/users/set_emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/users/set_profile_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/users/set_username.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/users/unblock_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/users/update_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.029796 maling-2.1.7/team/methods/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/utilities/add_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/utilities/compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/utilities/export_session_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/utilities/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/utilities/remove_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/utilities/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/utilities/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/utilities/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/utilities/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-23 16:39:29.000000 maling-2.1.7/team/methods/utilities/stop_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61915 2024-04-23 16:39:29.000000 maling-2.1.7/team/mime_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.029796 maling-2.1.7/team/nandev/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-23 16:39:29.000000 maling-2.1.7/team/nandev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-23 16:39:29.000000 maling-2.1.7/team/nandev/autopilot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-23 16:39:29.000000 maling-2.1.7/team/nandev/class_emoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-23 16:39:29.000000 maling-2.1.7/team/nandev/class_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-23 16:39:29.000000 maling-2.1.7/team/nandev/class_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-23 16:39:29.000000 maling-2.1.7/team/nandev/class_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-23 16:39:29.000000 maling-2.1.7/team/nandev/class_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-23 16:39:29.000000 maling-2.1.7/team/nandev/class_pytgc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17762 2024-04-23 16:39:29.000000 maling-2.1.7/team/nandev/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26991 2024-04-23 16:39:29.000000 maling-2.1.7/team/nandev/new_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.033796 maling-2.1.7/team/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-23 16:39:29.000000 maling-2.1.7/team/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8660 2024-04-23 16:39:29.000000 maling-2.1.7/team/parser/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-23 16:39:29.000000 maling-2.1.7/team/parser/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-23 16:39:29.000000 maling-2.1.7/team/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-23 16:39:29.000000 maling-2.1.7/team/parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:39:29.000000 maling-2.1.7/team/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.033796 maling-2.1.7/team/raw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.033796 maling-2.1.7/team/raw/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/future_salt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/future_salts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/gzip_packed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/msg_container.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.033796 maling-2.1.7/team/raw/core/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/primitives/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/primitives/double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/primitives/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/primitives/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-23 16:39:29.000000 maling-2.1.7/team/raw/core/tl_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.037796 maling-2.1.7/team/session/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-23 16:39:29.000000 maling-2.1.7/team/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11418 2024-04-23 16:39:29.000000 maling-2.1.7/team/session/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.037796 maling-2.1.7/team/session/internals/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-23 16:39:29.000000 maling-2.1.7/team/session/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-23 16:39:29.000000 maling-2.1.7/team/session/internals/data_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-23 16:39:29.000000 maling-2.1.7/team/session/internals/msg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-23 16:39:29.000000 maling-2.1.7/team/session/internals/msg_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-23 16:39:29.000000 maling-2.1.7/team/session/internals/seq_no.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-04-23 16:39:29.000000 maling-2.1.7/team/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.037796 maling-2.1.7/team/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-23 16:39:29.000000 maling-2.1.7/team/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-23 16:39:29.000000 maling-2.1.7/team/storage/file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-23 16:39:29.000000 maling-2.1.7/team/storage/memory_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-23 16:39:29.000000 maling-2.1.7/team/storage/sqlite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-23 16:39:29.000000 maling-2.1.7/team/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-23 16:39:29.000000 maling-2.1.7/team/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.037796 maling-2.1.7/team/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.037796 maling-2.1.7/team/types/authorization/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/authorization/sent_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/authorization/terms_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.041796 maling-2.1.7/team/types/bots_and_keyboards/
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.045796 maling-2.1.7/team/types/inline_mode/
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.049796 maling-2.1.7/team/types/input_media/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/input_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/input_media/input_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/input_media/input_media_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/input_media/input_media_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/input_media/input_media_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/input_media/input_media_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/input_media/input_media_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.049796 maling-2.1.7/team/types/input_message_content/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/input_message_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/input_message_content/input_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.053796 maling-2.1.7/team/types/messages_and_media/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/game.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)   143655 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/message_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/poll_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/venue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/video_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/voice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/messages_and_media/web_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.057796 maling-2.1.7/team/types/user_and_chats/
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32339 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19667 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/chat_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/restriction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-23 16:39:29.000000 maling-2.1.7/team/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-04-23 16:39:29.000000 maling-2.1.7/team/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.061796 maling-2.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 16:39:29.000000 maling-2.1.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.061796 maling-2.1.7/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-23 16:39:29.000000 maling-2.1.7/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-23 16:39:29.000000 maling-2.1.7/tests/filters/test_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:40:17.061796 maling-2.1.7/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 16:39:29.000000 maling-2.1.7/tests/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-23 16:39:29.000000 maling-2.1.7/tests/parser/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-04-23 16:39:29.000000 maling-2.1.7/tests/test_file_id.py
```

### Comparing `maling-2.1.6/COPYING` & `maling-2.1.7/COPYING`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/COPYING.lesser` & `maling-2.1.7/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/NOTICE` & `maling-2.1.7/NOTICE`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/PKG-INFO` & `maling-2.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maling
-Version: 2.1.6
+Version: 2.1.7
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/team
 Download-URL: https://github.com/team/team/releases/latest
 Author: Dan
 Author-email: dan@team.org
 License: LGPLv3
 Project-URL: Tracker, https://github.com/team/team/issues
```

### Comparing `maling-2.1.6/compiler/__init__.py` & `maling-2.1.7/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/api/__init__.py` & `maling-2.1.7/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/api/compiler.py` & `maling-2.1.7/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/api/source/auth_key.tl` & `maling-2.1.7/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/api/source/main_api.tl` & `maling-2.1.7/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/api/source/sys_msgs.tl` & `maling-2.1.7/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/api/template/combinator.txt` & `maling-2.1.7/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/api/template/type.txt` & `maling-2.1.7/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/errors/__init__.py` & `maling-2.1.7/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/errors/compiler.py` & `maling-2.1.7/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/errors/sort.py` & `maling-2.1.7/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/errors/source/400_BAD_REQUEST.tsv` & `maling-2.1.7/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/errors/source/401_UNAUTHORIZED.tsv` & `maling-2.1.7/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/errors/source/403_FORBIDDEN.tsv` & `maling-2.1.7/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `maling-2.1.7/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `maling-2.1.7/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/maling.egg-info/PKG-INFO` & `maling-2.1.7/maling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maling
-Version: 2.1.6
+Version: 2.1.7
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/team
 Download-URL: https://github.com/team/team/releases/latest
 Author: Dan
 Author-email: dan@team.org
 License: LGPLv3
 Project-URL: Tracker, https://github.com/team/team/issues
```

### Comparing `maling-2.1.6/maling.egg-info/SOURCES.txt` & `maling-2.1.7/maling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/setup.py` & `maling-2.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/__init__.py` & `maling-2.1.7/team/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 
-__version__ = "2.1.6"
+__version__ = "2.1.7"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `maling-2.1.6/team/client.py` & `maling-2.1.7/team/client.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/connection/__init__.py` & `maling-2.1.7/team/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/connection/connection.py` & `maling-2.1.7/team/connection/connection.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/connection/transport/__init__.py` & `maling-2.1.7/team/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/connection/transport/tcp/__init__.py` & `maling-2.1.7/team/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/connection/transport/tcp/tcp.py` & `maling-2.1.7/team/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/connection/transport/tcp/tcp_abridged.py` & `maling-2.1.7/team/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/connection/transport/tcp/tcp_abridged_o.py` & `maling-2.1.7/team/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/connection/transport/tcp/tcp_full.py` & `maling-2.1.7/team/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/connection/transport/tcp/tcp_intermediate.py` & `maling-2.1.7/team/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/connection/transport/tcp/tcp_intermediate_o.py` & `maling-2.1.7/team/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/crypto/__init__.py` & `maling-2.1.7/team/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/crypto/aes.py` & `maling-2.1.7/team/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/crypto/mtproto.py` & `maling-2.1.7/team/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/crypto/prime.py` & `maling-2.1.7/team/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/crypto/rsa.py` & `maling-2.1.7/team/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/dispatcher.py` & `maling-2.1.7/team/dispatcher.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/emoji.py` & `maling-2.1.7/team/emoji.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/__init__.py` & `maling-2.1.7/team/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/auto_name.py` & `maling-2.1.7/team/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/chat_action.py` & `maling-2.1.7/team/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/chat_event_action.py` & `maling-2.1.7/team/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/chat_member_status.py` & `maling-2.1.7/team/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/chat_members_filter.py` & `maling-2.1.7/team/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/chat_type.py` & `maling-2.1.7/team/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/message_entity_type.py` & `maling-2.1.7/team/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/message_media_type.py` & `maling-2.1.7/team/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/message_service_type.py` & `maling-2.1.7/team/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/messages_filter.py` & `maling-2.1.7/team/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/next_code_type.py` & `maling-2.1.7/team/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/parse_mode.py` & `maling-2.1.7/team/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/poll_type.py` & `maling-2.1.7/team/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/sent_code_type.py` & `maling-2.1.7/team/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/enums/user_status.py` & `maling-2.1.7/team/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/errors/__init__.py` & `maling-2.1.7/team/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/errors/rpc_error.py` & `maling-2.1.7/team/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/file_id.py` & `maling-2.1.7/team/file_id.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/filters.py` & `maling-2.1.7/team/filters.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/handlers/__init__.py` & `maling-2.1.7/team/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/handlers/callback_query_handler.py` & `maling-2.1.7/team/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/handlers/chat_join_request_handler.py` & `maling-2.1.7/team/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/handlers/chat_member_updated_handler.py` & `maling-2.1.7/team/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/handlers/chosen_inline_result_handler.py` & `maling-2.1.7/team/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/handlers/deleted_messages_handler.py` & `maling-2.1.7/team/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/handlers/disconnect_handler.py` & `maling-2.1.7/team/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/handlers/edited_message_handler.py` & `maling-2.1.7/team/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/handlers/handler.py` & `maling-2.1.7/team/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/handlers/inline_query_handler.py` & `maling-2.1.7/team/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/handlers/message_handler.py` & `maling-2.1.7/team/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/handlers/poll_handler.py` & `maling-2.1.7/team/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/handlers/raw_update_handler.py` & `maling-2.1.7/team/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/handlers/user_status_handler.py` & `maling-2.1.7/team/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/__init__.py` & `maling-2.1.7/team/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/advanced/__init__.py` & `maling-2.1.7/team/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/advanced/invoke.py` & `maling-2.1.7/team/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/advanced/resolve_peer.py` & `maling-2.1.7/team/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/advanced/save_file.py` & `maling-2.1.7/team/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/__init__.py` & `maling-2.1.7/team/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/accept_terms_of_service.py` & `maling-2.1.7/team/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/check_password.py` & `maling-2.1.7/team/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/connect.py` & `maling-2.1.7/team/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/disconnect.py` & `maling-2.1.7/team/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/get_password_hint.py` & `maling-2.1.7/team/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/initialize.py` & `maling-2.1.7/team/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/log_out.py` & `maling-2.1.7/team/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/recover_password.py` & `maling-2.1.7/team/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/resend_code.py` & `maling-2.1.7/team/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/send_code.py` & `maling-2.1.7/team/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/send_recovery_code.py` & `maling-2.1.7/team/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/sign_in.py` & `maling-2.1.7/team/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/sign_in_bot.py` & `maling-2.1.7/team/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/sign_up.py` & `maling-2.1.7/team/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/auth/terminate.py` & `maling-2.1.7/team/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/__init__.py` & `maling-2.1.7/team/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/answer_callback_query.py` & `maling-2.1.7/team/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/answer_inline_query.py` & `maling-2.1.7/team/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/answer_web_app_query.py` & `maling-2.1.7/team/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/delete_bot_commands.py` & `maling-2.1.7/team/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/get_bot_commands.py` & `maling-2.1.7/team/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/get_bot_default_privileges.py` & `maling-2.1.7/team/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/get_chat_menu_button.py` & `maling-2.1.7/team/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/get_game_high_scores.py` & `maling-2.1.7/team/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/get_inline_bot_results.py` & `maling-2.1.7/team/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/request_callback_answer.py` & `maling-2.1.7/team/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/send_game.py` & `maling-2.1.7/team/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/send_inline_bot_result.py` & `maling-2.1.7/team/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/set_bot_commands.py` & `maling-2.1.7/team/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/set_bot_default_privileges.py` & `maling-2.1.7/team/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/set_chat_menu_button.py` & `maling-2.1.7/team/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/bots/set_game_score.py` & `maling-2.1.7/team/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/__init__.py` & `maling-2.1.7/team/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/add_chat_members.py` & `maling-2.1.7/team/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/archive_chats.py` & `maling-2.1.7/team/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/ban_chat_member.py` & `maling-2.1.7/team/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/create_channel.py` & `maling-2.1.7/team/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/create_group.py` & `maling-2.1.7/team/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/create_supergroup.py` & `maling-2.1.7/team/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/delete_channel.py` & `maling-2.1.7/team/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/delete_chat_photo.py` & `maling-2.1.7/team/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/delete_supergroup.py` & `maling-2.1.7/team/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/delete_user_history.py` & `maling-2.1.7/team/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/get_chat.py` & `maling-2.1.7/team/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/get_chat_event_log.py` & `maling-2.1.7/team/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/get_chat_member.py` & `maling-2.1.7/team/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/get_chat_members.py` & `maling-2.1.7/team/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/get_chat_members_count.py` & `maling-2.1.7/team/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/get_chat_online_count.py` & `maling-2.1.7/team/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/get_dialogs.py` & `maling-2.1.7/team/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/get_dialogs_count.py` & `maling-2.1.7/team/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/get_nearby_chats.py` & `maling-2.1.7/team/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/get_send_as_chats.py` & `maling-2.1.7/team/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/join_chat.py` & `maling-2.1.7/team/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/leave_chat.py` & `maling-2.1.7/team/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/mark_chat_unread.py` & `maling-2.1.7/team/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/pin_chat_message.py` & `maling-2.1.7/team/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/promote_chat_member.py` & `maling-2.1.7/team/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/restrict_chat_member.py` & `maling-2.1.7/team/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/set_administrator_title.py` & `maling-2.1.7/team/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/set_chat_description.py` & `maling-2.1.7/team/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/set_chat_permissions.py` & `maling-2.1.7/team/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/set_chat_photo.py` & `maling-2.1.7/team/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/set_chat_protected_content.py` & `maling-2.1.7/team/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/set_chat_title.py` & `maling-2.1.7/team/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/set_chat_username.py` & `maling-2.1.7/team/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/set_send_as_chat.py` & `maling-2.1.7/team/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/set_slow_mode.py` & `maling-2.1.7/team/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/unarchive_chats.py` & `maling-2.1.7/team/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/unban_chat_member.py` & `maling-2.1.7/team/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/unpin_all_chat_messages.py` & `maling-2.1.7/team/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/chats/unpin_chat_message.py` & `maling-2.1.7/team/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/contacts/__init__.py` & `maling-2.1.7/team/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/contacts/add_contact.py` & `maling-2.1.7/team/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/contacts/delete_contacts.py` & `maling-2.1.7/team/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/contacts/get_contacts.py` & `maling-2.1.7/team/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/contacts/get_contacts_count.py` & `maling-2.1.7/team/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/contacts/import_contacts.py` & `maling-2.1.7/team/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/decorators/__init__.py` & `maling-2.1.7/team/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/decorators/on_callback_query.py` & `maling-2.1.7/team/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/decorators/on_chat_join_request.py` & `maling-2.1.7/team/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/decorators/on_chat_member_updated.py` & `maling-2.1.7/team/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/decorators/on_chosen_inline_result.py` & `maling-2.1.7/team/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/decorators/on_deleted_messages.py` & `maling-2.1.7/team/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/decorators/on_disconnect.py` & `maling-2.1.7/team/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/decorators/on_edited_message.py` & `maling-2.1.7/team/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/decorators/on_inline_query.py` & `maling-2.1.7/team/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/decorators/on_message.py` & `maling-2.1.7/team/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/decorators/on_poll.py` & `maling-2.1.7/team/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/decorators/on_raw_update.py` & `maling-2.1.7/team/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/decorators/on_user_status.py` & `maling-2.1.7/team/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/__init__.py` & `maling-2.1.7/team/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/approve_all_chat_join_requests.py` & `maling-2.1.7/team/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/approve_chat_join_request.py` & `maling-2.1.7/team/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/create_chat_invite_link.py` & `maling-2.1.7/team/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/decline_all_chat_join_requests.py` & `maling-2.1.7/team/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/decline_chat_join_request.py` & `maling-2.1.7/team/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/delete_chat_admin_invite_links.py` & `maling-2.1.7/team/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/delete_chat_invite_link.py` & `maling-2.1.7/team/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/edit_chat_invite_link.py` & `maling-2.1.7/team/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/export_chat_invite_link.py` & `maling-2.1.7/team/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/get_chat_admin_invite_links.py` & `maling-2.1.7/team/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/get_chat_admin_invite_links_count.py` & `maling-2.1.7/team/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/get_chat_admins_with_invite_links.py` & `maling-2.1.7/team/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/get_chat_invite_link.py` & `maling-2.1.7/team/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/get_chat_invite_link_joiners.py` & `maling-2.1.7/team/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/get_chat_invite_link_joiners_count.py` & `maling-2.1.7/team/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/get_chat_join_requests.py` & `maling-2.1.7/team/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/invite_links/revoke_chat_invite_link.py` & `maling-2.1.7/team/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/__init__.py` & `maling-2.1.7/team/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/copy_media_group.py` & `maling-2.1.7/team/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/copy_message.py` & `maling-2.1.7/team/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/delete_messages.py` & `maling-2.1.7/team/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/download_media.py` & `maling-2.1.7/team/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/edit_inline_caption.py` & `maling-2.1.7/team/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/edit_inline_media.py` & `maling-2.1.7/team/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/edit_inline_reply_markup.py` & `maling-2.1.7/team/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/edit_inline_text.py` & `maling-2.1.7/team/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/edit_message_caption.py` & `maling-2.1.7/team/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/edit_message_media.py` & `maling-2.1.7/team/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/edit_message_reply_markup.py` & `maling-2.1.7/team/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/edit_message_text.py` & `maling-2.1.7/team/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/forward_messages.py` & `maling-2.1.7/team/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/get_chat_history.py` & `maling-2.1.7/team/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/get_chat_history_count.py` & `maling-2.1.7/team/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/get_custom_emoji_stickers.py` & `maling-2.1.7/team/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/get_discussion_message.py` & `maling-2.1.7/team/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/get_discussion_replies.py` & `maling-2.1.7/team/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/get_discussion_replies_count.py` & `maling-2.1.7/team/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/get_media_group.py` & `maling-2.1.7/team/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/get_messages.py` & `maling-2.1.7/team/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/inline_session.py` & `maling-2.1.7/team/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/read_chat_history.py` & `maling-2.1.7/team/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/retract_vote.py` & `maling-2.1.7/team/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/search_global.py` & `maling-2.1.7/team/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/search_global_count.py` & `maling-2.1.7/team/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/search_messages.py` & `maling-2.1.7/team/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/search_messages_count.py` & `maling-2.1.7/team/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_animation.py` & `maling-2.1.7/team/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_audio.py` & `maling-2.1.7/team/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_cached_media.py` & `maling-2.1.7/team/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_chat_action.py` & `maling-2.1.7/team/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_contact.py` & `maling-2.1.7/team/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_dice.py` & `maling-2.1.7/team/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_document.py` & `maling-2.1.7/team/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_location.py` & `maling-2.1.7/team/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_media_group.py` & `maling-2.1.7/team/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_message.py` & `maling-2.1.7/team/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_photo.py` & `maling-2.1.7/team/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_poll.py` & `maling-2.1.7/team/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_reaction.py` & `maling-2.1.7/team/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_sticker.py` & `maling-2.1.7/team/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_venue.py` & `maling-2.1.7/team/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_video.py` & `maling-2.1.7/team/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_video_note.py` & `maling-2.1.7/team/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/send_voice.py` & `maling-2.1.7/team/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/stop_poll.py` & `maling-2.1.7/team/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/stream_media.py` & `maling-2.1.7/team/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/messages/vote_poll.py` & `maling-2.1.7/team/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/password/__init__.py` & `maling-2.1.7/team/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/password/change_cloud_password.py` & `maling-2.1.7/team/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/password/enable_cloud_password.py` & `maling-2.1.7/team/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/password/remove_cloud_password.py` & `maling-2.1.7/team/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/users/__init__.py` & `maling-2.1.7/team/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/users/block_user.py` & `maling-2.1.7/team/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/users/delete_profile_photos.py` & `maling-2.1.7/team/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/users/get_chat_photos.py` & `maling-2.1.7/team/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/users/get_chat_photos_count.py` & `maling-2.1.7/team/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/users/get_common_chats.py` & `maling-2.1.7/team/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/users/get_default_emoji_statuses.py` & `maling-2.1.7/team/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/users/get_me.py` & `maling-2.1.7/team/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/users/get_users.py` & `maling-2.1.7/team/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/users/set_emoji_status.py` & `maling-2.1.7/team/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/users/set_profile_photo.py` & `maling-2.1.7/team/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/users/set_username.py` & `maling-2.1.7/team/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/users/unblock_user.py` & `maling-2.1.7/team/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/users/update_profile.py` & `maling-2.1.7/team/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/utilities/__init__.py` & `maling-2.1.7/team/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/utilities/add_handler.py` & `maling-2.1.7/team/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/utilities/compose.py` & `maling-2.1.7/team/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/utilities/export_session_string.py` & `maling-2.1.7/team/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/utilities/idle.py` & `maling-2.1.7/team/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/utilities/remove_handler.py` & `maling-2.1.7/team/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/utilities/restart.py` & `maling-2.1.7/team/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/utilities/run.py` & `maling-2.1.7/team/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/utilities/start.py` & `maling-2.1.7/team/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/utilities/stop.py` & `maling-2.1.7/team/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/methods/utilities/stop_transmission.py` & `maling-2.1.7/team/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/mime_types.py` & `maling-2.1.7/team/mime_types.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/nandev/autopilot.py` & `maling-2.1.7/team/nandev/autopilot.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/nandev/class_emoji.py` & `maling-2.1.7/team/nandev/class_emoji.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/nandev/class_handler.py` & `maling-2.1.7/team/nandev/class_handler.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/nandev/class_log.py` & `maling-2.1.7/team/nandev/class_log.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/nandev/class_modules.py` & `maling-2.1.7/team/nandev/class_modules.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/nandev/class_mongo.py` & `maling-2.1.7/team/nandev/class_mongo.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/nandev/class_pytgc.py` & `maling-2.1.7/team/nandev/class_pytgc.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/nandev/database.py` & `maling-2.1.7/team/nandev/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,47 @@
 langm = {}
 
 class MongoDB:
     def __init__(self, db_name, mongo_url: str) -> None:
         self._db = MongoClient(mongo_url)
         self._db = self._db[db_name]
 
+  def add_ubot(self, user_id, api_id, api_hash, session_string):
+        ubotdb = self._db.ubotdb
+
+        ubotdb.update_one(
+            {"user_id": user_id},
+            {
+                "$set": {
+                    "api_id": api_id,
+                    "api_hash": api_hash,
+                    "session_string": session_string,
+                }
+            },
+            upsert=True,
+        )
+
+    def remove_ubot(self, user_id):
+        ubotdb = self._db.ubotdb
+
+        ubotdb.delete_one({"user_id": user_id})
+
+    def get_userbots(self):
+        ubotdb = self._db.ubotdb
+        data = ubotdb.find({"user_id": {"$exists": 1}}, {"_id": 0})
+        return [
+            {
+                "name": str(ubot["user_id"]),
+                "api_id": ubot["api_id"],
+                "api_hash": ubot["api_hash"],
+                "session_string": ubot["session_string"],
+            }
+            for ubot in data
+        ]
+
     def get_pref(self, user_id):
         user_prefixes = self._db.user_prefixes
 
         result = user_prefixes.find_one({"user_id": user_id}, {"_id": 0, "prefix": 1})
 
         return json.loads(result["prefix"]) if result and "prefix" in result else "."
 
@@ -558,8 +591,8 @@
         _er = True
     if not _er:
         LOGGER(
             "No DB requirement fullfilled!\nPlease install redis, mongo or sql dependencies...\nTill then using local file as database."
         )
     sys.exit()
     
-ndB = MixDB()
+ndB = MixDB()
```

### Comparing `maling-2.1.6/team/nandev/new_database.py` & `maling-2.1.7/team/nandev/new_database.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/parser/__init__.py` & `maling-2.1.7/team/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/parser/html.py` & `maling-2.1.7/team/parser/html.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/parser/markdown.py` & `maling-2.1.7/team/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/parser/parser.py` & `maling-2.1.7/team/parser/parser.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/parser/utils.py` & `maling-2.1.7/team/parser/utils.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/__init__.py` & `maling-2.1.7/team/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/__init__.py` & `maling-2.1.7/team/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/future_salt.py` & `maling-2.1.7/team/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/future_salts.py` & `maling-2.1.7/team/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/gzip_packed.py` & `maling-2.1.7/team/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/list.py` & `maling-2.1.7/team/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/message.py` & `maling-2.1.7/team/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/msg_container.py` & `maling-2.1.7/team/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/primitives/__init__.py` & `maling-2.1.7/team/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/primitives/bool.py` & `maling-2.1.7/team/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/primitives/bytes.py` & `maling-2.1.7/team/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/primitives/double.py` & `maling-2.1.7/team/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/primitives/int.py` & `maling-2.1.7/team/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/primitives/string.py` & `maling-2.1.7/team/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/primitives/vector.py` & `maling-2.1.7/team/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/raw/core/tl_object.py` & `maling-2.1.7/team/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/session/__init__.py` & `maling-2.1.7/team/session/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/session/auth.py` & `maling-2.1.7/team/session/auth.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/session/internals/__init__.py` & `maling-2.1.7/team/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/session/internals/data_center.py` & `maling-2.1.7/team/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/session/internals/msg_factory.py` & `maling-2.1.7/team/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/session/internals/msg_id.py` & `maling-2.1.7/team/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/session/internals/seq_no.py` & `maling-2.1.7/team/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/session/session.py` & `maling-2.1.7/team/session/session.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/storage/__init__.py` & `maling-2.1.7/team/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/storage/file_storage.py` & `maling-2.1.7/team/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/storage/memory_storage.py` & `maling-2.1.7/team/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/storage/sqlite_storage.py` & `maling-2.1.7/team/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/storage/storage.py` & `maling-2.1.7/team/storage/storage.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/sync.py` & `maling-2.1.7/team/sync.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/__init__.py` & `maling-2.1.7/team/types/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/authorization/__init__.py` & `maling-2.1.7/team/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/authorization/sent_code.py` & `maling-2.1.7/team/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/authorization/terms_of_service.py` & `maling-2.1.7/team/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/__init__.py` & `maling-2.1.7/team/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/bot_command.py` & `maling-2.1.7/team/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope.py` & `maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope_chat.py` & `maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/bot_command_scope_default.py` & `maling-2.1.7/team/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/callback_game.py` & `maling-2.1.7/team/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/callback_query.py` & `maling-2.1.7/team/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/force_reply.py` & `maling-2.1.7/team/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/game_high_score.py` & `maling-2.1.7/team/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/inline_keyboard_button.py` & `maling-2.1.7/team/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/inline_keyboard_markup.py` & `maling-2.1.7/team/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/keyboard_button.py` & `maling-2.1.7/team/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/login_url.py` & `maling-2.1.7/team/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/menu_button.py` & `maling-2.1.7/team/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/menu_button_commands.py` & `maling-2.1.7/team/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/menu_button_default.py` & `maling-2.1.7/team/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/menu_button_web_app.py` & `maling-2.1.7/team/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/reply_keyboard_markup.py` & `maling-2.1.7/team/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/reply_keyboard_remove.py` & `maling-2.1.7/team/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/sent_web_app_message.py` & `maling-2.1.7/team/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/bots_and_keyboards/web_app_info.py` & `maling-2.1.7/team/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/__init__.py` & `maling-2.1.7/team/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/chosen_inline_result.py` & `maling-2.1.7/team/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query.py` & `maling-2.1.7/team/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_animation.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_article.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_audio.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_cached_animation.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_cached_audio.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_cached_document.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_cached_photo.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_cached_sticker.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_cached_video.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_cached_voice.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_contact.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_document.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_location.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_photo.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_venue.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_video.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/inline_mode/inline_query_result_voice.py` & `maling-2.1.7/team/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/input_media/__init__.py` & `maling-2.1.7/team/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/input_media/input_media.py` & `maling-2.1.7/team/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/input_media/input_media_animation.py` & `maling-2.1.7/team/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/input_media/input_media_audio.py` & `maling-2.1.7/team/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/input_media/input_media_document.py` & `maling-2.1.7/team/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/input_media/input_media_photo.py` & `maling-2.1.7/team/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/input_media/input_media_video.py` & `maling-2.1.7/team/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/input_media/input_phone_contact.py` & `maling-2.1.7/team/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/input_message_content/__init__.py` & `maling-2.1.7/team/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/input_message_content/input_message_content.py` & `maling-2.1.7/team/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/input_message_content/input_text_message_content.py` & `maling-2.1.7/team/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/list.py` & `maling-2.1.7/team/types/list.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/__init__.py` & `maling-2.1.7/team/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/animation.py` & `maling-2.1.7/team/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/audio.py` & `maling-2.1.7/team/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/contact.py` & `maling-2.1.7/team/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/dice.py` & `maling-2.1.7/team/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/document.py` & `maling-2.1.7/team/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/game.py` & `maling-2.1.7/team/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/location.py` & `maling-2.1.7/team/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/message.py` & `maling-2.1.7/team/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/message_entity.py` & `maling-2.1.7/team/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/message_reactions.py` & `maling-2.1.7/team/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/photo.py` & `maling-2.1.7/team/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/poll.py` & `maling-2.1.7/team/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/poll_option.py` & `maling-2.1.7/team/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/reaction.py` & `maling-2.1.7/team/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/sticker.py` & `maling-2.1.7/team/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/stripped_thumbnail.py` & `maling-2.1.7/team/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/thumbnail.py` & `maling-2.1.7/team/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/venue.py` & `maling-2.1.7/team/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/video.py` & `maling-2.1.7/team/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/video_note.py` & `maling-2.1.7/team/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/voice.py` & `maling-2.1.7/team/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/web_app_data.py` & `maling-2.1.7/team/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/messages_and_media/web_page.py` & `maling-2.1.7/team/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/object.py` & `maling-2.1.7/team/types/object.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/update.py` & `maling-2.1.7/team/types/update.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/__init__.py` & `maling-2.1.7/team/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/chat.py` & `maling-2.1.7/team/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/chat_admin_with_invite_links.py` & `maling-2.1.7/team/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/chat_event.py` & `maling-2.1.7/team/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/chat_event_filter.py` & `maling-2.1.7/team/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/chat_invite_link.py` & `maling-2.1.7/team/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/chat_join_request.py` & `maling-2.1.7/team/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/chat_joiner.py` & `maling-2.1.7/team/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/chat_member.py` & `maling-2.1.7/team/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/chat_member_updated.py` & `maling-2.1.7/team/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/chat_permissions.py` & `maling-2.1.7/team/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/chat_photo.py` & `maling-2.1.7/team/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/chat_preview.py` & `maling-2.1.7/team/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/chat_privileges.py` & `maling-2.1.7/team/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/chat_reactions.py` & `maling-2.1.7/team/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/dialog.py` & `maling-2.1.7/team/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/emoji_status.py` & `maling-2.1.7/team/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/invite_link_importer.py` & `maling-2.1.7/team/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/restriction.py` & `maling-2.1.7/team/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/user.py` & `maling-2.1.7/team/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/video_chat_ended.py` & `maling-2.1.7/team/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/video_chat_members_invited.py` & `maling-2.1.7/team/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/video_chat_scheduled.py` & `maling-2.1.7/team/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/types/user_and_chats/video_chat_started.py` & `maling-2.1.7/team/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/team/utils.py` & `maling-2.1.7/team/utils.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/tests/__init__.py` & `maling-2.1.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/tests/filters/__init__.py` & `maling-2.1.7/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/tests/filters/test_command.py` & `maling-2.1.7/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/tests/parser/__init__.py` & `maling-2.1.7/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/tests/parser/test_html.py` & `maling-2.1.7/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `maling-2.1.6/tests/test_file_id.py` & `maling-2.1.7/tests/test_file_id.py`

 * *Files identical despite different names*

