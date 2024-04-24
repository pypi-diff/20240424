# Comparing `tmp/ofscraper-3.9.0.dev9.tar.gz` & `tmp/ofscraper-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-3.9.0.dev9.tar", max compression
+gzip compressed data, was "ofscraper-3.9.1.tar", max compression
```

## Comparing `ofscraper-3.9.0.dev9.tar` & `ofscraper-3.9.1.tar`

### file list

```diff
@@ -1,179 +1,188 @@
--rw-r--r--   0        0        0     1067 2024-04-08 04:31:25.239239 ofscraper-3.9.0.dev9/LICENSE
--rw-r--r--   0        0        0     4188 2024-04-08 04:31:25.239239 ofscraper-3.9.0.dev9/README.md
--rwxr-xr-x   0        0        0      283 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/__main__.py
--rw-r--r--   0        0        0     1064 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/__version__.pye
--rw-r--r--   0        0        0        1 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/actions/__init__.py
--rw-r--r--   0        0        0     9230 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/actions/like.py
--rw-r--r--   0        0        0     9868 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/actions/process.py
--rw-r--r--   0        0        0    21931 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/actions/scraper.py
--rw-r--r--   0        0        0    15975 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/api/archive.py
--rw-r--r--   0        0        0    19152 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1479 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/api/init.py
--rw-r--r--   0        0        0    16927 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/api/labels.py
--rw-r--r--   0        0        0     4724 2024-04-08 04:31:25.243239 ofscraper-3.9.0.dev9/ofscraper/api/me.py
--rw-r--r--   0        0        0    19945 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/messages.py
--rw-r--r--   0        0        0    17203 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/paid.py
--rw-r--r--   0        0        0     9960 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     8914 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3069 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/helpers.py
--rw-r--r--   0        0        0     3036 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/individual.py
--rw-r--r--   0        0        0    14604 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/lists.py
--rw-r--r--   0        0        0    11817 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/subscriptions.py
--rw-r--r--   0        0        0    16816 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     1413 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/base.py
--rw-r--r--   0        0        0      876 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/labels.py
--rw-r--r--   0        0        0    15247 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/media.py
--rw-r--r--   0        0        0     5892 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/models.py
--rw-r--r--   0        0        0     1771 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/multiprocessprogress.py
--rw-r--r--   0        0        0    20470 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     5157 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/posts.py
--rw-r--r--   0        0        0      489 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/semaphoreDelayed.py
--rw-r--r--   0        0        0     8226 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/sessionbuilder.py
--rw-r--r--   0        0        0    31982 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/classes/table.py
--rw-r--r--   0        0        0    21412 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/commands/check.py
--rw-r--r--   0        0        0     9739 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/commands/manual.py
--rw-r--r--   0        0        0      430 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/commands/picker.py
--rwxr-xr-x   0        0        0     3915 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0       53 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/binary.py
--rw-r--r--   0        0        0     1580 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/config.py
--rw-r--r--   0        0        0      927 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/constants.py
--rw-r--r--   0        0        0       73 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/date.py
--rw-r--r--   0        0        0      184 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/download.py
--rw-r--r--   0        0        0      204 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/files.py
--rw-r--r--   0        0        0     1231 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/general.py
--rw-r--r--   0        0        0       93 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/logger.py
--rw-r--r--   0        0        0      775 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/other_url.py
--rw-r--r--   0        0        0     1876 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/prompts.py
--rw-r--r--   0        0        0      615 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/req.py
--rw-r--r--   0        0        0   265533 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/test_constants.py
--rw-r--r--   0        0        0      212 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/time.py
--rw-r--r--   0        0        0     3516 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/const/url.py
--rw-r--r--   0        0        0        1 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    11310 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations.py
--rw-r--r--   0        0        0      176 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/helpers.py
--rw-r--r--   0        0        0     8102 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/labels.py
--rw-r--r--   0        0        0    15102 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/media.py
--rw-r--r--   0        0        0     7983 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/messages.py
--rw-r--r--   0        0        0     8318 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/others.py
--rw-r--r--   0        0        0     9448 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/posts.py
--rw-r--r--   0        0        0     5914 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/profile.py
--rw-r--r--   0        0        0     7128 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/stories.py
--rw-r--r--   0        0        0     4597 2024-04-08 04:31:25.247238 ofscraper-3.9.0.dev9/ofscraper/db/operations_/wrapper.py
--rw-r--r--   0        0        0    14966 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/alt_download.py
--rw-r--r--   0        0        0    15078 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/alt_downloadbatch.py
--rw-r--r--   0        0        0     6173 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/common.py
--rw-r--r--   0        0        0     2699 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/globals.py
--rw-r--r--   0        0        0    12589 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/keyhelpers.py
--rw-r--r--   0        0        0     3451 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/log.py
--rw-r--r--   0        0        0      790 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/message.py
--rw-r--r--   0        0        0     5875 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/metadata.py
--rw-r--r--   0        0        0     2092 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/paths.py
--rw-r--r--   0        0        0      453 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/progress.py
--rw-r--r--   0        0        0     1161 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/sem.py
--rw-r--r--   0        0        0     1075 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/common/text.py
--rw-r--r--   0        0        0     3431 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/download.py
--rw-r--r--   0        0        0    16936 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/downloadbatch.py
--rw-r--r--   0        0        0     9047 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/downloadnormal.py
--rw-r--r--   0        0        0    13473 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/main_download.py
--rw-r--r--   0        0        0    14084 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/download/main_downloadbatch.py
--rw-r--r--   0        0        0     5480 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/media/helpers.py
--rw-r--r--   0        0        0    12331 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/media/main.py
--rw-r--r--   0        0        0     2682 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/models/date.py
--rw-r--r--   0        0        0     2532 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/models/flags.py
--rw-r--r--   0        0        0      586 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/models/other.py
--rw-r--r--   0        0        0     6342 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/models/price.py
--rw-r--r--   0        0        0     1415 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/models/sort.py
--rw-r--r--   0        0        0     1122 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/filters/models/subtype.py
--rw-r--r--   0        0        0     3436 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/models/retriver.py
--rw-r--r--   0        0        0     7125 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/models/selector.py
--rw-r--r--   0        0        0     2466 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/helpers/model_helpers.py
--rw-r--r--   0        0        0    13078 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/helpers/prompt_helpers.py
--rw-r--r--   0        0        0      846 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     7310 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0      917 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/actions.py
--rw-r--r--   0        0        0     6596 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/area.py
--rw-r--r--   0        0        0     8258 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/auth.py
--rw-r--r--   0        0        0     4622 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/binary.py
--rw-r--r--   0        0        0    27530 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/config.py
--rw-r--r--   0        0        0     1879 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/menu.py
--rw-r--r--   0        0        0    16008 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/model.py
--rw-r--r--   0        0        0     4135 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/profile.py
--rw-r--r--   0        0        0     7589 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    10184 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0     1290 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0      567 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/runner/exit.py
--rw-r--r--   0        0        0     1486 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/runner/load.py
--rw-r--r--   0        0        0     2748 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/runner/run.py
--rw-r--r--   0        0        0        1 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     3803 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/actions.py
--rw-r--r--   0        0        0     1838 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/areas.py
--rw-r--r--   0        0        0       12 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/globals.py
--rw-r--r--   0        0        0     6289 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/common_args.py
--rw-r--r--   0        0        0    20274 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/main_args.py
--rw-r--r--   0        0        0     1302 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/manual_args.py
--rw-r--r--   0        0        0     1587 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/message_args.py
--rw-r--r--   0        0        0     1582 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/paid_args.py
--rw-r--r--   0        0        0     1956 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/post_args.py
--rw-r--r--   0        0        0     1635 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/story_args.py
--rw-r--r--   0        0        0     5623 2024-04-08 04:31:25.251239 ofscraper-3.9.0.dev9/ofscraper/utils/args/helpers.py
--rw-r--r--   0        0        0     1684 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/args/parse.py
--rw-r--r--   0        0        0      395 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/args/quality.py
--rw-r--r--   0        0        0      863 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/args/read.py
--rw-r--r--   0        0        0      718 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/args/user.py
--rw-r--r--   0        0        0      261 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/args/write.py
--rw-r--r--   0        0        0     2148 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/auth/context.py
--rw-r--r--   0        0        0     1680 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/auth/data.py
--rw-r--r--   0        0        0     2131 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/auth/file.py
--rw-r--r--   0        0        0     2844 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/auth/helpers.py
--rw-r--r--   0        0        0     1756 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/auth/make.py
--rw-r--r--   0        0        0     6092 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/auth/request.py
--rw-r--r--   0        0        0      802 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/auth/schema.py
--rw-r--r--   0        0        0     9824 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0     1780 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/cache.py
--rw-r--r--   0        0        0     1650 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/checkers.py
--rw-r--r--   0        0        0     2894 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/config.py
--rw-r--r--   0        0        0     1090 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/context.py
--rw-r--r--   0        0        0      452 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/custom.py
--rw-r--r--   0        0        0    23180 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/data.py
--rw-r--r--   0        0        0     2110 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/file.py
--rw-r--r--   0        0        0     2111 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/menu.py
--rw-r--r--   0        0        0     4716 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/schema.py
--rw-r--r--   0        0        0      405 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/config/wrapper.py
--rw-r--r--   0        0        0      499 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/console.py
--rw-r--r--   0        0        0      461 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/constants.py
--rw-r--r--   0        0        0     3401 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/context/exit.py
--rw-r--r--   0        0        0     1135 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/context/run_async.py
--rw-r--r--   0        0        0     1014 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/context/stdout.py
--rw-r--r--   0        0        0     2679 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/dates.py
--rw-r--r--   0        0        0     1040 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     1716 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/hash.py
--rw-r--r--   0        0        0     8325 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/classes.py
--rw-r--r--   0        0        0     2588 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/close.py
--rw-r--r--   0        0        0      477 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/globals.py
--rw-r--r--   0        0        0     1551 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/helpers.py
--rw-r--r--   0        0        0     2098 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/logger.py
--rw-r--r--   0        0        0     1672 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/logs.py
--rw-r--r--   0        0        0     5955 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/other.py
--rw-r--r--   0        0        0     3652 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/logs/stdout.py
--rw-r--r--   0        0        0      616 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/manager.py
--rw-r--r--   0        0        0      388 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/me.py
--rw-r--r--   0        0        0     4085 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/menu.py
--rw-r--r--   0        0        0     1732 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/paths/check.py
--rw-r--r--   0        0        0     3105 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/paths/common.py
--rw-r--r--   0        0        0      279 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/paths/manage.py
--rw-r--r--   0        0        0     5061 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/paths/paths.py
--rw-r--r--   0        0        0     1058 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/profiles/data.py
--rw-r--r--   0        0        0     2785 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/profiles/manage.py
--rw-r--r--   0        0        0     1606 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/profiles/tools.py
--rw-r--r--   0        0        0    10457 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/progress.py
--rw-r--r--   0        0        0     4447 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/run.py
--rw-r--r--   0        0        0      255 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/sems.py
--rw-r--r--   0        0        0     1595 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/separate.py
--rw-r--r--   0        0        0     3887 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/settings.py
--rw-r--r--   0        0        0      417 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/system/free.py
--rw-r--r--   0        0        0     3108 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/system/network.py
--rw-r--r--   0        0        0     2448 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/system/system.py
--rw-r--r--   0        0        0     2052 2024-04-08 04:31:25.255239 ofscraper-3.9.0.dev9/ofscraper/utils/text.py
--rw-r--r--   0        0        0     2123 2024-04-08 04:31:49.787098 ofscraper-3.9.0.dev9/pyproject.toml
--rw-r--r--   0        0        0     6349 1970-01-01 00:00:00.000000 ofscraper-3.9.0.dev9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-24 16:29:27.777091 ofscraper-3.9.1/LICENSE
+-rw-r--r--   0        0        0     4188 2024-04-24 16:29:27.777091 ofscraper-3.9.1/README.md
+-rwxr-xr-x   0        0        0      283 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/__main__.py
+-rw-r--r--   0        0        0     1064 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/__version__.pye
+-rw-r--r--   0        0        0        1 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/actions/__init__.py
+-rw-r--r--   0        0        0     8503 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/actions/like.py
+-rw-r--r--   0        0        0    10058 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/actions/process.py
+-rw-r--r--   0        0        0    22168 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/actions/scraper.py
+-rw-r--r--   0        0        0    15380 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/api/archive.py
+-rw-r--r--   0        0        0      274 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/api/common/logs.py
+-rw-r--r--   0        0        0    14634 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1479 2024-04-24 16:29:27.781091 ofscraper-3.9.1/ofscraper/api/init.py
+-rw-r--r--   0        0        0    14107 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     2912 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/me.py
+-rw-r--r--   0        0        0    18532 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/messages.py
+-rw-r--r--   0        0        0    13898 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     8079 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     6176 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     1768 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/subscriptions/helpers.py
+-rw-r--r--   0        0        0     3275 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/subscriptions/individual.py
+-rw-r--r--   0        0        0    11196 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/subscriptions/lists.py
+-rw-r--r--   0        0        0     8149 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/subscriptions/subscriptions.py
+-rw-r--r--   0        0        0    16397 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     1453 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/base.py
+-rw-r--r--   0        0        0      876 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0    15565 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     6005 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/models.py
+-rw-r--r--   0        0        0     1771 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/multiprocessprogress.py
+-rw-r--r--   0        0        0    20557 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     5152 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0      456 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/semaphoreDelayed.py
+-rw-r--r--   0        0        0    15929 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/sessionmanager.py
+-rw-r--r--   0        0        0    31982 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/classes/table.py
+-rw-r--r--   0        0        0    25956 2024-04-24 16:29:27.869090 ofscraper-3.9.1/ofscraper/commands/check.py
+-rw-r--r--   0        0        0    10964 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/commands/manual.py
+-rw-r--r--   0        0        0      430 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/commands/picker.py
+-rwxr-xr-x   0        0        0     3941 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0       53 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/binary.py
+-rw-r--r--   0        0        0     1655 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/config.py
+-rw-r--r--   0        0        0      966 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/constants.py
+-rw-r--r--   0        0        0       74 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/date.py
+-rw-r--r--   0        0        0      184 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/download.py
+-rw-r--r--   0        0        0      204 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/files.py
+-rw-r--r--   0        0        0     1333 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/general.py
+-rw-r--r--   0        0        0       93 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/logger.py
+-rw-r--r--   0        0        0       69 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/metadata.py
+-rw-r--r--   0        0        0      862 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/other_url.py
+-rw-r--r--   0        0        0     1907 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/prompts.py
+-rw-r--r--   0        0        0     1719 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/req.py
+-rw-r--r--   0        0        0   265533 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/test_constants.py
+-rw-r--r--   0        0        0      248 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/time.py
+-rw-r--r--   0        0        0     3612 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/const/url.py
+-rw-r--r--   0        0        0        1 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    14326 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/db/operations.py
+-rw-r--r--   0        0        0      206 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/db/operations_/helpers.py
+-rw-r--r--   0        0        0     8568 2024-04-24 16:29:27.785091 ofscraper-3.9.1/ofscraper/db/operations_/labels.py
+-rw-r--r--   0        0        0    19112 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/media.py
+-rw-r--r--   0        0        0     9805 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/merge.py
+-rw-r--r--   0        0        0     8504 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/messages.py
+-rw-r--r--   0        0        0     8928 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/others.py
+-rw-r--r--   0        0        0    10366 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/posts.py
+-rw-r--r--   0        0        0     6725 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/profile.py
+-rw-r--r--   0        0        0     7485 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/stories.py
+-rw-r--r--   0        0        0     4810 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/db/operations_/wrapper.py
+-rw-r--r--   0        0        0    10851 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/alt_download.py
+-rw-r--r--   0        0        0    10692 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/alt_downloadbatch.py
+-rw-r--r--   0        0        0     4852 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/download.py
+-rw-r--r--   0        0        0    17155 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/downloadbatch.py
+-rw-r--r--   0        0        0     9116 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/downloadnormal.py
+-rw-r--r--   0        0        0    10789 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/main_download.py
+-rw-r--r--   0        0        0    11235 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/main_downloadbatch.py
+-rw-r--r--   0        0        0     1261 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/classes/retries.py
+-rw-r--r--   0        0        0     1193 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/classes/session.py
+-rw-r--r--   0        0        0     3741 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/common/alt_common.py
+-rw-r--r--   0        0        0     6486 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/common/general.py
+-rw-r--r--   0        0        0     2054 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/common/main_common.py
+-rw-r--r--   0        0        0     2403 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/globals.py
+-rw-r--r--   0        0        0     9419 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/keyhelpers.py
+-rw-r--r--   0        0        0     3431 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/log.py
+-rw-r--r--   0        0        0      317 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/media.py
+-rw-r--r--   0        0        0      790 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/message.py
+-rw-r--r--   0        0        0     3884 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/metadata.py
+-rw-r--r--   0        0        0     2590 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/paths.py
+-rw-r--r--   0        0        0      453 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/progress.py
+-rw-r--r--   0        0        0     1155 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/download/shared/utils/text.py
+-rw-r--r--   0        0        0     7949 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/media/helpers.py
+-rw-r--r--   0        0        0     5019 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/media/main.py
+-rw-r--r--   0        0        0     2682 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/models/date.py
+-rw-r--r--   0        0        0     2532 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/models/flags.py
+-rw-r--r--   0        0        0      586 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/models/other.py
+-rw-r--r--   0        0        0     6342 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/models/price.py
+-rw-r--r--   0        0        0     1415 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/models/sort.py
+-rw-r--r--   0        0        0     1122 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/filters/models/subtype.py
+-rw-r--r--   0        0        0     3462 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/models/retriver.py
+-rw-r--r--   0        0        0     8003 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/models/selector.py
+-rw-r--r--   0        0        0     2466 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/helpers/model_helpers.py
+-rw-r--r--   0        0        0    15211 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/helpers/prompt_helpers.py
+-rw-r--r--   0        0        0      846 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     7747 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0      917 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/actions.py
+-rw-r--r--   0        0        0     6596 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/area.py
+-rw-r--r--   0        0        0     8258 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/auth.py
+-rw-r--r--   0        0        0     4622 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/binary.py
+-rw-r--r--   0        0        0    27896 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/config.py
+-rw-r--r--   0        0        0     1879 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/menu.py
+-rw-r--r--   0        0        0     2615 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/merge.py
+-rw-r--r--   0        0        0    16078 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/model.py
+-rw-r--r--   0        0        0     4135 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_groups/profile.py
+-rw-r--r--   0        0        0     7609 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    10184 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0     1342 2024-04-24 16:29:27.789090 ofscraper-3.9.1/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      567 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/runner/exit.py
+-rw-r--r--   0        0        0     1486 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/runner/load.py
+-rw-r--r--   0        0        0     2748 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/runner/run.py
+-rw-r--r--   0        0        0        1 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     3803 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/actions.py
+-rw-r--r--   0        0        0     1838 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/areas.py
+-rw-r--r--   0        0        0       12 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/globals.py
+-rw-r--r--   0        0        0     6624 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/groups/common_args.py
+-rw-r--r--   0        0        0    20010 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/groups/main_args.py
+-rw-r--r--   0        0        0     1318 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/groups/manual_args.py
+-rw-r--r--   0        0        0     1587 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/groups/message_args.py
+-rw-r--r--   0        0        0     1588 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/groups/paid_args.py
+-rw-r--r--   0        0        0     1955 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/groups/post_args.py
+-rw-r--r--   0        0        0     1641 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/groups/story_args.py
+-rw-r--r--   0        0        0     5623 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/helpers.py
+-rw-r--r--   0        0        0     1928 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/parse.py
+-rw-r--r--   0        0        0      395 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/quality.py
+-rw-r--r--   0        0        0      863 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/read.py
+-rw-r--r--   0        0        0      721 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/user.py
+-rw-r--r--   0        0        0      261 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/args/write.py
+-rw-r--r--   0        0        0     2148 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/auth/context.py
+-rw-r--r--   0        0        0     1680 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/auth/data.py
+-rw-r--r--   0        0        0     2034 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/auth/file.py
+-rw-r--r--   0        0        0     2844 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/auth/helpers.py
+-rw-r--r--   0        0        0     1756 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/auth/make.py
+-rw-r--r--   0        0        0     6940 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/auth/request.py
+-rw-r--r--   0        0        0      802 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/auth/schema.py
+-rw-r--r--   0        0        0     9824 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0     1780 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/cache.py
+-rw-r--r--   0        0        0     1650 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/checkers.py
+-rw-r--r--   0        0        0     2894 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/config.py
+-rw-r--r--   0        0        0     1447 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/context.py
+-rw-r--r--   0        0        0      522 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/custom.py
+-rw-r--r--   0        0        0    23743 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/data.py
+-rw-r--r--   0        0        0     2146 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/file.py
+-rw-r--r--   0        0        0     2111 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/menu.py
+-rw-r--r--   0        0        0     4797 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/schema.py
+-rw-r--r--   0        0        0      405 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/config/wrapper.py
+-rw-r--r--   0        0        0      499 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      786 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/constants.py
+-rw-r--r--   0        0        0     3401 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/context/exit.py
+-rw-r--r--   0        0        0     1135 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/context/run_async.py
+-rw-r--r--   0        0        0     1014 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/context/stdout.py
+-rw-r--r--   0        0        0     3460 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0     1040 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     1716 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/hash.py
+-rw-r--r--   0        0        0     7231 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/classes.py
+-rw-r--r--   0        0        0     2588 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/close.py
+-rw-r--r--   0        0        0      477 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/globals.py
+-rw-r--r--   0        0        0     1736 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/helpers.py
+-rw-r--r--   0        0        0     2098 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/logger.py
+-rw-r--r--   0        0        0     1672 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/logs.py
+-rw-r--r--   0        0        0     5955 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/other.py
+-rw-r--r--   0        0        0     3652 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/logs/stdout.py
+-rw-r--r--   0        0        0      617 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/manager.py
+-rw-r--r--   0        0        0      388 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/me.py
+-rw-r--r--   0        0        0     4200 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/menu.py
+-rw-r--r--   0        0        0      659 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/merge.py
+-rw-r--r--   0        0        0     1732 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/paths/check.py
+-rw-r--r--   0        0        0     3092 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/paths/common.py
+-rw-r--r--   0        0        0      279 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/paths/manage.py
+-rw-r--r--   0        0        0     5218 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/paths/paths.py
+-rw-r--r--   0        0        0     1058 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/profiles/data.py
+-rw-r--r--   0        0        0     2785 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/profiles/manage.py
+-rw-r--r--   0        0        0     1606 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/profiles/tools.py
+-rw-r--r--   0        0        0    10649 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/progress.py
+-rw-r--r--   0        0        0     4447 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/run.py
+-rw-r--r--   0        0        0        1 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/sems.py
+-rw-r--r--   0        0        0     1595 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0     4038 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/settings.py
+-rw-r--r--   0        0        0      417 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/system/free.py
+-rw-r--r--   0        0        0     3285 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/system/network.py
+-rw-r--r--   0        0        0     2472 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/system/system.py
+-rw-r--r--   0        0        0     2052 2024-04-24 16:29:27.793090 ofscraper-3.9.1/ofscraper/utils/text.py
+-rw-r--r--   0        0        0     2142 2024-04-24 16:29:53.460801 ofscraper-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6388 1970-01-01 00:00:00.000000 ofscraper-3.9.1/PKG-INFO
```

### Comparing `ofscraper-3.9.0.dev9/LICENSE` & `ofscraper-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/README.md` & `ofscraper-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/__version__.py` & `ofscraper-3.9.1/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/__version__.pye` & `ofscraper-3.9.1/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/actions/like.py` & `ofscraper-3.9.1/ofscraper/actions/like.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,60 +8,57 @@
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
 import asyncio
+import functools
 import logging
-import traceback
+import time
 
 from rich.progress import (
     BarColumn,
     MofNCompleteColumn,
     Progress,
     SpinnerColumn,
     TextColumn,
 )
 from rich.style import Style
-from tenacity import (
-    AsyncRetrying,
-    retry,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random,
-)
 
 import ofscraper.api.archive as archive
 import ofscraper.api.labels as labels_api
 import ofscraper.api.pinned as pinned
 import ofscraper.api.timeline as timeline
-import ofscraper.classes.labels as labels
 import ofscraper.classes.posts as posts_
-import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.args.areas as areas
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.console as console
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.system.system as system
-from ofscraper.classes.semaphoreDelayed import semaphoreDelayed
 from ofscraper.utils.context.run_async import run
 
-sem = semaphoreDelayed(1)
 log = logging.getLogger("shared")
 
 
 @run
 async def get_posts(model_id, username):
     responses = []
     final_post_areas = set(areas.get_like_area())
     tasks = []
     with progress_utils.setup_api_split_progress_live():
-        async with sessionbuilder.sessionBuilder() as c:
+        async with sessionManager.sessionManager(
+            sem=constants.getattr("LIKE_MAX_SEMS"),
+            retries=constants.getattr("API_NUM_TRIES"),
+            wait_min=constants.getattr("OF_MIN_WAIT_API"),
+            wait_max=constants.getattr("OF_MAX_WAIT_API"),
+            new_request_auth=True,
+        ) as c:
             while True:
                 max_count = min(
                     constants.getattr("API_MAX_AREAS"),
                     system.getcpu_count(),
                     len(final_post_areas),
                 )
                 if not bool(tasks) and not bool(final_post_areas):
@@ -145,21 +142,21 @@
 
 def get_post_for_like(model_id, username):
     post = get_posts(model_id, username)
     return filter_for_unfavorited(post)
 
 
 def filter_for_unfavorited(posts: list) -> list:
-    output = list(filter(lambda x: x.favorited == False, posts))
+    output = list(filter(lambda x: x.favorited == False and x.opened, posts))
     log.debug(f"[bold]Number of unliked post[/bold] {len(output)}")
     return output
 
 
 def filter_for_favorited(posts: list) -> list:
-    output = list(filter(lambda x: x.favorited == True, posts))
+    output = list(filter(lambda x: x.favorited == True and x.opened, posts))
     log.debug(f"[bold]Number of liked post[/bold] {len(output)}")
     return output
 
 
 def pre_filter(posts):
     valid_post = list(filter(lambda x: x.opened, posts))
     seen = set()
@@ -168,83 +165,60 @@
     ]
 
 
 def get_post_ids(posts: list) -> list:
     return list(map(lambda x: x.id, posts))
 
 
-def like(model_id, username, ids: list):
-    _like(model_id, username, ids, True)
+def like(model_id, ids: list):
+    _like(model_id, ids, True)
 
 
-def unlike(model_id, username, ids: list):
-    _like(model_id, username, ids, False)
+def unlike(model_id, ids: list):
+    _like(model_id, ids, False)
 
 
-@run
-async def _like(model_id, username, ids: list, like_action: bool):
+def _like(model_id, ids: list, like_action: bool):
     title = "Liking" if like_action else "Unliking"
-    global sem
-    sem.delay = 3
     with Progress(
         SpinnerColumn(style=Style(color="blue")),
         TextColumn("{task.description}"),
         BarColumn(),
         MofNCompleteColumn(),
         console=console.get_shared_console(),
     ) as overall_progress:
-        async with sessionbuilder.sessionBuilder() as c:
+        with sessionManager.sessionManager(
+            sem=1,
+            new_request_auth=True,
+            backend="httpx",
+            retries=constants.getattr("API_LIKE_NUM_TRIES"),
+            wait_min=constants.getattr("OF_MIN_WAIT_API"),
+            wait_max=constants.getattr("OF_MAX_WAIT_API"),
+        ) as c:
             tasks = []
             task1 = overall_progress.add_task(f"{title} posts...\n", total=len(ids))
 
             [
-                tasks.append(asyncio.create_task(_like_request(c, id, model_id)))
+                tasks.append(functools.partial(_like_request, c, id, model_id))
                 for id in ids
             ]
-            for count, coro in enumerate(asyncio.as_completed(tasks)):
-                id = await coro
+            sleep_duration = 3
+            for count, func in enumerate(tasks):
+                id = func()
                 log.debug(
                     f"ID: {id} Performed {'like' if like_action==True else 'unlike'} action"
                 )
-
                 if count + 1 % 60 == 0 and count + 1 % 50 == 0:
-                    sem.delay = 15
-                elif count + 1 % 60 == 0:
-                    sem.delay = 3
-                elif count + 1 % 50 == 0:
-                    sem.delay = 30
-
+                    sleep_duration = 40
+                elif count % 60 == 0:
+                    sleep_duration = 1  # Divisible by 60 - 1 second sleep
+                elif count % 50 == 0:
+                    sleep_duration = 30  # Divisible by 50 - 30 seconds sleep
                 overall_progress.update(task1, advance=1, refresh=True)
+                time.sleep(sleep_duration)
 
 
-async def _like_request(c, id, model_id):
-    global sem
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            await sem.acquire()
-            try:
-                async with c.requests(
-                    constants.getattr("favoriteEP").format(id, model_id), "post"
-                )() as r:
-                    if r.ok:
-                        return id
-                    else:
-                        log.debug(
-                            f"[bold]timeline response status code:[/bold]{r.status}"
-                        )
-                        log.debug(f"[bold]timeline response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
-                        r.raise_for_status()
-            except Exception as E:
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
-            finally:
-                sem.release()
+def _like_request(c, id, model_id):
+    with c.requests(
+        constants.getattr("favoriteEP").format(id, model_id), method="post"
+    ) as _:
+        return id
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/actions/process.py` & `ofscraper-3.9.1/ofscraper/actions/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
-import asyncio
 import logging
 import time
 import timeit
 import traceback
 from contextlib import contextmanager
 
 import arrow
@@ -65,15 +64,15 @@
 """
     )
 
 
 @exit.exit_wrapper
 def process_post():
     if read_args.retriveArgs().users_first:
-        asyncio.run(process_post_user_first())
+        process_post_user_first()
     else:
         normal_post_process()
 
 
 @exit.exit_wrapper
 def process_post_user_first():
     with scrape_context_manager():
@@ -83,35 +82,36 @@
             https://of-scraper.gitbook.io/of-scraper/config-options/customizing-save-path#warning[/red]      \
             "
             )
             time.sleep(constants.getattr("LOG_DISPLAY_TIMEOUT") * 3)
 
         profile_tools.print_current_profile()
         init.print_sign_status()
-        userdata = userselector.getselected_usernames(rescan=False)
-        length = len(userdata)
-        output = []
-        asyncio.create_task()
-
-        # log.info(f"Data retrival progressing on model {count+1}/{length}")
+        data = {}
+        for user in userselector.getselected_usernames(rescan=False):
+            data.update(process_user_first_data_retriver(user))
+        for model_id, val in data.items():
+            download.download_process(
+                val["username"], model_id, val["media"], posts=val["posts"]
+            )
 
 
-def process_user_first_helper(ele):
+def process_user_first_data_retriver(ele):
     if constants.getattr("SHOW_AVATAR") and ele.avatar:
         log.warning(f"Avatar : {ele.avatar}")
     if bool(areas.get_download_area()):
         log.info(
             f"Getting {','.join(areas.get_download_area())} for [bold]{ele.name}[/bold]\n[bold]Subscription Active:[/bold] {ele.active}"
         )
     try:
         model_id = ele.id
         username = ele.name
         operations.table_init_create(model_id=model_id, username=username)
-        results, posts = OF.process_areas(ele, model_id, job_progress=False)
-        return results
+        media, posts = OF.process_areas(ele, model_id)
+        return {model_id: {"username": username, "posts": posts, "media": media}}
     except Exception as e:
         if isinstance(e, KeyboardInterrupt):
             raise e
         log.traceback_(f"failed with exception: {e}")
         log.traceback_(traceback.format_exc())
 
 
@@ -156,16 +156,16 @@
             if constants.getattr("SHOW_AVATAR") and ele.avatar:
                 log.warning(f"Avatar : {ele.avatar}")
             log.warning(
                 f"Getting {','.join(areas.get_download_area())} for [bold]{ele.name}[/bold]\n[bold]Subscription Active:[/bold] {ele.active}"
             )
             try:
                 model_id = ele.id
-                operations.table_init_create(model_id, ele.name)
-                combined_urls, posts = asyncio.run(OF.process_areas(ele, model_id))
+                operations.table_init_create(model_id=model_id, username=ele.name)
+                combined_urls, posts = OF.process_areas(ele, model_id)
                 download.download_process(
                     ele.name, model_id, combined_urls, posts=posts
                 )
             except Exception as e:
                 if isinstance(e, KeyboardInterrupt):
                     raise e
                 log.traceback_(f"failed with exception: {e}")
@@ -186,21 +186,23 @@
                 log.info(f"Like action progressing on model {count+1}/{length}")
                 if constants.getattr("SHOW_AVATAR") and ele.avatar:
                     log.warning(f"Avatar : {ele.avatar}")
                 log.warning(
                     f"Getting {','.join(areas.get_like_area())} for [bold]{ele.name}[/bold]\n[bold]Subscription Active:[/bold] {ele.active}"
                 )
                 model_id = ele.id
-                operations.table_init_create(model_id, ele.name)
-                unfavorited_posts = like.get_post_for_like(model_id, ele.name)
+                operations.table_init_create(model_id=model_id, username=ele.name)
+                unfavorited_posts = like.get_post_for_like(
+                    model_id=model_id, username=ele.name
+                )
                 unfavorited_posts = filters.post_filter_for_like(
                     unfavorited_posts, like=True
                 )
                 post_ids = like.get_post_ids(unfavorited_posts)
-                like.like(model_id, ele.name, post_ids)
+                like.like(model_id, post_ids)
 
 
 @exit.exit_wrapper
 def process_unlike():
     with scrape_context_manager():
         profile_tools.print_current_profile()
         init.print_sign_status()
@@ -213,21 +215,21 @@
                 log.info(f"Unlike action progressing on model {count+1}/{length}")
                 if constants.getattr("SHOW_AVATAR") and ele.avatar:
                     log.warning(f"Avatar : {ele.avatar}")
                 log.warning(
                     f"Getting {','.join(areas.get_like_area())} for [bold]{ele.name}[/bold]\n[bold]Subscription Active:[/bold] {ele.active}"
                 )
                 model_id = profile.get_id(ele.name)
-                operations.table_init_create(model_id, ele.name)
+                operations.table_init_create(model_id=model_id, username=ele.name)
                 favorited_posts = like.get_posts_for_unlike(model_id, ele.name)
                 favorited_posts = filters.post_filter_for_like(
                     favorited_posts, like=False
                 )
                 post_ids = like.get_post_ids(favorited_posts)
-                like.unlike(model_id, ele.name, post_ids)
+                like.unlike(model_id, post_ids)
 
 
 def add_selected_areas():
     functs = []
     action = read_args.retriveArgs().action
     if "like" in action and "download" in action:
         actions.select_areas()
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/actions/scraper.py` & `ofscraper-3.9.1/ofscraper/actions/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import ofscraper.api.paid as paid
 import ofscraper.api.pinned as pinned
 import ofscraper.api.profile as profile
 import ofscraper.api.timeline as timeline
 import ofscraper.classes.labels as labels
 import ofscraper.classes.media as media
 import ofscraper.classes.posts as posts_
-import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.db.operations as operations
 import ofscraper.filters.media.main as filters
 import ofscraper.utils.args.areas as areas
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.context.stdout as stdout
@@ -59,15 +59,15 @@
             )
 
             log.debug(
                 f"[bold]Messages media count with locked[/bold] {sum(map(lambda x:len(x.post_media),messages_))}"
             )
             log.debug("Removing locked messages media")
             output = []
-            [output.extend(message.media) for message in messages_]
+            [output.extend(message.all_media) for message in messages_]
             log.debug(f"[bold]Messages media count[/bold] {len(output)}")
             # Update after database
             cache.set(
                 f"{model_id}_scrape_messages",
                 read_args.retriveArgs().after is not None
                 and read_args.retriveArgs().after != 0,
             )
@@ -94,15 +94,15 @@
             )
             await operations.make_post_table_changes(
                 paid_content,
                 model_id=model_id,
                 username=username,
             )
             output = []
-            [output.extend(post.media) for post in paid_content]
+            [output.extend(post.all_media) for post in paid_content]
             log.debug(f"[bold]Paid media count without locked[/bold] {len(output)}")
 
             await operations.batch_mediainsert(
                 output,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
@@ -139,15 +139,15 @@
                 username=username,
             )
 
             log.debug(
                 f"[bold]Story media count[/bold] {sum(map(lambda x:len(x.post_media), stories))}"
             )
             output = []
-            [output.extend(stories.media) for stories in stories]
+            [output.extend(stories.all_media) for stories in stories]
             await operations.batch_mediainsert(
                 output,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
             )
 
@@ -179,15 +179,15 @@
                 username=username,
             )
 
             log.debug(
                 f"[bold]highlight media count[/bold] {sum(map(lambda x:len(x.post_media), highlights_))}"
             )
             output = []
-            [output.extend(stories.media) for stories in highlights_]
+            [output.extend(stories.all_media) for stories in highlights_]
             await operations.batch_mediainsert(
                 output,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
             )
 
@@ -227,15 +227,15 @@
                 username=username,
             )
             log.debug(
                 f"[bold]Timeline media count with locked[/bold] {sum(map(lambda x:len(x.post_media),timeline_only_posts))}"
             )
             log.debug("Removing locked timeline media")
             output = []
-            [output.extend(post.media) for post in timeline_only_posts]
+            [output.extend(post.all_media) for post in timeline_only_posts]
             log.debug(f"[bold]Timeline media count without locked[/bold] {len(output)}")
 
             await operations.batch_mediainsert(
                 output,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
@@ -277,15 +277,15 @@
             )
 
             log.debug(
                 f"[bold]Archived media count with locked[/bold] {sum(map(lambda x:len(x.post_media),archived_posts))}"
             )
             log.debug("Removing locked archived media")
             output = []
-            [output.extend(post.media) for post in archived_posts]
+            [output.extend(post.all_media) for post in archived_posts]
             log.debug(f"[bold]Archived media count without locked[/bold] {len(output)}")
 
             await operations.batch_mediainsert(
                 output,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
@@ -321,15 +321,15 @@
             )
 
             log.debug(
                 f"[bold]Pinned media count with locked[/bold] {sum(map(lambda x:len(x.post_media),pinned_posts))}"
             )
             log.debug("Removing locked pinned media")
             output = []
-            [output.extend(post.media) for post in pinned_posts]
+            [output.extend(post.all_media) for post in pinned_posts]
             log.debug(f"[bold]Pinned media count without locked[/bold] {len(output)}")
 
             await operations.batch_mediainsert(
                 output,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
@@ -344,15 +344,15 @@
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
         except:
             print(E)
 
 
 @free.space_checker
-async def process_profile(username, c) -> list:
+async def process_profile(username) -> list:
     try:
         with stdout.lowstdout():
             user_profile = profile.scrape_profile(username)
             urls, info = profile.parse_profile(user_profile)
             profile.print_profile_info(info)
             output = []
             posts = []
@@ -381,28 +381,21 @@
 
 
 @free.space_checker
 @run
 async def process_all_paid():
     with stdout.lowstdout():
         paid_content = await paid.get_all_paid_posts()
-        user_dict = {}
-        for ele in paid_content:
-            user_id = ele.get("fromUser", {}).get("id") or ele.get("author", {}).get(
-                "id"
-            )
-            user_dict.setdefault(user_id, []).append(ele)
         output = {}
-        for model_id, value in user_dict.items():
+        for model_id, value in paid_content.items():
             username = profile.scrape_profile(model_id).get("username")
-            if (
-                username == "modeldeleted"
-                and await operations.check_profile_table_exists(
-                    model_id=model_id, username=username
-                )
+            if username == constants.getattr(
+                "DELETED_MODEL_PLACEHOLDER"
+            ) and await operations.check_profile_table_exists(
+                model_id=model_id, username=username
             ):
                 username = (
                     await operations.get_profile_info(
                         model_id=model_id, username=username
                     )
                     or username
                 )
@@ -417,15 +410,15 @@
             )
             seen = set()
             new_posts = [
                 post
                 for post in all_posts
                 if post.id not in seen and not seen.add(post.id)
             ]
-            new_medias = [item for post in new_posts for item in post.media]
+            new_medias = [item for post in new_posts for item in post.all_media]
             new_medias = filters.filterMedia(new_medias)
             new_posts = filters.filterPost(new_posts)
             await operations.make_post_table_changes(
                 new_posts,
                 model_id=model_id,
                 username=username,
             )
@@ -451,84 +444,93 @@
 
 @free.space_checker
 async def process_labels(model_id, username, c):
     try:
         with stdout.lowstdout():
             labelled_posts_ = await labels_api.get_labels_progress(model_id, c=c)
 
-            labelled_posts_ = list(
+            labelled_posts_labels = list(
                 map(lambda x: labels.Label(x, model_id, username), labelled_posts_)
             )
             await operations.make_label_table_changes(
-                    labelled_posts_,
-                    model_id=model_id,
-                    username=username,
+                labelled_posts_labels,
+                model_id=model_id,
+                username=username,
             )
 
             log.debug(
-                f"[bold]Label media count with locked[/bold] {sum(map(lambda x:len(x),[post.post_media for labelled_post in labelled_posts_ for post in labelled_post.posts]))}"
+                f"[bold]Label media count with locked[/bold] {sum(map(lambda x:len(x),[post.post_media for labelled_post in labelled_posts_labels for post in labelled_post.posts]))}"
             )
             log.debug("Removing locked messages media")
             output = [
-                post.media
-                for labelled_post in labelled_posts_
+                post.all_media
+                for labelled_post in labelled_posts_labels
                 for post in labelled_post.posts
             ]
             log.debug(
                 f"[bold]Label media count without locked[/bold] {sum(map(lambda x:len(x),output))}"
             )
 
             return [item for sublist in output for item in sublist], [
-                post for ele in labelled_posts_ for post in ele.posts
+                post for ele in labelled_posts_labels for post in ele.posts
             ]
     except Exception as E:
         try:
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
         except:
             print(E)
 
 
+@run
 async def process_areas(ele, model_id) -> list:
-    executor = (
-        ProcessPoolExecutor()
-        if platform.system() not in constants.getattr("API_REQUEST_THREADONLY")
-        else ThreadPoolExecutor()
-    )
-    try:
-        with executor:
-            asyncio.get_event_loop().set_default_executor(executor)
-            username = ele.name
-            output = []
-            with progress_utils.setup_api_split_progress_live():
-                medias, posts = await process_task(model_id, username, ele)
-                output.extend(medias)
-        return filters.filterMedia(output), filters.filterPost(posts)
-    except Exception as E:
-        print(E)
-        raise E
+    with stdout.lowstdout():
+        executor = (
+            ProcessPoolExecutor()
+            if platform.system() not in constants.getattr("API_REQUEST_THREADONLY")
+            else ThreadPoolExecutor()
+        )
+        try:
+            with executor:
+                asyncio.get_event_loop().set_default_executor(executor)
+                username = ele.name
+                output = []
+                with progress_utils.setup_api_split_progress_live():
+                    medias, posts = await process_task(model_id, username, ele)
+                    output.extend(medias)
+            return filters.filterMedia(output), filters.filterPost(posts)
+        except Exception as E:
+            print(E)
+            raise E
 
 
 async def process_task(model_id, username, ele):
     mediaObjs = []
     postObjs = []
     final_post_areas = set(areas.get_download_area())
     tasks = []
-    async with sessionbuilder.sessionBuilder() as c:
+    async with sessionManager.sessionManager(
+        sem=constants.getattr("API_REQ_SEM_MAX"),
+        retries=constants.getattr("API_NUM_TRIES"),
+        wait_min=constants.getattr("OF_MIN_WAIT_API"),
+        wait_max=constants.getattr("OF_MAX_WAIT_API"),
+        total_timeout=constants.getattr("API_TIMEOUT_PER_TASK"),
+        new_request_auth=True,
+    ) as c:
         while True:
             max_count = min(
                 constants.getattr("API_MAX_AREAS"),
                 system.getcpu_count(),
                 len(final_post_areas),
             )
             if not bool(tasks) and not bool(final_post_areas):
                 break
             for _ in range(max_count - len(tasks)):
                 if "Profile" in final_post_areas:
-                    tasks.append(asyncio.create_task(process_profile(username, c)))
+                    tasks.append(asyncio.create_task(process_profile(username)))
                     final_post_areas.remove("Profile")
                 elif "Pinned" in final_post_areas:
                     tasks.append(
                         asyncio.create_task(process_pinned_posts(model_id, username, c))
                     )
                     setattr(progress_utils.pinned_layout, "visible", True)
                     final_post_areas.remove("Pinned")
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/api/archive.py` & `ofscraper-3.9.1/ofscraper/api/archive.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,168 +4,147 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import asyncio
-import contextvars
 import logging
 import math
 import traceback
 
 import arrow
-from tenacity import (
-    AsyncRetrying,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random,
-)
 
+import ofscraper.api.common.logs as common_logs
 import ofscraper.db.operations as operations
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.settings as settings
-from ofscraper.classes.semaphoreDelayed import semaphoreDelayed
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
-attempt = contextvars.ContextVar("attempt")
 
 
 sem = None
 
 
 @run
 async def get_archived_posts_progress(model_id, username, forced_after=None, c=None):
 
     oldarchived = (
-        await operations.get_archived_postinfo(model_id=model_id, username=username)
+        await operations.get_archived_post_info(model_id=model_id, username=username)
         if not read_args.retriveArgs().no_cache
         else []
     )
-
-    log.trace(
-        "oldarchive {posts}".format(
-            posts="\n\n".join(list(map(lambda x: f"oldarchive: {str(x)}", oldarchived)))
-        )
-    )
+    trace_log_old(oldarchived)
 
     log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
     oldarchived = list(filter(lambda x: x != None, oldarchived))
     after = await get_after(model_id, username, forced_after)
-    splitArrays = get_split_array(oldarchived, username, after)
+    after_log(username, after)
+    splitArrays = get_split_array(oldarchived, after)
     tasks = get_tasks(splitArrays, c, model_id, after)
     data = await process_tasks(tasks, model_id, after)
     progress_utils.archived_layout.visible = False
     return data
 
 
 @run
 async def get_archived_posts(model_id, username, forced_after=None, c=None):
     oldarchived = (
-        await operations.get_archived_postinfo(model_id=model_id, username=username)
+        await operations.get_archived_post_info(model_id=model_id, username=username)
         if not read_args.retriveArgs().no_cache
         else []
     )
-    log.trace(
-        "oldarchive {posts}".format(
-            posts="\n\n".join(list(map(lambda x: f"oldarchive: {str(x)}", oldarchived)))
-        )
-    )
+    trace_log_old(oldarchived)
 
     log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
     oldarchived = list(filter(lambda x: x != None, oldarchived))
     after = await get_after(model_id, username, forced_after)
+    after_log(username, after)
     with progress_utils.set_up_api_archived():
-        splitArrays = get_split_array(oldarchived, username, after)
+        splitArrays = get_split_array(oldarchived, after)
         tasks = get_tasks(splitArrays, c, model_id, after)
         return await process_tasks(tasks, model_id, after)
 
 
 async def process_tasks(tasks, model_id, after):
     responseArray = []
     page_count = 0
     overall_progress = progress_utils.overall_progress
 
     page_task = overall_progress.add_task(
         f"Archived Content Pages Progress: {page_count}", visible=True
     )
-    while bool(tasks):
+    seen = set()
+    while tasks:
         new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task,
-                            description=f"Archived Content Pages Progress: {page_count}",
+        for task in asyncio.as_completed(tasks):
+            try:
+                result, new_tasks_batch = await task
+                new_tasks.extend(new_tasks_batch)
+                page_count = page_count + 1
+                overall_progress.update(
+                    page_task,
+                    description=f"Archived Content Pages Progress: {page_count}",
+                )
+
+                new_posts = [
+                    post
+                    for post in result
+                    if post["id"] not in seen and not seen.add(post["id"])
+                ]
+                log.debug(
+                    f"{common_logs.PROGRESS_IDS.format('Archived')} {list(map(lambda x:x['id'],new_posts))}"
+                )
+                log.trace(
+                    f"{common_logs.PROGRESS_RAW.format('Archived')}".format(
+                        posts="\n\n".join(
+                            map(
+                                lambda x: f"{common_logs.RAW_INNER} {x}",
+                                new_posts,
+                            )
                         )
-                        responseArray.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            cache.set(f"{model_id}_full_archived_scrape", True)
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
+                    )
+                )
+
+                responseArray.extend(new_posts)
+
+            except Exception as E:
+                log.traceback_(E)
+                log.traceback_(traceback.format_exc())
+                continue
+            tasks = new_tasks
 
-        tasks = new_tasks
     overall_progress.remove_task(page_task)
-    seen = set()
-    new_posts = [
-        post
-        for post in responseArray
-        if post["id"] not in seen and not seen.add(post["id"])
-    ]
 
-    log.trace(f"archive postids {list(map(lambda x:x.get('id'),new_posts))}")
-    log.trace(
-        "archived raw unduped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo archive: {str(x)}", new_posts))
-            )
-        )
+    log.debug(
+        f"{common_logs.FINAL_IDS.format('Archived')} {list(map(lambda x:x['id'],responseArray))}"
     )
-    log.debug(f"[bold]Archived Count without Dupes[/bold] {len(new_posts)} found")
-    set_check(new_posts, model_id, after)
-    return new_posts
+    trace_log_task(responseArray)
+    log.debug(f"{common_logs.FINAL_COUNT.format('Archived')} {len(responseArray)}")
 
+    set_check(responseArray, model_id, after)
+    return responseArray
 
-def get_split_array(oldarchived, username, after):
-    min_posts = 50
-    log.trace(
-        "oldarchived {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"oldarchived: {str(x)}", oldarchived))
-            )
-        )
+
+def get_split_array(oldarchived, after):
+    if len(oldarchived) == 0:
+        return []
+    min_posts = max(
+        len(oldarchived) // constants.getattr("REASONABLE_MAX_PAGE"),
+        constants.getattr("MIN_PAGE_POST_COUNT"),
     )
     log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
     oldarchived = list(filter(lambda x: x != None, oldarchived))
     postsDataArray = sorted(oldarchived, key=lambda x: x.get("created_at"))
-    log.info(
-        f"""
-Setting initial archived scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
-[yellow]Hint: append ' --after 2000' to command to force scan of all archived posts + download of new files only[/yellow]
-[yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all archived posts + download/re-download of all files[/yellow]
-
-            """
-    )
     filteredArray = list(filter(lambda x: x.get("created_at") >= after, postsDataArray))
 
-    # c= c or sessionbuilder.sessionBuilder( limit=constants.getattr("API_MAX_CONNECTION"))
     splitArrays = [
         filteredArray[i : i + min_posts]
         for i in range(0, len(filteredArray), min_posts)
     ]
     return splitArrays
 
 
@@ -247,15 +226,15 @@
             for post in cache.get(f"archived_check_{model_id}", default=[]) + unduped
             if post["id"] not in seen and not seen.add(post["id"])
         ]
 
         cache.set(
             f"archived_check_{model_id}",
             all_posts,
-            expire=constants.getattr("DAY_SECONDS"),
+            expire=constants.getattr("THREE_DAY_SECONDS"),
         )
         cache.close()
 
 
 async def get_after(model_id, username, forced_after=None):
     if forced_after != None:
         return forced_after
@@ -274,142 +253,170 @@
     curr = await operations.get_archived_media(model_id=model_id, username=username)
     if len(curr) == 0:
         log.debug("Setting date to zero because database is empty")
         return 0
     missing_items = list(filter(lambda x: x.get("downloaded") != 1, curr))
     missing_items = list(sorted(missing_items, key=lambda x: x.get("posted_at") or 0))
     if len(missing_items) == 0:
-        log.debug("Using last db date because,all downloads in db marked as downloaded")
-        return await operations.get_last_archived_date(
-            model_id=model_id, username=username
+        log.debug(
+            "Using newest db date because,all downloads in db marked as downloaded"
         )
+        return arrow.get(
+            await operations.get_youngest_archived_date(
+                model_id=model_id, username=username
+            )
+        ).float_timestamp
     else:
         log.debug(
             f"Setting date slightly before earliest missing item\nbecause {len(missing_items)} posts in db are marked as undownloaded"
         )
-        return missing_items[0].get("posted_at") or 9
+        return arrow.get(missing_items[0]["posted_at"] or 0).float_timestamp
 
 
 async def scrape_archived_posts(
     c, model_id, job_progress=None, timestamp=None, required_ids=None, offset=False
 ) -> list:
     global sem
     posts = None
-    attempt.set(0)
-    sem = semaphoreDelayed(constants.getattr("AlT_SEM"))
     if timestamp and (
         float(timestamp)
         > (read_args.retriveArgs().before or arrow.now()).float_timestamp
     ):
         return []
     timestamp = float(timestamp) - 1000 if timestamp and offset else timestamp
     url = (
         constants.getattr("archivedNextEP").format(model_id, str(timestamp))
         if timestamp
         else constants.getattr("archivedEP").format(model_id)
     )
     log.debug(url)
+    new_tasks = []
+    try:
+        task = (
+            job_progress.add_task(
+                f"Timestamp -> {arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}",
+                visible=True,
+            )
+            if job_progress
+            else None
+        )
+        async with c.requests_async(url) as r:
+            posts = (await r.json_())["list"]
+            log_id = f"timestamp:{arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp is not None  else 'initial'}"
+            if not bool(posts):
+                log.debug(f"{log_id} -> no posts found")
+                return [], []
+            log.debug(f"{log_id} -> number of archived post found {len(posts)}")
+            log.debug(
+                f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}"
+            )
+            log.debug(
+                f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}"
+            )
+            log.debug(
+                f"{log_id} -> found archived post IDs {list(map(lambda x:x.get('id'),posts))}"
+            )
+            log.trace(
+                "{log_id} -> archive raw {posts}".format(
+                    log_id=log_id,
+                    posts="\n\n".join(
+                        map(
+                            lambda x: f"scrapeinfo archive: {str(x)}",
+                            posts,
+                        )
+                    ),
+                )
+            )
 
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            new_tasks = []
-            await sem.acquire()
-            try:
-                attempt.set(attempt.get(0) + 1)
-                task = (
-                    job_progress.add_task(
-                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')}: Timestamp -> {arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}",
-                        visible=True,
+            if not required_ids:
+                new_tasks.append(
+                    asyncio.create_task(
+                        scrape_archived_posts(
+                            c,
+                            model_id,
+                            job_progress=job_progress,
+                            timestamp=posts[-1]["postedAtPrecise"],
+                            offset=False,
+                        )
                     )
-                    if job_progress
-                    else None
                 )
-                async with c.requests(url)() as r:
-                    if r.ok:
-                        posts = (await r.json_())["list"]
-                        log_id = f"timestamp:{arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}"
-                        if not posts or len(posts) == 0:
-                            log.debug(f" {log_id} -> number of post found 0")
-                        elif len(posts) > 0:
-                            log.debug(
-                                f"{log_id} -> number of archived post found {len(posts)}"
-                            )
-                            log.debug(
-                                f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}"
-                            )
-                            log.debug(
-                                f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}"
-                            )
-                            log.debug(
-                                f"{log_id} -> found archived post IDs {list(map(lambda x:x.get('id'),posts))}"
-                            )
-                            log.trace(
-                                "{log_id} -> archive raw {posts}".format(
-                                    log_id=log_id,
-                                    posts="\n\n".join(
-                                        list(
-                                            map(
-                                                lambda x: f"scrapeinfo archive: {str(x)}",
-                                                posts,
-                                            )
-                                        )
-                                    ),
-                                )
+            elif max(map(lambda x: float(x["postedAtPrecise"]), posts)) >= max(
+                required_ids
+            ):
+                pass
+            elif float(timestamp or 0) >= max(required_ids):
+                pass
+            else:
+                log.debug(f"{log_id} Required before {required_ids}")
+                [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
+                log.debug(f"{log_id} Required after {required_ids}")
+
+                if len(required_ids) > 0:
+                    new_tasks.append(
+                        asyncio.create_task(
+                            scrape_archived_posts(
+                                c,
+                                model_id,
+                                job_progress=job_progress,
+                                timestamp=posts[-1]["postedAtPrecise"],
+                                required_ids=required_ids,
+                                offset=False,
                             )
-
-                            if not required_ids:
-                                new_tasks.append(
-                                    asyncio.create_task(
-                                        scrape_archived_posts(
-                                            c,
-                                            model_id,
-                                            job_progress=job_progress,
-                                            timestamp=posts[-1]["postedAtPrecise"],
-                                            offset=False,
-                                        )
-                                    )
-                                )
-                            else:
-                                [
-                                    required_ids.discard(float(ele["postedAtPrecise"]))
-                                    for ele in posts
-                                ]
-
-                                if len(required_ids) > 0 and float(
-                                    timestamp or 0
-                                ) < max(required_ids):
-                                    new_tasks.append(
-                                        asyncio.create_task(
-                                            scrape_archived_posts(
-                                                c,
-                                                model_id,
-                                                job_progress=job_progress,
-                                                timestamp=posts[-1]["postedAtPrecise"],
-                                                required_ids=required_ids,
-                                                offset=False,
-                                            )
-                                        )
-                                    )
-                    else:
-                        log.debug(
-                            f"[bold]archived response status code:[/bold]{r.status}"
                         )
-                        log.debug(f"[bold]archived response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]archived headers:[/bold] {r.headers}")
-                        r.raise_for_status()
-            except Exception as E:
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
-
-            finally:
-                sem.release()
-                job_progress.remove_task(task) if job_progress and task else None
+                    )
             return posts, new_tasks
+    except asyncio.TimeoutError as _:
+        raise Exception(f"Task timed out {url}")
+    except Exception as E:
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
+
+    finally:
+        job_progress.remove_task(task) if job_progress and task else None
+    return posts, new_tasks
+
+
+def trace_log_task(responseArray):
+    chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
+    for i in range(1, len(responseArray) + 1, chunk_size):
+        # Calculate end index considering potential last chunk being smaller
+        end_index = min(
+            i + chunk_size - 1, len(responseArray)
+        )  # Adjust end_index calculation
+        chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
+        api_str = "\n\n".join(
+            map(lambda post: f"{common_logs.RAW_INNER} {post}\n\n", chunk)
+        )
+        log.trace(f"{common_logs.FINAL_RAW.format('Archived')}".format(posts=api_str))
+        # Check if there are more elements remaining after this chunk
+        if i + chunk_size > len(responseArray):
+            break  # Exit the loop if we've processed all elements
+
+
+def trace_log_old(responseArray):
+    chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
+    for i in range(1, len(responseArray) + 1, chunk_size):
+        # Calculate end index considering potential last chunk being smaller
+        end_index = min(
+            i + chunk_size - 1, len(responseArray)
+        )  # Adjust end_index calculation
+        chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
+        log.trace(
+            "oldarchived {posts}".format(
+                posts="\n\n".join(list(map(lambda x: f"oldarchived: {str(x)}", chunk)))
+            )
+        )
+        # Check if there are more elements remaining after this chunk
+        if i + chunk_size > len(responseArray):
+            break  # Exit the loop if we've processed all elements
+
+
+def after_log(username, after):
+    log.info(
+        f"""
+Setting initial archived scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
+[yellow]Hint: append ' --after 2000' to command to force scan of all archived posts + download of new files only[/yellow]
+[yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all archived posts + download/re-download of all files[/yellow]
+
+            """
+    )
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/api/highlights.py` & `ofscraper-3.9.1/ofscraper/api/highlights.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,44 +8,32 @@
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
 import asyncio
-import contextvars
 import logging
 import traceback
 
-from tenacity import (
-    AsyncRetrying,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random,
-)
-
-import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.api.common.logs as common_logs
+import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
-from ofscraper.classes.semaphoreDelayed import semaphoreDelayed
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
-sem = None
-attempt = contextvars.ContextVar("attempt")
 
 
 #############################################################################
 #### Stories
 ####
 ##############################################################################
 @run
 async def get_stories_post_progress(model_id, c=None):
-    global sem
-    sem = semaphoreDelayed(1)
     tasks = []
     job_progress = progress_utils.stories_progress
 
     tasks.append(
         asyncio.create_task(scrape_stories(c, model_id, job_progress=job_progress))
     )
 
@@ -53,162 +41,129 @@
 
     progress_utils.stories_layout.visible = False
     return data
 
 
 @run
 async def get_stories_post(model_id, c=None):
-    global sem
-    sem = semaphoreDelayed(1)
     tasks = []
     with progress_utils.set_up_api_stories():
         tasks.append(
             asyncio.create_task(
                 scrape_stories(
                     c, model_id, job_progress=progress_utils.stories_progress
                 )
             )
         )
         return await process_stories_tasks(tasks)
 
 
 async def scrape_stories(c, user_id, job_progress=None) -> list:
-    global sem
-    global tasks
     stories = None
-    attempt.set(0)
-
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            new_tasks = []
-            await sem.acquire()
-            await asyncio.sleep(1)
-            try:
-                attempt.set(attempt.get(0) + 1)
-                task = (
-                    job_progress.add_task(
-                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} : user id -> {user_id}",
-                        visible=True,
+    new_tasks = []
+    await asyncio.sleep(1)
+    url = constants.getattr("highlightsWithAStoryEP").format(user_id)
+    try:
+        task = (
+            job_progress.add_task(
+                f"user id -> {user_id}",
+                visible=True,
+            )
+            if job_progress
+            else None
+        )
+        async with c.requests_async(url=url) as r:
+            stories = await r.json_()
+            log.debug(
+                f"stories: -> found stories ids {list(map(lambda x:x.get('id'),stories))}"
+            )
+            log.trace(
+                "stories: -> stories raw {posts}".format(
+                    posts="\n\n".join(
+                        map(
+                            lambda x: f"scrapeinfo stories: {str(x)}",
+                            stories,
+                        )
                     )
-                    if job_progress
-                    else None
                 )
-                async with c.requests(
-                    url=constants.getattr("highlightsWithAStoryEP").format(user_id)
-                )() as r:
-                    if r.ok:
-                        stories = await r.json_()
-                        log.debug(
-                            f"stories: -> found stories ids {list(map(lambda x:x.get('id'),stories))}"
-                        )
-                        log.trace(
-                            "stories: -> stories raw {posts}".format(
-                                posts="\n\n".join(
-                                    list(
-                                        map(
-                                            lambda x: f"scrapeinfo stories: {str(x)}",
-                                            stories,
-                                        )
-                                    )
-                                )
-                            )
-                        )
-                    else:
-                        log.debug(
-                            f"[bold]stories response status code:[/bold]{r.status}"
-                        )
-                        log.debug(f"[bold]stories response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]stories headers:[/bold] {r.headers}")
-                        r.raise_for_status()
-            except Exception as E:
-                await asyncio.sleep(1)
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
+            )
+    except asyncio.TimeoutError as _:
+        raise Exception(f"Task timed out {url}")
+    except Exception as E:
+        await asyncio.sleep(1)
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
 
-            finally:
-                sem.release()
-                (
-                    job_progress.remove_task(task)
-                    if job_progress and task != None
-                    else None
-                )
+    finally:
+        (job_progress.remove_task(task) if job_progress and task is not None else None)
 
-            return stories, new_tasks
+    return stories, new_tasks
 
 
 async def process_stories_tasks(tasks):
     responseArray = []
     page_count = 0
     overall_progress = progress_utils.overall_progress
     page_task = overall_progress.add_task(
         f"Stories Pages Progress: {page_count}", visible=True
     )
 
-    while bool(tasks):
+    seen = set()
+    while tasks:
         new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task,
-                            description=f"Stories Content Pages Progress: {page_count}",
+        for task in asyncio.as_completed(tasks):
+            try:
+                result, new_tasks_batch = await task
+                new_tasks.extend(new_tasks_batch)
+                page_count = page_count + 1
+                overall_progress.update(
+                    page_task,
+                    description=f"Stories Content Pages Progress: {page_count}",
+                )
+                new_posts = [
+                    post
+                    for post in result
+                    if post["id"] not in seen and not seen.add(post["id"])
+                ]
+                log.debug(
+                    f"{common_logs.PROGRESS_IDS.format('Stories')} {list(map(lambda x:x['id'],new_posts))}"
+                )
+                log.trace(
+                    f"{common_logs.PROGRESS_RAW.format('Stories')}".format(
+                        posts="\n\n".join(
+                            map(
+                                lambda x: f"{common_logs.RAW_INNER} {x}",
+                                new_posts,
+                            )
                         )
-                        responseArray.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-        tasks = new_tasks
+                    )
+                )
 
-    overall_progress.remove_task(page_task)
+                responseArray.extend(new_posts)
+            except Exception as E:
+                log.traceback_(E)
+                log.traceback_(traceback.format_exc())
+                continue
 
-    log.trace(
-        "stories raw duped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"dupedinfo stories: {str(x)}", responseArray))
-            )
-        )
+        tasks = new_tasks
+    overall_progress.remove_task(page_task)
+    log.debug(
+        f"{common_logs.FINAL_IDS.format('Stories')} {list(map(lambda x:x['id'],responseArray))}"
     )
-    log.debug(f"[bold]stories Count with Dupes[/bold] {len(responseArray)} found")
-    seen = set()
-    new_posts = [
-        post
-        for post in responseArray
-        if post["id"] not in seen and not seen.add(post["id"])
-    ]
-
-    log.trace(f"stories postids {list(map(lambda x:x.get('id'),new_posts))}")
     log.trace(
-        "post raw unduped {posts}".format(
+        f"{common_logs.FINAL_RAW.format('Stories')}".format(
             posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo stories: {str(x)}", new_posts))
+                map(lambda x: f"{common_logs.RAW_INNER} {x}", responseArray)
             )
         )
     )
-    log.debug(f"[bold]Stories Count without Dupes[/bold] {len(new_posts)} found")
+    log.debug(f"{common_logs.FINAL_COUNT.format('Stories')} {len(responseArray)}")
 
-    return new_posts
+    return responseArray
 
 
 ##############################################################################
 #### Highlights
 ####
 ##############################################################################
 
@@ -216,17 +171,14 @@
 @run
 async def get_highlight_post_progress(model_id, c=None):
     highlightLists = await get_highlight_list_progress(model_id, c)
     return await get_highlights_via_list_progress(highlightLists, c)
 
 
 async def get_highlight_list_progress(model_id, c=None):
-    global sem
-    sem = semaphoreDelayed(1)
-
     tasks = []
     tasks.append(
         asyncio.create_task(
             scrape_highlight_list(
                 c, model_id, job_progress=progress_utils.highlights_progress
             )
         )
@@ -250,17 +202,14 @@
 @run
 async def get_highlight_post(model_id, c=None):
     highlightList = await get_highlight_list(model_id, c)
     return await get_highlights_via_list(highlightList, c)
 
 
 async def get_highlight_list(model_id, c=None):
-    global sem
-    sem = semaphoreDelayed(1)
-
     with progress_utils.set_up_api_highlights_lists():
         tasks = []
         tasks.append(
             asyncio.create_task(
                 scrape_highlight_list(
                     c, model_id, job_progress=progress_utils.highlights_progress
                 )
@@ -291,223 +240,176 @@
 
     page_count = 0
     overall_progress = progress_utils.overall_progress
 
     page_task = overall_progress.add_task(
         f"Highlights List Pages Progress: {page_count}", visible=True
     )
-    while bool(tasks):
+    seen = set()
+    while tasks:
         new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task,
-                            description=f"Highlights List Pages Progress: {page_count}",
-                        )
-                        highlightLists.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
+        for task in asyncio.as_completed(tasks):
+            try:
+                result, new_tasks_batch = await task
+                new_tasks.extend(new_tasks_batch)
+                page_count = page_count + 1
+                overall_progress.update(
+                    page_task,
+                    description=f"Highlights List Pages Progress: {page_count}",
+                )
+                new_posts = [
+                    post for post in result if post not in seen and not seen.add(post)
+                ]
+                log.debug(
+                    f"{common_logs.PROGRESS_IDS.format('Highlight List')} {list(map(lambda x:x,new_posts))}"
+                )
 
+                highlightLists.extend(new_posts)
+            except Exception as E:
+                log.traceback_(E)
+                log.traceback_(traceback.format_exc())
+                continue
         tasks = new_tasks
+
     overall_progress.remove_task(page_task)
+    log.trace(
+        f"{common_logs.FINAL_IDS.format('Highlight List')} {map(lambda x:x,highlightLists)}"
+    )
+    log.debug(
+        f"{common_logs.FINAL_COUNT.format('Highlight List')} {len(highlightLists)}"
+    )
+
     return highlightLists
 
 
 async def process_task_highlights(tasks):
     highlightResponse = []
     page_count = 0
     overall_progress = progress_utils.overall_progress
     page_task = overall_progress.add_task(
         f"Highlight Content via List Pages Progress: {page_count}", visible=True
     )
-    while bool(tasks):
+    seen = set()
+    while tasks:
         new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task,
-                            description=f"Highlight Content via List Pages Progress: {page_count}",
+        for task in asyncio.as_completed(tasks):
+            try:
+                result, new_tasks_batch = await task
+                new_tasks.extend(new_tasks_batch)
+                page_count = page_count + 1
+                overall_progress.update(
+                    page_task,
+                    description=f"Highlights Content via list Pages Progress: {page_count}",
+                )
+                new_posts = [
+                    post
+                    for post in result
+                    if post["id"] not in seen and not seen.add(post["id"])
+                ]
+                log.debug(
+                    f"{common_logs.PROGRESS_IDS.format('Highlight List Posts')} {list(map(lambda x:x['id'],new_posts))}"
+                )
+                log.trace(
+                    f"{common_logs.PROGRESS_RAW.format('Highlight List Posts')}".format(
+                        posts="\n\n".join(
+                            map(
+                                lambda x: f"{common_logs.RAW_INNER} {x}",
+                                new_posts,
+                            )
                         )
-                        highlightResponse.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
+                    )
+                )
+
+                highlightResponse.extend(new_posts)
+            except Exception as E:
+                log.traceback_(E)
+                log.traceback_(traceback.format_exc())
+                continue
         tasks = new_tasks
-    log.trace(
-        "highlight raw duped {posts}".format(
-            posts="\n\n".join(
-                list(
-                    map(lambda x: f"dupedinfo heighlight: {str(x)}", highlightResponse)
+        log.debug(
+            f"{common_logs.FINAL_IDS.format('Highlight List Posts')} {list(map(lambda x:x['id'],highlightResponse))}"
+        )
+        log.trace(
+            f"{common_logs.FINAL_RAW.format('Highlight List Posts')}".format(
+                posts="\n\n".join(
+                    map(lambda x: f"{common_logs.RAW_INNER} {x}", highlightResponse)
                 )
             )
         )
-    )
-    log.debug(f"[bold]highlight Count with Dupes[/bold] {len(highlightResponse)} found")
-    seen = set()
-    new_posts = [
-        post
-        for post in highlightResponse
-        if post["id"] not in seen and not seen.add(post["id"])
-    ]
-
-    log.trace(f"highlights postids {list(map(lambda x:x.get('id'),new_posts))}")
-    log.trace(
-        "highlights raw unduped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo highlights: {str(x)}", new_posts))
-            )
+        log.debug(
+            f"{common_logs.FINAL_COUNT.format('Highlight List Posts')} {len(highlightResponse)}"
         )
-    )
-    log.debug(f"[bold]Highlights Count without Dupes[/bold] {len(new_posts)} found")
-
-    return new_posts
+    return highlightResponse
 
 
 async def scrape_highlight_list(c, user_id, job_progress=None, offset=0) -> list:
-    global sem
-    attempt.set(0)
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            new_tasks = []
-            await sem.acquire()
-            await asyncio.sleep(1)
-            try:
-                attempt.set(attempt.get(0) + 1)
-                task = (
-                    job_progress.add_task(
-                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} scraping highlight list  offset-> {offset}",
-                        visible=True,
-                    )
-                    if job_progress
-                    else None
-                )
-                async with c.requests(
-                    url=constants.getattr("highlightsWithStoriesEP").format(
-                        user_id, offset
-                    )
-                )() as r:
-                    if r.ok:
-                        resp_data = await r.json_()
-                        log.trace(
-                            f"highlights list: -> found highlights list data {resp_data}"
-                        )
-                        data = get_highlightList(resp_data)
-                        log.debug(f"highlights list: -> found list ids {data}")
-
-                    else:
-                        log.debug(
-                            f"[bold]highlight list response status code:[/bold]{r.status}"
-                        )
-                        log.debug(
-                            f"[bold]highlight list response:[/bold] {await r.text_()}"
-                        )
-                        log.debug(f"[bold]highlight list headers:[/bold] {r.headers}")
-            except Exception as E:
-                await asyncio.sleep(1)
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
+    new_tasks = []
+    await asyncio.sleep(1)
+    url = constants.getattr("highlightsWithStoriesEP").format(user_id, offset)
+    try:
+        task = (
+            job_progress.add_task(
+                f"scraping highlight list  offset-> {offset}",
+                visible=True,
+            )
+            if job_progress
+            else None
+        )
+        async with c.requests_async(url) as r:
+            resp_data = await r.json_()
+            log.trace(f"highlights list: -> found highlights list data {resp_data}")
+            data = get_highlightList(resp_data)
+            log.debug(f"highlights list: -> found list ids {data}")
+
+    except asyncio.TimeoutError:
+        raise Exception(f"Task timed out {url}")
+    except Exception as E:
+        await asyncio.sleep(1)
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
 
-            finally:
-                sem.release()
-                (
-                    job_progress.remove_task(task)
-                    if job_progress and task != None
-                    else None
-                )
+    finally:
+        (job_progress.remove_task(task) if job_progress and task != None else None)
 
-            return data, new_tasks
+    return data, new_tasks
 
 
 async def scrape_highlights(c, id, job_progress=None) -> list:
-    global sem
-    attempt.set(0)
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            new_tasks = []
-            await sem.acquire()
-            await asyncio.sleep(1)
-            try:
-                attempt.set(attempt.get(0) + 1)
-                task = (
-                    job_progress.add_task(
-                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} highlights id -> {id}",
-                        visible=True,
-                    )
-                    if job_progress
-                    else None
-                )
-                async with c.requests(
-                    url=constants.getattr("storyEP").format(id)
-                )() as r:
-                    if r.ok:
-                        resp_data = await r.json_()
-                        log.trace(f"highlights: -> found highlights data {resp_data}")
-                        log.debug(
-                            f"highlights: -> found ids {list(map(lambda x:x.get('id'),resp_data['stories']))}"
-                        )
-                    else:
-                        log.debug(f"[bold]highlight status code:[/bold]{r.status}")
-                        log.debug(f"[bold]highlight response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]h ighlight headers:[/bold] {r.headers}")
-                        r.raise_for_status()
-            except Exception as E:
-                await asyncio.sleep(1)
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
+    new_tasks = []
+    await asyncio.sleep(1)
+    url = constants.getattr("storyEP").format(id)
+    try:
+        task = (
+            job_progress.add_task(
+                f"highlights id -> {id}",
+                visible=True,
+            )
+            if job_progress
+            else None
+        )
+        async with c.requests_async(url=url) as r:
+            resp_data = await r.json_()
+            log.trace(f"highlights: -> found highlights data {resp_data}")
+            log.debug(
+                f"highlights: -> found ids {list(map(lambda x:x.get('id'),resp_data['stories']))}"
+            )
+    except asyncio.TimeoutError:
+        raise Exception(f"Task timed out {url}")
 
-            finally:
-                sem.release()
-                (
-                    job_progress.remove_task(task)
-                    if job_progress and task != None
-                    else None
-                )
+    except Exception as E:
+        await asyncio.sleep(1)
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
+
+    finally:
+        (job_progress.remove_task(task) if job_progress and task != None else None)
 
-            return resp_data["stories"], new_tasks
+    return resp_data["stories"], new_tasks
 
 
 def get_highlightList(data):
     for ele in list(filter(lambda x: isinstance(x, list), data.values())):
         if (
             len(
                 list(
@@ -522,27 +424,20 @@
         ):
             return list(map(lambda x: x.get("id"), ele))
     return []
 
 
 def get_individual_highlights(id):
     return get_individual_stories(id)
-    # with c.requests(constants.getattr("highlightSPECIFIC").format(id))() as r:
-    #     if r.ok:
-    #         log.trace(f"highlight raw highlight individua; {r.json()}")
-    #         return r.json()
-    #     else:
-    #         log.debug(f"[bold]highlight response status code:[/bold]{r.status}")
-    #         log.debug(f"[bold]highlightresponse:[/bold] {await r.text_()}")
-    #         log.debug(f"[bold]highlight headers:[/bold] {r.headers}")
 
 
 def get_individual_stories(id, c=None):
-    with sessionbuilder.sessionBuilder(backend="httpx") as c:
-        with c.requests(constants.getattr("storiesSPECIFIC").format(id))() as r:
-            if r.ok:
-                log.trace(f"highlight raw highlight individua; {r.json_()}")
-                return r.json()
-            else:
-                log.debug(f"[bold]highlight response status code:[/bold]{r.status}")
-                log.debug(f"[bold]highlightresponse:[/bold] {r.text_()}")
-                log.debug(f"[bold]highlight headers:[/bold] {r.headers}")
+    with sessionManager.sessionManager(
+        backend="httpx",
+        retries=constants.getattr("API_INDVIDIUAL_NUM_TRIES"),
+        wait_min=constants.getattr("OF_MIN_WAIT_API"),
+        wait_max=constants.getattr("OF_MAX_WAIT_API"),
+        new_request_auth=True,
+    ) as c:
+        with c.requests_async(constants.getattr("storiesSPECIFIC").format(id)) as r:
+            log.trace(f"highlight raw highlight individua; {r.json_()}")
+            return r.json()
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/api/init.py` & `ofscraper-3.9.1/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/api/labels.py` & `ofscraper-3.9.1/ofscraper/api/labels.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,471 +1,420 @@
 r"""
-                                                      o       
+                                                            
  _______  _______         _______  _______  _______  _______  _______  _______  _______ 
 (  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
 | (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
 import asyncio
-import contextvars
 import logging
 import traceback
 
-from tenacity import (
-    AsyncRetrying,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random,
-)
-
+import ofscraper.api.common.logs as common_logs
+import ofscraper.utils.args.read as read_args
+import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
-import ofscraper.utils.sems as sems
-import ofscraper.utils.args.read as read_args
 from ofscraper.utils.context.run_async import run
-import ofscraper.utils.cache as cache
-
 
 log = logging.getLogger("shared")
-attempt = contextvars.ContextVar("attempt")
-sem = None
+
 
 @run
 async def get_labels_progress(model_id, c=None):
     labels_ = await get_labels_data_progress(model_id, c=c)
     labels_ = (
         labels_
         if not read_args.retriveArgs().label
         else list(
             filter(
-                lambda x: x.get("name").lower()
-                in read_args.retriveArgs().label,
+                lambda x: x.get("name").lower() in read_args.retriveArgs().label,
                 labels_,
             )
         )
     )
-    return await get_posts_for_labels_progress(
-                labels_, model_id, c=c
-     )
+    return await get_posts_for_labels_progress(labels_, model_id, c=c)
+
+
 @run
 async def get_labels_data_progress(model_id, c=None):
-    global sem
-    sem = sems.get_req_sem()
     tasks = []
     tasks.append(
         asyncio.create_task(
             scrape_labels(c, model_id, job_progress=progress_utils.labelled_progress)
         )
     )
     progress_utils.labelled_layout.visible = False
     return await process_tasks_labels(tasks)
+
+
 @run
 async def get_posts_for_labels_progress(labels, model_id, c=None):
-    global sem
-    sem = sems.get_req_sem()
     tasks = []
 
     [
         tasks.append(
             asyncio.create_task(
-                scrape_posts_labels(c, label, model_id, job_progress= progress_utils.labelled_progress)
+                scrape_posts_labels(
+                    c, label, model_id, job_progress=progress_utils.labelled_progress
+                )
             )
         )
         for label in labels
     ]
-    labels_final=await process_tasks_get_posts_for_labels(tasks,labels,model_id)
+    labels_final = await process_tasks_get_posts_for_labels(tasks, labels, model_id)
     progress_utils.labelled_layout.visible = False
     return labels_final
 
 
 @run
 async def get_labels(model_id, c=None):
     labels_ = await get_labels_data(model_id, c=c)
     labels_ = (
         labels_
         if not read_args.retriveArgs().label
         else list(
             filter(
-                lambda x: x.get("name").lower()
-                in read_args.retriveArgs().label,
+                lambda x: x.get("name").lower() in read_args.retriveArgs().label,
                 labels_,
             )
         )
     )
-    return await get_posts_for_labels(
-                labels_, model_id, c=c
-     )
+    return await get_posts_for_labels(labels_, model_id, c=c)
+
+
 @run
 async def get_labels_data(model_id, c=None):
-    global sem
-    sem = sems.get_req_sem()
     with progress_utils.set_up_api_labels():
         tasks = []
         tasks.append(
             asyncio.create_task(
-                scrape_labels(c, model_id, job_progress=progress_utils.labelled_progress)
+                scrape_labels(
+                    c, model_id, job_progress=progress_utils.labelled_progress
+                )
             )
         )
         return await process_tasks_labels(tasks)
 
+
 @run
 async def get_posts_for_labels(labels, model_id, c=None):
-    global sem
-    sem = sems.get_req_sem()
     with progress_utils.set_up_api_posts_labels():
         tasks = []
         [
             tasks.append(
                 asyncio.create_task(
-                    scrape_posts_labels(c, label, model_id, job_progress= progress_utils.labelled_progress)
+                    scrape_posts_labels(
+                        c,
+                        label,
+                        model_id,
+                        job_progress=progress_utils.labelled_progress,
+                    )
                 )
             )
             for label in labels
         ]
-        return await process_tasks_get_posts_for_labels(tasks,labels,model_id)
+        return await process_tasks_get_posts_for_labels(tasks, labels, model_id)
+
 
 async def process_tasks_labels(tasks):
     responseArray = []
 
     page_count = 0
     overall_progress = progress_utils.overall_progress
 
     page_task = overall_progress.add_task(
         f"Label Names Pages Progress: {page_count}", visible=True
     )
-    while bool(tasks):
+    seen = set()
+    while tasks:
         new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task,
-                            description=f"Label Names Pages Progress: {page_count}",
+        for task in asyncio.as_completed(tasks):
+            try:
+                result, new_tasks_batch = await task
+                new_tasks.extend(new_tasks_batch)
+                page_count = page_count + 1
+                overall_progress.update(
+                    page_task,
+                    description=f"Label Names Pages Progress: {page_count}",
+                )
+
+                new_posts = [
+                    post
+                    for post in result
+                    if post["id"] not in seen and not seen.add(post["id"])
+                ]
+                log.debug(
+                    f"{common_logs.PROGRESS_IDS.format('Label Names')} {list(map(lambda x:x['id'],new_posts))}"
+                )
+                log.trace(
+                    f"{common_logs.PROGRESS_RAW.format('Label Names')}".format(
+                        posts="\n\n".join(
+                            map(
+                                lambda x: f"{common_logs.RAW_INNER} {x}",
+                                new_posts,
+                            )
                         )
-                        responseArray.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-            tasks = new_tasks
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
+                    )
+                )
+                responseArray.extend(new_posts)
+            except Exception as E:
+                log.traceback_(E)
+                log.traceback_(traceback.format_exc())
+                continue
+        tasks = new_tasks
     overall_progress.remove_task(page_task)
-    log.trace(
-        "post label names unduped {posts}".format(
-            posts="\n\n".join(map(lambda x: f" label name unduped:{x}", responseArray))
-        )
-    )
     log.debug(
-        f"[bold]Labels name count without Dupes[/bold] {len(responseArray)} found"
+        f"{common_logs.FINAL_IDS.format('Labels Names')} {list(map(lambda x:x['id'],responseArray))}"
     )
+    trace_log_task(responseArray)
+    log.debug(f"{common_logs.FINAL_COUNT.format('Labels Name')} {len(responseArray)}")
+
     return responseArray
 
- 
+
 async def scrape_labels(c, model_id, job_progress=None, offset=0):
-    global sem
     labels = None
-    attempt.set(0)
-    async for _ in AsyncRetrying(
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            new_tasks = []
-            await sem.acquire()
-            await asyncio.sleep(1)
-            try:
-                attempt.set(attempt.get(0) + 1)
-
-                task = (
-                    job_progress.add_task(
-                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} labels offset -> {offset}",
-                        visible=True,
-                    )
-                    if job_progress
-                    else None
+    new_tasks = []
+    await asyncio.sleep(1)
+    url = constants.getattr("labelsEP").format(model_id, offset)
+    try:
+
+        task = (
+            job_progress.add_task(
+                f"labels offset -> {offset}",
+                visible=True,
+            )
+            if job_progress
+            else None
+        )
+        async with c.requests_async(url) as r:
+            data = await r.json_()
+            labels = list(filter(lambda x: isinstance(x, list), data.values()))[0]
+            log.debug(f"offset:{offset} -> labels names found {len(labels)}")
+            log.debug(
+                f"offset:{offset} -> hasMore value in json {data.get('hasMore','undefined') }"
+            )
+            log.trace(
+                "offset:{offset} -> label names raw: {posts}".format(
+                    offset=offset, posts=data
                 )
-                async with c.requests(
-                    url=constants.getattr("labelsEP").format(model_id, offset)
-                )() as r:
-                    if r.ok:
-                        data = await r.json_()
-                        labels = list(
-                            filter(lambda x: isinstance(x, list), data.values())
-                        )[0]
-                        log.debug(
-                            f"offset:{offset} -> labels names found {len(labels)}"
-                        )
-                        log.debug(
-                            f"offset:{offset} -> hasMore value in json {data.get('hasMore','undefined') }"
-                        )
-                        log.trace(
-                            "offset:{offset} -> label names raw: {posts}".format(
-                                offset=offset, posts=data
-                            )
-                        )
-
-                        if (
-                            data.get("hasMore")
-                            and len(data.get("list")) > 0
-                            and data.get("nextOffset") != offset
-                        ):
-                            offset = offset + len(data.get("list"))
-                            new_tasks.append(
-                                asyncio.create_task(
-                                    scrape_labels(
-                                        c,
-                                        model_id,
-                                        job_progress=job_progress,
-                                        offset=offset,
-                                    )
-                                )
-                            )
-                        return data.get("list"), new_tasks
+            )
 
-                    else:
-                        log.debug(
-                            f"[bold]labels response status code:[/bold]{r.status}"
+            if (
+                data.get("hasMore")
+                and len(data.get("list")) > 0
+                and data.get("nextOffset") != offset
+            ):
+                offset = offset + len(data.get("list"))
+                new_tasks.append(
+                    asyncio.create_task(
+                        scrape_labels(
+                            c,
+                            model_id,
+                            job_progress=job_progress,
+                            offset=offset,
                         )
-                        log.debug(f"[bold]labels response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]labels headers:[/bold] {r.headers}")
-                        r.raise_for_status()
-            except Exception as E:
-                await asyncio.sleep(1)
-
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
-
-            finally:
-                sem.release()
-                (
-                    job_progress.remove_task(task)
-                    if job_progress and task != None
-                    else None
+                    )
                 )
+            return data.get("list"), new_tasks
+    except asyncio.TimeoutError:
+        raise Exception(f"Task timed out {url}")
+    except Exception as E:
+        await asyncio.sleep(1)
+
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
 
+    finally:
+        (job_progress.remove_task(task) if job_progress and task != None else None)
 
-async def process_tasks_get_posts_for_labels(tasks,labels,model_id):
-    responseDict =get_default_label_dict(labels)
+
+async def process_tasks_get_posts_for_labels(tasks, labels, model_id):
+    responseDict = get_default_label_dict(labels)
 
     page_count = 0
     overall_progress = progress_utils.overall_progress
 
     page_task = overall_progress.add_task(
-        f" Labels Progress: {page_count}", visible=True
+        f"Labels Progress: {page_count}", visible=True
     )
 
-    while bool(tasks):
-
+    while tasks:
         new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        label, new_posts, new_tasks = await task
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task, description=f"Labels Progress: {page_count}"
-                        )
-                        log.debug(
-                            f"[bold]Label {label['name']} new post count with Dupes[/bold] {len(new_posts)} found"
-                        )
-                        new_posts = label_dedupe(new_posts)
-                        log.trace(
-                            f"{label['name']} postids {list(map(lambda x:x.get('id'),new_posts))}"
-                        )
-                        log.trace(
-                            f"{label['name']} post raw unduped {{posts}}".format(
-                                posts="\n\n".join(
-                                    list(
-                                        map(
-                                            lambda x: f"undupedinfo label: {str(x)}",
-                                            new_posts,
-                                        )
-                                    )
-                                )
+        for task in asyncio.as_completed(tasks):
+            try:
+                label, new_posts, new_tasks = await task
+                page_count = page_count + 1
+                overall_progress.update(
+                    page_task, description=f"Labels Progress: {page_count}"
+                )
+                unduped_posts = label_dedupe(
+                    responseDict[label["id"]]["seen"], new_posts
+                )
+                log.debug(
+                    f"{common_logs.PROGRESS_IDS.format('Label Content')} {list(map(lambda x:x['id'],unduped_posts))}"
+                )
+                log.trace(
+                    f"{common_logs.PROGRESS_RAW.format('Label Content')}".format(
+                        posts="\n\n".join(
+                            map(
+                                lambda x: f"{common_logs.RAW_INNER} {x}",
+                                unduped_posts,
                             )
                         )
-
-                        log.debug(
-                            f"[bold]Label {label['name']} new post count without Dupes[/bold] {len(new_posts)} found"
-                        )
-                        posts = label_dedupe(
-                            responseDict[label["id"]].get("posts", []) + new_posts
-                        )
-                        responseDict[label["id"]]["posts"] = posts
-                        tasks.extend(new_tasks)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-        tasks = new_tasks
-    labels=list(responseDict.values())
-    set_check(labels, model_id)
-    log.trace(
-        "post label joined {posts}".format(
-            posts="\n\n".join(
-                list(
-                    map(
-                        lambda x: f"label post joined: {str(x)}",
-                        list(),
                     )
                 )
-            )
+
+                responseDict[label["id"]]["posts"].extend(unduped_posts)
+            except Exception as E:
+                log.traceback_(E)
+                log.traceback_(traceback.format_exc())
+                continue
+            tasks.extend(new_tasks)
+        tasks = new_tasks
+    [label.pop("seen", None) for label in responseDict.values()]
+    set_check(responseDict.values(), model_id)
+    log.debug(
+        f"{common_logs.FINAL_IDS.format('All Labels Content')} {[item['id'] for value in responseDict.values() for item in value.get('posts', [])]}"
+    )
+    log.debug(
+        f"{common_logs.FINAL_IDS.format('Labels Individual Content')}"
+        + "\n".join(
+            [
+                f"{responseDict[key]['id']}:{list(map(lambda x:x['id'],responseDict[key]['posts']))}"
+                for key in responseDict.keys()
+            ]
+        )
+    )
+    log.debug(
+        f"{common_logs.FINAL_COUNT.format('All Labels Content')} {len([item['id'] for value in responseDict.values() for item in value.get('posts', [])])}"
+    )
+    log.debug(
+        f"{common_logs.FINAL_COUNT.format('Labels Individual Content')}"
+        + "\n".join(
+            [
+                f"{responseDict[key]['id']}:{len(responseDict[key]['posts'])}"
+                for key in responseDict.keys()
+            ]
         )
     )
-    log.debug(f"[bold]Labels count without Dupes[/bold] {len(labels)} found")
+    trace_log_task(list(responseDict.values()), header="All Labels Content")
     overall_progress.remove_task(page_task)
-    return labels
+    return list(responseDict.values())
+
 
 async def scrape_posts_labels(c, label, model_id, job_progress=None, offset=0):
-    global sem
     posts = None
-    attempt.set(0)
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            new_tasks = []
-            await sem.acquire()
-            await asyncio.sleep(1)
-            try:
-                attempt.set(attempt.get(0) + 1)
-                task = (
-                    job_progress.add_task(
-                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} : getting posts from label -> {label['name']}",
-                        visible=True,
-                    )
-                    if job_progress
-                    else None
-                )
-                async with c.requests(
-                    url=constants.getattr("labelledPostsEP").format(
-                        model_id, offset, label["id"]
-                    )
-                )() as r:
-                    if r.ok:
-                        data = await r.json_()
-                        posts = list(
-                            filter(lambda x: isinstance(x, list), data.values())
-                        )[0]
-                        log.debug(
-                            f"offset:{offset} -> labelled posts found {len(posts)}"
-                        )
-                        log.debug(
-                            f"offset:{offset} -> hasMore value in json {data.get('hasMore','undefined') }"
-                        )
-                        log.trace(
-                            "{offset} -> {posts}".format(
-                                offset=offset,
-                                posts="\n\n".join(
-                                    list(
-                                        map(
-                                            lambda x: f"scrapeinfo label {str(x)}",
-                                            posts,
-                                        )
-                                    )
-                                ),
-                            )
+    new_tasks = []
+    url = constants.getattr("labelledPostsEP").format(model_id, offset, label["id"])
+    await asyncio.sleep(1)
+    try:
+
+        task = (
+            job_progress.add_task(
+                f": getting posts from label -> {label['name']}",
+                visible=True,
+            )
+            if job_progress
+            else None
+        )
+        async with c.requests_async(url) as r:
+            data = await r.json_()
+            posts = list(filter(lambda x: isinstance(x, list), data.values()))[0]
+            log.debug(f"offset:{offset} -> labelled posts found {len(posts)}")
+            log.debug(
+                f"offset:{offset} -> hasMore value in json {data.get('hasMore','undefined') }"
+            )
+            log.trace(
+                "{offset} -> {posts}".format(
+                    offset=offset,
+                    posts="\n\n".join(
+                        map(
+                            lambda x: f"scrapeinfo label {str(x)}",
+                            posts,
                         )
+                    ),
+                )
+            )
 
-                        if data.get("hasMore") and len(posts) > 0:
-                            offset += len(posts)
-                            new_tasks.append(
-                                asyncio.create_task(
-                                    scrape_posts_labels(
-                                        c,
-                                        label,
-                                        model_id,
-                                        job_progress=job_progress,
-                                        offset=offset,
-                                    )
-                                )
-                            )
-
-                    else:
-                        log.debug(
-                            f"[bold]labelled posts response status code:[/bold]{r.status}"
-                        )
-                        log.debug(
-                            f"[bold]labelled posts response:[/bold] {await r.text_()}"
+            if data.get("hasMore") and len(posts) > 0:
+                offset += len(posts)
+                new_tasks.append(
+                    asyncio.create_task(
+                        scrape_posts_labels(
+                            c,
+                            label,
+                            model_id,
+                            job_progress=job_progress,
+                            offset=offset,
                         )
-                        log.debug(f"[bold]labelled posts headers:[/bold] {r.headers}")
+                    )
+                )
 
-                        r.raise_for_status()
-            except Exception as E:
-                await asyncio.sleep(1)
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
+    except asyncio.TimeoutError:
+        raise Exception(f"Task timed out {url}")
+    except Exception as E:
+        await asyncio.sleep(1)
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
 
-            finally:
-                sem.release()
-                (
-                    job_progress.remove_task(task)
-                    if job_progress and task != None
-                    else None
-                )
+    finally:
+        (job_progress.remove_task(task) if job_progress and task != None else None)
 
-            return label, posts, new_tasks
+    return label, posts, new_tasks
 
 
-def label_dedupe(labelArray):
-    seen = set()
+def label_dedupe(seen, labelArray):
     new_posts = [
         post
         for post in labelArray
         if post["id"] not in seen and not seen.add(post["id"])
     ]
     return new_posts
 
 
 def get_default_label_dict(labels):
     output = {}
     for label in labels:
         output[label["id"]] = label
+        output[label["id"]]["seen"] = set()
+        output[label["id"]]["posts"] = []
     return output
 
+
 def set_check(unduped, model_id):
-    seen = set()
-    new_posts = [post for label in unduped for post in label["posts"]]
-    all_posts = [
-        post
-        for post in cache.get(f"labels_check_{model_id}", default=[]) + new_posts
-        if post["id"] not in seen and not seen.add(post["id"])
-    ]
     cache.set(
         f"labels_check_{model_id}",
-        all_posts,
-        expire=constants.getattr("DAY_SECONDS"),
+        list(unduped),
+        expire=constants.getattr("THREE_DAY_SECONDS"),
     )
     cache.close()
+
+
+def trace_log_task(responseArray, header=None):
+    chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
+    for i in range(1, len(responseArray) + 1, chunk_size):
+        # Calculate end index considering potential last chunk being smaller
+        end_index = min(
+            i + chunk_size - 1, len(responseArray)
+        )  # Adjust end_index calculation
+        chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
+        api_str = "\n\n".join(
+            map(lambda post: f"{common_logs.RAW_INNER} {post}\n\n", chunk)
+        )
+        log.trace(
+            f"{common_logs.FINAL_RAW.format(header or 'Labels Names')}".format(
+                posts=api_str
+            )
+        )
+        # Check if there are more elements remaining after this chunk
+        if i + chunk_size > len(responseArray):
+            break  # Exit the loop if we've processed all elements
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/api/me.py` & `ofscraper-3.9.1/ofscraper/api/profile.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,110 +7,180 @@
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
+import asyncio
 import logging
 import traceback
+from typing import Union
 
-from tenacity import (
-    Retrying,
-    retry,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random,
-)
+from rich.console import Console
+from xxhash import xxh128
 
-import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.classes.sessionmanager as sessionManager
+import ofscraper.utils.args.read as read_args
+import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
-import ofscraper.utils.logs.helpers as log_helpers
 
+from ..utils import encoding
+
+console = Console()
 log = logging.getLogger("shared")
 
 
-def scrape_user():
-    with sessionbuilder.sessionBuilder(
-        backend="httpx", limit=constants.getattr("API_MAX_CONNECTION")
+# can get profile from username or id
+def scrape_profile(username: Union[int, str]) -> dict:
+    with sessionManager.sessionManager(
+        backend="httpx",
+        limit=constants.getattr("API_MAX_CONNECTION"),
+        retries=constants.getattr("API_INDVIDIUAL_NUM_TRIES"),
+        wait_min=constants.getattr("OF_MIN_WAIT_API"),
+        wait_max=constants.getattr("OF_MAX_WAIT_API"),
+        new_request_auth=True,
     ) as c:
-        return _scraper_user_helper(c)
+        return scrape_profile_helper(c, username)
 
 
-def _scraper_user_helper(c):
-    data = None
-    for _ in Retrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("LOGIN_NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_AUTH_MIN"),
-            max=constants.getattr("OF_AUTH_MAX"),
-        ),
-        reraise=True,
-        after=lambda retry_state: print(
-            f"Trying to login attempt:{retry_state.attempt_number}/{constants.getattr('NUM_TRIES')}"
-        ),
-    ):
-        with _:
-            try:
-                with c.requests(constants.getattr("meEP"))() as r:
-                    if r.ok:
-                        data = r.json_()
-                        log_helpers.updateSenstiveDict(data["id"], "userid")
-                        log_helpers.updateSenstiveDict(
-                            f"{data['username']} | {data['username']}|\\b{data['username']}\\b",
-                            "username",
-                        )
-                        log_helpers.updateSenstiveDict(
-                            f"{data['name']} | {data['name']}|\\b{data['name']}\\b",
-                            "name",
-                        )
-                    else:
-                        log.debug(
-                            f"[bold]user request response status code:[/bold]{r.status}"
-                        )
-                        log.debug(f"[bold]user request response:[/bold] {r.text_()}")
-                        log.debug(f"[bold]user request headers:[/bold] {r.headers}")
-                        r.raise_for_status()
-            except Exception as E:
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
-            return data
-
-
-def parse_subscriber_count():
-    with sessionbuilder.sessionBuilder(
-        backend="httpx", limit=constants.getattr("API_MAX_CONNECTION")
-    ) as c:
-        for _ in Retrying(
-            retry=retry_if_not_exception_type(KeyboardInterrupt),
-            stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-            wait=wait_random(
-                min=constants.getattr("OF_MIN"),
-                max=constants.getattr("OF_MAX"),
-            ),
-            reraise=True,
-        ):
-            with _:
-                try:
-                    with c.requests(constants.getattr("subscribeCountEP"))() as r:
-                        if r.ok:
-                            data = r.json_()
-                            return (
-                                data["subscriptions"]["active"],
-                                data["subscriptions"]["expired"],
-                            )
-                        else:
-                            log.debug(
-                                f"[bold]subscriber count response status code:[/bold]{r.status}"
-                            )
-                            log.debug(
-                                f"[bold]subscriber countresponse:[/bold] {r.text_()}"
-                            )
-                            log.debug(
-                                f"[bold]subscriber count headers:[/bold] {r.headers}"
-                            )
-                except Exception as E:
-                    log.traceback_(E)
-                    log.traceback_(traceback.format_exc())
-                    raise E
+def scrape_profile_helper(c, username: Union[int, str]):
+    data = cache.get(f"username_{username}", default=None)
+    log.trace(f"username date: {data}")
+    if data and not read_args.retriveArgs().update_profile:
+        return data
+    try:
+        with c.requests(constants.getattr("profileEP").format(username)) as r:
+            if r.status == 404:
+                return {"username": constants.getattr("DELETED_MODEL_PLACEHOLDER")}
+
+            cache.set(
+                f"username_{username}",
+                r.json(),
+                int(constants.getattr("PROFILE_DATA_EXPIRY")),
+            )
+            cache.close()
+            log.trace(f"username date: {r.json()}")
+            return r.json()
+    except Exception as E:
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
+
+
+async def scrape_profile_helper_async(c, username: Union[int, str]):
+    data = cache.get(f"username_{username}", default=None)
+    log.trace(f"username date: {data}")
+    if data and not read_args.retriveArgs().update_profile:
+        return data
+    try:
+
+        log.info(f"to get profile {username}")
+        await asyncio.sleep(1)
+        async with c.requests_async(
+            constants.getattr("profileEP").format(username)
+        ) as r:
+            if r.status == 404:
+                return {"username": constants.getattr("DELETED_MODEL_PLACEHOLDER")}
+            cache.set(
+                f"username_{username}",
+                await r.json_(),
+                int(constants.getattr("PROFILE_DATA_EXPIRY_ASYNC")),
+            )
+            cache.close()
+            log.trace(f"username date: {await r.json_()}")
+            return await r.json_()
+    except Exception as E:
+        await asyncio.sleep(1)
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
+
+
+def parse_profile(profile: dict) -> tuple:
+    media = []
+    media.append(profile.get("avatar"))
+    media.append(profile.get("header"))
+    media.append(profile.get("profile"))
+    media = list(filter(lambda x: x != None, media))
+
+    output = []
+    for ele in media:
+        output.append(
+            {
+                "url": ele,
+                "responsetype": "profile",
+                "mediatype": "photo",
+                "value": "free",
+                "createdAt": profile["joinDate"],
+                "text": profile["about"],
+                "id": xxh128(ele).hexdigest(),
+                "mediaid": xxh128(ele[:-1]).hexdigest(),
+            }
+        )
+
+    name = encoding.encode_utf_16(profile["name"])
+    username = profile["username"]
+    id_ = profile["id"]
+    join_date = profile["joinDate"]
+    posts_count = profile["postsCount"]
+    photos_count = profile["photosCount"]
+    videos_count = profile["videosCount"]
+    audios_count = profile["audiosCount"]
+    archived_posts_count = profile["archivedPostsCount"]
+    info = (
+        name,
+        username,
+        id_,
+        join_date,
+        posts_count,
+        photos_count,
+        videos_count,
+        audios_count,
+        archived_posts_count,
+    )
+
+    return output, info
+
+
+def print_profile_info(info):
+    header_fmt = "Name: {} | Username: {} | ID: {} | Joined: {}\n"
+    info_fmt = (
+        "- {} posts\n -- {} photos\n -- {} videos\n -- {} audios\n- {} archived posts"
+    )
+    final_fmt = header_fmt + info_fmt
+    log.info(final_fmt.format(*info))
+
+
+def get_id(username, c=None):
+    c = c or sessionManager.sessionManager(
+        backend="httpx",
+        retries=constants.getattr("API_INDVIDIUAL_NUM_TRIES"),
+        wait_min=constants.getattr("OF_MIN_WAIT_API"),
+        wait_max=constants.getattr("OF_MAX_WAIT_API"),
+    )
+    with c as c:
+        return get_id_helper(c, username)
+
+
+def get_id_helper(c, username):
+    if username.isnumeric():
+        return username
+    if username == constants.getattr("DELETED_MODEL_PLACEHOLDER"):
+        raise Exception("could not get ID")
+    id = cache.get(f"model_id_{username}")
+    if id:
+        return id
+    try:
+
+        log.info(f"to get id {username}")
+
+        with c.requests(constants.getattr("profileEP").format(username)) as r:
+            id = r.json()["id"]
+            cache.set(f"model_id_{username}", id, constants.getattr("DAY_SECONDS"))
+            cache.close()
+            return id
+
+    except Exception as E:
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/api/messages.py` & `ofscraper-3.9.1/ofscraper/api/messages.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,100 +13,65 @@
 
 import asyncio
 import contextvars
 import logging
 import traceback
 
 import arrow
-from tenacity import (
-    AsyncRetrying,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random,
-)
 
-import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.api.common.logs as common_logs
+import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.db.operations as operations
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
-import ofscraper.utils.sems as sems
 import ofscraper.utils.settings as settings
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
-attempt = contextvars.ContextVar("attempt")
-sem = None
 
 
 @run
 async def get_messages_progress(model_id, username, forced_after=None, c=None):
-    global sem
-    sem = sems.get_req_sem()
     global after
 
     oldmessages = (
         await operations.get_messages_post_info(model_id=model_id, username=username)
         if not read_args.retriveArgs().no_cache
         else []
     )
+    trace_log_old(oldmessages)
 
-    log.trace(
-        "oldmessage {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"oldmessages: {str(x)}", oldmessages))
-            )
-        )
-    )
     before = (read_args.retriveArgs().before or arrow.now()).float_timestamp
     after = await get_after(model_id, username, forced_after)
-
-    log.debug(f"Messages after = {after}")
-
-    log.debug(f"Messages before = {before}")
-
-    log.info(
-        f"""
-Setting initial message scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
-[yellow]Hint: append ' --after 2000' to command to force scan of all messages + download of new files only[/yellow]
-[yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all messages + download/re-download of all files[/yellow]
-
-        """
-    )
+    log_after_before(after, before, username)
 
     filteredArray = get_filterArray(after, before, oldmessages)
     splitArrays = get_split_array(filteredArray)
     tasks = get_tasks(splitArrays, filteredArray, oldmessages, model_id, c)
     data = await process_tasks(tasks, model_id)
     progress_utils.messages_layout.visible = False
     return data
 
 
 @run
 async def get_messages(model_id, username, forced_after=None, c=None):
-    global sem
-    sem = sems.get_req_sem()
     global after
 
     oldmessages = (
         await operations.get_messages_post_info(model_id=model_id, username=username)
         if not read_args.retriveArgs().no_cache
         else []
     )
-    log.trace(
-        "oldmessage {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"oldmessages: {str(x)}", oldmessages))
-            )
-        )
-    )
+    trace_log_old(oldmessages)
 
     before = (read_args.retriveArgs().before or arrow.now()).float_timestamp
     after = await get_after(model_id, username, forced_after)
+    log_after_before(after, before, username)
 
     log.debug(f"Messages after = {after}")
 
     log.debug(f"Messages before = {before}")
 
     log.info(
         f"""
@@ -116,90 +81,80 @@
 
         """
     )
 
     filteredArray = get_filterArray(after, before, oldmessages)
     splitArrays = get_split_array(filteredArray)
     with progress_utils.set_up_api_messages():
-        tasks = get_tasks(
-        splitArrays, filteredArray, oldmessages, model_id, c
-    )
+        tasks = get_tasks(splitArrays, filteredArray, oldmessages, model_id, c)
         return await process_tasks(tasks, model_id)
 
 
 async def process_tasks(tasks, model_id):
     page_count = 0
     responseArray = []
     overall_progress = progress_utils.overall_progress
     page_task = overall_progress.add_task(
-        f" Message Content Pages Progress: {page_count}", visible=True
+        f"Message Content Pages Progress: {page_count}", visible=True
     )
-
-    while bool(tasks):
+    seen = set()
+    while tasks:
         new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task,
-                            description=f"Message Content Pages Progress: {page_count}",
+        for task in asyncio.as_completed(tasks):
+            try:
+                result, new_tasks_batch = await task
+                new_tasks.extend(new_tasks_batch)
+                page_count = page_count + 1
+                overall_progress.update(
+                    page_task,
+                    description=f"Message Content Pages Progress: {page_count}",
+                )
+                new_posts = [
+                    post
+                    for post in result
+                    if post["id"] not in seen and not seen.add(post["id"])
+                ]
+                log.debug(
+                    f"{common_logs.PROGRESS_IDS.format('Messages')} {list(map(lambda x:x['id'],new_posts))}"
+                )
+                log.trace(
+                    f"{common_logs.PROGRESS_RAW.format('Messages')}".format(
+                        posts="\n\n".join(
+                            map(
+                                lambda x: f"{common_logs.RAW_INNER} {x}",
+                                new_posts,
+                            )
                         )
-                        responseArray.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            cache.set(f"{model_id}_scrape_messages")
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
+                    )
+                )
+
+                responseArray.extend(new_posts)
+            except Exception as E:
+                log.traceback_(E)
+                log.traceback_(traceback.format_exc())
+                continue
         tasks = new_tasks
-    overall_progress.remove_task(page_task)
 
-    log.debug(f"[bold]Messages Count with Dupes[/bold] {len(responseArray)} found")
-    log.trace(
-        "messages raw duped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"dupedinfo message: {str(x)}", responseArray))
-            )
-        )
+    overall_progress.remove_task(page_task)
+    log.debug(
+        f"{common_logs.FINAL_IDS.format('Messages')} {list(map(lambda x:x['id'],responseArray))}"
     )
-    seen = set()
-    new_posts = [
-        post
-        for post in responseArray
-        if post["id"] not in seen and not seen.add(post["id"])
-    ]
+    trace_log_task(responseArray)
+    log.debug(f"{common_logs.FINAL_COUNT.format('Messages')} {len(responseArray)}")
 
-    log.debug(f"[bold]Messages Count without Dupes[/bold] {len(responseArray)} found")
-
-    log.trace(f"messages messageids {list(map(lambda x:x.get('id'),new_posts))}")
-    log.trace(
-        "messages raw unduped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo message: {str(x)}", new_posts))
-            )
-        )
-    )
-    set_check(new_posts, model_id, after)
-    return new_posts
+    set_check(responseArray, model_id, after)
+    return responseArray
 
 
 def get_filterArray(after, before, oldmessages):
-    oldmessages = list(filter(lambda x: (x.get("created_at")) != None, oldmessages))
     log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
+    oldmessages = list(filter(lambda x: x["created_at"] is not None, oldmessages))
     oldmessages = sorted(
         oldmessages,
-        key=lambda x: x.get("created_at"),
+        key=lambda x: arrow.get(x["created_at"] or 0),
         reverse=True,
     )
     if after > before:
         return []
     elif len(oldmessages) <= 2:
         return oldmessages
     else:
@@ -229,28 +184,32 @@
 def get_j(oldmessages, after):
     """
     iterate through posts until a date less then or equal
     to after , set index to +1 this point
     """
     if after >= oldmessages[0].get("created_at"):
         return 0
-    if after < oldmessages[-1].get("created_at"):
-        return len(oldmessages) - 1
+    if after <= oldmessages[-1].get("created_at"):
+        return len(oldmessages)
     return min(
         next(
             index + 1
             for index, message in enumerate(oldmessages)
             if message.get("created_at") <= after
         ),
         len(oldmessages) - 1,
     )
 
 
 def get_split_array(filteredArray):
-    min_posts = 50
+    min_posts = max(
+        len(filteredArray) // constants.getattr("REASONABLE_MAX_PAGE_MESSAGES"),
+        constants.getattr("MIN_PAGE_POST_COUNT"),
+    )
+
     return [
         filteredArray[i : i + min_posts]
         for i in range(0, len(filteredArray), min_posts)
     ]
 
 
 def get_tasks(splitArrays, filteredArray, oldmessages, model_id, c):
@@ -261,30 +220,30 @@
         tasks.append(
             asyncio.create_task(
                 scrape_messages(
                     c,
                     model_id,
                     job_progress=job_progress,
                     message_id=(
-                        splitArrays[0][0].get("id")
+                        splitArrays[0][0].get("post_id")
                         if len(filteredArray) == len(oldmessages)
                         else None
                     ),
                     required_ids=set([ele.get("created_at") for ele in splitArrays[0]]),
                 )
             )
         )
         [
             tasks.append(
                 asyncio.create_task(
                     scrape_messages(
                         c,
                         model_id,
                         job_progress=job_progress,
-                        message_id=splitArrays[i - 1][-1].get("id"),
+                        message_id=splitArrays[i - 1][-1].get("post_id"),
                         required_ids=set(
                             [ele.get("created_at") for ele in splitArrays[i]]
                         ),
                     )
                 )
             )
             for i in range(1, len(splitArrays) - 1)
@@ -292,15 +251,15 @@
         # keeping grabbing until nothing left
         tasks.append(
             asyncio.create_task(
                 scrape_messages(
                     c,
                     model_id,
                     job_progress=job_progress,
-                    message_id=splitArrays[-2][-1].get("id"),
+                    message_id=splitArrays[-2][-1].get("post_id"),
                     required_ids=set(
                         [ele.get("created_at") for ele in splitArrays[-1]]
                     ),
                 )
             )
         )
     # use the first split if less then 3
@@ -309,15 +268,15 @@
             asyncio.create_task(
                 scrape_messages(
                     c,
                     model_id,
                     job_progress=job_progress,
                     required_ids=None,
                     message_id=(
-                        splitArrays[0][0].get("id")
+                        splitArrays[0][0].get("post_id")
                         if len(filteredArray) == len(oldmessages)
                         else None
                     ),
                 )
             )
         )
     # set init message to none
@@ -343,171 +302,137 @@
             post
             for post in cache.get(f"message_check_{model_id}", default=[]) + unduped
             if post["id"] not in seen and not seen.add(post["id"])
         ]
         cache.set(
             f"message_check_{model_id}",
             list(all_posts),
-            expire=constants.getattr("DAY_SECONDS"),
+            expire=constants.getattr("THREE_DAY_SECONDS"),
         )
         cache.close()
 
 
 async def scrape_messages(
     c, model_id, job_progress=None, message_id=None, required_ids=None
 ) -> list:
-    global sem
     messages = None
-    attempt.set(0)
     ep = (
         constants.getattr("messagesNextEP")
         if message_id
         else constants.getattr("messagesEP")
     )
     url = ep.format(model_id, message_id)
     log.debug(f"{message_id if message_id else 'init'} {url}")
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            new_tasks = []
-            await sem.acquire()
-            await asyncio.sleep(1)
-            try:
-                async with c.requests(url=url)() as r:
-                    attempt.set(attempt.get(0) + 1)
+    new_tasks = []
+    await asyncio.sleep(1)
+    try:
+        async with c.requests_async(url=url) as r:
+
+            task = (
+                job_progress.add_task(
+                    f": Message ID-> {message_id if message_id else 'initial'}"
+                )
+                if job_progress
+                else None
+            )
+            messages = (await r.json_())["list"]
+            log_id = f"offset messageid:{message_id if message_id else 'init id'}"
+            if not bool(messages):
+                log.debug(f"{log_id} -> no messages found")
+                return [], []
+            log.debug(f"{log_id} -> number of messages found {len(messages)}")
+            log.debug(
+                f"{log_id} -> first date {arrow.get(messages[-1].get('createdAt') or messages[0].get('postedAt')).format(constants.getattr('API_DATE_FORMAT'))}"
+            )
+            log.debug(
+                f"{log_id} -> last date {arrow.get(messages[-1].get('createdAt') or messages[0].get('postedAt')).format(constants.getattr('API_DATE_FORMAT'))}"
+            )
+            log.debug(
+                f"{log_id} -> found message ids {list(map(lambda x:x.get('id'),messages))}"
+            )
+            log.trace(
+                "{log_id} -> messages raw {posts}".format(
+                    log_id=log_id,
+                    posts="\n\n".join(
+                        map(
+                            lambda x: f"messages scrapeinfo: {str(x)}",
+                            messages,
+                        )
+                    ),
+                )
+            )
 
-                    task = (
-                        job_progress.add_task(
-                            f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')}: Message ID-> {message_id if message_id else 'initial'}"
+            if not required_ids:
+                new_tasks.append(
+                    asyncio.create_task(
+                        scrape_messages(
+                            c,
+                            model_id,
+                            job_progress=job_progress,
+                            message_id=messages[-1]["id"],
                         )
-                        if job_progress
-                        else None
                     )
-                    if r.ok:
-                        messages = (await r.json_())["list"]
-                        log_id = f"offset messageid:{message_id if message_id else 'init id'}"
-                        if not messages:
-                            messages = []
-                        if len(messages) == 0:
-                            log.debug(f"{log_id} -> number of messages found 0")
-                        elif len(messages) > 0:
-                            log.debug(
-                                f"{log_id} -> number of messages found {len(messages)}"
-                            )
-                            log.debug(
-                                f"{log_id} -> first date {arrow.get(messages[-1].get('createdAt') or messages[0].get('postedAt')).format(constants.getattr('API_DATE_FORMAT'))}"
-                            )
-                            log.debug(
-                                f"{log_id} -> last date {arrow.get(messages[-1].get('createdAt') or messages[0].get('postedAt')).format(constants.getattr('API_DATE_FORMAT'))}"
-                            )
-                            log.debug(
-                                f"{log_id} -> found message ids {list(map(lambda x:x.get('id'),messages))}"
-                            )
-                            log.trace(
-                                "{log_id} -> messages raw {posts}".format(
-                                    log_id=log_id,
-                                    posts="\n\n".join(
-                                        list(
-                                            map(
-                                                lambda x: f" messages scrapeinfo: {str(x)}",
-                                                messages,
-                                            )
-                                        )
-                                    ),
-                                )
-                            )
-                            timestamp = arrow.get(
-                                messages[-1].get("createdAt")
-                                or messages[-1].get("postedAt")
-                            ).float_timestamp
-
-                            if timestamp < after:
-                                attempt.set(0)
-                            elif required_ids == None:
-                                attempt.set(0)
-                                new_tasks.append(
-                                    asyncio.create_task(
-                                        scrape_messages(
-                                            c,
-                                            model_id,
-                                            job_progress=job_progress,
-                                            message_id=messages[-1]["id"],
-                                        )
-                                    )
-                                )
-                            else:
-                                [
-                                    required_ids.discard(
-                                        ele.get("createdAt") or ele.get("postedAt")
-                                    )
-                                    for ele in messages
-                                ]
-
-                                if len(required_ids) > 0 and timestamp > min(
-                                    list(required_ids)
-                                ):
-                                    attempt.set(0)
-                                    new_tasks.append(
-                                        asyncio.create_task(
-                                            scrape_messages(
-                                                c,
-                                                model_id,
-                                                job_progress=job_progress,
-                                                message_id=messages[-1]["id"],
-                                                required_ids=required_ids,
-                                            )
-                                        )
-                                    )
-
-                    else:
-                        log.debug(
-                            f"[bold]message response status code:[/bold]{r.status}"
-                        )
-                        log.debug(f"[bold]message response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]message headers:[/bold] {r.headers}")
+                )
 
-                        r.raise_for_status()
-            except Exception as E:
-                await asyncio.sleep(1)
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
-            finally:
-                sem.release()
-                (
-                    job_progress.remove_task(task)
-                    if job_progress and task != None
-                    else None
+            elif min(
+                map(
+                    lambda x: arrow.get(
+                        x.get("createdAt", 0) or x.get("postedAt", 0)
+                    ).float_timestamp,
+                    messages,
                 )
-            return messages, new_tasks
+            ) <= min(required_ids):
+                pass
+            else:
+                [
+                    required_ids.discard(
+                        arrow.get(
+                            ele.get("createdAt") or ele.get("postedAt")
+                        ).float_timestamp
+                    )
+                    for ele in messages
+                ]
+
+                if len(required_ids) > 0:
+                    new_tasks.append(
+                        asyncio.create_task(
+                            scrape_messages(
+                                c,
+                                model_id,
+                                job_progress=job_progress,
+                                message_id=messages[-1]["id"],
+                                required_ids=required_ids,
+                            )
+                        )
+                    )
+        return messages, new_tasks
+    except asyncio.TimeoutError:
+        raise Exception(f"Task timed out {url}")
+    except Exception as E:
+        await asyncio.sleep(1)
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
+    finally:
+        (job_progress.remove_task(task) if job_progress and task != None else None)
 
 
 def get_individual_post(model_id, postid):
-    with sessionbuilder.sessionBuilder(
+    with sessionManager.sessionManager(
         backend="httpx",
+        retries=constants.getattr("API_INDVIDIUAL_NUM_TRIES"),
+        wait_min=constants.getattr("OF_MIN_WAIT_API"),
+        wait_max=constants.getattr("OF_MAX_WAIT_API"),
+        new_request_auth=True,
     ) as c:
         with c.requests(
             url=constants.getattr("messageSPECIFIC").format(model_id, postid)
-        )() as r:
-            if r.ok:
-                log.trace(f"message raw individual {r.json()}")
-                return r.json()["list"][0]
-            else:
-                log.debug(
-                    f"[bold]Individual message response status code:[/bold]{r.status}"
-                )
-                log.debug(f"[bold]Individual message  response:[/bold] {r.text_()}")
-                log.debug(f"[bold]Individual message  headers:[/bold] {r.headers}")
+        ) as r:
+            log.trace(f"message raw individual {r.json()}")
+            return r.json()["list"][0]
 
 
 async def get_after(model_id, username, forced_after=None):
     if forced_after != None:
         return forced_after
     elif not settings.get_after_enabled():
         return 0
@@ -520,23 +445,75 @@
             "Used --after previously. Scraping all messages required to make sure content is not missing"
         )
         return 0
     curr = await operations.get_messages_media(model_id=model_id, username=username)
     if len(curr) == 0:
         log.debug("Setting date to zero because database is empty")
         return 0
-    missing_items = list(filter(lambda x: x.get("downloaded") != 1, curr))
+    missing_items = list(
+        filter(lambda x: x.get("downloaded") != 1 and x.get("unlocked") != 0, curr)
+    )
     missing_items = list(
         sorted(missing_items, key=lambda x: arrow.get(x.get("posted_at") or 0))
     )
     if len(missing_items) == 0:
         log.debug(
-            "Using last db date because,all downloads in db are marked as downloaded"
+            "Using newest db date because,all downloads in db are marked as downloaded"
         )
         return arrow.get(
-            await operations.get_last_message_date(model_id=model_id, username=username)
+            await operations.get_youngest_message_date(
+                model_id=model_id, username=username
+            )
         ).float_timestamp
     else:
         log.debug(
-            f"Setting date slightly before earliest missing item\nbecause {len(missing_items)} messages in db are marked as undownloaded"
+            f"Setting date slightly before oldest missing item\nbecause {len(missing_items)} messages in db are marked as undownloaded"
+        )
+        return arrow.get(missing_items[0]["posted_at"]).float_timestamp
+
+
+def trace_log_task(responseArray):
+    chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
+    for i in range(1, len(responseArray) + 1, chunk_size):
+        # Calculate end index considering potential last chunk being smaller
+        end_index = min(
+            i + chunk_size - 1, len(responseArray)
+        )  # Adjust end_index calculation
+        chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
+        api_str = "\n\n".join(
+            map(lambda post: f"{common_logs.RAW_INNER} {post}\n\n", chunk)
+        )
+        log.trace(f"{common_logs.FINAL_RAW.format('Messages')}".format(posts=api_str))
+        # Check if there are more elements remaining after this chunk
+        if i + chunk_size > len(responseArray):
+            break  # Exit the loop if we've processed all elements
+
+
+def trace_log_old(responseArray):
+    chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
+    for i in range(1, len(responseArray) + 1, chunk_size):
+        # Calculate end index considering potential last chunk being smaller
+        end_index = min(
+            i + chunk_size - 1, len(responseArray)
+        )  # Adjust end_index calculation
+        chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
+        log.trace(
+            "oldmessages {posts}".format(
+                posts="\n\n".join(list(map(lambda x: f"oldmessage: {str(x)}", chunk)))
+            )
         )
-        return arrow.get(missing_items[0].get("posted_at") or 0).float_timestamp
+        # Check if there are more elements remaining after this chunk
+        if i + chunk_size > len(responseArray):
+            break  # Exit the loop if we've processed all elements
+
+
+def log_after_before(after, before, username):
+    log.debug(f"Messages before = {before}")
+
+    log.info(
+        f"""
+Setting initial message scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
+[yellow]Hint: append ' --after 2000' to command to force scan of all messages + download of new files only[/yellow]
+[yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all messages + download/re-download of all files[/yellow]
+
+        """
+    )
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/api/paid.py` & `ofscraper-3.9.1/ofscraper/api/paid.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,64 +8,46 @@
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
 import asyncio
-import contextvars
 import logging
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 
-from tenacity import (
-    AsyncRetrying,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random,
-)
-
-import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.api.common.logs as common_logs
+import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
-import ofscraper.utils.sems as sems
 from ofscraper.utils.context.run_async import run
 
 paid_content_list_name = "list"
 log = logging.getLogger("shared")
-attempt = contextvars.ContextVar("attempt")
-sem = None
 
 
 @run
 async def get_paid_posts_progress(username, model_id, c=None):
-    global sem
-    sem = sems.get_req_sem()
     tasks = []
 
     job_progress = progress_utils.paid_progress
     tasks.append(
         asyncio.create_task(scrape_paid(c, username, job_progress=job_progress))
     )
     data = await process_tasks(tasks, model_id)
 
     progress_utils.paid_layout.visible = False
     return data
 
 
 @run
 async def get_paid_posts(model_id, username, c=None):
-    global sem
-    sem = sems.get_req_sem()
     tasks = []
-
-    # async with c or sessionbuilder.sessionBuilder(
-    #     limit=constants.getattr("API_MAX_CONNECTION")
-    # ) as c:
     with progress_utils.set_up_api_paid():
         job_progress = progress_utils.paid_progress
         tasks.append(
             asyncio.create_task(scrape_paid(c, username, job_progress=job_progress))
         )
         return await process_tasks(tasks, model_id)
 
@@ -73,377 +55,321 @@
 async def process_tasks(tasks, model_id):
     page_count = 0
     overall_progress = progress_utils.overall_progress
     page_task = overall_progress.add_task(
         f"Paid Content Pages Progress: {page_count}", visible=True
     )
     responseArray = []
-    while bool(tasks):
+    seen = set()
+
+    while tasks:
         new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task,
-                            description=f"Paid Content Pages Progress: {page_count}",
+        for task in asyncio.as_completed(tasks):
+            try:
+                result, new_tasks_batch = await task
+                new_tasks.extend(new_tasks_batch)
+                page_count = page_count + 1
+                overall_progress.update(
+                    page_task,
+                    description=f"Paid Content Pages Progress: {page_count}",
+                )
+                new_posts = [
+                    post
+                    for post in result
+                    if post["id"] not in seen and not seen.add(post["id"])
+                ]
+                log.debug(
+                    f"{common_logs.PROGRESS_IDS.format('Paid')} {list(map(lambda x:x['id'],new_posts))}"
+                )
+                log.trace(
+                    f"{common_logs.PROGRESS_RAW.format('Paid')}".format(
+                        posts="\n\n".join(
+                            map(
+                                lambda x: f"{common_logs.RAW_INNER} {x}",
+                                new_posts,
+                            )
                         )
-                        responseArray.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-        tasks = new_tasks
-    overall_progress.remove_task(page_task)
-    log.debug(f"[bold]Paid Count with Dupes[/bold] {len(responseArray)} found")
-
-    seen = set()
-    new_posts = [
-        post
-        for post in responseArray
-        if post["id"] not in seen and not seen.add(post["id"])
-    ]
+                    )
+                )
 
-    log.trace(f"paid postids {list(map(lambda x:x.get('id'),new_posts))}")
+                responseArray.extend(new_posts)
+            except Exception as E:
+                log.traceback_(E)
+                log.traceback_(traceback.format_exc())
+                continue
+        tasks = new_tasks
 
-    log.trace(
-        "paid raw unduped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo paid: {str(x)}", new_posts))
-            )
-        )
+    overall_progress.remove_task(page_task)
+    log.debug(
+        f"{common_logs.FINAL_IDS.format('Paid')} {list(map(lambda x:x['id'],responseArray))}"
     )
-    log.debug(f"[bold]Paid Count without Dupes[/bold] {len(new_posts)} found")
 
-    set_check(new_posts, model_id)
-    return new_posts
-
-
-def set_check(unduped, model_id):
-    seen = set()
-    all_posts = [
-        post
-        for post in cache.get(f"purchase_check_{model_id}", default=[]) + unduped
-        if post["id"] not in seen and not seen.add(post["id"])
-    ]
-    cache.set(
-        f"purchased_check_{model_id}",
-        all_posts,
-        expire=constants.getattr("DAY_SECONDS"),
-    )
-    cache.close()
+    paid_str = ""
+    for post in responseArray:
+        paid_str += f"{common_logs.RAW_INNER} {post}\n\n"
+    log.trace(f"{common_logs.FINAL_RAW.format('Paid')}".format(posts=paid_str))
+    log.debug(f"{common_logs.FINAL_COUNT.format('Paid')} {len(responseArray)}")
+    set_check(model_id, responseArray)
+    return responseArray
 
 
 @run
 async def scrape_paid(c, username, job_progress=None, offset=0):
     """Takes headers to access onlyfans as an argument and then checks the purchased content
     url to look for any purchased content. If it finds some it will return it as a list.
     """
-    global sem
     media = None
 
-    attempt.set(0)
-
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            await sem.acquire()
-            await asyncio.sleep(1)
+    await asyncio.sleep(1)
 
-            new_tasks = []
-            try:
-                attempt.set(attempt.get(0) + 1)
-                task = (
-                    (
-                        job_progress.add_task(
-                            f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} scrape paid offset -> {offset} username -> {username}",
-                            visible=True,
-                        )
-                        if job_progress
-                        else None
-                    )
-                    if job_progress
-                    else None
+    new_tasks = []
+    url = constants.getattr("purchased_contentEP").format(offset, username)
+    try:
+
+        task = (
+            (
+                job_progress.add_task(
+                    f"scrape paid offset -> {offset} username -> {username}",
+                    visible=True,
                 )
+                if job_progress
+                else None
+            )
+            if job_progress
+            else None
+        )
 
-                async with c.requests(
-                    url=constants.getattr("purchased_contentEP").format(
-                        offset, username
+        async with c.requests_async(url) as r:
+            data = await r.json_()
+            log.trace("paid raw {posts}".format(posts=data))
+
+            media = list(filter(lambda x: isinstance(x, list), data.values()))[0]
+            log.debug(f"offset:{offset} -> media found {len(media)}")
+            log.debug(
+                f"offset:{offset} -> hasmore value in json {data.get('hasMore','undefined') }"
+            )
+            log.debug(
+                f"offset:{offset} -> found paid content ids {list(map(lambda x:x.get('id'),media))}"
+            )
+            if data.get("hasMore") and len(media) > 0:
+                offset += len(media)
+                new_tasks.append(
+                    asyncio.create_task(
+                        scrape_paid(c, username, job_progress, offset=offset)
                     )
-                )() as r:
-                    if r.ok:
-                        data = await r.json_()
-                        log.trace("paid raw {posts}".format(posts=data))
-
-                        media = list(
-                            filter(lambda x: isinstance(x, list), data.values())
-                        )[0]
-                        log.debug(f"offset:{offset} -> media found {len(media)}")
-                        log.debug(
-                            f"offset:{offset} -> hasmore value in json {data.get('hasMore','undefined') }"
-                        )
-                        log.debug(
-                            f"offset:{offset} -> found paid content ids {list(map(lambda x:x.get('id'),media))}"
-                        )
-                        if data.get("hasMore") and len(media) > 0:
-                            offset += len(media)
-                            new_tasks.append(
-                                asyncio.create_task(
-                                    scrape_paid(
-                                        c, username, job_progress, offset=offset
-                                    )
-                                )
-                            )
-                        (
-                            job_progress.remove_task(task)
-                            if task and job_progress
-                            else None
-                        )
-
-                    else:
-                        log.debug(f"[bold]paid response status code:[/bold]{r.status}")
-                        log.debug(f"[bold]paid response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]paid headers:[/bold] {r.headers}")
-                        job_progress.remove_task(task)
-                        r.raise_for_status()
-            except Exception as E:
-                await asyncio.sleep(1)
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
+                )
+            (job_progress.remove_task(task) if task and job_progress else None)
+    except asyncio.TimeoutError:
+        raise Exception(f"Task timed out {url}")
+    except Exception as E:
+        await asyncio.sleep(1)
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
 
-            finally:
-                sem.release()
-                job_progress.remove_task(task) if task and job_progress else None
+    finally:
+        job_progress.remove_task(task) if task and job_progress else None
 
-        return media, new_tasks
+    return media, new_tasks
 
 
 @run
 async def get_all_paid_posts():
-    global sem
-    sem = sems.get_req_sem()
+    data = await process_and_create_tasks()
+    return create_all_paid_dict(data)
+
+
+async def process_and_create_tasks():
     with ThreadPoolExecutor(
-        max_workers=constants.getattr("MAX_REQUEST_WORKERS")
+        max_workers=constants.getattr("MAX_THREAD_WORKERS")
     ) as executor:
         asyncio.get_event_loop().set_default_executor(executor)
 
         output = []
-        min_posts = 100
+        min_posts = 80
         tasks = []
         page_count = 0
         with progress_utils.setup_all_paid_live():
             job_progress = progress_utils.all_paid_progress
             overall_progress = progress_utils.overall_progress
-
-            async with sessionbuilder.sessionBuilder() as c:
+            async with sessionManager.sessionManager(
+                sem=constants.getattr("SCRAPE_PAID_SEMS"),
+                retries=constants.getattr("API_PAID_NUM_TRIES"),
+                wait_min=constants.getattr("OF_MIN_WAIT_API"),
+                wait_max=constants.getattr("OF_MAX_WAIT_API"),
+                new_request_auth=True,
+            ) as c:
                 allpaid = cache.get("purchased_all", default=[])
                 log.debug(f"[bold]All Paid Cache[/bold] {len(allpaid)} found")
 
                 if len(allpaid) > min_posts:
                     splitArrays = [i for i in range(0, len(allpaid), min_posts)]
-                    # use the previous split for timesamp
-                    tasks.append(
-                        asyncio.create_task(
-                            scrape_all_paid(
-                                c, job_progress, offset=0, count=0, required=0
-                            )
-                        )
-                    )
                     [
                         tasks.append(
                             asyncio.create_task(
                                 scrape_all_paid(
                                     c,
                                     job_progress,
-                                    count=0,
-                                    required=0,
+                                    required=min_posts,
                                     offset=splitArrays[i],
                                 )
                             )
                         )
-                        for i in range(1, len(splitArrays))
+                        for i in range(0, len(splitArrays) - 1)
                     ]
-                    # keeping grabbing until nothign left
                     tasks.append(
                         asyncio.create_task(
-                            scrape_all_paid(c, job_progress, offset=len(allpaid))
+                            scrape_all_paid(
+                                c, job_progress, offset=splitArrays[-1], required=None
+                            )
                         )
                     )
                 else:
                     tasks.append(asyncio.create_task(scrape_all_paid(c, job_progress)))
 
                 page_task = overall_progress.add_task(
-                    f" Pages Progress: {page_count}", visible=True
+                    f"Pages Progress: {page_count}", visible=True
                 )
                 while tasks:
-                    done, pending = await asyncio.wait(
-                        tasks, return_when=asyncio.FIRST_COMPLETED
-                    )
-                    tasks = list(pending)
-                    await asyncio.sleep(1)
-                    for result in done:
+                    new_tasks = []
+                    for task in asyncio.as_completed(tasks):
                         try:
-                            result, new_tasks = await result
+                            result, new_tasks_batch = await task
                             page_count = page_count + 1
                             overall_progress.update(
                                 page_task, description=f"Pages Progress: {page_count}"
                             )
                             output.extend(result)
-                            tasks.extend(new_tasks)
+                            log.debug(
+                                f"{common_logs.PROGRESS_IDS.format('ALL Paid')} {list(map(lambda x:x['id'],result))}"
+                            )
+                            paid_str = ""
+                            for post in output:
+                                paid_str += f"{common_logs.RAW_INNER} {post}\n\n"
+
+                            log.trace(
+                                f"{common_logs.PROGRESS_RAW.format('All Paid')}".format(
+                                    posts=paid_str
+                                )
+                            )
+                            new_tasks.extend(new_tasks_batch)
                             await asyncio.sleep(1)
                         except Exception as E:
                             await asyncio.sleep(1)
-                            log.debug(E)
+                            log.traceback_(E)
+                            log.traceback_(traceback.format_exc())
                             continue
-
+                    tasks = new_tasks
                 overall_progress.remove_task(page_task)
 
         log.debug(f"[bold]Paid Post count with Dupes[/bold] {len(output)} found")
         log.trace(
             "paid raw duped {posts}".format(
                 posts="\n\n".join(
-                    list(map(lambda x: f"dupedinfo all paid: {str(x)}", output))
-                )
-            )
-        )
-        seen = set()
-        new_posts = [
-            post
-            for post in output
-            if post["id"] not in seen and not seen.add(post["id"])
-        ]
-        log.trace(f"all paid postids {list(map(lambda x:x.get('id'),new_posts))}")
-        log.debug(f"[bold]Paid Post count without Dupes[/bold] {len(new_posts)} found")
-        log.trace(
-            "paid raw duped {posts}".format(
-                posts="\n\n".join(
-                    list(map(lambda x: f"undupedinfo all paid: {str(x)}", new_posts))
+                    map(lambda x: f"dupedinfo all paid: {str(x)}", output)
                 )
             )
         )
         cache.set(
             "purchased_all",
-            list(map(lambda x: x.get("id"), list())),
+            list(map(lambda x: x.get("id"), list(output))),
             expire=constants.getattr("RESPONSE_EXPIRY"),
         )
         cache.close()
         # filter at user level
         return output
 
 
-async def scrape_all_paid(c, job_progress=None, offset=0, count=0, required=0):
+def create_all_paid_dict(paid_content):
+    user_dict = {}
+    for ele in paid_content:
+        user_id = ele.get("fromUser", {}).get("id") or ele.get("author", {}).get("id")
+        user_dict.setdefault(str(user_id), []).append(ele)
+    [set_check(key, val) for key, val in user_dict.items()]
+    return user_dict
+
+
+async def scrape_all_paid(c, job_progress=None, offset=0, required=None):
     """Takes headers to access onlyfans as an argument and then checks the purchased content
     url to look for any purchased content. If it finds some it will return it as a list.
     """
-    global sem
     media = None
 
-    attempt.set(0)
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            await sem.acquire()
-            await asyncio.sleep(1)
-            new_tasks = []
-            try:
-                attempt.set(attempt.get(0) + 1)
-                task = job_progress.add_task(
-                    f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} scrape entire paid page offset={offset}",
-                    visible=True,
-                )
+    await asyncio.sleep(1)
+    new_tasks = []
+    url = constants.getattr("purchased_contentALL").format(offset)
+    try:
+
+        task = job_progress.add_task(
+            f"scrape entire paid page offset={offset}",
+            visible=True,
+        )
 
-                async with c.requests(
-                    url=constants.getattr("purchased_contentALL").format(offset)
-                )() as r:
-                    if r.ok:
-                        log_id = f"offset {offset or 0}:"
-                        data = await r.json_()
-                        media = list(
-                            filter(lambda x: isinstance(x, list), data.values())
-                        )[0]
-                        if not data.get("hasMore"):
-                            media = []
-                        if not media:
-                            media = []
-                        if len(media) == 0:
-                            log.debug(f"{log_id} -> number of post found 0")
-                        elif len(media) > 0:
-                            log.debug(f"{log_id} -> number of post found {len(media)}")
-                            log.debug(
-                                f"{log_id} -> first date {media[0].get('createdAt') or media[0].get('postedAt')}"
-                            )
-                            log.debug(
-                                f"{log_id} -> last date {media[-1].get('createdAt') or media[-1].get('postedAt')}"
-                            )
-                            log.debug(
-                                f"{log_id} -> found paid content ids {list(map(lambda x:x.get('id'),media))}"
-                            )
+        async with c.requests_async(url) as r:
+            log_id = f"offset {offset or 0}:"
+            data = await r.json_()
+            media = list(filter(lambda x: isinstance(x, list), data.values()))[0]
+            if not data.get("hasMore") or not bool(media):
+                log.debug(f"{log_id} -> no paid posts found")
+                return media, new_tasks
+            log.debug(f"{log_id} -> number of post found {len(media)}")
+            log.debug(
+                f"{log_id} -> first date {media[0].get('createdAt') or media[0].get('postedAt')}"
+            )
+            log.debug(
+                f"{log_id} -> last date {media[-1].get('createdAt') or media[-1].get('postedAt')}"
+            )
+            log.debug(
+                f"{log_id} -> found paid content ids {list(map(lambda x:x.get('id'),media))}"
+            )
 
-                            if required == 0:
-                                new_tasks.append(
-                                    asyncio.create_task(
-                                        scrape_all_paid(
-                                            c, job_progress, offset=offset + len(media)
-                                        )
-                                    )
-                                )
+            if required is None:
+                new_tasks.append(
+                    asyncio.create_task(
+                        scrape_all_paid(c, job_progress, offset=offset + len(media))
+                    )
+                )
+            elif len(media) < required:
+                new_tasks.append(
+                    asyncio.create_task(
+                        scrape_all_paid(
+                            c,
+                            job_progress,
+                            offset=offset + len(media),
+                            required=required - len(media),
+                        )
+                    )
+                )
+            return media, new_tasks
 
-                            elif len(count) < len(required):
-                                new_tasks.append(
-                                    asyncio.create_task(
-                                        scrape_all_paid(
-                                            c,
-                                            job_progress,
-                                            offset=offset + len(media),
-                                            required=required,
-                                            count=count + len(media),
-                                        )
-                                    )
-                                )
+    except asyncio.TimeoutError:
+        raise Exception(f"Task timed out {url}")
+    except Exception as E:
+        await asyncio.sleep(1)
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
 
-                    else:
-                        log.debug(f"[bold]paid response status code:[/bold]{r.status}")
-                        log.debug(f"[bold]paid response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]paid headers:[/bold] {r.headers}")
-                        job_progress.remove_task(task)
-                        r.raise_for_status()
-            except Exception as E:
-                await asyncio.sleep(1)
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
+    finally:
+        job_progress.remove_task(task)
 
-            finally:
-                sem.release()
-                job_progress.remove_task(task)
 
-            return media, new_tasks
+def set_check(model_id, unduped):
+    seen = set()
+    all_posts = [
+        post
+        for post in cache.get(f"purchase_check_{model_id}", default=[]) + unduped
+        if post["id"] not in seen and not seen.add(post["id"])
+    ]
+    cache.set(
+        f"purchased_check_{model_id}",
+        all_posts,
+        expire=constants.getattr("THREE_DAY_SECONDS"),
+    )
+    cache.close()
 
 
 def get_individual_post(username, model_id, postid):
     data = get_paid_posts_progress(username, model_id)
     postid = int(postid)
     posts = list(filter(lambda x: int(x["id"]) == postid, data))
     if len(posts) > 0:
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/api/pinned.py` & `ofscraper-3.9.1/ofscraper/api/pinned.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,47 +4,34 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import asyncio
-import contextvars
 import logging
 import math
 import traceback
 
 import arrow
-from tenacity import (
-    AsyncRetrying,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random,
-)
 
+import ofscraper.api.common.logs as common_logs
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
-from ofscraper.classes.semaphoreDelayed import semaphoreDelayed
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
-attempt = contextvars.ContextVar("attempt")
-sem = None
 
 
 @run
 async def get_pinned_posts_progress(model_id, c=None):
     tasks = []
     job_progress = progress_utils.pinned_progress
-
-    # async with sessionbuilder.sessionBuilder(
-    #     limit=constants.getattr("API_MAX_CONNECTION")
-    # ) as c:
     tasks.append(
         asyncio.create_task(
             scrape_pinned_posts(
                 c,
                 model_id,
                 job_progress=job_progress,
                 timestamp=(
@@ -86,185 +73,167 @@
     responseArray = []
     page_count = 0
     overall_progress = progress_utils.overall_progress
 
     page_task = overall_progress.add_task(
         f"Pinned Content Pages Progress: {page_count}", visible=True
     )
-    while bool(tasks):
+    seen = set()
+
+    while tasks:
         new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task,
-                            description=f"Pinned Content Pages Progress: {page_count}",
+        for task in asyncio.as_completed(tasks):
+            try:
+                result, new_tasks_batch = await task
+                new_tasks.extend(new_tasks_batch)
+                page_count = page_count + 1
+                overall_progress.update(
+                    page_task,
+                    description=f"Pinned Content Pages Progress: {page_count}",
+                )
+                new_posts = [
+                    post
+                    for post in result
+                    if post["id"] not in seen and not seen.add(post["id"])
+                ]
+                log.debug(
+                    f"{common_logs.PROGRESS_IDS.format('Pinned')} {list(map(lambda x:x['id'],new_posts))}"
+                )
+                log.trace(
+                    f"{common_logs.PROGRESS_RAW.format('Pinned')}".format(
+                        posts="\n\n".join(
+                            map(
+                                lambda x: f"{common_logs.RAW_INNER} {x}",
+                                new_posts,
+                            )
                         )
-                        responseArray.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
+                    )
+                )
+
+                responseArray.extend(new_posts)
+            except Exception as E:
+                log.traceback_(E)
+                log.traceback_(traceback.format_exc())
+                continue
         tasks = new_tasks
     overall_progress.remove_task(page_task)
     log.debug(f"[bold]Pinned Count with Dupes[/bold] {len(responseArray)} found")
     log.trace(
         "pinned raw duped {posts}".format(
             posts="\n\n".join(
-                list(map(lambda x: f"dupedinfo pinned: {str(x)}", responseArray))
+                map(lambda x: f"dupedinfo pinned: {str(x)}", responseArray)
             )
         )
     )
-    seen = set()
-    new_posts = [
-        post
-        for post in responseArray
-        if post["id"] not in seen and not seen.add(post["id"])
-    ]
-
-    log.trace(f"pinned postids{list(map(lambda x:x.get('id'),new_posts))}")
-    log.trace(
-        "pinned raw unduped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo pinned: {str(x)}", new_posts))
-            )
-        )
+    log.debug(
+        f"{common_logs.FINAL_IDS.format('Pinned')} {list(map(lambda x:x['id'],responseArray))}"
     )
-    log.debug(f"[bold]Pinned Count without Dupes[/bold] {len(new_posts)} found")
-    set_check(new_posts, model_id)
-    return new_posts
+
+    pinned_str = ""
+    for post in responseArray:
+        pinned_str += f"{common_logs.RAW_INNER} {post}\n\n"
+    log.trace(f"{common_logs.FINAL_RAW.format('Pinned')}".format(posts=pinned_str))
+    log.debug(f"{common_logs.FINAL_COUNT.format('Pinned')} {len(responseArray)}")
+
+    set_check(responseArray, model_id)
+    return responseArray
 
 
 def set_check(unduped, model_id):
     if not read_args.retriveArgs().after:
         seen = set()
         all_posts = [
             post
             for post in cache.get(f"pinned_check_{model_id}", default=[]) + unduped
             if post["id"] not in seen and not seen.add(post["id"])
         ]
         cache.set(
             f"pinned_check_{model_id}",
             all_posts,
-            expire=constants.getattr("DAY_SECONDS"),
+            expire=constants.getattr("THREE_DAY_SECONDS"),
         )
         cache.close()
 
 
 async def scrape_pinned_posts(
     c, model_id, job_progress=None, timestamp=None, count=0
 ) -> list:
-    global sem
-    sem = semaphoreDelayed(constants.getattr("AlT_SEM"))
     posts = None
-    attempt.set(0)
 
     if timestamp and (
         float(timestamp)
         > (read_args.retriveArgs().before or arrow.now()).float_timestamp
     ):
         return []
     url = constants.getattr("timelinePinnedEP").format(model_id, count)
     log.debug(url)
-
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            new_tasks = []
-            await sem.acquire()
-            await asyncio.sleep(1)
-            try:
-                attempt.set(attempt.get(0) + 1)
-                task = (
-                    job_progress.add_task(
-                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')}: Timestamp -> {arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}",
-                        visible=True,
-                    )
-                    if job_progress
-                    else None
+    new_tasks = []
+    await asyncio.sleep(1)
+    try:
+
+        task = (
+            job_progress.add_task(
+                f"Timestamp -> {arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}",
+                visible=True,
+            )
+            if job_progress
+            else None
+        )
+        async with c.requests_async(url=url) as r:
+            posts = (await r.json_())["list"]
+            posts = list(sorted(posts, key=lambda x: float(x["postedAtPrecise"])))
+            posts = list(
+                filter(
+                    lambda x: float(x["postedAtPrecise"]) > float(timestamp or 0),
+                    posts,
                 )
-                async with c.requests(url=url)() as r:
-                    if r.ok:
-                        posts = (await r.json_())["list"]
-                        posts = list(
-                            sorted(posts, key=lambda x: float(x["postedAtPrecise"]))
-                        )
-                        posts = list(
-                            filter(
-                                lambda x: float(x["postedAtPrecise"])
-                                > float(timestamp or 0),
+            )
+            log_id = f"timestamp:{arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}"
+            if not posts:
+                posts = []
+            if len(posts) == 0:
+                log.debug(f"{log_id} -> number of pinned post found 0")
+            else:
+                log.debug(f"{log_id} -> number of pinned post found {len(posts)}")
+                log.debug(
+                    f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}"
+                )
+                log.debug(
+                    f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}"
+                )
+                log.debug(
+                    f"{log_id} -> found pinned post IDs {list(map(lambda x:x.get('id'),posts))}"
+                )
+                log.trace(
+                    "{log_id} -> pinned raw {posts}".format(
+                        log_id=log_id,
+                        posts="\n\n".join(
+                            map(
+                                lambda x: f"scrapeinfo pinned: {str(x)}",
                                 posts,
                             )
+                        ),
+                    )
+                )
+                new_tasks.append(
+                    asyncio.create_task(
+                        scrape_pinned_posts(
+                            c,
+                            model_id,
+                            job_progress=job_progress,
+                            timestamp=posts[-1]["postedAtPrecise"],
+                            count=count + len(posts),
                         )
-                        log_id = f"timestamp:{arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}"
-                        if not posts:
-                            posts = []
-                        if len(posts) == 0:
-                            log.debug(f"{log_id} -> number of pinned post found 0")
-                        else:
-                            log.debug(
-                                f"{log_id} -> number of pinned post found {len(posts)}"
-                            )
-                            log.debug(
-                                f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}"
-                            )
-                            log.debug(
-                                f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}"
-                            )
-                            log.debug(
-                                f"{log_id} -> found pinned post IDs {list(map(lambda x:x.get('id'),posts))}"
-                            )
-                            log.trace(
-                                "{log_id} -> pinned raw {posts}".format(
-                                    log_id=log_id,
-                                    posts="\n\n".join(
-                                        list(
-                                            map(
-                                                lambda x: f"scrapeinfo pinned: {str(x)}",
-                                                posts,
-                                            )
-                                        )
-                                    ),
-                                )
-                            )
-                            new_tasks.append(
-                                asyncio.create_task(
-                                    scrape_pinned_posts(
-                                        c,
-                                        model_id,
-                                        job_progress=job_progress,
-                                        timestamp=posts[-1]["postedAtPrecise"],
-                                        count=count + len(posts),
-                                    )
-                                )
-                            )
-                    else:
-                        log.debug(f"[bold]t response status code:[/bold]{r.status}")
-                        log.debug(f"[bold]pinned response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]pinned headers:[/bold] {r.headers}")
-                        r.raise_for_status()
-            except Exception as E:
-                await asyncio.sleep(1)
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
+                    )
+                )
+    except asyncio.TimeoutError:
+        raise Exception(f"Task timed out {url}")
 
-            finally:
-                sem.release()
-                job_progress.remove_task(task) if job_progress and task else None
-            return posts, new_tasks
+    except Exception as E:
+        await asyncio.sleep(1)
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
+
+    finally:
+        job_progress.remove_task(task) if job_progress and task else None
+    return posts, new_tasks
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/helpers.py` & `ofscraper-3.9.1/ofscraper/utils/auth/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,79 +7,71 @@
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
-import contextvars
+import json
 import logging
-import traceback
 
+import browser_cookie3
+import requests
 from rich.console import Console
-from tenacity import (
-    AsyncRetrying,
-    retry,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random,
-)
-
-import ofscraper.utils.constants as constants
-import ofscraper.utils.settings as settings
-from ofscraper.classes.semaphoreDelayed import semaphoreDelayed
-from ofscraper.utils.context.run_async import run
 
-log = logging.getLogger("shared")
-attempt = contextvars.ContextVar("attempt")
-console = Console()
-sem = None
+import ofscraper.prompts.prompts as prompts
+import ofscraper.utils.paths.common as common_paths
 
+console = Console()
+log = logging.getLogger("shared")
 
-def get_user_list_helper():
-    return settings.get_userlist(as_list=True)
 
+def get_auth_dict(authStr=None):
+    auth = json.loads(authStr or get_auth_string())
+    if "auth" in auth:
+        return auth.get("auth")
+    return auth
+
+
+def get_auth_string():
+    authFile = common_paths.get_auth_file()
+    with open(authFile, "r") as f:
+        authText = f.read()
+    return authText
+
+
+def get_empty():
+    return {
+        "sess": "",
+        "auth_id": "",
+        "auth_uid": "",
+        "user_agent": "",
+        "x-bc": "",
+    }
+
+
+def authwarning(authFile):
+    console.print(
+        "[bold yellow]For an example of how your auth file should look see \
+            \n [bold blue]https://of-scraper.gitbook.io/of-scraper/auth#example[/bold blue][/bold yellow]"
+    )
+    console.print(
+        f"[bold yellow]If you still can't authenticate after editing from script consider manually edit the file at\n[bold blue]{authFile}[/bold blue][/bold yellow]"
+    )
+
+
+def browser_cookie_helper(auth, browserSelect):
+    temp = requests.utils.dict_from_cookiejar(
+        getattr(browser_cookie3, browserSelect.lower())(domain_name="onlyfans")
+    )
+    for key in ["sess", "auth_id", "auth_uid_"]:
+        auth[key] = auth[key] or temp.get(key, "")
+    console.print(
+        "You'll need to go to onlyfans.com and retrive/update header information\nGo to https://github.com/datawhores/OF-Scraper and find the section named 'Getting Your Auth Info'\nCookie information has been retived automatically\nSo You only need to retrive the x-bc header and the user-agent",
+        style="yellow",
+    )
+    auth["x-bc"] = prompts.xbc_prompt(auth.get("x-bc"))
+    auth["user_agent"] = prompts.user_agent_prompt(auth.get("user_agent"))
 
-def get_black_list_helper():
-    return settings.get_blacklist(as_list=True)
-
-
-async def sort_list(c) -> list:
-    global sem
-    sem = semaphoreDelayed(constants.getattr("AlT_SEM"))
-    attempt.set(0)
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            await sem.acquire()
-            try:
-                attempt.set(attempt.get(0) + 1)
-                async with c.requests(
-                    constants.getattr("sortSubscription"),
-                    method="post",
-                    json={"order": "users.name", "direction": "desc", "type": "all"},
-                )() as r:
-                    if r.ok:
-                        None
-                    else:
-                        log.debug(
-                            f"[bold]subscriptions response status code:[/bold]{r.status}"
-                        )
-                        log.debug(
-                            f"[bold]subscriptions response:[/bold] {await r.text_()}"
-                        )
-                        log.debug(f"[bold]subscriptions headers:[/bold] {r.headers}")
-                        r.raise_for_status()
-            except Exception as E:
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
 
-            finally:
-                sem.release()
+def cookie_helper_extension():
+    return prompts.auth_full_paste()
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/individual.py` & `ofscraper-3.9.1/ofscraper/api/subscriptions/individual.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,46 +16,52 @@
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from rich.style import Style
 
 import ofscraper.api.profile as profile
-import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.constants as constants
-from ofscraper.classes.semaphoreDelayed import semaphoreDelayed
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
 
 
 @run
 async def get_subscription(accounts=None):
-    global sem
-    sem = semaphoreDelayed(constants.getattr("AlT_SEM"))
     accounts = accounts or read_args.retriveArgs().usernames
     if not isinstance(accounts, list) and not isinstance(accounts, set):
         accounts = set([accounts])
     with ThreadPoolExecutor(
-        max_workers=constants.getattr("MAX_REQUEST_WORKERS")
+        max_workers=constants.getattr("MAX_THREAD_WORKERS")
     ) as executor:
         asyncio.get_event_loop().set_default_executor(executor)
 
         with Progress(
             SpinnerColumn(style=Style(color="blue")), TextColumn("{task.description}")
         ) as job_progress:
             task1 = job_progress.add_task(
                 f"Getting the following accounts => {accounts} (this may take awhile)..."
             )
-            async with sessionbuilder.sessionBuilder() as c:
+            async with sessionManager.sessionManager(
+                sem=constants.getattr("SUBSCRIPTION_SEMS"),
+                retries=constants.getattr("API_INDVIDIUAL_NUM_TRIES"),
+                wait_min=constants.getattr("OF_MIN_WAIT_API"),
+                wait_max=constants.getattr("OF_MAX_WAIT_API"),
+                new_request_auth=True,
+            ) as c:
                 out = await get_subscription_helper(c, accounts)
                 job_progress.remove_task(task1)
         outdict = {}
-        for ele in filter(lambda x: x["username"] != "modeldeleted", out):
+        for ele in filter(
+            lambda x: x["username"] != constants.getattr("DELETED_MODEL_PLACEHOLDER"),
+            out,
+        ):
             outdict[ele["id"]] = ele
         log.debug(f"Total subscriptions found {len(outdict.values())}")
         return list(outdict.values())
 
 
 async def get_subscription_helper(c, accounts):
     output = []
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/lists.py` & `ofscraper-3.9.1/ofscraper/api/subscriptions/lists.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,32 +18,23 @@
 from concurrent.futures import ThreadPoolExecutor
 
 from rich.console import Group
 from rich.live import Live
 from rich.panel import Panel
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from rich.style import Style
-from tenacity import (
-    AsyncRetrying,
-    retry,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random,
-)
 
-import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.console as console
 import ofscraper.utils.constants as constants
-import ofscraper.utils.sems as sems
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
 attempt = contextvars.ContextVar("attempt")
-sem = None
 
 
 @run
 async def get_otherlist():
     out = []
     if any(
         [
@@ -54,15 +45,15 @@
             ]
             for ele in read_args.retriveArgs().user_list or []
         ]
     ):
         out.extend(await get_lists())
     out = list(
         filter(
-            lambda x: x.get("name").lower() in read_args.retriveArgs().user_list or[],
+            lambda x: x.get("name").lower() in read_args.retriveArgs().user_list or [],
             out,
         )
     )
     log.debug(
         f"User lists found on profile {list(map(lambda x:x.get('name').lower(),out))}"
     )
     return await get_list_users(out)
@@ -84,15 +75,15 @@
     )
     names = list(await get_list_users(out))
     return set(list(map(lambda x: x["id"], names)))
 
 
 async def get_lists():
     with ThreadPoolExecutor(
-        max_workers=constants.getattr("MAX_REQUEST_WORKERS")
+        max_workers=constants.getattr("MAX_THREAD_WORKERS")
     ) as executor:
         asyncio.get_event_loop().set_default_executor(executor)
         overall_progress = Progress(
             SpinnerColumn(style=Style(color="blue")),
             TextColumn("Getting lists...\n{task.description}"),
         )
         job_progress = Progress("{task.description}")
@@ -100,128 +91,99 @@
 
         output = []
         tasks = []
         page_count = 0
         with Live(
             progress_group, refresh_per_second=5, console=console.get_shared_console()
         ):
-            async with sessionbuilder.sessionBuilder() as c:
-                tasks.append(asyncio.create_task(scrape_lists(c, job_progress)))
+            async with sessionManager.sessionManager(
+                sem=constants.getattr("SUBSCRIPTION_SEMS"),
+                retries=constants.getattr("API_INDVIDIUAL_NUM_TRIES"),
+                wait_min=constants.getattr("OF_MIN_WAIT_API"),
+                wait_max=constants.getattr("OF_MAX_WAIT_API"),
+                new_request_auth=True,
+            ) as c:
+                tasks.append(asyncio.create_task(scrape_for_list(c, job_progress)))
                 page_task = overall_progress.add_task(
                     f"UserList Pages Progress: {page_count}", visible=True
                 )
-                while bool(tasks):
+                while tasks:
                     new_tasks = []
-                    try:
-                        async with asyncio.timeout(
-                            constants.getattr("API_TIMEOUT_PER_TASKS")
-                            * max(len(tasks), 2)
-                        ):
-                            for task in asyncio.as_completed(tasks):
-                                try:
-                                    result, new_tasks_batch = await task
-                                    new_tasks.extend(new_tasks_batch)
-                                    page_count = page_count + 1
-                                    overall_progress.update(
-                                        page_task,
-                                        description=f"UserList Pages Progress: {page_count}",
-                                    )
-                                    output.extend(result)
-                                except Exception as E:
-                                    log.traceback_(E)
-                                    log.traceback_(traceback.format_exc())
-                                    continue
-                    except TimeoutError as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
+                    for task in asyncio.as_completed(tasks):
+                        try:
+                            result, new_tasks_batch = await task
+                            new_tasks.extend(new_tasks_batch)
+                            page_count = page_count + 1
+                            overall_progress.update(
+                                page_task,
+                                description=f"UserList Pages Progress: {page_count}",
+                            )
+                            output.extend(result)
+                        except Exception as E:
+                            log.traceback_(E)
+                            log.traceback_(traceback.format_exc())
+                            continue
                     tasks = new_tasks
-
-        overall_progress.remove_task(page_task)
-        log.trace(
-            "list unduped {posts}".format(
-                posts="\n\n".join(map(lambda x: f" list data raw:{x}", output))
-            )
+    overall_progress.remove_task(page_task)
+    log.trace(
+        "list unduped {posts}".format(
+            posts="\n\n".join(map(lambda x: f" list data raw:{x}", output))
         )
-        log.debug(f"[bold]lists name count without Dupes[/bold] {len(output)} found")
-        return output
+    )
+    log.debug(f"[bold]lists name count without Dupes[/bold] {len(output)} found")
+    return output
 
 
-async def scrape_lists(c, job_progress, offset=0):
-    global sem
-    global tasks
-    sem = sems.get_req_sem()
+async def scrape_for_list(c, job_progress, offset=0):
     attempt.set(0)
-    async for _ in AsyncRetrying(
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            new_tasks = []
-            await sem.acquire()
-            try:
-                attempt.set(attempt.get(0) + 1)
-                task = job_progress.add_task(
-                    f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} : getting lists offset -> {offset}",
-                    visible=True,
+    new_tasks = []
+    url = constants.getattr("listEP").format(offset)
+    try:
+        attempt.set(attempt.get(0) + 1)
+        task = job_progress.add_task(
+            f" : getting lists offset -> {offset}",
+            visible=True,
+        )
+        async with c.requests_async(url=url) as r:
+            data = await r.json_()
+            out_list = data["list"] or []
+            log.debug(
+                f"offset:{offset} -> lists names found {list(map(lambda x:x['name'],out_list))}"
+            )
+            log.debug(f"offset:{offset} -> number of lists found {len(out_list)}")
+            log.debug(
+                f"offset:{offset} -> hasMore value in json {data.get('hasMore','undefined') }"
+            )
+            log.trace(
+                "offset:{offset} -> label names raw: {posts}".format(
+                    offset=offset, posts=data
                 )
-                async with c.requests(
-                    url=constants.getattr("listEP").format(offset)
-                )() as r:
-                    if r.ok:
-                        data = await r.json_()
-                        out_list = data["list"] or []
-                        log.debug(
-                            f"offset:{offset} -> lists names found {list(map(lambda x:x['name'],out_list))}"
-                        )
-                        log.debug(
-                            f"offset:{offset} -> number of lists found {len(out_list)}"
-                        )
-                        log.debug(
-                            f"offset:{offset} -> hasMore value in json {data.get('hasMore','undefined') }"
-                        )
-                        log.trace(
-                            "offset:{offset} -> label names raw: {posts}".format(
-                                offset=offset, posts=data
-                            )
-                        )
+            )
 
-                        if data.get("hasMore") and len(out_list) > 0:
-                            offset = offset + len(out_list)
-                            new_tasks.append(
-                                asyncio.create_task(
-                                    scrape_lists(c, job_progress, offset=offset)
-                                )
-                            )
+            if data.get("hasMore") and len(out_list) > 0:
+                offset = offset + len(out_list)
+                new_tasks.append(
+                    asyncio.create_task(scrape_for_list(c, job_progress, offset=offset))
+                )
+    except asyncio.TimeoutError:
+        raise Exception(f"Task timed out {url}")
 
-                    else:
-                        log.debug(f"[bold]lists response status code:[/bold]{r.status}")
-                        log.debug(f"[bold]lists response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]lists headers:[/bold] {r.headers}")
-                        r.raise_for_status()
-            except Exception as E:
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
-
-            finally:
-                sem.release()
-                job_progress.remove_task(task)
-            return out_list, new_tasks
+    except Exception as E:
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
+
+    finally:
+        job_progress.remove_task(task)
+    return out_list, new_tasks
 
 
 async def get_list_users(lists):
-    global sem
-    sem = sems.get_req_sem()
     with ThreadPoolExecutor(
-        max_workers=constants.getattr("MAX_REQUEST_WORKERS")
+        max_workers=constants.getattr("MAX_THREAD_WORKERS")
     ) as executor:
         asyncio.get_event_loop().set_default_executor(executor)
         overall_progress = Progress(
             SpinnerColumn(style=Style(color="blue")),
             TextColumn(
                 "Getting users from lists (this may take awhile)...\n{task.description}"
             ),
@@ -231,138 +193,108 @@
 
         output = []
         tasks = []
         page_count = 0
         with Live(
             progress_group, refresh_per_second=5, console=console.get_shared_console()
         ):
-            async with sessionbuilder.sessionBuilder() as c:
+            async with sessionManager.sessionManager(
+                sem=constants.getattr("SUBSCRIPTION_SEMS"),
+                retries=constants.getattr("API_INDVIDIUAL_NUM_TRIES"),
+                wait_min=constants.getattr("OF_MIN_WAIT_API"),
+                wait_max=constants.getattr("OF_MAX_WAIT_API"),
+                new_request_auth=True,
+            ) as c:
                 [
-                    tasks.append(asyncio.create_task(scrape_list(c, id, job_progress)))
+                    tasks.append(
+                        asyncio.create_task(scrape_list_members(c, id, job_progress))
+                    )
                     for id in lists
                 ]
                 page_task = overall_progress.add_task(
                     f"UserList Users Pages Progress: {page_count}", visible=True
                 )
-                while bool(tasks):
+                while tasks:
                     new_tasks = []
-                    try:
-                        async with asyncio.timeout(
-                            constants.getattr("API_TIMEOUT_PER_TASKS")
-                            * max(len(tasks), 2)
-                        ):
-                            for task in asyncio.as_completed(tasks):
-                                try:
-                                    result, new_tasks_batch = await task
-                                    new_tasks.extend(new_tasks_batch)
-                                    page_count = page_count + 1
-                                    overall_progress.update(
-                                        page_task,
-                                        description=f"UserList Users Pages Progress: {page_count}",
-                                    )
-                                    output.extend(result)
-                                except Exception as E:
-                                    log.traceback_(E)
-                                    log.traceback_(traceback.format_exc())
-                                    continue
-                    except TimeoutError as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-
+                    for task in asyncio.as_completed(tasks):
+                        try:
+                            result, new_tasks_batch = await task
+                            new_tasks.extend(new_tasks_batch)
+                            page_count = page_count + 1
+                            overall_progress.update(
+                                page_task,
+                                description=f"UserList Users Pages Progress: {page_count}",
+                            )
+                            output.extend(result)
+                        except Exception as E:
+                            log.traceback_(E)
+                            log.traceback_(traceback.format_exc())
+                            continue
                     tasks = new_tasks
+
     overall_progress.remove_task(page_task)
     outdict = {}
     for ele in output:
         outdict[ele["id"]] = ele
     log.trace(
         "users found {users}".format(
-            users="\n\n".join(
-                list(map(lambda x: f"user data: {str(x)}", outdict.values()))
-            )
+            users="\n\n".join(map(lambda x: f"user data: {str(x)}", outdict.values()))
         )
     )
     log.debug(f"[bold]users count without Dupes[/bold] {len(outdict.values())} found")
     return outdict.values()
 
 
-async def scrape_list(c, item, job_progress, offset=0):
-    global sem
-    global tasks
+async def scrape_list_members(c, item, job_progress, offset=0):
     users = None
     attempt.set(0)
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            new_tasks = []
-            await sem.acquire()
-            try:
-                attempt.set(attempt.get(0) + 1)
-                task = job_progress.add_task(
-                    f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} : offset -> {offset} + list name -> {item.get('name')}",
-                    visible=True,
-                )
+    new_tasks = []
+    url = constants.getattr("listusersEP").format(item.get("id"), offset)
+    try:
+        attempt.set(attempt.get(0) + 1)
+        task = job_progress.add_task(
+            f" : offset -> {offset} + list name -> {item.get('name')}",
+            visible=True,
+        )
 
-                async with c.requests(
-                    url=constants.getattr("listusersEP").format(item.get("id"), offset)
-                )() as r:
-                    log_id = f"offset:{offset} list:{item.get('name')} =>"
-                    if r.ok:
-                        data = await r.json_()
-                        users = data.get("list") or []
-                        log.debug(f"{log_id} -> names found {len(users)}")
-                        log.debug(
-                            f"{log_id}  -> hasMore value in json {data.get('hasMore','undefined') }"
-                        )
-                        log.debug(
-                            f"usernames {log_id} : usernames retrived -> {list(map(lambda x:x.get('username'),users))}"
-                        )
-                        log.trace(
-                            "offset: {offset} list: {item} -> {posts}".format(
-                                item=item.get("name"),
-                                offset=offset,
-                                posts="\n\n".join(
-                                    list(
-                                        map(
-                                            lambda x: f"scrapeinfo list {str(x)}", users
-                                        )
-                                    )
-                                ),
-                            )
-                        )
-                        if (
-                            data.get("hasMore")
-                            and len(users) > 0
-                            and offset != data.get("nextOffset")
-                        ):
-                            offset += len(users)
-                            new_tasks.append(
-                                asyncio.create_task(
-                                    scrape_list(c, item, job_progress, offset=offset)
-                                )
-                            )
+        async with c.requests_async(url=url) as r:
+            log_id = f"offset:{offset} list:{item.get('name')} =>"
+            data = await r.json_()
+            users = data.get("list") or []
+            log.debug(f"{log_id} -> names found {len(users)}")
+            log.debug(
+                f"{log_id}  -> hasMore value in json {data.get('hasMore','undefined') }"
+            )
+            log.debug(
+                f"usernames {log_id} : usernames retrived -> {list(map(lambda x:x.get('username'),users))}"
+            )
+            log.trace(
+                "offset: {offset} list: {item} -> {posts}".format(
+                    item=item.get("name"),
+                    offset=offset,
+                    posts="\n\n".join(
+                        map(lambda x: f"scrapeinfo list {str(x)}", users)
+                    ),
+                )
+            )
+            if (
+                data.get("hasMore")
+                and len(users) > 0
+                and offset != data.get("nextOffset")
+            ):
+                offset += len(users)
+                new_tasks.append(
+                    asyncio.create_task(
+                        scrape_list_members(c, item, job_progress, offset=offset)
+                    )
+                )
+    except asyncio.TimeoutError:
+        raise Exception(f"Task timed out {url}")
 
-                    else:
-                        log.debug(
-                            f"[bold]labelled posts response status code:[/bold]{r.status}"
-                        )
-                        log.debug(
-                            f"[bold]labelled posts response:[/bold] {await r.text_()}"
-                        )
-                        log.debug(f"[bold]labelled posts headers:[/bold] {r.headers}")
-
-                        r.raise_for_status()
-            except Exception as E:
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
-
-            finally:
-                sem.release()
-                job_progress.remove_task(task)
-            return users, new_tasks
+    except Exception as E:
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
+
+    finally:
+        job_progress.remove_task(task)
+    return users, new_tasks
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/api/subscriptions/subscriptions.py` & `ofscraper-3.9.1/ofscraper/api/subscriptions/subscriptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,73 +8,62 @@
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
 import asyncio
-import contextvars
 import logging
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 
 from rich.console import Console
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from rich.style import Style
-from tenacity import (
-    AsyncRetrying,
-    retry,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random,
-)
 
 import ofscraper.api.subscriptions.helpers as helpers
-import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.constants as constants
-from ofscraper.classes.semaphoreDelayed import semaphoreDelayed
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
-attempt = contextvars.ContextVar("attempt")
 console = Console()
-sem = None
 
 
 @run
 async def get_subscriptions(subscribe_count, account="active"):
-    global sem
-    sem = semaphoreDelayed(constants.getattr("AlT_SEM"))
     with ThreadPoolExecutor(
-        max_workers=constants.getattr("MAX_REQUEST_WORKERS")
+        max_workers=constants.getattr("MAX_THREAD_WORKERS")
     ) as executor:
         asyncio.get_event_loop().set_default_executor(executor)
 
         with Progress(
             SpinnerColumn(style=Style(color="blue")), TextColumn("{task.description}")
         ) as job_progress:
             task1 = job_progress.add_task(
                 f"Getting your {account} subscriptions (this may take awhile)..."
             )
-            async with sessionbuilder.sessionBuilder() as c:
+            async with sessionManager.sessionManager(
+                sem=constants.getattr("SUBSCRIPTION_SEMS"),
+                retries=constants.getattr("API_INDVIDIUAL_NUM_TRIES"),
+                wait_min=constants.getattr("OF_MIN_WAIT_API"),
+                wait_max=constants.getattr("OF_MAX_WAIT_API"),
+                new_request_auth=True,
+            ) as c:
                 if account == "active":
                     out = await activeHelper(subscribe_count, c)
                 else:
                     out = await expiredHelper(subscribe_count, c)
                 job_progress.remove_task(task1)
-        outdict = {}
-        for ele in out:
-            outdict[ele["id"]] = ele
-        log.debug(f"Total {account} subscriptions found {len(outdict.values())}")
-        return list(outdict.values())
 
+        log.debug(f"Total {account} subscriptions found {len(out)}")
+        return out
 
-async def activeHelper(subscribe_count, c):
-    output = []
 
+async def activeHelper(subscribe_count, c):
     if any(
         x in helpers.get_black_list_helper()
         for x in [
             constants.getattr("OFSCRAPER_RESERVED_LIST"),
             constants.getattr("OFSCRAPER_RESERVED_LIST_ALT"),
         ]
     ) or any(
@@ -102,38 +91,18 @@
     funct = scrape_subscriptions_active
 
     tasks = [
         asyncio.create_task(funct(c, offset))
         for offset in range(0, subscribe_count + 1, 10)
     ]
     tasks.extend([asyncio.create_task(funct(c, subscribe_count + 1, recur=True))])
-    while bool(tasks):
-        new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        output.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-        tasks = new_tasks
-    return output
+    return await process_task(tasks)
 
 
 async def expiredHelper(subscribe_count, c):
-    output = []
     if any(
         x in helpers.get_black_list_helper()
         for x in [
             constants.getattr("OFSCRAPER_RESERVED_LIST"),
             constants.getattr("OFSCRAPER_RESERVED_LIST_ALT"),
         ]
     ) or any(
@@ -162,152 +131,101 @@
 
     tasks = [
         asyncio.create_task(funct(c, offset))
         for offset in range(0, subscribe_count + 1, 10)
     ]
     tasks.extend([asyncio.create_task(funct(c, subscribe_count + 1, recur=True))])
 
-    while bool(tasks):
-        new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        output.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-        tasks = new_tasks
-    return output
+    return await process_task(tasks)
 
 
-async def scrape_subscriptions_active(c, offset=0, num=0, recur=False) -> list:
-    sem = semaphoreDelayed(constants.getattr("AlT_SEM"))
-    attempt.set(0)
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            new_tasks = []
-            await sem.acquire()
+async def process_task(tasks):
+    output = []
+    seen = set()
+    while tasks:
+        new_tasks = []
+        for task in asyncio.as_completed(tasks):
             try:
-                attempt.set(attempt.get(0) + 1)
-                log.debug(
-                    f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} usernames active offset {offset}"
-                )
-                async with c.requests(
-                    constants.getattr("subscriptionsActiveEP").format(offset)
-                )() as r:
-                    if r.ok:
-                        subscriptions = (await r.json_())["list"]
-                        log.debug(
-                            f"usernames retrived -> {list(map(lambda x:x.get('username'),subscriptions))}"
-                        )
-                        if len(subscriptions) == 0:
-                            return subscriptions
-                        elif recur == False:
-                            None
-                        elif (await r.json_())["hasMore"] == True:
-                            new_tasks.append(
-                                asyncio.create_task(
-                                    scrape_subscriptions_active(
-                                        c,
-                                        recur=True,
-                                        offset=offset + len(subscriptions),
-                                    )
-                                )
-                            )
-                        return subscriptions, new_tasks
-                    else:
-                        log.debug(
-                            f"[bold]subscriptions response status code:[/bold]{r.status}"
-                        )
-                        log.debug(
-                            f"[bold]subscriptions response:[/bold] {await r.text_()}"
-                        )
-                        log.debug(f"[bold]subscriptions headers:[/bold] {r.headers}")
-                        r.raise_for_status()
+                result, new_tasks_batch = await task
+                new_tasks.extend(new_tasks_batch)
+                users = [
+                    user
+                    for user in result
+                    if user["id"] not in seen and not seen.add(user["id"])
+                ]
+                output.extend(users)
             except Exception as E:
                 log.traceback_(E)
                 log.traceback_(traceback.format_exc())
-                raise E
+                continue
+        tasks = new_tasks
+    return output
 
-            finally:
-                sem.release()
 
+async def scrape_subscriptions_active(c, offset=0, num=0, recur=False) -> list:
+    new_tasks = []
+    url = constants.getattr("subscriptionsActiveEP").format(offset)
+    try:
+        log.debug(f"usernames active offset {offset}")
+        async with c.requests_async(url=url) as r:
+            subscriptions = (await r.json_())["list"]
+            log.debug(
+                f"usernames retrived -> {list(map(lambda x:x.get('username'),subscriptions))}"
+            )
+            if len(subscriptions) == 0:
+                return subscriptions
+            elif recur is False:
+                pass
+            elif (await r.json_())["hasMore"] is True:
+                new_tasks.append(
+                    asyncio.create_task(
+                        scrape_subscriptions_active(
+                            c,
+                            recur=True,
+                            offset=offset + len(subscriptions),
+                        )
+                    )
+                )
+            return subscriptions, new_tasks
+    except asyncio.TimeoutError:
+        raise Exception(f"Task timed out {url}")
+
+    except Exception as E:
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
 
-async def scrape_subscriptions_disabled(c, offset=0, num=0, recur=False) -> list:
-    attempt.set(0)
-    sem = semaphoreDelayed(constants.getattr("AlT_SEM"))
 
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            new_tasks = []
-            await sem.acquire()
-            try:
-                attempt.set(attempt.get(0) + 1)
-                log.debug(
-                    f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')} usernames offset expired {offset}"
-                )
-                async with c.requests(
-                    constants.getattr("subscriptionsExpiredEP").format(offset)
-                )() as r:
-                    if r.ok:
-                        subscriptions = (await r.json_())["list"]
-                        log.debug(
-                            f"usernames retrived -> {list(map(lambda x:x.get('username'),subscriptions))}"
-                        )
+async def scrape_subscriptions_disabled(c, offset=0, num=0, recur=False) -> list:
+    new_tasks = []
+    url = constants.getattr("subscriptionsExpiredEP").format(offset)
+    try:
+        log.debug(f"usernames offset expired {offset}")
+        async with c.requests_async(url=url) as r:
+            subscriptions = (await r.json_())["list"]
+            log.debug(
+                f"usernames retrived -> {list(map(lambda x:x.get('username'),subscriptions))}"
+            )
 
-                        if len(subscriptions) == 0:
-                            return subscriptions
-                        elif recur == False:
-                            None
-                        elif (await r.json_())["hasMore"] == True:
-                            new_tasks.append(
-                                asyncio.create_task(
-                                    scrape_subscriptions_disabled(
-                                        c,
-                                        recur=True,
-                                        offset=offset + len(subscriptions),
-                                    )
-                                )
-                            )
-
-                        return subscriptions, new_tasks
-                    else:
-                        log.debug(
-                            f"[bold]subscriptions response status code:[/bold]{r.status}"
-                        )
-                        log.debug(
-                            f"[bold]subscriptions response:[/bold] {await r.text_()}"
+            if len(subscriptions) == 0:
+                return subscriptions
+            elif recur is False:
+                pass
+            elif (await r.json_())["hasMore"] is True:
+                new_tasks.append(
+                    asyncio.create_task(
+                        scrape_subscriptions_disabled(
+                            c,
+                            recur=True,
+                            offset=offset + len(subscriptions),
                         )
-                        log.debug(f"[bold]subscriptions headers:[/bold] {r.headers}")
-                        r.raise_for_status()
-            except Exception as E:
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
+                    )
+                )
 
-            finally:
-                sem.release()
+            return subscriptions, new_tasks
+    except asyncio.TimeoutError:
+        raise Exception(f"Task timed out {url}")
+
+    except Exception as E:
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/api/timeline.py` & `ofscraper-3.9.1/ofscraper/api/timeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,175 +4,160 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import asyncio
-import contextvars
 import logging
 import math
 import traceback
 
 import arrow
-from tenacity import (
-    AsyncRetrying,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random,
-)
 
-import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.api.common.logs as common_logs
+import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.db.operations as operations
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
-import ofscraper.utils.sems as sems
 import ofscraper.utils.settings as settings
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
-attempt = contextvars.ContextVar("attempt")
-sem = None
 
 
 @run
 async def get_timeline_posts_progress(model_id, username, forced_after=None, c=None):
-    global sem
-    sem = sems.get_req_sem()
 
     after = await get_after(model_id, username, forced_after)
-
+    after_log(username, after)
     splitArrays = await get_split_array(model_id, username, after)
     tasks = get_tasks(splitArrays, c, model_id, after)
-    data = await process_tasks(tasks, model_id, after)
+    data = await process_tasks(tasks)
     progress_utils.timeline_layout.visible = False
     return data
 
 
 @run
 async def get_timeline_posts(model_id, username, forced_after=None, c=None):
-    global sem
-    sem = sems.get_req_sem()
-
     if not read_args.retriveArgs().no_cache:
-        oldtimeline = await operations.get_timeline_postsinfo(
+        oldtimeline = await operations.get_timeline_posts_info(
             model_id=model_id, username=username
         )
     else:
         oldtimeline = []
-    log.trace(
-        "oldtimeline {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"oldtimeline: {str(x)}", oldtimeline))
-            )
-        )
-    )
+    trace_log_old(oldtimeline)
+
     log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
     oldtimeline = list(filter(lambda x: x != None, oldtimeline))
     after = await get_after(model_id, username, forced_after)
+    after_log(username, after)
 
     with progress_utils.set_up_api_timeline():
         splitArrays = await get_split_array(model_id, username, after)
         tasks = get_tasks(splitArrays, c, model_id, after)
-        return await process_tasks(tasks, model_id, after)
+        return await process_tasks(tasks)
 
 
-async def process_tasks(tasks, model_id, after):
+async def process_tasks(tasks):
     responseArray = []
     page_count = 0
     overall_progress = progress_utils.overall_progress
 
     page_task = overall_progress.add_task(
         f" Timeline Content Pages Progress: {page_count}", visible=True
     )
-    while bool(tasks):
+    seen = set()
+    while tasks:
         new_tasks = []
-        try:
-            async with asyncio.timeout(
-                constants.getattr("API_TIMEOUT_PER_TASKS") * max(len(tasks), 2)
-            ):
-                for task in asyncio.as_completed(tasks):
-                    try:
-                        result, new_tasks_batch = await task
-                        new_tasks.extend(new_tasks_batch)
-                        page_count = page_count + 1
-                        overall_progress.update(
-                            page_task,
-                            description=f"Timeline Content Pages Progress: {page_count}",
+        for task in asyncio.as_completed(tasks):
+            try:
+                result, new_tasks_batch = await task
+                new_tasks.extend(new_tasks_batch)
+                page_count = page_count + 1
+                overall_progress.update(
+                    page_task,
+                    description=f"Timeline Content Pages Progress: {page_count}",
+                )
+                new_posts = [
+                    post
+                    for post in result
+                    if post["id"] not in seen and not seen.add(post["id"])
+                ]
+                log.debug(
+                    f"{common_logs.PROGRESS_IDS.format('Timeline')} {list(map(lambda x:x['id'],new_posts))}"
+                )
+                log.trace(
+                    f"{common_logs.PROGRESS_RAW.format('Timeline')}".format(
+                        posts="\n\n".join(
+                            list(
+                                map(
+                                    lambda x: f"{common_logs.RAW_INNER} {x}",
+                                    new_posts,
+                                )
+                            )
                         )
-                        responseArray.extend(result)
-                    except Exception as E:
-                        log.traceback_(E)
-                        log.traceback_(traceback.format_exc())
-                        continue
-        except TimeoutError as E:
-            cache.set(f"{model_id}_full_timeline_scrape")
-            log.traceback_(E)
-            log.traceback_(traceback.format_exc())
-        tasks = new_tasks
-    overall_progress.remove_task(page_task)
+                    )
+                )
 
-    log.debug(f"[bold]Timeline Count with Dupes[/bold] {len(responseArray)} found")
-    log.trace(
-        "post raw duped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"dupedinfo timeline: {str(x)}", responseArray))
-            )
-        )
-    )
-    seen = set()
-    new_posts = [
-        post
-        for post in responseArray
-        if post["id"] not in seen and not seen.add(post["id"])
-    ]
+                responseArray.extend(new_posts)
+            except Exception as E:
+                log.traceback_(E)
+                log.traceback_(traceback.format_exc())
+                continue
+        tasks = new_tasks
 
-    log.trace(f"timeline postids {list(map(lambda x:x.get('id'),new_posts))}")
-    log.trace(
-        "post raw unduped {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"undupedinfo timeline: {str(x)}", new_posts))
-            )
-        )
+    overall_progress.remove_task(page_task)
+    log.debug(
+        f"{common_logs.FINAL_IDS.format('Timeline')} {list(map(lambda x:x['id'],responseArray))}"
     )
-    log.debug(f"[bold]Timeline Count without Dupes[/bold] {len(new_posts)} found")
-    set_check(new_posts, model_id, after)
-    return new_posts
+    log.debug(f"{common_logs.FINAL_COUNT.format('Timeline')} {len(responseArray)}")
 
+    trace_log_task(responseArray)
+    return responseArray
 
-async def get_split_array(model_id, username, after):
-    min_posts = 50
 
+async def get_oldtimeline(model_id, username):
     if not read_args.retriveArgs().no_cache:
-        oldtimeline = await operations.get_timeline_postsinfo(
+        oldtimeline = await operations.get_timeline_posts_info(
             model_id=model_id, username=username
         )
     else:
         oldtimeline = []
-    log.trace(
-        "oldtimeline {posts}".format(
-            posts="\n\n".join(
-                list(map(lambda x: f"oldtimeline: {str(x)}", oldtimeline))
-            )
-        )
-    )
-    log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
     oldtimeline = list(filter(lambda x: x is not None, oldtimeline))
-    postsDataArray = sorted(oldtimeline, key=lambda x: x.get("created_at"))
-    log.info(
-        f"""
-Setting initial timeline scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
-[yellow]Hint: append ' --after 2000' to command to force scan of all timeline posts + download of new files only[/yellow]
-[yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all timeline posts + download/re-download of all files[/yellow]
+    # dedupe oldtimeline
+    seen = set()
+    oldtimeline = [
+        post
+        for post in oldtimeline
+        if post["post_id"] not in seen and not seen.add(post["post_id"])
+    ]
+    log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
+    trace_log_old(oldtimeline)
+    return oldtimeline
 
-            """
+
+async def get_split_array(model_id, username, after):
+
+    oldtimeline = await get_oldtimeline(model_id, username)
+    if len(oldtimeline) == 0:
+        return []
+    min_posts = max(
+        len(oldtimeline) // constants.getattr("REASONABLE_MAX_PAGE"),
+        constants.getattr("MIN_PAGE_POST_COUNT"),
+    )
+    postsDataArray = sorted(oldtimeline, key=lambda x: arrow.get(x["created_at"]))
+    filteredArray = list(filter(lambda x: bool(x["created_at"]), postsDataArray))
+    filteredArray = list(
+        filter(
+            lambda x: arrow.get(x["created_at"]).float_timestamp >= after, filteredArray
+        )
     )
-    filteredArray = list(filter(lambda x: x.get("created_at") >= after, postsDataArray))
 
     splitArrays = [
         filteredArray[i : i + min_posts]
         for i in range(0, len(filteredArray), min_posts)
     ]
     return splitArrays
 
@@ -241,202 +226,225 @@
         tasks.append(
             asyncio.create_task(
                 scrape_timeline_posts(
                     c, model_id, job_progress=job_progress, timestamp=after, offset=True
                 )
             )
         )
+
     return tasks
 
 
 def set_check(unduped, model_id, after):
     if not after:
         seen = set()
         all_posts = [
             post
             for post in cache.get(f"timeline_check_{model_id}", default=[]) + unduped
             if post["id"] not in seen and not seen.add(post["id"])
         ]
         cache.set(
             f"timeline_check_{model_id}",
             all_posts,
-            expire=constants.getattr("DAY_SECONDS"),
+            expire=constants.getattr("THREE_DAY_SECONDS"),
         )
         cache.close()
 
 
 def get_individual_post(id):
-    with sessionbuilder.sessionBuilder(backend="httpx") as c:
-        with c.requests(constants.getattr("INDIVIDUAL_TIMELINE").format(id))() as r:
-            if r.ok:
-                log.trace(f"post raw individual {r.json()}")
-                return r.json()
-            else:
-                log.debug(
-                    f"[bold]individual post response status code:[/bold]{r.status}"
-                )
-                log.debug(f"[bold]individual post response:[/bold] {r.text_()}")
-                log.debug(f"[bold]individual post headers:[/bold] {r.headers}")
+    with sessionManager.sessionManager(
+        backend="httpx",
+        retries=constants.getattr("API_INDVIDIUAL_NUM_TRIES"),
+        wait_min=constants.getattr("OF_MIN_WAIT_API"),
+        wait_max=constants.getattr("OF_MAX_WAIT_API"),
+        new_request_auth=True,
+    ) as c:
+        with c.requests(constants.getattr("INDIVIDUAL_TIMELINE").format(id)) as r:
+            log.trace(f"post raw individual {r.json()}")
+            return r.json()
 
 
 async def get_after(model_id, username, forced_after=None):
     if forced_after is not None:
         return forced_after
-    elif not settings.get_after_enabled():
-        return 0
-    elif read_args.retriveArgs().after == 0:
-        return 0
     elif read_args.retriveArgs().after:
         return read_args.retriveArgs().after.float_timestamp
+    elif read_args.retriveArgs().after == 0:
+        return 0
+    elif not settings.get_after_enabled():
+        return 0
     elif cache.get(f"{model_id}_full_timeline_scrape"):
         log.info(
             "Used --after previously. Scraping all timeline posts required to make sure content is not missing"
         )
         return 0
     curr = await operations.get_timeline_media(model_id=model_id, username=username)
     if len(curr) == 0:
-        log.debug("Setting date to zero because database is empty")
+        log.debug("Setting oldest date to zero because database is empty")
         return 0
-    missing_items = list(filter(lambda x: x.get("downloaded") != 1, curr))
     missing_items = list(
-        sorted(missing_items, key=lambda x: arrow.get(x.get("posted_at") or 0))
+        filter(lambda x: x.get("downloaded") != 1 and x.get("unlocked") != 0, curr)
     )
+    missing_items = list(sorted(missing_items, key=lambda x: arrow.get(x["posted_at"])))
     if len(missing_items) == 0:
-        log.debug("Using last db date because,all downloads in db marked as downloaded")
-        return await operations.get_last_timeline_date(
-            model_id=model_id, username=username
+        log.debug(
+            "Using using newest db date, because all downloads in db marked as downloaded"
         )
+        return arrow.get(
+            await operations.get_youngest_timeline_date(
+                model_id=model_id, username=username
+            )
+        ).float_timestamp
     else:
         log.debug(
-            f"Setting date slightly before earliest missing item\nbecause {len(missing_items)} posts in db are marked as undownloaded"
+            f"Setting date slightly before oldest missing item\nbecause {len(missing_items)} posts in db are marked as undownloaded"
         )
-        return arrow.get(missing_items[0]["posted_at"] or 0).float_timestamp
+        return arrow.get(missing_items[0]["posted_at"]).float_timestamp
 
 
 async def scrape_timeline_posts(
     c, model_id, job_progress=None, timestamp=None, required_ids=None, offset=False
 ) -> list:
     posts = None
-    attempt.set(0)
-    timestamp = float(timestamp) - 1000 if timestamp and offset else timestamp
+    timestamp = float(timestamp) - 100 if timestamp and offset else timestamp
 
-    if timestamp and (
-        float(timestamp)
-        > (read_args.retriveArgs().before or arrow.now()).float_timestamp
-    ):
-        return [], []
     url = (
         constants.getattr("timelineNextEP").format(model_id, str(timestamp))
         if timestamp
         else constants.getattr("timelineEP").format(model_id)
     )
     log.debug(url)
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            await sem.acquire()
-            await asyncio.sleep(1)
-            new_tasks = []
-            try:
-                attempt.set(attempt.get(0) + 1)
-                task = (
-                    job_progress.add_task(
-                        f"Attempt {attempt.get()}/{constants.getattr('NUM_TRIES')}: Timestamp -> {arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}",
-                        visible=True,
-                    )
-                    if job_progress
-                    else None
-                )
+    await asyncio.sleep(1)
+    new_tasks = []
+    try:
+        task = (
+            job_progress.add_task(
+                f"Timestamp -> {arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}",
+                visible=True,
+            )
+            if job_progress
+            else None
+        )
 
-                async with c.requests(url=url)() as r:
-                    if r.ok:
-                        posts = (await r.json_())["list"]
-                        log_id = f"timestamp:{arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}"
-                        if not posts:
-                            posts = []
-                        if len(posts) == 0:
-                            log.debug(f"{log_id} -> number of post found 0")
-
-                        elif len(posts) > 0:
-                            log.debug(f"{log_id} -> number of post found {len(posts)}")
-                            log.debug(
-                                f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}"
-                            )
-                            log.debug(
-                                f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}"
-                            )
-                            log.debug(
-                                f"{log_id} -> found postids {list(map(lambda x:x.get('id'),posts))}"
-                            )
-                            log.trace(
-                                "{log_id} -> post raw {posts}".format(
-                                    log_id=log_id,
-                                    posts="\n\n".join(
-                                        list(
-                                            map(
-                                                lambda x: f"scrapeinfo timeline: {str(x)}",
-                                                posts,
-                                            )
-                                        )
-                                    ),
-                                )
+        async with c.requests_async(url=url) as r:
+            posts = (await r.json_())["list"]
+            log_id = f"timestamp:{arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp!=None  else 'initial'}"
+            if not bool(posts):
+                log.debug(f"{log_id} -> no posts found")
+                return [], []
+
+            log.debug(f"{log_id} -> number of post found {len(posts)}")
+            log.debug(
+                f"{log_id} -> first date {arrow.get(posts[0].get('createdAt') or posts[0].get('postedAt')).format(constants.getattr('API_DATE_FORMAT'))}"
+            )
+            log.debug(
+                f"{log_id} -> last date {arrow.get(posts[-1].get('createdAt') or posts[-1].get('postedAt')).format(constants.getattr('API_DATE_FORMAT'))}"
+            )
+            log.debug(
+                f"{log_id} -> found postids {list(map(lambda x:x.get('id'),posts))}"
+            )
+            log.trace(
+                "{log_id} -> post raw {posts}".format(
+                    log_id=log_id,
+                    posts="\n\n".join(
+                        list(
+                            map(
+                                lambda x: f"scrapeinfo timeline: {str(x)}",
+                                posts,
                             )
-                            if not required_ids:
-                                new_tasks.append(
-                                    asyncio.create_task(
-                                        scrape_timeline_posts(
-                                            c,
-                                            model_id,
-                                            job_progress=job_progress,
-                                            timestamp=posts[-1]["postedAtPrecise"],
-                                            offset=False,
-                                        )
-                                    )
-                                )
-                            else:
-                                [
-                                    required_ids.discard(float(ele["postedAtPrecise"]))
-                                    for ele in posts
-                                ]
-                                if len(required_ids) > 0 and float(
-                                    (timestamp) or 0
-                                ) <= max(required_ids):
-                                    new_tasks.append(
-                                        asyncio.create_task(
-                                            scrape_timeline_posts(
-                                                c,
-                                                model_id,
-                                                job_progress=job_progress,
-                                                timestamp=posts[-1]["postedAtPrecise"],
-                                                required_ids=required_ids,
-                                                offset=False,
-                                            )
-                                        )
-                                    )
-                    else:
-                        log.debug(
-                            f"[bold]timeline response status code:[/bold]{r.status}"
                         )
-                        log.debug(f"[bold]timeline response:[/bold] {await r.text_()}")
-                        log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
-                        r.raise_for_status()
-            except Exception as E:
-                await asyncio.sleep(1)
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
+                    ),
+                )
+            )
 
-            finally:
-                sem.release()
-                (
-                    job_progress.remove_task(task)
-                    if job_progress and task != None
-                    else None
+            if not required_ids:
+                new_tasks.append(
+                    asyncio.create_task(
+                        scrape_timeline_posts(
+                            c,
+                            model_id,
+                            job_progress=job_progress,
+                            timestamp=posts[-1]["postedAtPrecise"],
+                            offset=False,
+                        )
+                    )
                 )
+
+            elif max(map(lambda x: float(x["postedAtPrecise"]), posts)) >= max(
+                required_ids
+            ):
+                pass
+            elif float(timestamp or 0) >= max(required_ids):
+                pass
+            else:
+                log.debug(f"{log_id} Required before {required_ids}")
+                [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
+                log.debug(f"{log_id} Required after {required_ids}")
+                if len(required_ids) > 0:
+                    new_tasks.append(
+                        asyncio.create_task(
+                            scrape_timeline_posts(
+                                c,
+                                model_id,
+                                job_progress=job_progress,
+                                timestamp=posts[-1]["postedAtPrecise"],
+                                required_ids=required_ids,
+                                offset=False,
+                            )
+                        )
+                    )
             return posts, new_tasks
+    except asyncio.TimeoutError:
+        raise Exception(f"Task timed out {url}")
+    except Exception as E:
+        await asyncio.sleep(1)
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
+    finally:
+        job_progress.remove_task(task) if job_progress and task != None else None
+
+
+def trace_log_task(responseArray):
+    chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
+    for i in range(1, len(responseArray) + 1, chunk_size):
+        # Calculate end index considering potential last chunk being smaller
+        end_index = min(
+            i + chunk_size - 1, len(responseArray)
+        )  # Adjust end_index calculation
+        chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
+        api_str = "\n\n".join(
+            map(lambda post: f"{common_logs.RAW_INNER} {post}\n\n", chunk)
+        )
+        log.trace(f"{common_logs.FINAL_RAW.format('Timeline')}".format(posts=api_str))
+        # Check if there are more elements remaining after this chunk
+        if i + chunk_size > len(responseArray):
+            break  # Exit the loop if we've processed all elements
+
+
+def trace_log_old(responseArray):
+    chunk_size = constants.getattr("LARGE_TRACE_CHUNK_SIZE")
+    for i in range(1, len(responseArray) + 1, chunk_size):
+        # Calculate end index considering potential last chunk being smaller
+        end_index = min(
+            i + chunk_size - 1, len(responseArray)
+        )  # Adjust end_index calculation
+        chunk = responseArray[i - 1 : end_index]  # Adjust slice to start at i-1
+        log.trace(
+            "oldtimelines {posts}".format(
+                posts="\n\n".join(list(map(lambda x: f"oldtimeline: {str(x)}", chunk)))
+            )
+        )
+        # Check if there are more elements remaining after this chunk
+        if i + chunk_size > len(responseArray):
+            break  # Exit the loop if we've processed all elements
+
+
+def after_log(username, after):
+    log.info(
+        f"""
+Setting initial timeline scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
+[yellow]Hint: append ' --after 2000' to command to force scan of all timeline posts + download of new files only[/yellow]
+[yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all timeline posts + download/re-download of all files[/yellow]
+
+            """
+    )
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/classes/base.py` & `ofscraper-3.9.1/ofscraper/classes/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,18 +29,19 @@
             splitArray = wordarray[: length + 1]
             text = f"{''.join(splitArray)}"
         text = re.sub(" +$", "", text)
         return text
 
     def file_cleanup(self, text, mediatype=None):
         text = str(text)
+        text = re.sub("<[^>]*>", "", text)
         text = re.sub('[\n<>:"/\|?*:;]+', "", text)
         text = re.sub("-+", "_", text)
         text = re.sub(" +", " ", text)
         text = re.sub(" ", data.get_spacereplacer(mediatype=mediatype), text)
         return text
 
     def db_cleanup(self, string):
-        text = str(text)
         string = re.sub("<[^>]*>", "", string)
         string = " ".join(string.split())
         string = BeautifulSoup(string, html_parser).get_text()
+        return string
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/classes/labels.py` & `ofscraper-3.9.1/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/classes/media.py` & `ofscraper-3.9.1/ofscraper/classes/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,44 @@
+import asyncio
 import logging
 import re
 import string
 
 # supress warnings
 import warnings
 
 import arrow
 from bs4 import MarkupResemblesLocatorWarning
 from mpegdash.parser import MPEGDASHParser
-from tenacity import (
-    AsyncRetrying,
-    retry,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random,
-)
 
 import ofscraper.classes.base as base
-import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.args.quality as quality
 import ofscraper.utils.config.data as data
 import ofscraper.utils.constants as constants
+import ofscraper.utils.dates as dates
 import ofscraper.utils.logs.helpers as log_helpers
 
 warnings.filterwarnings("ignore", category=MarkupResemblesLocatorWarning)
 
 
 log = logging.getLogger("shared")
 
+semaphore = asyncio.Semaphore(constants.getattr("MPD_MAX_SEMS"))
+
 
 class Media(base.base):
     def __init__(self, media, count, post):
         super().__init__()
         self._media = media
         self._count = count
         self._post = post
         self._final_url = None
         self._cached_parse_mpd = None
+        self._mpd=None
 
     def __eq__(self, other):
         return self.postid == other.postid
 
     @property
     def expires(self):
         return self._post.expires
@@ -65,22 +63,22 @@
             return "videos"
         elif self._media["type"] == "forced_skipped":
             return "forced_skipped"
         else:
             return f"{self._media['type']}s".lower()
 
     @property
-    def length(self):
+    def duration(self):
         return self._media.get("duration") or self.media_source.get("duration")
 
     @property
-    def numeric_length(self):
-        if not self.length:
+    def numeric_duration(self):
+        if not self.duration:
             return "N/A"
-        return str((arrow.get(self.length) - arrow.get(0)))
+        return str((arrow.get(self.duration) - arrow.get(0)))
 
     @property
     def url(self):
         if self.protected == True:
             return None
         elif self._final_url:
             None
@@ -109,19 +107,18 @@
     # ID for use in dynamic names
     @property
     def file_postid(self):
         return self._post._post["id"]
 
     @property
     def canview(self):
-        return (
-            self._media.get("canView") or True
-            if (self.url or self.mpd) != None
-            else False
-        )
+        # profiles are always viewable
+        if self.responsetype.lower() == "profile":
+            return True
+        return self._media.get("canView") if (self.url or self.mpd) != None else False
 
     @property
     def label(self):
         return self._post.label
 
     # used for placeholder
     @property
@@ -181,15 +178,17 @@
 
     @property
     def text(self):
         return self._post.text
 
     @property
     def mpd(self):
-        if self.protected == False:
+        if self._mpd:
+            return self._mpd
+        elif self.protected == False:
             return None
         return (
             self._media.get("files", {}).get("drm", {}).get("manifest", {}).get("dash")
         )
 
     @property
     def policy(self):
@@ -266,32 +265,32 @@
                 .split("/")[-1]
                 .strip("/,.;!_-@#$%^&*()+\\ "),
             )
             return f"{filename}_{arrow.get(self.date).format(data.get_date(mediatype=self.mediatype))}"
 
     @property
     async def final_filename(self):
-        filename = self.filename or self.id
+        filename = self.filename or str(self.id)
         if self.mediatype == "videos":
             filename = re.sub("_[a-z0-9]+$", f"", filename)
-            filename = f"{filename}_{await self.selected_quality}"
+            filename = f"{filename}_{await self.selected_quality_placeholder}"
         # cleanup
         try:
             filename = self.file_cleanup(filename)
             filename = re.sub(
                 " ", data.get_spacereplacer(mediatype=self.mediatype), filename
             )
 
         except Exception as E:
             print(E)
         return filename
 
     @property
     def no_quality_final_filename(self):
-        filename = self.filename or self.id
+        filename = self.filename or str(self.id)
         if self.mediatype == "videos":
             filename = re.sub("_[a-z]+", f"", filename)
         # cleanup
         try:
             filename = self.file_cleanup(filename)
             filename = re.sub(
                 " ", data.get_spacereplacer(mediatype=self.mediatype), filename
@@ -322,30 +321,24 @@
         if not self.mpd:
             return
         params = {
             "Policy": self.policy,
             "Key-Pair-Id": self.keypair,
             "Signature": self.signature,
         }
-        async with sessionbuilder.sessionBuilder() as c:
-            async for _ in AsyncRetrying(
-                retry=retry_if_not_exception_type(KeyboardInterrupt),
-                stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-                wait=wait_random(
-                    min=constants.getattr("OF_MIN"),
-                    max=constants.getattr("OF_MAX"),
-                ),
-                reraise=True,
-            ):
-                with _:
-                    async with c.requests(url=self.mpd, params=params)() as r:
-                        if not r.ok:
-                            r.raise_for_status()
-                        self._cached_parse_mpd = MPEGDASHParser.parse(await r.text_())
-                        return self._cached_parse_mpd
+        async with sessionManager.sessionManager(
+            retries=constants.getattr("MPD_NUM_TRIES"),
+            wait_min=constants.getattr("OF_MIN_WAIT_API"),
+            wait_max=constants.getattr("OF_MAX_WAIT_API"),
+            new_request_auth=True,
+            semaphore=semaphore,
+        ) as c:
+            async with c.requests_async(url=self.mpd, params=params) as r:
+                self._cached_parse_mpd = MPEGDASHParser.parse(await r.text_())
+                return self._cached_parse_mpd
 
     @property
     async def mpd_dict(self):
         if not self.mpd:
             return
         mpd = await self.parse_mpd
         video = await self.mpd_video_helper(mpd=mpd)
@@ -367,21 +360,33 @@
     def mass(self):
         return self._post.mass
 
     @mediatype.setter
     def mediatype(self, val):
         self._media["type"] = val
 
+    @url.setter
+    def url(self, val):
+        self._final_url=val
+    @mpd.setter
+    def mpd(self, val):
+        self._mpd=val
     @property
     async def selected_quality(self):
         if self.protected == False:
             return self.normal_quality_helper()
         return await self.alt_quality_helper()
 
     @property
+    async def selected_quality_placeholder(self):
+        return await self.selected_quality or constants.getattr(
+            "QUALITY_UNKNOWN_DEFAULT"
+        )
+
+    @property
     def protected(self):
         if self.mediatype not in {"videos", "texts"}:
             return False
         elif bool(self.media_source.get("source")):
             return False
         elif bool(self.files_source):
             return False
@@ -410,14 +415,18 @@
     def username(self):
         return self._post.username
 
     @property
     def model_id(self):
         return self._post.model_id
 
+    @property
+    def duration_string(self):
+        return dates.format_seconds(self.duration) if self.duration else None
+
     def get_text(self):
         if self.responsetype != "Profile":
             text = (
                 self._post.file_sanitized_text
                 or self.filename
                 or arrow.get(self.date).format(data.get_date(mediatype=self.mediatype))
             )
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/classes/models.py` & `ofscraper-3.9.1/ofscraper/classes/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         else:
             return self.subscribed_data.get("expiredAt") or self.subscribed_expired_date
 
     @property
     def final_expired(self):
         if not self.expired:
             return 0
-        return self.expired
+        return arrow.get(self.expired).float_timestamp
 
     """
     Best values to retrive depends on how many times subscribed
 
     """
 
     @property
@@ -174,18 +174,18 @@
         elif self.regular_price is not None:
             return self.regular_price
         else:
             return 0
 
     @property
     def final_regular_price(self):
-        if self.regular_price is not None:
-            return self.regular_price
-        else:
-            return 0
+        if self.subscribed_data:
+            return self.subscribed_data.get("regularPrice")
+        elif self.model:
+            return self.model.get("subscribePrice")
 
     @property
     def final_promo_price(self):
         if self.lowest_promo_all is not None:
             return self.lowest_promo_all
         elif self.regular_price is not None:
             return self.regular_price
@@ -197,17 +197,17 @@
         if last_seen:
             return arrow.get(last_seen).format(FORMAT)
 
     @property
     def final_last_seen(self):
         last_seen = self._model.get("lastSeen")
         if not last_seen:
-            return arrow.now()
+            return arrow.now().float_timestamp
         else:
-            return arrow.get(last_seen)
+            return arrow.get(last_seen).float_timestamp
 
     @property
     def renewed_string(self):
         if not self.renewed:
             return None
         return arrow.get(self.renewed).format(FORMAT)
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/classes/multiprocessprogress.py` & `ofscraper-3.9.1/ofscraper/classes/multiprocessprogress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/classes/placeholder.py` & `ofscraper-3.9.1/ofscraper/classes/placeholder.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
             }
         )
         self._variables.update({"model_username": username})
         self._variables.update({"response_type": ele.modified_responsetype})
         self._variables.update({"label": ele.label_string})
         self._variables.update({"download_type": ele.downloadtype})
         self._variables.update({"modelObj": selector.get_model_fromParsed(username)})
-        self._variables.update({"quality": await ele.selected_quality})
+        self._variables.update({"quality": await ele.selected_quality_placeholder})
         self._variables.update({"file_name": await ele.final_filename})
         self._variables.update({"original_filename": ele.filename})
         self._variables.update({"only_file_name": ele.no_quality_final_filename})
         self._variables.update({"only_filename": ele.no_quality_final_filename})
         self._variables.update({"text": ele.file_text})
         self._variables.update({"config": config_file.open_config()})
         self._variables.update({"args": read_args.retriveArgs()})
@@ -337,15 +337,17 @@
             out = data.get_fileformat(mediatype=ele.mediatype).format(**self._variables)
         out = self._addcount(ele, out)
         log.debug(f"final filename path {out}")
         self._filename = out
         return out
 
     def _addcount(self, ele, out):
-        if not ele.needs_count:
+        if not constants.getattr("FILE_COUNT_PLACEHOLDER"):
+            return
+        elif not ele.needs_count:
             return out
         out = re.sub(" $", "", out)
         # insert count
         if re.search(r"\.(?:[a-zA-Z0-9]+)$", out):
             out = re.sub(r"(\.(?!\.))", f"_{ele.count}.", out)
         else:
             out = f"{out}_{ele.count}"
@@ -508,15 +510,15 @@
         ext = self._ext
         username = ele.username
         model_id = ele.model_id
         self._variables.update({"ext": ext})
         await self.add_common_variables(ele, username, model_id)
         globals().update(self._variables)
         log.trace(
-            f"modelid:{model_id}  filename placeholders {list(filter(lambda x:x[0] in set(list(self._variables.keys())),list(locals().items())))}"
+            f"modelid:{model_id}  filename placeholders {filter(lambda x:x[0] in set(list(self._variables.keys())),list(locals().items()))}"
         )
         out = None
         if ele.responsetype == "profile":
             text = ele.file_sanitized_text
             text = re.sub(" ", data.get_spacereplacer(mediatype="Text"), text)
             out = f"{text}.{ext}"
         elif data.get_allow_code_execution():
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/classes/posts.py` & `ofscraper-3.9.1/ofscraper/classes/posts.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     @property
     def responsetype(self):
         if self._responsetype:
             return self._responsetype
         elif self.pinned:
             return "pinned"
         elif self.archived:
-            return "self.archived"
+            return "archived"
         elif self.post.get("responseType") == "post":
             return "timeline"
         return self.post.get("responseType")
 
     @property
     def modified_responsetype(self):
         return self.modified_response_helper()
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/classes/table.py` & `ofscraper-3.9.1/ofscraper/classes/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/commands/manual.py` & `ofscraper-3.9.1/ofscraper/commands/manual.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,135 +1,182 @@
 import logging
 import re
+import traceback
 
 import ofscraper.api.highlights as highlights_
 import ofscraper.api.messages as messages_
 import ofscraper.api.paid as paid
 import ofscraper.api.profile as profile
 import ofscraper.api.timeline as timeline
 import ofscraper.classes.media as media_
 import ofscraper.classes.posts as posts_
-import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.db.operations as operations
 import ofscraper.download.download as download
 import ofscraper.models.selector as selector
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.args.write as write_args
 import ofscraper.utils.constants as constants
+import ofscraper.utils.context.stdout as stdout
 import ofscraper.utils.system.network as network
-import ofscraper.utils.args.user as user_helper
 from ofscraper.utils.context.run_async import run
 
 
 def manual_download(urls=None):
     log = logging.getLogger("shared")
-    network.check_cdm()
-    allow_manual_dupes()
-    url_dicts = process_urls(urls)
-    all_media=[item for media_list in url_dicts.values() for item in media_list.get("media_list", [])]
-    all_posts=[item for post_list in url_dicts.values() for item in post_list.get("post_list", [])]
-    log.debug(f"Number of values from media dict  {len(all_media)}")
-    log.debug(f"Number of values from post dict  {len(all_posts)}")
-    if len(all_media)==0 and len(all_posts)==0:
-        return
-    set_user_data(url_dicts)
-    for _,value in url_dicts.items():
-        model_id = value.get("model_id")
-        username = value.get("username")
-        model_id = value.get("model_id")
-        username = value.get("username")
-        log.info(f"Downloading individual media for {username}")
-        operations.table_init_create(model_id=model_id, username=username)
-        operations.make_changes_to_content_tables(value.get("post_list",[]),model_id=model_id,username=username)
-        download.download_process(username, model_id, value.get("media_list",[]), posts=None)
-        operations.batch_mediainsert(value.get("media_list"),username=username,model_id=model_id)
+    with stdout.lowstdout():
+        try:
+            network.check_cdm()
+            allow_manual_dupes()
+            url_dicts = process_urls(urls)
+            all_media = [
+                item
+                for media_list in url_dicts.values()
+                for item in media_list.get("media_list", [])
+            ]
+            all_posts = [
+                item
+                for post_list in url_dicts.values()
+                for item in post_list.get("post_list", [])
+            ]
+            log.debug(f"Number of values from media dict  {len(all_media)}")
+            log.debug(f"Number of values from post dict  {len(all_posts)}")
+            if len(all_media) == 0 and len(all_posts) == 0:
+                return
+            set_user_data(url_dicts)
+            for _, value in url_dicts.items():
+                model_id = value.get("model_id")
+                username = value.get("username")
+                model_id = value.get("model_id")
+                username = value.get("username")
+                log.info(f"Downloading individual media for {username}")
+                operations.table_init_create(model_id=model_id, username=username)
+                operations.make_changes_to_content_tables(
+                    value.get("post_list", []), model_id=model_id, username=username
+                )
+                download.download_process(
+                    username, model_id, value.get("media_list", []), posts=None
+                )
+                operations.batch_mediainsert(
+                    value.get("media_list"), username=username, model_id=model_id
+                )
+        except Exception as e:
+            log.traceback_(e)
+            log.traceback_(traceback.format_exc())
+            raise e
 
 
 def allow_manual_dupes():
     args = read_args.retriveArgs()
     args.force_all = True
     write_args.setArgs(args)
 
 
 def set_user_data(url_dicts):
-    user_helper.set_users_arg([nested_dict.get("username") for nested_dict in url_dicts.values()])
-    selector.all_subs_helper()
+    selector.set_data_all_subs_dict(
+        [nested_dict.get("username") for nested_dict in url_dicts.values()]
+    )
+
 
 def process_urls(urls):
-    out_dict={}
+    out_dict = {}
 
     for url in url_helper(urls):
         response = get_info(url)
         model = response[0]
         postid = response[1]
         type = response[2]
-        if type == "post":  
-            user_data=profile.scrape_profile(model)
+        if type == "post":
+            user_data = profile.scrape_profile(model)
             model_id = user_data.get("id")
-            username= user_data.get("username")
-            out_dict.setdefault(model_id, {})["model_id"]= model_id
-            out_dict.setdefault(model_id, {})["username"]= username
+            username = user_data.get("username")
+            out_dict.setdefault(model_id, {})["model_id"] = model_id
+            out_dict.setdefault(model_id, {})["username"] = username
 
             value = timeline.get_individual_post(postid)
 
-            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(get_all_media(postid, model_id, value))
-            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(get_post_item(model_id, value))
+            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(
+                get_all_media(postid, model_id, value)
+            )
+            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(
+                get_post_item(model_id, value)
+            )
         elif type == "msg":
-            user_data=profile.scrape_profile(model).get("username")
+            user_data = profile.scrape_profile(model)
             model_id = user_data.get("id")
-            username= user_data.get("username")
-            out_dict.setdefault(model_id, {})["model_id"]= model_id
-            out_dict.setdefault(model_id, {})["username"]= username
-            
+            username = user_data.get("username")
+            out_dict.setdefault(model_id, {})["model_id"] = model_id
+            out_dict.setdefault(model_id, {})["username"] = username
+
             value = messages_.get_individual_post(model_id, postid)
-            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(get_all_media(postid, model_id, value))
-            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(get_post_item(model_id, value))
+            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(
+                get_all_media(postid, model_id, value)
+            )
+            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(
+                get_post_item(model_id, value)
+            )
         elif type == "msg2":
-            user_data=profile.scrape_profile(model)
-            username= user_data.get("username")
-            model_id=user_data.get("id")
-            out_dict.setdefault(model_id, {})["model_id"]= model_id
-            out_dict.setdefault(model_id, {})["username"]= username
+            user_data = profile.scrape_profile(model)
+            username = user_data.get("username")
+            model_id = user_data.get("id")
+            out_dict.setdefault(model_id, {})["model_id"] = model_id
+            out_dict.setdefault(model_id, {})["username"] = username
 
             value = messages_.get_individual_post(model_id, postid)
-            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(get_all_media(postid, model_id, value))
-            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(get_post_item(model_id, value))
+            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(
+                get_all_media(postid, model_id, value)
+            )
+            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(
+                get_post_item(model_id, value)
+            )
         elif type == "unknown":
             value = unknown_type_helper(postid) or {}
             model_id = value.get("author", {}).get("id")
             if not model_id:
                 continue
-            username=profile.scrape_profile(model_id).get("username")
-            out_dict.setdefault(model_id, {})["model_id"]= model_id
-            out_dict.setdefault(model_id, {})["username"]= username
-
-            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(get_all_media(postid, model_id, value))
-            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(get_post_item(model_id, value))
+            username = profile.scrape_profile(model_id).get("username")
+            out_dict.setdefault(model_id, {})["model_id"] = model_id
+            out_dict.setdefault(model_id, {})["username"] = username
+
+            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(
+                get_all_media(postid, model_id, value)
+            )
+            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(
+                get_post_item(model_id, value)
+            )
         elif type == "highlights":
             value = highlights_.get_individual_highlights(postid) or {}
             model_id = value.get("userId")
             if not model_id:
                 continue
-            username= profile.scrape_profile(model_id).get("username")
-            out_dict.setdefault(model_id, {})["model_id"]= model_id
-            out_dict.setdefault(model_id, {})["username"]= username
-
-            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(get_all_media(postid, model_id, value,responsetype="highlights"))
-            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(get_post_item(model_id, value,responsetype="highlights"))
+            username = profile.scrape_profile(model_id).get("username")
+            out_dict.setdefault(model_id, {})["model_id"] = model_id
+            out_dict.setdefault(model_id, {})["username"] = username
+
+            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(
+                get_all_media(postid, model_id, value, responsetype="highlights")
+            )
+            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(
+                get_post_item(model_id, value, responsetype="highlights")
+            )
             # special case
         elif type == "stories":
             value = highlights_.get_individual_stories(postid) or {}
             model_id = value.get("userId")
             if not model_id:
                 continue
-            username= profile.scrape_profile(model_id).get("username")
-            out_dict.setdefault(model_id, {})["model_id"]= model_id
-            out_dict.setdefault(model_id, {})["username"]= username
-            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(get_all_media(postid, model_id, value,responsetype="stories"))
-            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(get_post_item(model_id, value,responsetype="stories"))
+            username = profile.scrape_profile(model_id).get("username")
+            out_dict.setdefault(model_id, {})["model_id"] = model_id
+            out_dict.setdefault(model_id, {})["username"] = username
+            out_dict.setdefault(model_id, {}).setdefault("media_list", []).extend(
+                get_all_media(postid, model_id, value, responsetype="stories")
+            )
+            out_dict.setdefault(model_id, {}).setdefault("post_list", []).extend(
+                get_post_item(model_id, value, responsetype="stories")
+            )
             # special case
     return out_dict
 
 
 def unknown_type_helper(postid):
     return timeline.get_individual_post(postid)
 
@@ -138,15 +185,15 @@
     if value == None:
         return []
     user_name = profile.scrape_profile(model_id)["username"]
     post = posts_.Post(value, model_id, user_name, responsetype=responsetype)
     return [post]
 
 
-def get_all_media(posts_id, model_id, value,responsetype=None):
+def get_all_media(posts_id, model_id, value, responsetype=None):
     value = value or {}
     media = []
     if model_id == None:
         return {}
     user_name = profile.scrape_profile(model_id)["username"]
     post_item = posts_.Post(value, model_id, user_name, responsetype=responsetype)
     media = post_item.media
@@ -157,21 +204,29 @@
             media,
         )
     )
     if len(media) == 0:
         media.extend(paid_failback(posts_id, model_id, user_name))
     return media
 
+
 @run
 async def paid_failback(post_id, model_id, username):
     logging.getLogger("shared").debug(
         "Using failback search because query return 0 media"
     )
     post_id = str(post_id)
-    async with sessionbuilder.sessionBuilder(backend="httpx") as c:
+    async with sessionManager.sessionManager(
+        backend="httpx",
+        sem=constants.getattr("API_REQ_CHECK_MAX"),
+        retries=constants.getattr("API_CHECK_NUM_TRIES"),
+        wait_min=constants.getattr("OF_MIN_WAIT_API"),
+        wait_max=constants.getattr("OF_MAX_WAIT_API"),
+        new_request_auth=True,
+    ) as c:
         data = await paid.get_paid_posts(id, username, c=c) or []
         posts = list(
             map(lambda x: posts_.Post(x, model_id, username, responsetype="paid"), data)
         )
         output = []
         [output.extend(post.media) for post in posts]
         return list(
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/commands/scraper.py` & `ofscraper-3.9.1/ofscraper/commands/scraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import ofscraper.utils.console as console
 import ofscraper.utils.context.exit as exit
 import ofscraper.utils.context.stdout as stdout
 import ofscraper.utils.menu as menu
 import ofscraper.utils.paths.paths as paths
 import ofscraper.utils.run as run
 import ofscraper.utils.system.network as network
+from ofscraper.__version__ import __version__
 
 log = logging.getLogger("shared")
 
 
 def process_selected_areas():
     log.debug(f"[bold blue] Running Action Mode [/bold blue]")
     functs = process_actions.add_selected_areas()
@@ -65,15 +66,15 @@
         elif prompts.continue_prompt() == "No":
             break
 
 
 def print_start():
     with stdout.lowstdout():
         console.get_shared_console().print(
-            f"[bold green]Version {read_args.retriveArgs().version}[/bold green]"
+            f"[bold green]Version {__version__}[/bold green]"
         )
 
 
 def main():
     try:
         print_start()
         paths.temp_cleanup()
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/const/config.py` & `ofscraper-3.9.1/ofscraper/const/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 DIR_FORMAT_DEFAULT = "{model_username}/{responsetype}/{mediatype}/"
 FILE_FORMAT_DEFAULT = "{filename}.{ext}"
 METADATA_DEFAULT = "{configpath}/{profile}/.data/{model_username}_{model_id}"
 FILE_SIZE_LIMIT_DEFAULT = 0
 FILE_SIZE_MIN_DEFAULT = 0
 TEXTLENGTH_DEFAULT = 0
 SPACE_REPLACER_DEFAULT = " "
+PROGRESS_DEFAULT = False
 FILTER_DEFAULT = ["Images", "Audios", "Videos"]
 SAVE_PATH_DEFAULT = str(pathlib.Path.home() / "Data/ofscraper")
 DATE_DEFAULT = "MM-DD-YYYY"
 PROFILE_DEFAULT = "main_profile"
 PREMIUM_DEFAULT = "Premium"
 KEYDB_DEFAULT = ""
 MP4DECRYPT_DEFAULT = ""
@@ -39,19 +40,21 @@
     "stories": "Stories",
     "highlights": "Stories",
     "profile": "Profile",
     "pinned": "Posts",
 }
 SYSTEM_FREEMIN_DEFAULT = 0
 AVATAR_DEFAULT = True
-PROGRESS_DEFAULT = False
+havROGRESS_DEFAULT = False
 KEYDB_DEFAULT = ""
 CODE_EXECUTION_DEFAULT = False
 INFINITE_LOOP_DEFAULT = False
 DISABLE_AFTER_DEFAULT = False
 DEFAULT_USER_LIST = "main"
 DEFAULT_BLACK_LIST = ""
 HASHED_DEFAULT = False
 EMPTY_MEDIA_DEFAULT = {}
 DEFAULT_LOG_LEVEL = "DEBUG"
 INCLUDE_LABELS_ALL = False
 DISCORD_THREAD_OVERRIDE = False
+USE_CACHE_KEY = True
+POST_SCRIPT_DEFAULT = None
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/const/constants.py` & `ofscraper-3.9.1/ofscraper/const/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,13 +11,14 @@
 from ofscraper.const.binary import *
 from ofscraper.const.config import *
 from ofscraper.const.date import *
 from ofscraper.const.download import *
 from ofscraper.const.files import *
 from ofscraper.const.general import *
 from ofscraper.const.logger import *
+from ofscraper.const.metadata import *
 from ofscraper.const.other_url import *
 from ofscraper.const.prompts import *
 from ofscraper.const.req import *
 from ofscraper.const.test_constants import *
 from ofscraper.const.time import *
 from ofscraper.const.url import *
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/const/general.py` & `ofscraper-3.9.1/ofscraper/const/general.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,7 +19,10 @@
 CONTINUE_BOOL = True
 WINDOWS_MAX_PATH = 255
 MAC_MAX_PATH = 255
 LINUX_MAX_FILE = 254
 BUF_SIZE = 1000000
 MAX_TEXT_LENGTH = 70
 MAX_TEXT_WORKER = 30
+FILE_COUNT_PLACEHOLDER = True
+DELETED_MODEL_PLACEHOLDER = "modeldeleted"
+LARGE_TRACE_CHUNK_SIZE = 100
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/const/prompts.py` & `ofscraper-3.9.1/ofscraper/const/prompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 mainPromptChoices = {
     "Perform Action(s)": "action",
     "Edit auth.json file": "auth",
     "Edit config.json file": "config",
     "Edit Profile": "profile",
+    "Merge Databases":"merge",
     "Quit": "quit",
 }
 
 configPromptChoices = {
     "General Options": "general",
     "File Options": "file",
     "Download Options": "download",
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/const/test_constants.py` & `ofscraper-3.9.1/ofscraper/const/test_constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/const/url.py` & `ofscraper-3.9.1/ofscraper/const/url.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 postURL = "https://onlyfans.com/{}/{}"
 
 DIGITALCRIMINALS = (
     "https://raw.githubusercontent.com/DATAHOARDERS/dynamic-rules/main/onlyfans.json"
 )
 
 DEVIINT = "https://raw.githubusercontent.com/deviint/onlyfans-dynamic-rules/main/dynamicRules.json"
+SNEAKY = "https://raw.githubusercontent.com/SneakyOvis/onlyfans-dynamic-rules/main/rules.json"
+
 donateEP = "https://www.buymeacoffee.com/excludedBittern"
 
 purchased_contentEP = "https://onlyfans.com/api2/v2/posts/paid?limit=100&skip_users=all&format=infinite&offset={}&user_id={}"
 purchased_contentALL = "https://onlyfans.com/api2/v2/posts/paid?limit=100&skip_users=all&format=infinite&offset={}"
 
 highlightSPECIFIC = "https://onlyfans.com/api2/v2/stories/highlights/{}"
 storiesSPECIFIC = "https://onlyfans.com/api2/v2/stories/{}"
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/db/operations_/labels.py` & `ofscraper-3.9.1/ofscraper/db/operations_/labels.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,22 +13,20 @@
 
 import contextlib
 import logging
 import sqlite3
 
 from rich.console import Console
 
+import ofscraper.classes.labels as labels_class
 import ofscraper.db.operations_.helpers as helpers
+import ofscraper.db.operations_.posts as post_
 import ofscraper.db.operations_.wrapper as wrapper
 import ofscraper.utils.args.read as read_args
-from ofscraper.db.operations_.profile import get_single_model
-import ofscraper.db.operations_.posts as post_
-import ofscraper.classes.labels as labels_class
-
-
+from ofscraper.db.operations_.profile import get_single_model_via_profile
 
 console = Console()
 log = logging.getLogger("shared")
 labelsCreate = """
 CREATE TABLE IF NOT EXISTS labels (
 	id INTEGER NOT NULL, 
     label_id INTEGER,
@@ -48,15 +46,15 @@
 labelUpdate = """Update 'labels'
 SET label_id=?,name=?,type=?,post_id=?,model_id=?
 WHERE label_id=(?) and model_id=(?) and post_id=(?);"""
 labelPostsID = """
 SELECT post_id  FROM  labels where model_id=(?) and label_id=(?)
 """
 
-labelALLTransition = """
+labelSelectTransition = """
 SELECT
     CASE WHEN EXISTS (SELECT 1 FROM pragma_table_info('labels') WHERE name = 'label_id')
         THEN label_id
         ELSE id
     END AS label_id,
         CASE WHEN EXISTS (SELECT 1 FROM pragma_table_info('labels') WHERE name = 'model_id')
         THEN model_id
@@ -67,23 +65,25 @@
 """
 labelDrop = """
 drop table labels;
 """
 
 
 @wrapper.operation_wrapper_async
-def create_labels_table(model_id=None, username=None, conn=None):
+def create_labels_table(
+    model_id=None, username=None, conn=None, db_path=None, **kwargs
+):
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(labelsCreate)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def write_labels_table(
-    label: dict, posts: dict, model_id=None, username=None, conn=None
+    label: dict, posts: dict, model_id=None, username=None, conn=None, **kwargs
 ):
     with contextlib.closing(conn.cursor()) as curr:
         insertData = list(
             map(
                 lambda post: (
                     label.label_id,
                     label.name,
@@ -96,15 +96,15 @@
         )
         curr.executemany(labelInsert, insertData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def update_labels_table(
-    label: dict, posts: dict, model_id=None, username=None, conn=None
+    label: dict, posts: dict, model_id=None, username=None, conn=None, **kwargs
 ):
     with contextlib.closing(conn.cursor()) as curr:
         insertData = list(
             map(
                 lambda post: (
                     label.label_id,
                     label.name,
@@ -120,25 +120,25 @@
         )
         curr.executemany(labelUpdate, insertData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def write_labels_table_transition(
-    inputData: list, model_id=None, username=None, conn=None
+    inputData: list, model_id=None, username=None, conn=None, **kwargs
 ):
     with contextlib.closing(conn.cursor()) as curr:
         ordered_keys = ["label_id", "name", "type", "post_id", "model_id"]
         insertData = [tuple([data[key] for key in ordered_keys]) for data in inputData]
         curr.executemany(labelInsert, insertData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def get_all_labels_posts(label, model_id=None, username=None, conn=None):
+def get_all_labels_posts(label, model_id=None, username=None, conn=None, **kwargs):
     with contextlib.closing(conn.cursor()) as curr:
         curr.execute(labelPostsID, [model_id, label.label_id])
         return [dict(row)["post_id"] for row in curr.fetchall()]
 
 
 @wrapper.operation_wrapper_async
 def add_column_labels_ID(conn=None, **kwargs):
@@ -156,23 +156,23 @@
             conn.commit()
         except sqlite3.Error as e:
             conn.rollback()
             raise e  # Raise the error for handling
 
 
 @wrapper.operation_wrapper_async
-def drop_labels_table(model_id=None, username=None, conn=None) -> list:
+def drop_labels_table(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(labelDrop)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def get_all_labels_transition(
-    model_id=None, username=None, conn=None, database_model=None
+    model_id=None, username=None, conn=None, database_model=None, **kwargs
 ) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         # Check for column existence (label_id)
         cur.execute("PRAGMA table_info('labels')")
         columns = [row[1] for row in cur.fetchall()]  # Get column names
 
         # Build SELECT clause dynamically
@@ -195,36 +195,60 @@
                 label_id=row.get("label_id") or row.get("id"),
                 model_id=row.get("model_id") or database_model,
             )
             for row in data
         ]
 
 
-async def modify_unique_constriant_labels(model_id=None, username=None):
-    database_model = get_single_model(model_id=model_id, username=username)
+async def modify_unique_constriant_labels(
+    model_id=None, username=None, db_path=None, **kwargs
+):
+    database_model = get_single_model_via_profile(
+        model_id=model_id, username=username, db_path=db_path
+    )
     data = await get_all_labels_transition(
-        model_id=model_id, username=username, database_model=database_model
+        model_id=model_id,
+        username=username,
+        database_model=database_model,
+        db_path=db_path,
+    )
+    await drop_labels_table(model_id=model_id, username=username, db_path=db_path)
+    await create_labels_table(model_id=model_id, username=username, db_path=db_path)
+    await write_labels_table_transition(
+        data, model_id=model_id, username=username, db_path=db_path
     )
-    await drop_labels_table(model_id=model_id, username=username)
-    await create_labels_table(model_id=model_id, username=username)
-    await write_labels_table_transition(data, model_id=model_id, username=username)
 
 
-async def make_label_table_changes(labels, model_id=None, username=None,posts=True):
+async def make_label_table_changes(
+    labels, model_id=None, username=None, posts=True, **kwargs
+):
     labels = list(
-                map(lambda x: labels_class.Label(x, model_id, username) if not isinstance(x,labels_class.Label) else x , labels)
+        map(
+            lambda x: (
+                labels_class.Label(x, model_id, username)
+                if not isinstance(x, labels_class.Label)
+                else x
+            ),
+            labels,
+        )
     )
     for label in labels:
-        curr = set(await get_all_labels_posts(label, model_id=model_id, username=username))
+        curr = set(
+            await get_all_labels_posts(label, model_id=model_id, username=username)
+        )
         new_posts = list(filter(lambda x: x.id not in curr, label.posts))
         curr_posts = list(filter(lambda x: x.id in curr, label.posts))
         if len(new_posts) > 0:
             new_posts = helpers.converthelper(new_posts)
-            await write_labels_table(label, new_posts, model_id=model_id, username=username)
+            await write_labels_table(
+                label, new_posts, model_id=model_id, username=username
+            )
         if read_args.retriveArgs().metadata and len(curr_posts) > 0:
             curr_posts = helpers.converthelper(curr_posts)
             await update_labels_table(
                 label, curr_posts, model_id=model_id, username=username
             )
     if posts:
         all_posts = [post for label in labels for post in label.posts]
-        await post_.make_post_table_changes(all_posts, model_id=model_id, username=username)
+        await post_.make_post_table_changes(
+            all_posts, model_id=model_id, username=username
+        )
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/db/operations_/media.py` & `ofscraper-3.9.1/ofscraper/db/operations_/media.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pathlib
 import sqlite3
 
 import arrow
 from rich.console import Console
 
 import ofscraper.db.operations_.wrapper as wrapper
-from ofscraper.db.operations_.profile import get_single_model
+from ofscraper.db.operations_.profile import get_single_model_via_profile
 from ofscraper.utils.context.run_async import run
 
 console = Console()
 log = logging.getLogger("shared")
 
 mediaCreate = """
 CREATE TABLE IF NOT EXISTS medias (
@@ -39,34 +39,48 @@
 	api_type VARCHAR, 
 	media_type VARCHAR, 
 	preview INTEGER, 
 	linked VARCHAR, 
 	downloaded INTEGER, 
 	created_at TIMESTAMP, 
     posted_at TIMESTAMP,
+    duration VARCHAR,
+    unlocked BOOL,
 	hash VARCHAR,
     model_id INTEGER,
 	PRIMARY KEY (id), 
 	UNIQUE (media_id,model_id)
 );"""
-mediaALLTransition = """
+mediaSelectTransition = """
 SELECT  media_id,post_id,link,directory,filename,size,api_type,
-media_type,preview,linked,downloaded,created_at,posted_at,hash,
+media_type,preview,linked,downloaded,created_at,unlocked,
        CASE WHEN EXISTS (SELECT 1 FROM pragma_table_info('medias') WHERE name = 'model_id')
             THEN model_id
             ELSE NULL
-       END AS model_id
+       END AS model_id,
+      CASE WHEN EXISTS (SELECT 1 FROM pragma_table_info('medias') WHERE name = 'posted_at')
+            THEN posted_at
+            ELSE NULL
+       END AS posted_at,
+        CASE WHEN EXISTS (SELECT 1 FROM pragma_table_info('medias') WHERE name = 'hash')
+            THEN hash
+            ELSE NULL
+       END AS hash,
+        CASE WHEN EXISTS (SELECT 1 FROM pragma_table_info('medias') WHERE name = 'duration')
+            THEN duration
+            ELSE NULL
+       END AS duration
 FROM medias;
 """
 mediaDrop = """
 drop table medias;
 """
 mediaUpdateAPI = """Update 'medias'
 SET
-media_id=?,post_id=?,linked=?,api_type=?,media_type=?,preview=?,created_at=?,posted_at=?,model_id=?
+media_id=?,post_id=?,linked=?,api_type=?,media_type=?,preview=?,created_at=?,posted_at=?,model_id=?,duration=?,unlocked=?
 WHERE media_id=(?) and model_id=(?);"""
 mediaUpdateDownload = """Update 'medias'
 SET
 directory=?,filename=?,size=?,downloaded=?,hash=?
 WHERE media_id=(?) and model_id=(?);"""
 
 
@@ -96,26 +110,26 @@
 HAVING COUNT(*) > 1;
 """
 mediaDupeFiles = """
 SELECT filename
 FROM medias
 where hash=(?)
 """
-mediaInsert = """INSERT INTO 'medias'(
+mediaInsertAPI = """INSERT INTO 'medias'(
 media_id,post_id,link,api_type,
 media_type,preview,linked,
-created_at,posted_at,model_id)
-            VALUES (?,?,?,?,?,?,?,?,?,?);"""
+created_at,posted_at,model_id,duration,unlocked)
+            VALUES (?,?,?,?,?,?,?,?,?,?,?,?);"""
 
-mediaInsertFull = """INSERT INTO 'medias'(
+mediaInsertTransition = """INSERT INTO 'medias'(
 media_id,post_id,link,directory,
 filename,size,api_type,
 media_type,preview,linked,
-downloaded,created_at,posted_at,hash,model_id)
-            VALUES (?,?,?,?,?,?,?,?,?,?,?,?,?,?,?);"""
+downloaded,created_at,posted_at,hash,model_id,duration,unlocked)
+            VALUES (?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?);"""
 mediaDownloadSelect = """
 SELECT  
 directory,filename,size
 downloaded,hash
 FROM medias where media_id=(?)
 """
 allIDCheck = """
@@ -128,42 +142,44 @@
 allDLModelIDCheck = """
 SELECT media_id FROM medias where downloaded=(1) and model_id=(?)
 """
 getTimelineMedia = """
 SELECT
 media_id,post_id,link,directory
 filename,size,api_type,media_type
-preview,linked,downloaded,created_at,posted_at,hash,model_id
+preview,linked,downloaded,created_at,posted_at,hash,model_id,unlocked
 FROM medias where api_type=('Timeline') and model_id=(?)
 """
 getArchivedMedia = """
 SELECT
 media_id,post_id,link,directory
 filename,size,api_type,media_type
-preview,linked,downloaded,created_at,posted_at,hash,model_id
+preview,linked,downloaded,created_at,posted_at,hash,model_id,unlocked
 FROM medias where api_type=('Archived') and model_id=(?)
 """
 getMessagesMedia = """
 SELECT 
 media_id,post_id,link,directory
 filename,size,api_type,media_type
-preview,linked,downloaded,created_at,posted_at,hash,model_id
+preview,linked,downloaded,created_at,posted_at,hash,model_id,unlocked
 FROM medias where api_type=('Message') or api_type=('Messages') and model_id=(?)
 """
 
 
 @wrapper.operation_wrapper_async
-def create_media_table(model_id=None, username=None, conn=None):
+def create_media_table(model_id=None, username=None, conn=None, db_path=None, **kwargs):
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(mediaCreate)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def add_column_media_hash(model_id=None, username=None, conn=None):
+def add_column_media_hash(
+    model_id=None, username=None, conn=None, db_path=None, **kwargs
+):
     with contextlib.closing(conn.cursor()) as cur:
         try:
             # Check if column exists (separate statement)
             cur.execute(
                 "SELECT CASE WHEN EXISTS (SELECT 1 FROM PRAGMA_TABLE_INFO('medias') WHERE name = 'hash') THEN 1 ELSE 0 END AS alter_required;"
             )
             alter_required = cur.fetchone()[0]  # Fetch the result (0 or 1)
@@ -174,14 +190,33 @@
             conn.commit()
         except sqlite3.Error as e:
             conn.rollback()
             raise e  # Rollback in case of errors
 
 
 @wrapper.operation_wrapper_async
+def add_column_media_unlocked(model_id=None, username=None, conn=None, **kwargs):
+    with contextlib.closing(conn.cursor()) as cur:
+        try:
+            # Check if column exists (separate statement)
+            cur.execute(
+                "SELECT CASE WHEN EXISTS (SELECT 1 FROM PRAGMA_TABLE_INFO('medias') WHERE name = 'unlocked') THEN 1 ELSE 0 END AS alter_required;"
+            )
+            alter_required = cur.fetchone()[0]  # Fetch the result (0 or 1)
+            # Add column if necessary (conditional execution)
+            if alter_required == 0:
+                cur.execute("ALTER TABLE medias ADD COLUMN unlocked BOOL;")
+                # Commit changes
+            conn.commit()
+        except sqlite3.Error as e:
+            conn.rollback()
+            raise e  # Rollback in case of errors
+
+
+@wrapper.operation_wrapper_async
 def add_column_media_posted_at(conn=None, **kwargs):
     with contextlib.closing(conn.cursor()) as cur:
         try:
             # Check if column exists (separate statement)
             cur.execute(
                 "SELECT CASE WHEN EXISTS (SELECT 1 FROM PRAGMA_TABLE_INFO('medias') WHERE name = 'posted_at') THEN 1 ELSE 0 END AS alter_required;"
             )
@@ -194,15 +229,15 @@
             conn.commit()
         except sqlite3.Error as e:
             conn.rollback()
             raise e  # Rollback in case of errors
 
 
 @wrapper.operation_wrapper_async
-def add_column_media_ID(model_id=None, username=None, conn=None):
+def add_column_media_ID(model_id=None, username=None, conn=None, **kwargs):
     with contextlib.closing(conn.cursor()) as cur:
         try:
             # Check if column exists (separate statement)
             cur.execute(
                 "SELECT CASE WHEN EXISTS (SELECT 1 FROM PRAGMA_TABLE_INFO('medias') WHERE name = 'model_id') THEN 1 ELSE 0 END AS alter_required;"
             )
             alter_required = cur.fetchone()[0]  # Fetch the result (0 or 1)
@@ -215,14 +250,33 @@
             conn.commit()
         except sqlite3.Error as e:
             conn.rollback()
             raise e  # Rollback in case of errors
 
 
 @wrapper.operation_wrapper_async
+def add_column_media_duration(model_id=None, username=None, conn=None, **kwargs):
+    with contextlib.closing(conn.cursor()) as cur:
+        try:
+            # Check if column exists (separate statement)
+            cur.execute(
+                "SELECT CASE WHEN EXISTS (SELECT 1 FROM PRAGMA_TABLE_INFO('medias') WHERE name = 'duration') THEN 1 ELSE 0 END AS alter_required;"
+            )
+            alter_required = cur.fetchone()[0]  # Fetch the result (0 or 1)
+            # Add column if necessary (conditional execution)
+            if alter_required == 0:
+                cur.execute("ALTER TABLE medias ADD COLUMN duration VARCHAR;")
+                # Commit changes
+            conn.commit()
+        except sqlite3.Error as e:
+            conn.rollback()
+            raise e  # Rollback in case of errors
+
+
+@wrapper.operation_wrapper_async
 def get_media_ids(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(allIDCheck)
         return [dict(row)["media_id"] for row in cur.fetchall()]
 
 
 @wrapper.operation_wrapper
@@ -266,14 +320,15 @@
 def download_media_update(
     media,
     model_id=None,
     conn=None,
     filename=None,
     downloaded=None,
     hashdata=None,
+    changed=False,
     **kwargs,
 ):
     with contextlib.closing(conn.cursor()) as curr:
         update_media_table_via_api_helper(
             media, curr=curr, model_id=model_id, conn=conn
         )
         update_media_table_download_helper(
@@ -281,14 +336,15 @@
             model_id,
             filename=filename,
             hashdata=hashdata,
             conn=conn,
             curr=curr,
             downloaded=downloaded,
         )
+        return curr.rowcount if changed else None
 
 
 @wrapper.operation_wrapper_async
 def write_media_table_via_api_batch(medias, model_id=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as curr:
         insertData = list(
             map(
@@ -299,19 +355,50 @@
                     media.responsetype.capitalize(),
                     media.mediatype.capitalize(),
                     media.preview,
                     media.linked,
                     media.date,
                     media.postdate,
                     model_id,
+                    media.duration_string,
+                    media.canview,
+                ],
+                medias,
+            )
+        )
+        curr.executemany(mediaInsertAPI, insertData)
+        conn.commit()
+
+
+@wrapper.operation_wrapper_async
+def update_media_table_via_api_batch(
+    medias, model_id=None, conn=None, **kwargs
+) -> list:
+    with contextlib.closing(conn.cursor()) as curr:
+        insertData = list(
+            map(
+                lambda media: [
+                    media.id,
+                    media.postid,
+                    media.url or media.mpd,
+                    media.responsetype.capitalize(),
+                    media.mediatype.capitalize(),
+                    media.preview,
+                    media.date,
+                    media.postdate,
+                    model_id,
+                    media.duration_string,
+                    media.canview,
+                    media.id,
+                    model_id,
                 ],
                 medias,
             )
         )
-        curr.executemany(mediaInsert, insertData)
+        curr.executemany(mediaUpdateAPI, insertData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def write_media_table_transition(inputData, model_id=None, conn=None, **kwargs):
     with contextlib.closing(conn.cursor()) as curr:
         ordered_keys = [
@@ -326,88 +413,98 @@
             "preview",
             "linked",
             "downloaded",
             "created_at",
             "posted_at",
             "hash",
             "model_id",
+            "duration",
+            "unlocked",
         ]
         insertData = [tuple([data[key] for key in ordered_keys]) for data in inputData]
-        curr.executemany(mediaInsertFull, insertData)
+        curr.executemany(mediaInsertTransition, insertData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def get_all_medias_transition(
-    model_id=None, username=None, conn=None, database_model=None
+    model_id=None, username=None, conn=None, database_model=None, **kwargs
 ) -> list:
     with contextlib.closing(conn.cursor()) as cur:
-        cur.execute(mediaALLTransition)
-        conn.commit()
+        cur.execute(mediaSelectTransition)
         data = [dict(row) for row in cur.fetchall()]
         return [
-            dict(row, model_id=row.get("model_id") or database_model) for row in data
+            dict(
+                row,
+                model_id=row.get("model_id") or database_model,
+                duration=row.get("duration"),
+                unlocked=row.get("unlocked"),
+            )
+            for row in data
         ]
 
 
 @wrapper.operation_wrapper_async
-def drop_media_table(model_id=None, username=None, conn=None) -> list:
+def drop_media_table(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(mediaDrop)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def get_messages_media(conn=None, model_id=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(getMessagesMedia, [model_id])
         data = [dict(row) for row in cur.fetchall()]
         return [
-            dict(ele, posted_at=arrow.get(ele.get("posted_at") or 0).float_timestamp)
+            dict(ele, posted_at=arrow.get(ele["posted_at"] or 0).float_timestamp)
             for ele in data
         ]
 
 
 @run
 @wrapper.operation_wrapper_async
 def get_archived_media(conn=None, model_id=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(getArchivedMedia, [model_id])
         data = [dict(row) for row in cur.fetchall()]
         return [
-            dict(ele, posted_at=arrow.get(ele.get("posted_at") or 0).float_timestamp)
+            dict(ele, posted_at=arrow.get(ele["posted_at"] or 0).float_timestamp)
             for ele in data
         ]
 
 
 @run
 @wrapper.operation_wrapper_async
-def get_timeline_media(model_id=None, username=None, conn=None) -> list:
+def get_timeline_media(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(getTimelineMedia, [model_id])
         data = [dict(row) for row in cur.fetchall()]
         return [
-            dict(ele, posted_at=arrow.get(ele.get("posted_at") or 0).float_timestamp)
+            dict(ele, posted_at=arrow.get(ele["posted_at"] or ele["created_at"] or 0))
             for ele in data
         ]
 
 
 def update_media_table_via_api_helper(
     media, model_id=None, conn=None, curr=None, **kwargs
 ) -> list:
+
     insertData = [
         media.id,
         media.postid,
         media.url or media.mpd,
         media.responsetype.capitalize(),
         media.mediatype.capitalize(),
         media.preview,
         media.date,
         media.postdate,
         model_id,
+        media.duration_string,
+        media.canview,
         media.id,
         model_id,
     ]
     curr.execute(mediaUpdateAPI, insertData)
     conn.commit()
 
 
@@ -428,15 +525,15 @@
     )
     insertData.extend([media.id, model_id])
     curr.execute(mediaUpdateDownload, insertData)
     conn.commit()
 
 
 def media_exist_insert_helper(
-    filename=None, downloaded=None, hashdata=None, prevData=None
+    filename=None, downloaded=None, hashdata=None, prevData=None, **kwargs
 ):
     directory = None
     filename_path = None
     size = None
     if filename and pathlib.Path(filename).exists():
         directory = str(pathlib.Path(filename).parent)
         filename_path = str(pathlib.Path(filename).name)
@@ -465,16 +562,29 @@
     mediaDict = {}
     for ele in media:
         mediaDict[ele.id] = ele
     await write_media_table_via_api_batch(
         list(filter(lambda x: x.id not in curr, mediaDict.values())), **kwargs
     )
 
+    await update_media_table_via_api_batch(
+        list(filter(lambda x: x.id in curr, mediaDict.values())), **kwargs
+    )
+
 
-async def modify_unique_constriant_media(model_id=None, username=None):
-    database_model = get_single_model(model_id=model_id, username=username)
+async def modify_unique_constriant_media(
+    model_id=None, username=None, db_path=None, **kwargs
+):
+    database_model = get_single_model_via_profile(
+        model_id=model_id, username=username, db_path=db_path
+    )
     data = await get_all_medias_transition(
-        model_id=model_id, username=username, database_model=database_model
+        model_id=model_id,
+        username=username,
+        database_model=database_model,
+        db_path=db_path,
+    )
+    await drop_media_table(model_id=model_id, username=username, db_path=db_path)
+    await create_media_table(model_id=model_id, username=username, db_path=db_path)
+    await write_media_table_transition(
+        data, model_id=model_id, username=username, db_path=db_path
     )
-    await drop_media_table(model_id=model_id, username=username)
-    await create_media_table(model_id=model_id, username=username)
-    await write_media_table_transition(data, model_id=model_id, username=username)
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/db/operations_/messages.py` & `ofscraper-3.9.1/ofscraper/db/operations_/messages.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import arrow
 from rich.console import Console
 
 import ofscraper.db.operations_.helpers as helpers
 import ofscraper.db.operations_.media as media
 import ofscraper.db.operations_.wrapper as wrapper
 import ofscraper.utils.args.read as read_args
-from ofscraper.db.operations_.profile import get_single_model
+from ofscraper.db.operations_.profile import get_single_model_via_profile
 
 console = Console()
 log = logging.getLogger("shared")
 
 # user_id==sender
 messagesCreate = """
 CREATE TABLE IF NOT EXISTS messages (
@@ -49,15 +49,15 @@
             VALUES (?, ?,?,?,?,?,?,?);"""
 messagesUpdate = """UPDATE messages
 SET text = ?, price = ?, paid = ?, archived = ?, created_at = ?, user_id=?,model_id=?
 WHERE post_id = ? and model_id=(?);"""
 allMessagesCheck = """
 SELECT post_id FROM messages
 """
-messagesALLTransition = """
+messagesSelectTransition = """
 SELECT post_id, text, price, paid, archived, created_at, user_id,
        CASE WHEN EXISTS (SELECT 1 FROM pragma_table_info('messages') WHERE name = 'model_id')
             THEN model_id
             ELSE NULL
        END AS model_id
 FROM messages;
 """
@@ -66,15 +66,17 @@
 """
 messagesData = """
 SELECT created_at,post_id FROM messages where model_id=(?)
 """
 
 
 @wrapper.operation_wrapper_async
-def create_message_table(model_id=None, username=None, conn=None):
+def create_message_table(
+    model_id=None, username=None, conn=None, db_path=None, **kwargs
+):
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(messagesCreate)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def update_messages_table(messages: dict, model_id=None, conn=None, **kwargs):
@@ -138,47 +140,47 @@
         ]
         insertData = [tuple([data[key] for key in ordered_keys]) for data in inputData]
         cur.executemany(messagesInsert, insertData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def get_all_messages_ids(model_id=None, username=None, conn=None) -> list:
+def get_all_messages_ids(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(allMessagesCheck)
         return [dict(row)["post_id"] for row in cur.fetchall()]
 
 
 @wrapper.operation_wrapper_async
 def get_all_messages_transition(
-    model_id=None, username=None, conn=None, database_model=None
+    model_id=None, username=None, conn=None, database_model=None, **kwargs
 ) -> list:
     with contextlib.closing(conn.cursor()) as cur:
-        cur.execute(messagesALLTransition)
+        cur.execute(messagesSelectTransition)
+        data = [dict(row) for row in cur.fetchall()]
         return [
-            dict(row, model_id=row.get("model_id") or database_model)
-            for row in cur.fetchall()
+            dict(row, model_id=row.get("model_id") or database_model) for row in data
         ]
 
 
 @wrapper.operation_wrapper_async
-def drop_messages_table(model_id=None, username=None, conn=None) -> list:
+def drop_messages_table(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(messagesDrop)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def get_messages_post_info(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(messagesData, [model_id])
         conn.commit()
         data = [dict(row) for row in cur.fetchall()]
         return [
-            dict(ele, created_at=arrow.get(ele.get("created_at")).float_timestamp)
+            dict(ele, created_at=arrow.get(ele.get("created_at") or 0).float_timestamp)
             for ele in data
         ]
 
 
 @wrapper.operation_wrapper_async
 def add_column_messages_ID(conn=None, **kwargs):
     with contextlib.closing(conn.cursor()) as cur:
@@ -194,34 +196,50 @@
             # Commit changes
             conn.commit()
         except sqlite3.Error as e:
             conn.rollback()
             raise e
 
 
-async def modify_unique_constriant_messages(model_id=None, username=None):
-    database_model = get_single_model(model_id=model_id, username=username)
+async def modify_unique_constriant_messages(
+    model_id=None, username=None, db_path=None, **kwargs
+):
+    database_model = get_single_model_via_profile(
+        model_id=model_id, username=username, db_path=db_path
+    )
     data = await get_all_messages_transition(
-        model_id=model_id, username=username, database_model=database_model
+        model_id=model_id,
+        username=username,
+        database_model=database_model,
+        db_path=db_path,
+    )
+    await drop_messages_table(model_id=model_id, username=username, db_path=db_path)
+    await create_message_table(model_id=model_id, username=username, db_path=db_path)
+    await write_messages_table_transition(
+        data, model_id=model_id, username=username, db_path=db_path
     )
-    await drop_messages_table(model_id=model_id, username=username)
-    await create_message_table(model_id=model_id, username=username)
-    await write_messages_table_transition(data, model_id=model_id, username=username)
 
 
-async def make_messages_table_changes(all_messages, model_id=None, username=None):
+async def make_messages_table_changes(
+    all_messages, model_id=None, username=None, **kwargs
+):
     curr_id = set(await get_all_messages_ids(model_id=model_id, username=username))
-    all_messages_filtered = filter(lambda x: x.responsetype=="messages", all_messages)
-
-    new_posts = list(filter(lambda x: x.id not in curr_id, all_messages_filtered))
-    curr_posts = list(filter(lambda x: x.id in curr_id, all_messages_filtered))
+    new_posts = list(filter(lambda x: x.id not in curr_id, all_messages))
+    curr_posts = list(filter(lambda x: x.id in curr_id, all_messages))
     if len(new_posts) > 0:
         new_posts = helpers.converthelper(new_posts)
         await write_messages_table(new_posts, model_id=model_id, username=username)
     if read_args.retriveArgs().metadata and len(curr_posts) > 0:
         curr_posts = helpers.converthelper(curr_posts)
         await update_messages_table(curr_posts, model_id=model_id, username=username)
 
 
-async def get_last_message_date(model_id=None, username=None):
+async def get_oldest_message_date(model_id=None, username=None, **kwargs):
+    data = await media.get_messages_media(model_id=model_id, username=username)
+    last_item = sorted(data, key=lambda x: arrow.get(x["posted_at"] or 0))[0]
+    return last_item["posted_at"] or 0
+
+
+async def get_youngest_message_date(model_id=None, username=None, **kwargs):
     data = await media.get_messages_media(model_id=model_id, username=username)
-    return sorted(data, key=lambda x: x.get("posted_at") or 0)[-1].get("posted_at") or 0
+    last_item = sorted(data, key=lambda x: arrow.get(x["posted_at"] or 0))[-1]
+    return last_item["posted_at"] or 0
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/db/operations_/others.py` & `ofscraper-3.9.1/ofscraper/db/operations_/others.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import contextlib
 import logging
 import sqlite3
 
 from rich.console import Console
 
 import ofscraper.db.operations_.wrapper as wrapper
-from ofscraper.db.operations_.profile import get_single_model
+from ofscraper.db.operations_.profile import get_single_model_via_profile
 
 console = Console()
 log = logging.getLogger("shared")
 
 otherCreate = """
 CREATE TABLE IF NOT EXISTS others (
 	id INTEGER NOT NULL,  
@@ -59,30 +59,30 @@
 schemaAll = """
 SELECT flag_name FROM schema_flags WHERE flag_value = 1;
 """
 schemaInsert = """
 INSERT OR REPLACE INTO schema_flags (flag_name, flag_value)
 VALUES (?, ?);
 """
-othersALLTransition = """
+othersSelectTransition = """
 SELECT text,price,paid,archived,created_at ,
        CASE WHEN EXISTS (SELECT 1 FROM pragma_table_info('others') WHERE name = 'model_id')
             THEN model_id
             ELSE NULL
        END AS model_id
 FROM others;
 """
 othersDrop = """
 drop table others;
 """
 othersInsert = """INSERT INTO 'others'(
 post_id, text,price,paid,archived,
 created_at,model_id)
 VALUES (?, ?,?,?,?,?,?);"""
-productsALLTransition = """
+productsSelectTransition = """
 SELECT text,price,paid,archived,created_at ,
        CASE WHEN EXISTS (SELECT 1 FROM pragma_table_info('products') WHERE name = 'model_id')
             THEN model_id
             ELSE NULL
        END AS model_id
 FROM products;
 """
@@ -92,22 +92,26 @@
 productsInsert = """INSERT INTO 'products'(
 post_id, text,price,paid,archived,
 created_at,title,model_id)
 VALUES (?, ?,?,?,?,?,?,?);"""
 
 
 @wrapper.operation_wrapper_async
-def create_products_table(model_id=None, username=None, conn=None):
+def create_products_table(
+    model_id=None, username=None, conn=None, db_path=None, **kwargs
+):
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(productCreate)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def create_others_table(model_id=None, username=None, conn=None):
+def create_others_table(
+    model_id=None, username=None, conn=None, db_path=None, **kwargs
+):
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(otherCreate)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def add_column_other_ID(conn=None, **kwargs):
@@ -146,48 +150,50 @@
             conn.commit()
         except sqlite3.Error as e:
             conn.rollback()
             raise e
 
 
 @wrapper.operation_wrapper_async
-def create_schema_table(model_id=None, username=None, conn=None):
+def create_schema_table(
+    model_id=None, username=None, conn=None, db_path=None, **kwargs
+):
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(schemaCreate)
         conn.commit()
 
 
 @wrapper.operation_wrapper
-def get_schema_changes(model_id=None, username=None, conn=None):
+def get_schema_changes(model_id=None, username=None, conn=None, db_path=None, **kwargs):
     with contextlib.closing(conn.cursor()) as cur:
         data = cur.execute(schemaAll).fetchall()
         return set(list(map(lambda x: x[0], data)))
 
 
 @wrapper.operation_wrapper_async
-def add_flag_schema(flag, model_id=None, username=None, conn=None):
+def add_flag_schema(flag, model_id=None, username=None, conn=None, **kwargs):
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(schemaInsert, [flag, 1])
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def get_all_others_transition(
-    model_id=None, username=None, conn=None, database_model=None
+    model_id=None, username=None, conn=None, database_model=None, **kwargs
 ):
     with contextlib.closing(conn.cursor()) as cur:
-        cur.execute(othersALLTransition)
+        cur.execute(othersSelectTransition)
+        data = [dict(row) for row in cur.fetchall()]
         return [
-            dict(row, model_id=row.get("model_id") or database_model)
-            for row in cur.fetchall()
+            dict(row, model_id=row.get("model_id") or database_model) for row in data
         ]
 
 
 @wrapper.operation_wrapper_async
-def drop_others_table(model_id=None, username=None, conn=None):
+def drop_others_table(model_id=None, username=None, conn=None, **kwargs):
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(othersDrop)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def write_others_table_transition(
@@ -198,26 +204,26 @@
         insertData = [tuple([data[key] for key in ordered_keys]) for data in inputData]
         cur.executemany(othersInsert, insertData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def get_all_products_transition(
-    model_id=None, username=None, conn=None, database_model=None
+    model_id=None, username=None, conn=None, database_model=None, **kwargs
 ):
     with contextlib.closing(conn.cursor()) as cur:
-        cur.execute(productsALLTransition)
+        cur.execute(productsSelectTransition)
+        data = [dict(row) for row in cur.fetchall()]
         return [
-            dict(row, model_id=row.get("model_id") or database_model)
-            for row in cur.fetchall()
+            dict(row, model_id=row.get("model_id") or database_model) for row in data
         ]
 
 
 @wrapper.operation_wrapper_async
-def drop_products_table(model_id=None, username=None, conn=None):
+def drop_products_table(model_id=None, username=None, conn=None, **kwargs):
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(productsDrop)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def write_products_table_transition(
@@ -226,25 +232,43 @@
     with contextlib.closing(conn.cursor()) as cur:
         ordered_keys = ["text", "price", "paid", "archived", "created_at", "model_id"]
         insertData = [tuple([data[key] for key in ordered_keys]) for data in inputData]
         cur.executemany(productsInsert, insertData)
         conn.commit()
 
 
-async def modify_unique_constriant_others(model_id=None, username=None):
-    database_model = get_single_model(model_id=model_id, username=username)
+async def modify_unique_constriant_others(
+    model_id=None, username=None, db_path=None, **kwargs
+):
+    database_model = get_single_model_via_profile(
+        model_id=model_id, username=username, db_path=db_path
+    )
     data = await get_all_others_transition(
-        model_id=model_id, username=username, database_model=database_model
+        model_id=model_id,
+        username=username,
+        database_model=database_model,
+        db_path=db_path,
+    )
+    await drop_others_table(model_id=model_id, username=username, db_path=db_path)
+    await create_others_table(model_id=model_id, username=username, db_path=db_path)
+    await write_others_table_transition(
+        data, model_id=model_id, username=username, db_path=db_path
     )
-    await drop_others_table(model_id=model_id, username=username)
-    await create_others_table(model_id=model_id, username=username)
-    await write_others_table_transition(data, model_id=model_id, username=username)
 
 
-async def modify_unique_constriant_products(model_id=None, username=None):
-    database_model = get_single_model(model_id=model_id, username=username)
+async def modify_unique_constriant_products(
+    model_id=None, username=None, db_path=None, **kwargs
+):
+    database_model = get_single_model_via_profile(
+        model_id=model_id, username=username, db_path=db_path
+    )
     data = await get_all_products_transition(
-        model_id=model_id, username=username, database_model=database_model
+        model_id=model_id,
+        username=username,
+        database_model=database_model,
+        db_path=db_path,
+    )
+    await drop_products_table(model_id=model_id, username=username, db_path=db_path)
+    await create_products_table(model_id=model_id, username=username, db_path=db_path)
+    await write_products_table_transition(
+        data, model_id=model_id, username=username, db_path=db_path
     )
-    await drop_products_table(model_id=model_id, username=username)
-    await create_products_table(model_id=model_id, username=username)
-    await write_products_table_transition(data, model_id=model_id, username=username)
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/db/operations_/posts.py` & `ofscraper-3.9.1/ofscraper/db/operations_/posts.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import arrow
 from rich.console import Console
 
 import ofscraper.db.operations_.helpers as helpers
 import ofscraper.db.operations_.media as media
 import ofscraper.db.operations_.wrapper as wrapper
 import ofscraper.utils.args.read as read_args
-from ofscraper.db.operations_.profile import get_single_model
+from ofscraper.db.operations_.profile import get_single_model_via_profile
 
 console = Console()
 log = logging.getLogger("shared")
 
 postCreate = """
 CREATE TABLE IF NOT EXISTS posts (
 	id INTEGER NOT NULL, 
@@ -47,15 +47,15 @@
 VALUES (?, ?,?,?,?,?,?,?);"""
 postUpdate = """UPDATE posts
 SET text = ?, price = ?, paid = ?, archived = ?, created_at = ?, model_id=?
 WHERE post_id = ? and model_id=(?);"""
 timelinePostInfo = """
 SELECT created_at,post_id FROM posts where archived=(0) and model_id=(?)
 """
-postsALLTransition = """
+postsSelectTransition = """
 SELECT post_id, text, price, paid, archived, created_at,
        CASE WHEN EXISTS (SELECT 1 FROM pragma_table_info('posts') WHERE name = 'model_id')
             THEN model_id
             ELSE NULL
        END AS model_id
 FROM posts;
 """
@@ -68,15 +68,15 @@
 
 archivedPostInfo = """
 SELECT created_at,post_id FROM posts where archived=(1) and model_id=(?)
 """
 
 
 @wrapper.operation_wrapper_async
-def write_post_table(posts: list, model_id=None, username=None, conn=None):
+def write_post_table(posts: list, model_id=None, username=None, conn=None, **kwargs):
     with contextlib.closing(conn.cursor()) as cur:
         insertData = list(
             map(
                 lambda data: (
                     data.id,
                     data.db_text,
                     data.price,
@@ -91,15 +91,15 @@
         )
         cur.executemany(postInsert, insertData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def write_post_table_transition(
-    inputData: list, model_id=None, username=None, conn=None
+    inputData: list, model_id=None, username=None, conn=None, **kwargs
 ):
     with contextlib.closing(conn.cursor()) as cur:
         ordered_keys = (
             "post_id",
             "text",
             "price",
             "paid",
@@ -110,15 +110,15 @@
         )
         insertData = [tuple([data[key] for key in ordered_keys]) for data in inputData]
         cur.executemany(postInsert, insertData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def update_posts_table(posts: list, model_id=None, username=None, conn=None):
+def update_posts_table(posts: list, model_id=None, username=None, conn=None, **kwargs):
     with contextlib.closing(conn.cursor()) as cur:
         updateData = list(
             map(
                 lambda data: [
                     data.db_text,
                     data.price,
                     data.paid,
@@ -132,57 +132,57 @@
             )
         )
         cur.executemany(postUpdate, updateData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def get_timeline_postsinfo(model_id=None, username=None, conn=None, **kwargs) -> list:
+def get_timeline_posts_info(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(timelinePostInfo, [model_id])
         data = [dict(row) for row in cur.fetchall()]
         return [
-            dict(ele, created_at=arrow.get(ele.get("created_at")).float_timestamp)
+            dict(ele, created_at=arrow.get(ele.get("created_at") or 0).float_timestamp)
             for ele in data
         ]
 
 
 @wrapper.operation_wrapper_async
-def create_post_table(model_id=None, username=None, conn=None):
+def create_post_table(model_id=None, username=None, conn=None, db_path=None, **kwargs):
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(postCreate)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def get_all_post_ids(model_id=None, username=None, conn=None) -> list:
+def get_all_post_ids(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(allPOSTCheck)
         return [dict(row)["post_id"] for row in cur.fetchall()]
 
 
 @wrapper.operation_wrapper_async
 def get_all_posts_transition(
-    model_id=None, username=None, conn=None, database_model=None
+    model_id=None, username=None, conn=None, database_model=None, **kwargs
 ) -> list:
     with contextlib.closing(conn.cursor()) as cur:
-        cur.execute(postsALLTransition)
+        cur.execute(postsSelectTransition)
         data = [dict(row) for row in cur.fetchall()]
         return [
             dict(
                 row,
                 pinned=row.get("pinned"),
                 model_id=row.get("model_id") or database_model,
             )
             for row in data
         ]
 
 
 @wrapper.operation_wrapper_async
-def drop_posts_table(model_id=None, username=None, conn=None) -> list:
+def drop_posts_table(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(postsDrop)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def add_column_post_ID(conn=None, **kwargs):
@@ -222,48 +222,71 @@
 
         except sqlite3.Error as e:
             conn.rollback()
             raise e  # Rollback in case of errors
 
 
 @wrapper.operation_wrapper_async
-def get_archived_postinfo(model_id=None, username=None, conn=None, **kwargs) -> list:
+def get_archived_post_info(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(archivedPostInfo, [model_id])
         conn.commit()
         data = [dict(row) for row in cur.fetchall()]
         return [
-            dict(ele, created_at=arrow.get(ele.get("created_at")).float_timestamp)
+            dict(ele, created_at=arrow.get(ele.get("created_at") or 0).float_timestamp)
             for ele in data
         ]
 
 
-async def modify_unique_constriant_posts(model_id=None, username=None):
-    database_model = get_single_model(model_id=model_id, username=username)
+async def modify_unique_constriant_posts(
+    model_id=None, username=None, db_path=None, **kwargs
+):
+    database_model = get_single_model_via_profile(
+        model_id=model_id, username=username, db_path=db_path
+    )
     data = await get_all_posts_transition(
-        model_id=model_id, username=username, database_model=database_model
+        model_id=model_id,
+        username=username,
+        database_model=database_model,
+        db_path=db_path,
+    )
+    await drop_posts_table(model_id=model_id, username=username, db_path=db_path)
+    await create_post_table(model_id=model_id, username=username, db_path=db_path)
+    await write_post_table_transition(
+        data, model_id=model_id, username=username, db_path=db_path
     )
-    await drop_posts_table(model_id=model_id, username=username)
-    await create_post_table(model_id=model_id, username=username)
-    await write_post_table_transition(data, model_id=model_id, username=username)
 
 
-async def make_post_table_changes(all_posts, model_id=None, username=None):
+async def make_post_table_changes(all_posts, model_id=None, username=None, **kwargs):
     curr_id = set(await get_all_post_ids(model_id=model_id, username=username))
     new_posts = list(filter(lambda x: x.id not in curr_id, all_posts))
     curr_posts = list(filter(lambda x: x.id in curr_id, all_posts))
     if len(new_posts) > 0:
         new_posts = helpers.converthelper(new_posts)
         await write_post_table(new_posts, model_id=model_id, username=username)
     if read_args.retriveArgs().metadata and len(curr_posts) > 0:
         curr_posts = helpers.converthelper(curr_posts)
         await update_posts_table(curr_posts, model_id=model_id, username=username)
 
 
-async def get_last_archived_date(model_id=None, username=None):
+async def get_oldest_archived_date(model_id=None, username=None, **kwargs):
     data = await media.get_archived_media(model_id=model_id, username=username)
-    return sorted(data, key=lambda x: x["posted_at"] or 0)[-1].get("posted_at") or 0
+    last_item = sorted(data, key=lambda x: arrow.get(x["posted_at"]))[0]
+    return last_item["posted_at"] or 0
+
+
+async def get_youngest_archived_date(model_id=None, username=None, **kwargs):
+    data = await media.get_archived_media(model_id=model_id, username=username)
+    last_item = sorted(data, key=lambda x: arrow.get(x["posted_at"]))[-1]
+    return last_item["posted_at"] or 0
+
+
+async def get_oldest_timeline_date(model_id=None, username=None, **kwargs):
+    data = await media.get_timeline_media(model_id=model_id, username=username)
+    last_item = sorted(data, key=lambda x: arrow.get(x["posted_at"]))[0]
+    return last_item["posted_at"]
 
 
-async def get_last_timeline_date(model_id=None, username=None):
+async def get_youngest_timeline_date(model_id=None, username=None, **kwargs):
     data = await media.get_timeline_media(model_id=model_id, username=username)
-    return sorted(data, key=lambda x: x["posted_at"] or 0)[-1].get("posted_at") or 0
+    last_item = sorted(data, key=lambda x: arrow.get(x["posted_at"]))[-1]
+    return last_item["posted_at"]
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/db/operations_/profile.py` & `ofscraper-3.9.1/ofscraper/db/operations_/profile.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 # user_id==modes.id cause of legacy
 profilesCreate = """
 CREATE TABLE IF NOT EXISTS profiles (
 	id INTEGER NOT NULL, 
 	user_id INTEGER NOT NULL, 
 	username VARCHAR NOT NULL,
 	PRIMARY KEY (id)
+    UNIQUE (user_id,username)
 )
 """
 modelsCreate = """
 CREATE TABLE IF NOT EXISTS models (
 	id INTEGER NOT NULL,
 	model_id INTEGER NOT NULL,
 	UNIQUE (model_id)
@@ -72,22 +73,26 @@
 profilesALL = """
 select user_id,username from profiles
 """
 profilesDrop = """
 DROP TABLE profiles;
 """
 
+modelsALL = """
+select model_id from models
+"""
+
 
 profileUnique = """
 SELECT DISTINCT user_id FROM profiles
 """
 
 
 @wrapper.operation_wrapper_async
-def get_profile_info(model_id=None, username=None, conn=None) -> list:
+def get_profile_info(model_id=None, username=None, conn=None, **kwargs) -> list:
     database_path = placeholder.databasePlaceholder().databasePathHelper(
         model_id, username
     )
     if not pathlib.Path(database_path).exists():
         return None
     with contextlib.closing(conn.cursor()) as cur:
         try:
@@ -96,94 +101,118 @@
         except sqlite3.OperationalError:
             None
         except Exception as E:
             raise E
 
 
 @wrapper.operation_wrapper_async
-def create_profile_table(model_id=None, username=None, conn=None):
+def create_profile_table(
+    model_id=None, username=None, conn=None, db_path=None, **kwargs
+):
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(profilesCreate)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def write_profile_table(model_id=None, username=None, conn=None) -> list:
+def write_profile_table(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         insertData = [model_id, username, model_id, username]
         cur.execute(profileInsert, insertData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def write_profile_table_transition(insertData, conn=None, **kwargs) -> list:
+def write_profile_table_transition(inputData, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
+        ordered_keys = [
+            "user_id",
+            "username",
+        ]
+        insertData = [tuple([data[key] for key in ordered_keys]) for data in inputData]
         cur.executemany(profileInsertTransition, insertData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def check_profile_table_exists(model_id=None, username=None, conn=None):
+def check_profile_table_exists(model_id=None, username=None, conn=None, **kwargs):
     database_path = placeholder.databasePlaceholder().databasePathHelper(
         model_id, username
     )
     if not pathlib.Path(database_path).exists():
         return False
     with contextlib.closing(conn.cursor()) as cur:
         if len(cur.execute(profileTableCheck).fetchall()) > 0:
             return True
         return False
 
 
 @wrapper.operation_wrapper_async
-def get_all_profiles(model_id=None, username=None, conn=None) -> list:
-    database_path = placeholder.databasePlaceholder().databasePathHelper(
+def get_all_profiles(
+    model_id=None, username=None, conn=None, db_path=None, **kwargs
+) -> list:
+    database_path = db_path or placeholder.databasePlaceholder().databasePathHelper(
         model_id, username
     )
     if not pathlib.Path(database_path).exists():
         return None
     with contextlib.closing(conn.cursor()) as cur:
         try:
-            profiles = cur.execute(profilesALL).fetchall()
-            conn.commit()
+            profiles = [dict(row) for row in (cur.execute(profilesALL).fetchall())]
             return profiles
         except sqlite3.OperationalError as E:
             None
         except Exception as E:
             raise E
 
 
 @wrapper.operation_wrapper_async
-def drop_profiles_table(model_id=None, username=None, conn=None) -> list:
+def drop_profiles_table(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(profilesDrop)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def create_models_table(model_id=None, username=None, conn=None):
+def create_models_table(
+    model_id=None, username=None, db_path=None, conn=None, **kwargs
+):
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(modelsCreate)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def write_models_table(model_id=None, username=None, conn=None) -> list:
+def write_models_table(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(modelInsert, [model_id, model_id])
         conn.commit()
 
 
 @wrapper.operation_wrapper
-def get_single_model(model_id=None, username=None, conn=None) -> list:
+def get_single_model_via_profile(
+    model_id=None, username=None, conn=None, db_path=None, **kwargs
+) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         models_ids = [
             dict(row)["user_id"] for row in cur.execute(profileUnique).fetchall()
         ]
         return models_ids[0] if len(models_ids) == 1 else None
 
 
-async def remove_unique_constriant_profile(model_id=None, username=None):
-    data = await get_all_profiles(model_id=model_id, username=username)
-    await drop_profiles_table(model_id=model_id, username=username)
-    await create_profile_table(model_id=model_id, username=username)
-    await write_profile_table_transition(data, model_id=model_id, username=username)
+@wrapper.operation_wrapper_async
+def get_all_models(
+    model_id=None, username=None, conn=None, db_path=None, **kwargs
+) -> list:
+    with contextlib.closing(conn.cursor()) as cur:
+        return [dict(row) for row in (cur.execute(modelsALL).fetchall())]
+
+
+async def modify_unique_constriant_profile(
+    model_id=None, username=None, db_path=None, **kwargs
+):
+    data = await get_all_profiles(model_id=model_id, username=username, db_path=db_path)
+    await drop_profiles_table(model_id=model_id, username=username, db_path=db_path)
+    await create_profile_table(model_id=model_id, username=username, db_path=db_path)
+    await write_profile_table_transition(
+        data, model_id=model_id, username=username, db_path=db_path
+    )
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/db/operations_/stories.py` & `ofscraper-3.9.1/ofscraper/db/operations_/stories.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import sqlite3
 
 from rich.console import Console
 
 import ofscraper.db.operations_.helpers as helpers
 import ofscraper.db.operations_.wrapper as wrapper
 import ofscraper.utils.args.read as read_args
-from ofscraper.db.operations_.profile import get_single_model
+from ofscraper.db.operations_.profile import get_single_model_via_profile
 
 console = Console()
 log = logging.getLogger("shared")
 
 storiesCreate = """
 CREATE TABLE IF NOT EXISTS stories (
 	id INTEGER NOT NULL, 
@@ -43,15 +43,15 @@
 post_id, text,price,paid,archived,created_at,model_id)
             VALUES (?, ?,?,?,?,?,?);"""
 storiesUpdate = """UPDATE stories
 SET text = ?, price = ?, paid = ?, archived = ?, created_at = ? ,model_id=?
 WHERE post_id = ? and model_id=(?);"""
 
 
-storiesALLTransition = """
+storiesSelectTransition = """
 SELECT post_id,text,price,paid,archived,created_at,
        CASE WHEN EXISTS (SELECT 1 FROM pragma_table_info('stories') WHERE name = 'model_id')
             THEN model_id
             ELSE NULL
        END AS model_id
 FROM stories;
 
@@ -61,22 +61,26 @@
 """
 allStoriesCheck = """
 SELECT post_id FROM stories
 """
 
 
 @wrapper.operation_wrapper_async
-def create_stories_table(model_id=None, username=None, conn=None):
+def create_stories_table(
+    model_id=None, username=None, conn=None, db_path=None, **kwargs
+):
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(storiesCreate)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def write_stories_table(stories: dict, model_id=None, username=None, conn=None):
+def write_stories_table(
+    stories: dict, model_id=None, username=None, conn=None, **kwargs
+):
     with contextlib.closing(conn.cursor()) as cur:
         stories = helpers.converthelper(stories)
         insertData = list(
             map(
                 lambda data: (
                     data.id,
                     data.db_text or data.title or "",
@@ -91,15 +95,15 @@
         )
         cur.executemany(storiesInsert, insertData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
 def write_stories_table_transition(
-    inputData: dict, model_id=None, username=None, conn=None
+    inputData: dict, model_id=None, username=None, conn=None, **kwargs
 ):
     with contextlib.closing(conn.cursor()) as cur:
         ordered_keys = [
             "post_id",
             "text",
             "price",
             "paid",
@@ -109,15 +113,17 @@
         ]
         insertData = [tuple([data[key] for key in ordered_keys]) for data in inputData]
         cur.executemany(storiesInsert, insertData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def update_stories_table(stories: dict, model_id=None, username=None, conn=None):
+def update_stories_table(
+    stories: dict, model_id=None, username=None, conn=None, **kwargs
+):
     with contextlib.closing(conn.cursor()) as cur:
         stories = helpers.converthelper(stories)
         updateData = list(
             map(
                 lambda data: (
                     data.db_text or data.title or "",
                     data.price,
@@ -132,29 +138,29 @@
             )
         )
         cur.executemany(storiesUpdate, updateData)
         conn.commit()
 
 
 @wrapper.operation_wrapper_async
-def get_all_stories_ids(model_id=None, username=None, conn=None) -> list:
+def get_all_stories_ids(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(allStoriesCheck)
         return list(map(lambda x: x[0], cur.fetchall()))
 
 
 @wrapper.operation_wrapper_async
 def get_all_stories_transition(
-    model_id=None, username=None, conn=None, database_model=None
+    model_id=None, username=None, conn=None, database_model=None, **kwargs
 ) -> list:
     with contextlib.closing(conn.cursor()) as cur:
-        cur.execute(storiesALLTransition)
+        cur.execute(storiesSelectTransition)
+        data = [dict(row) for row in cur.fetchall()]
         return [
-            dict(row, model_id=row.get("model_id") or database_model)
-            for row in cur.fetchall()
+            dict(row, model_id=row.get("model_id") or database_model) for row in data
         ]
 
 
 @wrapper.operation_wrapper_async
 def add_column_stories_ID(conn=None, **kwargs):
     with contextlib.closing(conn.cursor()) as cur:
         try:
@@ -170,34 +176,46 @@
             conn.commit()
         except sqlite3.Error as e:
             conn.rollback()
             raise e
 
 
 @wrapper.operation_wrapper_async
-def drop_stories_table(model_id=None, username=None, conn=None) -> list:
+def drop_stories_table(model_id=None, username=None, conn=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(storiesDrop)
         conn.commit()
 
 
-async def modify_unique_constriant_stories(model_id=None, username=None):
-    database_model = get_single_model(model_id=model_id, username=username)
+async def modify_unique_constriant_stories(
+    model_id=None, username=None, db_path=None, **kwargs
+):
+    database_model = get_single_model_via_profile(
+        model_id=model_id, username=username, db_path=db_path
+    )
     data = await get_all_stories_transition(
-        model_id=model_id, username=username, database_model=database_model
+        model_id=model_id,
+        username=username,
+        database_model=database_model,
+        db_path=db_path,
+    )
+
+    await drop_stories_table(model_id=model_id, username=username, db_path=db_path)
+    await create_stories_table(model_id=model_id, username=username, db_path=db_path)
+    await write_stories_table_transition(
+        data, model_id=model_id, username=username, db_path=db_path
     )
-    await drop_stories_table(model_id=model_id, username=username)
-    await create_stories_table(model_id=model_id, username=username)
-    await write_stories_table_transition(data, model_id=model_id, username=username)
 
 
 async def make_stories_table_changes(
-    all_stories: dict, model_id=None, username=None, conn=None
+    all_stories: dict, model_id=None, username=None, conn=None, **kwargs
 ):
-    all_stories_filtered = filter(lambda x: x.responsetype in {"stories","highlights"}, all_stories)
+    all_stories_filtered = filter(
+        lambda x: x.responsetype in {"stories", "highlights"}, all_stories
+    )
 
     curr_id = set(await get_all_stories_ids(model_id=model_id, username=username))
     new_posts = list(filter(lambda x: x.id not in curr_id, all_stories_filtered))
     curr_posts = list(filter(lambda x: x.id in curr_id, all_stories_filtered))
     if len(new_posts) > 0:
         new_posts = helpers.converthelper(new_posts)
         await write_stories_table(new_posts, model_id=model_id, username=username)
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/db/operations_/wrapper.py` & `ofscraper-3.9.1/ofscraper/db/operations_/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
 import asyncio
 import logging
+import pathlib
 import sqlite3
 from collections import abc
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 
 from filelock import FileLock
 from rich.console import Console
@@ -38,16 +39,19 @@
         conn = None
         try:
             LOCK_POOL = ThreadPoolExecutor()
             PROCESS_POOL = ThreadPoolExecutor(max_workers=1)
             lock = FileLock(common_paths.getDB(), timeout=-1)
             loop = asyncio.get_event_loop()
             await loop.run_in_executor(LOCK_POOL, lock.acquire)
-            database_path = placeholder.databasePlaceholder().databasePathHelper(
-                kwargs.get("model_id"), kwargs.get("username")
+            database_path = pathlib.Path(
+                kwargs.get("db_path", None)
+                or placeholder.databasePlaceholder().databasePathHelper(
+                    kwargs.get("model_id"), kwargs.get("username")
+                )
             )
             database_path.parent.mkdir(parents=True, exist_ok=True)
             conn = sqlite3.connect(database_path, check_same_thread=False, timeout=10)
             conn.row_factory = sqlite3.Row
             return await loop.run_in_executor(
                 PROCESS_POOL, partial(func, *args, **kwargs, conn=conn)
             )
@@ -85,16 +89,19 @@
     def inner(*args, **kwargs):
         try:
             lock = FileLock(common_paths.getDB(), timeout=-1)
         except Exception as E:
             raise E
         try:
             lock.acquire(timeout=-1)
-            database_path = placeholder.databasePlaceholder().databasePathHelper(
-                kwargs.get("model_id"), kwargs.get("username")
+            database_path = pathlib.Path(
+                kwargs.get("db_path", None)
+                or placeholder.databasePlaceholder().databasePathHelper(
+                    kwargs.get("model_id"), kwargs.get("username")
+                )
             )
             database_path.parent.mkdir(parents=True, exist_ok=True)
             conn = sqlite3.connect(database_path, check_same_thread=True, timeout=10)
             conn.row_factory = sqlite3.Row
             return func(*args, **kwargs, conn=conn)
         except sqlite3.OperationalError as E:
             log.info("DB may be locked")
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/alt_download.py` & `ofscraper-3.9.1/ofscraper/download/main_download.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,379 +9,268 @@
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
 import asyncio
 import pathlib
-import re
-import subprocess
 import traceback
 from functools import partial
 
 import aiofiles
-import arrow
 import psutil
-from tenacity import (
-    AsyncRetrying,
-    retry_if_not_exception_message,
-    stop_after_attempt,
-    wait_random,
-)
 
 try:
     from win32_setctime import setctime  # pylint: disable=import-error
 except ModuleNotFoundError:
     pass
 import ofscraper.classes.placeholder as placeholder
-import ofscraper.db.operations as operations
-import ofscraper.download.common.common as common
-import ofscraper.download.common.globals as common_globals
-import ofscraper.download.common.keyhelpers as keyhelpers
-import ofscraper.utils.args.read as read_args
+import ofscraper.download.shared.common.general as common
+import ofscraper.download.shared.globals as common_globals
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
-import ofscraper.utils.dates as dates
 import ofscraper.utils.settings as settings
-from ofscraper.download.common.common import (
-    addGlobalDir,
+from ofscraper.download.shared.common.general import (
     check_forced_skip,
     downloadspace,
-    get_item_total,
+    get_data,
     get_medialog,
     get_resume_size,
-    get_url_log,
-    metadata,
-    moveHelper,
-    path_to_file_logger,
-    sem_wrapper,
-    set_time,
+    get_unknown_content_type,
     size_checker,
-    temp_file_logger,
-    update_total,
 )
+from ofscraper.download.shared.utils.log import get_url_log, path_to_file_logger
+from ofscraper.download.shared.common.main_common import handle_result_main
+from ofscraper.download.shared.utils.metadata import force_download
+from ofscraper.download.shared.classes.retries import download_retry
 
 
-async def alt_download(c, ele, username, model_id, job_progress):
-    common_globals.log.debug(
-        f"{get_medialog(ele)} Downloading with protected media downloader"
-    )
-    sharedPlaceholderObj = await placeholder.Placeholders(ele, "mp4").init()
-    common_globals.log.debug(f"{get_medialog(ele)} download url:  {get_url_log(ele)}")
-    if read_args.retriveArgs().metadata != None:
-        return await metadata(
-            c, ele, username, model_id, placeholderObj=sharedPlaceholderObj
-        )
-
-    audio, video = await ele.mpd_dict
-    path_to_file_logger(sharedPlaceholderObj, ele)
-
-    audio = await alt_download_downloader(audio, c, ele, job_progress)
-    video = await alt_download_downloader(video, c, ele, job_progress)
 
-    post_result = await media_item_post_process(audio, video, ele, username, model_id)
-    if post_result:
-        return post_result
-    await media_item_keys(c, audio, video, ele)
-
-    return await handle_result(
-        sharedPlaceholderObj, ele, audio, video, username, model_id
-    )
 
-
-async def handle_result(sharedPlaceholderObj, ele, audio, video, username, model_id):
-    tempPlaceholder = await placeholder.tempFilePlaceholder(
-        ele, f"temp_{ele.id or await ele.final_filename}.mp4"
-    ).init()
-    temp_path = tempPlaceholder.tempfilepath
-    temp_path.unlink(missing_ok=True)
-    t = subprocess.run(
-        [
-            settings.get_ffmpeg(),
-            "-i",
-            str(video["path"]),
-            "-i",
-            str(audio["path"]),
-            "-c",
-            "copy",
-            "-movflags",
-            "use_metadata_tags",
-            str(temp_path),
-        ],
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-    )
-    if t.stderr.decode().find("Output") == -1:
-        common_globals.log.debug(f"{get_medialog(ele)} ffmpeg failed")
-        common_globals.log.debug(f"{get_medialog(ele)} ffmpeg {t.stderr.decode()}")
-        common_globals.log.debug(f"{get_medialog(ele)} ffmpeg {t.stdout.decode()}")
-
-    video["path"].unlink(missing_ok=True)
-    audio["path"].unlink(missing_ok=True)
-
-    common_globals.log.debug(
-        f"Moving intermediate path {temp_path} to {sharedPlaceholderObj.trunicated_filepath}"
-    )
-    moveHelper(temp_path, sharedPlaceholderObj.trunicated_filepath, ele)
-    addGlobalDir(sharedPlaceholderObj.trunicated_filepath)
-    if ele.postdate:
-        newDate = dates.convert_local_time(ele.postdate)
-        common_globals.log.debug(
-            f"{get_medialog(ele)} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}"
-        )
-        set_time(sharedPlaceholderObj.trunicated_filepath, newDate)
+async def main_download(c, ele, username, model_id, job_progress):
+    common_globals.log.debug(f"{get_medialog(ele)} Downloading with normal downloader")
+    common_globals.log.debug(f"{get_medialog(ele)} download url:  {get_url_log(ele)}")
+    if common.is_bad_url(ele.url):
         common_globals.log.debug(
-            f"{get_medialog(ele)} Date set to {arrow.get(sharedPlaceholderObj.trunicated_filepath.stat().st_mtime).format('YYYY-MM-DD HH:mm')}"
-        )
-    if ele.id:
-        await operations.download_media_update(
-            ele,
-            filename=sharedPlaceholderObj.trunicated_filepath,
-            model_id=model_id,
-            username=username,
-            downloaded=True,
-            hashdata=await common.get_hash(
-                sharedPlaceholderObj, mediatype=ele.mediatype
-            ),
+            f"{get_medialog(ele)} Forcing download because known bad url"
         )
-    return ele.mediatype, video["total"] + audio["total"]
-
+        await force_download(ele, username, model_id)
+        return ele.mediatype, 0
+    result = await main_download_downloader(
+        c,
+        ele,
+        job_progress,
+    )
 
-async def media_item_post_process(audio, video, ele, username, model_id):
-    if (audio["total"] + video["total"]) == 0:
+    # special case for zero byte files
+    if result[0] == 0:
         if ele.mediatype != "forced_skipped":
-            await operations.download_media_update(
-                ele,
-                filename=None,
-                model_id=model_id,
-                username=username,
-                downloaded=True,
-            )
+            await force_download(ele, username, model_id)
         return ele.mediatype, 0
-    for m in [audio, video]:
-        m["total"] = get_item_total(m)
-
-    for m in [audio, video]:
-        if not isinstance(m, dict):
-            return m
-        await size_checker(m["path"], ele, m["total"])
-
+    return await handle_result_main(result, ele, username, model_id)
 
-async def media_item_keys(c, audio, video, ele):
-    for item in [audio, video]:
-        item = await keyhelpers.un_encrypt(item, c, ele)
 
-
-async def alt_download_downloader(item, c, ele, job_progress):
+async def main_download_downloader(c, ele, job_progress):
     downloadspace(mediatype=ele.mediatype)
-    placeholderObj = await placeholder.tempFilePlaceholder(
-        ele, f"{item['name']}.part"
+    tempholderObj = await placeholder.tempFilePlaceholder(
+        ele, f"{await ele.final_filename}_{ele.id}.part"
     ).init()
-    item["path"] = placeholderObj.tempfilepath
-    item["total"] = None
-    async for _ in AsyncRetrying(
-        stop=stop_after_attempt(constants.getattr("DOWNLOAD_RETRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"), max=constants.getattr("OF_MAX")
-        ),
-        retry=retry_if_not_exception_message(
-            constants.getattr("SPACE_DOWNLOAD_MESSAGE")
-        ),
-        reraise=True,
-    ):
+    async for _ in download_retry():
         with _:
             try:
-                _attempt = common.alt_attempt_get(item)
-                _attempt.set(_attempt.get(0) + 1)
+                data = await get_data(ele)
+                common_globals.attempt.set(common_globals.attempt.get(0) + 1)
                 (
-                    pathlib.Path(placeholderObj.tempfilepath).unlink(missing_ok=True)
-                    if _attempt.get() > 1
+                    pathlib.Path(tempholderObj.tempfilepath).unlink(missing_ok=True)
+                    if common_globals.attempt.get() > 1
                     else None
                 )
-                data = await asyncio.get_event_loop().run_in_executor(
-                    common_globals.cache_thread,
-                    partial(cache.get, f"{item['name']}_headers"),
-                )
                 if data:
                     return await main_data_handler(
-                        data, item, c, ele, placeholderObj, job_progress
+                        data, c, tempholderObj, ele, job_progress
                     )
-
                 else:
-                    return await alt_data_handler(
-                        item, c, ele, placeholderObj, job_progress
-                    )
+                    return await alt_data_handler(c, tempholderObj, ele, job_progress)
             except OSError as E:
                 await asyncio.sleep(1)
                 common_globals.log.debug(
-                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] Number of Open Files -> { len(psutil.Process().open_files())}"
+                    f"[attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] Number of Open Files -> { len(psutil.Process().open_files())}"
                 )
                 common_globals.log.debug(
-                    f" {get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] Open Files -> {list(map(lambda x:(x.path,x.fd),psutil.Process().open_files()))}"
+                    f"[attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] Open Files  -> {list(map(lambda x:(x.path,x.fd),psutil.Process().open_files()))}"
                 )
                 raise E
             except Exception as E:
                 await asyncio.sleep(1)
                 common_globals.log.traceback_(
-                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] {traceback.format_exc()}"
+                    f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] {traceback.format_exc()}"
                 )
                 common_globals.log.traceback_(
-                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] {E}"
+                    f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] {E}"
                 )
                 raise E
 
 
-async def main_data_handler(data, item, c, ele, placeholderObj, job_progress):
-    item["total"] = int(data.get("content-length"))
-    resume_size = get_resume_size(placeholderObj, mediatype=ele.mediatype)
-    if await check_forced_skip(ele, item["total"]):
-        item["total"] = 0
-        return item
-    elif item["total"] == resume_size:
-        temp_file_logger(placeholderObj, ele)
-        return item
-    elif item["total"] != resume_size:
-        return await alt_download_sendreq(item, c, ele, placeholderObj, job_progress)
-
-
-async def alt_data_handler(item, c, ele, placeholderObj, job_progress):
+async def alt_data_handler(c, tempholderObj, ele, job_progress):
     result = None
     try:
-        result = await alt_download_sendreq(item, c, ele, placeholderObj, job_progress)
+        result = await main_download_sendreq(
+            c, ele, tempholderObj, job_progress, placeholderObj=None, total=None
+        )
     except Exception as E:
         raise E
     return result
 
 
-async def alt_download_sendreq(item, c, ele, placeholderObj, job_progress):
+async def main_data_handler(data, c, tempholderObj, ele, job_progress):
+    content_type = data.get("content-type").split("/")[-1]
+    total = int(data.get("content-length"))
+    placeholderObj = await placeholder.Placeholders(ele, content_type).init()
+    resume_size = get_resume_size(tempholderObj, mediatype=ele.mediatype)
+    # other
+    if await check_forced_skip(ele, total) == 0:
+        path_to_file_logger(placeholderObj, ele)
+        return [0]
+    elif total == resume_size:
+        path_to_file_logger(placeholderObj, ele)
+        return (
+            total,
+            tempholderObj.tempfilepath,
+            placeholderObj,
+        )
+
+    else:
+        try:
+            return await main_download_sendreq(
+                c,
+                ele,
+                tempholderObj,
+                job_progress,
+                total=total,
+                placeholderObj=placeholderObj,
+            )
+        except Exception as E:
+            raise E
+
+
+async def main_download_sendreq(
+    c, ele, tempholderObj, job_progress, total=None, placeholderObj=None
+):
     try:
-        _attempt = common.alt_attempt_get(item)
-        item["total"] = item["total"] if _attempt == 1 else None
-        base_url = re.sub("[0-9a-z]*\.mpd$", "", ele.mpd, re.IGNORECASE)
-        url = f"{base_url}{item['origname']}"
         common_globals.log.debug(
-            f"{get_medialog(ele)} Attempting to download media {item['origname']} with {url}"
+            f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] download temp path {tempholderObj.tempfilepath}"
         )
-        common_globals.log.debug(
-            f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] download temp path {placeholderObj.tempfilepath}"
+        total = total if common_globals.attempt.get() == 1 else None
+        return await send_req_inner(
+            c,
+            ele,
+            tempholderObj,
+            job_progress,
+            placeholderObj=placeholderObj,
+            total=total,
         )
-        return await send_req_inner(c, ele, item, placeholderObj, job_progress)
     except OSError as E:
         raise E
     except Exception as E:
         raise E
 
 
-async def send_req_inner(c, ele, item, placeholderObj, job_progress):
-    old_total = item["total"]
-    total = old_total
+async def send_req_inner(
+    c, ele, tempholderObj, job_progress, placeholderObj=None, total=None
+):
+    old_total = total
     try:
         await common.total_change_helper(None, total)
-        resume_size = get_resume_size(placeholderObj, mediatype=ele.mediatype)
+        resume_size = get_resume_size(tempholderObj, mediatype=ele.mediatype)
         headers = (
             None
             if resume_size == 0 or not total
             else {"Range": f"bytes={resume_size}-{total}"}
         )
-        params = {
-            "Policy": ele.policy,
-            "Key-Pair-Id": ele.keypair,
-            "Signature": ele.signature,
-        }
-        base_url = re.sub("[0-9a-z]*\.mpd$", "", ele.mpd, re.IGNORECASE)
-        url = f"{base_url}{item['origname']}"
-        async with sem_wrapper(common_globals.req_sem):
-            async with c.requests(url=url, headers=headers, params=params)() as l:
-                if l.ok:
-                    await asyncio.get_event_loop().run_in_executor(
-                        common_globals.cache_thread,
-                        partial(
-                            cache.set,
-                            f"{item['name']}_headers",
-                            {
-                                "content-length": l.headers.get("content-length"),
-                                "content-type": l.headers.get("content-type"),
-                            },
-                        ),
-                    )
-                    new_total = int(l.headers["content-length"])
-                    temp_file_logger(placeholderObj, ele)
-                    if await check_forced_skip(ele, new_total):
-                        item["total"] = 0
-                        await common.total_change_helper(None, old_total)
-                    elif total == resume_size:
-                        None
-                    else:
-                        item["total"] = new_total
-                        total = new_total
-                        await common.total_change_helper(old_total, total)
-                        await download_fileobject_writer(
-                            total, l, ele, job_progress, placeholderObj
-                        )
-                else:
-                    common_globals.log.debug(
-                        f"[bold]  {get_medialog(ele)}  alt download status[/bold]: {l.status}"
-                    )
-                    common_globals.log.debug(
-                        f"[bold] {get_medialog(ele)}  alt download text [/bold]: {await l.text_()}"
-                    )
-                    common_globals.log.debug(
-                        f"[bold]  {get_medialog(ele)} alt download  headers [/bold]: {l.headers}"
-                    )
-                    l.raise_for_status()
+        common_globals.log.debug(
+            f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] Downloading media with url {ele.url}"
+        )
+        async with c.requests_async(url=ele.url, headers=headers) as r:
+            await asyncio.get_event_loop().run_in_executor(
+                common_globals.cache_thread,
+                partial(
+                    cache.set,
+                    f"{ele.id}_headers",
+                    {
+                        "content-length": r.headers.get("content-length"),
+                        "content-type": r.headers.get("content-type"),
+                    },
+                ),
+            )
+            new_total = int(r.headers["content-length"])
+            content_type = r.headers.get("content-type").split("/")[-1]
+            content_type = content_type or get_unknown_content_type(ele)
+            if not placeholderObj:
+                placeholderObj = await placeholder.Placeholders(
+                    ele, content_type
+                ).init()
+            path_to_file_logger(placeholderObj, ele)
+            if await check_forced_skip(ele, new_total):
+                total = 0
+                await common.total_change_helper(old_total, total)
+            elif total != resume_size:
+                total = new_total
+                await common.total_change_helper(old_total, total)
+                await download_fileobject_writer(
+                    r, job_progress, ele, tempholderObj, placeholderObj, total
+                )
 
-        await size_checker(placeholderObj.tempfilepath, ele, total)
-        return item
+        await size_checker(tempholderObj.tempfilepath, ele, total)
+        return (total, tempholderObj.tempfilepath, placeholderObj)
     except Exception as E:
         await common.total_change_helper(None, -(total or 0))
         raise E
 
 
-async def download_fileobject_writer(total, l, ele, job_progress, placeholderObj):
-    pathstr = str(placeholderObj.tempfilepath)
-
+async def download_fileobject_writer(
+    r, job_progress, ele, tempholderObj, placeholderObj, total
+):
+    pathstr = str(placeholderObj.trunicated_filepath)
     downloadprogress = settings.get_download_bars()
-
     task1 = job_progress.add_task(
         f"{(pathstr[:constants.getattr('PATH_STR_MAX')] + '....') if len(pathstr) > constants.getattr('PATH_STR_MAX') else pathstr}\n",
         total=total,
         visible=True if downloadprogress else False,
     )
-    count = 0
-    loop = asyncio.get_event_loop()
-
-    fileobject = await aiofiles.open(placeholderObj.tempfilepath, "ab").__aenter__()
-    download_sleep = constants.getattr("DOWNLOAD_SLEEP")
     try:
-        async for chunk in l.iter_chunked(constants.getattr("maxChunkSize")):
+        count = 0
+        loop = asyncio.get_event_loop()
+        fileobject = await aiofiles.open(tempholderObj.tempfilepath, "ab").__aenter__()
+        download_sleep = constants.getattr("DOWNLOAD_SLEEP")
+
+        async for chunk in r.iter_chunked(constants.getattr("maxChunkSize")):
             if downloadprogress:
                 count = count + 1
+            await fileobject.write(chunk)
             common_globals.log.trace(
-                f"{get_medialog(ele)} Download Progress:{(pathlib.Path(placeholderObj.tempfilepath).absolute().stat().st_size)}/{total}"
+                f"{get_medialog(ele)} Download Progress:{(pathlib.Path(tempholderObj.tempfilepath).absolute().stat().st_size)}/{total}"
             )
-            await fileobject.write(chunk)
             if (count + 1) % constants.getattr("CHUNK_ITER") == 0:
                 await loop.run_in_executor(
                     common_globals.thread,
                     partial(
                         job_progress.update,
                         task1,
-                        completed=pathlib.Path(placeholderObj.tempfilepath)
+                        completed=pathlib.Path(tempholderObj.tempfilepath)
                         .absolute()
                         .stat()
                         .st_size,
                     ),
                 )
             (await asyncio.sleep(download_sleep)) if download_sleep else None
     except Exception as E:
         raise E
     finally:
         # Close file if needed
         try:
             await fileobject.close()
         except Exception:
             None
-
         try:
             job_progress.remove_task(task1)
         except Exception:
             None
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/alt_downloadbatch.py` & `ofscraper-3.9.1/ofscraper/download/alt_downloadbatch.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,193 +1,87 @@
 import asyncio
 import pathlib
 import re
-import subprocess
 import traceback
 from functools import partial
 
 import aiofiles
-import arrow
-from tenacity import (
-    AsyncRetrying,
-    retry,
-    retry_if_not_exception_message,
-    stop_after_attempt,
-    wait_random,
-)
+
 
 try:
     from win32_setctime import setctime  # pylint: disable=import-error
 except ModuleNotFoundError:
     pass
 import ofscraper.classes.placeholder as placeholder
-import ofscraper.db.operations as operations
-import ofscraper.download.common.common as common
-import ofscraper.download.common.globals as common_globals
-import ofscraper.download.common.keyhelpers as keyhelpers
-import ofscraper.utils.args.read as read_args
+import ofscraper.download.shared.common.general as common
+import ofscraper.download.shared.globals as common_globals
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
-import ofscraper.utils.dates as dates
-import ofscraper.utils.settings as settings
 import ofscraper.utils.system.system as system
-from ofscraper.download.common.common import (
-    addLocalDir,
+from ofscraper.download.shared.common.alt_common import (
+    handle_result_alt,
+    media_item_keys_alt,
+    media_item_post_process_alt,
+)
+from ofscraper.download.shared.common.general import (
     check_forced_skip,
     downloadspace,
-    get_item_total,
     get_medialog,
     get_resume_size,
+    size_checker,
+)
+from ofscraper.download.shared.utils.log import (
     get_url_log,
-    metadata,
-    moveHelper,
     path_to_file_logger,
-    sem_wrapper,
-    set_time,
-    size_checker,
     temp_file_logger,
 )
-from ofscraper.utils.context.run_async import run
+
+from ofscraper.download.shared.classes.retries import (
+    download_retry
+)
 
 
 async def alt_download(c, ele, username, model_id):
     common_globals.innerlog.get().debug(
         f"{get_medialog(ele)} Downloading with batch protected media downloader"
     )
     common_globals.innerlog.get().debug(
         f"{get_medialog(ele)} download url:  {get_url_log(ele)}"
     )
-    sharedPlaceholderObj = await placeholder.Placeholders(ele, "mp4").init()
-    if read_args.retriveArgs().metadata != None:
-        return await metadata(
-            c, ele, username, model_id, placeholderObj=sharedPlaceholderObj
-        )
-    audio, video = await ele.mpd_dict
+    async for _ in download_retry():
+        with _:
+            sharedPlaceholderObj = await placeholder.Placeholders(ele, "mp4").init()
+            audio, video = await ele.mpd_dict
     path_to_file_logger(sharedPlaceholderObj, ele, common_globals.innerlog.get())
     audio = await alt_download_downloader(audio, c, ele)
     video = await alt_download_downloader(video, c, ele)
 
-    post_result = await media_item_post_process(audio, video, ele, username, model_id)
+    post_result = await media_item_post_process_alt(
+        audio, video, ele, username, model_id
+    )
     if post_result:
         return post_result
-    await media_item_keys(c, audio, video, ele)
-    return await handle_result(
+    await media_item_keys_alt(c, audio, video, ele)
+    return await handle_result_alt(
         sharedPlaceholderObj, ele, audio, video, username, model_id
     )
 
 
-async def handle_result(sharedPlaceholderObj, ele, audio, video, username, model_id):
-    tempPlaceholder = await placeholder.tempFilePlaceholder(
-        ele, f"temp_{ele.id or await ele.final_filename}.mp4"
-    ).init()
-    temp_path = tempPlaceholder.tempfilepath
-
-    temp_path.unlink(missing_ok=True)
-    t = subprocess.run(
-        [
-            settings.get_ffmpeg(),
-            "-i",
-            str(video["path"]),
-            "-i",
-            str(audio["path"]),
-            "-c",
-            "copy",
-            "-movflags",
-            "use_metadata_tags",
-            str(temp_path),
-        ],
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-    )
-    if t.stderr.decode().find("Output") == -1:
-        common_globals.innerlog.get().debug(f"{get_medialog(ele)} ffmpeg failed")
-        common_globals.innerlog.get().debug(
-            f"{get_medialog(ele)} ffmpeg {t.stderr.decode()}"
-        )
-        common_globals.innerlog.get().debug(
-            f"{get_medialog(ele)} ffmpeg {t.stdout.decode()}"
-        )
-    video["path"].unlink(missing_ok=True)
-    audio["path"].unlink(missing_ok=True)
-    common_globals.innerlog.get().debug(
-        f"Moving intermediate path {temp_path} to {sharedPlaceholderObj.trunicated_filepath}"
-    )
-    moveHelper(
-        temp_path,
-        sharedPlaceholderObj.trunicated_filepath,
-        ele,
-        common_globals.innerlog.get(),
-    )
-    addLocalDir(sharedPlaceholderObj.trunicated_filepath)
-    if ele.postdate:
-        newDate = dates.convert_local_time(ele.postdate)
-        set_time(sharedPlaceholderObj.trunicated_filepath, newDate)
-        common_globals.innerlog.get().debug(
-            f"{get_medialog(ele)} Date set to {arrow.get(sharedPlaceholderObj.trunicated_filepath.stat().st_mtime).format('YYYY-MM-DD HH:mm')}"
-        )
-    if ele.id:
-        await operations.download_media_update(
-            ele,
-            filename=sharedPlaceholderObj.trunicated_filepath,
-            model_id=model_id,
-            username=username,
-            downloaded=True,
-            hashdata=await common.get_hash(
-                sharedPlaceholderObj, mediatype=ele.mediatype
-            ),
-        )
-    return ele.mediatype, video["total"] + audio["total"]
-
-
-async def media_item_post_process(audio, video, ele, username, model_id):
-    if (audio["total"] + video["total"]) == 0:
-        if ele.mediatype != "forced_skipped":
-            await operations.download_media_update(
-                ele,
-                filename=None,
-                model_id=model_id,
-                username=username,
-                downloaded=True,
-            )
-        return ele.mediatype, 0
-    for m in [audio, video]:
-        m["total"] = get_item_total(m)
-
-    for m in [audio, video]:
-        if not isinstance(m, dict):
-            return m
-        await size_checker(m["path"], ele, m["total"])
-
-
-async def media_item_keys(c, audio, video, ele):
-    for item in [audio, video]:
-        item = await keyhelpers.un_encrypt(item, c, ele, common_globals.innerlog.get())
-
-
 async def alt_download_downloader(
     item,
     c,
     ele,
 ):
     downloadspace(mediatype=ele.mediatype)
     placeholderObj = placeholder.tempFilePlaceholder(ele, f"{item['name']}.part")
     await placeholderObj.init()
     item["path"] = placeholderObj.tempfilepath
     item["total"] = None
 
-    async for _ in AsyncRetrying(
-        stop=stop_after_attempt(constants.getattr("DOWNLOAD_RETRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"), max=constants.getattr("OF_MAX")
-        ),
-        retry=retry_if_not_exception_message(
-            constants.getattr("SPACE_DOWNLOAD_MESSAGE")
-        ),
-        reraise=True,
-    ):
+    async for _ in download_retry():
         with _:
             try:
                 _attempt = common.alt_attempt_get(item)
                 _attempt.set(_attempt.get(0) + 1)
                 (
                     pathlib.Path(placeholderObj.tempfilepath).unlink(missing_ok=True)
                     if _attempt.get() > 1
@@ -199,29 +93,29 @@
                 )
                 if data:
                     return await main_data_handler(data, item, c, ele, placeholderObj)
                 else:
                     return await alt_data_handler(item, c, ele, placeholderObj)
             except OSError as E:
                 common_globals.log.debug(
-                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] Number of open Files across all processes-> {len(system.getOpenFiles(unique=False))}"
+                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] Number of open Files across all processes-> {len(system.getOpenFiles(unique=False))}"
                 )
                 common_globals.log.debug(
-                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] Number of unique open files across all processes-> {len(system.getOpenFiles())}"
+                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] Number of unique open files across all processes-> {len(system.getOpenFiles())}"
                 )
                 common_globals.log.debug(
-                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] Unique files data across all process -> {list(map(lambda x:(x.path,x.fd),(system.getOpenFiles())))}"
+                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] Unique files data across all process -> {list(map(lambda x:(x.path,x.fd),(system.getOpenFiles())))}"
                 )
                 raise E
             except Exception as E:
                 common_globals.innerlog.get().traceback_(
-                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] {traceback.format_exc()}"
+                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] {traceback.format_exc()}"
                 )
                 common_globals.innerlog.get().traceback_(
-                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] {E}"
+                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] {E}"
                 )
                 raise E
 
 
 async def main_data_handler(data, item, c, ele, placeholderObj):
     item["total"] = int(data.get("content-length"))
     resume_size = get_resume_size(placeholderObj, mediatype=ele.mediatype)
@@ -247,28 +141,28 @@
     _attempt = common.alt_attempt_get(item)
     base_url = re.sub("[0-9a-z]*\.mpd$", "", ele.mpd, re.IGNORECASE)
     url = f"{base_url}{item['origname']}"
     common_globals.innerlog.get().debug(
         f"{get_medialog(ele)} Attempting to download media {item['origname']} with {url}"
     )
     common_globals.innerlog.get().debug(
-        f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] download temp path {placeholderObj.tempfilepath}"
+        f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] download temp path {placeholderObj.tempfilepath}"
     )
     item["total"] = item["total"] if _attempt.get() == 1 else None
 
     try:
         _attempt = common.alt_attempt_get(item)
         item["total"] = item["total"] if _attempt == 1 else None
         base_url = re.sub("[0-9a-z]*\.mpd$", "", ele.mpd, re.IGNORECASE)
         url = f"{base_url}{item['origname']}"
         common_globals.log.debug(
             f"{get_medialog(ele)} Attempting to download media {item['origname']} with {url}"
         )
         common_globals.log.debug(
-            f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] download temp path {placeholderObj.tempfilepath}"
+            f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] download temp path {placeholderObj.tempfilepath}"
         )
         return await send_req_inner(c, ele, item, placeholderObj)
     except OSError as E:
         raise E
     except Exception as E:
         raise E
 
@@ -287,52 +181,42 @@
         params = {
             "Policy": ele.policy,
             "Key-Pair-Id": ele.keypair,
             "Signature": ele.signature,
         }
         base_url = re.sub("[0-9a-z]*\.mpd$", "", ele.mpd, re.IGNORECASE)
         url = f"{base_url}{item['origname']}"
-        async with sem_wrapper(common_globals.req_sem):
-            async with c.requests(url=url, headers=headers, params=params)() as l:
-                if l.ok:
-                    await asyncio.get_event_loop().run_in_executor(
-                        common_globals.cache_thread,
-                        partial(
-                            cache.set,
-                            f"{item['name']}_headers",
-                            {
-                                "content-length": l.headers.get("content-length"),
-                                "content-type": l.headers.get("content-type"),
-                            },
-                        ),
-                    )
-                    new_total = int(l.headers["content-length"])
-                    temp_file_logger(placeholderObj, ele, common_globals.innerlog.get())
-                    if await check_forced_skip(ele, new_total) == 0:
-                        item["total"] = 0
-                        await common.batch_total_change_helper(old_total, 0)
-                        return item
-                    elif item["total"] == resume_size:
-                        None
-                    else:
-                        item["total"] = new_total
-                        total = new_total
-                        await common.batch_total_change_helper(old_total, total)
-                        await download_fileobject_writer(total, l, ele, placeholderObj)
-                else:
-                    common_globals.innerlog.get().debug(
-                        f"[bold]  {get_medialog(ele)}  main download data finder status[/bold]: {l.status}"
-                    )
-                    common_globals.innerlog.get().debug(
-                        f"[bold] {get_medialog(ele)}  main download data finder text [/bold]: {await l.text_()}"
-                    )
-                    common_globals.innerlog.get().debug(
-                        f"[bold]  {get_medialog(ele)} main download data finder headers [/bold]: {l.headers}"
-                    )
-                    l.raise_for_status()
+
+        common_globals.log.debug(
+            f"{get_medialog(ele)} [attempt {common.alt_attempt_get(item).get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] Downloading media with url {url}"
+        )
+
+        async with c.requests_async(url=url, headers=headers, params=params) as l:
+            await asyncio.get_event_loop().run_in_executor(
+                common_globals.cache_thread,
+                partial(
+                    cache.set,
+                    f"{item['name']}_headers",
+                    {
+                        "content-length": l.headers.get("content-length"),
+                        "content-type": l.headers.get("content-type"),
+                    },
+                ),
+            )
+            new_total = int(l.headers["content-length"])
+            temp_file_logger(placeholderObj, ele, common_globals.innerlog.get())
+            if await check_forced_skip(ele, new_total) == 0:
+                item["total"] = 0
+                await common.batch_total_change_helper(old_total, 0)
+                return item
+            elif total != resume_size:
+                item["total"] = new_total
+                total = new_total
+                await common.batch_total_change_helper(old_total, total)
+                await download_fileobject_writer(total, l, ele, placeholderObj)
         await size_checker(placeholderObj.tempfilepath, ele, item["total"])
         return item
     except Exception as E:
         await common.batch_total_change_helper(None, -(total or 0))
         raise E
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/common/common.py` & `ofscraper-3.9.1/ofscraper/download/shared/common/general.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,36 +9,40 @@
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
 import asyncio
 import pathlib
+import re
 from functools import partial, singledispatch
 
 from humanfriendly import format_size
 
-import ofscraper.download.common.globals as common_globals
+import ofscraper.download.shared.globals as common_globals
 import ofscraper.models.selector as selector
 import ofscraper.utils.args.write as write_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.config.data as config_data
 import ofscraper.utils.constants as constants
 import ofscraper.utils.dates as dates
 import ofscraper.utils.hash as hash
 import ofscraper.utils.settings as settings
 import ofscraper.utils.system.free as system
-from ofscraper.download.common.log import *
-from ofscraper.download.common.message import *
-from ofscraper.download.common.metadata import *
-from ofscraper.download.common.paths import *
-from ofscraper.download.common.progress import *
-from ofscraper.download.common.sem import sem_wrapper
-from ofscraper.download.common.text import *
+from ofscraper.download.shared.utils.log import get_medialog
+from ofscraper.download.shared.utils.media import add_path
+from ofscraper.download.shared.utils.message import send_msg, set_send_msg
+from ofscraper.download.shared.utils.progress import update_total
 from ofscraper.utils.context.run_async import run
+import ofscraper.utils.args.read as read_args
+
+
+
+def add_additional_data(placeholderObj, ele):
+    add_path(placeholderObj, ele)
 
 
 def subProcessVariableInit(dateDict, userList, pipeCopy, logCopy, argsCopy):
     common_globals.reset_globals()
     write_args.setArgs(argsCopy)
     dates.setLogDate(dateDict)
     selector.set_ALL_SUBS_DICT(userList)
@@ -156,7 +160,18 @@
 async def total_change_helper(total, new_total):
     if not new_total and not new_total:
         return
     elif not total:
         await update_total(new_total)
     elif total and new_total - total != 0:
         await update_total(new_total - total)
+
+
+def is_bad_url(url):
+    match = re.search(r"^https://([^/]+)", url)
+    if not match:
+        return False
+    elif len(match.groups()) < 1:
+        return False
+    elif match.group(1) in constants.getattr("BAD_URL_HOST"):
+        return True
+
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/common/globals.py` & `ofscraper-3.9.1/ofscraper/download/shared/globals.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import asyncio
 import contextvars
 import threading
 from concurrent.futures import ThreadPoolExecutor
 
 import aioprocessing
 
-import ofscraper.utils.args.read as read_args
 import ofscraper.utils.config.data as config_data
 import ofscraper.utils.console as console_
 import ofscraper.utils.constants as constants
 from ofscraper.classes.semaphoreDelayed import semaphoreDelayed
 
 attempt = None
 attempt2 = None
 total_count = None
 total_count2 = None
 innerlog = None
 localDirSet = None
-req_sem = None
-
+desc = "Progress: ({p_count} photos, {v_count} videos, {a_count} audios, {forced_skipped} skipped, {skipped} failed || {sumcount}/{mediacount}||{total_bytes_download}/{total_bytes})"
 
 def reset_globals():
     # reset globals_z
     main_globals()
     set_up_contexvars()
 
 
@@ -37,52 +35,38 @@
     video_count = 0
     global audio_count
     audio_count = 0
     global skipped
     skipped = 0
     global forced_skipped
     forced_skipped = 0
-    global data
-    data = 0
-    global total_data
-    total_data = 0
     global count_lock
     count_lock = aioprocessing.AioLock()
     global chunk_lock
     chunk_lock = aioprocessing.AioLock()
 
     # global
     global thread
     thread = ThreadPoolExecutor(max_workers=config_data.get_download_semaphores() * 2)
     global sem
-    sem = semaphoreDelayed(config_data.get_download_semaphores())
+    sem = config_data.get_download_semaphores()
     global cache_thread
     cache_thread = ThreadPoolExecutor()
     global dirSet
     dirSet = set()
-    global mpd_sem
-    mpd_sem = semaphoreDelayed(config_data.get_download_semaphores())
     global lock
     lock = asyncio.Lock()
     global maxfile_sem
     maxfile_sem = semaphoreDelayed(constants.getattr("MAXFILE_SEMAPHORE"))
     global console
     console = console_.get_shared_console()
     global localDirSet
     localDirSet = set()
     global fileHashes
     fileHashes = {}
-    global req_sem
-    req_sem = semaphoreDelayed(
-        min(
-            constants.getattr("REQ_SEMAPHORE_MULTI"),
-            config_data.get_download_semaphores()
-            * constants.getattr("REQ_SEMAPHORE_MULTI"),
-        )
-    )
 
 
 def set_up_contexvars():
     global attempt
     global attempt2
     global total_count
     global total_count2
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/common/keyhelpers.py` & `ofscraper-3.9.1/ofscraper/download/shared/utils/keyhelpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,58 +6,58 @@
 import traceback
 from functools import partial
 
 from bs4 import BeautifulSoup
 from pywidevine.cdm import Cdm
 from pywidevine.device import Device
 from pywidevine.pssh import PSSH
-from tenacity import (
-    AsyncRetrying,
-    retry,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_random,
-)
 
-import ofscraper.classes.sessionbuilder as sessionbuilder
-import ofscraper.download.common.globals as common_globals
+import ofscraper.download.shared.globals as common_globals
 import ofscraper.utils.auth.request as auth_requests
 import ofscraper.utils.cache as cache
 import ofscraper.utils.config.data as config_data
 import ofscraper.utils.constants as constants
 import ofscraper.utils.settings as settings
-from ofscraper.download.common.common import get_medialog
+from ofscraper.download.shared.common.general import get_medialog
+from ofscraper.download.shared.classes.retries import get_cmd_download_req_retries
+from ofscraper.download.shared.classes.session import cdm_session
+
+
 
 log = None
 
 
 def setLog(input_):
     global log
     log = input_
 
 
 async def un_encrypt(item, c, ele, input_=None):
     setLog(input_ or common_globals.log)
     key = None
     keymode = settings.get_key_mode()
-    past_key = await asyncio.get_event_loop().run_in_executor(
-        common_globals.cache_thread, partial(cache.get, ele.license)
+    past_key = (
+        await asyncio.get_event_loop().run_in_executor(
+            common_globals.cache_thread, partial(cache.get, ele.license)
+        )
+        if constants.getattr("USE_CACHE_KEY")
+        else None
     )
     if past_key:
         key = past_key
         log.debug(f"{get_medialog(ele)} got key from cache")
-    if keymode == "manual":
+    elif keymode == "manual":
         key = await key_helper_manual(c, item["pssh"], ele.license, ele.id)
     elif keymode == "keydb":
         key = await key_helper_keydb(c, item["pssh"], ele.license, ele.id)
     elif keymode == "cdrm":
         key = await key_helper_cdrm(c, item["pssh"], ele.license, ele.id)
     elif keymode == "cdrm2":
         key = await key_helper_cdrm2(c, item["pssh"], ele.license, ele.id)
-    if key == None:
+    if not key:
         raise Exception(f"{get_medialog(ele)} Could not get key")
     await asyncio.get_event_loop().run_in_executor(
         common_globals.cache_thread,
         partial(cache.set, ele.license, key, expire=constants.getattr("KEY_EXPIRY")),
     )
     log.debug(f"{get_medialog(ele)} got key")
     newpath = pathlib.Path(re.sub("\.part$", "", str(item["path"]), re.IGNORECASE))
@@ -84,235 +84,183 @@
     pathlib.Path(item["path"]).unlink(missing_ok=True)
     item["path"] = newpath
     return item
 
 
 async def key_helper_cdrm(c, pssh, licence_url, id):
     log.debug(f"ID:{id} using cdrm auto key helper")
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            try:
-                log.debug(f"ID:{id} pssh: {pssh!=None}")
-                log.debug(f"ID:{id} licence: {licence_url}")
-                headers = auth_requests.make_headers()
-                headers["cookie"] = auth_requests.get_cookies()
-                auth_requests.create_sign(licence_url, headers)
-                json_data = {
-                    "license": licence_url,
-                    "headers": json.dumps(headers),
-                    "pssh": pssh,
-                    "buildInfo": "",
-                    "proxy": "",
-                    "cache": True,
-                }
-                async with c.requests(
-                    url=constants.getattr("CDRM"), method="post", json=json_data
-                )() as r:
-                    if r.ok:
-                        httpcontent = await r.text_()
-                        log.debug(f"ID:{id} key_response: {httpcontent}")
-                        soup = BeautifulSoup(httpcontent, "html.parser")
-                        out = soup.find("li").contents[0]
-                    else:
-                        log.debug(f"[bold]  key helper cdrm status[/bold]: {r.status}")
-                        log.debug(
-                            f"[bold]  key helper cdrm text [/bold]: {await r.text_()}"
-                        )
-                        log.debug(
-                            f"[bold]  key helper cdrm headers [/bold]: {r.headers}"
-                        )
-                        r.raise_for_status()
-                    return out
-            except Exception as E:
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
+    try:
+        log.debug(f"ID:{id} pssh: {pssh!=None}")
+        log.debug(f"ID:{id} licence: {licence_url}")
+        headers = auth_requests.make_headers()
+        headers["cookie"] = auth_requests.get_cookies()
+        auth_requests.create_sign(licence_url, headers)
+        json_data = {
+            "license": licence_url,
+            "headers": json.dumps(headers),
+            "pssh": pssh,
+            "buildInfo": "",
+            "proxy": "",
+            "cache": True,
+        }
+        async with c.requests_async(
+            url=constants.getattr("CDRM"),
+            method="post",
+            json=json_data,
+            retries=get_cmd_download_req_retries(),
+            wait_min=constants.getattr("OF_MIN_WAIT_API"),
+            wait_max=constants.getattr("OF_MAX_WAIT_API"),
+            total_timeout=constants.getattr("CDM_TIMEOUT"),
+        ) as r:
+            httpcontent = await r.text_()
+            log.debug(f"ID:{id} key_response: {httpcontent}")
+            soup = BeautifulSoup(httpcontent, "html.parser")
+            out = soup.find("li").contents[0]
+        return out
+    except Exception as E:
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
 
 
 async def key_helper_cdrm2(c, pssh, licence_url, id):
     log.debug(f"ID:{id} using cdrm2 auto key helper")
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            try:
-                log.debug(f"ID:{id} pssh: {pssh!=None}")
-                log.debug(f"ID:{id} licence: {licence_url}")
-                headers = auth_requests.make_headers()
-                headers["cookie"] = auth_requests.get_cookies()
-                auth_requests.create_sign(licence_url, headers)
-                json_data = {
-                    "license": licence_url,
-                    "headers": json.dumps(headers),
-                    "pssh": pssh,
-                    "buildInfo": "google/sdk_gphone_x86/generic_x86:8.1.0/OSM1.180201.037/6739391:userdebug/dev-keys",
-                    "proxy": "",
-                    "cache": True,
-                }
-                async with c.requests(
-                    url=constants.getattr("CDRM2"), method="post", json=json_data
-                )() as r:
-                    if r.ok:
-                        httpcontent = await r.text_()
-                        log.debug(f"ID:{id} key_response: {httpcontent}")
-                        soup = BeautifulSoup(httpcontent, "html.parser")
-                        out = soup.find("li").contents[0]
-                    else:
-                        log.debug(f"[bold]  key helper cdrm2 status[/bold]: {r.status}")
-                        log.debug(
-                            f"[bold]  key helper cdrm2 text [/bold]: {await r.text_()}"
-                        )
-                        log.debug(
-                            f"[bold]  key helper cdrm2 headers [/bold]: {r.headers}"
-                        )
-                        r.raise_for_status()
-                return out
-            except Exception as E:
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
+    try:
+        log.debug(f"ID:{id} pssh: {pssh!=None}")
+        log.debug(f"ID:{id} licence: {licence_url}")
+        headers = auth_requests.make_headers()
+        headers["cookie"] = auth_requests.get_cookies()
+        auth_requests.create_sign(licence_url, headers)
+        json_data = {
+            "license": licence_url,
+            "headers": json.dumps(headers),
+            "pssh": pssh,
+            "buildInfo": "google/sdk_gphone_x86/generic_x86:8.1.0/OSM1.180201.037/6739391:userdebug/dev-keys",
+            "proxy": "",
+            "cache": True,
+        }
+        async with c.requests_async(
+            url=constants.getattr("CDRM2"),
+            method="post",
+            json=json_data,
+            retries=get_cmd_download_req_retries(),
+            wait_min=constants.getattr("OF_MIN_WAIT_API"),
+            wait_max=constants.getattr("OF_MAX_WAIT_API"),
+            total_timeout=constants.getattr("CDM_TIMEOUT"),
+        ) as r:
+            httpcontent = await r.text_()
+            log.debug(f"ID:{id} key_response: {httpcontent}")
+            soup = BeautifulSoup(httpcontent, "html.parser")
+            out = soup.find("li").contents[0]
+        return out
+    except Exception as E:
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
 
 
 async def key_helper_keydb(c, pssh, licence_url, id):
     log.debug(f"ID:{id} using keydb auto key helper")
-    async for _ in AsyncRetrying(
-        retry=retry_if_not_exception_type(KeyboardInterrupt),
-        stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"),
-            max=constants.getattr("OF_MAX"),
-        ),
-        reraise=True,
-    ):
-        with _:
-            try:
-                log.debug(f"ID:{id} pssh: {pssh!=None}")
-                log.debug(f"ID:{id} licence: {licence_url}")
-                headers = auth_requests.make_headers()
-                headers["cookie"] = auth_requests.get_cookies()
-                auth_requests.create_sign(licence_url, headers)
-                json_data = {
-                    "license_url": licence_url,
-                    "headers": json.dumps(headers),
-                    "pssh": pssh,
-                    "buildInfo": "",
-                    "proxy": "",
-                    "cache": True,
-                }
-
-                headers = {
-                    "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (Ktesttemp, like Gecko) Chrome/90.0.4430.85 Safari/537.36",
-                    "Content-Type": "application/json",
-                    "X-API-Key": config_data.get_keydb_api(),
-                }
-
-                async with c.requests(
-                    url=constants.getattr("KEYDB"),
-                    method="post",
-                    json=json_data,
-                    headers=headers,
-                )() as r:
-                    if r.ok:
-                        data = await r.json_()
-                        log.debug(f"keydb json {data}")
-                        if isinstance(data, str):
-                            out = data
-                        elif isinstance(data["keys"][0], str):
-                            out = data["keys"][0]
-                        elif isinstance(data["keys"][0], object):
-                            out = data["keys"][0]["key"]
-                        await asyncio.get_event_loop().run_in_executor(
-                            common_globals.cache_thread,
-                            partial(
-                                cache.set,
-                                licence_url,
-                                out,
-                                expire=constants.getattr("KEY_EXPIRY"),
-                            ),
-                        )
-                    else:
-                        log.debug(f"[bold]  key helper keydb status[/bold]: {r.status}")
-                        log.debug(
-                            f"[bold]  key helper keydb text [/bold]: {await r.text_()}"
-                        )
-                        log.debug(
-                            f"[bold]  key helper keydb headers [/bold]: {r.headers}"
-                        )
-                        r.raise_for_status()
-                return out
-            except Exception as E:
-                log.traceback_(E)
-                log.traceback_(traceback.format_exc())
-                raise E
+    try:
+        log.debug(f"ID:{id} pssh: {pssh!=None}")
+        log.debug(f"ID:{id} licence: {licence_url}")
+        headers = auth_requests.make_headers()
+        headers["cookie"] = auth_requests.get_cookies()
+        auth_requests.create_sign(licence_url, headers)
+        json_data = {
+            "license_url": licence_url,
+            "headers": json.dumps(headers),
+            "pssh": pssh,
+            "buildInfo": "",
+            "proxy": "",
+            "cache": True,
+        }
+
+        headers = {
+            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (Ktesttemp, like Gecko) Chrome/90.0.4430.85 Safari/537.36",
+            "Content-Type": "application/json",
+            "X-API-Key": config_data.get_keydb_api(),
+        }
+
+        async with c.requests_async(
+            url=constants.getattr("KEYDB"),
+            method="post",
+            json=json_data,
+            headers=headers,
+            retries=get_cmd_download_req_retries(),
+            wait_min=constants.getattr("OF_MIN_WAIT_API"),
+            wait_max=constants.getattr("OF_MAX_WAIT_API"),
+            total_timeout=constants.getattr("CDM_TIMEOUT"),
+        ) as r:
+            data = await r.json_()
+            log.debug(f"keydb json {data}")
+            if isinstance(data, str):
+                out = data
+            elif isinstance(data["keys"][0], str):
+                out = data["keys"][0]
+            elif isinstance(data["keys"][0], object):
+                out = data["keys"][0]["key"]
+            await asyncio.get_event_loop().run_in_executor(
+                common_globals.cache_thread,
+                partial(
+                    cache.set,
+                    licence_url,
+                    out,
+                    expire=constants.getattr("KEY_EXPIRY"),
+                ),
+            )
+        return out
+    except Exception as E:
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
 
 
 async def key_helper_manual(c, pssh, licence_url, id):
-    async with sessionbuilder.sessionBuilder(backend="aio") as c:
-        log.debug(f"ID:{id}  manual key helper")
-        async for _ in AsyncRetrying(
-            retry=retry_if_not_exception_type(KeyboardInterrupt),
-            stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-            wait=wait_random(
-                min=constants.getattr("OF_MIN"),
-                max=constants.getattr("OF_MAX"),
-            ),
-            reraise=True,
-        ):
-            with _:
-                try:
-                    log.debug(f"ID:{id} pssh: {pssh!=None}")
-                    log.debug(f"ID:{id} licence: {licence_url}")
-
-                    # prepare pssh
-                    pssh_obj = PSSH(pssh)
-
-                    # load device
-                    private_key = pathlib.Path(
-                        config_data.get_private_key()
-                    ).read_bytes()
-                    client_id = pathlib.Path(config_data.get_client_id()).read_bytes()
-                    device = Device(
-                        security_level=3,
-                        private_key=private_key,
-                        client_id=client_id,
-                        type_="ANDROID",
-                        flags=None,
-                    )
-
-                    # load cdm
-                    cdm = Cdm.from_device(device)
-
-                    # open cdm session
-                    session_id = cdm.open()
-
-                    keys = None
-                    challenge = cdm.get_license_challenge(session_id, pssh_obj)
-                    async with c.requests(
-                        url=licence_url, method="post", data=challenge
-                    )() as r:
-                        cdm.parse_license(session_id, (await r.content.read()))
-
-                        # cdm.parse_license(session_id, (await r.content.read()))
-                        keys = cdm.get_keys(session_id)
-                        cdm.close(session_id)
-                    keyobject = list(filter(lambda x: x.type == "CONTENT", keys))[0]
-
-                    key = "{}:{}".format(keyobject.kid.hex, keyobject.key.hex())
-                    return key
-                except Exception as E:
-                    log.traceback_(E)
-                    log.traceback_(traceback.format_exc())
-                    raise E
+    log.debug(f"ID:{id}  manual key helper")
+    try:
+        log.debug(f"ID:{id} pssh: {pssh!=None}")
+        log.debug(f"ID:{id} licence: {licence_url}")
+
+        # prepare pssh
+        pssh_obj = PSSH(pssh)
+
+        # load device
+        private_key = pathlib.Path(config_data.get_private_key()).read_bytes()
+        client_id = pathlib.Path(config_data.get_client_id()).read_bytes()
+        device = Device(
+            security_level=3,
+            private_key=private_key,
+            client_id=client_id,
+            type_="ANDROID",
+            flags=None,
+        )
+
+        # load cdm
+        cdm = Cdm.from_device(device)
+
+        # open cdm session
+        session_id = cdm.open()
+
+        keys = None
+        challenge = cdm.get_license_challenge(session_id, pssh_obj)
+        async with cdm_session() as c:
+            async with c.requests_async(
+                url=licence_url,
+                method="post",
+                data=challenge,
+                retries=get_cmd_download_req_retries() ,
+                wait_min=constants.getattr("OF_MIN_WAIT_API"),
+                wait_max=constants.getattr("OF_MAX_WAIT_API"),
+                total_timeout=constants.getattr("CDM_TIMEOUT"),
+            ) as r:
+                cdm.parse_license(session_id, (await r.read_()))
+                keys = cdm.get_keys(session_id)
+                cdm.close(session_id)
+            keyobject = list(filter(lambda x: x.type == "CONTENT", keys))[0]
+
+        key = "{}:{}".format(keyobject.kid.hex, keyobject.key.hex())
+        return key
+    except Exception as E:
+        log.traceback_(E)
+        log.traceback_(traceback.format_exc())
+        raise E
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/common/log.py` & `ofscraper-3.9.1/ofscraper/download/shared/utils/log.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import re
 
 from humanfriendly import format_size
 
-import ofscraper.download.common.globals as common_globals
+import ofscraper.download.shared.globals as common_globals
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.constants as constants
 
 
 def get_medialog(ele):
     return f"Media:{ele.id} Post:{ele.postid}"
 
 
 def path_to_file_logger(placeholderObj, ele, innerlog=None):
     innerlog = innerlog or common_globals.log
     innerlog.debug(
-        f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('NUM_TRIES')}] filename from config {placeholderObj.filename}"
+        f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('API_NUM_TRIES')}] filename from config {placeholderObj.filename}"
     )
     innerlog.debug(
-        f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('NUM_TRIES')}] full path from config {placeholderObj.filepath}"
+        f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('API_NUM_TRIES')}] full path from config {placeholderObj.filepath}"
     )
     innerlog.debug(
-        f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('NUM_TRIES')}] full path trunicated from config {placeholderObj.trunicated_filepath}"
+        f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('API_NUM_TRIES')}] full path trunicated from config {placeholderObj.trunicated_filepath}"
     )
 
 
 def temp_file_logger(placeholderObj, ele, innerlog=None):
     innerlog = innerlog or common_globals.log
     innerlog.debug(
-        f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('NUM_TRIES')}] filename from config {placeholderObj.tempfilepath}"
+        f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('API_NUM_TRIES')}] filename from config {placeholderObj.tempfilepath}"
     )
 
 
 def get_url_log(ele):
     url = ele.url or ele.mpd
     url = re.sub("/\w{5}\w+", "/{hidden}", url)
     if ele.url:
@@ -53,27 +53,28 @@
             f"In progress -> {format_size(common_globals.total_bytes )}) ({common_globals.photo_count+common_globals.audio_count+common_globals.video_count} \
 downloads total [{common_globals.video_count} videos, {common_globals.audio_count} audios, {common_globals.photo_count} photos], \
             {common_globals.forced_skipped} skipped, {common_globals.skipped} failed)"
         )
 
 
 def final_log(username, log=None):
-    skipped_word = "skipped"
-    (log or common_globals.log).warning(
-        f"[bold]{username}[/bold] ({format_size(common_globals.total_bytes )}) ({common_globals.photo_count+common_globals.audio_count+common_globals.video_count}"
-        f" downloads total [{common_globals.video_count} videos, {common_globals.audio_count} audios, {common_globals.photo_count} photos], "
-        f"{common_globals.forced_skipped} {skipped_word}, {common_globals.skipped} failed)"
-    )
+
     if read_args.retriveArgs().metadata:
         skipped_word = "media metadata unchanged"
-        (log or common_globals.log).warning(
+        (log or common_globals.log).error(
+            f"[bold]{username}[/bold] ({format_size(common_globals.total_bytes )}) ({common_globals.photo_count+common_globals.audio_count+common_globals.video_count}"
+            f" downloads total [{common_globals.video_count} videos, {common_globals.audio_count} audios, {common_globals.photo_count} photos], "
+            f"{common_globals.forced_skipped} {skipped_word}, {common_globals.skipped} failed)"
+        )
+    else:
+        skipped_word = "skipped"
+        (log or common_globals.log).error(
             f"[bold]{username}[/bold] ({format_size(common_globals.total_bytes )}) ({common_globals.photo_count+common_globals.audio_count+common_globals.video_count}"
             f" downloads total [{common_globals.video_count} videos, {common_globals.audio_count} audios, {common_globals.photo_count} photos], "
             f"{common_globals.forced_skipped} {skipped_word}, {common_globals.skipped} failed)"
         )
-        log.info("This only includes updates for the media table")
 
 
 def text_log(username, value=0, fails=0, exists=0, log=None):
     (log or common_globals.log).warning(
         f"[bold]{username}[/bold] {value} text, {exists} skipped, {fails} failed"
     )
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/common/message.py` & `ofscraper-3.9.1/ofscraper/download/shared/utils/message.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import platform
 
-import ofscraper.download.common.globals as common_globals
+import ofscraper.download.shared.globals as common_globals
 
 
 def set_send_msg():
     global send_msg_helper
     if platform.system() != "Windows":
         send_msg_helper = send_msg_unix
     else:
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/common/metadata.py` & `ofscraper-3.9.1/ofscraper/download/shared/utils/metadata.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,158 +1,114 @@
 import asyncio
 import pathlib
-import traceback
 from functools import partial
 
-from tenacity import AsyncRetrying, retry, stop_after_attempt, wait_random
-
 import ofscraper.classes.placeholder as placeholder
 import ofscraper.db.operations as operations
-import ofscraper.download.common.globals as common_globals
+import ofscraper.download.shared.common.general as common
+import ofscraper.download.shared.globals as common_globals
+import ofscraper.download.shared.utils.media as media
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
-from ofscraper.download.common.log import get_medialog
-from ofscraper.download.common.sem import sem_wrapper
+from ofscraper.download.shared.utils.log import get_medialog
+
+
+async def force_download(ele, username, model_id):
+    await operations.download_media_update(
+        ele,
+        filename=None,
+        model_id=model_id,
+        username=username,
+        downloaded=True,
+    )
 
 
 async def metadata(c, ele, username, model_id, placeholderObj=None):
     common_globals.log.info(
         f"{get_medialog(ele)} skipping adding download to disk because metadata is on"
     )
-    download_data = await asyncio.get_event_loop().run_in_executor(
-        common_globals.cache_thread, partial(cache.get, f"{ele.id}_headers")
+    placeholderObj = placeholderObj or await placeholderObjHelper(c, ele)
+    await placeholderObj.init()
+    common.add_additional_data(placeholderObj, ele)
+    effected = None
+    if ele.id:
+        effected = await operations.download_media_update(
+            ele,
+            filename=placeholderObj.trunicated_filepath,
+            model_id=model_id,
+            username=username,
+            downloaded=await metadata_downloaded_helper(placeholderObj),
+            changed=True,
+        )
+
+    return (
+        (ele.mediatype if effected else "forced_skipped"),
+        0,
     )
-    for _ in range(2):
-        if placeholderObj:
-            if ele.id:
-                await operations.download_media_update(
-                    ele,
-                    filename=placeholderObj.trunicated_filepath,
-                    model_id=model_id,
-                    username=username,
-                    downloaded=await metadata_downloaded_helper(placeholderObj),
-                )
-            return (
-                (
-                    ele.mediatype
-                    if await metadata_downloaded_helper(placeholderObj)
-                    else "forced_skipped"
-                ),
-                0,
-            )
-        elif download_data and download_data.get("content-type"):
-            content_type = download_data.get("content-type").split("/")[-1]
-            placeholderObj = await placeholder.Placeholders(ele, content_type).init()
-            if ele.id:
-                await operations.download_media_update(
-                    ele,
-                    filename=placeholderObj.trunicated_filepath,
-                    model_id=model_id,
-                    username=username,
-                    downloaded=await metadata_downloaded_helper(placeholderObj),
-                )
-            return (
-                (
-                    ele.mediatype
-                    if await metadata_downloaded_helper(placeholderObj)
-                    else "forced_skipped"
-                ),
-                0,
-            )
-        elif _ == 1:
-            break
-        else:
-            try:
-                async for _ in AsyncRetrying(
-                    stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-                    wait=wait_random(
-                        min=constants.getattr("OF_MIN"), max=constants.getattr("OF_MAX")
-                    ),
-                    reraise=True,
-                ):
-                    with _:
-                        try:
-                            placeholderObj = await metadata_helper(
-                                c, ele, placeholderObj
-                            )
-                        except Exception as E:
-                            raise E
-            except Exception as E:
-                common_globals.log.traceback_(
-                    f"{get_medialog(ele)} Could not get placeholderObj {E}"
-                )
-                common_globals.log.traceback_(
-                    f"{get_medialog(ele)} Could not get placeholderObj {traceback.format_exc()}"
-                )
-                common_globals.log.debug(
-                    f"{get_medialog(ele)} using a generic placeholderObj"
-                )
-                placeholderObj = await meta_data_placeholder(ele)
 
 
 async def metadata_downloaded_helper(placeholderObj):
-    placeholderObj = await placeholderObj.init()
     if read_args.retriveArgs().metadata == "none":
         return None
 
     elif read_args.retriveArgs().metadata == "complete":
         return 1
     elif pathlib.Path(placeholderObj.trunicated_filepath).exists():
         return 1
     return 0
 
 
-@sem_wrapper
-async def metadata_helper(c, ele, placeholderObj=None):
-    url = ele.url or ele.mpd
-
-    params = (
-        {
-            "Policy": ele.policy,
-            "Key-Pair-Id": ele.keypair,
-            "Signature": ele.signature,
-        }
-        if ele.mpd
-        else None
-    )
-    common_globals.attempt.set(common_globals.attempt.get() + 1)
-    common_globals.log.debug(
-        f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}]  Getting data for metadata insert"
-    )
-    async with c.requests(url=url, headers=None, params=params)() as r:
-        if r.ok:
+async def metadata_helper(c, ele):
+    if not ele.url and not ele.mpd:
+        placeholderObj = placeholder.Placeholders(
+            ele, ext=media.content_type_missing(ele)
+        )
+        return placeholderObj
+    else:
+        url = ele.url or ele.mpd
+        params = (
+            {
+                "Policy": ele.policy,
+                "Key-Pair-Id": ele.keypair,
+                "Signature": ele.signature,
+            }
+            if ele.mpd
+            else None
+        )
+        common_globals.attempt.set(common_globals.attempt.get() + 1)
+        common_globals.log.debug(
+            f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}]  Getting data for metadata insert"
+        )
+        async with c.requests_async(url=url, headers=None, params=params) as r:
             headers = r.headers
             await asyncio.get_event_loop().run_in_executor(
                 common_globals.cache_thread,
                 partial(
                     cache.set,
                     f"{ele.id}_headers",
                     {
                         "content-length": headers.get("content-length"),
                         "content-type": headers.get("content-type"),
                     },
                 ),
             )
-            content_type = headers.get("content-type").split("/")[-1]
-            if not content_type and ele.mediatype.lower() == "videos":
-                content_type = "mp4"
-            elif not content_type and ele.mediatype.lower() == "images":
-                content_type = "jpg"
+            content_type = headers.get("content-type").split("/")[
+                -1
+            ] or media.content_type_missing(ele)
             placeholderObj = await (
                 placeholderObj or placeholder.Placeholders(ele, ext=content_type)
             ).init()
             return placeholderObj
 
-        else:
-            r.raise_for_status()
 
-
-async def meta_data_placeholder(ele):
-    if ele.mediatype.lower() == "videos":
-        content_type = "mp4"
-    elif ele.mediatype.lower() == "images":
-        content_type = "jpg"
-    elif ele.mediatype.lower() == "audios":
-        content_type = "mp3"
-    placeholderObj = await placeholder.Placeholders(ele, ext=content_type).init()
-    return placeholderObj
+async def placeholderObjHelper(c, ele):
+    download_data = await asyncio.get_event_loop().run_in_executor(
+        common_globals.cache_thread, partial(cache.get, f"{ele.id}_headers")
+    )
+    if download_data:
+        content_type = download_data.get("content-type").split("/")[
+            -1
+        ] or media.content_type_missing(ele)
+        return placeholder.Placeholders(ele, content_type)
+    # final fallback
+    return await metadata_helper(c, ele)
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/common/paths.py` & `ofscraper-3.9.1/ofscraper/download/shared/utils/paths.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 import os
 import pathlib
 import platform
 import shutil
+from collections.abc import Iterable
 
-import ofscraper.download.common.globals as common_globals
+import ofscraper.download.shared.globals as common_globals
 import ofscraper.utils.dates as dates
 import ofscraper.utils.paths.common as common_paths
-from ofscraper.download.common.log import get_medialog
+from ofscraper.download.shared.utils.log import get_medialog
 
 try:
     from win32_setctime import setctime  # pylint: disable=import-error
 except ModuleNotFoundError:
     pass
 
 
@@ -26,23 +27,42 @@
     else:
         pathlib.Path(temp).unlink(missing_ok=True)
         log_ = log_ or logging.getLogger("shared")
         log_.debug(f"{get_medialog(ele)} smaller then previous file")
     # set variables based on parent process
 
 
-def addGlobalDir(input):
-    if isinstance(input, pathlib.Path):
-        common_globals.dirSet.add(input.parent)
-    else:
-        common_globals.dirSet.update(input)
+def addGlobalDir(path):
+    paths = [path] if not isinstance(path, Iterable) else path
+    paths = list(
+        map(
+            lambda x: (
+                path.resolve(x).parent
+                if not pathlib.Path(x).is_dir
+                else path.resolve(x)
+            ),
+            paths,
+        )
+    )
+    common_globals.dirSet.update(paths)
 
 
 def addLocalDir(path):
-    common_globals.localDirSet.add(path.resolve().parent)
+    paths = [path] if not isinstance(path, list) else path
+    paths = list(
+        map(
+            lambda x: (
+                path.resolve(x).parent
+                if not pathlib.Path(x).is_dir
+                else path.resolve(x)
+            ),
+            paths,
+        )
+    )
+    common_globals.dirSet.update(paths)
 
 
 def set_time(path, timestamp):
     if platform.system() == "Windows":
         setctime(path, timestamp)
     pathlib.os.utime(path, (timestamp, timestamp))
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/common/text.py` & `ofscraper-3.9.1/ofscraper/download/shared/utils/text.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import logging
 import traceback
 
 import ofscraper.classes.media as media_class
-import ofscraper.download.common.log as logs
+import ofscraper.download.shared.utils.log as logs
 import ofscraper.utils.settings as settings
 import ofscraper.utils.text as text
 from ofscraper.utils.context.run_async import run
 
 
 @run
 async def textDownloader(objectdicts, username=None):
     log = logging.getLogger("shared")
     if objectdicts == None:
         return
     try:
-        objectdicts = list(objectdicts)
+        objectdicts = (
+            [objectdicts] if not isinstance(objectdicts, list) else objectdicts
+        )
         if not "Text" in settings.get_mediatypes():
             log.info("Skipping Downloading of Text Files")
             return
         log.info("Downloading Text Files")
         data = (
             {
                 e.postid if isinstance(e, media_class.Media) else e.id: e
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/download.py` & `ofscraper-3.9.1/ofscraper/download/download.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,81 @@
+import json
 import logging
+import subprocess
+import traceback
 
 import ofscraper.db.operations as operations
 import ofscraper.download.downloadbatch as batchdownloader
 import ofscraper.download.downloadnormal as normaldownloader
 import ofscraper.filters.media.helpers as helpers
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.config.data as config_data
 import ofscraper.utils.constants as constants
 import ofscraper.utils.hash as hash
 import ofscraper.utils.separate as seperate
 import ofscraper.utils.settings as settings
 import ofscraper.utils.system.system as system
-from ofscraper.download.common.common import textDownloader
-from ofscraper.utils.context.run_async import run
+from ofscraper.download.shared.utils.text import textDownloader
 
 
 def medialist_filter(medialist, model_id, username):
     log = logging.getLogger("shared")
     if read_args.retriveArgs().force_all:
-        log.info(f"forcing all downloads media count {len(medialist)}")
+        log.info("forcing all")
     elif read_args.retriveArgs().force_model_unique:
-        log.info("Downloading unique for model")
+        log.info("Downloading unique medi afor model")
         media_ids = set(
             operations.get_media_ids_downloaded_model(
                 model_id=model_id, username=username
             )
         )
         log.debug(
             f"Number of unique media ids in database for {username}: {len(media_ids)}"
         )
         medialist = seperate.separate_by_id(medialist, media_ids)
         log.debug(f"Number of new mediaids with dupe ids removed: {len(medialist)}")
         medialist = seperate.seperate_avatars(medialist)
         log.debug("Removed previously downloaded avatars/headers")
         log.debug(f"Final Number of media to download {len(medialist)}")
     else:
-        log.info("Downloading unique across all models")
+        log.info("Downloading unique media across all models")
         media_ids = set(
             operations.get_media_ids_downloaded(model_id=model_id, username=username)
         )
         log.debug("Number of unique media ids in database for all models")
         medialist = seperate.separate_by_id(medialist, media_ids)
         log.debug(f"Number of new mediaids with dupe ids removed: {len(medialist)}")
         medialist = seperate.seperate_avatars(medialist)
         log.debug("Removed previously downloaded avatars/headers")
         log.debug(f"Final Number of media to download {len(medialist)} ")
     return medialist
 
 
 def download_process(username, model_id, medialist, posts=None):
-    medialist = medialist_filter(medialist, model_id, username)
-    medialist = helpers.ele_count_filter(medialist)
-    textDownloader(posts, username=username)
-    download_picker(username, model_id, medialist)
-    remove_downloads_with_hashes(username, model_id)
+    data = None
+    if read_args.retriveArgs().metadata:
+        medialist = (
+            list(filter(lambda x: x.canview, medialist))
+            if constants.getattr("REMOVE_UNVIEWABLE_METADATA")
+            else medialist
+        )
+        logging.getLogger().info(f"Final media count for metadata {len(medialist)}")
+        medialist = medialist_filter(medialist, model_id, username)
+        medialist = helpers.ele_count_filter(medialist)
+        data = download_picker(username, model_id, medialist)
+    else:
+        medialist = list(filter(lambda x: x.canview, medialist))
+        medialist = medialist_filter(medialist, model_id, username)
+        medialist = helpers.ele_count_filter(medialist)
+        logging.getLogger().info(f"Final media count for download {len(medialist)}")
+        textDownloader(posts, username=username)
+        data = download_picker(username, model_id, medialist)
+        remove_downloads_with_hashes(username, model_id)
+    download_post_process(username, model_id, medialist, posts)
+    return data
 
 
 def download_picker(username, model_id, medialist):
     if len(medialist) == 0:
         logging.getLogger("shared").error(
             f"[bold]{username}[/bold] ({0} photos, {0} videos, {0} audios,  {0} skipped, {0} failed)"
         )
@@ -75,7 +93,29 @@
         return normaldownloader.process_dicts(username, model_id, medialist)
 
 
 def remove_downloads_with_hashes(username, model_id):
     hash.remove_dupes_hash(username, model_id, "audios")
     hash.remove_dupes_hash(username, model_id, "images")
     hash.remove_dupes_hash(username, model_id, "videos")
+
+
+def download_post_process(username, model_id, medialist, postlist):
+    log = logging.getLogger("shared")
+    if not settings.get_post_download_script():
+        return
+    try:
+        mediadump = json.dumps(list(map(lambda x: x.media, medialist)))
+        postdump = json.dumps(list(map(lambda x: x.post, postlist)))
+        model_id = str(model_id)
+        subprocess.run(
+            [
+                settings.get_post_download_script(),
+                username,
+                model_id,
+                mediadump,
+                postdump,
+            ]
+        )
+    except Exception as e:
+        log.traceback_(e)
+        log.traceback_(traceback.format_exc())
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/downloadbatch.py` & `ofscraper-3.9.1/ofscraper/download/downloadbatch.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 
 import aioprocessing
 import more_itertools
 import psutil
 from aioprocessing import AioPipe
 from rich.live import Live
 
-import ofscraper.classes.sessionbuilder as sessionbuilder
-import ofscraper.download.common.common as common
-import ofscraper.download.common.globals as common_globals
+import ofscraper.download.shared.common.general as common
+import ofscraper.download.shared.globals as common_globals
 import ofscraper.models.selector as selector
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.console as console
 import ofscraper.utils.constants as constants
 import ofscraper.utils.context.exit as exit
 import ofscraper.utils.context.stdout as stdout
@@ -28,25 +27,24 @@
 import ofscraper.utils.logs.logger as logger
 import ofscraper.utils.logs.other as other_logs
 import ofscraper.utils.logs.stdout as stdout_logs
 import ofscraper.utils.manager as manager_
 import ofscraper.utils.settings as settings
 import ofscraper.utils.system.system as system
 from ofscraper.download.alt_downloadbatch import alt_download
-from ofscraper.download.common.common import (
-    addGlobalDir,
-    convert_num_bytes,
-    get_medialog,
-    log_download_progress,
-    setDirectoriesDate,
-    subProcessVariableInit,
-)
+from ofscraper.download.shared.common.general import get_medialog, subProcessVariableInit
+from ofscraper.download.shared.utils.log import final_log, log_download_progress
+from ofscraper.download.shared.utils.metadata import metadata
+from ofscraper.download.shared.utils.paths import addGlobalDir, setDirectoriesDate
+from ofscraper.download.shared.utils.progress import convert_num_bytes
 from ofscraper.download.main_downloadbatch import main_download
 from ofscraper.utils.context.run_async import run
 from ofscraper.utils.progress import setupDownloadProgressBar
+from ofscraper.download.shared.classes.session import download_session
+
 
 platform_name = platform.system()
 
 
 def process_dicts(username, model_id, filtered_medialist):
     log = logging.getLogger("shared")
     common_globals.log = log
@@ -96,26 +94,23 @@
         [process.start() for process in processes]
         progress_group, overall_progress, job_progress = setupDownloadProgressBar(
             multi=True
         )
 
         task1 = overall_progress.add_task(
             common_globals.desc.format(
-                p_count=common_globals.photo_count,
-                v_count=common_globals.video_count,
-                a_count=common_globals.audio_count,
-                skipped=common_globals.skipped,
+                p_count=0,
+                v_count=0,
+                a_count=0,
+                skipped=0,
                 mediacount=len(filtered_medialist),
-                sumcount=common_globals.video_count
-                + common_globals.audio_count
-                + common_globals.photo_count
-                + common_globals.skipped,
-                forced_skipped=common_globals.forced_skipped,
-                data=common_globals.data,
-                total=common_globals.total_data,
+                forced_skipped=0,
+                sumcount=0,
+                total_bytes_download=0,
+                total_bytes=0,
             ),
             total=len(filtered_medialist),
             visible=True,
         )
 
         # for reading completed downloads
         queue_threads = [
@@ -134,14 +129,15 @@
         ]
         [thread.start() for thread in queue_threads]
         with stdout.lowstdout():
             with Live(
                 progress_group,
                 refresh_per_second=constants.getattr("refreshScreen"),
                 console=console.get_shared_console(),
+                transient=True 
             ):
                 log.debug(f"Initial Queue Threads: {queue_threads}")
                 log.debug(f"Number of initial Queue Threads: {len(queue_threads)}")
                 while True:
                     newqueue_threads = list(
                         filter(lambda x: x and x.is_alive(), queue_threads)
                     )
@@ -205,15 +201,15 @@
                 raise E
         except KeyboardInterrupt:
             with exit.DelayedKeyboardInterrupt():
                 raise E
         except Exception:
             with exit.DelayedKeyboardInterrupt():
                 raise E
-    common.final_log(username)
+    final_log(username)
     return (
         common_globals.photo_count,
         common_globals.video_count,
         common_globals.audio_count,
         common_globals.forced_skipped,
         common_globals.skipped,
     )
@@ -232,67 +228,66 @@
         ):
             break
         results = pipe_.recv()
         if not isinstance(results, list):
             results = [results]
 
         for result in results:
-            if result is None:
-                count = count + 1
-                continue
-            if isinstance(result, dict) and not downloadprogress:
-                continue
-            if isinstance(result, set):
-                addGlobalDir(result)
-                continue
-            if isinstance(result, dict):
-                job_progress_helper(job_progress, result)
-                continue
-            media_type, num_bytes_downloaded, total_size = result
-            with common_globals.count_lock:
-                common_globals.total_bytes_downloaded = (
-                    common_globals.total_bytes_downloaded + num_bytes_downloaded
-                )
-                common_globals.total_bytes = common_globals.total_bytes + total_size
-                if media_type == "images":
-                    common_globals.photo_count += 1
-
-                elif media_type == "videos":
-                    common_globals.video_count += 1
-                elif media_type == "audios":
-                    common_globals.audio_count += 1
-                elif media_type == "skipped":
-                    common_globals.skipped += 1
-                elif media_type == "forced_skipped":
-                    common_globals.forced_skipped += 1
-                log_download_progress(media_type)
-                overall_progress.update(
-                    task1,
-                    description=common_globals.desc.format(
-                        p_count=common_globals.photo_count,
-                        v_count=common_globals.video_count,
-                        a_count=common_globals.audio_count,
-                        skipped=common_globals.skipped,
-                        forced_skipped=common_globals.forced_skipped,
-                        data=convert_num_bytes(common_globals.total_bytes_downloaded),
-                        total=convert_num_bytes(common_globals.total_bytes),
-                        mediacount=total,
-                        sumcount=common_globals.video_count
+            if isinstance(result, list) or isinstance(result, tuple):
+                media_type, num_bytes_downloaded, total_size = result
+                with common_globals.count_lock:
+                    common_globals.total_bytes_downloaded = (
+                        common_globals.total_bytes_downloaded + num_bytes_downloaded
+                    )
+                    common_globals.total_bytes = common_globals.total_bytes + total_size
+                    if media_type == "images":
+                        common_globals.photo_count += 1
+
+                    elif media_type == "videos":
+                        common_globals.video_count += 1
+                    elif media_type == "audios":
+                        common_globals.audio_count += 1
+                    elif media_type == "skipped":
+                        common_globals.skipped += 1
+                    elif media_type == "forced_skipped":
+                        common_globals.forced_skipped += 1
+                    log_download_progress(media_type)
+                    overall_progress.update(
+                        task1,
+                        description=common_globals.desc.format(
+                            p_count=common_globals.photo_count,
+                            v_count=common_globals.video_count,
+                            a_count=common_globals.audio_count,
+                            skipped=common_globals.skipped,
+                            forced_skipped=common_globals.forced_skipped,
+                            total_bytes_download=convert_num_bytes(
+                                common_globals.total_bytes_downloaded
+                            ),
+                            total_bytes=convert_num_bytes(common_globals.total_bytes),
+                            mediacount=total,
+                            sumcount=common_globals.video_count
+                            + common_globals.audio_count
+                            + common_globals.photo_count
+                            + common_globals.skipped
+                            + common_globals.forced_skipped,
+                        ),
+                        refresh=True,
+                        completed=common_globals.video_count
                         + common_globals.audio_count
                         + common_globals.photo_count
                         + common_globals.skipped
                         + common_globals.forced_skipped,
-                    ),
-                    refresh=True,
-                    completed=common_globals.video_count
-                    + common_globals.audio_count
-                    + common_globals.photo_count
-                    + common_globals.skipped
-                    + common_globals.forced_skipped,
-                )
+                    )
+
+            elif result is None:
+                count = count + 1
+            elif isinstance(result, dict) and "dir_update" in result:
+                addGlobalDir(result["dir_update"])
+            elif isinstance(result, dict) and downloadprogress:
+                job_progress_helper(job_progress, result)
 
 
 def get_mediasplits(medialist):
     user_count = settings.get_threads()
     final_count = max(min(user_count, system.getcpu_count(), len(medialist) // 5), 1)
     return more_itertools.divide(final_count, medialist)
 
@@ -367,70 +362,70 @@
 
 
 @run
 async def process_dicts_split(username, model_id, medialist):
     common_globals.log.debug(f"{pid_log_helper()} start inner thread for other loggers")
     # set variables based on parent process
     # start consumer for other
-    other_thread = other_logs.start_other_thread(
+    other_logs.start_other_thread(
         input_=common_globals.log.handlers[1].queue, name=str(os.getpid()), count=1
     )
     medialist = list(medialist)
     # This need to be here: https://stackoverflow.com/questions/73599594/asyncio-works-in-python-3-10-but-not-in-python-3-8
 
     common_globals.log.debug(f"{pid_log_helper()} starting process")
     common_globals.log.debug(
         f"{pid_log_helper()} process mediasplit from total {len(medialist)}"
     )
-
     aws = []
-    async with sessionbuilder.sessionBuilder() as c:
+    async with download_session() as c:
         for ele in medialist:
             aws.append(asyncio.create_task(download(c, ele, model_id, username)))
         for coro in asyncio.as_completed(aws):
             try:
                 pack = await coro
                 common_globals.log.debug(f"unpack {pack} count {len(pack)}")
                 media_type, num_bytes_downloaded = pack
                 await common.send_msg((media_type, num_bytes_downloaded, 0))
             except Exception as e:
-                common_globals.log.traceback_(f"Download Failed because\n{e}")
+                common_globals.log.info(f"Download Failed because\n{e}")
                 common_globals.log.traceback_(traceback.format_exc())
                 media_type = "skipped"
                 num_bytes_downloaded = 0
                 await common.send_msg((media_type, num_bytes_downloaded, 0))
 
     common_globals.log.debug(f"{pid_log_helper()} download process thread closing")
     # send message directly
     await asyncio.get_event_loop().run_in_executor(
         common_globals.cache_thread, cache.close
     )
     common_globals.cache_thread.shutdown()
     common_globals.log.handlers[0].queue.put("None")
     common_globals.log.handlers[1].queue.put("None")
-    other_thread.join() if other_thread else None
     common_globals.log.debug("other thread closed")
-    await common.send_msg(common_globals.localDirSet)
+    await common.send_msg({"dir_update": common_globals.localDirSet})
     await common.send_msg(None)
 
 
 def pid_log_helper():
     return f"PID: {os.getpid()}"
 
 
 async def download(c, ele, model_id, username):
     async with common_globals.maxfile_sem:
         templog_ = logger.get_shared_logger(
             name=str(ele.id), main_=aioprocessing.Queue(), other_=aioprocessing.Queue()
         )
         common_globals.innerlog.set(templog_)
         try:
-            if ele.url:
+            if read_args.retriveArgs().metadata:
+                return await metadata(c, ele, username, model_id)
+            elif ele.url:
                 return await main_download(c, ele, username, model_id)
-            if ele.mpd:
+            elif ele.mpd:
                 return await alt_download(c, ele, username, model_id)
         except Exception as e:
             common_globals.innerlog.get().traceback_(
                 f"{get_medialog(ele)} Download Failed\n{e}"
             )
             common_globals.innerlog.get().traceback_(
                 f"{get_medialog(ele)} exception {traceback.format_exc()}"
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/downloadnormal.py` & `ofscraper-3.9.1/ofscraper/download/downloadnormal.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,36 +14,36 @@
 import asyncio
 import logging
 import traceback
 
 from humanfriendly import format_size
 from rich.live import Live
 
-import ofscraper.classes.sessionbuilder as sessionbuilder
-import ofscraper.download.common.common as common
-import ofscraper.download.common.globals as common_globals
+import ofscraper.download.shared.globals as common_globals
+import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.console as console
 import ofscraper.utils.constants as constants
 import ofscraper.utils.context.exit as exit
 import ofscraper.utils.context.stdout as stdout
 import ofscraper.utils.logs.logger as logger
 import ofscraper.utils.logs.other as other_logs
 import ofscraper.utils.logs.stdout as stdout_logs
 import ofscraper.utils.manager as manager_
 from ofscraper.download.alt_download import alt_download
-from ofscraper.download.common.common import (
-    convert_num_bytes,
-    get_medialog,
-    log_download_progress,
-    setDirectoriesDate,
-)
+from ofscraper.download.shared.common.general import get_medialog
+from ofscraper.download.shared.utils.log import final_log, log_download_progress
+from ofscraper.download.shared.utils.metadata import metadata
+from ofscraper.download.shared.utils.paths import setDirectoriesDate
+from ofscraper.download.shared.utils.progress import convert_num_bytes
 from ofscraper.download.main_download import main_download
 from ofscraper.utils.context.run_async import run
 from ofscraper.utils.progress import setupDownloadProgressBar
+from ofscraper.download.shared.classes.session import download_session
+
 
 
 @run
 async def process_dicts(username, model_id, medialist):
     with stdout.lowstdout():
         progress_group, overall_progress, job_progress = setupDownloadProgressBar()
         # This need to be here: https://stackoverflow.com/questions/73599594/asyncio-works-in-python-3-10-but-not-in-python-3-8
@@ -64,48 +64,48 @@
             other_thread = other_logs.start_other_thread(
                 input_=otherqueue, name="ofscraper_normal_other"
             )
             with Live(
                 progress_group,
                 refresh_per_second=constants.getattr("refreshScreen"),
                 console=console.shared_console,
+                transient=True 
             ):
                 aws = []
-                desc = "Progress: ({p_count} photos, {v_count} videos, {a_count} audios, {forced_skipped} skipped, {skipped} failed || {sumcount}/{mediacount}||{total_bytes_download}/{total_bytes})"
 
-                async with sessionbuilder.sessionBuilder() as c:
+                async with download_session() as c:
                     for ele in medialist:
                         aws.append(
                             asyncio.create_task(
                                 download(c, ele, model_id, username, job_progress)
                             )
                         )
                     task1 = overall_progress.add_task(
-                        desc.format(
-                            p_count=common_globals.photo_count,
-                            v_count=common_globals.video_count,
-                            a_count=common_globals.audio_count,
-                            skipped=common_globals.skipped,
+                        common_globals.desc.format(
+                            p_count=0,
+                            v_count=0,
+                            a_count=0,
+                            skipped=0,
                             mediacount=len(medialist),
-                            forced_skipped=common_globals.forced_skipped,
+                            forced_skipped=0,
                             sumcount=0,
                             total_bytes_download=0,
                             total_bytes=0,
                         ),
                         total=len(aws),
                         visible=True,
                     )
                     for coro in asyncio.as_completed(aws):
                         try:
                             pack = await coro
                             common_globals.log.debug(f"unpack {pack} count {len(pack)}")
                             media_type, num_bytes_downloaded = pack
                         except Exception as e:
-                            common_globals.log.traceback_(
-                                f"Download Failed because\n{e}"
+                            common_globals.log.info(
+                                f"{get_medialog(ele)} Download Failed because\n{e}"
                             )
                             common_globals.log.traceback_(traceback.format_exc())
                             media_type = "skipped"
                             num_bytes_downloaded = 0
 
                         common_globals.total_bytes_downloaded = (
                             common_globals.total_bytes_downloaded + num_bytes_downloaded
@@ -127,15 +127,15 @@
                             + common_globals.audio_count
                             + common_globals.skipped
                             + common_globals.forced_skipped
                         )
                         log_download_progress(media_type)
                         overall_progress.update(
                             task1,
-                            description=desc.format(
+                            description=common_globals.desc.format(
                                 p_count=common_globals.photo_count,
                                 v_count=common_globals.video_count,
                                 a_count=common_globals.audio_count,
                                 skipped=common_globals.skipped,
                                 forced_skipped=common_globals.forced_skipped,
                                 mediacount=len(medialist),
                                 sumcount=sum_count,
@@ -152,15 +152,15 @@
             overall_progress.remove_task(task1)
             setDirectoriesDate()
             # close thread
             otherqueue.put("None")
             logqueue.put("None")
             log_thread.join()
             other_thread.join() if other_thread else None
-            common.final_log(username, log=logging.getLogger("shared"))
+            final_log(username, log=logging.getLogger("shared"))
             return (
                 common_globals.photo_count,
                 common_globals.video_count,
                 common_globals.audio_count,
                 common_globals.forced_skipped,
                 common_globals.skipped,
             )
@@ -174,15 +174,17 @@
             )
             common_globals.cache_thread.shutdown()
 
 
 async def download(c, ele, model_id, username, job_progress):
     async with common_globals.maxfile_sem:
         try:
-            if ele.url:
+            if read_args.retriveArgs().metadata:
+                return await metadata(c, ele, username, model_id)
+            elif ele.url:
                 return await main_download(
                     c,
                     ele,
                     username,
                     model_id,
                     job_progress,
                 )
@@ -190,13 +192,14 @@
                 return await alt_download(
                     c,
                     ele,
                     username,
                     model_id,
                     job_progress,
                 )
+
         except Exception as E:
             common_globals.log.debug(f"{get_medialog(ele)} exception {E}")
             common_globals.log.debug(
                 f"{get_medialog(ele)} exception {traceback.format_exc()}"
             )
             return "skipped", 0
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/main_download.py` & `ofscraper-3.9.1/ofscraper/download/main_downloadbatch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-r"""
+"""
                                                              
  _______  _______         _______  _______  _______  _______  _______  _______  _______ 
 (  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
 | (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
@@ -13,340 +13,258 @@
 
 import asyncio
 import pathlib
 import traceback
 from functools import partial
 
 import aiofiles
-import arrow
-import psutil
-from tenacity import (
-    AsyncRetrying,
-    retry_if_not_exception_message,
-    stop_after_attempt,
-    wait_random,
-)
 
 try:
     from win32_setctime import setctime  # pylint: disable=import-error
 except ModuleNotFoundError:
     pass
 import ofscraper.classes.placeholder as placeholder
-import ofscraper.db.operations as operations
-import ofscraper.download.common.common as common
-import ofscraper.download.common.globals as common_globals
-import ofscraper.utils.args.read as read_args
+import ofscraper.download.shared.common.general as common
+import ofscraper.download.shared.globals as common_globals
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
-import ofscraper.utils.dates as dates
-import ofscraper.utils.paths.paths as paths
 import ofscraper.utils.settings as settings
-from ofscraper.download.common.common import (
-    addGlobalDir,
+import ofscraper.utils.system.system as system
+from ofscraper.download.shared.common.general import (
     check_forced_skip,
     downloadspace,
     get_data,
     get_medialog,
     get_resume_size,
     get_unknown_content_type,
-    get_url_log,
-    metadata,
-    moveHelper,
-    path_to_file_logger,
-    sem_wrapper,
-    set_profile_cache_helper,
-    set_time,
     size_checker,
 )
+from ofscraper.download.shared.utils.log import get_url_log, path_to_file_logger
+from ofscraper.download.shared.common.main_common import handle_result_main
+from ofscraper.download.shared.utils.metadata import force_download
+from ofscraper.download.shared.classes.retries import download_retry
 
 
-async def main_download(c, ele, username, model_id, job_progress):
-    common_globals.log.debug(f"{get_medialog(ele)} Downloading with normal downloader")
-    common_globals.log.debug(f"{get_medialog(ele)} download url:  {get_url_log(ele)}")
-    # total may be none if no .part file
-    if read_args.retriveArgs().metadata != None:
-        return await metadata(
-            c,
-            ele,
-            username,
-            model_id,
-        )
-    result = await main_download_downloader(
-        c,
-        ele,
-        job_progress,
-    )
-    # special case for zero byte files
-    if result[0] == 0:
-        if ele.mediatype != "forced_skipped":
-            await operations.download_media_update(
-                ele,
-                filename=None,
-                model_id=model_id,
-                username=username,
-                downloaded=True,
-            )
-        return ele.mediatype, 0
-    return await handle_result(result, ele, username, model_id)
-
 
-async def handle_result(result, ele, username, model_id):
-    total, temp, placeholderObj = result
-    path_to_file = placeholderObj.trunicated_filepath
-    await size_checker(temp, ele, total)
-    common_globals.log.debug(
-        f"{get_medialog(ele)} {await ele.final_filename} size match target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}"
+async def main_download(c, ele, username, model_id):
+    common_globals.innerlog.get().debug(
+        f"{get_medialog(ele)} Downloading with normal batch downloader"
     )
-    common_globals.log.debug(
-        f"{get_medialog(ele)} renaming {pathlib.Path(temp).absolute()} -> {path_to_file}"
+    common_globals.innerlog.get().debug(
+        f"{get_medialog(ele)} download url: {get_url_log(ele)}"
     )
-    moveHelper(temp, path_to_file, ele)
-    addGlobalDir(placeholderObj.filedir)
-    if ele.postdate:
-        newDate = dates.convert_local_time(ele.postdate)
+    if common.is_bad_url(ele.url):
         common_globals.log.debug(
-            f"{get_medialog(ele)} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}"
-        )
-        set_time(path_to_file, newDate)
-        common_globals.log.debug(
-            f"{get_medialog(ele)} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}"
+            f"{get_medialog(ele)} Forcing download because known bad url"
         )
+        await force_download(ele, username, model_id)
+        return ele.mediatype, 0
 
-    if ele.id:
-        await operations.download_media_update(
-            ele,
-            filename=path_to_file,
-            model_id=model_id,
-            username=username,
-            downloaded=True,
-            hashdata=await common.get_hash(path_to_file, mediatype=ele.mediatype),
-        )
-    await set_profile_cache_helper(ele)
-    return ele.mediatype, total
+    result = list(await main_download_downloader(c, ele))
+    if result[0] == 0:
+        if ele.mediatype != "forced_skipped":
+            await force_download(ele, username, model_id)
+        return ele.mediatype, 0
+    return await handle_result_main(result, ele, username, model_id)
 
 
-async def main_download_downloader(c, ele, job_progress):
+async def main_download_downloader(c, ele):
     downloadspace(mediatype=ele.mediatype)
     tempholderObj = await placeholder.tempFilePlaceholder(
         ele, f"{await ele.final_filename}_{ele.id}.part"
     ).init()
-    async for _ in AsyncRetrying(
-        stop=stop_after_attempt(constants.getattr("DOWNLOAD_RETRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"), max=constants.getattr("OF_MAX")
-        ),
-        retry=retry_if_not_exception_message(
-            constants.getattr("SPACE_DOWNLOAD_MESSAGE")
-        ),
-        reraise=True,
-    ):
+    async for _ in download_retry():
         with _:
             try:
-                data = await get_data(ele)
                 common_globals.attempt.set(common_globals.attempt.get(0) + 1)
                 (
                     pathlib.Path(tempholderObj.tempfilepath).unlink(missing_ok=True)
                     if common_globals.attempt.get() > 1
                     else None
                 )
+                data = await get_data(ele)
                 if data:
-                    return await main_data_handler(
-                        data, c, tempholderObj, ele, job_progress
-                    )
+                    return await main_data_handler(data, c, ele, tempholderObj)
                 else:
-                    return await alt_data_handler(c, tempholderObj, ele, job_progress)
+                    return await alt_data_handler(c, ele, tempholderObj)
+
             except OSError as E:
-                await asyncio.sleep(1)
-                common_globals.log.debug(
-                    f"[attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] Number of Open Files -> { len(psutil.Process().open_files())}"
+                common_globals.innerlog.get().debug(
+                    f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] Number of open Files across all processes-> {len(system.getOpenFiles(unique=False))}"
                 )
-                common_globals.log.debug(
-                    f"[attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] Open Files  -> {list(map(lambda x:(x.path,x.fd),psutil.Process().open_files()))}"
+                common_globals.innerlog.get().debug(
+                    f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] Number of unique open files across all processes-> {len(system.getOpenFiles())}"
+                )
+                common_globals.innerlog.get().debug(
+                    f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] Unique files data across all process -> {list(map(lambda x:(x.path,x.fd),(system.getOpenFiles())))}"
                 )
                 raise E
             except Exception as E:
-                await asyncio.sleep(1)
-                common_globals.log.traceback_(
-                    f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] {traceback.format_exc()}"
+                common_globals.innerlog.get().traceback_(
+                    f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] {traceback.format_exc()}"
                 )
-                common_globals.log.traceback_(
-                    f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] {E}"
+                common_globals.innerlog.get().traceback_(
+                    f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] {E}"
                 )
                 raise E
 
 
-async def alt_data_handler(c, tempholderObj, ele, job_progress):
+async def alt_data_handler(c, ele, tempholderObj):
     result = None
     try:
         result = await main_download_sendreq(
-            c, ele, tempholderObj, job_progress, placeholderObj=None, total=None
+            c, ele, tempholderObj, placeholderObj=None, total=None
         )
     except Exception as E:
         raise E
     return result
 
 
-async def main_data_handler(data, c, tempholderObj, ele, job_progress):
+async def main_data_handler(data, c, ele, tempholderObj):
     content_type = data.get("content-type").split("/")[-1]
     total = int(data.get("content-length"))
     placeholderObj = await placeholder.Placeholders(ele, content_type).init()
     resume_size = get_resume_size(tempholderObj, mediatype=ele.mediatype)
     # other
     if await check_forced_skip(ele, total) == 0:
-        path_to_file_logger(placeholderObj, ele)
+        path_to_file_logger(placeholderObj, ele, common_globals.innerlog.get())
         return [0]
     elif total == resume_size:
-        path_to_file_logger(placeholderObj, ele)
+        path_to_file_logger(placeholderObj, ele, common_globals.innerlog.get())
         return (
             total,
             tempholderObj.tempfilepath,
             placeholderObj,
         )
 
     else:
         try:
             return await main_download_sendreq(
-                c,
-                ele,
-                tempholderObj,
-                job_progress,
-                total=total,
-                placeholderObj=placeholderObj,
+                c, ele, tempholderObj, total=total, placeholderObj=placeholderObj
             )
         except Exception as E:
             raise E
 
 
-async def main_download_sendreq(
-    c, ele, tempholderObj, job_progress, total=None, placeholderObj=None
-):
+async def main_download_sendreq(c, ele, tempholderObj, placeholderObj=None, total=None):
     try:
-        common_globals.log.debug(
-            f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] download temp path {tempholderObj.tempfilepath}"
+        common_globals.innerlog.get().debug(
+            f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] download temp path {tempholderObj.tempfilepath}"
         )
         total = total if common_globals.attempt.get() == 1 else None
         return await send_req_inner(
-            c,
-            ele,
-            tempholderObj,
-            job_progress,
-            placeholderObj=placeholderObj,
-            total=total,
+            c, ele, tempholderObj, placeholderObj=placeholderObj, total=total
         )
     except OSError as E:
         raise E
     except Exception as E:
         raise E
 
 
-async def send_req_inner(
-    c, ele, tempholderObj, job_progress, placeholderObj=None, total=None
-):
+async def send_req_inner(c, ele, tempholderObj, placeholderObj=None, total=None):
     old_total = total
     try:
-        await common.total_change_helper(None, total)
+        await common.batch_total_change_helper(None, total)
         resume_size = get_resume_size(tempholderObj, mediatype=ele.mediatype)
         headers = (
             None
-            if resume_size == 0 or not total
+            if resume_size == 0 or not old_total
             else {"Range": f"bytes={resume_size}-{total}"}
         )
-        async with sem_wrapper(common_globals.req_sem):
-            async with c.requests(url=ele.url, headers=headers)() as r:
-                if r.ok:
-                    await asyncio.get_event_loop().run_in_executor(
-                        common_globals.cache_thread,
-                        partial(
-                            cache.set,
-                            f"{ele.id}_headers",
-                            {
-                                "content-length": r.headers.get("content-length"),
-                                "content-type": r.headers.get("content-type"),
-                            },
-                        ),
-                    )
-                    new_total = int(r.headers["content-length"])
-                    content_type = r.headers.get("content-type").split("/")[-1]
-                    content_type = content_type or get_unknown_content_type(ele)
-                    if not placeholderObj:
-                        placeholderObj = await placeholder.Placeholders(
-                            ele, content_type
-                        ).init()
-                    path_to_file_logger(placeholderObj, ele)
-                    if await check_forced_skip(ele, new_total):
-                        total = 0
-                        await common.total_change_helper(old_total, total)
-                    elif total == resume_size:
-                        None
-                    else:
-                        total = new_total
-                        await common.total_change_helper(old_total, total)
-                        await download_fileobject_writer(
-                            r, job_progress, ele, tempholderObj, placeholderObj, total
-                        )
-                else:
-                    common_globals.log.debug(
-                        f"[bold] {get_medialog(ele)} main download response status code [/bold]: {r.status}"
-                    )
-                    common_globals.log.debug(
-                        f"[bold] {get_medialog(ele)}  main download  response text [/bold]: {await r.text_()}"
-                    )
-                    common_globals.log.debug(
-                        f"[bold] {get_medialog(ele)}  main download headers [/bold]: {r.headers}"
-                    )
-                    r.raise_for_status()
-
+        common_globals.log.debug(
+            f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] Downloading media with url {ele.url}"
+        )
+        async with c.requests_async(url=ele.url, headers=headers) as r:
+            await asyncio.get_event_loop().run_in_executor(
+                common_globals.cache_thread,
+                partial(
+                    cache.set,
+                    f"{ele.id}_headers",
+                    {
+                        "content-length": r.headers.get("content-length"),
+                        "content-type": r.headers.get("content-type"),
+                    },
+                ),
+            )
+            new_total = int(r.headers["content-length"])
+            content_type = r.headers.get("content-type").split("/")[
+                -1
+            ] or get_unknown_content_type(ele)
+            if not placeholderObj:
+                placeholderObj = await placeholder.Placeholders(
+                    ele, content_type
+                ).init()
+            path_to_file_logger(placeholderObj, ele, common_globals.innerlog.get())
+            if await check_forced_skip(ele, new_total) == 0:
+                total = 0
+                await common.batch_total_change_helper(old_total, total)
+                return (total, tempholderObj.tempfilepath, placeholderObj)
+            elif total != resume_size:
+                total = new_total
+                await common.batch_total_change_helper(old_total, total)
+                await download_fileobject_writer(
+                    r, ele, total, tempholderObj, placeholderObj
+                )
         await size_checker(tempholderObj.tempfilepath, ele, total)
         return (total, tempholderObj.tempfilepath, placeholderObj)
     except Exception as E:
-        await common.total_change_helper(None, -(total or 0))
+        await common.batch_total_change_helper(None, -(total or 0))
         raise E
 
 
-async def download_fileobject_writer(
-    r, job_progress, ele, tempholderObj, placeholderObj, total
-):
+async def download_fileobject_writer(r, ele, total, tempholderObj, placeholderObj):
     pathstr = str(placeholderObj.trunicated_filepath)
     downloadprogress = settings.get_download_bars()
-    task1 = job_progress.add_task(
-        f"{(pathstr[:constants.getattr('PATH_STR_MAX')] + '....') if len(pathstr) > constants.getattr('PATH_STR_MAX') else pathstr}\n",
-        total=total,
-        visible=True if downloadprogress else False,
-    )
     try:
         count = 0
-        loop = asyncio.get_event_loop()
+        await common.send_msg(
+            {
+                "type": "add_task",
+                "args": (
+                    f"{(pathstr[:constants.getattr('PATH_STR_MAX')] + '....') if len(pathstr) > constants.getattr('PATH_STR_MAX') else pathstr}\n",
+                    ele.id,
+                ),
+                "total": total,
+                "visible": False,
+            }
+        )
+
         fileobject = await aiofiles.open(tempholderObj.tempfilepath, "ab").__aenter__()
         download_sleep = constants.getattr("DOWNLOAD_SLEEP")
 
-        async for chunk in r.iter_chunked(constants.getattr("maxChunkSize")):
+        await common.send_msg({"type": "update", "args": (ele.id,), "visible": True})
+        async for chunk in r.iter_chunked(constants.getattr("maxChunkSizeB")):
+            count = count + 1
             if downloadprogress:
                 count = count + 1
-            await fileobject.write(chunk)
-            common_globals.log.trace(
+            common_globals.innerlog.get().trace(
                 f"{get_medialog(ele)} Download Progress:{(pathlib.Path(tempholderObj.tempfilepath).absolute().stat().st_size)}/{total}"
             )
-            if (count + 1) % constants.getattr("CHUNK_ITER") == 0:
-                await loop.run_in_executor(
-                    common_globals.thread,
-                    partial(
-                        job_progress.update,
-                        task1,
-                        completed=pathlib.Path(tempholderObj.tempfilepath)
-                        .absolute()
-                        .stat()
-                        .st_size,
-                    ),
+            await fileobject.write(chunk)
+            if count == constants.getattr("CHUNK_ITER"):
+                await common.send_msg(
+                    {
+                        "type": "update",
+                        "args": (ele.id,),
+                        "completed": (
+                            pathlib.Path(tempholderObj.tempfilepath)
+                            .absolute()
+                            .stat()
+                            .st_size
+                        ),
+                    }
                 )
+                count = 0
             (await asyncio.sleep(download_sleep)) if download_sleep else None
     except Exception as E:
+        # reset download data
         raise E
     finally:
-        # Close file if needed
         try:
-            await fileobject.close()
-        except Exception:
+            await common.send_msg({"type": "remove_task", "args": (ele.id,)})
+        except:
             None
+
         try:
-            job_progress.remove_task(task1)
+            await fileobject.close()
         except Exception:
             None
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/download/main_downloadbatch.py` & `ofscraper-3.9.1/ofscraper/download/alt_download.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,349 +1,277 @@
-"""
+r"""
                                                              
  _______  _______         _______  _______  _______  _______  _______  _______  _______ 
 (  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
 | (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
 | |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
 | |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
 import asyncio
 import pathlib
+import re
 import traceback
 from functools import partial
 
 import aiofiles
-import arrow
-from tenacity import (
-    AsyncRetrying,
-    retry_if_not_exception_message,
-    stop_after_attempt,
-    wait_random,
-)
-
+import psutil
 try:
     from win32_setctime import setctime  # pylint: disable=import-error
 except ModuleNotFoundError:
     pass
 import ofscraper.classes.placeholder as placeholder
-import ofscraper.db.operations as operations
-import ofscraper.download.common.common as common
-import ofscraper.download.common.globals as common_globals
-import ofscraper.utils.args.read as read_args
+import ofscraper.download.shared.common.general as common
+import ofscraper.download.shared.globals as common_globals
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
-import ofscraper.utils.dates as dates
 import ofscraper.utils.settings as settings
-import ofscraper.utils.system.system as system
-from ofscraper.download.common.common import (
-    addLocalDir,
+from ofscraper.download.shared.common.alt_common import (
+    handle_result_alt,
+    media_item_keys_alt,
+    media_item_post_process_alt,
+)
+from ofscraper.download.shared.common.general import (
     check_forced_skip,
     downloadspace,
-    get_data,
     get_medialog,
     get_resume_size,
-    get_unknown_content_type,
+    size_checker,
+)
+from ofscraper.download.shared.utils.log import (
     get_url_log,
-    metadata,
-    moveHelper,
     path_to_file_logger,
-    sem_wrapper,
-    set_profile_cache_helper,
-    set_time,
-    size_checker,
+    temp_file_logger,
 )
-from ofscraper.utils.context.run_async import run
 
+from ofscraper.download.shared.classes.retries import (
+    download_retry
+)
 
-async def main_download(c, ele, username, model_id):
-    common_globals.innerlog.get().debug(
-        f"{get_medialog(ele)} Downloading with normal batch downloader"
-    )
-    common_globals.innerlog.get().debug(
-        f"{get_medialog(ele)} download url: {get_url_log(ele)}"
+
+async def alt_download(c, ele, username, model_id, job_progress):
+    common_globals.log.debug(
+        f"{get_medialog(ele)} Downloading with protected media downloader"
     )
-    if read_args.retriveArgs().metadata != None:
-        return await metadata(
-            c,
-            ele,
-            username,
-            model_id,
-        )
+    async for _ in download_retry():
+        with _:
+            try:
+                sharedPlaceholderObj = await placeholder.Placeholders(ele, "mp4").init()
+                common_globals.log.debug(f"{get_medialog(ele)} download url:  {get_url_log(ele)}")
+            except Exception as e:
+                raise e
 
-    result = list(await main_download_downloader(c, ele))
-    if result[0] == 0:
-        if ele.mediatype != "forced_skipped":
-            await operations.download_media_update(
-                ele,
-                filename=None,
-                model_id=model_id,
-                username=username,
-                downloaded=True,
-            )
-        return ele.mediatype, 0
-    return await handle_result(result, ele, username, model_id)
+    audio, video = await ele.mpd_dict
+    path_to_file_logger(sharedPlaceholderObj, ele)
 
+    audio = await alt_download_downloader(audio, c, ele, job_progress)
+    video = await alt_download_downloader(video, c, ele, job_progress)
 
-async def handle_result(result, ele, username, model_id):
-    total, temp_path, placeholderObj = result
-    path_to_file = placeholderObj.trunicated_filepath
-    await size_checker(temp_path, ele, total, path_to_file)
-    common_globals.innerlog.get().debug(
-        f"{get_medialog(ele)} { await ele.final_filename} size match target: {total} vs actual: {pathlib.Path(temp_path).absolute().stat().st_size}"
+    post_result = await media_item_post_process_alt(
+        audio, video, ele, username, model_id
     )
-    common_globals.innerlog.get().debug(
-        f"{get_medialog(ele)} renaming {pathlib.Path(temp_path).absolute()} -> {path_to_file}"
+    if post_result:
+        return post_result
+    await media_item_keys_alt(c, audio, video, ele)
+
+    return await handle_result_alt(
+        sharedPlaceholderObj, ele, audio, video, username, model_id
     )
-    moveHelper(temp_path, path_to_file, ele, common_globals.innerlog.get())
-    addLocalDir(placeholderObj.filedir)
-    if ele.postdate:
-        newDate = dates.convert_local_time(ele.postdate)
-        common_globals.innerlog.get().debug(
-            f"{get_medialog(ele)} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}"
-        )
-        set_time(path_to_file, newDate)
-        common_globals.innerlog.get().debug(
-            f"{get_medialog(ele)} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}"
-        )
-    if ele.id:
-        await operations.download_media_update(
-            ele,
-            filename=path_to_file,
-            model_id=model_id,
-            username=username,
-            downloaded=True,
-            hashdata=await common.get_hash(path_to_file, mediatype=ele.mediatype),
-        )
-    await set_profile_cache_helper(ele)
-    return ele.mediatype, total
 
 
-async def main_download_downloader(c, ele):
+async def alt_download_downloader(item, c, ele, job_progress):
     downloadspace(mediatype=ele.mediatype)
-    tempholderObj = await placeholder.tempFilePlaceholder(
-        ele, f"{await ele.final_filename}_{ele.id}.part"
+    placeholderObj = await placeholder.tempFilePlaceholder(
+        ele, f"{item['name']}.part"
     ).init()
-    async for _ in AsyncRetrying(
-        stop=stop_after_attempt(constants.getattr("DOWNLOAD_RETRIES")),
-        wait=wait_random(
-            min=constants.getattr("OF_MIN"), max=constants.getattr("OF_MAX")
-        ),
-        retry=retry_if_not_exception_message(
-            constants.getattr("SPACE_DOWNLOAD_MESSAGE")
-        ),
-        reraise=True,
-    ):
+    item["path"] = placeholderObj.tempfilepath
+    item["total"] = None
+    async for _ in download_retry():
         with _:
             try:
-                common_globals.attempt.set(common_globals.attempt.get(0) + 1)
+                _attempt = common.alt_attempt_get(item)
+                _attempt.set(_attempt.get(0) + 1)
                 (
-                    pathlib.Path(tempholderObj.tempfilepath).unlink(missing_ok=True)
-                    if common_globals.attempt.get() > 1
+                    pathlib.Path(placeholderObj.tempfilepath).unlink(missing_ok=True)
+                    if _attempt.get() > 1
                     else None
                 )
-                data = await get_data(ele)
+                data = await asyncio.get_event_loop().run_in_executor(
+                    common_globals.cache_thread,
+                    partial(cache.get, f"{item['name']}_headers"),
+                )
                 if data:
-                    return await main_data_handler(data, c, ele, tempholderObj)
-                else:
-                    return await alt_data_handler(c, ele, tempholderObj)
+                    return await main_data_handler(
+                        data, item, c, ele, placeholderObj, job_progress
+                    )
 
+                else:
+                    return await alt_data_handler(
+                        item, c, ele, placeholderObj, job_progress
+                    )
             except OSError as E:
-                common_globals.innerlog.get().debug(
-                    f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] Number of open Files across all processes-> {len(system.getOpenFiles(unique=False))}"
-                )
-                common_globals.innerlog.get().debug(
-                    f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] Number of unique open files across all processes-> {len(system.getOpenFiles())}"
+                await asyncio.sleep(1)
+                common_globals.log.debug(
+                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] Number of Open Files -> { len(psutil.Process().open_files())}"
                 )
-                common_globals.innerlog.get().debug(
-                    f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] Unique files data across all process -> {list(map(lambda x:(x.path,x.fd),(system.getOpenFiles())))}"
+                common_globals.log.debug(
+                    f" {get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] Open Files -> {list(map(lambda x:(x.path,x.fd),psutil.Process().open_files()))}"
                 )
                 raise E
             except Exception as E:
-                common_globals.innerlog.get().traceback_(
-                    f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] {traceback.format_exc()}"
+                await asyncio.sleep(1)
+                common_globals.log.traceback_(
+                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] {traceback.format_exc()}"
                 )
-                common_globals.innerlog.get().traceback_(
-                    f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] {E}"
+                common_globals.log.traceback_(
+                    f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] {E}"
                 )
                 raise E
 
 
-async def alt_data_handler(c, ele, tempholderObj):
+async def main_data_handler(data, item, c, ele, placeholderObj, job_progress):
+    item["total"] = int(data.get("content-length"))
+    resume_size = get_resume_size(placeholderObj, mediatype=ele.mediatype)
+    if await check_forced_skip(ele, item["total"]):
+        item["total"] = 0
+        return item
+    elif item["total"] == resume_size:
+        temp_file_logger(placeholderObj, ele)
+        return item
+    elif item["total"] != resume_size:
+        return await alt_download_sendreq(item, c, ele, placeholderObj, job_progress)
+
+
+async def alt_data_handler(item, c, ele, placeholderObj, job_progress):
     result = None
     try:
-        result = await main_download_sendreq(
-            c, ele, tempholderObj, placeholderObj=None, total=None
-        )
+        result = await alt_download_sendreq(item, c, ele, placeholderObj, job_progress)
     except Exception as E:
         raise E
     return result
 
 
-async def main_data_handler(data, c, ele, tempholderObj):
-    content_type = data.get("content-type").split("/")[-1]
-    total = int(data.get("content-length"))
-    placeholderObj = await placeholder.Placeholders(ele, content_type).init()
-    resume_size = get_resume_size(tempholderObj, mediatype=ele.mediatype)
-    # other
-    if await check_forced_skip(ele, total) == 0:
-        path_to_file_logger(placeholderObj, ele, common_globals.innerlog.get())
-        return [0]
-    elif total == resume_size:
-        path_to_file_logger(placeholderObj, ele, common_globals.innerlog.get())
-        return (
-            total,
-            tempholderObj.tempfilepath,
-            placeholderObj,
-        )
-
-    else:
-        try:
-            return await main_download_sendreq(
-                c, ele, tempholderObj, total=total, placeholderObj=placeholderObj
-            )
-        except Exception as E:
-            raise E
-
-
-async def main_download_sendreq(c, ele, tempholderObj, placeholderObj=None, total=None):
+async def alt_download_sendreq(item, c, ele, placeholderObj, job_progress):
     try:
-        common_globals.innerlog.get().debug(
-            f"{get_medialog(ele)} [attempt {common_globals.attempt.get()}/{constants.getattr('DOWNLOAD_RETRIES')}] download temp path {tempholderObj.tempfilepath}"
+        _attempt = common.alt_attempt_get(item)
+        item["total"] = item["total"] if _attempt == 1 else None
+        base_url = re.sub("[0-9a-z]*\.mpd$", "", ele.mpd, re.IGNORECASE)
+        url = f"{base_url}{item['origname']}"
+        common_globals.log.debug(
+            f"{get_medialog(ele)} Attempting to download media {item['origname']} with {url}"
         )
-        total = total if common_globals.attempt.get() == 1 else None
-        return await send_req_inner(
-            c, ele, tempholderObj, placeholderObj=placeholderObj, total=total
+        common_globals.log.debug(
+            f"{get_medialog(ele)} [attempt {_attempt.get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] download temp path {placeholderObj.tempfilepath}"
         )
+        return await send_req_inner(c, ele, item, placeholderObj, job_progress)
     except OSError as E:
         raise E
     except Exception as E:
         raise E
 
 
-async def send_req_inner(c, ele, tempholderObj, placeholderObj=None, total=None):
-    old_total = total
+async def send_req_inner(c, ele, item, placeholderObj, job_progress):
+    old_total = item["total"]
+    total = old_total
     try:
-        await common.batch_total_change_helper(None, total)
-        resume_size = get_resume_size(tempholderObj, mediatype=ele.mediatype)
+        await common.total_change_helper(None, total)
+        resume_size = get_resume_size(placeholderObj, mediatype=ele.mediatype)
         headers = (
             None
-            if resume_size == 0 or not old_total
+            if resume_size == 0 or not total
             else {"Range": f"bytes={resume_size}-{total}"}
         )
-        async with sem_wrapper(common_globals.req_sem):
-            async with c.requests(url=ele.url, headers=headers)() as r:
-                if r.ok:
-                    await asyncio.get_event_loop().run_in_executor(
-                        common_globals.cache_thread,
-                        partial(
-                            cache.set,
-                            f"{ele.id}_headers",
-                            {
-                                "content-length": r.headers.get("content-length"),
-                                "content-type": r.headers.get("content-type"),
-                            },
-                        ),
-                    )
-                    new_total = int(r.headers["content-length"])
-                    content_type = r.headers.get("content-type").split("/")[
-                        -1
-                    ] or get_unknown_content_type(ele)
-                    if not placeholderObj:
-                        placeholderObj = await placeholder.Placeholders(
-                            ele, content_type
-                        ).init()
-                    path_to_file_logger(
-                        placeholderObj, ele, common_globals.innerlog.get()
-                    )
-                    if await check_forced_skip(ele, new_total) == 0:
-                        total = 0
-                        await common.batch_total_change_helper(old_total, total)
-                        return (total, tempholderObj.tempfilepath, placeholderObj)
-                    elif total == resume_size:
-                        None
-                    else:
-                        total = new_total
-                        await common.batch_total_change_helper(old_total, total)
-                        await download_fileobject_writer(
-                            r, ele, total, tempholderObj, placeholderObj
-                        )
-                else:
-                    common_globals.innerlog.get().debug(
-                        f"[bold] {get_medialog(ele)} main download response status code [/bold]: {r.status}"
-                    )
-                    common_globals.innerlog.get().debug(
-                        f"[bold] {get_medialog(ele)} main download  response text [/bold]: {await r.text_()}"
-                    )
-                    common_globals.innerlog.get().debug(
-                        f"[bold] {get_medialog(ele)}main download headers [/bold]: {r.headers}"
-                    )
-                    r.raise_for_status()
+        params = {
+            "Policy": ele.policy,
+            "Key-Pair-Id": ele.keypair,
+            "Signature": ele.signature,
+        }
+        base_url = re.sub("[0-9a-z]*\.mpd$", "", ele.mpd, re.IGNORECASE)
+        url = f"{base_url}{item['origname']}"
 
-        await size_checker(tempholderObj.tempfilepath, ele, total)
-        return (total, tempholderObj.tempfilepath, placeholderObj)
+        common_globals.log.debug(
+            f"{get_medialog(ele)} [attempt {common.alt_attempt_get(item).get()}/{constants.getattr('DOWNLOAD_FILE_NUM_TRIES')}] Downloading media with url {url}"
+        )
+        async with c.requests_async(url=url, headers=headers, params=params) as l:
+            await asyncio.get_event_loop().run_in_executor(
+                common_globals.cache_thread,
+                partial(
+                    cache.set,
+                    f"{item['name']}_headers",
+                    {
+                        "content-length": l.headers.get("content-length"),
+                        "content-type": l.headers.get("content-type"),
+                    },
+                ),
+            )
+            new_total = int(l.headers["content-length"])
+            temp_file_logger(placeholderObj, ele)
+            if await check_forced_skip(ele, new_total):
+                item["total"] = 0
+                await common.total_change_helper(None, old_total)
+            elif total != resume_size:
+                item["total"] = new_total
+                total = new_total
+                await common.total_change_helper(old_total, total)
+                await download_fileobject_writer(
+                    total, l, ele, job_progress, placeholderObj
+                )
+        await size_checker(placeholderObj.tempfilepath, ele, total)
+        return item
     except Exception as E:
-        await common.batch_total_change_helper(None, -(total or 0))
+        await common.total_change_helper(None, -(total or 0))
         raise E
 
 
-async def download_fileobject_writer(r, ele, total, tempholderObj, placeholderObj):
-    pathstr = str(placeholderObj.trunicated_filepath)
+async def download_fileobject_writer(total, l, ele, job_progress, placeholderObj):
+    pathstr = str(placeholderObj.tempfilepath)
+
     downloadprogress = settings.get_download_bars()
-    try:
-        count = 0
-        await common.send_msg(
-            {
-                "type": "add_task",
-                "args": (
-                    f"{(pathstr[:constants.getattr('PATH_STR_MAX')] + '....') if len(pathstr) > constants.getattr('PATH_STR_MAX') else pathstr}\n",
-                    ele.id,
-                ),
-                "total": total,
-                "visible": False,
-            }
-        )
 
-        fileobject = await aiofiles.open(tempholderObj.tempfilepath, "ab").__aenter__()
-        download_sleep = constants.getattr("DOWNLOAD_SLEEP")
+    task1 = job_progress.add_task(
+        f"{(pathstr[:constants.getattr('PATH_STR_MAX')] + '....') if len(pathstr) > constants.getattr('PATH_STR_MAX') else pathstr}\n",
+        total=total,
+        visible=True if downloadprogress else False,
+    )
+    count = 0
+    loop = asyncio.get_event_loop()
 
-        await common.send_msg({"type": "update", "args": (ele.id,), "visible": True})
-        async for chunk in r.iter_chunked(constants.getattr("maxChunkSizeB")):
-            count = count + 1
+    fileobject = await aiofiles.open(placeholderObj.tempfilepath, "ab").__aenter__()
+    download_sleep = constants.getattr("DOWNLOAD_SLEEP")
+    try:
+        async for chunk in l.iter_chunked(constants.getattr("maxChunkSize")):
             if downloadprogress:
                 count = count + 1
-            common_globals.innerlog.get().trace(
-                f"{get_medialog(ele)} Download Progress:{(pathlib.Path(tempholderObj.tempfilepath).absolute().stat().st_size)}/{total}"
+            common_globals.log.trace(
+                f"{get_medialog(ele)} Download Progress:{(pathlib.Path(placeholderObj.tempfilepath).absolute().stat().st_size)}/{total}"
             )
             await fileobject.write(chunk)
-            if count == constants.getattr("CHUNK_ITER"):
-                await common.send_msg(
-                    {
-                        "type": "update",
-                        "args": (ele.id,),
-                        "completed": (
-                            pathlib.Path(tempholderObj.tempfilepath)
-                            .absolute()
-                            .stat()
-                            .st_size
-                        ),
-                    }
+            if (count + 1) % constants.getattr("CHUNK_ITER") == 0:
+                await loop.run_in_executor(
+                    common_globals.thread,
+                    partial(
+                        job_progress.update,
+                        task1,
+                        completed=pathlib.Path(placeholderObj.tempfilepath)
+                        .absolute()
+                        .stat()
+                        .st_size,
+                    ),
                 )
-                count = 0
             (await asyncio.sleep(download_sleep)) if download_sleep else None
     except Exception as E:
-        # reset download data
         raise E
     finally:
+        # Close file if needed
         try:
-            await common.send_msg({"type": "remove_task", "args": (ele.id,)})
-        except:
+            await fileobject.close()
+        except Exception:
             None
 
         try:
-            await fileobject.close()
+            job_progress.remove_task(task1)
         except Exception:
             None
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/filters/models/date.py` & `ofscraper-3.9.1/ofscraper/filters/models/date.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/filters/models/flags.py` & `ofscraper-3.9.1/ofscraper/filters/models/flags.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/filters/models/other.py` & `ofscraper-3.9.1/ofscraper/filters/models/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/filters/models/price.py` & `ofscraper-3.9.1/ofscraper/filters/models/price.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/filters/models/sort.py` & `ofscraper-3.9.1/ofscraper/filters/models/sort.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/filters/models/subtype.py` & `ofscraper-3.9.1/ofscraper/filters/models/subtype.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/models/retriver.py` & `ofscraper-3.9.1/ofscraper/models/retriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,24 +29,26 @@
         else:
             return await get_via_list(count)
 
 
 async def get_via_list(count):
     out = []
     active_subscriptions = await subscriptions.get_subscriptions(count[0])
-    expired_subscriptions = await subscriptions.get_subscriptions(count[1], account="expired")
+    expired_subscriptions = await subscriptions.get_subscriptions(
+        count[1], account="expired"
+    )
     console.get_shared_console().print(
         "[yellow]Warning: Numbering on OF site can be iffy\nExample Including deactived accounts in expired\nSee: https://of-scraper.gitbook.io/of-scraper/faq#number-of-users-doesnt-match-account-number[/yellow]"
     )
 
-    other_subscriptions = lists.get_otherlist()
+    other_subscriptions = await lists.get_otherlist()
     out.extend(active_subscriptions)
     out.extend(expired_subscriptions)
     out.extend(other_subscriptions)
-    black_list = lists.get_blacklist()
+    black_list = await lists.get_blacklist()
     out = list(filter(lambda x: x.get("id") not in black_list, out))
     models_objects = list(map(lambda x: models.Model(x), out))
     return models_objects
 
 
 async def get_main_list(count):
     out = []
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/models/selector.py` & `ofscraper-3.9.1/ofscraper/models/selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import ofscraper.utils.constants as constants
 import ofscraper.utils.manager as manager
 import ofscraper.utils.settings as settings
 from ofscraper.utils.context.run_async import run
 
 ALL_SUBS = None
 PARSED_SUBS = None
-ALL_SUBS_DICT = None
+ALL_SUBS_DICT = {}
 log = logging.getLogger("shared")
 
 
 def get_model_fromParsed(name):
     global ALL_SUBS_DICT
     return ALL_SUBS_DICT.get(name)
 
@@ -81,14 +81,38 @@
         parsed_subscriptions_helper()
     else:
         all_subs_helper(refetch=False)
         parsed_subscriptions_helper()
     return PARSED_SUBS
 
 
+@run
+async def set_data_all_subs_dict(username):
+    args = read_args.retriveArgs()
+    oldusernames = args.usernames or set()
+    all_usernames = set()
+    all_usernames.update([username] if not isinstance(username, list) else username)
+    all_usernames.update(oldusernames)
+
+    seen = set()
+    new_names = [
+        username
+        for username in all_usernames
+        if username not in seen
+        and not seen.add(username)
+        and username not in oldusernames
+        and username != constants.getattr("DELETED_MODEL_PLACEHOLDER")
+    ]
+
+    args.usernames = new_names
+    write_args.setArgs(args)
+    await all_subs_helper() if len(new_names) > 0 else None
+    args.usernames = set(all_usernames)
+    write_args.setArgs(args)
+
 
 @run
 async def all_subs_helper(refetch=True, main=False, check=True):
     global ALL_SUBS
     if bool(ALL_SUBS) and not refetch:
         return
     while True:
@@ -156,14 +180,17 @@
             old_list = old_args.user_list
             args = prompts.modify_list_prompt(old_args)
             if not list(sorted(old_blacklist)) == list(
                 sorted(args.black_list)
             ) or not list(sorted(old_list)) == list(sorted(args.user_list)):
                 print("Updating Models")
                 all_subs_helper(check=False)
+        elif choice == "select":
+            old_args = read_args.retriveArgs()
+            args = prompts.modify_list_prompt(old_args)
         write_args.setArgs(args)
 
 
 def filterNSort():
     global ALL_SUBS
     while True:
         # paid/free
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/helpers/model_helpers.py` & `ofscraper-3.9.1/ofscraper/prompts/helpers/model_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/helpers/prompt_helpers.py` & `ofscraper-3.9.1/ofscraper/prompts/helpers/prompt_helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import inspect
 import re
 
+import pynumparser
+from InquirerPy.base import Choice
 from prompt_toolkit.shortcuts import prompt as prompt
 from rich.console import Console
 
+import ofscraper.filters.models.sort as sort
 import ofscraper.models.selector as userselector
 import ofscraper.prompts.helpers.model_helpers as modelHelpers
 import ofscraper.prompts.prompt_strings as prompt_strings
+import ofscraper.prompts.promptConvert as promptConvert
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.config.data as config_data
 import ofscraper.utils.context.stdout as stdout
 import ofscraper.utils.settings as settings
 
 console = Console()
 
@@ -111,21 +115,15 @@
     prompt("")
     return prompt_
 
 
 def model_funct(prompt):
     userselector.setfilter()
     with stdout.nostdout():
-        models = userselector.filterOnly()
-        choices = list(
-            map(
-                lambda x: modelHelpers.model_selectorHelper(x[0], x[1]),
-                enumerate(models),
-            )
-        )
+        choices = _get_choices()
         selectedSet = set(
             map(
                 lambda x: re.search("^[0-9]+: ([^ ]+)", x["name"]).group(1),
                 prompt.selected_choices or [],
             )
         )
         for model in choices:
@@ -136,14 +134,81 @@
         prompt.content_control.choices = prompt.content_control._get_choices(
             prompt.content_control._raw_choices, prompt.content_control._default
         )
         prompt.content_control._format_choices()
         return prompt
 
 
+def model_select_funct(prompt):
+    with stdout.nostdout():
+        try:
+            toggle = promptConvert.getChecklistSelection(
+                choices=[
+                    Choice(True, "Range Select"),
+                    Choice(False, "Range Deselect"),
+                ]
+            )
+
+            # select new
+            choices = _select_helper(prompt, toggle)
+            prompt.content_control._raw_choices = choices
+            prompt.content_control.choices = prompt.content_control._get_choices(
+                prompt.content_control._raw_choices, prompt.content_control._default
+            )
+            prompt.content_control._format_choices()
+            return prompt
+        except Exception as E:
+            raise E
+
+
+def _select_helper(prompt, toggle=True):
+    try:
+        choices = _get_choices()
+        selectedSet = set(
+            map(
+                lambda x: re.search("^[0-9]+: ([^ ]+)", x["name"]).group(1),
+                prompt.selected_choices or [],
+            )
+        )
+
+        changes = set(
+            pynumparser.NumberSequence().parse(
+                promptConvert.multiline_input_prompt(
+                    message="Enter Num Sequences: ",
+                    more_instruction="Example Input: '1-2,20-50 => [1,2,20...50] inclusive' ",
+                )
+            )
+        )
+        if toggle:
+            for count, model in enumerate(choices):
+                name = re.search("^[0-9]+: ([^ ]+)", model.name).group(1)
+                if name in selectedSet or count + 1 in changes:
+                    model.enabled = True
+        elif not toggle:
+            for count, model in enumerate(choices):
+                name = re.search("^[0-9]+: ([^ ]+)", model.name).group(1)
+                if name in selectedSet and count + 1 not in changes:
+                    model.enabled = True
+
+    except Exception as E:
+        raise E
+    return choices
+
+
+def _get_choices():
+    models = userselector.filterOnly()
+    models = sort.sort_models_helper(models)
+    return list(
+        map(
+            lambda x: modelHelpers.model_selectorHelper(x[0], x[1]),
+            enumerate(models),
+        )
+    )
+
+
 def user_list(model_str):
     model_list = re.split("(,|\n)", model_str)
     model_list = map(lambda x: re.sub("[^a-zA-Z0-9 ]", "", x), model_list)
     model_list = filter(lambda x: len(x) != 0, model_list)
     return model_list
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/keybindings.py` & `ofscraper-3.9.1/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/promptConvert.py` & `ofscraper-3.9.1/ofscraper/prompts/promptConvert.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,65 +35,79 @@
             )
         )
         kwargs["message"] = f"{kwargs.get('message')}" if kwargs.get("message") else ""
 
         altv_action = kwargs.pop("altv", None) or long_message
         altx_action = kwargs.pop("altx", None)
         altd_action = kwargs.pop("altd", None)
-        action_set = set()
+        additional_keys = kwargs.pop("additional_keys", {})
+        action = [None]
         prompt_ = funct(*args, **kwargs)
 
-        register_keys(prompt_, altx_action, altd_action, action_set)
+        register_keys(prompt_, altx_action, altd_action, additional_keys, action)
 
         while True:
             out = prompt_.execute()
             prompt_._default = get_default(funct, prompt_)
-            if "altx" in action_set:
+            select = action[0]
+            action[0] = None
+            if select == "altx":
                 prompt_ = altx_action(prompt_)
-            elif "altv" in action_set:
+            elif select == "altv":
                 altv_action()
-            elif "alt-d" in action_set:
+            elif select == "altd":
                 altd_action(prompt_)
+            elif additional_keys.get(select):
+                prompt_ = additional_keys.get(select)(prompt_)
             else:
                 break
-            action_set.clear()
 
         return out
 
     return inner
 
 
-def register_keys(prompt_, altx_action, altd_action, action_set):
+def register_keys(prompt_, altx_action, altd_action, additional_keys, action):
+    for key in (additional_keys).keys():
+        extra_key_helper(prompt_, key, action)
+
     if altx_action:
 
         @prompt_.register_kb("alt-x")
         def _handle_alt_x(event):
-            action_set.add("altx")
+            action[0] = "altx"
             event.app.exit()
 
         @prompt_.register_kb("c-b")
         def _handle_alt_x(event):
-            action_set.add("altx")
+            action[0] = "altx"
             event.app.exit()
 
     if altd_action:
 
         @prompt_.register_kb("alt-d")
         def _handle_altd(event):
-            action_set.add("alt-d")
+            action[0] = "altd"
             event.app.exit()
 
     @prompt_.register_kb("alt-v")
     def _handle_alt_v(event):
-        action_set.add("altv")
+        action[0] = "altv"
         event.app.exit()
 
     @prompt_.register_kb("c-v")
     def _handle_alt_v(event):
-        action_set.add("altv")
+        action[0] = "altv"
+        event.app.exit()
+
+
+def extra_key_helper(prompt_, key, action):
+    @prompt_.register_kb(key.lower())
+    def _handle_alt(event):
+        action[0] = key
         event.app.exit()
 
 
 def get_default(funct, prompt):
     if funct.__name__ in {"getChecklistSelection", "getFuzzySelection", "checkbox"}:
         return prompt.selected_choices
     elif funct.__name__ in {"number_type"}:
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/actions.py` & `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/area.py` & `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/area.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 def scrape_paid_prompt():
     name = "value"
     answer = promptClasses.batchConverter(
         *[
             {
                 "type": "list",
                 "name": name,
-                "message": "Scrape entire paid page\n\n[Warning: initial Scan can be slow]\n[Caution: You should not need this unless your're looking to scrape paid content from a deleted/banned model]",
+                "message": "Scrape entire paid page\n\n[Warning: initial Scan can be slow]\n[Caution: You should not need this unless you are looking to scrape paid content from a deleted/banned model]",
                 "choices": [Choice(True, "True"), Choice(False, "False", enabled=True)],
                 "long_instruction": prompt_strings.SCRAPE_PAID,
                 "default": False,
             },
         ]
     )
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/auth.py` & `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/binary.py` & `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/binary.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/config.py` & `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     [CDM Options]
     private-key: for manual cdm
     client-id: for manual cdm
     key-mode-default: which cdm
     keydb_api: for keydb cdm
     -----------------------------------
     [Performance Options]
-    download-sems: number of downloads per processor/worker
+    download-sem: number of downloads per processor/worker
     threads: number of processors/workers
     -----------------------------------
     [Advanced Options]
     code-execution: allow eval on custom_val
     dynamic-mode-default: source of signed header values
     backend: which downloader to utilize
     downloadbars: toggle for download-bars
@@ -387,26 +387,26 @@
     )
 
     out.update(threads)
     max_allowed = cache.get("speed_download")
     if not cache.get("speed_download") or promptClasses.getChecklistSelection(
         choices=[Choice(True, "Yes"), Choice(False, "No")],
         message="Re-run speedtest",
-        more_instruction="Download Sems max value is based on calculated speed",
+        more_instruction="Download sem max value is based on calculated speed",
         default=False,
     ):
         speed = get_speed(threads)
         max_allowed = speed
         cache.set("speed_download", speed)
         cache.close()
     answer = promptClasses.batchConverter(
         *[
             {
                 "type": "number",
-                "name": "download-sems",
+                "name": "download-sem",
                 "message": "Number of semaphores per thread: ",
                 "min_allowed": 1,
                 "max_allowed": max_allowed,
                 "validate": EmptyInputValidator(),
                 "option_instruction": f"Value can be 1-{max_allowed}",
                 "default": data.get_download_semaphores(),
             }
@@ -462,15 +462,15 @@
     new_settings = promptClasses.batchConverter(
         *[
             {
                 "type": "list",
                 "name": "dynamic-mode-default",
                 "message": "What would you like to use for dynamic rules",
                 "default": data.get_dynamic(),
-                "choices": ["deviint", "digitalcriminals"],
+                "choices": ["deviint", "digitalcriminals", "sneaky"],
             },
             {
                 "type": "list",
                 "name": "cache-mode",
                 "message": "sqlite should be fine unless your using a network drive\nSee https://grantjenks.com/docs/diskcache/tutorial.html#caveats ",
                 "default": data.cache_mode_helper(),
                 "choices": ["sqlite", "json", "disabled"],
@@ -482,14 +482,15 @@
                 "message": "Select Which Backend you want:\n",
                 "default": data.get_backend() or "",
             },
             # value because of legacy config values
             {
                 "type": "input",
                 "name": "custom",
+                "multiline": True,
                 "message": "edit custom value:\n",
                 "option_instruction": "This is a helper value for remapping placeholder values",
                 "default": (
                     json.dumps(custom.get_custom())
                     if not isinstance(custom.get_custom(), str)
                     else custom.get_custom() or ""
                 ),
@@ -506,17 +507,24 @@
                 "name": "code-execution",
                 "message": "Enable Code Execution:",
                 "choices": [Choice(True, "Yes"), Choice(False, "No", enabled=True)],
                 "default": data.get_allow_code_execution(),
                 "option_instruction": "Allows for use of eval to evaluate custom values in placeholders",
             },
             {
+                "type": "input",
+                "name": "post_download_script",
+                "message": "Script to run after model download",
+                "default": data.get_post_download_script() or "",
+                "option_instruction": "Leave empty to skip post download script",
+            },
+            {
                 "type": "filepath",
                 "name": "temp_dir",
-                "message": "Location to store temp file",
+                "message": "Location to store temp files",
                 "default": data.get_TempDir() or "",
                 "option_instruction": "Leave empty to use default location",
             },
             {
                 "type": "list",
                 "name": "appendlog",
                 "message": "append logs into daily log files",
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/menu.py` & `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/model.py` & `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         transformer=lambda result: ",".join(map(lambda x: x.split(" ")[1], result)),
         multiselect=True,
         more_instruction=prompt_strings.MODEL_SELECT,
         long_message=prompt_strings.MODEL_FUZZY,
         altx=prompt_helpers.model_funct,
         altd=prompt_helpers.model_details,
         validate=prompt_validators.emptyListValidator(),
+        additional_keys={"Alt-B": prompt_helpers.model_select_funct},
         prompt="Filter: ",
         message="Which models do you want to scrape\n:",
         info=True,
     )
 
     return p
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_groups/profile.py` & `ofscraper-3.9.1/ofscraper/prompts/prompt_groups/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_strings.py` & `ofscraper-3.9.1/ofscraper/prompts/prompt_strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,16 +183,16 @@
 """
 
 NUMBER = """
 SHOW INSTRUCTIONS: [ALT+V] or [CTRL+V]
 """
 
 MODEL_SELECT = """
-CHANGE SORT/CHANGE FILTER: [ALT+X] or [CTRL+B]
-MODEL DETAILS: [ALT+D]
+CHANGE SORT/FILTER: [ALT+X] or [CTRL+B]
+MODEL DETAILS: [ALT+D] ||| RANGE SELECT: [ALT+B] 
 """
 PRICE_DETAILS = """
 SHOW CURRENT PRICE STATUS/INFO: [ALT+D]
 """
 FILTER_DETAILS = """
 SHOW CURRENT FILTERS/SORTING: [ALT+D]
 """
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/prompt_validators.py` & `ofscraper-3.9.1/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/prompts/prompts.py` & `ofscraper-3.9.1/ofscraper/prompts/prompts.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,7 +15,8 @@
 from ofscraper.prompts.prompt_groups.area import *
 from ofscraper.prompts.prompt_groups.auth import *
 from ofscraper.prompts.prompt_groups.binary import *
 from ofscraper.prompts.prompt_groups.config import *
 from ofscraper.prompts.prompt_groups.menu import *
 from ofscraper.prompts.prompt_groups.model import *
 from ofscraper.prompts.prompt_groups.profile import *
+from ofscraper.prompts.prompt_groups.merge import *
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/runner/exit.py` & `ofscraper-3.9.1/ofscraper/runner/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/runner/load.py` & `ofscraper-3.9.1/ofscraper/runner/load.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/runner/run.py` & `ofscraper-3.9.1/ofscraper/runner/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/actions.py` & `ofscraper-3.9.1/ofscraper/utils/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/args/areas.py` & `ofscraper-3.9.1/ofscraper/utils/args/areas.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/common_args.py` & `ofscraper-3.9.1/ofscraper/utils/args/groups/common_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ofscraper.const.constants import KEY_OPTIONS
 
 
 def common_params(func):
 
     @click.option_group(
         "Program Options",
-        click.version_option(version=__version__),
+        click.version_option(__version__, "-v", "--version", package_name="OF-Scraper"),
         click.option(
             "-cg",
             "--config",
             help="Change location of config folder/file",
             default=None,
         ),
         click.option(
@@ -89,15 +89,15 @@
             type=click.Choice(KEY_OPTIONS),
         ),
         click.option(
             "-dr",
             "--dynamic-rules",
             help="Dynamic signing",
             default=None,
-            type=click.Choice(["dc", "deviint"], case_sensitive=False),
+            type=click.Choice(["dc", "deviint", "sneaky"], case_sensitive=False),
             callback=lambda ctx, param, value: value.lower() if value else None,
         ),
         click.option(
             "-ar",
             "--no-auto-resume",
             help="Cleanup temp .part files (removes resume ability)",
             default=False,
@@ -108,15 +108,15 @@
             "--downloadbars",
             help="Show individual download progress bars",
             default=False,
             is_flag=True,
         ),
         click.option(
             "-sd",
-            "--downloadsems",
+            "--downloadsem",
             help="Number of concurrent downloads per thread",
             default=None,
             type=int,
         ),
         click.option(
             "-dp",
             "--downloadthreads",
@@ -135,37 +135,47 @@
             "-md",
             "--metadata",
             "metadata",
             help="""
             \b
             Skip media downloads and gather metadata only 
             [no change to download status] 
-            [select onw one --metadata or --metadata-update or --metadata-complete]""",
+            [select one --metadata or --metadata-update or --metadata-complete]""",
             flag_value="none",  # Enforce "none" as the only valid value
         ),
         click.option(
             "-mu",
             "--metadata-update",
             "metadata",
             help="""
             \b
             Skip media downloads, gather metadata, and update download status based on file presence 
-            [select onw one --metadata or --metadata-update or --metadata-complete]""",
+            [select one --metadata or --metadata-update or --metadata-complete]""",
             flag_value="file",
         ),
         click.option(
             "-mc",
             "--metadata-complete",
             "metadata",
             help="""
             \b
             Skip media downloads, gather metadata, and mark all media as downloaded 
-            [select onw one --metadata or --metadata-update or --metadata-complete]""",
+            [select one --metadata or --metadata-update or --metadata-complete]""",
             flag_value="complete",
         ),
+        click.option(
+            "-ds",
+            "--download-script",
+            "download_script",
+            help="""
+            \b
+            runs a script post model download
+            addional args sent to script username, model_id, media json ,and post json
+            """,
+        ),
         help="Advanced control of program behavior",
     )
     @functools.wraps(func)
     @click.pass_context
     def wrapper(ctx, *args, **kwargs):
         return func(ctx, *args, **kwargs)
 
@@ -175,15 +185,15 @@
 def common_other_params(func):
     click.option_group(
         "Downloading options",
         click.option(
             "-g",
             "--original",
             help="Don't truncate long paths",
-            is_flag=True,  
+            is_flag=True,
         ),
         click.option(
             "-q",
             "--quality",
             type=click.Choice(["240", "720", "source"], case_sensitive=False),
         ),
         click.option(
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/main_args.py` & `ofscraper-3.9.1/ofscraper/utils/args/groups/main_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,21 +119,27 @@
             ]
         ),
     ),
     click.constraints.mutually_exclusive(
         click.option(
             "-e",
             "--force-all",
+            "--dupe",
+            "--dupe-all",
+            "force_all",
             help="Download all files regardless of database presence",
             default=False,
             is_flag=True,
         ),
         click.option(
             "-eq",
             "--force-model-unique",
+            "--dupe-model-unique",
+            "--dupe-model",
+            "--force_model_unique",
             help="Only download files not present for the current model in the database",
             default=False,
             is_flag=True,
         ),
     ),
     click.constraints.mutually_exclusive(
         click.option(
@@ -146,100 +152,99 @@
         click.option(
             "-no",
             "--normal-only",
             help="Only download content that does not require decryption",
             default=False,
             is_flag=True,
         ),
-        click.option(
-            "-lb",
-            "--label",
-            help="Filter by label (use helpers.label_helper to process)",
-            default=[],
-            required=False,
-            type=helpers.label_helper,
-            callback=lambda ctx, param, value: (
-                list(set(itertools.chain.from_iterable(value))) if value else []
-            ),
-            multiple=True,
-        ),
-        click.option(
-            "-be",
-            "--before",
-            help="Process posts at or before the given date (MM/DD/YYYY) for likes, unlikes, and downloads",
-            type=helpers.arrow_helper,
-        ),
-        click.option(
-            "-af",
-            "--after",
-            help="Process posts at or after the given date (MM/DD/YYYY) for likes, unlikes, and downloads",
-            type=helpers.arrow_helper,
-        ),
-        click.option(
-            "-mt",
-            "--mediatype",
-            help="Filter by media type (Videos, Audios, Images)",
-            default=[],
-            required=False,
-            type=helpers.mediatype_helper,
-            callback=lambda ctx, param, value: (
-                list(set(itertools.chain.from_iterable(value))) if value else []
-            ),
-            multiple=True,
-        ),
-        click.option(
-            "-sx",
-            "--size-max",
-            help="Filter out files larger than the given size (bytes or human-readable, e.g., 10mb)",
-            required=False,
-            type=parse_size,
-        ),
-        click.option(
-            "-sm",
-            "--size-min",
-            help="Filter out files smaller than the given size (bytes or human-readable, e.g., 10mb)",
-            required=False,
-            type=parse_size,
-        ),
-        click.option(
-            "-mm/-ms",
-            "--mass-only/--mass-skip",
-            "mass_msg",
-            help="""
-            \b
-            Flag for enabling/disabling mass content or promos 
-            [select one --mass-only or --mass-skip]""",
-            default=None,
-            required=False,
+    ),
+    click.option(
+        "-lb",
+        "--label",
+        help="Filter by label (use helpers.label_helper to process)",
+        default=[],
+        required=False,
+        type=helpers.label_helper,
+        callback=lambda ctx, param, value: (
+            list(set(itertools.chain.from_iterable(value))) if value else []
         ),
-        click.option(
-            "-ok/-sk",
-            "--only-timed/--skip-timed",
-            "timed_only",
-            default=None,
-            help="""
-            \b
-            Flag for enabling/disabling promotional or temporary posts
-            [select one --only-timed or --skip-timed]""",
+        multiple=True,
+    ),
+    click.option(
+        "-be",
+        "--before",
+        help="Process posts at or before the given date (MM/DD/YYYY) for likes, unlikes, and downloads",
+        type=helpers.arrow_helper,
+    ),
+    click.option(
+        "-af",
+        "--after",
+        help="Process posts at or after the given date (MM/DD/YYYY) for likes, unlikes, and downloads",
+        type=helpers.arrow_helper,
+    ),
+    click.option(
+        "-mt",
+        "--mediatype",
+        help="Filter by media type (Videos, Audios, Images)",
+        default=[],
+        required=False,
+        type=helpers.mediatype_helper,
+        callback=lambda ctx, param, value: (
+            list(set(itertools.chain.from_iterable(value))) if value else []
         ),
+        multiple=True,
+    ),
+    click.option(
+        "-sx",
+        "--size-max",
+        help="Filter out files larger than the given size (bytes or human-readable, e.g., 10mb)",
+        required=False,
+        type=parse_size,
+    ),
+    click.option(
+        "-sm",
+        "--size-min",
+        help="Filter out files smaller than the given size (bytes or human-readable, e.g., 10mb)",
+        required=False,
+        type=parse_size,
+    ),
+    click.option(
+        "-mm/-ms",
+        "--mass-only/--mass-skip",
+        "mass_msg",
+        help="""
+        \b
+        Flag for enabling/disabling mass content or promos 
+        [select one --mass-only or --mass-skip]""",
+        default=None,
+        required=False,
+    ),
+    click.option(
+        "-ok/-sk",
+        "--only-timed/--skip-timed",
+        "timed_only",
+        default=None,
+        help="""
+        \b
+        Flag for enabling/disabling promotional or temporary posts
+        [select one --only-timed or --skip-timed]""",
     ),
     help="""
     \b
     Define what posts to target (areas, filters) and actions to perform (like, unlike, download)
     Filter by type, date, label, size, and media type""",
 )
 @click.option_group(
     "Automation Options",
     click.option(
         "-d",
         "--daemon",
         help="Run script in the background. Set value to minimum minutes between script runs. Overdue runs will run as soon as previous run finishes",
         type=float,
     ),
-
     click.option(
         "-a",
         "--action",
         help="""
     Select batch action(s) to perform [like,unlike,download].
     Accepts space or comma-separated list. Like and unlike cannot be combined.
     """,
@@ -248,15 +253,14 @@
         default=None,
         callback=lambda ctx, param, value: (
             list(set(itertools.chain.from_iterable(value))) if value else []
         ),
     ),
     help="Control automated actions (like/unlike/download) and background execution",
 )
-
 @click.option_group(
     "User Selection Options",
     click.option(
         "-u",
         "--usernames",
         "--username",
         help="Select which username to process (name,name2). Set to ALL for all users",
@@ -274,16 +278,15 @@
         type=helpers.username_helper,
         default=None,
         multiple=True,
         callback=lambda ctx, param, value: (
             list(set(itertools.chain.from_iterable(value))) if value else []
         ),
     ),
-
-        click.option(
+    click.option(
         "-ul",
         "--user-list",
         help="Filter by userlist. Note: the lists 'ofscraper.main', 'ofscraper.expired', and 'ofscraper.active' are reserved and should not be the name of any list you have on OF",
         default=None,
         multiple=True,
         callback=lambda ctx, param, value: list(
             set(
@@ -321,20 +324,16 @@
                     ]
                 )
                 if value
                 else []
             )
         ),
     ),
-
-help="""Specify users for scraping  with usernames, userlists, or blacklists"""
+    help="""Specify users for scraping  with usernames, userlists, or blacklists""",
 )
-
-
-
 @click.option_group(
     "User List Filter Options",
     click.option(
         "-cp",
         "--current-price",
         help="Filter accounts based on either the subscription price, lowest claimable promotional price, or regular price",
         default=None,
@@ -366,25 +365,25 @@
         help="Filter accounts based on either the lowest promotional price regardless of claimability, or regular price",
         default=None,
         required=False,
         type=click.Choice(["paid", "free"], case_sensitive=False),
         callback=lambda ctx, param, value: value.lower() if value else None,
     ),
     click.option(
-            "-lo/-ls",
-            "--last-seen-only/--last-seen-skip",
-            "last_seen",
-            help="""
+        "-lo/-ls",
+        "--last-seen-only/--last-seen-skip",
+        "last_seen",
+        help="""
             \b
             Flag for filtering accounts based on last seen being visible
             select one --free-trial-only or --free-trial-skip]""",
-            default=None,
-            required=False,
-            is_flag=True,
-        ),
+        default=None,
+        required=False,
+        is_flag=True,
+    ),
     click.option(
         "-fo/-fs",
         "--free-trial-only/--free-trial-skip",
         "free_trail",  # Positional argument for destination attribute
         help="""
         \b
         Flag for enabling/disabling accounts with free trial
@@ -394,27 +393,27 @@
         required=False,
         is_flag=True,
         default=None,
     ),
     click.option(
         "-po/-ps",
         "--promo-only/--promo-skip",
-        "promo", 
+        "promo",
         help="""
         \b
         Flag for enabling/disabling accounts with a claimable promo price
         [select one --promo-only or --promo-skip]""",
         default=None,
         required=False,
         is_flag=True,
     ),
     click.option(
         "-ao",
         "--all-promo-only/--all-promo-skip",
-        "all_promo",  
+        "all_promo",
         help="""
             \b
             Flag for enabling/disabling  accounts with any promo price
             [select one ppall-promo-only or --all-promo-skip]""",
         default=None,
         required=False,
         is_flag=True,
@@ -430,24 +429,22 @@
         required=False,
         is_flag=True,
     ),
     click.option(
         "-ro/-rf",
         "--renew-on/--renew-off",
         "renewal",
-        help=\
-        """
+        help="""
         \b
         Flag for enabling/disabling accounts set to renew renew flag on 
         [select one --renew-on or --renew-off]""",
         default=None,
         required=False,
         is_flag=True,
     ),
-
     help="Filter users with options like price (current/renewal/regular/promo), free trial, promo availability, alongside userlist filters (include/exclude)",
 )
 @click.option_group(
     "Advanced User List Filter Options",
     click.option(
         "-ppn",
         "--promo-price-min",
@@ -603,37 +600,36 @@
         is_flag=True,
         default=False,
     ),
     help="Define the order in which models are displayed and processed for actions like liking posts, downloading content, or data gathering",
 )
 @click.option_group(
     "Advanced Search & Processing Options",
+    click.option(
+        "-uf",
+        "--users-first",
+        help="Process all users first rather than one at a time (affects --action)",
+        default=False,
+        is_flag=True,  # Shorthand for action="store_true"
+    ),
+    click.constraints.mutually_exclusive(
         click.option(
-            "-uf",
-            "--users-first",
-            help="Process all users first rather than one at a time (affects --action)",
+            "-fi",
+            "--individual",
+            help="Search each username as a separate request when --username is provided",
             default=False,
-            is_flag=True,  # Shorthand for action="store_true"
+            is_flag=True,
         ),
-            click.constraints.mutually_exclusive(
-            click.option(
-                "-fi",
-                "--individual",
-                help="Search each username as a separate request when --username is provided",
-                default=False,
-                is_flag=True,
-            ),
-            click.option(
-                "-fl",
-                "--list",
-                help="Search entire enabled lists before filtering for usernames when --username is provided",
-                default=False,
-                is_flag=True,
-            ),
+        click.option(
+            "-fl",
+            "--list",
+            help="Search entire enabled lists before filtering for usernames when --username is provided",
+            default=False,
+            is_flag=True,
         ),
-        help="Choose how usernames are searched, and define the order in which users are processed for actions"
+    ),
+    help="Choose how usernames are searched, and define the order in which users are processed for actions",
 )
 @common.common_params
 @click.pass_context
 def program(ctx, *args, **kwargs):
     return ctx.params, ctx.info_name
-
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/manual_args.py` & `ofscraper-3.9.1/ofscraper/utils/args/groups/manual_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 
 import cloup as click
 
 import ofscraper.utils.args.groups.common_args as common
 import ofscraper.utils.args.helpers as helpers
 
 
-@click.command("manual",help= "Manually download media by providing a list of urls or IDs",short_help="Manually download media by providing a list of urls or IDs")
+@click.command(
+    "manual",
+    help="Manually download media by providing a list of urls or IDs",
+    short_help="Manually download media by providing a list of urls or IDs",
+)
 @click.constraints.require_one(
     click.option(
         "-u",
         "--url",
         help="A space or comma seperated list of urls to download",
         default=None,
         multiple=True,
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/message_args.py` & `ofscraper-3.9.1/ofscraper/utils/args/groups/message_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 
 import cloup as click
 
 import ofscraper.utils.args.groups.common_args as common
 import ofscraper.utils.args.helpers as helpers
 
 
-@click.command("msg_check", short_help="""\b
-               Produces a media table from messages with filterable entries and quick downloads""",help=
-               """
+@click.command(
+    "msg_check",
+    short_help="""\b
+               Produces a media table from messages with filterable entries and quick downloads""",
+    help="""
 The msg_check subcommand gathers information on media content from messages
 It presents this data in a table format with filtering options for focused searches 
 Allows unlocked media entries to be directly downloaded through the table
-""")
+""",
+)
 @click.constraints.require_one(
     click.option(
         "-u",
         "--url",
         help="Scan messages via space or comma seperated list of urls",
         default=None,
         multiple=True,
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/paid_args.py` & `ofscraper-3.9.1/ofscraper/utils/args/groups/paid_args.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 
 import cloup as click
 
 import ofscraper.utils.args.groups.common_args as common
 import ofscraper.utils.args.helpers as helpers
 
 
-@click.command("paid_check", short_help="""\b
-               Produces a media table from purchases with filterable entries and quick downloads""",help=
-               """
+@click.command(
+    "paid_check",
+    short_help="""\b
+               Produces a media table from purchases with filterable entries and quick downloads""",
+    help="""
 The paid_check subcommand gathers information on media content from purchases
 It presents this data in a table format with filtering options for focused searches 
 Allows unlocked media entries to be directly downloaded through the table
-""")
+""",
+)
 @click.constraints.require_one(
     click.option(
         "-u",
         "--usernames",
         "--username",
-        "usernames",
+        "check_usernames",
         help="Scan purchases via username(s)",
         default=None,
         multiple=True,
         type=helpers.check_strhelper,
         callback=lambda ctx, param, value: (
             list(set(itertools.chain.from_iterable(value))) if value else []
         ),
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/post_args.py` & `ofscraper-3.9.1/ofscraper/utils/args/groups/post_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 
 import cloup as click
 
 import ofscraper.utils.args.groups.common_args as common
 import ofscraper.utils.args.helpers as helpers
 
 
-@click.command("post_check",  short_help="""\b
+@click.command(
+    "post_check",
+    short_help="""\b
                Produces a media table from posts with filterable entries and quick downloads""",
-               help="""The post_check subcommand gathers information on media content from posts
+    help="""The post_check subcommand gathers information on media content from posts
 It presents this data in a table format with filtering options for focused searches 
-Allows unlocked media entries to be directly downloaded through the table""")
+Allows unlocked media entries to be directly downloaded through the table""",
+)
 @click.constraints.require_one(
     click.option(
         "-u",
         "--url",
         help="Scan posts via space or comma seperated list of urls",
         default=None,
         multiple=True,
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/args/groups/story_args.py` & `ofscraper-3.9.1/ofscraper/utils/args/groups/story_args.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 
 import cloup as click
 
 import ofscraper.utils.args.groups.common_args as common
 import ofscraper.utils.args.helpers as helpers
 
 
-@click.command("story_check", short_help="""\b
-               Produces a media table from stories and highlights with filterable entries and quick downloads""",help=
-               """
+@click.command(
+    "story_check",
+    short_help="""\b
+               Produces a media table from stories and highlights with filterable entries and quick downloads""",
+    help="""
 The story_check subcommand gathers information on media content from stories and highlights
 It presents this data in a table format with filtering options for focused searches 
 Allows unlocked media entries to be directly downloaded through the table
-""")
+""",
+)
 @click.constraints.require_one(
     click.option(
         "-u",
         "--usernames",
         "--username",
-        "usernames",
+        "check_usernames",
         help="Scan stories/highlights via username(s)",
         default=None,
         multiple=True,
         type=helpers.check_strhelper,
         callback=lambda ctx, param, value: (
             list(set(itertools.chain.from_iterable(value))) if value else []
         ),
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/args/helpers.py` & `ofscraper-3.9.1/ofscraper/utils/args/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/args/parse.py` & `ofscraper-3.9.1/ofscraper/utils/args/parse.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import re
+import sys
+
 import ofscraper.utils.args.groups.main_args as main
 import ofscraper.utils.args.groups.manual_args as manual
 import ofscraper.utils.args.groups.message_args as message
 import ofscraper.utils.args.groups.paid_args as paid
 import ofscraper.utils.args.groups.post_args as post
 import ofscraper.utils.args.groups.story_args as story
 import ofscraper.utils.args.write as write_args
@@ -34,17 +37,22 @@
     try:
         main.program.add_command(manual.manual, "manual")
         main.program.add_command(message.message_check, "msg_check")
         main.program.add_command(story.story_check, "story_check")
         main.program.add_command(paid.paid_check, "paid_check")
         main.program.add_command(post.post_check, "post_check")
 
-        result = main.program(standalone_mode=False)
+        filter_str = r"\b(multiprocessing|pipe_handle|fork|parent_pid)\b"
+        result = main.program(
+            standalone_mode=False,
+            prog_name="OF-Scraper",
+            args=[text for text in sys.argv if not re.search(filter_str, text)][1:],
+        )
         if result == 0:
-            quit()
+            sys.exit()
         args, command = result
         args["command"] = command
         d = AutoDotDict(args)
         write_args.setArgs(d)
         return d
     except SystemExit as e:
         if e.code != 0:
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/args/read.py` & `ofscraper-3.9.1/ofscraper/utils/args/read.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/args/user.py` & `ofscraper-3.9.1/ofscraper/utils/args/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.args.write as write_args
 
 
-
 def resetUserFilters():
     args = read_args.retriveArgs()
     args.user_list = []
     args.black_list = []
     args.renewal = None
     args.sub_status = None
     args.last_seen = None
@@ -19,11 +18,12 @@
     args.renewal_price = None
     args.current_price = None
     args.promo_price = None
     args.sort = "name"
     args.desc = False
     return args
 
+
 def set_users_arg(input_):
     args = read_args.retriveArgs()
-    args.usernames=input_
-    write_args.setArgs(args)
+    args.usernames = input_
+    write_args.setArgs(args)
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/auth/context.py` & `ofscraper-3.9.1/ofscraper/utils/auth/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/auth/data.py` & `ofscraper-3.9.1/ofscraper/utils/auth/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/auth/file.py` & `ofscraper-3.9.1/ofscraper/utils/auth/file.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 """
 import json
 
 from rich.console import Console
 
 import ofscraper.utils.auth.context as auth_context
 import ofscraper.utils.auth.make as make
-import ofscraper.utils.auth.request as request_auth
 import ofscraper.utils.auth.schema as auth_schema
 import ofscraper.utils.paths.common as common_paths
 
 console = Console()
 
 
 def read_auth():
@@ -30,15 +29,14 @@
         with auth_context.auth_context():
             old_auth = helpers.get_auth_dict()
             auth = auth_schema.auth_schema(old_auth)
             if auth_schema.auth_key_missing(old_auth):
                 auth = write_auth(auth)
             if auth_schema.auth_key_null(auth):
                 auth = make.make_auth(auth)
-            request_auth.make_request_auth()
             return auth
 
 
 def edit_auth():
     while True:
         with auth_context.auth_context():
             auth = helpers.get_auth_dict()
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/auth/make.py` & `ofscraper-3.9.1/ofscraper/utils/auth/make.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/auth/schema.py` & `ofscraper-3.9.1/ofscraper/utils/auth/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/binaries.py` & `ofscraper-3.9.1/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/cache.py` & `ofscraper-3.9.1/ofscraper/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/checkers.py` & `ofscraper-3.9.1/ofscraper/utils/checkers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/config/config.py` & `ofscraper-3.9.1/ofscraper/utils/config/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/config/data.py` & `ofscraper-3.9.1/ofscraper/utils/config/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,26 @@
         val
         if not any(x == val for x in [None, ""])
         else constants_attr.getattr("DEFAULT_USER_LIST")
     )
 
 
 @wrapper.config_reader
+def get_post_download_script(config=None):
+    if config is False:
+        return constants.POST_SCRIPT_DEFAULT
+    val = (
+        config.get("post_download_script")
+        if config.get("post_download_script") is not None
+        else config.get("advanced_options", {}).get("post_download_script")
+    )
+    return val if val is not None else constants_attr.getattr("POST_SCRIPT_DEFAULT")
+
+
+@wrapper.config_reader
 def get_default_blacklist(config=None):
     if config == False:
         return constants.DEFAULT_BLACK_LIST
     val = (
         config.get("default_black_list")
         if not any(x == config.get("default_black_list") for x in [None, ""])
         else config.get("advanced_options", {}).get("default_black_list")
@@ -494,15 +506,24 @@
         "advanced_options", {}
     ).get("dynamic-mode-default")
     return (
         value.lower()
         if value
         and value.lower()
         in set(
-            ["deviint", "digitalcriminals", "dv", "dev", "dc", "digital", "digitials"]
+            [
+                "deviint",
+                "digitalcriminals",
+                "dv",
+                "dev",
+                "dc",
+                "digital",
+                "digitials",
+                "sneaky",
+            ]
         )
         else "deviint"
     )
 
 
 @wrapper.config_reader
 def get_part_file_clean(config=None, mediatype=None):
@@ -530,24 +551,24 @@
     )
 
 
 @wrapper.config_reader
 def get_download_semaphores(config=None):
     if config == False:
         return constants.DOWNLOAD_SEM_DEFAULT
-    sems = (
-        config.get("download-sems")
-        or config.get("performance_options", {}).get("download-sems")
+    sem = (
+        config.get("download-sem")
+        or config.get("performance_options", {}).get("download-sem")
         or constants_attr.getattr("DOWNLOAD_SEM_DEFAULT")
     )
     try:
-        sems = int(sems)
+        sem = int(sem)
     except ValueError:
-        sems = int(constants_attr.getattr("DOWNLOAD_SEM_DEFAULT"))
-    return sems
+        sem = int(constants_attr.getattr("DOWNLOAD_SEM_DEFAULT"))
+    return sem
 
 
 @wrapper.config_reader
 def get_show_downloadprogress(config=None):
     if config == False:
         return constants.PROGRESS_DEFAULT
     val = (
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/config/file.py` & `ofscraper-3.9.1/ofscraper/utils/config/file.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import logging
 import pathlib
 import re
 
+import ofscraper.utils.config.context as config_context
 import ofscraper.utils.config.schema as schema
 import ofscraper.utils.console as console_
 import ofscraper.utils.paths.common as common_paths
 
 console = console_.get_shared_console()
 log = logging.getLogger("shared")
 
@@ -26,25 +27,24 @@
 
 
 def make_config_original():
     make_config(config=False)
 
 
 def open_config():
-    configText = config_string()
-    config = json_loads(configText)
-    if config.get("config"):
-        return config.get("config")
-    return config
+    with config_context.config_context():
+        configText = config_string()
+        config = json_loads(configText)
+        if config.get("config"):
+            return config.get("config")
+        return config
 
 
 def config_string():
     p = pathlib.Path(common_paths.get_config_path())
-    if not p.parent.is_dir():
-        p.parent.mkdir(parents=True, exist_ok=True)
     with open(p, "r") as f:
         configText = f.read()
     return configText
 
 
 def write_config(updated_config):
     if isinstance(updated_config, str):
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/config/menu.py` & `ofscraper-3.9.1/ofscraper/utils/config/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/config/schema.py` & `ofscraper-3.9.1/ofscraper/utils/config/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,29 +38,30 @@
         "cdm_options": {
             "private-key": data.get_private_key(config=config),
             "client-id": data.get_client_id(config=config),
             "key-mode-default": data.get_key_mode(config=config),
             "keydb_api": data.get_keydb_api(config=config),
         },
         "performance_options": {
-            "download-sems": data.get_download_semaphores(config=config),
+            "download-sem": data.get_download_semaphores(config=config),
             "threads": data.get_threads(config=config),
         },
         "advanced_options": {
             "code-execution": data.get_allow_code_execution(config=config),
             "dynamic-mode-default": data.get_dynamic(config=config),
             "backend": data.get_backend(config=config),
             "downloadbars": data.get_show_downloadprogress(config=config),
             "cache-mode": data.cache_mode_helper(config=config),
             "appendlog": data.get_appendlog(config=config),
             "custom_values": custom.get_custom(config=config),
             "sanitize_text": data.get_sanitizeDB(config=config),
             "temp_dir": data.get_TempDir(config=config),
             "remove_hash_match": data.get_hash(config=config),
             "infinite_loop_action_mode": data.get_InfiniteLoop(config=config),
+            "post_download_script": data.get_post_download_script(config=config),
             "disable_auto_after": data.get_disable_after(config=config),
             "default_user_list": data.get_default_userlist(config=config),
             "default_black_list": data.get_default_blacklist(config=config),
         },
         "responsetype": {
             "timeline": data.get_timeline_responsetype(config=config),
             "message": data.get_messages_progress_responsetype(config=config),
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/context/exit.py` & `ofscraper-3.9.1/ofscraper/utils/context/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/context/run_async.py` & `ofscraper-3.9.1/ofscraper/utils/context/run_async.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/context/stdout.py` & `ofscraper-3.9.1/ofscraper/utils/context/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/encoding.py` & `ofscraper-3.9.1/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/hash.py` & `ofscraper-3.9.1/ofscraper/utils/hash.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/logs/classes.py` & `ofscraper-3.9.1/ofscraper/utils/logs/classes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 import copy
 import logging
 import re
 
-from tenacity import (
-    Retrying,
-    retry,
-    retry_if_not_exception_type,
-    stop_after_attempt,
-    wait_fixed,
-)
-
-import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.config.data as data
 import ofscraper.utils.constants as constants
 import ofscraper.utils.dates as dates_manager
 import ofscraper.utils.logs.helpers as helpers
 
 
 class PipeHandler(logging.Handler):
@@ -115,84 +107,67 @@
             return False
         return True
 
 
 class DiscordHandler(logging.Handler):
     def __init__(self):
         logging.Handler.__init__(self)
-        self.sess = sessionbuilder.sessionBuilder(
+        self.sess = sessionManager.sessionManager(
             backend="httpx",
-            set_header=False,
-            set_cookies=False,
-            set_sign=False,
-            total_timeout=10,
+            total_timeout=constants.getattr("DISCORD_TOTAL_TIMEOUT"),
+            retries=constants.getattr("DISCORD_NUM_TRIES"),
+            wait_min=constants.getattr("DISCORD_MIN_WAIT"),
+            wait_max=constants.getattr("DISCORD_MAX_WAIT"),
         )
         self._thread = None
         self._baseurl = data.get_discord()
         self._url = self._baseurl
         self._appendhelper()
 
     def _appendhelper(self, date=None):
         if constants.getattr("DISCORD_THREAD_OVERRIDE"):
             with self.sess as sess:
-                for _ in Retrying(
-                    retry=retry_if_not_exception_type(KeyboardInterrupt),
-                    stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-                    wait=wait_fixed(8),
-                ):
-                    with _:
-                        try:
-                            with sess.requests(
-                                "{url}?wait=true".format(url=self._baseurl),
-                                "post",
-                                headers={"Content-type": "application/json"},
-                                json={
-                                    "thread_name": date
-                                    or dates_manager.getLogDate().get("now"),
-                                    "content": date
-                                    or dates_manager.getLogDate().get("now"),
-                                },
-                            )() as r:
-                                if r.status == 200:
-                                    resp_data = r.json()
-                                    self._url = "{url}?thread_id={id}".format(
-                                        url=self._baseurl, id=resp_data.get("id")
-                                    )
-                                else:
-                                    r.raise_for_status()
-                        except Exception as E:
-                            None
+                try:
+                    with sess.requests(
+                        "{url}?wait=true".format(url=self._baseurl),
+                        "post",
+                        headers={"Content-type": "application/json"},
+                        json={
+                            "thread_name": date
+                            or dates_manager.getLogDate().get("now"),
+                            "content": date or dates_manager.getLogDate().get("now"),
+                        },
+                    ) as _:
+                        pass
+                except Exception as E:
+                    None
 
     def emit(self, record):
         if isinstance(record, str):
             self._url = record
             return
 
         def inner(sess):
             with sess:
-                for _ in Retrying(
-                    retry=retry_if_not_exception_type(KeyboardInterrupt),
-                    stop=stop_after_attempt(constants.getattr("NUM_TRIES")),
-                    wait=wait_fixed(8),
-                ):
-                    with _:
-                        try:
-                            with sess.requests(
-                                self._url,
-                                "post",
-                                headers={"Content-type": "application/json"},
-                                json={
-                                    "content": log_entry,
-                                    "thread_name": self._thread,
-                                },
-                            )() as r:
-                                if not r.status == 204:
-                                    raise Exception
-                        except Exception:
-                            None
+                try:
+                    with sess.requests(
+                        self._url,
+                        "post",
+                        cookies=False,
+                        sign=False,
+                        headers={"Content-type": "application/json"},
+                        json={
+                            "content": log_entry,
+                            "thread_name": self._thread,
+                        },
+                    ) as r:
+                        if not r.status == 204:
+                            raise Exception
+                except Exception:
+                    None
 
         log_entry = self.format(record)
         url = data.get_discord()
         log_entry = re.sub("\[bold\]|\[/bold\]", "**", log_entry)
         log_entry = f"{log_entry}\n\n"
         if url == None or url == "":
             return
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/logs/close.py` & `ofscraper-3.9.1/ofscraper/utils/logs/close.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/logs/helpers.py` & `ofscraper-3.9.1/ofscraper/utils/logs/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 
+import ofscraper.utils.args.read as read_args
+
 senstiveDict = {}
 
 
 def logForLevel(level):
     def inner(self, message, *args, **kwargs):
         if self.isEnabledFor(level):
             self._log(level, message, args, **kwargs)
@@ -68,7 +70,12 @@
 
 
 def getNumber(input_):
     input_ = getLevel(input_)
     if isinstance(input_, str):
         return logging.getLevelName(input_)
     return input_
+
+
+def is_trace():
+    args = read_args.retriveArgs()
+    return args.discord == "TRACE" or args.logs == "TRACE" or args.output == "TRACE"
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/logs/logger.py` & `ofscraper-3.9.1/ofscraper/utils/logs/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/logs/logs.py` & `ofscraper-3.9.1/ofscraper/utils/logs/logs.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/logs/other.py` & `ofscraper-3.9.1/ofscraper/utils/logs/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/logs/stdout.py` & `ofscraper-3.9.1/ofscraper/utils/logs/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/manager.py` & `ofscraper-3.9.1/ofscraper/utils/manager.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import multiprocess
 import asyncio
-manager = None
-manager_dict = None
 
+import multiprocess
 
+manager = None
+manager_dict = None
 
 
 def get_manager():
     global manager
     if manager:
         return manager
     manager = multiprocess.Manager()
@@ -28,8 +28,8 @@
         manager.shutdown()
         manager == None
 
 
 def update_dict(new_dict):
     manager_dict = get_manager_process_dict()
     manager_dict.update(new_dict)
-    return manager_dict
+    return manager_dict
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/menu.py` & `ofscraper-3.9.1/ofscraper/utils/menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import ofscraper.prompts.prompts as prompts
 import ofscraper.utils.actions as actions
 import ofscraper.utils.auth.file as auth_file
 import ofscraper.utils.config.menu as config_menu
 import ofscraper.utils.profiles.manage as profiles_manage
 import ofscraper.utils.profiles.tools as profile_tools
 import ofscraper.utils.run as run
+import ofscraper.utils.merge as merge
 
 log = logging.getLogger("shared")
 count = 0
 
 
 def update_count():
     global count
@@ -64,14 +65,16 @@
                 result_profiles_prompt = prompts.profiles_prompt()
                 if result_profiles_prompt == "quit":
                     return True
                 elif result_profiles_prompt == "main":
                     break
                 else:
                     profile_menu_helper(result_profiles_prompt)
+        elif result_main_prompt == "merge":
+            merge.merge_runner()
         elif result_main_prompt == "quit":
             return True
 
 
 def profile_menu_helper(result_profiles_prompt):
     if result_profiles_prompt == "default":
         # Change profiles
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/paths/check.py` & `ofscraper-3.9.1/ofscraper/utils/paths/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/paths/common.py` & `ofscraper-3.9.1/ofscraper/utils/paths/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import pathlib
 
-import arrow
 
 import ofscraper.const.constants as constants
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.config.data as data
 import ofscraper.utils.config.file as config_file
 import ofscraper.utils.constants as constants_attr
 import ofscraper.utils.dates as dates_manager
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/paths/paths.py` & `ofscraper-3.9.1/ofscraper/utils/paths/paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,7 +153,14 @@
         )
     except PermissionError:
         None
 
 
 def speed_file():
     return pathlib.Path(common_paths.get_profile_path() / "speed.zip")
+
+
+def get_all_db(path):
+    for ele in filter(
+        lambda x: re.search("user_data.db", str(x)), pathlib.Path(path).glob("**/*")
+    ):
+        yield ele
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/profiles/data.py` & `ofscraper-3.9.1/ofscraper/utils/profiles/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/profiles/manage.py` & `ofscraper-3.9.1/ofscraper/utils/profiles/manage.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/profiles/tools.py` & `ofscraper-3.9.1/ofscraper/utils/profiles/tools.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/progress.py` & `ofscraper-3.9.1/ofscraper/utils/progress.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     overall_progress = Progress(
         SpinnerColumn(style=Style(color="blue")),
         TextColumn("{task.description}"),
     )
     progress_group = Group(overall_progress, Panel(Group(all_paid_progress)))
 
     return Live(
-        progress_group, refresh_per_second=5, console=console_.get_shared_console()
+        progress_group, refresh_per_second=5, console=console_.get_shared_console(),transient=True 
     )
 
 
 def setup_api_split_progress_live():
     global timeline_layout
     global pinned_layout
     global archived_layout
@@ -63,15 +63,15 @@
         paid_layout,
         stories_layout,
         highlights_layout,
         Layout(name="OF-Scaper", size=0, ratio=0),
     )
 
     progress_group = Group(overall_progress, layout)
-    return Live(progress_group, console=console_.get_shared_console())
+    return Live(progress_group, console=console_.get_shared_console(),transient=True )
 
 
 def setup_layout():
     global timeline_progress
     global pinned_progress
     global overall_progress
     global archived_progress
@@ -185,136 +185,135 @@
     overall_progress = Progress(
         SpinnerColumn(style=Style(color="blue")),
         TextColumn(f"Getting timeline posts...\n{{task.description}}"),
     )
     timeline_progress = Progress("{task.description}")
     progress_group = Group(overall_progress, Panel(Group(timeline_progress)))
     return Live(
-        progress_group, refresh_per_second=5, console=console_.get_shared_console()
+        progress_group, refresh_per_second=5, console=console_.get_shared_console() ,transient=True 
     )
 
 
 def set_up_api_pinned():
     global overall_progress
     global pinned_progress
     overall_progress = Progress(
         SpinnerColumn(style=Style(color="blue")),
         TextColumn(f"Getting pinned posts...\n{{task.description}}"),
     )
     pinned_progress = Progress("{task.description}")
     progress_group = Group(overall_progress, Panel(Group(pinned_progress)))
     return Live(
-        progress_group, refresh_per_second=5, console=console_.get_shared_console()
+        progress_group, refresh_per_second=5, console=console_.get_shared_console(),transient=True 
     )
 
 
 def set_up_api_paid():
     global overall_progress
     global paid_progress
     overall_progress = Progress(
         SpinnerColumn(style=Style(color="blue")),
         TextColumn(f"Getting paid posts...\n{{task.description}}"),
     )
     paid_progress = Progress("{task.description}")
     progress_group = Group(overall_progress, Panel(Group(paid_progress)))
     return Live(
-        progress_group, refresh_per_second=5, console=console_.get_shared_console()
+        progress_group, refresh_per_second=5, console=console_.get_shared_console(),transient=True 
     )
 
 
 def set_up_api_messages():
     global overall_progress
     global messages_progress
     overall_progress = Progress(
         SpinnerColumn(style=Style(color="blue")),
         TextColumn(f"Getting messages...\n{{task.description}}"),
     )
     messages_progress = Progress("{task.description}")
     progress_group = Group(overall_progress, Panel(Group(messages_progress)))
     return Live(
-        progress_group, refresh_per_second=5, console=console_.get_shared_console()
+        progress_group, refresh_per_second=5, console=console_.get_shared_console(),transient=True 
     )
 
 
 def set_up_api_archived():
     global overall_progress
     global archived_progress
     overall_progress = Progress(
         SpinnerColumn(style=Style(color="blue")),
         TextColumn(f"Getting archived...\n{{task.description}}"),
     )
     archived_progress = Progress("{task.description}")
     progress_group = Group(overall_progress, Panel(Group(archived_progress)))
     return Live(
-        progress_group, refresh_per_second=5, console=console_.get_shared_console()
+        progress_group, refresh_per_second=5, console=console_.get_shared_console(),transient=True 
     )
 
 
 def set_up_api_stories():
     global overall_progress
     global stories_progress
     overall_progress = Progress(
         SpinnerColumn(style=Style(color="blue")),
         TextColumn(f"Getting stories...\n{{task.description}}"),
     )
     stories_progress = Progress("{task.description}")
     progress_group = Group(overall_progress, Panel(Group(stories_progress)))
     return Live(
-        progress_group, refresh_per_second=5, console=console_.get_shared_console()
+        progress_group, refresh_per_second=5, console=console_.get_shared_console(),transient=True 
     )
 
 
 def set_up_api_highlights_lists():
     global overall_progress
     global highlights_progress
     overall_progress = Progress(
         SpinnerColumn(style=Style(color="blue")),
         TextColumn(f"Getting highlights lists...\n{{task.description}}"),
     )
     highlights_progress = Progress("{task.description}")
     progress_group = Group(overall_progress, Panel(Group(highlights_progress)))
     return Live(
-        progress_group, refresh_per_second=5, console=console_.get_shared_console()
+        progress_group, refresh_per_second=5, console=console_.get_shared_console(),transient=True 
     )
 
 
 def set_up_api_highlights():
     global overall_progress
     global highlights_progress
     overall_progress = Progress(
         SpinnerColumn(style=Style(color="blue")),
         TextColumn(f"Getting highlights via list..\n{{task.description}}"),
     )
     highlights_progress = Progress("{task.description}")
     progress_group = Group(overall_progress, Panel(Group(highlights_progress)))
     return Live(
-        progress_group, refresh_per_second=5, console=console_.get_shared_console()
+        progress_group, refresh_per_second=5, console=console_.get_shared_console(),transient=True 
     )
 
 
-
-
 def set_up_api_labels():
     global overall_progress
     global labelled_progress
     overall_progress = Progress(
         SpinnerColumn(style=Style(color="blue")),
         TextColumn(f"Getting Labels\n{{task.description}}"),
     )
     labelled_progress = Progress("{task.description}")
     progress_group = Group(overall_progress, Panel(Group(labelled_progress)))
     return Live(
-        progress_group, refresh_per_second=5, console=console_.get_shared_console()
+        progress_group, refresh_per_second=5, console=console_.get_shared_console(),transient=True 
     )
 
+
 def set_up_api_posts_labels():
     global overall_progress
     global labelled_progress
     overall_progress = Progress(
         SpinnerColumn(style=Style(color="blue")),
         TextColumn(f"Getting Posts via labels\n{{task.description}}"),
     )
     labelled_progress = Progress("{task.description}")
     progress_group = Group(overall_progress, Panel(Group(labelled_progress)))
     return Live(
-        progress_group, refresh_per_second=5, console=console_.get_shared_console()
+        progress_group, refresh_per_second=5, console=console_.get_shared_console(),transient=True 
     )
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/run.py` & `ofscraper-3.9.1/ofscraper/utils/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/separate.py` & `ofscraper-3.9.1/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/settings.py` & `ofscraper-3.9.1/ofscraper/utils/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,7 +140,14 @@
     )
 
 
 def get_after_enabled():
     return (
         read_args.retriveArgs().after is not None or not config_data.get_disable_after()
     )
+
+
+def get_post_download_script():
+    return (
+        read_args.retriveArgs().download_script
+        or config_data.get_post_download_script()
+    )
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/system/network.py` & `ofscraper-3.9.1/ofscraper/utils/system/network.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import logging
 import time
 import traceback
 
 import httpx
 
-import ofscraper.classes.sessionbuilder as sessionbuilder
-import ofscraper.utils.args.read as read_args
-import ofscraper.utils.config.data as data
+import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.console as console_
 import ofscraper.utils.constants as constants
 import ofscraper.utils.context.stdout as stdout
 import ofscraper.utils.settings as settings
 
 
 def check_cdm():
@@ -28,16 +26,22 @@
         elif keymode == "keydb":
             url = constants.getattr("KEYDB")
         elif keymode == "cdrm":
             url = constants.getattr("CDRM")
         elif keymode == "cdrm2":
             url = constants.getattr("CDRM2")
         try:
-            with sessionbuilder.sessionBuilder(backend="httpx", total_timeout=30) as c:
-                with c.requests(url=url)() as r:
+            with sessionManager.sessionManager(
+                backend="httpx",
+                total_timeout=constants.getattr("CDM_TEST_TIMEOUT"),
+                retries=constants.getattr("CDM_TEST_NUM_TRIES") ,
+                wait_min=constants.getattr("CDM_MIN_WAIT"),
+                wait_max=constants.getattr("CDM_MAX_WAIT"),
+            ) as c:
+                with c.requests(url=url) as r:
                     if r.ok:
                         console.print(
                             "[green] CDM service seems to be working\n[/green]"
                         )
                         console.print(
                             "[yellow]WARNING:Make sure you have all the correct settings for choosen cdm\nhttps://of-scraper.gitbook.io/of-scraper/cdm-options\n\n[/yellow]"
                         )
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/system/system.py` & `ofscraper-3.9.1/ofscraper/utils/system/system.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import asyncio
 import json
 import logging
-import multiprocessing
 import os
 import platform
 import subprocess
 import sys
 
+import multiprocess
 import psutil
 from setproctitle import setproctitle
 
 
 def is_frozen():
     if getattr(sys, "frozen", False) and hasattr(sys, "_MEIPASS"):
         return True
     else:
         return False
 
 
+def get_parent_process():
+    return multiprocess.parent_process() is None
+
+
 def get_parent():
-    return (
-        multiprocessing.parent_process() != None or "pytest" in sys.modules
-    ) == False
+    return get_parent_process() or "pytest" not in sys.modules
 
 
 def getcpu_count():
     if platform.system() != "Darwin":
         return len(psutil.Process().cpu_affinity())
     else:
         return psutil.cpu_count()
@@ -57,21 +59,21 @@
                 match.add(ele.fd)
     return out
 
 
 def set_mulitproc_start_type():
     plat = platform.system()
     if plat == "Darwin":
-        multiprocessing.set_start_method("spawn")
+        multiprocess.set_start_method("spawn")
         os.environ["OBJC_DISABLE_INITIALIZE_FORK_SAFETY"] = "YES"
         os.environ["no_proxy"] = "*"
     elif plat == "Windows":
-        multiprocessing.set_start_method("spawn")
+        multiprocess.set_start_method("spawn")
     else:
-        multiprocessing.set_start_method("forkserver")
+        multiprocess.set_start_method("forkserver")
 
 
 def set_eventloop():
     plat = platform.system()
     if plat == "Linux":
         import uvloop
```

### Comparing `ofscraper-3.9.0.dev9/ofscraper/utils/text.py` & `ofscraper-3.9.1/ofscraper/utils/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev9/pyproject.toml` & `ofscraper-3.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "3.9.0dev9"
+version = "3.9.1"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.14"
 
@@ -43,14 +43,15 @@
 speedtest-cli = "^2.1.3"
 prompt-toolkit = "^3.0.43"
 setproctitle = "^1.3.3"
 lxml = "^5.1.0"
 multiprocess = "^0.70.16"
 dill = "^0.3.8"
 cloup = "^3.0.5"
+pynumparser = "^1.4.1"
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 
 
 [tool.poetry.group.test]
```

### Comparing `ofscraper-3.9.0.dev9/PKG-INFO` & `ofscraper-3.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 3.9.0.dev9
+Version: 3.9.1
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -31,14 +31,15 @@
 Requires-Dist: mpegdash (>=0.4.0,<0.5.0)
 Requires-Dist: multiprocess (>=0.70.16,<0.71.0)
 Requires-Dist: pathvalidate (>=3.2.0,<4.0.0)
 Requires-Dist: poetry-dynamic-versioning (>=1.2.0,<2.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pycryptodome (>=3.20.0,<4.0.0)
+Requires-Dist: pynumparser (>=1.4.1,<2.0.0)
 Requires-Dist: pywidevine (>=1.8.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: schedule (>=1.2.1,<2.0.0)
 Requires-Dist: setproctitle (>=1.3.3,<2.0.0)
 Requires-Dist: setuptools (>=69.1.1,<70.0.0)
 Requires-Dist: speedtest-cli (>=2.1.3,<3.0.0)
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
-Metadata-Version: 2.1 Name: ofscraper Version: 3.9.0.dev9 Summary:
-automatically scrape onlyfans Author: datawhores Author-email:
-datawhores@riseup.net Requires-Python: >=3.11,<3.14 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Provides-Extra: pyinstaller
-Requires-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: aiohttp[speedups]
-(>=3.8.5,<4.0.0) Requires-Dist: aioprocessing (>=2.0.1,<3.0.0) Requires-Dist:
-aiosqlite (>=0.20.0,<0.21.0) Requires-Dist: arrow (>=1.3.0,<2.0.0) Requires-
-Dist: browser-cookie3 (==0.19.1) Requires-Dist: bs4 (>=0.0.2,<0.0.3) Requires-
-Dist: certifi (>=2024.2.2,<2025.0.0) Requires-Dist: cloup (>=3.0.5,<4.0.0)
-Requires-Dist: dill (>=0.3.8,<0.4.0) Requires-Dist: diskcache (>=5.6.3,<6.0.0)
-Requires-Dist: dunamai (>=1.19.2,<2.0.0) Requires-Dist: faust-cchardet
-(>=2.1.19,<3.0.0) Requires-Dist: filelock (>=3.13.1,<4.0.0) Requires-Dist:
-httpx[http2] (>=0.27.0,<0.28.0) Requires-Dist: humanfriendly (>=10.0,<11.0)
-Requires-Dist: inquirerpy (>=0.3.4,<0.4.0) Requires-Dist: lxml (>=5.1.0,<6.0.0)
-Requires-Dist: more-itertools (>=10.2.0,<11.0.0) Requires-Dist: mpegdash
-(>=0.4.0,<0.5.0) Requires-Dist: multiprocess (>=0.70.16,<0.71.0) Requires-Dist:
-pathvalidate (>=3.2.0,<4.0.0) Requires-Dist: poetry-dynamic-versioning
-(>=1.2.0,<2.0.0) Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0) Requires-Dist:
-psutil (>=5.9.8,<6.0.0) Requires-Dist: pycryptodome (>=3.20.0,<4.0.0) Requires-
-Dist: pywidevine (>=1.8.0,<2.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.7.1,<14.0.0) Requires-Dist: schedule (>=1.2.1,<2.0.0)
-Requires-Dist: setproctitle (>=1.3.3,<2.0.0) Requires-Dist: setuptools
-(>=69.1.1,<70.0.0) Requires-Dist: speedtest-cli (>=2.1.3,<3.0.0) Requires-Dist:
-tenacity (>=8.2.3,<9.0.0) Requires-Dist: textual (==0.52.1) Requires-Dist:
-uvloop (>=0.19.0,<0.20.0) ; sys_platform == "linux" or sys_platform == "linux2"
+Metadata-Version: 2.1 Name: ofscraper Version: 3.9.1 Summary: automatically
+scrape onlyfans Author: datawhores Author-email: datawhores@riseup.net
+Requires-Python: >=3.11,<3.14 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Provides-Extra: pyinstaller Requires-Dist: aiofiles
+(>=23.2.1,<24.0.0) Requires-Dist: aiohttp[speedups] (>=3.8.5,<4.0.0) Requires-
+Dist: aioprocessing (>=2.0.1,<3.0.0) Requires-Dist: aiosqlite
+(>=0.20.0,<0.21.0) Requires-Dist: arrow (>=1.3.0,<2.0.0) Requires-Dist:
+browser-cookie3 (==0.19.1) Requires-Dist: bs4 (>=0.0.2,<0.0.3) Requires-Dist:
+certifi (>=2024.2.2,<2025.0.0) Requires-Dist: cloup (>=3.0.5,<4.0.0) Requires-
+Dist: dill (>=0.3.8,<0.4.0) Requires-Dist: diskcache (>=5.6.3,<6.0.0) Requires-
+Dist: dunamai (>=1.19.2,<2.0.0) Requires-Dist: faust-cchardet (>=2.1.19,<3.0.0)
+Requires-Dist: filelock (>=3.13.1,<4.0.0) Requires-Dist: httpx[http2]
+(>=0.27.0,<0.28.0) Requires-Dist: humanfriendly (>=10.0,<11.0) Requires-Dist:
+inquirerpy (>=0.3.4,<0.4.0) Requires-Dist: lxml (>=5.1.0,<6.0.0) Requires-Dist:
+more-itertools (>=10.2.0,<11.0.0) Requires-Dist: mpegdash (>=0.4.0,<0.5.0)
+Requires-Dist: multiprocess (>=0.70.16,<0.71.0) Requires-Dist: pathvalidate
+(>=3.2.0,<4.0.0) Requires-Dist: poetry-dynamic-versioning (>=1.2.0,<2.0.0)
+Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0) Requires-Dist: psutil
+(>=5.9.8,<6.0.0) Requires-Dist: pycryptodome (>=3.20.0,<4.0.0) Requires-Dist:
+pynumparser (>=1.4.1,<2.0.0) Requires-Dist: pywidevine (>=1.8.0,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: rich
+(>=13.7.1,<14.0.0) Requires-Dist: schedule (>=1.2.1,<2.0.0) Requires-Dist:
+setproctitle (>=1.3.3,<2.0.0) Requires-Dist: setuptools (>=69.1.1,<70.0.0)
+Requires-Dist: speedtest-cli (>=2.1.3,<3.0.0) Requires-Dist: tenacity
+(>=8.2.3,<9.0.0) Requires-Dist: textual (==0.52.1) Requires-Dist: uvloop
+(>=0.19.0,<0.20.0) ; sys_platform == "linux" or sys_platform == "linux2"
 Requires-Dist: win32-setctime (>=1.1.0,<2.0.0) Requires-Dist: xxhash
 (>=3.4.1,<4.0.0) Project-URL: Homepage, https://github.com/datawhores/OF-
 Scraper Description-Content-Type: text/markdown # Releases [Releases Page]
 (https://pypi.org/project/ofscraper/#history) ``` Docker and binary releases
 also availible ``` ## Stable
 _[_d_r_a_w_i_n_g_]
 ## Dev
```

