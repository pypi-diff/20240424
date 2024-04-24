# Comparing `tmp/telegrinder-0.1.dev8.tar.gz` & `tmp/telegrinder-0.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegrinder-0.1.dev8.tar", max compression
+gzip compressed data, was "telegrinder-0.1.dev9.tar", max compression
```

## Comparing `telegrinder-0.1.dev8.tar` & `telegrinder-0.1.dev9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1063 2022-04-17 10:00:22.519972 telegrinder-0.1.dev8/LICENSE
--rw-r--r--   0        0        0      532 2022-10-18 17:40:24.895635 telegrinder-0.1.dev8/pyproject.toml
--rw-r--r--   0        0        0      722 2022-10-09 16:36:29.440236 telegrinder-0.1.dev8/telegrinder/__init__.py
--rw-r--r--   0        0        0      124 2022-10-05 12:31:51.515560 telegrinder-0.1.dev8/telegrinder/api/__init__.py
--rw-r--r--   0        0        0     1002 2022-10-10 13:55:09.234603 telegrinder-0.1.dev8/telegrinder/api/abc.py
--rw-r--r--   0        0        0     1993 2022-10-12 17:10:49.127709 telegrinder-0.1.dev8/telegrinder/api/api.py
--rw-r--r--   0        0        0      162 2022-10-09 17:03:40.721083 telegrinder-0.1.dev8/telegrinder/api/error.py
--rw-r--r--   0        0        0      463 2022-10-09 16:45:29.841169 telegrinder-0.1.dev8/telegrinder/api/response.py
--rw-r--r--   0        0        0      391 2022-08-07 12:51:13.884678 telegrinder-0.1.dev8/telegrinder/bot/__init__.py
--rw-r--r--   0        0        0     1733 2022-10-10 14:21:42.027571 telegrinder-0.1.dev8/telegrinder/bot/bot.py
--rw-r--r--   0        0        0      121 2022-08-07 12:51:13.884858 telegrinder-0.1.dev8/telegrinder/bot/cute_types/__init__.py
--rw-r--r--   0        0        0      792 2022-10-09 17:03:40.722525 telegrinder-0.1.dev8/telegrinder/bot/cute_types/callback_query.py
--rw-r--r--   0        0        0     1034 2022-10-09 17:03:40.723014 telegrinder-0.1.dev8/telegrinder/bot/cute_types/inline_query.py
--rw-r--r--   0        0        0     2284 2022-10-09 17:03:40.723789 telegrinder-0.1.dev8/telegrinder/bot/cute_types/message.py
--rw-r--r--   0        0        0      240 2022-08-07 12:51:13.885192 telegrinder-0.1.dev8/telegrinder/bot/dispatch/__init__.py
--rw-r--r--   0        0        0      448 2022-10-05 15:55:53.816795 telegrinder-0.1.dev8/telegrinder/bot/dispatch/abc.py
--rw-r--r--   0        0        0     2899 2022-10-18 13:32:16.921651 telegrinder-0.1.dev8/telegrinder/bot/dispatch/dispatch.py
--rw-r--r--   0        0        0       58 2022-04-20 18:58:21.519892 telegrinder-0.1.dev8/telegrinder/bot/dispatch/handler/__init__.py
--rw-r--r--   0        0        0      411 2022-10-06 16:37:24.658158 telegrinder-0.1.dev8/telegrinder/bot/dispatch/handler/abc.py
--rw-r--r--   0        0        0     1482 2022-10-09 17:03:40.725135 telegrinder-0.1.dev8/telegrinder/bot/dispatch/handler/func.py
--rw-r--r--   0        0        0       31 2022-04-22 08:48:08.508568 telegrinder-0.1.dev8/telegrinder/bot/dispatch/middleware/__init__.py
--rw-r--r--   0        0        0      268 2022-04-22 08:48:08.506726 telegrinder-0.1.dev8/telegrinder/bot/dispatch/middleware/abc.py
--rw-r--r--   0        0        0     2000 2022-10-18 13:32:16.919781 telegrinder-0.1.dev8/telegrinder/bot/dispatch/process.py
--rw-r--r--   0        0        0      146 2022-08-07 12:51:13.885835 telegrinder-0.1.dev8/telegrinder/bot/dispatch/view/__init__.py
--rw-r--r--   0        0        0      389 2022-10-05 15:56:33.906807 telegrinder-0.1.dev8/telegrinder/bot/dispatch/view/abc.py
--rw-r--r--   0        0        0     1863 2022-10-06 16:40:20.648209 telegrinder-0.1.dev8/telegrinder/bot/dispatch/view/callback_query.py
--rw-r--r--   0        0        0     1829 2022-10-06 16:40:20.651095 telegrinder-0.1.dev8/telegrinder/bot/dispatch/view/inline_query.py
--rw-r--r--   0        0        0     2103 2022-10-09 17:03:40.725804 telegrinder-0.1.dev8/telegrinder/bot/dispatch/view/message.py
--rw-r--r--   0        0        0      990 2022-10-09 17:03:40.726368 telegrinder-0.1.dev8/telegrinder/bot/dispatch/waiter.py
--rw-r--r--   0        0        0       57 2022-04-16 18:15:00.717683 telegrinder-0.1.dev8/telegrinder/bot/polling/__init__.py
--rw-r--r--   0        0        0      401 2022-10-05 16:13:52.521597 telegrinder-0.1.dev8/telegrinder/bot/polling/abc.py
--rw-r--r--   0        0        0     1893 2022-10-10 14:18:43.785077 telegrinder-0.1.dev8/telegrinder/bot/polling/polling.py
--rw-r--r--   0        0        0      364 2022-10-18 08:21:39.198635 telegrinder-0.1.dev8/telegrinder/bot/rules/__init__.py
--rw-r--r--   0        0        0     3027 2022-10-18 13:30:21.755501 telegrinder-0.1.dev8/telegrinder/bot/rules/abc.py
--rw-r--r--   0        0        0      683 2022-10-05 16:22:23.755433 telegrinder-0.1.dev8/telegrinder/bot/rules/callback_data.py
--rw-r--r--   0        0        0      859 2022-10-05 16:26:12.738773 telegrinder-0.1.dev8/telegrinder/bot/rules/func.py
--rw-r--r--   0        0        0      675 2022-10-05 12:31:51.543146 telegrinder-0.1.dev8/telegrinder/bot/rules/fuzzy.py
--rw-r--r--   0        0        0      419 2022-10-18 13:32:16.909888 telegrinder-0.1.dev8/telegrinder/bot/rules/integer.py
--rw-r--r--   0        0        0      306 2022-08-09 15:45:11.810780 telegrinder-0.1.dev8/telegrinder/bot/rules/is_from.py
--rw-r--r--   0        0        0      848 2022-10-05 16:22:34.205327 telegrinder-0.1.dev8/telegrinder/bot/rules/markup.py
--rw-r--r--   0        0        0      877 2022-10-18 17:38:53.362772 telegrinder-0.1.dev8/telegrinder/bot/rules/regex.py
--rw-r--r--   0        0        0      759 2022-10-18 13:32:16.914222 telegrinder-0.1.dev8/telegrinder/bot/rules/text.py
--rw-r--r--   0        0        0       60 2022-04-26 20:09:36.774195 telegrinder-0.1.dev8/telegrinder/bot/scenario/__init__.py
--rw-r--r--   0        0        0      289 2022-04-26 20:04:34.251102 telegrinder-0.1.dev8/telegrinder/bot/scenario/abc.py
--rw-r--r--   0        0        0     3655 2022-09-11 11:14:52.608453 telegrinder-0.1.dev8/telegrinder/bot/scenario/checkbox.py
--rw-r--r--   0        0        0       74 2022-10-09 16:34:03.453588 telegrinder-0.1.dev8/telegrinder/client/__init__.py
--rw-r--r--   0        0        0     1305 2022-10-09 17:03:40.727766 telegrinder-0.1.dev8/telegrinder/client/abc.py
--rw-r--r--   0        0        0     3624 2022-10-09 17:03:40.728145 telegrinder-0.1.dev8/telegrinder/client/aiohttp.py
--rw-r--r--   0        0        0     1305 2022-10-12 17:10:02.257864 telegrinder-0.1.dev8/telegrinder/model.py
--rw-r--r--   0        0        0      610 2022-04-20 18:39:32.829598 telegrinder-0.1.dev8/telegrinder/modules.py
--rw-r--r--   0        0        0      904 2022-10-09 16:34:03.446826 telegrinder-0.1.dev8/telegrinder/result.py
--rw-r--r--   0        0        0      317 2022-10-09 16:34:03.450525 telegrinder-0.1.dev8/telegrinder/tools/__init__.py
--rw-r--r--   0        0        0     1277 2022-04-17 05:35:56.975145 telegrinder-0.1.dev8/telegrinder/tools/buttons.py
--rw-r--r--   0        0        0      102 2022-07-03 07:15:53.180547 telegrinder-0.1.dev8/telegrinder/tools/formatting/__init__.py
--rw-r--r--   0        0        0      958 2022-08-07 12:51:13.875127 telegrinder-0.1.dev8/telegrinder/tools/formatting/abc.py
--rw-r--r--   0        0        0     1606 2022-10-05 12:31:51.565411 telegrinder-0.1.dev8/telegrinder/tools/formatting/html.py
--rw-r--r--   0        0        0     1833 2022-08-11 11:39:10.120725 telegrinder-0.1.dev8/telegrinder/tools/formatting/markdown.py
--rw-r--r--   0        0        0       86 2022-05-10 13:21:05.250288 telegrinder-0.1.dev8/telegrinder/tools/kb_set/__init__.py
--rw-r--r--   0        0        0      191 2022-05-10 12:42:26.141026 telegrinder-0.1.dev8/telegrinder/tools/kb_set/base.py
--rw-r--r--   0        0        0     1830 2022-08-07 12:51:13.886941 telegrinder-0.1.dev8/telegrinder/tools/kb_set/yaml.py
--rw-r--r--   0        0        0     2910 2022-07-04 07:26:47.118891 telegrinder-0.1.dev8/telegrinder/tools/keyboard.py
--rw-r--r--   0        0        0     1201 2022-10-18 17:34:13.359753 telegrinder-0.1.dev8/telegrinder/tools/magic.py
--rw-r--r--   0        0        0      147 2022-07-03 07:28:46.397440 telegrinder-0.1.dev8/telegrinder/tools/parse_mode.py
--rw-r--r--   0        0        0       39 2022-10-06 21:09:42.264757 telegrinder-0.1.dev8/telegrinder/typegen/__init__.py
--rw-r--r--   0        0        0       60 2022-10-06 21:00:00.907223 telegrinder-0.1.dev8/telegrinder/typegen/__main__.py
--rw-r--r--   0        0        0      767 2022-10-10 14:25:57.752535 telegrinder-0.1.dev8/telegrinder/typegen/nicification.py
--rw-r--r--   0        0        0     8284 2022-10-18 13:32:16.988246 telegrinder-0.1.dev8/telegrinder/typegen/schema_generator.py
--rw-r--r--   0        0        0       40 2022-10-10 14:26:02.207568 telegrinder-0.1.dev8/telegrinder/types/__init__.py
--rw-r--r--   0        0        0    50649 2022-10-10 14:26:02.945020 telegrinder-0.1.dev8/telegrinder/types/methods.py
--rw-r--r--   0        0        0    76929 2022-10-18 13:32:17.373504 telegrinder-0.1.dev8/telegrinder/types/objects.py
--rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 telegrinder-0.1.dev8/setup.py
--rw-r--r--   0        0        0      808 1970-01-01 00:00:00.000000 telegrinder-0.1.dev8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-04-17 10:00:22.519972 telegrinder-0.1.dev9/LICENSE
+-rw-r--r--   0        0        0      490 2022-10-19 10:48:59.359801 telegrinder-0.1.dev9/pyproject.toml
+-rw-r--r--   0        0        0      722 2022-10-09 16:36:29.440236 telegrinder-0.1.dev9/telegrinder/__init__.py
+-rw-r--r--   0        0        0      124 2022-10-05 12:31:51.515560 telegrinder-0.1.dev9/telegrinder/api/__init__.py
+-rw-r--r--   0        0        0     1002 2022-10-10 13:55:09.234603 telegrinder-0.1.dev9/telegrinder/api/abc.py
+-rw-r--r--   0        0        0     1993 2022-10-12 17:10:49.127709 telegrinder-0.1.dev9/telegrinder/api/api.py
+-rw-r--r--   0        0        0      162 2022-10-09 17:03:40.721083 telegrinder-0.1.dev9/telegrinder/api/error.py
+-rw-r--r--   0        0        0      463 2022-10-09 16:45:29.841169 telegrinder-0.1.dev9/telegrinder/api/response.py
+-rw-r--r--   0        0        0      391 2022-08-07 12:51:13.884678 telegrinder-0.1.dev9/telegrinder/bot/__init__.py
+-rw-r--r--   0        0        0     1802 2022-10-19 10:42:08.341854 telegrinder-0.1.dev9/telegrinder/bot/bot.py
+-rw-r--r--   0        0        0      121 2022-08-07 12:51:13.884858 telegrinder-0.1.dev9/telegrinder/bot/cute_types/__init__.py
+-rw-r--r--   0        0        0      792 2022-10-09 17:03:40.722525 telegrinder-0.1.dev9/telegrinder/bot/cute_types/callback_query.py
+-rw-r--r--   0        0        0     1034 2022-10-09 17:03:40.723014 telegrinder-0.1.dev9/telegrinder/bot/cute_types/inline_query.py
+-rw-r--r--   0        0        0     2284 2022-10-09 17:03:40.723789 telegrinder-0.1.dev9/telegrinder/bot/cute_types/message.py
+-rw-r--r--   0        0        0      240 2022-08-07 12:51:13.885192 telegrinder-0.1.dev9/telegrinder/bot/dispatch/__init__.py
+-rw-r--r--   0        0        0      448 2022-10-05 15:55:53.816795 telegrinder-0.1.dev9/telegrinder/bot/dispatch/abc.py
+-rw-r--r--   0        0        0     2931 2022-10-19 10:46:47.753146 telegrinder-0.1.dev9/telegrinder/bot/dispatch/dispatch.py
+-rw-r--r--   0        0        0       58 2022-04-20 18:58:21.519892 telegrinder-0.1.dev9/telegrinder/bot/dispatch/handler/__init__.py
+-rw-r--r--   0        0        0      411 2022-10-06 16:37:24.658158 telegrinder-0.1.dev9/telegrinder/bot/dispatch/handler/abc.py
+-rw-r--r--   0        0        0     1482 2022-10-09 17:03:40.725135 telegrinder-0.1.dev9/telegrinder/bot/dispatch/handler/func.py
+-rw-r--r--   0        0        0       31 2022-04-22 08:48:08.508568 telegrinder-0.1.dev9/telegrinder/bot/dispatch/middleware/__init__.py
+-rw-r--r--   0        0        0      268 2022-04-22 08:48:08.506726 telegrinder-0.1.dev9/telegrinder/bot/dispatch/middleware/abc.py
+-rw-r--r--   0        0        0     2000 2022-10-19 10:46:47.757369 telegrinder-0.1.dev9/telegrinder/bot/dispatch/process.py
+-rw-r--r--   0        0        0      146 2022-08-07 12:51:13.885835 telegrinder-0.1.dev9/telegrinder/bot/dispatch/view/__init__.py
+-rw-r--r--   0        0        0      389 2022-10-05 15:56:33.906807 telegrinder-0.1.dev9/telegrinder/bot/dispatch/view/abc.py
+-rw-r--r--   0        0        0     1803 2022-10-19 05:32:17.783830 telegrinder-0.1.dev9/telegrinder/bot/dispatch/view/callback_query.py
+-rw-r--r--   0        0        0     1769 2022-10-19 05:32:17.779302 telegrinder-0.1.dev9/telegrinder/bot/dispatch/view/inline_query.py
+-rw-r--r--   0        0        0     2043 2022-10-19 05:32:17.799043 telegrinder-0.1.dev9/telegrinder/bot/dispatch/view/message.py
+-rw-r--r--   0        0        0      990 2022-10-09 17:03:40.726368 telegrinder-0.1.dev9/telegrinder/bot/dispatch/waiter.py
+-rw-r--r--   0        0        0       57 2022-04-16 18:15:00.717683 telegrinder-0.1.dev9/telegrinder/bot/polling/__init__.py
+-rw-r--r--   0        0        0      401 2022-10-05 16:13:52.521597 telegrinder-0.1.dev9/telegrinder/bot/polling/abc.py
+-rw-r--r--   0        0        0     1893 2022-10-10 14:18:43.785077 telegrinder-0.1.dev9/telegrinder/bot/polling/polling.py
+-rw-r--r--   0        0        0      364 2022-10-18 08:21:39.198635 telegrinder-0.1.dev9/telegrinder/bot/rules/__init__.py
+-rw-r--r--   0        0        0     3027 2022-10-18 13:30:21.755501 telegrinder-0.1.dev9/telegrinder/bot/rules/abc.py
+-rw-r--r--   0        0        0      683 2022-10-05 16:22:23.755433 telegrinder-0.1.dev9/telegrinder/bot/rules/callback_data.py
+-rw-r--r--   0        0        0      859 2022-10-05 16:26:12.738773 telegrinder-0.1.dev9/telegrinder/bot/rules/func.py
+-rw-r--r--   0        0        0      675 2022-10-05 12:31:51.543146 telegrinder-0.1.dev9/telegrinder/bot/rules/fuzzy.py
+-rw-r--r--   0        0        0      419 2022-10-18 13:32:16.909888 telegrinder-0.1.dev9/telegrinder/bot/rules/integer.py
+-rw-r--r--   0        0        0      306 2022-08-09 15:45:11.810780 telegrinder-0.1.dev9/telegrinder/bot/rules/is_from.py
+-rw-r--r--   0        0        0      848 2022-10-05 16:22:34.205327 telegrinder-0.1.dev9/telegrinder/bot/rules/markup.py
+-rw-r--r--   0        0        0      877 2022-10-18 17:38:53.362772 telegrinder-0.1.dev9/telegrinder/bot/rules/regex.py
+-rw-r--r--   0        0        0      759 2022-10-18 13:32:16.914222 telegrinder-0.1.dev9/telegrinder/bot/rules/text.py
+-rw-r--r--   0        0        0       60 2022-04-26 20:09:36.774195 telegrinder-0.1.dev9/telegrinder/bot/scenario/__init__.py
+-rw-r--r--   0        0        0      289 2022-04-26 20:04:34.251102 telegrinder-0.1.dev9/telegrinder/bot/scenario/abc.py
+-rw-r--r--   0        0        0     3655 2022-09-11 11:14:52.608453 telegrinder-0.1.dev9/telegrinder/bot/scenario/checkbox.py
+-rw-r--r--   0        0        0       74 2022-10-09 16:34:03.453588 telegrinder-0.1.dev9/telegrinder/client/__init__.py
+-rw-r--r--   0        0        0     1305 2022-10-09 17:03:40.727766 telegrinder-0.1.dev9/telegrinder/client/abc.py
+-rw-r--r--   0        0        0     3556 2022-10-19 10:44:15.139353 telegrinder-0.1.dev9/telegrinder/client/aiohttp.py
+-rw-r--r--   0        0        0     1305 2022-10-12 17:10:02.257864 telegrinder-0.1.dev9/telegrinder/model.py
+-rw-r--r--   0        0        0     2286 2022-10-19 05:23:47.186405 telegrinder-0.1.dev9/telegrinder/modules.py
+-rw-r--r--   0        0        0      904 2022-10-09 16:34:03.446826 telegrinder-0.1.dev9/telegrinder/result.py
+-rw-r--r--   0        0        0      317 2022-10-09 16:34:03.450525 telegrinder-0.1.dev9/telegrinder/tools/__init__.py
+-rw-r--r--   0        0        0     1277 2022-04-17 05:35:56.975145 telegrinder-0.1.dev9/telegrinder/tools/buttons.py
+-rw-r--r--   0        0        0      102 2022-07-03 07:15:53.180547 telegrinder-0.1.dev9/telegrinder/tools/formatting/__init__.py
+-rw-r--r--   0        0        0      958 2022-08-07 12:51:13.875127 telegrinder-0.1.dev9/telegrinder/tools/formatting/abc.py
+-rw-r--r--   0        0        0     1606 2022-10-05 12:31:51.565411 telegrinder-0.1.dev9/telegrinder/tools/formatting/html.py
+-rw-r--r--   0        0        0     1833 2022-08-11 11:39:10.120725 telegrinder-0.1.dev9/telegrinder/tools/formatting/markdown.py
+-rw-r--r--   0        0        0       86 2022-05-10 13:21:05.250288 telegrinder-0.1.dev9/telegrinder/tools/kb_set/__init__.py
+-rw-r--r--   0        0        0      191 2022-05-10 12:42:26.141026 telegrinder-0.1.dev9/telegrinder/tools/kb_set/base.py
+-rw-r--r--   0        0        0     1830 2022-08-07 12:51:13.886941 telegrinder-0.1.dev9/telegrinder/tools/kb_set/yaml.py
+-rw-r--r--   0        0        0     2910 2022-07-04 07:26:47.118891 telegrinder-0.1.dev9/telegrinder/tools/keyboard.py
+-rw-r--r--   0        0        0     1201 2022-10-18 17:34:13.359753 telegrinder-0.1.dev9/telegrinder/tools/magic.py
+-rw-r--r--   0        0        0      147 2022-07-03 07:28:46.397440 telegrinder-0.1.dev9/telegrinder/tools/parse_mode.py
+-rw-r--r--   0        0        0       39 2022-10-06 21:09:42.264757 telegrinder-0.1.dev9/telegrinder/typegen/__init__.py
+-rw-r--r--   0        0        0       60 2022-10-06 21:00:00.907223 telegrinder-0.1.dev9/telegrinder/typegen/__main__.py
+-rw-r--r--   0        0        0      767 2022-10-10 14:25:57.752535 telegrinder-0.1.dev9/telegrinder/typegen/nicification.py
+-rw-r--r--   0        0        0     8284 2022-10-18 13:32:16.988246 telegrinder-0.1.dev9/telegrinder/typegen/schema_generator.py
+-rw-r--r--   0        0        0       40 2022-10-10 14:26:02.207568 telegrinder-0.1.dev9/telegrinder/types/__init__.py
+-rw-r--r--   0        0        0    50649 2022-10-10 14:26:02.945020 telegrinder-0.1.dev9/telegrinder/types/methods.py
+-rw-r--r--   0        0        0    76929 2022-10-18 13:32:17.373504 telegrinder-0.1.dev9/telegrinder/types/objects.py
+-rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 telegrinder-0.1.dev9/setup.py
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 telegrinder-0.1.dev9/PKG-INFO
```

### Comparing `telegrinder-0.1.dev8/LICENSE` & `telegrinder-0.1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/__init__.py` & `telegrinder-0.1.dev9/telegrinder/__init__.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/api/abc.py` & `telegrinder-0.1.dev9/telegrinder/api/abc.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/api/api.py` & `telegrinder-0.1.dev9/telegrinder/api/api.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/bot.py` & `telegrinder-0.1.dev9/telegrinder/bot/bot.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,20 +30,24 @@
 
     async def run_polling(self, offset: int = 0, skip_updates: bool = False) -> None:
         if skip_updates:
             logger.debug("dropping pending updates")
             await self.reset_webhook()
             await self.api.delete_webhook(drop_pending_updates=True)
         self.polling.offset = offset
+
+        loop = asyncio.get_running_loop()
+        assert loop, "No running loop"
+
         async for updates in self.polling.listen():
             for update in updates:
-                logger.debug("received update (update_id=%d)", update.update_id)
-                self.dispatch.loop.create_task(self.dispatch.feed(update, self.api))
+                logger.debug("received update (update_id={})", update.update_id)
+                loop.create_task(self.dispatch.feed(update, self.api))
 
     def run_forever(self, offset: int = 0, skip_updates: bool = False) -> None:
-        logger.debug("running blocking polling (id=%d)", self.api.id)
-        loop = asyncio.get_event_loop()
+        logger.debug("running blocking polling (id={})", self.api.id)
+        loop = asyncio.new_event_loop()
         loop.create_task(self.run_polling(offset, skip_updates=skip_updates))
         try:
             loop.run_forever()
         except KeyboardInterrupt:
             logger.info("KeyboardInterrupt")
```

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/cute_types/callback_query.py` & `telegrinder-0.1.dev9/telegrinder/bot/cute_types/callback_query.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/cute_types/inline_query.py` & `telegrinder-0.1.dev9/telegrinder/bot/cute_types/inline_query.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/cute_types/message.py` & `telegrinder-0.1.dev9/telegrinder/bot/cute_types/message.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/dispatch/dispatch.py` & `telegrinder-0.1.dev9/telegrinder/bot/dispatch/dispatch.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 DEFAULT_DATACLASS = Update
 
 
 class Dispatch(ABCDispatch):
     def __init__(self):
         self.default_handlers: typing.List[ABCHandler] = []
-        self.loop = asyncio.get_event_loop()
         self.message = MessageView()
         self.callback_query = CallbackQueryView()
         self.inline_query = InlineQueryView()
         self.views = ["message", "callback_query", "inline_query"]
 
     def handle(
         self,
@@ -55,31 +54,34 @@
             view = getattr(self, view_name)
             assert view, f"View {view_name} is undefined in dispatch"
             view_external = getattr(external, view_name)
             assert view_external, f"View {view_name} is undefined in external dispatch"
             view.load(view_external)
 
     async def feed(self, event: Update, api: ABCAPI) -> bool:
-        logger.debug("processing update (update_id=%d)", event.update_id)
+        logger.debug("processing update (update_id={})", event.update_id)
         for view in self.get_views():
             if await view.check(event):
                 logger.debug(
-                    "update %d matched view %s",
+                    "update {} matched view {}",
                     event.update_id,
                     view.__class__.__name__,
                 )
                 await view.process(event, api)
                 return True
 
+        loop = asyncio.get_running_loop()
+        assert loop, "No running loop"
+
         found = False
         for handler in self.default_handlers:
             result = await handler.check(api, event)
             if result:
                 found = True
-                self.loop.create_task(handler.run(event))
+                loop.create_task(handler.run(event))
                 if handler.is_blocking:
                     return True
         return found
 
     def mount(self, view_t: typing.Type["ABCView"], name: str):
         self.views.append(name)
         setattr(self, name, view_t)
```

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/dispatch/handler/func.py` & `telegrinder-0.1.dev9/telegrinder/bot/dispatch/handler/func.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/dispatch/process.py` & `telegrinder-0.1.dev9/telegrinder/bot/dispatch/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     raw_event: dict,
     str_handler: typing.Callable,
 ) -> bool:
     if key not in waiters:
         return False
 
     logger.debug(
-        "update %s found in waiter (key=%s)", event.__class__.__name__, str(key)
+        "update {} found in waiter (key={})", event.__class__.__name__, str(key)
     )
 
     waiter = waiters[key]
     ctx = {}
 
     for rule in waiter.rules:
         chk_event = event
@@ -50,15 +50,15 @@
 
 async def process_inner(
     event: T,
     raw_event: Update,
     middlewares: typing.List[ABCMiddleware[T]],
     handlers: typing.List[ABCHandler[T]],
 ) -> bool:
-    logger.debug("processing %s", event.__class__.__name__)
+    logger.debug("processing {}", event.__class__.__name__)
     ctx = {}
 
     for middleware in middlewares:
         if await middleware.pre(event, ctx) is False:
             return False
 
     found = False
```

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/dispatch/view/callback_query.py` & `telegrinder-0.1.dev9/telegrinder/bot/dispatch/view/callback_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,21 @@
 from telegrinder.bot.rules import ABCRule
 from telegrinder.bot.cute_types import CallbackQueryCute
 from telegrinder.api.abc import ABCAPI
 from telegrinder.bot.dispatch.waiter import WithWaiter
 from telegrinder.bot.dispatch.process import process_waiters, process_inner
 from telegrinder.types import Update
 import typing
-import asyncio
 
 
 class CallbackQueryView(ABCView, WithWaiter[int, CallbackQueryCute]):
     def __init__(self):
         self.handlers: typing.List[ABCHandler[CallbackQueryCute]] = []
         self.middlewares: typing.List[ABCMiddleware[CallbackQueryCute]] = []
         self.short_waiters: typing.Dict[int, Waiter] = {}
-        self.loop = asyncio.get_event_loop()
 
     def __call__(self, *rules: ABCRule, is_blocking: bool = True):
         def wrapper(func: typing.Callable[..., typing.Coroutine]):
             self.handlers.append(
                 FuncHandler(func, list(rules), is_blocking, dataclass=None)
             )
             return func
```

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/dispatch/view/inline_query.py` & `telegrinder-0.1.dev9/telegrinder/bot/dispatch/view/inline_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,21 @@
 from telegrinder.bot.rules import ABCRule
 from telegrinder.bot.cute_types import InlineQueryCute
 from telegrinder.api.abc import ABCAPI
 from telegrinder.bot.dispatch.waiter import WithWaiter
 from telegrinder.bot.dispatch.process import process_waiters, process_inner
 from telegrinder.types import Update
 import typing
-import asyncio
 
 
 class InlineQueryView(ABCView, WithWaiter[str, InlineQueryCute]):
     def __init__(self):
         self.handlers: typing.List[ABCHandler[InlineQueryCute]] = []
         self.middlewares: typing.List[ABCMiddleware[InlineQueryCute]] = []
         self.short_waiters: typing.Dict[str, Waiter] = {}
-        self.loop = asyncio.get_event_loop()
 
     def __call__(self, *rules: ABCRule, is_blocking: bool = True):
         def wrapper(func: typing.Callable[..., typing.Coroutine]):
             self.handlers.append(
                 FuncHandler(func, list(rules), is_blocking, dataclass=None)
             )
             return func
```

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/dispatch/view/message.py` & `telegrinder-0.1.dev9/telegrinder/bot/dispatch/view/message.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,23 +5,21 @@
 from telegrinder.bot.rules import ABCRule
 from telegrinder.bot.cute_types import MessageCute
 from telegrinder.api.abc import ABCAPI
 from telegrinder.bot.dispatch.waiter import WithWaiter, DefaultWaiterHandler
 from telegrinder.bot.dispatch.process import process_waiters, process_inner
 from telegrinder.types import Update
 import typing
-import asyncio
 
 
 class MessageView(ABCView, WithWaiter[int, MessageCute]):
     def __init__(self):
         self.handlers: typing.List[ABCHandler[MessageCute]] = []
         self.middlewares: typing.List[ABCMiddleware[MessageCute]] = []
         self.short_waiters: typing.Dict[int, Waiter] = {}
-        self.loop = asyncio.get_event_loop()
 
     def __call__(self, *rules: ABCRule, is_blocking: bool = True):
         def wrapper(func: typing.Callable[..., typing.Coroutine]):
             self.handlers.append(
                 FuncHandler(func, list(rules), is_blocking, dataclass=None)
             )
             return func
```

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/dispatch/waiter.py` & `telegrinder-0.1.dev9/telegrinder/bot/dispatch/waiter.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/polling/polling.py` & `telegrinder-0.1.dev9/telegrinder/bot/polling/polling.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/rules/abc.py` & `telegrinder-0.1.dev9/telegrinder/bot/rules/abc.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/rules/callback_data.py` & `telegrinder-0.1.dev9/telegrinder/bot/rules/callback_data.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/rules/func.py` & `telegrinder-0.1.dev9/telegrinder/bot/rules/func.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/rules/fuzzy.py` & `telegrinder-0.1.dev9/telegrinder/bot/rules/fuzzy.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/rules/markup.py` & `telegrinder-0.1.dev9/telegrinder/bot/rules/markup.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/rules/regex.py` & `telegrinder-0.1.dev9/telegrinder/bot/rules/regex.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/rules/text.py` & `telegrinder-0.1.dev9/telegrinder/bot/rules/text.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/bot/scenario/checkbox.py` & `telegrinder-0.1.dev9/telegrinder/bot/scenario/checkbox.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/client/abc.py` & `telegrinder-0.1.dev9/telegrinder/client/abc.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/client/aiohttp.py` & `telegrinder-0.1.dev9/telegrinder/client/aiohttp.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,21 +11,19 @@
 if typing.TYPE_CHECKING:
     from aiohttp import ClientResponse
 
 
 class AiohttpClient(ABCClient):
     def __init__(
         self,
-        loop: typing.Optional[ClientSession] = None,
         session: typing.Optional[ClientSession] = None,
         json_processing_module: typing.Optional[JSONModule] = None,
         timeout: typing.Optional[aiohttp.ClientTimeout] = None,
         **session_params
     ):
-        self.loop = loop
         self.session = session
         self.json_processing_module = json_processing_module or json
         self.session_params = session_params
         self.timeout = timeout or aiohttp.ClientTimeout(total=0)
 
     async def request_raw(
         self,
@@ -101,15 +99,15 @@
         form = aiohttp.formdata.FormData(quote_fields=False)
         for k, v in data.items():
             params = {}
             if isinstance(v, tuple):
                 params["filename"], v = v[0], v[1]
             else:
                 v = str(v)
-            form.add_field(k, v)
+            form.add_field(k, v, **params)
         return form
 
     def __del__(self):
         if self.session and not self.session.closed:
             if self.session._connector is not None and self.session._connector_owner:
                 self.session._connector.close()
             self.session._connector = None
```

### Comparing `telegrinder-0.1.dev8/telegrinder/model.py` & `telegrinder-0.1.dev9/telegrinder/model.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/result.py` & `telegrinder-0.1.dev9/telegrinder/result.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/tools/buttons.py` & `telegrinder-0.1.dev9/telegrinder/tools/buttons.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/tools/formatting/abc.py` & `telegrinder-0.1.dev9/telegrinder/tools/formatting/abc.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/tools/formatting/html.py` & `telegrinder-0.1.dev9/telegrinder/tools/formatting/html.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/tools/formatting/markdown.py` & `telegrinder-0.1.dev9/telegrinder/tools/formatting/markdown.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/tools/kb_set/yaml.py` & `telegrinder-0.1.dev9/telegrinder/tools/kb_set/yaml.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/tools/keyboard.py` & `telegrinder-0.1.dev9/telegrinder/tools/keyboard.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/tools/magic.py` & `telegrinder-0.1.dev9/telegrinder/tools/magic.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/typegen/nicification.py` & `telegrinder-0.1.dev9/telegrinder/typegen/nicification.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/typegen/schema_generator.py` & `telegrinder-0.1.dev9/telegrinder/typegen/schema_generator.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/types/methods.py` & `telegrinder-0.1.dev9/telegrinder/types/methods.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/telegrinder/types/objects.py` & `telegrinder-0.1.dev9/telegrinder/types/objects.py`

 * *Files identical despite different names*

### Comparing `telegrinder-0.1.dev8/setup.py` & `telegrinder-0.1.dev9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,16 +31,16 @@
  'envparse>=0.2.0,<0.3.0',
  'msgspec>=0.9.0,<0.10.0',
  'requests>=2.28.1,<3.0.0',
  'vbml>=1.1.post1,<2.0']
 
 setup_kwargs = {
     'name': 'telegrinder',
-    'version': '0.1.dev8',
-    'description': 'Grinding telegram events – customizable tool to build telegram bots',
+    'version': '0.1.dev9',
+    'description': 'async telegram bot building',
     'long_description': 'None',
     'author': 'timoniq',
     'author_email': 'tesseradecades@mail.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `telegrinder-0.1.dev8/PKG-INFO` & `telegrinder-0.1.dev9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: telegrinder
-Version: 0.1.dev8
-Summary: Grinding telegram events – customizable tool to build telegram bots
+Version: 0.1.dev9
+Summary: async telegram bot building
 License: MIT
 Author: timoniq
 Author-email: tesseradecades@mail.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

