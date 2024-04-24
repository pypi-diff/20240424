# Comparing `tmp/open_interpreter-0.2.4.tar.gz` & `tmp/open_interpreter-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.2.4.tar", max compression
+gzip compressed data, was "open_interpreter-0.2.5.tar", max compression
```

## Comparing `open_interpreter-0.2.4.tar` & `open_interpreter-0.2.5.tar`

### file list

```diff
@@ -1,115 +1,105 @@
--rw-r--r--   0        0        0    33813 2023-12-01 04:54:45.541108 open_interpreter-0.2.4/LICENSE
--rw-r--r--   0        0        0    13204 2024-03-21 19:18:14.111032 open_interpreter-0.2.4/README.md
--rw-r--r--   0        0        0      633 2024-03-10 03:34:39.801216 open_interpreter-0.2.4/interpreter/__init__.py
--rw-r--r--   0        0        0     2820 2024-01-26 04:00:30.851366 open_interpreter-0.2.4/interpreter/core/ARCHIVE_extend_system_message.py
--rw-r--r--   0        0        0     1293 2024-01-02 00:53:21.768004 open_interpreter-0.2.4/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
--rw-r--r--   0        0        0     3138 2023-12-28 08:17:40.566266 open_interpreter-0.2.4/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
--rw-r--r--   0        0        0        0 2023-09-23 02:28:30.998293 open_interpreter-0.2.4/interpreter/core/ARCHIVE_rag/__init__.py
--rw-r--r--   0        0        0        0 2023-09-23 02:28:30.996698 open_interpreter-0.2.4/interpreter/core/__init__.py
--rw-r--r--   0        0        0        0 2023-12-10 04:34:15.003063 open_interpreter-0.2.4/interpreter/core/computer/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 06:12:00.162775 open_interpreter-0.2.4/interpreter/core/computer/ai/__init__.py
--rw-r--r--   0        0        0     5688 2024-02-23 17:05:07.439829 open_interpreter-0.2.4/interpreter/core/computer/ai/ai.py
--rw-r--r--   0        0        0        0 2024-01-26 09:19:12.776957 open_interpreter-0.2.4/interpreter/core/computer/browser/__init__.py
--rw-r--r--   0        0        0      416 2024-03-11 23:06:39.793968 open_interpreter-0.2.4/interpreter/core/computer/browser/browser.py
--rw-r--r--   0        0        0        0 2024-03-09 23:13:07.737048 open_interpreter-0.2.4/interpreter/core/computer/calendar/__init__.py
--rw-r--r--   0        0        0    13006 2024-03-19 02:56:22.058086 open_interpreter-0.2.4/interpreter/core/computer/calendar/calendar.py
--rw-r--r--   0        0        0        0 2023-12-10 22:45:24.479631 open_interpreter-0.2.4/interpreter/core/computer/clipboard/__init__.py
--rw-r--r--   0        0        0      879 2024-02-17 09:50:43.570212 open_interpreter-0.2.4/interpreter/core/computer/clipboard/clipboard.py
--rw-r--r--   0        0        0     2917 2024-03-24 07:07:37.046332 open_interpreter-0.2.4/interpreter/core/computer/computer.py
--rw-r--r--   0        0        0        0 2024-03-09 23:13:07.739073 open_interpreter-0.2.4/interpreter/core/computer/contacts/__init__.py
--rw-r--r--   0        0        0     3293 2024-03-12 06:06:38.617061 open_interpreter-0.2.4/interpreter/core/computer/contacts/contacts.py
--rw-r--r--   0        0        0        0 2023-12-10 05:08:49.684549 open_interpreter-0.2.4/interpreter/core/computer/display/__init__.py
--rw-r--r--   0        0        0    10556 2024-03-12 08:30:48.912183 open_interpreter-0.2.4/interpreter/core/computer/display/display.py
--rw-r--r--   0        0        0    26182 2024-03-11 23:06:40.051135 open_interpreter-0.2.4/interpreter/core/computer/display/point/point.py
--rw-r--r--   0        0        0        0 2024-02-08 19:38:14.852311 open_interpreter-0.2.4/interpreter/core/computer/docs/__init__.py
--rw-r--r--   0        0        0      749 2024-02-19 04:03:05.979003 open_interpreter-0.2.4/interpreter/core/computer/docs/docs.py
--rw-r--r--   0        0        0        0 2024-01-26 09:19:05.454871 open_interpreter-0.2.4/interpreter/core/computer/files/__init__.py
--rw-r--r--   0        0        0     1698 2024-02-17 09:50:43.572183 open_interpreter-0.2.4/interpreter/core/computer/files/files.py
--rw-r--r--   0        0        0        0 2023-12-10 04:31:00.631851 open_interpreter-0.2.4/interpreter/core/computer/keyboard/__init__.py
--rw-r--r--   0        0        0     3553 2024-02-17 09:50:43.572720 open_interpreter-0.2.4/interpreter/core/computer/keyboard/keyboard.py
--rw-r--r--   0        0        0        0 2024-03-09 23:13:07.739526 open_interpreter-0.2.4/interpreter/core/computer/mail/__init__.py
--rw-r--r--   0        0        0     6350 2024-03-12 09:21:27.712324 open_interpreter-0.2.4/interpreter/core/computer/mail/mail.py
--rw-r--r--   0        0        0        0 2023-12-10 04:31:04.410095 open_interpreter-0.2.4/interpreter/core/computer/mouse/__init__.py
--rw-r--r--   0        0        0    12423 2024-03-11 01:22:58.718724 open_interpreter-0.2.4/interpreter/core/computer/mouse/mouse.py
--rw-r--r--   0        0        0        0 2023-12-19 20:14:08.928003 open_interpreter-0.2.4/interpreter/core/computer/os/__init__.py
--rw-r--r--   0        0        0     2955 2024-02-17 09:50:43.573672 open_interpreter-0.2.4/interpreter/core/computer/os/os.py
--rw-r--r--   0        0        0     5932 2024-03-24 07:07:31.433103 open_interpreter-0.2.4/interpreter/core/computer/skills/skills.py
--rw-r--r--   0        0        0        0 2024-03-09 23:13:07.739864 open_interpreter-0.2.4/interpreter/core/computer/sms/__init__.py
--rw-r--r--   0        0        0     1399 2024-03-12 06:06:38.617738 open_interpreter-0.2.4/interpreter/core/computer/sms/sms.py
--rw-r--r--   0        0        0        0 2023-12-10 04:30:55.768473 open_interpreter-0.2.4/interpreter/core/computer/terminal/__init__.py
--rw-r--r--   0        0        0     1090 2024-01-07 07:39:34.135356 open_interpreter-0.2.4/interpreter/core/computer/terminal/base_language.py
--rw-r--r--   0        0        0     5164 2023-12-17 10:57:48.454324 open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
--rw-r--r--   0        0        0        0 2023-12-01 04:54:45.543496 open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/__init__.py
--rw-r--r--   0        0        0     1812 2023-12-10 07:26:58.734679 open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/applescript.py
--rw-r--r--   0        0        0      858 2023-12-10 06:51:28.978069 open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/html.py
--rw-r--r--   0        0        0     1924 2024-01-05 02:01:12.636229 open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/javascript.py
--rw-r--r--   0        0        0    15287 2024-03-13 10:19:01.356805 open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/jupyter_language.py
--rw-r--r--   0        0        0     2193 2023-12-10 06:51:18.120564 open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/powershell.py
--rw-r--r--   0        0        0      293 2023-12-28 08:24:31.936959 open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/python.py
--rw-r--r--   0        0        0     2360 2023-12-10 06:51:21.914617 open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/r.py
--rw-r--r--   0        0        0     2503 2024-03-10 04:38:00.386717 open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/react.py
--rw-r--r--   0        0        0     2727 2023-12-10 19:56:47.221058 open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/shell.py
--rw-r--r--   0        0        0     6715 2023-12-28 08:17:40.478532 open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/subprocess_language.py
--rw-r--r--   0        0        0     4946 2024-03-13 09:42:35.656561 open_interpreter-0.2.4/interpreter/core/computer/terminal/terminal.py
--rw-r--r--   0        0        0     7097 2024-03-10 10:24:40.130329 open_interpreter-0.2.4/interpreter/core/computer/utils/computer_vision.py
--rw-r--r--   0        0        0     1479 2024-01-03 12:15:42.013393 open_interpreter-0.2.4/interpreter/core/computer/utils/get_active_window.py
--rw-r--r--   0        0        0      929 2023-12-19 21:39:53.013384 open_interpreter-0.2.4/interpreter/core/computer/utils/html_to_png_base64.py
--rw-r--r--   0        0        0      396 2024-01-02 01:05:06.051382 open_interpreter-0.2.4/interpreter/core/computer/utils/recipient_utils.py
--rw-r--r--   0        0        0     1053 2024-03-19 02:56:22.059193 open_interpreter-0.2.4/interpreter/core/computer/utils/run_applescript.py
--rw-r--r--   0        0        0    14511 2024-03-24 06:46:26.831243 open_interpreter-0.2.4/interpreter/core/core.py
--rw-r--r--   0        0        0     3282 2024-03-19 02:56:22.060207 open_interpreter-0.2.4/interpreter/core/default_system_message.py
--rw-r--r--   0        0        0        0 2023-09-23 02:28:30.997182 open_interpreter-0.2.4/interpreter/core/llm/__init__.py
--rw-r--r--   0        0        0     8675 2024-03-20 04:09:09.112595 open_interpreter-0.2.4/interpreter/core/llm/llm.py
--rw-r--r--   0        0        0     5052 2024-03-12 01:23:40.325749 open_interpreter-0.2.4/interpreter/core/llm/run_function_calling_llm.py
--rw-r--r--   0        0        0     2616 2024-01-02 01:05:06.084251 open_interpreter-0.2.4/interpreter/core/llm/run_text_llm.py
--rw-r--r--   0        0        0     8677 2024-03-13 10:30:39.799436 open_interpreter-0.2.4/interpreter/core/llm/utils/convert_to_openai_messages.py
--rw-r--r--   0        0        0      711 2024-01-18 07:07:05.653072 open_interpreter-0.2.4/interpreter/core/llm/utils/merge_deltas.py
--rw-r--r--   0        0        0     1800 2024-01-14 06:05:45.235518 open_interpreter-0.2.4/interpreter/core/llm/utils/parse_partial_json.py
--rw-r--r--   0        0        0      538 2024-03-07 18:53:17.146944 open_interpreter-0.2.4/interpreter/core/llm/vision_for_text_llms.py
--rw-r--r--   0        0        0     1688 2024-03-13 10:27:27.941493 open_interpreter-0.2.4/interpreter/core/render_message.py
--rw-r--r--   0        0        0    13763 2024-03-20 04:09:09.113006 open_interpreter-0.2.4/interpreter/core/respond.py
--rw-r--r--   0        0        0     6162 2024-01-31 07:55:31.444394 open_interpreter-0.2.4/interpreter/core/server.py
--rw-r--r--   0        0        0      630 2023-11-05 01:31:54.681649 open_interpreter-0.2.4/interpreter/core/utils/ARCHIVE_embed.py
--rw-r--r--   0        0        0      360 2024-01-26 04:00:21.014189 open_interpreter-0.2.4/interpreter/core/utils/ARCHIVE_get_user_info_string.py
--rw-r--r--   0        0        0     1096 2023-11-05 01:29:01.227904 open_interpreter-0.2.4/interpreter/core/utils/ARCHIVE_vector_search.py
--rw-r--r--   0        0        0        0 2023-09-23 02:28:31.002568 open_interpreter-0.2.4/interpreter/core/utils/__init__.py
--rw-r--r--   0        0        0      920 2024-02-17 09:50:43.576535 open_interpreter-0.2.4/interpreter/core/utils/lazy_import.py
--rw-r--r--   0        0        0     2118 2023-12-28 08:17:40.528813 open_interpreter-0.2.4/interpreter/core/utils/scan_code.py
--rw-r--r--   0        0        0     4404 2024-01-07 07:39:34.178302 open_interpreter-0.2.4/interpreter/core/utils/system_debug_info.py
--rw-r--r--   0        0        0     1736 2024-01-15 01:25:05.923499 open_interpreter-0.2.4/interpreter/core/utils/telemetry.py
--rw-r--r--   0        0        0     1098 2023-09-28 20:53:00.949736 open_interpreter-0.2.4/interpreter/core/utils/temporary_file.py
--rw-r--r--   0        0        0      510 2023-11-01 04:34:50.868691 open_interpreter-0.2.4/interpreter/core/utils/truncate_output.py
--rw-r--r--   0        0        0     2421 2024-01-26 01:37:35.706247 open_interpreter-0.2.4/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py
--rw-r--r--   0        0        0        0 2023-09-23 02:28:30.998571 open_interpreter-0.2.4/interpreter/terminal_interface/__init__.py
--rw-r--r--   0        0        0      611 2023-11-01 04:34:50.864816 open_interpreter-0.2.4/interpreter/terminal_interface/components/base_block.py
--rw-r--r--   0        0        0     2664 2024-01-27 04:54:05.332821 open_interpreter-0.2.4/interpreter/terminal_interface/components/code_block.py
--rw-r--r--   0        0        0     1386 2023-12-13 08:26:44.851269 open_interpreter-0.2.4/interpreter/terminal_interface/components/message_block.py
--rw-r--r--   0        0        0     2905 2024-02-17 09:50:43.577169 open_interpreter-0.2.4/interpreter/terminal_interface/conversation_navigator.py
--rw-r--r--   0        0        0    10580 2024-02-17 09:50:43.577608 open_interpreter-0.2.4/interpreter/terminal_interface/magic_commands.py
--rw-r--r--   0        0        0    14744 2024-03-19 02:56:22.060994 open_interpreter-0.2.4/interpreter/terminal_interface/profiles/defaults/01.py
--rw-r--r--   0        0        0      974 2024-03-08 04:29:05.658173 open_interpreter-0.2.4/interpreter/terminal_interface/profiles/defaults/default.yaml
--rw-r--r--   0        0        0     1287 2024-03-08 04:29:05.658598 open_interpreter-0.2.4/interpreter/terminal_interface/profiles/defaults/fast.yaml
--rw-r--r--   0        0        0    14587 2024-03-20 04:09:09.113696 open_interpreter-0.2.4/interpreter/terminal_interface/profiles/defaults/local.py
--rw-r--r--   0        0        0    10838 2024-03-12 04:55:33.650157 open_interpreter-0.2.4/interpreter/terminal_interface/profiles/defaults/os.py
--rw-r--r--   0        0        0     1198 2024-03-08 04:29:05.659492 open_interpreter-0.2.4/interpreter/terminal_interface/profiles/defaults/vision.yaml
--rw-r--r--   0        0        0       25 2024-01-26 03:07:17.828725 open_interpreter-0.2.4/interpreter/terminal_interface/profiles/historical_profiles.py
--rw-r--r--   0        0        0    40464 2024-03-20 04:09:09.114385 open_interpreter-0.2.4/interpreter/terminal_interface/profiles/profiles.py
--rw-r--r--   0        0        0     2304 2024-01-31 01:14:13.686159 open_interpreter-0.2.4/interpreter/terminal_interface/render_past_conversation.py
--rw-r--r--   0        0        0    15772 2024-03-24 07:43:13.359394 open_interpreter-0.2.4/interpreter/terminal_interface/start_terminal_interface.py
--rw-r--r--   0        0        0    20287 2024-03-07 11:14:28.680622 open_interpreter-0.2.4/interpreter/terminal_interface/terminal_interface.py
--rw-r--r--   0        0        0    25763 2024-01-26 01:37:36.016594 open_interpreter-0.2.4/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
--rw-r--r--   0        0        0     3099 2024-01-26 03:59:56.254993 open_interpreter-0.2.4/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
--rw-r--r--   0        0        0      512 2023-11-20 05:25:30.624843 open_interpreter-0.2.4/interpreter/terminal_interface/utils/check_for_package.py
--rw-r--r--   0        0        0      481 2023-11-05 01:34:27.337773 open_interpreter-0.2.4/interpreter/terminal_interface/utils/check_for_update.py
--rw-r--r--   0        0        0      419 2024-03-07 11:14:28.681094 open_interpreter-0.2.4/interpreter/terminal_interface/utils/cli_input.py
--rw-r--r--   0        0        0     1939 2024-01-03 12:15:41.692984 open_interpreter-0.2.4/interpreter/terminal_interface/utils/count_tokens.py
--rw-r--r--   0        0        0      884 2024-01-25 21:39:42.258551 open_interpreter-0.2.4/interpreter/terminal_interface/utils/display_markdown_message.py
--rw-r--r--   0        0        0     3069 2024-01-13 20:23:21.041610 open_interpreter-0.2.4/interpreter/terminal_interface/utils/display_output.py
--rw-r--r--   0        0        0      459 2023-11-11 08:24:50.947604 open_interpreter-0.2.4/interpreter/terminal_interface/utils/find_image_path.py
--rw-r--r--   0        0        0      250 2023-11-20 05:25:42.539104 open_interpreter-0.2.4/interpreter/terminal_interface/utils/get_conversations.py
--rw-r--r--   0        0        0      184 2023-12-05 07:45:32.479315 open_interpreter-0.2.4/interpreter/terminal_interface/utils/in_jupyter_notebook.py
--rw-r--r--   0        0        0      316 2024-03-08 04:29:05.661476 open_interpreter-0.2.4/interpreter/terminal_interface/utils/local_storage_path.py
--rw-r--r--   0        0        0       79 2024-03-08 04:29:05.662377 open_interpreter-0.2.4/interpreter/terminal_interface/utils/oi_dir.py
--rw-r--r--   0        0        0     2914 2024-03-20 04:09:09.115471 open_interpreter-0.2.4/interpreter/terminal_interface/validate_llm_settings.py
--rw-r--r--   0        0        0     2233 2024-03-24 07:46:33.716127 open_interpreter-0.2.4/pyproject.toml
--rw-r--r--   0        0        0    15427 1970-01-01 00:00:00.000000 open_interpreter-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    33813 2023-12-01 04:54:45.541108 open_interpreter-0.2.5/LICENSE
+-rw-r--r--   0        0        0    14202 2024-04-24 00:28:27.703962 open_interpreter-0.2.5/README.md
+-rw-r--r--   0        0        0      633 2024-03-10 03:34:39.801216 open_interpreter-0.2.5/interpreter/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-23 02:28:30.996698 open_interpreter-0.2.5/interpreter/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-10 04:34:15.003063 open_interpreter-0.2.5/interpreter/core/computer/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 06:12:00.162775 open_interpreter-0.2.5/interpreter/core/computer/ai/__init__.py
+-rw-r--r--   0        0        0     5688 2024-02-23 17:05:07.439829 open_interpreter-0.2.5/interpreter/core/computer/ai/ai.py
+-rw-r--r--   0        0        0        0 2024-01-26 09:19:12.776957 open_interpreter-0.2.5/interpreter/core/computer/browser/__init__.py
+-rw-r--r--   0        0        0      416 2024-03-11 23:06:39.793968 open_interpreter-0.2.5/interpreter/core/computer/browser/browser.py
+-rw-r--r--   0        0        0        0 2024-03-09 23:13:07.737048 open_interpreter-0.2.5/interpreter/core/computer/calendar/__init__.py
+-rw-r--r--   0        0        0    12989 2024-04-17 01:29:13.076979 open_interpreter-0.2.5/interpreter/core/computer/calendar/calendar.py
+-rw-r--r--   0        0        0        0 2023-12-10 22:45:24.479631 open_interpreter-0.2.5/interpreter/core/computer/clipboard/__init__.py
+-rw-r--r--   0        0        0      879 2024-02-17 09:50:43.570212 open_interpreter-0.2.5/interpreter/core/computer/clipboard/clipboard.py
+-rw-r--r--   0        0        0     2995 2024-04-12 01:34:49.648220 open_interpreter-0.2.5/interpreter/core/computer/computer.py
+-rw-r--r--   0        0        0        0 2024-03-09 23:13:07.739073 open_interpreter-0.2.5/interpreter/core/computer/contacts/__init__.py
+-rw-r--r--   0        0        0     3293 2024-03-12 06:06:38.617061 open_interpreter-0.2.5/interpreter/core/computer/contacts/contacts.py
+-rw-r--r--   0        0        0        0 2023-12-10 05:08:49.684549 open_interpreter-0.2.5/interpreter/core/computer/display/__init__.py
+-rw-r--r--   0        0        0    14468 2024-04-17 01:29:13.077750 open_interpreter-0.2.5/interpreter/core/computer/display/display.py
+-rw-r--r--   0        0        0    26276 2024-04-03 20:16:49.361329 open_interpreter-0.2.5/interpreter/core/computer/display/point/point.py
+-rw-r--r--   0        0        0        0 2024-02-08 19:38:14.852311 open_interpreter-0.2.5/interpreter/core/computer/docs/__init__.py
+-rw-r--r--   0        0        0      749 2024-02-19 04:03:05.979003 open_interpreter-0.2.5/interpreter/core/computer/docs/docs.py
+-rw-r--r--   0        0        0        0 2024-01-26 09:19:05.454871 open_interpreter-0.2.5/interpreter/core/computer/files/__init__.py
+-rw-r--r--   0        0        0     1698 2024-02-17 09:50:43.572183 open_interpreter-0.2.5/interpreter/core/computer/files/files.py
+-rw-r--r--   0        0        0        0 2023-12-10 04:31:00.631851 open_interpreter-0.2.5/interpreter/core/computer/keyboard/__init__.py
+-rw-r--r--   0        0        0     3553 2024-02-17 09:50:43.572720 open_interpreter-0.2.5/interpreter/core/computer/keyboard/keyboard.py
+-rw-r--r--   0        0        0        0 2024-03-09 23:13:07.739526 open_interpreter-0.2.5/interpreter/core/computer/mail/__init__.py
+-rw-r--r--   0        0        0     6350 2024-03-12 09:21:27.712324 open_interpreter-0.2.5/interpreter/core/computer/mail/mail.py
+-rw-r--r--   0        0        0        0 2023-12-10 04:31:04.410095 open_interpreter-0.2.5/interpreter/core/computer/mouse/__init__.py
+-rw-r--r--   0        0        0    12423 2024-03-11 01:22:58.718724 open_interpreter-0.2.5/interpreter/core/computer/mouse/mouse.py
+-rw-r--r--   0        0        0        0 2023-12-19 20:14:08.928003 open_interpreter-0.2.5/interpreter/core/computer/os/__init__.py
+-rw-r--r--   0        0        0     2955 2024-02-17 09:50:43.573672 open_interpreter-0.2.5/interpreter/core/computer/os/os.py
+-rw-r--r--   0        0        0     5894 2024-04-03 20:16:49.361530 open_interpreter-0.2.5/interpreter/core/computer/skills/skills.py
+-rw-r--r--   0        0        0        0 2024-03-09 23:13:07.739864 open_interpreter-0.2.5/interpreter/core/computer/sms/__init__.py
+-rw-r--r--   0        0        0     1399 2024-03-12 06:06:38.617738 open_interpreter-0.2.5/interpreter/core/computer/sms/sms.py
+-rw-r--r--   0        0        0        0 2023-12-10 04:30:55.768473 open_interpreter-0.2.5/interpreter/core/computer/terminal/__init__.py
+-rw-r--r--   0        0        0     1090 2024-01-07 07:39:34.135356 open_interpreter-0.2.5/interpreter/core/computer/terminal/base_language.py
+-rw-r--r--   0        0        0        0 2023-12-01 04:54:45.543496 open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/__init__.py
+-rw-r--r--   0        0        0     1812 2023-12-10 07:26:58.734679 open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/applescript.py
+-rw-r--r--   0        0        0      858 2023-12-10 06:51:28.978069 open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/html.py
+-rw-r--r--   0        0        0     1924 2024-01-05 02:01:12.636229 open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/javascript.py
+-rw-r--r--   0        0        0    15335 2024-04-12 01:34:49.648992 open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/jupyter_language.py
+-rw-r--r--   0        0        0     2193 2023-12-10 06:51:18.120564 open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/powershell.py
+-rw-r--r--   0        0        0      293 2023-12-28 08:24:31.936959 open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/python.py
+-rw-r--r--   0        0        0     2360 2023-12-10 06:51:21.914617 open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/r.py
+-rw-r--r--   0        0        0     2503 2024-03-10 04:38:00.386717 open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/react.py
+-rw-r--r--   0        0        0     1773 2024-04-03 20:16:49.362144 open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/ruby.py
+-rw-r--r--   0        0        0     2727 2023-12-10 19:56:47.221058 open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/shell.py
+-rw-r--r--   0        0        0     6715 2023-12-28 08:17:40.478532 open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/subprocess_language.py
+-rw-r--r--   0        0        0     5357 2024-04-24 00:28:27.706481 open_interpreter-0.2.5/interpreter/core/computer/terminal/terminal.py
+-rw-r--r--   0        0        0     7097 2024-03-10 10:24:40.130329 open_interpreter-0.2.5/interpreter/core/computer/utils/computer_vision.py
+-rw-r--r--   0        0        0     1479 2024-01-03 12:15:42.013393 open_interpreter-0.2.5/interpreter/core/computer/utils/get_active_window.py
+-rw-r--r--   0        0        0      929 2023-12-19 21:39:53.013384 open_interpreter-0.2.5/interpreter/core/computer/utils/html_to_png_base64.py
+-rw-r--r--   0        0        0      396 2024-01-02 01:05:06.051382 open_interpreter-0.2.5/interpreter/core/computer/utils/recipient_utils.py
+-rw-r--r--   0        0        0     1053 2024-03-19 02:56:22.059193 open_interpreter-0.2.5/interpreter/core/computer/utils/run_applescript.py
+-rw-r--r--   0        0        0    14816 2024-04-12 01:34:49.649602 open_interpreter-0.2.5/interpreter/core/core.py
+-rw-r--r--   0        0        0     3287 2024-04-17 01:29:13.078363 open_interpreter-0.2.5/interpreter/core/default_system_message.py
+-rw-r--r--   0        0        0        0 2023-09-23 02:28:30.997182 open_interpreter-0.2.5/interpreter/core/llm/__init__.py
+-rw-r--r--   0        0        0     8414 2024-04-24 05:33:16.850552 open_interpreter-0.2.5/interpreter/core/llm/llm.py
+-rw-r--r--   0        0        0     5052 2024-03-12 01:23:40.325749 open_interpreter-0.2.5/interpreter/core/llm/run_function_calling_llm.py
+-rw-r--r--   0        0        0     2706 2024-04-12 01:34:25.728520 open_interpreter-0.2.5/interpreter/core/llm/run_text_llm.py
+-rw-r--r--   0        0        0     8741 2024-04-12 01:37:38.248951 open_interpreter-0.2.5/interpreter/core/llm/utils/convert_to_openai_messages.py
+-rw-r--r--   0        0        0      711 2024-01-18 07:07:05.653072 open_interpreter-0.2.5/interpreter/core/llm/utils/merge_deltas.py
+-rw-r--r--   0        0        0     1800 2024-01-14 06:05:45.235518 open_interpreter-0.2.5/interpreter/core/llm/utils/parse_partial_json.py
+-rw-r--r--   0        0        0      538 2024-03-07 18:53:17.146944 open_interpreter-0.2.5/interpreter/core/llm/vision_for_text_llms.py
+-rw-r--r--   0        0        0     1290 2024-04-17 01:29:13.078867 open_interpreter-0.2.5/interpreter/core/render_message.py
+-rw-r--r--   0        0        0    13904 2024-04-12 01:34:49.650160 open_interpreter-0.2.5/interpreter/core/respond.py
+-rw-r--r--   0        0        0     6162 2024-01-31 07:55:31.444394 open_interpreter-0.2.5/interpreter/core/server.py
+-rw-r--r--   0        0        0        0 2023-09-23 02:28:31.002568 open_interpreter-0.2.5/interpreter/core/utils/__init__.py
+-rw-r--r--   0        0        0      920 2024-02-17 09:50:43.576535 open_interpreter-0.2.5/interpreter/core/utils/lazy_import.py
+-rw-r--r--   0        0        0     2118 2023-12-28 08:17:40.528813 open_interpreter-0.2.5/interpreter/core/utils/scan_code.py
+-rw-r--r--   0        0        0     4404 2024-01-07 07:39:34.178302 open_interpreter-0.2.5/interpreter/core/utils/system_debug_info.py
+-rw-r--r--   0        0        0     2757 2024-04-24 00:28:27.706766 open_interpreter-0.2.5/interpreter/core/utils/telemetry.py
+-rw-r--r--   0        0        0     1098 2023-09-28 20:53:00.949736 open_interpreter-0.2.5/interpreter/core/utils/temporary_file.py
+-rw-r--r--   0        0        0      510 2023-11-01 04:34:50.868691 open_interpreter-0.2.5/interpreter/core/utils/truncate_output.py
+-rw-r--r--   0        0        0        0 2023-09-23 02:28:30.998571 open_interpreter-0.2.5/interpreter/terminal_interface/__init__.py
+-rw-r--r--   0        0        0      611 2023-11-01 04:34:50.864816 open_interpreter-0.2.5/interpreter/terminal_interface/components/base_block.py
+-rw-r--r--   0        0        0     2664 2024-01-27 04:54:05.332821 open_interpreter-0.2.5/interpreter/terminal_interface/components/code_block.py
+-rw-r--r--   0        0        0     1386 2023-12-13 08:26:44.851269 open_interpreter-0.2.5/interpreter/terminal_interface/components/message_block.py
+-rw-r--r--   0        0        0     2905 2024-02-17 09:50:43.577169 open_interpreter-0.2.5/interpreter/terminal_interface/conversation_navigator.py
+-rw-r--r--   0        0        0    10581 2024-04-24 00:28:27.706955 open_interpreter-0.2.5/interpreter/terminal_interface/magic_commands.py
+-rw-r--r--   0        0        0    15149 2024-04-17 01:29:13.079349 open_interpreter-0.2.5/interpreter/terminal_interface/profiles/defaults/01.py
+-rw-r--r--   0        0        0     1059 2024-04-24 00:28:27.707064 open_interpreter-0.2.5/interpreter/terminal_interface/profiles/defaults/default.yaml
+-rw-r--r--   0        0        0     1287 2024-03-08 04:29:05.658598 open_interpreter-0.2.5/interpreter/terminal_interface/profiles/defaults/fast.yaml
+-rw-r--r--   0        0        0    17069 2024-04-24 05:33:16.851394 open_interpreter-0.2.5/interpreter/terminal_interface/profiles/defaults/local.py
+-rw-r--r--   0        0        0    11276 2024-04-24 00:28:26.196622 open_interpreter-0.2.5/interpreter/terminal_interface/profiles/defaults/os.py
+-rw-r--r--   0        0        0     1198 2024-03-08 04:29:05.659492 open_interpreter-0.2.5/interpreter/terminal_interface/profiles/defaults/vision.yaml
+-rw-r--r--   0        0        0       25 2024-01-26 03:07:17.828725 open_interpreter-0.2.5/interpreter/terminal_interface/profiles/historical_profiles.py
+-rw-r--r--   0        0        0    41316 2024-04-24 05:33:09.979342 open_interpreter-0.2.5/interpreter/terminal_interface/profiles/profiles.py
+-rw-r--r--   0        0        0     2304 2024-01-31 01:14:13.686159 open_interpreter-0.2.5/interpreter/terminal_interface/render_past_conversation.py
+-rw-r--r--   0        0        0    16524 2024-04-12 01:34:49.653490 open_interpreter-0.2.5/interpreter/terminal_interface/start_terminal_interface.py
+-rw-r--r--   0        0        0    20223 2024-04-17 01:29:13.080572 open_interpreter-0.2.5/interpreter/terminal_interface/terminal_interface.py
+-rw-r--r--   0        0        0      512 2023-11-20 05:25:30.624843 open_interpreter-0.2.5/interpreter/terminal_interface/utils/check_for_package.py
+-rw-r--r--   0        0        0      481 2023-11-05 01:34:27.337773 open_interpreter-0.2.5/interpreter/terminal_interface/utils/check_for_update.py
+-rw-r--r--   0        0        0      419 2024-03-07 11:14:28.681094 open_interpreter-0.2.5/interpreter/terminal_interface/utils/cli_input.py
+-rw-r--r--   0        0        0     1939 2024-01-03 12:15:41.692984 open_interpreter-0.2.5/interpreter/terminal_interface/utils/count_tokens.py
+-rw-r--r--   0        0        0      884 2024-01-25 21:39:42.258551 open_interpreter-0.2.5/interpreter/terminal_interface/utils/display_markdown_message.py
+-rw-r--r--   0        0        0     3069 2024-01-13 20:23:21.041610 open_interpreter-0.2.5/interpreter/terminal_interface/utils/display_output.py
+-rw-r--r--   0        0        0      459 2023-11-11 08:24:50.947604 open_interpreter-0.2.5/interpreter/terminal_interface/utils/find_image_path.py
+-rw-r--r--   0        0        0      250 2023-11-20 05:25:42.539104 open_interpreter-0.2.5/interpreter/terminal_interface/utils/get_conversations.py
+-rw-r--r--   0        0        0      184 2023-12-05 07:45:32.479315 open_interpreter-0.2.5/interpreter/terminal_interface/utils/in_jupyter_notebook.py
+-rw-r--r--   0        0        0      316 2024-03-08 04:29:05.661476 open_interpreter-0.2.5/interpreter/terminal_interface/utils/local_storage_path.py
+-rw-r--r--   0        0        0       79 2024-03-08 04:29:05.662377 open_interpreter-0.2.5/interpreter/terminal_interface/utils/oi_dir.py
+-rw-r--r--   0        0        0     3105 2024-04-12 01:34:49.654612 open_interpreter-0.2.5/interpreter/terminal_interface/validate_llm_settings.py
+-rw-r--r--   0        0        0     2163 2024-04-24 05:33:16.857995 open_interpreter-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    16518 1970-01-01 00:00:00.000000 open_interpreter-0.2.5/PKG-INFO
```

### Comparing `open_interpreter-0.2.4/LICENSE` & `open_interpreter-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/README.md` & `open_interpreter-0.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,25 @@
         <img alt="Discord" src="https://img.shields.io/discord/1146610656779440188?logo=discord&style=flat&logoColor=white"/></a>
     <a href="docs/README_JA.md"><img src="https://img.shields.io/badge/ドキュメント-日本語-white.svg" alt="JA doc"/></a>
     <a href="docs/README_ZH.md"><img src="https://img.shields.io/badge/文档-中文版-white.svg" alt="ZH doc"/></a>
     <a href="docs/README_IN.md"><img src="https://img.shields.io/badge/Hindi-white.svg" alt="IN doc"/></a>
     <img src="https://img.shields.io/static/v1?label=license&message=AGPL&color=white&style=flat" alt="License"/>
     <br>
     <br>
-    <strong>Today we launched a new computer (the 01) with Open Interpreter at the center. <a href="https://github.com/OpenInterpreter/01">Star the repo →</a></strong><br>
-    <br><a href="https://openinterpreter.com">Get early access to the desktop app</a>‎ ‎ |‎ ‎ <a href="https://docs.openinterpreter.com/">Documentation</a><br>
+    <br><a href="https://0ggfznkwh4j.typeform.com/to/G21i9lJ2">Get early access to the desktop app</a>‎ ‎ |‎ ‎ <a href="https://docs.openinterpreter.com/">Documentation</a><br>
 </p>
 
 <br>
 
 ![poster](https://github.com/KillianLucas/open-interpreter/assets/63927363/08f0d493-956b-4d49-982e-67d4b20c4b56)
 
 <br>
-<!--<p align="center">
-<strong>The New Computer Update</strong> introduces <strong><code>--os</code></strong> and a new <strong>Computer API</strong>. <a href="https://changes.openinterpreter.com/log/the-new-computer-update">Read On →</a>
-</p>-->
+<p align="center">
+<strong>The New Computer Update</strong> introduced <strong><code>--os</code></strong> and a new <strong>Computer API</strong>. <a href="https://changes.openinterpreter.com/log/the-new-computer-update">Read On →</a>
+</p>
 <br>
 
 ```shell
 pip install open-interpreter
 ```
 
 > Not working? Read our [setup guide](https://docs.openinterpreter.com/getting-started/setup).
@@ -79,14 +78,18 @@
 ```python
 from interpreter import interpreter
 
 interpreter.chat("Plot AAPL and META's normalized stock prices") # Executes a single command
 interpreter.chat() # Starts an interactive chat
 ```
 
+### GitHub Codespaces
+
+Press the `,` key on this repository's GitHub page to create a codespace. After a moment, you'll receive a cloud virtual machine environment pre-installed with open-interpreter. You can then start interacting with it directly and freely confirm its execution of system commands without worrying about damaging the system.
+
 ## Comparison to ChatGPT's Code Interpreter
 
 OpenAI's release of [Code Interpreter](https://openai.com/blog/chatgpt-plugins#code-interpreter) with GPT-4 presents a fantastic opportunity to accomplish real-world tasks with ChatGPT.
 
 However, OpenAI's service is hosted, closed-source, and heavily restricted:
 
 - No internet access.
@@ -356,14 +359,42 @@
 
 ## How Does it Work?
 
 Open Interpreter equips a [function-calling language model](https://platform.openai.com/docs/guides/gpt/function-calling) with an `exec()` function, which accepts a `language` (like "Python" or "JavaScript") and `code` to run.
 
 We then stream the model's messages, code, and your system's outputs to the terminal as Markdown.
 
+# Access Documentation Offline
+
+The full [documentation](https://docs.openinterpreter.com/) is accessible on-the-go without the need for an internet connection.
+
+[Node](https://nodejs.org/en) is a pre-requisite:
+
+- Version 18.17.0 or any later 18.x.x version.
+- Version 20.3.0 or any later 20.x.x version.
+- Any version starting from 21.0.0 onwards, with no upper limit specified.
+
+Install [Mintlify](https://mintlify.com/):
+
+```bash
+npm i -g mintlify@latest
+```
+
+Change into the docs directory and run the appropriate command:
+
+```bash
+# Assuming you're at the project's root directory
+cd ./docs
+
+# Run the documentation server
+mintlify dev
+```
+
+A new browser window should open. The documentation will be available at [http://localhost:3000](http://localhost:3000) as long as the documentation server is running.
+
 # Contributing
 
 Thank you for your interest in contributing! We welcome involvement from the community.
 
 Please see our [contributing guidelines](docs/CONTRIBUTING.md) for more details on how to get involved.
 
 # Roadmap
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
                       ************ ?â?? OOppeenn IInntteerrpprreetteerr ************
                   _[_D_i_s_c_o_r_d_]_[_J_A_ _d_o_c_]_[_Z_H_ _d_o_c_]_[_I_N_ _d_o_c_][License]
 
-TTooddaayy wwee llaauunncchheedd aa nneeww ccoommppuutteerr ((tthhee 0011)) wwiitthh OOppeenn IInntteerrpprreetteerr aatt tthhee cceenntteerr..
-                               _SS_tt_aa_rr_ _tt_hh_ee_ _rr_ee_pp_oo_ _?â_?_?
 
        _G_e_t_ _e_a_r_l_y_ _a_c_c_e_s_s_ _t_o_ _t_h_e_ _d_e_s_k_t_o_p_ _a_p_pâ â |â â _D_o_c_u_m_e_n_t_a_t_i_o_n
 
 ![poster](https://github.com/KillianLucas/open-interpreter/assets/63927363/
 08f0d493-956b-4d49-982e-67d4b20c4b56)
+  TThhee NNeeww CCoommppuutteerr UUppddaattee introduced ----ooss and a new CCoommppuutteerr AAPPII. _R_e_a_d_ _O_n_ _â__
 
 ```shell pip install open-interpreter ``` > Not working? Read our [setup guide]
 (https://docs.openinterpreter.com/getting-started/setup). ```shell interpreter
 ```
 **Open Interpreter** lets LLMs run code (Python, Javascript, Shell, and more)
 locally. You can chat with Open Interpreter through a ChatGPT-like interface in
 your terminal by running `$ interpreter` after installing. This provides a
@@ -27,31 +26,36 @@
 interface, inspired by _Her_: [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1NojYGHDgxH6Y1G1oxThEBBb2AtyODBIK) ## Quick
 Start ```shell pip install open-interpreter ``` ### Terminal After
 installation, simply run `interpreter`: ```shell interpreter ``` ### Python
 ```python from interpreter import interpreter interpreter.chat("Plot AAPL and
 META's normalized stock prices") # Executes a single command interpreter.chat()
-# Starts an interactive chat ``` ## Comparison to ChatGPT's Code Interpreter
-OpenAI's release of [Code Interpreter](https://openai.com/blog/chatgpt-
-plugins#code-interpreter) with GPT-4 presents a fantastic opportunity to
-accomplish real-world tasks with ChatGPT. However, OpenAI's service is hosted,
-closed-source, and heavily restricted: - No internet access. - [Limited set of
-pre-installed packages](https://wfhbrian.com/mastering-chatgpts-code-
-interpreter-list-of-python-packages/). - 100 MB maximum upload, 120.0 second
-runtime limit. - State is cleared (along with any generated files or links)
-when the environment dies. --- Open Interpreter overcomes these limitations by
-running in your local environment. It has full access to the internet, isn't
-restricted by time or file size, and can utilize any package or library. This
-combines the power of GPT-4's Code Interpreter with the flexibility of your
-local development environment. ## Commands **Update:** The Generator Update
-(0.1.5) introduced streaming: ```python message = "What operating system are we
-on?" for chunk in interpreter.chat(message, display=False, stream=True): print
-(chunk) ``` ### Interactive Chat To start an interactive chat in your terminal,
-either run `interpreter` from the command line: ```shell interpreter ``` Or
+# Starts an interactive chat ``` ### GitHub Codespaces Press the `,` key on
+this repository's GitHub page to create a codespace. After a moment, you'll
+receive a cloud virtual machine environment pre-installed with open-
+interpreter. You can then start interacting with it directly and freely confirm
+its execution of system commands without worrying about damaging the system. ##
+Comparison to ChatGPT's Code Interpreter OpenAI's release of [Code Interpreter]
+(https://openai.com/blog/chatgpt-plugins#code-interpreter) with GPT-4 presents
+a fantastic opportunity to accomplish real-world tasks with ChatGPT. However,
+OpenAI's service is hosted, closed-source, and heavily restricted: - No
+internet access. - [Limited set of pre-installed packages](https://
+wfhbrian.com/mastering-chatgpts-code-interpreter-list-of-python-packages/). -
+100 MB maximum upload, 120.0 second runtime limit. - State is cleared (along
+with any generated files or links) when the environment dies. --- Open
+Interpreter overcomes these limitations by running in your local environment.
+It has full access to the internet, isn't restricted by time or file size, and
+can utilize any package or library. This combines the power of GPT-4's Code
+Interpreter with the flexibility of your local development environment. ##
+Commands **Update:** The Generator Update (0.1.5) introduced streaming:
+```python message = "What operating system are we on?" for chunk in
+interpreter.chat(message, display=False, stream=True): print(chunk) ``` ###
+Interactive Chat To start an interactive chat in your terminal, either run
+`interpreter` from the command line: ```shell interpreter ``` Or
 `interpreter.chat()` from a .py file: ```python interpreter.chat() ``` **You
 can also stream each chunk:** ```python message = "What operating system are we
 on?" for chunk in interpreter.chat(message, display=False, stream=True): print
 (chunk) ``` ### Programmatic Chat For more precise control, you can pass
 messages directly to `.chat(message)`: ```python interpreter.chat("Add
 subtitles to all videos in /videos.") # ... Streams output to your terminal,
 completes task ... interpreter.chat("These look great but can you make the
@@ -148,18 +152,29 @@
 Open Interpreter in a restricted environment like Google Colab or Replit. These
 environments are more isolated, reducing the risks of executing arbitrary code.
 There is **experimental** support for a [safe mode](docs/SAFE_MODE.md) to help
 mitigate some risks. ## How Does it Work? Open Interpreter equips a [function-
 calling language model](https://platform.openai.com/docs/guides/gpt/function-
 calling) with an `exec()` function, which accepts a `language` (like "Python"
 or "JavaScript") and `code` to run. We then stream the model's messages, code,
-and your system's outputs to the terminal as Markdown. # Contributing Thank you
-for your interest in contributing! We welcome involvement from the community.
-Please see our [contributing guidelines](docs/CONTRIBUTING.md) for more details
-on how to get involved. # Roadmap Visit [our roadmap](https://github.com/
-KillianLucas/open-interpreter/blob/main/docs/ROADMAP.md) to preview the future
-of Open Interpreter. **Note**: This software is not affiliated with OpenAI. !
-[thumbnail-ncu](https://github.com/KillianLucas/open-interpreter/assets/
-63927363/1b19a5db-b486-41fd-a7a1-fe2028031686) > Having access to a junior
-programmer working at the speed of your fingertips ... can make new workflows
-effortless and efficient, as well as open the benefits of programming to new
-audiences. > > â _OpenAI's Code Interpreter Release_
+and your system's outputs to the terminal as Markdown. # Access Documentation
+Offline The full [documentation](https://docs.openinterpreter.com/) is
+accessible on-the-go without the need for an internet connection. [Node](https:
+//nodejs.org/en) is a pre-requisite: - Version 18.17.0 or any later 18.x.x
+version. - Version 20.3.0 or any later 20.x.x version. - Any version starting
+from 21.0.0 onwards, with no upper limit specified. Install [Mintlify](https://
+mintlify.com/): ```bash npm i -g mintlify@latest ``` Change into the docs
+directory and run the appropriate command: ```bash # Assuming you're at the
+project's root directory cd ./docs # Run the documentation server mintlify dev
+``` A new browser window should open. The documentation will be available at
+[http://localhost:3000](http://localhost:3000) as long as the documentation
+server is running. # Contributing Thank you for your interest in contributing!
+We welcome involvement from the community. Please see our [contributing
+guidelines](docs/CONTRIBUTING.md) for more details on how to get involved. #
+Roadmap Visit [our roadmap](https://github.com/KillianLucas/open-interpreter/
+blob/main/docs/ROADMAP.md) to preview the future of Open Interpreter. **Note**:
+This software is not affiliated with OpenAI. ![thumbnail-ncu](https://
+github.com/KillianLucas/open-interpreter/assets/63927363/1b19a5db-b486-41fd-
+a7a1-fe2028031686) > Having access to a junior programmer working at the speed
+of your fingertips ... can make new workflows effortless and efficient, as well
+as open the benefits of programming to new audiences. > > â _OpenAI's Code
+Interpreter Release_
```

### Comparing `open_interpreter-0.2.4/interpreter/__init__.py` & `open_interpreter-0.2.5/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/ai/ai.py` & `open_interpreter-0.2.5/interpreter/core/computer/ai/ai.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/calendar/calendar.py` & `open_interpreter-0.2.5/interpreter/core/computer/calendar/calendar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 import datetime
 import platform
 import subprocess
 
 from ..utils.run_applescript import run_applescript, run_applescript_capture
 
 
+makeDateFunction = """
+on makeDate(yr, mon, day, hour, min, sec)
+	set theDate to current date
+	tell theDate
+		set its year to yr
+		set its month to mon
+		set its day to day
+		set its hours to hour
+		set its minutes to min
+		set its seconds to sec
+	end tell
+	return theDate
+end makeDate
+"""
+
 class Calendar:
     def __init__(self, computer):
         self.computer = computer
         # In the future, we might consider a way to use a different calender app. For now its Calendar
         self.calendar_app = "Calendar"
 
     def get_events(self, start_date=datetime.date.today(), end_date=None):
         """
         Fetches calendar events for the given date or date range.
         """
         if platform.system() != "Darwin":
             return "This method is only supported on MacOS"
 
-        # Format dates for AppleScript
-        applescript_start_date = (
-            start_date.strftime("%A, %B %d, %Y") + " at 12:00:00 AM"
-        )
-        if end_date:
-            applescript_end_date = (
-                end_date.strftime("%A, %B %d, %Y") + " at 11:59:59 PM"
-            )
-        else:
-            applescript_end_date = (
-                start_date.strftime("%A, %B %d, %Y") + " at 11:59:59 PM"
-            )
-
+        if not end_date:
+            end_date = start_date
         # AppleScript command
         script = f"""
-        set theDate to date "{applescript_start_date}"
-        set endDate to date "{applescript_end_date}"
+        {makeDateFunction}
+        set theDate to makeDate({start_date.strftime("%Y, %m, %d, 0, 0, 0")})
+        set endDate to makeDate({end_date.strftime("%Y, %m, %d, 23, 59, 59")})
         tell application "System Events"
             set calendarIsRunning to (name of processes) contains "{self.calendar_app}"
             if calendarIsRunning then
                 tell application "{self.calendar_app}" to activate
             else
                 tell application "{self.calendar_app}" to launch
                 delay 1 -- Wait for the application to open
@@ -175,29 +180,30 @@
         # If there is no calendar, lets use the first calendar applescript returns. This should probably be modified in the future
         if calendar is None:
             calendar = self.get_first_calendar()
             if calendar is None:
                 return "Can't find a default calendar. Please try again and specify a calendar name."
 
         script = f"""
+        {makeDateFunction}
+        set startDate to makeDate({start_date.strftime("%Y, %m, %d, %H, %M, %S")})
+        set endDate to makeDate({end_date.strftime("%Y, %m, %d, %H, %M, %S")})
         -- Open and activate calendar first
         tell application "System Events"
             set calendarIsRunning to (name of processes) contains "{self.calendar_app}"
             if calendarIsRunning then
                 tell application "{self.calendar_app}" to activate
             else
                 tell application "{self.calendar_app}" to launch
                 delay 1 -- Wait for the application to open
                 tell application "{self.calendar_app}" to activate
             end if
         end tell
         tell application "{self.calendar_app}"
             tell calendar "{calendar}"
-                set startDate to date "{applescript_start_date}"
-                set endDate to date "{applescript_end_date}"
                 make new event at end with properties {{summary:"{title}", start date:startDate, end date:endDate, location:"{location}", description:"{notes}"}}
             end tell
             -- tell the Calendar app to refresh if it's running, so the new event shows up immediately
             tell application "{self.calendar_app}" to reload calendars
         end tell
         """
 
@@ -219,17 +225,17 @@
 
         # If there is no calendar, lets use the first calendar applescript returns. This should probably be modified in the future
         if calendar is None:
             calendar = self.get_first_calendar()
             if not calendar:
                 return "Can't find a default calendar. Please try again and specify a calendar name."
 
-        # Format datetime for AppleScript
-        applescript_start_date = start_date.strftime("%B %d, %Y %I:%M:%S %p")
         script = f"""
+        {makeDateFunction}
+        set eventStartDate to makeDate({start_date.strftime("%Y, %m, %d, %H, %M, %S")})
         -- Open and activate calendar first
         tell application "System Events"
             set calendarIsRunning to (name of processes) contains "{self.calendar_app}"
             if calendarIsRunning then
                 tell application "{self.calendar_app}" to activate
             else
                 tell application "{self.calendar_app}" to launch
@@ -238,15 +244,14 @@
             end if
         end tell
         tell application "{self.calendar_app}"
             -- Specify the name of the calendar where the event is located
             set myCalendar to calendar "{calendar}"
             
             -- Define the exact start date and name of the event to find and delete
-            set eventStartDate to date "{applescript_start_date}"
             set eventSummary to "{event_title}"
             
             -- Find the event by start date and summary
             set theEvents to (every event of myCalendar where its start date is eventStartDate and its summary is eventSummary)
             
             -- Check if any events were found
             if (count of theEvents) is equal to 0 then
```

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/clipboard/clipboard.py` & `open_interpreter-0.2.5/interpreter/core/computer/clipboard/clipboard.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/computer.py` & `open_interpreter-0.2.5/interpreter/core/computer/computer.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,17 @@
         self.emit_images = True
         self.api_base = "https://api.openinterpreter.com/v0"
         self.save_skills = True
 
         self.import_computer_api = False  # Defaults to false
         self._has_imported_computer_api = False  # Because we only want to do this once
 
+        self.import_skills = False
+        self._has_imported_skills = False
+
     # Shortcut for computer.terminal.languages
     @property
     def languages(self):
         return self.terminal.languages
 
     @languages.setter
     def languages(self, value):
```

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/contacts/contacts.py` & `open_interpreter-0.2.5/interpreter/core/computer/contacts/contacts.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/display/display.py` & `open_interpreter-0.2.5/interpreter/core/computer/display/display.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,28 +2,33 @@
 import os
 import platform
 import pprint
 import time
 import warnings
 from contextlib import redirect_stdout
 from io import BytesIO
-
+import io
+import subprocess
+from PIL import Image
 import requests
-
 from ...utils.lazy_import import lazy_import
 from ..utils.recipient_utils import format_to_recipient
+from screeninfo import get_monitors # for getting info about connected monitors
+
 
 # Still experimenting with this
 # from utils.get_active_window import get_active_window
 
 # Lazy import of optional packages
+cv2 = lazy_import("cv2")
 pyautogui = lazy_import("pyautogui")
 np = lazy_import("numpy")
 plt = lazy_import("matplotlib.pyplot")
 
+
 from ..utils.computer_vision import find_text_in_image, pytesseract_get_text
 
 
 class Display:
     def __init__(self, computer):
         self.computer = computer
         # set width and height to None initially to prevent pyautogui from importing until it's needed
@@ -52,28 +57,38 @@
 
     def center(self):
         """
         Calculates and returns the center point of the screen as a tuple (x, y).
         """
         return self.width // 2, self.height // 2
 
-    def view(self, show=True, quadrant=None):
+    def info(self):
+        """
+        Returns a list of all connected montitor/displays and thir information
+        """
+        return get_displays()
+    
+    
+    def view(self, show=True, quadrant=None, screen=0, combine_screens=True
+    ):
         """
         Redirects to self.screenshot
         """
-        return self.screenshot(show, quadrant)
+        return self.screenshot(screen=screen, show=show, quadrant=quadrant, combine_screens=combine_screens)
 
     # def get_active_window(self):
     #     return get_active_window()
 
     def screenshot(
-        self, show=True, quadrant=None, active_app_only=False, force_image=False
+        self, screen=0, show=True, quadrant=None, active_app_only=False, force_image=False,combine_screens=True
     ):
         """
         Shows you what's on the screen by taking a screenshot of the entire screen or a specified quadrant. Returns a `pil_image` `in case you need it (rarely). **You almost always want to do this first!**
+        :param screen: specify which display; 0 for primary and 1 and above for secondary.
+        :param combine_screens: If True, a collage of all display screens will be returned. Otherwise, a list of display screens will be returned.
         """
         if not self.computer.emit_images and force_image == False:
             text = self.get_text_as_list_of_lists()
             pp = pprint.PrettyPrinter(indent=4)
             pretty_text = pp.pformat(text)  # language models like it pretty!
             pretty_text = format_to_recipient(pretty_text, "assistant")
             print(pretty_text)
@@ -87,18 +102,15 @@
 
         if quadrant == None:
             # Implement active_app_only!
             if active_app_only:
                 region = self.get_active_window()["region"]
                 screenshot = pyautogui.screenshot(region=region)
             else:
-                if platform.system() == "Darwin":
-                    screenshot = take_screenshot_to_pil()
-                else:
-                    screenshot = pyautogui.screenshot()
+                screenshot = take_screenshot_to_pil(screen=screen, combine_screens=combine_screens) #  this function uses pyautogui.screenshot which works fine for all OS (mac, linux and windows)
                 # message = format_to_recipient("Taking a screenshot of the entire screen. This is not recommended. You (the language model assistant) will recieve it with low resolution.\n\nTo maximize performance, use computer.display.view(active_app_only=True). This will produce an ultra high quality image of the active application.", "assistant")
                 # print(message)
 
         else:
             screen_width, screen_height = pyautogui.size()
 
             quadrant_width = screen_width // 2
@@ -117,26 +129,34 @@
                     region=(x, y, quadrant_width, quadrant_height)
                 )
             else:
                 raise ValueError("Invalid quadrant. Choose between 1 and 4.")
 
         # Open the image file with PIL
         # IPython interactive mode auto-displays plots, causing RGBA handling issues, possibly MacOS-specific.
-        screenshot = screenshot.convert("RGB")
+        if isinstance(screenshot, list):
+            screenshot = [img.convert("RGB") for img in screenshot] # if screenshot is a list (i.e combine_screens=False).
+        else:
+            screenshot = screenshot.convert("RGB")
 
         if show:
             # Show the image using matplotlib
-            plt.imshow(np.array(screenshot))
+            if isinstance(screenshot, list):
+                for img in screenshot:
+                    plt.imshow(np.array(img))
+                    plt.show()
+            else:
+                plt.imshow(np.array(screenshot))
 
             with warnings.catch_warnings():
                 # It displays an annoying message about Agg not being able to display something or WHATEVER
                 warnings.simplefilter("ignore")
                 plt.show()
 
-        return screenshot
+        return screenshot # this will be a list of combine_screens == False
 
     def find(self, description, screenshot=None):
         if description.startswith('"') and description.endswith('"'):
             return self.find_text(description.strip('"'), screenshot)
         else:
             try:
                 if self.computer.debug:
@@ -256,26 +276,82 @@
             return pytesseract_get_text(screenshot)
         except:
             raise Exception(
                 "Failed to find text locally.\n\nTo find text in order to use the mouse, please make sure you've installed `pytesseract` along with the Tesseract executable (see this Stack Overflow answer for help installing Tesseract: https://stackoverflow.com/questions/50951955/pytesseract-tesseractnotfound-error-tesseract-is-not-installed-or-its-not-i)."
             )
 
 
-import io
-import subprocess
-
-from PIL import Image
+def take_screenshot_to_pil(screen=0, combine_screens=True):
+    # Get information about all screens
+    monitors = get_monitors()
+    if screen == -1: # All screens
+        
+        # Take a screenshot of each screen and save them in a list
+        screenshots = [pyautogui.screenshot(region=(monitor.x, monitor.y, monitor.width, monitor.height)) for monitor in monitors]
+
+        if combine_screens:
+            # Combine all screenshots horizontally
+            total_width = sum([img.width for img in screenshots])
+            max_height = max([img.height for img in screenshots])
+
+            # Create a new image with a size that can contain all screenshots
+            new_img = Image.new('RGB', (total_width, max_height))
+
+            # Paste each screenshot into the new image
+            x_offset = 0
+            for i, img in enumerate(screenshots):
+                # Convert PIL Image to OpenCV Image (numpy array)
+                img_cv = np.array(img)
+                img_cv = cv2.cvtColor(img_cv, cv2.COLOR_RGB2BGR)
+
+                # Convert new_img PIL Image to OpenCV Image (numpy array)
+                new_img_cv = np.array(new_img)
+                new_img_cv = cv2.cvtColor(new_img_cv, cv2.COLOR_RGB2BGR)
+
+                # Paste each screenshot into the new image using OpenCV
+                new_img_cv[0:img_cv.shape[0], x_offset:x_offset+img_cv.shape[1]] = img_cv
+                x_offset += img.width
+
+                # Add monitor labels using OpenCV
+                font = cv2.FONT_HERSHEY_SIMPLEX
+                font_scale = 4
+                font_color = (255, 255, 255)
+                line_type = 2
 
+                if i == 0:
+                    text = "Primary Monitor"
+                else:
+                    text = f"Monitor {i}"
+                
+                # Calculate the font scale that will fit the text perfectly in the center of the monitor
+                text_size = cv2.getTextSize(text, font, font_scale, line_type)[0]
+                font_scale = min(img.width / text_size[0], img.height / text_size[1])
+                
+                # Recalculate the text size with the new font scale
+                text_size = cv2.getTextSize(text, font, font_scale, line_type)[0]
+                
+                # Calculate the position to center the text
+                text_x = x_offset - img.width // 2 - text_size[0] // 2
+                text_y = max_height // 2 - text_size[1] // 2
+                
+                cv2.putText(new_img_cv, text, (text_x, text_y), font, font_scale, font_color, line_type)
+
+                # Convert new_img from OpenCV Image back to PIL Image
+                new_img_cv = cv2.cvtColor(new_img_cv, cv2.COLOR_BGR2RGB)
+                new_img = Image.fromarray(new_img_cv)
 
-def take_screenshot_to_pil(filename="temp_screenshot.png"):
-    # Capture the screenshot and save it to a temporary file
-    subprocess.run(["screencapture", "-x", filename], check=True)
-
-    # Open the image file with PIL
-    with open(filename, "rb") as f:
-        image_data = f.read()
-    image = Image.open(io.BytesIO(image_data))
+            return new_img
+        else:
+            return screenshots
+    elif screen > 0:
+        # Take a screenshot of the selected screen
+        return pyautogui.screenshot(region=(monitors[screen].x, monitors[screen].y, monitors[screen].width, monitors[screen].height))
+        
+    else:
+        # Take a screenshot of the primary screen
+        return pyautogui.screenshot(region=(monitors[screen].x, monitors[screen].y, monitors[screen].width, monitors[screen].height))
 
-    # Optionally, delete the temporary file if you don't need it after loading
-    os.remove(filename)
 
-    return image
+def get_displays():
+    monitors = get_monitors()
+    return monitors
+
```

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/display/point/point.py` & `open_interpreter-0.2.5/interpreter/core/computer/display/point/point.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,21 @@
         return embeddings
 
     # Usage:
     # images = [Image.open(io.BytesIO(image_bytes1)), Image.open(io.BytesIO(image_bytes2)), ...]
     # embeddings = embed_images(images, model, transforms)
 
 
-device = torch.device("cpu")  # or 'cpu' for CPU, 'cuda:0' for the first GPU, etc.
+if torch.cuda.is_available():
+    device = torch.device("cuda")
+elif torch.backends.mps.is_available():
+    device = torch.device("mps")
+else:
+    device = torch.device("cpu")
+
 # Move the model to the specified device
 model = model.to(device)
 
 
 def image_search(query, icons, hashes, debug):
     hashed_icons = [icon for icon in icons if icon["hash"] in hashes]
     unhashed_icons = [icon for icon in icons if icon["hash"] not in hashes]
```

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/docs/docs.py` & `open_interpreter-0.2.5/interpreter/core/computer/docs/docs.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/files/files.py` & `open_interpreter-0.2.5/interpreter/core/computer/files/files.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/keyboard/keyboard.py` & `open_interpreter-0.2.5/interpreter/core/computer/keyboard/keyboard.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/mail/mail.py` & `open_interpreter-0.2.5/interpreter/core/computer/mail/mail.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/mouse/mouse.py` & `open_interpreter-0.2.5/interpreter/core/computer/mouse/mouse.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/os/os.py` & `open_interpreter-0.2.5/interpreter/core/computer/os/os.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/skills/skills.py` & `open_interpreter-0.2.5/interpreter/core/computer/skills/skills.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,26 +45,26 @@
                 code_to_run += f.read() + "\n"
 
         if self.computer.interpreter.debug:
             print("IMPORTING SKILLS:\n", code_to_run)
 
         output = self.computer.run("python", code_to_run)
 
-        if type(output) == str and "traceback" in output.lower():
+        if "traceback" in str(output).lower():
             # Import them individually
             for file in glob.glob(os.path.join(self.path, "*.py")):
                 with open(file, "r") as f:
                     code_to_run = f.read() + "\n"
 
                 if self.computer.interpreter.debug:
                     print("IMPORTING SKILL:\n", code_to_run)
 
                 output = self.computer.run("python", code_to_run)
 
-                if type(output) == str and "traceback" in output.lower():
+                if "traceback" in str(output).lower():
                     print(
                         f"Skill at {file} might be broken— it produces a traceback when run."
                     )
 
         self.computer.save_skills = previous_save_skills_setting
```

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/sms/sms.py` & `open_interpreter-0.2.5/interpreter/core/computer/sms/sms.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/terminal/base_language.py` & `open_interpreter-0.2.5/interpreter/core/computer/terminal/base_language.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/applescript.py` & `open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/applescript.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/html.py` & `open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/html.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/javascript.py` & `open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/javascript.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/jupyter_language.py` & `open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/jupyter_language.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,29 +6,31 @@
 import ast
 import os
 import queue
 import re
 import threading
 import time
 import traceback
+import logging
 
 from jupyter_client import KernelManager
 
 from ..base_language import BaseLanguage
 
 DEBUG_MODE = False
 
 
 class JupyterLanguage(BaseLanguage):
     file_extension = "py"
     name = "Python"
+    aliases = ["py"]
 
     def __init__(self, computer):
         self.computer = computer
-
+            
         self.km = KernelManager(kernel_name="python3")
         self.km.start_kernel()
         self.kc = self.km.client()
         self.kc.start_channels()
         while not self.kc.is_alive():
             time.sleep(0.1)
         time.sleep(0.5)
```

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/powershell.py` & `open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/powershell.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/r.py` & `open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/r.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/react.py` & `open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/react.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/shell.py` & `open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/shell.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/terminal/languages/subprocess_language.py` & `open_interpreter-0.2.5/interpreter/core/computer/terminal/languages/subprocess_language.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/terminal/terminal.py` & `open_interpreter-0.2.5/interpreter/core/computer/terminal/terminal.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,57 +2,63 @@
 from .languages.applescript import AppleScript
 from .languages.html import HTML
 from .languages.javascript import JavaScript
 from .languages.powershell import PowerShell
 from .languages.python import Python
 from .languages.r import R
 from .languages.react import React
+from .languages.ruby import Ruby
 from .languages.shell import Shell
 
 # Should this be renamed to OS or System?
 
 
 class Terminal:
     def __init__(self, computer):
         self.computer = computer
         self.languages = [
+            Ruby,
             Python,
             Shell,
             JavaScript,
             HTML,
             AppleScript,
             R,
             PowerShell,
             React,
         ]
         self._active_languages = {}
 
     def get_language(self, language):
         for lang in self.languages:
             if language.lower() == lang.name.lower() or (
-                hasattr(lang, "aliases") and language in lang.aliases
+                hasattr(lang, "aliases") and language.lower() in (alias.lower() for alias in lang.aliases)
             ):
                 return lang
         return None
 
     def run(self, language, code, stream=False, display=False):
-        if (
-            language == "python"
-            and self.computer.import_computer_api
-            and "computer" in code
-        ):
-            if not self.computer._has_imported_computer_api:
+        if language == "python":
+            if self.computer.import_computer_api and not self.computer._has_imported_computer_api and "computer" in code:
                 self.computer._has_imported_computer_api = True
                 # Give it access to the computer via Python
                 self.computer.run(
                     language="python",
                     code="import time\nfrom interpreter import interpreter\ncomputer = interpreter.computer",  # We ask it to use time, so
                     display=self.computer.verbose,
                 )
 
+            if self.computer.import_skills and not self.computer._has_imported_skills:
+                self.computer._has_imported_skills = True
+                self.computer.skills.import_skills()
+
+        # Llama 3 likes to hallucinate this tick new line thing at the start of code blocks
+        if code.startswith("`\n"):
+            code = code[2:].strip()
+
         if stream == False:
             # If stream == False, *pull* from _streaming_run.
             output_messages = []
             for chunk in self._streaming_run(language, code, display=display):
                 if chunk.get("format") != "active_line":
                     # Should we append this to the last message, or make a new one?
                     if (
@@ -100,15 +106,15 @@
 
                 # Print it also if display = True
                 if (
                     display
                     and chunk.get("format") != "active_line"
                     and chunk.get("content")
                 ):
-                    print(chunk["content"])
+                    print(chunk["content"], end="")
 
         except GeneratorExit:
             self.stop()
 
     def stop(self):
         for language in self._active_languages.values():
             language.stop()
```

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/utils/computer_vision.py` & `open_interpreter-0.2.5/interpreter/core/computer/utils/computer_vision.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/utils/get_active_window.py` & `open_interpreter-0.2.5/interpreter/core/computer/utils/get_active_window.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/utils/html_to_png_base64.py` & `open_interpreter-0.2.5/interpreter/core/computer/utils/html_to_png_base64.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/computer/utils/run_applescript.py` & `open_interpreter-0.2.5/interpreter/core/computer/utils/run_applescript.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/core.py` & `open_interpreter-0.2.5/interpreter/core/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,29 +53,29 @@
         force_task_completion_message="""Proceed. You CAN run code on my machine. If you want to run code, start your message with "```"! If the entire task I asked for is done, say exactly 'The task is done.' If you need some specific information (like username or password) say EXACTLY 'Please provide more information.' If it's impossible, say 'The task is impossible.' (If I haven't provided a task, say exactly 'Let me know what you'd like to do next.') Otherwise keep going.""",
         force_task_completion_breakers=[
             "the task is done.",
             "the task is impossible.",
             "let me know what you'd like to do next.",
             "please provide more information.",
         ],
-        anonymous_telemetry=os.getenv("ANONYMIZED_TELEMETRY", "True") == "True",
+        disable_telemetry=os.getenv("DISABLE_TELEMETRY", "false").lower() == "true",
         in_terminal_interface=False,
         conversation_history=True,
         conversation_filename=None,
         conversation_history_path=get_storage_path("conversations"),
         os=False,
         speak_messages=False,
         llm=None,
         system_message=default_system_message,
         custom_instructions="",
         computer=None,
-        sync_computer=True,
+        sync_computer=False,
         import_computer_api=False,
         skills_path=None,
-        import_skills=True,
+        import_skills=False,
         multi_line=False,
     ):
         # State
         self.messages = [] if messages is None else messages
         self.responding = False
         self.last_messages_count = 0
 
@@ -83,15 +83,15 @@
         self.offline = offline
         self.auto_run = auto_run
         self.verbose = verbose
         self.debug = debug
         self.max_output = max_output
         self.safe_mode = safe_mode
         self.shrink_images = shrink_images
-        self.anonymous_telemetry = anonymous_telemetry
+        self.disable_telemetry = disable_telemetry
         self.in_terminal_interface = in_terminal_interface
         self.multi_line = multi_line
 
         # Loop messages
         self.force_task_completion = force_task_completion
         self.force_task_completion_message = force_task_completion_message
         self.force_task_completion_breakers = force_task_completion_breakers
@@ -110,41 +110,40 @@
 
         # These are LLM related
         self.system_message = system_message
         self.custom_instructions = custom_instructions
 
         # Computer
         self.computer = Computer(self) if computer is None else computer
-
         self.sync_computer = sync_computer
         self.computer.import_computer_api = import_computer_api
 
         # Skills
         if skills_path:
             self.computer.skills.path = skills_path
 
-        self.import_skills = import_skills
-        if import_skills:
-            if self.verbose:
-                print("Importing skills")
-            self.computer.skills.import_skills()
+        self.computer.import_skills = import_skills
 
     def server(self, *args, **kwargs):
         server(self, *args, **kwargs)
 
     def wait(self):
         while self.responding:
             time.sleep(0.2)
         # Return new messages
         return self.messages[self.last_messages_count :]
 
+    @property
+    def anonymous_telemetry(self) -> bool:
+        return not self.disable_telemetry and not self.offline
+
     def chat(self, message=None, display=True, stream=False, blocking=True):
         try:
             self.responding = True
-            if self.anonymous_telemetry and not self.offline:
+            if self.anonymous_telemetry:
                 message_type = type(
                     message
                 ).__name__  # Only send message type, no content
                 send_telemetry(
                     "started_chat",
                     properties={
                         "in_terminal_interface": self.in_terminal_interface,
@@ -169,15 +168,15 @@
 
             # Return new messages
             self.responding = False
             return self.messages[self.last_messages_count :]
 
         except Exception as e:
             self.responding = False
-            if self.anonymous_telemetry and not self.offline:
+            if self.anonymous_telemetry:
                 message_type = type(message).__name__
                 send_telemetry(
                     "errored",
                     properties={
                         "error": str(e),
                         "in_terminal_interface": self.in_terminal_interface,
                         "message_type": message_type,
@@ -234,17 +233,19 @@
             # This is where it all happens!
             yield from self._respond_and_store()
 
             # Save conversation if we've turned conversation_history on
             if self.conversation_history:
                 # If it's the first message, set the conversation name
                 if not self.conversation_filename:
-                    first_few_words = "_".join(
-                        self.messages[0]["content"][:25].split(" ")[:-1]
-                    )
+                    first_few_words_list = self.messages[0]["content"][:25].split(" ")
+                    if len(first_few_words_list) >= 2:  # for languages like English with blank between words
+                        first_few_words = "_".join(first_few_words_list[:-1])
+                    else:  # for languages like Chinese without blank between words
+                        first_few_words = self.messages[0]["content"][:15]
                     for char in '<>:"/\\|?*!':  # Invalid characters for filenames
                         first_few_words = first_few_words.replace(char, "")
 
                     date = datetime.now().strftime("%B_%d_%Y_%H-%M-%S")
                     self.conversation_filename = (
                         "__".join([first_few_words, date]) + ".json"
                     )
@@ -348,14 +349,15 @@
 
         # Yield a final end flag
         if last_flag_base:
             yield {**last_flag_base, "end": True}
 
     def reset(self):
         self.computer.terminate()  # Terminates all languages
+        self.computer._has_imported_computer_api = False  # Flag reset
         self.messages = []
         self.last_messages_count = 0
 
     def display_message(self, markdown):
         # This is just handy for start_script in profiles.
         display_markdown_message(markdown)
```

### Comparing `open_interpreter-0.2.4/interpreter/core/default_system_message.py` & `open_interpreter-0.2.5/interpreter/core/default_system_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # THE COMPUTER API
 
 A python `computer` module is ALREADY IMPORTED, and can be used for many tasks:
 
 ```python
 computer.browser.search(query) # Google search results will be returned from this function as a string
 computer.files.edit(path_to_file, original_text, replacement_text) # Edit a file
-computer.calendar.create_event(title="Meeting", start_date=datetime.datetime.now(), end=datetime.datetime.now() + datetime.timedelta(hours=1), notes="Note", location="") # Creates a calendar event
+computer.calendar.create_event(title="Meeting", start_date=datetime.datetime.now(), end_date=datetime.datetime.now() + datetime.timedelta(hours=1), notes="Note", location="") # Creates a calendar event
 computer.calendar.get_events(start_date=datetime.date.today(), end_date=None) # Get events between dates. If end_date is None, only gets events for start_date
 computer.calendar.delete_event(event_title="Meeting", start_date=datetime.datetime) # Delete a specific event with a matching title and start date, you may need to get use get_events() to find the specific event object first
 computer.contacts.get_phone_number("John Doe")
 computer.contacts.get_email_address("John Doe")
 computer.mail.send("john@email.com", "Meeting Reminder", "Reminder that our meeting is at 3pm today.", ["path/to/attachment.pdf", "path/to/attachment2.pdf"]) # Send an email with a optional attachments
 computer.mail.get(4, unread=True) # Returns the {number} of unread emails, or all emails if False is passed
 computer.mail.unread_count() # Returns the number of unread emails
```

### Comparing `open_interpreter-0.2.4/interpreter/core/llm/llm.py` & `open_interpreter-0.2.5/interpreter/core/llm/llm.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         # Store a reference to parent interpreter
         self.interpreter = interpreter
 
         # Chat completions "endpoint"
         self.completions = fixed_litellm_completions
 
         # Settings
-        self.model = "gpt-4"
+        self.model = "gpt-4-turbo"
         self.temperature = 0
         self.supports_vision = False
         self.supports_functions = None  # Will try to auto-detect
 
         # Optional settings
         self.context_window = None
         self.max_tokens = None
@@ -55,28 +55,23 @@
         ), "First message must have the role 'system'"
         for msg in messages[1:]:
             assert (
                 msg["role"] != "system"
             ), "No message after the first can have the role 'system'"
 
         # Detect function support
-        if self.supports_functions != None:
-            supports_functions = self.supports_functions
-        else:
-            # Guess whether or not it's a function calling LLM
-            if not self.interpreter.offline and (
-                self.interpreter.llm.model != "gpt-4-vision-preview"
-                and self.model in litellm.open_ai_chat_completion_models
-                or self.model.startswith("azure/")
-                # Once Litellm supports it, add Anthropic models here
-            ):
-                supports_functions = True
-            else:
-                supports_functions = False
-
+        if self.supports_functions == None:
+            try:
+                if litellm.supports_function_calling(self.model):
+                    self.supports_functions = True
+                else:
+                    self.supports_functions = False
+            except:
+                self.supports_functions = False
+            
         # Trim image messages if they're there
         if self.supports_vision:
             image_messages = [msg for msg in messages if msg["type"] == "image"]
 
             if self.interpreter.os:
                 # Keep only the last two images if the interpreter is running in OS mode
                 if len(image_messages) > 1:
@@ -92,15 +87,15 @@
                         if self.interpreter.verbose:
                             print("Removing image message!")
                 # Idea: we could set detail: low for the middle messages, instead of deleting them
 
         # Convert to OpenAI messages format
         messages = convert_to_openai_messages(
             messages,
-            function_calling=supports_functions,
+            function_calling=self.supports_functions,
             vision=self.supports_vision,
             shrink_images=self.interpreter.shrink_images,
         )
 
         if self.interpreter.debug:
             print("\n\n\nOPENAI COMPATIBLE MESSAGES\n\n\n")
             for message in messages:
@@ -196,15 +191,15 @@
 
         # Set some params directly on LiteLLM
         if self.max_budget:
             litellm.max_budget = self.max_budget
         if self.interpreter.verbose:
             litellm.set_verbose = True
 
-        if supports_functions:
+        if self.supports_functions:
             yield from run_function_calling_llm(self, params)
         else:
             yield from run_text_llm(self, params)
 
 
 def fixed_litellm_completions(**params):
     """
```

### Comparing `open_interpreter-0.2.4/interpreter/core/llm/run_function_calling_llm.py` & `open_interpreter-0.2.5/interpreter/core/llm/run_function_calling_llm.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/llm/run_text_llm.py` & `open_interpreter-0.2.5/interpreter/core/llm/run_text_llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 def run_text_llm(llm, params):
     ## Setup
 
-    try:
-        # Add the system message
-        params["messages"][0][
-            "content"
-        ] += "\nTo execute code on the user's machine, write a markdown code block. Specify the language after the ```. You will receive the output. Use any programming language."
-    except:
-        print('params["messages"][0]', params["messages"][0])
-        raise
+    if llm.interpreter.computer.terminal.languages != []:
+        try:
+            # Add the system message
+            params["messages"][0][
+                "content"
+            ] += "\nTo execute code on the user's machine, write a markdown code block. Specify the language after the ```. You will receive the output. Use any programming language."
+        except:
+            print('params["messages"][0]', params["messages"][0])
+            raise
 
     ## Convert output to LMC format
 
     inside_code_block = False
     accumulated_block = ""
     language = None
```

### Comparing `open_interpreter-0.2.4/interpreter/core/llm/utils/convert_to_openai_messages.py` & `open_interpreter-0.2.5/interpreter/core/llm/utils/convert_to_openai_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,18 +36,18 @@
                 new_message["function_call"] = {
                     "name": "execute",
                     "arguments": json.dumps(
                         {"language": message["format"], "code": message["content"]}
                     ),
                     # parsed_arguments isn't actually an OpenAI thing, it's an OI thing.
                     # but it's soo useful!
-                    "parsed_arguments": {
-                        "language": message["format"],
-                        "code": message["content"],
-                    },
+                    # "parsed_arguments": {
+                    #     "language": message["format"],
+                    #     "code": message["content"],
+                    # },
                 }
                 # Add empty content to avoid error "openai.error.InvalidRequestError: 'content' is a required property - 'messages.*'"
                 # especially for the OpenAI service hosted on Azure
                 new_message["content"] = ""
             else:
                 new_message[
                     "content"
@@ -166,15 +166,16 @@
 
         elif message["type"] == "file":
             new_message = {"role": "user", "content": message["content"]}
 
         else:
             raise Exception(f"Unable to convert this message type: {message}")
 
-        new_message["content"] = new_message["content"].strip()
+        if isinstance(new_message["content"], str):
+            new_message["content"] = new_message["content"].strip()
 
         new_messages.append(new_message)
 
     """
     # Combine adjacent user messages
     combined_messages = []
     i = 0
```

### Comparing `open_interpreter-0.2.4/interpreter/core/llm/utils/merge_deltas.py` & `open_interpreter-0.2.5/interpreter/core/llm/utils/merge_deltas.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/llm/utils/parse_partial_json.py` & `open_interpreter-0.2.5/interpreter/core/llm/utils/parse_partial_json.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/llm/vision_for_text_llms.py` & `open_interpreter-0.2.5/interpreter/core/llm/vision_for_text_llms.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/render_message.py` & `open_interpreter-0.2.5/interpreter/core/render_message.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,34 @@
 import re
-import time
 
 
 def render_message(interpreter, message):
     """
     Renders a dynamic message into a string.
     """
 
     previous_save_skills_setting = interpreter.computer.save_skills
     interpreter.computer.save_skills = False
 
     # Split the message into parts by {{ and }}, including multi-line strings
     parts = re.split(r"({{.*?}})", message, flags=re.DOTALL)
 
-    for i in range(len(parts)):
-        part = parts[i]
+    for i, part in enumerate(parts):
         # If the part is enclosed in {{ and }}
         if part.startswith("{{") and part.endswith("}}"):
             # Run the code inside the brackets
             output = interpreter.computer.run(
                 "python", part[2:-2].strip(), display=interpreter.verbose
             )
 
-            # Turn it into just a simple string
-            outputs = []
-            for line in output:
-                if interpreter.debug:
-                    print(line)
-                if line.get("format") == "output":
-                    if "IGNORE_ALL_ABOVE_THIS_LINE" in line["content"]:
-                        outputs.append(
-                            line["content"].split("IGNORE_ALL_ABOVE_THIS_LINE")[1]
-                        )
-                    else:
-                        outputs.append(line["content"])
-            output = "\n".join(outputs)
+            # Extract the output content
+            outputs = (line["content"] for line in output if line.get("format") == "output" and "IGNORE_ALL_ABOVE_THIS_LINE" not in line["content"])
 
             # Replace the part with the output
-            parts[i] = output
+            parts[i] = "\n".join(outputs)
 
     # Join the parts back into the message
     rendered_message = "".join(parts).strip()
 
     if interpreter.debug:
         print("\n\n\nSYSTEM MESSAGE\n\n\n")
         print(rendered_message)
```

### Comparing `open_interpreter-0.2.4/interpreter/core/respond.py` & `open_interpreter-0.2.5/interpreter/core/respond.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             if (
                 interpreter.offline == False
                 and "auth" in str(e).lower()
                 or "api key" in str(e).lower()
             ):
                 output = traceback.format_exc()
                 raise Exception(
-                    f"{output}\n\nThere might be an issue with your API key(s).\n\nTo reset your API key (we'll use OPENAI_API_KEY for this example, but you may need to reset your ANTHROPIC_API_KEY, HUGGINGFACE_API_KEY, etc):\n        Mac/Linux: 'export OPENAI_API_KEY=your-key-here',\n        Windows: 'setx OPENAI_API_KEY your-key-here' then restart terminal.\n\n"
+                    f"{output}\n\nThere might be an issue with your API key(s).\n\nTo reset your API key (we'll use OPENAI_API_KEY for this example, but you may need to reset your ANTHROPIC_API_KEY, HUGGINGFACE_API_KEY, etc):\n        Mac/Linux: 'export OPENAI_API_KEY=your-key-here'. Update your ~/.zshrc on MacOS or ~/.bashrc on Linux with the new key if it has already been persisted there.,\n        Windows: 'setx OPENAI_API_KEY your-key-here' then restart terminal.\n\n"
                 )
             elif interpreter.offline == False and "not have access" in str(e).lower():
                 response = input(
                     f"  You do not have access to {interpreter.llm.model}. You will need to add a payment method and purchase credits for the OpenAI API billing page (different from ChatGPT) to use `GPT-4`.\n\nhttps://platform.openai.com/account/billing/overview\n\nWould you like to try GPT-3.5-TURBO instead? (y/n)\n\n  "
                 )
                 print("")  # <- Aesthetic choice
 
@@ -182,20 +182,20 @@
                             f"{x.strip()} = computer.{x.strip()}"
                             for x in m.group(1).split(", ")
                         ),
                         code,
                     )
                     code = re.sub(r"import computer\.\w+\n", "pass\n", code)
                     # If it does this it sees the screenshot twice (which is expected jupyter behavior)
-                    if code.split("\n")[-1] in [
-                        "computer.display.view()",
-                        "computer.display.screenshot()",
-                        "computer.view()",
-                        "computer.screenshot()",
-                    ]:
+                    if any(code.split("\n")[-1].startswith(text) for text in [
+                        "computer.display.view",
+                        "computer.display.screenshot",
+                        "computer.view",
+                        "computer.screenshot",
+                    ]):
                         code = code + "\npass"
 
                 # sync up some things (is this how we want to do this?)
                 interpreter.computer.verbose = interpreter.verbose
                 interpreter.computer.debug = interpreter.debug
                 interpreter.computer.emit_images = interpreter.llm.supports_vision
 
@@ -270,15 +270,15 @@
             force_task_completion_breakers = interpreter.force_task_completion_breakers
 
             if (
                 interpreter.force_task_completion
                 and interpreter.messages
                 and interpreter.messages[-1].get("role", "").lower() == "assistant"
                 and not any(
-                    task_status in interpreter.messages[-1].get("content", "")
+                    task_status in interpreter.messages[-1].get("content", "").lower()
                     for task_status in force_task_completion_breakers
                 )
             ):
                 # Remove past force_task_completion_message messages
                 interpreter.messages = [
                     message
                     for message in interpreter.messages
```

### Comparing `open_interpreter-0.2.4/interpreter/core/server.py` & `open_interpreter-0.2.5/interpreter/core/server.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/utils/lazy_import.py` & `open_interpreter-0.2.5/interpreter/core/utils/lazy_import.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/utils/scan_code.py` & `open_interpreter-0.2.5/interpreter/core/utils/scan_code.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/utils/system_debug_info.py` & `open_interpreter-0.2.5/interpreter/core/utils/system_debug_info.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/core/utils/telemetry.py` & `open_interpreter-0.2.5/interpreter/core/utils/telemetry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """
 Sends anonymous telemetry to posthog. This helps us know how people are using OI / what needs our focus.
 
-Disable this by running `interpreter --disable_telemetry` or `interpreter.anonymized_telemetry = False` or setting the `ANONYMIZED_TELEMETRY` os var to `false`.
+Disable anonymous telemetry by execute one of below:
+1. Running `interpreter --disable_telemetry` in command line.
+2. Executing `interpreter.disable_telemetry = True` in Python.
+3. Setting the `DISABLE_TELEMETRY` os var to `true`.
 
 based on ChromaDB's telemetry: https://github.com/chroma-core/chroma/tree/main/chromadb/telemetry/product
 """
 
 import contextlib
 import os
 import uuid
 
 import pkg_resources
 from posthog import Posthog
+import requests
 
 posthog = Posthog(
     "phc_6cmXy4MEbLfNGezqGjuUTY8abLu0sAwtGzZFpQW97lc", host="https://app.posthog.com"
 )
 
 
 def get_or_create_uuid():
@@ -53,7 +57,33 @@
         with open(os.devnull, "w") as f, contextlib.redirect_stdout(
             f
         ), contextlib.redirect_stderr(f):
             posthog.capture(user_id, event_name, properties)
     except:
         # Non blocking
         pass
+
+
+def contribute_conversations(conversations):
+    url = "https://api.openinterpreter.com/v0/conversations/contribute/"
+    version = pkg_resources.get_distribution("open-interpreter").version
+    
+    if conversations and len(conversations) > 1:
+        payload = {
+            "conversations": [conv for sublist in conversations for conv in sublist],
+            "oi_version": version
+        }
+    else:
+        payload = {
+            "conversations": [conversations[0]],
+            "oi_version": version
+        }
+    try:
+        response = requests.post(url, json=payload)
+        if response.status_code != 200:
+            print(f"Failed to contribute conversation: {response.status_code} {response.text}")
+            return None
+        else:
+            print(f"Successfully contributed conversation!")
+    except requests.RequestException as e:
+        print(f"Failed to contribute conversation: {e}")
+        return None
```

### Comparing `open_interpreter-0.2.4/interpreter/core/utils/temporary_file.py` & `open_interpreter-0.2.5/interpreter/core/utils/temporary_file.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/components/base_block.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/components/base_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/components/code_block.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/components/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/components/message_block.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/components/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/conversation_navigator.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/conversation_navigator.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/magic_commands.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/magic_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
     display_markdown_message(f"Jupyter notebook file exported to {os.path.abspath(notebook_path)}")
 
 
 def handle_magic_command(self, user_input):
     # Handle shell
     if user_input.startswith("%%"):
         code = user_input[2:].strip()
-        self.computer.run("shell", code, stream=True, display=True)
+        self.computer.run("shell", code, stream=False, display=True)
         print("")
         return
 
     # split the command into the command and the arguments, by the first whitespace
     switch = {
         "help": handle_help,
         "verbose": handle_verbose,
```

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/profiles/defaults/01.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/profiles/defaults/01.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 # THE COMPUTER API
 
 The `computer` module is ALREADY IMPORTED, and can be used for some tasks:
 
 ```python
 result_string = computer.browser.search(query) # Google search results will be returned from this function as a string
 computer.files.edit(path_to_file, original_text, replacement_text) # Edit a file
-computer.calendar.create_event(title="Meeting", start_date=datetime.datetime.now(), end=datetime.datetime.now() + datetime.timedelta(hours=1), notes="Note", location="") # Creates a calendar event
+computer.calendar.create_event(title="Meeting", start_date=datetime.datetime.now(), end_date=datetime.datetime.now() + datetime.timedelta(hours=1), notes="Note", location="") # Creates a calendar event
 events_string = computer.calendar.get_events(start_date=datetime.date.today(), end_date=None) # Get events between dates. If end_date is None, only gets events for start_date
 computer.calendar.delete_event(event_title="Meeting", start_date=datetime.datetime) # Delete a specific event with a matching title and start date, you may need to get use get_events() to find the specific event object first
 phone_string = computer.contacts.get_phone_number("John Doe")
 contact_string = computer.contacts.get_email_address("John Doe")
 computer.mail.send("john@email.com", "Meeting Reminder", "Reminder that our meeting is at 3pm today.", ["path/to/attachment.pdf", "path/to/attachment2.pdf"]) # Send an email with a optional attachments
 emails_string = computer.mail.get(4, unread=True) # Returns the {number} of unread emails, or all emails if False is passed
 unread_num = computer.mail.unread_count() # Returns the number of unread emails
@@ -86,15 +86,16 @@
 
 # GUI CONTROL (RARE)
 
 You are a computer controlling language model. You can control the user's GUI.
 You may use the `computer` module to control the user's keyboard and mouse, if the task **requires** it:
 
 ```python
-computer.display.view() # Shows you what's on the screen, returns a `pil_image` `in case you need it (rarely). **You almost always want to do this first!**
+computer.display.info() # Returns a list of connected monitors/Displays and their info (x and y cordinates, width, height, width_mm, height_mm, name). Use this to verify the monitors connected before using computer.display.view() when neccessary
+computer.display.view() # Shows you what's on the screen (primary display by default), returns a `pil_image` `in case you need it (rarely). To get a specific display, use the parameter screen=DISPLAY_NUMBER (0 for primary monitor 1 and above for secondary monitors). **You almost always want to do this first!**
 computer.keyboard.hotkey(" ", "command") # Opens spotlight
 computer.keyboard.write("hello")
 computer.mouse.click("text onscreen") # This clicks on the UI element with that text. Use this **frequently** and get creative! To click a video, you could pass the *timestamp* (which is usually written on the thumbnail) into this.
 computer.mouse.move("open recent >") # This moves the mouse over the UI element with that text. Many dropdowns will disappear if you click them. You have to hover over items to reveal more.
 computer.mouse.click(x=500, y=500) # Use this very, very rarely. It's highly inaccurate
 computer.mouse.click(icon="gear icon") # Moves mouse to the icon with that description. Use this very often
 computer.mouse.scroll(-10) # Scrolls down. If you don't find some text on screen that you expected to be there, you probably want to do this
@@ -211,15 +212,15 @@
     user_input = input("(y/n) > ")
     if user_input.lower() != "y":
         print("\nPlease try to install them manually.\n\n")
         time.sleep(2)
         print("Attempting to start OS control anyway...\n\n")
 
     for pip_name in ["pip", "pip3"]:
-        command = f"{pip_name} install 'open-interpreter[os]'"
+        command = f"{pip_name} install open-interpreter[os]"
 
         interpreter.computer.run("shell", command, display=True)
 
         got_em = True
         for package in missing_packages:
             try:
                 __import__(package)
```

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/profiles/defaults/default.yaml` & `open_interpreter-0.2.5/interpreter/terminal_interface/profiles/defaults/default.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 ### OPEN INTERPRETER CONFIGURATION FILE
 
 # Remove the "#" before the settings below to use them.
 
+# LLM Settings
 llm:
-  model: "gpt-4"
+  model: "gpt-4-turbo"
   temperature: 0
   # api_key: ...  # Your API key, if the API requires it
   # api_base: ...  # The URL where an OpenAI-compatible server is running to handle LLM API requests
   # api_version: ...  # The version of the API (this is primarily for Azure)
   # max_output: 2500  # The maximum characters of code output visible to the LLM
+
+# Custom Instructions
 # custom_instructions: ""  # This will be appended to the system message
+
+# General Configuration
 # auto_run: False  # If True, code will run without asking for confirmation
 # safe_mode: "off"  # The safety mode for the LLM — one of "off", "ask", "auto"
 # offline: False  # If True, will disable some online features like checking for updates
 # verbose: False  # If True, will print detailed logs
 # multi_line: False # If True, you can input multiple lines starting and ending with ```
 
+# Documentation
 # All options: https://docs.openinterpreter.com/settings
```

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/profiles/defaults/fast.yaml` & `open_interpreter-0.2.5/interpreter/terminal_interface/profiles/defaults/fast.yaml`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/profiles/defaults/local.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/profiles/defaults/local.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,159 +1,190 @@
-import sys
 import os
 import platform
 import subprocess
+import sys
 import time
 import inquirer
-
 from interpreter import interpreter
 
+
+def get_ram():
+    import psutil
+
+    total_ram = psutil.virtual_memory().total / (
+        1024 * 1024 * 1024
+    )  # Convert bytes to GB
+    return total_ram
+
 def download_model(models_dir, models, interpreter):
     # For some reason, these imports need to be inside the function
     import inquirer
-    import wget
     import psutil
+    import wget
 
     # Get RAM and disk information
-    total_ram = psutil.virtual_memory().total / (1024 * 1024 * 1024)  # Convert bytes to GB
-    free_disk_space =  psutil.disk_usage('/').free / (1024 * 1024 * 1024)  # Convert bytes to GB
-    
+    total_ram = get_ram()
+    free_disk_space = psutil.disk_usage("/").free / (
+        1024 * 1024 * 1024
+    )  # Convert bytes to GB
+
     time.sleep(1)
-    
+
     # Display the users hardware specs
-    interpreter.display_message(f"Your machine has `{total_ram:.2f}GB` of RAM, and `{free_disk_space:.2f}GB` of free storage space.")
-    
+    interpreter.display_message(
+        f"Your machine has `{total_ram:.2f}GB` of RAM, and `{free_disk_space:.2f}GB` of free storage space."
+    )
+
     time.sleep(2)
-    
+
     if total_ram < 10:
-        interpreter.display_message(f"\nYour computer realistically can only run smaller models less than 4GB, Phi-2 might be the best model for your computer.\n")
+        interpreter.display_message(
+            f"\nYour computer realistically can only run smaller models less than 4GB, Phi-2 might be the best model for your computer.\n"
+        )
     elif 10 <= total_ram < 30:
-        interpreter.display_message(f"\nYour computer could handle a mid-sized model (4-10GB), Mistral-7B might be the best model for your computer.\n")
+        interpreter.display_message(
+            f"\nYour computer could handle a mid-sized model (4-10GB), Mistral-7B might be the best model for your computer.\n"
+        )
     else:
-        interpreter.display_message(f"\nYour computer should have enough RAM to run any model below.\n")
-    
-    
+        interpreter.display_message(
+            f"\nYour computer should have enough RAM to run any model below.\n"
+        )
+
     time.sleep(1)
-    
-    interpreter.display_message(f"In general, the larger the model, the better the performance, but choose a model that best fits your computer's hardware. \nOnly models you have the storage space to download are shown:\n")
-    
+
+    interpreter.display_message(
+        f"In general, the larger the model, the better the performance, but choose a model that best fits your computer's hardware. \nOnly models you have the storage space to download are shown:\n"
+    )
+
     time.sleep(1)
-    
+
     try:
         model_list = [
             {
                 "name": "TinyLlama-1.1B",
                 "file_name": "TinyLlama-1.1B-Chat-v1.0.Q5_K_M.llamafile",
                 "size": 0.76,
-                "url": "https://huggingface.co/jartine/TinyLlama-1.1B-Chat-v1.0-GGUF/resolve/main/TinyLlama-1.1B-Chat-v1.0.Q5_K_M.llamafile?download=true"
+                "url": "https://huggingface.co/jartine/TinyLlama-1.1B-Chat-v1.0-GGUF/resolve/main/TinyLlama-1.1B-Chat-v1.0.Q5_K_M.llamafile?download=true",
             },
             {
                 "name": "Rocket-3B",
                 "file_name": "rocket-3b.Q5_K_M.llamafile",
                 "size": 1.89,
-                "url": "https://huggingface.co/jartine/rocket-3B-llamafile/resolve/main/rocket-3b.Q5_K_M.llamafile?download=true"
+                "url": "https://huggingface.co/jartine/rocket-3B-llamafile/resolve/main/rocket-3b.Q5_K_M.llamafile?download=true",
             },
             {
                 "name": "Phi-2",
                 "file_name": "phi-2.Q5_K_M.llamafile",
                 "size": 1.96,
-                "url": "https://huggingface.co/jartine/phi-2-llamafile/resolve/main/phi-2.Q5_K_M.llamafile?download=true"
+                "url": "https://huggingface.co/jartine/phi-2-llamafile/resolve/main/phi-2.Q5_K_M.llamafile?download=true",
             },
             {
                 "name": "LLaVA 1.5",
                 "file_name": "llava-v1.5-7b-q4.llamafile",
                 "size": 3.97,
-                "url": "https://huggingface.co/jartine/llava-v1.5-7B-GGUF/resolve/main/llava-v1.5-7b-q4.llamafile?download=true"
+                "url": "https://huggingface.co/jartine/llava-v1.5-7B-GGUF/resolve/main/llava-v1.5-7b-q4.llamafile?download=true",
             },
             {
                 "name": "Mistral-7B-Instruct",
                 "file_name": "mistral-7b-instruct-v0.2.Q5_K_M.llamafile",
                 "size": 5.15,
-                "url": "https://huggingface.co/jartine/Mistral-7B-Instruct-v0.2-llamafile/resolve/main/mistral-7b-instruct-v0.2.Q5_K_M.llamafile?download=true"
+                "url": "https://huggingface.co/jartine/Mistral-7B-Instruct-v0.2-llamafile/resolve/main/mistral-7b-instruct-v0.2.Q5_K_M.llamafile?download=true",
             },
             {
                 "name": "WizardCoder-Python-13B",
                 "file_name": "wizardcoder-python-13b.llamafile",
                 "size": 7.33,
-                "url": "https://huggingface.co/jartine/wizardcoder-13b-python/resolve/main/wizardcoder-python-13b.llamafile?download=true"
+                "url": "https://huggingface.co/jartine/wizardcoder-13b-python/resolve/main/wizardcoder-python-13b.llamafile?download=true",
             },
             {
                 "name": "WizardCoder-Python-34B",
                 "file_name": "wizardcoder-python-34b-v1.0.Q5_K_M.llamafile",
                 "size": 22.23,
-                "url": "https://huggingface.co/jartine/WizardCoder-Python-34B-V1.0-llamafile/resolve/main/wizardcoder-python-34b-v1.0.Q5_K_M.llamafile?download=true"
+                "url": "https://huggingface.co/jartine/WizardCoder-Python-34B-V1.0-llamafile/resolve/main/wizardcoder-python-34b-v1.0.Q5_K_M.llamafile?download=true",
             },
             {
                 "name": "Mixtral-8x7B-Instruct",
                 "file_name": "mixtral-8x7b-instruct-v0.1.Q5_K_M.llamafile",
                 "size": 30.03,
-                "url": "https://huggingface.co/jartine/Mixtral-8x7B-Instruct-v0.1-llamafile/resolve/main/mixtral-8x7b-instruct-v0.1.Q5_K_M.llamafile?download=true"
-            }
+                "url": "https://huggingface.co/jartine/Mixtral-8x7B-Instruct-v0.1-llamafile/resolve/main/mixtral-8x7b-instruct-v0.1.Q5_K_M.llamafile?download=true",
+            },
         ]
-        
+
         # Filter models based on available disk space and RAM
-        filtered_models = [model for model in model_list if model["size"] <= free_disk_space and model["file_name"] not in models]
+        filtered_models = [
+            model
+            for model in model_list
+            if model["size"] <= free_disk_space and model["file_name"] not in models
+        ]
         if filtered_models:
-            
             time.sleep(1)
-            
+
             # Prompt the user to select a model
             model_choices = [
-                f"{model['name']} ({model['size']:.2f}GB)"
-                for model in filtered_models
+                f"{model['name']} ({model['size']:.2f}GB)" for model in filtered_models
             ]
             questions = [
                 inquirer.List(
                     "model",
                     message="Select a model to download:",
-                    choices=model_choices
+                    choices=model_choices,
                 )
             ]
             answers = inquirer.prompt(questions)
-            
+
             # Get the selected model
-            selected_model = next(model for model in filtered_models if f"{model['name']} ({model['size']}GB)" == answers["model"])
-            
+            selected_model = next(
+                model
+                for model in filtered_models
+                if f"{model['name']} ({model['size']}GB)" == answers["model"]
+            )
+
             # Download the selected model
             model_url = selected_model["url"]
             # Extract the basename and remove query parameters
-            filename = os.path.basename(model_url).split('?')[0]
+            filename = os.path.basename(model_url).split("?")[0]
             model_path = os.path.join(models_dir, filename)
-            
+
             time.sleep(1)
             print(f"\nDownloading {selected_model['name']}...\n")
             wget.download(model_url, model_path)
-            
+
             # Make the model executable if not on Windows
             if platform.system() != "Windows":
                 subprocess.run(["chmod", "+x", model_path], check=True)
-                
+
             print(f"\nModel '{selected_model['name']}' downloaded successfully.\n")
-            
-            interpreter.display_message("To view or delete downloaded local models, run `interpreter --local_models`\n\n")
-            
+
+            interpreter.display_message(
+                "To view or delete downloaded local models, run `interpreter --local_models`\n\n"
+            )
+
             return model_path
         else:
-            print("\nYour computer does not have enough storage to download any local LLMs.\n")
+            print(
+                "\nYour computer does not have enough storage to download any local LLMs.\n"
+            )
             return None
     except Exception as e:
         print(e)
-        print("\nAn error occurred while trying to download the model. Please try again or use a different local model provider.\n")
+        print(
+            "\nAn error occurred while trying to download the model. Please try again or use a different local model provider.\n"
+        )
         return None
 
 
-
-
 # START OF LOCAL MODEL PROVIDER LOGIC
-interpreter.display_message("> Open Interpreter is compatible with several local model providers.\n")
+interpreter.display_message(
+    "> Open Interpreter is compatible with several local model providers.\n"
+)
 
 # Define the choices for local models
 choices = [
-    "Llamafile",
     "Ollama",
+    "Llamafile",
     "LM Studio",
     "Jan",
 ]
 
 # Use inquirer to let the user select an option
 questions = [
     inquirer.List(
@@ -179,63 +210,84 @@
 4. Select your model at the top, then click **Start Server**.
 
 
 Once the server is running, you can begin your conversation below.
 
 """
     )
-    
+    interpreter.llm.supports_functions = False
     interpreter.llm.api_base = "http://localhost:1234/v1"
-    interpreter.llm.max_tokens = 1000
-    interpreter.llm.context_window = 3000
     interpreter.llm.api_key = "x"
 
 elif selected_model == "Ollama":
     try:
-        
         # List out all downloaded ollama models. Will fail if ollama isn't installed
-        result = subprocess.run(["ollama", "list"], capture_output=True, text=True, check=True)
-        lines = result.stdout.split('\n')
-        names = [line.split()[0].replace(":latest", "") for line in lines[1:] if line.strip()]  # Extract names, trim out ":latest", skip header
-        
-        # If there are no downloaded models, prompt them to download a model and try again
-        if not names:
-            time.sleep(1)
-            
-            interpreter.display_message(f"\nYou don't have any Ollama models downloaded. To download a new model, run `ollama run <model-name>`, then start a new interpreter session. \n\n For a full list of downloadable models, check out [https://ollama.com/library](https://ollama.com/library) \n")
-            
-            print("Please download a model then try again\n")
-            time.sleep(2)
-            sys.exit(1)
-        
+        def list_ollama_models():
+            result = subprocess.run(
+                ["ollama", "list"], capture_output=True, text=True, check=True
+            )
+            lines = result.stdout.split("\n")
+            names = [
+                line.split()[0].replace(":latest", "")
+                for line in lines[1:]
+                if line.strip()
+            ]  # Extract names, trim out ":latest", skip header
+            return names
+
+        llama3_installed = True
+        names = list_ollama_models()
+        if "llama3" not in names:
+            # If a user has other models installed but not llama3, let's display the correct message
+            if not names:
+                llama3_installed = False
+            names.insert(0, "llama3")
+
         # If there are models, prompt them to select one
-        else:
-            time.sleep(1)
-            interpreter.display_message(f"**{len(names)} Ollama model{'s' if len(names) != 1 else ''} found.** To download a new model, run `ollama run <model-name>`, then start a new interpreter session. \n\n For a full list of downloadable models, check out [https://ollama.com/library](https://ollama.com/library) \n")
+        time.sleep(1)
+
+        if llama3_installed:
+            interpreter.display_message(
+                f"**{len(names)} Ollama model{'s' if len(names) != 1 else ''} found.** To download a new model, run `ollama run <model-name>`, then start a new interpreter session. \n\n For a full list of downloadable models, check out [https://ollama.com/library](https://ollama.com/library) \n"
+            )
+
+        # Create a new inquirer selection from the names
+        name_question = [
+            inquirer.List(
+                "name",
+                message="Select a downloaded Ollama model:"
+                if llama3_installed
+                else "No models found. Select a model to install:",
+                choices=names,
+            ),
+        ]
+        name_answer = inquirer.prompt(name_question)
+        selected_name = name_answer["name"] if name_answer else None
+
+        if selected_name is "llama3":
+            # If the user selects llama3, we need to check if it's installed, and if not, install it
+            all_models = list_ollama_models()
+            if "llama3" not in all_models:
+                interpreter.display_message(f"\nDownloading Llama3...\n")
+                subprocess.run(["ollama", "pull", "llama3"], check=True)
+
+        # Set the model to the selected model
+        interpreter.llm.model = f"ollama/{selected_name}"
+        interpreter.display_message(f"\nUsing Ollama model: `{selected_name}` \n")
+        time.sleep(1)
 
-            # Create a new inquirer selection from the names
-            name_question = [
-                inquirer.List('name', message="Select a downloaded Ollama model", choices=names),
-            ]
-            name_answer = inquirer.prompt(name_question)
-            selected_name = name_answer['name'] if name_answer else None
-            
-            # Set the model to the selected model
-            interpreter.llm.model = f"ollama/{selected_name}"
-            interpreter.display_message(f"\nUsing Ollama model: `{selected_name}` \n")
-            time.sleep(1)
-        
     # If Ollama is not installed or not recognized as a command, prompt the user to download Ollama and try again
     except (subprocess.CalledProcessError, FileNotFoundError) as e:
         print("Ollama is not installed or not recognized as a command.")
         time.sleep(1)
-        interpreter.display_message(f"\nPlease visit [https://ollama.com/](https://ollama.com/) to download Ollama and try again\n")
+        interpreter.display_message(
+            f"\nPlease visit [https://ollama.com/](https://ollama.com/) to download Ollama and try again\n"
+        )
         time.sleep(2)
         sys.exit(1)
-        
+
 elif selected_model == "Jan":
     interpreter.display_message(
         """
 To use use Open Interpreter with **Jan**, you will need to run **Jan** in the background.
 
 1. Download **Jan** from [https://jan.ai/](https://jan.ai/), then start it.
 2. Select a language model from the "Hub" tab, then click **Download**.
@@ -244,78 +296,85 @@
 
 
 Once the server is running, enter the id of the model below, then you can begin your conversation below.
 
 """
     )
     interpreter.llm.api_base = "http://localhost:1337/v1"
-    interpreter.llm.max_tokens = 1000
-    interpreter.llm.context_window = 3000
     time.sleep(1)
-    
+
     # Prompt the user to enter the name of the model running on Jan
     model_name_question = [
-        inquirer.Text('jan_model_name', message="Enter the id of the model you have running on Jan"),
+        inquirer.Text(
+            "jan_model_name",
+            message="Enter the id of the model you have running on Jan",
+        ),
     ]
     model_name_answer = inquirer.prompt(model_name_question)
-    jan_model_name = model_name_answer['jan_model_name'] if model_name_answer else None
+    jan_model_name = model_name_answer["jan_model_name"] if model_name_answer else None
     interpreter.llm.model = f"jan/{jan_model_name}"
     interpreter.display_message(f"\nUsing Jan model: `{jan_model_name}` \n")
     time.sleep(1)
-    
-    
 
-elif selected_model == "Llamafile":
 
+elif selected_model == "Llamafile":
     if platform.system() == "Darwin":  # Check if the system is MacOS
         result = subprocess.run(
             ["xcode-select", "-p"], stdout=subprocess.PIPE, stderr=subprocess.STDOUT
         )
         if result.returncode != 0:
             interpreter.display_message(
                 "To use Llamafile, Open Interpreter requires Mac users to have Xcode installed. You can install Xcode from https://developer.apple.com/xcode/ .\n\nAlternatively, you can use `LM Studio`, `Jan.ai`, or `Ollama` to manage local language models. Learn more at https://docs.openinterpreter.com/guides/running-locally ."
             )
             time.sleep(3)
-            raise Exception("Xcode is not installed. Please install Xcode and try again.")
+            raise Exception(
+                "Xcode is not installed. Please install Xcode and try again."
+            )
 
     # Define the path to the models directory
     models_dir = os.path.join(interpreter.get_oi_dir(), "models")
 
     # Check and create the models directory if it doesn't exist
     if not os.path.exists(models_dir):
         os.makedirs(models_dir)
 
     # Check if there are any models in the models folder
     models = [f for f in os.listdir(models_dir) if f.endswith(".llamafile")]
 
     if not models:
         print("\nThere are no models currently downloaded. Let's download a new one.\n")
-        model_path = download_model(models_dir,  models, interpreter)
+        model_path = download_model(models_dir, models, interpreter)
     else:
         # Prompt the user to select a downloaded model or download a new one
         model_choices = models + [" ↓ Download new model"]
         questions = [
             inquirer.List(
                 "model",
                 message="Select a Llamafile model to run or download a new one:",
-                choices=model_choices
+                choices=model_choices,
             )
         ]
         answers = inquirer.prompt(questions)
-        
+
         if answers["model"] == " ↓ Download new model":
             model_path = download_model(models_dir, models, interpreter)
         else:
             model_path = os.path.join(models_dir, answers["model"])
-            
+
         if model_path:
             try:
                 # Run the selected model and hide its output
-                process = subprocess.Popen(f'"{model_path}" ' + " ".join(["--nobrowser", "-ngl", "9999"]), shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, text=True)
-                
+                process = subprocess.Popen(
+                    f'"{model_path}" ' + " ".join(["--nobrowser", "-ngl", "9999"]),
+                    shell=True,
+                    stdout=subprocess.PIPE,
+                    stderr=subprocess.STDOUT,
+                    text=True,
+                )
+
                 print("Waiting for the model to load...")
                 for line in process.stdout:
                     if "llama server listening at http://127.0.0.1:8080" in line:
                         print("\nModel loaded \n")
                         time.sleep(1)
                         break  # Exit the loop once the server is ready
             except Exception as e:
@@ -323,18 +382,35 @@
                 print(e)
                 print("Model process terminated.")
 
     # Set flags for Llamafile to work with interpreter
     interpreter.llm.model = "local"
     interpreter.llm.temperature = 0
     interpreter.llm.api_base = "http://localhost:8080/v1"
-    interpreter.llm.max_tokens = 1000
-    interpreter.llm.context_window = 3000
     interpreter.llm.supports_functions = False
 
+user_ram = get_ram()
+# Set context window and max tokens for all local models based on the users available RAM
+if user_ram and user_ram > 9:
+    interpreter.llm.max_tokens = 1200
+    interpreter.llm.context_window = 8000
+else:
+    interpreter.llm.max_tokens = 1000
+    interpreter.llm.context_window = 3000
 # Set the system message to a minimal version for all local models.
-interpreter.system_message = "You are Open Interpreter, a world-class programmer that can execute code on the user's machine."
+interpreter.system_message = """
+You are Open Interpreter, a world-class programmer that can execute code on the user's machine.
+First, list all of the information you know related to the user's request.
+Next, write a plan. **Always recap the plan between each code block** (you have extreme short-term memory loss, so you need to recap the plan between each message block to retain it).
+The code you write must be able to be executed as is. Invalid syntax will cause a catastrophic failure. Do not include the language of the code in the response.
+When you execute code, it will be executed **on the user's machine**. The user has given you **full and complete permission** to execute any code necessary to complete the task. Execute the code.
+You can access the internet. Run **any code** to achieve the goal, and if at first you don't succeed, try again and again.
+You can install new packages.
+When a user refers to a filename, they're likely referring to an existing file in the directory you're currently executing code in.
+Write messages to the user in Markdown.
+In general, try to **make plans** with as few steps as possible. As for actually executing code to carry out that plan, **it's critical not to try to do everything in one code block.** You should try something, print information about it, then continue from there in tiny, informed steps. You will never get it on the first try, and attempting it in one go will often lead to errors you cant see.
+You are capable of **any** task.
+Once you have accomplished the task, ask the user if they are happy with the result and wait for their response. It is very important to get feedback from the user. 
+The user will tell you the next task after you ask them.
+"""
 # Set offline for all local models
 interpreter.offline = True
-
-
-
```

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/profiles/defaults/os.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/profiles/defaults/os.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 interpreter.llm.model = "gpt-4-vision-preview"
 
 interpreter.llm.supports_functions = False
 interpreter.llm.context_window = 110000
 interpreter.llm.max_tokens = 4096
 interpreter.auto_run = True
 interpreter.force_task_completion = True
+interpreter.sync_computer = True
 
 interpreter.system_message = r"""
 
 You are Open Interpreter, a world-class programmer that can complete any goal by executing code.
 
 When you write code, it will be executed **on the user's machine**. The user has given you **full and complete permission** to execute any code necessary to complete the task.
 
@@ -31,15 +32,16 @@
 # Computer
 
 You may use the `computer` Python module to complete tasks:
 
 ```python
 computer.browser.search(query) # Silently searches Google for the query, returns result. The user's browser is unaffected. (does not open a browser!)
 
-computer.display.view() # Shows you what's on the screen, returns a `pil_image` `in case you need it (rarely). **You almost always want to do this first!**
+computer.display.info() # Returns a list of connected monitors/Displays and their info (x and y cordinates, width, height, width_mm, height_mm, name). Use this to verify the monitors connected before using computer.display.view() when neccessary
+computer.display.view() # Shows you what's on the screen (primary display by default), returns a `pil_image` `in case you need it (rarely). To get a specific display, use the parameter screen=DISPLAY_NUMBER (0 for primary monitor 1 and above for secondary monitors). **You almost always want to do this first!**
 
 computer.keyboard.hotkey(" ", "command") # Opens spotlight (very useful)
 computer.keyboard.write("hello")
 
 # Use this to click text:
 computer.mouse.click("text onscreen") # This clicks on the UI element with that text. Use this **frequently** and get creative! To click a video, you could pass the *timestamp* (which is usually written on the thumbnail) into this.
 # Use this to click an icon, button, or other symbol:
@@ -56,15 +58,15 @@
 
 {{
 import platform
 if platform.system() == 'Darwin':
         print('''
 computer.browser.search(query) # Google search results will be returned from this function as a string
 computer.files.edit(path_to_file, original_text, replacement_text) # Edit a file
-computer.calendar.create_event(title="Meeting", start_date=datetime.datetime.now(), end=datetime.datetime.now() + datetime.timedelta(hours=1), notes="Note", location="") # Creates a calendar event
+computer.calendar.create_event(title="Meeting", start_date=datetime.datetime.now(), end_date=datetime.datetime.now() + datetime.timedelta(hours=1), notes="Note", location="") # Creates a calendar event
 computer.calendar.get_events(start_date=datetime.date.today(), end_date=None) # Get events between dates. If end_date is None, only gets events for start_date
 computer.calendar.delete_event(event_title="Meeting", start_date=datetime.datetime) # Delete a specific event with a matching title and start date, you may need to get use get_events() to find the specific event object first
 computer.contacts.get_phone_number("John Doe")
 computer.contacts.get_email_address("John Doe")
 computer.mail.send("john@email.com", "Meeting Reminder", "Reminder that our meeting is at 3pm today.", ["path/to/attachment.pdf", "path/to/attachment2.pdf"]) # Send an email with a optional attachments
 computer.mail.get(4, unread=True) # Returns the {number} of unread emails, or all emails if False is passed
 computer.mail.unread_count() # Returns the number of unread emails
@@ -164,15 +166,15 @@
     user_input = input("(y/n) > ")
     if user_input.lower() != "y":
         print("\nPlease try to install them manually.\n\n")
         time.sleep(2)
         print("Attempting to start OS control anyway...\n\n")
 
     for pip_name in ["pip", "pip3"]:
-        command = f"{pip_name} install 'open-interpreter[os]'"
+        command = f"{pip_name} install open-interpreter[os]"
 
         interpreter.computer.run("shell", command, display=True)
 
         got_em = True
         for package in missing_packages:
             try:
                 __import__(package)
```

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/profiles/defaults/vision.yaml` & `open_interpreter-0.2.5/interpreter/terminal_interface/profiles/defaults/vision.yaml`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/profiles/profiles.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/profiles/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 oi_default_profiles_path = os.path.join(here, "defaults")
 default_profiles_paths = glob.glob(os.path.join(oi_default_profiles_path, "*"))
 default_profiles_names = [os.path.basename(path) for path in default_profiles_paths]
 
 # Constant to hold the version number
-OI_VERSION = "0.2.1"
+OI_VERSION = "0.2.5"
 
 
 def profile(interpreter, filename_or_url):
     # See if they're doing shorthand for a default profile
     filename_without_extension = os.path.splitext(filename_or_url)[0]
     for profile in default_profiles_names:
         if filename_without_extension == os.path.splitext(profile)[0]:
@@ -151,20 +151,40 @@
         "version" not in profile or profile["version"] != OI_VERSION
     ):  # Remember to update this version number at the top of the file ^
         print("")
         print(
             "We have updated our profile file format. Would you like to migrate your profile file to the new format? No data will be lost."
         )
         print("")
-        message = input("(y/n): ")
+        message = input("(y/n) ")
         print("")
         if message.lower() == "y":
             migrate_user_app_directory()
             print("Migration complete.")
             print("")
+            if profile_path.endswith("default.yaml"):
+                with open(profile_path, "r") as file:
+                    text = file.read()
+                text = text.replace(
+                    "version: " + str(profile["version"]), f"version: {OI_VERSION}"
+                )
+
+                try:
+                    if profile["llm"]["model"] == "gpt-4":
+                        text = text.replace("gpt-4", "gpt-4-turbo")
+                        profile["llm"]["model"] = "gpt-4-turbo"
+                    elif profile["llm"]["model"] == "gpt-4-turbo-preview":
+                        text = text.replace("gpt-4-turbo-preview", "gpt-4-turbo")
+                        profile["llm"]["model"] = "gpt-4-turbo"
+                except:
+                    raise
+                    pass  # fine
+
+                with open(profile_path, "w") as file:
+                    file.write(text)
         else:
             print("Skipping loading profile...")
             print("")
             # If the migration is skipped, add the version number to the end of the file
             if profile_path.endswith("default.yaml"):
                 with open(profile_path, "a") as file:
                     file.write(
@@ -545,28 +565,29 @@
             apply_profile_to_object(getattr(obj, key), value)
         else:
             setattr(obj, key, value)
 
 
 def open_storage_dir(directory):
     dir = os.path.join(oi_dir, directory)
-    
+
     print(f"Opening {directory} directory ({dir})...")
 
     if platform.system() == "Windows":
         os.startfile(dir)
     else:
         try:
             # Try using xdg-open on non-Windows platforms
             subprocess.call(["xdg-open", dir])
         except FileNotFoundError:
             # Fallback to using 'open' on macOS if 'xdg-open' is not available
             subprocess.call(["open", dir])
     return
 
+
 def reset_profile(specific_default_profile=None):
     if (
         specific_default_profile
         and specific_default_profile not in default_profiles_names
     ):
         raise ValueError(
             f"The specific default profile '{specific_default_profile}' is not a default profile."
@@ -607,17 +628,15 @@
                     )
             if not create_oi_directory:
                 print(f"{filename} has been reset.")
         else:
             with open(target_file, "r") as file:
                 current_profile = file.read()
             if current_profile not in historical_profiles:
-                user_input = input(
-                    f"Would you like to reset/update {filename}? (y/n): "
-                )
+                user_input = input(f"Would you like to reset/update {filename}? (y/n) ")
                 if user_input.lower() == "y":
                     send2trash.send2trash(
                         target_file
                     )  # This way, people can recover it from the trash
                     shutil.copy(default_yaml_file, target_file)
                     print(f"{filename} has been reset.")
                 else:
```

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/render_past_conversation.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/render_past_conversation.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/start_terminal_interface.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/start_terminal_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,17 +140,16 @@
             "attribute": {"object": interpreter, "attr_name": "force_task_completion"},
         },
         {
             "name": "disable_telemetry",
             "nickname": "dt",
             "help_text": "disables sending of basic anonymous usage stats",
             "type": bool,
-            "default": True,
-            "action": "store_false",
-            "attribute": {"object": interpreter, "attr_name": "anonymous_telemetry"},
+            "default": False,
+            "attribute": {"object": interpreter, "attr_name": "disable_telemetry"},
         },
         {
             "name": "offline",
             "nickname": "o",
             "help_text": "turns off all online features (except the language model, if it's hosted)",
             "type": bool,
             "attribute": {"object": interpreter, "attr_name": "offline"},
@@ -248,76 +247,73 @@
     for old_flag, new_flag in deprecated_flags.items():
         if old_flag in sys.argv:
             print(f"\n`{old_flag}` has been renamed to `{new_flag}`.\n")
             time.sleep(1.5)
             sys.argv.remove(old_flag)
             sys.argv.append(new_flag)
 
-    parser = argparse.ArgumentParser(description="Open Interpreter")
+    parser = argparse.ArgumentParser(
+        description="Open Interpreter", usage="%(prog)s [options]"
+    )
 
     # Add arguments
     for arg in arguments:
+        default = arg.get("default")
         action = arg.get("action", "store_true")
         nickname = arg.get("nickname")
-        default = arg.get("default")
+
+        name_or_flags = [f'--{arg["name"]}']
+        if nickname:
+            name_or_flags.append(f"-{nickname}")
+
+        # Construct argument name flags
+        flags = (
+            [f"-{nickname}", f'--{arg["name"]}'] if nickname else [f'--{arg["name"]}']
+        )
 
         if arg["type"] == bool:
-            if nickname:
-                parser.add_argument(
-                    f"-{nickname}",
-                    f'--{arg["name"]}',
-                    dest=arg["name"],
-                    help=arg["help_text"],
-                    action=action,
-                    default=default,
-                )
-            else:
-                parser.add_argument(
-                    f'--{arg["name"]}',
-                    dest=arg["name"],
-                    help=arg["help_text"],
-                    action=action,
-                    default=default,
-                )
+            parser.add_argument(
+                *flags,
+                dest=arg["name"],
+                help=arg["help_text"],
+                action=action,
+                default=default,
+            )
         else:
             choices = arg.get("choices")
-
-            if nickname:
-                parser.add_argument(
-                    f"-{nickname}",
-                    f'--{arg["name"]}',
-                    dest=arg["name"],
-                    help=arg["help_text"],
-                    type=arg["type"],
-                    choices=choices,
-                    default=default,
-                    nargs=arg.get("nargs"),
-                )
-            else:
-                parser.add_argument(
-                    f'--{arg["name"]}',
-                    dest=arg["name"],
-                    help=arg["help_text"],
-                    type=arg["type"],
-                    choices=choices,
-                    default=default,
-                    nargs=arg.get("nargs"),
-                )
-
-    args = parser.parse_args()
+            parser.add_argument(
+                *flags,
+                dest=arg["name"],
+                help=arg["help_text"],
+                type=arg["type"],
+                choices=choices,
+                default=default,
+                nargs=arg.get("nargs"),
+            )
+
+    args, unknown_args = parser.parse_known_args()
+
+    # handle unknown arguments
+    if unknown_args:
+        print(f"\nUnrecognized argument(s): {unknown_args}")
+        parser.print_usage()
+        print(
+            "For detailed documentation of supported arguments, please visit: https://docs.openinterpreter.com/settings/all-settings"
+        )
+        sys.exit(1)
 
     if args.profiles:
         open_storage_dir("profiles")
         return
 
     if args.local_models:
         open_storage_dir("models")
         return
 
-    if args.reset_profile != "NOT_PROVIDED":
+    if args.reset_profile is not None and args.reset_profile != "NOT_PROVIDED":
         reset_profile(
             args.reset_profile
         )  # This will be None if they just ran `--reset_profile`
         return
 
     if args.version:
         version = pkg_resources.get_distribution("open-interpreter").version
@@ -345,31 +341,47 @@
 
     ### Set attributes on interpreter, so that a profile script can read the arguments passed in via the CLI
 
     set_attributes(args, arguments)
 
     ### Apply profile
 
-    interpreter = profile(interpreter, args.profile)
+    interpreter = profile(interpreter, args.profile or get_argument_dictionary(arguments, "profile")["default"])
 
     ### Set attributes on interpreter, because the arguments passed in via the CLI should override profile
 
     set_attributes(args, arguments)
 
     ### Set some helpful settings we know are likely to be true
 
-    if interpreter.llm.model == "gpt-4-1106-preview":
+    if interpreter.llm.model == "gpt-4" or interpreter.llm.model == "openai/gpt-4":
         if interpreter.llm.context_window is None:
-            interpreter.llm.context_window = 128000
+            interpreter.llm.context_window = 6500
         if interpreter.llm.max_tokens is None:
             interpreter.llm.max_tokens = 4096
         if interpreter.llm.supports_functions is None:
-            interpreter.llm.supports_functions = True
+            interpreter.llm.supports_functions = (
+                False if "vision" in interpreter.llm.model else True
+            )
 
-    if interpreter.llm.model == "gpt-3.5-turbo-1106":
+    elif interpreter.llm.model.startswith("gpt-4") or interpreter.llm.model.startswith(
+        "openai/gpt-4"
+    ):
+        if interpreter.llm.context_window is None:
+            interpreter.llm.context_window = 123000
+        if interpreter.llm.max_tokens is None:
+            interpreter.llm.max_tokens = 4096
+        if interpreter.llm.supports_functions is None:
+            interpreter.llm.supports_functions = (
+                False if "vision" in interpreter.llm.model else True
+            )
+
+    if interpreter.llm.model.startswith(
+        "gpt-3.5-turbo"
+    ) or interpreter.llm.model.startswith("openai/gpt-3.5-turbo"):
         if interpreter.llm.context_window is None:
             interpreter.llm.context_window = 16000
         if interpreter.llm.max_tokens is None:
             interpreter.llm.max_tokens = 4096
         if interpreter.llm.supports_functions is None:
             interpreter.llm.supports_functions = True
 
@@ -414,26 +426,32 @@
 
     interpreter.chat()
 
 
 def set_attributes(args, arguments):
     for argument_name, argument_value in vars(args).items():
         if argument_value is not None:
-            argument_dictionary = [a for a in arguments if a["name"] == argument_name]
-            if len(argument_dictionary) > 0:
-                argument_dictionary = argument_dictionary[0]
+            if argument_dictionary := get_argument_dictionary(arguments, argument_name):
                 if "attribute" in argument_dictionary:
                     attr_dict = argument_dictionary["attribute"]
                     setattr(attr_dict["object"], attr_dict["attr_name"], argument_value)
 
                     if args.verbose:
                         print(
                             f"Setting attribute {attr_dict['attr_name']} on {attr_dict['object'].__class__.__name__.lower()} to '{argument_value}'..."
                         )
 
 
+def get_argument_dictionary(arguments: list[dict], key: str) -> dict:
+    if len(argument_dictionary_list := list(filter(lambda x: x["name"] == key, arguments))) > 0:
+        return argument_dictionary_list[0]
+    return {}
+
+
 def main():
     interpreter = OpenInterpreter(import_computer_api=True)
     try:
         start_terminal_interface(interpreter)
     except KeyboardInterrupt:
         pass
+    finally:
+        interpreter.computer.terminate()
```

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/terminal_interface.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/terminal_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,36 +69,33 @@
     else:
         interactive = True
 
     active_block = None
     voice_subprocess = None
 
     while True:
-        try:
-            if interactive:
-                ### This is the primary input for Open Interpreter.
-                message = cli_input("> ").strip() if interpreter.multi_line else input("> ").strip()
-
-                try:
-                    # This lets users hit the up arrow key for past messages
-                    readline.add_history(message)
-                except:
-                    # If the user doesn't have readline (may be the case on windows), that's fine
-                    pass
-
-        except KeyboardInterrupt:
-            # Exit gracefully
-            # Disconnect from the computer interface
-            interpreter.computer.terminate()
-            break
+        if interactive:
+            ### This is the primary input for Open Interpreter.
+            message = cli_input("> ").strip() if interpreter.multi_line else input("> ").strip()
+
+            try:
+                # This lets users hit the up arrow key for past messages
+                readline.add_history(message)
+            except:
+                # If the user doesn't have readline (may be the case on windows), that's fine
+                pass
 
         if isinstance(message, str):
             # This is for the terminal interface being used as a CLI — messages are strings.
             # This won't fire if they're in the python package, display=True, and they passed in an array of messages (for example).
 
+            if message == "":
+                # Ignore empty messages when user presses enter without typing anything
+                continue
+
             if message.startswith("%") and interactive:
                 handle_magic_command(interpreter, message)
                 continue
 
             # Many users do this
             if message.strip() == "interpreter --local":
                 print("Please exit this conversation, then run `interpreter --local`.")
@@ -364,20 +361,20 @@
                                 else:
                                     arguments = None
 
                                 # NOTE: Do not put the text you're clicking on screen
                                 # (unless we figure out how to do this AFTER taking the screenshot)
                                 # otherwise it will try to click this notification!
 
-                                if action in [
-                                    "computer.screenshot()",
-                                    "computer.display.screenshot()",
-                                    "computer.display.view()",
-                                    "computer.view()",
-                                ]:
+                                if any(action.startswith(text) for text in [
+                                    "computer.screenshot",
+                                    "computer.display.screenshot",
+                                    "computer.display.view",
+                                    "computer.view"
+                                ]):
                                     description = "Viewing screen..."
                                 elif action == "computer.mouse.click()":
                                     description = "Clicking..."
                                 elif action.startswith("computer.mouse.click("):
                                     if "icon=" in arguments:
                                         text_or_icon = "icon"
                                     else:
```

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/utils/check_for_package.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/utils/check_for_package.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/utils/count_tokens.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/utils/count_tokens.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/utils/display_markdown_message.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/utils/display_markdown_message.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/utils/display_output.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/utils/display_output.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.2.4/interpreter/terminal_interface/validate_llm_settings.py` & `open_interpreter-0.2.5/interpreter/terminal_interface/validate_llm_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,18 @@
                     )
 
                     response = prompt("OpenAI API key: ", is_password=True)
 
                     display_markdown_message(
                         """
 
-                    **Tip:** To save this key for later, run `export OPENAI_API_KEY=your_api_key` on Mac/Linux or `setx OPENAI_API_KEY your_api_key` on Windows.
+                    **Tip:** To save this key for later, run one of the following and then restart your terminal. 
+                    MacOS: `echo '\\nexport OPENAI_API_KEY=your_api_key' >> ~/.zshrc`
+                    Linux: `echo '\\nexport OPENAI_API_KEY=your_api_key' >> ~/.bashrc`
+                    Windows: `setx OPENAI_API_KEY your_api_key`
                     
                     ---"""
                     )
 
                     interpreter.llm.api_key = response
                     time.sleep(2)
                     break
```

### Comparing `open_interpreter-0.2.4/pyproject.toml` & `open_interpreter-0.2.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.2.4" # Use "-rc1", "-rc2", etc. for pre-release versions
+version = "0.2.5" # Use "-rc1", "-rc2", etc. for pre-release versions
 description = "Let language models run code"
 authors = ["Killian Lucas <killian@openinterpreter.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python = ">=3.9,<4"
 
 astor = "^0.8.1"
 git-python = "^1.0.3"
 inquirer = "^3.1.3"
-litellm = "^1.18.4"
+litellm = "^1.34.38"
 pyyaml = "^6.0.1"
 rich = "^13.4.2"
 six = "^1.16.0"
 tokentrim = "^0.1.13"
 wget = "^3.2"
 psutil = "^5.9.6"
 pyreadline3 = {version = "^3.4.1", markers = "sys_platform == 'win32'"}
 html2image = "^2.0.4.3"
 ipykernel = "^6.26.0"
 jupyter-client = "^8.6.0"
 matplotlib = "^3.8.2"
 toml = "^0.10.2"
 posthog = "^3.1.0"
-tiktoken = "^0.5.2"
+tiktoken = "^0.6.0"
+
 
 #Optional dependencies
-opencv-python = { version = "^4.8.1.78", optional = true }
-pyautogui = { version = "^0.9.54", optional = true }
-plyer = { version = "^2.1.0", optional = true }
-pywinctl = { version = "^0.3", optional = true }
+opencv-python = { version = "^4.8.1.78", optional = false }
+pyautogui = "^0.9.54"
+plyer = "^2.1.0"
+pywinctl = "^0.3"
 semgrep = { version = "^1.52.0", optional = true }
 yaspin = { version = "^3.0.1", optional = true }
 pytesseract = { version = "^0.3.10", optional = true }
 sentence-transformers = { version = "^2.5.1", optional = true }
 nltk = { version = "^3.8.1", optional = true }
 ipywidgets = { version = "^8.1.2", optional = true }
 torch = { version = "^2.2.1", optional = true }
 timm = { version = "^0.9.16", optional = true }
 prompt-toolkit = "^3.0.43"
 send2trash = "^1.8.2"
 uvicorn = "^0.27.0"
 fastapi = "^0.110.0"
-aifs = "^0.0.9"
 platformdirs = "^4.2.0"
 pydantic = "^2.6.4"
+screeninfo = "^0.8.1"
+aifs = "^0.0.15"
 
 [tool.poetry.extras]
 os = ["opencv-python", "pyautogui", "plyer", "pywinctl", "pytesseract", "sentence-transformers", "ipywidgets", "torch", "timm"]
 safe = ["semgrep", "yaspin"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.10.1"
```

### Comparing `open_interpreter-0.2.4/PKG-INFO` & `open_interpreter-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.2.4
+Version: 0.2.5
 Summary: Let language models run code
 Author: Killian Lucas
 Author-email: killian@openinterpreter.com
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: os
 Provides-Extra: safe
-Requires-Dist: aifs (>=0.0.9,<0.0.10)
+Requires-Dist: aifs (>=0.0.15,<0.0.16)
 Requires-Dist: astor (>=0.8.1,<0.9.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: git-python (>=1.0.3,<2.0.0)
 Requires-Dist: html2image (>=2.0.4.3,<3.0.0.0)
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
 Requires-Dist: ipykernel (>=6.26.0,<7.0.0)
 Requires-Dist: ipywidgets (>=8.1.2,<9.0.0) ; extra == "os"
 Requires-Dist: jupyter-client (>=8.6.0,<9.0.0)
-Requires-Dist: litellm (>=1.18.4,<2.0.0)
+Requires-Dist: litellm (>=1.34.38,<2.0.0)
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: opencv-python (>=4.8.1.78,<5.0.0.0) ; extra == "os"
 Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
 Requires-Dist: plyer (>=2.1.0,<3.0.0) ; extra == "os"
 Requires-Dist: posthog (>=3.1.0,<4.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0)
@@ -32,19 +33,20 @@
 Requires-Dist: pyautogui (>=0.9.54,<0.10.0) ; extra == "os"
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0) ; sys_platform == "win32"
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0) ; extra == "os"
 Requires-Dist: pywinctl (>=0.3,<0.4) ; extra == "os"
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: screeninfo (>=0.8.1,<0.9.0)
 Requires-Dist: semgrep (>=1.52.0,<2.0.0) ; extra == "safe"
 Requires-Dist: send2trash (>=1.8.2,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.5.1,<3.0.0) ; extra == "os"
 Requires-Dist: six (>=1.16.0,<2.0.0)
-Requires-Dist: tiktoken (>=0.5.2,<0.6.0)
+Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: timm (>=0.9.16,<0.10.0) ; extra == "os"
 Requires-Dist: tokentrim (>=0.1.13,<0.2.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: torch (>=2.2.1,<3.0.0) ; extra == "os"
 Requires-Dist: uvicorn (>=0.27.0,<0.28.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Requires-Dist: yaspin (>=3.0.1,<4.0.0) ; extra == "safe"
@@ -57,26 +59,25 @@
         <img alt="Discord" src="https://img.shields.io/discord/1146610656779440188?logo=discord&style=flat&logoColor=white"/></a>
     <a href="docs/README_JA.md"><img src="https://img.shields.io/badge/ドキュメント-日本語-white.svg" alt="JA doc"/></a>
     <a href="docs/README_ZH.md"><img src="https://img.shields.io/badge/文档-中文版-white.svg" alt="ZH doc"/></a>
     <a href="docs/README_IN.md"><img src="https://img.shields.io/badge/Hindi-white.svg" alt="IN doc"/></a>
     <img src="https://img.shields.io/static/v1?label=license&message=AGPL&color=white&style=flat" alt="License"/>
     <br>
     <br>
-    <strong>Today we launched a new computer (the 01) with Open Interpreter at the center. <a href="https://github.com/OpenInterpreter/01">Star the repo →</a></strong><br>
-    <br><a href="https://openinterpreter.com">Get early access to the desktop app</a>‎ ‎ |‎ ‎ <a href="https://docs.openinterpreter.com/">Documentation</a><br>
+    <br><a href="https://0ggfznkwh4j.typeform.com/to/G21i9lJ2">Get early access to the desktop app</a>‎ ‎ |‎ ‎ <a href="https://docs.openinterpreter.com/">Documentation</a><br>
 </p>
 
 <br>
 
 ![poster](https://github.com/KillianLucas/open-interpreter/assets/63927363/08f0d493-956b-4d49-982e-67d4b20c4b56)
 
 <br>
-<!--<p align="center">
-<strong>The New Computer Update</strong> introduces <strong><code>--os</code></strong> and a new <strong>Computer API</strong>. <a href="https://changes.openinterpreter.com/log/the-new-computer-update">Read On →</a>
-</p>-->
+<p align="center">
+<strong>The New Computer Update</strong> introduced <strong><code>--os</code></strong> and a new <strong>Computer API</strong>. <a href="https://changes.openinterpreter.com/log/the-new-computer-update">Read On →</a>
+</p>
 <br>
 
 ```shell
 pip install open-interpreter
 ```
 
 > Not working? Read our [setup guide](https://docs.openinterpreter.com/getting-started/setup).
@@ -131,14 +132,18 @@
 ```python
 from interpreter import interpreter
 
 interpreter.chat("Plot AAPL and META's normalized stock prices") # Executes a single command
 interpreter.chat() # Starts an interactive chat
 ```
 
+### GitHub Codespaces
+
+Press the `,` key on this repository's GitHub page to create a codespace. After a moment, you'll receive a cloud virtual machine environment pre-installed with open-interpreter. You can then start interacting with it directly and freely confirm its execution of system commands without worrying about damaging the system.
+
 ## Comparison to ChatGPT's Code Interpreter
 
 OpenAI's release of [Code Interpreter](https://openai.com/blog/chatgpt-plugins#code-interpreter) with GPT-4 presents a fantastic opportunity to accomplish real-world tasks with ChatGPT.
 
 However, OpenAI's service is hosted, closed-source, and heavily restricted:
 
 - No internet access.
@@ -408,14 +413,42 @@
 
 ## How Does it Work?
 
 Open Interpreter equips a [function-calling language model](https://platform.openai.com/docs/guides/gpt/function-calling) with an `exec()` function, which accepts a `language` (like "Python" or "JavaScript") and `code` to run.
 
 We then stream the model's messages, code, and your system's outputs to the terminal as Markdown.
 
+# Access Documentation Offline
+
+The full [documentation](https://docs.openinterpreter.com/) is accessible on-the-go without the need for an internet connection.
+
+[Node](https://nodejs.org/en) is a pre-requisite:
+
+- Version 18.17.0 or any later 18.x.x version.
+- Version 20.3.0 or any later 20.x.x version.
+- Any version starting from 21.0.0 onwards, with no upper limit specified.
+
+Install [Mintlify](https://mintlify.com/):
+
+```bash
+npm i -g mintlify@latest
+```
+
+Change into the docs directory and run the appropriate command:
+
+```bash
+# Assuming you're at the project's root directory
+cd ./docs
+
+# Run the documentation server
+mintlify dev
+```
+
+A new browser window should open. The documentation will be available at [http://localhost:3000](http://localhost:3000) as long as the documentation server is running.
+
 # Contributing
 
 Thank you for your interest in contributing! We welcome involvement from the community.
 
 Please see our [contributing guidelines](docs/CONTRIBUTING.md) for more details on how to get involved.
 
 # Roadmap
```

#### html2text {}

```diff
@@ -1,47 +1,48 @@
-Metadata-Version: 2.1 Name: open-interpreter Version: 0.2.4 Summary: Let
+Metadata-Version: 2.1 Name: open-interpreter Version: 0.2.5 Summary: Let
 language models run code Author: Killian Lucas Author-email:
-killian@openinterpreter.com Requires-Python: >=3.9,<3.12 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Provides-Extra: os Provides-Extra: safe
-Requires-Dist: aifs (>=0.0.9,<0.0.10) Requires-Dist: astor (>=0.8.1,<0.9.0)
-Requires-Dist: fastapi (>=0.110.0,<0.111.0) Requires-Dist: git-python
-(>=1.0.3,<2.0.0) Requires-Dist: html2image (>=2.0.4.3,<3.0.0.0) Requires-Dist:
-inquirer (>=3.1.3,<4.0.0) Requires-Dist: ipykernel (>=6.26.0,<7.0.0) Requires-
-Dist: ipywidgets (>=8.1.2,<9.0.0) ; extra == "os" Requires-Dist: jupyter-client
-(>=8.6.0,<9.0.0) Requires-Dist: litellm (>=1.18.4,<2.0.0) Requires-Dist:
-matplotlib (>=3.8.2,<4.0.0) Requires-Dist: nltk (>=3.8.1,<4.0.0) Requires-Dist:
-opencv-python (>=4.8.1.78,<5.0.0.0) ; extra == "os" Requires-Dist: platformdirs
+killian@openinterpreter.com Requires-Python: >=3.9,<4 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: os Provides-Extra: safe Requires-Dist: aifs (>=0.0.15,<0.0.16)
+Requires-Dist: astor (>=0.8.1,<0.9.0) Requires-Dist: fastapi
+(>=0.110.0,<0.111.0) Requires-Dist: git-python (>=1.0.3,<2.0.0) Requires-Dist:
+html2image (>=2.0.4.3,<3.0.0.0) Requires-Dist: inquirer (>=3.1.3,<4.0.0)
+Requires-Dist: ipykernel (>=6.26.0,<7.0.0) Requires-Dist: ipywidgets
+(>=8.1.2,<9.0.0) ; extra == "os" Requires-Dist: jupyter-client (>=8.6.0,<9.0.0)
+Requires-Dist: litellm (>=1.34.38,<2.0.0) Requires-Dist: matplotlib
+(>=3.8.2,<4.0.0) Requires-Dist: nltk (>=3.8.1,<4.0.0) Requires-Dist: opencv-
+python (>=4.8.1.78,<5.0.0.0) ; extra == "os" Requires-Dist: platformdirs
 (>=4.2.0,<5.0.0) Requires-Dist: plyer (>=2.1.0,<3.0.0) ; extra == "os"
 Requires-Dist: posthog (>=3.1.0,<4.0.0) Requires-Dist: prompt-toolkit
 (>=3.0.43,<4.0.0) Requires-Dist: psutil (>=5.9.6,<6.0.0) Requires-Dist:
 pyautogui (>=0.9.54,<0.10.0) ; extra == "os" Requires-Dist: pydantic
 (>=2.6.4,<3.0.0) Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0) ; sys_platform ==
 "win32" Requires-Dist: pytesseract (>=0.3.10,<0.4.0) ; extra == "os" Requires-
 Dist: pywinctl (>=0.3,<0.4) ; extra == "os" Requires-Dist: pyyaml
-(>=6.0.1,<7.0.0) Requires-Dist: rich (>=13.4.2,<14.0.0) Requires-Dist: semgrep
-(>=1.52.0,<2.0.0) ; extra == "safe" Requires-Dist: send2trash (>=1.8.2,<2.0.0)
-Requires-Dist: sentence-transformers (>=2.5.1,<3.0.0) ; extra == "os" Requires-
-Dist: six (>=1.16.0,<2.0.0) Requires-Dist: tiktoken (>=0.5.2,<0.6.0) Requires-
-Dist: timm (>=0.9.16,<0.10.0) ; extra == "os" Requires-Dist: tokentrim
-(>=0.1.13,<0.2.0) Requires-Dist: toml (>=0.10.2,<0.11.0) Requires-Dist: torch
-(>=2.2.1,<3.0.0) ; extra == "os" Requires-Dist: uvicorn (>=0.27.0,<0.28.0)
-Requires-Dist: wget (>=3.2,<4.0) Requires-Dist: yaspin (>=3.0.1,<4.0.0) ; extra
-== "safe" Description-Content-Type: text/markdown
+(>=6.0.1,<7.0.0) Requires-Dist: rich (>=13.4.2,<14.0.0) Requires-Dist:
+screeninfo (>=0.8.1,<0.9.0) Requires-Dist: semgrep (>=1.52.0,<2.0.0) ; extra ==
+"safe" Requires-Dist: send2trash (>=1.8.2,<2.0.0) Requires-Dist: sentence-
+transformers (>=2.5.1,<3.0.0) ; extra == "os" Requires-Dist: six
+(>=1.16.0,<2.0.0) Requires-Dist: tiktoken (>=0.6.0,<0.7.0) Requires-Dist: timm
+(>=0.9.16,<0.10.0) ; extra == "os" Requires-Dist: tokentrim (>=0.1.13,<0.2.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0) Requires-Dist: torch (>=2.2.1,<3.0.0) ;
+extra == "os" Requires-Dist: uvicorn (>=0.27.0,<0.28.0) Requires-Dist: wget
+(>=3.2,<4.0) Requires-Dist: yaspin (>=3.0.1,<4.0.0) ; extra == "safe"
+Description-Content-Type: text/markdown
                       ************ ?â?? OOppeenn IInntteerrpprreetteerr ************
                   _[_D_i_s_c_o_r_d_]_[_J_A_ _d_o_c_]_[_Z_H_ _d_o_c_]_[_I_N_ _d_o_c_][License]
 
-TTooddaayy wwee llaauunncchheedd aa nneeww ccoommppuutteerr ((tthhee 0011)) wwiitthh OOppeenn IInntteerrpprreetteerr aatt tthhee cceenntteerr..
-                               _SS_tt_aa_rr_ _tt_hh_ee_ _rr_ee_pp_oo_ _?â_?_?
 
        _G_e_t_ _e_a_r_l_y_ _a_c_c_e_s_s_ _t_o_ _t_h_e_ _d_e_s_k_t_o_p_ _a_p_pâ â |â â _D_o_c_u_m_e_n_t_a_t_i_o_n
 
 ![poster](https://github.com/KillianLucas/open-interpreter/assets/63927363/
 08f0d493-956b-4d49-982e-67d4b20c4b56)
+  TThhee NNeeww CCoommppuutteerr UUppddaattee introduced ----ooss and a new CCoommppuutteerr AAPPII. _R_e_a_d_ _O_n_ _â__
 
 ```shell pip install open-interpreter ``` > Not working? Read our [setup guide]
 (https://docs.openinterpreter.com/getting-started/setup). ```shell interpreter
 ```
 **Open Interpreter** lets LLMs run code (Python, Javascript, Shell, and more)
 locally. You can chat with Open Interpreter through a ChatGPT-like interface in
 your terminal by running `$ interpreter` after installing. This provides a
@@ -57,31 +58,36 @@
 interface, inspired by _Her_: [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1NojYGHDgxH6Y1G1oxThEBBb2AtyODBIK) ## Quick
 Start ```shell pip install open-interpreter ``` ### Terminal After
 installation, simply run `interpreter`: ```shell interpreter ``` ### Python
 ```python from interpreter import interpreter interpreter.chat("Plot AAPL and
 META's normalized stock prices") # Executes a single command interpreter.chat()
-# Starts an interactive chat ``` ## Comparison to ChatGPT's Code Interpreter
-OpenAI's release of [Code Interpreter](https://openai.com/blog/chatgpt-
-plugins#code-interpreter) with GPT-4 presents a fantastic opportunity to
-accomplish real-world tasks with ChatGPT. However, OpenAI's service is hosted,
-closed-source, and heavily restricted: - No internet access. - [Limited set of
-pre-installed packages](https://wfhbrian.com/mastering-chatgpts-code-
-interpreter-list-of-python-packages/). - 100 MB maximum upload, 120.0 second
-runtime limit. - State is cleared (along with any generated files or links)
-when the environment dies. --- Open Interpreter overcomes these limitations by
-running in your local environment. It has full access to the internet, isn't
-restricted by time or file size, and can utilize any package or library. This
-combines the power of GPT-4's Code Interpreter with the flexibility of your
-local development environment. ## Commands **Update:** The Generator Update
-(0.1.5) introduced streaming: ```python message = "What operating system are we
-on?" for chunk in interpreter.chat(message, display=False, stream=True): print
-(chunk) ``` ### Interactive Chat To start an interactive chat in your terminal,
-either run `interpreter` from the command line: ```shell interpreter ``` Or
+# Starts an interactive chat ``` ### GitHub Codespaces Press the `,` key on
+this repository's GitHub page to create a codespace. After a moment, you'll
+receive a cloud virtual machine environment pre-installed with open-
+interpreter. You can then start interacting with it directly and freely confirm
+its execution of system commands without worrying about damaging the system. ##
+Comparison to ChatGPT's Code Interpreter OpenAI's release of [Code Interpreter]
+(https://openai.com/blog/chatgpt-plugins#code-interpreter) with GPT-4 presents
+a fantastic opportunity to accomplish real-world tasks with ChatGPT. However,
+OpenAI's service is hosted, closed-source, and heavily restricted: - No
+internet access. - [Limited set of pre-installed packages](https://
+wfhbrian.com/mastering-chatgpts-code-interpreter-list-of-python-packages/). -
+100 MB maximum upload, 120.0 second runtime limit. - State is cleared (along
+with any generated files or links) when the environment dies. --- Open
+Interpreter overcomes these limitations by running in your local environment.
+It has full access to the internet, isn't restricted by time or file size, and
+can utilize any package or library. This combines the power of GPT-4's Code
+Interpreter with the flexibility of your local development environment. ##
+Commands **Update:** The Generator Update (0.1.5) introduced streaming:
+```python message = "What operating system are we on?" for chunk in
+interpreter.chat(message, display=False, stream=True): print(chunk) ``` ###
+Interactive Chat To start an interactive chat in your terminal, either run
+`interpreter` from the command line: ```shell interpreter ``` Or
 `interpreter.chat()` from a .py file: ```python interpreter.chat() ``` **You
 can also stream each chunk:** ```python message = "What operating system are we
 on?" for chunk in interpreter.chat(message, display=False, stream=True): print
 (chunk) ``` ### Programmatic Chat For more precise control, you can pass
 messages directly to `.chat(message)`: ```python interpreter.chat("Add
 subtitles to all videos in /videos.") # ... Streams output to your terminal,
 completes task ... interpreter.chat("These look great but can you make the
@@ -178,18 +184,29 @@
 Open Interpreter in a restricted environment like Google Colab or Replit. These
 environments are more isolated, reducing the risks of executing arbitrary code.
 There is **experimental** support for a [safe mode](docs/SAFE_MODE.md) to help
 mitigate some risks. ## How Does it Work? Open Interpreter equips a [function-
 calling language model](https://platform.openai.com/docs/guides/gpt/function-
 calling) with an `exec()` function, which accepts a `language` (like "Python"
 or "JavaScript") and `code` to run. We then stream the model's messages, code,
-and your system's outputs to the terminal as Markdown. # Contributing Thank you
-for your interest in contributing! We welcome involvement from the community.
-Please see our [contributing guidelines](docs/CONTRIBUTING.md) for more details
-on how to get involved. # Roadmap Visit [our roadmap](https://github.com/
-KillianLucas/open-interpreter/blob/main/docs/ROADMAP.md) to preview the future
-of Open Interpreter. **Note**: This software is not affiliated with OpenAI. !
-[thumbnail-ncu](https://github.com/KillianLucas/open-interpreter/assets/
-63927363/1b19a5db-b486-41fd-a7a1-fe2028031686) > Having access to a junior
-programmer working at the speed of your fingertips ... can make new workflows
-effortless and efficient, as well as open the benefits of programming to new
-audiences. > > â _OpenAI's Code Interpreter Release_
+and your system's outputs to the terminal as Markdown. # Access Documentation
+Offline The full [documentation](https://docs.openinterpreter.com/) is
+accessible on-the-go without the need for an internet connection. [Node](https:
+//nodejs.org/en) is a pre-requisite: - Version 18.17.0 or any later 18.x.x
+version. - Version 20.3.0 or any later 20.x.x version. - Any version starting
+from 21.0.0 onwards, with no upper limit specified. Install [Mintlify](https://
+mintlify.com/): ```bash npm i -g mintlify@latest ``` Change into the docs
+directory and run the appropriate command: ```bash # Assuming you're at the
+project's root directory cd ./docs # Run the documentation server mintlify dev
+``` A new browser window should open. The documentation will be available at
+[http://localhost:3000](http://localhost:3000) as long as the documentation
+server is running. # Contributing Thank you for your interest in contributing!
+We welcome involvement from the community. Please see our [contributing
+guidelines](docs/CONTRIBUTING.md) for more details on how to get involved. #
+Roadmap Visit [our roadmap](https://github.com/KillianLucas/open-interpreter/
+blob/main/docs/ROADMAP.md) to preview the future of Open Interpreter. **Note**:
+This software is not affiliated with OpenAI. ![thumbnail-ncu](https://
+github.com/KillianLucas/open-interpreter/assets/63927363/1b19a5db-b486-41fd-
+a7a1-fe2028031686) > Having access to a junior programmer working at the speed
+of your fingertips ... can make new workflows effortless and efficient, as well
+as open the benefits of programming to new audiences. > > â _OpenAI's Code
+Interpreter Release_
```

