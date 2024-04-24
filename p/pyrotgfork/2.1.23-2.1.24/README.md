# Comparing `tmp/pyrotgfork-2.1.23.tar.gz` & `tmp/pyrotgfork-2.1.24.tar.gz`

## Comparing `pyrotgfork-2.1.23.tar` & `pyrotgfork-2.1.24.tar`

### file list

```diff
@@ -1,474 +1,474 @@
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/__init__.py
--rw-r--r--   0        0        0    46382 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/client.py
--rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/dispatcher.py
--rw-r--r--   0        0        0   208021 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/emoji.py
--rw-r--r--   0        0        0    16314 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/file_id.py
--rw-r--r--   0        0        0    28452 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/filters.py
--rw-r--r--   0        0        0    61915 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/mime_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/py.typed
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/sync.py
--rw-r--r--   0        0        0    17420 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/utils.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/connection/__init__.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/connection/connection.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/connection/transport/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/crypto/__init__.py
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/crypto/aes.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/crypto/mtproto.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/crypto/prime.py
--rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/crypto/rsa.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/accent_color.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/auto_name.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/chat_action.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/chat_event_action.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/chat_member_status.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/chat_type.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/client_platform.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/message_entity_type.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/message_media_type.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/message_service_type.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/messages_filter.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/next_code_type.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/parse_mode.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/poll_type.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/profile_color.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/sent_code_type.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/enums/user_status.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/errors/__init__.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/errors/rpc_error.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/__init__.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/handler.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/message_handler.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/message_reaction_count_updated_handler.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/message_reaction_updated_handler.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/poll_handler.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/handlers/user_status_handler.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/__init__.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/advanced/save_file.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/__init__.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/check_password.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/connect.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/initialize.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/log_out.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/send_code.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/auth/terminate.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/__init__.py
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/send_game.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/bots/set_game_score.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/business/__init__.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/business/get_business_connection.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chat_topics/__init__.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chat_topics/close_forum_topic.py
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chat_topics/create_forum_topic.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chat_topics/delete_forum_topic.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chat_topics/edit_forum_topic.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chat_topics/get_forum_topic.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chat_topics/get_forum_topics.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chat_topics/hide_forum_topic.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chat_topics/reopen_forum_topic.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chat_topics/unhide_forum_topic.py
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/__init__.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/create_group.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/get_created_chats.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/set_chat_ttl.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/chats/unpin_chat_message.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/contacts/import_contacts.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/on_message_reaction_count_updated.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/on_message_reaction_updated.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/decorators/on_user_status.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/invite_links/revoke_chat_invite_link.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/__init__.py
--rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/download_media.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/search_global.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0        0        0     6774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0        0        0    13425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_document.py
--rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_location.py
--rw-r--r--   0        0        0    22833 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_message.py
--rw-r--r--   0        0        0    12533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0        0        0    15141 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_video.py
--rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/set_reaction.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/messages/vote_poll.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/password/__init__.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/password/remove_cloud_password.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/stickers/get_stickers.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/__init__.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/block_user.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/get_me.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/get_users.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/set_birthdate.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/set_personal_chat.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/set_username.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/users/update_profile.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/utilities/compose.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/utilities/idle.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/utilities/restart.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/utilities/run.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/utilities/start.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/utilities/stop.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/parser/__init__.py
--rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/parser/html.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/parser/markdown.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/parser/parser.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/parser/utils.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/__init__.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/__init__.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/future_salt.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/future_salts.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/list.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/message.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/msg_container.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/tl_object.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/session/__init__.py
--rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/session/auth.py
--rw-r--r--   0        0        0    14294 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/session/session.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/session/internals/__init__.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/session/internals/data_center.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/session/internals/msg_id.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/session/internals/seq_no.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/storage/__init__.py
--rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/storage/aio_sqlite_storage.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/storage/file_storage.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/storage/memory_storage.py
--rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/storage/storage.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/list.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/object.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/update.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/authorization/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/authorization/terms_of_service.py
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0        0        0    14613 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/web_app_info.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/business/__init__.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/business/business_connection.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/business/business_intro.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/business/business_location.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/business/business_opening_hours.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/business/business_opening_hours_interval.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/chat_topics/__init__.py
--rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/chat_topics/forum_topic.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/chat_topics/forum_topic_closed.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/chat_topics/forum_topic_created.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/chat_topics/forum_topic_edited.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/chat_topics/forum_topic_reopened.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/chat_topics/general_forum_topic_hidden.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/chat_topics/general_forum_topic_unhidden.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_voice.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/input_media/__init__.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/input_media/input_media.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/input_media/input_phone_contact.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/input_media/link_preview_options.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0        0        0    13513 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/input_message_content/external_reply_info.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/input_message_content/reply_parameters.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/message_origin/__init__.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/message_origin/message_import_info.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/message_origin/message_origin.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/message_origin/message_origin_channel.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/message_origin/message_origin_chat.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/message_origin/message_origin_hidden_user.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/message_origin/message_origin_user.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/chat_boost_added.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/gift_code.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/gifted_premium.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/giveaway.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/giveaway_completed.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/giveaway_winners.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0        0        0   190251 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/message_reaction_count_updated.py
--rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/message_reaction_updated.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/story.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/birthdate.py
--rw-r--r--   0        0        0    45767 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_color.py
--rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_shared.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0        0        0    18356 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/users_shared.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/video_chat_participants_invited.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/COPYING
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/COPYING.lesser
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/NOTICE
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/README.md
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/hatch_build.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/pyproject.toml
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.23/PKG-INFO
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/__init__.py
+-rw-r--r--   0        0        0    46382 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/client.py
+-rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/dispatcher.py
+-rw-r--r--   0        0        0   208021 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/emoji.py
+-rw-r--r--   0        0        0    16314 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/file_id.py
+-rw-r--r--   0        0        0    28452 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/filters.py
+-rw-r--r--   0        0        0    61915 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/mime_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/py.typed
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/sync.py
+-rw-r--r--   0        0        0    17420 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/utils.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/connection/__init__.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/connection/connection.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/connection/transport/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/crypto/__init__.py
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/crypto/aes.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/crypto/mtproto.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/crypto/prime.py
+-rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/crypto/rsa.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/accent_color.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/auto_name.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/chat_action.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/chat_type.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/client_platform.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/message_media_type.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/message_service_type.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/messages_filter.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/next_code_type.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/parse_mode.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/poll_type.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/profile_color.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/enums/user_status.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/errors/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/errors/rpc_error.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/__init__.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/handler.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/message_handler.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/message_reaction_count_updated_handler.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/message_reaction_updated_handler.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/handlers/user_status_handler.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/__init__.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/advanced/save_file.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/connect.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/auth/terminate.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/bots/set_game_score.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/business/__init__.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/business/get_business_connection.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chat_topics/__init__.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chat_topics/close_forum_topic.py
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chat_topics/create_forum_topic.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chat_topics/delete_forum_topic.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chat_topics/edit_forum_topic.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chat_topics/get_forum_topic.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chat_topics/get_forum_topics.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chat_topics/hide_forum_topic.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chat_topics/reopen_forum_topic.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chat_topics/unhide_forum_topic.py
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/get_created_chats.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/set_chat_ttl.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/chats/unpin_chat_message.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/contacts/import_contacts.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/on_message_reaction_count_updated.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/on_message_reaction_updated.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/decorators/on_user_status.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0        0        0     6774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0        0        0    13425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0        0        0     6504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0        0        0    22833 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0        0        0    12533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0        0        0    15141 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/set_reaction.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/messages/vote_poll.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/password/__init__.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/password/remove_cloud_password.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/stickers/get_stickers.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/__init__.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/block_user.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/get_me.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/get_users.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/set_birthdate.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/set_personal_chat.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/set_username.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/users/update_profile.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/utilities/run.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/utilities/start.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/parser/__init__.py
+-rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/parser/html.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/parser/markdown.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/parser/parser.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/parser/utils.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/__init__.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/__init__.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/list.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/message.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/msg_container.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/tl_object.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/session/__init__.py
+-rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/session/auth.py
+-rw-r--r--   0        0        0    14294 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/session/session.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/session/internals/__init__.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/session/internals/data_center.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/storage/__init__.py
+-rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/storage/aio_sqlite_storage.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/storage/file_storage.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/storage/memory_storage.py
+-rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/storage/storage.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/list.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/object.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/update.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/authorization/terms_of_service.py
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0        0        0    14613 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/web_app_info.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/business/__init__.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/business/business_connection.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/business/business_intro.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/business/business_location.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/business/business_opening_hours.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/business/business_opening_hours_interval.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/chat_topics/__init__.py
+-rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/chat_topics/forum_topic.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/chat_topics/forum_topic_closed.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/chat_topics/forum_topic_created.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/chat_topics/forum_topic_edited.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/chat_topics/forum_topic_reopened.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/chat_topics/general_forum_topic_hidden.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/chat_topics/general_forum_topic_unhidden.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_voice.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/input_media/input_phone_contact.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/input_media/link_preview_options.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0        0        0    13513 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/input_message_content/external_reply_info.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/input_message_content/reply_parameters.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/message_origin/__init__.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/message_origin/message_import_info.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/message_origin/message_origin.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/message_origin/message_origin_channel.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/message_origin/message_origin_chat.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/message_origin/message_origin_hidden_user.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/message_origin/message_origin_user.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/chat_boost_added.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/gift_code.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/gifted_premium.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/giveaway.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/giveaway_completed.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/giveaway_winners.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0        0        0   190251 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/message_reaction_count_updated.py
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/message_reaction_updated.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/story.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/birthdate.py
+-rw-r--r--   0        0        0    46436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_color.py
+-rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_shared.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0        0        0    18356 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/users_shared.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/video_chat_participants_invited.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/COPYING
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/COPYING.lesser
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/NOTICE
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/README.md
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/hatch_build.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/pyproject.toml
+-rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.24/PKG-INFO
```

### Comparing `pyrotgfork-2.1.23/pyrogram/__init__.py` & `pyrotgfork-2.1.24/pyrogram/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "2.1.23"
+__version__ = "2.1.24"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `pyrotgfork-2.1.23/pyrogram/client.py` & `pyrotgfork-2.1.24/pyrogram/client.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/dispatcher.py` & `pyrotgfork-2.1.24/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/emoji.py` & `pyrotgfork-2.1.24/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/file_id.py` & `pyrotgfork-2.1.24/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/filters.py` & `pyrotgfork-2.1.24/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/mime_types.py` & `pyrotgfork-2.1.24/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/sync.py` & `pyrotgfork-2.1.24/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/utils.py` & `pyrotgfork-2.1.24/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/connection/__init__.py` & `pyrotgfork-2.1.24/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/connection/connection.py` & `pyrotgfork-2.1.24/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/connection/transport/__init__.py` & `pyrotgfork-2.1.24/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/connection/transport/tcp/__init__.py` & `pyrotgfork-2.1.24/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/connection/transport/tcp/tcp.py` & `pyrotgfork-2.1.24/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/connection/transport/tcp/tcp_abridged.py` & `pyrotgfork-2.1.24/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `pyrotgfork-2.1.24/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/connection/transport/tcp/tcp_full.py` & `pyrotgfork-2.1.24/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `pyrotgfork-2.1.24/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `pyrotgfork-2.1.24/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/crypto/__init__.py` & `pyrotgfork-2.1.24/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/crypto/aes.py` & `pyrotgfork-2.1.24/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/crypto/mtproto.py` & `pyrotgfork-2.1.24/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/crypto/prime.py` & `pyrotgfork-2.1.24/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/crypto/rsa.py` & `pyrotgfork-2.1.24/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/__init__.py` & `pyrotgfork-2.1.24/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/accent_color.py` & `pyrotgfork-2.1.24/pyrogram/enums/accent_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/auto_name.py` & `pyrotgfork-2.1.24/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/chat_action.py` & `pyrotgfork-2.1.24/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/chat_event_action.py` & `pyrotgfork-2.1.24/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/chat_member_status.py` & `pyrotgfork-2.1.24/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/chat_members_filter.py` & `pyrotgfork-2.1.24/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/chat_type.py` & `pyrotgfork-2.1.24/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/client_platform.py` & `pyrotgfork-2.1.24/pyrogram/enums/client_platform.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/message_entity_type.py` & `pyrotgfork-2.1.24/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/message_media_type.py` & `pyrotgfork-2.1.24/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/message_service_type.py` & `pyrotgfork-2.1.24/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/messages_filter.py` & `pyrotgfork-2.1.24/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/next_code_type.py` & `pyrotgfork-2.1.24/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/parse_mode.py` & `pyrotgfork-2.1.24/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/poll_type.py` & `pyrotgfork-2.1.24/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/profile_color.py` & `pyrotgfork-2.1.24/pyrogram/enums/profile_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/sent_code_type.py` & `pyrotgfork-2.1.24/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/enums/user_status.py` & `pyrotgfork-2.1.24/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/errors/__init__.py` & `pyrotgfork-2.1.24/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/errors/rpc_error.py` & `pyrotgfork-2.1.24/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/__init__.py` & `pyrotgfork-2.1.24/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/callback_query_handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/chat_join_request_handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/chat_member_updated_handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/chosen_inline_result_handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/deleted_messages_handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/disconnect_handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/edited_message_handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/inline_query_handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/message_handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/message_reaction_count_updated_handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/message_reaction_count_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/message_reaction_updated_handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/message_reaction_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/poll_handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/raw_update_handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/handlers/user_status_handler.py` & `pyrotgfork-2.1.24/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/advanced/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/advanced/invoke.py` & `pyrotgfork-2.1.24/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/advanced/resolve_peer.py` & `pyrotgfork-2.1.24/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/advanced/save_file.py` & `pyrotgfork-2.1.24/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/accept_terms_of_service.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/check_password.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/connect.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/disconnect.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/get_password_hint.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/initialize.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/log_out.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/recover_password.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/resend_code.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/send_code.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/send_recovery_code.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/sign_in.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/sign_in_bot.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/sign_up.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/auth/terminate.py` & `pyrotgfork-2.1.24/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/answer_callback_query.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/answer_inline_query.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/answer_web_app_query.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/delete_bot_commands.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/get_bot_commands.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/get_bot_default_privileges.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/get_chat_menu_button.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/get_game_high_scores.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/get_inline_bot_results.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/request_callback_answer.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/send_game.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/send_inline_bot_result.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/set_bot_commands.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/set_bot_default_privileges.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/set_chat_menu_button.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/bots/set_game_score.py` & `pyrotgfork-2.1.24/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/business/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/business/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/business/get_business_connection.py` & `pyrotgfork-2.1.24/pyrogram/methods/business/get_business_connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chat_topics/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/chat_topics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chat_topics/close_forum_topic.py` & `pyrotgfork-2.1.24/pyrogram/methods/chat_topics/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chat_topics/create_forum_topic.py` & `pyrotgfork-2.1.24/pyrogram/methods/chat_topics/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chat_topics/delete_forum_topic.py` & `pyrotgfork-2.1.24/pyrogram/methods/chat_topics/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chat_topics/edit_forum_topic.py` & `pyrotgfork-2.1.24/pyrogram/methods/chat_topics/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chat_topics/get_forum_topic.py` & `pyrotgfork-2.1.24/pyrogram/methods/chat_topics/get_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py` & `pyrotgfork-2.1.24/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chat_topics/get_forum_topics.py` & `pyrotgfork-2.1.24/pyrogram/methods/chat_topics/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chat_topics/hide_forum_topic.py` & `pyrotgfork-2.1.24/pyrogram/methods/chat_topics/hide_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chat_topics/reopen_forum_topic.py` & `pyrotgfork-2.1.24/pyrogram/methods/chat_topics/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chat_topics/unhide_forum_topic.py` & `pyrotgfork-2.1.24/pyrogram/methods/chat_topics/unhide_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/add_chat_members.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/archive_chats.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/ban_chat_member.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/create_channel.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/create_group.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/create_supergroup.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/delete_channel.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/delete_chat_photo.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/delete_supergroup.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/delete_user_history.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/get_chat.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/get_chat_event_log.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/get_chat_member.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/get_chat_members.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/get_chat_members_count.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/get_chat_online_count.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/get_created_chats.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/get_created_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/get_dialogs.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/get_dialogs_count.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/get_nearby_chats.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/get_send_as_chats.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/join_chat.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/leave_chat.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/mark_chat_unread.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/pin_chat_message.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/promote_chat_member.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/restrict_chat_member.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/set_administrator_title.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/set_chat_description.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/set_chat_permissions.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/set_chat_photo.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/set_chat_protected_content.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/set_chat_title.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/set_chat_ttl.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/set_chat_ttl.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/set_chat_username.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/set_send_as_chat.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/set_slow_mode.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/unarchive_chats.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/unban_chat_member.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/unpin_all_chat_messages.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/chats/unpin_chat_message.py` & `pyrotgfork-2.1.24/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/contacts/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/contacts/add_contact.py` & `pyrotgfork-2.1.24/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/contacts/delete_contacts.py` & `pyrotgfork-2.1.24/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/contacts/get_contacts.py` & `pyrotgfork-2.1.24/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/contacts/get_contacts_count.py` & `pyrotgfork-2.1.24/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/contacts/import_contacts.py` & `pyrotgfork-2.1.24/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/on_callback_query.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/on_chat_join_request.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/on_chat_member_updated.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/on_chosen_inline_result.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/on_deleted_messages.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/on_disconnect.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/on_edited_message.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/on_inline_query.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/on_message.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/on_message_reaction_count_updated.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/on_message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/on_message_reaction_updated.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/on_message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/on_poll.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/on_raw_update.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/decorators/on_user_status.py` & `pyrotgfork-2.1.24/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/approve_chat_join_request.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/create_chat_invite_link.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/decline_chat_join_request.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/export_chat_invite_link.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/get_chat_invite_link.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/get_chat_join_requests.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `pyrotgfork-2.1.24/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/copy_media_group.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/copy_message.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/delete_messages.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/download_media.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/edit_inline_caption.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/edit_inline_media.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/edit_inline_reply_markup.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/edit_inline_text.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/edit_message_caption.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/edit_message_media.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/edit_message_reply_markup.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/edit_message_text.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/forward_messages.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/get_chat_history.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/get_chat_history_count.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/get_discussion_message.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/get_discussion_replies.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/get_discussion_replies_count.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/get_media_group.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/get_messages.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/inline_session.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/read_chat_history.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/retract_vote.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/search_global.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/search_global.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 class SearchGlobal:
     async def search_global(
         self: "pyrogram.Client",
         query: str = "",
         filter: "enums.MessagesFilter" = enums.MessagesFilter.EMPTY,
         limit: int = 0,
         chat_list: int = 0,
+        is_channel: bool = False,
     ) -> Optional[AsyncGenerator["types.Message", None]]:
         """Search messages globally from all of your chats.
 
         If you want to get the messages count only, see :meth:`~pyrogram.Client.search_global_count`.
 
         .. note::
 
@@ -55,14 +56,18 @@
             limit (``int``, *optional*):
                 Limits the number of messages to be retrieved.
                 By default, no limit is applied and all messages are returned.
 
             chat_list (``int``, *optional*):
                 Chat list in which to search messages; Only Main (0) and Archive (1) chat lists are supported. Defaults to (0) Main chat list.
 
+            is_channel (``bool``, *optional*):
+                True, if should search only in joined channels.
+                Defaults to False. All available chats are searched.
+
         Returns:
             ``Generator``: A generator yielding :obj:`~pyrogram.types.Message` objects.
 
         Example:
             .. code-block:: python
 
                 from pyrogram import enums
@@ -93,15 +98,16 @@
                         filter=filter.value(),
                         min_date=0,
                         max_date=0,
                         offset_rate=offset_date,
                         offset_peer=offset_peer,
                         offset_id=offset_id,
                         limit=limit,
-                        folder_id=chat_list
+                        folder_id=chat_list,
+                        broadcasts_only=is_channel
                     ),
                     sleep_threshold=60
                 ),
                 replies=0
             )
 
             if not messages:
```

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/search_global_count.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/search_global_count.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 class SearchGlobalCount:
     async def search_global_count(
         self: "pyrogram.Client",
         query: str = "",
         filter: "enums.MessagesFilter" = enums.MessagesFilter.EMPTY,
         chat_list: int = 0,
+        is_channel: bool = False,
     ) -> int:
         """Get the count of messages resulting from a global search.
 
         If you want to get the actual messages, see :meth:`~pyrogram.Client.search_global`.
 
         .. include:: /_includes/usable-by/users.rst
 
@@ -40,28 +41,33 @@
 
             filter (:obj:`~pyrogram.enums.MessagesFilter`, *optional*):
                 Pass a filter in order to search for specific kind of messages only:
 
             chat_list (``int``, *optional*):
                 Chat list in which to search messages; Only Main (0) and Archive (1) chat lists are supported. Defaults to (0) Main chat list.
 
+            is_channel (``bool``, *optional*):
+                True, if should search only in joined channels.
+                Defaults to False. All available chats are searched.
+
         Returns:
             ``int``: On success, the messages count is returned.
         """
         r = await self.invoke(
             raw.functions.messages.SearchGlobal(
                 q=query,
                 filter=filter.value(),
                 min_date=0,
                 max_date=0,
                 offset_rate=0,
                 offset_peer=raw.types.InputPeerEmpty(),
                 offset_id=0,
                 limit=1,
-                folder_id=chat_list
+                folder_id=chat_list,
+                broadcasts_only=is_channel
             )
         )
 
         if hasattr(r, "count"):
             return r.count
         else:
             return len(r.messages)
```

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/search_messages.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/search_messages_count.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_animation.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_audio.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_cached_media.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_chat_action.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_contact.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_dice.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_document.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_location.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_media_group.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_message.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_photo.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_poll.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_sticker.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_venue.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_video.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_video_note.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/send_voice.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/set_reaction.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/set_reaction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/stop_poll.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/stream_media.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/messages/vote_poll.py` & `pyrotgfork-2.1.24/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/password/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/password/change_cloud_password.py` & `pyrotgfork-2.1.24/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/password/enable_cloud_password.py` & `pyrotgfork-2.1.24/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/password/remove_cloud_password.py` & `pyrotgfork-2.1.24/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/stickers/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/stickers/get_stickers.py` & `pyrotgfork-2.1.24/pyrogram/methods/stickers/get_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/block_user.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/delete_profile_photos.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/get_chat_photos.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/get_chat_photos_count.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/get_common_chats.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/get_default_emoji_statuses.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/get_me.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/get_users.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/set_birthdate.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/set_birthdate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/set_emoji_status.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/set_personal_chat.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/set_personal_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/set_profile_photo.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/set_username.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/unblock_user.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/users/update_profile.py` & `pyrotgfork-2.1.24/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/utilities/__init__.py` & `pyrotgfork-2.1.24/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/utilities/add_handler.py` & `pyrotgfork-2.1.24/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/utilities/compose.py` & `pyrotgfork-2.1.24/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/utilities/export_session_string.py` & `pyrotgfork-2.1.24/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/utilities/idle.py` & `pyrotgfork-2.1.24/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/utilities/remove_handler.py` & `pyrotgfork-2.1.24/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/utilities/restart.py` & `pyrotgfork-2.1.24/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/utilities/run.py` & `pyrotgfork-2.1.24/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/utilities/start.py` & `pyrotgfork-2.1.24/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/utilities/stop.py` & `pyrotgfork-2.1.24/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/methods/utilities/stop_transmission.py` & `pyrotgfork-2.1.24/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/parser/__init__.py` & `pyrotgfork-2.1.24/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/parser/html.py` & `pyrotgfork-2.1.24/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/parser/markdown.py` & `pyrotgfork-2.1.24/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/parser/parser.py` & `pyrotgfork-2.1.24/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/parser/utils.py` & `pyrotgfork-2.1.24/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/__init__.py` & `pyrotgfork-2.1.24/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/__init__.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/future_salt.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/future_salts.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/gzip_packed.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/list.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/message.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/msg_container.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/tl_object.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/primitives/__init__.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/primitives/bool.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/primitives/bytes.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/primitives/double.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/primitives/int.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/primitives/string.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/raw/core/primitives/vector.py` & `pyrotgfork-2.1.24/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/session/__init__.py` & `pyrotgfork-2.1.24/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/session/auth.py` & `pyrotgfork-2.1.24/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/session/session.py` & `pyrotgfork-2.1.24/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/session/internals/__init__.py` & `pyrotgfork-2.1.24/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/session/internals/data_center.py` & `pyrotgfork-2.1.24/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/session/internals/msg_factory.py` & `pyrotgfork-2.1.24/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/session/internals/msg_id.py` & `pyrotgfork-2.1.24/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/session/internals/seq_no.py` & `pyrotgfork-2.1.24/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/storage/__init__.py` & `pyrotgfork-2.1.24/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/storage/aio_sqlite_storage.py` & `pyrotgfork-2.1.24/pyrogram/storage/aio_sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/storage/file_storage.py` & `pyrotgfork-2.1.24/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/storage/memory_storage.py` & `pyrotgfork-2.1.24/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/storage/sqlite_storage.py` & `pyrotgfork-2.1.24/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/storage/storage.py` & `pyrotgfork-2.1.24/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/__init__.py` & `pyrotgfork-2.1.24/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/list.py` & `pyrotgfork-2.1.24/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/object.py` & `pyrotgfork-2.1.24/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/update.py` & `pyrotgfork-2.1.24/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/authorization/__init__.py` & `pyrotgfork-2.1.24/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/authorization/sent_code.py` & `pyrotgfork-2.1.24/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/authorization/terms_of_service.py` & `pyrotgfork-2.1.24/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/__init__.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/callback_game.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/callback_query.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/force_reply.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/game_high_score.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/login_url.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/menu_button.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/bots_and_keyboards/web_app_info.py` & `pyrotgfork-2.1.24/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/business/__init__.py` & `pyrotgfork-2.1.24/pyrogram/types/business/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/business/business_connection.py` & `pyrotgfork-2.1.24/pyrogram/types/business/business_connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/business/business_intro.py` & `pyrotgfork-2.1.24/pyrogram/types/business/business_intro.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/business/business_location.py` & `pyrotgfork-2.1.24/pyrogram/types/business/business_location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/business/business_opening_hours.py` & `pyrotgfork-2.1.24/pyrogram/types/business/business_opening_hours.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/business/business_opening_hours_interval.py` & `pyrotgfork-2.1.24/pyrogram/types/business/business_opening_hours_interval.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/chat_topics/__init__.py` & `pyrotgfork-2.1.24/pyrogram/types/chat_topics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/chat_topics/forum_topic.py` & `pyrotgfork-2.1.24/pyrogram/types/chat_topics/forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/chat_topics/forum_topic_closed.py` & `pyrotgfork-2.1.24/pyrogram/types/chat_topics/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/chat_topics/forum_topic_created.py` & `pyrotgfork-2.1.24/pyrogram/types/chat_topics/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/chat_topics/forum_topic_edited.py` & `pyrotgfork-2.1.24/pyrogram/types/chat_topics/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/chat_topics/forum_topic_reopened.py` & `pyrotgfork-2.1.24/pyrogram/types/chat_topics/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/chat_topics/general_forum_topic_hidden.py` & `pyrotgfork-2.1.24/pyrogram/types/chat_topics/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/chat_topics/general_forum_topic_unhidden.py` & `pyrotgfork-2.1.24/pyrogram/types/chat_topics/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/__init__.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/chosen_inline_result.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_animation.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_article.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_audio.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_contact.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_document.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_location.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_photo.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_venue.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_video.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/inline_mode/inline_query_result_voice.py` & `pyrotgfork-2.1.24/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/input_media/__init__.py` & `pyrotgfork-2.1.24/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/input_media/input_media.py` & `pyrotgfork-2.1.24/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/input_media/input_media_animation.py` & `pyrotgfork-2.1.24/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/input_media/input_media_audio.py` & `pyrotgfork-2.1.24/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/input_media/input_media_document.py` & `pyrotgfork-2.1.24/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/input_media/input_media_photo.py` & `pyrotgfork-2.1.24/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/input_media/input_media_video.py` & `pyrotgfork-2.1.24/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/input_media/input_phone_contact.py` & `pyrotgfork-2.1.24/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/input_media/link_preview_options.py` & `pyrotgfork-2.1.24/pyrogram/types/input_media/link_preview_options.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/input_message_content/__init__.py` & `pyrotgfork-2.1.24/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/input_message_content/external_reply_info.py` & `pyrotgfork-2.1.24/pyrogram/types/input_message_content/external_reply_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/input_message_content/input_message_content.py` & `pyrotgfork-2.1.24/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/input_message_content/input_text_message_content.py` & `pyrotgfork-2.1.24/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/input_message_content/reply_parameters.py` & `pyrotgfork-2.1.24/pyrogram/types/input_message_content/reply_parameters.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/message_origin/__init__.py` & `pyrotgfork-2.1.24/pyrogram/types/message_origin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/message_origin/message_import_info.py` & `pyrotgfork-2.1.24/pyrogram/types/message_origin/message_import_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/message_origin/message_origin.py` & `pyrotgfork-2.1.24/pyrogram/types/message_origin/message_origin.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/message_origin/message_origin_channel.py` & `pyrotgfork-2.1.24/pyrogram/types/message_origin/message_origin_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/message_origin/message_origin_chat.py` & `pyrotgfork-2.1.24/pyrogram/types/message_origin/message_origin_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/message_origin/message_origin_hidden_user.py` & `pyrotgfork-2.1.24/pyrogram/types/message_origin/message_origin_hidden_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/message_origin/message_origin_user.py` & `pyrotgfork-2.1.24/pyrogram/types/message_origin/message_origin_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/__init__.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/animation.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/audio.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/chat_boost_added.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/chat_boost_added.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/contact.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/dice.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/document.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/game.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/gift_code.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/gift_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/gifted_premium.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/gifted_premium.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/giveaway.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/giveaway.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/giveaway_completed.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/giveaway_completed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/giveaway_winners.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/giveaway_winners.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/location.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/message.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/message_entity.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/message_reaction_count_updated.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/message_reaction_updated.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/message_reactions.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/photo.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/poll.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/poll_option.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/reaction.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/sticker.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/story.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/story.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/thumbnail.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/venue.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/video.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/video_note.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/voice.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/web_app_data.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/messages_and_media/web_page.py` & `pyrotgfork-2.1.24/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/__init__.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/birthdate.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/birthdate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 
         business_opening_hours (:obj:`~pyrogram.types.BusinessOpeningHours`, *optional*):
             For private chats with business accounts, the opening hours of the business.
 
         personal_chat (:obj:`~pyrogram.types.Chat`, *optional*):
             For private chats, the personal channel of the user.
 
+        personal_chat_message (:obj:`~pyrogram.types.Message`, *optional*):
+            **TEMPORARY**: For private chats, the personal message_id in the ``personal_chat``.
+
         available_reactions (:obj:`~pyrogram.types.ChatReactions`, *optional*):
             Available reactions in the chat.
             Returned only in :meth:`~pyrogram.Client.get_chat`.
 
         accent_color (:obj:`~pyrogram.types.ChatColor`, *optional*):
             Chat accent color.
 
@@ -305,14 +308,15 @@
         self.slowmode_next_send_date = slowmode_next_send_date
         self.is_forum = is_forum
         self.unrestrict_boost_count = unrestrict_boost_count
         self.is_public = is_public
         self.join_by_request = join_by_request
         self.is_peak_preview = is_peak_preview
         self.personal_chat = personal_chat
+        self.personal_chat_message = personal_chat_message
         self.birthdate = birthdate
         self.business_intro = business_intro
         self.business_location = business_location
         self.business_opening_hours = business_opening_hours
         self.active_usernames = active_usernames
         self._raw = _raw
 
@@ -474,26 +478,33 @@
 
     @staticmethod
     async def _parse_full(client, chat_full: Union[raw.types.messages.ChatFull, raw.types.users.UserFull]) -> "Chat":
         users = {u.id: u for u in chat_full.users}
         chats = {c.id: c for c in chat_full.chats}
 
         personal_chat = None
+        personal_chat_message = None
 
         if isinstance(chat_full, raw.types.users.UserFull):
             full_user = chat_full.full_user
 
             parsed_chat = Chat._parse_user_chat(client, users[full_user.id])
             parsed_chat.bio = full_user.about
 
             if getattr(full_user, "personal_channel_id", None):
                 personal_chat = Chat._parse_channel_chat(
                     client,
                     chats[full_user.personal_channel_id]
                 )
+            # TODO:?|
+            if getattr(full_user, "personal_channel_message", None):
+                personal_chat_message = types.Message(
+                    client=client,
+                    id=full_user.personal_channel_message
+                )
 
             if full_user.pinned_msg_id:
                 try:
                     parsed_chat.pinned_message = await client.get_messages(
                         chat_id=parsed_chat.id,
                         message_ids=full_user.pinned_msg_id
                     )
@@ -588,18 +599,20 @@
                     )
 
             if isinstance(full_chat.exported_invite, raw.types.ChatInviteExported):
                 parsed_chat.invite_link = full_chat.exported_invite.link
 
             parsed_chat.available_reactions = types.ChatReactions._parse(
                 client,
-                full_chat.available_reactions
+                full_chat.available_reactions,
+                reactions_limit=getattr(full_chat, "reactions_limit", None)
             )
 
         parsed_chat.personal_chat = personal_chat
+        parsed_chat.personal_chat_message = personal_chat_message
         parsed_chat._raw = chat_full
 
         return parsed_chat
 
     @staticmethod
     def _parse_chat(client, chat: Union[raw.types.Chat, raw.types.User, raw.types.Channel]) -> "Chat":
         if isinstance(chat, raw.types.Chat):
```

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_color.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_event.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_event_filter.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_invite_link.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_join_request.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_joiner.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_member.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_member_updated.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_permissions.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_photo.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_privileges.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_reactions.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,45 +30,52 @@
         all_are_enabled (``bool``, *optional*)
 
         allow_custom_emoji (``bool``, *optional*):
             Whether custom emoji are allowed or not.
 
         reactions (List of :obj:`~pyrogram.types.Reaction`, *optional*):
             Reactions available.
+        
+        limit (``int``, *optional*):
+            Limit of the number of different unique reactions that can be added to a message, including already published ones. Can have values between 1 and 11. Defaults to 11, if not specified. Only applicable for :obj:`~pyrogram.enums.ChatType.CHANNEL`.
     """
 
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
         all_are_enabled: Optional[bool] = None,
         allow_custom_emoji: Optional[bool] = None,
         reactions: Optional[List["types.Reaction"]] = None,
+        limit: int = 11,
     ):
         super().__init__(client)
 
         self.all_are_enabled = all_are_enabled
         self.allow_custom_emoji = allow_custom_emoji
         self.reactions = reactions
+        self.limit = limit
 
     @staticmethod
-    def _parse(client, chat_reactions: "raw.base.ChatReactions") -> Optional["ChatReactions"]:
+    def _parse(client, chat_reactions: "raw.base.ChatReactions", reactions_limit: int = 11) -> Optional["ChatReactions"]:
         if isinstance(chat_reactions, raw.types.ChatReactionsAll):
             return ChatReactions(
                 client=client,
                 all_are_enabled=True,
-                allow_custom_emoji=chat_reactions.allow_custom
+                allow_custom_emoji=chat_reactions.allow_custom,
+                limit=reactions_limit
             )
 
         if isinstance(chat_reactions, raw.types.ChatReactionsSome):
             return ChatReactions(
                 client=client,
                 reactions=[
                     types.ReactionType._parse(client, reaction)
                     for reaction in chat_reactions.reactions
-                ]
+                ],
+                limit=reactions_limit
             )
 
         if isinstance(chat_reactions, raw.types.ChatReactionsNone):
             return None
 
         return None
```

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/chat_shared.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/chat_shared.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/dialog.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/emoji_status.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/invite_link_importer.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/restriction.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/user.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/username.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/users_shared.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/users_shared.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/video_chat_ended.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/video_chat_participants_invited.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/video_chat_participants_invited.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyrogram/types/user_and_chats/video_chat_started.py` & `pyrotgfork-2.1.24/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/.gitignore` & `pyrotgfork-2.1.24/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/COPYING` & `pyrotgfork-2.1.24/COPYING`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/COPYING.lesser` & `pyrotgfork-2.1.24/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/NOTICE` & `pyrotgfork-2.1.24/NOTICE`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/README.md` & `pyrotgfork-2.1.24/README.md`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/hatch_build.py` & `pyrotgfork-2.1.24/hatch_build.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/pyproject.toml` & `pyrotgfork-2.1.24/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.23/PKG-INFO` & `pyrotgfork-2.1.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyrotgfork
-Version: 2.1.23
+Version: 2.1.24
 Summary: Fork of Pyrogram. Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Project-URL: Homepage, https://telegramplayground.github.io/pyrogram/releases/
 Project-URL: Tracker, https://github.com/TelegramPlayGround/Pyrogram/issues
 Project-URL: Community, https://t.me/PyroTGFork
 Project-URL: Source, https://github.com/TelegramPlayGround/Pyrogram
 Project-URL: Documentation, https://telegramplayground.github.io/pyrogram/
 Author-email: SpEcHIDe <pyrogram@iamidiotareyoutoo.com>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: pyrotgfork Version: 2.1.23 Summary: Fork of
+Metadata-Version: 2.3 Name: pyrotgfork Version: 2.1.24 Summary: Fork of
 Pyrogram. Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Project-URL: Homepage, https://
 telegramplayground.github.io/pyrogram/releases/ Project-URL: Tracker, https://
 github.com/TelegramPlayGround/Pyrogram/issues Project-URL: Community, https://
 t.me/PyroTGFork Project-URL: Source, https://github.com/TelegramPlayGround/
 Pyrogram Project-URL: Documentation, https://telegramplayground.github.io/
 pyrogram/ Author-email: SpEcHIDe
```

